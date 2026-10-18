# 2026-10-12: Public GitHub reference intake

## Confirmed capability

The connected GitHub integration can read public repositories and, when permissions allow, read private repositories owned by the authenticated account. It can retrieve repository metadata, directory listings, text files, search results, issues, pull requests, and related read-only resources.

The same connection can create branches, files, commits, and pull requests in repositories where the account has write permission. External public repositories remain read-only unless their owner grants access.

## Checked source

- [M3E4Unity](https://github.com/NarYuki/M3E4Unity)
- README
- LICENSE
- repository metadata and package layout

## Classification

- External reference: `docs/external-references/M3E4Unity.md`
- Possible future UI design comparison: `docs/design/m3e4unity-ui-evaluation.md`
- No code or asset imported
- No package installed
- No source repository modified

## Working rule

External information may influence an implementation plan, but the final behavior must be validated against the current N.Worlds Unity project, installed SDK/package versions, Naturlin naming/storage rules, UdonSharp constraints, and actual Scene/Prefab wiring.