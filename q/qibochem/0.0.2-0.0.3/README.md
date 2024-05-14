# Comparing `tmp/qibochem-0.0.2.tar.gz` & `tmp/qibochem-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qibochem-0.0.2.tar", max compression
+gzip compressed data, was "qibochem-0.0.3.tar", max compression
```

## Comparing `qibochem-0.0.2.tar` & `qibochem-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11558 2024-02-19 08:53:45.327945 qibochem-0.0.2/LICENSE
--rw-r--r--   0        0        0     1969 2024-02-19 08:53:45.327945 qibochem-0.0.2/README.md
--rw-r--r--   0        0        0     1584 2024-02-19 08:53:45.331945 qibochem-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      126 2024-02-19 08:53:45.331945 qibochem-0.0.2/src/qibochem/__init__.py
--rw-r--r--   0        0        0      432 2024-02-19 08:53:45.331945 qibochem-0.0.2/src/qibochem/ansatz/__init__.py
--rw-r--r--   0        0        0     6014 2024-02-19 08:53:45.331945 qibochem-0.0.2/src/qibochem/ansatz/basis_rotation.py
--rw-r--r--   0        0        0     1340 2024-02-19 08:53:45.331945 qibochem-0.0.2/src/qibochem/ansatz/hardware_efficient.py
--rw-r--r--   0        0        0     3057 2024-02-19 08:53:45.331945 qibochem-0.0.2/src/qibochem/ansatz/hf_reference.py
--rw-r--r--   0        0        0    16097 2024-02-19 08:53:45.331945 qibochem-0.0.2/src/qibochem/ansatz/ucc.py
--rw-r--r--   0        0        0      190 2024-02-19 08:53:45.331945 qibochem-0.0.2/src/qibochem/driver/__init__.py
--rw-r--r--   0        0        0     3481 2024-02-19 08:53:45.331945 qibochem-0.0.2/src/qibochem/driver/hamiltonian.py
--rw-r--r--   0        0        0    19600 2024-02-19 08:53:45.331945 qibochem-0.0.2/src/qibochem/driver/molecule.py
--rw-r--r--   0        0        0       57 2024-02-19 08:53:45.331945 qibochem-0.0.2/src/qibochem/measurement/__init__.py
--rw-r--r--   0        0        0     5124 2024-02-19 08:53:45.331945 qibochem-0.0.2/src/qibochem/measurement/expectation.py
--rw-r--r--   0        0        0     6605 2024-02-19 08:53:45.331945 qibochem-0.0.2/src/qibochem/measurement/optimization.py
--rw-r--r--   0        0        0     2844 1970-01-01 00:00:00.000000 qibochem-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11558 2024-05-14 09:06:41.357939 qibochem-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1969 2024-05-14 09:06:41.357939 qibochem-0.0.3/README.md
+-rw-r--r--   0        0        0     1584 2024-05-14 09:06:41.361939 qibochem-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      126 2024-05-14 09:06:41.365939 qibochem-0.0.3/src/qibochem/__init__.py
+-rw-r--r--   0        0        0      422 2024-05-14 09:06:41.365939 qibochem-0.0.3/src/qibochem/ansatz/__init__.py
+-rw-r--r--   0        0        0     9551 2024-05-14 09:06:41.365939 qibochem-0.0.3/src/qibochem/ansatz/basis_rotation.py
+-rw-r--r--   0        0        0     1496 2024-05-14 09:06:41.365939 qibochem-0.0.3/src/qibochem/ansatz/hardware_efficient.py
+-rw-r--r--   0        0        0     3057 2024-05-14 09:06:41.365939 qibochem-0.0.3/src/qibochem/ansatz/hf_reference.py
+-rw-r--r--   0        0        0    15745 2024-05-14 09:06:41.365939 qibochem-0.0.3/src/qibochem/ansatz/ucc.py
+-rw-r--r--   0        0        0       46 2024-05-14 09:06:41.365939 qibochem-0.0.3/src/qibochem/driver/__init__.py
+-rw-r--r--   0        0        0     2421 2024-05-14 09:06:41.365939 qibochem-0.0.3/src/qibochem/driver/hamiltonian.py
+-rw-r--r--   0        0        0    19649 2024-05-14 09:06:41.365939 qibochem-0.0.3/src/qibochem/driver/molecule.py
+-rw-r--r--   0        0        0       78 2024-05-14 09:06:41.365939 qibochem-0.0.3/src/qibochem/measurement/__init__.py
+-rw-r--r--   0        0        0    11232 2024-05-14 09:06:41.365939 qibochem-0.0.3/src/qibochem/measurement/optimization.py
+-rw-r--r--   0        0        0     5443 2024-05-14 09:06:41.365939 qibochem-0.0.3/src/qibochem/measurement/result.py
+-rw-r--r--   0        0        0     2844 1970-01-01 00:00:00.000000 qibochem-0.0.3/PKG-INFO
```

### Comparing `qibochem-0.0.2/LICENSE` & `qibochem-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qibochem-0.0.2/README.md` & `qibochem-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `qibochem-0.0.2/pyproject.toml` & `qibochem-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qibochem"
-version = "0.0.2"
+version = "0.0.3"
 description = "Quantum chemistry module for quantum computing with Qibo"
 authors = ["The Qibo team"]
 license = "Apache License 2.0"
 readme = "README.md"
 repository = "https://github.com/qiboteam/qibochem/"
 documentation = "https://qibo.science/qibochem/stable"
 keywords = []
```

