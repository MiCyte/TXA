# TXA

Documentation for MiCyte's taxonomy: the `txa` tree and `txa_registry` in the taxonomy
sandbox, and the archetypes that read them (plant profiles, plantae entries, the TXA local
domain source and its viewscope).

TXA is the shared classification instances denote their records against: a crop, a plant
or a product names its place in the tree rather than spelling it, so two instances that
mean the same species write the same address.

## What this repository is, and is not

It organizes and documents the taxonomy: its branches, how a node is addressed, how a node
joins a profile, and how the tree is changed without breaking what cites it. It is **not**
how an instance uses TXA. On the network the taxonomy is an MSS binary payload served over
the MSN protocol, and that payload is what an instance reads and verifies.

## Layout

| path | what it documents |
|---|---|
| `tree/` | the branches of `txa` and how a node is addressed |
| `registry/` | `txa_registry`: the named entries and their joins |
| `archetypes/` | the documents that read TXA: plant profiles, plantae entries, local domain source |
| `changes/` | how a node is added, moved or retired, and what that costs the documents citing it |

The folders fill as each part is documented. The core software, its versioning and its wiki
are in [MiCyte/MiCyte](https://github.com/MiCyte/MiCyte).

## Licence

AGPL-3.0, the same as the core.
