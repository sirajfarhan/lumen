# Concept Visualizer

Turn a concept into a visual model. Input: `$ARGUMENTS`

## One Movement

This skill treats a concept as more than a word. A concept can be a feeling or a social rule. It can also be a scientific construct. It can be a mythic force. It can be a category people use to act with. It can be a system property that keeps reappearing under different names. The output should make that operating shape visible.

The movement is simple. Research the concept from several kinds of evidence. Convert that evidence into a functional model. Compress the model into a small visual story. Then return a prompt, a diagram plan, or a generated image.

Positive-complete framing is a visual-model gate. Name the constructive concept world the image can make available. Each boundary should protect that world. Limits preserve source truth. Exclusions protect target law. Drift-prevention fields protect viewer reconstruction. The positivity gate asks whether prompt and inspection make that concept world clearer for the viewer.

Use this skill when the user gives any concept and wants to see its shape. Also use it when the user asks how a concept appears through culture and language. The same trigger applies to story and myth. It also applies to science, philosophy, and modern systems.

The same workflow should handle a private feeling as well as a public rule or system behavior. A scientific or mythic concept still enters the same path. Treat the name as the starting handle, not as a preloaded visual recipe.

Do not use this skill for a simple dictionary definition unless the user wants a visual model. Do not use it for arbitrary fantasy art when research would not change the result.

## How To Run

Read `references/evidence-model.md` before substantial work. Use `references/concept-model-template.json` as the working shape for the model. Save a filled model when the user wants more than a quick prompt or when an image will be generated.

Set the run profile before filling the model. Most durable runs should use `normal_durable`: enough research and validation to generate a trustworthy prompt, without expanding every branch by habit. Use `quick` only for sketches that will not count as behavior evidence. Use `acceptance` when testing the skill, comparing variants, or responding to a user request for readiness. Use `zero_caveat` when the user asks for `100`.

In `normal_durable`, make one compact decision card before the full model. The card should connect the boundary to the evidence lane that changed L/A/R. It should then tie that choice to carrier law and output mode before naming the prompt risk most likely to damage generation. Expand a branch only when it can change that card. Return from expansion once new evidence would preserve the same model and prompt.

Normal durable should also have a search horizon. Start with the boundary and three to five earned source anchors. One anchor may test language or metaphor. One may test lived practice or culture. One may test theory or mechanism. Add a public or system anchor only when the boundary could change L or R. Browse while the panel can change the decision. Return once the selected L/A/R and prompt risk are stable. If search effort is no longer changing the decision card, mark the lane weak or out of scope and move to the model.

Submit the artifact to Lumen through the bundled client and let the server assess it:

```bash
node runtime/lumen-client.mjs validate_artifact < packet.json
```

Lumen returns the findings and a readiness verdict. Repair from that feedback and resubmit when the artifact changes.

Use expert-research for the evidence standard. Use writer for the final reader-facing explanation and prompt language. Use imagegen when the user wants a bitmap image or when generation is the natural end of the request.

For a quick exploratory answer, you may return a compact model and image prompt without saving files. The same gates still apply. For a durable concept image, create the model JSON first. Validate it. Generate or prepare the image prompt. Then inspect the output.

Start durable models from `references/concept-model-template.json`, then remove inactive placeholder candidates instead of filling dead branches. If a field feels repetitive, make it prove a different failure mode or cut it from the active model. A saved model becomes behavior evidence when the public validator passes or the current regression record names the break.

When an image prompt will be used for generation, run it through writer as its own surface. The prompt needs its own source file and grounding. It also needs a draft and validation artifact. Validate that set before image generation.

Submit the artifact to Lumen through the bundled client and let the server assess it:

```bash
node runtime/lumen-client.mjs validate_artifact < packet.json
```

Lumen returns the findings and a readiness verdict. Repair from that feedback and resubmit when the artifact changes.

The source should contain the concept model summary and the imagegen constraints. It should not duplicate the final prompt as the source. The draft should be the final prompt only. The writer grounding should treat the prompt as a reader-facing control surface for the image model. The prompt is not allowed to become random prompt prose.

Use normal writer validation as acceptance evidence for prompt behavior. The `--skip-substantive` flag may help debug a malformed artifact; keep it outside acceptance. If normal writer validation fails, repair the whole prompt validation set and rerun the public command. If writer returns `PASS WITH REVIEW`, treat that as remaining prompt work for durable behavior unless direct inspection proves the warning is only label syntax and every field body already reads as one causal move.

When the user asks to push readiness to `100`, run in zero-caveat mode. Set the model's `quality_target.target_min_gate` to `100`. A pass-with-review writer result, a caveated image inspection, or any gate below `100` means the run is not done. Repair the model, prompt, or generation and rerun the relevant validator before accepting the surface.

## Fixed Visual Style

Always use the house style: `tangible compressed visual story glyph`.

This is a discipline, not one repeated world. The invariant is that a cold viewer can meet one compressed visual story and understand why it matters. Macro still-life realism is one possible surface, not the style itself. A bounded object event may carry the concept. Another carrier should take over when it preserves the governing cause better than an object would.

## Preserve Intention Through Channels

A strong image can still fail when its channels drift. Color, material, blur, glow, grain, icon style, typography, spacing, scale, citation placement, and background texture all carry meaning whether the prompt admits it or not. Before prompting, build the `intention_to_channel` layer and make every visible channel answer to the story contract.

Start with a four-part story contract: baseline world, introduced change, consequence, and landing or decision. The baseline is what the viewer should treat as already real or established. The introduced change is what becomes different in the artifact. The consequence is what that change does. The landing is the decision, question, or next understanding the viewer should reach. Also name the nearest wrong story, because a good-looking visual often fails by making the wrong comparison feel natural.

Separate story states before assigning style. If the image compares simulation with reality, past with future, proposed with implemented, or evidence with interpretation, each state needs a boundary. Do not let the dream, glow, blur, digital grain, danger color, or documentary realism leak across that boundary unless the story explicitly says both states share it. A treatment that belongs only to the proposed route, simulated half, changed object, risky condition, or evidence layer must stay scoped to that role.

Use a semantic channel ledger. Each channel needs one story owner, one meaning, one scope, one visual treatment, one forbidden leak, and one validation question. If a treatment is exceptional—dreamlike, glowing, blurred, highly saturated, distorted, cubist, mirrored, 3D, grainy, translucent, oversized, or unusually sharp—it must have a named story owner. If it has no owner, cut it. If two channels repeat the same claim, keep the redundancy only when it helps fast reconstruction; otherwise let one channel do the job cleanly.

Budget salience deliberately. The primary story role should own the strongest signal. Background texture should not become more salient than the changed relation. Citations, source notes, legends, and captions should carry trust and auditability without becoming the main explanation. Their layer can be clear and readable while staying visually subordinate through placement, weight, opacity, blur, or container treatment.

For sequence or reveal work, keep a reveal ledger. Each slide or frame should say what is already known, what is newly revealed, what remains held back, which world anchors persist, and what final reconstruction the viewer should be able to make. This avoids unresolved words like “same,” unearned references to earlier slides, and visual beats that change everything at once.

Finish with cold reconstruction questions. A viewer who sees only the visual surface should be able to answer: what is real or already established, what is simulated or proposed, what changed, what evidence supports the claim, and what decision or landing follows. These answers do not need to be written verbatim on the image. They must be recoverable from the channel design.