### Comparing `qibochem-0.0.2/src/qibochem/ansatz/hf_reference.py` & `qibochem-0.0.3/src/qibochem/ansatz/hf_reference.py`

 * *Files identical despite different names*

### Comparing `qibochem-0.0.2/src/qibochem/ansatz/ucc.py` & `qibochem-0.0.3/src/qibochem/ansatz/ucc.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,81 +1,71 @@
 """
 Circuit representing the Unitary Coupled Cluster ansatz in quantum chemistry
 """
 
 import numpy as np
 import openfermion
-from qibo import gates, models
+from qibo import Circuit, gates
 
 from qibochem.ansatz.hf_reference import hf_circuit
 
 
-def expi_pauli(n_qubits, theta, pauli_string):
+def expi_pauli(n_qubits, pauli_string, theta):
     """
     Build circuit representing exp(i*theta*pauli_string)
 
     Args:
         n_qubits: No. of qubits in the quantum circuit
-        theta: parameter
-        pauli_string: OpenFermion QubitOperator object, e.g. X_0 Y_1 Z_2 X_4
+        pauli_string: String in the format: ``"X0 Z1 Y3 X11"``
+        theta: Real number
 
     Returns:
         circuit: Qibo Circuit object representing exp(i*theta*pauli_string)
-        coeff: Coefficient of theta. May be useful for VQE
     """
-    # Unpack the dictionary from pauli_string.terms.items() into
-    # a (tuple of Pauli letters) and the coefficient of the pauli_string
-    [(p_letters, _coeff)] = pauli_string.terms.items()
-
-    # _coeff is an imaginary number, i.e. exp(i\theta something)
-    # Convert to the real coefficient for multiplying theta
-    coeff = -2.0 * np.real(_coeff * -1.0j)
-
-    # Generate the list of basis change gates using the p_letters list
-    basis_changes = [
-        gates.H(_qubit) if _gate == "X" else gates.RX(_qubit, -0.5 * np.pi, trainable=False)
-        for _qubit, _gate in p_letters
-        if _gate != "Z"
-    ]
+    # Split pauli_string into the old p_letters format
+    pauli_ops = sorted(((int(_op[1:]), _op[0]) for _op in pauli_string.split()), key=lambda x: x[0])
+    n_pauli_ops = len(pauli_ops)
+
+    # Convert theta into a real number for applying with a RZ gate
+    rz_parameter = -2.0 * theta
+
+    # Generate the list of basis change gates using the pauli_ops list
+    basis_changes = []
+    for qubit, pauli_op in pauli_ops:
+        if pauli_op == "Y":
+            basis_changes.append(gates.S(qubit).dagger())
+        if pauli_op not in ("I", "Z"):
+            basis_changes.append(gates.H(qubit))
 
     # Build the circuit
