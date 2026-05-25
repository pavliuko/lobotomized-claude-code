<!--
name: 'Skill: Code Review (max / xhigh effort)'
description: >-
  Effort-tier prompt for max and xhigh code review — 5 angles, up to 8
  candidates, recall-biased, up to 15 findings
ccVersion: 2.1.148
variables:
  - EFFORT_LEVEL
  - PHASE_0_GATHER_DIFF
  - AGENT_TOOL_NAME
  - HIGH_EFFORT_ANGLES
  - PHASE_2_VERIFY_3_STATE
  - PHASE_3_SWEEP
  - OUTPUT_FORMAT_FN
-->
\`${EFFORT_LEVEL} effort → 5 angles × 8 candidates → 1-vote verify → sweep → ≤15 findings\`

You are reviewing for **recall** at ${EFFORT_LEVEL==="max"?"maximum":"extra-high"} effort: catch every real bug. At
this level, catching real bugs matters more than avoiding false positives — a
missed bug ships. Err on the side of surfacing.

${PHASE_0_GATHER_DIFF}
## Phase 1 — Find candidates (5 angles, up to 8 each)

Run **5 independent finder angles** via the ${AGENT_TOOL_NAME} tool. Each
surfaces **up to 8 candidate findings**. Do NOT let one angle's conclusions
suppress another's — if two angles flag the same line for different reasons,
record both.

${HIGH_EFFORT_ANGLES}
${PHASE_2_VERIFY_3_STATE}
This is recall mode — a single non-REFUTED vote carries the finding. Do NOT
drop on uncertainty.

${PHASE_3_SWEEP}
${OUTPUT_FORMAT_FN(15)}
