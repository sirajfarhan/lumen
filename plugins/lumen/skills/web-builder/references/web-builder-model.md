# Web Builder

Build the website the story has earned. Input: `$ARGUMENTS`

## One Movement

This skill turns a user request into a working React web experience. The result can be a quiet page or a full interactive surface. The runtime question stays the same: what visitor change must the site create, and which web form creates that change with the least distortion?

Begin from the visitor's starting mental model and the proof the site must carry. Let templates and trends serve that judgment only after the visitor path is known. When the visual bar matters, make source contact before implementation. The source might be a working precedent or a reusable component. It might be a motion demo or a visual reference that solves the same kind of pressure. Borrow the transferable invariant and leave the source identity behind. Choose the smallest web carrier that can make the proof legible. Choose the content lane before copy enters the page. Choose the reference lane before code or mechanics are adapted. Choose the style stack before the page inherits defaults. Compose the carrier in React. Validate the rendered artifact in four passes. It has to work. It has to reconstruct. It has to read in the user's voice. It has to feel like a specific visual world.

The skill stays one integrated capability. Routing stays with composition because both serve the same visitor-facing judgment. Validation stays in the same runtime path because the rendered artifact is the proof. Use Writer as the separate content craft lane whenever the site has meaningful reader-facing copy. Use the web style stack as the separate art-direction lane whenever the request is greenfield or the current design system is weak. Split work inside the run when the artifact itself earns deeper support. Operation earns tool-state depth. Spatial proof earns 3D depth. Evidence-heavy claims earn source and chart depth. The default path remains one React build with one story model and one rendered validation pass.

## Runtime Default

For a greenfield web artifact, use React as the default execution world. Use the existing project conventions when the user is working inside a repo that already has a React setup. If there is no project setup, create the smallest React implementation that can run locally and be inspected. Keep framework attention on React unless the user explicitly asks for a framework decision or the existing codebase requires a non-React answer.

Run a render feasibility preflight before coding. Name the result in `react_execution.runtime_feasibility`. The preflight answers one question: which current path will let this page become inspectable here? Prefer existing project scripts when they exist. Use installed local dependencies when they are already present. Use an approved install when package work is the route. Use a bundled or cached runtime when it carries the same job. When a self-contained inspection shell is the fastest current surface, use it for screenshot judgment and label it as diagnostic. Name the dependency step that would complete React acceptance. Full readiness uses a runnable React artifact with current screenshots and independent reconstruction.

Use `references/web-style-stack.md` when a greenfield build needs art direction. Also use it when the user asks for high visual quality or when the first attempt feels generic. The normal high-quality path is React with a deliberate style system that gives stronger control than generic CSS. Use Tailwind as the token and layout layer when it speeds precision. Use shadcn/ui when editable local component code helps. Use Radix, Base UI, or React Aria when accessible primitives let the surface become more custom while preserving behavior. Use Motion for ordinary interface animation. Use GSAP when timeline or scroll choreography is the proof. Use React Three Fiber with Drei when spatial proof passes the 3D gate.

Use other libraries only when the carrier earns them. A chart library earns its cost when evidence must be inspectable. Three.js earns its cost only when spatial proof passes the 3D gate. Animation libraries earn their cost only when motion clarifies state or sequence. Asset generation earns its cost only when the visual asset carries the story better than available material.

When the request needs high visual quality, calibrate the first invented composition against source contact. Search and inspect. Use the existing project first when it has a strong design system. Otherwise make two kinds of source contact. One contact calibrates taste through strong finished work. The other contacts implementation through reusable code. A reusable source is useful when it lets the builder inspect the mechanism. A setup source can still support the build. Vite bootstrapping or a basic CSS reference explains how the local app runs. Mechanism-source credit belongs to the source that carries the hard build move. Download or clone a candidate when inspection of real source would change the build. Keep that work outside the user's project until the code will actually be incorporated. Record what was inspected. Record what was borrowed. Record why the final implementation is transformed enough to stand on its own.

## Story Model

For substantial work, copy `references/web-experience-model-template.json` into the run folder as `web-experience-model.json` and fill it before building. For quick work, hold the same model in notes. The model is the control surface that keeps a beautiful page answering the right visitor question. The canonical acceptance bundle should use that `web-experience-model.json` path so planning evidence and final rendered evidence stay in one current file.