-    circuit = models.Circuit(n_qubits)
+    circuit = Circuit(n_qubits)
     # 1. Change to X/Y where necessary
-    circuit.add(_gate for _gate in basis_changes)
-    # 2. Add CNOTs to all pairs of qubits in p_letters, starting from the last letter
-    circuit.add(
-        gates.CNOT(_qubit1, _qubit2) for (_qubit1, _g1), (_qubit2, _g2) in zip(p_letters[::-1], p_letters[::-1][1:])
-    )
-    # 3. Add RZ gate to last element of p_letters
-    circuit.add(gates.RZ(p_letters[0][0], coeff * theta))
-    # 4. Add CNOTs to all pairs of qubits in p_letters
-    circuit.add(gates.CNOT(_qubit2, _qubit1) for (_qubit1, _g1), (_qubit2, _g2) in zip(p_letters, p_letters[1:]))
+    circuit.add(basis_changes)
+    # 2. Add CNOTs to all pairs of qubits in pauli_ops, starting from the last letter
+    circuit.add(gates.CNOT(pauli_ops[_i][0], pauli_ops[_i - 1][0]) for _i in range(n_pauli_ops - 1, 0, -1))
+    # 3. Add RZ gate to last element of pauli_ops
+    circuit.add(gates.RZ(pauli_ops[0][0], rz_parameter))
+    # 4. Add CNOTs to all pairs of qubits in pauli_ops
+    circuit.add(gates.CNOT(pauli_ops[_i + 1][0], pauli_ops[_i][0]) for _i in range(n_pauli_ops - 1))
     # 3. Change back to the Z basis
-    # .dagger() doesn't keep trainable=False, so need to use a for loop
-    # circuit.add(_gate.dagger() for _gate in basis_changes)
-    for _gate in basis_changes:
-        gate = _gate.dagger()
-        gate.trainable = False
-        circuit.add(gate)
-    return circuit, coeff
+    circuit.add(_gate.dagger() for _gate in reversed(basis_changes))
+    return circuit
 
 
-def ucc_circuit(n_qubits, excitation, theta=0.0, trotter_steps=1, ferm_qubit_map=None, coeffs=None):
+def ucc_circuit(n_qubits, excitation, theta=0.0, trotter_steps=1, ferm_qubit_map=None):
     r"""
     Circuit corresponding to the unitary coupled-cluster ansatz for a single excitation
 
     Args:
         n_qubits: Number of qubits in the quantum circuit
         excitation: Iterable of orbitals involved in the excitation; must have an even number of elements
             E.g. ``[0, 1, 2, 3]`` represents the excitation of electrons in orbitals ``(0, 1)`` to ``(2, 3)``
         theta: UCC parameter. Defaults to 0.0
         trotter_steps: Number of Trotter steps; i.e. number of times the UCC ansatz is applied with ``theta`` = ``theta / trotter_steps``. Default: 1
         ferm_qubit_map: Fermion-to-qubit transformation. Default is Jordan-Wigner (``jw``).
-        coeffs: List to hold the coefficients for the rotation parameter in each Pauli string.
-            May be useful in running the VQE. WARNING: Will be modified in this function
 
     Returns:
         Qibo ``Circuit``: Circuit corresponding to a single UCC excitation
     """
     # Check size of orbitals input
     n_orbitals = len(excitation)
     assert n_orbitals % 2 == 0, f"{excitation} must have an even number of items"
@@ -99,33 +89,36 @@
     elif ferm_qubit_map == "bk":
         qubit_ucc_operator = openfermion.bravyi_kitaev(ucc_operator)
     else:
         raise KeyError("Fermon-to-qubit mapping must be either 'jw' or 'bk'")
 
     # Apply the qubit_ucc_operator 'trotter_steps' times:
     assert trotter_steps > 0, f"{trotter_steps} must be > 0!"
