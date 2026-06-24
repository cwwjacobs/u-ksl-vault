# Tool Data Leverage Protocol

## Purpose

We are not collecting thinking traces, hidden reasoning, private chain-of-thought, or model mind-reading artifacts.

We are collecting **tool data** and **observable work products**.

The leverage engine is:

```text
U-KSL directive -> bounded model task -> tool/event outputs -> file-path findings -> Codex handoff -> PR roadmap
```

## Rule

Do not ask a model to expose reasoning.
Do not ask for hidden trace.
Do not preserve private reasoning as a project artifact.

Ask for observable outputs:

- tool calls
- tool results
- files inspected
- dependency findings
- command outputs
- errors
- checkpoints
- artifacts created
- ranked upgrade candidates
- PR-sized recommendations
- uncertainty list
- questions for the next walker

## Observable tool-data cards

Gemini should return the following cards:

1. **Scout Output Card**
   - current project read
   - strongest short-term upgrade hypotheses
   - biggest unknowns

2. **Tool/Data Target Card**
   - which repo areas need tool-backed inspection
   - which files Codex should inspect
   - which commands/tests may produce useful evidence
   - which artifacts should exist after inspection

3. **Risk Card**
   - user-safety risks
   - data-handling risks
   - trust-boundary risks
   - product-positioning risks

4. **Leverage Card**
   - what can become OSS core
   - what can become paid Skill packs
   - what can become pro CLI
   - what should be deferred

5. **Codex Handoff Card**
   - top questions Codex must verify in files
   - repo paths likely worth inspection
   - hypotheses Codex should confirm/refute with evidence

6. **Exit Card**
   - ranked short-term upgrade candidates
   - recommended first PR direction
   - what not to decide yet

## How to leverage Gemini

Use Gemini as a scout engine, not a final authority.

Gemini should:

- surface options
- identify risks
- sharpen Codex questions
- preserve optionality
- identify repo/tool-data targets
- avoid dashboard/SaaS/default-UI gravity
- avoid enterprise-security claims

Gemini should not:

- rewrite the roadmap
- decide mid-term or long-term strategy
- claim file facts without evidence
- produce unbounded strategy fog
- provide or preserve hidden reasoning traces

## Handoff to Codex

Codex receives:

1. U-KSL Directive
2. Gemini Scout output
3. Repo access

Codex then performs the repo-grounded pass:

```text
inspect files -> run/check commands -> confirm/refute -> cite file paths -> return PR-sized moves
```

## Optional AFR capture

If Gemini is called through a local script/API wrapper, record only the observable boundary with AFR:

- prompt -> model input artifact
- response -> model output artifact
- files/tools used -> tool data if available
- final scout output -> checkpoint artifact
- final handoff -> exportable artifact

Do not record or request hidden reasoning.

If Gemini is used through a web UI, capture manually:

- paste final output into this vault run
- add a Stage 2 scout result file
- summarize key findings into the stage log

## Short-term leverage principle

The engine is useful only if every model pass produces one of these:

- a ranked decision
- a sharpened question
- a verified file-path finding
- a tool output
- a command/test result
- a PR-sized recommendation
- a defer/avoid boundary

Anything else is model vapor wearing a badge.
