

# STACK

inherits: /canonic/machine/os/

---

## Purpose

Define STACK as the observational composition layer for multiple CANONIC machines.

STACK provides a unified, read-only view across independent machines by observing their published artifacts and ledgers.

STACK does not govern, enforce, execute, or interpret.

---

## Scope

- Applies to `/canonic/machine/os/stack/`.
- Inherits constraints from the OS scope.
- Operates exclusively through observation of existing machines.

---

## Normative language

The key words **MUST**, **MUST NOT**, **SHOULD**, **SHOULD NOT**, and **MAY** are to be interpreted as described in RFC 2119.

Statements using these key words are normative. All other text is descriptive.

---

## Principles

### 4.1 Observational role

STACK is observational only.

STACK does not introduce authority, behavior, or policy.

---

### 4.2 Ledger-first coordination

STACK coordinates machines solely through their published LEDGER history.

No direct state sharing or implicit coupling between machines is permitted.

---

### 4.3 Structural normalization

STACK MAY project published machine artifacts into a common representation for observation.

Such normalization is structural only and MUST NOT alter meaning, add semantics, or introduce interpretation.

---

### 4.4 Deterministic observability

STACK MUST define a deterministic ordering across observed ledger events.

Ordering exists to support reproducibility and replay, not interpretation.

---

## Constraints

- STACK **MUST** reference machines only through their published CANON and LEDGER artifacts.
- STACK **MAY** materialize a normalized descriptor view derived from those published artifacts.
- STACK **MUST** define the domain of events it orders (e.g., commits, tags, episodes).
- STACK **MUST NOT** modify, annotate, or reinterpret ledger history.
- STACK **MUST NOT** introduce governance, enforcement, or execution behavior.

---

## Validation

A STACK scope is valid if and only if:

- it observes machines exclusively via published artifacts,
- ordering is deterministic and reproducible,
- normalization is structural only, and
- no authority or interpretation is introduced.

---

## Consumption notes

- STACK output is read-only and informational.
- STACK may be used to reconstruct cross-machine timelines.
- STACK output may inform analysis but has no canonical force.
- Compliance reports may include repository-root `LICENSE` and `NOTICE` checks per `/canonic/CANON.md`.

---

**This file defines the STACK law.**

---
