# 12 QA Launch Handoff

## Brief Description

Validate the website for launch readiness and produce the operational documentation needed for deployment and handoff.

## Expected Input

- Relevant files from `/home/henry/Desktop/projects/web-designer/outputs/11-ai-first-development/`
- Prior strategic, content, design, and technical outputs as validation references

## Expected Outputs

Create the following files inside `/home/henry/Desktop/projects/web-designer/outputs/12-qa-launch-handoff/`:

- `qa-report.md`: Findings across functionality, responsiveness, accessibility, content fidelity, and visual consistency
- `launch-checklist.md`: Pre-launch checks, deployment checks, analytics readiness, and rollback considerations
- `handoff.md`: Final handoff notes, maintenance considerations, and known issues

## Success Criteria

- Critical issues are identified clearly
- Launch readiness is assessed honestly
- Handoff documentation is sufficient for another person or agent to continue work safely

## Constraints

- Do not mark the site as launch-ready if critical issues remain
- Keep known issues explicit and prioritized
- Do not modify files outside `/home/henry/Desktop/projects/web-designer/outputs/12-qa-launch-handoff/`

## Execution Notes

- Validate the build against the original strategic, content, and design intent, not only against code-level correctness
- Separate critical launch blockers from minor polish items
- Make it clear which issues must be fixed before launch and which can be deferred safely

## Stop Conditions Or Approval Gates

- Stop and ask the user if the implementation outputs needed for validation are missing or incomplete
- Stop and ask the user before declaring launch readiness when unresolved issues remain ambiguous in severity
- Stop and ask the user if deployment or handoff requirements are unclear and materially affect the launch checklist
