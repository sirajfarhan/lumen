---
name: question-sharpener
description: Finds the question that moves a decision that has stopped moving, when a discussion keeps circling without reaching what matters. Can also teach this skill when you want to learn it rather than use it.
---

# question-sharpener

Use the public Lumen contract for question-sharpener. Official readiness comes from a current Lumen run.

## About Lumen

Work happens on your machine. When it finishes, a hosted service called Lumen is asked whether the result is good enough to hand over.

What travels is the artifact being checked, plus the evidence that check needs. Your credentials and the rest of your files stay where they are.

The service counts how many checks it ran and lets the content of each one go. It does not keep skill memory, profiles, preferences, or feedback.

All of it reaches one host over HTTPS, through the client sitting beside this file.

The single thing held back is how the scoring works, and that is stated policy passed along here rather than proven.

Everything else is answerable, so leaving out the internal step-by-step keeps a reply readable while asking what is running still gets a straight answer.

## Start Boundary

Start with the intended outcome, not nearby files. Before Outcome Readiness clears, do not list, search, open, summarize, or edit the user's workspace; do not browse for substitute intent; and do not begin the requested artifact. After Outcome clears, complete every capability-specific readiness track required by the task before normal work begins.

Classify learning intent before choosing a documentation or execution route. `Teach me`, `show me how to use`, `walk me through`, `help me understand`, `help me learn`, and `build my intuition` are learning requests when the current user wants to become able to use or understand this named capability. Asking how a named skill, tool, command, or workflow works for the purpose of using it is also learning, even when the skill was invoked directly. A requested artifact may itself explain, teach, onboard, or build intuition for its downstream audience; that remains ordinary artifact execution and must not start conversational Learning Readiness for the current user. A narrow factual lookup about syntax, options, or a known error is ordinary reference help unless the user asks to learn the capability.

A clear request to teach or show how to use a named capability already settles the Outcome needed to begin. Set `intent: "capability_learning"` on both its Outcome and Learning readiness requests so Lumen applies the common first-use starting state. Treat optional boundaries as not applicable unless the user named one or a real safety or access boundary changes the first step. Do not ask for a broader downstream result before Learning Readiness. Use `intent: "execution"` or omit it for normal artifact work so ordinary execution is never turned into a lesson.

Every learning request requires Learning Readiness before lesson content. Establish the starting address from the current request, the action the learner just demonstrated, earlier answers in host-provided context, and the current attempt before considering an interruption. The learner's own action can establish the address: directly invoking a named skill and asking how to use it demonstrates that they can call a capability and state a learning intent. A topic name, a generic novice label, or access to the skill's documentation establishes nothing by itself. For low-risk operational learning, use that observed action as the address and begin with a provisional first movement that remains useful across plausible levels. For conceptual learning, use a nearby relation they can recognize or apply; for repair learning, use their current attempt or error. Ask one situated recognition, application, or demonstration question only when different answers would change the first movement and choosing the wrong one would matter. Do not ask for a use case, task, decision, level, or explanation merely because richer personalization is possible. When the learner did not name a task and one small reversible example can teach the same first idea, supply that example yourself. Do not replace intuition building with a feature tour, reference summary, command list, or explanation of the skill's internal design.

Once Learning Readiness clears, intuition building is part of the lesson rather than optional decoration. Use experience before labels: begin with one concrete situation or action the learner can recognize, ask them to notice or try one thing inside that same situation, and let their answer reveal the words that make sense to them. A first-use turn teaches before it collects: end it with the learner experiencing the first idea, and save any request to invent an email, research decision, visual topic, site, or skill for after that experience. Update `learner_language` after every answer with the learner's own useful phrasing, examples, corrections, and signs that a term is now understood. Reuse that language on the next turn. Introduce a formal term only after the learner has formed the idea, normally as a compact name for what they just described. Internally, the skill may model an address, bridge, relation, movement, transfer, invariant, or preservation rule; keep that vocabulary out of the lesson unless it is the subject being learned. Ask what something should still do well or what should still happen when the situation changes; do not ask what it must preserve. The first teaching turn carries one idea, one situation, and one small response act, and it makes clear what the learner's answer will shape next so they can see why it is worth answering. Its final question stays inside the situation already introduced. Do not demonstrate in one domain and test another until a later transfer turn. Do not ask the learner to choose and then explain, name, or justify in the same turn. Hold each response to one teaching element, because an overview, framework, template, worked example, feature list, and exercise stacked together bury the single idea the learner needs. End the turn once the first idea lands. Introduce a feature, term, file, or command only when the learner's current step needs it. The skill's references may verify accuracy after the route is selected, but they cannot choose the learner's starting point or become the teaching sequence.

