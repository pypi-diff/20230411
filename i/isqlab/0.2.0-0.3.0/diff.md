# Comparing `tmp/isqlab-0.2.0.tar.gz` & `tmp/isqlab-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isqlab-0.2.0.tar", last modified: Mon Apr 10 07:35:17 2023, max compression
+gzip compressed data, was "isqlab-0.3.0.tar", last modified: Tue Apr 11 06:59:12 2023, max compression
```

## Comparing `isqlab-0.2.0.tar` & `isqlab-0.3.0.tar`

### file list

```diff
@@ -1,32 +1,31 @@
-drwxr-xr-x   0 yangys    (1000) yangys    (1000)        0 2023-04-10 07:35:17.263422 isqlab-0.2.0/
--rw-r--r--   0 yangys    (1000) yangys    (1000)     1073 2023-04-10 07:35:01.000000 isqlab-0.2.0/LICENSE
--rw-r--r--   0 yangys    (1000) yangys    (1000)      844 2023-04-10 07:35:17.263422 isqlab-0.2.0/PKG-INFO
--rw-r--r--   0 yangys    (1000) yangys    (1000)      610 2023-04-10 07:35:01.000000 isqlab-0.2.0/README.md
-drwxr-xr-x   0 yangys    (1000) yangys    (1000)        0 2023-04-10 07:35:17.263422 isqlab-0.2.0/isqlab/
--rw-r--r--   0 yangys    (1000) yangys    (1000)      442 2023-04-10 07:35:01.000000 isqlab-0.2.0/isqlab/__init__.py
-drwxr-xr-x   0 yangys    (1000) yangys    (1000)        0 2023-04-10 07:35:17.263422 isqlab-0.2.0/isqlab/circuits/
--rw-r--r--   0 yangys    (1000) yangys    (1000)       44 2023-04-10 07:35:01.000000 isqlab-0.2.0/isqlab/circuits/__init__.py
--rw-r--r--   0 yangys    (1000) yangys    (1000)    20874 2023-04-10 07:35:01.000000 isqlab-0.2.0/isqlab/circuits/quantum_circuit.py
-drwxr-xr-x   0 yangys    (1000) yangys    (1000)        0 2023-04-10 07:35:17.263422 isqlab-0.2.0/isqlab/linkers/
--rw-r--r--   0 yangys    (1000) yangys    (1000)       38 2023-04-10 07:35:01.000000 isqlab-0.2.0/isqlab/linkers/__init__.py
--rw-r--r--   0 yangys    (1000) yangys    (1000)    10356 2023-04-10 07:35:01.000000 isqlab-0.2.0/isqlab/linkers/torch_linker.py
-drwxr-xr-x   0 yangys    (1000) yangys    (1000)        0 2023-04-10 07:35:17.263422 isqlab-0.2.0/isqlab/neural_networks/
--rw-r--r--   0 yangys    (1000) yangys    (1000)       42 2023-04-10 07:35:01.000000 isqlab-0.2.0/isqlab/neural_networks/__init__.py
--rw-r--r--   0 yangys    (1000) yangys    (1000)     8563 2023-04-10 07:35:01.000000 isqlab-0.2.0/isqlab/neural_networks/neural_network.py
--rw-r--r--   0 yangys    (1000) yangys    (1000)     1452 2023-04-10 07:35:01.000000 isqlab-0.2.0/isqlab/neural_networks/qnn_autograd.py
--rw-r--r--   0 yangys    (1000) yangys    (1000)     1351 2023-04-10 07:35:01.000000 isqlab-0.2.0/isqlab/neural_networks/qnn_jax.py
--rw-r--r--   0 yangys    (1000) yangys    (1000)     4143 2023-04-10 07:35:01.000000 isqlab-0.2.0/isqlab/neural_networks/qnn_simulator.py
-drwxr-xr-x   0 yangys    (1000) yangys    (1000)        0 2023-04-10 07:35:17.263422 isqlab-0.2.0/isqlab/vqe/
--rw-r--r--   0 yangys    (1000) yangys    (1000)       53 2023-04-10 07:35:01.000000 isqlab-0.2.0/isqlab/vqe/__init__.py
--rw-r--r--   0 yangys    (1000) yangys    (1000)     4835 2023-04-10 07:35:01.000000 isqlab-0.2.0/isqlab/vqe/chem.py
--rw-r--r--   0 yangys    (1000) yangys    (1000)     1581 2023-04-10 07:35:01.000000 isqlab-0.2.0/isqlab/vqe/hamiltonian_measure.py
--rw-r--r--   0 yangys    (1000) yangys    (1000)     8916 2023-04-10 07:35:01.000000 isqlab-0.2.0/isqlab/vqe/ucc.py
--rw-r--r--   0 yangys    (1000) yangys    (1000)     4564 2023-04-10 07:35:01.000000 isqlab-0.2.0/isqlab/vqe/uccsd.py
-drwxr-xr-x   0 yangys    (1000) yangys    (1000)        0 2023-04-10 07:35:17.263422 isqlab-0.2.0/isqlab.egg-info/
--rw-r--r--   0 yangys    (1000) yangys    (1000)      844 2023-04-10 07:35:17.000000 isqlab-0.2.0/isqlab.egg-info/PKG-INFO
--rw-r--r--   0 yangys    (1000) yangys    (1000)      628 2023-04-10 07:35:17.000000 isqlab-0.2.0/isqlab.egg-info/SOURCES.txt
--rw-r--r--   0 yangys    (1000) yangys    (1000)        1 2023-04-10 07:35:17.000000 isqlab-0.2.0/isqlab.egg-info/dependency_links.txt
--rw-r--r--   0 yangys    (1000) yangys    (1000)        8 2023-04-10 07:35:17.000000 isqlab-0.2.0/isqlab.egg-info/requires.txt
--rw-r--r--   0 yangys    (1000) yangys    (1000)        7 2023-04-10 07:35:17.000000 isqlab-0.2.0/isqlab.egg-info/top_level.txt
--rw-r--r--   0 yangys    (1000) yangys    (1000)      107 2023-04-10 07:35:17.263422 isqlab-0.2.0/setup.cfg
--rw-r--r--   0 yangys    (1000) yangys    (1000)      750 2023-04-10 07:35:01.000000 isqlab-0.2.0/setup.py
+drwxr-xr-x   0 yangys    (1000) yangys    (1000)        0 2023-04-11 06:59:12.607251 isqlab-0.3.0/
+-rw-r--r--   0 yangys    (1000) yangys    (1000)     1151 2023-04-11 06:59:12.607251 isqlab-0.3.0/PKG-INFO
+-rw-r--r--   0 yangys    (1000) yangys    (1000)      610 2023-04-11 06:59:01.000000 isqlab-0.3.0/README.md
+drwxr-xr-x   0 yangys    (1000) yangys    (1000)        0 2023-04-11 06:59:12.607251 isqlab-0.3.0/isqlab/
+-rw-r--r--   0 yangys    (1000) yangys    (1000)      442 2023-04-11 06:59:01.000000 isqlab-0.3.0/isqlab/__init__.py
+drwxr-xr-x   0 yangys    (1000) yangys    (1000)        0 2023-04-11 06:59:12.607251 isqlab-0.3.0/isqlab/circuits/
+-rw-r--r--   0 yangys    (1000) yangys    (1000)       44 2023-04-11 06:59:01.000000 isqlab-0.3.0/isqlab/circuits/__init__.py
+-rw-r--r--   0 yangys    (1000) yangys    (1000)    20874 2023-04-11 06:59:01.000000 isqlab-0.3.0/isqlab/circuits/quantum_circuit.py
+drwxr-xr-x   0 yangys    (1000) yangys    (1000)        0 2023-04-11 06:59:12.607251 isqlab-0.3.0/isqlab/linkers/
+-rw-r--r--   0 yangys    (1000) yangys    (1000)       38 2023-04-11 06:59:01.000000 isqlab-0.3.0/isqlab/linkers/__init__.py
+-rw-r--r--   0 yangys    (1000) yangys    (1000)    10356 2023-04-11 06:59:01.000000 isqlab-0.3.0/isqlab/linkers/torch_linker.py
+drwxr-xr-x   0 yangys    (1000) yangys    (1000)        0 2023-04-11 06:59:12.607251 isqlab-0.3.0/isqlab/neural_networks/
+-rw-r--r--   0 yangys    (1000) yangys    (1000)       42 2023-04-11 06:59:01.000000 isqlab-0.3.0/isqlab/neural_networks/__init__.py
+-rw-r--r--   0 yangys    (1000) yangys    (1000)     8563 2023-04-11 06:59:01.000000 isqlab-0.3.0/isqlab/neural_networks/neural_network.py
+-rw-r--r--   0 yangys    (1000) yangys    (1000)     1452 2023-04-11 06:59:01.000000 isqlab-0.3.0/isqlab/neural_networks/qnn_autograd.py
+-rw-r--r--   0 yangys    (1000) yangys    (1000)     1351 2023-04-11 06:59:01.000000 isqlab-0.3.0/isqlab/neural_networks/qnn_jax.py
+-rw-r--r--   0 yangys    (1000) yangys    (1000)     4143 2023-04-11 06:59:01.000000 isqlab-0.3.0/isqlab/neural_networks/qnn_simulator.py
+drwxr-xr-x   0 yangys    (1000) yangys    (1000)        0 2023-04-11 06:59:12.607251 isqlab-0.3.0/isqlab/vqe/
+-rw-r--r--   0 yangys    (1000) yangys    (1000)       53 2023-04-11 06:59:01.000000 isqlab-0.3.0/isqlab/vqe/__init__.py
+-rw-r--r--   0 yangys    (1000) yangys    (1000)     6876 2023-04-11 06:59:01.000000 isqlab-0.3.0/isqlab/vqe/chem.py
+-rw-r--r--   0 yangys    (1000) yangys    (1000)     1581 2023-04-11 06:59:01.000000 isqlab-0.3.0/isqlab/vqe/hamiltonian_measure.py
+-rw-r--r--   0 yangys    (1000) yangys    (1000)     3499 2023-04-11 06:59:01.000000 isqlab-0.3.0/isqlab/vqe/kupccgsd.py
+-rw-r--r--   0 yangys    (1000) yangys    (1000)    10721 2023-04-11 06:59:01.000000 isqlab-0.3.0/isqlab/vqe/ucc.py
+-rw-r--r--   0 yangys    (1000) yangys    (1000)     3391 2023-04-11 06:59:01.000000 isqlab-0.3.0/isqlab/vqe/uccsd.py
+drwxr-xr-x   0 yangys    (1000) yangys    (1000)        0 2023-04-11 06:59:12.607251 isqlab-0.3.0/isqlab.egg-info/
+-rw-r--r--   0 yangys    (1000) yangys    (1000)     1151 2023-04-11 06:59:12.000000 isqlab-0.3.0/isqlab.egg-info/PKG-INFO
+-rw-r--r--   0 yangys    (1000) yangys    (1000)      614 2023-04-11 06:59:12.000000 isqlab-0.3.0/isqlab.egg-info/SOURCES.txt
+-rw-r--r--   0 yangys    (1000) yangys    (1000)        1 2023-04-11 06:59:12.000000 isqlab-0.3.0/isqlab.egg-info/dependency_links.txt
+-rw-r--r--   0 yangys    (1000) yangys    (1000)        7 2023-04-11 06:59:12.000000 isqlab-0.3.0/isqlab.egg-info/top_level.txt
+-rw-r--r--   0 yangys    (1000) yangys    (1000)      107 2023-04-11 06:59:12.607251 isqlab-0.3.0/setup.cfg
+-rw-r--r--   0 yangys    (1000) yangys    (1000)      752 2023-04-11 06:59:01.000000 isqlab-0.3.0/setup.py
```

### Comparing `isqlab-0.2.0/PKG-INFO` & `isqlab-0.3.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: isqlab
-Version: 0.2.0
-Summary: application modules for isq
-Author: Yusheng Yang
-Author-email: yangys@arclightquantum.com
-Platform: python 3.8+
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 Isqlab is a Python library for isQ.
 
 ## Key Features
 
 - *isQ backend.*
 
 - *Quantum Machine Learning*. Connect to quantum device using **PyTorch**.
