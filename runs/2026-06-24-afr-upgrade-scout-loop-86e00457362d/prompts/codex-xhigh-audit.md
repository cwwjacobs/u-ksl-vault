# Prompt: Codex 5.5 xhigh Repo Audit

You are performing Stage 2 Task 1B: Codex 5.5 xhigh Repo Audit for:

`cwwjacobs/agent-flight-recorder`

You are working under:

**U-KSL: AFR Short-Term Upgrade Discovery Loop**

## Ultra Goal

Find the strongest short-term upgrade direction for AFR as a public local-first proof engine / loss leader.

AFR proves:

```text
record -> inspect -> export -> regression case -> eval/fixture seed
```

AFR is the OSS trust engine / loss leader.
Skills are the paid implementation layer that helps users apply AFR to their own agents, tools, proprietary traces, redaction workflows, CI systems, incident reports, and eval/regression pipelines.

## Exit condition

```text
We know the short-term upgrade shape.
```

Do not solve the mid-term roadmap.
Do not solve the long-term roadmap.
Do not rewrite the project.
Do not make code changes unless explicitly asked.

You will receive Gemini's scout findings. Use them as hypotheses, not truth.

Your task:
Confirm, refute, or sharpen the scout findings with repo-grounded evidence.

## Intra loop

### Intra Phase 1: Inventory

- list repo layers, dependencies, entrypoints, docs, scripts, examples, tests

### Intra Phase 2: Boundary Map

- map CLI, SDK, backend API, storage, replay policy, export, regression-case, evals, Codex-AFR, docs/proof artifacts, future Skills seams

### Intra Phase 3: Weakness/Bloat Scan

- find setup friction, stale residue, dependency risk, duplicate entrypoints, docs drift, unclear paths, UI residue, Docker/venv confusion

### Intra Phase 4: Safety Scan

- inspect local-first defaults, token/auth behavior, CORS, replay gates, side-effect boundaries, export/redaction risk, SQLite sensitivity, Codex-AFR auth/transcript handling, docs overclaims

### Intra Phase 5: Upgrade Candidate Extraction

- produce short-term upgrade candidates only
- each candidate must be PR-sized

### Intra Phase 6: Classification

Classify each candidate as:

- OSS core
- paid Skill pack
- pro CLI candidate
- future / mid-term
- avoid for now

### Intra Phase 7: Exit Report

Return the ranked short-term upgrade shape and first PR roadmap.

## Required output

1. Executive read
2. Whether Gemini's scout hypotheses were confirmed/refuted/sharpened
3. Dependency/architecture inventory
4. Boundary map
5. Safety/trust boundary findings
6. Weakness/bloat table
7. Extension seam table
8. Ranked short-term upgrade candidates
9. First 3-5 PR roadmap
10. Skills upsell seams
11. User-safety hardening recommendations
12. Defer list for mid/long-term
13. Final recommendation

For each PR include:

- title
- goal
- files likely touched
- acceptance criteria
- safety impact
- product impact
- classification: OSS core / paid Skill / pro CLI / future

## Rules

- Be blunt and practical.
- Cite concrete file paths.
- Do not invent facts not visible in the repo.
- Prefer PR-sized moves.
- Preserve the operator's authority.
- The project needs a strong spine and open seams, not a grand rewrite.