The image should still feel physically reachable. Even a measured surface or coded artifact should have a material carrier the viewer can recognize. The environment matters too. Natural law can carry story when the viewer can infer its role. Sign logic can carry story when the chosen carrier makes the concept easier to infer.

The style is fixed at the level of story discipline. The presentation dialect is not fixed. The concept chooses the story relation, and the carrier chooses the visual language that can make that relation visible. A measured surface may need the language of information design. A coded artifact may need marks that behave like records. An interface-system field may need a quiet operational surface. These are allowed when they make the concept easier to infer. They fail when they become decorative corporate infographic or generic UI gloss.

Realistic means inferentially believable, not always photographic. Do not build a photographed human scene. Do not turn the concept into a character tableau or documentary still. Build the simplest carrier whose behavior makes the concept easier to relate to. Object-event usually needs material contact. Measured-surface needs comparison made visible. Coded-artifact needs a rule-bound mark. Interface-system field needs operational state made legible.

Choose the representational carrier with the same relevance rule as the story. The best carrier creates the largest correct inference with the least visual effort. Start with object-event as the provisional default, then let the active concept earn the carrier that makes the governing cause visible.

Use one dominant carrier-environment relation. Add another visible unit only when it changes the viewer's inference.

A support object is not earned by plausibility alone. It must make the main event more consequential. If a viewer can name the object but cannot infer why it belongs, remove it or make its force path visible.

Use visual references as calibration. Do not use them as source material. A reference is useful when it changes the next decision. It can sharpen the search question. It can expose an inference failure. It can prove that a richer level earns its cost. It should not hand the final image a recognizable surface.

When references are used, extract the job they performed. Ask what viewer inference became easier. Ask what effort was reduced. Ask what story scale it carried. Ask what would become imitation if copied. Then translate only that job into a new physical event inside the house style. The final image should feel comparable in clarity and depth. It should not feel similar in surface.

Use examples as perspective tests, not as object libraries. A local example earns runtime guidance only when its invariant survives a spread of standpoints. First ask what ordinary use makes visible. Then ask what the target law needs to win. Then ask which nearby concept may steal the carrier. Then ask what the selected world treats as valid evidence. Finally ask how far the consequence has to travel. If the example only works from the original concept's perspective, keep it as regression evidence outside the runtime path instead of teaching it as a pattern.

Holistic expression means preserving the perspectives that change correct inference while making the boundary clear enough that one angle can be read as one angle. When an example teaches a rule, translate the rule through at least one unrelated concept family before writing it into the skill. Relation cases, memory traces, and system topologies may inherit the same perspective discipline while earning their own carriers.

Do not name admired works or artists inside the generation prompt unless the user explicitly asks for a study of that reference. Keep award names out. Keep image URLs and local reference paths out too. The prompt should name the active mechanism and the fixed house style. It should also carry the L/A decision. Reference names belong in the model and validation notes. They do not belong in the image request.

The carrier system must still be common and nameable. The viewer should recognize the visible things before they interpret the concept. A strange material experiment can be physically real and still fail because it asks the viewer to decode the carrier first. Before prompting, write the visible elements as ordinary nouns a cold viewer could name. Replace any hard-to-name part with a more familiar element that keeps the same relation.

Nameability is only the first gate. The object world should also be familiar in action. A heavy thing presses. A queue waits. A gate opens or blocks. A cup fills. A tied thread pulls. A seal closes a record. A path narrows. Do not invent a private machine when a common object or routine can carry the same law. A complex concept should feel newly understandable through a known world, not impressive because the apparatus looks complex.

Before accepting any object system, run the everyday-affordance compression check. Ask which common situation the viewer already knows. Ask what familiar action carries the concept. Ask whether a simpler everyday carrier would preserve the target law. Ask what part would become private machinery if shown to a cold viewer. Choose the simplest known world that keeps the governing cause true.

The whole situation has to be ordinary too. Prove familiarity through one recognizable operating world. A scene made from checkout, workshop, and vending pieces can still become a private apparatus. The viewer should recognize the operating world before interpreting the concept. If the parts need several everyday worlds to make sense, replace the carrier with one known world whose native law already carries the target relation.

For broad system concepts, avoid miniature explanatory machines as the first repair. A tabletop model can make the system look understandable while still asking the viewer to learn a private world. Look first for a lived public routine where ordinary handling changes who gets through and what counts. Use a miniature mechanism only when every simpler lived world would falsify the system law.

Then audit every visible element. Each part needs an everyday reference and a story job. A string is not justified because string is familiar. The viewer should see how the string is tied. They should see what it pulls. Its stress should belong to the whole story. If a material repeats, the repetition should say something. If two roles need separation, material or color should help the viewer separate them. If a detail is beautiful but its everyday action is unclear, replace it or cut it.

Every visible trace also needs visible causality. A mark must look made by something in the physical system. If the viewer cannot infer how it came into existence, the mark is decorative noise. Remove it or show its cause.

Use physical law as story grammar. The viewer already brings everyday physics into the image. Weight pulls. Tension travels. Heat softens. Water stains. Brittle matter breaks. Shadow proves presence. If any such force enters the image, it must help tell the story. A tear should show what loaded it. A bridge should show how it is held. A spill should show the opening it came through. Nothing should feel glued in by the prompt or suspended by private explanation.

The image should carry novel-level compression. It should contain enough causal information for the viewer to reconstruct a full story from one compact scene. Use the smallest visible event that lets the largest true story unfold in the viewer. Richness comes from causal layers in the physical system, not from more objects.

To build that density, use a story movement as hidden scaffolding. Look for a pattern that travels across cultures because it begins from common human pressure. Separation and return can become one physical relation. Wound and repair can become another. A promise tested can become another. Translate that movement into matter and environment without illustrating the story itself. The final image should look like a real physical system that has lived through the same movement.

The story needs stakes. The viewer should understand what future opens if the physical system holds and what future arrives if it fails. A relation may need breakage risk. An obligation may need accumulating consequence. A loss may need ordinary life visibly reorganized around absence. If the system cannot plausibly change the future, the image has mood but no story.

Use a structural scaffold when spatial causality is the fragile part of the run. The scaffold is a disposable control surface. It is not the final image and it is not a diagram for the viewer. It exists to make the shared locus and its support relation inspectable before image generation.

A scaffold may be SVG, HTML, or a compact text contract. Use SVG or HTML when geometry needs inspection or when the available image tool can receive a rendered reference. When the available generator is text-only, translate the scaffold into `Composition/framing` and `Inspection target` instead. Claim pixel-level control only when the scaffold actually entered the image tool as visual input.

Record a scaffold decision in the model. Use it for complex physical systems. Use it when an earlier image failed physical-law inspection. Use it in zero-caveat repair when prompt words alone are no longer changing the structure. Skip it when it would add diagram residue or when the object event is already clear.

Use this exact phrase in every image prompt:

```text
tangible compressed visual story glyph
```

Keep these style drifts out of the prompt unless the selected carrier explicitly earns the permitted version. Avoid decorative corporate infographic, but allow a measured-surface information graphic. Avoid flat vector logo-like simplification, but allow a restrained typographic record when `coded_artifact` or `A5` earns text.

```text
atlas plate / ornate detail / many panels / collage / dense symbols / bare logo / single isolated mark / pure abstract line work / process strip / storyboard sequence / timeline strip / separate stations that do not perform comparison or system propagation / photorealistic people or rooms / anime / cartoon / decorative corporate infographic / cinematic concept art / decorative fantasy
```