```

### Comparing `isqlab-0.2.0/isqlab/circuits/quantum_circuit.py` & `isqlab-0.3.0/isqlab/circuits/quantum_circuit.py`

 * *Files identical despite different names*

### Comparing `isqlab-0.2.0/isqlab/linkers/torch_linker.py` & `isqlab-0.3.0/isqlab/linkers/torch_linker.py`

 * *Files identical despite different names*

### Comparing `isqlab-0.2.0/isqlab/neural_networks/neural_network.py` & `isqlab-0.3.0/isqlab/neural_networks/neural_network.py`

 * *Files identical despite different names*

### Comparing `isqlab-0.2.0/isqlab/neural_networks/qnn_autograd.py` & `isqlab-0.3.0/isqlab/neural_networks/qnn_autograd.py`

 * *Files identical despite different names*

### Comparing `isqlab-0.2.0/isqlab/neural_networks/qnn_jax.py` & `isqlab-0.3.0/isqlab/neural_networks/qnn_jax.py`

 * *Files identical despite different names*

### Comparing `isqlab-0.2.0/isqlab/neural_networks/qnn_simulator.py` & `isqlab-0.3.0/isqlab/neural_networks/qnn_simulator.py`

 * *Files identical despite different names*

### Comparing `isqlab-0.2.0/isqlab/vqe/chem.py` & `isqlab-0.3.0/isqlab/vqe/chem.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,15 +9,20 @@
 
 import numpy as np
 from typing import Tuple
 from itertools import product
 from pyscf.scf.hf import RHF
 from pyscf.mcscf import CASCI
 from pyscf import ao2mo, gto