The router should name the visitor before it names the page. It should capture the visitor's starting mental model and the uncertainty the site must change. It should also name the visitor goal and the site owner's goal. From there it should state the core claim, the proof that can make the claim believable, and the action or feeling the site should make available. It should also name the render path that makes the current artifact inspectable. If one of those fields is unknown, infer the safest useful version from the request and mark the assumption. Ask the user only when the missing answer would change the carrier or make the site dishonest.

The model must also name three lanes beside the route. The content lane says how Writer will shape or validate the visible words. The reference lane says where source contact happened and what source was inspected. It also says what invariant was borrowed, where the license boundary sits, and how the result will be transformed. The style lane names the visual target and the toolkit path that turns it into a rendered world. It also names the specific visual world that should replace default-demo residue. A site can pass code checks while still needing Web Builder repair when it looks like a familiar demo more than the specific world the visitor should enter.

Choose three axes before choosing the visual form.

```text
Journey Span asks how far the story travels.
Signal: one primary viewport or short scroll carries the point.
Sequence: authored sections or state changes build meaning over time.
Session: the visitor must compare, operate, or complete meaningful work.

Participation Contract asks how much agency the visitor must take.
Witness: the site carries the story through reading, scrolling, stepping, or light reveal.
Choose: the visitor filters, compares, branches, or inspects within an authored frame.
Operate: the visitor manipulates variables, completes a workflow, or uses a tool.

Proof Substrate asks what web material carries belief.
Layout: copy, imagery, hierarchy, rhythm, and composition carry the proof.
Evidence: sources, charts, comparisons, annotations, or methods carry the proof.
System: product behavior, model response, workflow, or state change carries the proof.
Space: geometry, scale, route, location, adjacency, or embodied placement carries the proof.
```

Default to `Sequence`, `Witness`, and `Layout` unless the request proves another level. Escalate Journey Span only when the story genuinely needs more time or state. Escalate Participation when interaction creates understanding beyond reading. Escalate Proof Substrate when evidence, system behavior, or space makes the claim stronger and more honest.

## Carrier Choice

Choose the carrier after the axes. A carrier is the kind of web world that can carry the story.

A reading surface wins when the visitor needs recognition before exploration. It can also win when orientation or a clean emotional proposition is the main job. Route toward a proof or state carrier when the claim needs inspectable evidence or behavior.

A guided story surface wins when authored sequence makes a complex idea easier to receive. Route toward exploration when the visitor's real job is open comparison, and keep pacing tied to understanding.

An evidence surface wins when the site must make a claim inspectable. It is ready when charts and source blocks stay close to the claim and interaction makes the answer easier to inspect.

A product surface wins when the story must move the visitor toward a business or service action. It is ready when the offer, proof, and product behavior make the action feel warranted.

A story-tool wins when doing the thing reveals the story better than reading about it. It is ready when the visitor understands the reason to operate before the interface asks for meaningful effort.

A spatial world wins when spatial relation is the proof. Depth may carry that relation. Scale may carry it. Place or route or physical fit may carry it. Space is ready when geometry makes the story more reconstructable than the best flat alternative.

Pick the carrier that creates the largest correct visitor reconstruction for the least effort. Record the nearest rejected carrier and the reason the selected carrier creates stronger reconstruction. This keeps the page moving toward the right form and a specific style law.

## React Composition

Build the chosen carrier as a coherent React experience through the render path named in the preflight. Let components map to story units first. A component earns its place when it makes the visitor understand, believe, or act more clearly.

The first viewport should make the site legible. The visitor should know what world they entered, why it matters, and what kind of movement is available. Show a hint of the next meaningful layer when the page continues. Lead with the actual experience unless the request is specifically a marketing page and the offer itself is the first experience.

Create one visual world. Typography should obey the story law. Spacing and color should obey it too. Motion should feel native to that law. Imagery should feel like it comes from the same world. Data marks should inherit the same logic. Controls and component states should feel native to the world. Style variety is allowed when the carrier changes the visitor's job. Different presentation dialects should still obey one route decision.

