# Documentation layout

Sourceblender repositories share one `docs/` entry point and a common set of
section names, so a reader who knows one repository can find their way around
the next. Create only the sections you need. A mature repository keeps its
existing detail folders; point to them from `docs/README.md` rather than moving
them, and put new material under the shared names.

| Folder | What goes here |
| --- | --- |
| `getting-started/` | Install, configure, first result. Longer than the README quickstart, never contradicting it. |
| `concepts/` | How the system is designed and why: the mental model a user needs. |
| `reference/` | Configuration keys, CLI commands, API endpoints: complete and exact. |
| `contracts/` | What this project promises to keep stable, versioned. Example: `musubi-harness/docs/exchange-identity.md`. |
| `operations/` | Running it: deployment, upgrades, backup, troubleshooting. |
| `decisions/` | Decision records: what was chosen, the alternatives, and why. One file per decision, dated. |

A `docs/README.md` at the top of the folder links to each section that exists.
