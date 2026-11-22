<!--
SPDX-License-Identifier: AGPL-3.0-or-later
Commercial license available
© Concepts 1996–2026 Miroslav Šotek. All rights reserved.
© Code 2020–2026 Miroslav Šotek. All rights reserved.
ORCID: 0009-0009-3560-0851
Contact: www.anulum.li | protoscience@anulum.li
SC-NC-ENGINE — repository foundation
-->

# Repository architecture

## Current executable tooling

**What it contains:** the repository's metadata, source-provenance, workflow, dependency-alignment, documentation, inventory and preflight controls.

**What each control does:** it inspects its fixed, declared local scope.

**What received metadata cannot do:** select another acceptance policy or grant domain authority.

Foundation qualification is in progress.

## Intended domain boundaries

| Record | Responsibility | Required evidence |
| --- | --- | --- |
| Execution plan | Which models, populations, steps and backend lane a run uses | Plan checks against the catalogue and the selected backend |
| Checkpoint state | The complete state of a run at a step, enough to resume it exactly | Resume from a checkpoint gives the same continuation as the uninterrupted run |
| Trace summary | A bounded summary of a run's events and state, with its source digests | Summary checks against the full trace it summarises |

## Planned record schemas

- `sc_nc_engine.execution_plan.v1`
- `sc_nc_engine.checkpoint_state.v1`
- `sc_nc_engine.trace_summary.v1`

These are planned identifiers. None of them is registered or qualified here.

Read [validation tooling](validation-tooling.md) for the executable repository interfaces.
