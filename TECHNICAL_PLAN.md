# PrintBatch - technical plan

**Planning document, not an implementation report.**

## Product objective

A transparent planning-only scheduler that does not depend on a single printer-cloud ecosystem.

## Intended system boundary

- **Input:** Invented jobs, machine capabilities, and durations.
- **Processing stages:** Machine and job constraint schemas; Greedy baseline and alternative scheduler; Local schedule persistence; Drag-and-drop planning UI.
- **Output:** A sample fleet produces a feasible schedule with explicit constraints.
- **Runtime / build stack (tentative):** Python 3.12+, FastAPI, SQLite, Svelte, pytest
- **Explicitly excluded:** Remote printer control, real customer orders, personal information, or live cloud telemetry.

## Functional modules

- Define printer capabilities and material compatibility rules
- Import synthetic job manifests including predicted print duration
- Assign jobs to machines using deterministic constraints
- Compare earliest-completion and material-change-minimizing schedules
- Export offline job calendars and explain unassigned jobs

## Demonstration and acceptance cases

**Test 1:** Schedule fictional PLA and PETG jobs on three printers

**Test 2:** Explain why a large model cannot fit a chosen build volume

**Test 3:** Compare batching to minimize hypothetical filament swaps

## Safety, privacy, and provenance

1. Keep example datasets fictional, self-created, or appropriately licensed.
2. Run locally for the initial prototype; do not collect data on actual third parties.
3. Document origin and versions of external specifications and dependencies.
4. Exclude production credentials; put environment variable *names* only in `.env.example` if required later.
5. Do not make certification, legal compliance, professional safety, or performance guarantees without independent validation.

## Engineering unknowns and constraints

Scheduling outcomes depend on inaccurate duration forecasts; keep estimates editable and clearly labeled.

## Release definition

A first release requires a runnable prototype, verified README instructions, automated tests tied to the three demonstrations, the full LICENSE file, and an honest public GitHub development history. The roadmap estimates are hypotheses until reviewed during implementation.
