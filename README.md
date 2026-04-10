# Quantum Computing — Intuition & Circuits

> Learning quantum computing by building, predicting, and experimenting with circuits in Qiskit.

---

## Purpose

This project documents my process of developing intuition for quantum computing through hands-on experiments.

Instead of focusing on theory, I use a simple approach:
- Predict what a circuit will do  
- Run the circuit  
- Compare the result  
- Explain what happened  

---

## What I Learned

- How the **X gate** creates deterministic behavior  
- How the **H gate** creates randomness  
- The difference between **independent qubits** and **entangled qubits**  
- How to build **Bell states** and **GHZ states**  
- How entanglement can be **created, modified, and broken**  
- How the **order of gates affects outcomes**  

---

## Project Structure

- `experiments/` — Python files for each circuit experiment  
- `notes/experiment_log.md` — predictions, results, and explanations  

---

## Example Insight

In one experiment, I created a GHZ state and then partially broke it by changing the order of gates.

**Result:**
- Outputs: `000` and `101`

**Insight:**
- Entanglement is not just about which gates are used, but also when they are applied.
- Changing the order of operations changes which qubits remain correlated.

---

## Tools Used

- Python  
- Qiskit  
- Qiskit Aer  

---

## Goal

Build intuition, not just follow tutorials.
