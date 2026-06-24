# U-KSL Directive: AFR Short-Term Upgrade Discovery Loop

Primitive name: **AFR Upgrade Scout Loop**

## Purpose

Use U-KSL to discover the best short-term upgrades for Agent Flight Recorder without boxing the project into a premature mid-term or long-term product shape.

This loop is intentionally primitive.

We are not deciding the whole future of AFR yet. We are identifying the **short-term upgrade shape** that should be done next, based on repo architecture, user safety, dependency reality, and product leverage.

## Current Ultra Stage

```text
Ultra Stage 1: Map / Kernel / Boundary / Dispatch
```

Stage 1 defines:

- Ultra Goal
- Kernel
- boundaries
- current proof
- Stage 2 task shape
- agent dispatch order
- exit condition
- Stage 3 verification shape

Stage 1 does not rewrite the repo.
Stage 1 does not choose mid-term or long-term strategy.
Stage 1 only defines the bounded discovery loop.

## Ultra Goal

Find the strongest short-term upgrade direction for AFR as a public local-first proof engine / loss leader.

The short-term upgrade direction must strengthen:

```text
record -> inspect -> export -> regression case -> eval/fixture seed
```

It must preserve:

```text
AFR = OSS trust engine / loss leader
Skills = paid implementation and proprietary-data workflow layer
```

## Ultra Kernel

AFR should make agent failures visible, exportable, and reusable as regression/eval artifacts while keeping user data local and preserving honest safety boundaries.

## Current proof

The toy-trip-planner proof has shown:

- model call capture
- tool call capture
- state snapshots
- checkpoints
- failed tool call visibility
- error event visibility
- retry visibility
- export bundle generation
- regression case generation
- generated pytest scaffold passing

This is enough proof to stop arguing whether the core idea works. It works.

The current question is:

```text
What short-term upgrades make this easier, safer, clearer, and more commercially useful?
```

## Exit condition

The loop exits when we have:

1. A ranked list of short-term upgrade candidates.
2. A clear recommendation for the first 3-5 short-term PRs.
3. A short explanation of why those upgrades matter.
4. A classification of each upgrade:
   - OSS core
   - paid Skill pack
   - pro CLI candidate
   - future / mid-term
   - avoid for now
5. A decision on what should not be addressed until mid-term or long-term planning.

The loop does not need to solve mid-term or long-term strategy.
The loop does not need to define every future product.

The loop exits at:

```text
We know the short-term upgrade shape.
```

## Boundary

### In scope

- setup friction
- CLI usability
- proof/demo path
- dependency/architecture clarity
- user-safety hardening
- Codex-AFR usability
- export/regression-case polish
- eval seed promotion path
- local proprietary-data workflow
- redaction/review path
- Skills upsell seams
- release-readiness gaps
- short-term PR roadmap

### Out of scope for this loop

- full SaaS design
- dashboard-first roadmap
- enterprise security claims
- hidden reasoning capture
- model interpretability claims
- full plugin marketplace design
- long-term pricing architecture
- complete paid product catalog
- major rewrites
- speculative features without short-term leverage

## Do-not-box-in constraints

AFR must not be boxed into being only:

- Codex
- Python
- evals
- toy demos
- dashboard
- SaaS
- enterprise security
- one agent framework
- one proprietary workflow

AFR is the base proof engine. Expansion seams must remain open.

## Stage shape

```text
Ultra Stage 1: Map / Kernel / Boundary / Dispatch
  -> define this directive
  -> bound Gemini scout
  -> bound Codex repo audit
  -> define exit condition

Ultra Stage 2: Walk / Scout / Audit
  -> Gemini Pro/Flash scouts short-term upgrade directions
  -> Codex 5.5 xhigh performs repo-grounded deep pass
  -> optional Qwen/Gwen compresses findings into tables

Ultra Stage 3: Verify / Select / Bound Next Loop
  -> audit results against this directive
  -> select short-term upgrade shape
  -> produce first PR roadmap
  -> explicitly defer mid-term and long-term decisions
```

## Ultra Stage 3 verification questions

1. Did the results identify short-term upgrades?
2. Did they avoid solving mid/long-term too early?
3. Did they preserve local-first and CLI-first?
4. Did they preserve user proprietary-data safety?
5. Did they avoid hidden-reasoning and enterprise-security overclaims?
6. Did they keep Skills as the upsell layer?
7. Did they preserve expansion seams?
8. Are the recommended PRs small enough to execute?
9. Do the recommendations strengthen the existing proof loop?
10. Are any recommendations out of scope for this loop?

## Stage 3 exit states

```text
DONE:
  We have a ranked short-term upgrade shape and first PR roadmap.

DEFICIENT:
  The results are too broad, too speculative, or not repo-grounded.

RETURN TO STAGE 1:
  The Ultra Goal or boundary is wrong.

RETURN TO STAGE 2:
  The audit missed critical repo/security/product facts.
```

## Stage 3 final artifact

The final artifact should be:

```text
AFR Short-Term Upgrade Shape
```

It should include:

- top 3 short-term upgrades
- next 3-5 PRs
- what belongs to Skills upsell
- what is deferred to mid-term
- what is deferred to long-term
- what to avoid for now

## Current U-KSL exit condition restated

```text
We know what to upgrade first, why it matters, and what not to touch yet.
```

Only then do we start the next Ultra loop for mid-term and long-term shaping.
