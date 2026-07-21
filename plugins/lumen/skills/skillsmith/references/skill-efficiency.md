# Skill Efficiency

Use this reference when a skill change affects runtime cost or route choice. Use it when validation depth or resource files may change. Use it when examples or scripts are being added. Use it when subagents or research loops are being considered. Also use it when the user asks about efficiency or speed. Read it for cost. Read it for latency. Read it for bloat. Read it for simplification or over-validation.

Skill efficiency means least sufficient burden for a required quality and failure envelope. A skill is efficient when a future agent can preserve the intended capability with the lowest total runtime burden that still keeps quality, boundary, and recovery intact under expected variation.

Efficiency is not speed or cheapness. A shorter skill can be fake-efficient when it omits the model a future agent needs. A heavier skill can be inefficient when it forces every task through deep validation or extra references even when the output would not change. Density and resilience are constraints on efficiency. The skill must preserve enough capability before burden reduction counts as real.

The best efficiency repair often improves output because some burden is distortion. Delay weakens feedback. Noise weakens signals. Handoffs and re-entry create translation loss. Interruption and context switching weaken judgment. Rework moves the real fault into the future. Remove those burdens before removing control. Preserve sensing. Preserve validation that catches real risk. Preserve adaptive margin.

Attention leak is one of the highest-cost distortions. The run starts solving a nearby concern instead of the accepted question under discussion. That wastes time and can lower quality because every later step optimizes the wrong object. Efficient skills keep a source-level lane: answer the accepted question, add adjacent material only when it changes the result, and keep hard safety boundaries local to the unsafe part.

Efficiency work should begin with burden localization when the skill already exists. Measure or reconstruct the current run before editing when the task allows it. Separate model-building time from drafting or generation time. Separate inspection from repair. Separate public validation from the private work that should have made validation easy. The point is to find the burden that distorts output, not to make every stage shorter.

Repeated repair is usually late sensing. If a validator catches the same fault twice during tuning, the skill is learning too late. The efficient repair is upstream control. Put the missing distinction in the normal route. Put the required proof in the template before drafting. Put the route trigger before the expensive branch. Then rerun the same task and a nearby variation to see whether the validator becomes quiet while quality rises.

Quality-improving efficiency has a recognizable shape. The output improves because feedback reaches the source of the fault sooner. The agent spends less time patching stale artifacts. Evidence stays closer to the claim or surface it supports. The final run should feel calmer as well as faster because fewer late repairs are fighting the first pass.

## Efficiency Card

Use this card as a design review. Write short answers in prose. Do not turn it into a total score.

Boundary and horizon name what counts as part of the skill run and how far future burden should count. A narrow boundary can make a skill look efficient by hiding rework, maintenance, or user interruption outside the frame.

Quality and failure envelope names the result that must not degrade. It includes the minimum output quality, the mistakes that would make the result untrustworthy, and the recovery behavior that should remain available.

Normal path names the least route that should work for ordinary cases. It should be visible enough that a fresh agent does not waste effort choosing among equal-looking options.

Escalation trigger names when extra work earns its cost. Extra work can mean opening a reference. It can mean running a script or browsing. It can mean asking the user or calling a subagent. It can also mean using a fresh-agent panel. Take that step only when it is likely to change the output, reduce meaningful risk, or protect the boundary.

Return rule, also called the Stop rule, names when added work has earned its cost. Return when the expected improvement, risk reduction, or option value sits below the total burden of more work.

Burden ledger names what the skill spends. Count future-agent attention first. Then count context load and file reads. Count tool calls and validation cycles. Count subagent work and user clarification. Count maintenance, rework, and fragility caused by thin guidance.

Attention-leak ledger names the side frames the skill is tempted to answer. It should also name the trigger that makes each side frame legitimate. If the trigger is absent, the side frame is not caution. It is waste.

Adaptive margin names the minimum slack the skill needs under variation. Some fallback, validation, or conditional detail can be efficient when it prevents larger downstream failure. Zero slack is not efficient when the task is variable.

Frontier evidence names what a version costs and what it buys. Compare quality at a fixed burden and burden at a fixed quality. Use a profile instead of a single score when time and quality pull against each other. Use the same profile when risk and future burden move in different directions.