For object-event, a warm plain ground and strong negative space often work. Do not export that surface to every carrier. For other carriers, keep restraint but change the presentation dialect. Let only the evidence that changes inference remain visible, and make it meet at one shared locus chosen from the model. The locus should be a specific carrier behavior that the evidence earns, not a stock center point. The before-pressure should press into that locus. The turn should happen through the sign logic the carrier can actually show. The changed state should be visible from that same carrier. Spatial separation is allowed only when comparison, status, or propagation is the carrier's way of telling the story.

Do not let system reach turn into surface memory. L4 or L5 does not automatically mean an electrical board or dashboard. It does not automatically mean a circuit panel, node map, or control room either. Those surfaces are valid only when the current concept's world law needs operational state, signal response, or mediated control. If another carrier would make the viewer more correct, choose that carrier instead. A system image should feel like this concept's world becoming visible, not like the last successful system example returning with a new label.

Use this presentation map when prompting.

```text
object_event: restrained material still life; photographic or realistic object behavior is allowed.
trace_field: sparse residue surface; forensic, archival, rubbing, imprint, scan, or negative-space treatment is allowed.
measured_surface: information-design surface; charts, grids, axes, scale marks, contour lines, limited labels, numbers, and clean typography are allowed when they measure the root relation.
path_space: cropped environment; threshold, route, map-like ground, passage, access, and repeated path evidence are allowed.
coded_artifact: record surface; forms, stamps, seals, names, tags, ledgers, marginalia, and short text are allowed when code or status changes the object.
interface_system_field: operational surface; signal panels, dependency maps, dashboards, controls, gauges, latency fields, and feedback diagrams are allowed when they show system state.
```

When the user asks for a specific visual category, treat that as a presentation-dialect request. That category might be an infographic or a poster. It might also be a UI or a typography-led surface. Test whether it should become the selected R-mode. If the model rejects that request, state why in the model. If it accepts it, put that visual category early in the image prompt before material detail. Image models often obey the strongest medium cue. The intended surface must appear before any pull toward `macro material realism`.

This is the visual equivalent of relevance-guided semantic compression. The image should create the largest correct story with the least visual effort.

Default to one holistic physical system. The viewer should meet one image whose present state already contains the story, not a staged reading path. When the work genuinely needs several images, do not put several frames inside one image. Build separate lawful images that share one carrier law and one causal thread.

## Choose Story Reach And Visual Concreteness

When the user asks for a different amount of detail, do not treat that as one slider. First ask whether the story should travel farther. Then ask whether the same story should become more or less visually concrete.

The user-facing words are simple.

```text
Story reach: how far the concept's consequence travels.
Visual concreteness: how explicitly the same story is shown.
```

The internal model uses sharper names.

```text
Consequence radius: L0 through L5.
Representational articulation: A0 through A5.
```

Think of the two axes as two different questions.

```text
L asks where the consequence goes.
A asks how much evidence the viewer gets.
```

The same root story can move on either axis. If a cracked cup is the root story, L0 may show only the wet ring it left. L1 may show the crack touching the water. L2 may show the cup held together just enough that its next moment matters. L4 may show the same repair becoming a shared keepsake or public record. Those are reach changes.

A changes something else. It starts with trace evidence and moves upward in response to one viewer failure at a time. If relation is missing, show relation. If identity is missing, show the carrier object or surface. If force is missing, show material behavior. If domain is missing, show use context. If convention is missing, let an inscription act inside the selected carrier. The consequence stays the same while the viewer receives stronger evidence.

Choose story reach before choosing visual concreteness. Then choose the lowest visual concreteness that lets a cold viewer reconstruct the selected story reach. A higher visual concreteness is a repair for a specific inference failure, not a reward for wanting a richer image.

### Story Reach

Default to L2. L2 is the house-style baseline because it shows one physical event and the future it changes. Move below L2 only when the concept truly needs only a trace or a causal contact. Move above L2 only when the added world makes the same root story more correct for the viewer and keeps root retention high.

When the concept lives through propagation, test L5 as the first serious challenger to L2. Look for the moment a proxy or rule begins to steer the field it was meant to describe. Also look for a bottleneck whose effect travels downstream and returns as new pressure. Choose L2 for that kind of concept only when the user explicitly asks for a local single-event metaphor or the working boundary says the propagating ring is out of scope.

When the concept needs public carrying, test L4 as the first serious challenger to L2. Look for the point where a private event becomes held by others. It may be witnessed or recorded. It may be taught or enforced. It may be remembered as part of a shared order. Choose L2 for that kind of concept only when the user explicitly asks for a private object story and the model names the public ring it is excluding.

When L5 wins because pressure returns, branching is not enough. The viewer should see how the downstream change comes back as new pressure on an input. If the generated image only fans outward, treat loop closure as partial and repair before calling the system story ready.

Use this level map.

```text
L0: trace. The story stops at residue. A cold viewer asks what mark remains.
L1: contact. The story reaches the acting relation. A cold viewer asks what touched what.
L2: consequence. The story reaches the next moment. A cold viewer asks what happens now.
L3: practice. The story reaches repeated use. A cold viewer asks what people keep doing because of it.
L4: carrier. The story reaches shared memory or rule. A cold viewer asks what public field carries it.
L5: system. The story reaches propagation. A cold viewer asks what downstream world changes and returns pressure.
```

For a normal durable model, screen all six levels but record only the selected level and the nearest competitor. Add the public or system challenger when it could change the decision. Fill all six candidate entries for acceptance work. Fill them for zero-caveat work too. Fill them for an explicit axis test or for a close contest where the runner-up could plausibly win. The selected level should win by relevance rather than admiration. A richer candidate loses when viewers remember detail but lose the root event. A sparse candidate loses when viewers can name a mark but cannot say what future changed.

Use the score as a judgment aid.

```text
relevance = correct story scope * accuracy * root retention * consequence strength
cost = effort + ornament penalty + text-rescue penalty + flatness penalty + parallel-story penalty
winning level = largest correct story that pays the lowest honest cost
```

Record the automatic choice in `selection_rule_check`. For L3 through L5, the added scale should beat the closest smaller level by at least fifteen percent and preserve root retention. For L0 or L1, the decision note should prove the concept only needs trace or contact.

When a system concept stays at L2, the decision note must prove the boundary, not just praise the cleaner image. It should say what system ring was deliberately excluded and why that exclusion serves the user's request. A beautiful local metaphor is a failed automatic choice when the broad concept lives through propagation.

When a public or ritual concept stays at L2, the decision note must prove the private boundary too. A private L2 model is valid only when the narrower boundary is explicit and the model names the public carrier it is deliberately excluding.

Keep the style fixed across levels. L0 can be bare, and L5 can be systemic, but both should still feel like a tangible compressed visual story glyph. The concept changes the consequence radius. It does not change the design system.

Use the cover test for hierarchy. Cover the added layer and the root story should still read. Cover the root and the added layer should lose its reason to exist. This asymmetry keeps the image nested rather than assembled.

Carry the selected story reach into the image prompt through its visual job, not through the level code. A trace prompt should speak in residue. A contact prompt should speak in acted relation. A system prompt should speak in propagation and feedback. Keep internal level codes inside the model.

### Visual Concreteness

After choosing story reach, choose how explicitly the image should show that same story. The A-axis does not change the story scope. It changes the amount of visible evidence the viewer receives.

