# M3E4Unity

- Status: Reference only / Candidate
- Repository: https://github.com/NarYuki/M3E4Unity
- Repository owner: NarYuki
- Default branch checked: `main`
- Retrieved: 2026-10-12
- License: Apache License 2.0
- Related notice: repository README states that third-party notices are provided in `NOTICE`; bundled fonts may use Apache-2.0 or SIL Open Font License 1.1.

## What was confirmed

The public README describes M3E4Unity as a Material 3 Expressive implementation for Unity uGUI with support for ordinary Unity and VRChat/UdonSharp use.

The package layout described by the repository includes:

- `Packages/com.m3e4unity/` as the Unity package
- Runtime core, Udon/runtime behaviours, markers, showcase, and Editor builders
- Shaders and fonts
- Tests and porting/generation tools

The README also describes VCC/ALCOM, UPM Git URL, and release-based installation paths. These are reference information only; installation into N.Worlds Project has not been performed.

## Potential value for N.Worlds

- Compare Material 3 tokens, shape, motion, typography, and component composition with existing N.IntegratedMenu/N.WIM UI.
- Use the repository's Udon-specific differences as a checklist before considering a UI library.
- Compare its theme asset and editor-builder workflow with the existing Naturlin inspector and prefab conventions.
- Use its compile/golden-test separation as a model for library-level validation.

## Known constraints to carry into evaluation

The README documents VRChat/Udon differences such as tap-based time-dial input instead of drag input, delayed date separator insertion, and limitations around text-field focus, font sizing, and caret styling. These must be tested against actual N UI input paths rather than assumed compatible.

## Copying and licensing boundary

No M3E4Unity source code, shader, font, screenshot, or asset was copied into N.WorldProjects by this reference intake.

If future work adapts code or assets:

- preserve the Apache-2.0 license;
- retain required copyright, license, and NOTICE attribution;
- check each bundled font and third-party dependency separately;
- record the exact source tag/commit and modified files;
- perform a legal/licensing review before redistribution.

## Next evaluation

Before adoption, create a separate design note comparing:

- dependency and package layout;
- uGUI/EventSystem and Udon event routing;
- Desktop and VR input;
- synchronization and ownership;
- shader compatibility and performance;
- Japanese font and localization requirements;
- inspector and prefab authoring workflow;
- PlayMode and VRChat client validation.

No adoption decision has been made.