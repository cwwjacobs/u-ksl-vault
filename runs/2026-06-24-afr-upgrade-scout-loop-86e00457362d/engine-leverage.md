# Engine Leverage Protocol

## Purpose

We do not need to see Gemini's hidden reasoning. We need to force the model to leave useful observable residue while it works.

The leverage engine is:

```text
U-KSL directive -> bounded scout prompt -> checkpoint artifacts -> Codex handoff -> synthesis -> PR roadmap
```

## Rule

Do not ask a model to "think deeply" and return a blob.

Ask it to return phase checkpoints, uncertainty, and downstream handoff material.

## Observable checkpoints

Gemini should return the following cards:

1. **Scout Snapshot**
   - current read of the project
   - strongest short-term upgrade hypotheses
   - biggest unknowns

2. **Risk Card**
   - user-safety risks
   - trust-boundary risks
   - product-positioning risks

3. **Leverage Card**
   - what can become OSS core
   - what can become paid Skill packs
   - what can become pro CLI
   - what should be deferred

4. **Codex Handoff Card**
   - top questions Codex must verify in files
   - repo paths likely worth inspection
   - hypotheses Codex should confirm/refute

5. **Exit Card**
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
- avoid dashboard/SaaS/default-UI gravity
- avoid hidden-reasoning or enterprise-security claims

Gemini should not:

- rewrite the roadmap
- decide mid-term or long-term strategy
- make repo claims without evidence
- produce unbounded strategy fog

## Handoff to Codex

Codex receives:

1. U-KSL Directive
2. Gemini Scout output
3. Repo access

Codex then performs the repo-grounded pass:

```text
confirm -> refute -> sharpen -> cite file paths -> return PR-sized moves
```

## Optional AFR capture

If Gemini is called through a local script/API wrapper, record the interaction with AFR as a model call:

- prompt -> model input
- response -> model output
- phase -> state snapshot
- scout result -> checkpoint
- final handoff -> exportable artifact

This turns model work into a traceable run.

If Gemini is used through a web UI, capture manually:

- paste final output into this vault run
- add a Stage 2 scout result file
- summarize key findings into the stage log

## Short-term leverage principle

The engine is useful only if every model pass produces one of these:

- a ranked decision
- a sharpened question
- a verified file-path finding
- a PR-sized recommendation
- a defer/avoid boundary

Anything else is just model vapor wearing a badge.