-from openfermion import FermionOperator, QubitOperator
+from openfermion import (
+    FermionOperator,
+    QubitOperator,
+    binary_code_transform,
+    parity_code,
+)
 from openfermion.ops.representations import InteractionOperator
 from openfermion.utils import hermitian_conjugated
 
 
 TOLERANCE = 1e-8
 
 
@@ -173,7 +178,79 @@
             reversed([(
                 n_qubits - 1 - idx,
                 symbol,
             ) for idx, symbol in pauli_string])
         )
         ret.terms[pauli_string] = value
     return ret
+
+
+def reverse_fop_idx(
+    op: FermionOperator,
+    n_qubits: int,
+) -> FermionOperator:
+    ret = FermionOperator()
+    for word, v in op.terms.items():
+        word = tuple([(n_qubits - 1 - idx, symbol) for idx, symbol in word])
+        ret.terms[word] = v
+    return ret
+
+
+def parity(
+    fermion_operator: FermionOperator,
+    n_modes: int,
+    n_elec: int,
+) -> QubitOperator:
+    """
+    Performs parity transformation.
+
+    Parameters
+    ----------
+    fermion_operator: FermionOperator
+        The fermion operator.
+    n_modes: int
+        The number of modes (spin-orbitals).
+    n_elec: int
+        The number of electrons.
+
+    Returns
+    -------
+    qubit_operator: QubitOperator
+    """
+    qubit_operator = _parity(
+        reverse_fop_idx(
+            fermion_operator,
+            n_modes,
+        ),
+        n_modes,
+    )
+    res = 0
+    assert n_modes % 2 == 0
+    reduction_indices = [n_modes // 2 - 1, n_modes - 1]
+    phase_alpha = (-1) ** (n_elec // 2)
+    for qop in qubit_operator:
+        # qop example: 0.5 [Z1 X2 X3]
+        pauli_string, coeff = next(iter(qop.terms.items()))
+        # pauli_string example: ((1, 'Z'), (2, 'X'), (3, 'X'))
+        # coeff example: 0.5
+        new_pauli_string = []
+        for idx, symbol in pauli_string:
+            is_alpha = idx <= reduction_indices[0]
+            if idx in reduction_indices:
+                if symbol in ["X", "Y"]:
+                    # discard this term because the bit will never change
+                    continue
+                else:
+                    assert symbol == "Z"
+                    if is_alpha:
+                        coeff *= phase_alpha
+                    continue
+            if not is_alpha:
+                idx -= 1
+            new_pauli_string.append((idx, symbol))
+        qop.terms = {tuple(new_pauli_string): coeff}
+        res += qop
+    return res
+
+
+def _parity(fermion_operator, n_modes):
+    return binary_code_transform(fermion_operator, parity_code(n_modes))
```

### Comparing `isqlab-0.2.0/isqlab/vqe/hamiltonian_measure.py` & `isqlab-0.3.0/isqlab/vqe/hamiltonian_measure.py`

 * *Files identical despite different names*

### Comparing `isqlab-0.2.0/isqlab/vqe/ucc.py` & `isqlab-0.3.0/isqlab/vqe/ucc.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,60 +4,75 @@
 
 """
 UCC ansatzs implementation.
 This file is inspired by TenCirChem and OpenFermion.
 """
 
 from isqlab.circuits import QuantumCircuit
+from isqlab.vqe.chem import ex_op_to_fop, reverse_qop_idx, canonical_mo_coeff
 import numpy as np
-from typing import Tuple, List, Union
+from typing import Tuple, List, Union, Optional, Sequence
 from pyscf.cc.addons import spatial2spin
+from pyscf import gto
+from openfermion import jordan_wigner
 
 
 class UCC:
     """Basic class for couple cluster"""
 
     def __init__(
         self,
-        mol,
-        active_space=None,
-        mo_coeff=None,
+        mol: gto.Mole,
+        active_space: Tuple[int, int] = None,
+        mo_coeff: Optional[np.ndarray] = None,
     ) -> None:
 
         self.mol = mol
+        # self.mol = mol.copy()
         if active_space is None:
             active_space = (mol.nelectron, int(mol.nao))
 
         self.n_qubits = 2 * active_space[1]
         self.active_space = active_space
         self.n_elec = active_space[0]
         self.active = active_space[1]
         self.inactive_occ = mol.nelectron // 2 - active_space[0] // 2
         self.inactive_vir = mol.nao - active_space[1] - self.inactive_occ
-
-        frozen_idx = list(range(self.inactive_occ)) + \
+        self.frozen_idx = list(range(self.inactive_occ)) + \
             list(range(mol.nao - self.inactive_vir, mol.nao))
 
         # classical quantum chemistry
         self.e_nuc = mol.energy_nuc()
         # initial guess
         self.t1 = self.t2 = None
 
+        if mo_coeff is not None:
+            # use user defined coefficient
+            self.mo_coeff = canonical_mo_coeff(mo_coeff)
+
+        self.ex_ops = None
+        self.param_idx = None
+
     @property
     def no(self) -> int:
         """The number of occupied orbitals."""
         return self.n_elec // 2
 
     @property
     def nv(self) -> int:
         """The number of virtual (unoccupied orbitals)."""
         return self.active - self.no
 
     @staticmethod
-    def evolve_pauli(circuit: QuantumCircuit, pauli_string: Tuple, theta: str, value: complex) -> None:
+    def evolve_pauli(
+        circuit: QuantumCircuit,
+        pauli_string: Tuple,
+        theta: str,
+        value: complex,
+    ) -> None:
         # pauli_string in openfermion.QubitOperator.terms format
         for idx, symbol in pauli_string:
             if symbol == "X":
                 circuit.H(idx)
             elif symbol == "Y":
                 circuit.SD(idx)
                 circuit.H(idx)
@@ -98,16 +113,57 @@
             circuit = QuantumCircuit(n_qubits)
             for i in range(n_elec // 2):
                 circuit.X(i)
                 circuit.X(n_qubits // 2 + i)
 
         return circuit
 
-    def get_ex_ops(self, t1: np.ndarray = None, t2: np.ndarray = None):
-        """Virtual method to be implemented"""
+    def get_circuit(
+        self,
+        params_name: str = "theta",
+        ex_ops: list = None,
+        param_ids: Sequence = None,
+        init_state: Union[QuantumCircuit, str] = None,
+        trotter: bool = True,
+    ) -> QuantumCircuit:
+
+        if ex_ops is None:
+            ex_ops = self.ex_ops
+
+        if param_ids is None:
+            param_ids = self.param_ids
+
+        circuit = QuantumCircuit(self.n_qubits)
+
+        if init_state:
+            init_circuit = self.get_init_circuit(
+                self.n_qubits, self.n_elec, init_state)
+            circuit.extend(init_circuit)
+
+        for param_id, f_idx in zip(param_ids, ex_ops):
+            theta = f"{params_name}[{param_id}]"
+            fop = ex_op_to_fop(f_idx, with_conjugation=True)
+            qop = reverse_qop_idx(jordan_wigner(fop), self.n_qubits)
+            if trotter:
+                for pauli_string, value in qop.terms.items():
+                    self.evolve_pauli(circuit, pauli_string, theta, value)
+            else:
+                raise NotImplementedError("multicontrol_ry")
+                # TODO:
+                # https://arxiv.org/pdf/2005.14475.pdf
+                # circuit = evolve_excitation(
+                #     circuit, f_idx, qop, 2 * theta, decompose_multicontrol)
+        return circuit
+
+    def get_ex_ops(
+        self,
+        t1: np.ndarray = None,
+        t2: np.ndarray = None,
+    ):
+        """Abs method to be implemented"""
         raise NotImplementedError
 
     def get_ex1_ops(
         self,
         t1: np.ndarray = None,
     ) -> Tuple[List[Tuple], List[int], List[float]]:
         """Get one-body excitation operators."""
```

### Comparing `isqlab-0.2.0/isqlab/vqe/uccsd.py` & `isqlab-0.3.0/isqlab/vqe/uccsd.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,112 +1,82 @@
 # This code is part of isQ.
 # (C) Copyright ArcLight Quantum 2023.
 # This code is licensed under the MIT License.
 
 """
-UCC ansatzs implementation.
+UCCSD ansatzs implementation.
 This file is inspired by TenCirChem and OpenFermion.
 """
 
 from .ucc import UCC
-from isqlab.circuits import QuantumCircuit
-from isqlab.vqe.chem import ex_op_to_fop, reverse_qop_idx
 import numpy as np
-from typing import Tuple, List, Union, Sequence
-from openfermion import jordan_wigner
+from typing import Tuple, List, Optional
+from pyscf import gto
 
 
 DISCARD_EPS = 1e-12
 
 
 class UCCSD(UCC):
     """UCCSD"""
 
     def __init__(
         self,
-        mol,
-        active_space=None,
-        mo_coeff=None,
-        pick_ex2: bool = True,
+        mol: gto.Mole,
+        active_space: Tuple[int, int] = None,
+        mo_coeff: Optional[np.ndarray] = None,
         epsilon: float = DISCARD_EPS,
-        sort_ex2: bool = True,
+        pick_ex2: bool = False,
+        sort_ex2: bool = False,
+        run_ccsd: bool = False,
     ) -> None:
+
         super().__init__(
-            mol,
-            active_space,
-            mo_coeff,
+            mol=mol,
+            active_space=active_space,
+            mo_coeff=mo_coeff,
         )
 
         self.pick_ex2 = pick_ex2
         self.sort_ex2 = sort_ex2
 
         # screen out excitation operators based on t2 amplitude
         self.t2_discard_eps = epsilon
 
+        if run_ccsd:
+            ccsd = mol.CCSD()
+            if self.frozen_idx:
+                ccsd.frozen = self.frozen_idx
+            e_corr_ccsd, ccsd_t1, ccsd_t2 = ccsd.kernel()
+            self.t1, self.t2 = ccsd_t1, ccsd_t2
+
         self.ex_ops, self.param_ids, self.init_guess = self.get_ex_ops(
             self.t1,
             self.t2,
         )
         self.num_params = self.param_ids[-1] + 1
 
-    def get_circuit(
-        self,
-        params_name: str = "theta",
-        ex_ops: list = None,
-        param_ids: Sequence = None,
-        init_state: Union[QuantumCircuit, str] = None,
-        trotter: bool = True,
-    ):
-
-        if ex_ops is None:
-            ex_ops = self.ex_ops
-
-        if param_ids is None:
-            param_ids = self.param_ids
-
-        circuit = QuantumCircuit(self.n_qubits)
-
-        if init_state:
-            init_circuit = self.get_init_circuit(
-                self.n_qubits, self.n_elec, init_state)
-            circuit.extend(init_circuit)
-
-        for param_id, f_idx in zip(param_ids, ex_ops):
-            theta = f"{params_name}[{param_id}]"
-            fop = ex_op_to_fop(f_idx, with_conjugation=True)
-            qop = reverse_qop_idx(jordan_wigner(fop), self.n_qubits)
-            if trotter:
-                for pauli_string, value in qop.terms.items():
-                    self.evolve_pauli(circuit, pauli_string, theta, value)
-            else:
-                raise NotImplementedError("multicontrol_ry")
-                # TODO:
-                # https://arxiv.org/pdf/2005.14475.pdf
-                # circuit = evolve_excitation(
-                #     circuit, f_idx, qop, 2 * theta, decompose_multicontrol)
-        return circuit
-
     def get_ex_ops(
         self,
         t1: np.ndarray = None,
         t2: np.ndarray = None,
     ) -> Tuple[List[Tuple], List[int], List[float]]:
         """Get one-body and two-body excitation operators for UCCSD ansatz."""
 
         ex1_ops, ex1_param_ids, ex1_init_guess = self.get_ex1_ops(self.t1)
         ex2_ops, ex2_param_ids, ex2_init_guess = self.get_ex2_ops(self.t2)
 
         # screen out symmetrically not allowed excitation
-        # ex2_ops, ex2_param_ids, ex2_init_guess = self.pick_and_sort(
-        #     ex2_ops,
-        #     ex2_param_ids,
-        #     ex2_init_guess,
-        #     self.pick_ex2,
-        #     self.sort_ex2,
-        # )
+        ex2_ops, ex2_param_ids, ex2_init_guess = self.pick_and_sort(
+            ex2_ops,
+            ex2_param_ids,
+            ex2_init_guess,
+            self.pick_ex2,
+            self.sort_ex2,
+        )
 
         ex_op = ex1_ops + ex2_ops
         param_ids = ex1_param_ids + \
             [i + max(ex1_param_ids) + 1 for i in ex2_param_ids]
         init_guess = ex1_init_guess + ex2_init_guess
         return ex_op, param_ids, init_guess
 
@@ -122,18 +92,14 @@
         if do_sort:
             sorted_ex_ops = sorted(
                 zip(ex_ops, param_ids), key=lambda x: -np.abs(init_guess[x[1]]))
         else:
             sorted_ex_ops = list(zip(ex_ops, param_ids))
         ret_ex_ops = []
         ret_param_ids = []
-        # print(sorted_ex_ops)
-        # [((1, 3, 2, 0), 0)]
-        # print(init_guess)
-        # [0.0]
         for ex_op, param_id in sorted_ex_ops:
             # discard operators with tiny amplitude.
             # The default eps is so small that the screened out excitations are probably not allowed
             if do_pick and np.abs(init_guess[param_id]) < self.t2_discard_eps:
                 continue
             ret_ex_ops.append(ex_op)
             ret_param_ids.append(param_id)
```

### Comparing `isqlab-0.2.0/isqlab.egg-info/SOURCES.txt` & `isqlab-0.3.0/isqlab.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-LICENSE
 README.md
 setup.cfg
 setup.py
 isqlab/__init__.py
 isqlab.egg-info/PKG-INFO
 isqlab.egg-info/SOURCES.txt
 isqlab.egg-info/dependency_links.txt
-isqlab.egg-info/requires.txt
 isqlab.egg-info/top_level.txt
 isqlab/circuits/__init__.py
 isqlab/circuits/quantum_circuit.py
 isqlab/linkers/__init__.py
 isqlab/linkers/torch_linker.py
 isqlab/neural_networks/__init__.py
 isqlab/neural_networks/neural_network.py
 isqlab/neural_networks/qnn_autograd.py
 isqlab/neural_networks/qnn_jax.py
 isqlab/neural_networks/qnn_simulator.py
 isqlab/vqe/__init__.py
 isqlab/vqe/chem.py
 isqlab/vqe/hamiltonian_measure.py
+isqlab/vqe/kupccgsd.py
 isqlab/vqe/ucc.py
 isqlab/vqe/uccsd.py
```

### Comparing `isqlab-0.2.0/setup.py` & `isqlab-0.3.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 from setuptools import setup, find_packages
 
 
 with open("README.md", "r", encoding="utf-8") as readme:
     long_description = readme.read()
 
 requirements = [
-    "isqopen",
+    # "isqopen",
     # "pyscf",
     # "openfermion",
     # "openfermionpyscf",
 ]
 
 setup(
     name="isqlab",
-    version="0.2.0",
+    version="0.3.0",
     description="application modules for isq",
     platforms="python 3.8+",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Yusheng Yang",
     author_email="yangys@arclightquantum.com",
     packages=find_packages(where="."),
```

