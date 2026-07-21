# Quality Judge

How to review this skill's user-facing messages — setup questions, teaching turns, and repair notes — before they reach the user. Progress lines and one-line statuses come from the server already checked; do not re-judge them. Do not judge instruction bodies, schemas, or safety rules, and skip this review entirely for a short single-turn task that carries no setup question or teaching turn.

## Protocol

Run the review in a fresh subagent where the host provides one — the reviewer must not be the author of the message. Where no isolated reviewer is available, run the review as its own separate pass before sending, reading only the message and this reference.

For each criterion below, write one sentence of reasoning first, then a verdict of exactly `pass` or `fail`. Never score, weight, or average. If any criterion fails, return exactly one primary fix — the most consequential one — phrased in the task's own terms, naming the sentence's gap, never the skill's competence, with a bounded direction such as "name the user's page in the question" rather than "be clearer".

Repair and re-review at most three times. A criterion that passed in an earlier cycle stays passed; do not reopen it for preference. After the third cycle, send the best current version and record the review as flagged rather than clean.

## Criteria

### grounded-referent

Would this user, reading only this message, recognize every thing it refers to as theirs — their page, their email, their decision — rather than a placeholder like "the work" or an unexplained term?

Example that FAILS this criterion:

> First, make clear what should become easier or different.

### visible-consequence

Can the user see what their answer will change about the result, without knowing anything about how this skill works inside?

Example that FAILS this criterion:

> What would materially change how I handle this?

### example-first

If the message needs an idea the user may not hold, does one short familiar situation come before the ask — supplied by the skill when the user is new to the idea, not demanded from them?

Example that FAILS this criterion:

> What familiar experience would make eigenvectors easier to grasp?

### task-term-why

If the message states a reason, does the reason name what changes for the user's task — not a generic justification?

Example that FAILS this criterion:

> Please answer so I can establish what's needed to proceed.

### survives-one-reading

Do the referent and the ask both survive a single reading — enough restatement that a non-expert is not forced to re-read or guess?

Example that FAILS this criterion:

> Boundaries?

### regrounds-not-repeats

If this is a response to "I don't follow", does it ground the same idea differently — tied to something already established — rather than repeating the earlier wording or escalating abstraction?

Example that FAILS this criterion:

> As stated before: name any limit that would change the work.

### first-screen-concrete

Is the question about the experience anchored to a screen or action the user can picture, rather than an abstract product goal?

Example that FAILS this criterion:

> What should the site accomplish for your business?

### solo-justified

If this run skipped a layout/concept pass, does the recorded one-line reason hold for THIS build — is the layout genuinely standard?

Example that FAILS this criterion:

> Skipped the layout pass because the page is simple. (The request was a novel interactive bento-grid landing page.)

## Record

Attach a compact review line to the validation packet as an artifact named `surface review`: each criterion id with its final verdict, the number of cycles used, and `flagged` or `clean`. The review is evidence for the server's audit lane; it never replaces the server's own checks, and official readiness still comes only from a current Lumen run.
