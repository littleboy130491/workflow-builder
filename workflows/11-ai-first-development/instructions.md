# 11 AI First Development

## Brief Description

Implement the website using an AI-first workflow that still keeps code quality, design accuracy, and reviewability under control.

## Expected Input

- Relevant page copy from `outputs/05-copywriting/`
- Relevant files from `outputs/08-design-system/`
- Relevant files from `outputs/09-high-fidelity-design/`
- Relevant files from `outputs/10-technical-architecture/`

## Expected Outputs

Create the following files inside `outputs/11-ai-first-development/`:

- `build-log.md`: Execution log of the implementation work and major milestones
- `component-status.md`: Component progress, completeness, and unresolved issues
- `issues-and-decisions.md`: Implementation tradeoffs, deviations, and technical decisions
- `verification-checklist.md`: Design, content, accessibility, and functional verification results

## Success Criteria

- The implementation follows the approved content, design, and technical plan
- AI-generated work is reviewed and corrected as needed
- Deviations are documented instead of silently accepted
- Verification is performed during development, not only at the end

## Constraints

- Do not trust generated code without inspection
- Do not drift from the approved design and copy without recording the change
- Keep execution incremental and testable

## Execution Notes

- Use AI for bounded tasks such as component scaffolding, refactors, repetitive patterns, and issue triage
- Review generated code against design specs, content fidelity, responsiveness, and maintainability