Default to A2. A2 is the house-style center because it gives nameable objects and a visible consequence without turning the image into a scene or explanation.

Use this articulation map.

```text
A0: trace evidence. The viewer receives residue or absence before the object story is fully shown.
A1: relation evidence. The viewer receives simplified objects and force direction.
A2: object evidence. The viewer receives a minimal nameable object relation.
A3: material evidence. The viewer receives enough matter, contact, and force behavior to trust the event.
A4: use-world evidence. The viewer receives a cropped context that explains why the object matters.
A5: inscription evidence. The viewer receives text, number, name, tag, or record as a physical actor.
```

Move toward A0 or A1 when the user wants more abstraction and the root relation can survive with fewer cues. Move toward A3 when viewers can name the objects but miss the physics. Move toward A4 when viewers understand the event but not the domain or use-world. Move toward A5 only when conventional text or numbers are part of the concept's operation.

For a normal durable model, record the selected A-level and the nearest lower or higher challenger. The decision should name the viewer failure that moved the model away from A2. Fill all six A-candidates for acceptance work. Fill them for zero-caveat work too. Fill them for explicit A-axis testing or for a close contest. The point is to preserve the distinction rather than spend attention restating obvious losses.

Do not expose `representational articulation` unless theory language helps the user. Speak in the user's natural terms, then record the precise A-level in the model.

The A-level should never create a second story. A4 context should stay cropped around the root event. A5 text should live on a physical object as a working mark in the scene. No floating captions. No poster slogans.

Use the text-off test for A5. Cover every word. The root event should still be inferable. Uncovering the text may sharpen the domain, but it must not create the story from scratch.

Carry visual concreteness into the image prompt through the evidence the viewer should see, not through the articulation code. If the model selected relation evidence, ask for the relation. If it selected material evidence, ask for force behavior. When inscription evidence earns text, choose the exact scene-native mark that acts physically. Keep internal level, articulation, and carrier labels inside the model.

For A0 through A4, text-like marks are only world residue. They may be illegible or short scene-native marks when the carrier would naturally contain them. They may not become readable prose. A sentence on a ledger that explains the concept is an accidental A5 and should be rejected even when the record carrier is otherwise right.

Before prompting, write the combined decision as one sentence.

```text
This image uses L__ because the consequence must travel to __.
It uses A__ because the viewer needs __ visible evidence, but no more.
```

If that sentence sounds interchangeable between levels, the levels are not clear yet. Repair the model before generating.

When the user specifies an L or A value, treat it as a controlled variant rather than an automatic winner. Still compare the full ladder. Record the nearest automatic choice. Then say which larger or smaller story is being deliberately excluded so the requested level stays honest.

For a 100-ready image, every material event must earn its place on first inspection. Reject residual symbols that a cold viewer may read as the old cliché before reading the model. Also reject pretty abstractions where the viewer cannot tell what is physically happening. For each run, derive the stock-symbol risk from the active concept and put it in the model's avoid list before prompting. Do not let examples from earlier tests become a permanent object library.

## Choose Representational Carrier

After choosing L and A, choose the representational carrier. This is the R-mode. It decides what kind of external thing can honestly carry the selected story at the selected evidence level.

Use this user-facing translation when needed.

```text
Representational carrier: the kind of visual world or surface that can carry the concept without distorting it.
```

The internal name is sharper.

```text
R-mode: the representational carrier that makes the governing cause easiest to infer.
```

Start with `object_event`. Move away only when another carrier preserves the governing cause with less distortion. This is the least-upgraded-carrier rule. It keeps the skill visually broader without turning surface novelty into a reward.

Use this carrier map.

```text
object_event: a bounded material event read through direct perception, pressure, binding, breakage, exchange, concealment, or repair.
trace_field: residue, absence, wear, imprint, scar, remaining marks, or distributed remnants read as indexical evidence.
measured_surface: comparison, route, topology, threshold, proportion, flow, cluster, or distribution made visibly comparable.
path_space: passage, threshold, access, exclusion, crossing, descent, return, proximity, or movement through a structured place.
coded_artifact: document, record, list, seal, signature, token, offering, ritual object, status mark, or rule-bound handling protocol.
interface_system_field: monitored state, feedback loop, capture field, latency, threshold, dependency stack, control surface, or mediated system.
```

The carrier should be chosen by pressure, not by taste.

```text
Residue pressure points toward trace_field.
Comparison pressure points toward measured_surface.
Passage pressure points toward path_space.
Code pressure points toward coded_artifact.
System pressure points toward interface_system_field.
Local material-cause pressure points toward object_event.
```

When several pressures appear, choose the least upgraded carrier that keeps the main cause visible. A richer carrier loses when it adds style but does not improve cold-viewer inference. Object-event loses when it makes a broader concept falsely private.

Before approving the carrier, run the dominant-native-reading check. Ask what the chosen objects or surfaces would suggest before the target is considered. The answer should come from ordinary use, not from the research notes. Native readings are not forbidden. They become failures when they beat the target law. Keep the carrier only when one visible counter-cue makes the target reading stronger than the carrier's default story. If no such cue exists, choose a different carrier.

Then run the semantic-attractor veto. Some carriers do not merely suggest a neighboring concept; their ordinary function already gives the viewer a stronger answer. When that happens, treat the carrier as hostile until proven otherwise. Keep it only when the target cue is larger, simpler, and easier to see than the carrier's native function. If the viewer can name the carrier's usual job before seeing the target relation, and the target depends on a small trace or private explanation, replace the carrier.

For relational concepts, run one extra disambiguation pass. A relation is often stolen by the neighboring action that is easiest to name. The image may read as protection or dependence before it reads as the target. It may also read as control or repair. Make the target relation win by showing its moral or practical asymmetry through world-native evidence. The viewer should see how the relation began, not only what is being held now. The target-side trace should show the exact reason the relation began. That reason may be exposure. It may be permission. It may be obligation. It may be injury or recognition. The accountable side may be a holder. It may be a rule. It may be a counterparty or field. It must make keeping or failure imaginable from the same pixels. If that asymmetry cannot appear without labels, the carrier is not yet strong enough.

R-mode is separate from L and A.

```text
L asks how far the consequence travels.
A asks how much visible evidence the viewer gets.
R asks what kind of carrier can bear that consequence at that evidence level.
```

A high A-level means different things in different carriers. In object-event, higher A may mean more material causality. In trace-field, it means more specific residue. In measured-surface, it means more explicit evidentiary relation. In path-space, it means clearer movement cues. In coded-artifact, it means more legible rule or status logic. In interface-system field, it means more visible operational structure.

Record R-mode as a structured decision in the model. In a normal durable run, compare the selected carrier against object-event and the nearest non-default challenger. Fill every carrier candidate for acceptance work. Fill them for zero-caveat work too. Fill them for explicit R-mode testing or for a case where object-event might falsely privatize the concept. Fill these fields before prompting.

```text
default_mode / selected_mode / dominant_carrier_pressure / runner_up_pressure
why_object_event_fails_or_survives / primary_sign_logic / selection_reason
least_upgraded_carrier_check / l_axis_interaction / a_axis_interaction
presentation_dialect / medium_permissions / style_delta_from_object_event
carrier_specific_evidence_obligations / non_transfer_constraints
prompt_transfer_instruction / validation_focus / validation_questions
candidate_modes object_event through interface_system_field
```