Turn framework primitives into authored style. A component library gives primitives. Tailwind utilities give control. A motion library gives time. Choose a style stack by the world the visitor must believe in. Then customize the tokens until type scale governs density, state design carries behavior, and motion feels native to the world. The site should gain force from a style that would feel too specific to swap onto a generic SaaS or portfolio page.

Use Writer before embedding substantial visible copy. Let Writer shape the first viewport promise and the touchable words when those words create trust, action, or emotional movement. After implementation, inspect the visible copy as interface writing. When the copy is substantial enough to export, run Writer text validation on the current readable copy or content draft and repair true positives before claiming acceptance.

Use interaction as story grammar. A reveal should reduce load or create earned surprise. A filter should make comparison clearer. A control should expose system behavior. A hover or animation should clarify relation, state, or sequence. Keep interactions that make the story stronger.

Use evidence as proof. Put the source close to the claim it supports. Put method or comparison there when the claim needs it. Put uncertainty there when the claim would otherwise feel too certain. Let source support govern every proof asset. Metrics and testimonials need that support. Logos, counts, and case evidence need it too. If realistic placeholder data is needed for a prototype, mark it visibly in the artifact or return notes according to the user's context.

Use motion with restraint. Respect reduced-motion preferences. Motion should help the visitor perceive hierarchy or continuity. It can also reveal causality or state. Design quality should come from the whole visual world, with motion serving that world.

## Aspect Improvement Loop

When improving an existing site, do not tune the whole artifact at once. Choose the aspect whose failure most limits the visitor change. The aspect might be copy, hierarchy, spacing, color, motion, state, proof placement, 3D framing, performance, or responsive behavior. Name the accepted improvement question before acting: what hidden thing is failing, and what would become easier for the visitor to see after this repair?

Use Question Sharpener when the aspect is blurry, repeatedly failing, or competing with other attractive fixes. The handoff should name the target, current cover, hiddenness type, reveal instrument, check instrument, and reality-contact rung. Use expert-research when outside craft knowledge, current tooling, standards, accessibility, performance, or benchmark practice could change the repair. Keep the research panel small and decision-shaped. Stop research when the next source would not change the module rule, implementation choice, or validation contact.

Convert the result into one build rule before editing. A build rule says which module owns the repair, what proof job it has, how it will be validated in the rendered artifact, and what later work must wait. Then implement the smallest change that can prove or disprove the rule. Inspect the live page or screenshot before widening the repair. If the finding transfers beyond this site or appears twice as the same failure class, update the story model or the skill. If it is local taste or one-off polish, keep it in the project notes and continue.

Use this loop as a holistic repair path. A focused aspect still has to fit the route, carrier, visual world, and validation bundle. If the local repair improves the aspect while weakening reconstruction, voice, accessibility, performance, or source-transfer quality, repair the earlier route or module boundary before polishing.

## 3D Gate

3D earns its place when the story's proof is spatial. Pass all four gates before building a spatial carrier.

```text
Spatial necessity: the central claim depends on geometry, scale, occlusion, route, site context, fit, or embodied placement.
Comparative gain: the spatial carrier creates clearer understanding than the best flat alternative.
Burden control: orientation, reset, landmarks, target clarity, motion policy, and input cost are handled.
Progressive delivery: the core message still exists in a flat shell or fallback when 3D is unavailable or unsuitable.
```

When a gate remains open, choose the strongest simpler carrier. Use an annotated flat sequence before reaching for a full spatial world. A map inset may be enough. A rotatable product view inside a flat page may be enough. A guided perspective cut may be enough. When 3D passes, use Three.js or the project's existing React-compatible 3D stack. Then inspect the canvas on desktop and mobile. Acceptance requires a meaningful framed canvas. The spatial relation should be framed. Promised interaction should work. Performance should stay steady. Visible cues should make the relation understandable.

For 3D or spatial hero work, build by dependency ladder. Start with the route contract. Then prove the scene shell: one composed viewport with camera, light, background, fallback, and readable copy. Then prove the spatial law: the terrain, object field, or geometry must carry the main relation before labels explain it. Then add semantic objects or landmarks. Then add the state transition that changes understanding. Then add motion grammar. Then polish material, color, shadow, and interaction feel. Finally run shipping checks. Work on the earliest failing rung. Static reconstruction comes before motion. Motion earns attention only when it clarifies continuity, causality, or state. Material polish earns attention after the scene can already be understood.