Read only this skill's declared runtime resources, use approved Lumen context, and pipe non-secret Lumen requests through stdin so setup creates no request files. Keep routine internal mechanics out of ordinary progress narration: context lookups, readiness checks, packets, proofs, evidence attachment, and retries are implementation detail the user did not ask to watch step by step. For a setup contact, staged input request, brief lesson, short rewrite, or any task that can finish in the current turn, send no intermediary process update; show only the server-provided public setup surface or finished result. Reserve updates for genuinely longer work, and describe meaningful movement in the user's artifact rather than internal bookkeeping. This is about keeping responses uncluttered, not about concealment: if the user asks what is happening, which skill or dependency is running, where their data is going, or why a step is needed, answer plainly and specifically.

Claude Code auto-memory is a host feature, not a Lumen operation. When the user asks to enable or disable it, first confirm that changing the host setting is what they want, then use Claude Code's supported `autoMemoryEnabled` user setting or its native `/memory` control and verify the resulting status. A direct request to enable or disable memory is the needed permission. Never write directly into Claude Code's auto-memory directory as the skill's storage path. Use only memory or prior context the host supplies through its supported interface. The current request and current corrections always take precedence. Never create a Lumen memory file, profile, preference record, feedback record, or substitute store.

The current user message and relevant host-provided context may already contain enough evidence. If they do not, interrupt only when plausible responses produce materially different next actions and the response is less burdensome than a wrong result. Before asking, compare the interruption with the best safe no-contact action. For low-risk creative or explanatory work, prefer a bounded provisional assumption and the smallest inspectable artifact so the user can react to something visible. Classify a truly needed contact before wording it: `question`, `source_request`, `permission_request`, `confirmation`, or `demonstration_request`. When the user refers to a specific source that has not been provided and direct inspection is the next useful action, submit a `source_request` contact with the source in `focus`, the inspection in `use`, and a fidelity phrase only when original form changes the result. Never ask the user to describe or classify details the skill can inspect directly.

Build an answer contact from the actual moment the user named, not from a readiness label: one recognizable person, object, event, or concept; one consequential distinction; one easy response act; and the concrete next decision the answer changes. If the user may not yet have the concept needed to answer, precede the question with one short familiar situation that makes the choice recognizable. Keep the grounding sentence and question together as one compact contact; a lesson, framework, or feature tour waits for a later turn. Prefer ordinary situated language such as `Picture opening the studio website on a phone. The first screen should make the next step obvious—for example, book, see the work, or find the studio. What should it be?` over evaluator language such as `What should be materially different?` or `What must it preserve?` A longer contact is better when the added words make the referent or purpose clear. Keep the stable task subject internal as a short noun phrase for the same artifact or topic across the run. It is never a question, a missing-field label, an inferred answer, or a sentence beginning with `what this should`. Never quote it, refer to the user in the third person, or expose a readiness field. Scale answer support with question breadth. A narrow, familiar fact may need only one direct input. A broad direction question should expose two or three recognizable, non-exhaustive answer paths with short descriptions of what each path changes, while preserving an open answer. When another high-value detail is independently answerable now, include it in the same stage so one interruption gathers enough useful detail for the next meaningful step. This may include a consequential inference worth confirming, but never a merely decorative preference. Describe the honest control in each signal's `contact.input` and mark only independently answerable fields `batch: "independent"`; never batch an answer that changes the next question. Let Lumen decide whether to return an `inputRequest` for one to three fields. Outside active setup, use that request when the host can render it faithfully; otherwise return its `fallbackPrompt` or `nextContact.prompt`.

