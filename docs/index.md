<!--
SPDX-License-Identifier: AGPL-3.0-or-later
Commercial license available
© Concepts 1996–2026 Miroslav Šotek. All rights reserved.
© Code 2020–2026 Miroslav Šotek. All rights reserved.
ORCID: 0009-0009-3560-0851
Contact: www.anulum.li | protoscience@anulum.li
SC-NC-ENGINE — repository foundation
-->

# SC-NC Engine

SC-NC Engine is being built as the simulation engine split out of SC-NeuroCore: the execution plans that run catalogued models over time, the native Rust and accelerated lanes that run them, and the checkpoint state and trace summaries that make a run resumable and comparable. It imports only SC-NC Core and SC-NC Catalogue. Its current executable surface is repository validation tooling. It has no installed execution engine, native-lane runner, checkpoint store or qualified record schema.

Read [Architecture](ARCHITECTURE.md), [validation tooling](validation-tooling.md), [data boundaries](THREAT_MODEL.md) and the [repository boundary decision](adr/0001-repository-boundary.md).