## Tool-State Gate

Operate-level work changes the story proof. When a site becomes a tool, model the task loop before building controls. Name the entry state before the first interaction. Name the empty state before data exists. Name the active state while work is happening. Name the error state and the success state. Then define recovery. Decide where focus moves after user action. Decide what a user can complete and what they should understand after completing it.

A tool still needs an authored frame. The visitor should know why they are being asked to manipulate anything before the interface asks for meaningful effort. When a guided surface can make the same point clearly, choose the guided surface.

## Research And Assets

Use question-sharpener when the request is too blurry to know what the site must reveal. Use expert-research when outside reality would change the site. Current product claims can trigger that. Scientific or legal accuracy can trigger it too. Benchmark choice can trigger it. Accessibility rules can trigger it. Performance standards can trigger it. Domain-specific trust can trigger it. Toolkit choice can trigger it when the user asks for a best-current framework path. Use Writer for visible copy and section movement. Use it for product language and validation prose too. Use imagegen when a bitmap asset would carry the story better than available assets. Inspect the generated asset before embedding it.

Research by route pressure. Research earns its cost when it changes the route or proof. It also earns its cost when it changes content, claim boundary, or validation risk. Keep research records outside the skill package. Distill the runtime rule into the model or implementation.

Use visual references as calibration. Borrow the invariant that made the reference work. Keep surface copying out of the build unless the user's brand or existing design system explicitly requires it.

## Reference And Code Adaptation

High-quality web work usually comes from source contact. Use that contact like a developer. Inspect the thing. Learn the mechanism. Then build the user's site with a transformed version of the useful move.

Start with the hidden visual problem. A product page may need a believable component system. A 3D site may need proven spatial mechanics. A story page may need pacing. An evidence surface may need a proof-near-claim pattern. The reference search should answer that problem as its main target.

Search in two rings when quality is important. The first ring calibrates visual judgment. Use strong finished work to see what excellent attention looks like for this carrier. Treat that ring as inspiration unless the source explicitly provides reusable assets or code. The second ring contacts implementation. Prefer sources where real code can be inspected. Official examples reveal supported mechanics. Documented component blocks reveal ownership patterns. Public demos and repositories reveal source shape. Adapt those mechanics only after license review.

Treat the mechanism source as its own gate. A mechanism source is the inspected thing that changes how the site is built. It might govern component behavior. It might govern state. It might govern charting. It might govern motion. It might govern spatial control or responsive composition. It might reveal source-file structure. Vite setup explains the app shell. Package installation docs explain dependency entry. Generic MDN layout pages explain baseline browser behavior. Generated images and earlier local runs can support the work. For an ambitious build where interaction carries proof, mechanism credit belongs to an inspectable source that carries the hard move. The same is true when evidence, tooling, or space carries proof.

Search for mechanism sources the way a developer would. Start with official examples and owned component registries when they fit the carrier. If the mechanism is still unclear, inspect a public demo or a source-linked example. Inspect a GitHub repository when file shape matters. A story-tool might inspect a slider pattern. It might inspect a calculator or stateful form pattern. An evidence surface might inspect a chart or heatmap pattern. It might inspect annotation or proof-near-claim structure. A spatial world should inspect a Three.js source family such as React Three Fiber or Drei. A guided story surface should inspect motion or scroll sequence examples when pacing is part of the proof. When the best result can be safely invented, record why the mechanism is simple enough and still inspect one source when it would improve confidence.

When a public repository or demo looks useful, inspect it before building. Prefer `git clone --depth 1` into a temporary research folder when file structure matters. Otherwise inspect the linked source, docs, or example file directly. Check the license first. Then inspect the files that carry the useful move. That move might live in component shape. It might live in styling method, motion setup, or mobile behavior. Run install scripts from outside projects only when the value justifies the risk and the source looks trustworthy. When the repo is only an inspiration source or the license is unclear, extract the idea and write new code.