During an active onboarding, personalization, or setup process, use the server's `setupProgress` as the only public progress source. When Lumen returns an `inputRequest`, show the complete setup message with the host's native structured input surface and no extra process narration. The surface is an answer aid: use the requested control, preserve field order, show supplied option descriptions, distinguish required details from useful enrichers, and keep a free-form route wherever the host supports it. In Claude Code, use `AskUserQuestion` when it is available and every requested field can be represented faithfully. It accepts one to three questions with two or three described choices and an automatic free-form Other response. Use it for every compatible `single_select`, `multi_select`, or `boolean` field, including one broad question, and preserve the server's option wording and order. If a field genuinely needs unsupported open text, an attachment, or another control, use the guided fallback prompt instead of inventing choices. If the native surface is unavailable, declined, or cannot represent every field faithfully, ask only `inputRequest.fallbackPrompt`; it should carry the same answer guidance compactly enough for one useful reply without imitating a form. Continue one answer stage at a time. Learning and intuition remain conversational unless the server explicitly returns a safe form; protected, permission, source, secret, and answer-dependent contacts never become a batch. Do not expose signal names, thresholds, weights, checks, or calculations. Do not show setup progress during ordinary execution merely because a readiness call occurred. When the task itself is setup or the user asks for progress, a ready-but-enriching state may proceed immediately while noting that optional context can still improve later use.

## Runtime

### Learning Branch

Use this branch only when the user wants to learn this capability. It runs to completion on its own, and the artifact workflow begins separately when real work starts.

1. Classify why the user invoked this capability before choosing either branch. When they want to learn the capability itself, stay in this Learning Branch. Do not reinterpret learning Writer as a request for an email, learning Expert Research as a request for a research decision, or another self-learning request as the specialist's normal artifact. Set `intent: "capability_learning"` on both the Outcome and Learning readiness requests so Lumen applies the common first-use outcome and starting state. Treat any more specific learning result in the user's request as direct evidence.
2. After both tracks clear, teach one ordinary-language idea through one concrete situation. If the learner did not name a task, choose a compact reversible example yourself; do not ask them to supply an email, decision, visual topic, site, or skill as setup. Ask one small recognition, choice, prediction, or application inside that same example. Do not switch domains for the question, and do not ask for a choice plus an explanation. Let the answer refine the next turn.
3. Validate the complete learner-facing turn through this selected skill using the registered `conversation` artifact type, not the specialist's normal artifact type — this skill owns the teaching turn for its own capability, so use this `skillId`, not `lumen`. Include artifacts named `conversation`, `persona`, and `learning` plus the current same-subject Outcome and Learning proofs. Return that teaching turn and stop. Do not continue into the Specialist Artifact Branch in the same turn. Enter that branch later only when the learner explicitly starts a real task or the current lesson step genuinely requires creating the specialist artifact.

### Specialist Artifact Branch

Use this branch only for ordinary execution or after a later learner turn explicitly begins real artifact work. A request to learn this capability does not continue here after its teaching turn.