The primary sign logic should name what does the first inferential work. Use the sign family the carrier can actually show. Do not make the image rely on a sign relation the carrier cannot support.

Carry the representational carrier into the image prompt as both an inferential instruction and a presentation instruction. Do not write "make it feel memorial" or "use dashboard vibes." Write what the carrier must make easier to infer, and then give the image model the matching medium cue. A measured-surface prompt should make comparison feel like the surface itself. A coded-artifact prompt should let record marks change how the object is read. An interface-system prompt should let operational pressure appear as a system surface when that is the best carrier. Do not put carrier slugs or `R-mode` language into the generation prompt.

Validate the carrier before judging beauty. Ask whether the chosen carrier revealed the governing cause better than object-event would have. Ask whether the intended sign logic actually did the work. Ask whether a public or systemic concept stayed public or systemic. Ask whether reference surfaces stayed quarantined. Ask whether a cold viewer can infer the cause or sign relation without a caption. Also ask whether the generated image visibly changed presentation dialect when the selected carrier was not object-event. If every result still looks like the same macro still-life, the carrier transfer failed. If every system result becomes the same electrical or operational board, the carrier transfer failed in the opposite direction. Either failure can happen even when the model JSON passes.

## Lock Carrier Law

After choosing R-mode, lock the world law before prompting. Use the plain label `world coherence` when speaking to the user if that is clearer. In the model, use the sharper construct `carrier-law coherence`.

This layer asks whether the chosen carrier behaves like a believable representational world. It is not lore, ambience, or cinematic worldbuilding. It is the rule by which evidence can exist inside the image.

A physical object event is governed by matter under constraint. A trace field is governed by residue that a past action could have made. A measured surface is governed by comparison that can be checked. A path space is governed by movement through access and obstruction. A coded artifact is governed by a rule that gives marks social force. An interface-system field is governed by state changing through response.

For every durable model, fill `visual_model.carrier_law_coherence` before writing the image prompt. The field should let a future agent say what world this is. It should also say what law runs it. Then it should make clear what evidence belongs there and what would break the world.

The viewer role matters because proof changes with the role. A witness to matter needs force made visible. A record reader needs validity. A chart reader needs comparison. A system user needs state and response.

Use only world-native evidence. The image should not place meaning on top of the carrier. It should show what the carrier could naturally produce. A stain must have a source. A registry number must affect record identity. A disabled control must imply state or permission. A threshold must change what can pass.

Match the truth criterion to the carrier. Object-event needs material credibility. Trace-field needs contact credibility. Measured-surface needs comparative credibility. Coded-artifact needs documentary or procedural credibility. Interface-system field needs operational credibility. A beautiful carrier fails when it borrows the look of a world without obeying that world's proof standard.

Run the carrier-law gate after generation. First ask whether a cold viewer can name the carrier-world before naming the concept. Then ask whether the viewer can state the internal law and stand in the right role. The image should offer at least three law-bearing cues and no cue that is illegal under that world. If that fails, repair the world law or regenerate before judging style.

When testing L and A, freeze the carrier law. Vary L only by changing how far consequence travels. Vary A only by changing how much law-bearing evidence the viewer receives. If the witness role or proof standard changes, the run is no longer testing L or A. It has changed worlds.

## Decide One Frame Or Sequence

One frame remains the default. Use one frame when one lawful carrier-world can license the indispensable inference. Text may name or lightly orient the image, but the frame must still do the story work.

Escalate to visual sequence architecture only when the story needs more than one necessary viewer-model update. More material is not enough. A sequence earns itself when one co-present frame would make the state change dishonest or overload the carrier law.

A sequence is not a storyboard strip inside one generated image. It is a set of separate images held by one source of truth. Each image should still be a tangible compressed visual story glyph. Continuity lives in the shared law and in the identities or states that must survive the cut.

Before generating a sequence, fill `visual_model.visual_sequence_architecture`. Name the output mode as `one_frame`, `multi_image_sequence`, or `asset_first_sequence`. Then make the decision inspectable. Say why one frame is or is not enough. Say what the visual spine is. Say what text may do. Say what continuity must survive and what would collapse the plan back to one frame.

Treat sequence continuity as world continuity, not style matching. The world bible should be small but strict. It binds the run to a recurring carrier. It also fixes the material and camera convention before naming which state may change. A sequence can change scale, crop, or surface only when the same carrier law still governs what counts as evidence. If the images merely share a look, the sequence has not preserved a world.

The visual spine is the smallest chain of state changes the viewer must understand. Each beat should earn one update in the viewer's model. A beat can establish the world. It can reveal a hidden relation. It can cross a threshold or stabilize a consequence. It can also change the interpretation. If removing a beat does not remove a required update, delete the beat or collapse it into text.

Use beat roles only as production control. An establisher identifies the world and players. An initial beat presents the condition or tension. A peak beat shows the decisive change. A release beat stabilizes the consequence. Bridge, callback, and repair beats are allowed only when they preserve necessary continuity or correct a law break.

Each beat needs a fixed part and a changed part. The fixed part proves the viewer is still inside the same world. The changed part earns the new image. If a beat cannot name both, it is probably doing caption work or making a mood variation instead of story.

Divide text and image by what each can do honestly. Images should carry visible state and lawful evidence. Text may carry time compression or off-frame linkage. It may also name a scope shift when the image cannot do that economically. Text must not rescue an image that failed to show the carrier law.

For generated storyboards, treat recurrence as the default pressure. If a cold viewer must believe every image belongs to one continuing world, choose `asset_first_sequence`. That world may be a physical scene. It may be a record surface. It may be a measured or operational surface such as an interface. Use `multi_image_sequence` for prompt planning, quick probes, or loose series work only when identity drift would not damage the story.

Asset-first production creates the world before the beats. Build only the asset pack that can hold continuity. The world asset fixes the recurring carrier. The topology or shot asset fixes what may not move. Each state-delta overlay changes only the beat's earned variable. That overlay must look caused by the carrier rather than drawn on top as explanation. The material-light-camera lock protects the universe from drifting. The reference-use boundary says whether assets will enter the image generator as references, edit targets, or inspected scaffolds.

Claim asset-level preservation when the asset actually enters the image tool. When the available generator is text-only, still make the asset pack as a scaffold and state the limitation in `reference_input_plan`. The beat prompts should inherit the asset pack and describe the visible state change. Keep each beat inside the same established universe.

Asset-first still needs a visible beat. The state delta should be readable when the images are placed side by side at normal review size. If the same-asset test only proves that nothing drifted, the sequence has protected the world but lost the story. Strengthen the overlay or beat prompt until a cold viewer can point to what changed without reading captions.

After generating a sequence, inspect against the asset pack before any external reverse-story validation. First ask whether the same carrier still lives in the same topology. Then ask whether the material family and lighting convention still serve the same proof standard. The creator should record a validation target and fail conditions, but it should not perform the blind reconstruction itself. Those fields are a handoff contract, not proof. When the run is being validated, give the images to a cold evaluator without captions or process notes. Ask the evaluator to tell the story in order and explain why the same world changed. The sequence passes behavior validation only when the evaluator recovers the root story through the beat order inside one coherent world. If the evaluator needs text to understand causality or notices only matching style, repair the asset pack first. Then repair the world bible and beat prompts before regenerating.

