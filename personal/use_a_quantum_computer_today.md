# Use a quantum computer today



# Table of Contents

1. [Build and run your first quantum program](#build-and-run-your-first-quantum-program)



<br>



## Build and run your first quantum program

* **`QuantumCircuit`**: the class where we define qubits and operations
* **`AerSimulator`**: needed to simulate quantum circuits
* **`preset_passmanagers`**: needed to optimize circuits to run efficiently on hardware
* **`Sampler`** and **`QiskitRuntimeService`**: necessary to run the circuit on the quantum computer

```python
from qiskit import QuantumCircuit
from qiskit.visualization import plot_histogram
from qiskit_aer import AerSimulator
from qiskit.transpiler.preset_passmanagers import generate_preset_pass_manager
from qiskit_ibm_runtime import SamplerV2 as Sampler, QiskitRuntimeService
```

* **Composer**: used to build circuits by dragging the gates onto the wires
* **Hadamard gate (H)**: creates a superposition state of qubit 0
    * Superposition states allow either outcomes to happen when you measure