-    circuit = models.Circuit(n_qubits)
+    circuit = Circuit(n_qubits)
     for _i in range(trotter_steps):
         # Use the get_operators() generator to get the list of excitation operators
-        for pauli_string in qubit_ucc_operator.get_operators():
-            _circuit, coeff = expi_pauli(n_qubits, theta / trotter_steps, pauli_string)
+        for raw_pauli_string in qubit_ucc_operator.get_operators():
+            # Convert each operator into a string and get the associated coefficient
+            ((pauli_ops, coeff),) = raw_pauli_string.terms.items()  # Unpack the single-item dictionary
+            pauli_string = " ".join(f"{pauli_op[1]}{pauli_op[0]}" for pauli_op in pauli_ops)
+            # Build the circuit and add it on
+            _circuit = expi_pauli(
+                n_qubits, pauli_string, -1.0j * coeff * theta / trotter_steps
+            )  # Divide imag. coeff by 1.0j
             circuit += _circuit
-            if isinstance(coeffs, list):
-                coeffs.append(coeff)
-
     return circuit
 
 
 # Utility functions
 
 
 def mp2_amplitude(excitation, orbital_energies, tei):
-    """
+    r"""
     Calculate the MP2 guess amplitude for a single UCC circuit: 0.0 for a single excitation.
-        for a double excitation (In SO basis): t_{ij}^{ab} = (g_{ijab} - g_{ijba}) / (e_i + e_j - e_a - e_b)
+        for a double excitation (In SO basis): :math:`t_{ij}^{ab} = (g_{ijab} - g_{ijba}) / (e_i + e_j - e_a - e_b)`
 
     Args:
         excitation: Iterable of spin-orbitals representing a excitation. Must have either 2 or 4 elements exactly,
             representing a single or double excitation respectively.
         orbital_energies: eigenvalues of the Fock operator, i.e. orbital energies
         tei: Two-electron integrals in MO basis and second quantization notation
 
@@ -171,15 +164,15 @@
         List of lists, e.g. [[0, 1]]
     """
     # If order of excitation > either number of electrons/orbitals, return list of empty list
     if order > min(len(excite_from), len(excite_to)):
         return [[]]
 
     # Generate all possible excitations first
-    from itertools import combinations
+    from itertools import combinations  # pylint: disable=C0415
 
     all_excitations = [
         [*_from, *_to] for _from in combinations(excite_from, order) for _to in combinations(excite_to, order)
     ]
     # Filter out the excitations if conserve_spin set
     if conserve_spin:
         # Not sure if this filtering is exhaustive; might not remove some redundant excitations?
@@ -215,16 +208,17 @@
 
     # Define variables for the while loop
     copy_excitations = [list(_ex) for _ex in excitations]
     result = []
     prev = []
 
     # No idea how I came up with this, but it seems to work for double excitations
-    # Default sorting is OK for single excitations
-    sorting_fn = lambda x: sum((order + 1 - _i) * abs(x[2 * _i + 1] // 2 - x[2 * _i] // 2) for _i in range(0, order))
+    def sorting_fn(x):
+        # Default sorting is OK for single excitations
+        return sum((order + 1 - _i) * abs(x[2 * _i + 1] // 2 - x[2 * _i] // 2) for _i in range(0, order))
 
     # Make a copy of the list of excitations, and use it populate a new list iteratively
     while copy_excitations:
         if not prev:
             # Take out all pair excitations first
             pair_excitations = [
                 _ex
@@ -340,17 +334,11 @@
         # Check that number of circuit variables (i.e. thetas) matches the number of circuit parameters
         assert len(thetas) == n_parameters, "Number of input parameters doesn't match the number of circuit parameters!"
 
     # Build the circuit
     if include_hf:
         circuit = hf_circuit(n_orbs, n_elec, ferm_qubit_map=ferm_qubit_map)
     else:
-        circuit = models.Circuit(n_orbs)
+        circuit = Circuit(n_orbs)
     for excitation, theta in zip(excitations, thetas):
-        # coeffs = []
-        circuit += ucc_circuit(
-            n_orbs, excitation, theta, trotter_steps=trotter_steps, ferm_qubit_map=ferm_qubit_map  # , coeffs=coeffs)
-        )
-        # if isinstance(all_coeffs, list):
-        #     all_coeffs.append(np.array(coeffs))
-
+        circuit += ucc_circuit(n_orbs, excitation, theta, trotter_steps=trotter_steps, ferm_qubit_map=ferm_qubit_map)
     return circuit
```

### Comparing `qibochem-0.0.2/src/qibochem/driver/molecule.py` & `qibochem-0.0.3/src/qibochem/driver/molecule.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,21 +2,20 @@
 Driver for obtaining molecular integrals from either PySCF or PSI4
 """
 
 from pathlib import Path
 
 import numpy as np
 import openfermion
