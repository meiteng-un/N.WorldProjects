# N.Worlds Project Baseline

- Status: Maintained reference
- Scope: Naturlin VRChat World / UdonSharp work
- Last reviewed: 2026-10-12

## Storage and naming

- New Naturlin systems use an `N.<Category>/N.<GimmickName>/` structure.
- Keep Runtime, Editor, Prefabs, and Docs separated where the system needs them.
- Use an `N` prefix, underscores instead of spaces for new asset names, and existing project naming conventions.
- Treat Scene files, archives, and editor-only assets as protected areas unless the task explicitly requires them.

## N.Script and Inspector

- N.Script components use the shared Naturlin inspector contract when available.
- Inspector labels and controls should support Japanese and English.
- Program Source, Program Script, Synchronization Method, and Utilities are hidden unless a task explicitly requires them.
- Lock controls are resolved before language or display settings.
- Missing-only reference repair is lightweight and must not become an automatic scene-wide rebuild.
- Duplicate candidates should be warned about rather than silently selected.

The shared editor contract includes the common base, scene cache, validation, lock state, Undo recording, and correct reacquisition of array-element properties after resize or reorder.

## UdonSharp authoring

A new UdonSharp system is not complete when the C# file merely parses. A valid prefab/system pass also needs:

- UdonSharp-aware component creation
- a backing UdonBehaviour
- a valid Program Asset and source reference
- a runtime assembly marker when the assembly requires one
- compile/refresh confirmation
- serialized prefab and scene reference checks

## UI and input

For interactive world-space UI, trace the complete EventSystem and pointer path:

- Desktop input
- VR pointer/touch input
- follow, lock, grab, resize, and dock state
- EventTrigger or equivalent event wiring
- Udon event routing
- visual feedback and reset/debug behavior

A static event count, clean source analysis, or saved Scene is not proof that real Desktop or VR interaction works.

## Operational boundary

This document records project conventions and reusable checks. It is not a claim that every existing Scene, Prefab, or feature currently satisfies them. Record feature-specific verification in the relevant error, design, note, or PR document.