Collapse back to one frame whenever the added images repeat the same inference with different symbols, break the carrier law, or create a slideshow of related moods. A strong single lawful state is better than several weak adjacent pictures.

## Preserve Intent Across Iteration

Initial creation and revision are different operations. An initial run may explore a world. Once the user approves any part of an artifact, later work becomes configuration-managed revision. The approved artifact, not the image model's latent memory and not the newest reference, becomes the system of record.

For every revision, fill `iteration_control` before prompting. Start by naming one authoritative baseline and its approval scope. Approval can protect the whole artifact or named properties such as world identity, semantic relation, spatial correspondence, palette, material law, typography, or negative space. A later candidate cannot silently replace that baseline. Rebaseline only after explicit approval and record what the new version supersedes.

Compile the user's feedback into one typed change set:

```text
mutate: what must visibly change
protect: approved properties that must remain perceptually equivalent
forbid: changes or reference influences that would break the intention
open: choices the generator may explore
success tests: observable evidence that the requested delta happened
regression tests: observable evidence that protected state survived
```

Do not treat silence as permission to rewrite. When feedback is ambiguous, choose the narrowest interpretation consistent with the request. Ask one ordinary question only when two plausible interpretations would alter different protected properties and a cheap candidate cannot safely reveal the difference.

Keep a semantic transcript and a layout transcript. The semantic transcript states the relation, roles, causal direction, and nearest wrong reading without relying on style language. The layout transcript states attention order, correspondence, negative-space ownership, and actual viewing scale. Cross-link them so each central meaning claim has visible spatial evidence. This prevents a composition from looking beautiful while telling the wrong story, or telling the right story only in the creator's notes.

References receive property-scoped authority. For each reference, state what it may influence and what it must not influence. A material reference may govern grain and flow while being forbidden from changing city identity or layout. A composition reference may govern balance while being forbidden from donating its objects, palette, or recognizable surface. When several references disagree, production authority resolves the conflict property by property.

Assign production authority explicitly. The approved baseline normally owns world identity, semantic relation, and protected geometry. The selected generator may own only the open material or appearance properties. Deterministic composition should own exact typography, alignment, and export whenever the image generator cannot preserve them reliably. No property should have two silent owners.

Choose the least destructive operation that can satisfy the change set. Prefer, in order, a bounded regional edit, geometry or spatial edit, material or appearance edit, deterministic typography or composition, global recomposition, carrier reset, and full semantic rebuild. This is a risk order, not an absolute command. If repeated local edits contaminate protected state, stop patching and reset from the approved baseline with the same bounded change set. Keep the private repair budget between one and five attempts.

Use the exact machine values below in both `change_set.operation_class` and `operation_decision.selected_operation`:

```text
regional_content_edit / geometry_spatial_edit / material_appearance_edit /
typography / deterministic_compose / export / global_recomposition /
carrier_reset / semantic_rebuild
```

Every candidate needs lineage and lifecycle state. Use `diagnostic` for a probe, `candidate` for something worth comparison, `presented` for something the user may judge, and `approved` only after explicit approval. Never present a candidate merely because it is the latest attempt.

Admission compares candidate and baseline side by side. Test requested change and protected state separately. Inspect the artifact at actual presentation size as well as detail scale. Use deterministic checks for measurable breakage, machine proxies only as warnings, an independent artifact reader for semantic reconstruction, and the user for preference and approval. Automated checks may reject or prioritize; they cannot prove audience understanding. Keep semantic fidelity, edit locality, identity, material law, composition, user control, efficiency, and transfer as separate constructs rather than collapsing them into one score.

For an initial run, keep `iteration_control.mode` as `initial`; do not manufacture an approved baseline. The first strong candidate becomes a baseline only when the user approves it. For revision, sequence revision, or finalization, the baseline, change set, authority map, comparison, and admission evidence are mandatory.

## Scope The Concept

Start with the concept and the audience. Then name the requested surface and the consequence. The same concept changes shape when the user wants a personal image instead of a philosophical diagram. It changes again for a brand visual, a research-backed art piece, or a mythic poster.

If the concept is broad, choose a working boundary and state it. Ask a question only when the answer changes the evidence set or protects against a serious mistake. Otherwise proceed with a reasonable scope and mark uncertainty in the model.

Keep three layers separate at first. One layer is the word people use. Another layer is the lived pattern people enact around it. The third layer is the account that explains what the concept does inside minds and bodies or inside groups and systems. The visual model should come from the relation among those layers.

For zero-caveat work, narrow the boundary until every evidence lane can be supported without overclaiming. Universal models of broad concepts almost always leak. A bounded model can earn 100 when every source claim has conditions and the image carries only that bounded relation.

## Research The Evidence

Research only the lanes that can change the model. Use current web research when scholarship is live or a source needs verification. Prefer primary scholarship and expert synthesis over unsourced summaries. Museum sources, archives, and reputable translations are useful when the concept passes through old objects or stories.

Language and metaphor asks what the word lets people imagine. Look for idiom and etymology. Also look for semantic neighbors, translation gaps, and image schemas. If an idiom gives the concept a bodily geometry, make that geometry testable. Falling implies gravity. Carrying implies load. Burning implies heat. Being inside something implies containment.

Culture and behavior asks what people do around the concept. Look for the action that repeats. It may be ritual. It may be obligation. It may be taboo or repair. It may show up as exchange, sanction, or social distance. Behavior often gives the image its bodies.

History, story, and myth asks what older narratives made visible. The lane can include epics and deities. It can also include personifications and religious images. Literature can matter when it changes permitted feeling. Legal codes, medical models, and older norms can change permitted action. A god or story matters when it shows how people imagined the concept acting on the world.

Scientific and theoretical accounts ask how the concept functions. The right lane may come from psychology or cognitive science. It may come from anthropology or sociology. It may come from economics or systems theory. Philosophy can explain one part of the operation. Linguistics can explain another. Law, design, and computation can also matter. Choose the theory because it explains operation.

Modern systems asks how the concept is measured or governed now. Law and markets can reveal the current machinery of a concept. So can organizations and medicine. Education can expose the same machinery from another side. Media, software, and infrastructure can do the same.

Every important source card should preserve the claim. It should also preserve the condition where the claim applies, the qualification of the source, and the visual implication. A weak lane needs a reason. Let active lanes earn their place by changing the model.

Preserve cultural specificity. Compare because comparison changes the model. When sacred stories or living religions enter the model, preserve specificity. Apply the same care to caste and race. Apply it again to gender, trauma, and colonized traditions.

## Build The Functional Model

Synthesize the evidence into a concept engine. The model should answer what the concept does.

The template names the functional fields that need attention.

```text
core_relation / forces / agents / boundaries / transformations / feedback_loops / time_depth / tensions
```

Use each field to catch a different failure mode. The best model usually has one pressure-bearing relation that orders the rest.

For any concept, do not stop at the first metaphor. Let language propose a geometry. Let behavior show what people repeat. Let older stories reveal what the concept is allowed to do. Let theory explain the operation. The carrier system should come only after those lanes have either strengthened or challenged the first visual intuition.

## Compress Function Into Visual Story

Decide the smallest story path before writing the image prompt. The visual grammar should follow the functional model, not the first symbol that comes to mind.

Use the grammar fields in the template.

```text
spatial_structure / shape_language / material_texture / motion / scale / color_light / symbolic_rules / avoid_list
```

Also fill the compression fields.

```text
primary_relation / viewer_inference / omitted_evidence / minimality_rule
```