-import qibo
 from qibo.hamiltonians import SymbolicHamiltonian
 
 from qibochem.driver.hamiltonian import (
     fermionic_hamiltonian,
     qubit_hamiltonian,
-    symbolic_hamiltonian,
+    qubit_to_symbolic_hamiltonian,
 )
 
 
 class Molecule:
     """
     Class representing a single molecule
 
@@ -119,15 +118,15 @@
         """
         Run a Hartree-Fock calculation with PySCF to obtain molecule quantities and
             molecular integrals
 
         Args:
             max_scf_cycles: Maximum number of SCF cycles in PySCF
         """
-        import pyscf
+        import pyscf  # pylint: disable=C0415
 
         # Set up and run PySCF calculation
         geom_string = "".join("{} {:.6f} {:.6f} {:.6f} ; ".format(_atom[0], *_atom[1]) for _atom in self.geometry)
         spin = self.multiplicity - 1  # PySCF spin is 2S
         pyscf_mol = pyscf.gto.M(charge=self.charge, spin=spin, atom=geom_string, basis=self.basis, symmetry="C1")
 
         pyscf_job = pyscf.scf.RHF(pyscf_mol)
@@ -175,15 +174,15 @@
     #     Run a Hartree-Fock calculation with PSI4 to obtain the molecular quantities and
     #         molecular integrals
 
     #     Args:
     #         output: Name of PSI4 output file. ``None`` suppresses the output on non-Windows systems,
     #             and uses ``psi4_output.dat`` otherwise
     #     """
-    #     import psi4  # pylint: disable=import-error
+    #     import psi4  # pylint: disable=C0415
 
     #     # PSI4 input string
     #     chgmul_string = f"{self.charge} {self.multiplicity} \n"
     #     geom_string = "\n".join("{} {:.6f} {:.6f} {:.6f}".format(_atom[0], *_atom[1]) for _atom in self.geometry)
     #     opt1_string = "\n\nunits angstrom\nsymmetry c1\n"
     #     mol_string = f"{chgmul_string}{geom_string}{opt1_string}"
     #     # PSI4 calculation options
@@ -409,29 +408,29 @@
             return ham
         ham = qubit_hamiltonian(ham, ferm_qubit_map)
         if ham_type in ("q", "qubit"):
             # OpenFermion QubitOperator Hamiltonian
             return ham
         if ham_type in ("s", "sym"):
             # Qibo SymbolicHamiltonian
-            return symbolic_hamiltonian(ham)
+            return qubit_to_symbolic_hamiltonian(ham)
         raise NameError(f"Unknown {ham_type}!")  # Shouldn't ever reach here
 
     @staticmethod
     def eigenvalues(hamiltonian):
         """
         Finds the lowest 6 exact eigenvalues of the molecular Hamiltonian
             Note: Uses the ``eigenvalues()`` class method for a Qibo ``SymbolicHamiltonian`` object
 
         Args:
             hamiltonian: Molecular Hamiltonian, given as a ``FermionOperator``, ``QubitOperator``, or
                 ``SymbolicHamiltonian`` (not recommended)
         """
         if isinstance(hamiltonian, (openfermion.FermionOperator, openfermion.QubitOperator)):
