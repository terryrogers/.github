<!-- repository-standard: schema=1; standard=Repository Standards; version=1.1.0; scope=local-required; source=local -->
# Conditional Repository Documents

Add these files only when their trigger applies. Record each applicable document in the repository profile, and do not create empty files or placeholder folders.

| File | Add When |
| --- | --- |
| `ARCHITECTURE.md` | The design is not obvious from the source tree. |
| `ROADMAP.md` | A public development direction is intentionally maintained. |
| `GOVERNANCE.md` | Multiple maintainers or organisations share decisions. |
| `CITATION.cff` | Software, research, data, or hardware should be academically cited. |
| `NOTICE` | A licence or bundled dependency requires attribution notices. |
| `THIRD_PARTY_NOTICES.md` | The distributed artifact contains material third-party components. |
| `MIGRATION.md` | Releases introduce significant upgrade or data-migration steps. |
| `DEPRECATIONS.md` | Users need a consolidated deprecation schedule. |
| `RELEASING.md` | Maintainers need a repository-visible release procedure. |
| `.github/FUNDING.yml` | The project accepts sponsorship. |
| `MAINTAINERS.md` | Maintainer responsibilities are public & not adequately represented by `CODEOWNERS`. |

Use one canonical architecture document. Choose root `ARCHITECTURE.md` for a compact standalone overview or `docs/architecture.md` when the detail belongs in a broader documentation set. If both are justified, keep the root file to a concise summary & link.
