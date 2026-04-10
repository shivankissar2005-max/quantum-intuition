# Experiment Log

---

## Experiment 01 — X Gate

**Goal:** Understand deterministic behavior of a single qubit.

**Prediction:** Output should always be `1`.

**Result:** `{'1': 1000}`

**What I learned:** The X gate flips a qubit from 0 to 1. Unlike the H gate, it does not introduce randomness.

---

## Experiment 02 — H Gate

**Goal:** Observe randomness in a single qubit.

**Prediction:** Output should be about half `0` and half `1`.

**Result:** ~50/50 distribution

**What I learned:** The H gate creates a superposition, which results in probabilistic outcomes when measured.

---

## Experiment 03 — Independence

**Goal:** Compare independent qubits to entangled qubits.

**Prediction:** Outputs should be `00` and `01`.

**Result:** `{'01': 504, '00': 496}`

**What I learned:** Qubit 0 becomes random due to the H gate, while qubit 1 remains 0 because it is not affected by any gate. The qubits behave independently.

---

## Experiment 04 — Bell State

**Goal:** Create a two-qubit entangled state.

**Prediction:** Outputs should be `00` and `11`.

**Result:** `{'00': 492, '11': 508}`

**What I learned:** The CX gate transforms independent randomness into correlated outcomes. Instead of all combinations being possible, only matching states remain.

---

## Experiment 05 — Controlled Behavior

**Goal:** Understand the CX gate without randomness.

**Prediction:** Output should always be `11`.

**Result:** `{'11': 1000}`

**What I learned:** The CX gate flips the target qubit only when the control qubit is 1. This creates deterministic behavior when the control is fixed.

---

## Experiment 06 — GHZ State

**Goal:** Extend entanglement to three qubits.

**Prediction:** Outputs should be `000` and `111`.

**Result:** `{'111': 525, '000': 475}`

**What I learned:** Entanglement can extend across multiple qubits. All three qubits behave as a single system, producing only fully matched outcomes.

---

## Experiment 07 — Break Bell State

**Goal:** Test whether CX undoes itself.

**Prediction:** Outputs should be `00` and `01`.

**Result:** `{'01': 503, '00': 497}`

**What I learned:** Applying the same CX gate twice cancels its effect. The entanglement disappears, and the system returns to independent behavior.

---

## Experiment 08 — Break GHZ State

**Goal:** Undo part of a multi-qubit entangled system.

**Prediction:** Qubit 2 becomes unaffected while qubits 0 and 1 remain linked.

**Result:** `{'000': 504, '011': 496}`

**What I learned:** Removing one link in a multi-qubit system breaks part of the entanglement. Qubit 2 becomes independent again, while qubits 0 and 1 remain correlated.

---

## Experiment 09 — Partial Break GHZ

**Goal:** Change which qubits remain correlated by altering gate order.

**Prediction:** Qubits 0 and 2 remain linked, while qubit 1 becomes independent. Outputs should be `000` and `101`.

**Result:** `{'101': 502, '000': 498}`

**What I learned:** The order and placement of CX gates determines how correlations propagate. Entanglement is not just about which gates are used, but also when they are applied.