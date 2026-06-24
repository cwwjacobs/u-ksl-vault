# Stage Log

## 2026-06-24

### Run opened

The operator created `u-ksl-vault` as the canonical archive for U-KSL runs.

### Project under analysis

- Repository: `cwwjacobs/agent-flight-recorder`
- Public proof/loss-leader project: Agent Flight Recorder (AFR)
- Upsell layer: Skills / tools / implementation packs

### Current proof from AFR

The toy-trip-planner run proved the loop:

```text
record -> inspect -> export -> regression case -> test
```

Observed proof:

- run id: `72fa97e2-aee7-42b5-b77d-c263a0079e02`
- checkpoint after-flights: `5dea34ff-98fd-47c5-b367-6712a88d5ee4`
- checkpoint after-hotel: `b878de65-7521-47e1-a1a7-4c96b61a861a`
- 16 events
- 3 checkpoints
- failed `search_hotels` tool call captured
- error event captured
- retry behavior captured
- export created at local path: `exports/toy-trip-planner.json`
- regression case created at local path: `cases/toy-after-flights`
- generated pytest scaffold passed: `2 passed in 0.01s`

### GitHub receipts

AFR issue:

- `cwwjacobs/agent-flight-recorder#18`
- Title: `Stage 2 Task 1: Deep dependency and architecture triage`

Recent AFR PRs:

- `#15` merged: CLI-first repair spine and regression-case/eval seed flow
- `#16` merged: backend/CLI-first cleanup, React/UI removed from default path
- `#17` open/mergeable at time of capture: friendly CLI commands and `latest` selectors

### Current U-KSL state

```text
Ultra Stage 1: Map / Kernel / Boundary / Dispatch
```

The exit condition for this run is:

```text
We know what to upgrade first, why it matters, and what not to touch yet.
```

### Dispatch decision

Corrected model route:

```text
1. Gemini Pro / Flash scout pass
2. Codex 5.5 xhigh repo-grounded audit
3. Qwen/Gwen table/checklist compression
4. Maia/current instance Ultra-KSL synthesis
```

Reason:

- Gemini Pro/Flash scouts the broad question.
- Codex 5.5 xhigh performs the strongest repo-grounded audit after the scout sharpens the target.
- Qwen/Gwen compresses into operator tables.
- Maia/current instance performs Stage 3 verification and synthesis.

## Open TODO

- Add Gemini scout results when returned.
- Add Codex xhigh audit results when returned.
- Add optional Qwen/Gwen compression.
- Perform Ultra Stage 3 verification.
- Produce final artifact: `AFR Short-Term Upgrade Shape`.

## Qwen status update

Qwen CLI/API access was restricted during Stage 2 setup.

Decision:
- Qwen is optional for this loop.
- Qwen is not part of the critical path.
- Compression/table extraction can be done by Kimi, Codex, Maia/current instance, or another available engine.

Updated route:

```text
Gemini / Flash scout
-> Codex 5.5 xhigh repo audit
-> optional Kimi/compression pass
-> Maia/current instance Ultra Stage 3 synthesis
```

## Qwen status update

Qwen CLI/API access was restricted during Stage 2 setup.

Decision:
- Qwen is optional for this loop.
- Qwen is not part of the critical path.
- Compression/table extraction can be done by Kimi, Codex, Maia/current instance, or another available engine.

Updated route:

```text
Gemini / Flash scout
-> Codex 5.5 xhigh repo audit
-> optional Kimi/compression pass
-> Maia/current instance Ultra Stage 3 synthesis
cat >> runs/2026-06-24-afr-upgrade-scout-loop-86e00457362d/stage-log.md <<'EOF'

## Qwen status update

Qwen CLI/API access was restricted during Stage 2 setup.

Decision:
- Qwen is optional for this loop.
- Qwen is not part of the critical path.
- Compression/table extraction can be done by Kimi, Codex, Maia/current instance, or another available engine.

Updated route:

```text
Gemini / Flash scout
-> Codex 5.5 xhigh repo audit
-> optional Kimi/compression pass
-> Maia/current instance Ultra Stage 3 synthesis

```

## Qwen status update

Qwen CLI/API access was restricted during Stage 2 setup.

Decision:
- Qwen is optional for this loop.
- Qwen is not part of the critical path.
- Compression/table extraction can be done by Kimi, Codex, Maia/current instance, or another available engine.

Updated route:

```text
Gemini / Flash scout
-> Codex 5.5 xhigh repo audit
-> optional Kimi/compression pass
-> Maia/current instance Ultra Stage 3 synthesis