Better-output evidence names the causal leading indicators. Feedback latency should fall when late correction was the problem. Signal quality should rise when noisy checks were the problem. Work-in-process or queue age should fall when hidden errors were the problem. Human burden should fall when attention load was creating mistakes. Coordination burden should fall when dependencies were creating loss. Learning rate should rise when slow discovery was holding quality down.

Runtime affordance fit names how the skill should use the system it runs on without becoming provider-specific. Serialize when the next step needs the previous judgment. Serialize when two edits touch the same state or when a shared source must be interpreted once. Ordering also belongs in the path when it protects truth. Parallelize when branches are independent enough to complete without changing one another. File reads and static checks are common candidates. Fresh-agent evaluations and artifact inspections can also run together when their outputs have a clear reunion point. Disjoint edits need clear ownership before they earn parallel work. The gain is real only when branch reunification is simple and the saved latency does not return as merge confusion, duplicate reasoning, or inconsistent state.

## Coupling Scan

Scan for fake efficiency. A fast path with a weak quality envelope becomes cheap-thin output. A broad skill with no normal path makes agents spend effort selecting a route. A validator with no stop rule creates ritual. A script that saves local effort but adds maintenance may move burden rather than remove it. A reference that every run must read is probably main-path doctrine or bloat.

Fake efficiency can also look like dense bullets. If the bullets are only inventory, the future agent pays attention tax later. Use a list when order matters. Use a list when contrast or scanability changes the run. Otherwise write the relation as prose so the next decision is easier to feel.

The strongest repair is usually route clarity. Name the ordinary path. Name the trigger that earns extra work. Name the condition where the agent should stop and return. If a safeguard is too heavy, calibrate it to risk instead of deleting it.

Inspect serialization pressure before adding more instructions. Some workflows are slow because they force independent work through one lane. Split them only when each branch has clear ownership and a bounded output. Each branch also needs a reunification check. Keep the work serial when the branch would need the same live context. Keep it serial when disagreement cannot be resolved cheaply. Keep it serial when parallel agents would spend more effort coordinating than doing the work.

Repetition is hidden burden. A narrow skill should teach each boundary at the earliest action point. Put the rule where it changes behavior first. Later, check that it survived. If a generated narrow skill no longer fits in one careful read, look for repeated boundary language before adding another section.

Attention-leak rules should follow the same placement rule. Put the lane in the generation path. Put the check near validation. A single well-placed warning protects attention better than repeated warning language that becomes its own leak.

Use a compact target before the hard ceiling. A narrow one-file skill should usually stay well below the ceiling while still carrying the working relation from cue to trusted return. Moving close to the ceiling is acceptable when the task has route variety or serious risk. It is a warning sign when the extra words restate the same boundary.

Use source-level control as the simplification test. Add effort when fault detection is late. Add it when escape cost is high. Add it when the process is unstable. Add it when the skill lacks enough response variety. Stop when added checks no longer change outcomes. Stop when they no longer sharpen signals or protect resilience. Simplify when a step mainly creates waiting. Simplify when it mainly creates translation or dependency. Remove validation only after source controls exist and the check's hit rate no longer earns its burden. Convert universal checks into triggered review when that preserves signal without taxing every run.

Use an executable support gate for scripts. A script is efficient when it catches objective failures that prose review misses or catches too slowly. It is not efficient when it only restates judgment, creates maintenance work, or makes every future run prepare files for a check that rarely changes the output. For judgment-heavy skills, keep validation in the main workflow unless the script has clear inputs. Its findings should be repeatable. Its result should not create false confidence. Its repair move should beat direct inspection on total burden.

## Placement

Put efficiency support where it changes runtime behavior. Keep the quality floor and normal route in `SKILL.md`. Put conditional tradeoff detail in a direct reference when it would crowd the main path. Put repeatable measurement or validation in scripts. Keep research records outside the package. Keep A/B runs, timing logs, and panel results outside too.

When efficiency is weak, do not only shorten the text. First ask whether the quality floor is clear. Then ask whether the normal path is clear. Then ask whether escalation and stop conditions are visible. Cut only the burden that does not protect quality, reduce risk, or preserve useful options.