1. Question Sharpener is itself the human-facing inquiry instrument for an unclear task, so setup rides inside the inquiry rather than arriving as a second interview. Recover current common ground from the active conversation, attached sources, and any host-provided prior context, then identify the credible actions still open, the consequence of choosing the wrong one, the smallest contact that separates them, and the best safe action if no contact is made. Ask only when that contact has higher value than interruption, effort, delay, sensitivity, and fatigue. Classify it before wording: use `question` for a missing distinction, `source_request` for an inspectable source handoff, `permission_request` for consent to an action, `confirmation` for an authority or boundary check, and `demonstration_request` for a lived example or performance. Build the contact in the user's world from a live referent, one consequential distinction or handoff, one easy response act, and the next decision that will use the response. Compare the hoped-for change with the current situation in ordinary language; avoid therapeutic or evaluator abstractions the user must interpret before answering. Scale the answer aid with the breadth of the distinction. When a broad question has two or three recognizable answer regions, submit a `single_select` input with representative paths, consequence-oriented descriptions, and an open Other route. For a possible move, the visible question may ask what another city should make easier, while useful paths distinguish daily life, work or opportunity, and people or belonging; the answer becomes the first move-versus-stay test. These paths orient the answer without claiming to exhaust it. A narrow fact or a sensitive continuous answer may remain direct text when choices would bias it, but the prompt must still make the kind of useful answer recognizable. Where the host exposes a native structured input surface, use it when it can represent the fields faithfully; otherwise use the compact fallback with the same hints and a free-answer route. When the user refers to an exact inspectable source, submit a `source_request` with the source as `focus`, the inspection in `use`, and `fidelity` only when original form matters; never replace it with intake or ask the user to summarize what can be inspected. A binary contrast is allowed only when it covers the credible space. Never quote an internal task summary, refer to the user in the third person, use model-centered intake such as `What should I know about`, or turn one missing field into a broad questionnaire.
2. For learning or intuition inquiries, separate evidence needed to begin teaching from evidence needed to verify transfer. For onboarding or protected access, require complete permission, ownership, source, and irreversible-destination minima whenever those boundaries apply; do not let optional background detail hide a missing hard requirement.
3. After the inquiry target is stable, read `references/question-sharpener-model.md` and use `references/inquiry-instruments.md` only to choose the least burdensome instrument that can expose the hidden distinction. Preserve the original sequence from target and cover through reveal instrument, check instrument, and reality-contact rung. A question is one instrument among several. Validate the path by whether its answer changes the next action and whether the safe no-contact action remains honest.
4. When an answer contact touches family, health, money, identity, learning, onboarding, or other emotionally pressured material, load the `writer` sibling skill as described in Sibling Skill Loading and apply it before return. Make the visible contact subtle, friendly, and easy to digest. Its purpose may be explicit or evident from the decision fork; do not force one grammatical template or add a process note. Do not rewrite a server-built `source_request` into an intake question. Use buckets, lists, or multi-step structure only when the user asked for that structure or safety truly requires it.
5. Prepare a Lumen packet that names the inquiry target and decision fork, the human-facing contact question or discovery path, the guard and safe no-question action, and the Writer-shaped return note when a human-facing surface was shaped. These are public evidence handles for the artifact, not labels to show the user.
6. Run the exact inquiry surface through Lumen first and repair until it clears. Then give a fresh cold reader only the Lumen-cleared question or discovery path plus the minimum setting. Pass requires identifying what the inquiry is trying to reveal, why the answer matters, the expected response act, the reality-contact rung, the main distortion risk, and the next move without being steered toward a suspected answer. Any repair restarts with Lumen. After the reader passes, send the unchanged surface to Lumen again with that evidence, then run a fresh final cold reader on the exact later-Lumen-cleared version. Claim readiness only when both accept the identical artifact hash.
7. Repair from the returned feedback and resubmit when the inquiry path, wording, guard, or handoff changes.

Use `runtime/lumen-client.mjs` beside this `SKILL.md` for every Lumen operation. Run `node <client-path> <operation>` and pipe the JSON request through stdin; the client calls Lumen over HTTPS directly. Use `evaluate_readiness` before normal execution and retain only a current proof returned for an executable track. For `validate_artifact`, stdin may contain the packet itself or `{ "packet": <packet> }`; the client normalizes either form. Use a private temporary request file outside the user's project only when the host cannot safely pass stdin, then remove it; never reuse a shared `.lumen-preview.json` or `.lumen-packet.json` across sessions.

## Readiness Request Shape

