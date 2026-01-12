

# STACK

## 1. Purpose

Define the STACK scope as the composition layer for multiple CANONIC machines.

STACK exists to coordinate and observe multiple machines and their ledgers as a single ordered system, without introducing governance, enforcement, or execution behavior.

---

## 2. Scope

- Applies to `/canonic/stack/`.
- Inherits directly from `/`.
- Operates across multiple independent CANONIC machines.

---

## 3. Normative language

The key words **MUST**, **MUST NOT**, **SHOULD**, **SHOULD NOT**, and **MAY** are to be interpreted as described in RFC 2119.

Statements using these key words are normative. Examples and diagrams are non-normative unless explicitly marked otherwise.

---

## 4. Principles

### 4.1 Composition without authority

STACK composes machines without exercising authority over them.

Each machine retains its own governance, enforcement semantics, and local validity rules.

---

### 4.2 Ledger-first coordination

STACK coordinates machines exclusively through their respective LEDGER instances.

No direct state sharing or implicit coupling between machines is permitted.

---

### 4.3 Deterministic observability

STACK provides a deterministic, reproducible view of machine activity by ordering ledger events.

Given identical machine inputs and ledgers, STACK observations are identical.

---

## 5. Constraints

- STACK **MUST** reference machines only through their published CANON and LEDGER artifacts.
- STACK **MUST** aggregate multiple LEDGER instances into a unified, ordered multi-ledger view.
- STACK **MUST** define a deterministic ordering across machines and their ledger events.
- STACK **MUST NOT** introduce governance, enforcement, execution semantics, or interpretation.
- STACK **MUST NOT** modify, rewrite, or reinterpret machine-local LEDGER history.

---

## 6. Validation

A STACK scope is valid if and only if:

- the triad (`CANON.md`, `VOCAB.md`, `README.md`) is present,
- all referenced machines are valid CANONIC machines,
- ledger aggregation preserves per-machine immutability, and
- ordering is deterministic and reproducible.

---

## 7. Consumption notes

- STACK may be used to analyze, observe, or replay activity across multiple machines.
- STACK output is observational and non-authoritative.
- Governance changes require explicit updates within individual machine CANON scopes.

---

**This SPEC is descriptive and non-authoritative.**  
**Governance is defined exclusively by CANON.**

---