# MethodOps

Human-governed research CI/CD for simulation and methodological workflows.

## Core idea
MethodOps combines:
1. **Good-practice encoding via stage-specific `SKILL.md` policies**
2. **Hard human gates** at plan/codegen/release boundaries
3. **Iterative improvement** through versioned human feedback

This is designed to improve reliability, auditability, and scientific quality versus autonomy-first pipelines.

## Why this exists
Many AI research automation systems optimize for throughput. MethodOps optimizes for **governed quality**:
- explicit methodology policy context,
- enforceable checkpoints,
- reproducible artifacts and manifests,
- transparent claim–evidence–caveat discipline.

## MVP architecture
- `stages/01_planning_codegen/`: LLM-assisted ADEMP planning + code generation (with human approval)
- `stages/02_execution_interpretation/`: execution + diagnostics + LLM interpretation (with human approval)
- `policy/`: stage policies (`SKILL.md`) and checklists
- `artifacts/`: immutable run artifacts and manifests

## Current status
Early prototype (v0.1 concept + stage notebooks). Actively iterating on governance, portability, and policy enforcement.

## Roadmap (short)
- v0.1: stage-separated notebooks + policy placeholders + gating
- v0.2: executable validators for policy compliance
- v0.3: end-to-end orchestrator with pluggable backends
- v1.0: stable governed research pipeline + benchmark suite

## Citation
If you use this concept/framework, cite via `CITATION.cff`.

## Contact
Open an issue for collaboration or design feedback.
