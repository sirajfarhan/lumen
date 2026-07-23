# Oracle Calibration Protocol

Use this protocol before a multimodal model reader contributes acceptance evidence. It calibrates a reader family against the current artifact class and construct family. It does not certify the model in general, and it does not turn a model into a real audience.

Start from the exact candidate or an approved calibration surface with the same artifact class. Freeze its hash. Choose one construct and one reader family from `oracle-registry.json`. Do not combine constructs merely to reduce calls. Prepare neutral copies whose names, metadata, and order do not reveal the expected answer.

## Verify Input Delivery First

Before asking for judgment, prove that every neutral image rendered through the host's actual image-inspection path. The reader records the observed dimensions and one non-semantic visual anchor for each surface, such as “a wide pale slide with a road occupying the right half.” This anchor proves contact with the pixels without revealing the expected defect. When the host requires an explicit image-open or attachment action, perform it for every surface.

Compare this delivery record with direct file facts. If a reader describes a pixel-identical control as blank, reports the wrong dimensions, cannot open one candidate, or sees a different number of surfaces, mark the run `invalid_input_delivery`. Do not score the seven checks. Do not call the model reader insensitive. Repair the attachment or rendering path and start again in a fresh session.

## The Seven Checks

### Image removal

Give the reader the same task without the image. Pass only when it abstains, lowers confidence, or explicitly says the visual claim cannot be localized. A reader that returns substantially the same visual finding without pixels is not admissible for that construct.

### Image swap

Replace the image while keeping the task and audience boundary unchanged. The replacement must differ on the selected construct. Pass only when the finding and localization move with the pixels rather than the prompt, filename, or expected answer.

### Order permutation

For pairwise judgment, show A/B and then B/A in a fresh pass. Pass only when the preferred artifact and localized reason remain the same after position reversal. A tie may remain a tie. Do not average contradictory orders.

### Semantic mutation

Change one story-bearing cue while preserving unrelated presentation properties. The mutation should attack the selected construct, not make the whole image obviously worse. Pass only when the reader detects the intended change, localizes it, and updates the construct finding.

### Irrelevant mutation

Change something that should not affect the construct: encoding metadata, a neutral filename, equivalent wording outside the raster, or a truly non-story-bearing pixel change. Pass only when the reader keeps the same construct verdict or returns a tie. Aesthetic preference cannot turn an irrelevant mutation into evidence.

### Defect localization

Require a region, object relation, text span, frame transition, or source-to-image mismatch that supports every material finding. Pass only when the localization overlaps the seeded defect or names the correct relation. General commentary without visible contact is not localization.

### Abstention

Include one case where the available inputs cannot support the claim. Pass only when the reader says the evidence is insufficient and names the missing oracle input. Examples include factual fidelity without a source, continuity without a baseline, and real-audience transfer without people.

## Building Mutations

Choose the smallest mutation that changes one construct while protecting the others. A semantic-channel mutation may swap two channel owners while keeping contrast. A hierarchy mutation may strengthen one secondary region without changing the copy. A world-law mutation may break one path or affordance without restyling the scene. An evidence mutation may alter one must-survive relation while leaving the composition intact. A continuity mutation may change one protected property outside the requested delta.

Do not teach the skill a specific object, colour, city, or slide as the mutation. Record the construct attacked, the protected properties, the exact changed region or relation, and the expected observable response. The same mutation logic should be usable in another content world.

## Admission

Record the run in `oracle-calibration-template.json`. Each check has one of four states: `pass`, `fail`, `pending`, or `not_applicable`.

`not_applicable` is allowed only when the check genuinely cannot apply to that oracle. Explain why and name the alternative evidence. For example, order permutation is not applicable to a single-candidate factual-fidelity check unless a reference-versus-candidate order could bias the reader. Image removal, image swap, semantic mutation, irrelevant mutation, localization, and abstention normally remain required for model readers.

A reader family is admissible for one construct family only when input delivery is verified and every applicable check passes. Any fail or pending state keeps the reader diagnostic. Invalid input delivery invalidates the run rather than failing the reader. Record disagreement by construct. Do not rescue a failed calibration with an average, a majority vote, or eloquent reasoning.

The calibration record binds to the exact reader family, model identity when known, construct ids, artifact class, task wording, candidate hashes, and timestamp. A material change in model family, reader prompt, artifact class, or construct family requires recalibration. A harmless new candidate does not.

After calibration, run the actual reader on the untouched current candidate in a fresh session. Calibration mutations are never shown to that final reader. The final reader's evidence remains bounded by the stopping boundary in the registry.