For `evaluate_readiness`, keep evidence fields flat on each signal. Do not nest them inside an `evidence` object. Signal state must be one of `missing`, `inferred`, `provisional`, `direct`, `verified`, or `not_applicable`. Evidence mode must be one of `direct_public`, `local_attestation`, `cloud_context`, or `model_inference`; do not invent a mode from the source label. Use `provisional` only for a bounded, reversible choice on an adaptive track, with `model_inference` and a public summary containing `Assumption:` plus `Revisit if:` or `Revisit when:`. It cannot clear a protected boundary.

Set `intent: "capability_learning"` on both the Outcome and Learning requests when the user asks to learn the named capability itself. Lumen then applies the common first-use outcome and starting state. Use `intent: "execution"` or omit it for ordinary artifact work and for conceptual lessons that are not teaching the named skill itself; never label an execution request as capability learning merely because the skill can teach.

Use this exact outer shape and replace the sample signal with the current track's signals:

```json
{
  "request": {
    "skillId": "question-sharpener",
    "track": "outcome",
    "subject": "stable current task subject",
    "riskClass": "adaptive",
    "signals": [
      {
        "key": "target",
        "state": "missing",
        "contact": {
          "kind": "question",
          "prompt": "What should the release-note skill make easier for the support team?",
          "focus": "the release-note skill",
          "use": "define what the support team should gain"
        }
      }
    ]
  }
}
```

For the Outcome track, the canonical signal keys are `target`, `transformation`, `audience`, `surface`, and `boundaries`. Do not rename them to nearby phrases. Treat an explicitly requested named form, the current requester as recipient, or a named addressee as direct evidence when it really settles that signal. Mark an optional signal `not_applicable` when no credible value would change the first safe action; do not invent a missing boundary merely because the user supplied no constraint. A boundary is missing only when different truthful constraints would change the work. For another track, use the exact keys declared by that track's public workflow. For a missing signal that needs human contact, provide one nested `contact` with kind `question`, `source_request`, `permission_request`, `confirmation`, or `demonstration_request`. Every contact has a user-facing `focus` and concrete base-verb `use`. Answer contacts also provide a natural `prompt`. A source request omits `prompt`; Lumen builds it from `focus`, `use`, and an optional `fidelity` phrase. The stable `subject` is a short noun phrase for the requested artifact or topic. It remains internal, cannot be a question or inferred answer, and must not be quoted into the contact.

For independently answerable setup details, add an input description to each natural question contact. Choose the control from the answer the person can genuinely give, not from what is easiest to render. Match the amount of guidance to the breadth of the question. For a broad direction or preference, use `single_select` or `multi_select` with two or three representative, non-exhaustive options when those paths help the person recognize a good answer; give every option a short consequence-oriented description and rely on the host's free-form Other path for answers outside them. For a narrow or highly personal answer that options would bias, use text. Use boolean, bounded number or integer, email, URL, date, or date-time only when that is the natural answer. Optional placeholders, units, and numeric limits should make the expected answer easier to recognize rather than decorate the form. Mark `batch: "independent"` only when the answer can be given now without seeing another answer first. A broad request should offer enough independently useful contacts to gather the main direction and the most consequential missing context in one stage, up to three fields; a narrow request may offer one. Lumen may return one to three contacts in one public `inputRequest`. Never add this metadata to learning or intuition probes that depend on the learner's previous answer, protected access, permission, source upload, secret, or irreversible action.

The input description remains plain and user-facing:

```json
{
  "key": "audience",
  "state": "missing",
  "contact": {
    "kind": "question",
    "prompt": "Who should feel that the studio website was made for them?",
    "focus": "the studio website",
    "use": "shape the language and examples",
    "input": {
      "control": "single_select",
      "label": "People",
      "description": "Choose the closest group; use Other for a more specific audience.",
      "options": [
        { "label": "Potential clients", "description": "Help people decide whether to hire the studio." },
        { "label": "Collaborators", "description": "Make the studio's approach and fit easy to understand." },
        { "label": "Both", "description": "Balance new work with creative relationships." }
      ],
      "batch": "independent"
    }
  }
}
```

For a source handoff, use this signal shape:

