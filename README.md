# QuantumJam 2025: BB84 QKD on Noisy Simulators

**Authors:** Juan Quiroga Bonetto, Naomi Couriel, Ana Paula Tissera, and Athina Salim

## 1. The Problem: The Decline of RSA and the Dual Quantum Solution

Current public-key cryptography (such as RSA) is based on mathematical problems that are intractable for classical computers. However, Shor’s algorithm makes them trivial for a quantum computer, creating an existential threat to our secure communications.

In response, the scientific community has proposed two distinct solutions:

1. **Post-Quantum Cryptography (PQC):** Classical algorithms (based on mathematics) believed to be resistant to quantum attacks.  
2. **Quantum Key Distribution (QKD):** Protocols that use quantum physics to distribute a key. Their security is not based on mathematical assumptions, but on the laws of nature.

## 2. Our Mission: From the Ideal Model to the Chaos of Noise

In the notebook shown in `hackathon.ipynb`, we implement the **BB84** protocol, the cornerstone of QKD.

But we don’t stop at an ideal simulation. Our goal is to investigate the protocol’s practical viability. To do this, we use `NoiseModel` from Qiskit Aer to simulate the imperfections of real hardware (read errors, decoherence, photon loss) and analyze how this noise impacts the key security metric: the **Quantum Bit Error Rate (QBER)**.
