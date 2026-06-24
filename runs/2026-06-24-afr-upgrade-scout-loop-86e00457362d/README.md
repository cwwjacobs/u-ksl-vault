# U-KSL: AFR Short-Term Upgrade Discovery Loop

Primitive name: **AFR Upgrade Scout Loop**

Date: **2026-06-24**

Canonical hash:

```text
86e00457362d6aa30d0eea6192249b14eed82efe0fe53198becb91d68c0e146f
```

## Purpose

This folder is the canonical save for the first U-KSL run recorded in `u-ksl-vault`.

It captures the Ultra Stage 1 directive, dispatch prompts, current proof, and exit condition for the AFR short-term upgrade discovery loop.

## Current stage

```text
Ultra Stage 1: Map / Kernel / Boundary / Dispatch
```

## Ultra Goal

Find the strongest short-term upgrade direction for AFR as a public local-first proof engine / loss leader.

## Kernel

AFR should make agent failures visible, exportable, and reusable as regression/eval artifacts while keeping user data local and preserving honest safety boundaries.

## Exit condition

```text
We know what to upgrade first, why it matters, and what not to touch yet.
```

## Included files

- `MANIFEST.json` — machine-readable run metadata and canonical hash
- `u-ksl-directive.md` — directive for this U-KSL run
- `stage-log.md` — current proof, dispatch state, and TODOs
- `prompts/gemini-scout.md` — Stage 2 Task 1A scout prompt
- `prompts/codex-xhigh-audit.md` — Stage 2 Task 1B repo-audit prompt

## Current proof captured

The AFR toy-trip-planner proof showed:

- model call capture
- tool call capture
- failed tool call capture
- error event capture
- retry behavior capture
- state snapshots
- checkpoints
- export bundle generation
- regression-case generation
- generated pytest scaffold passing

## Dispatch route

```text
1. Gemini Pro / Flash scout pass
2. Codex 5.5 xhigh repo-grounded audit
3. Qwen/Gwen table/checklist compression
4. Maia/current instance Ultra-KSL synthesis
```

## Stage 3 verification target

The final artifact for this loop should be:

```text
AFR Short-Term Upgrade Shape
```

It should identify:

- top 3 short-term upgrades
- next 3-5 PRs
- what belongs to Skills upsell
- what is deferred to mid-term
- what is deferred to long-term
- what to avoid for now