The borrowed unit should be an invariant more than a look. A good invariant explains how the source works under pressure. It might describe rhythm. It might describe a responsive relation. It might describe state. It might describe orientation. It might describe timing, density, or proof placement. Strong borrowing keeps the useful mechanism while the user's own visual identity becomes native to the new site. A full page skeleton needs transformation before it belongs to the user's site.

Transform the source before implementation is considered original enough for this skill. The visitor problem should change the code's purpose. The content should change the page's meaning. The token system should belong to the user's site. The object world should too. So should the section relation. So should the interaction state and responsive law. If compatible source code is adapted, preserve attribution or license obligations in the project where required. If only the idea is used, the implementation should feel clearly native to the user's site for a cold viewer.

Record the reference decision in the model before coding. Name at least one selected source and one lower-fit source. Name the mechanism source separately from taste references and setup docs. Say what was inspected or downloaded. Say why the selected source belongs to this visitor problem. Say the license boundary. Say what will be transferred into the React build. If a prior local run is inspected for validator shape, label it as contract support with a clear boundary from visual or code precedent. When the page looks generic after the first render, return to this lane before adding decorative polish.

After implementation, compare the result with the source as transfer. A source-aware reviewer may see both surfaces. The question is whether the useful mechanism still works after the visitor problem has changed the site's purpose and visual law. Do not score screenshot likeness as the goal. Visual resemblance is useful only when it proves the same working move survived. The borrowed invariant should be recognizable as behavior. The source identity should be absent as style.

Make the comparison in three passes. First, name the comparison unit. For a reading surface, that unit may be an attention move or proof placement. For a tool, it may be state behavior. For a spatial world, it may be the spatial operation. For a material world, it may be the governing visual law. Second, compare that unit in the source and in the finished site. Third, name the next repair from the weakest gate. Source fit asks whether the reference belonged to this pressure. Mechanism parity asks whether the hard move survived. Transformation distance asks whether the result became its own site. Quality parity asks whether craft stayed comparable for the new scale. Medium proof gain asks whether the web form made understanding stronger. Identity safety asks whether the final kept signature source residue out. Let the weakest gate control repair. A beautiful site needs mechanism and mood together. An original site still needs the source mechanism that made the precedent useful.

Use different measurement pressure for 2D and 3D inspiration. A 2D review follows the reading path. The source transfer works when the final page makes the same attention move feel inevitable from first contact through proof into state change, including on a narrow screen. Read hierarchy first. Then inspect rhythm. Then inspect proof placement. Then inspect mobile composition and interaction state. A 3D review follows the spatial law. The source transfer works when camera work turns scale with depth and occlusion into one readable relation. Read camera framing first. Then inspect landmarks. Then inspect orientation recovery. Then inspect input burden. Then inspect mobile framing. Then inspect flat-fallback gain. A spatial result earns acceptance when the source mechanism survives as a lawful spatial operation in the new site and the cold viewer can reconstruct the story from the visible surface.

## Validation

Validate the rendered artifact as code and story. Deterministic checks answer whether the site survives as software. Judgment checks answer whether it survives as story. Treat the acceptance bundle as part of the artifact, not as after-the-fact notes. A ready substantial run makes the page agree with the canonical model. That same current artifact then carries rendered inspection. It also carries source-transfer proof and independent reconstruction.

For substantial work, validate the filled story model before the React build starts. Run the public package check from this skill folder.

Submit the artifact to Lumen through the bundled client and let the server assess it:

```bash
node runtime/lumen-client.mjs validate_artifact < packet.json
```

Lumen returns the findings and a readiness verdict. Repair from that feedback and resubmit when the artifact changes.

This command checks the route contract before final quality is judged. It asks whether the model can carry visitor pressure into a chosen React carrier before the page exists. It also makes any extra depth justify itself before implementation. If it reports a hard finding, repair the route model before writing more interface code. A repaired route model gives the UI a better chance to answer the right visitor question before polish begins.

Start validation from the render feasibility preflight. Run the project's normal build command when it exists. Run typecheck, lint, or tests when the project provides them. If package installation is the chosen path, request approval early and return to the acceptance bundle after the install path completes. If the site needs a dev server, start it and inspect the running page. If a self-contained inspection shell is the current surface, inspect it as diagnostic composition evidence and keep the React acceptance step named. Use Playwright or the available browser tooling for desktop and mobile screenshots when possible. At minimum, inspect a desktop viewport and a narrow mobile viewport around 390px wide. Check that text is readable. Check that controls fit. Check that important content is fully visible. Check that fixed elements leave the story unobscured. Check that the first screen feels intentionally composed.