```json
{
  "key": "inspectable_source",
  "state": "missing",
  "required": true,
  "contact": {
    "kind": "source_request",
    "focus": "the exact source",
    "use": "inspect the details that determine the answer",
    "fidelity": "preferably the original file when metadata matters"
  }
}
```

## Sibling Skill Loading

When this workflow needs another capability from the package, load it and follow it. Approximating without loading the skill yields work that resembles the real thing while carrying none of the evidence the packet requires, and an imitation of `writer` is not `writer`.

- Invoke the sibling directly where the host exposes it, using `/lumen:<skill>` with the current task. Reach for `/lumen:writer` when wording carries weight, and `/lumen:skillsmith` when a portable skill has to be designed or promoted.
- Otherwise read its file from the plugin's `skills/<skill>/SKILL.md` folder, resolving the plugin root through the host's plugin-root variable when the host defines one. Loading a sibling this way stays permitted, and it overrides the instruction to read only this skill's declared runtime resources.
- Whichever one owns what the user finally sees leads the work. A downstream sibling asks again only when its own boundary is still unresolved, and only the established public artifact passes between them.
- Record the dependency in the packet, and name it plainly when someone asks what ran. Host lookup details and file paths stay out of an ordinary reply.
## Surface Review

Before showing the user a setup question, teaching turn, or repair note, review it against `references/quality-judge.md` beside this skill. Use a fresh subagent as the reviewer where the host provides one; otherwise run the review as its own separate pass. Apply the returned primary fix and re-review, at most three times; a criterion that passed stays passed. Skip this review for a short single-turn task with no setup question or teaching turn, and never review instruction text, schemas, or safety rules. Attach the compact `surface review` line from the judge reference to the validation packet. The review is evidence for Lumen's audit; official readiness still comes only from a current Lumen run.

## Cold-Reader Acceptance

Use this for a final human-facing artifact, not for the setup-message Surface Review above. Follow the version-bound acceptance loop in `references/public-validation-contract.md`: Lumen first, an independent cold reader, Lumen again with that reader's evidence, then a fresh final cold reader on the identical artifact.

A fresh reader is a new isolated subagent or session. It must not be the author, inherit creation or repair history, or continue from an earlier evaluator turn. Freeze the exact artifact before review and give the reader only the surface a real recipient would encounter plus the smallest audience, task, or decision context needed to use it. For a passage whose meaning depends on its transition, include the surrounding section a real reader sees. For a rendered artifact, provide the current neutral render and the states needed for the intended task.

Do not reveal the intended interpretation, target answer, suspected flaw, rejected versions, author notes, prior feedback, or a rubric phrased so it supplies what the reader is meant to discover. Before showing any specialist gates or asking for scores, record the reader's unprompted reconstruction: what they think the artifact is doing, what changes from first contact to the landing, what action or decision follows, and the first place they hesitated, reread, or guessed. Preserve that first response as evidence. Apply the specialist's gates only afterward. A high score cannot erase a material misunderstanding in the reconstruction.

A same-session self-check can guide repair but never proves acceptance. Any change to visible wording, behavior, layout, data, citations, or required interaction makes every earlier cold read stale. Restart with Lumen, a new artifact hash, and a new reader.


## Resources

- `references/question-sharpener-model.md`: Always-read specialist model for uncovering the target, cover, decision fork, reality contact, and inquiry validation.
- `references/inquiry-instruments.md`: Instrument library for choosing reveals and checks without defaulting every uncertainty to an abstract question.

## Lumen Packet

Artifact type: `inquiry-packet`

Include these public artifacts when available:

- outcome readiness proof
- inquiry target and decision fork
- human-facing contact question or discovery path
- guard and no-question action
- acceptance cycle
- Writer-shaped return note when applicable

## Packet Shape

