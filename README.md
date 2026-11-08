# PrintBatch

> Offline production scheduling for mixed 3D-printer fleets.

**Current state:** Documentation starter / proposed product. The presence of this README does **not** mean the software has been implemented, deployed, used. Update this status to reflect real work.

## What it is

PrintBatch is a proposed specialist software tool for Small 3D print farms, prototyping labs, and technical schools. Scheduling jobs across dissimilar printers is complicated when each machine has different build volume, material, and time requirements. The intended differentiation is: A transparent planning-only scheduler that does not depend on a single printer-cloud ecosystem.

## Intended users and use cases

- Schedule fictional PLA and PETG jobs on three printers
- Explain why a large model cannot fit a chosen build volume
- Compare batching to minimize hypothetical filament swaps

## Planned features

- Define printer capabilities and material compatibility rules
- Import synthetic job manifests including predicted print duration
- Assign jobs to machines using deterministic constraints
- Compare earliest-completion and material-change-minimizing schedules
- Export offline job calendars and explain unassigned jobs

## Proposed technology

Python 3.12+, FastAPI, SQLite, Svelte, pytest

These technologies are *planned*, not a claim that dependencies have already been installed or code has been written. Revise this section when actual implementation decisions are made.

## Proposed architecture

- Machine and job constraint schemas
- Greedy baseline and alternative scheduler
- Local schedule persistence
- Drag-and-drop planning UI

See [TECHNICAL_PLAN.md](TECHNICAL_PLAN.md) for technical boundaries and acceptance tests.

## Running locally

**Not yet runnable.** This package contains documentation templates, not software. When a functioning implementation is available, replace this paragraph with tested prerequisites, install instructions, a verified executable command, and a reproducible example using `Invented jobs, machine capabilities, and durations.`

## Data boundaries and exclusions

Remote printer control, real customer orders, personal information, or live cloud telemetry. All public examples should use Invented jobs, machine capabilities, and durations.

## Known limitations / validation risks

Scheduling outcomes depend on inaccurate duration forecasts; keep estimates editable and clearly labeled.

## Development roadmap

Work is broken into estimated, not-yet-completed milestones in [ROADMAP.md](ROADMAP.md). They are *planning estimates*, not an assertion that development has begun or that work will definitely be performed.

## Business direction

Potential commercial extensions: Pro scheduling modes and slicer integration add-ons. 

## Contributing and licensing

License: [Mozilla Public License 2.0](LICENSE) (`MPL-2.0`). The distribution contains the complete license text. Any future source files can include the SPDX identifier `MPL-2.0` and the Exhibit A notice where appropriate. Rights in contributions and project ownership must be verified before licensing.

