# Low-token role workflow

## Roles and defaults

| Role | Model / effort | Output |
| --- | --- | --- |
| User | Human | Goal, constraints, material choices |
| Coordinator | gpt-6.1-sol / low | Scope, assignment, decisions, final review |
| Research | gpt-6-luna / medium | Relevant sources, verified facts, open questions |
| Product/UI design | gpt-6-luna / medium | Behavior, layout, alternatives, acceptance criteria |
| Code design/implementation | gpt-6-astra / low | Interfaces, state, code changes, risks |
| Integration/report | gpt-6-luna / medium | Applied changes, evidence, issues and next actions |

Roles are responsibilities, not mandatory separate agents. The coordinator may perform any small role directly.

## Dispatch

- Small fixes, skill/config edits, cheap reads, Unity health/schema checks and compilation waiting stay with the main agent.
- Spawn only when the saved work exceeds context/tool overhead; prefer one bounded specialist and reuse it.
- Research and design may share one Luna agent. A routine implementation with settled design needs no Astra pass.
- Use explicitly requested model/effort when supported. Verify current tool availability; report unavailable combinations. These instructions cannot switch the already-running main model; use the app model selector for that.
- Increase effort/model only when unresolved ambiguity, difficult failures or observed quality justify it.
- Parallelize independent scopes; sequence design-dependent implementation. Assign each file and Unity operation to one writer.
- Ordinary Unity operations stay on the main agent under the user's efficiency rules. A separate integration agent is appropriate only for sufficiently substantial independent work with access to the required tools; otherwise Luna provides a bounded report/review and the main agent applies changes.

## Minimum handoff

Provide goal, exact paths/objects, relevant decisions, constraints, acceptance checks and requested output. Prefer file/commit links and small excerpts. Do not fork full history by default or resend full logs, manuals or tool registries.

Research output: relevant links with purpose labels, facts, recommendation and unresolved points.
Design output: behavior/interfaces/state, affected paths, conflicts and checks.
Implementation output: changed paths/commit, verification evidence, unresolved failures and next action.

Aim for roughly 300-600 words per handoff/report, extending only for necessary code or evidence. Reuse artifacts; do not re-investigate settled results.

## Review and storage

Coordinator reads the diff and specialist result once, checks consequential claims, then consolidates problems/improvements. No automatic second full investigation.

For substantial work, use docs/tasks/<task-slug>/ with a single brief.md and report.md; split research/design files only when they are materially useful. Cross-task standards belong in project-context/ or validation/; sources in external-references/; accepted decisions in decisions/; reproducible failures in errors/. Link documents instead of copying them.

Documentation/GitHub updates need no Unity compile. Actual implementation uses targeted compile/reference/input checks and explicitly records untested paths. Token reduction is a design objective; do not claim measured savings without usage data.
