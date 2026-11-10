# Project objectives
1. Prepare an entangled 2-qubit Bell pair state.
2. Prepare an error detection system using an ancilla
3. Simulate operations across Ideal, noisy, protected conditions

# Approach
1. A qubit is initially taken and hadmard gate is applied to it, then CNOT with the other qubit as target - therefore creating a bell pair state.

2. CNOT gate is applied to both qubits with the ancilla qubit as target. If the ancilla qubit flips - it is not a bell pair. Otherwise it is.

3. Modules are used to simulate noisy environment.
Post selection is used to simulate protected environment.

# Results summary
Fidelity order -
Ideal>protected>noisy

# Architecture and Parameter Documentation
Qubit count - 3
Gates used - H(Hadamard), CNOT(Controlled-NOT)
Execution shots - 1000
Backend Name & Version - qiskit_aer.AerSimulator
Protection method - Post-selection filtering
