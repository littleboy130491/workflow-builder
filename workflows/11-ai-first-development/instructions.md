# 11 AI First Development

## Brief Description

Implement the website using an AI-first workflow that still keeps code quality, design accuracy, and reviewability under control.

## Expected Input

- Relevant page copy from `/home/henry/Desktop/projects/web-designer/outputs/05-copywriting/`
- Relevant files from `/home/henry/Desktop/projects/web-designer/outputs/08-design-system/`
- Relevant files from `/home/henry/Desktop/projects/web-designer/outputs/09-high-fidelity-design/`
- Relevant files from `/home/henry/Desktop/projects/web-designer/outputs/10-technical-architecture/`

## Expected Outputs

Create the following files inside `/home/henry/Desktop/projects/web-designer/outputs/11-ai-first-development/`:

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
- Do not modify files outside `/home/henry/Desktop/projects/web-designer/outputs/11-ai-first-development/` unless the user explicitly asks for build artifacts or source changes elsewhere

## Execution Notes

- Use AI for bounded tasks such as component scaffolding, refactors, repetitive patterns, and issue triage
- Review generated code against design specs, content fidelity, responsiveness, and maintainability
- Keep the build log and verification artifacts current enough that another agent could resume work safely

## Stop Conditions Or Approval Gates

- Stop and ask the user if required content, design, or technical inputs are missing
- Stop and ask the user if a requested implementation change conflicts materially with approved copy, design, or architecture outputs
- Stop and ask the user before taking irreversible actions, external deployments, or any step that would modify production systems
