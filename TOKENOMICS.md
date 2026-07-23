# Lumen Readiness Review Economy

## Thesis

Under the proposed economy, Lumen skills stay open and users pay only for protected readiness review of agent work. The creator defines what the review should notice and when the agent should call it. The review criteria stay protected.

Protected means the criteria are not published in the public skill or returned in the result. The creator approves the exact review version; the user receives its hash, the creator's signature, and execution evidence rather than the criteria themselves.

People continue working in their existing AI harness. The first stage is a bounded pilot with manual payment. The second-stage proposal adds NEAR account access, payment, and a receipt for each review.

The proposed NEAR flow describes the intended second-stage product.

![Lumen readiness review loop](assets/lumen-readiness-review-loop.png)

## What users pay for

The user pays to apply the creator's protected review to the agent's work. The fee is for that judgment, whether the review returns `ready` or `needs review`.

## Proposed user flow

After the NEAR infrastructure is built:

1. **The user starts in their existing AI harness.** The public skill runs inside Codex, Claude Code, or another AI harness.
2. **The user connects a NEAR account.** The account proves control of that account and handles payment approval.
3. **The user approves the review.** The user sees the price and the exact work and sources selected for review, chooses NEAR or a supported stablecoin, and approves the set and amount.
4. **Lumen runs the protected review.** Lumen receives only the approved set and deletes the submitted content after returning the result.
5. **The user receives the result and receipt.** A `ready` result tells the agent it may continue under the review policy; `needs review` names what the agent must fix. The receipt records the payment, review-version hash, result, and payment split. Creator approval for that hash remains a separate signed record.

## What creates value and what the receipt proves

| Readiness review creates value | Review receipt proves the event |
|---|---|
| Applies the creator's judgment to the work | Records the review version and result |
| Returns policy permission to continue or points to a repair | Links the payment and its split to that review |

The receipt's claim stops at the recorded review event and payment. Review correctness and whether the work deserved `ready` remain outside it.

The review fee can support the creator, maintainers, and the infrastructure that runs the review. Shares for contributors or a marketplace require published acceptance and split rules.

## Why NEAR

Lumen can use NEAR accounts for access, NEAR Intents for flexible payments, and NEAR AI Cloud for private inference with signed request-and-response evidence. AI Cloud provides evidence that a signed request and response were processed inside an attested trusted execution environment (TEE). A separate creator-signed record must bind the approved review version to its creator.

NEAR AI Cloud is in beta, and the older standalone Shade Agent framework is deprecated.

## Before a paid pilot

Before the first paid pilot, publish the price, fee split, challenge process, selected-data display, deletion timing, and retained receipt fields. If the pilot includes contributors, publish their acceptance and credit rules first. Publish token or community-decision rules before those features exist.

## Launch path

1. **Prove demand.** Run one bounded review with manual payment and measure repeat use, cost, speed, what it helps repair, and the share of `ready` results later challenged or reversed under the published process.
2. **Add the NEAR layer after the published thresholds are met.** Add account access, payment, receipts, and fee splits under the published rules.
3. **Add an optional token only if the activity shows a problem it solves.** NEAR and supported stablecoins remain the default payment methods.
