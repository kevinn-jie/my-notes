# Use a quantum computer today



# Table of Contents

1. [Build and run your first quantum program](#build-and-run-your-first-quantum-program)



<br>



## Build and run your first quantum program

* In the `QuantumCircuit` class, we define qubits & operations
* With `AerSimulator`, we can simulate quantum circuits
* `preset_passmanagers` optimizes circuits to run efficiently on hardware
* `Sampler` and `QiskitRuntimeService` are necessary to actually run the circuit on the quantum computer

```python
from qiskit import QuantumCircuit
from qiskit.visualization import plot_histogram
from qiskit_aer import AerSimulator
from qiskit.transpiler.preset_passmanagers import generate_preset_pass_manager
from qiskit_ibm_runtime import SamplerV2 as Sampler, QiskitRuntimeService
```