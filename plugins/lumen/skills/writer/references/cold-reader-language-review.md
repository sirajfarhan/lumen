# Cold-Reader Language Review

Use this review after the reader has already described the final in their own words. Do not show these criteria first. The first reconstruction must remain unprompted.

The review has two jobs:

1. find language that makes this audience guess at a consequential relation;
2. identify surface language that may have been smoothed away from the speaker's voice.

It does not reward simple vocabulary for its own sake. A technical term, compact abstraction, or formal sentence may remain when the audience knows it, the surrounding text makes its function clear, or accuracy requires it.

## Translation audit

Ask the reader to quote every consequential phrase they had to reread, translate into ordinary language, or complete by inference. For each quoted span, record:

```text
Exact span:
Reader paraphrase:
What the sentence states clearly:
What the reader had to guess:
Missing relation: actor | action | condition | consequence | referent | technical function
Why the missing relation matters here:
Consequence level: blocking | important | optional
Smallest repair that would remove the guess:
```

The phrase needs repair when the intended reader cannot explain what happens without repeating its abstract nouns, cannot identify who acts or what changes, cannot resolve a referent, or cannot tell why a named mechanism appears here. Several abstract nouns in one phrase are only a warning; fail the phrase only when they hide a relation this audience needs.

Classify the consequence from the current audience and decision:

- `blocking`: without the relation, the reader cannot understand the central claim, follow the process, take the requested action, or judge a material promise about payment, privacy, safety, ownership, or control;
- `important`: the reader can follow the whole, but the missing relation can materially change trust, scope, responsibility, or the decision;
- `optional`: the detail would satisfy curiosity or implementation planning but does not change what this audience must understand or do on this surface.

Repair blocking and important findings. Keep optional findings separate as possible follow-up detail; they do not lower the current language decision. When uncertain, state what decision would make the detail important instead of silently upgrading it to a failure.

A technical name is not a failure merely because it is specialized. Keep it when the reader must recognize or use it. Explain it locally when the reader needs its function to follow the decision. For an expert audience, an established term may need no gloss when its role in the sentence is already clear.

## Surface voice risk

Next ask the reader to quote any line that feels generic, corporate, performative, slogan-like, unusually smooth, or written from outside the speaker's situation. For each span, record:

```text
Exact span:
Surface impression:
What in the wording creates that impression:
Source comparison required: yes
```

This is a risk report, not proof of voice drift. A final-only reader cannot know whether a line sounds like the user. Compare the flagged span with eligible voice evidence. Confirm over-smoothing only when the rewrite changed a meaningful part of the user's stance: ownership, bounded uncertainty, reasoning order, relationship pressure, natural emphasis, or characteristic landing. Formality and grammatical finish alone are not failures.

## Repair map

Choose the smallest repair that matches the diagnosed failure:

- missing actor: name who or what acts;
- missing action: replace the process noun with the concrete verb;
- missing condition: state when the claim or mechanism applies;
- missing consequence: say what changes for the reader, user, or decision;
- unresolved referent: replace the pointer with its actual subject;
- unclear technical function: keep the necessary name and explain what it enables here;
- internal model label: remove the label and state the relation directly;
- slogan-shaped line: separate the actual claim from its consequence;
- confirmed voice smoothing: restore the user's ownership, uncertainty, causal order, relationship pressure, or ordinary wording.

Never repair a missing relation by inventing a fact, actor, promise, or degree of certainty. Ask for source material when the missing detail changes the claim; otherwise omit it or keep the statement within what the source supports.

## Acceptance

Pass the language review only when:

- no blocking or important phrase still depends on a guess;
- necessary technical terms are accurate and locally usable for this audience;
- the reader can paraphrase the important relations without borrowing the final's abstract wording;
- any surface voice risk has been checked against eligible voice evidence;
- every repair preserves the source's facts, certainty, and intended movement.

A favorable overall impression cannot erase one material translation failure. Any repair creates a new artifact and requires a new cold reader.

## Transfer examples

These examples teach the distinction, not preferred wording.

Technical and clear:

> OAuth with PKCE prevents someone who intercepts the login code from reusing it.

The specialized name stays because the sentence immediately states its function.

Compact and clear for a specialist:

> The API verifies the JWT before reading its claims.

This may pass for an API developer because the action and order are already explicit. The same line may need a brief explanation for a nontechnical buyer.

Relation hidden:

> The maintained standard governs readiness at meaningful boundaries.

The reader must guess who maintains the standard, when it is used, what it checks, and what happens afterward. Repair the missing relation rather than replacing individual nouns with simpler synonyms.

Voice smoothed away:

```text
Source: I don't think this is ready yet. The numbers still feel off to me.
Rewrite: The initiative remains positioned for further quantitative refinement.
```

The rewrite removes ownership, uncertainty, and the speaker's direct reason. A useful repair restores those relations without copying every rough surface feature.

Formal but earned:

```text
Source: We recommend pausing enrollment until the safety review is complete.
Rewrite: We recommend pausing enrollment until the safety review is complete.
```

The sentence is polished and formal, but it is not over-smoothed: the source, audience, action, and condition all support that form.