-            from scipy.sparse import linalg
+            from scipy.sparse import linalg  # pylint: disable=C0415
 
             hamiltonian_matrix = openfermion.get_sparse_operator(hamiltonian)
             # k argument in eigsh will depend on the size of the Hamiltonian
             n_eigenvals = min(6, hamiltonian_matrix.shape[0] - 2)
             # which=SA and return_eigenvalues=False returns the eigenvalues sorted by absolute value
             eigenvalues = linalg.eigsh(hamiltonian_matrix, k=n_eigenvals, which="SA", return_eigenvectors=False)
             # So need to sort again by their (algebraic) value to get the order: smallest->largest
```

### Comparing `qibochem-0.0.2/src/qibochem/measurement/expectation.py` & `qibochem-0.0.3/src/qibochem/measurement/result.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,107 +1,117 @@
+"""
+Functions for obtaining the expectation value for some given circuit and Hamiltonian, either from a state
+vector simulation, or from sample measurements
+"""
+
 from functools import reduce
 
-import numpy as np
 import qibo
 from qibo.hamiltonians import SymbolicHamiltonian
 from qibo.symbols import Z
 
 from qibochem.measurement.optimization import (
     allocate_shots,
     measurement_basis_rotations,
 )
 
 
+def expectation(circuit: qibo.models.Circuit, hamiltonian: SymbolicHamiltonian):
+    """
+    Expectation value using state vector simulations
+
+    Args:
+        circuit (qibo.models.Circuit): Quantum circuit ansatz
+        hamiltonian (qibo.hamiltonians.SymbolicHamiltonian): Molecular Hamiltonian
+
+    Returns:
+        float: Expectation value of the Hamiltonian for the given circuit
+    """
+    result = circuit(nshots=1)
+    state_ket = result.state()
+    return hamiltonian.expectation(state_ket)
+
+
 def symbolic_term_to_symbol(symbolic_term):
     """Convert a single Pauli word in the form of a Qibo SymbolicTerm to a Qibo Symbol"""
     return symbolic_term.coefficient * reduce(lambda x, y: x * y, symbolic_term.factors, 1.0)
 
 
-def pauli_term_measurement_expectation(pauli_term, frequencies):
+def pauli_term_measurement_expectation(pauli_term, frequencies, qubit_map):
     """
     Calculate the expectation value of a single general Pauli string for some measurement frequencies
 
     Args:
         pauli_term (SymbolicTerm): Single general Pauli term, e.g. X0*Z2
         frequencies: Measurement frequencies, taken from MeasurementOutcomes.frequencies(binary=True)
 
     Returns:
         float: Expectation value of pauli_term
     """
     # Replace every (non-I) Symbol with Z, then include the term coefficient
     pauli_z = [Z(int(factor.target_qubit)) for factor in pauli_term.factors if factor.name[0] != "I"]
     z_only_ham = SymbolicHamiltonian(pauli_term.coefficient * reduce(lambda x, y: x * y, pauli_z, 1.0))
     # Can now apply expectation_from_samples directly
