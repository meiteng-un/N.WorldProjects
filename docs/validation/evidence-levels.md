# Validation Evidence Levels

Use separate evidence levels so that one successful check does not hide an untested deployment path.

| Level | Evidence | What it proves | What it does not prove |
| --- | --- | --- | --- |
| L0 | File/source inspection | Intended fields, symbols, paths, and references exist | Unity serialization, compilation, or runtime behavior |
| L1 | Unity import/compile and fresh Console check | Unity accepted the source and current compile has no relevant errors | Scene installation, input, visual layout, or networking |
| L2 | Prefab/Scene serialization and reference audit | References and serialized fields are saved and non-missing | PlayMode behavior or VRChat client behavior |
| L3 | Unity PlayMode | Local state transitions, UI events, and reset/debug paths work in the editor | VRChat SDK runtime differences, real users, performance |
| L4 | VRChat Desktop/VR client | Actual input, rendering, Udon runtime behavior, and user-facing flow | Multi-user edge cases unless explicitly tested |
| L5 | Multi-user and performance/visual review | Synchronization, ownership, layout, frame cost, and device-specific behavior | Unrelated systems or future changes |

## Reporting rules

- Name the highest completed level and list lower-level evidence that supports it.
- List every relevant unverified level.
- Do not report a clean syntax analyzer as a clean Unity build.
- Do not report a clean build as working PlayMode or VRChat behavior.
- Do not claim a performance improvement without a measurement or profiler capture.
- When a long Unity operation times out, distinguish still running/unknown from failed.

## Suggested PR summary

```text
Validated: L0, L1, L2
Not validated: L3 PlayMode, L4 VRChat Desktop/VR, L5 multi-user/profiler
Evidence: <links to logs, screenshots, or files>
```