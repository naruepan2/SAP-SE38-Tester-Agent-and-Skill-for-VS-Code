# SAP Reverse Engineer and Runtime Tester Agent/Skill History

This repository stores the current SAP ABAP Reverse Engineer V8.7.2, a reconstructed Runtime Tester V7 baseline, verified reverse-engineer release archives, and evidence-labeled history.

## Current production-oriented package

- Reverse Engineer Agent: `agents/sap-abap-reverse-engineer.agent.md`
- Reverse Engineer Skill: `skills/sap-abap-reverse-engineering/`
- Current version: `8.7.2`

## Reconstructed package

- Runtime Tester Agent: `agents/sap-abap-runtime-tester.agent.md`
- Runtime Tester Skill: `skills/sap-abap-runtime-testing/`
- Status: `V7 RECONSTRUCTED`, requiring connector/tool validation before production use

## History integrity

History is labeled as:

- `VERIFIED`: archive/source is bundled.
- `RECONSTRUCTED`: supported by historical design records but not the original release archive.
- `UNVERIFIED`: exact version boundaries cannot be proven and are not invented.

See:
- `CHANGELOG.md`
- `docs/HISTORY.md`
- `docs/DECISION_LOG.md`
- `docs/history/`

## Repository structure

```text
agents/
skills/
  sap-abap-reverse-engineering/
  sap-abap-runtime-testing/
docs/
  history/
releases/
  reverse-engineer/verified/
  runtime-tester/reconstructed/
benchmarks/runtime-tester/
release-assets/
```

## Safety separation

Reverse Engineer is strictly static/read-only and never executes programs. Runtime Tester has a separate execution-preflight gate and must not run without explicit approval of system, client, target, inputs, and operation.

## Upload

See `GITHUB_UPLOAD_INSTRUCTIONS.md`.
