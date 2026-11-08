# PrintBatch - development roadmap

**Status:** Planned work only. None of the boxes are marked completed. Estimates are rough.

## Product-level acceptance criterion

A sample fleet produces a feasible schedule with explicit constraints.

## Estimated work breakdown

| Step | Milestone | Estimated hours | Observable outcome |
|---|---|---:|---|
| 1 | Define constraint models | 8 | Machine/job schemas and synthetic cases |
| 2 | Implement baseline scheduler | 11 | Feasible assignments and explanations |
| 3 | Add alternative scheduling priorities | 9 | Comparisons with objective measures |
| 4 | Build scenario import/export | 8 | Repeatable CSV and JSON projects |
| 5 | Create local planning UI | 10 | User can inspect and adjust schedules |
| 6 | Tests, docs, and demo data | 10 | Documented end-to-end simulation |
| | **Total estimated** | **56** | |

## Detailed milestones

### 1. Define constraint models (8 estimated hours)

- [ ] Deliverable: Machine/job schemas and synthetic cases.
- [ ] Add tests or demonstrations proving the deliverable works.
- [ ] Record a genuine development commit and update documentation only after the work occurs.

### 2. Implement baseline scheduler (11 estimated hours)

- [ ] Deliverable: Feasible assignments and explanations.
- [ ] Add tests or demonstrations proving the deliverable works.
- [ ] Record a genuine development commit and update documentation only after the work occurs.

### 3. Add alternative scheduling priorities (9 estimated hours)

- [ ] Deliverable: Comparisons with objective measures.
- [ ] Add tests or demonstrations proving the deliverable works.
- [ ] Record a genuine development commit and update documentation only after the work occurs.

### 4. Build scenario import/export (8 estimated hours)

- [ ] Deliverable: Repeatable CSV and JSON projects.
- [ ] Add tests or demonstrations proving the deliverable works.
- [ ] Record a genuine development commit and update documentation only after the work occurs.

### 5. Create local planning UI (10 estimated hours)

- [ ] Deliverable: User can inspect and adjust schedules.
- [ ] Add tests or demonstrations proving the deliverable works.
- [ ] Record a genuine development commit and update documentation only after the work occurs.

### 6. Tests, docs, and demo data (10 estimated hours)

- [ ] Deliverable: Documented end-to-end simulation.
- [ ] Add tests or demonstrations proving the deliverable works.
- [ ] Record a genuine development commit and update documentation only after the work occurs.

## QA and release gates

- [ ] A real runnable implementation exists, with verified setup commands in `README.md`.
- [ ] Automated tests pass in a clean environment and failures are actionable.
- [ ] Only fabricated, original, openly licensed, or otherwise authorized sample data is published.
- [ ] No passwords, API keys, secrets, customer records, or employer/client confidential artifacts appear in repository history.
- [ ] A source-linked change log and actual progress notes distinguish finished work from plans.
- [ ] The GitHub history preserves authentic work and authorship; do **not** manufacture or backdate commits.

## Parking lot and risks

- Technical: Scheduling outcomes depend on inaccurate duration forecasts; keep estimates editable and clearly labeled.
- Commercial hypothesis (not validated): Pro scheduling modes and slicer integration add-ons.
- Beyond MVP: defer paid extensions and hosted features until the underlying product works.
