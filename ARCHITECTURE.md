<!--
SPDX-License-Identifier: AGPL-3.0-or-later
Commercial license available
© Concepts 1996–2026 Miroslav Šotek. All rights reserved.
© Code 2020–2026 Miroslav Šotek. All rights reserved.
ORCID: 0009-0009-3560-0851
Contact: www.anulum.li | protoscience@anulum.li
SC-NC-ENGINE — repository foundation
-->

# Architecture

## Current executable surface

The checkout contains:
- repository validation tooling;
- dedicated tests;
- workflow definitions;
- native documentation.

No domain component of SC-NC Engine is implemented yet, and no code has moved here from SC-NeuroCore. The metadata keeps domain capabilities, claims and qualified record formats empty.

## Intended records

1. **Execution plan:** Which models, populations, steps and backend lane a run uses.
2. **Checkpoint state:** The complete state of a run at a step, enough to resume it exactly.
3. **Trace summary:** A bounded summary of a run's events and state, with its source digests.

## Ownership

**This project owns** the planned SC-NC Engine records and boundary rules.

**Owned elsewhere:**

| Responsibility | Owner |
|---|---|
| models and model descriptors | SC-NC Catalogue |
| datasets, encoders and codecs | SC-NC Data |
| benchmarks and energy accounting | SC-NC Bench |
| the public package, documentation and releases of the monolith | SC-NeuroCore |

## Interpretation

- **Speed.** Lane parity is checked; no speed or throughput figure is claimed by this foundation.
- **Moves.** Code arrives only through SC-NeuroCore's split import gate, unit by unit; a planned move is not a moved capability.

Read [the documentation architecture](docs/ARCHITECTURE.md) for the planned records, rules and schema identifiers.
