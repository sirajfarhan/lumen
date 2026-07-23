# Lumen Plugin — End User License Agreement

**Effective:** 21 July 2026
**Licensor:** Siraj (hello@siraj.ai)

## 1. What you are licensed to do

Subject to these terms, you are granted a non-exclusive, non-transferable, revocable licence to install and use the Lumen plugin package ("the Plugin") with a compatible agent host, for your own work or the work of the organisation that obtained the licence.

## 2. What you may not do

You may not: resell, sublicense, or redistribute the Plugin; remove or alter its licensing or attribution; reverse engineer the hosted Lumen service or attempt to derive its scoring logic, prompts, or thresholds; use the Plugin to build a competing validation service; or represent Lumen validation results as your own product's guarantee.

## 3. What runs where

The Plugin runs locally in your agent host. It calls the hosted Lumen service over HTTPS to evaluate readiness and validate artifacts. The Lumen service, including its scoring logic, prompts, and thresholds, is proprietary and is not distributed with the Plugin.

## 4. Your data

- Requests carry the task evidence needed to evaluate readiness or validate an artifact.
- **Lumen does not retain submitted content.** It stores aggregate counts of validation requests and nothing else.
- Lumen keeps no skill memory, profiles, preferences, or feedback. A compatible agent host may provide its own memory when you enable it there; the Plugin uses only what that host supplies and does not create a second store.
- Your API key authenticates your account. Keep it secret; you are responsible for use made under it.

Full detail: `references/public-validation-contract.md`, shipped with every skill.

## 5. Availability and warranty

The Plugin and the Lumen service are provided "as is", without warranty of any kind, express or implied. Validation results are advisory quality signals. They do not constitute professional, legal, financial, or safety advice, and do not remove your responsibility to review the work an agent produces.

## 6. Liability

To the maximum extent permitted by law, the Licensor is not liable for indirect, incidental, or consequential damages, or for loss of profit, data, or business, arising from use of the Plugin. Total liability is limited to the fees paid for the Plugin in the twelve months preceding the claim.

## 7. Term

This licence continues until terminated. It ends automatically if you breach these terms. On termination you must stop using and remove the Plugin.

## 8. Changes

These terms may be updated for new releases. Continued use of a new release constitutes acceptance of the terms shipped with it.

## 9. Contact

Questions, data removal requests, and licensing enquiries: hello@siraj.ai
