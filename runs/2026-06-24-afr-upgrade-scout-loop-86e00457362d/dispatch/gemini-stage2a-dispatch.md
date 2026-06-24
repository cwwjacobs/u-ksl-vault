# Gemini Stage 2A Dispatch Packet

## U-KSL Run

**U-KSL: AFR Short-Term Upgrade Discovery Loop**

Primitive name: **AFR Upgrade Scout Loop**

## Operator frame

The operator owns direction and authority. Gemini is a Stage 2 walker. Gemini does not own the roadmap.

## Task

Perform **Stage 2 Task 1A: Scout Pass** for:

```text
cwwjacobs/agent-flight-recorder
```

## Ultra Goal

Find the strongest short-term upgrade direction for AFR as a public local-first proof engine / loss leader.

AFR should prove:

```text
record -> inspect -> export -> regression case -> eval/fixture seed
```

AFR is the OSS trust engine / loss leader.
Skills are the paid implementation layer that help users apply AFR to their own agents, tools, proprietary traces, redaction workflows, CI systems, incident reports, and eval/regression pipelines.

## Exit condition for this scout

Gemini exits when it returns:

1. Top 5 short-term upgrade hypotheses.
2. Top 5 risks / unknowns.
3. Top 10 questions for Codex 5.5 xhigh.
4. Tool/data targets for Codex to verify.
5. What not to decide yet.
6. Recommended Codex audit focus.

## Hard boundary

Do not rewrite the repo.
Do not make code changes.
Do not solve the mid-term roadmap.
Do not solve the long-term roadmap.
Do not push SaaS-first, dashboard-first, enterprise-security-first, hidden-reasoning, or model-interpretability framing.
Do not produce private internal process notes.

Return observable outputs only:

- repo areas to inspect
- files Codex should verify
- commands/tests that may produce evidence
- risks
- upgrade hypotheses
- PR-sized candidates
- defer/avoid list
- Codex handoff questions

## Known proof

A toy-trip-planner run successfully showed:

- model calls
- tool calls
- state snapshots
- checkpoints
- failed tool call
- error event
- retry behavior
- export bundle
- generated regression case
- passing generated pytest scaffold

## Required output format

# Stage 2 Task 1A: Gemini Scout Result

## 1. Executive scout read

## 2. Top 5 short-term upgrade hypotheses

For each:

- hypothesis
- why it matters
- expected product impact
- expected safety impact
- likely classification: OSS core / paid Skill / pro CLI / future / avoid

## 3. Top 5 risks or unknowns

For each:

- risk / unknown
- why it matters
- what Codex should inspect to verify it

## 4. Tool/Data Target Card

### Repo areas needing tool-backed inspection

### Files Codex should inspect

### Commands/tests likely to produce useful evidence

### Artifacts that should exist after inspection

## 5. Likely OSS core upgrades

## 6. Likely paid Skill pack seams

## 7. User-safety concerns

## 8. Top 10 questions for Codex 5.5 xhigh

Each question must be repo-verifiable.

## 9. Do-not-decide-yet list

## 10. Recommended Codex audit focus

## 11. Final scout recommendation

Give a concise recommendation for what the short-term upgrade shape probably is, while clearly marking it as a scout hypothesis for Codex to confirm/refute.
