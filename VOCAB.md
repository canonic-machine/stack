# VOCAB (/canonic/stack/)

---

## Content Concepts

### aggregation

The process of combining multiple ledgers into a unified view.

---

### authority

The property of being the definitive source of truth.

---

### boundary

The separation between machines in a STACK.

---

### CANON

The governance artifact of a scope.

---

### CANONIC

The constitutional governance paradigm that defines the minimal structural and semantic rules all scopes must satisfy.

---

### composition

The combination of multiple machines into a single ordered system.

---

### enforcement

The process by which MACHINE evaluates states against CANON.

---

### execution

The realization of state transitions.

---

### governance

The set of axioms that define validity.

---

### immutability

The property that persisted history cannot be altered.

---

### LEDGER

The authoritative record of state transitions.

---

### machine

An independent CANONIC system with its own governance.

---

### ordering

The deterministic sequence of machines and their ledgers.

---

### scope

A directory governed by a triad.

---

### signal

A recorded LEDGER event enabling cross-machine interaction.

---

### STACK

The composition layer for multiple CANONIC machines.

---

### logical inheritance

Cross-repository inheritance where inheritance paths reference the logical stack hierarchy rather than physical file paths. Each repository declares its position in the governance hierarchy via inheritance paths like `/canonic/machine/os/` even though these paths exist across separate repositories unified by the STACK.

---

### multi-repository stack

A STACK composed of separate git repositories unified under a single organization, where the organization boundary defines the stack boundary.

---

### visibility

The access control level for a repository in the STACK. Three layers exist in order of increasing restriction:

1. **public** — Open to all; published on GitHub with public visibility.
2. **private** — Restricted to organization members; published on GitHub with private visibility.
3. **local** — Never published; exists only on local machines with no remote.

Local is the strongest privacy level. A repository marked `local: true` MUST NOT have a remote configured.

---
