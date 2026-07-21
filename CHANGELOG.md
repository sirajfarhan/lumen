# Changelog

## 0.2.62 — 2026-07-22

**Skills review their own messages**

- Each skill now ships a quality-judge reference: before a setup question or teaching turn reaches you, a fresh reviewer checks it against plain-communication criteria (does it name your actual thing, ask one question, ground the idea first), applies at most one fix per cycle, and records the review.
- The review is skipped for short single-turn tasks, so quick work stays fast.
- Reviews are recorded alongside each validation so message quality is auditable over time.

## 0.2.61 — 2026-07-22

**Skillsmith builds and repairs to a standard**

- Every skill Skillsmith designs now follows one plain-communication standard: it names the user's actual thing, uses ordinary words, grounds a question before asking it, asks one thing at a time, and reports progress in the user's own terms.
- Skillsmith places each skill in the system — declaring what it consumes, what it produces, and when another skill should run first — and prefers a single skill unless a pre-step clearly earns its cost.
- Skillsmith can now repair an existing skill's cryptic user-facing messages, one fix at a time, while preserving what each message asks for.

## 0.2.60 — 2026-07-22

**Skills work as a system**

- Each specialist now carries guidance on when another skill should run first: a page build considers a layout/concept pass before building, and decision research considers sharpening the question when the decision is still unformed. The result is recorded so the contribution is traceable.
- The router runs a single skill by default and composes only when a pre-step clearly earns its cost, rather than stacking skills a task does not need.

**Host-neutral**

- Removed host-specific wording from skill instructions; each installed copy names its own host through the existing per-host mechanism, so the source reads the same everywhere.

## 0.2.59 — 2026-07-21

**Fixes**

- Renamed the orchestrator skill from `lumen` to `route`, so the skill list no longer shows a second "lumen" next to the plugin of the same name. It is now invoked as `/lumen:route`. Its server skill id is unchanged, so validation and existing readiness records are unaffected.

**Contact**

- Every place that pointed users to `lumen.siraj.ai` for a key now points to `hello@siraj.ai`: the README, the marketplace description, and the plugin's not-connected message. The plugin homepage is now `https://siraj.ai`.

## 0.2.58 — 2026-07-21

**Transparency**

- Every skill now ships an "About Lumen" block stating what is sent, what is kept (aggregate request counts only), where it goes, and what stays private. Instructions that told the agent to conceal routine operation have been removed — the goal was uncluttered responses, and it is now written that way. Skills answer plainly when asked what they are doing.
- Added `TRUST.md` (public data-handling page) and `PROTECTION.md` (internal boundary guide).
- Replaced `UNLICENSED` with a real EULA (`LICENSE.md`), now shipped in the package.

**Fixes**

- **Cross-skill invocation was missing from every specialist.** Only the orchestrator knew how to load a sibling skill, while `expert-research`, `question-sharpener`, and `web-builder` each instructed the agent to "use Writer" with no mechanism — so it improvised instead of running Writer, and packets were missing required voice evidence. All seven skills now share one sibling-loading contract naming `/lumen:writer` and `/lumen:skillsmith`.
- **`concept-visualizer` was shipping frozen instructions.** A stale hand-written `SKILL.md` (v0.2.55) in its source folder was overwriting the generated file on every build, so it silently missed two versions of compiler improvements. Removed, and the build now fails if generated output appears in a source folder.
- Builds no longer fail with an opaque `EPERM` when sync-conflict folders (`writer 3/`) appear in generated output; the compiler now names the exact folders to delete.

**Size and usability**

- Moved the full public contract out of every skill body into `references/public-validation-contract.md`. Specialist skills are roughly 55% smaller (Writer: 14,576 → 8,230 words), which lowers context cost per run.
- The not-connected message now explains what Lumen does, where to get a key, and how to continue without one, instead of `Add LUMEN_API_KEY to finish this run.`
- Skill descriptions rewritten around what users ask for rather than internal process, so skill routers match them correctly.

**Copy**

- Every reader-facing surface now passes Writer's `draft_shape` and `source_faithfulness` gates: the six skill descriptions, the About Lumen disclosure block, the not-connected message, the sibling-loading section, the marketplace README, and TRUST.md. The descriptions and disclosure block additionally pass `user_voice`. Earlier drafts failed on invented anchors, packed item lists, and negated framing; each was repaired against real source facts rather than reworded around the checker.
- Instruction bodies and reference models were deliberately left outside Writer's scope. Its gates measure reader movement and prose shape, so applying them to a specification would truncate state enums and soften safety prohibitions. Those files are covered by `quick-validate`, the cold-read audit, and the red-team suite instead.

**Writer lint over instruction text**

- Ran Writer's shape diagnostics across all seven SKILL.md files and the shared contract as a lint, with judgment applied per finding rather than mechanical gate-chasing. Required-tier findings fell from 72 to 4 across the skill bodies and from 26 to 14 in the contract. Fixes led with the desired action while preserving every boundary: "Stop before the second idea" became "End the turn once the first idea lands," double negations were straightened, and em-dash splices were removed.
- The remaining findings are deliberate keeps, where negation is the load-bearing semantics: "Never store or ship a user's completed private profile," "Never imitate a full upgrade," "Never send raw private conversations," the anti-echo list, and the property-authority scoping rule. These protect privacy, upgrade integrity, and IP, and stay as written.
- One transparency conflict surfaced by the lint: the contract still said "never describe how it was stored" about the key, contradicting TRUST.md. Now: the key value is secret; its storage location is answerable.
- Large reference models (writer-model.md, concept-visualizer-model.md, and peers) carry review-tier style findings and were deliberately deferred: they are specifications, and the remaining flags sit on precise enumerations a prose rewrite would degrade.

**Validation moved fully server-side**

- The package no longer ships executable validators. Eighteen Python files (~11,800 lines) previously shipped, and many of their detectors duplicated checks the service already performed — publishing exact thresholds such as the 4-proper-noun cluster trigger and the source × 1.25 word budget, and creating a path where a local pass could contradict the service verdict on the same text.
- Packets no longer need to attest that a local checker ran. The service already assessed every submitted artifact independently, so that requirement was redundant rather than load-bearing. Assessment coverage is unchanged; only the client-side duplicate is gone.
- Manifests no longer reference scripts in runtime steps, resources, or required packet artifacts, and five reference documents now show the Lumen submission call in place of local checker invocations.
- The compiler excludes `scripts/` from the package, and `npm run publish` fails on any shipped `.py` or `.sh` file.

**Tests**

- `red-team-public-boundary` now asserts transparency in both directions: scoring internals must stay in, and the disclosure block must stay present. Concealment phrasing fails the build.

## 0.2.57

Claim-level Expert Research provenance: discovery/evidence separation, inspected anchors, dependence-aware consensus, transfer and coverage contracts, correction propagation, reproducible trajectories, and stage-specific backend validation.
