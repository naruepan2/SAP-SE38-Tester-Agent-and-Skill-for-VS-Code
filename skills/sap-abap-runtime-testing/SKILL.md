---
name: sap-abap-runtime-testing
description: controlled sap abap runtime testing with execution preflight, first-divergence analysis, root-cause evidence, defect chains, comparison, prioritization, coverage, and runtime test reporting. use for approved se38 reports, function modules, classes, methods, and related executable targets.
---
# SAP ABAP Runtime Testing

## Status
This is a reconstructed V7 baseline derived from historical design records. Treat connector names and execution operations as capability classes until validated in the current environment.

## Load policy
- Always: `references/safety-and-execution-policy.md`, `references/user-input-handshake.md`.
- Preflight: `references/execution-preflight.md`, then the relevant target section in `references/target-playbooks.md`.
- Analysis: `references/first-divergence-engine.md`, `references/root-cause-and-defect-chain.md`, and `references/defect-pattern-library.md`.
- Comparison: `references/snapshot-and-comparison.md`.
- Finish: `references/prioritization-coverage-and-reporting.md` and `templates/runtime-test-report-template.md`.

## State
Maintain approved execution scope, system/client/target identity, inputs, expected behavior, execution evidence, snapshots, observations, first divergence, hypotheses, defect chains, findings, coverage, limitations, and completion status.

## Workflow
1. Confirm execution permission and exact target.
2. Reject write, posting, scheduling, transport, configuration, or unknown-side-effect operations.
3. Build a bounded test plan with stop conditions.
4. Execute only approved scenarios using verified tools.
5. Compare expected and actual evidence.
6. Identify first divergence, root cause, downstream effects, and visible symptoms.
7. Prioritize confirmed findings and separate hypotheses.
8. Generate and validate the report.
