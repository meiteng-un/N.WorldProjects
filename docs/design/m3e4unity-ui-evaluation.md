# M3E4Unity UI Evaluation

- Status: Proposed
- Related reference: [M3E4Unity](../external-references/M3E4Unity.md)
- Scope: N.IntegratedMenu / N.WIM UI comparison only

## Goal

Determine whether M3E4Unity should influence visual tokens, component composition, or authoring workflow in N.Worlds without breaking existing Naturlin UI input, UdonSharp, synchronization, and prefab contracts.

## Evaluation order

1. Inventory current N UI components, input routes, theme fields, and prefab references.
2. Compare component behavior and dependencies without installing or replacing the current UI.
3. Prototype one isolated panel or component.
4. Validate EventSystem, Desktop, VR pointer, follow/lock, reset/debug, and Udon event routes.
5. Check package size, shader/material cost, font licensing, and build compatibility.
6. Record evidence at L0-L5 in [validation levels](../validation/evidence-levels.md).
7. Make an explicit Accepted or Rejected decision in `docs/decisions/`.

## Acceptance criteria

- Existing N UI public/serialized field contracts remain stable.
- Existing input paths do not silently change.
- UdonSharp compile and serialized Program Assets remain valid.
- Japanese text, font fallback, and localization remain usable.
- Desktop and VR interaction are both tested.
- Visual and performance changes are measured rather than assumed.
- Required third-party notices can be distributed with the resulting world/package.

## Current decision

Do not install or replace the existing UI based on README similarity alone. Treat M3E4Unity as a reference and isolated candidate until a small prototype passes the evaluation order.