-    return z_only_ham.expectation_from_samples(frequencies)
+    return z_only_ham.expectation_from_samples(frequencies, qubit_map=qubit_map)
 
 
-def expectation(
+def expectation_from_samples(
     circuit: qibo.models.Circuit,
     hamiltonian: SymbolicHamiltonian,
-    from_samples: bool = False,
     n_shots: int = 1000,
     group_pauli_terms=None,
     n_shots_per_pauli_term: bool = True,
     shot_allocation=None,
 ) -> float:
     """
-    Calculate expectation value of some Hamiltonian using either the state vector or sample measurements from running a
-    quantum circuit
+    Calculate expectation value of some Hamiltonian using sample measurements from running a Qibo quantum circuit
 
     Args:
         circuit (qibo.models.Circuit): Quantum circuit ansatz
         hamiltonian (qibo.hamiltonians.SymbolicHamiltonian): Molecular Hamiltonian
-        from_samples (bool): Whether the expectation value calculation uses samples or the simulated
-            state vector. Default: ``False``; Results are from a state vector simulation
-        n_shots (int): Number of times the circuit is run if ``from_samples=True``. Default: ``1000``
-        group_pauli_terms: Whether or not to group Pauli X/Y terms in the Hamiltonian together to reduce the measurement cost.
-            Default: ``None``; each of the Hamiltonian terms containing X/Y are in their own individual groups.
+        n_shots (int): Number of times the circuit is run. Default: ``1000``
+        group_pauli_terms: Whether or not to group Pauli X/Y terms in the Hamiltonian together to reduce the measurement
+            cost. Available options: ``None``: (Default) Hamiltonian terms containing X/Y are not grouped together, and
+            ``"qwc"``: Terms that commute qubitwise are grouped together
         n_shots_per_pauli_term (bool): Whether or not ``n_shots`` is used for each Pauli term in the Hamiltonian, or for
             *all* the terms in the Hamiltonian. Default: ``True``; ``n_shots`` are used to get the expectation value for each
             term in the Hamiltonian.
         shot_allocation: Iterable containing the number of shots to be allocated to each term in the Hamiltonian respectively if
             n_shots_per_pauli_term is ``False``. Default: ``None``; shots are allocated based on the magnitudes of the coefficients
             of the Hamiltonian terms.
 
     Returns:
         float: Hamiltonian expectation value
     """
-    if not from_samples:
-        # Expectation value from state vector simulation
-        result = circuit(nshots=1)
-        state_ket = result.state()
-        return hamiltonian.expectation(state_ket)
-
-    # From sample measurements:
-    # (Eventually) measurement_basis_rotations will be used to group up some terms so that one
-    # set of measurements can be used for multiple X/Y terms
-    grouped_terms = measurement_basis_rotations(hamiltonian, circuit.nqubits, grouping=group_pauli_terms)
+    # Group up Hamiltonian terms to reduce the measurement cost
+    grouped_terms = measurement_basis_rotations(hamiltonian, grouping=group_pauli_terms)
 
     # Check shot_allocation argument if not using n_shots_per_pauli_term
     if not n_shots_per_pauli_term:
         if shot_allocation is None:
             shot_allocation = allocate_shots(grouped_terms, n_shots)
         assert len(shot_allocation) == len(
             grouped_terms
-        ), "shot_allocation list must be the same size as the number of grouped terms!"
+        ), f"shot_allocation list ({len(shot_allocation)}) doesn't match the number of grouped terms ({len(grouped_terms)})"
 
     total = 0.0
     for _i, (measurement_gates, terms) in enumerate(grouped_terms):
         if measurement_gates and terms:
             _circuit = circuit.copy()
             _circuit.add(measurement_gates)
 
             # Number of shots used to run the circuit depends on n_shots_per_pauli_term
             result = _circuit(nshots=n_shots if n_shots_per_pauli_term else shot_allocation[_i])
 
             frequencies = result.frequencies(binary=True)
+            qubit_map = sorted(qubit for gate in measurement_gates for qubit in gate.target_qubits)
             if frequencies:  # Needed because might have cases whereby no shots allocated to a group
                 # First term is all Z terms, can use expectation_from_samples directly.
-                # Otherwise, need to use the general pauli_term_measurement_expectation function
                 if _i > 0:
-                    total += sum(pauli_term_measurement_expectation(term, frequencies) for term in terms)
+                    total += sum(pauli_term_measurement_expectation(term, frequencies, qubit_map) for term in terms)
+                # Otherwise, need to use the general pauli_term_measurement_expectation function
                 else:
                     z_ham = SymbolicHamiltonian(sum(symbolic_term_to_symbol(term) for term in terms))
-                    total += z_ham.expectation_from_samples(frequencies)
+                    total += z_ham.expectation_from_samples(frequencies, qubit_map=qubit_map)
     # Add the constant term if present. Note: Energies (in chemistry) are all real values
     total += hamiltonian.constant.real
     return total
```

### Comparing `qibochem-0.0.2/PKG-INFO` & `qibochem-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qibochem
-Version: 0.0.2
+Version: 0.0.3
 Summary: Quantum chemistry module for quantum computing with Qibo
 Home-page: https://github.com/qiboteam/qibochem/
 License: Apache-2.0
 Author: The Qibo team
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

