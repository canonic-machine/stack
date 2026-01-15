# STACK

The composition layer for multiple CANONIC machines.

---

## Overview

STACK aggregates multiple LEDGER instances into a unified, ordered multi-ledger view without introducing governance or altering machine-local state.

---

## Membership

Public membership is open; see [`public/STACK.yml`](public/STACK.yml) for the tracked repositories.

A private overlay may include closed repositories. STACK is observational: it records membership but does not govern member behavior.

Enforcement is a private role; its outcomes appear in the ledger.

Member repository roots are expected to include `LICENSE` and `NOTICE` per [`/canonic/CANON.md`](https://github.com/canonic-machine/canonic/blob/main/CANON.md). STACK may report compliance but does not enforce it.

---

## Triad

| Artifact | Purpose |
|----------|---------|
| [CANON.md](CANON.md) | Governance axioms |
| [VOCAB.md](VOCAB.md) | Vocabulary definitions |
| [README.md](README.md) | This file (non-normative) |

---

## Stack Navigation

| Layer | Repository | Purpose |
|-------|------------|---------|
| Root | [canonic](https://github.com/canonic-machine/canonic) | Constitutional foundation |
| Enforcement | [machine](https://github.com/canonic-machine/machine) | Execution semantics |
| Bounds | [os](https://github.com/canonic-machine/os) | Operational scope |
| Record | [ledger](https://github.com/canonic-machine/ledger) | Immutable evidence |
| Production | [writing](https://github.com/canonic-machine/writing) | Episode creation |
| Publication | [paper](https://github.com/canonic-machine/paper) | Manuscript artifacts |
| Execution | [agents](https://github.com/canonic-machine/agents) | Subordinate AI |
| Composition | **stack** | Multi-repo layer |

---