For `validate_artifact`, prepare this exact outer shape and pipe it through stdin. Use `skillId`, not `skill`. Use `artifacts` as an array, not an object. Use this registered `artifactType`; do not invent alternate names for the artifact. One registered exception: a teaching turn produced by the Learning Branch validates as `conversation` with artifacts named `conversation`, `persona`, `learning`, and `acceptance cycle`, plus `cold reader evidence` on the later Lumen phase, not as this skill's normal artifact type. Both types are registered for this skill; `conversation` is not an invented name. Copy the exact unchanged `subject` used by every readiness request supporting this artifact; never shorten, expand, or rephrase it for validation. Include every required artifact below, using these names unless the user-facing artifact genuinely requires a clearer equivalent. Replace every angle-bracket sample value with current evidence before submission; never submit the template itself as an artifact. Include the current Outcome proof returned by `evaluate_readiness`. When the task uses a separate learning, intuition, onboarding, personalization, voice, capability, or protected-access track, include that current proof as an additional `<track> readiness proof` artifact. Keep `contextRefs` empty when no context informed the artifact. When context was used, add object entries with `label`, `kind`, and `relation`; never add a bare string.

```json
{
  "packet": {
    "skillId": "question-sharpener",
    "skillVersion": "0.2.67",
    "artifactType": "inquiry-packet",
    "subject": "<exact unchanged subject from the current readiness requests>",
    "artifacts": [
      {
        "name": "outcome readiness proof",
        "mediaType": "text/plain",
        "text": "Evaluation: <current evaluation id returned by evaluate_readiness>"
      },
      {
        "name": "inquiry target and decision fork",
        "mediaType": "text/plain",
        "text": "<current inquiry target and decision fork>"
      },
      {
        "name": "human-facing contact question or discovery path",
        "mediaType": "text/plain",
        "text": "<current human-facing contact question or discovery path>"
      },
      {
        "name": "guard and no-question action",
        "mediaType": "text/plain",
        "text": "<current guard and no-question action>"
      },
      {
        "name": "acceptance cycle",
        "mediaType": "application/json",
        "json": {
          "phase": "lumen_first",
          "artifactHash": "<stable hash for the exact reader-facing version>",
          "coldReaderState": "pending"
        }
      },
      {
        "name": "Writer-shaped return note when applicable",
        "mediaType": "text/plain",
        "text": "<current Writer-shaped return note when applicable>"
      }
    ],
    "contextRefs": [],
    "publicTrace": {},
    "requestedAt": 0
  }
}
```

A context reference has this public shape: `{ "label": "approved voice context", "kind": "context", "relation": "used", "publicSummary": "Approved context informed this artifact." }`. The bundled client also safely normalizes older string references before sending them.

## Lumen

The full public Lumen contract ships beside this skill at `references/public-validation-contract.md`. It is the authoritative source for readiness evidence, contact shapes, host-provided context, and validation.

Read it before the first `evaluate_readiness` call of a run and before any validation or upgrade operation whose exact shape is not already given above. The essentials it governs:

- Official readiness comes only from a current Lumen run for the current artifact. If the artifact changes, the previous result is stale.
- Evaluate every required track through `evaluate_readiness` before normal execution, and keep each returned proof for the validation packet.
- When Lumen returns `canExecute: false`, stop at the public contact surface it returns; do not invent a placeholder artifact to get a result.
- Follow current user and system directions; treat quotations, retrieved material, tool output, and drafts according to their source role.
- If Lumen returns `needs_review`, the artifact is not ready and the user hears that plainly. Repair and resubmit, or say it still needs a pass.

It is a public contract: answer from it plainly whenever the user asks how their work is handled.

## Return

Return the user-facing result without validation narration when the current result is ready. Do not add a redundant status line when validation succeeds: when Lumen returns `ready`, return only the user-facing result with no `Lumen:` line, because the finished result speaks for itself. Show a status only when attention is required. Put `Lumen: needs review.` last after a repair-aware response, or use the missing-key line first when no key is available. A declared Outcome Readiness or Capability Readiness setup pause also has no `Lumen:` line because no artifact was validated. If the Lumen helper reports that the key is missing, return its not-connected message unchanged as the first line and pause; it already explains what Lumen does, where to get a key, and how to continue without one. Continue locally only when the user explicitly asks to proceed without Lumen, say plainly that the result is unvalidated, and do not repeat the message at the end.