Use screenshot judgment beside overflow metrics. `scrollWidth` can equal the viewport while the screenshot still shows a page that needs repair. The page may have collapsed into a narrow rail. It may have left a large blank field with a weak story job. It may repeat a sticky hero where one composed site should appear. Acceptance requires screenshot judgment. The model should say how desktop and mobile composition occupy the viewport by design and how they go beyond overflow checks.

Validate the content lane. If Writer shaped the copy, record the Writer role in the model. If substantial copy exists, keep a readable copy draft or extract the visible text and run Writer text mode where possible. Treat the result as a writing tripwire while reader comprehension remains a rendered-surface question. Repair generic product phrases and vague labels from the visitor movement. Repair any style-copy mismatch before updating the rendered surface.

Validate the style lane. Screenshot inspection should ask whether the chosen stack created a specific world. The page should show deliberate typography. Spacing should make material believable. Interaction states should feel designed. Motion should stay restrained. The inspection should also show why the selected framework path was more efficient than custom CSS or a heavier stack. If several generated sites all look like the same default design, repair the art direction and stack choice before judging the story.

Validate the reference-adaptation lane. The rendered site should reveal the borrowed invariant while keeping the source's identity out of the surface. The model should show real source contact. The agent may have inspected docs. It may have opened source. It may have downloaded a repository or cloned a demo. It may also state why direct code inspection was optional for this mechanism. The license and attribution boundary should be plain. Check whether the recorded mechanism source actually carries the hard part of this build. A Vite guide may support the app shell. A generic CSS page may support a layout decision. A generated image may support mood. An earlier local run may support validator shape. When custom interaction carries the hard build move, mechanism-source acceptance should point to a source that carries that move. The same rule applies when data visualization carries proof. It also applies when motion, 3D, or high-end visual composition carries proof. If the artifact depends on code from a public source, verify the source terms before acceptance. For a high-ambition visual build, inspect a mechanism source or record the concrete reason the mechanism was simple enough to build safely from first principles.

Run a source-transfer review before claiming acceptance for source-inspired work. The reviewer should know the selected source. The reviewer should also know the mechanism to preserve and the finished site. Record six scores from zero to one hundred. Source fit tests the match between reference pressure and visitor pressure. Mechanism parity tests survival of the hard move. Transformation distance tests whether the user's content and visual world changed the source enough. Quality parity tests craft at the scale of this artifact. Medium proof gain tests whether this web form made the story easier to reconstruct. Identity safety tests whether distinctive source identity stayed out of the final. Treat the lowest score as the repair signal. A production-craft target can sit above the acceptance floor, usually as a separate `quality_parity` threshold. A site can pass reconstruction while still needing craft repair.

Calibrate scores before scoring. The band should describe how much usable proof survives in the rendered artifact. Around sixty, the right idea is visible but the visitor path or craft still needs major repair. The seventies can describe a useful prototype with open burden. The eighties mean acceptance-level work with local limits. A ninety begins when the inspected source and the current rendered site carry the same hard move at a craft level a cold mobile reader can reconstruct with clean evidence. One hundred is the horizon where the artifact feels production-complete and stronger than the available reference path. A ninety belongs to the current rendered surface after the route and craft earn it. Source transfer must earn it too. Mobile composition and cold reconstruction must earn it.

The review should compare the reference with the result before it scores. For 2D work, follow the reading path from first attention into proof and state. The claim should sit where proof can answer it. The hierarchy should preserve the borrowed move at desktop and mobile size. Any interaction should reveal the same relation under state. For 3D work, follow the spatial operation. The camera should frame the useful relation. Scale and depth should make that relation truer. Landmarks and reset should let the visitor recover orientation. Input and fallback should keep the burden earned. A 3D transfer needs more evidence than a 2D transfer because depth can create spectacle while weakening reconstruction. When the 3D result scores lower than its source, repair the spatial law before decorative polish. Reframe the camera first. Then clarify objects. Then strengthen depth cues. Then reduce input cost or improve the flat fallback.