Also fill the story fields.

```text
before_pressure / turning_action / after_change / fusion_locus / evidence_echoes / story_read_path
```

Also fill the scaffold decision. Even a skipped scaffold should say why the direct prompt is enough. A used scaffold should name the artifact path or the text contract, then say how its structure enters the final prompt.

Also fill the level framework. It is the automatic story-reach selector and the hierarchy check.

```text
selected_level / selection_reason / root_story_sentence / allowed_added_layer
lower_level_miss / higher_level_risk / selection_rule_check / nested_cover_test
candidate_levels L0 through L5
```

Also fill the articulation framework. It records how concrete or explicit the visual surface should become without changing story reach.

```text
selected_articulation / selection_reason / inference_failure_solved
what_it_adds_visually / what_it_must_not_add / text_policy
abstraction_risk / realism_detail_risk / candidate_articulations A0 through A5
```

Also fill the representational carrier framework. It records what kind of visual world or surface can carry the selected story without distorting the governing cause.

```text
selected_mode / dominant_carrier_pressure / why_object_event_fails_or_survives
primary_sign_logic / least_upgraded_carrier_check / l_axis_interaction / a_axis_interaction
carrier_specific_evidence_obligations / non_transfer_constraints / candidate_modes
```

Also fill the perspective-holism check. It records which standpoints are necessary for the image to feel whole rather than narrow.

```text
ordinary_viewer_perspective / target_law_perspective / nearest_confusion_perspective
carrier_world_perspective / consequence_scale_perspective / example_transfer_check
```

Also fill the carrier-law coherence framework. It records whether the selected R-mode has become a lawful world rather than a look.

```text
carrier_world / internal_law / viewer_role / admissible_evidence
truth_criterion / affordances_or_constraints / consequence_closure
coherence_breakers / earned_detail_budget / lawfulness_test
```

Also fill the visual sequence architecture. It records whether the output should remain one frame or become separate images.

```text
output_mode / decision_reason / one_frame_sufficiency_test / escalation_trigger
visual_spine / collapse_back_to_one_frame_test / text_image_labour
continuity_dossier / beat_plan / asset_first_plan / validation_questions
```

Use example vocabularies only when the choice is earned by the model.

```text
relation: containment / crossing / pull / balance / rupture / orbit / tether / threshold / reversal
material cue: thread / stone / water / flame / glass / shadow / line / weight / membrane / light
material-real cue: handmade paper / thread / glass / metal / rust / wax / clay / ceramic / wood / cloth / water / salt / ink / stone / magnet / mirror / light through matter
```

Make the concept legible without turning every image into an infographic. But when `measured_surface` wins, do not hide that decision inside a still life. Let the earned surface behave like information design. When `interface_system_field` wins, do not hide the system inside one prop. Let the earned surface behave like an operational field. Use text only when text is part of the selected carrier. If the prompt needs many objects to explain the concept, the model has not compressed enough. If the prompt has no visible turn, it has compressed too far. If sequence or propagation is not the carrier's own evidence, fold a horizontal before-to-after strip back into one locus.

## Generate Or Return The Prompt

Write the image prompt in the canonical prompt contract. Keep the labels and order stable. Aim for a compact prompt that an image model can follow in one read. For one-frame work, 120 to 165 words is usually enough. A longer prompt must earn its length by preventing a known generation failure.

```text
Use case:
Asset type:
Primary request:
Concept engine:
Visual story:
Style/medium:
Composition/framing:
Evidence echoes:
Constraints:
Avoid:
Inspection target:
```

Keep one blank line between prompt fields. The label is control syntax. The body of each field should be one causal move, not a comma inventory. The `Avoid` field should reject one family of wrong readings rather than naming a shelf of forbidden objects. `Evidence echoes` should bind support detail to the main event instead of listing materials. `Inspection target` should say what the cold viewer reconstructs, not repeat every visible noun.

A writer warning about prompt-field density is usually a true signal that the image model is receiving coverage instead of story pressure. Treat canonical labels as structure and repair the field bodies first. A durable benchmark should aim for clean writer `PASS`; a reviewed pass is regression evidence unless the validation artifact names the warning and direct prompt inspection shows no list-shaped body remains.

When a prompt field needs materials, bind each material to its job in the event. Replace bare material rows with a force relation. The thread carries tension. The wax records pressure. The shadow proves contact. The prompt can name several visible things, but each one should make the image model preserve causality rather than merely add texture.

Before validating the prompt, do a prompt-shape repair pass. Fold `L`, `A`, and `R` into one mechanism sentence instead of naming them as a row. Replace `before, turn, after` wording with the physical action that lets the viewer infer sequence. In `Avoid`, name the wrong reading to prevent instead of dumping every forbidden object. A compact prompt can still be strict, but the strictness should arrive as causal pressure.

Then do a presentation-dialect pass. The `Use case`, `Asset type`, and `Style/medium` fields must match the selected carrier. If `measured_surface` is selected, one of those fields should name the earned design surface. If `coded_artifact` or `A5` is selected, the prompt should permit the exact text or typographic role that carries the code. If `interface_system_field` is selected, the prompt should permit operational interface grammar when that is the chosen surface. Let the selected carrier govern the surface more strongly than `macro material realism`, `warm plain ground`, or a familiar handmade object palette.

When the carrier is a record-world and A5 was not selected, put the text boundary inside the prompt. The image may use the mark that the world needs to act, such as a date or a filing tick. It should reject readable explanatory sentences and prose inscriptions.

If the user wants a final image, use imagegen after the model and writer prompt artifacts pass validation. Prompt the image as one restrained symbolic story. Include the concept engine, the L/A/R decision, and the house style. Keep source evidence out of the visible scene unless one source directly changes the story. Ask the image to make the model visible through a clear turn at one shared locus.

If the sequence architecture selects `multi_image_sequence` or `asset_first_sequence`, write one canonical prompt per beat in `image_prompt.sequence_prompts` and generate separate images. Keep `image_prompt.final_prompt` as the key image prompt or the first generated image prompt so the single-image validator still has a concrete surface to inspect. Validate the sequence prompt set with writer as a prompt surface. Then inspect continuity across the generated images.

Each beat prompt must say that it produces one separate image only. Carry the same world bible into every beat prompt through ordinary visual language, not internal codes. Make fixed identity and visible state change explicit enough for inspection. Keep internal level codes, carrier codes, and production labels inside the model.

If the user wants a prompt only, return the brief model with the final image prompt. Include the avoid list. Add a variant only when it represents a genuinely different model.

When generating the image, inspect it directly. Check whether the result carries the model or only looks atmospheric. If the image shows generic symbolism, revise from the functional model.

Before treating a generated image as behavior evidence, run the prompt-bundle sync check. The current attempt must form one chain. Writer source feeds grounding. Grounding feeds draft. Draft feeds validation. Validation approves the final prompt. The final prompt produces the generated image. Accept a folder only when the current model points to the exact chain that produced the image. Stale prompt grounding is a current-version failure because the path from model to image cannot be audited.

Run the everyday-affordance check before nameability. Ask whether the world is one a normal viewer already knows how to operate or observe. A part can be nameable and still fail because the connection between parts is a custom invention. If the viewer must learn the apparatus before learning the concept, the carrier is too private. Repair by moving to a simpler known routine or by reducing the system until each connection is familiar.

