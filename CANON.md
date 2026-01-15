

# STACK (/canonic/stack/)

inherits: /

---

## Axioms

### 1. Stack role

STACK defines the composition of multiple CANONIC machines into a single ordered system.

STACK **MUST** manage relationships between machines without altering their internal governance.

---

### 2. Ledger aggregation

STACK **MUST** aggregate multiple LEDGER instances into a unified, ordered multi-ledger view.

Each ledger **MUST** retain its own authority and immutability.

---

### 3. Non-interference

STACK **MUST NOT** introduce governance, enforcement, or execution semantics.

STACK **MUST NOT** modify, reinterpret, or override machine-local CANON or LEDGER state.

---

### 4. Ordering

STACK **MUST** define a deterministic ordering of machines and their corresponding ledgers.

Given identical inputs, STACK ordering **MUST** be reproducible.

---

### 5. Boundary preservation

STACK **MUST** preserve machine boundaries.

Cross-machine interaction **MUST** occur only through recorded LEDGER signals.

---

### 6. Logical inheritance

Inheritance paths declared in CANON files are logical, not physical.

- Paths like `/canonic/machine/os/` reference the stack hierarchy across repositories.
- Each repository declares its position in the logical hierarchy.
- The organization boundary defines the stack boundary.

---

### 7. Visibility enforcement

STACK membership **MUST** declare visibility for each repository.

Three visibility levels exist in order of increasing restriction:

1. **public** — Published with public visibility.
2. **private** — Published with private visibility.
3. **local** — Never published; no remote permitted.

Repositories marked `local: true` **MUST NOT** have a git remote configured.

Pushing a local repository to any remote is a governance violation.

---

### 8. Referential navigation

Each repository README **MUST** contain a stack navigation table.

The navigation table **MUST**:
- List all public stack members with markdown links
- Bold the current repository (no link)
- Link to governance artifacts (`CANON.md`, `VOCAB.md`) within the triad section

Cross-repo links enable seamless navigation across the multi-repository stack.

---

**This CANON defines validity for the STACK scope.**

---