For interactive surfaces, inspect the key states that carry the story. For evidence surfaces, inspect whether claims stay near proof. For tool surfaces, run the core task loop. Then inspect one error path or empty path. For spatial surfaces, inspect canvas pixels and framing. Inspect motion and fallback. Inspect the specific spatial relation the visitor should learn.

Use accessibility and performance tooling when available or when the carrier risk earns it. Lighthouse gives useful deterministic signals. Axe and aria snapshots do too. Keyboard checks and reduced-motion checks reveal issues that visual polish can hide. Treat automated accessibility results as supporting evidence. Complete the judgment through direct inspection of the visible interaction and semantic structure.

After direct rendered inspection, submit the exact substantial artifact to Lumen first and repair it until it clears. Then run a cold reconstruction check when the artifact is acceptance-level or likely to be reused. The reader should see only the Lumen-cleared final site or a current rendered screenshot packet plus the minimal audience task needed to judge it. A screenshot packet can prove reconstruction when it shows the present desktop and mobile surfaces and the key states that carry the story. Pair it with direct live inspection of interaction, accessibility, and performance for full acceptance. The reader must complete the primary path and required states without hidden explanation, clipped or missing content, ambiguous action, broken interaction, or unlocatable proof. They should also be able to say what the site is, who it is for, what changed in understanding, and which visible parts created that reconstruction. Use a fresh independent subagent for acceptance evidence. A same-session read stays in the diagnostic lane. Any repair restarts with Lumen.

After rendered inspection and reconstruction evidence have been written into the model, make that model the canonical acceptance bundle. Use `web-experience-model.json` as the default canonical filename for substantial runs. Name its path inside `validation_plan.evidence_sync.canonical_model_path`. Point `validation_plan.evidence_sync.current_artifact_path_or_url` to the rendered site or artifact that the screenshots and cold reader saw. If draft models or older notes remain in the folder, label them as draft or stale inside `validation_plan.evidence_sync.stale_or_draft_records` so the final evidence path is unambiguous. Then rerun the unchanged artifact through Lumen with the reader evidence and run a fresh final cold user on the exact later-Lumen-cleared version. Readiness requires both passes on one artifact hash.

Submit the artifact to Lumen through the bundled client and let the server assess it:

```bash
node runtime/lumen-client.mjs validate_artifact < packet.json
```

Lumen returns the findings and a readiness verdict. Repair from that feedback and resubmit when the artifact changes.

Acceptance mode proves that the evidence bundle is present and internally connected. It keeps same-session reconstruction in the diagnostic lane and reserves readiness for independent cold-reader evidence. It keeps limited cold reads in the diagnostic lane too. A screenshot packet is acceptance evidence when it is current, independent, and broad enough for the reader to reconstruct the actual visitor movement. It requires viewport composition evidence that supports the designed first encounter through a full, purposeful layout. Direct browser inspection proves live behavior. Screenshot judgment proves composition. Writer review proves the content lane. Style inspection proves the visual world. Independent reconstruction proves visitor understanding. If the site changes after this check, update the model evidence and rerun it.

Repair from the earliest weak link. When reconstruction needs help, return to the router. When the visitor understands the claim and still needs a clearer action path, repair the carrier or information architecture. When the site looks good and still feels generic, repair the world law and visible copy. When desktop works and mobile needs support, repair layout before claiming the story works. When package setup slows inspection, return to the preflight and choose the fastest current inspectable surface. When acceptance mode asks for missing evidence, complete the current acceptance bundle before returning readiness. When validation keeps catching the same issue, move that distinction earlier into routing or component design.

## Return Shape

Return the working URL or file path first. Then give the route decision in plain language. Name the selected Journey Span. Name the Participation Contract. Name the Proof Substrate and carrier. Name the render feasibility path. Name the canonical acceptance model path. Name the acceptance-mode result when it was run. Name the most important validation evidence and any remaining limitation. If acceptance evidence is diagnostic rather than ready, say that plainly and name the next evidence that would complete readiness. If you started a dev server, leave it running only when the user should try it now and include the URL. If the artifact can be opened directly, give the absolute path.

When the user asks for a site, build the artifact. Inspect it. Report what is ready.