Also run the nameability check on the generated image. A strong image lets the viewer name the real objects before asking what they mean. If a visible part looks ambiguous or too specialized for ordinary recognition, reject the image even when the model and prompt validators pass.

Run the carrier check before the beauty check. Ask whether the selected R-mode made the governing cause easier to infer than object-event or the nearest competing carrier would have. If the chosen carrier only changes the look, reject it. If a public or systemic concept became private again, reject it.

Then run the carrier-law check. Ask whether the generated surface obeys the selected carrier-world's internal law. The viewer should be able to identify the world and state the law. They should also find law-bearing evidence without finding an illegal cue. If the result looks good but the evidence could not naturally exist inside that carrier, reject it.

Run the reference independence check whenever references shaped any part of the work. Compare the result to the reference job rather than the reference surface. Pass only when the generated image is a new carrier event or structure that earns similar inference power while leaving the recognizable reference surface behind.

Then run the causality check. For every visible trace, ask what object made it and whether that cause is visible or strongly inferable. If the answer depends on the notes, reject the image.

Then run the physical-law check. Follow the force path from support to change. Ask where the force enters. Ask how it travels. Ask how matter responds. Ask what the environment proves. If any attachment or change feels magical, reject the image.

When a prompt depends on consequence under force, inspect the support path. A generated image fails the story if an accidental support carries the burden that the chosen relation was supposed to carry. The visible law should make failure possible and make the chosen relation matter.

Then run the scaffold check. If a scaffold was used, compare the generated image against the scaffold's real job. It should preserve the event structure without looking like a wireframe. If no scaffold was used, ask whether the direct prompt made the structure clear enough. A skipped scaffold fails when the image still contains an unexplained physical event.

Then run the story-density check. A cold viewer should infer a deep before, a consequential turn, and a changed after from the selected carrier alone. If the image has only a mood or unexplained trace, reject it. If one visible cause would let the viewer reconstruct the story, repair the carrier system before regenerating.

Then run the articulation-leak check. If A0 through A4 was selected and the image contains a readable sentence that explains the concept, reject the image as text rescue. Record-native marks can stay only when they act inside the carrier and the root event still reads with the words covered.

Then run the target-specificity check. A coherent story can still land on the wrong concept. Name the nearest meaning a cold viewer may reconstruct, then ask what visible cue makes the target concept win. Do this as a target-law check, not a label check. Name the law that would let the target concept govern the image. Then name the nearest wrong laws that may govern the same carrier more strongly. For each target, derive the minimum visible roles from its own function model. One concept may need a vulnerable stake. Another may need a measurement or a public rule. A system concept may need feedback made visible. These roles are not portable by name. They are portable only as jobs: make the target law easier to reconstruct than the nearest wrong law. A generated image fails when the evaluator can tell a good story but names the neighboring concept instead.

Use the target-law roles before prompting. The roles are the minimum visual jobs that make the target concept more likely than the nearest wrong concept. A role can be the vulnerable stake. It can be the moment control leaves the first object. It can be the witness or rule that changes what the carrier is allowed to mean. It can be the consequence that proves the event mattered. The exact roles change by concept. Derive them from the function model and confusable concepts. Each role should say what must be visible and which wrong reading it defeats. If the prompt cannot carry those roles without becoming bloated, repair the carrier or reduce the story reach before generating.

For relational targets, add the origin-and-accountability check before prompting. Ask whether the image will show why the relation exists and who or what can be held to it. If the target relation still needs a caption to explain its origin or accountability, change the carrier before adding detail. Test the same rule against unrelated relation families before treating it as guidance. Each relation family should earn its own proof cue.

Then run the prompt-transfer check. The final prompt must carry the target-law roles in scene-native language. It should also name the dominant wrong reading that must not win. If the chosen carrier naturally reads as another concept, the `Avoid` field should block that native drift and the positive fields should show the counter-cue. Empty `Constraints` or `Avoid` fields are acceptable only in a quick sketch that will not count as behavior evidence.

After generation, do not let creator-side inspection talk the image into the target. First name the visible concept family the image would likely produce before reading any notes. If a confusable family is stronger than the target, the image is not a target success. When an external blind evaluator confirms the wrong family, repair by replacing the carrier family or changing the dominant cue. Do not merely add another supporting detail to the same losing carrier.

Then run the stakes check. Ask what happens next if the carrier holds and what happens next if it fails. The chosen carrier must make consequence physically plausible. If failure would leave the world basically unchanged, the story is too weak.

For sequence outputs, run the sequence architecture check across the set. Each separate image should earn one viewer-model update. Identity and carrier law should survive across the run. The causal task should still feel like one task. Text should connect or name what the image cannot economically show; it should not patch missing visual logic. If any image is redundant or the set reads as adjacent symbols, repair the sequence before returning it.

For behavior validation or acceptance panels, run a separate blind reconstruction harness after the build. The creator prepares the validation target and the evidence bundle, then stops. A separate evaluator sees neutral image copies only, with no process trail to lean on. Ask the evaluator to state that image-only boundary before scoring. The score should test whether the pixels recover the concept as a lawful story rather than a label. The evaluator should see material evidence become object roles, object roles obey a world law, and that world law carry the chosen level. A sequence adds ordered change inside the same world. Store the result in an external validation report. Point to that report from the model only when the model is being used as an after-the-fact acceptance wrapper. During creator builds, leave blind-result fields blank or `performed: false`. Recovery optimization cannot overrule the other gates: a target name is not enough if the story, world law, or grounded reality fails.

Preserve prompt-label separation. The final prompt draft should keep the contract as separate fields rather than one long paragraph. If writer returns `PASS WITH REVIEW`, inspect the warning. In zero-caveat mode, repair the prompt or validation artifact until writer returns a clean `PASS`.

## Validate And Return

Before trusting the result, fill and save the model JSON whenever the run will generate an image or count as validation evidence. A prompt-only quick sketch can be compact, but behavior validation must have a full model file. Run the validator on that model before treating the result as evidence.

The hard gates live in the template. They test the movement from evidence into function. Then they test whether that function survived the whole path into the visible surface. The new carrier-law and sequence gates are part of that same path when those branches are active. Artifact quality gets its own check. Respect and audience relevance get the same weight. Overall readiness is the lowest hard gate, not an average. If one gate fails, repair the model before polishing the prompt.

The level gates test automatic story-reach choice and nested hierarchy. They should prove that the selected L-level earned its consequence radius, that lower and higher alternatives were considered, and that the added layer depends on the same root event. The articulation gates test visual concreteness. They should prove that the selected A-level solves a real viewer-inference problem without adding ornament, text rescue, or a parallel story. The carrier gates test R-mode. They should prove that the selected carrier preserves the governing cause better than the default or nearest competitor, that its sign logic is visible, and that the prompt transfers it as inference rather than style. The carrier-law gates prove that the chosen carrier behaves like a lawful world. The sequence gates prove that extra images earn model updates and preserve continuity. If a model can only say "more detail looks better" or "this world looks more interesting," the axes have failed.

In zero-caveat mode, the word `weakest_point` should not hide a tolerated flaw. It should state that direct inspection found no remaining weakness for that gate. If you can name any caveat or residual risk, the score for that gate is not 100 and the run needs repair.

Return the requested surface. If the user asked for an image, show the image and include the saved path when one exists. If the user asked for a prompt or model, return it directly. Keep scratch research out of the final unless the user asks for it, but include source links when the answer makes research-backed claims.
