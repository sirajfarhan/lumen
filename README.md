# Lumen

> Judgment is knowing where attention should go.

Experience changes what a person notices. Over years of work, they learn what deserves attention first, what can wait, which question changes a decision, and what should make them stop and look again. Lumen helps an agent follow that order. The skill's creator decides what the review should notice. The user's instructions decide whether the agent repairs the work, changes direction, or stops.

Each Lumen skill pairs a public method for doing the work with a private readiness review whose criteria stay protected. The review checks whether an important next step can proceed. The creator of each skill defines what its review should notice and when the skill should ask Lumen to run it. Each review either clears the step or points to something that needs repair.

## How Lumen works

The skill and readiness review work as one loop:

1. **The skill focuses the agent on what deserves attention.**
2. **Inside Codex, Claude Code, or another AI harness, the agent follows that guidance and does the work.**
3. **Before an important next step, the skill asks Lumen to run readiness review.**
4. **A `ready` result clears the step; `needs review` points the agent to what it must repair.**

## Skills in Lumen

Lumen currently has one router and six specialist skills. Use a specialist directly when you know what you need, or use `route` when the task may need more than one.

| Skill | What it helps the agent do |
|---|---|
| `route` | Choose the right skill or connect several of them |
| `skillsmith` | Turn a repeated workflow into a skill and test whether it works when reused |
| `writer` | Write in the user's voice while staying faithful to the source |
| `question-sharpener` | Find the question that can move a stalled decision |
| `expert-research` | Find qualified sources, compare what they say, and turn the result into a decision |
| `concept-visualizer` | Turn an idea into a diagram people can understand at a glance |
| `web-builder` | Build a working page and check it on the screens people will use |

Each skill can also teach its method. It begins with one example, then helps the user apply the same idea somewhere new. Codex, Claude Code, or another AI harness can save a preference the user approves and provide it to the skill later. The preference stays with that harness, and the current instruction always takes priority.

## Install

In Claude Code:

```text
/plugin marketplace add sirajfarhan/lumen
/plugin install lumen
```

In Codex, open Plugins, add `https://github.com/sirajfarhan/lumen` as a marketplace, and install Lumen.

### Connect Lumen

Get an API key from [hello@siraj.ai](mailto:hello@siraj.ai). Enter it when Lumen asks on the first task; it is saved locally in `~/.lumen/lumen.env` and reused in later sessions.

For each readiness check, the skill selects the work and supporting sources needed for review and sends that set to Lumen. Lumen discards the submitted content after returning the result. An API key activates readiness review, while the public skill guides the agent on its own.

### Start a task

```text
$lumen:route Turn these notes into a launch update.
```

In Claude Code, use `/lumen:route` instead. `route` chooses the right skill and brings in others when the task needs them. Readiness review keeps pointing the agent to what needs attention as the work moves.

## Public skill and readiness review

The skill is public. Anyone can inspect how it works, then use or improve it.

Readiness review runs while the agent works. When a decision could change the result, the review either clears the next move or points the agent to something that needs repair.

The public skill instructions remain open for anyone to inspect and improve. The creator can publish the method while keeping the review criteria that support their paid work protected. Lumen receives submitted review content for the check and discards it after returning the result.
