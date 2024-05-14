# Comparing `tmp/filter_functions-1.1.1.tar.gz` & `tmp/filter_functions-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filter_functions-1.1.1.tar", last modified: Tue Feb 22 15:51:33 2022, max compression
+gzip compressed data, was "filter_functions-1.1.2.tar", last modified: Mon May 23 17:08:56 2022, max compression
```

## Comparing `filter_functions-1.1.1.tar` & `filter_functions-1.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 15:51:33.920414 filter_functions-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (121)    32473 2022-02-22 15:51:24.000000 filter_functions-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     8770 2022-02-22 15:51:33.924416 filter_functions-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7976 2022-02-22 15:51:24.000000 filter_functions-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 15:51:33.920414 filter_functions-1.1.1/filter_functions/
--rw-r--r--   0 runner    (1001) docker     (121)     1850 2022-02-22 15:51:24.000000 filter_functions-1.1.1/filter_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2777 2022-02-22 15:51:24.000000 filter_functions-1.1.1/filter_functions/analytic.py
--rw-r--r--   0 runner    (1001) docker     (121)    29885 2022-02-22 15:51:24.000000 filter_functions-1.1.1/filter_functions/basis.py
--rw-r--r--   0 runner    (1001) docker     (121)    28500 2022-02-22 15:51:24.000000 filter_functions-1.1.1/filter_functions/gradient.py
--rw-r--r--   0 runner    (1001) docker     (121)    87840 2022-02-22 15:51:24.000000 filter_functions-1.1.1/filter_functions/numeric.py
--rw-r--r--   0 runner    (1001) docker     (121)    33705 2022-02-22 15:51:24.000000 filter_functions-1.1.1/filter_functions/plotting.py
--rw-r--r--   0 runner    (1001) docker     (121)   103675 2022-02-22 15:51:24.000000 filter_functions-1.1.1/filter_functions/pulse_sequence.py
--rw-r--r--   0 runner    (1001) docker     (121)     8786 2022-02-22 15:51:24.000000 filter_functions-1.1.1/filter_functions/superoperator.py
--rw-r--r--   0 runner    (1001) docker     (121)     2006 2022-02-22 15:51:24.000000 filter_functions-1.1.1/filter_functions/types.py
--rw-r--r--   0 runner    (1001) docker     (121)    38518 2022-02-22 15:51:24.000000 filter_functions-1.1.1/filter_functions/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 15:51:33.920414 filter_functions-1.1.1/filter_functions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8770 2022-02-22 15:51:33.000000 filter_functions-1.1.1/filter_functions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      525 2022-02-22 15:51:33.000000 filter_functions-1.1.1/filter_functions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-22 15:51:33.000000 filter_functions-1.1.1/filter_functions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      375 2022-02-22 15:51:33.000000 filter_functions-1.1.1/filter_functions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-02-22 15:51:33.000000 filter_functions-1.1.1/filter_functions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-02-22 15:51:33.924416 filter_functions-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1963 2022-02-22 15:51:24.000000 filter_functions-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 17:08:56.287131 filter_functions-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (121)    32473 2022-05-23 17:08:42.000000 filter_functions-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     8770 2022-05-23 17:08:56.287131 filter_functions-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     7976 2022-05-23 17:08:42.000000 filter_functions-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 17:08:56.287131 filter_functions-1.1.2/filter_functions/
+-rw-r--r--   0 runner    (1001) docker     (121)     1850 2022-05-23 17:08:42.000000 filter_functions-1.1.2/filter_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2777 2022-05-23 17:08:42.000000 filter_functions-1.1.2/filter_functions/analytic.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29901 2022-05-23 17:08:42.000000 filter_functions-1.1.2/filter_functions/basis.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28806 2022-05-23 17:08:42.000000 filter_functions-1.1.2/filter_functions/gradient.py
+-rw-r--r--   0 runner    (1001) docker     (121)    87494 2022-05-23 17:08:42.000000 filter_functions-1.1.2/filter_functions/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33160 2022-05-23 17:08:42.000000 filter_functions-1.1.2/filter_functions/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (121)   106793 2022-05-23 17:08:42.000000 filter_functions-1.1.2/filter_functions/pulse_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8786 2022-05-23 17:08:42.000000 filter_functions-1.1.2/filter_functions/superoperator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2051 2022-05-23 17:08:42.000000 filter_functions-1.1.2/filter_functions/types.py
+-rw-r--r--   0 runner    (1001) docker     (121)    39681 2022-05-23 17:08:42.000000 filter_functions-1.1.2/filter_functions/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 17:08:56.287131 filter_functions-1.1.2/filter_functions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     8770 2022-05-23 17:08:56.000000 filter_functions-1.1.2/filter_functions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      525 2022-05-23 17:08:56.000000 filter_functions-1.1.2/filter_functions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-23 17:08:56.000000 filter_functions-1.1.2/filter_functions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      375 2022-05-23 17:08:56.000000 filter_functions-1.1.2/filter_functions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-05-23 17:08:56.000000 filter_functions-1.1.2/filter_functions.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       93 2022-05-23 17:08:56.287131 filter_functions-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1963 2022-05-23 17:08:42.000000 filter_functions-1.1.2/setup.py
```

### Comparing `filter_functions-1.1.1/LICENSE` & `filter_functions-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `filter_functions-1.1.1/PKG-INFO` & `filter_functions-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filter_functions
-Version: 1.1.1
+Version: 1.1.2
 Summary: Package for efficient calculation of generalized filter functions
 Home-page: https://github.com/qutech/filter_functions
 Author: Quantum Technology Group, RWTH Aachen University
 Author-email: tobias.hangleiter@rwth-aachen.de
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `filter_functions-1.1.1/README.md` & `filter_functions-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `filter_functions-1.1.1/filter_functions/__init__.py` & `filter_functions-1.1.2/filter_functions/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,10 +28,10 @@
 from .superoperator import liouville_representation
 
 __all__ = ['Basis', 'PulseSequence', 'analytic', 'basis', 'concatenate', 'concatenate_periodic',
            'error_transfer_matrix', 'extend', 'infidelity', 'liouville_representation', 'numeric',
            'gradient', 'pulse_sequence', 'remap', 'util', 'superoperator', 'infidelity_derivative']
 
 
-__version__ = '1.1.1'
+__version__ = '1.1.2'
 __license__ = 'GNU GPLv3+'
 __author__ = 'Quantum Technology Group, RWTH Aachen University'
```

### Comparing `filter_functions-1.1.1/filter_functions/analytic.py` & `filter_functions-1.1.2/filter_functions/analytic.py`

 * *Files identical despite different names*

### Comparing `filter_functions-1.1.1/filter_functions/basis.py` & `filter_functions-1.1.2/filter_functions/basis.py`

 * *Files 1% similar despite different names*

```diff
@@ -549,16 +549,16 @@
     if not elems.isorthonorm:
         raise ValueError("The basis elements are not orthonormal!")
 
     if traceless is None:
         traceless = elems.istraceless
     else:
         if traceless and not elems.istraceless:
-            raise ValueError("The basis elements are not traceless (up to an identity element) " +
-                             "but a traceless basis was requested!")
+            raise ValueError("The basis elements are not traceless (up to an identity element) "
+                             + "but a traceless basis was requested!")
 
     if labels is not None and len(labels) not in (len(elems), elems.d**2):
         raise ValueError(f'Got {len(labels)} labels but expected {len(elems)} or {elems.d**2}')
 
     # Get a Generalized Gell-Mann basis to expand in (fulfills the desired
     # properties hermiticity and orthonormality, and therefore also linear
     # combinations, ie basis expansions, of it will). Split off the identity so
@@ -673,15 +673,16 @@
     .. math::
         M &= \sum_j c_j C_j, \\
         c_j &= \frac{\mathrm{tr}\big(M C_j\big)}
                     {\mathrm{tr}\big(C_j^\dagger C_j\big)}.
 
     """
 
-    def cast(arr): return arr.real if hermitian and basis.isherm else arr
+    def cast(arr):
+        return arr.real if hermitian and basis.isherm else arr
 
     coefficients = cast(np.tensordot(M, basis, axes=[(-2, -1), (-1, -2)]))
     if not normalized:
         coefficients /= cast(np.einsum('bij,bji->b', basis, basis))
 
     return util.remove_float_errors(coefficients) if tidyup else coefficients
 
@@ -720,15 +721,16 @@
         Bertlmann, R. A., & Krammer, P. (2008). Bloch vectors for
         qudits. Journal of Physics A: Mathematical and Theoretical,
         41(23). https://doi.org/10.1088/1751-8113/41/23/235303
     """
     if M.shape[-1] != M.shape[-2]:
         raise ValueError('M should be square in its last two axes')
 
-    def cast(arr): return arr.real if hermitian else arr
+    def cast(arr):
+        return arr.real if hermitian else arr
 
     # Squeeze out an extra dimension to be shape agnostic
     square = M.ndim < 3
     if square:
         M = M[None, ...]
 
     d = M.shape[-1]
```

### Comparing `filter_functions-1.1.1/filter_functions/gradient.py` & `filter_functions-1.1.2/filter_functions/gradient.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,16 +51,16 @@
 :func:`infidelity_derivative`
     Calculate the infidelity derivative.
 """
 from typing import Dict, Optional, Sequence, Tuple
 
 import numpy as np
 import opt_einsum as oe
-from opt_einsum.contract import ContractExpression
 from numpy import ndarray
+from opt_einsum.contract import ContractExpression
 
 from . import numeric, superoperator, util
 from .basis import Basis
 from .types import Coefficients, Operator
 
 __all__ = ['calculate_derivative_of_control_matrix_from_scratch',
            'calculate_filter_function_derivative', 'infidelity_derivative']
@@ -258,15 +258,15 @@
 
     Returns
     -------
     ctrlmat_g: ndarray, shape (n_dt, n_nops, d**2, n_omega)
         The individual control matrices of all time steps
     ctrlmat_g_deriv: ndarray, shape (n_dt, n_nops, d**2, n_ctrl, n_omega)
         The corresponding derivative with respect to the control
-        strength :math:`\frac{\partial\mathcal{B}_{\alpha j}^{(g)}(\omega)}
+        strength :math:`\frac{\partial\mathcal{B}_{\alpha j}^{(g)}(\omega)}`
 
     Notes
     -----
     The control matrix at each time step is evaluated according to
 
     .. math::
 
@@ -380,16 +380,14 @@
         eigvecs: ndarray,
         basis: Basis,
         t: Coefficients,
         dt: Coefficients,
         n_opers: Sequence[Operator],
         n_coeffs: Sequence[Coefficients],
         c_opers: Sequence[Operator],
-        all_identifiers: Sequence[str],
-        control_identifiers: Optional[Sequence[str]] = None,
         n_coeffs_deriv: Optional[Sequence[Coefficients]] = None,
         intermediates: Optional[Dict[str, ndarray]] = None
 ) -> ndarray:
     r"""
     Calculate the derivative of the control matrix from scratch.
 
     Parameters
@@ -417,36 +415,24 @@
         Sequence duration, i.e. for the :math:`g`-th pulse
         :math:`t_g - t_{g-1}`.
     n_opers: array_like, shape (n_nops, d, d)
         Noise operators :math:`B_\alpha`.
     n_coeffs: array_like, shape (n_nops, n_dt)
         The sensitivities of the system to the noise operators given by
         *n_opers* at the given time step.
-    c_opers: array_like, shape (n_cops, d, d)
-        Control operators :math:`H_k`.
-    all_identifiers: array_like, shape (n_cops)
-        Identifiers of all control operators.
-    control_identifiers: Sequence[str], shape (n_ctrl), Optional
-        Sequence of strings with the control identifiers to distinguish
-        between accessible control and drift Hamiltonian. The default is
-        None.
+    c_opers: array_like, shape (n_ctrl, d, d)
+        Control operators :math:`H_k` with respect to which the
+        derivative is computed.
     n_coeffs_deriv: array_like, shape (n_nops, n_ctrl, n_dt)
         The derivatives of the noise susceptibilities by the control
         amplitudes. Defaults to None.
     intermediates: Dict[str, ndarray], optional
         Optional dictionary containing intermediate results of the
         calculation of the control matrix.
 
-    Raises
-    ------
-    ValueError
-        If the given identifiers *control_identifier* are not subset of
-        the total identifiers *all_identifiers* of all control
-        operators.
-
     Returns
     -------
     ctrlmat_deriv: ndarray, shape (n_ctrl, n_omega, n_dt, n_nops, d**2)
         Partial derivatives of the total control matrix with respect to
         each control direction
         :math:`\frac{\partial\mathcal{B}_{\alpha k}(\omega)}{\partial
         u_h(t_{g'})}`.
@@ -466,32 +452,24 @@
                 {\partial u_h(t_{g'})} \right] \right)
 
     See Also
     --------
     _liouville_derivative
     _control_matrix_at_timestep_derivative
     """
-    # Distinction between control and drift operators and only
-    # calculate the derivatives in control direction
-    try:
-        idx = util.get_indices_from_identifiers(all_identifiers, control_identifiers)
-    except ValueError as err:
-        raise ValueError('Given control identifiers have to be a subset of (drift+control) ' +
-                         'Hamiltonian!') from err
-
     d = eigvecs.shape[-1]
     n_dt = len(dt)
-    n_ctrl = len(idx)
+    n_ctrl = len(c_opers)
     n_nops = len(n_opers)
     n_omega = len(omega)
 
     # Precompute some transformations or grab from cache if possible
     basis_transformed = numeric._transform_by_unitary(eigvecs[:, None], basis[None],
                                                       out=np.empty((n_dt, d**2, d, d), complex))
-    c_opers_transformed = numeric._transform_hamiltonian(eigvecs, c_opers[idx]).swapaxes(0, 1)
+    c_opers_transformed = numeric._transform_hamiltonian(eigvecs, c_opers).swapaxes(0, 1)
     if not intermediates:
         # None or empty
         n_opers_transformed = numeric._transform_hamiltonian(eigvecs, n_opers,
                                                              n_coeffs).swapaxes(0, 1)
         exp_buf, integral = np.empty((2, n_omega, d, d), dtype=complex)
     else:
         n_opers_transformed = intermediates['n_opers_transformed'].swapaxes(0, 1)
@@ -571,14 +549,15 @@
 
 
 def infidelity_derivative(
         pulse: 'PulseSequence',
         spectrum: Coefficients,
         omega: Coefficients,
         control_identifiers: Optional[Sequence[str]] = None,
+        n_oper_identifiers: Optional[Sequence[str]] = None,
         n_coeffs_deriv: Optional[Sequence[Coefficients]] = None
 ) -> ndarray:
     r"""Calculate the entanglement infidelity derivative of the
     ``PulseSequence`` *pulse*.
 
     Parameters
     ----------
@@ -595,32 +574,52 @@
         In the third and most general case, there may be a spectrum for
         each pair of noise operators corresponding to the correlations
         between them. n_nops is the number of noise operators considered
         and should be equal to ``len(n_oper_identifiers)``.
     omega: array_like, shape (n_omega,)
         The frequencies at which the integration is to be carried out.
     control_identifiers: Sequence[str], shape (n_ctrl,)
-        Sequence of strings with the control identifiern to distinguish
-        between accessible control and drift Hamiltonian.
+        Sequence of strings with the control identifiers to
+        distinguish between control and drift Hamiltonian. The
+        default is None, in which case the derivative is computed
+        for all known non-noise operators.
+    n_oper_identifiers: Sequence[str], shape (n_nops,)
+        Sequence of strings with the noise identifiers for which to
+        compute the derivative contribution. The default is None, in
+        which case it is computed for all known noise operators.
     n_coeffs_deriv: array_like, shape (n_nops, n_ctrl, n_dt)
         The derivatives of the noise susceptibilities by the control
-        amplitudes. Defaults to None.
+        amplitudes. The rows and columns should be in the same order
+        as the corresponding identifiers above. Defaults to None, in
+        which case the coefficients are assumed to be constant and
+        hence their derivative vanishing.
+
+        .. warning::
+
+            Internally, control and noise terms of the Hamiltonian
+            are stored alphanumerically sorted by their identifiers.
+            If the noise and/or control identifiers above are not
+            explicitly given, the rows and/or columns of this
+            parameter need to be sorted in the same fashion.
+
 
     Raises
     ------
     ValueError
         If the provided noise spectral density does not fit expected
         shape.
 
     Returns
     -------
     infid_deriv: ndarray, shape (n_nops, n_dt, n_ctrl)
         Array with the derivative of the infidelity for each noise
         source taken for each control direction at each time step
-        :math:`\frac{\partial I_e}{\partial u_h(t_{g'})}`.
+        :math:`\frac{\partial I_e}{\partial u_h(t_{g'})}`. Sorted in
+        the same fashion as `n_coeffs_deriv` or, if not given,
+        alphanumerically by the identifiers.
 
     Notes
     -----
     The infidelity's derivative is given by
 
     .. math::
 
@@ -653,15 +652,17 @@
 
     .. [Nie02]
         Nielsen, M. A. (2002). A simple formula for the average gate
         fidelity of a quantum dynamical operation. Physics Letters,
         Section A: General, Atomic and Solid State Physics, 303(4), 249–252.
         https://doi.org/10.1016/S0375-9601(02)01272-0
     """
-    spectrum = numeric._parse_spectrum(spectrum, omega, range(len(pulse.n_opers)))
-    filter_function_deriv = pulse.get_filter_function_derivative(omega, control_identifiers,
+    spectrum = util.parse_spectrum(spectrum, omega, range(len(pulse.n_opers)))
+    filter_function_deriv = pulse.get_filter_function_derivative(omega,
+                                                                 control_identifiers,
+                                                                 n_oper_identifiers,
                                                                  n_coeffs_deriv)
 
-    integrand = np.einsum('ao,atho->atho', spectrum, filter_function_deriv)
+    integrand = np.einsum('...o,...tho->...tho', spectrum, filter_function_deriv)
     infid_deriv = util.integrate(integrand, omega) / (2*np.pi*pulse.d)
 
     return infid_deriv
```

### Comparing `filter_functions-1.1.1/filter_functions/numeric.py` & `filter_functions-1.1.2/filter_functions/numeric.py`

 * *Files 1% similar despite different names*

```diff
@@ -632,4859 +632,4838 @@
 00002770: 7365 2077 6865 7265 206f 6d65 6761 202b  se where omega +
 00002780: 204f 6d65 6761 5f69 6a20 3d20 302c 206f   Omega_ij = 0, o
 00002790: 6d65 6761 202d 204f 6d65 6761 5f6d 6e20  mega - Omega_mn 
 000027a0: 3d20 300a 2020 2020 696e 745f 6275 665b  = 0.    int_buf[
 000027b0: 6d61 736b 5f6e 4564 455f 6e64 4545 5d20  mask_nEdE_ndEE] 
 000027c0: 3d20 6474 2a2a 3220 2f20 320a 2020 2020  = dt**2 / 2.    
 000027d0: 7265 7475 726e 2069 6e74 5f62 7566 0a0a  return int_buf..
-000027e0: 0a64 6566 205f 7061 7273 655f 7370 6563  .def _parse_spec
-000027f0: 7472 756d 2873 7065 6374 7275 6d3a 2053  trum(spectrum: S
-00002800: 6571 7565 6e63 652c 206f 6d65 6761 3a20  equence, omega: 
-00002810: 5365 7175 656e 6365 2c20 6964 783a 2053  Sequence, idx: S
-00002820: 6571 7565 6e63 6529 202d 3e20 6e64 6172  equence) -> ndar
-00002830: 7261 793a 0a20 2020 2073 7065 6374 7275  ray:.    spectru
-00002840: 6d20 3d20 6e70 2e61 7361 6e79 6172 7261  m = np.asanyarra
-00002850: 7928 7370 6563 7472 756d 290a 2020 2020  y(spectrum).    
-00002860: 6572 726f 7220 3d20 2753 7065 6374 7275  error = 'Spectru
-00002870: 6d20 7368 6f75 6c64 2062 6520 6f66 2073  m should be of s
-00002880: 6861 7065 207b 7d2c 206e 6f74 207b 7d2e  hape {}, not {}.
-00002890: 270a 2020 2020 7368 6170 6520 3d20 286c  '.    shape = (l
-000028a0: 656e 2869 6478 292c 292a 2873 7065 6374  en(idx),)*(spect
-000028b0: 7275 6d2e 6e64 696d 202d 2031 2920 2b20  rum.ndim - 1) + 
-000028c0: 286c 656e 286f 6d65 6761 292c 290a 2020  (len(omega),).  
-000028d0: 2020 6966 2073 7065 6374 7275 6d2e 7368    if spectrum.sh
-000028e0: 6170 6520 213d 2073 6861 7065 2061 6e64  ape != shape and
-000028f0: 2073 7065 6374 7275 6d2e 6e64 696d 203c   spectrum.ndim <
-00002900: 3d20 333a 0a20 2020 2020 2020 2072 6169  = 3:.        rai
-00002910: 7365 2056 616c 7565 4572 726f 7228 6572  se ValueError(er
-00002920: 726f 722e 666f 726d 6174 2873 6861 7065  ror.format(shape
-00002930: 2c20 7370 6563 7472 756d 2e73 6861 7065  , spectrum.shape
-00002940: 2929 0a0a 2020 2020 6966 2073 7065 6374  ))..    if spect
-00002950: 7275 6d2e 6e64 696d 203d 3d20 313a 0a20  rum.ndim == 1:. 
-00002960: 2020 2020 2020 2023 2041 7320 7765 2062         # As we b
-00002970: 726f 6164 6361 7374 206f 7665 7220 7468  roadcast over th
-00002980: 6520 6e6f 6973 6520 6f70 6572 6174 6f72  e noise operator
-00002990: 730a 2020 2020 2020 2020 7370 6563 7472  s.        spectr
-000029a0: 756d 203d 2073 7065 6374 7275 6d5b 4e6f  um = spectrum[No
-000029b0: 6e65 2c20 2e2e 2e5d 0a20 2020 2069 6620  ne, ...].    if 
-000029c0: 7370 6563 7472 756d 2e6e 6469 6d20 3d3d  spectrum.ndim ==
-000029d0: 2033 2061 6e64 206e 6f74 206e 702e 616c   3 and not np.al
-000029e0: 6c63 6c6f 7365 2873 7065 6374 7275 6d2c  lclose(spectrum,
-000029f0: 2073 7065 6374 7275 6d2e 636f 6e6a 2829   spectrum.conj()
-00002a00: 2e73 7761 7061 7865 7328 302c 2031 2929  .swapaxes(0, 1))
-00002a10: 3a0a 2020 2020 2020 2020 7261 6973 6520  :.        raise 
-00002a20: 5661 6c75 6545 7272 6f72 2827 4372 6f73  ValueError('Cros
-00002a30: 732d 7370 6563 7472 6120 6769 7665 6e20  s-spectra given 
-00002a40: 6275 7420 6e6f 7420 4865 726d 6974 6961  but not Hermitia
-00002a50: 6e20 616c 6f6e 6720 6669 7273 7420 7477  n along first tw
-00002a60: 6f20 6178 6573 2729 0a20 2020 2065 6c69  o axes').    eli
-00002a70: 6620 7370 6563 7472 756d 2e6e 6469 6d20  f spectrum.ndim 
-00002a80: 3e20 333a 0a20 2020 2020 2020 2072 6169  > 3:.        rai
-00002a90: 7365 2056 616c 7565 4572 726f 7228 6627  se ValueError(f'
-00002aa0: 4578 7065 6374 6564 2073 7065 6374 7275  Expected spectru
-00002ab0: 6d20 746f 2068 6176 6520 3c20 3420 6469  m to have < 4 di
-00002ac0: 6d65 6e73 696f 6e73 2c20 6e6f 7420 7b73  mensions, not {s
-00002ad0: 7065 6374 7275 6d2e 6e64 696d 7d27 290a  pectrum.ndim}').
-00002ae0: 0a20 2020 2072 6574 7572 6e20 7370 6563  .    return spec
-00002af0: 7472 756d 0a0a 0a64 6566 205f 6765 745f  trum...def _get_
-00002b00: 696e 7465 6772 616e 6428 0a20 2020 2020  integrand(.     
-00002b10: 2020 2073 7065 6374 7275 6d3a 206e 6461     spectrum: nda
-00002b20: 7272 6179 2c0a 2020 2020 2020 2020 6f6d  rray,.        om
-00002b30: 6567 613a 206e 6461 7272 6179 2c0a 2020  ega: ndarray,.  
-00002b40: 2020 2020 2020 6964 783a 206e 6461 7272        idx: ndarr
-00002b50: 6179 2c0a 2020 2020 2020 2020 7768 6963  ay,.        whic
-00002b60: 685f 7075 6c73 653a 2073 7472 2c0a 2020  h_pulse: str,.  
-00002b70: 2020 2020 2020 7768 6963 685f 4646 3a20        which_FF: 
-00002b80: 7374 722c 0a20 2020 2020 2020 2063 6f6e  str,.        con
-00002b90: 7472 6f6c 5f6d 6174 7269 783a 204f 7074  trol_matrix: Opt
-00002ba0: 696f 6e61 6c5b 556e 696f 6e5b 6e64 6172  ional[Union[ndar
-00002bb0: 7261 792c 2053 6571 7565 6e63 655b 6e64  ray, Sequence[nd
-00002bc0: 6172 7261 795d 5d5d 203d 204e 6f6e 652c  array]]] = None,
-00002bd0: 0a20 2020 2020 2020 2066 696c 7465 725f  .        filter_
-00002be0: 6675 6e63 7469 6f6e 3a20 4f70 7469 6f6e  function: Option
-00002bf0: 616c 5b6e 6461 7272 6179 5d20 3d20 4e6f  al[ndarray] = No
-00002c00: 6e65 0a29 202d 3e20 6e64 6172 7261 793a  ne.) -> ndarray:
-00002c10: 0a20 2020 2022 2222 0a20 2020 2050 7269  .    """.    Pri
-00002c20: 7661 7465 2066 756e 6374 696f 6e20 746f  vate function to
-00002c30: 2067 656e 6572 6174 6520 7468 6520 696e   generate the in
-00002c40: 7465 6772 616e 6420 666f 7220 6569 7468  tegrand for eith
-00002c50: 6572 0a20 2020 203a 6675 6e63 3a60 696e  er.    :func:`in
-00002c60: 6669 6465 6c69 7479 6020 6f72 203a 6675  fidelity` or :fu
-00002c70: 6e63 3a60 6361 6c63 756c 6174 655f 6465  nc:`calculate_de
-00002c80: 6361 795f 616d 706c 6974 7564 6573 602e  cay_amplitudes`.
-00002c90: 0a0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
-00002ca0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
-00002cb0: 2020 2020 7370 6563 7472 756d 3a20 6172      spectrum: ar
-00002cc0: 7261 795f 6c69 6b65 2c20 7368 6170 6520  ray_like, shape 
-00002cd0: 285b 5b6e 5f6e 6f70 732c 5d20 6e5f 6e6f  ([[n_nops,] n_no
-00002ce0: 7073 2c5d 206e 5f6f 6d65 6761 290a 2020  ps,] n_omega).  
-00002cf0: 2020 2020 2020 5468 6520 7477 6f2d 7369        The two-si
-00002d00: 6465 6420 6e6f 6973 6520 706f 7765 7220  ded noise power 
-00002d10: 7370 6563 7472 616c 2064 656e 7369 7479  spectral density
-00002d20: 2e0a 2020 2020 6f6d 6567 613a 2061 7272  ..    omega: arr
-00002d30: 6179 5f6c 696b 652c 0a20 2020 2020 2020  ay_like,.       
-00002d40: 2054 6865 2066 7265 7175 656e 6369 6573   The frequencies
-00002d50: 2061 7420 7768 6963 6820 746f 2063 616c   at which to cal
-00002d60: 6375 6c61 7465 2074 6865 2066 696c 7465  culate the filte
-00002d70: 7220 6675 6e63 7469 6f6e 732e 0a20 2020  r functions..   
-00002d80: 2069 6478 3a20 6e64 6172 7261 790a 2020   idx: ndarray.  
-00002d90: 2020 2020 2020 4e6f 6973 6520 6f70 6572        Noise oper
-00002da0: 6174 6f72 2069 6e64 6963 6573 2074 6f20  ator indices to 
-00002db0: 636f 6e73 6964 6572 2e0a 2020 2020 7768  consider..    wh
-00002dc0: 6963 685f 7075 6c73 653a 2073 7472 2c20  ich_pulse: str, 
-00002dd0: 6f70 7469 6f6e 616c 207b 2774 6f74 616c  optional {'total
-00002de0: 272c 2027 636f 7272 656c 6174 696f 6e73  ', 'correlations
-00002df0: 277d 0a20 2020 2020 2020 2055 7365 2070  '}.        Use p
-00002e00: 756c 7365 2063 6f72 7265 6c61 7469 6f6e  ulse correlation
-00002e10: 7320 6f72 2074 6f74 616c 2066 696c 7465  s or total filte
-00002e20: 7220 6675 6e63 7469 6f6e 2e0a 2020 2020  r function..    
-00002e30: 7768 6963 685f 4646 3a20 7374 722c 206f  which_FF: str, o
-00002e40: 7074 696f 6e61 6c20 7b27 6669 6465 6c69  ptional {'fideli
-00002e50: 7479 272c 2027 6765 6e65 7261 6c69 7a65  ty', 'generalize
-00002e60: 6427 7d0a 2020 2020 2020 2020 4669 6465  d'}.        Fide
-00002e70: 6c69 7479 206f 7220 6765 6e65 7261 6c69  lity or generali
-00002e80: 7a65 6420 6669 6c74 6572 2066 756e 6374  zed filter funct
-00002e90: 696f 6e73 2e20 4e65 6564 6564 2074 6f20  ions. Needed to 
-00002ea0: 6465 7465 726d 696e 650a 2020 2020 2020  determine.      
-00002eb0: 2020 6f75 7470 7574 2073 6861 7065 2e0a    output shape..
-00002ec0: 2020 2020 636f 6e74 726f 6c5f 6d61 7472      control_matr
-00002ed0: 6978 3a20 6e64 6172 7261 792c 206f 7074  ix: ndarray, opt
-00002ee0: 696f 6e61 6c0a 2020 2020 2020 2020 436f  ional.        Co
-00002ef0: 6e74 726f 6c20 6d61 7472 6978 2e20 4966  ntrol matrix. If
-00002f00: 2067 6976 656e 2c20 7265 7475 726e 7320   given, returns 
-00002f10: 7468 6520 696e 7465 6772 616e 6420 666f  the integrand fo
-00002f20: 720a 2020 2020 2020 2020 3a66 756e 633a  r.        :func:
-00002f30: 6063 616c 6375 6c61 7465 5f65 7272 6f72  `calculate_error
-00002f40: 5f76 6563 746f 725f 636f 7272 656c 6174  _vector_correlat
-00002f50: 696f 6e5f 6675 6e63 7469 6f6e 7360 2e20  ion_functions`. 
-00002f60: 4966 2067 6976 656e 0a20 2020 2020 2020  If given.       
-00002f70: 2061 7320 6120 6c69 7374 206f 7220 7475   as a list or tu
-00002f80: 706c 652c 2074 616b 656e 2074 6f20 6265  ple, taken to be
-00002f90: 2074 6865 206c 6566 7420 616e 6420 7269   the left and ri
-00002fa0: 6768 7420 636f 6e74 726f 6c0a 2020 2020  ght control.    
-00002fb0: 2020 2020 6d61 7472 6963 6573 2069 6e20      matrices in 
-00002fc0: 7468 6520 696e 7465 6772 616e 6420 2861  the integrand (a
-00002fd0: 6c6c 6f77 7320 666f 7220 736c 6963 696e  llows for slicin
-00002fe0: 6720 7570 2074 6865 2069 6e74 6567 7261  g up the integra
-00002ff0: 6e64 292e 0a20 2020 2066 696c 7465 725f  nd)..    filter_
-00003000: 6675 6e63 7469 6f6e 3a20 6e64 6172 7261  function: ndarra
-00003010: 792c 206f 7074 696f 6e61 6c0a 2020 2020  y, optional.    
-00003020: 2020 2020 4669 6c74 6572 2066 756e 6374      Filter funct
-00003030: 696f 6e2e 2049 6620 6769 7665 6e2c 2072  ion. If given, r
-00003040: 6574 7572 6e73 2074 6865 2069 6e74 6567  eturns the integ
-00003050: 7261 6e64 2066 6f72 0a20 2020 2020 2020  rand for.       
-00003060: 203a 6675 6e63 3a60 696e 6669 6465 6c69   :func:`infideli
-00003070: 7479 602e 0a0a 2020 2020 5261 6973 6573  ty`...    Raises
-00003080: 0a20 2020 202d 2d2d 2d2d 2d0a 2020 2020  .    ------.    
-00003090: 5661 6c75 6545 7272 6f72 0a20 2020 2020  ValueError.     
-000030a0: 2020 2049 6620 6060 7370 6563 7472 756d     If ``spectrum
-000030b0: 6060 2061 6e64 2060 6063 6f6e 7472 6f6c  `` and ``control
-000030c0: 5f6d 6174 7269 7860 6020 6f72 2060 6066  _matrix`` or ``f
-000030d0: 696c 7465 725f 6675 6e63 7469 6f6e 6060  ilter_function``
-000030e0: 2c0a 2020 2020 2020 2020 6465 7065 6e64  ,.        depend
-000030f0: 696e 6720 6f6e 2077 6869 6368 2077 6173  ing on which was
-00003100: 2067 6976 656e 2c20 6861 7665 2069 6e63   given, have inc
-00003110: 6f6d 7061 7469 626c 6520 7368 6170 6573  ompatible shapes
-00003120: 2e0a 0a20 2020 2052 6574 7572 6e73 0a20  ...    Returns. 
-00003130: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2069     -------.    i
-00003140: 6e74 6567 7261 6e64 3a20 6e64 6172 7261  ntegrand: ndarra
-00003150: 792c 2073 6861 7065 2028 2e2e 2e2c 206e  y, shape (..., n
-00003160: 5f6f 6d65 6761 290a 2020 2020 2020 2020  _omega).        
-00003170: 5468 6520 696e 7465 6772 616e 642e 2046  The integrand. F
-00003180: 6f72 206f 6e65 2d73 6964 6564 2073 7065  or one-sided spe
-00003190: 6374 7261 2028 6f6e 6c79 2070 6f73 6974  ctra (only posit
-000031a0: 6976 6520 6672 6571 7565 6e63 6965 7329  ive frequencies)
-000031b0: 0a20 2020 2020 2020 2069 7420 6d69 6768  .        it migh
-000031c0: 7420 6265 2063 6f6d 706c 6578 2e20 486f  t be complex. Ho
-000031d0: 7765 7665 722c 206d 6174 6865 6d61 7469  wever, mathemati
-000031e0: 6361 6c6c 7920 6974 2069 7320 6775 6172  cally it is guar
-000031f0: 616e 7465 6564 0a20 2020 2020 2020 2074  anteed.        t
-00003200: 6f20 6265 2073 7472 6963 746c 7920 7265  o be strictly re
-00003210: 616c 2066 6f72 2074 6865 2063 6f72 7265  al for the corre
-00003220: 6374 2074 776f 2d73 6964 6564 2073 7065  ct two-sided spe
-00003230: 6374 7275 6d2e 2054 6875 732c 0a20 2020  ctrum. Thus,.   
-00003240: 2020 2020 206f 6e6c 7920 7468 6520 7265       only the re
-00003250: 616c 2070 6172 7420 6973 2072 6574 7572  al part is retur
-00003260: 6e65 6420 696e 2061 6c6c 2063 6173 6573  ned in all cases
-00003270: 2e0a 0a20 2020 2022 2222 0a20 2020 2069  ...    """.    i
-00003280: 6620 636f 6e74 726f 6c5f 6d61 7472 6978  f control_matrix
-00003290: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000032a0: 2020 2020 2020 2320 6374 726c 5f6c 6566        # ctrl_lef
-000032b0: 7420 6973 2074 6865 2063 6f6d 706c 6578  t is the complex
-000032c0: 2063 6f6e 6a75 6761 7465 0a20 2020 2020   conjugate.     
-000032d0: 2020 2066 756e 7320 3d20 286e 702e 636f     funs = (np.co
-000032e0: 6e6a 2c20 6c61 6d62 6461 2078 3a20 7829  nj, lambda x: x)
-000032f0: 0a20 2020 2020 2020 2069 6620 6973 696e  .        if isin
-00003300: 7374 616e 6365 2863 6f6e 7472 6f6c 5f6d  stance(control_m
-00003310: 6174 7269 782c 2028 6c69 7374 2c20 7475  atrix, (list, tu
-00003320: 706c 6529 293a 0a20 2020 2020 2020 2020  ple)):.         
-00003330: 2020 2063 7472 6c5f 6c65 6674 2c20 6374     ctrl_left, ct
-00003340: 726c 5f72 6967 6874 203d 205b 6628 6329  rl_right = [f(c)
-00003350: 2066 6f72 2066 2c20 6320 696e 207a 6970   for f, c in zip
-00003360: 2866 756e 732c 2063 6f6e 7472 6f6c 5f6d  (funs, control_m
-00003370: 6174 7269 7829 5d0a 2020 2020 2020 2020  atrix)].        
-00003380: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00003390: 2020 6374 726c 5f6c 6566 742c 2063 7472    ctrl_left, ctr
-000033a0: 6c5f 7269 6768 7420 3d20 5b66 2872 2920  l_right = [f(r) 
-000033b0: 666f 7220 662c 2072 2069 6e20 7a69 7028  for f, r in zip(
-000033c0: 6675 6e73 2c20 5b63 6f6e 7472 6f6c 5f6d  funs, [control_m
-000033d0: 6174 7269 785d 2a32 295d 0a20 2020 2065  atrix]*2)].    e
-000033e0: 6c73 653a 0a20 2020 2020 2020 2023 2066  lse:.        # f
-000033f0: 696c 7465 725f 6675 6e63 7469 6f6e 2069  ilter_function i
-00003400: 7320 6e6f 7420 4e6f 6e65 0a20 2020 2020  s not None.     
-00003410: 2020 2069 6620 7768 6963 685f 4646 203d     if which_FF =
-00003420: 3d20 2767 656e 6572 616c 697a 6564 273a  = 'generalized':
-00003430: 0a20 2020 2020 2020 2020 2020 2023 2045  .            # E
-00003440: 7665 7279 7468 696e 6720 7369 6d70 6c65  verything simple
-00003450: 7220 6966 206e 6f69 7365 206f 7065 7261  r if noise opera
-00003460: 746f 7273 2061 6c77 6179 7320 6f6e 2032  tors always on 2
-00003470: 6e64 2d74 6f2d 6c61 7374 2061 7865 730a  nd-to-last axes.
-00003480: 2020 2020 2020 2020 2020 2020 6669 6c74              filt
-00003490: 6572 5f66 756e 6374 696f 6e20 3d20 6e70  er_function = np
-000034a0: 2e6d 6f76 6561 7869 7328 6669 6c74 6572  .moveaxis(filter
-000034b0: 5f66 756e 6374 696f 6e2c 2073 6f75 7263  _function, sourc
-000034c0: 653d 5b2d 352c 202d 345d 2c20 6465 7374  e=[-5, -4], dest
-000034d0: 696e 6174 696f 6e3d 5b2d 332c 202d 325d  ination=[-3, -2]
-000034e0: 290a 0a20 2020 2073 7065 6374 7275 6d20  )..    spectrum 
-000034f0: 3d20 5f70 6172 7365 5f73 7065 6374 7275  = _parse_spectru
-00003500: 6d28 7370 6563 7472 756d 2c20 6f6d 6567  m(spectrum, omeg
-00003510: 612c 2069 6478 290a 2020 2020 6966 2073  a, idx).    if s
-00003520: 7065 6374 7275 6d2e 6e64 696d 2069 6e20  pectrum.ndim in 
-00003530: 2831 2c20 3229 3a0a 2020 2020 2020 2020  (1, 2):.        
-00003540: 6966 2066 696c 7465 725f 6675 6e63 7469  if filter_functi
-00003550: 6f6e 2069 7320 6e6f 7420 4e6f 6e65 3a0a  on is not None:.
-00003560: 2020 2020 2020 2020 2020 2020 696e 7465              inte
-00003570: 6772 616e 6420 3d20 2866 696c 7465 725f  grand = (filter_
-00003580: 6675 6e63 7469 6f6e 5b2e 2e2e 2c20 7475  function[..., tu
-00003590: 706c 6528 6964 7829 2c20 7475 706c 6528  ple(idx), tuple(
-000035a0: 6964 7829 2c20 3a5d 2a73 7065 6374 7275  idx), :]*spectru
-000035b0: 6d29 0a20 2020 2020 2020 2020 2020 2069  m).            i
-000035c0: 6620 7768 6963 685f 4646 203d 3d20 2767  f which_FF == 'g
-000035d0: 656e 6572 616c 697a 6564 273a 0a20 2020  eneralized':.   
-000035e0: 2020 2020 2020 2020 2020 2020 2023 206d               # m
-000035f0: 6f76 6520 6178 6573 2062 6163 6b20 746f  ove axes back to
-00003600: 2065 7870 6563 7465 6420 706f 7369 7469   expected positi
-00003610: 6f6e 2c20 6965 2028 7075 6c73 6573 2c20  on, ie (pulses, 
-00003620: 6e6f 6973 6520 6f70 6572 732c 0a20 2020  noise opers,.   
-00003630: 2020 2020 2020 2020 2020 2020 2023 2062               # b
-00003640: 6173 6973 2065 6c65 6d65 6e74 732c 2066  asis elements, f
-00003650: 7265 7175 656e 6369 6573 290a 2020 2020  requencies).    
-00003660: 2020 2020 2020 2020 2020 2020 696e 7465              inte
-00003670: 6772 616e 6420 3d20 6e70 2e6d 6f76 6561  grand = np.movea
-00003680: 7869 7328 696e 7465 6772 616e 642c 2073  xis(integrand, s
-00003690: 6f75 7263 653d 2d32 2c20 6465 7374 696e  ource=-2, destin
-000036a0: 6174 696f 6e3d 2d34 290a 2020 2020 2020  ation=-4).      
-000036b0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-000036c0: 2020 2020 2320 5220 6973 206e 6f74 204e      # R is not N
-000036d0: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
-000036e0: 6966 2077 6869 6368 5f70 756c 7365 203d  if which_pulse =
-000036f0: 3d20 2763 6f72 7265 6c61 7469 6f6e 7327  = 'correlations'
-00003700: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00003710: 2020 6966 2077 6869 6368 5f46 4620 3d3d    if which_FF ==
-00003720: 2027 6669 6465 6c69 7479 273a 0a20 2020   'fidelity':.   
-00003730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003740: 2065 696e 7375 6d5f 7374 7220 3d20 2767   einsum_str = 'g
-00003750: 616b 6f2c 616f 2c68 616b 6f2d 3e67 6861  ako,ao,hako->gha
-00003760: 6f27 0a20 2020 2020 2020 2020 2020 2020  o'.             
-00003770: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00003780: 2020 2020 2020 2020 2020 2020 2023 2077               # w
-00003790: 6869 6368 5f46 4620 3d3d 2027 6765 6e65  hich_FF == 'gene
-000037a0: 7261 6c69 7a65 6427 0a20 2020 2020 2020  ralized'.       
-000037b0: 2020 2020 2020 2020 2020 2020 2065 696e               ein
-000037c0: 7375 6d5f 7374 7220 3d20 2767 616b 6f2c  sum_str = 'gako,
-000037d0: 616f 2c68 616c 6f2d 3e67 6861 6b6c 6f27  ao,halo->ghaklo'
-000037e0: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-000037f0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00003800: 2020 2023 2077 6869 6368 5f70 756c 7365     # which_pulse
-00003810: 203d 3d20 2774 6f74 616c 270a 2020 2020   == 'total'.    
-00003820: 2020 2020 2020 2020 2020 2020 6966 2077              if w
-00003830: 6869 6368 5f46 4620 3d3d 2027 6669 6465  hich_FF == 'fide
-00003840: 6c69 7479 273a 0a20 2020 2020 2020 2020  lity':.         
-00003850: 2020 2020 2020 2020 2020 2065 696e 7375             einsu
-00003860: 6d5f 7374 7220 3d20 2761 6b6f 2c61 6f2c  m_str = 'ako,ao,
-00003870: 616b 6f2d 3e61 6f27 0a20 2020 2020 2020  ako->ao'.       
-00003880: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+000027e0: 0a64 6566 205f 6765 745f 696e 7465 6772  .def _get_integr
+000027f0: 616e 6428 0a20 2020 2020 2020 2073 7065  and(.        spe
+00002800: 6374 7275 6d3a 206e 6461 7272 6179 2c0a  ctrum: ndarray,.
+00002810: 2020 2020 2020 2020 6f6d 6567 613a 206e          omega: n
+00002820: 6461 7272 6179 2c0a 2020 2020 2020 2020  darray,.        
+00002830: 6964 783a 206e 6461 7272 6179 2c0a 2020  idx: ndarray,.  
+00002840: 2020 2020 2020 7768 6963 685f 7075 6c73        which_puls
+00002850: 653a 2073 7472 2c0a 2020 2020 2020 2020  e: str,.        
+00002860: 7768 6963 685f 4646 3a20 7374 722c 0a20  which_FF: str,. 
+00002870: 2020 2020 2020 2063 6f6e 7472 6f6c 5f6d         control_m
+00002880: 6174 7269 783a 204f 7074 696f 6e61 6c5b  atrix: Optional[
+00002890: 556e 696f 6e5b 6e64 6172 7261 792c 2053  Union[ndarray, S
+000028a0: 6571 7565 6e63 655b 6e64 6172 7261 795d  equence[ndarray]
+000028b0: 5d5d 203d 204e 6f6e 652c 0a20 2020 2020  ]] = None,.     
+000028c0: 2020 2066 696c 7465 725f 6675 6e63 7469     filter_functi
+000028d0: 6f6e 3a20 4f70 7469 6f6e 616c 5b6e 6461  on: Optional[nda
+000028e0: 7272 6179 5d20 3d20 4e6f 6e65 0a29 202d  rray] = None.) -
+000028f0: 3e20 6e64 6172 7261 793a 0a20 2020 2022  > ndarray:.    "
+00002900: 2222 0a20 2020 2050 7269 7661 7465 2066  "".    Private f
+00002910: 756e 6374 696f 6e20 746f 2067 656e 6572  unction to gener
+00002920: 6174 6520 7468 6520 696e 7465 6772 616e  ate the integran
+00002930: 6420 666f 7220 6569 7468 6572 0a20 2020  d for either.   
+00002940: 203a 6675 6e63 3a60 696e 6669 6465 6c69   :func:`infideli
+00002950: 7479 6020 6f72 203a 6675 6e63 3a60 6361  ty` or :func:`ca
+00002960: 6c63 756c 6174 655f 6465 6361 795f 616d  lculate_decay_am
+00002970: 706c 6974 7564 6573 602e 0a0a 2020 2020  plitudes`...    
+00002980: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
+00002990: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 7370  ---------.    sp
+000029a0: 6563 7472 756d 3a20 6172 7261 795f 6c69  ectrum: array_li
+000029b0: 6b65 2c20 7368 6170 6520 285b 5b6e 5f6e  ke, shape ([[n_n
+000029c0: 6f70 732c 5d20 6e5f 6e6f 7073 2c5d 206e  ops,] n_nops,] n
+000029d0: 5f6f 6d65 6761 290a 2020 2020 2020 2020  _omega).        
+000029e0: 5468 6520 7477 6f2d 7369 6465 6420 6e6f  The two-sided no
+000029f0: 6973 6520 706f 7765 7220 7370 6563 7472  ise power spectr
+00002a00: 616c 2064 656e 7369 7479 2e0a 2020 2020  al density..    
+00002a10: 6f6d 6567 613a 2061 7272 6179 5f6c 696b  omega: array_lik
+00002a20: 652c 0a20 2020 2020 2020 2054 6865 2066  e,.        The f
+00002a30: 7265 7175 656e 6369 6573 2061 7420 7768  requencies at wh
+00002a40: 6963 6820 746f 2063 616c 6375 6c61 7465  ich to calculate
+00002a50: 2074 6865 2066 696c 7465 7220 6675 6e63   the filter func
+00002a60: 7469 6f6e 732e 0a20 2020 2069 6478 3a20  tions..    idx: 
+00002a70: 6e64 6172 7261 790a 2020 2020 2020 2020  ndarray.        
+00002a80: 4e6f 6973 6520 6f70 6572 6174 6f72 2069  Noise operator i
+00002a90: 6e64 6963 6573 2074 6f20 636f 6e73 6964  ndices to consid
+00002aa0: 6572 2e0a 2020 2020 7768 6963 685f 7075  er..    which_pu
+00002ab0: 6c73 653a 2073 7472 2c20 6f70 7469 6f6e  lse: str, option
+00002ac0: 616c 207b 2774 6f74 616c 272c 2027 636f  al {'total', 'co
+00002ad0: 7272 656c 6174 696f 6e73 277d 0a20 2020  rrelations'}.   
+00002ae0: 2020 2020 2055 7365 2070 756c 7365 2063       Use pulse c
+00002af0: 6f72 7265 6c61 7469 6f6e 7320 6f72 2074  orrelations or t
+00002b00: 6f74 616c 2066 696c 7465 7220 6675 6e63  otal filter func
+00002b10: 7469 6f6e 2e0a 2020 2020 7768 6963 685f  tion..    which_
+00002b20: 4646 3a20 7374 722c 206f 7074 696f 6e61  FF: str, optiona
+00002b30: 6c20 7b27 6669 6465 6c69 7479 272c 2027  l {'fidelity', '
+00002b40: 6765 6e65 7261 6c69 7a65 6427 7d0a 2020  generalized'}.  
+00002b50: 2020 2020 2020 4669 6465 6c69 7479 206f        Fidelity o
+00002b60: 7220 6765 6e65 7261 6c69 7a65 6420 6669  r generalized fi
+00002b70: 6c74 6572 2066 756e 6374 696f 6e73 2e20  lter functions. 
+00002b80: 4e65 6564 6564 2074 6f20 6465 7465 726d  Needed to determ
+00002b90: 696e 650a 2020 2020 2020 2020 6f75 7470  ine.        outp
+00002ba0: 7574 2073 6861 7065 2e0a 2020 2020 636f  ut shape..    co
+00002bb0: 6e74 726f 6c5f 6d61 7472 6978 3a20 6e64  ntrol_matrix: nd
+00002bc0: 6172 7261 792c 206f 7074 696f 6e61 6c0a  array, optional.
+00002bd0: 2020 2020 2020 2020 436f 6e74 726f 6c20          Control 
+00002be0: 6d61 7472 6978 2e20 4966 2067 6976 656e  matrix. If given
+00002bf0: 2c20 7265 7475 726e 7320 7468 6520 696e  , returns the in
+00002c00: 7465 6772 616e 6420 666f 720a 2020 2020  tegrand for.    
+00002c10: 2020 2020 3a66 756e 633a 6063 616c 6375      :func:`calcu
+00002c20: 6c61 7465 5f65 7272 6f72 5f76 6563 746f  late_error_vecto
+00002c30: 725f 636f 7272 656c 6174 696f 6e5f 6675  r_correlation_fu
+00002c40: 6e63 7469 6f6e 7360 2e20 4966 2067 6976  nctions`. If giv
+00002c50: 656e 0a20 2020 2020 2020 2061 7320 6120  en.        as a 
+00002c60: 6c69 7374 206f 7220 7475 706c 652c 2074  list or tuple, t
+00002c70: 616b 656e 2074 6f20 6265 2074 6865 206c  aken to be the l
+00002c80: 6566 7420 616e 6420 7269 6768 7420 636f  eft and right co
+00002c90: 6e74 726f 6c0a 2020 2020 2020 2020 6d61  ntrol.        ma
+00002ca0: 7472 6963 6573 2069 6e20 7468 6520 696e  trices in the in
+00002cb0: 7465 6772 616e 6420 2861 6c6c 6f77 7320  tegrand (allows 
+00002cc0: 666f 7220 736c 6963 696e 6720 7570 2074  for slicing up t
+00002cd0: 6865 2069 6e74 6567 7261 6e64 292e 0a20  he integrand).. 
+00002ce0: 2020 2066 696c 7465 725f 6675 6e63 7469     filter_functi
+00002cf0: 6f6e 3a20 6e64 6172 7261 792c 206f 7074  on: ndarray, opt
+00002d00: 696f 6e61 6c0a 2020 2020 2020 2020 4669  ional.        Fi
+00002d10: 6c74 6572 2066 756e 6374 696f 6e2e 2049  lter function. I
+00002d20: 6620 6769 7665 6e2c 2072 6574 7572 6e73  f given, returns
+00002d30: 2074 6865 2069 6e74 6567 7261 6e64 2066   the integrand f
+00002d40: 6f72 0a20 2020 2020 2020 203a 6675 6e63  or.        :func
+00002d50: 3a60 696e 6669 6465 6c69 7479 602e 0a0a  :`infidelity`...
+00002d60: 2020 2020 5261 6973 6573 0a20 2020 202d      Raises.    -
+00002d70: 2d2d 2d2d 2d0a 2020 2020 5661 6c75 6545  -----.    ValueE
+00002d80: 7272 6f72 0a20 2020 2020 2020 2049 6620  rror.        If 
+00002d90: 6060 7370 6563 7472 756d 6060 2061 6e64  ``spectrum`` and
+00002da0: 2060 6063 6f6e 7472 6f6c 5f6d 6174 7269   ``control_matri
+00002db0: 7860 6020 6f72 2060 6066 696c 7465 725f  x`` or ``filter_
+00002dc0: 6675 6e63 7469 6f6e 6060 2c0a 2020 2020  function``,.    
+00002dd0: 2020 2020 6465 7065 6e64 696e 6720 6f6e      depending on
+00002de0: 2077 6869 6368 2077 6173 2067 6976 656e   which was given
+00002df0: 2c20 6861 7665 2069 6e63 6f6d 7061 7469  , have incompati
+00002e00: 626c 6520 7368 6170 6573 2e0a 0a20 2020  ble shapes...   
+00002e10: 2052 6574 7572 6e73 0a20 2020 202d 2d2d   Returns.    ---
+00002e20: 2d2d 2d2d 0a20 2020 2069 6e74 6567 7261  ----.    integra
+00002e30: 6e64 3a20 6e64 6172 7261 792c 2073 6861  nd: ndarray, sha
+00002e40: 7065 2028 2e2e 2e2c 206e 5f6f 6d65 6761  pe (..., n_omega
+00002e50: 290a 2020 2020 2020 2020 5468 6520 696e  ).        The in
+00002e60: 7465 6772 616e 642e 2046 6f72 206f 6e65  tegrand. For one
+00002e70: 2d73 6964 6564 2073 7065 6374 7261 2028  -sided spectra (
+00002e80: 6f6e 6c79 2070 6f73 6974 6976 6520 6672  only positive fr
+00002e90: 6571 7565 6e63 6965 7329 0a20 2020 2020  equencies).     
+00002ea0: 2020 2069 7420 6d69 6768 7420 6265 2063     it might be c
+00002eb0: 6f6d 706c 6578 2e20 486f 7765 7665 722c  omplex. However,
+00002ec0: 206d 6174 6865 6d61 7469 6361 6c6c 7920   mathematically 
+00002ed0: 6974 2069 7320 6775 6172 616e 7465 6564  it is guaranteed
+00002ee0: 0a20 2020 2020 2020 2074 6f20 6265 2073  .        to be s
+00002ef0: 7472 6963 746c 7920 7265 616c 2066 6f72  trictly real for
+00002f00: 2074 6865 2063 6f72 7265 6374 2074 776f   the correct two
+00002f10: 2d73 6964 6564 2073 7065 6374 7275 6d2e  -sided spectrum.
+00002f20: 2054 6875 732c 0a20 2020 2020 2020 206f   Thus,.        o
+00002f30: 6e6c 7920 7468 6520 7265 616c 2070 6172  nly the real par
+00002f40: 7420 6973 2072 6574 7572 6e65 6420 696e  t is returned in
+00002f50: 2061 6c6c 2063 6173 6573 2e0a 0a20 2020   all cases...   
+00002f60: 2022 2222 0a20 2020 2069 6620 636f 6e74   """.    if cont
+00002f70: 726f 6c5f 6d61 7472 6978 2069 7320 6e6f  rol_matrix is no
+00002f80: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00002f90: 2320 6374 726c 5f6c 6566 7420 6973 2074  # ctrl_left is t
+00002fa0: 6865 2063 6f6d 706c 6578 2063 6f6e 6a75  he complex conju
+00002fb0: 6761 7465 0a20 2020 2020 2020 2066 756e  gate.        fun
+00002fc0: 7320 3d20 286e 702e 636f 6e6a 2c20 6c61  s = (np.conj, la
+00002fd0: 6d62 6461 2078 3a20 7829 0a20 2020 2020  mbda x: x).     
+00002fe0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+00002ff0: 2863 6f6e 7472 6f6c 5f6d 6174 7269 782c  (control_matrix,
+00003000: 2028 6c69 7374 2c20 7475 706c 6529 293a   (list, tuple)):
+00003010: 0a20 2020 2020 2020 2020 2020 2063 7472  .            ctr
+00003020: 6c5f 6c65 6674 2c20 6374 726c 5f72 6967  l_left, ctrl_rig
+00003030: 6874 203d 205b 6628 6329 2066 6f72 2066  ht = [f(c) for f
+00003040: 2c20 6320 696e 207a 6970 2866 756e 732c  , c in zip(funs,
+00003050: 2063 6f6e 7472 6f6c 5f6d 6174 7269 7829   control_matrix)
+00003060: 5d0a 2020 2020 2020 2020 656c 7365 3a0a  ].        else:.
+00003070: 2020 2020 2020 2020 2020 2020 6374 726c              ctrl
+00003080: 5f6c 6566 742c 2063 7472 6c5f 7269 6768  _left, ctrl_righ
+00003090: 7420 3d20 5b66 2872 2920 666f 7220 662c  t = [f(r) for f,
+000030a0: 2072 2069 6e20 7a69 7028 6675 6e73 2c20   r in zip(funs, 
+000030b0: 5b63 6f6e 7472 6f6c 5f6d 6174 7269 785d  [control_matrix]
+000030c0: 2a32 295d 0a20 2020 2065 6c73 653a 0a20  *2)].    else:. 
+000030d0: 2020 2020 2020 2023 2066 696c 7465 725f         # filter_
+000030e0: 6675 6e63 7469 6f6e 2069 7320 6e6f 7420  function is not 
+000030f0: 4e6f 6e65 0a20 2020 2020 2020 2069 6620  None.        if 
+00003100: 7768 6963 685f 4646 203d 3d20 2767 656e  which_FF == 'gen
+00003110: 6572 616c 697a 6564 273a 0a20 2020 2020  eralized':.     
+00003120: 2020 2020 2020 2023 2045 7665 7279 7468         # Everyth
+00003130: 696e 6720 7369 6d70 6c65 7220 6966 206e  ing simpler if n
+00003140: 6f69 7365 206f 7065 7261 746f 7273 2061  oise operators a
+00003150: 6c77 6179 7320 6f6e 2032 6e64 2d74 6f2d  lways on 2nd-to-
+00003160: 6c61 7374 2061 7865 730a 2020 2020 2020  last axes.      
+00003170: 2020 2020 2020 6669 6c74 6572 5f66 756e        filter_fun
+00003180: 6374 696f 6e20 3d20 6e70 2e6d 6f76 6561  ction = np.movea
+00003190: 7869 7328 6669 6c74 6572 5f66 756e 6374  xis(filter_funct
+000031a0: 696f 6e2c 2073 6f75 7263 653d 5b2d 352c  ion, source=[-5,
+000031b0: 202d 345d 2c20 6465 7374 696e 6174 696f   -4], destinatio
+000031c0: 6e3d 5b2d 332c 202d 325d 290a 0a20 2020  n=[-3, -2])..   
+000031d0: 2073 7065 6374 7275 6d20 3d20 7574 696c   spectrum = util
+000031e0: 2e70 6172 7365 5f73 7065 6374 7275 6d28  .parse_spectrum(
+000031f0: 7370 6563 7472 756d 2c20 6f6d 6567 612c  spectrum, omega,
+00003200: 2069 6478 290a 2020 2020 6966 2073 7065   idx).    if spe
+00003210: 6374 7275 6d2e 6e64 696d 2069 6e20 2831  ctrum.ndim in (1
+00003220: 2c20 3229 3a0a 2020 2020 2020 2020 6966  , 2):.        if
+00003230: 2066 696c 7465 725f 6675 6e63 7469 6f6e   filter_function
+00003240: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00003250: 2020 2020 2020 2020 2020 696e 7465 6772            integr
+00003260: 616e 6420 3d20 2866 696c 7465 725f 6675  and = (filter_fu
+00003270: 6e63 7469 6f6e 5b2e 2e2e 2c20 7475 706c  nction[..., tupl
+00003280: 6528 6964 7829 2c20 7475 706c 6528 6964  e(idx), tuple(id
+00003290: 7829 2c20 3a5d 2a73 7065 6374 7275 6d29  x), :]*spectrum)
+000032a0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+000032b0: 7768 6963 685f 4646 203d 3d20 2767 656e  which_FF == 'gen
+000032c0: 6572 616c 697a 6564 273a 0a20 2020 2020  eralized':.     
+000032d0: 2020 2020 2020 2020 2020 2023 206d 6f76             # mov
+000032e0: 6520 6178 6573 2062 6163 6b20 746f 2065  e axes back to e
+000032f0: 7870 6563 7465 6420 706f 7369 7469 6f6e  xpected position
+00003300: 2c20 6965 2028 7075 6c73 6573 2c20 6e6f  , ie (pulses, no
+00003310: 6973 6520 6f70 6572 732c 0a20 2020 2020  ise opers,.     
+00003320: 2020 2020 2020 2020 2020 2023 2062 6173             # bas
+00003330: 6973 2065 6c65 6d65 6e74 732c 2066 7265  is elements, fre
+00003340: 7175 656e 6369 6573 290a 2020 2020 2020  quencies).      
+00003350: 2020 2020 2020 2020 2020 696e 7465 6772            integr
+00003360: 616e 6420 3d20 6e70 2e6d 6f76 6561 7869  and = np.moveaxi
+00003370: 7328 696e 7465 6772 616e 642c 2073 6f75  s(integrand, sou
+00003380: 7263 653d 2d32 2c20 6465 7374 696e 6174  rce=-2, destinat
+00003390: 696f 6e3d 2d34 290a 2020 2020 2020 2020  ion=-4).        
+000033a0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+000033b0: 2020 2320 5220 6973 206e 6f74 204e 6f6e    # R is not Non
+000033c0: 650a 2020 2020 2020 2020 2020 2020 6966  e.            if
+000033d0: 2077 6869 6368 5f70 756c 7365 203d 3d20   which_pulse == 
+000033e0: 2763 6f72 7265 6c61 7469 6f6e 7327 3a0a  'correlations':.
+000033f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003400: 6966 2077 6869 6368 5f46 4620 3d3d 2027  if which_FF == '
+00003410: 6669 6465 6c69 7479 273a 0a20 2020 2020  fidelity':.     
+00003420: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00003430: 696e 7375 6d5f 7374 7220 3d20 2767 2e2e  insum_str = 'g..
+00003440: 2e6b 6f2c 2e2e 2e6f 2c68 2e2e 2e6b 6f2d  .ko,...o,h...ko-
+00003450: 3e67 682e 2e2e 6f27 0a20 2020 2020 2020  >gh...o'.       
+00003460: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+00003470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003480: 2020 2023 2077 6869 6368 5f46 4620 3d3d     # which_FF ==
+00003490: 2027 6765 6e65 7261 6c69 7a65 6427 0a20   'generalized'. 
+000034a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000034b0: 2020 2065 696e 7375 6d5f 7374 7220 3d20     einsum_str = 
+000034c0: 2767 2e2e 2e6b 6f2c 2e2e 2e6f 2c68 2e2e  'g...ko,...o,h..
+000034d0: 2e6c 6f2d 3e67 682e 2e2e 6b6c 6f27 0a20  .lo->gh...klo'. 
+000034e0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+000034f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003500: 2023 2077 6869 6368 5f70 756c 7365 203d   # which_pulse =
+00003510: 3d20 2774 6f74 616c 270a 2020 2020 2020  = 'total'.      
+00003520: 2020 2020 2020 2020 2020 6966 2077 6869            if whi
+00003530: 6368 5f46 4620 3d3d 2027 6669 6465 6c69  ch_FF == 'fideli
+00003540: 7479 273a 0a20 2020 2020 2020 2020 2020  ty':.           
+00003550: 2020 2020 2020 2020 2065 696e 7375 6d5f           einsum_
+00003560: 7374 7220 3d20 272e 2e2e 6b6f 2c2e 2e2e  str = '...ko,...
+00003570: 6f2c 2e2e 2e6b 6f2d 3e2e 2e2e 6f27 0a20  o,...ko->...o'. 
+00003580: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00003590: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+000035a0: 2020 2020 2020 2020 2023 2077 6869 6368           # which
+000035b0: 5f46 4620 3d3d 2027 6765 6e65 7261 6c69  _FF == 'generali
+000035c0: 7a65 6427 0a20 2020 2020 2020 2020 2020  zed'.           
+000035d0: 2020 2020 2020 2020 2065 696e 7375 6d5f           einsum_
+000035e0: 7374 7220 3d20 272e 2e2e 6b6f 2c2e 2e2e  str = '...ko,...
+000035f0: 6f2c 2e2e 2e6c 6f2d 3e2e 2e2e 6b6c 6f27  o,...lo->...klo'
+00003600: 0a0a 2020 2020 2020 2020 2020 2020 696e  ..            in
+00003610: 7465 6772 616e 6420 3d20 6e70 2e65 696e  tegrand = np.ein
+00003620: 7375 6d28 6569 6e73 756d 5f73 7472 2c0a  sum(einsum_str,.
+00003630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003650: 2020 6374 726c 5f6c 6566 745b 2e2e 2e2c    ctrl_left[...,
+00003660: 2069 6478 2c20 3a2c 203a 5d2c 2073 7065   idx, :, :], spe
+00003670: 6374 7275 6d2c 2063 7472 6c5f 7269 6768  ctrum, ctrl_righ
+00003680: 745b 2e2e 2e2c 2069 6478 2c20 3a2c 203a  t[..., idx, :, :
+00003690: 5d29 0a20 2020 2065 6c73 653a 0a20 2020  ]).    else:.   
+000036a0: 2020 2020 2023 2073 7065 6374 7275 6d2e       # spectrum.
+000036b0: 6e64 696d 203d 3d20 332c 2067 656e 6572  ndim == 3, gener
+000036c0: 616c 2063 6173 6520 7768 6572 6520 7370  al case where sp
+000036d0: 6563 7472 756d 2069 7320 6120 6d61 7472  ectrum is a matr
+000036e0: 6978 2077 6974 680a 2020 2020 2020 2020  ix with.        
+000036f0: 2320 636f 7272 656c 6174 696f 6e20 7370  # correlation sp
+00003700: 6563 7472 6120 6f6e 206f 6666 2d64 6961  ectra on off-dia
+00003710: 670a 2020 2020 2020 2020 6966 2066 696c  g.        if fil
+00003720: 7465 725f 6675 6e63 7469 6f6e 2069 7320  ter_function is 
+00003730: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00003740: 2020 2020 2020 696e 7465 6772 616e 6420        integrand 
+00003750: 3d20 6669 6c74 6572 5f66 756e 6374 696f  = filter_functio
+00003760: 6e5b 2e2e 2e2c 2069 6478 5b3a 2c20 4e6f  n[..., idx[:, No
+00003770: 6e65 5d2c 2069 6478 2c20 3a5d 2a73 7065  ne], idx, :]*spe
+00003780: 6374 7275 6d0a 2020 2020 2020 2020 2020  ctrum.          
+00003790: 2020 6966 2077 6869 6368 5f46 4620 3d3d    if which_FF ==
+000037a0: 2027 6765 6e65 7261 6c69 7a65 6427 3a0a   'generalized':.
+000037b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000037c0: 696e 7465 6772 616e 6420 3d20 6e70 2e6d  integrand = np.m
+000037d0: 6f76 6561 7869 7328 696e 7465 6772 616e  oveaxis(integran
+000037e0: 642c 2073 6f75 7263 653d 5b2d 332c 202d  d, source=[-3, -
+000037f0: 325d 2c20 6465 7374 696e 6174 696f 6e3d  2], destination=
+00003800: 5b2d 352c 202d 345d 290a 2020 2020 2020  [-5, -4]).      
+00003810: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00003820: 2020 2020 2320 5220 6973 206e 6f74 204e      # R is not N
+00003830: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
+00003840: 6966 2077 6869 6368 5f70 756c 7365 203d  if which_pulse =
+00003850: 3d20 2763 6f72 7265 6c61 7469 6f6e 7327  = 'correlations'
+00003860: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00003870: 2020 6966 2077 6869 6368 5f46 4620 3d3d    if which_FF ==
+00003880: 2027 6669 6465 6c69 7479 273a 0a20 2020   'fidelity':.   
 00003890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000038a0: 2020 2023 2077 6869 6368 5f46 4620 3d3d     # which_FF ==
-000038b0: 2027 6765 6e65 7261 6c69 7a65 6427 0a20   'generalized'. 
-000038c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000038d0: 2020 2065 696e 7375 6d5f 7374 7220 3d20     einsum_str = 
-000038e0: 2761 6b6f 2c61 6f2c 616c 6f2d 3e61 6b6c  'ako,ao,alo->akl
-000038f0: 6f27 0a0a 2020 2020 2020 2020 2020 2020  o'..            
-00003900: 696e 7465 6772 616e 6420 3d20 6e70 2e65  integrand = np.e
-00003910: 696e 7375 6d28 6569 6e73 756d 5f73 7472  insum(einsum_str
-00003920: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00003930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003940: 2020 2020 6374 726c 5f6c 6566 745b 2e2e      ctrl_left[..
-00003950: 2e2c 2069 6478 2c20 3a2c 203a 5d2c 2073  ., idx, :, :], s
-00003960: 7065 6374 7275 6d2c 2063 7472 6c5f 7269  pectrum, ctrl_ri
-00003970: 6768 745b 2e2e 2e2c 2069 6478 2c20 3a2c  ght[..., idx, :,
-00003980: 203a 5d29 0a20 2020 2065 6c73 653a 0a20   :]).    else:. 
-00003990: 2020 2020 2020 2023 2073 7065 6374 7275         # spectru
-000039a0: 6d2e 6e64 696d 203d 3d20 332c 2067 656e  m.ndim == 3, gen
-000039b0: 6572 616c 2063 6173 6520 7768 6572 6520  eral case where 
-000039c0: 7370 6563 7472 756d 2069 7320 6120 6d61  spectrum is a ma
-000039d0: 7472 6978 2077 6974 680a 2020 2020 2020  trix with.      
-000039e0: 2020 2320 636f 7272 656c 6174 696f 6e20    # correlation 
-000039f0: 7370 6563 7472 6120 6f6e 206f 6666 2d64  spectra on off-d
-00003a00: 6961 670a 2020 2020 2020 2020 6966 2066  iag.        if f
-00003a10: 696c 7465 725f 6675 6e63 7469 6f6e 2069  ilter_function i
-00003a20: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00003a30: 2020 2020 2020 2020 696e 7465 6772 616e          integran
-00003a40: 6420 3d20 6669 6c74 6572 5f66 756e 6374  d = filter_funct
-00003a50: 696f 6e5b 2e2e 2e2c 2069 6478 5b3a 2c20  ion[..., idx[:, 
-00003a60: 4e6f 6e65 5d2c 2069 6478 2c20 3a5d 2a73  None], idx, :]*s
-00003a70: 7065 6374 7275 6d0a 2020 2020 2020 2020  pectrum.        
-00003a80: 2020 2020 6966 2077 6869 6368 5f46 4620      if which_FF 
-00003a90: 3d3d 2027 6765 6e65 7261 6c69 7a65 6427  == 'generalized'
-00003aa0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00003ab0: 2020 696e 7465 6772 616e 6420 3d20 6e70    integrand = np
-00003ac0: 2e6d 6f76 6561 7869 7328 696e 7465 6772  .moveaxis(integr
-00003ad0: 616e 642c 2073 6f75 7263 653d 5b2d 332c  and, source=[-3,
-00003ae0: 202d 325d 2c20 6465 7374 696e 6174 696f   -2], destinatio
-00003af0: 6e3d 5b2d 352c 202d 345d 290a 2020 2020  n=[-5, -4]).    
-00003b00: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00003b10: 2020 2020 2020 2320 5220 6973 206e 6f74        # R is not
-00003b20: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
-00003b30: 2020 6966 2077 6869 6368 5f70 756c 7365    if which_pulse
-00003b40: 203d 3d20 2763 6f72 7265 6c61 7469 6f6e   == 'correlation
-00003b50: 7327 3a0a 2020 2020 2020 2020 2020 2020  s':.            
-00003b60: 2020 2020 6966 2077 6869 6368 5f46 4620      if which_FF 
-00003b70: 3d3d 2027 6669 6465 6c69 7479 273a 0a20  == 'fidelity':. 
-00003b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b90: 2020 2065 696e 7375 6d5f 7374 7220 3d20     einsum_str = 
-00003ba0: 2767 616b 6f2c 6162 6f2c 6862 6b6f 2d3e  'gako,abo,hbko->
-00003bb0: 6768 6162 6f27 0a20 2020 2020 2020 2020  ghabo'.         
-00003bc0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00003bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003be0: 2023 2077 6869 6368 5f46 4620 3d3d 2027   # which_FF == '
-00003bf0: 6765 6e65 7261 6c69 7a65 6427 0a20 2020  generalized'.   
-00003c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c10: 2065 696e 7375 6d5f 7374 7220 3d20 2767   einsum_str = 'g
-00003c20: 616b 6f2c 6162 6f2c 6862 6c6f 2d3e 6768  ako,abo,hblo->gh
-00003c30: 6162 6b6c 6f27 0a20 2020 2020 2020 2020  abklo'.         
-00003c40: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00003c50: 2020 2020 2020 2020 2023 2077 6869 6368           # which
-00003c60: 5f70 756c 7365 203d 3d20 2774 6f74 616c  _pulse == 'total
-00003c70: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
-00003c80: 2020 6966 2077 6869 6368 5f46 4620 3d3d    if which_FF ==
-00003c90: 2027 6669 6465 6c69 7479 273a 0a20 2020   'fidelity':.   
-00003ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003cb0: 2065 696e 7375 6d5f 7374 7220 3d20 2761   einsum_str = 'a
-00003cc0: 6b6f 2c61 626f 2c62 6b6f 2d3e 6162 6f27  ko,abo,bko->abo'
-00003cd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003ce0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00003cf0: 2020 2020 2020 2020 2020 2023 2077 6869             # whi
-00003d00: 6368 5f46 4620 3d3d 2027 6765 6e65 7261  ch_FF == 'genera
-00003d10: 6c69 7a65 6427 0a20 2020 2020 2020 2020  lized'.         
-00003d20: 2020 2020 2020 2020 2020 2065 696e 7375             einsu
-00003d30: 6d5f 7374 7220 3d20 2761 6b6f 2c61 626f  m_str = 'ako,abo
-00003d40: 2c62 6c6f 2d3e 6162 6b6c 6f27 0a0a 2020  ,blo->abklo'..  
-00003d50: 2020 2020 2020 2020 2020 696e 7465 6772            integr
-00003d60: 616e 6420 3d20 6e70 2e65 696e 7375 6d28  and = np.einsum(
-00003d70: 6569 6e73 756d 5f73 7472 2c0a 2020 2020  einsum_str,.    
-00003d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d90: 2020 2020 2020 2020 2020 2020 2020 6374                ct
-00003da0: 726c 5f6c 6566 745b 2e2e 2e2c 2069 6478  rl_left[..., idx
-00003db0: 2c20 3a2c 203a 5d2c 2073 7065 6374 7275  , :, :], spectru
-00003dc0: 6d2c 2063 7472 6c5f 7269 6768 745b 2e2e  m, ctrl_right[..
-00003dd0: 2e2c 2069 6478 2c20 3a2c 203a 5d29 0a0a  ., idx, :, :])..
-00003de0: 2020 2020 7265 7475 726e 2069 6e74 6567      return integ
-00003df0: 7261 6e64 2e72 6561 6c0a 0a0a 6465 6620  rand.real...def 
-00003e00: 6361 6c63 756c 6174 655f 6e6f 6973 655f  calculate_noise_
-00003e10: 6f70 6572 6174 6f72 735f 6672 6f6d 5f61  operators_from_a
-00003e20: 746f 6d69 6328 0a20 2020 2020 2020 2070  tomic(.        p
-00003e30: 6861 7365 733a 206e 6461 7272 6179 2c0a  hases: ndarray,.
-00003e40: 2020 2020 2020 2020 6e6f 6973 655f 6f70          noise_op
-00003e50: 6572 6174 6f72 735f 6174 6f6d 6963 3a20  erators_atomic: 
-00003e60: 6e64 6172 7261 792c 0a20 2020 2020 2020  ndarray,.       
-00003e70: 2070 726f 7061 6761 746f 7273 3a20 6e64   propagators: nd
-00003e80: 6172 7261 792c 0a20 2020 2020 2020 2073  array,.        s
-00003e90: 686f 775f 7072 6f67 7265 7373 6261 723a  how_progressbar:
-00003ea0: 2062 6f6f 6c20 3d20 4661 6c73 650a 2920   bool = False.) 
-00003eb0: 2d3e 206e 6461 7272 6179 3a0a 2020 2020  -> ndarray:.    
-00003ec0: 7222 2222 0a20 2020 2043 616c 6375 6c61  r""".    Calcula
-00003ed0: 7465 2074 6865 2069 6e74 6572 6163 7469  te the interacti
-00003ee0: 6f6e 2070 6963 7574 7265 206e 6f69 7365  on picutre noise
-00003ef0: 206f 7065 7261 746f 7273 2066 726f 6d20   operators from 
-00003f00: 6174 6f6d 6963 2073 6567 6d65 6e74 732e  atomic segments.
-00003f10: 0a0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
-00003f20: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
-00003f30: 2020 2020 7068 6173 6573 3a20 6172 7261      phases: arra
-00003f40: 795f 6c69 6b65 2c20 7368 6170 6520 286e  y_like, shape (n
-00003f50: 5f64 742c 206e 5f6f 6d65 6761 290a 2020  _dt, n_omega).  
-00003f60: 2020 2020 2020 5468 6520 7068 6173 6520        The phase 
-00003f70: 6661 6374 6f72 7320 666f 7220 3a6d 6174  factors for :mat
-00003f80: 683a 6067 5c69 6e5c 7b30 2c20 312c 205c  h:`g\in\{0, 1, \
-00003f90: 646f 7473 2c20 472d 315c 7d60 2e0a 2020  dots, G-1\}`..  
-00003fa0: 2020 6e6f 6973 655f 6f70 6572 6174 6f72    noise_operator
-00003fb0: 735f 6174 6f6d 6963 3a20 6172 7261 795f  s_atomic: array_
-00003fc0: 6c69 6b65 2c20 7368 6170 6520 286e 5f64  like, shape (n_d
-00003fd0: 742c 206e 5f6e 6f70 732c 2064 2c20 642c  t, n_nops, d, d,
-00003fe0: 206e 5f6f 6d65 6761 290a 2020 2020 2020   n_omega).      
-00003ff0: 2020 5468 6520 6e6f 6973 6520 6f70 6572    The noise oper
-00004000: 6174 6f72 7320 696e 2074 6865 2069 6e74  ators in the int
-00004010: 6572 6163 7469 6f6e 2070 6963 7475 7265  eraction picture
-00004020: 206f 6620 7468 6520 672d 7468 0a20 2020   of the g-th.   
-00004030: 2020 2020 2070 756c 7365 2c20 692e 652e       pulse, i.e.
-00004040: 2066 6f72 203a 6d61 7468 3a60 675c 696e   for :math:`g\in
-00004050: 5c7b 312c 2032 2c20 5c64 6f74 732c 2047  \{1, 2, \dots, G
-00004060: 5c7d 602e 0a20 2020 2070 726f 7061 6761  \}`..    propaga
-00004070: 746f 7273 3a20 6172 7261 795f 6c69 6b65  tors: array_like
-00004080: 2c20 7368 6170 6520 286e 5f64 742c 2064  , shape (n_dt, d
-00004090: 2c20 6429 0a20 2020 2020 2020 2054 6865  , d).        The
-000040a0: 2063 756d 756c 6174 6976 6520 7072 6f70   cumulative prop
-000040b0: 6167 6174 6f72 7320 6f66 2074 6865 2070  agators of the p
-000040c0: 756c 7365 730a 2020 2020 2020 2020 3a6d  ulses.        :m
-000040d0: 6174 683a 6067 5c69 6e5c 7b30 2c20 312c  ath:`g\in\{0, 1,
-000040e0: 205c 646f 7473 2c20 472d 315c 7d60 2e0a   \dots, G-1\}`..
-000040f0: 2020 2020 7368 6f77 5f70 726f 6772 6573      show_progres
-00004100: 7362 6172 3a20 626f 6f6c 2c20 6f70 7469  sbar: bool, opti
-00004110: 6f6e 616c 0a20 2020 2020 2020 2053 686f  onal.        Sho
-00004120: 7720 6120 7072 6f67 7265 7373 2062 6172  w a progress bar
-00004130: 2066 6f72 2074 6865 2063 616c 6375 6c61   for the calcula
-00004140: 7469 6f6e 2e0a 0a20 2020 2052 6574 7572  tion...    Retur
-00004150: 6e73 0a20 2020 202d 2d2d 2d2d 2d2d 0a20  ns.    -------. 
-00004160: 2020 206e 6f69 7365 5f6f 7065 7261 746f     noise_operato
-00004170: 7273 3a20 6e64 6172 7261 792c 2073 6861  rs: ndarray, sha
-00004180: 7065 2028 6e5f 6f6d 6567 612c 206e 5f6e  pe (n_omega, n_n
-00004190: 6f70 732c 2064 2c20 6429 0a20 2020 2020  ops, d, d).     
-000041a0: 2020 2054 6865 2069 6e74 6572 6163 7469     The interacti
-000041b0: 6f6e 2070 6963 7475 7265 206e 6f69 7365  on picture noise
-000041c0: 206f 7065 7261 746f 7273 0a20 2020 2020   operators.     
-000041d0: 2020 203a 6d61 7468 3a60 5c74 696c 6465     :math:`\tilde
-000041e0: 7b42 7d5f 5c61 6c70 6861 285c 6f6d 6567  {B}_\alpha(\omeg
-000041f0: 6129 602e 0a0a 2020 2020 4e6f 7465 730a  a)`...    Notes.
-00004200: 2020 2020 2d2d 2d2d 2d0a 2020 2020 5468      -----.    Th
-00004210: 6520 6e6f 6973 6520 6f70 6572 6174 6f72  e noise operator
-00004220: 7320 6172 6520 6361 6c63 756c 6174 6564  s are calculated
-00004230: 2062 7920 6576 616c 7561 7469 6e67 2074   by evaluating t
-00004240: 6865 2073 756d 0a0a 2020 2020 2e2e 206d  he sum..    .. m
-00004250: 6174 683a 3a0a 0a20 2020 2020 2020 205c  ath::..        \
-00004260: 7469 6c64 657b 427d 5f5c 616c 7068 6128  tilde{B}_\alpha(
-00004270: 5c6f 6d65 6761 2920 3d20 5c73 756d 5f7b  \omega) = \sum_{
-00004280: 673d 317d 5e47 2065 5e7b 695c 6f6d 6567  g=1}^G e^{i\omeg
-00004290: 6120 745f 7b67 2d31 7d7d 0a20 2020 2020  a t_{g-1}}.     
-000042a0: 2020 2020 2020 2020 515f 7b67 2d31 7d5e          Q_{g-1}^
-000042b0: 5c64 6167 6765 725c 7469 6c64 657b 427d  \dagger\tilde{B}
-000042c0: 5f5c 616c 7068 615e 7b28 6729 7d28 5c6f  _\alpha^{(g)}(\o
-000042d0: 6d65 6761 2920 515f 7b67 2d31 7d2e 0a0a  mega) Q_{g-1}...
-000042e0: 2020 2020 5468 6520 636f 6e74 726f 6c20      The control 
-000042f0: 6d61 7472 6978 2074 6865 6e20 636f 7272  matrix then corr
-00004300: 6573 706f 6e64 7320 746f 2074 6865 2063  esponds to the c
-00004310: 6f65 6666 6963 6965 6e74 7320 6f66 2065  oefficients of e
-00004320: 7870 616e 7369 6f6e 0a20 2020 2069 6e20  xpansion.    in 
-00004330: 616e 206f 7065 7261 746f 7220 6261 7369  an operator basi
-00004340: 7320 3a6d 6174 683a 605c 7b43 5f6b 5c7d  s :math:`\{C_k\}
-00004350: 5f6b 603a 0a0a 2020 2020 2e2e 206d 6174  _k`:..    .. mat
-00004360: 683a 3a0a 2020 2020 2020 2020 5c74 696c  h::.        \til
-00004370: 6465 7b5c 6d61 7468 6361 6c7b 427d 7d5f  de{\mathcal{B}}_
-00004380: 7b6b 5c61 6c70 6861 7d28 5c6f 6d65 6761  {k\alpha}(\omega
-00004390: 2920 3d0a 2020 2020 2020 2020 2020 2020  ) =.            
-000043a0: 5c6d 6174 6872 6d7b 7472 7d28 5c74 696c  \mathrm{tr}(\til
-000043b0: 6465 7b42 7d5f 5c61 6c70 6861 285c 6f6d  de{B}_\alpha(\om
-000043c0: 6567 6129 2043 5f6b 292e 0a0a 2020 2020  ega) C_k)...    
-000043d0: 4475 6520 746f 2064 6966 6665 7265 6e63  Due to differenc
-000043e0: 6573 2069 6e20 696d 706c 656d 656e 7461  es in implementa
-000043f0: 7469 6f6e 2028 666f 7220 7065 7266 6f72  tion (for perfor
-00004400: 6d61 6e63 6520 7265 6173 6f6e 7329 2c20  mance reasons), 
-00004410: 7468 650a 2020 2020 6178 6573 206f 6620  the.    axes of 
-00004420: 7468 6520 7265 7375 6c74 2061 7265 2074  the result are t
-00004430: 7261 6e73 706f 7365 6420 636f 6d70 6172  ransposed compar
-00004440: 6564 2074 6f20 7468 6520 636f 6e74 726f  ed to the contro
-00004450: 6c20 6d61 7472 6978 3a0a 0a20 2020 203e  l matrix:..    >
-00004460: 3e3e 2063 7472 6c6d 6174 203d 2063 616c  >> ctrlmat = cal
-00004470: 6375 6c61 7465 5f63 6f6e 7472 6f6c 5f6d  culate_control_m
-00004480: 6174 7269 785f 6672 6f6d 5f61 746f 6d69  atrix_from_atomi
-00004490: 6328 2e2e 2e29 0a20 2020 203e 3e3e 2063  c(...).    >>> c
-000044a0: 7472 6c6d 6174 2e73 6861 7065 0a20 2020  trlmat.shape.   
-000044b0: 2028 6e5f 6e6f 7073 2c20 642a 2a32 2c20   (n_nops, d**2, 
-000044c0: 6e5f 6f6d 6567 6129 0a20 2020 203e 3e3e  n_omega).    >>>
-000044d0: 206e 6f69 7365 6f70 7320 3d20 6361 6c63   noiseops = calc
-000044e0: 756c 6174 655f 6e6f 6973 655f 6f70 6572  ulate_noise_oper
-000044f0: 6174 6f72 735f 6672 6f6d 5f61 746f 6d69  ators_from_atomi
-00004500: 6328 2e2e 2e29 0a20 2020 203e 3e3e 206e  c(...).    >>> n
-00004510: 6f69 7365 6f70 732e 7368 6170 650a 2020  oiseops.shape.  
-00004520: 2020 286e 5f6f 6d65 6761 2c20 6e5f 6e6f    (n_omega, n_no
-00004530: 7073 2c20 642c 2064 290a 2020 2020 3e3e  ps, d, d).    >>
-00004540: 3e20 6374 726c 6d61 745f 6672 6f6d 5f6e  > ctrlmat_from_n
-00004550: 6f69 7365 6f70 7320 3d20 6666 2e62 6173  oiseops = ff.bas
-00004560: 6973 2e65 7870 616e 6428 6e6f 6973 656f  is.expand(noiseo
-00004570: 7073 2c20 6261 7369 7329 0a20 2020 203e  ps, basis).    >
-00004580: 3e3e 206e 702e 616c 6c63 6c6f 7365 2863  >> np.allclose(c
-00004590: 7472 6c6d 6174 2c20 6374 726c 6d61 745f  trlmat, ctrlmat_
-000045a0: 6672 6f6d 5f6e 6f69 7365 6f70 732e 7472  from_noiseops.tr
-000045b0: 616e 7370 6f73 6528 312c 2032 2c20 3029  anspose(1, 2, 0)
-000045c0: 290a 2020 2020 5472 7565 0a0a 2020 2020  ).    True..    
-000045d0: 5365 6520 416c 736f 0a20 2020 202d 2d2d  See Also.    ---
-000045e0: 2d2d 2d2d 2d0a 2020 2020 6361 6c63 756c  -----.    calcul
-000045f0: 6174 655f 6e6f 6973 655f 6f70 6572 6174  ate_noise_operat
-00004600: 6f72 735f 6672 6f6d 5f73 6372 6174 6368  ors_from_scratch
-00004610: 3a20 436f 6d70 7574 6520 7468 6520 6f70  : Compute the op
-00004620: 6572 6174 6f72 7320 6672 6f6d 2073 6372  erators from scr
-00004630: 6174 6368 2e0a 2020 2020 6361 6c63 756c  atch..    calcul
-00004640: 6174 655f 636f 6e74 726f 6c5f 6d61 7472  ate_control_matr
-00004650: 6978 5f66 726f 6d5f 6174 6f6d 6963 3a20  ix_from_atomic: 
-00004660: 5361 6d65 2063 616c 6375 6c61 7469 6f6e  Same calculation
-00004670: 2069 6e20 4c69 6f75 7669 6c6c 6520 7370   in Liouville sp
-00004680: 6163 652e 0a20 2020 2022 2222 0a20 2020  ace..    """.   
-00004690: 206e 203d 206c 656e 286e 6f69 7365 5f6f   n = len(noise_o
-000046a0: 7065 7261 746f 7273 5f61 746f 6d69 6329  perators_atomic)
-000046b0: 0a20 2020 2023 2041 6c6c 6f63 6174 6520  .    # Allocate 
-000046c0: 6d65 6d6f 7279 0a20 2020 206e 6f69 7365  memory.    noise
-000046d0: 5f6f 7065 7261 746f 7273 203d 206e 702e  _operators = np.
-000046e0: 7a65 726f 7328 6e6f 6973 655f 6f70 6572  zeros(noise_oper
-000046f0: 6174 6f72 735f 6174 6f6d 6963 2e73 6861  ators_atomic.sha
-00004700: 7065 5b31 3a5d 2c20 6474 7970 653d 636f  pe[1:], dtype=co
-00004710: 6d70 6c65 7829 0a0a 2020 2020 6578 7072  mplex)..    expr
-00004720: 203d 206f 652e 636f 6e74 7261 6374 5f65   = oe.contract_e
-00004730: 7870 7265 7373 696f 6e28 276a 692c 2e2e  xpression('ji,..
-00004740: 2e6a 6b2c 6b6c 2d3e 2e2e 2e69 6c27 2c0a  .jk,kl->...il',.
-00004750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004770: 2020 7072 6f70 6167 6174 6f72 732e 7368    propagators.sh
-00004780: 6170 655b 313a 5d2c 206e 6f69 7365 5f6f  ape[1:], noise_o
-00004790: 7065 7261 746f 7273 5f61 746f 6d69 632e  perators_atomic.
-000047a0: 7368 6170 655b 313a 5d2c 0a20 2020 2020  shape[1:],.     
-000047b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000047c0: 2020 2020 2020 2020 2020 2020 2070 726f               pro
-000047d0: 7061 6761 746f 7273 2e73 6861 7065 5b31  pagators.shape[1
-000047e0: 3a5d 2c20 6f70 7469 6d69 7a65 3d5b 2830  :], optimize=[(0
-000047f0: 2c20 3129 2c20 2830 2c20 3129 5d29 0a0a  , 1), (0, 1)])..
-00004800: 2020 2020 666f 7220 6720 696e 2075 7469      for g in uti
-00004810: 6c2e 7072 6f67 7265 7373 6261 725f 7261  l.progressbar_ra
-00004820: 6e67 6528 6e2c 2073 686f 775f 7072 6f67  nge(n, show_prog
-00004830: 7265 7373 6261 723d 7368 6f77 5f70 726f  ressbar=show_pro
-00004840: 6772 6573 7362 6172 2c0a 2020 2020 2020  gressbar,.      
-00004850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004860: 2020 2020 2020 2020 2020 2020 2020 6465                de
-00004870: 7363 3d27 4361 6c63 756c 6174 696e 6720  sc='Calculating 
-00004880: 6e6f 6973 6520 6f70 6572 6174 6f72 7327  noise operators'
-00004890: 293a 0a20 2020 2020 2020 206e 6f69 7365  ):.        noise
-000048a0: 5f6f 7065 7261 746f 7273 202b 3d20 6578  _operators += ex
-000048b0: 7072 2870 726f 7061 6761 746f 7273 5b67  pr(propagators[g
-000048c0: 5d2e 636f 6e6a 2829 2c0a 2020 2020 2020  ].conj(),.      
-000048d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000048e0: 2020 2020 2020 2020 2020 6e6f 6973 655f            noise_
-000048f0: 6f70 6572 6174 6f72 735f 6174 6f6d 6963  operators_atomic
-00004900: 5b67 5d2a 7068 6173 6573 5b67 2c20 3a2c  [g]*phases[g, :,
-00004910: 204e 6f6e 652c 204e 6f6e 652c 204e 6f6e   None, None, Non
-00004920: 655d 2c0a 2020 2020 2020 2020 2020 2020  e],.            
-00004930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004940: 2020 2020 7072 6f70 6167 6174 6f72 735b      propagators[
-00004950: 675d 290a 0a20 2020 2072 6574 7572 6e20  g])..    return 
-00004960: 6e6f 6973 655f 6f70 6572 6174 6f72 730a  noise_operators.
-00004970: 0a0a 6465 6620 6361 6c63 756c 6174 655f  ..def calculate_
-00004980: 6e6f 6973 655f 6f70 6572 6174 6f72 735f  noise_operators_
-00004990: 6672 6f6d 5f73 6372 6174 6368 280a 2020  from_scratch(.  
-000049a0: 2020 2020 2020 6569 6776 616c 733a 206e        eigvals: n
-000049b0: 6461 7272 6179 2c0a 2020 2020 2020 2020  darray,.        
-000049c0: 6569 6776 6563 733a 206e 6461 7272 6179  eigvecs: ndarray
-000049d0: 2c0a 2020 2020 2020 2020 7072 6f70 6167  ,.        propag
-000049e0: 6174 6f72 733a 206e 6461 7272 6179 2c0a  ators: ndarray,.
-000049f0: 2020 2020 2020 2020 6f6d 6567 613a 2043          omega: C
-00004a00: 6f65 6666 6963 6965 6e74 732c 0a20 2020  oefficients,.   
-00004a10: 2020 2020 206e 5f6f 7065 7273 3a20 5365       n_opers: Se
-00004a20: 7175 656e 6365 5b4f 7065 7261 746f 725d  quence[Operator]
-00004a30: 2c0a 2020 2020 2020 2020 6e5f 636f 6566  ,.        n_coef
-00004a40: 6673 3a20 5365 7175 656e 6365 5b43 6f65  fs: Sequence[Coe
-00004a50: 6666 6963 6965 6e74 735d 2c0a 2020 2020  fficients],.    
-00004a60: 2020 2020 6474 3a20 436f 6566 6669 6369      dt: Coeffici
-00004a70: 656e 7473 2c0a 2020 2020 2020 2020 743a  ents,.        t:
-00004a80: 204f 7074 696f 6e61 6c5b 436f 6566 6669   Optional[Coeffi
-00004a90: 6369 656e 7473 5d20 3d20 4e6f 6e65 2c0a  cients] = None,.
-00004aa0: 2020 2020 2020 2020 7368 6f77 5f70 726f          show_pro
-00004ab0: 6772 6573 7362 6172 3a20 626f 6f6c 203d  gressbar: bool =
-00004ac0: 2046 616c 7365 2c0a 2020 2020 2020 2020   False,.        
-00004ad0: 6361 6368 655f 696e 7465 726d 6564 6961  cache_intermedia
-00004ae0: 7465 733a 2062 6f6f 6c20 3d20 4661 6c73  tes: bool = Fals
-00004af0: 650a 2920 2d3e 2055 6e69 6f6e 5b6e 6461  e.) -> Union[nda
-00004b00: 7272 6179 2c20 5475 706c 655b 6e64 6172  rray, Tuple[ndar
-00004b10: 7261 792c 2044 6963 745b 7374 722c 206e  ray, Dict[str, n
-00004b20: 6461 7272 6179 5d5d 5d3a 0a20 2020 2072  darray]]]:.    r
-00004b30: 2222 220a 2020 2020 4361 6c63 756c 6174  """.    Calculat
-00004b40: 6520 7468 6520 6e6f 6973 6520 6f70 6572  e the noise oper
-00004b50: 6174 6f72 7320 696e 2069 6e74 6572 6163  ators in interac
-00004b60: 7469 6f6e 2070 6963 7475 7265 2066 726f  tion picture fro
-00004b70: 6d20 7363 7261 7463 682e 0a0a 2020 2020  m scratch...    
-00004b80: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
-00004b90: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6569  ---------.    ei
-00004ba0: 6776 616c 733a 2061 7272 6179 5f6c 696b  gvals: array_lik
-00004bb0: 652c 2073 6861 7065 2028 6e5f 6474 2c20  e, shape (n_dt, 
-00004bc0: 6429 0a20 2020 2020 2020 2045 6967 656e  d).        Eigen
-00004bd0: 7661 6c75 6520 7665 6374 6f72 7320 666f  value vectors fo
-00004be0: 7220 6561 6368 2074 696d 6520 7075 6c73  r each time puls
-00004bf0: 6520 7365 676d 656e 7420 2a67 2a20 7769  e segment *g* wi
-00004c00: 7468 2074 6865 0a20 2020 2020 2020 2066  th the.        f
-00004c10: 6972 7374 2061 7869 7320 636f 756e 7469  irst axis counti
-00004c20: 6e67 2074 6865 2070 756c 7365 2073 6567  ng the pulse seg
-00004c30: 6d65 6e74 2c20 692e 652e 0a20 2020 2020  ment, i.e..     
-00004c40: 2020 2060 6065 6967 7661 6c73 203d 3d20     ``eigvals == 
-00004c50: 6172 7261 7928 5b44 5f30 2c20 445f 312c  array([D_0, D_1,
-00004c60: 202e 2e2e 5d29 6060 2e0a 2020 2020 6569   ...])``..    ei
-00004c70: 6776 6563 733a 2061 7272 6179 5f6c 696b  gvecs: array_lik
-00004c80: 652c 2073 6861 7065 2028 6e5f 6474 2c20  e, shape (n_dt, 
-00004c90: 642c 2064 290a 2020 2020 2020 2020 4569  d, d).        Ei
-00004ca0: 6765 6e76 6563 746f 7220 6d61 7472 6963  genvector matric
-00004cb0: 6573 2066 6f72 2065 6163 6820 7469 6d65  es for each time
-00004cc0: 2070 756c 7365 2073 6567 6d65 6e74 202a   pulse segment *
-00004cd0: 672a 2077 6974 6820 7468 650a 2020 2020  g* with the.    
-00004ce0: 2020 2020 6669 7273 7420 6178 6973 2063      first axis c
-00004cf0: 6f75 6e74 696e 6720 7468 6520 7075 6c73  ounting the puls
-00004d00: 6520 7365 676d 656e 742c 2069 2e65 2e0a  e segment, i.e..
-00004d10: 2020 2020 2020 2020 6060 6569 6776 6563          ``eigvec
-00004d20: 7320 3d3d 2061 7272 6179 285b 565f 302c  s == array([V_0,
-00004d30: 2056 5f31 2c20 2e2e 2e5d 2960 602e 0a20   V_1, ...])``.. 
-00004d40: 2020 2070 726f 7061 6761 746f 7273 3a20     propagators: 
-00004d50: 6172 7261 795f 6c69 6b65 2c20 7368 6170  array_like, shap
-00004d60: 6520 286e 5f64 742b 312c 2064 2c20 6429  e (n_dt+1, d, d)
-00004d70: 0a20 2020 2020 2020 2054 6865 2070 726f  .        The pro
-00004d80: 7061 6761 746f 7273 203a 6d61 7468 3a60  pagators :math:`
-00004d90: 515f 6720 3d20 505f 6720 505f 7b67 2d31  Q_g = P_g P_{g-1
-00004da0: 7d5c 6364 6f74 7320 505f 3060 2061 7320  }\cdots P_0` as 
-00004db0: 6120 2864 2c20 6429 0a20 2020 2020 2020  a (d, d).       
-00004dc0: 2061 7272 6179 2077 6974 6820 2a64 2a20   array with *d* 
-00004dd0: 7468 6520 6469 6d65 6e73 696f 6e20 6f66  the dimension of
-00004de0: 2074 6865 2048 696c 6265 7274 2073 7061   the Hilbert spa
-00004df0: 6365 2e0a 2020 2020 6f6d 6567 613a 2061  ce..    omega: a
-00004e00: 7272 6179 5f6c 696b 652c 2073 6861 7065  rray_like, shape
-00004e10: 2028 6e5f 6f6d 6567 612c 290a 2020 2020   (n_omega,).    
-00004e20: 2020 2020 4672 6571 7565 6e63 6965 7320      Frequencies 
-00004e30: 6174 2077 6869 6368 2074 6865 2070 756c  at which the pul
-00004e40: 7365 2063 6f6e 7472 6f6c 206d 6174 7269  se control matri
-00004e50: 7820 6973 2074 6f20 6265 0a20 2020 2020  x is to be.     
-00004e60: 2020 2065 7661 6c75 6174 6564 2e0a 2020     evaluated..  
-00004e70: 2020 6e5f 6f70 6572 733a 2061 7272 6179    n_opers: array
-00004e80: 5f6c 696b 652c 2073 6861 7065 2028 6e5f  _like, shape (n_
-00004e90: 6e6f 7073 2c20 642c 2064 290a 2020 2020  nops, d, d).    
-00004ea0: 2020 2020 4e6f 6973 6520 6f70 6572 6174      Noise operat
-00004eb0: 6f72 7320 3a6d 6174 683a 6042 5f5c 616c  ors :math:`B_\al
-00004ec0: 7068 6160 2e0a 2020 2020 6e5f 636f 6566  pha`..    n_coef
-00004ed0: 6673 3a20 6172 7261 795f 6c69 6b65 2c20  fs: array_like, 
-00004ee0: 7368 6170 6520 286e 5f6e 6f70 732c 206e  shape (n_nops, n
-00004ef0: 5f64 7429 0a20 2020 2020 2020 2054 6865  _dt).        The
-00004f00: 2073 656e 7369 7469 7669 7469 6573 206f   sensitivities o
-00004f10: 6620 7468 6520 7379 7374 656d 2074 6f20  f the system to 
-00004f20: 7468 6520 6e6f 6973 6520 6f70 6572 6174  the noise operat
-00004f30: 6f72 7320 6769 7665 6e20 6279 0a20 2020  ors given by.   
-00004f40: 2020 2020 202a 6e5f 6f70 6572 732a 2061       *n_opers* a
-00004f50: 7420 7468 6520 6769 7665 6e20 7469 6d65  t the given time
-00004f60: 2073 7465 702e 0a20 2020 2064 743a 2061   step..    dt: a
-00004f70: 7272 6179 5f6c 696b 652c 2073 6861 7065  rray_like, shape
-00004f80: 2028 6e5f 6474 290a 2020 2020 2020 2020   (n_dt).        
-00004f90: 5365 7175 656e 6365 2064 7572 6174 696f  Sequence duratio
-00004fa0: 6e2c 2069 2e65 2e20 666f 7220 7468 6520  n, i.e. for the 
-00004fb0: 3a6d 6174 683a 6067 602d 7468 2070 756c  :math:`g`-th pul
-00004fc0: 7365 0a20 2020 2020 2020 203a 6d61 7468  se.        :math
-00004fd0: 3a60 745f 6720 2d20 745f 7b67 2d31 7d60  :`t_g - t_{g-1}`
-00004fe0: 2e0a 2020 2020 743a 2061 7272 6179 5f6c  ..    t: array_l
-00004ff0: 696b 652c 2073 6861 7065 2028 6e5f 6474  ike, shape (n_dt
-00005000: 2b31 292c 206f 7074 696f 6e61 6c0a 2020  +1), optional.  
-00005010: 2020 2020 2020 5468 6520 6162 736f 6c75        The absolu
-00005020: 7465 2074 696d 6573 206f 6620 7468 6520  te times of the 
-00005030: 6469 6666 6572 656e 7420 7365 676d 656e  different segmen
-00005040: 7473 2e20 4361 6e20 616c 736f 2062 650a  ts. Can also be.
-00005050: 2020 2020 2020 2020 636f 6d70 7574 6564          computed
-00005060: 2066 726f 6d20 2a64 742a 2e0a 2020 2020   from *dt*..    
-00005070: 7368 6f77 5f70 726f 6772 6573 7362 6172  show_progressbar
-00005080: 3a20 626f 6f6c 2c20 6f70 7469 6f6e 616c  : bool, optional
-00005090: 0a20 2020 2020 2020 2053 686f 7720 6120  .        Show a 
-000050a0: 7072 6f67 7265 7373 2062 6172 2066 6f72  progress bar for
-000050b0: 2074 6865 2063 616c 6375 6c61 7469 6f6e   the calculation
-000050c0: 2e0a 2020 2020 6361 6368 655f 696e 7465  ..    cache_inte
-000050d0: 726d 6564 6961 7465 733a 2062 6f6f 6c2c  rmediates: bool,
-000050e0: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
-000050f0: 2020 4b65 6570 2061 6e64 2072 6574 7572    Keep and retur
-00005100: 6e20 696e 7465 726d 6564 6961 7465 2074  n intermediate t
-00005110: 6572 6d73 206f 6620 7468 6520 6361 6c63  erms of the calc
-00005120: 756c 6174 696f 6e20 7468 6174 2063 616e  ulation that can
-00005130: 0a20 2020 2020 2020 2062 6520 7265 7573  .        be reus
-00005140: 6564 2069 6e20 6f74 6865 7220 636f 6d70  ed in other comp
-00005150: 7574 6174 696f 6e73 2028 7365 636f 6e64  utations (second
-00005160: 206f 7264 6572 206f 7220 6772 6164 6965   order or gradie
-00005170: 6e74 7329 2e0a 2020 2020 2020 2020 4f74  nts)..        Ot
-00005180: 6865 7277 6973 6520 7468 6520 7375 6d20  herwise the sum 
-00005190: 6973 2070 6572 666f 726d 6564 2069 6e2d  is performed in-
-000051a0: 706c 6163 652e 2054 6865 2064 6566 6175  place. The defau
-000051b0: 6c74 2069 7320 4661 6c73 652e 0a0a 2020  lt is False...  
-000051c0: 2020 5265 7475 726e 730a 2020 2020 2d2d    Returns.    --
-000051d0: 2d2d 2d2d 2d0a 2020 2020 6e6f 6973 655f  -----.    noise_
-000051e0: 6f70 6572 6174 6f72 733a 206e 6461 7272  operators: ndarr
-000051f0: 6179 2c20 7368 6170 6520 286e 5f6f 6d65  ay, shape (n_ome
-00005200: 6761 2c20 6e5f 6e6f 7073 2c20 642c 2064  ga, n_nops, d, d
-00005210: 290a 2020 2020 2020 2020 5468 6520 696e  ).        The in
-00005220: 7465 7261 6374 696f 6e20 7069 6374 7572  teraction pictur
-00005230: 6520 6e6f 6973 6520 6f70 6572 6174 6f72  e noise operator
-00005240: 730a 2020 2020 2020 2020 3a6d 6174 683a  s.        :math:
-00005250: 605c 7469 6c64 657b 427d 5f5c 616c 7068  `\tilde{B}_\alph
-00005260: 6128 5c6f 6d65 6761 2960 2e0a 2020 2020  a(\omega)`..    
-00005270: 696e 7465 726d 6564 6961 7465 733a 2064  intermediates: d
-00005280: 6963 745b 7374 722c 206e 6461 7272 6179  ict[str, ndarray
-00005290: 5d0a 2020 2020 2020 2020 496e 7465 726d  ].        Interm
-000052a0: 6564 6961 7465 2072 6573 756c 7473 206f  ediate results o
-000052b0: 6620 7468 6520 6361 6c63 756c 6174 696f  f the calculatio
-000052c0: 6e2e 204f 6e6c 7920 6966 0a20 2020 2020  n. Only if.     
-000052d0: 2020 2063 6163 6865 5f69 6e74 6572 6d65     cache_interme
-000052e0: 6469 6174 6573 2069 7320 5472 7565 2e0a  diates is True..
-000052f0: 0a20 2020 204e 6f74 6573 0a20 2020 202d  .    Notes.    -
-00005300: 2d2d 2d2d 0a20 2020 2054 6865 2069 6e74  ----.    The int
-00005310: 6572 6163 7469 6f6e 2070 6963 7475 7265  eraction picture
-00005320: 206e 6f69 7365 206f 7065 7261 746f 7273   noise operators
-00005330: 2061 7265 2063 616c 6375 6c61 7465 6420   are calculated 
-00005340: 6163 636f 7264 696e 6720 746f 0a0a 2020  according to..  
-00005350: 2020 2e2e 206d 6174 683a 3a0a 0a20 2020    .. math::..   
-00005360: 2020 2020 205c 7469 6c64 657b 427d 5f5c       \tilde{B}_\
-00005370: 616c 7068 6128 5c6f 6d65 6761 2920 3d20  alpha(\omega) = 
-00005380: 5c73 756d 5f7b 673d 317d 5e47 2065 5e7b  \sum_{g=1}^G e^{
-00005390: 695c 6f6d 6567 6120 745f 7b67 2d31 7d7d  i\omega t_{g-1}}
-000053a0: 0a20 2020 2020 2020 2020 2020 2073 5f5c  .            s_\
-000053b0: 616c 7068 615e 7b28 6729 7d20 505e 7b28  alpha^{(g)} P^{(
-000053c0: 6729 5c64 6167 6765 727d 5c6c 6566 745b  g)\dagger}\left[
-000053d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000053e0: 205c 6261 727b 427d 5e7b 2867 297d 5f5c   \bar{B}^{(g)}_\
-000053f0: 616c 7068 6120 5c63 6972 6320 495e 7b28  alpha \circ I^{(
-00005400: 6729 7d28 5c6f 6d65 6761 290a 2020 2020  g)}(\omega).    
-00005410: 2020 2020 2020 2020 5c72 6967 6874 5d20          \right] 
-00005420: 505e 7b28 6729 7d0a 0a20 2020 2077 6865  P^{(g)}..    whe
-00005430: 7265 0a0a 2020 2020 2e2e 206d 6174 683a  re..    .. math:
-00005440: 3a0a 0a20 2020 2020 2020 2049 5e7b 2867  :..        I^{(g
-00005450: 297d 5f7b 6e6d 7d28 5c6f 6d65 6761 2920  )}_{nm}(\omega) 
-00005460: 263d 205c 696e 745f 305e 7b74 5f67 202d  &= \int_0^{t_g -
-00005470: 2074 5f7b 672d 317d 7d5c 6d61 7468 726d   t_{g-1}}\mathrm
-00005480: 7b64 7d74 5c2c 0a20 2020 2020 2020 2020  {d}t\,.         
-00005490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000054a0: 2020 2020 2020 2065 5e7b 6928 5c6f 6d65         e^{i(\ome
-000054b0: 6761 2b5c 6f6d 6567 615f 6e2d 5c6f 6d65  ga+\omega_n-\ome
-000054c0: 6761 5f6d 2974 7d20 5c5c 0a20 2020 2020  ga_m)t} \\.     
-000054d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000054e0: 2020 2020 2020 2020 263d 205c 6672 6163          &= \frac
-000054f0: 7b65 5e7b 6928 5c6f 6d65 6761 2b5c 6f6d  {e^{i(\omega+\om
-00005500: 6567 615f 6e2d 5c6f 6d65 6761 5f6d 290a  ega_n-\omega_m).
-00005510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005530: 2874 5f67 202d 2074 5f7b 672d 317d 297d  (t_g - t_{g-1})}
-00005540: 202d 2031 7d0a 2020 2020 2020 2020 2020   - 1}.          
-00005550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005560: 2020 2020 2020 7b69 285c 6f6d 6567 612b        {i(\omega+
-00005570: 5c6f 6d65 6761 5f6e 2d5c 6f6d 6567 615f  \omega_n-\omega_
-00005580: 6d29 7d2c 205c 5c0a 2020 2020 2020 2020  m)}, \\.        
-00005590: 5c62 6172 7b42 7d5f 5c61 6c70 6861 5e7b  \bar{B}_\alpha^{
-000055a0: 2867 297d 2026 3d20 565e 7b28 6729 5c64  (g)} &= V^{(g)\d
-000055b0: 6167 6765 727d 2042 5f5c 616c 7068 6120  agger} B_\alpha 
-000055c0: 565e 7b28 6729 7d2c 205c 5c0a 2020 2020  V^{(g)}, \\.    
-000055d0: 2020 2020 505e 7b28 6729 7d20 263d 2056      P^{(g)} &= V
-000055e0: 5e7b 2867 295c 6461 6767 6572 7d20 515f  ^{(g)\dagger} Q_
-000055f0: 7b67 2d31 7d2c 0a0a 2020 2020 616e 6420  {g-1},..    and 
-00005600: 3a6d 6174 683a 6056 5e7b 2867 297d 6020  :math:`V^{(g)}` 
-00005610: 6973 2074 6865 206d 6174 7269 7820 6f66  is the matrix of
-00005620: 2065 6967 656e 7665 6374 6f72 7320 7468   eigenvectors th
-00005630: 6174 2064 6961 676f 6e61 6c69 7a65 730a  at diagonalizes.
-00005640: 2020 2020 3a6d 6174 683a 605c 7469 6c64      :math:`\tild
-00005650: 657b 5c6d 6174 6863 616c 7b48 7d7d 5f6e  e{\mathcal{H}}_n
-00005660: 5e7b 2867 297d 602c 203a 6d61 7468 3a60  ^{(g)}`, :math:`
-00005670: 425f 5c61 6c70 6861 6020 7468 650a 2020  B_\alpha` the.  
-00005680: 2020 3a6d 6174 683a 605c 616c 7068 6160    :math:`\alpha`
-00005690: 2d74 6820 6e6f 6973 6520 6f70 6572 6174  -th noise operat
-000056a0: 6f72 2c20 616e 6420 203a 6d61 7468 3a60  or, and  :math:`
-000056b0: 735f 5c61 6c70 6861 5e7b 2867 297d 6020  s_\alpha^{(g)}` 
-000056c0: 7468 650a 2020 2020 6e6f 6973 6520 7365  the.    noise se
-000056d0: 6e73 6974 6976 6974 7920 6475 7269 6e67  nsitivity during
-000056e0: 2069 6e74 6572 7661 6c20 3a6d 6174 683a   interval :math:
-000056f0: 6067 602e 0a0a 2020 2020 5468 6520 636f  `g`...    The co
-00005700: 6e74 726f 6c20 6d61 7472 6978 2074 6865  ntrol matrix the
-00005710: 6e20 636f 7272 6573 706f 6e64 7320 746f  n corresponds to
-00005720: 2074 6865 2063 6f65 6666 6963 6965 6e74   the coefficient
-00005730: 7320 6f66 2065 7870 616e 7369 6f6e 0a20  s of expansion. 
-00005740: 2020 2069 6e20 616e 206f 7065 7261 746f     in an operato
-00005750: 7220 6261 7369 7320 3a6d 6174 683a 605c  r basis :math:`\
-00005760: 7b43 5f6b 5c7d 5f6b 603a 0a0a 2020 2020  {C_k\}_k`:..    
-00005770: 2e2e 206d 6174 683a 3a0a 2020 2020 2020  .. math::.      
-00005780: 2020 5c74 696c 6465 7b5c 6d61 7468 6361    \tilde{\mathca
-00005790: 6c7b 427d 7d5f 7b6b 5c61 6c70 6861 7d28  l{B}}_{k\alpha}(
-000057a0: 5c6f 6d65 6761 2920 3d0a 2020 2020 2020  \omega) =.      
-000057b0: 2020 2020 2020 5c6d 6174 6872 6d7b 7472        \mathrm{tr
-000057c0: 7d28 5c74 696c 6465 7b42 7d5f 5c61 6c70  }(\tilde{B}_\alp
-000057d0: 6861 285c 6f6d 6567 6129 2043 5f6b 292e  ha(\omega) C_k).
-000057e0: 0a0a 2020 2020 4475 6520 746f 2064 6966  ..    Due to dif
-000057f0: 6665 7265 6e63 6573 2069 6e20 696d 706c  ferences in impl
-00005800: 656d 656e 7461 7469 6f6e 2028 666f 7220  ementation (for 
-00005810: 7065 7266 6f72 6d61 6e63 6520 7265 6173  performance reas
-00005820: 6f6e 7329 2c20 7468 650a 2020 2020 6178  ons), the.    ax
-00005830: 6573 206f 6620 7468 6520 7265 7375 6c74  es of the result
-00005840: 2061 7265 2074 7261 6e73 706f 7365 6420   are transposed 
-00005850: 636f 6d70 6172 6564 2074 6f20 7468 6520  compared to the 
-00005860: 636f 6e74 726f 6c20 6d61 7472 6978 3a0a  control matrix:.
-00005870: 0a20 2020 203e 3e3e 2063 7472 6c6d 6174  .    >>> ctrlmat
-00005880: 203d 2063 616c 6375 6c61 7465 5f63 6f6e   = calculate_con
-00005890: 7472 6f6c 5f6d 6174 7269 785f 6672 6f6d  trol_matrix_from
-000058a0: 5f73 6372 6174 6368 282e 2e2e 290a 2020  _scratch(...).  
-000058b0: 2020 3e3e 3e20 6374 726c 6d61 742e 7368    >>> ctrlmat.sh
-000058c0: 6170 650a 2020 2020 286e 5f6e 6f70 732c  ape.    (n_nops,
-000058d0: 2064 2a2a 322c 206e 5f6f 6d65 6761 290a   d**2, n_omega).
-000058e0: 2020 2020 3e3e 3e20 6e6f 6973 656f 7073      >>> noiseops
-000058f0: 203d 2063 616c 6375 6c61 7465 5f6e 6f69   = calculate_noi
-00005900: 7365 5f6f 7065 7261 746f 7273 5f66 726f  se_operators_fro
-00005910: 6d5f 7363 7261 7463 6828 2e2e 2e29 0a20  m_scratch(...). 
-00005920: 2020 203e 3e3e 206e 6f69 7365 6f70 732e     >>> noiseops.
-00005930: 7368 6170 650a 2020 2020 286e 5f6f 6d65  shape.    (n_ome
-00005940: 6761 2c20 6e5f 6e6f 7073 2c20 642c 2064  ga, n_nops, d, d
-00005950: 290a 2020 2020 3e3e 3e20 6374 726c 6d61  ).    >>> ctrlma
-00005960: 745f 6672 6f6d 5f6e 6f69 7365 6f70 7320  t_from_noiseops 
-00005970: 3d20 6666 2e62 6173 6973 2e65 7870 616e  = ff.basis.expan
-00005980: 6428 6e6f 6973 656f 7073 2c20 6261 7369  d(noiseops, basi
-00005990: 7329 0a20 2020 203e 3e3e 206e 702e 616c  s).    >>> np.al
-000059a0: 6c63 6c6f 7365 2863 7472 6c6d 6174 2c20  lclose(ctrlmat, 
-000059b0: 6374 726c 6d61 745f 6672 6f6d 5f6e 6f69  ctrlmat_from_noi
-000059c0: 7365 6f70 732e 7472 616e 7370 6f73 6528  seops.transpose(
-000059d0: 312c 2032 2c20 3029 290a 2020 2020 5472  1, 2, 0)).    Tr
-000059e0: 7565 0a0a 2020 2020 5365 6520 416c 736f  ue..    See Also
-000059f0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d0a 2020  .    --------.  
-00005a00: 2020 6361 6c63 756c 6174 655f 6e6f 6973    calculate_nois
-00005a10: 655f 6f70 6572 6174 6f72 735f 6672 6f6d  e_operators_from
-00005a20: 5f61 746f 6d69 633a 2043 6f6d 7075 7465  _atomic: Compute
-00005a30: 2074 6865 206f 7065 7261 746f 7273 2066   the operators f
-00005a40: 726f 6d20 6174 6f6d 6963 2073 6567 6d65  rom atomic segme
-00005a50: 6e74 732e 0a20 2020 2063 616c 6375 6c61  nts..    calcula
-00005a60: 7465 5f63 6f6e 7472 6f6c 5f6d 6174 7269  te_control_matri
-00005a70: 785f 6672 6f6d 5f73 6372 6174 6368 3a20  x_from_scratch: 
-00005a80: 5361 6d65 2063 616c 6375 6c61 7469 6f6e  Same calculation
-00005a90: 2069 6e20 4c69 6f75 7669 6c6c 6520 7370   in Liouville sp
-00005aa0: 6163 652e 0a20 2020 2022 2222 0a20 2020  ace..    """.   
-00005ab0: 2069 6620 7420 6973 204e 6f6e 653a 0a20   if t is None:. 
-00005ac0: 2020 2020 2020 2074 203d 206e 702e 636f         t = np.co
-00005ad0: 6e63 6174 656e 6174 6528 285b 305d 2c20  ncatenate(([0], 
-00005ae0: 6e70 2e61 7361 7272 6179 2864 7429 2e63  np.asarray(dt).c
-00005af0: 756d 7375 6d28 2929 290a 0a20 2020 2064  umsum()))..    d
-00005b00: 203d 2065 6967 7665 6373 2e73 6861 7065   = eigvecs.shape
-00005b10: 5b2d 315d 0a20 2020 206e 5f63 6f65 6666  [-1].    n_coeff
-00005b20: 7320 3d20 6e70 2e61 7361 7272 6179 286e  s = np.asarray(n
-00005b30: 5f63 6f65 6666 7329 0a0a 2020 2020 2320  _coeffs)..    # 
-00005b40: 5072 6563 6f6d 7075 7465 206e 6f69 7365  Precompute noise
-00005b50: 206f 7065 7273 2074 7261 6e73 666f 726d   opers transform
-00005b60: 6564 2074 6f20 6569 6765 6e62 6173 6973  ed to eigenbasis
-00005b70: 206f 6620 6561 6368 2070 756c 7365 0a20   of each pulse. 
-00005b80: 2020 2023 2073 6567 6d65 6e74 2061 6e64     # segment and
-00005b90: 2056 5e5c 6461 6767 6572 2040 2051 0a20   V^\dagger @ Q. 
-00005ba0: 2020 2065 6967 7665 6373 5f70 726f 7061     eigvecs_propa
-00005bb0: 6761 7465 6420 3d20 5f70 726f 7061 6761  gated = _propaga
-00005bc0: 7465 5f65 6967 656e 7665 6374 6f72 7328  te_eigenvectors(
-00005bd0: 6569 6776 6563 732c 2070 726f 7061 6761  eigvecs, propaga
-00005be0: 746f 7273 5b3a 2d31 5d29 0a20 2020 206e  tors[:-1]).    n
-00005bf0: 5f6f 7065 7273 5f74 7261 6e73 666f 726d  _opers_transform
-00005c00: 6564 203d 205f 7472 616e 7366 6f72 6d5f  ed = _transform_
-00005c10: 6861 6d69 6c74 6f6e 6961 6e28 6569 6776  hamiltonian(eigv
-00005c20: 6563 732c 206e 5f6f 7065 7273 2c20 6e5f  ecs, n_opers, n_
-00005c30: 636f 6566 6673 290a 0a20 2020 2023 2041  coeffs)..    # A
-00005c40: 6c6c 6f63 6174 6520 6d65 6d6f 7279 0a20  llocate memory. 
-00005c50: 2020 2065 7870 5f62 7566 2c20 696e 745f     exp_buf, int_
-00005c60: 6275 6620 3d20 6e70 2e65 6d70 7479 2828  buf = np.empty((
-00005c70: 322c 206c 656e 286f 6d65 6761 292c 2064  2, len(omega), d
-00005c80: 2c20 6429 2c20 6474 7970 653d 636f 6d70  , d), dtype=comp
-00005c90: 6c65 7829 0a20 2020 206e 6f69 7365 5f6f  lex).    noise_o
-00005ca0: 7065 7261 746f 7273 203d 206e 702e 7a65  perators = np.ze
-00005cb0: 726f 7328 286c 656e 286f 6d65 6761 292c  ros((len(omega),
-00005cc0: 206c 656e 286e 5f6f 7065 7273 292c 2064   len(n_opers), d
-00005cd0: 2c20 6429 2c20 6474 7970 653d 636f 6d70  , d), dtype=comp
-00005ce0: 6c65 7829 0a0a 2020 2020 6966 2063 6163  lex)..    if cac
-00005cf0: 6865 5f69 6e74 6572 6d65 6469 6174 6573  he_intermediates
-00005d00: 3a0a 2020 2020 2020 2020 7375 6d5f 6361  :.        sum_ca
-00005d10: 6368 6520 3d20 6e70 2e65 6d70 7479 2828  che = np.empty((
-00005d20: 6c65 6e28 6474 292c 206c 656e 286f 6d65  len(dt), len(ome
-00005d30: 6761 292c 206c 656e 286e 5f6f 7065 7273  ga), len(n_opers
-00005d40: 292c 2064 2c20 6429 2c20 6474 7970 653d  ), d, d), dtype=
-00005d50: 636f 6d70 6c65 7829 0a20 2020 2065 6c73  complex).    els
-00005d60: 653a 0a20 2020 2020 2020 2073 756d 5f62  e:.        sum_b
-00005d70: 7566 203d 206e 702e 656d 7074 7928 286c  uf = np.empty((l
-00005d80: 656e 286f 6d65 6761 292c 206c 656e 286e  en(omega), len(n
-00005d90: 5f6f 7065 7273 292c 2064 2c20 6429 2c20  _opers), d, d), 
-00005da0: 6474 7970 653d 636f 6d70 6c65 7829 0a0a  dtype=complex)..
-00005db0: 2020 2020 2320 5365 7420 7570 2072 6575      # Set up reu
-00005dc0: 7361 626c 6520 6578 7072 6573 7369 6f6e  sable expression
-00005dd0: 730a 2020 2020 6578 7072 5f31 203d 206f  s.    expr_1 = o
-00005de0: 652e 636f 6e74 7261 6374 5f65 7870 7265  e.contract_expre
-00005df0: 7373 696f 6e28 2761 6b6c 2c6f 6b6c 2d3e  ssion('akl,okl->
-00005e00: 6f61 6b6c 272c 0a20 2020 2020 2020 2020  oakl',.         
-00005e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e20: 2020 2020 2020 2020 2020 206e 5f6f 7065             n_ope
-00005e30: 7273 5f74 7261 6e73 666f 726d 6564 5b3a  rs_transformed[:
-00005e40: 2c20 305d 2e73 6861 7065 2c20 696e 745f  , 0].shape, int_
-00005e50: 6275 662e 7368 6170 6529 0a20 2020 2065  buf.shape).    e
-00005e60: 7870 725f 3220 3d20 6f65 2e63 6f6e 7472  xpr_2 = oe.contr
-00005e70: 6163 745f 6578 7072 6573 7369 6f6e 2827  act_expression('
-00005e80: 6a69 2c2e 2e2e 6a6b 2c6b 6c27 2c0a 2020  ji,...jk,kl',.  
-00005e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005eb0: 2020 6569 6776 6563 735f 7072 6f70 6167    eigvecs_propag
-00005ec0: 6174 6564 5b30 5d2e 7368 6170 652c 2028  ated[0].shape, (
-00005ed0: 6c65 6e28 6f6d 6567 6129 2c20 6c65 6e28  len(omega), len(
-00005ee0: 6e5f 6f70 6572 7329 2c20 642c 2064 292c  n_opers), d, d),
-00005ef0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f10: 2020 2020 2065 6967 7665 6373 5f70 726f       eigvecs_pro
-00005f20: 7061 6761 7465 645b 305d 2e73 6861 7065  pagated[0].shape
-00005f30: 2c20 6f70 7469 6d69 7a65 3d5b 2830 2c20  , optimize=[(0, 
-00005f40: 3129 2c20 2830 2c20 3129 5d29 0a0a 2020  1), (0, 1)])..  
-00005f50: 2020 666f 7220 6720 696e 2075 7469 6c2e    for g in util.
-00005f60: 7072 6f67 7265 7373 6261 725f 7261 6e67  progressbar_rang
-00005f70: 6528 6c65 6e28 6474 292c 2073 686f 775f  e(len(dt), show_
-00005f80: 7072 6f67 7265 7373 6261 723d 7368 6f77  progressbar=show
-00005f90: 5f70 726f 6772 6573 7362 6172 2c0a 2020  _progressbar,.  
-00005fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005fc0: 2020 6465 7363 3d27 4361 6c63 756c 6174    desc='Calculat
-00005fd0: 696e 6720 6e6f 6973 6520 6f70 6572 6174  ing noise operat
-00005fe0: 6f72 7327 293a 0a20 2020 2020 2020 2069  ors'):.        i
-00005ff0: 6620 6361 6368 655f 696e 7465 726d 6564  f cache_intermed
-00006000: 6961 7465 733a 0a20 2020 2020 2020 2020  iates:.         
-00006010: 2020 2023 2041 7373 6967 6e20 7265 6665     # Assign refe
-00006020: 7265 6e63 6573 2074 6f20 7468 6520 6c6f  rences to the lo
-00006030: 6361 7469 6f6e 7320 696e 2074 6865 2063  cations in the c
-00006040: 6163 6865 2066 6f72 2074 6865 2071 7561  ache for the qua
-00006050: 6e74 6974 6965 730a 2020 2020 2020 2020  ntities.        
-00006060: 2020 2020 2320 7468 6174 2073 686f 756c      # that shoul
-00006070: 6420 6265 2073 746f 7265 640a 2020 2020  d be stored.    
-00006080: 2020 2020 2020 2020 7375 6d5f 6275 6620          sum_buf 
-00006090: 3d20 7375 6d5f 6361 6368 655b 675d 0a0a  = sum_cache[g]..
-000060a0: 2020 2020 2020 2020 696e 745f 6275 6620          int_buf 
-000060b0: 3d20 5f66 6972 7374 5f6f 7264 6572 5f69  = _first_order_i
-000060c0: 6e74 6567 7261 6c28 6f6d 6567 612c 2065  ntegral(omega, e
-000060d0: 6967 7661 6c73 5b67 5d2c 2064 745b 675d  igvals[g], dt[g]
-000060e0: 2c20 6578 705f 6275 662c 2069 6e74 5f62  , exp_buf, int_b
-000060f0: 7566 290a 2020 2020 2020 2020 7375 6d5f  uf).        sum_
-00006100: 6275 6620 3d20 6578 7072 5f31 286e 5f6f  buf = expr_1(n_o
-00006110: 7065 7273 5f74 7261 6e73 666f 726d 6564  pers_transformed
-00006120: 5b3a 2c20 675d 2c20 7574 696c 2e63 6578  [:, g], util.cex
-00006130: 7028 6f6d 6567 612a 745b 675d 295b 3a2c  p(omega*t[g])[:,
-00006140: 204e 6f6e 652c 204e 6f6e 655d 2a69 6e74   None, None]*int
-00006150: 5f62 7566 2c0a 2020 2020 2020 2020 2020  _buf,.          
-00006160: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-00006170: 7574 3d73 756d 5f62 7566 290a 0a20 2020  ut=sum_buf)..   
-00006180: 2020 2020 206e 6f69 7365 5f6f 7065 7261       noise_opera
-00006190: 746f 7273 202b 3d20 6578 7072 5f32 2865  tors += expr_2(e
-000061a0: 6967 7665 6373 5f70 726f 7061 6761 7465  igvecs_propagate
-000061b0: 645b 675d 2e63 6f6e 6a28 292c 2073 756d  d[g].conj(), sum
-000061c0: 5f62 7566 2c20 6569 6776 6563 735f 7072  _buf, eigvecs_pr
-000061d0: 6f70 6167 6174 6564 5b67 5d2c 0a20 2020  opagated[g],.   
-000061e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000061f0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-00006200: 7574 3d73 756d 5f62 7566 290a 0a20 2020  ut=sum_buf)..   
-00006210: 2069 6620 6361 6368 655f 696e 7465 726d   if cache_interm
-00006220: 6564 6961 7465 733a 0a20 2020 2020 2020  ediates:.       
-00006230: 2069 6e74 6572 6d65 6469 6174 6573 203d   intermediates =
-00006240: 2064 6963 7428 6e5f 6f70 6572 735f 7472   dict(n_opers_tr
-00006250: 616e 7366 6f72 6d65 643d 6e5f 6f70 6572  ansformed=n_oper
-00006260: 735f 7472 616e 7366 6f72 6d65 642c 0a20  s_transformed,. 
-00006270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006280: 2020 2020 2020 2020 2020 2020 6e6f 6973              nois
-00006290: 655f 6f70 6572 6174 6f72 735f 7374 6570  e_operators_step
-000062a0: 3d73 756d 5f63 6163 6865 290a 2020 2020  =sum_cache).    
-000062b0: 2020 2020 7265 7475 726e 206e 6f69 7365      return noise
-000062c0: 5f6f 7065 7261 746f 7273 2c20 696e 7465  _operators, inte
-000062d0: 726d 6564 6961 7465 730a 0a20 2020 2072  rmediates..    r
-000062e0: 6574 7572 6e20 6e6f 6973 655f 6f70 6572  eturn noise_oper
-000062f0: 6174 6f72 730a 0a0a 4075 7469 6c2e 7061  ators...@util.pa
-00006300: 7273 655f 6f70 7469 6f6e 616c 5f70 6172  rse_optional_par
-00006310: 616d 6574 6572 7328 7768 6963 683d 2827  ameters(which=('
-00006320: 746f 7461 6c27 2c20 2763 6f72 7265 6c61  total', 'correla
-00006330: 7469 6f6e 7327 2929 0a64 6566 2063 616c  tions')).def cal
-00006340: 6375 6c61 7465 5f63 6f6e 7472 6f6c 5f6d  culate_control_m
-00006350: 6174 7269 785f 6672 6f6d 5f61 746f 6d69  atrix_from_atomi
-00006360: 6328 0a20 2020 2020 2020 2070 6861 7365  c(.        phase
-00006370: 733a 206e 6461 7272 6179 2c0a 2020 2020  s: ndarray,.    
-00006380: 2020 2020 636f 6e74 726f 6c5f 6d61 7472      control_matr
-00006390: 6978 5f61 746f 6d69 633a 206e 6461 7272  ix_atomic: ndarr
-000063a0: 6179 2c0a 2020 2020 2020 2020 7072 6f70  ay,.        prop
-000063b0: 6167 6174 6f72 735f 6c69 6f75 7669 6c6c  agators_liouvill
-000063c0: 653a 206e 6461 7272 6179 2c0a 2020 2020  e: ndarray,.    
-000063d0: 2020 2020 7368 6f77 5f70 726f 6772 6573      show_progres
-000063e0: 7362 6172 3a20 626f 6f6c 203d 2046 616c  sbar: bool = Fal
-000063f0: 7365 2c0a 2020 2020 2020 2020 7768 6963  se,.        whic
-00006400: 683a 2073 7472 203d 2027 746f 7461 6c27  h: str = 'total'
-00006410: 0a29 202d 3e20 6e64 6172 7261 793a 0a20  .) -> ndarray:. 
-00006420: 2020 2072 2222 220a 2020 2020 4361 6c63     r""".    Calc
-00006430: 756c 6174 6520 7468 6520 636f 6e74 726f  ulate the contro
-00006440: 6c20 6d61 7472 6978 2066 726f 6d20 7468  l matrix from th
-00006450: 6520 636f 6e74 726f 6c20 6d61 7472 6963  e control matric
-00006460: 6573 206f 6620 6174 6f6d 6963 0a20 2020  es of atomic.   
-00006470: 2073 6567 6d65 6e74 732e 0a0a 2020 2020   segments...    
-00006480: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
-00006490: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 7068  ---------.    ph
-000064a0: 6173 6573 3a20 6172 7261 795f 6c69 6b65  ases: array_like
-000064b0: 2c20 7368 6170 6520 286e 5f64 742c 206e  , shape (n_dt, n
-000064c0: 5f6f 6d65 6761 290a 2020 2020 2020 2020  _omega).        
-000064d0: 5468 6520 7068 6173 6520 6661 6374 6f72  The phase factor
-000064e0: 7320 666f 7220 3a6d 6174 683a 6067 5c69  s for :math:`g\i
-000064f0: 6e5c 7b30 2c20 312c 205c 646f 7473 2c20  n\{0, 1, \dots, 
-00006500: 472d 315c 7d60 2e0a 2020 2020 636f 6e74  G-1\}`..    cont
-00006510: 726f 6c5f 6d61 7472 6978 5f61 746f 6d69  rol_matrix_atomi
-00006520: 633a 2061 7272 6179 5f6c 696b 652c 2073  c: array_like, s
-00006530: 6861 7065 2028 6e5f 6474 2c20 6e5f 6e6f  hape (n_dt, n_no
-00006540: 7073 2c20 642a 2a32 2c20 6e5f 6f6d 6567  ps, d**2, n_omeg
-00006550: 6129 0a20 2020 2020 2020 2054 6865 2070  a).        The p
-00006560: 756c 7365 2063 6f6e 7472 6f6c 206d 6174  ulse control mat
-00006570: 7269 6365 7320 666f 7220 3a6d 6174 683a  rices for :math:
-00006580: 6067 5c69 6e5c 7b31 2c20 322c 205c 646f  `g\in\{1, 2, \do
-00006590: 7473 2c20 475c 7d60 2e0a 2020 2020 7072  ts, G\}`..    pr
-000065a0: 6f70 6167 6174 6f72 735f 6c69 6f75 7669  opagators_liouvi
-000065b0: 6c6c 653a 2061 7272 6179 5f6c 696b 652c  lle: array_like,
-000065c0: 2073 6861 7065 2028 6e5f 6474 2c20 6e5f   shape (n_dt, n_
-000065d0: 6e6f 7073 2c20 642a 2a32 2c20 642a 2a32  nops, d**2, d**2
-000065e0: 290a 2020 2020 2020 2020 5468 6520 7472  ).        The tr
-000065f0: 616e 7366 6572 206d 6174 7269 6365 7320  ansfer matrices 
-00006600: 6f66 2074 6865 2063 756d 756c 6174 6976  of the cumulativ
-00006610: 6520 7072 6f70 6167 6174 6f72 7320 666f  e propagators fo
-00006620: 720a 2020 2020 2020 2020 3a6d 6174 683a  r.        :math:
-00006630: 6067 5c69 6e5c 7b30 2c20 312c 205c 646f  `g\in\{0, 1, \do
-00006640: 7473 2c20 472d 315c 7d60 2e0a 2020 2020  ts, G-1\}`..    
-00006650: 7368 6f77 5f70 726f 6772 6573 7362 6172  show_progressbar
-00006660: 3a20 626f 6f6c 2c20 6f70 7469 6f6e 616c  : bool, optional
-00006670: 0a20 2020 2020 2020 2053 686f 7720 6120  .        Show a 
-00006680: 7072 6f67 7265 7373 2062 6172 2066 6f72  progress bar for
-00006690: 2074 6865 2063 616c 6375 6c61 7469 6f6e   the calculation
-000066a0: 2e0a 2020 2020 7768 6963 683a 2073 7472  ..    which: str
-000066b0: 2c20 2827 746f 7461 6c27 2c20 2763 6f72  , ('total', 'cor
-000066c0: 7265 6c61 7469 6f6e 7327 290a 2020 2020  relations').    
-000066d0: 2020 2020 436f 6d70 7574 6520 7468 6520      Compute the 
-000066e0: 746f 7461 6c20 636f 6e74 726f 6c20 6d61  total control ma
-000066f0: 7472 6978 2028 7468 6520 7375 6d20 6f66  trix (the sum of
-00006700: 2061 6c6c 2074 696d 6520 7374 6570 7329   all time steps)
-00006710: 206f 720a 2020 2020 2020 2020 7468 6520   or.        the 
-00006720: 636f 7272 656c 6174 696f 6e20 636f 6e74  correlation cont
-00006730: 726f 6c20 6d61 7472 6978 2028 6669 7273  rol matrix (firs
-00006740: 7420 6178 6973 2068 6f6c 6473 2065 6163  t axis holds eac
-00006750: 6820 7075 6c73 6573 270a 2020 2020 2020  h pulses'.      
-00006760: 2020 636f 6e74 7269 6275 7469 6f6e 290a    contribution).
-00006770: 0a20 2020 2052 6574 7572 6e73 0a20 2020  .    Returns.   
-00006780: 202d 2d2d 2d2d 2d2d 0a20 2020 2063 6f6e   -------.    con
-00006790: 7472 6f6c 5f6d 6174 7269 783a 206e 6461  trol_matrix: nda
-000067a0: 7272 6179 2c20 7368 6170 6520 285b 6e5f  rray, shape ([n_
-000067b0: 706c 732c 5d20 6e5f 6e6f 7073 2c20 642a  pls,] n_nops, d*
-000067c0: 2a32 2c20 6e5f 6f6d 6567 6129 0a20 2020  *2, n_omega).   
-000067d0: 2020 2020 2054 6865 2063 6f6e 7472 6f6c       The control
-000067e0: 206d 6174 7269 7820 3a6d 6174 683a 605c   matrix :math:`\
-000067f0: 7469 6c64 657b 5c6d 6174 6863 616c 7b42  tilde{\mathcal{B
-00006800: 7d7d 285c 6f6d 6567 6129 602e 0a0a 2020  }}(\omega)`...  
-00006810: 2020 4e6f 7465 730a 2020 2020 2d2d 2d2d    Notes.    ----
-00006820: 2d0a 2020 2020 5468 6520 636f 6e74 726f  -.    The contro
-00006830: 6c20 6d61 7472 6978 2069 7320 6361 6c63  l matrix is calc
-00006840: 756c 6174 6564 2062 7920 6576 616c 7561  ulated by evalua
-00006850: 7469 6e67 2074 6865 2073 756d 0a0a 2020  ting the sum..  
-00006860: 2020 2e2e 206d 6174 683a 3a0a 0a20 2020    .. math::..   
-00006870: 2020 2020 205c 7469 6c64 657b 5c6d 6174       \tilde{\mat
-00006880: 6863 616c 7b42 7d7d 285c 6f6d 6567 6129  hcal{B}}(\omega)
-00006890: 203d 205c 7375 6d5f 7b67 3d31 7d5e 4720   = \sum_{g=1}^G 
-000068a0: 655e 7b69 5c6f 6d65 6761 2074 5f7b 672d  e^{i\omega t_{g-
-000068b0: 317d 7d0a 2020 2020 2020 2020 2020 2020  1}}.            
-000068c0: 5c74 696c 6465 7b5c 6d61 7468 6361 6c7b  \tilde{\mathcal{
-000068d0: 427d 7d5e 7b28 6729 7d28 5c6f 6d65 6761  B}}^{(g)}(\omega
-000068e0: 295c 6d61 7468 6361 6c7b 517d 5e7b 2867  )\mathcal{Q}^{(g
-000068f0: 2d31 297d 2e0a 0a20 2020 2053 6565 2041  -1)}...    See A
-00006900: 6c73 6f0a 2020 2020 2d2d 2d2d 2d2d 2d2d  lso.    --------
-00006910: 0a20 2020 2063 616c 6375 6c61 7465 5f63  .    calculate_c
-00006920: 6f6e 7472 6f6c 5f6d 6174 7269 785f 6672  ontrol_matrix_fr
-00006930: 6f6d 5f73 6372 6174 6368 3a20 436f 6e74  om_scratch: Cont
-00006940: 726f 6c20 6d61 7472 6978 2066 726f 6d20  rol matrix from 
-00006950: 7363 7261 7463 682e 0a20 2020 206c 696f  scratch..    lio
-00006960: 7576 696c 6c65 5f72 6570 7265 7365 6e74  uville_represent
-00006970: 6174 696f 6e3a 204c 696f 7576 696c 6c65  ation: Liouville
-00006980: 2072 6570 7265 7365 6e74 6174 696f 6e20   representation 
-00006990: 666f 7220 6120 6769 7665 6e20 6261 7369  for a given basi
-000069a0: 732e 0a20 2020 2022 2222 0a20 2020 206e  s..    """.    n
-000069b0: 203d 206c 656e 2863 6f6e 7472 6f6c 5f6d   = len(control_m
-000069c0: 6174 7269 785f 6174 6f6d 6963 290a 2020  atrix_atomic).  
-000069d0: 2020 2320 5365 7420 7570 2061 2072 6575    # Set up a reu
-000069e0: 7361 626c 6520 636f 6e74 7261 6374 696f  sable contractio
-000069f0: 6e20 6578 7072 6573 7369 6f6e 2e20 496e  n expression. In
-00006a00: 2073 6f6d 6520 6361 7365 7320 6974 2069   some cases it i
-00006a10: 7320 6661 7374 6572 2074 6f0a 2020 2020  s faster to.    
-00006a20: 2320 616c 736f 2063 6f6e 7472 6163 7420  # also contract 
-00006a30: 7468 6520 7469 6d65 2064 696d 656e 7369  the time dimensi
-00006a40: 6f6e 2069 6e20 7468 6520 7361 6d65 2065  on in the same e
-00006a50: 7870 7265 7373 696f 6e20 696e 7374 6561  xpression instea
-00006a60: 6420 6f66 0a20 2020 2023 206c 6f6f 7069  d of.    # loopi
-00006a70: 6e67 206f 7665 7220 6974 2c20 6275 7420  ng over it, but 
-00006a80: 7765 2064 6f6e 2774 2064 6973 7469 6e67  we don't disting
-00006a90: 7569 7368 2068 6572 6520 666f 7220 7265  uish here for re
-00006aa0: 6164 6162 696c 6974 792e 0a20 2020 2065  adability..    e
-00006ab0: 7870 7220 3d20 6f65 2e63 6f6e 7472 6163  xpr = oe.contrac
-00006ac0: 745f 6578 7072 6573 7369 6f6e 2827 696a  t_expression('ij
-00006ad0: 6f2c 6a6b 2d3e 696b 6f27 2c0a 2020 2020  o,jk->iko',.    
-00006ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006af0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00006b00: 6e74 726f 6c5f 6d61 7472 6978 5f61 746f  ntrol_matrix_ato
-00006b10: 6d69 632e 7368 6170 655b 313a 5d2c 0a20  mic.shape[1:],. 
-00006b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b40: 2070 726f 7061 6761 746f 7273 5f6c 696f   propagators_lio
-00006b50: 7576 696c 6c65 2e73 6861 7065 5b31 3a5d  uville.shape[1:]
-00006b60: 290a 0a20 2020 2023 2041 6c6c 6f63 6174  )..    # Allocat
-00006b70: 6520 6d65 6d6f 7279 0a20 2020 2069 6620  e memory.    if 
-00006b80: 7768 6963 6820 3d3d 2027 746f 7461 6c27  which == 'total'
-00006b90: 3a0a 2020 2020 2020 2020 636f 6e74 726f  :.        contro
-00006ba0: 6c5f 6d61 7472 6978 203d 206e 702e 7a65  l_matrix = np.ze
-00006bb0: 726f 7328 636f 6e74 726f 6c5f 6d61 7472  ros(control_matr
-00006bc0: 6978 5f61 746f 6d69 632e 7368 6170 655b  ix_atomic.shape[
-00006bd0: 313a 5d2c 2064 7479 7065 3d63 6f6d 706c  1:], dtype=compl
-00006be0: 6578 290a 2020 2020 2020 2020 666f 7220  ex).        for 
-00006bf0: 6720 696e 2075 7469 6c2e 7072 6f67 7265  g in util.progre
-00006c00: 7373 6261 725f 7261 6e67 6528 6e2c 2073  ssbar_range(n, s
-00006c10: 686f 775f 7072 6f67 7265 7373 6261 723d  how_progressbar=
-00006c20: 7368 6f77 5f70 726f 6772 6573 7362 6172  show_progressbar
-00006c30: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00006c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c50: 2020 2020 2020 2020 2020 6465 7363 3d27            desc='
-00006c60: 4361 6c63 756c 6174 696e 6720 636f 6e74  Calculating cont
-00006c70: 726f 6c20 6d61 7472 6978 2729 3a0a 2020  rol matrix'):.  
-00006c80: 2020 2020 2020 2020 2020 636f 6e74 726f            contro
-00006c90: 6c5f 6d61 7472 6978 202b 3d20 6578 7072  l_matrix += expr
-00006ca0: 2870 6861 7365 735b 675d 2a63 6f6e 7472  (phases[g]*contr
-00006cb0: 6f6c 5f6d 6174 7269 785f 6174 6f6d 6963  ol_matrix_atomic
-00006cc0: 5b67 5d2c 2070 726f 7061 6761 746f 7273  [g], propagators
-00006cd0: 5f6c 696f 7576 696c 6c65 5b67 5d29 0a20  _liouville[g]). 
-00006ce0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00006cf0: 2023 2077 6869 6368 203d 3d20 2763 6f72   # which == 'cor
-00006d00: 7265 6c61 7469 6f6e 7327 0a20 2020 2020  relations'.     
-00006d10: 2020 2063 6f6e 7472 6f6c 5f6d 6174 7269     control_matri
-00006d20: 7820 3d20 6e70 2e7a 6572 6f73 2863 6f6e  x = np.zeros(con
-00006d30: 7472 6f6c 5f6d 6174 7269 785f 6174 6f6d  trol_matrix_atom
-00006d40: 6963 2e73 6861 7065 2c20 6474 7970 653d  ic.shape, dtype=
-00006d50: 636f 6d70 6c65 7829 0a20 2020 2020 2020  complex).       
-00006d60: 2066 6f72 2067 2069 6e20 7574 696c 2e70   for g in util.p
-00006d70: 726f 6772 6573 7362 6172 5f72 616e 6765  rogressbar_range
-00006d80: 286e 2c20 7368 6f77 5f70 726f 6772 6573  (n, show_progres
-00006d90: 7362 6172 3d73 686f 775f 7072 6f67 7265  sbar=show_progre
-00006da0: 7373 6261 722c 0a20 2020 2020 2020 2020  ssbar,.         
-00006db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006dc0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00006dd0: 6573 633d 2743 616c 6375 6c61 7469 6e67  esc='Calculating
-00006de0: 2063 6f6e 7472 6f6c 206d 6174 7269 7827   control matrix'
-00006df0: 293a 0a20 2020 2020 2020 2020 2020 2063  ):.            c
-00006e00: 6f6e 7472 6f6c 5f6d 6174 7269 785b 675d  ontrol_matrix[g]
-00006e10: 203d 2065 7870 7228 7068 6173 6573 5b67   = expr(phases[g
-00006e20: 5d2a 636f 6e74 726f 6c5f 6d61 7472 6978  ]*control_matrix
-00006e30: 5f61 746f 6d69 635b 675d 2c20 7072 6f70  _atomic[g], prop
-00006e40: 6167 6174 6f72 735f 6c69 6f75 7669 6c6c  agators_liouvill
-00006e50: 655b 675d 290a 0a20 2020 2072 6574 7572  e[g])..    retur
-00006e60: 6e20 636f 6e74 726f 6c5f 6d61 7472 6978  n control_matrix
-00006e70: 0a0a 0a64 6566 2063 616c 6375 6c61 7465  ...def calculate
-00006e80: 5f63 6f6e 7472 6f6c 5f6d 6174 7269 785f  _control_matrix_
-00006e90: 6672 6f6d 5f73 6372 6174 6368 280a 2020  from_scratch(.  
-00006ea0: 2020 2020 2020 6569 6776 616c 733a 206e        eigvals: n
-00006eb0: 6461 7272 6179 2c0a 2020 2020 2020 2020  darray,.        
-00006ec0: 6569 6776 6563 733a 206e 6461 7272 6179  eigvecs: ndarray
-00006ed0: 2c0a 2020 2020 2020 2020 7072 6f70 6167  ,.        propag
-00006ee0: 6174 6f72 733a 206e 6461 7272 6179 2c0a  ators: ndarray,.
-00006ef0: 2020 2020 2020 2020 6f6d 6567 613a 2043          omega: C
-00006f00: 6f65 6666 6963 6965 6e74 732c 0a20 2020  oefficients,.   
-00006f10: 2020 2020 2062 6173 6973 3a20 4261 7369       basis: Basi
-00006f20: 732c 0a20 2020 2020 2020 206e 5f6f 7065  s,.        n_ope
-00006f30: 7273 3a20 5365 7175 656e 6365 5b4f 7065  rs: Sequence[Ope
-00006f40: 7261 746f 725d 2c0a 2020 2020 2020 2020  rator],.        
-00006f50: 6e5f 636f 6566 6673 3a20 5365 7175 656e  n_coeffs: Sequen
-00006f60: 6365 5b43 6f65 6666 6963 6965 6e74 735d  ce[Coefficients]
-00006f70: 2c0a 2020 2020 2020 2020 6474 3a20 436f  ,.        dt: Co
-00006f80: 6566 6669 6369 656e 7473 2c0a 2020 2020  efficients,.    
-00006f90: 2020 2020 743a 204f 7074 696f 6e61 6c5b      t: Optional[
-00006fa0: 436f 6566 6669 6369 656e 7473 5d20 3d20  Coefficients] = 
-00006fb0: 4e6f 6e65 2c0a 2020 2020 2020 2020 7368  None,.        sh
-00006fc0: 6f77 5f70 726f 6772 6573 7362 6172 3a20  ow_progressbar: 
-00006fd0: 626f 6f6c 203d 2046 616c 7365 2c0a 2020  bool = False,.  
-00006fe0: 2020 2020 2020 6361 6368 655f 696e 7465        cache_inte
-00006ff0: 726d 6564 6961 7465 733a 2062 6f6f 6c20  rmediates: bool 
-00007000: 3d20 4661 6c73 652c 0a20 2020 2020 2020  = False,.       
-00007010: 206f 7574 3a20 4f70 7469 6f6e 616c 5b6e   out: Optional[n
-00007020: 6461 7272 6179 5d20 3d20 4e6f 6e65 0a29  darray] = None.)
-00007030: 202d 3e20 556e 696f 6e5b 6e64 6172 7261   -> Union[ndarra
-00007040: 792c 2054 7570 6c65 5b6e 6461 7272 6179  y, Tuple[ndarray
-00007050: 2c20 4469 6374 5b73 7472 2c20 6e64 6172  , Dict[str, ndar
-00007060: 7261 795d 5d5d 3a0a 2020 2020 7222 2222  ray]]]:.    r"""
-00007070: 0a20 2020 2043 616c 6375 6c61 7465 2074  .    Calculate t
-00007080: 6865 2063 6f6e 7472 6f6c 206d 6174 7269  he control matri
-00007090: 7820 6672 6f6d 2073 6372 6174 6368 2c20  x from scratch, 
-000070a0: 692e 652e 2077 6974 686f 7574 206b 6e6f  i.e. without kno
-000070b0: 776c 6564 6765 206f 660a 2020 2020 7468  wledge of.    th
-000070c0: 6520 636f 6e74 726f 6c20 6d61 7472 6963  e control matric
-000070d0: 6573 206f 6620 6d6f 7265 2061 746f 6d69  es of more atomi
-000070e0: 6320 7075 6c73 6520 7365 7175 656e 6365  c pulse sequence
-000070f0: 732e 0a0a 2020 2020 5061 7261 6d65 7465  s...    Paramete
-00007100: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
-00007110: 2d0a 2020 2020 6569 6776 616c 733a 2061  -.    eigvals: a
-00007120: 7272 6179 5f6c 696b 652c 2073 6861 7065  rray_like, shape
-00007130: 2028 6e5f 6474 2c20 6429 0a20 2020 2020   (n_dt, d).     
-00007140: 2020 2045 6967 656e 7661 6c75 6520 7665     Eigenvalue ve
-00007150: 6374 6f72 7320 666f 7220 6561 6368 2074  ctors for each t
-00007160: 696d 6520 7075 6c73 6520 7365 676d 656e  ime pulse segmen
-00007170: 7420 2a67 2a20 7769 7468 2074 6865 0a20  t *g* with the. 
-00007180: 2020 2020 2020 2066 6972 7374 2061 7869         first axi
-00007190: 7320 636f 756e 7469 6e67 2074 6865 2070  s counting the p
-000071a0: 756c 7365 2073 6567 6d65 6e74 2c20 692e  ulse segment, i.
-000071b0: 652e 0a20 2020 2020 2020 2060 6065 6967  e..        ``eig
-000071c0: 7661 6c73 203d 3d20 6172 7261 7928 5b44  vals == array([D
-000071d0: 5f30 2c20 445f 312c 202e 2e2e 5d29 6060  _0, D_1, ...])``
-000071e0: 2e0a 2020 2020 6569 6776 6563 733a 2061  ..    eigvecs: a
-000071f0: 7272 6179 5f6c 696b 652c 2073 6861 7065  rray_like, shape
-00007200: 2028 6e5f 6474 2c20 642c 2064 290a 2020   (n_dt, d, d).  
-00007210: 2020 2020 2020 4569 6765 6e76 6563 746f        Eigenvecto
-00007220: 7220 6d61 7472 6963 6573 2066 6f72 2065  r matrices for e
-00007230: 6163 6820 7469 6d65 2070 756c 7365 2073  ach time pulse s
-00007240: 6567 6d65 6e74 202a 672a 2077 6974 6820  egment *g* with 
-00007250: 7468 650a 2020 2020 2020 2020 6669 7273  the.        firs
-00007260: 7420 6178 6973 2063 6f75 6e74 696e 6720  t axis counting 
-00007270: 7468 6520 7075 6c73 6520 7365 676d 656e  the pulse segmen
-00007280: 742c 2069 2e65 2e0a 2020 2020 2020 2020  t, i.e..        
-00007290: 6060 6569 6776 6563 7320 3d3d 2061 7272  ``eigvecs == arr
-000072a0: 6179 285b 565f 302c 2056 5f31 2c20 2e2e  ay([V_0, V_1, ..
-000072b0: 2e5d 2960 602e 0a20 2020 2070 726f 7061  .])``..    propa
-000072c0: 6761 746f 7273 3a20 6172 7261 795f 6c69  gators: array_li
-000072d0: 6b65 2c20 7368 6170 6520 286e 5f64 742b  ke, shape (n_dt+
-000072e0: 312c 2064 2c20 6429 0a20 2020 2020 2020  1, d, d).       
-000072f0: 2054 6865 2070 726f 7061 6761 746f 7273   The propagators
-00007300: 203a 6d61 7468 3a60 515f 6720 3d20 505f   :math:`Q_g = P_
-00007310: 6720 505f 7b67 2d31 7d5c 6364 6f74 7320  g P_{g-1}\cdots 
-00007320: 505f 3060 2061 7320 6120 2864 2c20 6429  P_0` as a (d, d)
-00007330: 0a20 2020 2020 2020 2061 7272 6179 2077  .        array w
-00007340: 6974 6820 2a64 2a20 7468 6520 6469 6d65  ith *d* the dime
-00007350: 6e73 696f 6e20 6f66 2074 6865 2048 696c  nsion of the Hil
-00007360: 6265 7274 2073 7061 6365 2e0a 2020 2020  bert space..    
-00007370: 6f6d 6567 613a 2061 7272 6179 5f6c 696b  omega: array_lik
-00007380: 652c 2073 6861 7065 2028 6e5f 6f6d 6567  e, shape (n_omeg
-00007390: 612c 290a 2020 2020 2020 2020 4672 6571  a,).        Freq
-000073a0: 7565 6e63 6965 7320 6174 2077 6869 6368  uencies at which
-000073b0: 2074 6865 2070 756c 7365 2063 6f6e 7472   the pulse contr
-000073c0: 6f6c 206d 6174 7269 7820 6973 2074 6f20  ol matrix is to 
-000073d0: 6265 0a20 2020 2020 2020 2065 7661 6c75  be.        evalu
-000073e0: 6174 6564 2e0a 2020 2020 6261 7369 733a  ated..    basis:
-000073f0: 2042 6173 6973 2c20 7368 6170 6520 2864   Basis, shape (d
-00007400: 2a2a 322c 2064 2c20 6429 0a20 2020 2020  **2, d, d).     
-00007410: 2020 2054 6865 2062 6173 6973 2065 6c65     The basis ele
-00007420: 6d65 6e74 7320 696e 2077 6869 6368 2074  ments in which t
-00007430: 6865 2070 756c 7365 2063 6f6e 7472 6f6c  he pulse control
-00007440: 206d 6174 7269 7820 7769 6c6c 2062 650a   matrix will be.
-00007450: 2020 2020 2020 2020 6578 7061 6e64 6564          expanded
-00007460: 2e0a 2020 2020 6e5f 6f70 6572 733a 2061  ..    n_opers: a
-00007470: 7272 6179 5f6c 696b 652c 2073 6861 7065  rray_like, shape
-00007480: 2028 6e5f 6e6f 7073 2c20 642c 2064 290a   (n_nops, d, d).
-00007490: 2020 2020 2020 2020 4e6f 6973 6520 6f70          Noise op
-000074a0: 6572 6174 6f72 7320 3a6d 6174 683a 6042  erators :math:`B
-000074b0: 5f5c 616c 7068 6160 2e0a 2020 2020 6e5f  _\alpha`..    n_
-000074c0: 636f 6566 6673 3a20 6172 7261 795f 6c69  coeffs: array_li
-000074d0: 6b65 2c20 7368 6170 6520 286e 5f6e 6f70  ke, shape (n_nop
-000074e0: 732c 206e 5f64 7429 0a20 2020 2020 2020  s, n_dt).       
-000074f0: 2054 6865 2073 656e 7369 7469 7669 7469   The sensitiviti
-00007500: 6573 206f 6620 7468 6520 7379 7374 656d  es of the system
-00007510: 2074 6f20 7468 6520 6e6f 6973 6520 6f70   to the noise op
-00007520: 6572 6174 6f72 7320 6769 7665 6e20 6279  erators given by
-00007530: 0a20 2020 2020 2020 202a 6e5f 6f70 6572  .        *n_oper
-00007540: 732a 2061 7420 7468 6520 6769 7665 6e20  s* at the given 
-00007550: 7469 6d65 2073 7465 702e 0a20 2020 2064  time step..    d
-00007560: 743a 2061 7272 6179 5f6c 696b 652c 2073  t: array_like, s
-00007570: 6861 7065 2028 6e5f 6474 290a 2020 2020  hape (n_dt).    
-00007580: 2020 2020 5365 7175 656e 6365 2064 7572      Sequence dur
-00007590: 6174 696f 6e2c 2069 2e65 2e20 666f 7220  ation, i.e. for 
-000075a0: 7468 6520 3a6d 6174 683a 6067 602d 7468  the :math:`g`-th
-000075b0: 2070 756c 7365 0a20 2020 2020 2020 203a   pulse.        :
-000075c0: 6d61 7468 3a60 745f 6720 2d20 745f 7b67  math:`t_g - t_{g
-000075d0: 2d31 7d60 2e0a 2020 2020 743a 2061 7272  -1}`..    t: arr
-000075e0: 6179 5f6c 696b 652c 2073 6861 7065 2028  ay_like, shape (
-000075f0: 6e5f 6474 2b31 292c 206f 7074 696f 6e61  n_dt+1), optiona
-00007600: 6c0a 2020 2020 2020 2020 5468 6520 6162  l.        The ab
-00007610: 736f 6c75 7465 2074 696d 6573 206f 6620  solute times of 
-00007620: 7468 6520 6469 6666 6572 656e 7420 7365  the different se
-00007630: 676d 656e 7473 2e20 4361 6e20 616c 736f  gments. Can also
-00007640: 2062 650a 2020 2020 2020 2020 636f 6d70   be.        comp
-00007650: 7574 6564 2066 726f 6d20 2a64 742a 2e0a  uted from *dt*..
-00007660: 2020 2020 7368 6f77 5f70 726f 6772 6573      show_progres
-00007670: 7362 6172 3a20 626f 6f6c 2c20 6f70 7469  sbar: bool, opti
-00007680: 6f6e 616c 0a20 2020 2020 2020 2053 686f  onal.        Sho
-00007690: 7720 6120 7072 6f67 7265 7373 2062 6172  w a progress bar
-000076a0: 2066 6f72 2074 6865 2063 616c 6375 6c61   for the calcula
-000076b0: 7469 6f6e 2e0a 2020 2020 6361 6368 655f  tion..    cache_
-000076c0: 696e 7465 726d 6564 6961 7465 733a 2062  intermediates: b
-000076d0: 6f6f 6c2c 206f 7074 696f 6e61 6c0a 2020  ool, optional.  
-000076e0: 2020 2020 2020 4b65 6570 2061 6e64 2072        Keep and r
-000076f0: 6574 7572 6e20 696e 7465 726d 6564 6961  eturn intermedia
-00007700: 7465 2074 6572 6d73 206f 6620 7468 6520  te terms of the 
-00007710: 6361 6c63 756c 6174 696f 6e20 7468 6174  calculation that
-00007720: 2063 616e 0a20 2020 2020 2020 2062 6520   can.        be 
-00007730: 7265 7573 6564 2069 6e20 6f74 6865 7220  reused in other 
-00007740: 636f 6d70 7574 6174 696f 6e73 2028 7365  computations (se
-00007750: 636f 6e64 206f 7264 6572 206f 7220 6772  cond order or gr
-00007760: 6164 6965 6e74 7329 2e0a 2020 2020 2020  adients)..      
-00007770: 2020 4f74 6865 7277 6973 6520 7468 6520    Otherwise the 
-00007780: 7375 6d20 6973 2070 6572 666f 726d 6564  sum is performed
-00007790: 2069 6e2d 706c 6163 652e 2054 6865 2064   in-place. The d
-000077a0: 6566 6175 6c74 2069 7320 4661 6c73 652e  efault is False.
-000077b0: 0a20 2020 206f 7574 3a20 6e64 6172 7261  .    out: ndarra
-000077c0: 792c 206f 7074 696f 6e61 6c0a 2020 2020  y, optional.    
-000077d0: 2020 2020 4120 6c6f 6361 7469 6f6e 2069      A location i
-000077e0: 6e74 6f20 7768 6963 6820 7468 6520 7265  nto which the re
-000077f0: 7375 6c74 2069 7320 7374 6f72 6564 2e20  sult is stored. 
-00007800: 5365 650a 2020 2020 2020 2020 3a66 756e  See.        :fun
-00007810: 633a 606e 756d 7079 2e75 6675 6e63 602e  c:`numpy.ufunc`.
-00007820: 0a0a 2020 2020 5265 7475 726e 730a 2020  ..    Returns.  
-00007830: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 636f    -------.    co
-00007840: 6e74 726f 6c5f 6d61 7472 6978 3a20 6e64  ntrol_matrix: nd
-00007850: 6172 7261 792c 2073 6861 7065 2028 6e5f  array, shape (n_
-00007860: 6e6f 7073 2c20 642a 2a32 2c20 6e5f 6f6d  nops, d**2, n_om
-00007870: 6567 6129 0a20 2020 2020 2020 2054 6865  ega).        The
-00007880: 2063 6f6e 7472 6f6c 206d 6174 7269 7820   control matrix 
-00007890: 3a6d 6174 683a 605c 7469 6c64 657b 5c6d  :math:`\tilde{\m
-000078a0: 6174 6863 616c 7b42 7d7d 285c 6f6d 6567  athcal{B}}(\omeg
-000078b0: 6129 600a 2020 2020 696e 7465 726d 6564  a)`.    intermed
-000078c0: 6961 7465 733a 2064 6963 745b 7374 722c  iates: dict[str,
-000078d0: 206e 6461 7272 6179 5d0a 2020 2020 2020   ndarray].      
-000078e0: 2020 496e 7465 726d 6564 6961 7465 2072    Intermediate r
-000078f0: 6573 756c 7473 206f 6620 7468 6520 6361  esults of the ca
-00007900: 6c63 756c 6174 696f 6e2e 204f 6e6c 7920  lculation. Only 
-00007910: 6966 0a20 2020 2020 2020 2063 6163 6865  if.        cache
-00007920: 5f69 6e74 6572 6d65 6469 6174 6573 2069  _intermediates i
-00007930: 7320 5472 7565 2e0a 0a20 2020 204e 6f74  s True...    Not
-00007940: 6573 0a20 2020 202d 2d2d 2d2d 0a20 2020  es.    -----.   
-00007950: 2054 6865 2063 6f6e 7472 6f6c 206d 6174   The control mat
-00007960: 7269 7820 6973 2063 616c 6375 6c61 7465  rix is calculate
-00007970: 6420 6163 636f 7264 696e 6720 746f 0a0a  d according to..
-00007980: 2020 2020 2e2e 206d 6174 683a 3a0a 0a20      .. math::.. 
-00007990: 2020 2020 2020 205c 7469 6c64 657b 5c6d         \tilde{\m
-000079a0: 6174 6863 616c 7b42 7d7d 5f7b 5c61 6c70  athcal{B}}_{\alp
-000079b0: 6861 206b 7d28 5c6f 6d65 6761 2920 3d20  ha k}(\omega) = 
-000079c0: 5c73 756d 5f7b 673d 317d 5e47 0a20 2020  \sum_{g=1}^G.   
-000079d0: 2020 2020 2020 2020 2065 5e7b 695c 6f6d           e^{i\om
-000079e0: 6567 6120 745f 7b67 2d31 7d7d 2073 5f5c  ega t_{g-1}} s_\
-000079f0: 616c 7068 615e 7b28 6729 7d5c 6d61 7468  alpha^{(g)}\math
-00007a00: 726d 7b74 727d 5c6c 6566 7428 0a20 2020  rm{tr}\left(.   
-00007a10: 2020 2020 2020 2020 2020 2020 205b 5c62               [\b
-00007a20: 6172 7b42 7d5f 5c61 6c70 6861 5e7b 2867  ar{B}_\alpha^{(g
-00007a30: 297d 5c63 6972 6320 4928 5c6f 6d65 6761  )}\circ I(\omega
-00007a40: 295d 205c 6261 727b 437d 5f6b 5e7b 2867  )] \bar{C}_k^{(g
-00007a50: 297d 0a20 2020 2020 2020 2020 2020 205c  )}.            \
-00007a60: 7269 6768 7429 0a0a 2020 2020 7768 6572  right)..    wher
-00007a70: 650a 0a20 2020 202e 2e20 6d61 7468 3a3a  e..    .. math::
-00007a80: 0a0a 2020 2020 2020 2020 495e 7b28 6729  ..        I^{(g)
-00007a90: 7d5f 7b6e 6d7d 285c 6f6d 6567 6129 2026  }_{nm}(\omega) &
-00007aa0: 3d20 5c69 6e74 5f30 5e7b 745f 6c20 2d20  = \int_0^{t_l - 
-00007ab0: 745f 7b67 2d31 7d7d 5c6d 6174 6872 6d7b  t_{g-1}}\mathrm{
-00007ac0: 647d 745c 2c0a 2020 2020 2020 2020 2020  d}t\,.          
-00007ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ae0: 2020 2020 2020 655e 7b69 285c 6f6d 6567        e^{i(\omeg
-00007af0: 612b 5c6f 6d65 6761 5f6e 2d5c 6f6d 6567  a+\omega_n-\omeg
-00007b00: 615f 6d29 747d 205c 5c0a 2020 2020 2020  a_m)t} \\.      
-00007b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b20: 2020 2020 2020 2026 3d20 5c66 7261 637b         &= \frac{
-00007b30: 655e 7b69 285c 6f6d 6567 612b 5c6f 6d65  e^{i(\omega+\ome
-00007b40: 6761 5f6e 2d5c 6f6d 6567 615f 6d29 0a20  ga_n-\omega_m). 
-00007b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b60: 2020 2020 2020 2020 2020 2020 2020 2028                 (
-00007b70: 745f 6c20 2d20 745f 7b67 2d31 7d29 7d20  t_l - t_{g-1})} 
-00007b80: 2d20 317d 0a20 2020 2020 2020 2020 2020  - 1}.           
-00007b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ba0: 2020 2020 207b 6928 5c6f 6d65 6761 2b5c       {i(\omega+\
-00007bb0: 6f6d 6567 615f 6e2d 5c6f 6d65 6761 5f6d  omega_n-\omega_m
-00007bc0: 297d 2c20 5c5c 0a20 2020 2020 2020 205c  )}, \\.        \
-00007bd0: 6261 727b 427d 5f5c 616c 7068 615e 7b28  bar{B}_\alpha^{(
-00007be0: 6729 7d20 263d 2056 5e7b 2867 295c 6461  g)} &= V^{(g)\da
-00007bf0: 6767 6572 7d20 425f 5c61 6c70 6861 2056  gger} B_\alpha V
-00007c00: 5e7b 2867 297d 2c20 5c5c 0a20 2020 2020  ^{(g)}, \\.     
-00007c10: 2020 205c 6261 727b 437d 5f6b 5e7b 2867     \bar{C}_k^{(g
-00007c20: 297d 2026 3d20 565e 7b28 6729 5c64 6167  )} &= V^{(g)\dag
-00007c30: 6765 727d 2051 5f7b 672d 317d 2043 5f6b  ger} Q_{g-1} C_k
-00007c40: 2051 5f7b 672d 317d 5e5c 6461 6767 6572   Q_{g-1}^\dagger
-00007c50: 2056 5e7b 2867 297d 2c0a 0a20 2020 2061   V^{(g)},..    a
-00007c60: 6e64 203a 6d61 7468 3a60 565e 7b28 6729  nd :math:`V^{(g)
-00007c70: 7d60 2069 7320 7468 6520 6d61 7472 6978  }` is the matrix
-00007c80: 206f 6620 6569 6765 6e76 6563 746f 7273   of eigenvectors
-00007c90: 2074 6861 7420 6469 6167 6f6e 616c 697a   that diagonaliz
-00007ca0: 6573 0a20 2020 203a 6d61 7468 3a60 5c74  es.    :math:`\t
-00007cb0: 696c 6465 7b5c 6d61 7468 6361 6c7b 487d  ilde{\mathcal{H}
-00007cc0: 7d5f 6e5e 7b28 6729 7d60 2c20 3a6d 6174  }_n^{(g)}`, :mat
-00007cd0: 683a 6042 5f5c 616c 7068 6160 2074 6865  h:`B_\alpha` the
-00007ce0: 0a20 2020 203a 6d61 7468 3a60 5c61 6c70  .    :math:`\alp
-00007cf0: 6861 602d 7468 206e 6f69 7365 206f 7065  ha`-th noise ope
-00007d00: 7261 746f 7220 3a6d 6174 683a 6073 5f5c  rator :math:`s_\
-00007d10: 616c 7068 615e 7b28 6729 7d60 2074 6865  alpha^{(g)}` the
-00007d20: 206e 6f69 7365 0a20 2020 2073 656e 7369   noise.    sensi
-00007d30: 7469 7669 7479 2064 7572 696e 6720 696e  tivity during in
-00007d40: 7465 7276 616c 203a 6d61 7468 3a60 6760  terval :math:`g`
-00007d50: 2c20 616e 6420 3a6d 6174 683a 6043 5f6b  , and :math:`C_k
-00007d60: 6020 7468 650a 2020 2020 3a6d 6174 683a  ` the.    :math:
-00007d70: 606b 602d 7468 2062 6173 6973 2065 6c65  `k`-th basis ele
-00007d80: 6d65 6e74 2e0a 0a20 2020 2053 6565 2041  ment...    See A
-00007d90: 6c73 6f0a 2020 2020 2d2d 2d2d 2d2d 2d2d  lso.    --------
-00007da0: 0a20 2020 2063 616c 6375 6c61 7465 5f63  .    calculate_c
-00007db0: 6f6e 7472 6f6c 5f6d 6174 7269 785f 6672  ontrol_matrix_fr
-00007dc0: 6f6d 5f61 746f 6d69 633a 2043 6f6e 7472  om_atomic: Contr
-00007dd0: 6f6c 206d 6174 7269 7820 6672 6f6d 2063  ol matrix from c
-00007de0: 6f6e 6361 7465 6e61 7469 6f6e 2e0a 2020  oncatenation..  
-00007df0: 2020 6361 6c63 756c 6174 655f 636f 6e74    calculate_cont
-00007e00: 726f 6c5f 6d61 7472 6978 5f70 6572 696f  rol_matrix_perio
-00007e10: 6469 633a 2043 6f6e 7472 6f6c 206d 6174  dic: Control mat
-00007e20: 7269 7820 666f 7220 7065 7269 6f64 6963  rix for periodic
-00007e30: 2073 7973 7465 6d2e 0a20 2020 2022 2222   system..    """
-00007e40: 0a20 2020 2064 203d 2065 6967 7665 6373  .    d = eigvecs
-00007e50: 2e73 6861 7065 5b2d 315d 0a0a 2020 2020  .shape[-1]..    
-00007e60: 6966 2074 2069 7320 4e6f 6e65 3a0a 2020  if t is None:.  
-00007e70: 2020 2020 2020 7420 3d20 6e70 2e63 6f6e        t = np.con
-00007e80: 6361 7465 6e61 7465 2828 5b30 5d2c 206e  catenate(([0], n
-00007e90: 702e 6173 6172 7261 7928 6474 292e 6375  p.asarray(dt).cu
-00007ea0: 6d73 756d 2829 2929 0a0a 2020 2020 2320  msum()))..    # 
-00007eb0: 5072 6563 6f6d 7075 7465 206e 6f69 7365  Precompute noise
-00007ec0: 206f 7065 7273 2074 7261 6e73 666f 726d   opers transform
-00007ed0: 6564 2074 6f20 6569 6765 6e62 6173 6973  ed to eigenbasis
-00007ee0: 206f 6620 6561 6368 2070 756c 7365 2073   of each pulse s
-00007ef0: 6567 6d65 6e74 0a20 2020 2023 2061 6e64  egment.    # and
-00007f00: 2051 5e5c 6461 6767 6572 2040 2056 0a20   Q^\dagger @ V. 
-00007f10: 2020 2065 6967 7665 6373 5f70 726f 7061     eigvecs_propa
-00007f20: 6761 7465 6420 3d20 5f70 726f 7061 6761  gated = _propaga
-00007f30: 7465 5f65 6967 656e 7665 6374 6f72 7328  te_eigenvectors(
-00007f40: 7072 6f70 6167 6174 6f72 735b 3a2d 315d  propagators[:-1]
-00007f50: 2c20 6569 6776 6563 7329 0a20 2020 206e  , eigvecs).    n
-00007f60: 5f6f 7065 7273 5f74 7261 6e73 666f 726d  _opers_transform
-00007f70: 6564 203d 205f 7472 616e 7366 6f72 6d5f  ed = _transform_
-00007f80: 6861 6d69 6c74 6f6e 6961 6e28 6569 6776  hamiltonian(eigv
-00007f90: 6563 732c 206e 5f6f 7065 7273 2c20 6e5f  ecs, n_opers, n_
-00007fa0: 636f 6566 6673 290a 0a20 2020 2023 2041  coeffs)..    # A
-00007fb0: 6c6c 6f63 6174 6520 7265 7375 6c74 2061  llocate result a
-00007fc0: 6e64 2062 7566 6665 7273 2066 6f72 2069  nd buffers for i
-00007fd0: 6e74 6572 6d65 6469 6174 6520 6172 7261  ntermediate arra
-00007fe0: 7973 0a20 2020 2065 7870 5f62 7566 203d  ys.    exp_buf =
-00007ff0: 206e 702e 656d 7074 7928 286c 656e 286f   np.empty((len(o
-00008000: 6d65 6761 292c 2064 2c20 6429 2c20 6474  mega), d, d), dt
-00008010: 7970 653d 636f 6d70 6c65 7829 0a20 2020  ype=complex).   
-00008020: 2069 6620 6f75 7420 6973 204e 6f6e 653a   if out is None:
-00008030: 0a20 2020 2020 2020 206f 7574 203d 206e  .        out = n
-00008040: 702e 7a65 726f 7328 286c 656e 286e 5f6f  p.zeros((len(n_o
-00008050: 7065 7273 292c 206c 656e 2862 6173 6973  pers), len(basis
-00008060: 292c 206c 656e 286f 6d65 6761 2929 2c20  ), len(omega)), 
-00008070: 6474 7970 653d 636f 6d70 6c65 7829 0a0a  dtype=complex)..
-00008080: 2020 2020 6966 2063 6163 6865 5f69 6e74      if cache_int
-00008090: 6572 6d65 6469 6174 6573 3a0a 2020 2020  ermediates:.    
-000080a0: 2020 2020 6261 7369 735f 7472 616e 7366      basis_transf
-000080b0: 6f72 6d65 645f 6361 6368 6520 3d20 6e70  ormed_cache = np
-000080c0: 2e65 6d70 7479 2828 6c65 6e28 6474 292c  .empty((len(dt),
-000080d0: 202a 6261 7369 732e 7368 6170 6529 2c20   *basis.shape), 
-000080e0: 6474 7970 653d 636f 6d70 6c65 7829 0a20  dtype=complex). 
-000080f0: 2020 2020 2020 2070 6861 7365 5f66 6163         phase_fac
-00008100: 746f 7273 5f63 6163 6865 203d 206e 702e  tors_cache = np.
-00008110: 656d 7074 7928 286c 656e 2864 7429 2c20  empty((len(dt), 
-00008120: 6c65 6e28 6f6d 6567 6129 292c 2064 7479  len(omega)), dty
-00008130: 7065 3d63 6f6d 706c 6578 290a 2020 2020  pe=complex).    
-00008140: 2020 2020 696e 745f 6361 6368 6520 3d20      int_cache = 
-00008150: 6e70 2e65 6d70 7479 2828 6c65 6e28 6474  np.empty((len(dt
-00008160: 292c 206c 656e 286f 6d65 6761 292c 2064  ), len(omega), d
-00008170: 2c20 6429 2c20 6474 7970 653d 636f 6d70  , d), dtype=comp
-00008180: 6c65 7829 0a20 2020 2020 2020 2073 756d  lex).        sum
-00008190: 5f63 6163 6865 203d 206e 702e 656d 7074  _cache = np.empt
-000081a0: 7928 286c 656e 2864 7429 2c20 6c65 6e28  y((len(dt), len(
-000081b0: 6e5f 6f70 6572 7329 2c20 6c65 6e28 6261  n_opers), len(ba
-000081c0: 7369 7329 2c20 6c65 6e28 6f6d 6567 6129  sis), len(omega)
-000081d0: 292c 2064 7479 7065 3d63 6f6d 706c 6578  ), dtype=complex
-000081e0: 290a 2020 2020 656c 7365 3a0a 2020 2020  ).    else:.    
-000081f0: 2020 2020 6261 7369 735f 7472 616e 7366      basis_transf
-00008200: 6f72 6d65 6420 3d20 6e70 2e65 6d70 7479  ormed = np.empty
-00008210: 2862 6173 6973 2e73 6861 7065 2c20 6474  (basis.shape, dt
-00008220: 7970 653d 636f 6d70 6c65 7829 0a20 2020  ype=complex).   
-00008230: 2020 2020 2070 6861 7365 5f66 6163 746f       phase_facto
-00008240: 7273 203d 206e 702e 656d 7074 7928 6c65  rs = np.empty(le
-00008250: 6e28 6f6d 6567 6129 2c20 6474 7970 653d  n(omega), dtype=
-00008260: 636f 6d70 6c65 7829 0a20 2020 2020 2020  complex).       
-00008270: 2069 6e74 5f62 7566 203d 206e 702e 656d   int_buf = np.em
-00008280: 7074 7928 286c 656e 286f 6d65 6761 292c  pty((len(omega),
-00008290: 2064 2c20 6429 2c20 6474 7970 653d 636f   d, d), dtype=co
-000082a0: 6d70 6c65 7829 0a20 2020 2020 2020 2073  mplex).        s
-000082b0: 756d 5f62 7566 203d 206e 702e 656d 7074  um_buf = np.empt
-000082c0: 7928 286c 656e 286e 5f6f 7065 7273 292c  y((len(n_opers),
-000082d0: 206c 656e 2862 6173 6973 292c 206c 656e   len(basis), len
-000082e0: 286f 6d65 6761 2929 2c20 6474 7970 653d  (omega)), dtype=
-000082f0: 636f 6d70 6c65 7829 0a0a 2020 2020 2320  complex)..    # 
-00008300: 4f70 7469 6d69 7a65 2074 6865 2063 6f6e  Optimize the con
-00008310: 7472 6163 7469 6f6e 2070 6174 6820 6479  traction path dy
-00008320: 6e61 6d69 6361 6c6c 7920 7369 6e63 6520  namically since 
-00008330: 6974 2064 6966 6665 7273 2066 6f72 2064  it differs for d
-00008340: 6966 6665 7265 6e74 0a20 2020 2023 2076  ifferent.    # v
-00008350: 616c 7565 7320 6f66 2064 0a20 2020 2065  alues of d.    e
-00008360: 7870 7220 3d20 6f65 2e63 6f6e 7472 6163  xpr = oe.contrac
-00008370: 745f 6578 7072 6573 7369 6f6e 2827 6f2c  t_expression('o,
-00008380: 6a6d 6e2c 6f6d 6e2c 6b6e 6d2d 3e6a 6b6f  jmn,omn,knm->jko
-00008390: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
-000083a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000083b0: 2020 2020 206f 6d65 6761 2e73 6861 7065       omega.shape
-000083c0: 2c20 6e5f 6f70 6572 735f 7472 616e 7366  , n_opers_transf
-000083d0: 6f72 6d65 645b 3a2c 2030 5d2e 7368 6170  ormed[:, 0].shap
-000083e0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+000038a0: 2065 696e 7375 6d5f 7374 7220 3d20 2767   einsum_str = 'g
+000038b0: 616b 6f2c 6162 6f2c 6862 6b6f 2d3e 6768  ako,abo,hbko->gh
+000038c0: 6162 6f27 0a20 2020 2020 2020 2020 2020  abo'.           
+000038d0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+000038e0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+000038f0: 2077 6869 6368 5f46 4620 3d3d 2027 6765   which_FF == 'ge
+00003900: 6e65 7261 6c69 7a65 6427 0a20 2020 2020  neralized'.     
+00003910: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00003920: 696e 7375 6d5f 7374 7220 3d20 2767 616b  insum_str = 'gak
+00003930: 6f2c 6162 6f2c 6862 6c6f 2d3e 6768 6162  o,abo,hblo->ghab
+00003940: 6b6c 6f27 0a20 2020 2020 2020 2020 2020  klo'.           
+00003950: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00003960: 2020 2020 2020 2023 2077 6869 6368 5f70         # which_p
+00003970: 756c 7365 203d 3d20 2774 6f74 616c 270a  ulse == 'total'.
+00003980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003990: 6966 2077 6869 6368 5f46 4620 3d3d 2027  if which_FF == '
+000039a0: 6669 6465 6c69 7479 273a 0a20 2020 2020  fidelity':.     
+000039b0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+000039c0: 696e 7375 6d5f 7374 7220 3d20 2761 6b6f  insum_str = 'ako
+000039d0: 2c61 626f 2c62 6b6f 2d3e 6162 6f27 0a20  ,abo,bko->abo'. 
+000039e0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+000039f0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00003a00: 2020 2020 2020 2020 2023 2077 6869 6368           # which
+00003a10: 5f46 4620 3d3d 2027 6765 6e65 7261 6c69  _FF == 'generali
+00003a20: 7a65 6427 0a20 2020 2020 2020 2020 2020  zed'.           
+00003a30: 2020 2020 2020 2020 2065 696e 7375 6d5f           einsum_
+00003a40: 7374 7220 3d20 2761 6b6f 2c61 626f 2c62  str = 'ako,abo,b
+00003a50: 6c6f 2d3e 6162 6b6c 6f27 0a0a 2020 2020  lo->abklo'..    
+00003a60: 2020 2020 2020 2020 696e 7465 6772 616e          integran
+00003a70: 6420 3d20 6e70 2e65 696e 7375 6d28 6569  d = np.einsum(ei
+00003a80: 6e73 756d 5f73 7472 2c0a 2020 2020 2020  nsum_str,.      
+00003a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003aa0: 2020 2020 2020 2020 2020 2020 6374 726c              ctrl
+00003ab0: 5f6c 6566 745b 2e2e 2e2c 2069 6478 2c20  _left[..., idx, 
+00003ac0: 3a2c 203a 5d2c 2073 7065 6374 7275 6d2c  :, :], spectrum,
+00003ad0: 2063 7472 6c5f 7269 6768 745b 2e2e 2e2c   ctrl_right[...,
+00003ae0: 2069 6478 2c20 3a2c 203a 5d29 0a0a 2020   idx, :, :])..  
+00003af0: 2020 7265 7475 726e 2069 6e74 6567 7261    return integra
+00003b00: 6e64 2e72 6561 6c0a 0a0a 6465 6620 6361  nd.real...def ca
+00003b10: 6c63 756c 6174 655f 6e6f 6973 655f 6f70  lculate_noise_op
+00003b20: 6572 6174 6f72 735f 6672 6f6d 5f61 746f  erators_from_ato
+00003b30: 6d69 6328 0a20 2020 2020 2020 2070 6861  mic(.        pha
+00003b40: 7365 733a 206e 6461 7272 6179 2c0a 2020  ses: ndarray,.  
+00003b50: 2020 2020 2020 6e6f 6973 655f 6f70 6572        noise_oper
+00003b60: 6174 6f72 735f 6174 6f6d 6963 3a20 6e64  ators_atomic: nd
+00003b70: 6172 7261 792c 0a20 2020 2020 2020 2070  array,.        p
+00003b80: 726f 7061 6761 746f 7273 3a20 6e64 6172  ropagators: ndar
+00003b90: 7261 792c 0a20 2020 2020 2020 2073 686f  ray,.        sho
+00003ba0: 775f 7072 6f67 7265 7373 6261 723a 2062  w_progressbar: b
+00003bb0: 6f6f 6c20 3d20 4661 6c73 650a 2920 2d3e  ool = False.) ->
+00003bc0: 206e 6461 7272 6179 3a0a 2020 2020 7222   ndarray:.    r"
+00003bd0: 2222 0a20 2020 2043 616c 6375 6c61 7465  "".    Calculate
+00003be0: 2074 6865 2069 6e74 6572 6163 7469 6f6e   the interaction
+00003bf0: 2070 6963 7574 7265 206e 6f69 7365 206f   picutre noise o
+00003c00: 7065 7261 746f 7273 2066 726f 6d20 6174  perators from at
+00003c10: 6f6d 6963 2073 6567 6d65 6e74 732e 0a0a  omic segments...
+00003c20: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+00003c30: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+00003c40: 2020 7068 6173 6573 3a20 6172 7261 795f    phases: array_
+00003c50: 6c69 6b65 2c20 7368 6170 6520 286e 5f64  like, shape (n_d
+00003c60: 742c 206e 5f6f 6d65 6761 290a 2020 2020  t, n_omega).    
+00003c70: 2020 2020 5468 6520 7068 6173 6520 6661      The phase fa
+00003c80: 6374 6f72 7320 666f 7220 3a6d 6174 683a  ctors for :math:
+00003c90: 6067 5c69 6e5c 7b30 2c20 312c 205c 646f  `g\in\{0, 1, \do
+00003ca0: 7473 2c20 472d 315c 7d60 2e0a 2020 2020  ts, G-1\}`..    
+00003cb0: 6e6f 6973 655f 6f70 6572 6174 6f72 735f  noise_operators_
+00003cc0: 6174 6f6d 6963 3a20 6172 7261 795f 6c69  atomic: array_li
+00003cd0: 6b65 2c20 7368 6170 6520 286e 5f64 742c  ke, shape (n_dt,
+00003ce0: 206e 5f6e 6f70 732c 2064 2c20 642c 206e   n_nops, d, d, n
+00003cf0: 5f6f 6d65 6761 290a 2020 2020 2020 2020  _omega).        
+00003d00: 5468 6520 6e6f 6973 6520 6f70 6572 6174  The noise operat
+00003d10: 6f72 7320 696e 2074 6865 2069 6e74 6572  ors in the inter
+00003d20: 6163 7469 6f6e 2070 6963 7475 7265 206f  action picture o
+00003d30: 6620 7468 6520 672d 7468 0a20 2020 2020  f the g-th.     
+00003d40: 2020 2070 756c 7365 2c20 692e 652e 2066     pulse, i.e. f
+00003d50: 6f72 203a 6d61 7468 3a60 675c 696e 5c7b  or :math:`g\in\{
+00003d60: 312c 2032 2c20 5c64 6f74 732c 2047 5c7d  1, 2, \dots, G\}
+00003d70: 602e 0a20 2020 2070 726f 7061 6761 746f  `..    propagato
+00003d80: 7273 3a20 6172 7261 795f 6c69 6b65 2c20  rs: array_like, 
+00003d90: 7368 6170 6520 286e 5f64 742c 2064 2c20  shape (n_dt, d, 
+00003da0: 6429 0a20 2020 2020 2020 2054 6865 2063  d).        The c
+00003db0: 756d 756c 6174 6976 6520 7072 6f70 6167  umulative propag
+00003dc0: 6174 6f72 7320 6f66 2074 6865 2070 756c  ators of the pul
+00003dd0: 7365 730a 2020 2020 2020 2020 3a6d 6174  ses.        :mat
+00003de0: 683a 6067 5c69 6e5c 7b30 2c20 312c 205c  h:`g\in\{0, 1, \
+00003df0: 646f 7473 2c20 472d 315c 7d60 2e0a 2020  dots, G-1\}`..  
+00003e00: 2020 7368 6f77 5f70 726f 6772 6573 7362    show_progressb
+00003e10: 6172 3a20 626f 6f6c 2c20 6f70 7469 6f6e  ar: bool, option
+00003e20: 616c 0a20 2020 2020 2020 2053 686f 7720  al.        Show 
+00003e30: 6120 7072 6f67 7265 7373 2062 6172 2066  a progress bar f
+00003e40: 6f72 2074 6865 2063 616c 6375 6c61 7469  or the calculati
+00003e50: 6f6e 2e0a 0a20 2020 2052 6574 7572 6e73  on...    Returns
+00003e60: 0a20 2020 202d 2d2d 2d2d 2d2d 0a20 2020  .    -------.   
+00003e70: 206e 6f69 7365 5f6f 7065 7261 746f 7273   noise_operators
+00003e80: 3a20 6e64 6172 7261 792c 2073 6861 7065  : ndarray, shape
+00003e90: 2028 6e5f 6f6d 6567 612c 206e 5f6e 6f70   (n_omega, n_nop
+00003ea0: 732c 2064 2c20 6429 0a20 2020 2020 2020  s, d, d).       
+00003eb0: 2054 6865 2069 6e74 6572 6163 7469 6f6e   The interaction
+00003ec0: 2070 6963 7475 7265 206e 6f69 7365 206f   picture noise o
+00003ed0: 7065 7261 746f 7273 0a20 2020 2020 2020  perators.       
+00003ee0: 203a 6d61 7468 3a60 5c74 696c 6465 7b42   :math:`\tilde{B
+00003ef0: 7d5f 5c61 6c70 6861 285c 6f6d 6567 6129  }_\alpha(\omega)
+00003f00: 602e 0a0a 2020 2020 4e6f 7465 730a 2020  `...    Notes.  
+00003f10: 2020 2d2d 2d2d 2d0a 2020 2020 5468 6520    -----.    The 
+00003f20: 6e6f 6973 6520 6f70 6572 6174 6f72 7320  noise operators 
+00003f30: 6172 6520 6361 6c63 756c 6174 6564 2062  are calculated b
+00003f40: 7920 6576 616c 7561 7469 6e67 2074 6865  y evaluating the
+00003f50: 2073 756d 0a0a 2020 2020 2e2e 206d 6174   sum..    .. mat
+00003f60: 683a 3a0a 0a20 2020 2020 2020 205c 7469  h::..        \ti
+00003f70: 6c64 657b 427d 5f5c 616c 7068 6128 5c6f  lde{B}_\alpha(\o
+00003f80: 6d65 6761 2920 3d20 5c73 756d 5f7b 673d  mega) = \sum_{g=
+00003f90: 317d 5e47 2065 5e7b 695c 6f6d 6567 6120  1}^G e^{i\omega 
+00003fa0: 745f 7b67 2d31 7d7d 0a20 2020 2020 2020  t_{g-1}}.       
+00003fb0: 2020 2020 2020 515f 7b67 2d31 7d5e 5c64        Q_{g-1}^\d
+00003fc0: 6167 6765 725c 7469 6c64 657b 427d 5f5c  agger\tilde{B}_\
+00003fd0: 616c 7068 615e 7b28 6729 7d28 5c6f 6d65  alpha^{(g)}(\ome
+00003fe0: 6761 2920 515f 7b67 2d31 7d2e 0a0a 2020  ga) Q_{g-1}...  
+00003ff0: 2020 5468 6520 636f 6e74 726f 6c20 6d61    The control ma
+00004000: 7472 6978 2074 6865 6e20 636f 7272 6573  trix then corres
+00004010: 706f 6e64 7320 746f 2074 6865 2063 6f65  ponds to the coe
+00004020: 6666 6963 6965 6e74 7320 6f66 2065 7870  fficients of exp
+00004030: 616e 7369 6f6e 0a20 2020 2069 6e20 616e  ansion.    in an
+00004040: 206f 7065 7261 746f 7220 6261 7369 7320   operator basis 
+00004050: 3a6d 6174 683a 605c 7b43 5f6b 5c7d 5f6b  :math:`\{C_k\}_k
+00004060: 603a 0a0a 2020 2020 2e2e 206d 6174 683a  `:..    .. math:
+00004070: 3a0a 2020 2020 2020 2020 5c74 696c 6465  :.        \tilde
+00004080: 7b5c 6d61 7468 6361 6c7b 427d 7d5f 7b6b  {\mathcal{B}}_{k
+00004090: 5c61 6c70 6861 7d28 5c6f 6d65 6761 2920  \alpha}(\omega) 
+000040a0: 3d0a 2020 2020 2020 2020 2020 2020 5c6d  =.            \m
+000040b0: 6174 6872 6d7b 7472 7d28 5c74 696c 6465  athrm{tr}(\tilde
+000040c0: 7b42 7d5f 5c61 6c70 6861 285c 6f6d 6567  {B}_\alpha(\omeg
+000040d0: 6129 2043 5f6b 292e 0a0a 2020 2020 4475  a) C_k)...    Du
+000040e0: 6520 746f 2064 6966 6665 7265 6e63 6573  e to differences
+000040f0: 2069 6e20 696d 706c 656d 656e 7461 7469   in implementati
+00004100: 6f6e 2028 666f 7220 7065 7266 6f72 6d61  on (for performa
+00004110: 6e63 6520 7265 6173 6f6e 7329 2c20 7468  nce reasons), th
+00004120: 650a 2020 2020 6178 6573 206f 6620 7468  e.    axes of th
+00004130: 6520 7265 7375 6c74 2061 7265 2074 7261  e result are tra
+00004140: 6e73 706f 7365 6420 636f 6d70 6172 6564  nsposed compared
+00004150: 2074 6f20 7468 6520 636f 6e74 726f 6c20   to the control 
+00004160: 6d61 7472 6978 3a0a 0a20 2020 203e 3e3e  matrix:..    >>>
+00004170: 2063 7472 6c6d 6174 203d 2063 616c 6375   ctrlmat = calcu
+00004180: 6c61 7465 5f63 6f6e 7472 6f6c 5f6d 6174  late_control_mat
+00004190: 7269 785f 6672 6f6d 5f61 746f 6d69 6328  rix_from_atomic(
+000041a0: 2e2e 2e29 0a20 2020 203e 3e3e 2063 7472  ...).    >>> ctr
+000041b0: 6c6d 6174 2e73 6861 7065 0a20 2020 2028  lmat.shape.    (
+000041c0: 6e5f 6e6f 7073 2c20 642a 2a32 2c20 6e5f  n_nops, d**2, n_
+000041d0: 6f6d 6567 6129 0a20 2020 203e 3e3e 206e  omega).    >>> n
+000041e0: 6f69 7365 6f70 7320 3d20 6361 6c63 756c  oiseops = calcul
+000041f0: 6174 655f 6e6f 6973 655f 6f70 6572 6174  ate_noise_operat
+00004200: 6f72 735f 6672 6f6d 5f61 746f 6d69 6328  ors_from_atomic(
+00004210: 2e2e 2e29 0a20 2020 203e 3e3e 206e 6f69  ...).    >>> noi
+00004220: 7365 6f70 732e 7368 6170 650a 2020 2020  seops.shape.    
+00004230: 286e 5f6f 6d65 6761 2c20 6e5f 6e6f 7073  (n_omega, n_nops
+00004240: 2c20 642c 2064 290a 2020 2020 3e3e 3e20  , d, d).    >>> 
+00004250: 6374 726c 6d61 745f 6672 6f6d 5f6e 6f69  ctrlmat_from_noi
+00004260: 7365 6f70 7320 3d20 6666 2e62 6173 6973  seops = ff.basis
+00004270: 2e65 7870 616e 6428 6e6f 6973 656f 7073  .expand(noiseops
+00004280: 2c20 6261 7369 7329 0a20 2020 203e 3e3e  , basis).    >>>
+00004290: 206e 702e 616c 6c63 6c6f 7365 2863 7472   np.allclose(ctr
+000042a0: 6c6d 6174 2c20 6374 726c 6d61 745f 6672  lmat, ctrlmat_fr
+000042b0: 6f6d 5f6e 6f69 7365 6f70 732e 7472 616e  om_noiseops.tran
+000042c0: 7370 6f73 6528 312c 2032 2c20 3029 290a  spose(1, 2, 0)).
+000042d0: 2020 2020 5472 7565 0a0a 2020 2020 5365      True..    Se
+000042e0: 6520 416c 736f 0a20 2020 202d 2d2d 2d2d  e Also.    -----
+000042f0: 2d2d 2d0a 2020 2020 6361 6c63 756c 6174  ---.    calculat
+00004300: 655f 6e6f 6973 655f 6f70 6572 6174 6f72  e_noise_operator
+00004310: 735f 6672 6f6d 5f73 6372 6174 6368 3a20  s_from_scratch: 
+00004320: 436f 6d70 7574 6520 7468 6520 6f70 6572  Compute the oper
+00004330: 6174 6f72 7320 6672 6f6d 2073 6372 6174  ators from scrat
+00004340: 6368 2e0a 2020 2020 6361 6c63 756c 6174  ch..    calculat
+00004350: 655f 636f 6e74 726f 6c5f 6d61 7472 6978  e_control_matrix
+00004360: 5f66 726f 6d5f 6174 6f6d 6963 3a20 5361  _from_atomic: Sa
+00004370: 6d65 2063 616c 6375 6c61 7469 6f6e 2069  me calculation i
+00004380: 6e20 4c69 6f75 7669 6c6c 6520 7370 6163  n Liouville spac
+00004390: 652e 0a20 2020 2022 2222 0a20 2020 206e  e..    """.    n
+000043a0: 203d 206c 656e 286e 6f69 7365 5f6f 7065   = len(noise_ope
+000043b0: 7261 746f 7273 5f61 746f 6d69 6329 0a20  rators_atomic). 
+000043c0: 2020 2023 2041 6c6c 6f63 6174 6520 6d65     # Allocate me
+000043d0: 6d6f 7279 0a20 2020 206e 6f69 7365 5f6f  mory.    noise_o
+000043e0: 7065 7261 746f 7273 203d 206e 702e 7a65  perators = np.ze
+000043f0: 726f 7328 6e6f 6973 655f 6f70 6572 6174  ros(noise_operat
+00004400: 6f72 735f 6174 6f6d 6963 2e73 6861 7065  ors_atomic.shape
+00004410: 5b31 3a5d 2c20 6474 7970 653d 636f 6d70  [1:], dtype=comp
+00004420: 6c65 7829 0a0a 2020 2020 6578 7072 203d  lex)..    expr =
+00004430: 206f 652e 636f 6e74 7261 6374 5f65 7870   oe.contract_exp
+00004440: 7265 7373 696f 6e28 276a 692c 2e2e 2e6a  ression('ji,...j
+00004450: 6b2c 6b6c 2d3e 2e2e 2e69 6c27 2c0a 2020  k,kl->...il',.  
+00004460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004480: 7072 6f70 6167 6174 6f72 732e 7368 6170  propagators.shap
+00004490: 655b 313a 5d2c 206e 6f69 7365 5f6f 7065  e[1:], noise_ope
+000044a0: 7261 746f 7273 5f61 746f 6d69 632e 7368  rators_atomic.sh
+000044b0: 6170 655b 313a 5d2c 0a20 2020 2020 2020  ape[1:],.       
+000044c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000044d0: 2020 2020 2020 2020 2020 2070 726f 7061             propa
+000044e0: 6761 746f 7273 2e73 6861 7065 5b31 3a5d  gators.shape[1:]
+000044f0: 2c20 6f70 7469 6d69 7a65 3d5b 2830 2c20  , optimize=[(0, 
+00004500: 3129 2c20 2830 2c20 3129 5d29 0a0a 2020  1), (0, 1)])..  
+00004510: 2020 666f 7220 6720 696e 2075 7469 6c2e    for g in util.
+00004520: 7072 6f67 7265 7373 6261 725f 7261 6e67  progressbar_rang
+00004530: 6528 6e2c 2073 686f 775f 7072 6f67 7265  e(n, show_progre
+00004540: 7373 6261 723d 7368 6f77 5f70 726f 6772  ssbar=show_progr
+00004550: 6573 7362 6172 2c0a 2020 2020 2020 2020  essbar,.        
+00004560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004570: 2020 2020 2020 2020 2020 2020 6465 7363              desc
+00004580: 3d27 4361 6c63 756c 6174 696e 6720 6e6f  ='Calculating no
+00004590: 6973 6520 6f70 6572 6174 6f72 7327 293a  ise operators'):
+000045a0: 0a20 2020 2020 2020 206e 6f69 7365 5f6f  .        noise_o
+000045b0: 7065 7261 746f 7273 202b 3d20 6578 7072  perators += expr
+000045c0: 2870 726f 7061 6761 746f 7273 5b67 5d2e  (propagators[g].
+000045d0: 636f 6e6a 2829 2c0a 2020 2020 2020 2020  conj(),.        
+000045e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000045f0: 2020 2020 2020 2020 6e6f 6973 655f 6f70          noise_op
+00004600: 6572 6174 6f72 735f 6174 6f6d 6963 5b67  erators_atomic[g
+00004610: 5d2a 7068 6173 6573 5b67 2c20 3a2c 204e  ]*phases[g, :, N
+00004620: 6f6e 652c 204e 6f6e 652c 204e 6f6e 655d  one, None, None]
+00004630: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00004640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004650: 2020 7072 6f70 6167 6174 6f72 735b 675d    propagators[g]
+00004660: 290a 0a20 2020 2072 6574 7572 6e20 6e6f  )..    return no
+00004670: 6973 655f 6f70 6572 6174 6f72 730a 0a0a  ise_operators...
+00004680: 6465 6620 6361 6c63 756c 6174 655f 6e6f  def calculate_no
+00004690: 6973 655f 6f70 6572 6174 6f72 735f 6672  ise_operators_fr
+000046a0: 6f6d 5f73 6372 6174 6368 280a 2020 2020  om_scratch(.    
+000046b0: 2020 2020 6569 6776 616c 733a 206e 6461      eigvals: nda
+000046c0: 7272 6179 2c0a 2020 2020 2020 2020 6569  rray,.        ei
+000046d0: 6776 6563 733a 206e 6461 7272 6179 2c0a  gvecs: ndarray,.
+000046e0: 2020 2020 2020 2020 7072 6f70 6167 6174          propagat
+000046f0: 6f72 733a 206e 6461 7272 6179 2c0a 2020  ors: ndarray,.  
+00004700: 2020 2020 2020 6f6d 6567 613a 2043 6f65        omega: Coe
+00004710: 6666 6963 6965 6e74 732c 0a20 2020 2020  fficients,.     
+00004720: 2020 206e 5f6f 7065 7273 3a20 5365 7175     n_opers: Sequ
+00004730: 656e 6365 5b4f 7065 7261 746f 725d 2c0a  ence[Operator],.
+00004740: 2020 2020 2020 2020 6e5f 636f 6566 6673          n_coeffs
+00004750: 3a20 5365 7175 656e 6365 5b43 6f65 6666  : Sequence[Coeff
+00004760: 6963 6965 6e74 735d 2c0a 2020 2020 2020  icients],.      
+00004770: 2020 6474 3a20 436f 6566 6669 6369 656e    dt: Coefficien
+00004780: 7473 2c0a 2020 2020 2020 2020 743a 204f  ts,.        t: O
+00004790: 7074 696f 6e61 6c5b 436f 6566 6669 6369  ptional[Coeffici
+000047a0: 656e 7473 5d20 3d20 4e6f 6e65 2c0a 2020  ents] = None,.  
+000047b0: 2020 2020 2020 7368 6f77 5f70 726f 6772        show_progr
+000047c0: 6573 7362 6172 3a20 626f 6f6c 203d 2046  essbar: bool = F
+000047d0: 616c 7365 2c0a 2020 2020 2020 2020 6361  alse,.        ca
+000047e0: 6368 655f 696e 7465 726d 6564 6961 7465  che_intermediate
+000047f0: 733a 2062 6f6f 6c20 3d20 4661 6c73 650a  s: bool = False.
+00004800: 2920 2d3e 2055 6e69 6f6e 5b6e 6461 7272  ) -> Union[ndarr
+00004810: 6179 2c20 5475 706c 655b 6e64 6172 7261  ay, Tuple[ndarra
+00004820: 792c 2044 6963 745b 7374 722c 206e 6461  y, Dict[str, nda
+00004830: 7272 6179 5d5d 5d3a 0a20 2020 2072 2222  rray]]]:.    r""
+00004840: 220a 2020 2020 4361 6c63 756c 6174 6520  ".    Calculate 
+00004850: 7468 6520 6e6f 6973 6520 6f70 6572 6174  the noise operat
+00004860: 6f72 7320 696e 2069 6e74 6572 6163 7469  ors in interacti
+00004870: 6f6e 2070 6963 7475 7265 2066 726f 6d20  on picture from 
+00004880: 7363 7261 7463 682e 0a0a 2020 2020 5061  scratch...    Pa
+00004890: 7261 6d65 7465 7273 0a20 2020 202d 2d2d  rameters.    ---
+000048a0: 2d2d 2d2d 2d2d 2d0a 2020 2020 6569 6776  -------.    eigv
+000048b0: 616c 733a 2061 7272 6179 5f6c 696b 652c  als: array_like,
+000048c0: 2073 6861 7065 2028 6e5f 6474 2c20 6429   shape (n_dt, d)
+000048d0: 0a20 2020 2020 2020 2045 6967 656e 7661  .        Eigenva
+000048e0: 6c75 6520 7665 6374 6f72 7320 666f 7220  lue vectors for 
+000048f0: 6561 6368 2074 696d 6520 7075 6c73 6520  each time pulse 
+00004900: 7365 676d 656e 7420 2a67 2a20 7769 7468  segment *g* with
+00004910: 2074 6865 0a20 2020 2020 2020 2066 6972   the.        fir
+00004920: 7374 2061 7869 7320 636f 756e 7469 6e67  st axis counting
+00004930: 2074 6865 2070 756c 7365 2073 6567 6d65   the pulse segme
+00004940: 6e74 2c20 692e 652e 0a20 2020 2020 2020  nt, i.e..       
+00004950: 2060 6065 6967 7661 6c73 203d 3d20 6172   ``eigvals == ar
+00004960: 7261 7928 5b44 5f30 2c20 445f 312c 202e  ray([D_0, D_1, .
+00004970: 2e2e 5d29 6060 2e0a 2020 2020 6569 6776  ..])``..    eigv
+00004980: 6563 733a 2061 7272 6179 5f6c 696b 652c  ecs: array_like,
+00004990: 2073 6861 7065 2028 6e5f 6474 2c20 642c   shape (n_dt, d,
+000049a0: 2064 290a 2020 2020 2020 2020 4569 6765   d).        Eige
+000049b0: 6e76 6563 746f 7220 6d61 7472 6963 6573  nvector matrices
+000049c0: 2066 6f72 2065 6163 6820 7469 6d65 2070   for each time p
+000049d0: 756c 7365 2073 6567 6d65 6e74 202a 672a  ulse segment *g*
+000049e0: 2077 6974 6820 7468 650a 2020 2020 2020   with the.      
+000049f0: 2020 6669 7273 7420 6178 6973 2063 6f75    first axis cou
+00004a00: 6e74 696e 6720 7468 6520 7075 6c73 6520  nting the pulse 
+00004a10: 7365 676d 656e 742c 2069 2e65 2e0a 2020  segment, i.e..  
+00004a20: 2020 2020 2020 6060 6569 6776 6563 7320        ``eigvecs 
+00004a30: 3d3d 2061 7272 6179 285b 565f 302c 2056  == array([V_0, V
+00004a40: 5f31 2c20 2e2e 2e5d 2960 602e 0a20 2020  _1, ...])``..   
+00004a50: 2070 726f 7061 6761 746f 7273 3a20 6172   propagators: ar
+00004a60: 7261 795f 6c69 6b65 2c20 7368 6170 6520  ray_like, shape 
+00004a70: 286e 5f64 742b 312c 2064 2c20 6429 0a20  (n_dt+1, d, d). 
+00004a80: 2020 2020 2020 2054 6865 2070 726f 7061         The propa
+00004a90: 6761 746f 7273 203a 6d61 7468 3a60 515f  gators :math:`Q_
+00004aa0: 6720 3d20 505f 6720 505f 7b67 2d31 7d5c  g = P_g P_{g-1}\
+00004ab0: 6364 6f74 7320 505f 3060 2061 7320 6120  cdots P_0` as a 
+00004ac0: 2864 2c20 6429 0a20 2020 2020 2020 2061  (d, d).        a
+00004ad0: 7272 6179 2077 6974 6820 2a64 2a20 7468  rray with *d* th
+00004ae0: 6520 6469 6d65 6e73 696f 6e20 6f66 2074  e dimension of t
+00004af0: 6865 2048 696c 6265 7274 2073 7061 6365  he Hilbert space
+00004b00: 2e0a 2020 2020 6f6d 6567 613a 2061 7272  ..    omega: arr
+00004b10: 6179 5f6c 696b 652c 2073 6861 7065 2028  ay_like, shape (
+00004b20: 6e5f 6f6d 6567 612c 290a 2020 2020 2020  n_omega,).      
+00004b30: 2020 4672 6571 7565 6e63 6965 7320 6174    Frequencies at
+00004b40: 2077 6869 6368 2074 6865 2070 756c 7365   which the pulse
+00004b50: 2063 6f6e 7472 6f6c 206d 6174 7269 7820   control matrix 
+00004b60: 6973 2074 6f20 6265 0a20 2020 2020 2020  is to be.       
+00004b70: 2065 7661 6c75 6174 6564 2e0a 2020 2020   evaluated..    
+00004b80: 6e5f 6f70 6572 733a 2061 7272 6179 5f6c  n_opers: array_l
+00004b90: 696b 652c 2073 6861 7065 2028 6e5f 6e6f  ike, shape (n_no
+00004ba0: 7073 2c20 642c 2064 290a 2020 2020 2020  ps, d, d).      
+00004bb0: 2020 4e6f 6973 6520 6f70 6572 6174 6f72    Noise operator
+00004bc0: 7320 3a6d 6174 683a 6042 5f5c 616c 7068  s :math:`B_\alph
+00004bd0: 6160 2e0a 2020 2020 6e5f 636f 6566 6673  a`..    n_coeffs
+00004be0: 3a20 6172 7261 795f 6c69 6b65 2c20 7368  : array_like, sh
+00004bf0: 6170 6520 286e 5f6e 6f70 732c 206e 5f64  ape (n_nops, n_d
+00004c00: 7429 0a20 2020 2020 2020 2054 6865 2073  t).        The s
+00004c10: 656e 7369 7469 7669 7469 6573 206f 6620  ensitivities of 
+00004c20: 7468 6520 7379 7374 656d 2074 6f20 7468  the system to th
+00004c30: 6520 6e6f 6973 6520 6f70 6572 6174 6f72  e noise operator
+00004c40: 7320 6769 7665 6e20 6279 0a20 2020 2020  s given by.     
+00004c50: 2020 202a 6e5f 6f70 6572 732a 2061 7420     *n_opers* at 
+00004c60: 7468 6520 6769 7665 6e20 7469 6d65 2073  the given time s
+00004c70: 7465 702e 0a20 2020 2064 743a 2061 7272  tep..    dt: arr
+00004c80: 6179 5f6c 696b 652c 2073 6861 7065 2028  ay_like, shape (
+00004c90: 6e5f 6474 290a 2020 2020 2020 2020 5365  n_dt).        Se
+00004ca0: 7175 656e 6365 2064 7572 6174 696f 6e2c  quence duration,
+00004cb0: 2069 2e65 2e20 666f 7220 7468 6520 3a6d   i.e. for the :m
+00004cc0: 6174 683a 6067 602d 7468 2070 756c 7365  ath:`g`-th pulse
+00004cd0: 0a20 2020 2020 2020 203a 6d61 7468 3a60  .        :math:`
+00004ce0: 745f 6720 2d20 745f 7b67 2d31 7d60 2e0a  t_g - t_{g-1}`..
+00004cf0: 2020 2020 743a 2061 7272 6179 5f6c 696b      t: array_lik
+00004d00: 652c 2073 6861 7065 2028 6e5f 6474 2b31  e, shape (n_dt+1
+00004d10: 292c 206f 7074 696f 6e61 6c0a 2020 2020  ), optional.    
+00004d20: 2020 2020 5468 6520 6162 736f 6c75 7465      The absolute
+00004d30: 2074 696d 6573 206f 6620 7468 6520 6469   times of the di
+00004d40: 6666 6572 656e 7420 7365 676d 656e 7473  fferent segments
+00004d50: 2e20 4361 6e20 616c 736f 2062 650a 2020  . Can also be.  
+00004d60: 2020 2020 2020 636f 6d70 7574 6564 2066        computed f
+00004d70: 726f 6d20 2a64 742a 2e0a 2020 2020 7368  rom *dt*..    sh
+00004d80: 6f77 5f70 726f 6772 6573 7362 6172 3a20  ow_progressbar: 
+00004d90: 626f 6f6c 2c20 6f70 7469 6f6e 616c 0a20  bool, optional. 
+00004da0: 2020 2020 2020 2053 686f 7720 6120 7072         Show a pr
+00004db0: 6f67 7265 7373 2062 6172 2066 6f72 2074  ogress bar for t
+00004dc0: 6865 2063 616c 6375 6c61 7469 6f6e 2e0a  he calculation..
+00004dd0: 2020 2020 6361 6368 655f 696e 7465 726d      cache_interm
+00004de0: 6564 6961 7465 733a 2062 6f6f 6c2c 206f  ediates: bool, o
+00004df0: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
+00004e00: 4b65 6570 2061 6e64 2072 6574 7572 6e20  Keep and return 
+00004e10: 696e 7465 726d 6564 6961 7465 2074 6572  intermediate ter
+00004e20: 6d73 206f 6620 7468 6520 6361 6c63 756c  ms of the calcul
+00004e30: 6174 696f 6e20 7468 6174 2063 616e 0a20  ation that can. 
+00004e40: 2020 2020 2020 2062 6520 7265 7573 6564         be reused
+00004e50: 2069 6e20 6f74 6865 7220 636f 6d70 7574   in other comput
+00004e60: 6174 696f 6e73 2028 7365 636f 6e64 206f  ations (second o
+00004e70: 7264 6572 206f 7220 6772 6164 6965 6e74  rder or gradient
+00004e80: 7329 2e0a 2020 2020 2020 2020 4f74 6865  s)..        Othe
+00004e90: 7277 6973 6520 7468 6520 7375 6d20 6973  rwise the sum is
+00004ea0: 2070 6572 666f 726d 6564 2069 6e2d 706c   performed in-pl
+00004eb0: 6163 652e 2054 6865 2064 6566 6175 6c74  ace. The default
+00004ec0: 2069 7320 4661 6c73 652e 0a0a 2020 2020   is False...    
+00004ed0: 5265 7475 726e 730a 2020 2020 2d2d 2d2d  Returns.    ----
+00004ee0: 2d2d 2d0a 2020 2020 6e6f 6973 655f 6f70  ---.    noise_op
+00004ef0: 6572 6174 6f72 733a 206e 6461 7272 6179  erators: ndarray
+00004f00: 2c20 7368 6170 6520 286e 5f6f 6d65 6761  , shape (n_omega
+00004f10: 2c20 6e5f 6e6f 7073 2c20 642c 2064 290a  , n_nops, d, d).
+00004f20: 2020 2020 2020 2020 5468 6520 696e 7465          The inte
+00004f30: 7261 6374 696f 6e20 7069 6374 7572 6520  raction picture 
+00004f40: 6e6f 6973 6520 6f70 6572 6174 6f72 730a  noise operators.
+00004f50: 2020 2020 2020 2020 3a6d 6174 683a 605c          :math:`\
+00004f60: 7469 6c64 657b 427d 5f5c 616c 7068 6128  tilde{B}_\alpha(
+00004f70: 5c6f 6d65 6761 2960 2e0a 2020 2020 696e  \omega)`..    in
+00004f80: 7465 726d 6564 6961 7465 733a 2064 6963  termediates: dic
+00004f90: 745b 7374 722c 206e 6461 7272 6179 5d0a  t[str, ndarray].
+00004fa0: 2020 2020 2020 2020 496e 7465 726d 6564          Intermed
+00004fb0: 6961 7465 2072 6573 756c 7473 206f 6620  iate results of 
+00004fc0: 7468 6520 6361 6c63 756c 6174 696f 6e2e  the calculation.
+00004fd0: 204f 6e6c 7920 6966 0a20 2020 2020 2020   Only if.       
+00004fe0: 2063 6163 6865 5f69 6e74 6572 6d65 6469   cache_intermedi
+00004ff0: 6174 6573 2069 7320 5472 7565 2e0a 0a20  ates is True... 
+00005000: 2020 204e 6f74 6573 0a20 2020 202d 2d2d     Notes.    ---
+00005010: 2d2d 0a20 2020 2054 6865 2069 6e74 6572  --.    The inter
+00005020: 6163 7469 6f6e 2070 6963 7475 7265 206e  action picture n
+00005030: 6f69 7365 206f 7065 7261 746f 7273 2061  oise operators a
+00005040: 7265 2063 616c 6375 6c61 7465 6420 6163  re calculated ac
+00005050: 636f 7264 696e 6720 746f 0a0a 2020 2020  cording to..    
+00005060: 2e2e 206d 6174 683a 3a0a 0a20 2020 2020  .. math::..     
+00005070: 2020 205c 7469 6c64 657b 427d 5f5c 616c     \tilde{B}_\al
+00005080: 7068 6128 5c6f 6d65 6761 2920 3d20 5c73  pha(\omega) = \s
+00005090: 756d 5f7b 673d 317d 5e47 2065 5e7b 695c  um_{g=1}^G e^{i\
+000050a0: 6f6d 6567 6120 745f 7b67 2d31 7d7d 0a20  omega t_{g-1}}. 
+000050b0: 2020 2020 2020 2020 2020 2073 5f5c 616c             s_\al
+000050c0: 7068 615e 7b28 6729 7d20 505e 7b28 6729  pha^{(g)} P^{(g)
+000050d0: 5c64 6167 6765 727d 5c6c 6566 745b 0a20  \dagger}\left[. 
+000050e0: 2020 2020 2020 2020 2020 2020 2020 205c                 \
+000050f0: 6261 727b 427d 5e7b 2867 297d 5f5c 616c  bar{B}^{(g)}_\al
+00005100: 7068 6120 5c63 6972 6320 495e 7b28 6729  pha \circ I^{(g)
+00005110: 7d28 5c6f 6d65 6761 290a 2020 2020 2020  }(\omega).      
+00005120: 2020 2020 2020 5c72 6967 6874 5d20 505e        \right] P^
+00005130: 7b28 6729 7d0a 0a20 2020 2077 6865 7265  {(g)}..    where
+00005140: 0a0a 2020 2020 2e2e 206d 6174 683a 3a0a  ..    .. math::.
+00005150: 0a20 2020 2020 2020 2049 5e7b 2867 297d  .        I^{(g)}
+00005160: 5f7b 6e6d 7d28 5c6f 6d65 6761 2920 263d  _{nm}(\omega) &=
+00005170: 205c 696e 745f 305e 7b74 5f67 202d 2074   \int_0^{t_g - t
+00005180: 5f7b 672d 317d 7d5c 6d61 7468 726d 7b64  _{g-1}}\mathrm{d
+00005190: 7d74 5c2c 0a20 2020 2020 2020 2020 2020  }t\,.           
+000051a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000051b0: 2020 2020 2065 5e7b 6928 5c6f 6d65 6761       e^{i(\omega
+000051c0: 2b5c 6f6d 6567 615f 6e2d 5c6f 6d65 6761  +\omega_n-\omega
+000051d0: 5f6d 2974 7d20 5c5c 0a20 2020 2020 2020  _m)t} \\.       
+000051e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000051f0: 2020 2020 2020 263d 205c 6672 6163 7b65        &= \frac{e
+00005200: 5e7b 6928 5c6f 6d65 6761 2b5c 6f6d 6567  ^{i(\omega+\omeg
+00005210: 615f 6e2d 5c6f 6d65 6761 5f6d 290a 2020  a_n-\omega_m).  
+00005220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005230: 2020 2020 2020 2020 2020 2020 2020 2874                (t
+00005240: 5f67 202d 2074 5f7b 672d 317d 297d 202d  _g - t_{g-1})} -
+00005250: 2031 7d0a 2020 2020 2020 2020 2020 2020   1}.            
+00005260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005270: 2020 2020 7b69 285c 6f6d 6567 612b 5c6f      {i(\omega+\o
+00005280: 6d65 6761 5f6e 2d5c 6f6d 6567 615f 6d29  mega_n-\omega_m)
+00005290: 7d2c 205c 5c0a 2020 2020 2020 2020 5c62  }, \\.        \b
+000052a0: 6172 7b42 7d5f 5c61 6c70 6861 5e7b 2867  ar{B}_\alpha^{(g
+000052b0: 297d 2026 3d20 565e 7b28 6729 5c64 6167  )} &= V^{(g)\dag
+000052c0: 6765 727d 2042 5f5c 616c 7068 6120 565e  ger} B_\alpha V^
+000052d0: 7b28 6729 7d2c 205c 5c0a 2020 2020 2020  {(g)}, \\.      
+000052e0: 2020 505e 7b28 6729 7d20 263d 2056 5e7b    P^{(g)} &= V^{
+000052f0: 2867 295c 6461 6767 6572 7d20 515f 7b67  (g)\dagger} Q_{g
+00005300: 2d31 7d2c 0a0a 2020 2020 616e 6420 3a6d  -1},..    and :m
+00005310: 6174 683a 6056 5e7b 2867 297d 6020 6973  ath:`V^{(g)}` is
+00005320: 2074 6865 206d 6174 7269 7820 6f66 2065   the matrix of e
+00005330: 6967 656e 7665 6374 6f72 7320 7468 6174  igenvectors that
+00005340: 2064 6961 676f 6e61 6c69 7a65 730a 2020   diagonalizes.  
+00005350: 2020 3a6d 6174 683a 605c 7469 6c64 657b    :math:`\tilde{
+00005360: 5c6d 6174 6863 616c 7b48 7d7d 5f6e 5e7b  \mathcal{H}}_n^{
+00005370: 2867 297d 602c 203a 6d61 7468 3a60 425f  (g)}`, :math:`B_
+00005380: 5c61 6c70 6861 6020 7468 650a 2020 2020  \alpha` the.    
+00005390: 3a6d 6174 683a 605c 616c 7068 6160 2d74  :math:`\alpha`-t
+000053a0: 6820 6e6f 6973 6520 6f70 6572 6174 6f72  h noise operator
+000053b0: 2c20 616e 6420 203a 6d61 7468 3a60 735f  , and  :math:`s_
+000053c0: 5c61 6c70 6861 5e7b 2867 297d 6020 7468  \alpha^{(g)}` th
+000053d0: 650a 2020 2020 6e6f 6973 6520 7365 6e73  e.    noise sens
+000053e0: 6974 6976 6974 7920 6475 7269 6e67 2069  itivity during i
+000053f0: 6e74 6572 7661 6c20 3a6d 6174 683a 6067  nterval :math:`g
+00005400: 602e 0a0a 2020 2020 5468 6520 636f 6e74  `...    The cont
+00005410: 726f 6c20 6d61 7472 6978 2074 6865 6e20  rol matrix then 
+00005420: 636f 7272 6573 706f 6e64 7320 746f 2074  corresponds to t
+00005430: 6865 2063 6f65 6666 6963 6965 6e74 7320  he coefficients 
+00005440: 6f66 2065 7870 616e 7369 6f6e 0a20 2020  of expansion.   
+00005450: 2069 6e20 616e 206f 7065 7261 746f 7220   in an operator 
+00005460: 6261 7369 7320 3a6d 6174 683a 605c 7b43  basis :math:`\{C
+00005470: 5f6b 5c7d 5f6b 603a 0a0a 2020 2020 2e2e  _k\}_k`:..    ..
+00005480: 206d 6174 683a 3a0a 2020 2020 2020 2020   math::.        
+00005490: 5c74 696c 6465 7b5c 6d61 7468 6361 6c7b  \tilde{\mathcal{
+000054a0: 427d 7d5f 7b6b 5c61 6c70 6861 7d28 5c6f  B}}_{k\alpha}(\o
+000054b0: 6d65 6761 2920 3d0a 2020 2020 2020 2020  mega) =.        
+000054c0: 2020 2020 5c6d 6174 6872 6d7b 7472 7d28      \mathrm{tr}(
+000054d0: 5c74 696c 6465 7b42 7d5f 5c61 6c70 6861  \tilde{B}_\alpha
+000054e0: 285c 6f6d 6567 6129 2043 5f6b 292e 0a0a  (\omega) C_k)...
+000054f0: 2020 2020 4475 6520 746f 2064 6966 6665      Due to diffe
+00005500: 7265 6e63 6573 2069 6e20 696d 706c 656d  rences in implem
+00005510: 656e 7461 7469 6f6e 2028 666f 7220 7065  entation (for pe
+00005520: 7266 6f72 6d61 6e63 6520 7265 6173 6f6e  rformance reason
+00005530: 7329 2c20 7468 650a 2020 2020 6178 6573  s), the.    axes
+00005540: 206f 6620 7468 6520 7265 7375 6c74 2061   of the result a
+00005550: 7265 2074 7261 6e73 706f 7365 6420 636f  re transposed co
+00005560: 6d70 6172 6564 2074 6f20 7468 6520 636f  mpared to the co
+00005570: 6e74 726f 6c20 6d61 7472 6978 3a0a 0a20  ntrol matrix:.. 
+00005580: 2020 203e 3e3e 2063 7472 6c6d 6174 203d     >>> ctrlmat =
+00005590: 2063 616c 6375 6c61 7465 5f63 6f6e 7472   calculate_contr
+000055a0: 6f6c 5f6d 6174 7269 785f 6672 6f6d 5f73  ol_matrix_from_s
+000055b0: 6372 6174 6368 282e 2e2e 290a 2020 2020  cratch(...).    
+000055c0: 3e3e 3e20 6374 726c 6d61 742e 7368 6170  >>> ctrlmat.shap
+000055d0: 650a 2020 2020 286e 5f6e 6f70 732c 2064  e.    (n_nops, d
+000055e0: 2a2a 322c 206e 5f6f 6d65 6761 290a 2020  **2, n_omega).  
+000055f0: 2020 3e3e 3e20 6e6f 6973 656f 7073 203d    >>> noiseops =
+00005600: 2063 616c 6375 6c61 7465 5f6e 6f69 7365   calculate_noise
+00005610: 5f6f 7065 7261 746f 7273 5f66 726f 6d5f  _operators_from_
+00005620: 7363 7261 7463 6828 2e2e 2e29 0a20 2020  scratch(...).   
+00005630: 203e 3e3e 206e 6f69 7365 6f70 732e 7368   >>> noiseops.sh
+00005640: 6170 650a 2020 2020 286e 5f6f 6d65 6761  ape.    (n_omega
+00005650: 2c20 6e5f 6e6f 7073 2c20 642c 2064 290a  , n_nops, d, d).
+00005660: 2020 2020 3e3e 3e20 6374 726c 6d61 745f      >>> ctrlmat_
+00005670: 6672 6f6d 5f6e 6f69 7365 6f70 7320 3d20  from_noiseops = 
+00005680: 6666 2e62 6173 6973 2e65 7870 616e 6428  ff.basis.expand(
+00005690: 6e6f 6973 656f 7073 2c20 6261 7369 7329  noiseops, basis)
+000056a0: 0a20 2020 203e 3e3e 206e 702e 616c 6c63  .    >>> np.allc
+000056b0: 6c6f 7365 2863 7472 6c6d 6174 2c20 6374  lose(ctrlmat, ct
+000056c0: 726c 6d61 745f 6672 6f6d 5f6e 6f69 7365  rlmat_from_noise
+000056d0: 6f70 732e 7472 616e 7370 6f73 6528 312c  ops.transpose(1,
+000056e0: 2032 2c20 3029 290a 2020 2020 5472 7565   2, 0)).    True
+000056f0: 0a0a 2020 2020 5365 6520 416c 736f 0a20  ..    See Also. 
+00005700: 2020 202d 2d2d 2d2d 2d2d 2d0a 2020 2020     --------.    
+00005710: 6361 6c63 756c 6174 655f 6e6f 6973 655f  calculate_noise_
+00005720: 6f70 6572 6174 6f72 735f 6672 6f6d 5f61  operators_from_a
+00005730: 746f 6d69 633a 2043 6f6d 7075 7465 2074  tomic: Compute t
+00005740: 6865 206f 7065 7261 746f 7273 2066 726f  he operators fro
+00005750: 6d20 6174 6f6d 6963 2073 6567 6d65 6e74  m atomic segment
+00005760: 732e 0a20 2020 2063 616c 6375 6c61 7465  s..    calculate
+00005770: 5f63 6f6e 7472 6f6c 5f6d 6174 7269 785f  _control_matrix_
+00005780: 6672 6f6d 5f73 6372 6174 6368 3a20 5361  from_scratch: Sa
+00005790: 6d65 2063 616c 6375 6c61 7469 6f6e 2069  me calculation i
+000057a0: 6e20 4c69 6f75 7669 6c6c 6520 7370 6163  n Liouville spac
+000057b0: 652e 0a20 2020 2022 2222 0a20 2020 2069  e..    """.    i
+000057c0: 6620 7420 6973 204e 6f6e 653a 0a20 2020  f t is None:.   
+000057d0: 2020 2020 2074 203d 206e 702e 636f 6e63       t = np.conc
+000057e0: 6174 656e 6174 6528 285b 305d 2c20 6e70  atenate(([0], np
+000057f0: 2e61 7361 7272 6179 2864 7429 2e63 756d  .asarray(dt).cum
+00005800: 7375 6d28 2929 290a 0a20 2020 2064 203d  sum()))..    d =
+00005810: 2065 6967 7665 6373 2e73 6861 7065 5b2d   eigvecs.shape[-
+00005820: 315d 0a20 2020 206e 5f63 6f65 6666 7320  1].    n_coeffs 
+00005830: 3d20 6e70 2e61 7361 7272 6179 286e 5f63  = np.asarray(n_c
+00005840: 6f65 6666 7329 0a0a 2020 2020 2320 5072  oeffs)..    # Pr
+00005850: 6563 6f6d 7075 7465 206e 6f69 7365 206f  ecompute noise o
+00005860: 7065 7273 2074 7261 6e73 666f 726d 6564  pers transformed
+00005870: 2074 6f20 6569 6765 6e62 6173 6973 206f   to eigenbasis o
+00005880: 6620 6561 6368 2070 756c 7365 0a20 2020  f each pulse.   
+00005890: 2023 2073 6567 6d65 6e74 2061 6e64 2056   # segment and V
+000058a0: 5e5c 6461 6767 6572 2040 2051 0a20 2020  ^\dagger @ Q.   
+000058b0: 2065 6967 7665 6373 5f70 726f 7061 6761   eigvecs_propaga
+000058c0: 7465 6420 3d20 5f70 726f 7061 6761 7465  ted = _propagate
+000058d0: 5f65 6967 656e 7665 6374 6f72 7328 6569  _eigenvectors(ei
+000058e0: 6776 6563 732c 2070 726f 7061 6761 746f  gvecs, propagato
+000058f0: 7273 5b3a 2d31 5d29 0a20 2020 206e 5f6f  rs[:-1]).    n_o
+00005900: 7065 7273 5f74 7261 6e73 666f 726d 6564  pers_transformed
+00005910: 203d 205f 7472 616e 7366 6f72 6d5f 6861   = _transform_ha
+00005920: 6d69 6c74 6f6e 6961 6e28 6569 6776 6563  miltonian(eigvec
+00005930: 732c 206e 5f6f 7065 7273 2c20 6e5f 636f  s, n_opers, n_co
+00005940: 6566 6673 290a 0a20 2020 2023 2041 6c6c  effs)..    # All
+00005950: 6f63 6174 6520 6d65 6d6f 7279 0a20 2020  ocate memory.   
+00005960: 2065 7870 5f62 7566 2c20 696e 745f 6275   exp_buf, int_bu
+00005970: 6620 3d20 6e70 2e65 6d70 7479 2828 322c  f = np.empty((2,
+00005980: 206c 656e 286f 6d65 6761 292c 2064 2c20   len(omega), d, 
+00005990: 6429 2c20 6474 7970 653d 636f 6d70 6c65  d), dtype=comple
+000059a0: 7829 0a20 2020 206e 6f69 7365 5f6f 7065  x).    noise_ope
+000059b0: 7261 746f 7273 203d 206e 702e 7a65 726f  rators = np.zero
+000059c0: 7328 286c 656e 286f 6d65 6761 292c 206c  s((len(omega), l
+000059d0: 656e 286e 5f6f 7065 7273 292c 2064 2c20  en(n_opers), d, 
+000059e0: 6429 2c20 6474 7970 653d 636f 6d70 6c65  d), dtype=comple
+000059f0: 7829 0a0a 2020 2020 6966 2063 6163 6865  x)..    if cache
+00005a00: 5f69 6e74 6572 6d65 6469 6174 6573 3a0a  _intermediates:.
+00005a10: 2020 2020 2020 2020 7068 6173 655f 6661          phase_fa
+00005a20: 6374 6f72 735f 6361 6368 6520 3d20 6e70  ctors_cache = np
+00005a30: 2e65 6d70 7479 2828 6c65 6e28 6474 292c  .empty((len(dt),
+00005a40: 206c 656e 286f 6d65 6761 2929 2c20 6474   len(omega)), dt
+00005a50: 7970 653d 636f 6d70 6c65 7829 0a20 2020  ype=complex).   
+00005a60: 2020 2020 2069 6e74 5f63 6163 6865 203d       int_cache =
+00005a70: 206e 702e 656d 7074 7928 286c 656e 2864   np.empty((len(d
+00005a80: 7429 2c20 6c65 6e28 6f6d 6567 6129 2c20  t), len(omega), 
+00005a90: 642c 2064 292c 2064 7479 7065 3d63 6f6d  d, d), dtype=com
+00005aa0: 706c 6578 290a 2020 2020 2020 2020 7375  plex).        su
+00005ab0: 6d5f 6361 6368 6520 3d20 6e70 2e65 6d70  m_cache = np.emp
+00005ac0: 7479 2828 6c65 6e28 6474 292c 206c 656e  ty((len(dt), len
+00005ad0: 286f 6d65 6761 292c 206c 656e 286e 5f6f  (omega), len(n_o
+00005ae0: 7065 7273 292c 2064 2c20 6429 2c20 6474  pers), d, d), dt
+00005af0: 7970 653d 636f 6d70 6c65 7829 0a20 2020  ype=complex).   
+00005b00: 2065 6c73 653a 0a20 2020 2020 2020 2070   else:.        p
+00005b10: 6861 7365 5f66 6163 746f 7273 203d 206e  hase_factors = n
+00005b20: 702e 656d 7074 7928 286c 656e 286f 6d65  p.empty((len(ome
+00005b30: 6761 292c 292c 2064 7479 7065 3d63 6f6d  ga),), dtype=com
+00005b40: 706c 6578 290a 2020 2020 2020 2020 696e  plex).        in
+00005b50: 745f 6275 6620 3d20 6e70 2e65 6d70 7479  t_buf = np.empty
+00005b60: 2828 6c65 6e28 6f6d 6567 6129 2c20 642c  ((len(omega), d,
+00005b70: 2064 292c 2064 7479 7065 3d63 6f6d 706c   d), dtype=compl
+00005b80: 6578 290a 2020 2020 2020 2020 7375 6d5f  ex).        sum_
+00005b90: 6275 6620 3d20 6e70 2e65 6d70 7479 2828  buf = np.empty((
+00005ba0: 6c65 6e28 6f6d 6567 6129 2c20 6c65 6e28  len(omega), len(
+00005bb0: 6e5f 6f70 6572 7329 2c20 642c 2064 292c  n_opers), d, d),
+00005bc0: 2064 7479 7065 3d63 6f6d 706c 6578 290a   dtype=complex).
+00005bd0: 0a20 2020 2023 2053 6574 2075 7020 7265  .    # Set up re
+00005be0: 7573 6162 6c65 2065 7870 7265 7373 696f  usable expressio
+00005bf0: 6e73 0a20 2020 2065 7870 725f 3120 3d20  ns.    expr_1 = 
+00005c00: 6f65 2e63 6f6e 7472 6163 745f 6578 7072  oe.contract_expr
+00005c10: 6573 7369 6f6e 2827 616b 6c2c 6f6b 6c2d  ession('akl,okl-
+00005c20: 3e6f 616b 6c27 2c0a 2020 2020 2020 2020  >oakl',.        
+00005c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c40: 2020 2020 2020 2020 2020 2020 6e5f 6f70              n_op
+00005c50: 6572 735f 7472 616e 7366 6f72 6d65 645b  ers_transformed[
+00005c60: 3a2c 2030 5d2e 7368 6170 652c 2069 6e74  :, 0].shape, int
+00005c70: 5f62 7566 2e73 6861 7065 290a 2020 2020  _buf.shape).    
+00005c80: 6578 7072 5f32 203d 206f 652e 636f 6e74  expr_2 = oe.cont
+00005c90: 7261 6374 5f65 7870 7265 7373 696f 6e28  ract_expression(
+00005ca0: 276a 692c 2e2e 2e6a 6b2c 6b6c 272c 0a20  'ji,...jk,kl',. 
+00005cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005cd0: 2020 2065 6967 7665 6373 5f70 726f 7061     eigvecs_propa
+00005ce0: 6761 7465 645b 305d 2e73 6861 7065 2c20  gated[0].shape, 
+00005cf0: 286c 656e 286f 6d65 6761 292c 206c 656e  (len(omega), len
+00005d00: 286e 5f6f 7065 7273 292c 2064 2c20 6429  (n_opers), d, d)
+00005d10: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00005d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d30: 2020 2020 2020 6569 6776 6563 735f 7072        eigvecs_pr
+00005d40: 6f70 6167 6174 6564 5b30 5d2e 7368 6170  opagated[0].shap
+00005d50: 652c 206f 7074 696d 697a 653d 5b28 302c  e, optimize=[(0,
+00005d60: 2031 292c 2028 302c 2031 295d 290a 0a20   1), (0, 1)]).. 
+00005d70: 2020 2066 6f72 2067 2069 6e20 7574 696c     for g in util
+00005d80: 2e70 726f 6772 6573 7362 6172 5f72 616e  .progressbar_ran
+00005d90: 6765 286c 656e 2864 7429 2c20 7368 6f77  ge(len(dt), show
+00005da0: 5f70 726f 6772 6573 7362 6172 3d73 686f  _progressbar=sho
+00005db0: 775f 7072 6f67 7265 7373 6261 722c 0a20  w_progressbar,. 
+00005dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005de0: 2020 2064 6573 633d 2743 616c 6375 6c61     desc='Calcula
+00005df0: 7469 6e67 206e 6f69 7365 206f 7065 7261  ting noise opera
+00005e00: 746f 7273 2729 3a0a 2020 2020 2020 2020  tors'):.        
+00005e10: 6966 2063 6163 6865 5f69 6e74 6572 6d65  if cache_interme
+00005e20: 6469 6174 6573 3a0a 2020 2020 2020 2020  diates:.        
+00005e30: 2020 2020 2320 4173 7369 676e 2072 6566      # Assign ref
+00005e40: 6572 656e 6365 7320 746f 2074 6865 206c  erences to the l
+00005e50: 6f63 6174 696f 6e73 2069 6e20 7468 6520  ocations in the 
+00005e60: 6361 6368 6520 666f 7220 7468 6520 7175  cache for the qu
+00005e70: 616e 7469 7469 6573 0a20 2020 2020 2020  antities.       
+00005e80: 2020 2020 2023 2074 6861 7420 7368 6f75       # that shou
+00005e90: 6c64 2062 6520 7374 6f72 6564 0a20 2020  ld be stored.   
+00005ea0: 2020 2020 2020 2020 2070 6861 7365 5f66           phase_f
+00005eb0: 6163 746f 7273 203d 2070 6861 7365 5f66  actors = phase_f
+00005ec0: 6163 746f 7273 5f63 6163 6865 5b67 5d0a  actors_cache[g].
+00005ed0: 2020 2020 2020 2020 2020 2020 696e 745f              int_
+00005ee0: 6275 6620 3d20 696e 745f 6361 6368 655b  buf = int_cache[
+00005ef0: 675d 0a20 2020 2020 2020 2020 2020 2073  g].            s
+00005f00: 756d 5f62 7566 203d 2073 756d 5f63 6163  um_buf = sum_cac
+00005f10: 6865 5b67 5d0a 0a20 2020 2020 2020 2070  he[g]..        p
+00005f20: 6861 7365 5f66 6163 746f 7273 203d 2075  hase_factors = u
+00005f30: 7469 6c2e 6365 7870 286f 6d65 6761 2a74  til.cexp(omega*t
+00005f40: 5b67 5d2c 206f 7574 3d70 6861 7365 5f66  [g], out=phase_f
+00005f50: 6163 746f 7273 290a 2020 2020 2020 2020  actors).        
+00005f60: 696e 745f 6275 6620 3d20 5f66 6972 7374  int_buf = _first
+00005f70: 5f6f 7264 6572 5f69 6e74 6567 7261 6c28  _order_integral(
+00005f80: 6f6d 6567 612c 2065 6967 7661 6c73 5b67  omega, eigvals[g
+00005f90: 5d2c 2064 745b 675d 2c20 6578 705f 6275  ], dt[g], exp_bu
+00005fa0: 662c 2069 6e74 5f62 7566 290a 2020 2020  f, int_buf).    
+00005fb0: 2020 2020 7375 6d5f 6275 6620 3d20 6578      sum_buf = ex
+00005fc0: 7072 5f31 286e 5f6f 7065 7273 5f74 7261  pr_1(n_opers_tra
+00005fd0: 6e73 666f 726d 6564 5b3a 2c20 675d 2c20  nsformed[:, g], 
+00005fe0: 7068 6173 655f 6661 6374 6f72 735b 3a2c  phase_factors[:,
+00005ff0: 204e 6f6e 652c 204e 6f6e 655d 2a69 6e74   None, None]*int
+00006000: 5f62 7566 2c0a 2020 2020 2020 2020 2020  _buf,.          
+00006010: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+00006020: 7574 3d73 756d 5f62 7566 290a 0a20 2020  ut=sum_buf)..   
+00006030: 2020 2020 206e 6f69 7365 5f6f 7065 7261       noise_opera
+00006040: 746f 7273 202b 3d20 6578 7072 5f32 2865  tors += expr_2(e
+00006050: 6967 7665 6373 5f70 726f 7061 6761 7465  igvecs_propagate
+00006060: 645b 675d 2e63 6f6e 6a28 292c 2073 756d  d[g].conj(), sum
+00006070: 5f62 7566 2c20 6569 6776 6563 735f 7072  _buf, eigvecs_pr
+00006080: 6f70 6167 6174 6564 5b67 5d2c 0a20 2020  opagated[g],.   
+00006090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000060a0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+000060b0: 7574 3d73 756d 5f62 7566 290a 0a20 2020  ut=sum_buf)..   
+000060c0: 2069 6620 6361 6368 655f 696e 7465 726d   if cache_interm
+000060d0: 6564 6961 7465 733a 0a20 2020 2020 2020  ediates:.       
+000060e0: 2069 6e74 6572 6d65 6469 6174 6573 203d   intermediates =
+000060f0: 2064 6963 7428 6e5f 6f70 6572 735f 7472   dict(n_opers_tr
+00006100: 616e 7366 6f72 6d65 643d 6e5f 6f70 6572  ansformed=n_oper
+00006110: 735f 7472 616e 7366 6f72 6d65 642c 0a20  s_transformed,. 
+00006120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006130: 2020 2020 2020 2020 2020 2020 6669 7273              firs
+00006140: 745f 6f72 6465 725f 696e 7465 6772 616c  t_order_integral
+00006150: 3d69 6e74 5f63 6163 6865 2c0a 2020 2020  =int_cache,.    
+00006160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006170: 2020 2020 2020 2020 2070 6861 7365 5f66           phase_f
+00006180: 6163 746f 7273 3d70 6861 7365 5f66 6163  actors=phase_fac
+00006190: 746f 7273 5f63 6163 6865 2c0a 2020 2020  tors_cache,.    
+000061a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000061b0: 2020 2020 2020 2020 206e 6f69 7365 5f6f           noise_o
+000061c0: 7065 7261 746f 7273 5f73 7465 703d 7375  perators_step=su
+000061d0: 6d5f 6361 6368 6529 0a20 2020 2020 2020  m_cache).       
+000061e0: 2072 6574 7572 6e20 6e6f 6973 655f 6f70   return noise_op
+000061f0: 6572 6174 6f72 732c 2069 6e74 6572 6d65  erators, interme
+00006200: 6469 6174 6573 0a0a 2020 2020 7265 7475  diates..    retu
+00006210: 726e 206e 6f69 7365 5f6f 7065 7261 746f  rn noise_operato
+00006220: 7273 0a0a 0a40 7574 696c 2e70 6172 7365  rs...@util.parse
+00006230: 5f6f 7074 696f 6e61 6c5f 7061 7261 6d65  _optional_parame
+00006240: 7465 7273 2877 6869 6368 3d28 2774 6f74  ters(which=('tot
+00006250: 616c 272c 2027 636f 7272 656c 6174 696f  al', 'correlatio
+00006260: 6e73 2729 290a 6465 6620 6361 6c63 756c  ns')).def calcul
+00006270: 6174 655f 636f 6e74 726f 6c5f 6d61 7472  ate_control_matr
+00006280: 6978 5f66 726f 6d5f 6174 6f6d 6963 280a  ix_from_atomic(.
+00006290: 2020 2020 2020 2020 7068 6173 6573 3a20          phases: 
+000062a0: 6e64 6172 7261 792c 0a20 2020 2020 2020  ndarray,.       
+000062b0: 2063 6f6e 7472 6f6c 5f6d 6174 7269 785f   control_matrix_
+000062c0: 6174 6f6d 6963 3a20 6e64 6172 7261 792c  atomic: ndarray,
+000062d0: 0a20 2020 2020 2020 2070 726f 7061 6761  .        propaga
+000062e0: 746f 7273 5f6c 696f 7576 696c 6c65 3a20  tors_liouville: 
+000062f0: 6e64 6172 7261 792c 0a20 2020 2020 2020  ndarray,.       
+00006300: 2073 686f 775f 7072 6f67 7265 7373 6261   show_progressba
+00006310: 723a 2062 6f6f 6c20 3d20 4661 6c73 652c  r: bool = False,
+00006320: 0a20 2020 2020 2020 2077 6869 6368 3a20  .        which: 
+00006330: 7374 7220 3d20 2774 6f74 616c 270a 2920  str = 'total'.) 
+00006340: 2d3e 206e 6461 7272 6179 3a0a 2020 2020  -> ndarray:.    
+00006350: 7222 2222 0a20 2020 2043 616c 6375 6c61  r""".    Calcula
+00006360: 7465 2074 6865 2063 6f6e 7472 6f6c 206d  te the control m
+00006370: 6174 7269 7820 6672 6f6d 2074 6865 2063  atrix from the c
+00006380: 6f6e 7472 6f6c 206d 6174 7269 6365 7320  ontrol matrices 
+00006390: 6f66 2061 746f 6d69 630a 2020 2020 7365  of atomic.    se
+000063a0: 676d 656e 7473 2e0a 0a20 2020 2050 6172  gments...    Par
+000063b0: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
+000063c0: 2d2d 2d2d 2d2d 0a20 2020 2070 6861 7365  ------.    phase
+000063d0: 733a 2061 7272 6179 5f6c 696b 652c 2073  s: array_like, s
+000063e0: 6861 7065 2028 6e5f 6474 2c20 6e5f 6f6d  hape (n_dt, n_om
+000063f0: 6567 6129 0a20 2020 2020 2020 2054 6865  ega).        The
+00006400: 2070 6861 7365 2066 6163 746f 7273 2066   phase factors f
+00006410: 6f72 203a 6d61 7468 3a60 675c 696e 5c7b  or :math:`g\in\{
+00006420: 302c 2031 2c20 5c64 6f74 732c 2047 2d31  0, 1, \dots, G-1
+00006430: 5c7d 602e 0a20 2020 2063 6f6e 7472 6f6c  \}`..    control
+00006440: 5f6d 6174 7269 785f 6174 6f6d 6963 3a20  _matrix_atomic: 
+00006450: 6172 7261 795f 6c69 6b65 2c20 7368 6170  array_like, shap
+00006460: 6520 286e 5f64 742c 206e 5f6e 6f70 732c  e (n_dt, n_nops,
+00006470: 2064 2a2a 322c 206e 5f6f 6d65 6761 290a   d**2, n_omega).
+00006480: 2020 2020 2020 2020 5468 6520 7075 6c73          The puls
+00006490: 6520 636f 6e74 726f 6c20 6d61 7472 6963  e control matric
+000064a0: 6573 2066 6f72 203a 6d61 7468 3a60 675c  es for :math:`g\
+000064b0: 696e 5c7b 312c 2032 2c20 5c64 6f74 732c  in\{1, 2, \dots,
+000064c0: 2047 5c7d 602e 0a20 2020 2070 726f 7061   G\}`..    propa
+000064d0: 6761 746f 7273 5f6c 696f 7576 696c 6c65  gators_liouville
+000064e0: 3a20 6172 7261 795f 6c69 6b65 2c20 7368  : array_like, sh
+000064f0: 6170 6520 286e 5f64 742c 206e 5f6e 6f70  ape (n_dt, n_nop
+00006500: 732c 2064 2a2a 322c 2064 2a2a 3229 0a20  s, d**2, d**2). 
+00006510: 2020 2020 2020 2054 6865 2074 7261 6e73         The trans
+00006520: 6665 7220 6d61 7472 6963 6573 206f 6620  fer matrices of 
+00006530: 7468 6520 6375 6d75 6c61 7469 7665 2070  the cumulative p
+00006540: 726f 7061 6761 746f 7273 2066 6f72 0a20  ropagators for. 
+00006550: 2020 2020 2020 203a 6d61 7468 3a60 675c         :math:`g\
+00006560: 696e 5c7b 302c 2031 2c20 5c64 6f74 732c  in\{0, 1, \dots,
+00006570: 2047 2d31 5c7d 602e 0a20 2020 2073 686f   G-1\}`..    sho
+00006580: 775f 7072 6f67 7265 7373 6261 723a 2062  w_progressbar: b
+00006590: 6f6f 6c2c 206f 7074 696f 6e61 6c0a 2020  ool, optional.  
+000065a0: 2020 2020 2020 5368 6f77 2061 2070 726f        Show a pro
+000065b0: 6772 6573 7320 6261 7220 666f 7220 7468  gress bar for th
+000065c0: 6520 6361 6c63 756c 6174 696f 6e2e 0a20  e calculation.. 
+000065d0: 2020 2077 6869 6368 3a20 7374 722c 2028     which: str, (
+000065e0: 2774 6f74 616c 272c 2027 636f 7272 656c  'total', 'correl
+000065f0: 6174 696f 6e73 2729 0a20 2020 2020 2020  ations').       
+00006600: 2043 6f6d 7075 7465 2074 6865 2074 6f74   Compute the tot
+00006610: 616c 2063 6f6e 7472 6f6c 206d 6174 7269  al control matri
+00006620: 7820 2874 6865 2073 756d 206f 6620 616c  x (the sum of al
+00006630: 6c20 7469 6d65 2073 7465 7073 2920 6f72  l time steps) or
+00006640: 0a20 2020 2020 2020 2074 6865 2063 6f72  .        the cor
+00006650: 7265 6c61 7469 6f6e 2063 6f6e 7472 6f6c  relation control
+00006660: 206d 6174 7269 7820 2866 6972 7374 2061   matrix (first a
+00006670: 7869 7320 686f 6c64 7320 6561 6368 2070  xis holds each p
+00006680: 756c 7365 7327 0a20 2020 2020 2020 2063  ulses'.        c
+00006690: 6f6e 7472 6962 7574 696f 6e29 0a0a 2020  ontribution)..  
+000066a0: 2020 5265 7475 726e 730a 2020 2020 2d2d    Returns.    --
+000066b0: 2d2d 2d2d 2d0a 2020 2020 636f 6e74 726f  -----.    contro
+000066c0: 6c5f 6d61 7472 6978 3a20 6e64 6172 7261  l_matrix: ndarra
+000066d0: 792c 2073 6861 7065 2028 5b6e 5f70 6c73  y, shape ([n_pls
+000066e0: 2c5d 206e 5f6e 6f70 732c 2064 2a2a 322c  ,] n_nops, d**2,
+000066f0: 206e 5f6f 6d65 6761 290a 2020 2020 2020   n_omega).      
+00006700: 2020 5468 6520 636f 6e74 726f 6c20 6d61    The control ma
+00006710: 7472 6978 203a 6d61 7468 3a60 5c74 696c  trix :math:`\til
+00006720: 6465 7b5c 6d61 7468 6361 6c7b 427d 7d28  de{\mathcal{B}}(
+00006730: 5c6f 6d65 6761 2960 2e0a 0a20 2020 204e  \omega)`...    N
+00006740: 6f74 6573 0a20 2020 202d 2d2d 2d2d 0a20  otes.    -----. 
+00006750: 2020 2054 6865 2063 6f6e 7472 6f6c 206d     The control m
+00006760: 6174 7269 7820 6973 2063 616c 6375 6c61  atrix is calcula
+00006770: 7465 6420 6279 2065 7661 6c75 6174 696e  ted by evaluatin
+00006780: 6720 7468 6520 7375 6d0a 0a20 2020 202e  g the sum..    .
+00006790: 2e20 6d61 7468 3a3a 0a0a 2020 2020 2020  . math::..      
+000067a0: 2020 5c74 696c 6465 7b5c 6d61 7468 6361    \tilde{\mathca
+000067b0: 6c7b 427d 7d28 5c6f 6d65 6761 2920 3d20  l{B}}(\omega) = 
+000067c0: 5c73 756d 5f7b 673d 317d 5e47 2065 5e7b  \sum_{g=1}^G e^{
+000067d0: 695c 6f6d 6567 6120 745f 7b67 2d31 7d7d  i\omega t_{g-1}}
+000067e0: 0a20 2020 2020 2020 2020 2020 205c 7469  .            \ti
+000067f0: 6c64 657b 5c6d 6174 6863 616c 7b42 7d7d  lde{\mathcal{B}}
+00006800: 5e7b 2867 297d 285c 6f6d 6567 6129 5c6d  ^{(g)}(\omega)\m
+00006810: 6174 6863 616c 7b51 7d5e 7b28 672d 3129  athcal{Q}^{(g-1)
+00006820: 7d2e 0a0a 2020 2020 5365 6520 416c 736f  }...    See Also
+00006830: 0a20 2020 202d 2d2d 2d2d 2d2d 2d0a 2020  .    --------.  
+00006840: 2020 6361 6c63 756c 6174 655f 636f 6e74    calculate_cont
+00006850: 726f 6c5f 6d61 7472 6978 5f66 726f 6d5f  rol_matrix_from_
+00006860: 7363 7261 7463 683a 2043 6f6e 7472 6f6c  scratch: Control
+00006870: 206d 6174 7269 7820 6672 6f6d 2073 6372   matrix from scr
+00006880: 6174 6368 2e0a 2020 2020 6c69 6f75 7669  atch..    liouvi
+00006890: 6c6c 655f 7265 7072 6573 656e 7461 7469  lle_representati
+000068a0: 6f6e 3a20 4c69 6f75 7669 6c6c 6520 7265  on: Liouville re
+000068b0: 7072 6573 656e 7461 7469 6f6e 2066 6f72  presentation for
+000068c0: 2061 2067 6976 656e 2062 6173 6973 2e0a   a given basis..
+000068d0: 2020 2020 2222 220a 2020 2020 6e20 3d20      """.    n = 
+000068e0: 6c65 6e28 636f 6e74 726f 6c5f 6d61 7472  len(control_matr
+000068f0: 6978 5f61 746f 6d69 6329 0a20 2020 2023  ix_atomic).    #
+00006900: 2053 6574 2075 7020 6120 7265 7573 6162   Set up a reusab
+00006910: 6c65 2063 6f6e 7472 6163 7469 6f6e 2065  le contraction e
+00006920: 7870 7265 7373 696f 6e2e 2049 6e20 736f  xpression. In so
+00006930: 6d65 2063 6173 6573 2069 7420 6973 2066  me cases it is f
+00006940: 6173 7465 7220 746f 0a20 2020 2023 2061  aster to.    # a
+00006950: 6c73 6f20 636f 6e74 7261 6374 2074 6865  lso contract the
+00006960: 2074 696d 6520 6469 6d65 6e73 696f 6e20   time dimension 
+00006970: 696e 2074 6865 2073 616d 6520 6578 7072  in the same expr
+00006980: 6573 7369 6f6e 2069 6e73 7465 6164 206f  ession instead o
+00006990: 660a 2020 2020 2320 6c6f 6f70 696e 6720  f.    # looping 
+000069a0: 6f76 6572 2069 742c 2062 7574 2077 6520  over it, but we 
+000069b0: 646f 6e27 7420 6469 7374 696e 6775 6973  don't distinguis
+000069c0: 6820 6865 7265 2066 6f72 2072 6561 6461  h here for reada
+000069d0: 6269 6c69 7479 2e0a 2020 2020 6578 7072  bility..    expr
+000069e0: 203d 206f 652e 636f 6e74 7261 6374 5f65   = oe.contract_e
+000069f0: 7870 7265 7373 696f 6e28 2769 6a6f 2c6a  xpression('ijo,j
+00006a00: 6b2d 3e69 6b6f 272c 0a20 2020 2020 2020  k->iko',.       
+00006a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a20: 2020 2020 2020 2020 2020 2063 6f6e 7472             contr
+00006a30: 6f6c 5f6d 6174 7269 785f 6174 6f6d 6963  ol_matrix_atomic
+00006a40: 2e73 6861 7065 5b31 3a5d 2c0a 2020 2020  .shape[1:],.    
+00006a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a60: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00006a70: 6f70 6167 6174 6f72 735f 6c69 6f75 7669  opagators_liouvi
+00006a80: 6c6c 652e 7368 6170 655b 313a 5d29 0a0a  lle.shape[1:])..
+00006a90: 2020 2020 2320 416c 6c6f 6361 7465 206d      # Allocate m
+00006aa0: 656d 6f72 790a 2020 2020 6966 2077 6869  emory.    if whi
+00006ab0: 6368 203d 3d20 2774 6f74 616c 273a 0a20  ch == 'total':. 
+00006ac0: 2020 2020 2020 2063 6f6e 7472 6f6c 5f6d         control_m
+00006ad0: 6174 7269 7820 3d20 6e70 2e7a 6572 6f73  atrix = np.zeros
+00006ae0: 2863 6f6e 7472 6f6c 5f6d 6174 7269 785f  (control_matrix_
+00006af0: 6174 6f6d 6963 2e73 6861 7065 5b31 3a5d  atomic.shape[1:]
+00006b00: 2c20 6474 7970 653d 636f 6d70 6c65 7829  , dtype=complex)
+00006b10: 0a20 2020 2020 2020 2066 6f72 2067 2069  .        for g i
+00006b20: 6e20 7574 696c 2e70 726f 6772 6573 7362  n util.progressb
+00006b30: 6172 5f72 616e 6765 286e 2c20 7368 6f77  ar_range(n, show
+00006b40: 5f70 726f 6772 6573 7362 6172 3d73 686f  _progressbar=sho
+00006b50: 775f 7072 6f67 7265 7373 6261 722c 0a20  w_progressbar,. 
+00006b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006b80: 2020 2020 2020 2064 6573 633d 2743 616c         desc='Cal
+00006b90: 6375 6c61 7469 6e67 2063 6f6e 7472 6f6c  culating control
+00006ba0: 206d 6174 7269 7827 293a 0a20 2020 2020   matrix'):.     
+00006bb0: 2020 2020 2020 2063 6f6e 7472 6f6c 5f6d         control_m
+00006bc0: 6174 7269 7820 2b3d 2065 7870 7228 7068  atrix += expr(ph
+00006bd0: 6173 6573 5b67 5d2a 636f 6e74 726f 6c5f  ases[g]*control_
+00006be0: 6d61 7472 6978 5f61 746f 6d69 635b 675d  matrix_atomic[g]
+00006bf0: 2c20 7072 6f70 6167 6174 6f72 735f 6c69  , propagators_li
+00006c00: 6f75 7669 6c6c 655b 675d 290a 2020 2020  ouville[g]).    
+00006c10: 656c 7365 3a0a 2020 2020 2020 2020 2320  else:.        # 
+00006c20: 7768 6963 6820 3d3d 2027 636f 7272 656c  which == 'correl
+00006c30: 6174 696f 6e73 270a 2020 2020 2020 2020  ations'.        
+00006c40: 636f 6e74 726f 6c5f 6d61 7472 6978 203d  control_matrix =
+00006c50: 206e 702e 7a65 726f 7328 636f 6e74 726f   np.zeros(contro
+00006c60: 6c5f 6d61 7472 6978 5f61 746f 6d69 632e  l_matrix_atomic.
+00006c70: 7368 6170 652c 2064 7479 7065 3d63 6f6d  shape, dtype=com
+00006c80: 706c 6578 290a 2020 2020 2020 2020 666f  plex).        fo
+00006c90: 7220 6720 696e 2075 7469 6c2e 7072 6f67  r g in util.prog
+00006ca0: 7265 7373 6261 725f 7261 6e67 6528 6e2c  ressbar_range(n,
+00006cb0: 2073 686f 775f 7072 6f67 7265 7373 6261   show_progressba
+00006cc0: 723d 7368 6f77 5f70 726f 6772 6573 7362  r=show_progressb
+00006cd0: 6172 2c0a 2020 2020 2020 2020 2020 2020  ar,.            
+00006ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006cf0: 2020 2020 2020 2020 2020 2020 6465 7363              desc
+00006d00: 3d27 4361 6c63 756c 6174 696e 6720 636f  ='Calculating co
+00006d10: 6e74 726f 6c20 6d61 7472 6978 2729 3a0a  ntrol matrix'):.
+00006d20: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
+00006d30: 726f 6c5f 6d61 7472 6978 5b67 5d20 3d20  rol_matrix[g] = 
+00006d40: 6578 7072 2870 6861 7365 735b 675d 2a63  expr(phases[g]*c
+00006d50: 6f6e 7472 6f6c 5f6d 6174 7269 785f 6174  ontrol_matrix_at
+00006d60: 6f6d 6963 5b67 5d2c 2070 726f 7061 6761  omic[g], propaga
+00006d70: 746f 7273 5f6c 696f 7576 696c 6c65 5b67  tors_liouville[g
+00006d80: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+00006d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006da0: 2020 2020 2020 2020 6f75 743d 636f 6e74          out=cont
+00006db0: 726f 6c5f 6d61 7472 6978 5b67 5d29 0a0a  rol_matrix[g])..
+00006dc0: 2020 2020 7265 7475 726e 2063 6f6e 7472      return contr
+00006dd0: 6f6c 5f6d 6174 7269 780a 0a0a 6465 6620  ol_matrix...def 
+00006de0: 6361 6c63 756c 6174 655f 636f 6e74 726f  calculate_contro
+00006df0: 6c5f 6d61 7472 6978 5f66 726f 6d5f 7363  l_matrix_from_sc
+00006e00: 7261 7463 6828 0a20 2020 2020 2020 2065  ratch(.        e
+00006e10: 6967 7661 6c73 3a20 6e64 6172 7261 792c  igvals: ndarray,
+00006e20: 0a20 2020 2020 2020 2065 6967 7665 6373  .        eigvecs
+00006e30: 3a20 6e64 6172 7261 792c 0a20 2020 2020  : ndarray,.     
+00006e40: 2020 2070 726f 7061 6761 746f 7273 3a20     propagators: 
+00006e50: 6e64 6172 7261 792c 0a20 2020 2020 2020  ndarray,.       
+00006e60: 206f 6d65 6761 3a20 436f 6566 6669 6369   omega: Coeffici
+00006e70: 656e 7473 2c0a 2020 2020 2020 2020 6261  ents,.        ba
+00006e80: 7369 733a 2042 6173 6973 2c0a 2020 2020  sis: Basis,.    
+00006e90: 2020 2020 6e5f 6f70 6572 733a 2053 6571      n_opers: Seq
+00006ea0: 7565 6e63 655b 4f70 6572 6174 6f72 5d2c  uence[Operator],
+00006eb0: 0a20 2020 2020 2020 206e 5f63 6f65 6666  .        n_coeff
+00006ec0: 733a 2053 6571 7565 6e63 655b 436f 6566  s: Sequence[Coef
+00006ed0: 6669 6369 656e 7473 5d2c 0a20 2020 2020  ficients],.     
+00006ee0: 2020 2064 743a 2043 6f65 6666 6963 6965     dt: Coefficie
+00006ef0: 6e74 732c 0a20 2020 2020 2020 2074 3a20  nts,.        t: 
+00006f00: 4f70 7469 6f6e 616c 5b43 6f65 6666 6963  Optional[Coeffic
+00006f10: 6965 6e74 735d 203d 204e 6f6e 652c 0a20  ients] = None,. 
+00006f20: 2020 2020 2020 2073 686f 775f 7072 6f67         show_prog
+00006f30: 7265 7373 6261 723a 2062 6f6f 6c20 3d20  ressbar: bool = 
+00006f40: 4661 6c73 652c 0a20 2020 2020 2020 2063  False,.        c
+00006f50: 6163 6865 5f69 6e74 6572 6d65 6469 6174  ache_intermediat
+00006f60: 6573 3a20 626f 6f6c 203d 2046 616c 7365  es: bool = False
+00006f70: 2c0a 2020 2020 2020 2020 6f75 743a 204f  ,.        out: O
+00006f80: 7074 696f 6e61 6c5b 6e64 6172 7261 795d  ptional[ndarray]
+00006f90: 203d 204e 6f6e 650a 2920 2d3e 2055 6e69   = None.) -> Uni
+00006fa0: 6f6e 5b6e 6461 7272 6179 2c20 5475 706c  on[ndarray, Tupl
+00006fb0: 655b 6e64 6172 7261 792c 2044 6963 745b  e[ndarray, Dict[
+00006fc0: 7374 722c 206e 6461 7272 6179 5d5d 5d3a  str, ndarray]]]:
+00006fd0: 0a20 2020 2072 2222 220a 2020 2020 4361  .    r""".    Ca
+00006fe0: 6c63 756c 6174 6520 7468 6520 636f 6e74  lculate the cont
+00006ff0: 726f 6c20 6d61 7472 6978 2066 726f 6d20  rol matrix from 
+00007000: 7363 7261 7463 682c 2069 2e65 2e20 7769  scratch, i.e. wi
+00007010: 7468 6f75 7420 6b6e 6f77 6c65 6467 6520  thout knowledge 
+00007020: 6f66 0a20 2020 2074 6865 2063 6f6e 7472  of.    the contr
+00007030: 6f6c 206d 6174 7269 6365 7320 6f66 206d  ol matrices of m
+00007040: 6f72 6520 6174 6f6d 6963 2070 756c 7365  ore atomic pulse
+00007050: 2073 6571 7565 6e63 6573 2e0a 0a20 2020   sequences...   
+00007060: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
+00007070: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2065  ----------.    e
+00007080: 6967 7661 6c73 3a20 6172 7261 795f 6c69  igvals: array_li
+00007090: 6b65 2c20 7368 6170 6520 286e 5f64 742c  ke, shape (n_dt,
+000070a0: 2064 290a 2020 2020 2020 2020 4569 6765   d).        Eige
+000070b0: 6e76 616c 7565 2076 6563 746f 7273 2066  nvalue vectors f
+000070c0: 6f72 2065 6163 6820 7469 6d65 2070 756c  or each time pul
+000070d0: 7365 2073 6567 6d65 6e74 202a 672a 2077  se segment *g* w
+000070e0: 6974 6820 7468 650a 2020 2020 2020 2020  ith the.        
+000070f0: 6669 7273 7420 6178 6973 2063 6f75 6e74  first axis count
+00007100: 696e 6720 7468 6520 7075 6c73 6520 7365  ing the pulse se
+00007110: 676d 656e 742c 2069 2e65 2e0a 2020 2020  gment, i.e..    
+00007120: 2020 2020 6060 6569 6776 616c 7320 3d3d      ``eigvals ==
+00007130: 2061 7272 6179 285b 445f 302c 2044 5f31   array([D_0, D_1
+00007140: 2c20 2e2e 2e5d 2960 602e 0a20 2020 2065  , ...])``..    e
+00007150: 6967 7665 6373 3a20 6172 7261 795f 6c69  igvecs: array_li
+00007160: 6b65 2c20 7368 6170 6520 286e 5f64 742c  ke, shape (n_dt,
+00007170: 2064 2c20 6429 0a20 2020 2020 2020 2045   d, d).        E
+00007180: 6967 656e 7665 6374 6f72 206d 6174 7269  igenvector matri
+00007190: 6365 7320 666f 7220 6561 6368 2074 696d  ces for each tim
+000071a0: 6520 7075 6c73 6520 7365 676d 656e 7420  e pulse segment 
+000071b0: 2a67 2a20 7769 7468 2074 6865 0a20 2020  *g* with the.   
+000071c0: 2020 2020 2066 6972 7374 2061 7869 7320       first axis 
+000071d0: 636f 756e 7469 6e67 2074 6865 2070 756c  counting the pul
+000071e0: 7365 2073 6567 6d65 6e74 2c20 692e 652e  se segment, i.e.
+000071f0: 0a20 2020 2020 2020 2060 6065 6967 7665  .        ``eigve
+00007200: 6373 203d 3d20 6172 7261 7928 5b56 5f30  cs == array([V_0
+00007210: 2c20 565f 312c 202e 2e2e 5d29 6060 2e0a  , V_1, ...])``..
+00007220: 2020 2020 7072 6f70 6167 6174 6f72 733a      propagators:
+00007230: 2061 7272 6179 5f6c 696b 652c 2073 6861   array_like, sha
+00007240: 7065 2028 6e5f 6474 2b31 2c20 642c 2064  pe (n_dt+1, d, d
+00007250: 290a 2020 2020 2020 2020 5468 6520 7072  ).        The pr
+00007260: 6f70 6167 6174 6f72 7320 3a6d 6174 683a  opagators :math:
+00007270: 6051 5f67 203d 2050 5f67 2050 5f7b 672d  `Q_g = P_g P_{g-
+00007280: 317d 5c63 646f 7473 2050 5f30 6020 6173  1}\cdots P_0` as
+00007290: 2061 2028 642c 2064 290a 2020 2020 2020   a (d, d).      
+000072a0: 2020 6172 7261 7920 7769 7468 202a 642a    array with *d*
+000072b0: 2074 6865 2064 696d 656e 7369 6f6e 206f   the dimension o
+000072c0: 6620 7468 6520 4869 6c62 6572 7420 7370  f the Hilbert sp
+000072d0: 6163 652e 0a20 2020 206f 6d65 6761 3a20  ace..    omega: 
+000072e0: 6172 7261 795f 6c69 6b65 2c20 7368 6170  array_like, shap
+000072f0: 6520 286e 5f6f 6d65 6761 2c29 0a20 2020  e (n_omega,).   
+00007300: 2020 2020 2046 7265 7175 656e 6369 6573       Frequencies
+00007310: 2061 7420 7768 6963 6820 7468 6520 7075   at which the pu
+00007320: 6c73 6520 636f 6e74 726f 6c20 6d61 7472  lse control matr
+00007330: 6978 2069 7320 746f 2062 650a 2020 2020  ix is to be.    
+00007340: 2020 2020 6576 616c 7561 7465 642e 0a20      evaluated.. 
+00007350: 2020 2062 6173 6973 3a20 4261 7369 732c     basis: Basis,
+00007360: 2073 6861 7065 2028 642a 2a32 2c20 642c   shape (d**2, d,
+00007370: 2064 290a 2020 2020 2020 2020 5468 6520   d).        The 
+00007380: 6261 7369 7320 656c 656d 656e 7473 2069  basis elements i
+00007390: 6e20 7768 6963 6820 7468 6520 7075 6c73  n which the puls
+000073a0: 6520 636f 6e74 726f 6c20 6d61 7472 6978  e control matrix
+000073b0: 2077 696c 6c20 6265 0a20 2020 2020 2020   will be.       
+000073c0: 2065 7870 616e 6465 642e 0a20 2020 206e   expanded..    n
+000073d0: 5f6f 7065 7273 3a20 6172 7261 795f 6c69  _opers: array_li
+000073e0: 6b65 2c20 7368 6170 6520 286e 5f6e 6f70  ke, shape (n_nop
+000073f0: 732c 2064 2c20 6429 0a20 2020 2020 2020  s, d, d).       
+00007400: 204e 6f69 7365 206f 7065 7261 746f 7273   Noise operators
+00007410: 203a 6d61 7468 3a60 425f 5c61 6c70 6861   :math:`B_\alpha
+00007420: 602e 0a20 2020 206e 5f63 6f65 6666 733a  `..    n_coeffs:
+00007430: 2061 7272 6179 5f6c 696b 652c 2073 6861   array_like, sha
+00007440: 7065 2028 6e5f 6e6f 7073 2c20 6e5f 6474  pe (n_nops, n_dt
+00007450: 290a 2020 2020 2020 2020 5468 6520 7365  ).        The se
+00007460: 6e73 6974 6976 6974 6965 7320 6f66 2074  nsitivities of t
+00007470: 6865 2073 7973 7465 6d20 746f 2074 6865  he system to the
+00007480: 206e 6f69 7365 206f 7065 7261 746f 7273   noise operators
+00007490: 2067 6976 656e 2062 790a 2020 2020 2020   given by.      
+000074a0: 2020 2a6e 5f6f 7065 7273 2a20 6174 2074    *n_opers* at t
+000074b0: 6865 2067 6976 656e 2074 696d 6520 7374  he given time st
+000074c0: 6570 2e0a 2020 2020 6474 3a20 6172 7261  ep..    dt: arra
+000074d0: 795f 6c69 6b65 2c20 7368 6170 6520 286e  y_like, shape (n
+000074e0: 5f64 7429 0a20 2020 2020 2020 2053 6571  _dt).        Seq
+000074f0: 7565 6e63 6520 6475 7261 7469 6f6e 2c20  uence duration, 
+00007500: 692e 652e 2066 6f72 2074 6865 203a 6d61  i.e. for the :ma
+00007510: 7468 3a60 6760 2d74 6820 7075 6c73 650a  th:`g`-th pulse.
+00007520: 2020 2020 2020 2020 3a6d 6174 683a 6074          :math:`t
+00007530: 5f67 202d 2074 5f7b 672d 317d 602e 0a20  _g - t_{g-1}`.. 
+00007540: 2020 2074 3a20 6172 7261 795f 6c69 6b65     t: array_like
+00007550: 2c20 7368 6170 6520 286e 5f64 742b 3129  , shape (n_dt+1)
+00007560: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
+00007570: 2020 2054 6865 2061 6273 6f6c 7574 6520     The absolute 
+00007580: 7469 6d65 7320 6f66 2074 6865 2064 6966  times of the dif
+00007590: 6665 7265 6e74 2073 6567 6d65 6e74 732e  ferent segments.
+000075a0: 2043 616e 2061 6c73 6f20 6265 0a20 2020   Can also be.   
+000075b0: 2020 2020 2063 6f6d 7075 7465 6420 6672       computed fr
+000075c0: 6f6d 202a 6474 2a2e 0a20 2020 2073 686f  om *dt*..    sho
+000075d0: 775f 7072 6f67 7265 7373 6261 723a 2062  w_progressbar: b
+000075e0: 6f6f 6c2c 206f 7074 696f 6e61 6c0a 2020  ool, optional.  
+000075f0: 2020 2020 2020 5368 6f77 2061 2070 726f        Show a pro
+00007600: 6772 6573 7320 6261 7220 666f 7220 7468  gress bar for th
+00007610: 6520 6361 6c63 756c 6174 696f 6e2e 0a20  e calculation.. 
+00007620: 2020 2063 6163 6865 5f69 6e74 6572 6d65     cache_interme
+00007630: 6469 6174 6573 3a20 626f 6f6c 2c20 6f70  diates: bool, op
+00007640: 7469 6f6e 616c 0a20 2020 2020 2020 204b  tional.        K
+00007650: 6565 7020 616e 6420 7265 7475 726e 2069  eep and return i
+00007660: 6e74 6572 6d65 6469 6174 6520 7465 726d  ntermediate term
+00007670: 7320 6f66 2074 6865 2063 616c 6375 6c61  s of the calcula
+00007680: 7469 6f6e 2074 6861 7420 6361 6e0a 2020  tion that can.  
+00007690: 2020 2020 2020 6265 2072 6575 7365 6420        be reused 
+000076a0: 696e 206f 7468 6572 2063 6f6d 7075 7461  in other computa
+000076b0: 7469 6f6e 7320 2873 6563 6f6e 6420 6f72  tions (second or
+000076c0: 6465 7220 6f72 2067 7261 6469 656e 7473  der or gradients
+000076d0: 292e 0a20 2020 2020 2020 204f 7468 6572  )..        Other
+000076e0: 7769 7365 2074 6865 2073 756d 2069 7320  wise the sum is 
+000076f0: 7065 7266 6f72 6d65 6420 696e 2d70 6c61  performed in-pla
+00007700: 6365 2e20 5468 6520 6465 6661 756c 7420  ce. The default 
+00007710: 6973 2046 616c 7365 2e0a 2020 2020 6f75  is False..    ou
+00007720: 743a 206e 6461 7272 6179 2c20 6f70 7469  t: ndarray, opti
+00007730: 6f6e 616c 0a20 2020 2020 2020 2041 206c  onal.        A l
+00007740: 6f63 6174 696f 6e20 696e 746f 2077 6869  ocation into whi
+00007750: 6368 2074 6865 2072 6573 756c 7420 6973  ch the result is
+00007760: 2073 746f 7265 642e 2053 6565 0a20 2020   stored. See.   
+00007770: 2020 2020 203a 6675 6e63 3a60 6e75 6d70       :func:`nump
+00007780: 792e 7566 756e 6360 2e0a 0a20 2020 2052  y.ufunc`...    R
+00007790: 6574 7572 6e73 0a20 2020 202d 2d2d 2d2d  eturns.    -----
+000077a0: 2d2d 0a20 2020 2063 6f6e 7472 6f6c 5f6d  --.    control_m
+000077b0: 6174 7269 783a 206e 6461 7272 6179 2c20  atrix: ndarray, 
+000077c0: 7368 6170 6520 286e 5f6e 6f70 732c 2064  shape (n_nops, d
+000077d0: 2a2a 322c 206e 5f6f 6d65 6761 290a 2020  **2, n_omega).  
+000077e0: 2020 2020 2020 5468 6520 636f 6e74 726f        The contro
+000077f0: 6c20 6d61 7472 6978 203a 6d61 7468 3a60  l matrix :math:`
+00007800: 5c74 696c 6465 7b5c 6d61 7468 6361 6c7b  \tilde{\mathcal{
+00007810: 427d 7d28 5c6f 6d65 6761 2960 0a20 2020  B}}(\omega)`.   
+00007820: 2069 6e74 6572 6d65 6469 6174 6573 3a20   intermediates: 
+00007830: 6469 6374 5b73 7472 2c20 6e64 6172 7261  dict[str, ndarra
+00007840: 795d 0a20 2020 2020 2020 2049 6e74 6572  y].        Inter
+00007850: 6d65 6469 6174 6520 7265 7375 6c74 7320  mediate results 
+00007860: 6f66 2074 6865 2063 616c 6375 6c61 7469  of the calculati
+00007870: 6f6e 2e20 4f6e 6c79 2069 660a 2020 2020  on. Only if.    
+00007880: 2020 2020 6361 6368 655f 696e 7465 726d      cache_interm
+00007890: 6564 6961 7465 7320 6973 2054 7275 652e  ediates is True.
+000078a0: 0a0a 2020 2020 4e6f 7465 730a 2020 2020  ..    Notes.    
+000078b0: 2d2d 2d2d 2d0a 2020 2020 5468 6520 636f  -----.    The co
+000078c0: 6e74 726f 6c20 6d61 7472 6978 2069 7320  ntrol matrix is 
+000078d0: 6361 6c63 756c 6174 6564 2061 6363 6f72  calculated accor
+000078e0: 6469 6e67 2074 6f0a 0a20 2020 202e 2e20  ding to..    .. 
+000078f0: 6d61 7468 3a3a 0a0a 2020 2020 2020 2020  math::..        
+00007900: 5c74 696c 6465 7b5c 6d61 7468 6361 6c7b  \tilde{\mathcal{
+00007910: 427d 7d5f 7b5c 616c 7068 6120 6b7d 285c  B}}_{\alpha k}(\
+00007920: 6f6d 6567 6129 203d 205c 7375 6d5f 7b67  omega) = \sum_{g
+00007930: 3d31 7d5e 470a 2020 2020 2020 2020 2020  =1}^G.          
+00007940: 2020 655e 7b69 5c6f 6d65 6761 2074 5f7b    e^{i\omega t_{
+00007950: 672d 317d 7d20 735f 5c61 6c70 6861 5e7b  g-1}} s_\alpha^{
+00007960: 2867 297d 5c6d 6174 6872 6d7b 7472 7d5c  (g)}\mathrm{tr}\
+00007970: 6c65 6674 280a 2020 2020 2020 2020 2020  left(.          
+00007980: 2020 2020 2020 5b5c 6261 727b 427d 5f5c        [\bar{B}_\
+00007990: 616c 7068 615e 7b28 6729 7d5c 6369 7263  alpha^{(g)}\circ
+000079a0: 2049 285c 6f6d 6567 6129 5d20 5c62 6172   I(\omega)] \bar
+000079b0: 7b43 7d5f 6b5e 7b28 6729 7d0a 2020 2020  {C}_k^{(g)}.    
+000079c0: 2020 2020 2020 2020 5c72 6967 6874 290a          \right).
+000079d0: 0a20 2020 2077 6865 7265 0a0a 2020 2020  .    where..    
+000079e0: 2e2e 206d 6174 683a 3a0a 0a20 2020 2020  .. math::..     
+000079f0: 2020 2049 5e7b 2867 297d 5f7b 6e6d 7d28     I^{(g)}_{nm}(
+00007a00: 5c6f 6d65 6761 2920 263d 205c 696e 745f  \omega) &= \int_
+00007a10: 305e 7b74 5f6c 202d 2074 5f7b 672d 317d  0^{t_l - t_{g-1}
+00007a20: 7d5c 6d61 7468 726d 7b64 7d74 5c2c 0a20  }\mathrm{d}t\,. 
+00007a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a40: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00007a50: 5e7b 6928 5c6f 6d65 6761 2b5c 6f6d 6567  ^{i(\omega+\omeg
+00007a60: 615f 6e2d 5c6f 6d65 6761 5f6d 2974 7d20  a_n-\omega_m)t} 
+00007a70: 5c5c 0a20 2020 2020 2020 2020 2020 2020  \\.             
+00007a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a90: 263d 205c 6672 6163 7b65 5e7b 6928 5c6f  &= \frac{e^{i(\o
+00007aa0: 6d65 6761 2b5c 6f6d 6567 615f 6e2d 5c6f  mega+\omega_n-\o
+00007ab0: 6d65 6761 5f6d 290a 2020 2020 2020 2020  mega_m).        
+00007ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ad0: 2020 2020 2020 2020 2874 5f6c 202d 2074          (t_l - t
+00007ae0: 5f7b 672d 317d 297d 202d 2031 7d0a 2020  _{g-1})} - 1}.  
+00007af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007b00: 2020 2020 2020 2020 2020 2020 2020 7b69                {i
+00007b10: 285c 6f6d 6567 612b 5c6f 6d65 6761 5f6e  (\omega+\omega_n
+00007b20: 2d5c 6f6d 6567 615f 6d29 7d2c 205c 5c0a  -\omega_m)}, \\.
+00007b30: 2020 2020 2020 2020 5c62 6172 7b42 7d5f          \bar{B}_
+00007b40: 5c61 6c70 6861 5e7b 2867 297d 2026 3d20  \alpha^{(g)} &= 
+00007b50: 565e 7b28 6729 5c64 6167 6765 727d 2042  V^{(g)\dagger} B
+00007b60: 5f5c 616c 7068 6120 565e 7b28 6729 7d2c  _\alpha V^{(g)},
+00007b70: 205c 5c0a 2020 2020 2020 2020 5c62 6172   \\.        \bar
+00007b80: 7b43 7d5f 6b5e 7b28 6729 7d20 263d 2056  {C}_k^{(g)} &= V
+00007b90: 5e7b 2867 295c 6461 6767 6572 7d20 515f  ^{(g)\dagger} Q_
+00007ba0: 7b67 2d31 7d20 435f 6b20 515f 7b67 2d31  {g-1} C_k Q_{g-1
+00007bb0: 7d5e 5c64 6167 6765 7220 565e 7b28 6729  }^\dagger V^{(g)
+00007bc0: 7d2c 0a0a 2020 2020 616e 6420 3a6d 6174  },..    and :mat
+00007bd0: 683a 6056 5e7b 2867 297d 6020 6973 2074  h:`V^{(g)}` is t
+00007be0: 6865 206d 6174 7269 7820 6f66 2065 6967  he matrix of eig
+00007bf0: 656e 7665 6374 6f72 7320 7468 6174 2064  envectors that d
+00007c00: 6961 676f 6e61 6c69 7a65 730a 2020 2020  iagonalizes.    
+00007c10: 3a6d 6174 683a 605c 7469 6c64 657b 5c6d  :math:`\tilde{\m
+00007c20: 6174 6863 616c 7b48 7d7d 5f6e 5e7b 2867  athcal{H}}_n^{(g
+00007c30: 297d 602c 203a 6d61 7468 3a60 425f 5c61  )}`, :math:`B_\a
+00007c40: 6c70 6861 6020 7468 650a 2020 2020 3a6d  lpha` the.    :m
+00007c50: 6174 683a 605c 616c 7068 6160 2d74 6820  ath:`\alpha`-th 
+00007c60: 6e6f 6973 6520 6f70 6572 6174 6f72 203a  noise operator :
+00007c70: 6d61 7468 3a60 735f 5c61 6c70 6861 5e7b  math:`s_\alpha^{
+00007c80: 2867 297d 6020 7468 6520 6e6f 6973 650a  (g)}` the noise.
+00007c90: 2020 2020 7365 6e73 6974 6976 6974 7920      sensitivity 
+00007ca0: 6475 7269 6e67 2069 6e74 6572 7661 6c20  during interval 
+00007cb0: 3a6d 6174 683a 6067 602c 2061 6e64 203a  :math:`g`, and :
+00007cc0: 6d61 7468 3a60 435f 6b60 2074 6865 0a20  math:`C_k` the. 
+00007cd0: 2020 203a 6d61 7468 3a60 6b60 2d74 6820     :math:`k`-th 
+00007ce0: 6261 7369 7320 656c 656d 656e 742e 0a0a  basis element...
+00007cf0: 2020 2020 5365 6520 416c 736f 0a20 2020      See Also.   
+00007d00: 202d 2d2d 2d2d 2d2d 2d0a 2020 2020 6361   --------.    ca
+00007d10: 6c63 756c 6174 655f 636f 6e74 726f 6c5f  lculate_control_
+00007d20: 6d61 7472 6978 5f66 726f 6d5f 6174 6f6d  matrix_from_atom
+00007d30: 6963 3a20 436f 6e74 726f 6c20 6d61 7472  ic: Control matr
+00007d40: 6978 2066 726f 6d20 636f 6e63 6174 656e  ix from concaten
+00007d50: 6174 696f 6e2e 0a20 2020 2063 616c 6375  ation..    calcu
+00007d60: 6c61 7465 5f63 6f6e 7472 6f6c 5f6d 6174  late_control_mat
+00007d70: 7269 785f 7065 7269 6f64 6963 3a20 436f  rix_periodic: Co
+00007d80: 6e74 726f 6c20 6d61 7472 6978 2066 6f72  ntrol matrix for
+00007d90: 2070 6572 696f 6469 6320 7379 7374 656d   periodic system
+00007da0: 2e0a 2020 2020 2222 220a 2020 2020 6420  ..    """.    d 
+00007db0: 3d20 6569 6776 6563 732e 7368 6170 655b  = eigvecs.shape[
+00007dc0: 2d31 5d0a 0a20 2020 2069 6620 7420 6973  -1]..    if t is
+00007dd0: 204e 6f6e 653a 0a20 2020 2020 2020 2074   None:.        t
+00007de0: 203d 206e 702e 636f 6e63 6174 656e 6174   = np.concatenat
+00007df0: 6528 285b 305d 2c20 6e70 2e61 7361 7272  e(([0], np.asarr
+00007e00: 6179 2864 7429 2e63 756d 7375 6d28 2929  ay(dt).cumsum())
+00007e10: 290a 0a20 2020 2023 2050 7265 636f 6d70  )..    # Precomp
+00007e20: 7574 6520 6e6f 6973 6520 6f70 6572 7320  ute noise opers 
+00007e30: 7472 616e 7366 6f72 6d65 6420 746f 2065  transformed to e
+00007e40: 6967 656e 6261 7369 7320 6f66 2065 6163  igenbasis of eac
+00007e50: 6820 7075 6c73 6520 7365 676d 656e 740a  h pulse segment.
+00007e60: 2020 2020 2320 616e 6420 515e 5c64 6167      # and Q^\dag
+00007e70: 6765 7220 4020 560a 2020 2020 6569 6776  ger @ V.    eigv
+00007e80: 6563 735f 7072 6f70 6167 6174 6564 203d  ecs_propagated =
+00007e90: 205f 7072 6f70 6167 6174 655f 6569 6765   _propagate_eige
+00007ea0: 6e76 6563 746f 7273 2870 726f 7061 6761  nvectors(propaga
+00007eb0: 746f 7273 5b3a 2d31 5d2c 2065 6967 7665  tors[:-1], eigve
+00007ec0: 6373 290a 2020 2020 6e5f 6f70 6572 735f  cs).    n_opers_
+00007ed0: 7472 616e 7366 6f72 6d65 6420 3d20 5f74  transformed = _t
+00007ee0: 7261 6e73 666f 726d 5f68 616d 696c 746f  ransform_hamilto
+00007ef0: 6e69 616e 2865 6967 7665 6373 2c20 6e5f  nian(eigvecs, n_
+00007f00: 6f70 6572 732c 206e 5f63 6f65 6666 7329  opers, n_coeffs)
+00007f10: 0a0a 2020 2020 2320 416c 6c6f 6361 7465  ..    # Allocate
+00007f20: 2072 6573 756c 7420 616e 6420 6275 6666   result and buff
+00007f30: 6572 7320 666f 7220 696e 7465 726d 6564  ers for intermed
+00007f40: 6961 7465 2061 7272 6179 730a 2020 2020  iate arrays.    
+00007f50: 6578 705f 6275 6620 3d20 6e70 2e65 6d70  exp_buf = np.emp
+00007f60: 7479 2828 6c65 6e28 6f6d 6567 6129 2c20  ty((len(omega), 
+00007f70: 642c 2064 292c 2064 7479 7065 3d63 6f6d  d, d), dtype=com
+00007f80: 706c 6578 290a 2020 2020 6966 206f 7574  plex).    if out
+00007f90: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+00007fa0: 2020 6f75 7420 3d20 6e70 2e7a 6572 6f73    out = np.zeros
+00007fb0: 2828 6c65 6e28 6e5f 6f70 6572 7329 2c20  ((len(n_opers), 
+00007fc0: 6c65 6e28 6261 7369 7329 2c20 6c65 6e28  len(basis), len(
+00007fd0: 6f6d 6567 6129 292c 2064 7479 7065 3d63  omega)), dtype=c
+00007fe0: 6f6d 706c 6578 290a 0a20 2020 2069 6620  omplex)..    if 
+00007ff0: 6361 6368 655f 696e 7465 726d 6564 6961  cache_intermedia
+00008000: 7465 733a 0a20 2020 2020 2020 2062 6173  tes:.        bas
+00008010: 6973 5f74 7261 6e73 666f 726d 6564 5f63  is_transformed_c
+00008020: 6163 6865 203d 206e 702e 656d 7074 7928  ache = np.empty(
+00008030: 286c 656e 2864 7429 2c20 2a62 6173 6973  (len(dt), *basis
+00008040: 2e73 6861 7065 292c 2064 7479 7065 3d63  .shape), dtype=c
+00008050: 6f6d 706c 6578 290a 2020 2020 2020 2020  omplex).        
+00008060: 7068 6173 655f 6661 6374 6f72 735f 6361  phase_factors_ca
+00008070: 6368 6520 3d20 6e70 2e65 6d70 7479 2828  che = np.empty((
+00008080: 6c65 6e28 6474 292c 206c 656e 286f 6d65  len(dt), len(ome
+00008090: 6761 2929 2c20 6474 7970 653d 636f 6d70  ga)), dtype=comp
+000080a0: 6c65 7829 0a20 2020 2020 2020 2069 6e74  lex).        int
+000080b0: 5f63 6163 6865 203d 206e 702e 656d 7074  _cache = np.empt
+000080c0: 7928 286c 656e 2864 7429 2c20 6c65 6e28  y((len(dt), len(
+000080d0: 6f6d 6567 6129 2c20 642c 2064 292c 2064  omega), d, d), d
+000080e0: 7479 7065 3d63 6f6d 706c 6578 290a 2020  type=complex).  
+000080f0: 2020 2020 2020 7375 6d5f 6361 6368 6520        sum_cache 
+00008100: 3d20 6e70 2e65 6d70 7479 2828 6c65 6e28  = np.empty((len(
+00008110: 6474 292c 206c 656e 286e 5f6f 7065 7273  dt), len(n_opers
+00008120: 292c 206c 656e 2862 6173 6973 292c 206c  ), len(basis), l
+00008130: 656e 286f 6d65 6761 2929 2c20 6474 7970  en(omega)), dtyp
+00008140: 653d 636f 6d70 6c65 7829 0a20 2020 2065  e=complex).    e
+00008150: 6c73 653a 0a20 2020 2020 2020 2062 6173  lse:.        bas
+00008160: 6973 5f74 7261 6e73 666f 726d 6564 203d  is_transformed =
+00008170: 206e 702e 656d 7074 7928 6261 7369 732e   np.empty(basis.
+00008180: 7368 6170 652c 2064 7479 7065 3d63 6f6d  shape, dtype=com
+00008190: 706c 6578 290a 2020 2020 2020 2020 7068  plex).        ph
+000081a0: 6173 655f 6661 6374 6f72 7320 3d20 6e70  ase_factors = np
+000081b0: 2e65 6d70 7479 286c 656e 286f 6d65 6761  .empty(len(omega
+000081c0: 292c 2064 7479 7065 3d63 6f6d 706c 6578  ), dtype=complex
+000081d0: 290a 2020 2020 2020 2020 696e 745f 6275  ).        int_bu
+000081e0: 6620 3d20 6e70 2e65 6d70 7479 2828 6c65  f = np.empty((le
+000081f0: 6e28 6f6d 6567 6129 2c20 642c 2064 292c  n(omega), d, d),
+00008200: 2064 7479 7065 3d63 6f6d 706c 6578 290a   dtype=complex).
+00008210: 2020 2020 2020 2020 7375 6d5f 6275 6620          sum_buf 
+00008220: 3d20 6e70 2e65 6d70 7479 2828 6c65 6e28  = np.empty((len(
+00008230: 6e5f 6f70 6572 7329 2c20 6c65 6e28 6261  n_opers), len(ba
+00008240: 7369 7329 2c20 6c65 6e28 6f6d 6567 6129  sis), len(omega)
+00008250: 292c 2064 7479 7065 3d63 6f6d 706c 6578  ), dtype=complex
+00008260: 290a 0a20 2020 2023 204f 7074 696d 697a  )..    # Optimiz
+00008270: 6520 7468 6520 636f 6e74 7261 6374 696f  e the contractio
+00008280: 6e20 7061 7468 2064 796e 616d 6963 616c  n path dynamical
+00008290: 6c79 2073 696e 6365 2069 7420 6469 6666  ly since it diff
+000082a0: 6572 7320 666f 7220 6469 6666 6572 656e  ers for differen
+000082b0: 740a 2020 2020 2320 7661 6c75 6573 206f  t.    # values o
+000082c0: 6620 640a 2020 2020 6578 7072 203d 206f  f d.    expr = o
+000082d0: 652e 636f 6e74 7261 6374 5f65 7870 7265  e.contract_expre
+000082e0: 7373 696f 6e28 276f 2c6a 6d6e 2c6f 6d6e  ssion('o,jmn,omn
+000082f0: 2c6b 6e6d 2d3e 6a6b 6f27 2c0a 2020 2020  ,knm->jko',.    
+00008300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008310: 2020 2020 2020 2020 2020 2020 2020 6f6d                om
+00008320: 6567 612e 7368 6170 652c 206e 5f6f 7065  ega.shape, n_ope
+00008330: 7273 5f74 7261 6e73 666f 726d 6564 5b3a  rs_transformed[:
+00008340: 2c20 305d 2e73 6861 7065 2c0a 2020 2020  , 0].shape,.    
+00008350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008360: 2020 2020 2020 2020 2020 2020 2020 6578                ex
+00008370: 705f 6275 662e 7368 6170 652c 2062 6173  p_buf.shape, bas
+00008380: 6973 2e73 6861 7065 2c20 6f70 7469 6d69  is.shape, optimi
+00008390: 7a65 3d54 7275 6529 0a20 2020 2066 6f72  ze=True).    for
+000083a0: 2067 2069 6e20 7574 696c 2e70 726f 6772   g in util.progr
+000083b0: 6573 7362 6172 5f72 616e 6765 286c 656e  essbar_range(len
+000083c0: 2864 7429 2c20 7368 6f77 5f70 726f 6772  (dt), show_progr
+000083d0: 6573 7362 6172 3d73 686f 775f 7072 6f67  essbar=show_prog
+000083e0: 7265 7373 6261 722c 0a20 2020 2020 2020  ressbar,.       
 000083f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008400: 2020 2020 2065 7870 5f62 7566 2e73 6861       exp_buf.sha
-00008410: 7065 2c20 6261 7369 732e 7368 6170 652c  pe, basis.shape,
-00008420: 206f 7074 696d 697a 653d 5472 7565 290a   optimize=True).
-00008430: 2020 2020 666f 7220 6720 696e 2075 7469      for g in uti
-00008440: 6c2e 7072 6f67 7265 7373 6261 725f 7261  l.progressbar_ra
-00008450: 6e67 6528 6c65 6e28 6474 292c 2073 686f  nge(len(dt), sho
-00008460: 775f 7072 6f67 7265 7373 6261 723d 7368  w_progressbar=sh
-00008470: 6f77 5f70 726f 6772 6573 7362 6172 2c0a  ow_progressbar,.
-00008480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000084a0: 2020 2020 6465 7363 3d27 4361 6c63 756c      desc='Calcul
-000084b0: 6174 696e 6720 636f 6e74 726f 6c20 6d61  ating control ma
-000084c0: 7472 6978 2729 3a0a 0a20 2020 2020 2020  trix'):..       
-000084d0: 2069 6620 6361 6368 655f 696e 7465 726d   if cache_interm
-000084e0: 6564 6961 7465 733a 0a20 2020 2020 2020  ediates:.       
-000084f0: 2020 2020 2023 2041 7373 6967 6e20 7265       # Assign re
-00008500: 6665 7265 6e63 6573 2074 6f20 7468 6520  ferences to the 
-00008510: 6c6f 6361 7469 6f6e 7320 696e 2074 6865  locations in the
-00008520: 2063 6163 6865 2066 6f72 2074 6865 2071   cache for the q
-00008530: 7561 6e74 6974 6965 730a 2020 2020 2020  uantities.      
-00008540: 2020 2020 2020 2320 7468 6174 2073 686f        # that sho
-00008550: 756c 6420 6265 2073 746f 7265 640a 2020  uld be stored.  
-00008560: 2020 2020 2020 2020 2020 6261 7369 735f            basis_
-00008570: 7472 616e 7366 6f72 6d65 6420 3d20 6261  transformed = ba
-00008580: 7369 735f 7472 616e 7366 6f72 6d65 645f  sis_transformed_
-00008590: 6361 6368 655b 675d 0a20 2020 2020 2020  cache[g].       
-000085a0: 2020 2020 2070 6861 7365 5f66 6163 746f       phase_facto
-000085b0: 7273 203d 2070 6861 7365 5f66 6163 746f  rs = phase_facto
-000085c0: 7273 5f63 6163 6865 5b67 5d0a 2020 2020  rs_cache[g].    
-000085d0: 2020 2020 2020 2020 696e 745f 6275 6620          int_buf 
-000085e0: 3d20 696e 745f 6361 6368 655b 675d 0a20  = int_cache[g]. 
-000085f0: 2020 2020 2020 2020 2020 2073 756d 5f62             sum_b
-00008600: 7566 203d 2073 756d 5f63 6163 6865 5b67  uf = sum_cache[g
-00008610: 5d0a 0a20 2020 2020 2020 2062 6173 6973  ]..        basis
-00008620: 5f74 7261 6e73 666f 726d 6564 203d 205f  _transformed = _
-00008630: 7472 616e 7366 6f72 6d5f 6279 5f75 6e69  transform_by_uni
-00008640: 7461 7279 2865 6967 7665 6373 5f70 726f  tary(eigvecs_pro
-00008650: 7061 6761 7465 645b 675d 2c20 6261 7369  pagated[g], basi
-00008660: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
-00008670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008690: 2020 2020 206f 7574 3d62 6173 6973 5f74       out=basis_t
-000086a0: 7261 6e73 666f 726d 6564 290a 2020 2020  ransformed).    
-000086b0: 2020 2020 7068 6173 655f 6661 6374 6f72      phase_factor
-000086c0: 7320 3d20 7574 696c 2e63 6578 7028 6f6d  s = util.cexp(om
-000086d0: 6567 612a 745b 675d 2c20 6f75 743d 7068  ega*t[g], out=ph
-000086e0: 6173 655f 6661 6374 6f72 7329 0a20 2020  ase_factors).   
-000086f0: 2020 2020 2069 6e74 5f62 7566 203d 205f       int_buf = _
-00008700: 6669 7273 745f 6f72 6465 725f 696e 7465  first_order_inte
-00008710: 6772 616c 286f 6d65 6761 2c20 6569 6776  gral(omega, eigv
-00008720: 616c 735b 675d 2c20 6474 5b67 5d2c 2065  als[g], dt[g], e
-00008730: 7870 5f62 7566 2c20 696e 745f 6275 6629  xp_buf, int_buf)
-00008740: 0a20 2020 2020 2020 2073 756d 5f62 7566  .        sum_buf
-00008750: 203d 2065 7870 7228 7068 6173 655f 6661   = expr(phase_fa
-00008760: 6374 6f72 732c 206e 5f6f 7065 7273 5f74  ctors, n_opers_t
-00008770: 7261 6e73 666f 726d 6564 5b3a 2c20 675d  ransformed[:, g]
-00008780: 2c20 696e 745f 6275 662c 0a20 2020 2020  , int_buf,.     
-00008790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000087a0: 2020 6261 7369 735f 7472 616e 7366 6f72    basis_transfor
-000087b0: 6d65 642c 206f 7574 3d73 756d 5f62 7566  med, out=sum_buf
-000087c0: 290a 0a20 2020 2020 2020 206f 7574 202b  )..        out +
-000087d0: 3d20 7375 6d5f 6275 660a 0a20 2020 2069  = sum_buf..    i
-000087e0: 6620 6361 6368 655f 696e 7465 726d 6564  f cache_intermed
-000087f0: 6961 7465 733a 0a20 2020 2020 2020 2069  iates:.        i
-00008800: 6e74 6572 6d65 6469 6174 6573 203d 2064  ntermediates = d
-00008810: 6963 7428 6e5f 6f70 6572 735f 7472 616e  ict(n_opers_tran
-00008820: 7366 6f72 6d65 643d 6e5f 6f70 6572 735f  sformed=n_opers_
-00008830: 7472 616e 7366 6f72 6d65 642c 0a20 2020  transformed,.   
-00008840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008850: 2020 2020 2020 2020 2020 6261 7369 735f            basis_
-00008860: 7472 616e 7366 6f72 6d65 643d 6261 7369  transformed=basi
-00008870: 735f 7472 616e 7366 6f72 6d65 645f 6361  s_transformed_ca
-00008880: 6368 652c 0a20 2020 2020 2020 2020 2020  che,.           
-00008890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000088a0: 2020 7068 6173 655f 6661 6374 6f72 733d    phase_factors=
-000088b0: 7068 6173 655f 6661 6374 6f72 735f 6361  phase_factors_ca
-000088c0: 6368 652c 0a20 2020 2020 2020 2020 2020  che,.           
-000088d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000088e0: 2020 6669 7273 745f 6f72 6465 725f 696e    first_order_in
-000088f0: 7465 6772 616c 3d69 6e74 5f63 6163 6865  tegral=int_cache
-00008900: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00008910: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00008920: 6f6e 7472 6f6c 5f6d 6174 7269 785f 7374  ontrol_matrix_st
-00008930: 6570 3d73 756d 5f63 6163 6865 290a 2020  ep=sum_cache).  
-00008940: 2020 2020 2020 7265 7475 726e 206f 7574        return out
-00008950: 2c20 696e 7465 726d 6564 6961 7465 730a  , intermediates.
-00008960: 0a20 2020 2072 6574 7572 6e20 6f75 740a  .    return out.
-00008970: 0a0a 6465 6620 6361 6c63 756c 6174 655f  ..def calculate_
-00008980: 636f 6e74 726f 6c5f 6d61 7472 6978 5f70  control_matrix_p
-00008990: 6572 696f 6469 6328 7068 6173 6573 3a20  eriodic(phases: 
-000089a0: 6e64 6172 7261 792c 2063 6f6e 7472 6f6c  ndarray, control
-000089b0: 5f6d 6174 7269 783a 206e 6461 7272 6179  _matrix: ndarray
-000089c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000089d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000089e0: 2020 2020 2020 2020 746f 7461 6c5f 7072          total_pr
-000089f0: 6f70 6167 6174 6f72 5f6c 696f 7576 696c  opagator_liouvil
-00008a00: 6c65 3a20 6e64 6172 7261 792c 0a20 2020  le: ndarray,.   
-00008a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a30: 2020 2072 6570 6561 7473 3a20 696e 742c     repeats: int,
-00008a40: 2063 6865 636b 5f69 6e76 6572 7469 626c   check_invertibl
-00008a50: 653a 2062 6f6f 6c20 3d20 5472 7565 2920  e: bool = True) 
-00008a60: 2d3e 206e 6461 7272 6179 3a0a 2020 2020  -> ndarray:.    
-00008a70: 7222 2222 0a20 2020 2043 616c 6375 6c61  r""".    Calcula
-00008a80: 7465 2074 6865 2063 6f6e 7472 6f6c 206d  te the control m
-00008a90: 6174 7269 7820 6f66 2061 2070 6572 696f  atrix of a perio
-00008aa0: 6469 6320 7075 6c73 6520 6769 7665 6e20  dic pulse given 
-00008ab0: 7468 6520 7068 6173 650a 2020 2020 6661  the phase.    fa
-00008ac0: 6374 6f72 732c 2063 6f6e 7472 6f6c 206d  ctors, control m
-00008ad0: 6174 7269 7820 616e 6420 7472 616e 7366  atrix and transf
-00008ae0: 6572 206d 6174 7269 7820 6f66 2074 6865  er matrix of the
-00008af0: 2074 6f74 616c 2070 726f 7061 6761 746f   total propagato
-00008b00: 722c 0a20 2020 2074 6f74 616c 5f70 726f  r,.    total_pro
-00008b10: 7061 6761 746f 725f 6c69 6f75 7669 6c6c  pagator_liouvill
-00008b20: 652c 206f 6620 7468 6520 6174 6f6d 6963  e, of the atomic
-00008b30: 2070 756c 7365 2e0a 0a20 2020 2050 6172   pulse...    Par
-00008b40: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
-00008b50: 2d2d 2d2d 2d2d 0a20 2020 2070 6861 7365  ------.    phase
-00008b60: 733a 206e 6461 7272 6179 2c20 7368 6170  s: ndarray, shap
-00008b70: 6520 286e 5f6f 6d65 6761 2c29 0a20 2020  e (n_omega,).   
-00008b80: 2020 2020 2054 6865 2070 6861 7365 2066       The phase f
-00008b90: 6163 746f 7273 203a 6d61 7468 3a60 655e  actors :math:`e^
-00008ba0: 7b69 5c6f 6d65 6761 2054 7d60 206f 6620  {i\omega T}` of 
-00008bb0: 7468 6520 6174 6f6d 6963 2070 756c 7365  the atomic pulse
-00008bc0: 2e0a 2020 2020 636f 6e74 726f 6c5f 6d61  ..    control_ma
-00008bd0: 7472 6978 3a20 6e64 6172 7261 792c 2073  trix: ndarray, s
-00008be0: 6861 7065 2028 6e5f 6e6f 7073 2c20 642a  hape (n_nops, d*
-00008bf0: 2a32 2c20 6e5f 6f6d 6567 6129 0a20 2020  *2, n_omega).   
-00008c00: 2020 2020 2054 6865 2063 6f6e 7472 6f6c       The control
-00008c10: 206d 6174 7269 7820 3a6d 6174 683a 605c   matrix :math:`\
-00008c20: 7469 6c64 657b 5c6d 6174 6863 616c 7b42  tilde{\mathcal{B
-00008c30: 7d7d 5e7b 2831 297d 285c 6f6d 6567 6129  }}^{(1)}(\omega)
-00008c40: 6020 6f66 0a20 2020 2020 2020 2074 6865  ` of.        the
-00008c50: 2061 746f 6d69 6320 7075 6c73 652e 0a20   atomic pulse.. 
-00008c60: 2020 2074 6f74 616c 5f70 726f 7061 6761     total_propaga
-00008c70: 746f 725f 6c69 6f75 7669 6c6c 653a 206e  tor_liouville: n
-00008c80: 6461 7272 6179 2c20 7368 6170 6520 2864  darray, shape (d
-00008c90: 2a2a 322c 2064 2a2a 3229 0a20 2020 2020  **2, d**2).     
-00008ca0: 2020 2054 6865 2074 7261 6e73 6665 7220     The transfer 
-00008cb0: 6d61 7472 6978 203a 6d61 7468 3a60 5c6d  matrix :math:`\m
-00008cc0: 6174 6863 616c 7b51 7d5e 7b28 3129 7d60  athcal{Q}^{(1)}`
-00008cd0: 206f 6620 7468 6520 6174 6f6d 6963 0a20   of the atomic. 
-00008ce0: 2020 2020 2020 2070 756c 7365 2e0a 2020         pulse..  
-00008cf0: 2020 7265 7065 6174 733a 2069 6e74 0a20    repeats: int. 
-00008d00: 2020 2020 2020 2054 6865 206e 756d 6265         The numbe
-00008d10: 7220 6f66 2072 6570 6574 6974 696f 6e73  r of repetitions
-00008d20: 2e0a 2020 2020 6368 6563 6b5f 696e 7665  ..    check_inve
-00008d30: 7274 6962 6c65 3a20 626f 6f6c 2c20 6f70  rtible: bool, op
-00008d40: 7469 6f6e 616c 0a20 2020 2020 2020 2043  tional.        C
-00008d50: 6865 636b 2066 6f72 2061 6c6c 2066 7265  heck for all fre
-00008d60: 7175 656e 6369 6573 2069 6620 7468 6520  quencies if the 
-00008d70: 696e 7665 7273 6520 3a6d 6174 683a 605c  inverse :math:`\
-00008d80: 6d61 7468 6262 7b49 7d20 2d0a 2020 2020  mathbb{I} -.    
-00008d90: 2020 2020 655e 7b69 5c6f 6d65 6761 2054      e^{i\omega T
-00008da0: 7d20 5c6d 6174 6863 616c 7b51 7d5e 7b28  } \mathcal{Q}^{(
-00008db0: 3129 7d60 2065 7869 7374 7320 6279 2063  1)}` exists by c
-00008dc0: 616c 6375 6c61 7469 6e67 2074 6865 0a20  alculating the. 
-00008dd0: 2020 2020 2020 2064 6574 6572 6d69 6e61         determina
-00008de0: 6e74 2e20 4966 2069 7420 646f 6573 206e  nt. If it does n
-00008df0: 6f74 2065 7869 7374 2c20 7468 6520 7375  ot exist, the su
-00008e00: 6d20 6973 2065 7661 6c75 6174 6564 0a20  m is evaluated. 
-00008e10: 2020 2020 2020 2065 7870 6c69 6369 746c         explicitl
-00008e20: 7920 666f 7220 7468 6f73 6520 706f 696e  y for those poin
-00008e30: 7473 2e20 5468 6520 6465 6661 756c 7420  ts. The default 
-00008e40: 6973 2054 7275 652e 0a0a 2020 2020 5265  is True...    Re
-00008e50: 7475 726e 730a 2020 2020 2d2d 2d2d 2d2d  turns.    ------
-00008e60: 2d0a 2020 2020 636f 6e74 726f 6c5f 6d61  -.    control_ma
-00008e70: 7472 6978 3a20 6e64 6172 7261 792c 2073  trix: ndarray, s
-00008e80: 6861 7065 2028 6e5f 6e6f 7073 2c20 642a  hape (n_nops, d*
-00008e90: 2a32 2c20 6e5f 6f6d 6567 6129 0a20 2020  *2, n_omega).   
-00008ea0: 2020 2020 2054 6865 2063 6f6e 7472 6f6c       The control
-00008eb0: 206d 6174 7269 7820 3a6d 6174 683a 605c   matrix :math:`\
-00008ec0: 7469 6c64 657b 5c6d 6174 6863 616c 7b42  tilde{\mathcal{B
-00008ed0: 7d7d 285c 6f6d 6567 6129 6020 6f66 2074  }}(\omega)` of t
-00008ee0: 6865 0a20 2020 2020 2020 2072 6570 6561  he.        repea
-00008ef0: 7465 6420 7075 6c73 652e 0a0a 2020 2020  ted pulse...    
-00008f00: 4e6f 7465 730a 2020 2020 2d2d 2d2d 2d0a  Notes.    -----.
-00008f10: 2020 2020 5468 6520 636f 6e74 726f 6c20      The control 
-00008f20: 6d61 7472 6978 2069 7320 636f 6d70 7574  matrix is comput
-00008f30: 6564 2061 730a 0a20 2020 202e 2e20 6d61  ed as..    .. ma
-00008f40: 7468 3a3a 0a0a 2020 2020 2020 2020 5c74  th::..        \t
-00008f50: 696c 6465 7b5c 6d61 7468 6361 6c7b 427d  ilde{\mathcal{B}
-00008f60: 7d28 5c6f 6d65 6761 290a 2020 2020 2020  }(\omega).      
-00008f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f80: 2020 2020 2020 263d 205c 7469 6c64 657b        &= \tilde{
-00008f90: 5c6d 6174 6863 616c 7b42 7d7d 5e7b 2831  \mathcal{B}}^{(1
-00008fa0: 297d 285c 6f6d 6567 6129 0a20 2020 2020  )}(\omega).     
-00008fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008fc0: 2020 2020 2020 2020 2020 5c73 756d 5f7b            \sum_{
-00008fd0: 673d 307d 5e7b 472d 317d 0a20 2020 2020  g=0}^{G-1}.     
-00008fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ff0: 2020 2020 2020 2020 2020 5c6c 6566 7428            \left(
-00009000: 655e 7b69 5c6f 6d65 6761 2054 7d5c 7269  e^{i\omega T}\ri
-00009010: 6768 7429 5e67 205c 5c0a 2020 2020 2020  ght)^g \\.      
-00009020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009030: 2020 2020 2020 263d 205c 7469 6c64 657b        &= \tilde{
-00009040: 5c6d 6174 6863 616c 7b42 7d7d 5e7b 2831  \mathcal{B}}^{(1
-00009050: 297d 285c 6f6d 6567 6129 5c62 6967 6c28  )}(\omega)\bigl(
-00009060: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009080: 5c6d 6174 6862 627b 497d 202d 2065 5e7b  \mathbb{I} - e^{
-00009090: 695c 6f6d 6567 6120 547d 0a20 2020 2020  i\omega T}.     
-000090a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000090b0: 2020 2020 2020 2020 2020 5c6d 6174 6863            \mathc
-000090c0: 616c 7b51 7d5e 7b28 3129 7d5c 6269 6772  al{Q}^{(1)}\bigr
-000090d0: 295e 7b2d 317d 5c62 6967 6c28 0a20 2020  )^{-1}\bigl(.   
-000090e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000090f0: 2020 2020 2020 2020 2020 2020 5c6d 6174              \mat
-00009100: 6862 627b 497d 202d 205c 6269 676c 2865  hbb{I} - \bigl(e
-00009110: 5e7b 695c 6f6d 6567 6120 547d 0a20 2020  ^{i\omega T}.   
-00009120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009130: 2020 2020 2020 2020 2020 2020 5c6d 6174              \mat
-00009140: 6863 616c 7b51 7d5e 7b28 3129 7d5c 6269  hcal{Q}^{(1)}\bi
-00009150: 6772 295e 475c 6269 6772 292e 0a0a 2020  gr)^G\bigr)...  
-00009160: 2020 7769 7468 203a 6d61 7468 3a60 4760    with :math:`G`
-00009170: 2074 6865 206e 756d 6265 7220 6f66 2072   the number of r
-00009180: 6570 6574 6974 696f 6e73 2e0a 2020 2020  epetitions..    
-00009190: 2222 220a 2020 2020 2320 436f 6d70 7574  """.    # Comput
-000091a0: 6520 7468 6520 6669 6e69 7465 2067 656f  e the finite geo
-000091b0: 6d65 7472 6963 2073 6572 6965 7320 5c73  metric series \s
-000091c0: 756d 5f7b 673d 307d 5e7b 472d 317d 2054  um_{g=0}^{G-1} T
-000091d0: 5e67 2e20 4669 7273 7420 6368 6563 6b20  ^g. First check 
-000091e0: 6966 0a20 2020 2023 2069 6e76 2849 202d  if.    # inv(I -
-000091f0: 2054 2920 6973 2027 676f 6f64 272c 2069   T) is 'good', i
-00009200: 2e65 2e20 6966 2069 6e76 2849 202d 2054  .e. if inv(I - T
-00009210: 2920 4020 2849 202d 2054 2920 3d3d 2049  ) @ (I - T) == I
-00009220: 2c20 7369 6e63 6520 4e75 6d50 7920 7769  , since NumPy wi
-00009230: 6c6c 0a20 2020 2023 2063 6f6d 7075 7465  ll.    # compute
-00009240: 2074 6865 2069 6e76 6572 7365 2069 6e20   the inverse in 
-00009250: 616e 7920 6361 7365 2e20 466f 7220 7468  any case. For th
-00009260: 6f73 6520 6672 6571 7565 6e63 6965 7320  ose frequencies 
-00009270: 7768 6572 6520 7468 6520 696e 7665 7273  where the invers
-00009280: 650a 2020 2020 2320 6973 2077 656c 6c2d  e.    # is well-
-00009290: 6265 6861 7665 642c 2065 7661 6c75 6174  behaved, evaluat
-000092a0: 6520 7468 6520 7375 6d20 6173 2061 204e  e the sum as a N
-000092b0: 6575 6d61 6e6e 2073 6572 6965 7320 616e  eumann series an
-000092c0: 6420 666f 7220 7468 6520 7265 7374 0a20  d for the rest. 
-000092d0: 2020 2023 2065 7661 6c75 6174 6520 6974     # evaluate it
-000092e0: 2065 7870 6c69 6369 746c 792e 0a20 2020   explicitly..   
-000092f0: 2065 7965 203d 206e 702e 6579 6528 746f   eye = np.eye(to
-00009300: 7461 6c5f 7072 6f70 6167 6174 6f72 5f6c  tal_propagator_l
-00009310: 696f 7576 696c 6c65 2e73 6861 7065 5b30  iouville.shape[0
-00009320: 5d29 0a20 2020 2054 203d 206e 702e 6d75  ]).    T = np.mu
-00009330: 6c74 6970 6c79 2e6f 7574 6572 2870 6861  ltiply.outer(pha
-00009340: 7365 732c 2074 6f74 616c 5f70 726f 7061  ses, total_propa
-00009350: 6761 746f 725f 6c69 6f75 7669 6c6c 6529  gator_liouville)
-00009360: 0a20 2020 204d 203d 2065 7965 202d 2054  .    M = eye - T
-00009370: 0a20 2020 2069 6620 6368 6563 6b5f 696e  .    if check_in
-00009380: 7665 7274 6962 6c65 3a0a 2020 2020 2020  vertible:.      
-00009390: 2020 696e 7665 7274 6962 6c65 203d 207e    invertible = ~
-000093a0: 6e70 2e69 7363 6c6f 7365 286e 6c61 2e64  np.isclose(nla.d
-000093b0: 6574 284d 292c 2030 290a 2020 2020 656c  et(M), 0).    el
-000093c0: 7365 3a0a 2020 2020 2020 2020 696e 7665  se:.        inve
-000093d0: 7274 6962 6c65 203d 206e 702e 6172 7261  rtible = np.arra
-000093e0: 7928 5472 7565 290a 0a20 2020 2053 203d  y(True)..    S =
-000093f0: 206e 702e 656d 7074 7928 282a 7068 6173   np.empty((*phas
-00009400: 6573 2e73 6861 7065 2c20 2a74 6f74 616c  es.shape, *total
-00009410: 5f70 726f 7061 6761 746f 725f 6c69 6f75  _propagator_liou
-00009420: 7669 6c6c 652e 7368 6170 6529 2c20 6474  ville.shape), dt
-00009430: 7970 653d 636f 6d70 6c65 7829 0a20 2020  ype=complex).   
-00009440: 2023 2053 6f6c 7665 204c 5345 2069 6e73   # Solve LSE ins
-00009450: 7465 6164 206f 6620 636f 6d70 7574 696e  tead of computin
-00009460: 6720 696e 7665 7273 652c 2066 6173 7465  g inverse, faste
-00009470: 7220 2b20 6e75 6d65 7269 6361 6c6c 7920  r + numerically 
-00009480: 6d6f 7265 2073 7461 626c 650a 2020 2020  more stable.    
-00009490: 535b 696e 7665 7274 6962 6c65 5d20 3d20  S[invertible] = 
-000094a0: 6e6c 612e 736f 6c76 6528 4d5b 696e 7665  nla.solve(M[inve
-000094b0: 7274 6962 6c65 5d2c 2065 7965 202d 206e  rtible], eye - n
-000094c0: 6c61 2e6d 6174 7269 785f 706f 7765 7228  la.matrix_power(
-000094d0: 545b 696e 7665 7274 6962 6c65 5d2c 2072  T[invertible], r
-000094e0: 6570 6561 7473 2929 0a20 2020 2069 6620  epeats)).    if 
-000094f0: 287e 696e 7665 7274 6962 6c65 292e 616e  (~invertible).an
-00009500: 7928 293a 0a20 2020 2020 2020 2053 5b7e  y():.        S[~
-00009510: 696e 7665 7274 6962 6c65 5d20 3d20 6579  invertible] = ey
-00009520: 6520 2b20 7375 6d28 6163 6375 6d75 6c61  e + sum(accumula
-00009530: 7465 2872 6570 6561 7428 545b 7e69 6e76  te(repeat(T[~inv
-00009540: 6572 7469 626c 655d 2c20 7265 7065 6174  ertible], repeat
-00009550: 732d 3129 2c20 6e70 2e6d 6174 6d75 6c29  s-1), np.matmul)
-00009560: 290a 0a20 2020 2063 6f6e 7472 6f6c 5f6d  )..    control_m
-00009570: 6174 7269 785f 746f 7420 3d20 2863 6f6e  atrix_tot = (con
-00009580: 7472 6f6c 5f6d 6174 7269 782e 7472 616e  trol_matrix.tran
-00009590: 7370 6f73 6528 322c 2030 2c20 3129 2040  spose(2, 0, 1) @
-000095a0: 2053 292e 7472 616e 7370 6f73 6528 312c   S).transpose(1,
-000095b0: 2032 2c20 3029 0a20 2020 2072 6574 7572   2, 0).    retur
-000095c0: 6e20 636f 6e74 726f 6c5f 6d61 7472 6978  n control_matrix
-000095d0: 5f74 6f74 0a0a 0a40 7574 696c 2e70 6172  _tot...@util.par
-000095e0: 7365 5f6f 7074 696f 6e61 6c5f 7061 7261  se_optional_para
-000095f0: 6d65 7465 7273 2877 6869 6368 3d28 2774  meters(which=('t
-00009600: 6f74 616c 272c 2027 636f 7272 656c 6174  otal', 'correlat
-00009610: 696f 6e73 2729 290a 6465 6620 6361 6c63  ions')).def calc
-00009620: 756c 6174 655f 6375 6d75 6c61 6e74 5f66  ulate_cumulant_f
-00009630: 756e 6374 696f 6e28 0a20 2020 2020 2020  unction(.       
-00009640: 2070 756c 7365 3a20 2750 756c 7365 5365   pulse: 'PulseSe
-00009650: 7175 656e 6365 272c 0a20 2020 2020 2020  quence',.       
-00009660: 2073 7065 6374 7275 6d3a 204f 7074 696f   spectrum: Optio
-00009670: 6e61 6c5b 6e64 6172 7261 795d 203d 204e  nal[ndarray] = N
-00009680: 6f6e 652c 0a20 2020 2020 2020 206f 6d65  one,.        ome
-00009690: 6761 3a20 4f70 7469 6f6e 616c 5b43 6f65  ga: Optional[Coe
-000096a0: 6666 6963 6965 6e74 735d 203d 204e 6f6e  fficients] = Non
-000096b0: 652c 0a20 2020 2020 2020 206e 5f6f 7065  e,.        n_ope
-000096c0: 725f 6964 656e 7469 6669 6572 733a 204f  r_identifiers: O
-000096d0: 7074 696f 6e61 6c5b 5365 7175 656e 6365  ptional[Sequence
-000096e0: 5b73 7472 5d5d 203d 204e 6f6e 652c 0a20  [str]] = None,. 
-000096f0: 2020 2020 2020 2077 6869 6368 3a20 7374         which: st
-00009700: 7220 3d20 2774 6f74 616c 272c 0a20 2020  r = 'total',.   
-00009710: 2020 2020 2073 6563 6f6e 645f 6f72 6465       second_orde
-00009720: 723a 2062 6f6f 6c20 3d20 4661 6c73 652c  r: bool = False,
-00009730: 0a20 2020 2020 2020 2064 6563 6179 5f61  .        decay_a
-00009740: 6d70 6c69 7475 6465 733a 204f 7074 696f  mplitudes: Optio
-00009750: 6e61 6c5b 6e64 6172 7261 795d 203d 204e  nal[ndarray] = N
-00009760: 6f6e 652c 0a20 2020 2020 2020 2066 7265  one,.        fre
-00009770: 7175 656e 6379 5f73 6869 6674 733a 204f  quency_shifts: O
-00009780: 7074 696f 6e61 6c5b 6e64 6172 7261 795d  ptional[ndarray]
-00009790: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-000097a0: 2073 686f 775f 7072 6f67 7265 7373 6261   show_progressba
-000097b0: 723a 2062 6f6f 6c20 3d20 4661 6c73 652c  r: bool = False,
-000097c0: 0a20 2020 2020 2020 206d 656d 6f72 795f  .        memory_
-000097d0: 7061 7273 696d 6f6e 696f 7573 3a20 626f  parsimonious: bo
-000097e0: 6f6c 203d 2046 616c 7365 2c0a 2020 2020  ol = False,.    
-000097f0: 2020 2020 6361 6368 655f 696e 7465 726d      cache_interm
-00009800: 6564 6961 7465 733a 204f 7074 696f 6e61  ediates: Optiona
-00009810: 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65 0a29  l[bool] = None.)
-00009820: 202d 3e20 6e64 6172 7261 793a 0a20 2020   -> ndarray:.   
-00009830: 2072 2222 2243 616c 6375 6c61 7465 2074   r"""Calculate t
-00009840: 6865 2063 756d 756c 616e 7420 6675 6e63  he cumulant func
-00009850: 7469 6f6e 203a 6d61 7468 3a60 5c6d 6174  tion :math:`\mat
-00009860: 6863 616c 7b4b 7d28 5c74 6175 2960 2e0a  hcal{K}(\tau)`..
-00009870: 0a20 2020 2054 6865 2065 7272 6f72 2074  .    The error t
-00009880: 7261 6e73 6665 7220 6d61 7472 6978 2069  ransfer matrix i
-00009890: 7320 6f62 7461 696e 6564 2066 726f 6d20  s obtained from 
-000098a0: 7468 6520 6375 6d75 6c61 6e74 2066 756e  the cumulant fun
-000098b0: 6374 696f 6e20 6279 0a20 2020 2065 7870  ction by.    exp
-000098c0: 6f6e 656e 7469 6174 696f 6e2c 0a20 2020  onentiation,.   
-000098d0: 203a 6d61 7468 3a60 5c6c 616e 676c 655c   :math:`\langle\
-000098e0: 7469 6c64 657b 5c6d 6174 6863 616c 7b55  tilde{\mathcal{U
-000098f0: 7d7d 5c72 616e 676c 6520 3d20 5c65 7870  }}\rangle = \exp
-00009900: 5c6d 6174 6863 616c 7b4b 7d28 5c74 6175  \mathcal{K}(\tau
-00009910: 2960 2e0a 0a20 2020 2050 6172 616d 6574  )`...    Paramet
-00009920: 6572 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ers.    --------
-00009930: 2d2d 0a20 2020 2070 756c 7365 3a20 5075  --.    pulse: Pu
-00009940: 6c73 6553 6571 7565 6e63 650a 2020 2020  lseSequence.    
-00009950: 2020 2020 5468 6520 6060 5075 6c73 6553      The ``PulseS
-00009960: 6571 7565 6e63 6560 6020 696e 7374 616e  equence`` instan
-00009970: 6365 2066 6f72 2077 6869 6368 2074 6f20  ce for which to 
-00009980: 636f 6d70 7574 6520 7468 6520 6375 6d75  compute the cumu
-00009990: 6c61 6e74 0a20 2020 2020 2020 2066 756e  lant.        fun
-000099a0: 6374 696f 6e2e 0a20 2020 2073 7065 6374  ction..    spect
-000099b0: 7275 6d3a 2061 7272 6179 5f6c 696b 652c  rum: array_like,
-000099c0: 2073 6861 7065 2028 5b5b 6e5f 6e6f 7073   shape ([[n_nops
-000099d0: 2c5d 206e 5f6e 6f70 732c 5d20 6e5f 6f6d  ,] n_nops,] n_om
-000099e0: 6567 6129 2c20 6f70 7469 6f6e 616c 0a20  ega), optional. 
-000099f0: 2020 2020 2020 2054 6865 206e 6f69 7365         The noise
-00009a00: 2070 6f77 6572 2073 7065 6374 7261 6c20   power spectral 
-00009a10: 6465 6e73 6974 7920 696e 2075 6e69 7473  density in units
-00009a20: 206f 6620 696e 7665 7273 6520 6672 6571   of inverse freq
-00009a30: 7565 6e63 6965 730a 2020 2020 2020 2020  uencies.        
-00009a40: 6173 2061 6e20 6172 7261 7920 6f66 2073  as an array of s
-00009a50: 6861 7065 2028 6e5f 6f6d 6567 612c 292c  hape (n_omega,),
-00009a60: 2028 6e5f 6e6f 7073 2c20 6e5f 6f6d 6567   (n_nops, n_omeg
-00009a70: 6129 2c20 6f72 2028 6e5f 6e6f 7073 2c0a  a), or (n_nops,.
-00009a80: 2020 2020 2020 2020 6e5f 6e6f 7073 2c20          n_nops, 
-00009a90: 6e5f 6f6d 6567 6129 2e20 496e 2074 6865  n_omega). In the
-00009aa0: 2066 6972 7374 2063 6173 652c 2074 6865   first case, the
-00009ab0: 2073 616d 6520 7370 6563 7472 756d 2069   same spectrum i
-00009ac0: 7320 7461 6b65 6e0a 2020 2020 2020 2020  s taken.        
-00009ad0: 666f 7220 616c 6c20 6e6f 6973 6520 6f70  for all noise op
-00009ae0: 6572 6174 6f72 732c 2069 6e20 7468 6520  erators, in the 
-00009af0: 7365 636f 6e64 2c20 6974 2069 7320 6173  second, it is as
-00009b00: 7375 6d65 6420 7468 6174 2074 6865 7265  sumed that there
-00009b10: 0a20 2020 2020 2020 2061 7265 206e 6f20  .        are no 
-00009b20: 636f 7272 656c 6174 696f 6e73 2062 6574  correlations bet
-00009b30: 7765 656e 2064 6966 6665 7265 6e74 206e  ween different n
-00009b40: 6f69 7365 2073 6f75 7263 6573 2061 6e64  oise sources and
-00009b50: 2074 6875 730a 2020 2020 2020 2020 7468   thus.        th
-00009b60: 6572 6520 6973 206f 6e65 2073 7065 6374  ere is one spect
-00009b70: 7275 6d20 666f 7220 6561 6368 206e 6f69  rum for each noi
-00009b80: 7365 206f 7065 7261 746f 722e 2049 6e20  se operator. In 
-00009b90: 7468 6520 7468 6972 6420 616e 640a 2020  the third and.  
-00009ba0: 2020 2020 2020 6d6f 7374 2067 656e 6572        most gener
-00009bb0: 616c 2063 6173 652c 2074 6865 7265 206d  al case, there m
-00009bc0: 6179 2062 6520 6120 7370 6563 7472 756d  ay be a spectrum
-00009bd0: 2066 6f72 2065 6163 6820 7061 6972 206f   for each pair o
-00009be0: 660a 2020 2020 2020 2020 6e6f 6973 6520  f.        noise 
-00009bf0: 6f70 6572 6174 6f72 7320 636f 7272 6573  operators corres
-00009c00: 706f 6e64 696e 6720 746f 2074 6865 2063  ponding to the c
-00009c10: 6f72 7265 6c61 7469 6f6e 7320 6265 7477  orrelations betw
-00009c20: 6565 6e20 7468 656d 2e0a 2020 2020 2020  een them..      
-00009c30: 2020 6e5f 6e6f 7073 2069 7320 7468 6520    n_nops is the 
-00009c40: 6e75 6d62 6572 206f 6620 6e6f 6973 6520  number of noise 
-00009c50: 6f70 6572 6174 6f72 7320 636f 6e73 6964  operators consid
-00009c60: 6572 6564 2061 6e64 2073 686f 756c 6420  ered and should 
-00009c70: 6265 0a20 2020 2020 2020 2065 7175 616c  be.        equal
-00009c80: 2074 6f20 6060 6c65 6e28 6e5f 6f70 6572   to ``len(n_oper
-00009c90: 5f69 6465 6e74 6966 6965 7273 2960 602e  _identifiers)``.
-00009ca0: 0a20 2020 206f 6d65 6761 3a20 6172 7261  .    omega: arra
-00009cb0: 795f 6c69 6b65 2c20 7368 6170 6520 286e  y_like, shape (n
-00009cc0: 5f6f 6d65 6761 2c29 2c20 6f70 7469 6f6e  _omega,), option
-00009cd0: 616c 0a20 2020 2020 2020 2054 6865 2066  al.        The f
-00009ce0: 7265 7175 656e 6369 6573 2061 7420 7768  requencies at wh
-00009cf0: 6963 6820 746f 2065 7661 6c75 6174 6520  ich to evaluate 
-00009d00: 7468 6520 6669 6c74 6572 2066 756e 6374  the filter funct
-00009d10: 696f 6e73 2e0a 2020 2020 6e5f 6f70 6572  ions..    n_oper
-00009d20: 5f69 6465 6e74 6966 6965 7273 3a20 6172  _identifiers: ar
-00009d30: 7261 795f 6c69 6b65 2c20 6f70 7469 6f6e  ray_like, option
-00009d40: 616c 0a20 2020 2020 2020 2054 6865 2069  al.        The i
-00009d50: 6465 6e74 6966 6965 7273 206f 6620 7468  dentifiers of th
-00009d60: 6520 6e6f 6973 6520 6f70 6572 6174 6f72  e noise operator
-00009d70: 7320 666f 7220 7768 6963 6820 746f 2065  s for which to e
-00009d80: 7661 6c75 6174 6520 7468 650a 2020 2020  valuate the.    
-00009d90: 2020 2020 6375 6d75 6c61 6e74 2066 756e      cumulant fun
-00009da0: 6374 696f 6e2e 2054 6865 2064 6566 6175  ction. The defau
-00009db0: 6c74 2069 7320 616c 6c2e 0a20 2020 2077  lt is all..    w
-00009dc0: 6869 6368 3a20 7374 722c 206f 7074 696f  hich: str, optio
-00009dd0: 6e61 6c0a 2020 2020 2020 2020 5768 6963  nal.        Whic
-00009de0: 6820 6465 6361 7920 616d 706c 6974 7564  h decay amplitud
-00009df0: 6573 2073 686f 756c 6420 6265 2063 616c  es should be cal
-00009e00: 6375 6c61 7465 642c 206d 6179 2062 6520  culated, may be 
-00009e10: 6569 7468 6572 0a20 2020 2020 2020 2027  either.        '
-00009e20: 746f 7461 6c27 2028 6465 6661 756c 7429  total' (default)
-00009e30: 206f 7220 2763 6f72 7265 6c61 7469 6f6e   or 'correlation
-00009e40: 7327 2e20 5365 6520 3a66 756e 633a 6069  s'. See :func:`i
-00009e50: 6e66 6964 656c 6974 7960 2061 6e64 0a20  nfidelity` and. 
-00009e60: 2020 2020 2020 203a 7265 663a 604e 6f74         :ref:`Not
-00009e70: 6573 203c 6e6f 7465 733e 602e 204e 6f74  es <notes>`. Not
-00009e80: 6520 7468 6174 2074 6865 206c 6174 7465  e that the latte
-00009e90: 7220 6973 206e 6f74 2061 7661 696c 6162  r is not availab
-00009ea0: 6c65 2066 6f72 0a20 2020 2020 2020 2074  le for.        t
-00009eb0: 6865 2073 6563 6f6e 6420 6f72 6465 7220  he second order 
-00009ec0: 7465 726d 732e 0a20 2020 2073 6563 6f6e  terms..    secon
-00009ed0: 645f 6f72 6465 723a 2062 6f6f 6c2c 206f  d_order: bool, o
-00009ee0: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
-00009ef0: 416c 736f 2074 616b 6520 696e 746f 2061  Also take into a
-00009f00: 6363 6f75 6e74 2074 6865 2066 7265 7175  ccount the frequ
-00009f10: 656e 6379 2073 6869 6674 7320 3a6d 6174  ency shifts :mat
-00009f20: 683a 605c 4465 6c74 6160 2074 6861 740a  h:`\Delta` that.
-00009f30: 2020 2020 2020 2020 636f 7272 6573 706f          correspo
-00009f40: 6e64 2074 6f20 7365 636f 6e64 206f 7264  nd to second ord
-00009f50: 6572 204d 6167 6e75 7320 6578 7061 6e73  er Magnus expans
-00009f60: 696f 6e20 616e 6420 636f 6e73 7469 7475  ion and constitu
-00009f70: 7465 0a20 2020 2020 2020 2075 6e69 7461  te.        unita
-00009f80: 7279 2074 6572 6d73 2e20 4465 6661 756c  ry terms. Defaul
-00009f90: 7420 6060 4661 6c73 6560 602e 0a20 2020  t ``False``..   
-00009fa0: 2064 6563 6179 5f61 6d70 6c69 7475 6465   decay_amplitude
-00009fb0: 732c 2061 7272 6179 5f6c 696b 652c 2073  s, array_like, s
-00009fc0: 6861 7065 2028 5b5b 6e5f 706c 732c 206e  hape ([[n_pls, n
-00009fd0: 5f70 6c73 2c5d 206e 5f6e 6f70 732c 5d20  _pls,] n_nops,] 
-00009fe0: 6e5f 6e6f 7073 2c20 642a 2a32 2c20 642a  n_nops, d**2, d*
-00009ff0: 2a32 292c 206f 7074 696f 6e61 6c0a 2020  *2), optional.  
-0000a000: 2020 2020 2020 4120 7072 6563 6f6d 7075        A precompu
-0000a010: 7465 6420 6375 6d75 6c61 6e74 2066 756e  ted cumulant fun
-0000a020: 6374 696f 6e2e 2049 6620 6769 7665 6e2c  ction. If given,
-0000a030: 202a 7370 6563 7472 756d 2a2c 202a 6f6d   *spectrum*, *om
-0000a040: 6567 612a 0a20 2020 2020 2020 2061 7265  ega*.        are
-0000a050: 206e 6f74 2072 6571 7569 7265 642e 0a20   not required.. 
-0000a060: 2020 2066 7265 7175 656e 6379 5f73 6869     frequency_shi
-0000a070: 6674 732c 2061 7272 6179 5f6c 696b 652c  fts, array_like,
-0000a080: 2073 6861 7065 2028 5b5b 6e5f 706c 732c   shape ([[n_pls,
-0000a090: 206e 5f70 6c73 2c5d 206e 5f6e 6f70 732c   n_pls,] n_nops,
-0000a0a0: 5d20 6e5f 6e6f 7073 2c20 642a 2a32 2c20  ] n_nops, d**2, 
-0000a0b0: 642a 2a32 292c 206f 7074 696f 6e61 6c0a  d**2), optional.
-0000a0c0: 2020 2020 2020 2020 4120 7072 6563 6f6d          A precom
-0000a0d0: 7075 7465 6420 6672 6571 7565 6e63 7920  puted frequency 
-0000a0e0: 7368 6966 742e 2049 6620 6769 7665 6e2c  shift. If given,
-0000a0f0: 202a 7370 6563 7472 756d 2a2c 202a 6f6d   *spectrum*, *om
-0000a100: 6567 612a 0a20 2020 2020 2020 2061 7265  ega*.        are
-0000a110: 206e 6f74 2072 6571 7569 7265 6420 666f   not required fo
-0000a120: 7220 7365 636f 6e64 206f 7264 6572 2074  r second order t
-0000a130: 6572 6d73 2e0a 2020 2020 7368 6f77 5f70  erms..    show_p
-0000a140: 726f 6772 6573 7362 6172 3a20 626f 6f6c  rogressbar: bool
-0000a150: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
-0000a160: 2020 2053 686f 7720 6120 7072 6f67 7265     Show a progre
-0000a170: 7373 2062 6172 2066 6f72 2074 6865 2063  ss bar for the c
-0000a180: 616c 6375 6c61 7469 6f6e 206f 6620 7468  alculation of th
-0000a190: 6520 636f 6e74 726f 6c20 6d61 7472 6978  e control matrix
-0000a1a0: 2e0a 2020 2020 6d65 6d6f 7279 5f70 6172  ..    memory_par
-0000a1b0: 7369 6d6f 6e69 6f75 733a 2062 6f6f 6c2c  simonious: bool,
-0000a1c0: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
-0000a1d0: 2020 5472 6164 6520 6d65 6d6f 7279 2066    Trade memory f
-0000a1e0: 6f6f 7470 7269 6e74 2066 6f72 2070 6572  ootprint for per
-0000a1f0: 666f 726d 616e 6365 2e20 5365 650a 2020  formance. See.  
-0000a200: 2020 2020 2020 3a66 756e 633a 607e 6e75        :func:`~nu
-0000a210: 6d65 7269 632e 6361 6c63 756c 6174 655f  meric.calculate_
-0000a220: 6465 6361 795f 616d 706c 6974 7564 6573  decay_amplitudes
-0000a230: 602e 2054 6865 2064 6566 6175 6c74 2069  `. The default i
-0000a240: 730a 2020 2020 2020 2020 6060 4661 6c73  s.        ``Fals
-0000a250: 6560 602e 0a20 2020 2063 6163 6865 5f69  e``..    cache_i
-0000a260: 6e74 6572 6d65 6469 6174 6573 3a20 626f  ntermediates: bo
-0000a270: 6f6c 2c20 6f70 7469 6f6e 616c 0a20 2020  ol, optional.   
-0000a280: 2020 2020 204b 6565 7020 616e 6420 7265       Keep and re
-0000a290: 7475 726e 2069 6e74 6572 6d65 6469 6174  turn intermediat
-0000a2a0: 6520 7465 726d 7320 6f66 2074 6865 2063  e terms of the c
-0000a2b0: 616c 6375 6c61 7469 6f6e 206f 6620 7468  alculation of th
-0000a2c0: 650a 2020 2020 2020 2020 636f 6e74 726f  e.        contro
-0000a2d0: 6c20 6d61 7472 6978 2074 6861 7420 6361  l matrix that ca
-0000a2e0: 6e20 6265 2072 6575 7365 6420 696e 206f  n be reused in o
-0000a2f0: 7468 6572 2063 6f6d 7075 7461 7469 6f6e  ther computation
-0000a300: 7320 2873 6563 6f6e 640a 2020 2020 2020  s (second.      
-0000a310: 2020 6f72 6465 7220 6f72 2067 7261 6469    order or gradi
-0000a320: 656e 7473 292e 204f 7468 6572 7769 7365  ents). Otherwise
-0000a330: 2074 6865 2073 756d 2069 7320 7065 7266   the sum is perf
-0000a340: 6f72 6d65 6420 696e 2d70 6c61 6365 2e0a  ormed in-place..
-0000a350: 2020 2020 2020 2020 4465 6661 756c 7420          Default 
-0000a360: 6973 2054 7275 6520 6966 2073 6563 6f6e  is True if secon
-0000a370: 645f 6f72 6465 723d 5472 7565 2c20 656c  d_order=True, el
-0000a380: 7365 2046 616c 7365 2e0a 0a20 2020 2052  se False...    R
-0000a390: 6574 7572 6e73 0a20 2020 202d 2d2d 2d2d  eturns.    -----
-0000a3a0: 2d2d 0a20 2020 2063 756d 756c 616e 745f  --.    cumulant_
-0000a3b0: 6675 6e63 7469 6f6e 3a20 6e64 6172 7261  function: ndarra
-0000a3c0: 792c 2073 6861 7065 2028 5b5b 6e5f 706c  y, shape ([[n_pl
-0000a3d0: 732c 206e 5f70 6c73 2c5d 206e 5f6e 6f70  s, n_pls,] n_nop
-0000a3e0: 732c 5d20 6e5f 6e6f 7073 2c20 642a 2a32  s,] n_nops, d**2
-0000a3f0: 2c20 642a 2a32 290a 2020 2020 2020 2020  , d**2).        
-0000a400: 5468 6520 6375 6d75 6c61 6e74 2066 756e  The cumulant fun
-0000a410: 6374 696f 6e2e 2054 6865 2069 6e64 6976  ction. The indiv
-0000a420: 6964 7561 6c20 6e6f 6973 6520 6f70 6572  idual noise oper
-0000a430: 6174 6f72 0a20 2020 2020 2020 2063 6f6e  ator.        con
-0000a440: 7472 6962 7574 696f 6e73 2063 686f 7365  tributions chose
-0000a450: 6e20 6279 2060 606e 5f6f 7065 725f 6964  n by ``n_oper_id
-0000a460: 656e 7469 6669 6572 7360 6020 6172 6520  entifiers`` are 
-0000a470: 6f6e 2074 6865 2074 6869 7264 0a20 2020  on the third.   
-0000a480: 2020 2020 2074 6f20 6c61 7374 2061 7869       to last axi
-0000a490: 7320 2f20 6178 6573 2c20 6465 7065 6e64  s / axes, depend
-0000a4a0: 696e 6720 6f6e 2077 6865 7468 6572 2074  ing on whether t
-0000a4b0: 6865 206e 6f69 7365 2069 730a 2020 2020  he noise is.    
-0000a4c0: 2020 2020 6372 6f73 732d 636f 7272 656c      cross-correl
-0000a4d0: 6174 6564 206f 7220 6e6f 742e 2049 6620  ated or not. If 
-0000a4e0: 6060 7768 6963 6820 3d3d 2027 636f 7272  ``which == 'corr
-0000a4f0: 656c 6174 696f 6e73 2760 602c 2074 6865  elations'``, the
-0000a500: 0a20 2020 2020 2020 2066 6972 7374 2074  .        first t
-0000a510: 776f 2061 7865 7320 636f 7272 6573 706f  wo axes correspo
-0000a520: 6e64 2074 6f20 7468 6520 636f 6e74 7269  nd to the contri
-0000a530: 6275 7469 6f6e 7320 6f66 2074 6865 2070  butions of the p
-0000a540: 756c 7365 7320 696e 0a20 2020 2020 2020  ulses in.       
-0000a550: 2074 6865 2073 6571 7565 6e63 652e 0a0a   the sequence...
-0000a560: 2020 2020 2e2e 205f 6e6f 7465 733a 0a0a      .. _notes:..
-0000a570: 2020 2020 4e6f 7465 730a 2020 2020 2d2d      Notes.    --
-0000a580: 2d2d 2d0a 2020 2020 5468 6520 6375 6d75  ---.    The cumu
-0000a590: 6c61 6e74 2066 756e 6374 696f 6e20 6973  lant function is
-0000a5a0: 2067 6976 656e 2062 790a 0a20 2020 202e   given by..    .
-0000a5b0: 2e20 6d61 7468 3a3a 0a0a 2020 2020 2020  . math::..      
-0000a5c0: 2020 4b5f 7b5c 616c 7068 615c 6265 7461    K_{\alpha\beta
-0000a5d0: 2c69 6a7d 285c 7461 7529 203d 202d 5c66  ,ij}(\tau) = -\f
-0000a5e0: 7261 637b 317d 7b32 7d20 5c73 756d 5f7b  rac{1}{2} \sum_{
-0000a5f0: 6b6c 7d5c 6269 6767 6c28 0a20 2020 2020  kl}\biggl(.     
-0000a600: 2020 2020 2020 2026 5c44 656c 7461 5f7b         &\Delta_{
-0000a610: 5c61 6c70 6861 5c62 6574 612c 6b6c 7d5c  \alpha\beta,kl}\
-0000a620: 6c65 6674 280a 2020 2020 2020 2020 2020  left(.          
-0000a630: 2020 2020 2020 545f 7b6b 6c6a 697d 202d        T_{klji} -
-0000a640: 2054 5f7b 6c6b 6a69 7d20 2d20 545f 7b6b   T_{lkji} - T_{k
-0000a650: 6c69 6a7d 202b 2054 5f7b 6c6b 696a 7d0a  lij} + T_{lkij}.
-0000a660: 2020 2020 2020 2020 2020 2020 5c72 6967              \rig
-0000a670: 6874 2920 5c5c 202b 2026 5c47 616d 6d61  ht) \\ + &\Gamma
-0000a680: 5f7b 5c61 6c70 6861 5c62 6574 612c 6b6c  _{\alpha\beta,kl
-0000a690: 7d5c 6c65 6674 280a 2020 2020 2020 2020  }\left(.        
-0000a6a0: 2020 2020 2020 2020 545f 7b6b 6c6a 697d          T_{klji}
-0000a6b0: 202d 2054 5f7b 6b6a 6c69 7d20 2d20 545f   - T_{kjli} - T_
-0000a6c0: 7b6b 696c 6a7d 202b 2054 5f7b 6b69 6a6c  {kilj} + T_{kijl
-0000a6d0: 7d0a 2020 2020 2020 2020 2020 2020 5c72  }.            \r
-0000a6e0: 6967 6874 290a 2020 2020 2020 2020 5c62  ight).        \b
-0000a6f0: 6967 6772 290a 0a20 2020 2048 6572 652c  iggr)..    Here,
-0000a700: 203a 6d61 7468 3a60 545f 7b69 6a6b 6c7d   :math:`T_{ijkl}
-0000a710: 203d 205c 6d61 7468 726d 7b74 727d 2843   = \mathrm{tr}(C
-0000a720: 5f69 2043 5f6a 2043 5f6b 2043 5f6c 2960  _i C_j C_k C_l)`
-0000a730: 2069 7320 6120 7472 6976 6961 6c0a 2020   is a trivial.  
-0000a740: 2020 6675 6e63 7469 6f6e 206f 6620 7468    function of th
-0000a750: 6520 6261 7369 7320 656c 656d 656e 7473  e basis elements
-0000a760: 203a 6d61 7468 3a60 435f 6960 2c20 616e   :math:`C_i`, an
-0000a770: 640a 2020 2020 3a6d 6174 683a 605c 4761  d.    :math:`\Ga
-0000a780: 6d6d 615f 7b5c 616c 7068 615c 6265 7461  mma_{\alpha\beta
-0000a790: 2c6b 6c7d 6020 616e 6420 3a6d 6174 683a  ,kl}` and :math:
-0000a7a0: 605c 4465 6c74 615f 7b5c 616c 7068 615c  `\Delta_{\alpha\
-0000a7b0: 6265 7461 2c6b 6c7d 600a 2020 2020 6172  beta,kl}`.    ar
-0000a7c0: 6520 7468 6520 6465 6361 7920 616d 706c  e the decay ampl
-0000a7d0: 6974 7564 6573 2061 6e64 2066 7265 7175  itudes and frequ
-0000a7e0: 656e 6379 2073 6869 6674 7320 7768 6963  ency shifts whic
-0000a7f0: 6820 636f 7272 6573 706f 6e64 2074 6f0a  h correspond to.
-0000a800: 2020 2020 6669 7273 7420 616e 6420 7365      first and se
-0000a810: 636f 6e64 206f 7264 6572 2069 6e20 7468  cond order in th
-0000a820: 6520 4d61 676e 7573 2065 7870 616e 7369  e Magnus expansi
-0000a830: 6f6e 2c20 7265 7370 6563 7469 7665 6c79  on, respectively
-0000a840: 2e20 5369 6e63 650a 2020 2020 7468 6520  . Since.    the 
-0000a850: 6c61 7474 6572 2069 6e64 7563 6520 636f  latter induce co
-0000a860: 6865 7265 6e74 2065 7272 6f72 732c 2077  herent errors, w
-0000a870: 6520 6361 6e20 6170 7072 6f78 696d 6174  e can approximat
-0000a880: 656c 7920 6e65 676c 6563 7420 7468 656d  ely neglect them
-0000a890: 0a20 2020 2069 6620 7765 2061 7373 756d  .    if we assum
-0000a8a0: 6520 7468 6174 2074 6865 2070 756c 7365  e that the pulse
-0000a8b0: 2068 6173 2062 6565 6e20 6578 7065 7269   has been experi
-0000a8c0: 6d65 6e74 616c 6c79 2063 616c 6962 7261  mentally calibra
-0000a8d0: 7465 642e 0a0a 2020 2020 466f 7220 6120  ted...    For a 
-0000a8e0: 7369 6e67 6c65 2071 7562 6974 2061 6e64  single qubit and
-0000a8f0: 2072 6570 7265 7365 6e74 6564 2069 6e20   represented in 
-0000a900: 7468 6520 5061 756c 6920 6261 7369 732c  the Pauli basis,
-0000a910: 2074 6865 2061 626f 7665 0a20 2020 2072   the above.    r
-0000a920: 6564 7563 6573 2074 6f0a 0a20 2020 202e  educes to..    .
-0000a930: 2e20 6d61 7468 3a3a 0a0a 2020 2020 2020  . math::..      
-0000a940: 2020 4b5f 7b5c 616c 7068 615c 6265 7461    K_{\alpha\beta
-0000a950: 2c69 6a7d 285c 7461 7529 203d 205c 6265  ,ij}(\tau) = \be
-0000a960: 6769 6e7b 6361 7365 737d 0a20 2020 2020  gin{cases}.     
-0000a970: 2020 2020 2020 202d 205c 7375 6d5f 7b6b         - \sum_{k
-0000a980: 5c6e 6571 2069 7d5c 4761 6d6d 615f 7b5c  \neq i}\Gamma_{\
-0000a990: 616c 7068 615c 6265 7461 2c6b 6b7d 0a20  alpha\beta,kk}. 
-0000a9a0: 2020 2020 2020 2020 2020 2020 2020 2026                 &
-0000a9b0: 5c71 7561 645c 6d61 7468 726d 7b69 667d  \quad\mathrm{if}
-0000a9c0: 5c3a 2069 203d 206a 2c20 2020 5c5c 0a20  \: i = j,   \\. 
-0000a9d0: 2020 2020 2020 2020 2020 202d 205c 4465             - \De
-0000a9e0: 6c74 615f 7b5c 616c 7068 615c 6265 7461  lta_{\alpha\beta
-0000a9f0: 2c69 6a7d 202b 205c 4465 6c74 615f 7b5c  ,ij} + \Delta_{\
-0000aa00: 616c 7068 615c 6265 7461 2c6a 697d 0a20  alpha\beta,ji}. 
-0000aa10: 2020 2020 2020 2020 2020 202b 205c 4761             + \Ga
-0000aa20: 6d6d 615f 7b5c 616c 7068 615c 6265 7461  mma_{\alpha\beta
-0000aa30: 2c69 6a7d 0a20 2020 2020 2020 2020 2020  ,ij}.           
-0000aa40: 2020 2020 2026 5c71 7561 645c 6d61 7468       &\quad\math
-0000aa50: 726d 7b69 667d 5c3a 2069 5c6e 6571 206a  rm{if}\: i\neq j
-0000aa60: 2c0a 2020 2020 2020 2020 5c65 6e64 7b63  ,.        \end{c
-0000aa70: 6173 6573 7d0a 0a20 2020 2066 6f72 203a  ases}..    for :
-0000aa80: 6d61 7468 3a60 695c 696e 5c7b 312c 322c  math:`i\in\{1,2,
-0000aa90: 335c 7d60 2061 6e64 203a 6d61 7468 3a60  3\}` and :math:`
-0000aaa0: 4b5f 7b30 6a7d 203d 204b 5f7b 6930 7d20  K_{0j} = K_{i0} 
-0000aab0: 3d20 3060 2e0a 0a20 2020 204c 6173 746c  = 0`...    Lastl
-0000aac0: 792c 2074 6865 2070 756c 7365 2063 6f72  y, the pulse cor
-0000aad0: 7265 6c61 7469 6f6e 2063 756d 756c 616e  relation cumulan
-0000aae0: 7420 6675 6e63 7469 6f6e 2072 6573 6f6c  t function resol
-0000aaf0: 7665 730a 2020 2020 636f 7272 656c 6174  ves.    correlat
-0000ab00: 696f 6e73 2069 6e20 7468 6520 6375 6d75  ions in the cumu
-0000ab10: 6c61 6e74 2066 756e 6374 696f 6e20 6f66  lant function of
-0000ab20: 2061 2073 6571 7565 6e63 6520 6f66 2070   a sequence of p
-0000ab30: 756c 7365 730a 2020 2020 3a6d 6174 683a  ulses.    :math:
-0000ab40: 6067 203d 2031 2c5c 646f 7473 632c 4760  `g = 1,\dotsc,G`
-0000ab50: 2073 7563 6820 7468 6174 2074 6865 2066   such that the f
-0000ab60: 6f6c 6c6f 7769 6e67 2068 6f6c 6473 3a0a  ollowing holds:.
-0000ab70: 0a20 2020 202e 2e20 6d61 7468 3a3a 0a0a  .    .. math::..
-0000ab80: 2020 2020 2020 2020 4b5f 7b5c 616c 7068          K_{\alph
-0000ab90: 615c 6265 7461 2c69 6a7d 285c 7461 7529  a\beta,ij}(\tau)
-0000aba0: 203d 205c 7375 6d5f 7b67 2c67 273d 317d   = \sum_{g,g'=1}
-0000abb0: 5e47 0a20 2020 2020 2020 2020 2020 2020  ^G.             
-0000abc0: 4b5f 7b5c 616c 7068 615c 6265 7461 2c69  K_{\alpha\beta,i
-0000abd0: 6a7d 5e7b 2867 6727 297d 285c 7461 7529  j}^{(gg')}(\tau)
-0000abe0: 2e0a 0a20 2020 2053 6565 2041 6c73 6f0a  ...    See Also.
-0000abf0: 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020      --------.   
-0000ac00: 2063 616c 6375 6c61 7465 5f64 6563 6179   calculate_decay
-0000ac10: 5f61 6d70 6c69 7475 6465 733a 2043 616c  _amplitudes: Cal
-0000ac20: 6375 6c61 7465 2074 6865 203a 6d61 7468  culate the :math
-0000ac30: 3a60 5c47 616d 6d61 5f7b 5c61 6c70 6861  :`\Gamma_{\alpha
-0000ac40: 5c62 6574 612c 6b6c 7d60 0a20 2020 2065  \beta,kl}`.    e
-0000ac50: 7272 6f72 5f74 7261 6e73 6665 725f 6d61  rror_transfer_ma
-0000ac60: 7472 6978 3a20 4361 6c63 756c 6174 6520  trix: Calculate 
-0000ac70: 7468 6520 6572 726f 7220 7472 616e 7366  the error transf
-0000ac80: 6572 206d 6174 7269 7820 3a6d 6174 683a  er matrix :math:
-0000ac90: 605c 6578 705c 6d61 7468 6361 6c7b 4b7d  `\exp\mathcal{K}
-0000aca0: 602e 0a20 2020 2069 6e66 6964 656c 6974  `..    infidelit
-0000acb0: 793a 2043 616c 6375 6c61 7465 206f 6e6c  y: Calculate onl
-0000acc0: 7920 696e 6669 6465 6c69 7479 206f 6620  y infidelity of 
-0000acd0: 6120 7075 6c73 652e 0a20 2020 2070 756c  a pulse..    pul
-0000ace0: 7365 5f73 6571 7565 6e63 652e 636f 6e63  se_sequence.conc
-0000acf0: 6174 656e 6174 653a 2043 6f6e 6361 7465  atenate: Concate
-0000ad00: 6e61 7465 2060 6050 756c 7365 5365 7175  nate ``PulseSequ
-0000ad10: 656e 6365 6060 206f 626a 6563 7473 2e0a  ence`` objects..
-0000ad20: 2020 2020 6361 6c63 756c 6174 655f 7075      calculate_pu
-0000ad30: 6c73 655f 636f 7272 656c 6174 696f 6e5f  lse_correlation_
-0000ad40: 6669 6c74 6572 5f66 756e 6374 696f 6e0a  filter_function.
-0000ad50: 0a20 2020 2022 2222 0a20 2020 204e 2c20  .    """.    N, 
-0000ad60: 6420 3d20 7075 6c73 652e 6261 7369 732e  d = pulse.basis.
-0000ad70: 7368 6170 655b 3a32 5d0a 2020 2020 6966  shape[:2].    if
-0000ad80: 2073 7065 6374 7275 6d20 6973 204e 6f6e   spectrum is Non
-0000ad90: 6520 616e 6420 6f6d 6567 6120 6973 204e  e and omega is N
-0000ada0: 6f6e 653a 0a20 2020 2020 2020 2069 6620  one:.        if 
-0000adb0: 6465 6361 795f 616d 706c 6974 7564 6573  decay_amplitudes
-0000adc0: 2069 7320 4e6f 6e65 206f 7220 2866 7265   is None or (fre
-0000add0: 7175 656e 6379 5f73 6869 6674 7320 6973  quency_shifts is
-0000ade0: 204e 6f6e 6520 616e 6420 7365 636f 6e64   None and second
-0000adf0: 5f6f 7264 6572 293a 0a20 2020 2020 2020  _order):.       
-0000ae00: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-0000ae10: 4572 726f 7228 2752 6571 7569 7265 2065  Error('Require e
-0000ae20: 6974 6865 7220 7370 6563 7472 756d 2061  ither spectrum a
-0000ae30: 6e64 2066 7265 7175 656e 6369 6573 206f  nd frequencies o
-0000ae40: 7220 7072 6563 6f6d 7075 7465 6420 2720  r precomputed ' 
-0000ae50: 2b0a 2020 2020 2020 2020 2020 2020 2020  +.              
-0000ae60: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-0000ae70: 6465 6361 7920 616d 706c 6974 7564 6573  decay amplitudes
-0000ae80: 2028 6672 6571 7565 6e63 7920 7368 6966   (frequency shif
-0000ae90: 7473 2927 290a 0a20 2020 2069 6620 7768  ts)')..    if wh
-0000aea0: 6963 6820 3d3d 2027 636f 7272 656c 6174  ich == 'correlat
-0000aeb0: 696f 6e73 2720 616e 6420 7365 636f 6e64  ions' and second
-0000aec0: 5f6f 7264 6572 3a0a 2020 2020 2020 2020  _order:.        
-0000aed0: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-0000aee0: 2827 4361 6e6e 6f74 2063 6f6d 7075 7465  ('Cannot compute
-0000aef0: 2063 6f72 7265 6c61 7469 6f6e 2063 756d   correlation cum
-0000af00: 756c 616e 7420 6675 6e63 7469 6f6e 2066  ulant function f
-0000af10: 6f72 2073 6563 6f6e 6420 6f72 6465 7220  or second order 
-0000af20: 7465 726d 7327 290a 0a20 2020 2069 6620  terms')..    if 
-0000af30: 6361 6368 655f 696e 7465 726d 6564 6961  cache_intermedia
-0000af40: 7465 7320 6973 204e 6f6e 653a 0a20 2020  tes is None:.   
-0000af50: 2020 2020 2063 6163 6865 5f69 6e74 6572       cache_inter
-0000af60: 6d65 6469 6174 6573 203d 2073 6563 6f6e  mediates = secon
-0000af70: 645f 6f72 6465 720a 0a20 2020 2069 6620  d_order..    if 
-0000af80: 6465 6361 795f 616d 706c 6974 7564 6573  decay_amplitudes
-0000af90: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-0000afa0: 2020 6465 6361 795f 616d 706c 6974 7564    decay_amplitud
-0000afb0: 6573 203d 2063 616c 6375 6c61 7465 5f64  es = calculate_d
-0000afc0: 6563 6179 5f61 6d70 6c69 7475 6465 7328  ecay_amplitudes(
-0000afd0: 7075 6c73 652c 2073 7065 6374 7275 6d2c  pulse, spectrum,
-0000afe0: 206f 6d65 6761 2c20 6e5f 6f70 6572 5f69   omega, n_oper_i
-0000aff0: 6465 6e74 6966 6965 7273 2c0a 2020 2020  dentifiers,.    
-0000b000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b030: 2020 7768 6963 682c 2073 686f 775f 7072    which, show_pr
-0000b040: 6f67 7265 7373 6261 722c 2063 6163 6865  ogressbar, cache
-0000b050: 5f69 6e74 6572 6d65 6469 6174 6573 2c0a  _intermediates,.
-0000b060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b090: 2020 2020 2020 6d65 6d6f 7279 5f70 6172        memory_par
-0000b0a0: 7369 6d6f 6e69 6f75 7329 0a0a 2020 2020  simonious)..    
-0000b0b0: 6966 2073 6563 6f6e 645f 6f72 6465 723a  if second_order:
-0000b0c0: 0a20 2020 2020 2020 2069 6620 6672 6571  .        if freq
-0000b0d0: 7565 6e63 795f 7368 6966 7473 2069 7320  uency_shifts is 
-0000b0e0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0000b0f0: 2020 6966 206d 656d 6f72 795f 7061 7273    if memory_pars
-0000b100: 696d 6f6e 696f 7573 3a0a 2020 2020 2020  imonious:.      
-0000b110: 2020 2020 2020 2020 2020 7761 726e 2827            warn('
-0000b120: 4d65 6d6f 7279 2070 6172 7369 6d6f 6e69  Memory parsimoni
-0000b130: 6f75 7320 6361 6c63 756c 6174 696f 6e20  ous calculation 
-0000b140: 6e6f 7420 696d 706c 656d 656e 7465 6420  not implemented 
-0000b150: 666f 7220 6672 6571 7565 6e63 7920 7368  for frequency sh
-0000b160: 6966 7473 2e27 290a 0a20 2020 2020 2020  ifts.')..       
-0000b170: 2020 2020 2066 7265 7175 656e 6379 5f73       frequency_s
-0000b180: 6869 6674 7320 3d20 6361 6c63 756c 6174  hifts = calculat
-0000b190: 655f 6672 6571 7565 6e63 795f 7368 6966  e_frequency_shif
-0000b1a0: 7473 2870 756c 7365 2c20 7370 6563 7472  ts(pulse, spectr
-0000b1b0: 756d 2c20 6f6d 6567 612c 0a20 2020 2020  um, omega,.     
-0000b1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b1f0: 2020 2020 206e 5f6f 7065 725f 6964 656e       n_oper_iden
-0000b200: 7469 6669 6572 732c 2073 686f 775f 7072  tifiers, show_pr
-0000b210: 6f67 7265 7373 6261 7229 0a0a 2020 2020  ogressbar)..    
-0000b220: 2020 2020 6966 2066 7265 7175 656e 6379      if frequency
-0000b230: 5f73 6869 6674 732e 7368 6170 6520 213d  _shifts.shape !=
-0000b240: 2064 6563 6179 5f61 6d70 6c69 7475 6465   decay_amplitude
-0000b250: 732e 7368 6170 653a 0a20 2020 2020 2020  s.shape:.       
-0000b260: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-0000b270: 4572 726f 7228 2746 7265 7175 656e 6379  Error('Frequency
-0000b280: 2073 6869 6674 7320 6e6f 7420 7361 6d65   shifts not same
-0000b290: 2073 6861 7065 2061 7320 6465 6361 7920   shape as decay 
-0000b2a0: 616d 706c 6974 7564 6573 2729 0a0a 2020  amplitudes')..  
-0000b2b0: 2020 6966 2064 203d 3d20 3220 616e 6420    if d == 2 and 
-0000b2c0: 7075 6c73 652e 6261 7369 732e 6274 7970  pulse.basis.btyp
-0000b2d0: 6520 696e 2028 2750 6175 6c69 272c 2027  e in ('Pauli', '
-0000b2e0: 4747 4d27 293a 0a20 2020 2020 2020 2023  GGM'):.        #
-0000b2f0: 2053 696e 676c 6520 7175 6269 7420 6361   Single qubit ca
-0000b300: 7365 2e20 4361 6e20 7573 6520 7369 6d70  se. Can use simp
-0000b310: 6c69 6669 6564 2065 7870 7265 7373 696f  lified expressio
-0000b320: 6e0a 2020 2020 2020 2020 6375 6d75 6c61  n.        cumula
-0000b330: 6e74 5f66 756e 6374 696f 6e20 3d20 6e70  nt_function = np
-0000b340: 2e7a 6572 6f73 2864 6563 6179 5f61 6d70  .zeros(decay_amp
-0000b350: 6c69 7475 6465 732e 7368 6170 652c 2064  litudes.shape, d
-0000b360: 6563 6179 5f61 6d70 6c69 7475 6465 732e  ecay_amplitudes.
-0000b370: 6474 7970 6529 0a20 2020 2020 2020 2064  dtype).        d
-0000b380: 6961 675f 6d61 736b 203d 206e 702e 7a65  iag_mask = np.ze
-0000b390: 726f 7328 284e 2c20 4e29 2c20 6474 7970  ros((N, N), dtyp
-0000b3a0: 653d 626f 6f6c 290a 2020 2020 2020 2020  e=bool).        
-0000b3b0: 6469 6167 5f6d 6173 6b5b 313a 2c20 313a  diag_mask[1:, 1:
-0000b3c0: 5d20 3d20 7e6e 702e 6579 6528 4e2d 312c  ] = ~np.eye(N-1,
-0000b3d0: 2064 7479 7065 3d62 6f6f 6c29 0a0a 2020   dtype=bool)..  
-0000b3e0: 2020 2020 2020 2320 4f66 6664 6961 676f        # Offdiago
-0000b3f0: 6e61 6c20 7465 726d 730a 2020 2020 2020  nal terms.      
-0000b400: 2020 6375 6d75 6c61 6e74 5f66 756e 6374    cumulant_funct
-0000b410: 696f 6e5b 2e2e 2e2c 2064 6961 675f 6d61  ion[..., diag_ma
-0000b420: 736b 5d20 3d20 6465 6361 795f 616d 706c  sk] = decay_ampl
-0000b430: 6974 7564 6573 5b2e 2e2e 2c20 6469 6167  itudes[..., diag
-0000b440: 5f6d 6173 6b5d 0a0a 2020 2020 2020 2020  _mask]..        
-0000b450: 2320 4469 6167 6f6e 616c 2074 6572 6d73  # Diagonal terms
-0000b460: 204b 5f69 6920 6769 7665 6e20 6279 2073   K_ii given by s
-0000b470: 756d 206f 7665 7220 6469 6167 6f6e 616c  um over diagonal
-0000b480: 206f 6620 4761 6d6d 6120 6578 636c 7564   of Gamma exclud
-0000b490: 696e 670a 2020 2020 2020 2020 2320 4761  ing.        # Ga
-0000b4a0: 6d6d 615f 6969 2e20 5369 6e63 6520 7468  mma_ii. Since th
-0000b4b0: 6520 5061 756c 6920 6261 7369 7320 6973  e Pauli basis is
-0000b4c0: 2074 7261 6365 6c65 7373 2c20 4b5f 3030   traceless, K_00
-0000b4d0: 2069 7320 7a65 726f 2c20 7468 6572 6566   is zero, theref
-0000b4e0: 6f72 650a 2020 2020 2020 2020 2320 7374  ore.        # st
-0000b4f0: 6172 7420 6174 204b 5f31 312e 0a20 2020  art at K_11..   
-0000b500: 2020 2020 2064 6961 675f 6465 7175 6520       diag_deque 
-0000b510: 3d20 6465 7175 6528 2846 616c 7365 2c20  = deque((False, 
-0000b520: 5472 7565 2c20 5472 7565 2929 0a20 2020  True, True)).   
-0000b530: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
-0000b540: 6e67 6528 312c 204e 293a 0a20 2020 2020  nge(1, N):.     
-0000b550: 2020 2020 2020 2064 6961 675f 6964 7820         diag_idx 
-0000b560: 3d20 5b46 616c 7365 5d20 2b20 6c69 7374  = [False] + list
-0000b570: 2864 6961 675f 6465 7175 6529 0a20 2020  (diag_deque).   
-0000b580: 2020 2020 2020 2020 2063 756d 756c 616e           cumulan
-0000b590: 745f 6675 6e63 7469 6f6e 5b2e 2e2e 2c20  t_function[..., 
-0000b5a0: 692c 2069 5d20 3d20 2d64 6563 6179 5f61  i, i] = -decay_a
-0000b5b0: 6d70 6c69 7475 6465 735b 2e2e 2e2c 2064  mplitudes[..., d
-0000b5c0: 6961 675f 6964 782c 2064 6961 675f 6964  iag_idx, diag_id
-0000b5d0: 785d 2e73 756d 2861 7869 733d 2d31 290a  x].sum(axis=-1).
-0000b5e0: 2020 2020 2020 2020 2020 2020 2320 7368              # sh
-0000b5f0: 6966 7420 7468 6520 6974 656d 206e 6f74  ift the item not
-0000b600: 2073 756d 6d65 6420 6f76 6572 2062 7920   summed over by 
-0000b610: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
-0000b620: 6469 6167 5f64 6571 7565 2e72 6f74 6174  diag_deque.rotat
-0000b630: 6528 290a 0a20 2020 2020 2020 2069 6620  e()..        if 
-0000b640: 7365 636f 6e64 5f6f 7264 6572 3a0a 2020  second_order:.  
-0000b650: 2020 2020 2020 2020 2020 6375 6d75 6c61            cumula
-0000b660: 6e74 5f66 756e 6374 696f 6e5b 2e2e 2e2c  nt_function[...,
-0000b670: 2031 3a2c 2031 3a5d 202d 3d20 6672 6571   1:, 1:] -= freq
-0000b680: 7565 6e63 795f 7368 6966 7473 5b2e 2e2e  uency_shifts[...
-0000b690: 2c20 313a 2c20 313a 5d0a 2020 2020 2020  , 1:, 1:].      
-0000b6a0: 2020 2020 2020 6375 6d75 6c61 6e74 5f66        cumulant_f
-0000b6b0: 756e 6374 696f 6e5b 2e2e 2e2c 2031 3a2c  unction[..., 1:,
-0000b6c0: 2031 3a5d 202b 3d20 6672 6571 7565 6e63   1:] += frequenc
-0000b6d0: 795f 7368 6966 7473 5b2e 2e2e 2c20 313a  y_shifts[..., 1:
-0000b6e0: 2c20 313a 5d2e 7377 6170 6178 6573 282d  , 1:].swapaxes(-
-0000b6f0: 312c 202d 3229 0a20 2020 2065 6c73 653a  1, -2).    else:
-0000b700: 0a20 2020 2020 2020 2023 204d 756c 7469  .        # Multi
-0000b710: 2071 7562 6974 2063 6173 652e 2055 7365   qubit case. Use
-0000b720: 2067 656e 6572 616c 2065 7870 7265 7373   general express
-0000b730: 696f 6e2e 2044 726f 7020 696d 6167 696e  ion. Drop imagin
-0000b740: 6172 7920 7061 7274 2073 696e 6365 0a20  ary part since. 
-0000b750: 2020 2020 2020 2023 2072 6573 756c 7420         # result 
-0000b760: 6973 2067 7561 7261 6e74 6565 6420 746f  is guaranteed to
-0000b770: 2062 6520 7265 616c 2028 6966 2077 6520   be real (if we 
-0000b780: 6469 646e 2774 2064 6f20 616e 7974 6869  didn't do anythi
-0000b790: 6e67 2077 726f 6e67 290a 2020 2020 2020  ng wrong).      
-0000b7a0: 2020 7472 6163 6573 203d 2070 756c 7365    traces = pulse
-0000b7b0: 2e62 6173 6973 2e66 6f75 725f 656c 656d  .basis.four_elem
-0000b7c0: 656e 745f 7472 6163 6573 0a20 2020 2020  ent_traces.     
-0000b7d0: 2020 2063 756d 756c 616e 745f 6675 6e63     cumulant_func
-0000b7e0: 7469 6f6e 203d 202d 2028 0a20 2020 2020  tion = - (.     
-0000b7f0: 2020 2020 2020 202b 206f 652e 636f 6e74         + oe.cont
-0000b800: 7261 6374 2827 2e2e 2e6b 6c2c 6b6c 6a69  ract('...kl,klji
-0000b810: 2d3e 2e2e 2e69 6a27 2c20 6465 6361 795f  ->...ij', decay_
-0000b820: 616d 706c 6974 7564 6573 2c20 7472 6163  amplitudes, trac
-0000b830: 6573 2c20 6261 636b 656e 643d 2773 7061  es, backend='spa
-0000b840: 7273 6527 290a 2020 2020 2020 2020 2020  rse').          
-0000b850: 2020 2d20 6f65 2e63 6f6e 7472 6163 7428    - oe.contract(
-0000b860: 272e 2e2e 6b6c 2c6b 6a6c 692d 3e2e 2e2e  '...kl,kjli->...
-0000b870: 696a 272c 2064 6563 6179 5f61 6d70 6c69  ij', decay_ampli
-0000b880: 7475 6465 732c 2074 7261 6365 732c 2062  tudes, traces, b
-0000b890: 6163 6b65 6e64 3d27 7370 6172 7365 2729  ackend='sparse')
-0000b8a0: 0a20 2020 2020 2020 2020 2020 202d 206f  .            - o
-0000b8b0: 652e 636f 6e74 7261 6374 2827 2e2e 2e6b  e.contract('...k
-0000b8c0: 6c2c 6b69 6c6a 2d3e 2e2e 2e69 6a27 2c20  l,kilj->...ij', 
-0000b8d0: 6465 6361 795f 616d 706c 6974 7564 6573  decay_amplitudes
-0000b8e0: 2c20 7472 6163 6573 2c20 6261 636b 656e  , traces, backen
-0000b8f0: 643d 2773 7061 7273 6527 290a 2020 2020  d='sparse').    
-0000b900: 2020 2020 2020 2020 2b20 6f65 2e63 6f6e          + oe.con
-0000b910: 7472 6163 7428 272e 2e2e 6b6c 2c6b 696a  tract('...kl,kij
-0000b920: 6c2d 3e2e 2e2e 696a 272c 2064 6563 6179  l->...ij', decay
-0000b930: 5f61 6d70 6c69 7475 6465 732c 2074 7261  _amplitudes, tra
-0000b940: 6365 732c 2062 6163 6b65 6e64 3d27 7370  ces, backend='sp
-0000b950: 6172 7365 2729 0a20 2020 2020 2020 2029  arse').        )
-0000b960: 202f 2032 0a20 2020 2020 2020 2069 6620   / 2.        if 
-0000b970: 7365 636f 6e64 5f6f 7264 6572 3a0a 2020  second_order:.  
-0000b980: 2020 2020 2020 2020 2020 6375 6d75 6c61            cumula
-0000b990: 6e74 5f66 756e 6374 696f 6e20 2d3d 2028  nt_function -= (
-0000b9a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b9b0: 202b 206f 652e 636f 6e74 7261 6374 2827   + oe.contract('
-0000b9c0: 2e2e 2e6b 6c2c 6b6c 6a69 2d3e 2e2e 2e69  ...kl,klji->...i
-0000b9d0: 6a27 2c20 6672 6571 7565 6e63 795f 7368  j', frequency_sh
-0000b9e0: 6966 7473 2c20 7472 6163 6573 2c20 6261  ifts, traces, ba
-0000b9f0: 636b 656e 643d 2773 7061 7273 6527 290a  ckend='sparse').
-0000ba00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ba10: 2d20 6f65 2e63 6f6e 7472 6163 7428 272e  - oe.contract('.
-0000ba20: 2e2e 6b6c 2c6c 6b6a 692d 3e2e 2e2e 696a  ..kl,lkji->...ij
-0000ba30: 272c 2066 7265 7175 656e 6379 5f73 6869  ', frequency_shi
-0000ba40: 6674 732c 2074 7261 6365 732c 2062 6163  fts, traces, bac
-0000ba50: 6b65 6e64 3d27 7370 6172 7365 2729 0a20  kend='sparse'). 
-0000ba60: 2020 2020 2020 2020 2020 2020 2020 202d                 -
-0000ba70: 206f 652e 636f 6e74 7261 6374 2827 2e2e   oe.contract('..
-0000ba80: 2e6b 6c2c 6b6c 696a 2d3e 2e2e 2e69 6a27  .kl,klij->...ij'
-0000ba90: 2c20 6672 6571 7565 6e63 795f 7368 6966  , frequency_shif
-0000baa0: 7473 2c20 7472 6163 6573 2c20 6261 636b  ts, traces, back
-0000bab0: 656e 643d 2773 7061 7273 6527 290a 2020  end='sparse').  
-0000bac0: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-0000bad0: 6f65 2e63 6f6e 7472 6163 7428 272e 2e2e  oe.contract('...
-0000bae0: 6b6c 2c6c 6b69 6a2d 3e2e 2e2e 696a 272c  kl,lkij->...ij',
-0000baf0: 2066 7265 7175 656e 6379 5f73 6869 6674   frequency_shift
-0000bb00: 732c 2074 7261 6365 732c 2062 6163 6b65  s, traces, backe
-0000bb10: 6e64 3d27 7370 6172 7365 2729 0a20 2020  nd='sparse').   
-0000bb20: 2020 2020 2020 2020 2029 202f 2032 0a0a           ) / 2..
-0000bb30: 2020 2020 7265 7475 726e 2063 756d 756c      return cumul
-0000bb40: 616e 745f 6675 6e63 7469 6f6e 2e72 6561  ant_function.rea
-0000bb50: 6c0a 0a0a 4075 7469 6c2e 7061 7273 655f  l...@util.parse_
-0000bb60: 6f70 7469 6f6e 616c 5f70 6172 616d 6574  optional_paramet
-0000bb70: 6572 7328 7768 6963 683d 2827 746f 7461  ers(which=('tota
-0000bb80: 6c27 2c20 2763 6f72 7265 6c61 7469 6f6e  l', 'correlation
-0000bb90: 7327 2929 0a64 6566 2063 616c 6375 6c61  s')).def calcula
-0000bba0: 7465 5f64 6563 6179 5f61 6d70 6c69 7475  te_decay_amplitu
-0000bbb0: 6465 7328 0a20 2020 2020 2020 2070 756c  des(.        pul
-0000bbc0: 7365 3a20 2750 756c 7365 5365 7175 656e  se: 'PulseSequen
-0000bbd0: 6365 272c 0a20 2020 2020 2020 2073 7065  ce',.        spe
-0000bbe0: 6374 7275 6d3a 206e 6461 7272 6179 2c0a  ctrum: ndarray,.
-0000bbf0: 2020 2020 2020 2020 6f6d 6567 613a 2043          omega: C
-0000bc00: 6f65 6666 6963 6965 6e74 732c 0a20 2020  oefficients,.   
-0000bc10: 2020 2020 206e 5f6f 7065 725f 6964 656e       n_oper_iden
-0000bc20: 7469 6669 6572 733a 204f 7074 696f 6e61  tifiers: Optiona
-0000bc30: 6c5b 5365 7175 656e 6365 5b73 7472 5d5d  l[Sequence[str]]
-0000bc40: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-0000bc50: 2077 6869 6368 3a20 7374 7220 3d20 2774   which: str = 't
-0000bc60: 6f74 616c 272c 0a20 2020 2020 2020 2073  otal',.        s
-0000bc70: 686f 775f 7072 6f67 7265 7373 6261 723a  how_progressbar:
-0000bc80: 2062 6f6f 6c20 3d20 4661 6c73 652c 0a20   bool = False,. 
-0000bc90: 2020 2020 2020 2063 6163 6865 5f69 6e74         cache_int
-0000bca0: 6572 6d65 6469 6174 6573 3a20 626f 6f6c  ermediates: bool
-0000bcb0: 203d 2046 616c 7365 2c0a 2020 2020 2020   = False,.      
-0000bcc0: 2020 6d65 6d6f 7279 5f70 6172 7369 6d6f    memory_parsimo
-0000bcd0: 6e69 6f75 733a 2062 6f6f 6c20 3d20 4661  nious: bool = Fa
-0000bce0: 6c73 650a 2920 2d3e 206e 6461 7272 6179  lse.) -> ndarray
-0000bcf0: 3a0a 2020 2020 7222 2222 0a20 2020 2047  :.    r""".    G
-0000bd00: 6574 2074 6865 2064 6563 6179 2061 6d70  et the decay amp
-0000bd10: 6c69 7475 6465 7320 3a6d 6174 683a 605c  litudes :math:`\
-0000bd20: 4761 6d6d 615f 7b5c 616c 7068 615c 6265  Gamma_{\alpha\be
-0000bd30: 7461 2c20 6b6c 7d60 2066 6f72 206e 6f69  ta, kl}` for noi
-0000bd40: 7365 0a20 2020 2073 6f75 7263 6573 203a  se.    sources :
-0000bd50: 6d61 7468 3a60 5c61 6c70 6861 2c5c 6265  math:`\alpha,\be
-0000bd60: 7461 6020 616e 6420 6261 7369 7320 656c  ta` and basis el
-0000bd70: 656d 656e 7473 203a 6d61 7468 3a60 6b2c  ements :math:`k,
-0000bd80: 6c60 2e0a 0a20 2020 2050 6172 616d 6574  l`...    Paramet
-0000bd90: 6572 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ers.    --------
-0000bda0: 2d2d 0a20 2020 2070 756c 7365 3a20 5075  --.    pulse: Pu
-0000bdb0: 6c73 6553 6571 7565 6e63 650a 2020 2020  lseSequence.    
-0000bdc0: 2020 2020 5468 6520 6060 5075 6c73 6553      The ``PulseS
-0000bdd0: 6571 7565 6e63 6560 6020 696e 7374 616e  equence`` instan
-0000bde0: 6365 2066 6f72 2077 6869 6368 2074 6f20  ce for which to 
-0000bdf0: 636f 6d70 7574 6520 7468 6520 6465 6361  compute the deca
-0000be00: 790a 2020 2020 2020 2020 616d 706c 6974  y.        amplit
-0000be10: 7564 6573 2e0a 2020 2020 7370 6563 7472  udes..    spectr
-0000be20: 756d 3a20 6172 7261 795f 6c69 6b65 2c20  um: array_like, 
-0000be30: 7368 6170 6520 285b 5b6e 5f6e 6f70 732c  shape ([[n_nops,
-0000be40: 5d20 6e5f 6e6f 7073 2c5d 206e 5f6f 6d65  ] n_nops,] n_ome
-0000be50: 6761 290a 2020 2020 2020 2020 5468 6520  ga).        The 
-0000be60: 6e6f 6973 6520 706f 7765 7220 7370 6563  noise power spec
-0000be70: 7472 616c 2064 656e 7369 7479 2e20 4966  tral density. If
-0000be80: 2031 2d64 2c20 7468 6520 7361 6d65 2073   1-d, the same s
-0000be90: 7065 6374 7275 6d20 6973 0a20 2020 2020  pectrum is.     
-0000bea0: 2020 2075 7365 6420 666f 7220 616c 6c20     used for all 
-0000beb0: 6e6f 6973 6520 6f70 6572 6174 6f72 732e  noise operators.
-0000bec0: 2049 6620 322d 642c 206f 6e65 2028 7365   If 2-d, one (se
-0000bed0: 6c66 2d29 2073 7065 6374 7275 6d20 666f  lf-) spectrum fo
-0000bee0: 720a 2020 2020 2020 2020 6561 6368 206e  r.        each n
-0000bef0: 6f69 7365 206f 7065 7261 746f 7220 6973  oise operator is
-0000bf00: 2065 7870 6563 7465 642e 2049 6620 332d   expected. If 3-
-0000bf10: 642c 2073 686f 756c 6420 6265 2061 206d  d, should be a m
-0000bf20: 6174 7269 7820 6f66 0a20 2020 2020 2020  atrix of.       
-0000bf30: 2063 726f 7373 2d73 7065 6374 7261 2073   cross-spectra s
-0000bf40: 7563 6820 7468 6174 0a20 2020 2020 2020  uch that.       
-0000bf50: 2060 6073 7065 6374 7275 6d5b 692c 206a   ``spectrum[i, j
-0000bf60: 5d20 3d3d 2073 7065 6374 7275 6d5b 6a2c  ] == spectrum[j,
-0000bf70: 2069 5d2e 636f 6e6a 2829 6060 2e0a 2020   i].conj()``..  
-0000bf80: 2020 6f6d 6567 613a 2061 7272 6179 5f6c    omega: array_l
-0000bf90: 696b 652c 0a20 2020 2020 2020 2054 6865  ike,.        The
-0000bfa0: 2066 7265 7175 656e 6369 6573 2061 7420   frequencies at 
-0000bfb0: 7768 6963 6820 746f 2063 616c 6375 6c61  which to calcula
-0000bfc0: 7465 2074 6865 2066 696c 7465 7220 6675  te the filter fu
-0000bfd0: 6e63 7469 6f6e 732e 0a20 2020 206e 5f6f  nctions..    n_o
-0000bfe0: 7065 725f 6964 656e 7469 6669 6572 733a  per_identifiers:
-0000bff0: 2061 7272 6179 5f6c 696b 652c 206f 7074   array_like, opt
-0000c000: 696f 6e61 6c0a 2020 2020 2020 2020 5468  ional.        Th
-0000c010: 6520 6964 656e 7469 6669 6572 7320 6f66  e identifiers of
-0000c020: 2074 6865 206e 6f69 7365 206f 7065 7261   the noise opera
-0000c030: 746f 7273 2066 6f72 2077 6869 6368 2074  tors for which t
-0000c040: 6f20 6361 6c63 756c 6174 650a 2020 2020  o calculate.    
-0000c050: 2020 2020 7468 6520 6465 6361 7920 616d      the decay am
-0000c060: 706c 6974 7564 6573 2e20 5468 6520 6465  plitudes. The de
-0000c070: 6661 756c 7420 6973 2061 6c6c 2e0a 2020  fault is all..  
-0000c080: 2020 7768 6963 683a 2073 7472 2c20 6f70    which: str, op
-0000c090: 7469 6f6e 616c 0a20 2020 2020 2020 2057  tional.        W
-0000c0a0: 6869 6368 2064 6563 6179 2061 6d70 6c69  hich decay ampli
-0000c0b0: 7475 6465 7320 7368 6f75 6c64 2062 6520  tudes should be 
-0000c0c0: 6361 6c63 756c 6174 6564 2c20 6d61 7920  calculated, may 
-0000c0d0: 6265 2065 6974 6865 720a 2020 2020 2020  be either.      
-0000c0e0: 2020 2774 6f74 616c 2720 2864 6566 6175    'total' (defau
-0000c0f0: 6c74 2920 6f72 2027 636f 7272 656c 6174  lt) or 'correlat
-0000c100: 696f 6e73 272e 2053 6565 203a 6675 6e63  ions'. See :func
-0000c110: 3a60 696e 6669 6465 6c69 7479 6020 616e  :`infidelity` an
-0000c120: 640a 2020 2020 2020 2020 3a72 6566 3a60  d.        :ref:`
-0000c130: 4e6f 7465 7320 3c6e 6f74 6573 3e60 2e0a  Notes <notes>`..
-0000c140: 2020 2020 7368 6f77 5f70 726f 6772 6573      show_progres
-0000c150: 7362 6172 3a20 626f 6f6c 2c20 6f70 7469  sbar: bool, opti
-0000c160: 6f6e 616c 0a20 2020 2020 2020 2053 686f  onal.        Sho
-0000c170: 7720 6120 7072 6f67 7265 7373 2062 6172  w a progress bar
-0000c180: 2066 6f72 2074 6865 2063 616c 6375 6c61   for the calcula
-0000c190: 7469 6f6e 2e0a 2020 2020 6361 6368 655f  tion..    cache_
-0000c1a0: 696e 7465 726d 6564 6961 7465 733a 2062  intermediates: b
-0000c1b0: 6f6f 6c2c 206f 7074 696f 6e61 6c0a 2020  ool, optional.  
-0000c1c0: 2020 2020 2020 4b65 6570 2061 6e64 2072        Keep and r
-0000c1d0: 6574 7572 6e20 696e 7465 726d 6564 6961  eturn intermedia
-0000c1e0: 7465 2074 6572 6d73 206f 6620 7468 6520  te terms of the 
-0000c1f0: 6361 6c63 756c 6174 696f 6e20 7468 6174  calculation that
-0000c200: 2061 7265 0a20 2020 2020 2020 2075 7365   are.        use
-0000c210: 6675 6c20 696e 206f 7468 6572 2070 6c61  ful in other pla
-0000c220: 6365 7320 2869 6620 636f 6e74 726f 6c20  ces (if control 
-0000c230: 6d61 7472 6978 206e 6f74 2061 6c72 6561  matrix not alrea
-0000c240: 6479 2063 6163 6865 6429 2e0a 2020 2020  dy cached)..    
-0000c250: 6d65 6d6f 7279 5f70 6172 7369 6d6f 6e69  memory_parsimoni
-0000c260: 6f75 733a 2062 6f6f 6c2c 206f 7074 696f  ous: bool, optio
-0000c270: 6e61 6c0a 2020 2020 2020 2020 466f 7220  nal.        For 
-0000c280: 6c61 7267 6520 6469 6d65 6e73 696f 6e73  large dimensions
-0000c290: 2c20 7468 6520 696e 7465 6772 616e 640a  , the integrand.
-0000c2a0: 0a20 2020 2020 2020 202e 2e20 6d61 7468  .        .. math
-0000c2b0: 3a3a 0a0a 2020 2020 2020 2020 2020 2020  ::..            
-0000c2c0: 5c74 696c 6465 7b5c 6d61 7468 6361 6c7b  \tilde{\mathcal{
-0000c2d0: 427d 7d5e 5c61 7374 5f7b 5c61 6c70 6861  B}}^\ast_{\alpha
-0000c2e0: 206b 7d28 5c6f 6d65 6761 290a 2020 2020   k}(\omega).    
-0000c2f0: 2020 2020 2020 2020 535f 7b5c 616c 7068          S_{\alph
-0000c300: 615c 6265 7461 7d28 5c6f 6d65 6761 295c  a\beta}(\omega)\
-0000c310: 7469 6c64 657b 5c6d 6174 6863 616c 7b42  tilde{\mathcal{B
-0000c320: 7d7d 5f7b 5c62 6574 6120 6c7d 285c 6f6d  }}_{\beta l}(\om
-0000c330: 6567 6129 0a0a 2020 2020 2020 2020 6361  ega)..        ca
-0000c340: 6e20 636f 6e73 756d 6520 7175 6974 6520  n consume quite 
-0000c350: 6120 6c61 7267 6520 616d 6f75 6e74 206f  a large amount o
-0000c360: 6620 6d65 6d6f 7279 2069 6620 7365 7420  f memory if set 
-0000c370: 7570 2066 6f72 2061 6c6c 0a20 2020 2020  up for all.     
-0000c380: 2020 203a 6d61 7468 3a60 5c61 6c70 6861     :math:`\alpha
-0000c390: 2c5c 6265 7461 2c6b 2c6c 6020 6174 206f  ,\beta,k,l` at o
-0000c3a0: 6e63 652e 2049 6620 6060 5472 7565 6060  nce. If ``True``
-0000c3b0: 2c20 6974 2069 7320 6f6e 6c79 2073 6574  , it is only set
-0000c3c0: 2075 700a 2020 2020 2020 2020 616e 6420   up.        and 
-0000c3d0: 696e 7465 6772 6174 6564 2066 6f72 2061  integrated for a
-0000c3e0: 2073 696e 676c 6520 3a6d 6174 683a 606b   single :math:`k
-0000c3f0: 6020 6174 2061 2074 696d 6520 616e 6420  ` at a time and 
-0000c400: 6c6f 6f70 6564 206f 7665 722e 0a20 2020  looped over..   
-0000c410: 2020 2020 2054 6869 7320 6973 2073 6c6f       This is slo
-0000c420: 7765 7220 6275 7420 7265 7175 6972 6573  wer but requires
-0000c430: 206d 7563 6820 6c65 7373 206d 656d 6f72   much less memor
-0000c440: 792e 2054 6865 2064 6566 6175 6c74 2069  y. The default i
-0000c450: 730a 2020 2020 2020 2020 6060 4661 6c73  s.        ``Fals
-0000c460: 6560 602e 0a0a 2020 2020 5261 6973 6573  e``...    Raises
-0000c470: 0a20 2020 202d 2d2d 2d2d 2d0a 2020 2020  .    ------.    
-0000c480: 5661 6c75 6545 7272 6f72 0a20 2020 2020  ValueError.     
-0000c490: 2020 2049 6620 7370 6563 7472 756d 2068     If spectrum h
-0000c4a0: 6173 2069 6e63 6f6d 7061 7469 626c 6520  as incompatible 
-0000c4b0: 7368 6170 652e 0a0a 2020 2020 5265 7475  shape...    Retu
-0000c4c0: 726e 730a 2020 2020 2d2d 2d2d 2d2d 2d0a  rns.    -------.
-0000c4d0: 2020 2020 6465 6361 795f 616d 706c 6974      decay_amplit
-0000c4e0: 7564 6573 3a20 6e64 6172 7261 792c 2073  udes: ndarray, s
-0000c4f0: 6861 7065 2028 5b5b 6e5f 706c 732c 206e  hape ([[n_pls, n
-0000c500: 5f70 6c73 2c5d 206e 5f6e 6f70 732c 5d20  _pls,] n_nops,] 
-0000c510: 6e5f 6e6f 7073 2c20 642a 2a32 2c20 642a  n_nops, d**2, d*
-0000c520: 2a32 290a 2020 2020 2020 2020 5468 6520  *2).        The 
-0000c530: 6465 6361 7920 616d 706c 6974 7564 6573  decay amplitudes
-0000c540: 2e0a 0a20 2020 202e 2e20 5f6e 6f74 6573  ...    .. _notes
-0000c550: 3a0a 0a20 2020 204e 6f74 6573 0a20 2020  :..    Notes.   
-0000c560: 202d 2d2d 2d2d 0a20 2020 2054 6865 2074   -----.    The t
-0000c570: 6f74 616c 2064 6563 6179 2061 6d70 6c69  otal decay ampli
-0000c580: 7475 6465 7320 6172 6520 6769 7665 6e20  tudes are given 
-0000c590: 6279 0a0a 2020 2020 2e2e 206d 6174 683a  by..    .. math:
-0000c5a0: 3a0a 0a20 2020 2020 2020 205c 4761 6d6d  :..        \Gamm
-0000c5b0: 615f 7b5c 616c 7068 615c 6265 7461 2c20  a_{\alpha\beta, 
-0000c5c0: 6b6c 7d20 3d20 5c69 6e74 5c66 7261 637b  kl} = \int\frac{
-0000c5d0: 5c6d 6174 6872 6d7b 647d 5c6f 6d65 6761  \mathrm{d}\omega
-0000c5e0: 7d7b 325c 7069 7d0a 2020 2020 2020 2020  }{2\pi}.        
-0000c5f0: 2020 2020 5c74 696c 6465 7b5c 6d61 7468      \tilde{\math
-0000c600: 6361 6c7b 427d 7d5e 5c61 7374 5f7b 5c61  cal{B}}^\ast_{\a
-0000c610: 6c70 6861 206b 7d28 5c6f 6d65 6761 290a  lpha k}(\omega).
-0000c620: 2020 2020 2020 2020 2020 2020 535f 7b5c              S_{\
-0000c630: 616c 7068 615c 6265 7461 7d28 5c6f 6d65  alpha\beta}(\ome
-0000c640: 6761 295c 7469 6c64 657b 5c6d 6174 6863  ga)\tilde{\mathc
-0000c650: 616c 7b42 7d7d 5f7b 5c62 6574 6120 6c7d  al{B}}_{\beta l}
-0000c660: 285c 6f6d 6567 6129 2e0a 0a20 2020 2049  (\omega)...    I
-0000c670: 6620 7075 6c73 6520 636f 7272 656c 6174  f pulse correlat
-0000c680: 696f 6e73 2061 7265 2074 616b 656e 2069  ions are taken i
-0000c690: 6e74 6f20 6163 636f 756e 742c 2074 6865  nto account, the
-0000c6a0: 7920 6172 6520 6769 7665 6e20 6279 0a0a  y are given by..
-0000c6b0: 2020 2020 2e2e 206d 6174 683a 3a0a 0a20      .. math::.. 
-0000c6c0: 2020 2020 2020 205c 4761 6d6d 615f 7b5c         \Gamma_{\
-0000c6d0: 616c 7068 615c 6265 7461 2c20 6b6c 7d5e  alpha\beta, kl}^
-0000c6e0: 7b28 6767 2729 7d20 3d20 5c69 6e74 0a20  {(gg')} = \int. 
-0000c6f0: 2020 2020 2020 2020 2020 205c 6672 6163             \frac
-0000c700: 7b5c 6d61 7468 726d 7b64 7d5c 6f6d 6567  {\mathrm{d}\omeg
-0000c710: 617d 7b32 5c70 697d 2053 5f7b 5c61 6c70  a}{2\pi} S_{\alp
-0000c720: 6861 5c62 6574 617d 285c 6f6d 6567 6129  ha\beta}(\omega)
-0000c730: 0a20 2020 2020 2020 2020 2020 2046 5f7b  .            F_{
-0000c740: 5c61 6c70 6861 5c62 6574 612c 206b 6c7d  \alpha\beta, kl}
-0000c750: 5e7b 2867 6727 297d 285c 6f6d 6567 6129  ^{(gg')}(\omega)
-0000c760: 2e0a 0a20 2020 2053 6565 2041 6c73 6f0a  ...    See Also.
-0000c770: 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020      --------.   
-0000c780: 2069 6e66 6964 656c 6974 793a 2043 6f6d   infidelity: Com
-0000c790: 7075 7465 2074 6865 2069 6e66 6964 656c  pute the infidel
-0000c7a0: 6974 7920 6469 7265 6374 6c79 2e0a 2020  ity directly..  
-0000c7b0: 2020 7075 6c73 655f 7365 7175 656e 6365    pulse_sequence
-0000c7c0: 2e63 6f6e 6361 7465 6e61 7465 3a20 436f  .concatenate: Co
-0000c7d0: 6e63 6174 656e 6174 6520 6060 5075 6c73  ncatenate ``Puls
-0000c7e0: 6553 6571 7565 6e63 6560 6020 6f62 6a65  eSequence`` obje
-0000c7f0: 6374 732e 0a20 2020 2063 616c 6375 6c61  cts..    calcula
-0000c800: 7465 5f66 7265 7175 656e 6379 5f73 6869  te_frequency_shi
-0000c810: 6674 733a 2053 6563 6f6e 6420 6f72 6465  fts: Second orde
-0000c820: 7220 2875 6e69 7461 7279 2920 7465 726d  r (unitary) term
-0000c830: 732e 0a20 2020 2063 616c 6375 6c61 7465  s..    calculate
-0000c840: 5f70 756c 7365 5f63 6f72 7265 6c61 7469  _pulse_correlati
-0000c850: 6f6e 5f66 696c 7465 725f 6675 6e63 7469  on_filter_functi
-0000c860: 6f6e 0a20 2020 2022 2222 0a20 2020 2023  on.    """.    #
-0000c870: 2054 4f44 4f3a 2052 6570 6c61 6365 2069   TODO: Replace i
-0000c880: 6e66 6964 656c 6974 7928 2920 6279 2074  nfidelity() by t
-0000c890: 6869 733f 0a20 2020 2023 204e 6f69 7365  his?.    # Noise
-0000c8a0: 206f 7065 7261 746f 7220 696e 6469 6365   operator indice
-0000c8b0: 730a 2020 2020 6964 7820 3d20 7574 696c  s.    idx = util
-0000c8c0: 2e67 6574 5f69 6e64 6963 6573 5f66 726f  .get_indices_fro
-0000c8d0: 6d5f 6964 656e 7469 6669 6572 7328 7075  m_identifiers(pu
-0000c8e0: 6c73 652e 6e5f 6f70 6572 5f69 6465 6e74  lse.n_oper_ident
-0000c8f0: 6966 6965 7273 2c20 6e5f 6f70 6572 5f69  ifiers, n_oper_i
-0000c900: 6465 6e74 6966 6965 7273 290a 2020 2020  dentifiers).    
-0000c910: 6966 2077 6869 6368 203d 3d20 2774 6f74  if which == 'tot
-0000c920: 616c 273a 0a20 2020 2020 2020 2023 2046  al':.        # F
-0000c930: 6173 7465 7220 746f 2075 7365 2066 696c  aster to use fil
-0000c940: 7465 7220 6675 6e63 7469 6f6e 2069 6e73  ter function ins
-0000c950: 7465 6164 206f 6620 636f 6e74 726f 6c20  tead of control 
-0000c960: 6d61 7472 6978 0a20 2020 2020 2020 2069  matrix.        i
-0000c970: 6620 7075 6c73 652e 6973 5f63 6163 6865  f pulse.is_cache
-0000c980: 6428 2766 696c 7465 725f 6675 6e63 7469  d('filter_functi
-0000c990: 6f6e 5f67 656e 2729 3a0a 2020 2020 2020  on_gen'):.      
-0000c9a0: 2020 2020 2020 636f 6e74 726f 6c5f 6d61        control_ma
-0000c9b0: 7472 6978 203d 204e 6f6e 650a 2020 2020  trix = None.    
-0000c9c0: 2020 2020 2020 2020 6669 6c74 6572 5f66          filter_f
-0000c9d0: 756e 6374 696f 6e20 3d20 7075 6c73 652e  unction = pulse.
-0000c9e0: 6765 745f 6669 6c74 6572 5f66 756e 6374  get_filter_funct
-0000c9f0: 696f 6e28 6f6d 6567 612c 2077 6869 6368  ion(omega, which
-0000ca00: 3d27 6765 6e65 7261 6c69 7a65 6427 290a  ='generalized').
-0000ca10: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0000ca20: 2020 2020 2020 2020 2020 636f 6e74 726f            contro
-0000ca30: 6c5f 6d61 7472 6978 203d 2070 756c 7365  l_matrix = pulse
-0000ca40: 2e67 6574 5f63 6f6e 7472 6f6c 5f6d 6174  .get_control_mat
-0000ca50: 7269 7828 6f6d 6567 612c 2073 686f 775f  rix(omega, show_
-0000ca60: 7072 6f67 7265 7373 6261 722c 2063 6163  progressbar, cac
-0000ca70: 6865 5f69 6e74 6572 6d65 6469 6174 6573  he_intermediates
-0000ca80: 290a 2020 2020 2020 2020 2020 2020 6669  ).            fi
-0000ca90: 6c74 6572 5f66 756e 6374 696f 6e20 3d20  lter_function = 
-0000caa0: 4e6f 6e65 0a20 2020 2065 6c73 653a 0a20  None.    else:. 
-0000cab0: 2020 2020 2020 2023 2077 6869 6368 203d         # which =
-0000cac0: 3d20 2763 6f72 7265 6c61 7469 6f6e 7327  = 'correlations'
-0000cad0: 0a20 2020 2020 2020 2069 6620 7075 6c73  .        if puls
-0000cae0: 652e 6973 5f63 6163 6865 6428 276f 6d65  e.is_cached('ome
-0000caf0: 6761 2729 3a0a 2020 2020 2020 2020 2020  ga'):.          
-0000cb00: 2020 6966 206e 6f74 206e 702e 6172 7261    if not np.arra
-0000cb10: 795f 6571 7561 6c28 7075 6c73 652e 6f6d  y_equal(pulse.om
-0000cb20: 6567 612c 206f 6d65 6761 293a 0a20 2020  ega, omega):.   
-0000cb30: 2020 2020 2020 2020 2020 2020 2072 6169               rai
-0000cb40: 7365 2056 616c 7565 4572 726f 7228 2750  se ValueError('P
-0000cb50: 756c 7365 2063 6f72 7265 6c61 7469 6f6e  ulse correlation
-0000cb60: 2064 6563 6179 2061 6d70 6c69 7475 6465   decay amplitude
-0000cb70: 7320 7265 7175 6573 7465 6420 6275 7420  s requested but 
-0000cb80: 6f6d 6567 6120 6e6f 7420 2720 2b0a 2020  omega not ' +.  
-0000cb90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cba0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-0000cbb0: 6571 7561 6c20 746f 2063 6163 6865 6420  equal to cached 
-0000cbc0: 6672 6571 7565 6e63 6965 732e 2729 0a0a  frequencies.')..
-0000cbd0: 2020 2020 2020 2020 6966 2070 756c 7365          if pulse
-0000cbe0: 2e69 735f 6361 6368 6564 2827 6669 6c74  .is_cached('filt
-0000cbf0: 6572 5f66 756e 6374 696f 6e5f 7063 5f67  er_function_pc_g
-0000cc00: 656e 2729 3a0a 2020 2020 2020 2020 2020  en'):.          
-0000cc10: 2020 636f 6e74 726f 6c5f 6d61 7472 6978    control_matrix
-0000cc20: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
-0000cc30: 2020 2020 6669 6c74 6572 5f66 756e 6374      filter_funct
-0000cc40: 696f 6e20 3d20 7075 6c73 652e 6765 745f  ion = pulse.get_
-0000cc50: 7075 6c73 655f 636f 7272 656c 6174 696f  pulse_correlatio
-0000cc60: 6e5f 6669 6c74 6572 5f66 756e 6374 696f  n_filter_functio
-0000cc70: 6e28 7768 6963 683d 2767 656e 6572 616c  n(which='general
-0000cc80: 697a 6564 2729 0a20 2020 2020 2020 2065  ized').        e
-0000cc90: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000cca0: 2063 6f6e 7472 6f6c 5f6d 6174 7269 7820   control_matrix 
-0000ccb0: 3d20 7075 6c73 652e 6765 745f 7075 6c73  = pulse.get_puls
-0000ccc0: 655f 636f 7272 656c 6174 696f 6e5f 636f  e_correlation_co
-0000ccd0: 6e74 726f 6c5f 6d61 7472 6978 2829 0a20  ntrol_matrix(). 
-0000cce0: 2020 2020 2020 2020 2020 2066 696c 7465             filte
-0000ccf0: 725f 6675 6e63 7469 6f6e 203d 204e 6f6e  r_function = Non
-0000cd00: 650a 0a20 2020 2069 6620 6e6f 7420 6d65  e..    if not me
-0000cd10: 6d6f 7279 5f70 6172 7369 6d6f 6e69 6f75  mory_parsimoniou
-0000cd20: 733a 0a20 2020 2020 2020 2069 6e74 6567  s:.        integ
-0000cd30: 7261 6e64 203d 205f 6765 745f 696e 7465  rand = _get_inte
-0000cd40: 6772 616e 6428 7370 6563 7472 756d 2c20  grand(spectrum, 
-0000cd50: 6f6d 6567 612c 2069 6478 2c20 7768 6963  omega, idx, whic
-0000cd60: 682c 2027 6765 6e65 7261 6c69 7a65 6427  h, 'generalized'
-0000cd70: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000cd80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cd90: 2020 2020 2063 6f6e 7472 6f6c 5f6d 6174       control_mat
-0000cda0: 7269 783d 636f 6e74 726f 6c5f 6d61 7472  rix=control_matr
-0000cdb0: 6978 2c0a 2020 2020 2020 2020 2020 2020  ix,.            
-0000cdc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cdd0: 2020 2020 2020 2066 696c 7465 725f 6675         filter_fu
-0000cde0: 6e63 7469 6f6e 3d66 696c 7465 725f 6675  nction=filter_fu
-0000cdf0: 6e63 7469 6f6e 290a 2020 2020 2020 2020  nction).        
-0000ce00: 6465 6361 795f 616d 706c 6974 7564 6573  decay_amplitudes
-0000ce10: 203d 2075 7469 6c2e 696e 7465 6772 6174   = util.integrat
-0000ce20: 6528 696e 7465 6772 616e 642c 206f 6d65  e(integrand, ome
-0000ce30: 6761 292f 2832 2a6e 702e 7069 290a 2020  ga)/(2*np.pi).  
-0000ce40: 2020 2020 2020 7265 7475 726e 2064 6563        return dec
-0000ce50: 6179 5f61 6d70 6c69 7475 6465 730a 0a20  ay_amplitudes.. 
-0000ce60: 2020 206e 5f6b 6c20 3d20 6c65 6e28 7075     n_kl = len(pu
-0000ce70: 6c73 652e 6261 7369 7329 0a20 2020 2066  lse.basis).    f
-0000ce80: 6f72 206b 2069 6e20 7574 696c 2e70 726f  or k in util.pro
-0000ce90: 6772 6573 7362 6172 5f72 616e 6765 286e  gressbar_range(n
-0000cea0: 5f6b 6c2c 2073 686f 775f 7072 6f67 7265  _kl, show_progre
-0000ceb0: 7373 6261 723d 7368 6f77 5f70 726f 6772  ssbar=show_progr
-0000cec0: 6573 7362 6172 2c20 6465 7363 3d27 496e  essbar, desc='In
-0000ced0: 7465 6772 6174 696e 6727 293a 0a20 2020  tegrating'):.   
-0000cee0: 2020 2020 2069 6620 636f 6e74 726f 6c5f       if control_
-0000cef0: 6d61 7472 6978 2069 7320 6e6f 7420 4e6f  matrix is not No
-0000cf00: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0000cf10: 696e 7465 6772 616e 6420 3d20 5f67 6574  integrand = _get
-0000cf20: 5f69 6e74 6567 7261 6e64 280a 2020 2020  _integrand(.    
-0000cf30: 2020 2020 2020 2020 2020 2020 7370 6563              spec
-0000cf40: 7472 756d 2c20 6f6d 6567 612c 2069 6478  trum, omega, idx
-0000cf50: 2c20 7768 6963 682c 2027 6765 6e65 7261  , which, 'genera
-0000cf60: 6c69 7a65 6427 2c0a 2020 2020 2020 2020  lized',.        
-0000cf70: 2020 2020 2020 2020 636f 6e74 726f 6c5f          control_
-0000cf80: 6d61 7472 6978 3d5b 636f 6e74 726f 6c5f  matrix=[control_
-0000cf90: 6d61 7472 6978 5b2e 2e2e 2c20 6b3a 6b2b  matrix[..., k:k+
-0000cfa0: 312c 203a 5d2c 2063 6f6e 7472 6f6c 5f6d  1, :], control_m
-0000cfb0: 6174 7269 785d 2c0a 2020 2020 2020 2020  atrix],.        
-0000cfc0: 2020 2020 2020 2020 6669 6c74 6572 5f66          filter_f
-0000cfd0: 756e 6374 696f 6e3d 6669 6c74 6572 5f66  unction=filter_f
-0000cfe0: 756e 6374 696f 6e0a 2020 2020 2020 2020  unction.        
-0000cff0: 2020 2020 290a 2020 2020 2020 2020 656c      ).        el
-0000d000: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000d010: 696e 7465 6772 616e 6420 3d20 5f67 6574  integrand = _get
-0000d020: 5f69 6e74 6567 7261 6e64 280a 2020 2020  _integrand(.    
-0000d030: 2020 2020 2020 2020 2020 2020 7370 6563              spec
-0000d040: 7472 756d 2c20 6f6d 6567 612c 2069 6478  trum, omega, idx
-0000d050: 2c20 7768 6963 682c 2027 6765 6e65 7261  , which, 'genera
-0000d060: 6c69 7a65 6427 2c0a 2020 2020 2020 2020  lized',.        
-0000d070: 2020 2020 2020 2020 636f 6e74 726f 6c5f          control_
-0000d080: 6d61 7472 6978 3d63 6f6e 7472 6f6c 5f6d  matrix=control_m
-0000d090: 6174 7269 782c 0a20 2020 2020 2020 2020  atrix,.         
-0000d0a0: 2020 2020 2020 2066 696c 7465 725f 6675         filter_fu
-0000d0b0: 6e63 7469 6f6e 3d66 696c 7465 725f 6675  nction=filter_fu
-0000d0c0: 6e63 7469 6f6e 5b2e 2e2e 2c20 6b3a 6b2b  nction[..., k:k+
-0000d0d0: 312c 203a 2c20 3a5d 0a20 2020 2020 2020  1, :, :].       
-0000d0e0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-0000d0f0: 6966 206b 203d 3d20 303a 0a20 2020 2020  if k == 0:.     
-0000d100: 2020 2020 2020 2064 6563 6179 5f61 6d70         decay_amp
-0000d110: 6c69 7475 6465 7320 3d20 6e70 2e65 6d70  litudes = np.emp
-0000d120: 7479 2869 6e74 6567 7261 6e64 2e73 6861  ty(integrand.sha
-0000d130: 7065 5b3a 2d33 5d20 2b20 286e 5f6b 6c2c  pe[:-3] + (n_kl,
-0000d140: 292a 3229 0a0a 2020 2020 2020 2020 6465  )*2)..        de
-0000d150: 6361 795f 616d 706c 6974 7564 6573 5b2e  cay_amplitudes[.
-0000d160: 2e2e 2c20 6b3a 6b2b 312c 203a 5d20 3d20  .., k:k+1, :] = 
-0000d170: 7574 696c 2e69 6e74 6567 7261 7465 2869  util.integrate(i
-0000d180: 6e74 6567 7261 6e64 2c20 6f6d 6567 6129  ntegrand, omega)
-0000d190: 2f28 322a 6e70 2e70 6929 0a0a 2020 2020  /(2*np.pi)..    
-0000d1a0: 7265 7475 726e 2064 6563 6179 5f61 6d70  return decay_amp
-0000d1b0: 6c69 7475 6465 730a 0a0a 6465 6620 6361  litudes...def ca
-0000d1c0: 6c63 756c 6174 655f 6672 6571 7565 6e63  lculate_frequenc
-0000d1d0: 795f 7368 6966 7473 280a 2020 2020 2020  y_shifts(.      
-0000d1e0: 2020 7075 6c73 653a 2027 5075 6c73 6553    pulse: 'PulseS
-0000d1f0: 6571 7565 6e63 6527 2c0a 2020 2020 2020  equence',.      
-0000d200: 2020 7370 6563 7472 756d 3a20 6e64 6172    spectrum: ndar
-0000d210: 7261 792c 0a20 2020 2020 2020 206f 6d65  ray,.        ome
-0000d220: 6761 3a20 436f 6566 6669 6369 656e 7473  ga: Coefficients
-0000d230: 2c0a 2020 2020 2020 2020 6e5f 6f70 6572  ,.        n_oper
-0000d240: 5f69 6465 6e74 6966 6965 7273 3a20 4f70  _identifiers: Op
-0000d250: 7469 6f6e 616c 5b53 6571 7565 6e63 655b  tional[Sequence[
-0000d260: 7374 725d 5d20 3d20 4e6f 6e65 2c0a 2020  str]] = None,.  
-0000d270: 2020 2020 2020 7368 6f77 5f70 726f 6772        show_progr
-0000d280: 6573 7362 6172 3a20 626f 6f6c 203d 2046  essbar: bool = F
-0000d290: 616c 7365 0a29 202d 3e20 6e64 6172 7261  alse.) -> ndarra
-0000d2a0: 793a 0a20 2020 2072 2222 220a 2020 2020  y:.    r""".    
-0000d2b0: 4765 7420 7468 6520 6672 6571 7565 6e63  Get the frequenc
-0000d2c0: 7920 7368 6966 7473 203a 6d61 7468 3a60  y shifts :math:`
-0000d2d0: 5c44 656c 7461 5f7b 5c61 6c70 6861 5c62  \Delta_{\alpha\b
-0000d2e0: 6574 612c 206b 6c7d 6020 666f 7220 6e6f  eta, kl}` for no
-0000d2f0: 6973 650a 2020 2020 736f 7572 6365 7320  ise.    sources 
-0000d300: 3a6d 6174 683a 605c 616c 7068 612c 5c62  :math:`\alpha,\b
-0000d310: 6574 6160 2061 6e64 2062 6173 6973 2065  eta` and basis e
-0000d320: 6c65 6d65 6e74 7320 3a6d 6174 683a 606b  lements :math:`k
-0000d330: 2c6c 602e 0a0a 2020 2020 5061 7261 6d65  ,l`...    Parame
-0000d340: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
-0000d350: 2d2d 2d0a 2020 2020 7075 6c73 653a 2050  ---.    pulse: P
-0000d360: 756c 7365 5365 7175 656e 6365 0a20 2020  ulseSequence.   
-0000d370: 2020 2020 2054 6865 2060 6050 756c 7365       The ``Pulse
-0000d380: 5365 7175 656e 6365 6060 2069 6e73 7461  Sequence`` insta
-0000d390: 6e63 6520 666f 7220 7768 6963 6820 746f  nce for which to
-0000d3a0: 2063 6f6d 7075 7465 2074 6865 0a20 2020   compute the.   
-0000d3b0: 2020 2020 2066 7265 7175 656e 6379 2073       frequency s
-0000d3c0: 6869 6674 732e 0a20 2020 2073 7065 6374  hifts..    spect
-0000d3d0: 7275 6d3a 2061 7272 6179 5f6c 696b 652c  rum: array_like,
-0000d3e0: 2073 6861 7065 2028 5b5b 6e5f 6e6f 7073   shape ([[n_nops
-0000d3f0: 2c5d 206e 5f6e 6f70 732c 5d20 6e5f 6f6d  ,] n_nops,] n_om
-0000d400: 6567 6129 0a20 2020 2020 2020 2054 6865  ega).        The
-0000d410: 2074 776f 2d73 6964 6564 206e 6f69 7365   two-sided noise
-0000d420: 2070 6f77 6572 2073 7065 6374 7261 6c20   power spectral 
-0000d430: 6465 6e73 6974 792e 2049 6620 312d 642c  density. If 1-d,
-0000d440: 2074 6865 2073 616d 650a 2020 2020 2020   the same.      
-0000d450: 2020 7370 6563 7472 756d 2069 7320 7573    spectrum is us
-0000d460: 6564 2066 6f72 2061 6c6c 206e 6f69 7365  ed for all noise
-0000d470: 206f 7065 7261 746f 7273 2e20 4966 2032   operators. If 2
-0000d480: 2d64 2c20 6f6e 6520 2873 656c 662d 290a  -d, one (self-).
-0000d490: 2020 2020 2020 2020 7370 6563 7472 756d          spectrum
-0000d4a0: 2066 6f72 2065 6163 6820 6e6f 6973 6520   for each noise 
-0000d4b0: 6f70 6572 6174 6f72 2069 7320 6578 7065  operator is expe
-0000d4c0: 6374 6564 2e20 4966 2033 2d64 2c20 7368  cted. If 3-d, sh
-0000d4d0: 6f75 6c64 2062 650a 2020 2020 2020 2020  ould be.        
-0000d4e0: 6120 6d61 7472 6978 206f 6620 6372 6f73  a matrix of cros
-0000d4f0: 732d 7370 6563 7472 6120 7375 6368 2074  s-spectra such t
-0000d500: 6861 740a 2020 2020 2020 2020 6060 7370  hat.        ``sp
-0000d510: 6563 7472 756d 5b69 2c20 6a5d 203d 3d20  ectrum[i, j] == 
-0000d520: 7370 6563 7472 756d 5b6a 2c20 695d 2e63  spectrum[j, i].c
-0000d530: 6f6e 6a28 2960 602e 0a20 2020 206f 6d65  onj()``..    ome
-0000d540: 6761 3a20 6172 7261 795f 6c69 6b65 2c0a  ga: array_like,.
-0000d550: 2020 2020 2020 2020 5468 6520 6672 6571          The freq
-0000d560: 7565 6e63 6965 732e 204e 6f74 6520 7468  uencies. Note th
-0000d570: 6174 2074 6865 2066 7265 7175 656e 6369  at the frequenci
-0000d580: 6573 2061 7265 2061 7373 756d 6564 2074  es are assumed t
-0000d590: 6f20 6265 0a20 2020 2020 2020 2073 796d  o be.        sym
-0000d5a0: 6d65 7472 6963 2061 626f 7574 207a 6572  metric about zer
-0000d5b0: 6f2e 0a20 2020 206e 5f6f 7065 725f 6964  o..    n_oper_id
-0000d5c0: 656e 7469 6669 6572 733a 2061 7272 6179  entifiers: array
-0000d5d0: 5f6c 696b 652c 206f 7074 696f 6e61 6c0a  _like, optional.
-0000d5e0: 2020 2020 2020 2020 5468 6520 6964 656e          The iden
-0000d5f0: 7469 6669 6572 7320 6f66 2074 6865 206e  tifiers of the n
-0000d600: 6f69 7365 206f 7065 7261 746f 7273 2066  oise operators f
-0000d610: 6f72 2077 6869 6368 2074 6f20 6361 6c63  or which to calc
-0000d620: 756c 6174 650a 2020 2020 2020 2020 7468  ulate.        th
-0000d630: 6520 6672 6571 7565 6e63 7920 7368 6966  e frequency shif
-0000d640: 7473 2e20 5468 6520 6465 6661 756c 7420  ts. The default 
-0000d650: 6973 2061 6c6c 2e0a 2020 2020 7368 6f77  is all..    show
-0000d660: 5f70 726f 6772 6573 7362 6172 3a20 626f  _progressbar: bo
-0000d670: 6f6c 2c20 6f70 7469 6f6e 616c 0a20 2020  ol, optional.   
-0000d680: 2020 2020 2053 686f 7720 6120 7072 6f67       Show a prog
-0000d690: 7265 7373 2062 6172 2066 6f72 2074 6865  ress bar for the
-0000d6a0: 2063 616c 6375 6c61 7469 6f6e 2e0a 0a20   calculation... 
-0000d6b0: 2020 2052 6169 7365 730a 2020 2020 2d2d     Raises.    --
-0000d6c0: 2d2d 2d2d 0a20 2020 2056 616c 7565 4572  ----.    ValueEr
-0000d6d0: 726f 720a 2020 2020 2020 2020 4966 2073  ror.        If s
-0000d6e0: 7065 6374 7275 6d20 6861 7320 696e 636f  pectrum has inco
-0000d6f0: 6d70 6174 6962 6c65 2073 6861 7065 2e0a  mpatible shape..
-0000d700: 0a20 2020 2052 6574 7572 6e73 0a20 2020  .    Returns.   
-0000d710: 202d 2d2d 2d2d 2d2d 0a20 2020 2044 656c   -------.    Del
-0000d720: 7461 3a20 6e64 6172 7261 792c 2073 6861  ta: ndarray, sha
-0000d730: 7065 2028 5b6e 5f6e 6f70 732c 5d20 6e5f  pe ([n_nops,] n_
-0000d740: 6e6f 7073 2c20 642a 2a32 2c20 642a 2a32  nops, d**2, d**2
-0000d750: 290a 2020 2020 2020 2020 5468 6520 6672  ).        The fr
-0000d760: 6571 7565 6e63 7920 7368 6966 7473 2e0a  equency shifts..
-0000d770: 0a20 2020 202e 2e20 5f6e 6f74 6573 3a0a  .    .. _notes:.
-0000d780: 0a20 2020 204e 6f74 6573 0a20 2020 202d  .    Notes.    -
-0000d790: 2d2d 2d2d 0a20 2020 2054 6865 2074 6f74  ----.    The tot
-0000d7a0: 616c 2066 7265 7175 656e 6379 2073 6869  al frequency shi
-0000d7b0: 6674 7320 6172 6520 6769 7665 6e20 6279  fts are given by
-0000d7c0: 0a0a 2020 2020 2e2e 206d 6174 683a 3a0a  ..    .. math::.
-0000d7d0: 0a20 2020 2020 2020 205c 4465 6c74 615f  .        \Delta_
-0000d7e0: 7b5c 616c 7068 615c 6265 7461 2c20 6b6c  {\alpha\beta, kl
-0000d7f0: 7d20 3d20 5c69 6e74 5f7b 2d5c 696e 6674  } = \int_{-\inft
-0000d800: 797d 5e5c 696e 6674 790a 2020 2020 2020  y}^\infty.      
-0000d810: 2020 2020 2020 5c66 7261 637b 5c6d 6174        \frac{\mat
-0000d820: 6872 6d7b 647d 7b5c 6f6d 6567 617d 7d7b  hrm{d}{\omega}}{
-0000d830: 325c 7069 7d20 535f 7b5c 616c 7068 615c  2\pi} S_{\alpha\
-0000d840: 6265 7461 7d28 5c6f 6d65 6761 290a 2020  beta}(\omega).  
-0000d850: 2020 2020 2020 2020 2020 465f 7b5c 616c            F_{\al
-0000d860: 7068 615c 6265 7461 2c6b 6c7d 5e7b 2832  pha\beta,kl}^{(2
-0000d870: 297d 285c 6f6d 6567 6129 0a0a 2020 2020  )}(\omega)..    
-0000d880: 7769 7468 203a 6d61 7468 3a60 465f 7b5c  with :math:`F_{\
-0000d890: 616c 7068 615c 6265 7461 2c6b 6c7d 5e7b  alpha\beta,kl}^{
-0000d8a0: 2832 297d 285c 6f6d 6567 6129 6020 7468  (2)}(\omega)` th
-0000d8b0: 6520 7365 636f 6e64 206f 7264 6572 2066  e second order f
-0000d8c0: 696c 7465 720a 2020 2020 6675 6e63 7469  ilter.    functi
-0000d8d0: 6f6e 2e0a 0a20 2020 2053 6565 2041 6c73  on...    See Als
-0000d8e0: 6f0a 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20  o.    --------. 
-0000d8f0: 2020 2063 616c 6375 6c61 7465 5f73 6563     calculate_sec
-0000d900: 6f6e 645f 6f72 6465 725f 6669 6c74 6572  ond_order_filter
-0000d910: 5f66 756e 6374 696f 6e3a 2043 6f72 7265  _function: Corre
-0000d920: 7370 6f6e 6469 6e67 2066 696c 7465 7220  sponding filter 
-0000d930: 6675 6e63 7469 6f6e 2e0a 2020 2020 6361  function..    ca
-0000d940: 6c63 756c 6174 655f 6465 6361 795f 616d  lculate_decay_am
-0000d950: 706c 6974 7564 6573 3a20 4669 7273 7420  plitudes: First 
-0000d960: 6f72 6465 7220 2864 6973 7369 7061 7469  order (dissipati
-0000d970: 7665 2920 7465 726d 732e 0a20 2020 2069  ve) terms..    i
-0000d980: 6e66 6964 656c 6974 793a 2043 6f6d 7075  nfidelity: Compu
-0000d990: 7465 2074 6865 2069 6e66 6964 656c 6974  te the infidelit
-0000d9a0: 7920 6469 7265 6374 6c79 2e0a 2020 2020  y directly..    
-0000d9b0: 7075 6c73 655f 7365 7175 656e 6365 2e63  pulse_sequence.c
-0000d9c0: 6f6e 6361 7465 6e61 7465 3a20 436f 6e63  oncatenate: Conc
-0000d9d0: 6174 656e 6174 6520 6060 5075 6c73 6553  atenate ``PulseS
-0000d9e0: 6571 7565 6e63 6560 6020 6f62 6a65 6374  equence`` object
-0000d9f0: 732e 0a20 2020 2063 616c 6375 6c61 7465  s..    calculate
-0000da00: 5f70 756c 7365 5f63 6f72 7265 6c61 7469  _pulse_correlati
-0000da10: 6f6e 5f66 696c 7465 725f 6675 6e63 7469  on_filter_functi
-0000da20: 6f6e 0a20 2020 2022 2222 0a20 2020 2069  on.    """.    i
-0000da30: 6478 203d 2075 7469 6c2e 6765 745f 696e  dx = util.get_in
-0000da40: 6469 6365 735f 6672 6f6d 5f69 6465 6e74  dices_from_ident
-0000da50: 6966 6965 7273 2870 756c 7365 2e6e 5f6f  ifiers(pulse.n_o
-0000da60: 7065 725f 6964 656e 7469 6669 6572 732c  per_identifiers,
-0000da70: 206e 5f6f 7065 725f 6964 656e 7469 6669   n_oper_identifi
-0000da80: 6572 7329 0a20 2020 2066 696c 7465 725f  ers).    filter_
-0000da90: 6675 6e63 7469 6f6e 5f32 203d 2070 756c  function_2 = pul
-0000daa0: 7365 2e67 6574 5f66 696c 7465 725f 6675  se.get_filter_fu
-0000dab0: 6e63 7469 6f6e 286f 6d65 6761 2c20 6f72  nction(omega, or
-0000dac0: 6465 723d 322c 0a20 2020 2020 2020 2020  der=2,.         
-0000dad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000daf0: 2020 2020 2020 2020 2073 686f 775f 7072           show_pr
-0000db00: 6f67 7265 7373 6261 723d 7368 6f77 5f70  ogressbar=show_p
-0000db10: 726f 6772 6573 7362 6172 290a 2020 2020  rogressbar).    
-0000db20: 696e 7465 6772 616e 6420 3d20 5f67 6574  integrand = _get
-0000db30: 5f69 6e74 6567 7261 6e64 2873 7065 6374  _integrand(spect
-0000db40: 7275 6d2c 206f 6d65 6761 2c20 6964 782c  rum, omega, idx,
-0000db50: 2077 6869 6368 5f70 756c 7365 3d27 746f   which_pulse='to
-0000db60: 7461 6c27 2c20 7768 6963 685f 4646 3d27  tal', which_FF='
-0000db70: 6765 6e65 7261 6c69 7a65 6427 2c0a 2020  generalized',.  
-0000db80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db90: 2020 2020 2020 2020 2020 2020 2066 696c               fil
-0000dba0: 7465 725f 6675 6e63 7469 6f6e 3d66 696c  ter_function=fil
-0000dbb0: 7465 725f 6675 6e63 7469 6f6e 5f32 290a  ter_function_2).
-0000dbc0: 2020 2020 6672 6571 7565 6e63 795f 7368      frequency_sh
-0000dbd0: 6966 7473 203d 2075 7469 6c2e 696e 7465  ifts = util.inte
-0000dbe0: 6772 6174 6528 696e 7465 6772 616e 642c  grate(integrand,
-0000dbf0: 206f 6d65 6761 292f 2832 2a6e 702e 7069   omega)/(2*np.pi
-0000dc00: 290a 2020 2020 7265 7475 726e 2066 7265  ).    return fre
-0000dc10: 7175 656e 6379 5f73 6869 6674 730a 0a0a  quency_shifts...
-0000dc20: 4075 7469 6c2e 7061 7273 655f 6f70 7469  @util.parse_opti
-0000dc30: 6f6e 616c 5f70 6172 616d 6574 6572 7328  onal_parameters(
-0000dc40: 7768 6963 683d 2827 6669 6465 6c69 7479  which=('fidelity
-0000dc50: 272c 2027 6765 6e65 7261 6c69 7a65 6427  ', 'generalized'
-0000dc60: 2929 0a64 6566 2063 616c 6375 6c61 7465  )).def calculate
-0000dc70: 5f66 696c 7465 725f 6675 6e63 7469 6f6e  _filter_function
-0000dc80: 2863 6f6e 7472 6f6c 5f6d 6174 7269 783a  (control_matrix:
-0000dc90: 206e 6461 7272 6179 2c20 7768 6963 683a   ndarray, which:
-0000dca0: 2073 7472 203d 2027 6669 6465 6c69 7479   str = 'fidelity
-0000dcb0: 2729 202d 3e20 6e64 6172 7261 793a 0a20  ') -> ndarray:. 
-0000dcc0: 2020 2072 2222 2243 6f6d 7075 7465 2074     r"""Compute t
-0000dcd0: 6865 2066 696c 7465 7220 6675 6e63 7469  he filter functi
-0000dce0: 6f6e 2066 726f 6d20 7468 6520 636f 6e74  on from the cont
-0000dcf0: 726f 6c20 6d61 7472 6978 2e0a 0a20 2020  rol matrix...   
-0000dd00: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-0000dd10: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2063  ----------.    c
-0000dd20: 6f6e 7472 6f6c 5f6d 6174 7269 783a 2061  ontrol_matrix: a
-0000dd30: 7272 6179 5f6c 696b 652c 2073 6861 7065  rray_like, shape
-0000dd40: 2028 6e5f 6e6f 7073 2c20 642a 2a32 2c20   (n_nops, d**2, 
-0000dd50: 6e5f 6f6d 6567 6129 0a20 2020 2020 2020  n_omega).       
-0000dd60: 2054 6865 2063 6f6e 7472 6f6c 206d 6174   The control mat
-0000dd70: 7269 782e 0a20 2020 2077 6869 6368 203a  rix..    which :
-0000dd80: 2073 7472 2c20 6f70 7469 6f6e 616c 0a20   str, optional. 
-0000dd90: 2020 2020 2020 2057 6869 6368 2066 696c         Which fil
-0000dda0: 7465 7220 6675 6e63 7469 6f6e 2074 6f20  ter function to 
-0000ddb0: 7265 7475 726e 2e20 4569 7468 6572 2027  return. Either '
-0000ddc0: 6669 6465 6c69 7479 2720 2864 6566 6175  fidelity' (defau
-0000ddd0: 6c74 2920 6f72 0a20 2020 2020 2020 2027  lt) or.        '
-0000dde0: 6765 6e65 7261 6c69 7a65 6427 2028 7365  generalized' (se
-0000ddf0: 6520 3a72 6566 3a60 4e6f 7465 7320 3c6e  e :ref:`Notes <n
-0000de00: 6f74 6573 3e60 292e 0a0a 2020 2020 5265  otes>`)...    Re
-0000de10: 7475 726e 730a 2020 2020 2d2d 2d2d 2d2d  turns.    ------
-0000de20: 2d0a 2020 2020 6669 6c74 6572 5f66 756e  -.    filter_fun
-0000de30: 6374 696f 6e3a 206e 6461 7272 6179 2c20  ction: ndarray, 
-0000de40: 7368 6170 6520 286e 5f6e 6f70 732c 206e  shape (n_nops, n
-0000de50: 5f6e 6f70 732c 205b 642a 2a32 2c20 642a  _nops, [d**2, d*
-0000de60: 2a32 2c5d 206e 5f6f 6d65 6761 290a 2020  *2,] n_omega).  
-0000de70: 2020 2020 2020 5468 6520 6669 6c74 6572        The filter
-0000de80: 2066 756e 6374 696f 6e73 2066 6f72 2065   functions for e
-0000de90: 6163 6820 6e6f 6973 6520 6f70 6572 6174  ach noise operat
-0000dea0: 6f72 2063 6f72 7265 6c61 7469 6f6e 2e20  or correlation. 
-0000deb0: 5468 650a 2020 2020 2020 2020 6469 6167  The.        diag
-0000dec0: 6f6e 616c 2063 6f72 7265 7370 6f6e 6473  onal corresponds
-0000ded0: 2074 6f20 7468 6520 6669 6c74 6572 2066   to the filter f
-0000dee0: 756e 6374 696f 6e73 2066 6f72 2075 6e63  unctions for unc
-0000def0: 6f72 7265 6c61 7465 640a 2020 2020 2020  orrelated.      
-0000df00: 2020 6e6f 6973 6520 736f 7572 6365 732e    noise sources.
-0000df10: 0a0a 2020 2020 2e2e 205f 6e6f 7465 733a  ..    .. _notes:
-0000df20: 0a0a 2020 2020 4e6f 7465 730a 2020 2020  ..    Notes.    
-0000df30: 2d2d 2d2d 2d0a 2020 2020 5468 6520 6765  -----.    The ge
-0000df40: 6e65 7261 6c69 7a65 6420 6669 6c74 6572  neralized filter
-0000df50: 2066 756e 6374 696f 6e20 6973 2067 6976   function is giv
-0000df60: 656e 2062 790a 0a20 2020 202e 2e20 6d61  en by..    .. ma
-0000df70: 7468 3a3a 0a0a 2020 2020 2020 2020 465f  th::..        F_
-0000df80: 7b5c 616c 7068 615c 6265 7461 2c6b 6c7d  {\alpha\beta,kl}
-0000df90: 285c 6f6d 6567 6129 203d 0a20 2020 2020  (\omega) =.     
-0000dfa0: 2020 2020 2020 205c 7469 6c64 657b 5c6d         \tilde{\m
-0000dfb0: 6174 6863 616c 7b42 7d7d 5f7b 5c61 6c70  athcal{B}}_{\alp
-0000dfc0: 6861 206b 7d5e 5c61 7374 285c 6f6d 6567  ha k}^\ast(\omeg
-0000dfd0: 6129 0a20 2020 2020 2020 2020 2020 205c  a).            \
-0000dfe0: 7469 6c64 657b 5c6d 6174 6863 616c 7b42  tilde{\mathcal{B
-0000dff0: 7d7d 5f7b 5c62 6574 6120 6c7d 285c 6f6d  }}_{\beta l}(\om
-0000e000: 6567 6129 2c0a 0a20 2020 2077 6865 7265  ega),..    where
-0000e010: 203a 6d61 7468 3a60 5c61 6c70 6861 2c5c   :math:`\alpha,\
-0000e020: 6265 7461 6020 6172 6520 696e 6469 6365  beta` are indice
-0000e030: 7320 636f 756e 7469 6e67 2074 6865 206e  s counting the n
-0000e040: 6f69 7365 206f 7065 7261 746f 7273 0a20  oise operators. 
-0000e050: 2020 203a 6d61 7468 3a60 425f 5c61 6c70     :math:`B_\alp
-0000e060: 6861 6020 616e 6420 3a6d 6174 683a 606b  ha` and :math:`k
-0000e070: 2c6c 6020 696e 6469 6365 7320 636f 756e  ,l` indices coun
-0000e080: 7469 6e67 2074 6865 2062 6173 6973 2065  ting the basis e
-0000e090: 6c65 6d65 6e74 730a 2020 2020 3a6d 6174  lements.    :mat
-0000e0a0: 683a 6043 5f6b 602e 0a0a 2020 2020 5468  h:`C_k`...    Th
-0000e0b0: 6520 6669 6465 6c69 7479 2066 696c 7465  e fidelity filte
-0000e0c0: 7220 6675 6e63 7469 6f6e 2069 7320 6f62  r function is ob
-0000e0d0: 7461 696e 6564 2062 7920 7472 6163 696e  tained by tracin
-0000e0e0: 6720 6f76 6572 2074 6865 2062 6173 6973  g over the basis
-0000e0f0: 0a20 2020 2069 6e64 6963 6573 3a0a 0a20  .    indices:.. 
-0000e100: 2020 202e 2e20 6d61 7468 3a3a 0a0a 2020     .. math::..  
-0000e110: 2020 2020 2020 465f 7b5c 616c 7068 615c        F_{\alpha\
-0000e120: 6265 7461 7d28 5c6f 6d65 6761 2920 3d20  beta}(\omega) = 
-0000e130: 5c73 756d 5f7b 6b7d 2046 5f7b 5c61 6c70  \sum_{k} F_{\alp
-0000e140: 6861 5c62 6574 612c 6b6b 7d28 5c6f 6d65  ha\beta,kk}(\ome
-0000e150: 6761 292e 0a0a 2020 2020 5365 6520 416c  ga)...    See Al
-0000e160: 736f 0a20 2020 202d 2d2d 2d2d 2d2d 2d0a  so.    --------.
-0000e170: 2020 2020 6361 6c63 756c 6174 655f 636f      calculate_co
-0000e180: 6e74 726f 6c5f 6d61 7472 6978 5f66 726f  ntrol_matrix_fro
-0000e190: 6d5f 7363 7261 7463 683a 2043 6f6e 7472  m_scratch: Contr
-0000e1a0: 6f6c 206d 6174 7269 7820 6672 6f6d 2073  ol matrix from s
-0000e1b0: 6372 6174 6368 2e0a 2020 2020 6361 6c63  cratch..    calc
-0000e1c0: 756c 6174 655f 636f 6e74 726f 6c5f 6d61  ulate_control_ma
-0000e1d0: 7472 6978 5f66 726f 6d5f 6174 6f6d 6963  trix_from_atomic
-0000e1e0: 3a20 436f 6e74 726f 6c20 6d61 7472 6978  : Control matrix
-0000e1f0: 2066 726f 6d20 636f 6e63 6174 656e 6174   from concatenat
-0000e200: 696f 6e2e 0a20 2020 2063 616c 6375 6c61  ion..    calcula
-0000e210: 7465 5f70 756c 7365 5f63 6f72 7265 6c61  te_pulse_correla
-0000e220: 7469 6f6e 5f66 696c 7465 725f 6675 6e63  tion_filter_func
-0000e230: 7469 6f6e 3a20 5075 6c73 6520 636f 7272  tion: Pulse corr
-0000e240: 656c 6174 696f 6e73 2e0a 2020 2020 2222  elations..    ""
-0000e250: 220a 2020 2020 6966 2077 6869 6368 203d  ".    if which =
-0000e260: 3d20 2766 6964 656c 6974 7927 3a0a 2020  = 'fidelity':.  
-0000e270: 2020 2020 2020 7375 6273 6372 6970 7473        subscripts
-0000e280: 203d 2027 616b 6f2c 626b 6f2d 3e61 626f   = 'ako,bko->abo
-0000e290: 270a 2020 2020 656c 7365 3a0a 2020 2020  '.    else:.    
-0000e2a0: 2020 2020 2320 7768 6963 6820 3d3d 2027      # which == '
-0000e2b0: 6765 6e65 7261 6c69 7a65 6427 0a20 2020  generalized'.   
-0000e2c0: 2020 2020 2073 7562 7363 7269 7074 7320       subscripts 
-0000e2d0: 3d20 2761 6b6f 2c62 6c6f 2d3e 6162 6b6c  = 'ako,blo->abkl
-0000e2e0: 6f27 0a0a 2020 2020 7265 7475 726e 206e  o'..    return n
-0000e2f0: 702e 6569 6e73 756d 2873 7562 7363 7269  p.einsum(subscri
-0000e300: 7074 732c 2063 6f6e 7472 6f6c 5f6d 6174  pts, control_mat
-0000e310: 7269 782e 636f 6e6a 2829 2c20 636f 6e74  rix.conj(), cont
-0000e320: 726f 6c5f 6d61 7472 6978 290a 0a0a 6465  rol_matrix)...de
-0000e330: 6620 6361 6c63 756c 6174 655f 7365 636f  f calculate_seco
-0000e340: 6e64 5f6f 7264 6572 5f66 696c 7465 725f  nd_order_filter_
-0000e350: 6675 6e63 7469 6f6e 280a 2020 2020 2020  function(.      
-0000e360: 2020 6569 6776 616c 733a 206e 6461 7272    eigvals: ndarr
-0000e370: 6179 2c0a 2020 2020 2020 2020 6569 6776  ay,.        eigv
-0000e380: 6563 733a 206e 6461 7272 6179 2c0a 2020  ecs: ndarray,.  
-0000e390: 2020 2020 2020 7072 6f70 6167 6174 6f72        propagator
-0000e3a0: 733a 206e 6461 7272 6179 2c0a 2020 2020  s: ndarray,.    
-0000e3b0: 2020 2020 6f6d 6567 613a 2043 6f65 6666      omega: Coeff
-0000e3c0: 6963 6965 6e74 732c 0a20 2020 2020 2020  icients,.       
-0000e3d0: 2062 6173 6973 3a20 4261 7369 732c 0a20   basis: Basis,. 
-0000e3e0: 2020 2020 2020 206e 5f6f 7065 7273 3a20         n_opers: 
-0000e3f0: 5365 7175 656e 6365 5b4f 7065 7261 746f  Sequence[Operato
-0000e400: 725d 2c0a 2020 2020 2020 2020 6e5f 636f  r],.        n_co
-0000e410: 6566 6673 3a20 5365 7175 656e 6365 5b43  effs: Sequence[C
-0000e420: 6f65 6666 6963 6965 6e74 735d 2c0a 2020  oefficients],.  
-0000e430: 2020 2020 2020 6474 3a20 436f 6566 6669        dt: Coeffi
-0000e440: 6369 656e 7473 2c0a 2020 2020 2020 2020  cients,.        
-0000e450: 696e 7465 726d 6564 6961 7465 733a 204f  intermediates: O
-0000e460: 7074 696f 6e61 6c5b 4469 6374 5b73 7472  ptional[Dict[str
-0000e470: 2c20 6e64 6172 7261 795d 5d20 3d20 4e6f  , ndarray]] = No
-0000e480: 6e65 2c0a 2020 2020 2020 2020 7368 6f77  ne,.        show
-0000e490: 5f70 726f 6772 6573 7362 6172 3a20 626f  _progressbar: bo
-0000e4a0: 6f6c 203d 2046 616c 7365 0a29 202d 3e20  ol = False.) -> 
-0000e4b0: 6e64 6172 7261 793a 0a20 2020 2072 2222  ndarray:.    r""
-0000e4c0: 2243 616c 6375 6c61 7465 2074 6865 2073  "Calculate the s
-0000e4d0: 6563 6f6e 6420 6f72 6465 7220 6669 6c74  econd order filt
-0000e4e0: 6572 2066 756e 6374 696f 6e20 666f 7220  er function for 
-0000e4f0: 6672 6571 7565 6e63 7920 7368 6966 7473  frequency shifts
-0000e500: 2e0a 0a20 2020 2050 6172 616d 6574 6572  ...    Parameter
-0000e510: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  s.    ----------
-0000e520: 0a20 2020 2065 6967 7661 6c73 3a20 6172  .    eigvals: ar
-0000e530: 7261 795f 6c69 6b65 2c20 7368 6170 6520  ray_like, shape 
-0000e540: 286e 5f64 742c 2064 290a 2020 2020 2020  (n_dt, d).      
-0000e550: 2020 4569 6765 6e76 616c 7565 2076 6563    Eigenvalue vec
-0000e560: 746f 7273 2066 6f72 2065 6163 6820 7469  tors for each ti
-0000e570: 6d65 2070 756c 7365 2073 6567 6d65 6e74  me pulse segment
-0000e580: 202a 6c2a 2077 6974 6820 7468 650a 2020   *l* with the.  
-0000e590: 2020 2020 2020 6669 7273 7420 6178 6973        first axis
-0000e5a0: 2063 6f75 6e74 696e 6720 7468 6520 7075   counting the pu
-0000e5b0: 6c73 6520 7365 676d 656e 742c 2069 2e65  lse segment, i.e
-0000e5c0: 2e0a 2020 2020 2020 2020 6060 6569 6776  ..        ``eigv
-0000e5d0: 616c 7320 3d3d 2061 7272 6179 285b 445f  als == array([D_
-0000e5e0: 302c 2044 5f31 2c20 2e2e 2e5d 2960 602e  0, D_1, ...])``.
-0000e5f0: 0a20 2020 2065 6967 7665 6373 3a20 6172  .    eigvecs: ar
-0000e600: 7261 795f 6c69 6b65 2c20 7368 6170 6520  ray_like, shape 
-0000e610: 286e 5f64 742c 2064 2c20 6429 0a20 2020  (n_dt, d, d).   
-0000e620: 2020 2020 2045 6967 656e 7665 6374 6f72       Eigenvector
-0000e630: 206d 6174 7269 6365 7320 666f 7220 6561   matrices for ea
-0000e640: 6368 2074 696d 6520 7075 6c73 6520 7365  ch time pulse se
-0000e650: 676d 656e 7420 2a6c 2a20 7769 7468 2074  gment *l* with t
-0000e660: 6865 0a20 2020 2020 2020 2066 6972 7374  he.        first
-0000e670: 2061 7869 7320 636f 756e 7469 6e67 2074   axis counting t
-0000e680: 6865 2070 756c 7365 2073 6567 6d65 6e74  he pulse segment
-0000e690: 2c20 692e 652e 0a20 2020 2020 2020 2060  , i.e..        `
-0000e6a0: 6065 6967 7665 6373 203d 3d20 6172 7261  `eigvecs == arra
-0000e6b0: 7928 5b56 5f30 2c20 565f 312c 202e 2e2e  y([V_0, V_1, ...
-0000e6c0: 5d29 6060 2e0a 2020 2020 7072 6f70 6167  ])``..    propag
-0000e6d0: 6174 6f72 733a 2061 7272 6179 5f6c 696b  ators: array_lik
-0000e6e0: 652c 2073 6861 7065 2028 6e5f 6474 2b31  e, shape (n_dt+1
-0000e6f0: 2c20 642c 2064 290a 2020 2020 2020 2020  , d, d).        
-0000e700: 5468 6520 7072 6f70 6167 6174 6f72 7320  The propagators 
-0000e710: 3a6d 6174 683a 6051 5f6c 203d 2050 5f6c  :math:`Q_l = P_l
-0000e720: 2050 5f7b 6c2d 317d 5c63 646f 7473 2050   P_{l-1}\cdots P
-0000e730: 5f30 6020 6173 2061 2028 642c 2064 290a  _0` as a (d, d).
-0000e740: 2020 2020 2020 2020 6172 7261 7920 7769          array wi
-0000e750: 7468 202a 642a 2074 6865 2064 696d 656e  th *d* the dimen
-0000e760: 7369 6f6e 206f 6620 7468 6520 4869 6c62  sion of the Hilb
-0000e770: 6572 7420 7370 6163 652e 0a20 2020 206f  ert space..    o
-0000e780: 6d65 6761 3a20 6172 7261 795f 6c69 6b65  mega: array_like
-0000e790: 2c20 7368 6170 6520 286e 5f6f 6d65 6761  , shape (n_omega
-0000e7a0: 2c29 0a20 2020 2020 2020 2046 7265 7175  ,).        Frequ
-0000e7b0: 656e 6369 6573 2061 7420 7768 6963 6820  encies at which 
-0000e7c0: 7468 6520 7075 6c73 6520 636f 6e74 726f  the pulse contro
-0000e7d0: 6c20 6d61 7472 6978 2069 7320 746f 2062  l matrix is to b
-0000e7e0: 650a 2020 2020 2020 2020 6576 616c 7561  e.        evalua
-0000e7f0: 7465 642e 0a20 2020 2062 6173 6973 3a20  ted..    basis: 
-0000e800: 4261 7369 732c 2073 6861 7065 2028 642a  Basis, shape (d*
-0000e810: 2a32 2c20 642c 2064 290a 2020 2020 2020  *2, d, d).      
-0000e820: 2020 5468 6520 6261 7369 7320 656c 656d    The basis elem
-0000e830: 656e 7473 2069 6e20 7768 6963 6820 7468  ents in which th
-0000e840: 6520 7075 6c73 6520 636f 6e74 726f 6c20  e pulse control 
-0000e850: 6d61 7472 6978 2077 696c 6c20 6265 0a20  matrix will be. 
-0000e860: 2020 2020 2020 2065 7870 616e 6465 642e         expanded.
-0000e870: 0a20 2020 206e 5f6f 7065 7273 3a20 6172  .    n_opers: ar
-0000e880: 7261 795f 6c69 6b65 2c20 7368 6170 6520  ray_like, shape 
-0000e890: 286e 5f6e 6f70 732c 2064 2c20 6429 0a20  (n_nops, d, d). 
-0000e8a0: 2020 2020 2020 204e 6f69 7365 206f 7065         Noise ope
-0000e8b0: 7261 746f 7273 203a 6d61 7468 3a60 425f  rators :math:`B_
-0000e8c0: 5c61 6c70 6861 602e 0a20 2020 206e 5f63  \alpha`..    n_c
-0000e8d0: 6f65 6666 733a 2061 7272 6179 5f6c 696b  oeffs: array_lik
-0000e8e0: 652c 2073 6861 7065 2028 6e5f 6e6f 7073  e, shape (n_nops
-0000e8f0: 2c20 6e5f 6474 290a 2020 2020 2020 2020  , n_dt).        
-0000e900: 5468 6520 7365 6e73 6974 6976 6974 6965  The sensitivitie
-0000e910: 7320 6f66 2074 6865 2073 7973 7465 6d20  s of the system 
-0000e920: 746f 2074 6865 206e 6f69 7365 206f 7065  to the noise ope
-0000e930: 7261 746f 7273 2067 6976 656e 2062 790a  rators given by.
-0000e940: 2020 2020 2020 2020 2a6e 5f6f 7065 7273          *n_opers
-0000e950: 2a20 6174 2074 6865 2067 6976 656e 2074  * at the given t
-0000e960: 696d 6520 7374 6570 2e0a 2020 2020 6474  ime step..    dt
-0000e970: 3a20 6172 7261 795f 6c69 6b65 2c20 7368  : array_like, sh
-0000e980: 6170 6520 286e 5f64 7429 0a20 2020 2020  ape (n_dt).     
-0000e990: 2020 2053 6571 7565 6e63 6520 6475 7261     Sequence dura
-0000e9a0: 7469 6f6e 2c20 692e 652e 2066 6f72 2074  tion, i.e. for t
-0000e9b0: 6865 203a 6d61 7468 3a60 6c60 2d74 6820  he :math:`l`-th 
-0000e9c0: 7075 6c73 650a 2020 2020 2020 2020 3a6d  pulse.        :m
-0000e9d0: 6174 683a 6074 5f6c 202d 2074 5f7b 6c2d  ath:`t_l - t_{l-
-0000e9e0: 317d 602e 0a20 2020 2069 6e74 6572 6d65  1}`..    interme
-0000e9f0: 6469 6174 6573 3a20 4469 6374 5b73 7472  diates: Dict[str
-0000ea00: 2c20 6e64 6172 7261 795d 2c20 6f70 7469  , ndarray], opti
-0000ea10: 6f6e 616c 0a20 2020 2020 2020 2049 6e74  onal.        Int
-0000ea20: 6572 6d65 6469 6174 6520 7465 726d 7320  ermediate terms 
-0000ea30: 6f66 2074 6865 2063 616c 6375 6c61 7469  of the calculati
-0000ea40: 6f6e 206f 6620 7468 6520 636f 6e74 726f  on of the contro
-0000ea50: 6c20 6d61 7472 6978 2074 6861 740a 2020  l matrix that.  
-0000ea60: 2020 2020 2020 6361 6e20 6265 2072 6575        can be reu
-0000ea70: 7365 6420 6865 7265 2e20 4966 204e 6f6e  sed here. If Non
-0000ea80: 6520 2864 6566 6175 6c74 292c 2074 6865  e (default), the
-0000ea90: 7920 6172 6520 636f 6d70 7574 6564 2066  y are computed f
-0000eaa0: 726f 6d0a 2020 2020 2020 2020 7363 7261  rom.        scra
-0000eab0: 7463 682e 0a20 2020 2073 686f 775f 7072  tch..    show_pr
-0000eac0: 6f67 7265 7373 6261 723a 2062 6f6f 6c2c  ogressbar: bool,
-0000ead0: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
-0000eae0: 2020 5368 6f77 2061 2070 726f 6772 6573    Show a progres
-0000eaf0: 7320 6261 7220 666f 7220 7468 6520 6361  s bar for the ca
-0000eb00: 6c63 756c 6174 696f 6e2e 0a0a 2020 2020  lculation...    
-0000eb10: 5265 7475 726e 730a 2020 2020 2d2d 2d2d  Returns.    ----
-0000eb20: 2d2d 2d0a 2020 2020 7365 636f 6e64 5f6f  ---.    second_o
-0000eb30: 7264 6572 5f66 696c 7465 725f 6675 6e63  rder_filter_func
-0000eb40: 7469 6f6e 3a20 6e64 6172 7261 792c 2073  tion: ndarray, s
-0000eb50: 6861 7065 2028 6e5f 6e6f 7073 2c20 6e5f  hape (n_nops, n_
-0000eb60: 6e6f 7073 2c20 642a 2a32 2c20 642a 2a32  nops, d**2, d**2
-0000eb70: 2c20 6e5f 6f6d 6567 6129 0a20 2020 2020  , n_omega).     
-0000eb80: 2020 2054 6865 2073 6563 6f6e 6420 6f72     The second or
-0000eb90: 6465 7220 6669 6c74 6572 2066 756e 6374  der filter funct
-0000eba0: 696f 6e2e 0a0a 2020 2020 2e2e 205f 6e6f  ion...    .. _no
-0000ebb0: 7465 733a 0a0a 2020 2020 4e6f 7465 730a  tes:..    Notes.
-0000ebc0: 2020 2020 2d2d 2d2d 2d0a 2020 2020 5468      -----.    Th
-0000ebd0: 6520 7365 636f 6e64 206f 7264 6572 2066  e second order f
-0000ebe0: 696c 7465 7220 6675 6e63 7469 6f6e 2069  ilter function i
-0000ebf0: 7320 6769 7665 6e20 6279 0a0a 2020 2020  s given by..    
-0000ec00: 2e2e 206d 6174 683a 3a0a 0a20 2020 2020  .. math::..     
-0000ec10: 2020 2046 5f7b 5c61 6c70 6861 5c62 6574     F_{\alpha\bet
-0000ec20: 612c 206b 6c7d 5e7b 2832 297d 203d 205c  a, kl}^{(2)} = \
-0000ec30: 7375 6d5f 7b67 3d31 7d5e 475c 6c65 6674  sum_{g=1}^G\left
-0000ec40: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
-0000ec50: 2020 5c6d 6174 6863 616c 7b47 7d5f 7b5c    \mathcal{G}_{\
-0000ec60: 616c 7068 6120 6b7d 5e7b 2867 295c 6173  alpha k}^{(g)\as
-0000ec70: 747d 285c 6f6d 6567 6129 0a20 2020 2020  t}(\omega).     
-0000ec80: 2020 2020 2020 2020 2020 205c 7375 6d5f             \sum_
-0000ec90: 7b67 273d 317d 5e7b 672d 317d 5c6d 6174  {g'=1}^{g-1}\mat
-0000eca0: 6863 616c 7b47 7d5f 7b5c 6265 7461 206c  hcal{G}_{\beta l
-0000ecb0: 7d5e 7b28 6727 297d 285c 6f6d 6567 6129  }^{(g')}(\omega)
-0000ecc0: 202b 0a20 2020 2020 2020 2020 2020 2020   +.             
-0000ecd0: 2020 2073 5f5c 616c 7068 615e 7b28 6729     s_\alpha^{(g)
-0000ece0: 7d5c 6261 727b 427d 5f7b 5c61 6c70 6861  }\bar{B}_{\alpha
-0000ecf0: 2c69 6a7d 5e7b 2867 297d 5c62 6172 7b43  ,ij}^{(g)}\bar{C
-0000ed00: 7d5f 7b6b 2c6a 697d 5e7b 2867 297d 0a20  }_{k,ji}^{(g)}. 
-0000ed10: 2020 2020 2020 2020 2020 2020 2020 2049                 I
-0000ed20: 5f7b 696a 6d6e 7d5e 7b28 6729 7d28 5c6f  _{ijmn}^{(g)}(\o
-0000ed30: 6d65 6761 295c 6261 727b 437d 5f7b 6c2c  mega)\bar{C}_{l,
-0000ed40: 6e6d 7d5e 7b28 6729 0a20 2020 2020 2020  nm}^{(g).       
-0000ed50: 2020 2020 2020 2020 205c 6261 727b 427d           \bar{B}
-0000ed60: 5f7b 5c62 6574 612c 6d6e 7d5e 7b28 6729  _{\beta,mn}^{(g)
-0000ed70: 7d73 5f5c 6265 7461 5e7b 2867 297d 7d0a  }s_\beta^{(g)}}.
-0000ed80: 2020 2020 2020 2020 2020 2020 5c72 6967              \rig
-0000ed90: 6874 5d0a 0a20 2020 2077 6974 680a 0a20  ht]..    with.. 
-0000eda0: 2020 202e 2e20 6d61 7468 3a3a 0a0a 2020     .. math::..  
-0000edb0: 2020 2020 2020 5c6d 6174 6863 616c 7b47        \mathcal{G
-0000edc0: 7d5e 7b28 6729 7d28 5c6f 6d65 6761 2920  }^{(g)}(\omega) 
-0000edd0: 263d 0a20 2020 2020 2020 2020 2020 2065  &=.            e
-0000ede0: 5e7b 695c 6f6d 6567 6120 745f 7b67 2d31  ^{i\omega t_{g-1
-0000edf0: 7d7d 5c6d 6174 6863 616c 7b42 7d5e 7b28  }}\mathcal{B}^{(
-0000ee00: 6729 7d28 5c6f 6d65 6761 290a 2020 2020  g)}(\omega).    
-0000ee10: 2020 2020 2020 2020 5c6d 6174 6863 616c          \mathcal
-0000ee20: 7b51 7d5e 7b28 672d 3129 7d2c 205c 5c0a  {Q}^{(g-1)}, \\.
-0000ee30: 2020 2020 2020 2020 495f 7b69 6a6d 6e7d          I_{ijmn}
-0000ee40: 5e7b 2867 297d 285c 6f6d 6567 6129 2026  ^{(g)}(\omega) &
-0000ee50: 3d0a 2020 2020 2020 2020 2020 2020 5c69  =.            \i
-0000ee60: 6e74 5f7b 745f 7b67 2d31 7d7d 5e7b 745f  nt_{t_{g-1}}^{t_
-0000ee70: 677d 5c6d 6174 6872 6d7b 647d 7b74 7d0a  g}\mathrm{d}{t}.
-0000ee80: 2020 2020 2020 2020 2020 2020 655e 7b69              e^{i
-0000ee90: 5c4f 6d65 6761 5f7b 696a 7d5e 7b28 6729  \Omega_{ij}^{(g)
-0000eea0: 7d28 7420 2d20 745f 7b67 2d31 7d29 202d  }(t - t_{g-1}) -
-0000eeb0: 2069 5c6f 6d65 6761 2074 7d0a 2020 2020   i\omega t}.    
-0000eec0: 2020 2020 2020 2020 5c69 6e74 5f7b 745f          \int_{t_
-0000eed0: 7b67 2d31 7d7d 5e7b 747d 5c6d 6174 6872  {g-1}}^{t}\mathr
-0000eee0: 6d7b 647d 7b74 277d 0a20 2020 2020 2020  m{d}{t'}.       
-0000eef0: 2020 2020 2065 5e7b 695c 4f6d 6567 615f       e^{i\Omega_
-0000ef00: 7b6d 6e7d 5e7b 2867 297d 2874 2720 2d20  {mn}^{(g)}(t' - 
-0000ef10: 745f 7b67 2d31 7d29 202b 2069 5c6f 6d65  t_{g-1}) + i\ome
-0000ef20: 6761 2074 277d 2e0a 0a20 2020 2053 6565  ga t'}...    See
-0000ef30: 2041 6c73 6f0a 2020 2020 2d2d 2d2d 2d2d   Also.    ------
-0000ef40: 2d2d 0a20 2020 2063 616c 6375 6c61 7465  --.    calculate
-0000ef50: 5f66 7265 7175 656e 6379 5f73 6869 6674  _frequency_shift
-0000ef60: 733a 2049 6e74 6567 7261 7465 206f 7665  s: Integrate ove
-0000ef70: 7220 6669 6c74 6572 2066 756e 6374 696f  r filter functio
-0000ef80: 6e20 7469 6d65 7320 7370 6563 7472 756d  n times spectrum
-0000ef90: 2e0a 2020 2020 6361 6c63 756c 6174 655f  ..    calculate_
-0000efa0: 6465 6361 795f 616d 706c 6974 7564 6573  decay_amplitudes
-0000efb0: 3a20 4669 7273 7420 6f72 6465 7220 2864  : First order (d
-0000efc0: 6973 7369 7061 7469 7665 2920 7465 726d  issipative) term
-0000efd0: 732e 0a20 2020 2069 6e66 6964 656c 6974  s..    infidelit
-0000efe0: 793a 2043 6f6d 7075 7465 2074 6865 2069  y: Compute the i
-0000eff0: 6e66 6964 656c 6974 7920 6469 7265 6374  nfidelity direct
-0000f000: 6c79 2e0a 2020 2020 7075 6c73 655f 7365  ly..    pulse_se
-0000f010: 7175 656e 6365 2e63 6f6e 6361 7465 6e61  quence.concatena
-0000f020: 7465 3a20 436f 6e63 6174 656e 6174 6520  te: Concatenate 
-0000f030: 6060 5075 6c73 6553 6571 7565 6e63 6560  ``PulseSequence`
-0000f040: 6020 6f62 6a65 6374 732e 0a20 2020 2063  ` objects..    c
-0000f050: 616c 6375 6c61 7465 5f70 756c 7365 5f63  alculate_pulse_c
-0000f060: 6f72 7265 6c61 7469 6f6e 5f66 696c 7465  orrelation_filte
-0000f070: 725f 6675 6e63 7469 6f6e 0a20 2020 2022  r_function.    "
-0000f080: 2222 0a20 2020 2064 203d 2065 6967 7661  "".    d = eigva
-0000f090: 6c73 2e73 6861 7065 5b2d 315d 0a20 2020  ls.shape[-1].   
-0000f0a0: 2023 2057 6527 7265 206c 617a 790a 2020   # We're lazy.  
-0000f0b0: 2020 6e5f 636f 6566 6673 203d 206e 702e    n_coeffs = np.
-0000f0c0: 6173 6172 7261 7928 6e5f 636f 6566 6673  asarray(n_coeffs
-0000f0d0: 290a 0a20 2020 2023 2041 6c6c 6f63 6174  )..    # Allocat
-0000f0e0: 6520 7265 7375 6c74 2061 6e64 2062 7566  e result and buf
-0000f0f0: 6665 7273 2066 6f72 2069 6e74 6572 6d65  fers for interme
-0000f100: 6469 6174 6520 6172 7261 7973 0a20 2020  diate arrays.   
-0000f110: 2064 455f 6275 6673 203d 2028 6e70 2e65   dE_bufs = (np.e
-0000f120: 6d70 7479 2828 642c 2064 2c20 642c 2064  mpty((d, d, d, d
-0000f130: 292c 2064 7479 7065 3d66 6c6f 6174 292c  ), dtype=float),
-0000f140: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f150: 6e70 2e65 6d70 7479 2828 6c65 6e28 6f6d  np.empty((len(om
-0000f160: 6567 6129 2c20 642c 2064 292c 2064 7479  ega), d, d), dty
-0000f170: 7065 3d66 6c6f 6174 292c 0a20 2020 2020  pe=float),.     
-0000f180: 2020 2020 2020 2020 2020 6e70 2e65 6d70            np.emp
-0000f190: 7479 2828 6c65 6e28 6f6d 6567 6129 2c20  ty((len(omega), 
-0000f1a0: 642c 2064 292c 2064 7479 7065 3d66 6c6f  d, d), dtype=flo
-0000f1b0: 6174 2929 0a20 2020 2065 7870 5f62 7566  at)).    exp_buf
-0000f1c0: 203d 206e 702e 656d 7074 7928 286c 656e   = np.empty((len
-0000f1d0: 286f 6d65 6761 292c 2064 2c20 6429 2c20  (omega), d, d), 
-0000f1e0: 6474 7970 653d 636f 6d70 6c65 7829 0a20  dtype=complex). 
-0000f1f0: 2020 2066 7263 5f62 7566 7320 3d20 286e     frc_bufs = (n
-0000f200: 702e 656d 7074 7928 286c 656e 286f 6d65  p.empty((len(ome
-0000f210: 6761 292c 2064 2c20 6429 2c20 6474 7970  ga), d, d), dtyp
-0000f220: 653d 636f 6d70 6c65 7829 2c0a 2020 2020  e=complex),.    
-0000f230: 2020 2020 2020 2020 2020 2020 6e70 2e65              np.e
-0000f240: 6d70 7479 2828 642c 2064 2c20 642c 2064  mpty((d, d, d, d
-0000f250: 292c 2064 7479 7065 3d63 6f6d 706c 6578  ), dtype=complex
-0000f260: 2929 0a20 2020 2069 6e74 5f62 7566 203d  )).    int_buf =
-0000f270: 206e 702e 656d 7074 7928 286c 656e 286f   np.empty((len(o
-0000f280: 6d65 6761 292c 2064 2c20 642c 2064 2c20  mega), d, d, d, 
-0000f290: 6429 2c20 6474 7970 653d 636f 6d70 6c65  d), dtype=comple
-0000f2a0: 7829 0a20 2020 206d 736b 5f62 7566 7320  x).    msk_bufs 
-0000f2b0: 3d20 6e70 2e65 6d70 7479 2828 322c 206c  = np.empty((2, l
-0000f2c0: 656e 286f 6d65 6761 292c 2064 2c20 642c  en(omega), d, d,
-0000f2d0: 2064 2c20 6429 2c20 6474 7970 653d 626f   d, d), dtype=bo
-0000f2e0: 6f6c 290a 2020 2020 6374 726c 6d61 745f  ol).    ctrlmat_
-0000f2f0: 7374 6570 5f63 756d 756c 6174 6976 6520  step_cumulative 
-0000f300: 3d20 6e70 2e7a 6572 6f73 2828 6c65 6e28  = np.zeros((len(
-0000f310: 6e5f 636f 6566 6673 292c 206c 656e 2862  n_coeffs), len(b
-0000f320: 6173 6973 292c 206c 656e 286f 6d65 6761  asis), len(omega
-0000f330: 2929 2c20 6474 7970 653d 636f 6d70 6c65  )), dtype=comple
-0000f340: 7829 0a0a 2020 2020 7368 6170 6520 3d20  x)..    shape = 
-0000f350: 286c 656e 286e 5f63 6f65 6666 7329 2c20  (len(n_coeffs), 
-0000f360: 6c65 6e28 6e5f 636f 6566 6673 292c 206c  len(n_coeffs), l
-0000f370: 656e 2862 6173 6973 292c 206c 656e 2862  en(basis), len(b
-0000f380: 6173 6973 292c 206c 656e 286f 6d65 6761  asis), len(omega
-0000f390: 2929 0a20 2020 2073 7465 705f 6275 6620  )).    step_buf 
-0000f3a0: 3d20 6e70 2e65 6d70 7479 2873 6861 7065  = np.empty(shape
-0000f3b0: 2c20 6474 7970 653d 636f 6d70 6c65 7829  , dtype=complex)
-0000f3c0: 0a20 2020 2072 6573 756c 7420 3d20 6e70  .    result = np
-0000f3d0: 2e7a 6572 6f73 2873 6861 7065 2c20 6474  .zeros(shape, dt
-0000f3e0: 7970 653d 636f 6d70 6c65 7829 0a0a 2020  ype=complex)..  
-0000f3f0: 2020 2320 696e 7465 726d 6564 6961 7465    # intermediate
-0000f400: 2072 6573 756c 7473 2066 726f 6d20 6361   results from ca
-0000f410: 6c63 756c 6174 696f 6e20 6f66 2063 6f6e  lculation of con
-0000f420: 7472 6f6c 206d 6174 7269 780a 2020 2020  trol matrix.    
-0000f430: 6966 2069 6e74 6572 6d65 6469 6174 6573  if intermediates
-0000f440: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-0000f450: 2020 696e 7465 726d 6564 6961 7465 7320    intermediates 
-0000f460: 3d20 6469 6374 2829 0a0a 2020 2020 2320  = dict()..    # 
-0000f470: 576f 726b 2061 726f 756e 6420 706f 7373  Work around poss
-0000f480: 6962 6c79 2070 6f70 756c 6174 6564 2069  ibly populated i
-0000f490: 6e74 6572 6d65 6469 6174 6573 2064 6963  ntermediates dic
-0000f4a0: 7420 7769 7468 206d 6973 7369 6e67 206b  t with missing k
-0000f4b0: 6579 730a 2020 2020 6e5f 6f70 6572 735f  eys.    n_opers_
-0000f4c0: 7472 616e 7366 6f72 6d65 6420 3d20 696e  transformed = in
-0000f4d0: 7465 726d 6564 6961 7465 732e 6765 7428  termediates.get(
-0000f4e0: 276e 5f6f 7065 7273 5f74 7261 6e73 666f  'n_opers_transfo
-0000f4f0: 726d 6564 2729 0a20 2020 2069 6620 6e5f  rmed').    if n_
-0000f500: 6f70 6572 735f 7472 616e 7366 6f72 6d65  opers_transforme
-0000f510: 6420 6973 204e 6f6e 653a 0a20 2020 2020  d is None:.     
-0000f520: 2020 206e 5f6f 7065 7273 5f74 7261 6e73     n_opers_trans
-0000f530: 666f 726d 6564 203d 205f 7472 616e 7366  formed = _transf
-0000f540: 6f72 6d5f 6861 6d69 6c74 6f6e 6961 6e28  orm_hamiltonian(
-0000f550: 6569 6776 6563 732c 206e 5f6f 7065 7273  eigvecs, n_opers
-0000f560: 2c20 6e5f 636f 6566 6673 290a 0a20 2020  , n_coeffs)..   
-0000f570: 2074 7279 3a0a 2020 2020 2020 2020 6261   try:.        ba
-0000f580: 7369 735f 7472 616e 7366 6f72 6d65 645f  sis_transformed_
-0000f590: 6361 6368 6520 3d20 696e 7465 726d 6564  cache = intermed
-0000f5a0: 6961 7465 735b 2762 6173 6973 5f74 7261  iates['basis_tra
-0000f5b0: 6e73 666f 726d 6564 275d 0a20 2020 2020  nsformed'].     
-0000f5c0: 2020 2063 7472 6c6d 6174 5f73 7465 705f     ctrlmat_step_
-0000f5d0: 6361 6368 6520 3d20 696e 7465 726d 6564  cache = intermed
-0000f5e0: 6961 7465 735b 2763 6f6e 7472 6f6c 5f6d  iates['control_m
-0000f5f0: 6174 7269 785f 7374 6570 275d 0a20 2020  atrix_step'].   
-0000f600: 2020 2020 2068 6176 655f 696e 7465 726d       have_interm
-0000f610: 6564 6961 7465 7320 3d20 5472 7565 0a20  ediates = True. 
-0000f620: 2020 2065 7863 6570 7420 4b65 7945 7272     except KeyErr
-0000f630: 6f72 3a0a 2020 2020 2020 2020 6861 7665  or:.        have
-0000f640: 5f69 6e74 6572 6d65 6469 6174 6573 203d  _intermediates =
-0000f650: 2046 616c 7365 0a20 2020 2020 2020 2023   False.        #
-0000f660: 204e 6f20 6361 6368 652e 2050 7265 636f   No cache. Preco
-0000f670: 6d70 7574 6520 736f 6d65 2074 6869 6e67  mpute some thing
-0000f680: 7320 616e 6420 7065 7266 6f72 6d20 7468  s and perform th
-0000f690: 6520 636f 7374 6c79 2063 6f6d 7075 7461  e costly computa
-0000f6a0: 7469 6f6e 730a 2020 2020 2020 2020 2320  tions.        # 
-0000f6b0: 6475 7269 6e67 2065 6163 6820 6c6f 6f70  during each loop
-0000f6c0: 2069 7465 7261 7469 6f6e 2062 656c 6f77   iteration below
-0000f6d0: 0a20 2020 2020 2020 2074 203d 206e 702e  .        t = np.
-0000f6e0: 636f 6e63 6174 656e 6174 6528 285b 305d  concatenate(([0]
-0000f6f0: 2c20 6e70 2e61 7361 7272 6179 2864 7429  , np.asarray(dt)
-0000f700: 2e63 756d 7375 6d28 2929 290a 2020 2020  .cumsum())).    
-0000f710: 2020 2020 6569 6776 6563 735f 7072 6f70      eigvecs_prop
-0000f720: 6167 6174 6564 203d 205f 7072 6f70 6167  agated = _propag
-0000f730: 6174 655f 6569 6765 6e76 6563 746f 7273  ate_eigenvectors
-0000f740: 2870 726f 7061 6761 746f 7273 5b3a 2d31  (propagators[:-1
-0000f750: 5d2c 2065 6967 7665 6373 290a 2020 2020  ], eigvecs).    
-0000f760: 2020 2020 6261 7369 735f 7472 616e 7366      basis_transf
-0000f770: 6f72 6d65 6420 3d20 6e70 2e65 6d70 7479  ormed = np.empty
-0000f780: 2862 6173 6973 2e73 6861 7065 2c20 6474  (basis.shape, dt
-0000f790: 7970 653d 636f 6d70 6c65 7829 0a20 2020  ype=complex).   
-0000f7a0: 2020 2020 2063 7472 6c6d 6174 5f73 7465       ctrlmat_ste
-0000f7b0: 7020 3d20 6e70 2e7a 6572 6f73 2828 6c65  p = np.zeros((le
-0000f7c0: 6e28 6e5f 636f 6566 6673 292c 206c 656e  n(n_coeffs), len
-0000f7d0: 2862 6173 6973 292c 206c 656e 286f 6d65  (basis), len(ome
-0000f7e0: 6761 2929 2c20 6474 7970 653d 636f 6d70  ga)), dtype=comp
-0000f7f0: 6c65 7829 0a0a 2020 2020 7374 6570 5f65  lex)..    step_e
-0000f800: 7870 7220 3d20 6f65 2e63 6f6e 7472 6163  xpr = oe.contrac
-0000f810: 745f 6578 7072 6573 7369 6f6e 2827 6f69  t_expression('oi
-0000f820: 6a6d 6e2c 616b 696a 2c62 6c6d 6e2d 3e61  jmn,akij,blmn->a
-0000f830: 626b 6c6f 272c 2069 6e74 5f62 7566 2e73  bklo', int_buf.s
-0000f840: 6861 7065 2c0a 2020 2020 2020 2020 2020  hape,.          
-0000f850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f860: 2020 2020 2020 2020 2020 2020 202a 5b28               *[(
-0000f870: 6c65 6e28 6e5f 636f 6566 6673 292c 206c  len(n_coeffs), l
-0000f880: 656e 2862 6173 6973 292c 2064 2c20 6429  en(basis), d, d)
-0000f890: 5d2a 322c 0a20 2020 2020 2020 2020 2020  ]*2,.           
+00008400: 2020 2020 2020 2020 2020 2020 2064 6573               des
+00008410: 633d 2743 616c 6375 6c61 7469 6e67 2063  c='Calculating c
+00008420: 6f6e 7472 6f6c 206d 6174 7269 7827 293a  ontrol matrix'):
+00008430: 0a0a 2020 2020 2020 2020 6966 2063 6163  ..        if cac
+00008440: 6865 5f69 6e74 6572 6d65 6469 6174 6573  he_intermediates
+00008450: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
+00008460: 4173 7369 676e 2072 6566 6572 656e 6365  Assign reference
+00008470: 7320 746f 2074 6865 206c 6f63 6174 696f  s to the locatio
+00008480: 6e73 2069 6e20 7468 6520 6361 6368 6520  ns in the cache 
+00008490: 666f 7220 7468 6520 7175 616e 7469 7469  for the quantiti
+000084a0: 6573 0a20 2020 2020 2020 2020 2020 2023  es.            #
+000084b0: 2074 6861 7420 7368 6f75 6c64 2062 6520   that should be 
+000084c0: 7374 6f72 6564 0a20 2020 2020 2020 2020  stored.         
+000084d0: 2020 2062 6173 6973 5f74 7261 6e73 666f     basis_transfo
+000084e0: 726d 6564 203d 2062 6173 6973 5f74 7261  rmed = basis_tra
+000084f0: 6e73 666f 726d 6564 5f63 6163 6865 5b67  nsformed_cache[g
+00008500: 5d0a 2020 2020 2020 2020 2020 2020 7068  ].            ph
+00008510: 6173 655f 6661 6374 6f72 7320 3d20 7068  ase_factors = ph
+00008520: 6173 655f 6661 6374 6f72 735f 6361 6368  ase_factors_cach
+00008530: 655b 675d 0a20 2020 2020 2020 2020 2020  e[g].           
+00008540: 2069 6e74 5f62 7566 203d 2069 6e74 5f63   int_buf = int_c
+00008550: 6163 6865 5b67 5d0a 2020 2020 2020 2020  ache[g].        
+00008560: 2020 2020 7375 6d5f 6275 6620 3d20 7375      sum_buf = su
+00008570: 6d5f 6361 6368 655b 675d 0a0a 2020 2020  m_cache[g]..    
+00008580: 2020 2020 6261 7369 735f 7472 616e 7366      basis_transf
+00008590: 6f72 6d65 6420 3d20 5f74 7261 6e73 666f  ormed = _transfo
+000085a0: 726d 5f62 795f 756e 6974 6172 7928 6569  rm_by_unitary(ei
+000085b0: 6776 6563 735f 7072 6f70 6167 6174 6564  gvecs_propagated
+000085c0: 5b67 5d2c 2062 6173 6973 2c0a 2020 2020  [g], basis,.    
+000085d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000085e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000085f0: 2020 2020 2020 2020 2020 2020 2020 6f75                ou
+00008600: 743d 6261 7369 735f 7472 616e 7366 6f72  t=basis_transfor
+00008610: 6d65 6429 0a20 2020 2020 2020 2070 6861  med).        pha
+00008620: 7365 5f66 6163 746f 7273 203d 2075 7469  se_factors = uti
+00008630: 6c2e 6365 7870 286f 6d65 6761 2a74 5b67  l.cexp(omega*t[g
+00008640: 5d2c 206f 7574 3d70 6861 7365 5f66 6163  ], out=phase_fac
+00008650: 746f 7273 290a 2020 2020 2020 2020 696e  tors).        in
+00008660: 745f 6275 6620 3d20 5f66 6972 7374 5f6f  t_buf = _first_o
+00008670: 7264 6572 5f69 6e74 6567 7261 6c28 6f6d  rder_integral(om
+00008680: 6567 612c 2065 6967 7661 6c73 5b67 5d2c  ega, eigvals[g],
+00008690: 2064 745b 675d 2c20 6578 705f 6275 662c   dt[g], exp_buf,
+000086a0: 2069 6e74 5f62 7566 290a 2020 2020 2020   int_buf).      
+000086b0: 2020 7375 6d5f 6275 6620 3d20 6578 7072    sum_buf = expr
+000086c0: 2870 6861 7365 5f66 6163 746f 7273 2c20  (phase_factors, 
+000086d0: 6e5f 6f70 6572 735f 7472 616e 7366 6f72  n_opers_transfor
+000086e0: 6d65 645b 3a2c 2067 5d2c 2069 6e74 5f62  med[:, g], int_b
+000086f0: 7566 2c0a 2020 2020 2020 2020 2020 2020  uf,.            
+00008700: 2020 2020 2020 2020 2020 2062 6173 6973             basis
+00008710: 5f74 7261 6e73 666f 726d 6564 2c20 6f75  _transformed, ou
+00008720: 743d 7375 6d5f 6275 6629 0a0a 2020 2020  t=sum_buf)..    
+00008730: 2020 2020 6f75 7420 2b3d 2073 756d 5f62      out += sum_b
+00008740: 7566 0a0a 2020 2020 6966 2063 6163 6865  uf..    if cache
+00008750: 5f69 6e74 6572 6d65 6469 6174 6573 3a0a  _intermediates:.
+00008760: 2020 2020 2020 2020 696e 7465 726d 6564          intermed
+00008770: 6961 7465 7320 3d20 6469 6374 286e 5f6f  iates = dict(n_o
+00008780: 7065 7273 5f74 7261 6e73 666f 726d 6564  pers_transformed
+00008790: 3d6e 5f6f 7065 7273 5f74 7261 6e73 666f  =n_opers_transfo
+000087a0: 726d 6564 2c0a 2020 2020 2020 2020 2020  rmed,.          
+000087b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000087c0: 2020 2062 6173 6973 5f74 7261 6e73 666f     basis_transfo
+000087d0: 726d 6564 3d62 6173 6973 5f74 7261 6e73  rmed=basis_trans
+000087e0: 666f 726d 6564 5f63 6163 6865 2c0a 2020  formed_cache,.  
+000087f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008800: 2020 2020 2020 2020 2020 2070 6861 7365             phase
+00008810: 5f66 6163 746f 7273 3d70 6861 7365 5f66  _factors=phase_f
+00008820: 6163 746f 7273 5f63 6163 6865 2c0a 2020  actors_cache,.  
+00008830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008840: 2020 2020 2020 2020 2020 2066 6972 7374             first
+00008850: 5f6f 7264 6572 5f69 6e74 6567 7261 6c3d  _order_integral=
+00008860: 696e 745f 6361 6368 652c 0a20 2020 2020  int_cache,.     
+00008870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008880: 2020 2020 2020 2020 636f 6e74 726f 6c5f          control_
+00008890: 6d61 7472 6978 5f73 7465 703d 7375 6d5f  matrix_step=sum_
+000088a0: 6361 6368 6529 0a20 2020 2020 2020 2072  cache).        r
+000088b0: 6574 7572 6e20 6f75 742c 2069 6e74 6572  eturn out, inter
+000088c0: 6d65 6469 6174 6573 0a0a 2020 2020 7265  mediates..    re
+000088d0: 7475 726e 206f 7574 0a0a 0a64 6566 2063  turn out...def c
+000088e0: 616c 6375 6c61 7465 5f63 6f6e 7472 6f6c  alculate_control
+000088f0: 5f6d 6174 7269 785f 7065 7269 6f64 6963  _matrix_periodic
+00008900: 2870 6861 7365 733a 206e 6461 7272 6179  (phases: ndarray
+00008910: 2c20 636f 6e74 726f 6c5f 6d61 7472 6978  , control_matrix
+00008920: 3a20 6e64 6172 7261 792c 0a20 2020 2020  : ndarray,.     
+00008930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008950: 2074 6f74 616c 5f70 726f 7061 6761 746f   total_propagato
+00008960: 725f 6c69 6f75 7669 6c6c 653a 206e 6461  r_liouville: nda
+00008970: 7272 6179 2c0a 2020 2020 2020 2020 2020  rray,.          
+00008980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008990: 2020 2020 2020 2020 2020 2020 7265 7065              repe
+000089a0: 6174 733a 2069 6e74 2c20 6368 6563 6b5f  ats: int, check_
+000089b0: 696e 7665 7274 6962 6c65 3a20 626f 6f6c  invertible: bool
+000089c0: 203d 2054 7275 6529 202d 3e20 6e64 6172   = True) -> ndar
+000089d0: 7261 793a 0a20 2020 2072 2222 220a 2020  ray:.    r""".  
+000089e0: 2020 4361 6c63 756c 6174 6520 7468 6520    Calculate the 
+000089f0: 636f 6e74 726f 6c20 6d61 7472 6978 206f  control matrix o
+00008a00: 6620 6120 7065 7269 6f64 6963 2070 756c  f a periodic pul
+00008a10: 7365 2067 6976 656e 2074 6865 2070 6861  se given the pha
+00008a20: 7365 0a20 2020 2066 6163 746f 7273 2c20  se.    factors, 
+00008a30: 636f 6e74 726f 6c20 6d61 7472 6978 2061  control matrix a
+00008a40: 6e64 2074 7261 6e73 6665 7220 6d61 7472  nd transfer matr
+00008a50: 6978 206f 6620 7468 6520 746f 7461 6c20  ix of the total 
+00008a60: 7072 6f70 6167 6174 6f72 2c0a 2020 2020  propagator,.    
+00008a70: 746f 7461 6c5f 7072 6f70 6167 6174 6f72  total_propagator
+00008a80: 5f6c 696f 7576 696c 6c65 2c20 6f66 2074  _liouville, of t
+00008a90: 6865 2061 746f 6d69 6320 7075 6c73 652e  he atomic pulse.
+00008aa0: 0a0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
+00008ab0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
+00008ac0: 2020 2020 7068 6173 6573 3a20 6e64 6172      phases: ndar
+00008ad0: 7261 792c 2073 6861 7065 2028 6e5f 6f6d  ray, shape (n_om
+00008ae0: 6567 612c 290a 2020 2020 2020 2020 5468  ega,).        Th
+00008af0: 6520 7068 6173 6520 6661 6374 6f72 7320  e phase factors 
+00008b00: 3a6d 6174 683a 6065 5e7b 695c 6f6d 6567  :math:`e^{i\omeg
+00008b10: 6120 547d 6020 6f66 2074 6865 2061 746f  a T}` of the ato
+00008b20: 6d69 6320 7075 6c73 652e 0a20 2020 2063  mic pulse..    c
+00008b30: 6f6e 7472 6f6c 5f6d 6174 7269 783a 206e  ontrol_matrix: n
+00008b40: 6461 7272 6179 2c20 7368 6170 6520 286e  darray, shape (n
+00008b50: 5f6e 6f70 732c 2064 2a2a 322c 206e 5f6f  _nops, d**2, n_o
+00008b60: 6d65 6761 290a 2020 2020 2020 2020 5468  mega).        Th
+00008b70: 6520 636f 6e74 726f 6c20 6d61 7472 6978  e control matrix
+00008b80: 203a 6d61 7468 3a60 5c74 696c 6465 7b5c   :math:`\tilde{\
+00008b90: 6d61 7468 6361 6c7b 427d 7d5e 7b28 3129  mathcal{B}}^{(1)
+00008ba0: 7d28 5c6f 6d65 6761 2960 206f 660a 2020  }(\omega)` of.  
+00008bb0: 2020 2020 2020 7468 6520 6174 6f6d 6963        the atomic
+00008bc0: 2070 756c 7365 2e0a 2020 2020 746f 7461   pulse..    tota
+00008bd0: 6c5f 7072 6f70 6167 6174 6f72 5f6c 696f  l_propagator_lio
+00008be0: 7576 696c 6c65 3a20 6e64 6172 7261 792c  uville: ndarray,
+00008bf0: 2073 6861 7065 2028 642a 2a32 2c20 642a   shape (d**2, d*
+00008c00: 2a32 290a 2020 2020 2020 2020 5468 6520  *2).        The 
+00008c10: 7472 616e 7366 6572 206d 6174 7269 7820  transfer matrix 
+00008c20: 3a6d 6174 683a 605c 6d61 7468 6361 6c7b  :math:`\mathcal{
+00008c30: 517d 5e7b 2831 297d 6020 6f66 2074 6865  Q}^{(1)}` of the
+00008c40: 2061 746f 6d69 630a 2020 2020 2020 2020   atomic.        
+00008c50: 7075 6c73 652e 0a20 2020 2072 6570 6561  pulse..    repea
+00008c60: 7473 3a20 696e 740a 2020 2020 2020 2020  ts: int.        
+00008c70: 5468 6520 6e75 6d62 6572 206f 6620 7265  The number of re
+00008c80: 7065 7469 7469 6f6e 732e 0a20 2020 2063  petitions..    c
+00008c90: 6865 636b 5f69 6e76 6572 7469 626c 653a  heck_invertible:
+00008ca0: 2062 6f6f 6c2c 206f 7074 696f 6e61 6c0a   bool, optional.
+00008cb0: 2020 2020 2020 2020 4368 6563 6b20 666f          Check fo
+00008cc0: 7220 616c 6c20 6672 6571 7565 6e63 6965  r all frequencie
+00008cd0: 7320 6966 2074 6865 2069 6e76 6572 7365  s if the inverse
+00008ce0: 203a 6d61 7468 3a60 5c6d 6174 6862 627b   :math:`\mathbb{
+00008cf0: 497d 202d 0a20 2020 2020 2020 2065 5e7b  I} -.        e^{
+00008d00: 695c 6f6d 6567 6120 547d 205c 6d61 7468  i\omega T} \math
+00008d10: 6361 6c7b 517d 5e7b 2831 297d 6020 6578  cal{Q}^{(1)}` ex
+00008d20: 6973 7473 2062 7920 6361 6c63 756c 6174  ists by calculat
+00008d30: 696e 6720 7468 650a 2020 2020 2020 2020  ing the.        
+00008d40: 6465 7465 726d 696e 616e 742e 2049 6620  determinant. If 
+00008d50: 6974 2064 6f65 7320 6e6f 7420 6578 6973  it does not exis
+00008d60: 742c 2074 6865 2073 756d 2069 7320 6576  t, the sum is ev
+00008d70: 616c 7561 7465 640a 2020 2020 2020 2020  aluated.        
+00008d80: 6578 706c 6963 6974 6c79 2066 6f72 2074  explicitly for t
+00008d90: 686f 7365 2070 6f69 6e74 732e 2054 6865  hose points. The
+00008da0: 2064 6566 6175 6c74 2069 7320 5472 7565   default is True
+00008db0: 2e0a 0a20 2020 2052 6574 7572 6e73 0a20  ...    Returns. 
+00008dc0: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2063     -------.    c
+00008dd0: 6f6e 7472 6f6c 5f6d 6174 7269 783a 206e  ontrol_matrix: n
+00008de0: 6461 7272 6179 2c20 7368 6170 6520 286e  darray, shape (n
+00008df0: 5f6e 6f70 732c 2064 2a2a 322c 206e 5f6f  _nops, d**2, n_o
+00008e00: 6d65 6761 290a 2020 2020 2020 2020 5468  mega).        Th
+00008e10: 6520 636f 6e74 726f 6c20 6d61 7472 6978  e control matrix
+00008e20: 203a 6d61 7468 3a60 5c74 696c 6465 7b5c   :math:`\tilde{\
+00008e30: 6d61 7468 6361 6c7b 427d 7d28 5c6f 6d65  mathcal{B}}(\ome
+00008e40: 6761 2960 206f 6620 7468 650a 2020 2020  ga)` of the.    
+00008e50: 2020 2020 7265 7065 6174 6564 2070 756c      repeated pul
+00008e60: 7365 2e0a 0a20 2020 204e 6f74 6573 0a20  se...    Notes. 
+00008e70: 2020 202d 2d2d 2d2d 0a20 2020 2054 6865     -----.    The
+00008e80: 2063 6f6e 7472 6f6c 206d 6174 7269 7820   control matrix 
+00008e90: 6973 2063 6f6d 7075 7465 6420 6173 0a0a  is computed as..
+00008ea0: 2020 2020 2e2e 206d 6174 683a 3a0a 0a20      .. math::.. 
+00008eb0: 2020 2020 2020 205c 7469 6c64 657b 5c6d         \tilde{\m
+00008ec0: 6174 6863 616c 7b42 7d7d 285c 6f6d 6567  athcal{B}}(\omeg
+00008ed0: 6129 0a20 2020 2020 2020 2020 2020 2020  a).             
+00008ee0: 2020 2020 2020 2020 2020 2020 2020 2026                 &
+00008ef0: 3d20 5c74 696c 6465 7b5c 6d61 7468 6361  = \tilde{\mathca
+00008f00: 6c7b 427d 7d5e 7b28 3129 7d28 5c6f 6d65  l{B}}^{(1)}(\ome
+00008f10: 6761 290a 2020 2020 2020 2020 2020 2020  ga).            
+00008f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008f30: 2020 205c 7375 6d5f 7b67 3d30 7d5e 7b47     \sum_{g=0}^{G
+00008f40: 2d31 7d0a 2020 2020 2020 2020 2020 2020  -1}.            
+00008f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008f60: 2020 205c 6c65 6674 2865 5e7b 695c 6f6d     \left(e^{i\om
+00008f70: 6567 6120 547d 5c72 6967 6874 295e 6720  ega T}\right)^g 
+00008f80: 5c5c 0a20 2020 2020 2020 2020 2020 2020  \\.             
+00008f90: 2020 2020 2020 2020 2020 2020 2020 2026                 &
+00008fa0: 3d20 5c74 696c 6465 7b5c 6d61 7468 6361  = \tilde{\mathca
+00008fb0: 6c7b 427d 7d5e 7b28 3129 7d28 5c6f 6d65  l{B}}^{(1)}(\ome
+00008fc0: 6761 295c 6269 676c 280a 2020 2020 2020  ga)\bigl(.      
+00008fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008fe0: 2020 2020 2020 2020 205c 6d61 7468 6262           \mathbb
+00008ff0: 7b49 7d20 2d20 655e 7b69 5c6f 6d65 6761  {I} - e^{i\omega
+00009000: 2054 7d0a 2020 2020 2020 2020 2020 2020   T}.            
+00009010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009020: 2020 205c 6d61 7468 6361 6c7b 517d 5e7b     \mathcal{Q}^{
+00009030: 2831 297d 5c62 6967 7229 5e7b 2d31 7d5c  (1)}\bigr)^{-1}\
+00009040: 6269 676c 280a 2020 2020 2020 2020 2020  bigl(.          
+00009050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009060: 2020 2020 205c 6d61 7468 6262 7b49 7d20       \mathbb{I} 
+00009070: 2d20 5c62 6967 6c28 655e 7b69 5c6f 6d65  - \bigl(e^{i\ome
+00009080: 6761 2054 7d0a 2020 2020 2020 2020 2020  ga T}.          
+00009090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000090a0: 2020 2020 205c 6d61 7468 6361 6c7b 517d       \mathcal{Q}
+000090b0: 5e7b 2831 297d 5c62 6967 7229 5e47 5c62  ^{(1)}\bigr)^G\b
+000090c0: 6967 7229 2e0a 0a20 2020 2077 6974 6820  igr)...    with 
+000090d0: 3a6d 6174 683a 6047 6020 7468 6520 6e75  :math:`G` the nu
+000090e0: 6d62 6572 206f 6620 7265 7065 7469 7469  mber of repetiti
+000090f0: 6f6e 732e 0a20 2020 2022 2222 0a20 2020  ons..    """.   
+00009100: 2023 2043 6f6d 7075 7465 2074 6865 2066   # Compute the f
+00009110: 696e 6974 6520 6765 6f6d 6574 7269 6320  inite geometric 
+00009120: 7365 7269 6573 205c 7375 6d5f 7b67 3d30  series \sum_{g=0
+00009130: 7d5e 7b47 2d31 7d20 545e 672e 2046 6972  }^{G-1} T^g. Fir
+00009140: 7374 2063 6865 636b 2069 660a 2020 2020  st check if.    
+00009150: 2320 696e 7628 4920 2d20 5429 2069 7320  # inv(I - T) is 
+00009160: 2767 6f6f 6427 2c20 692e 652e 2069 6620  'good', i.e. if 
+00009170: 696e 7628 4920 2d20 5429 2040 2028 4920  inv(I - T) @ (I 
+00009180: 2d20 5429 203d 3d20 492c 2073 696e 6365  - T) == I, since
+00009190: 204e 756d 5079 2077 696c 6c0a 2020 2020   NumPy will.    
+000091a0: 2320 636f 6d70 7574 6520 7468 6520 696e  # compute the in
+000091b0: 7665 7273 6520 696e 2061 6e79 2063 6173  verse in any cas
+000091c0: 652e 2046 6f72 2074 686f 7365 2066 7265  e. For those fre
+000091d0: 7175 656e 6369 6573 2077 6865 7265 2074  quencies where t
+000091e0: 6865 2069 6e76 6572 7365 0a20 2020 2023  he inverse.    #
+000091f0: 2069 7320 7765 6c6c 2d62 6568 6176 6564   is well-behaved
+00009200: 2c20 6576 616c 7561 7465 2074 6865 2073  , evaluate the s
+00009210: 756d 2061 7320 6120 4e65 756d 616e 6e20  um as a Neumann 
+00009220: 7365 7269 6573 2061 6e64 2066 6f72 2074  series and for t
+00009230: 6865 2072 6573 740a 2020 2020 2320 6576  he rest.    # ev
+00009240: 616c 7561 7465 2069 7420 6578 706c 6963  aluate it explic
+00009250: 6974 6c79 2e0a 2020 2020 6579 6520 3d20  itly..    eye = 
+00009260: 6e70 2e65 7965 2874 6f74 616c 5f70 726f  np.eye(total_pro
+00009270: 7061 6761 746f 725f 6c69 6f75 7669 6c6c  pagator_liouvill
+00009280: 652e 7368 6170 655b 305d 290a 2020 2020  e.shape[0]).    
+00009290: 5420 3d20 6e70 2e6d 756c 7469 706c 792e  T = np.multiply.
+000092a0: 6f75 7465 7228 7068 6173 6573 2c20 746f  outer(phases, to
+000092b0: 7461 6c5f 7072 6f70 6167 6174 6f72 5f6c  tal_propagator_l
+000092c0: 696f 7576 696c 6c65 290a 2020 2020 4d20  iouville).    M 
+000092d0: 3d20 6579 6520 2d20 540a 2020 2020 6966  = eye - T.    if
+000092e0: 2063 6865 636b 5f69 6e76 6572 7469 626c   check_invertibl
+000092f0: 653a 0a20 2020 2020 2020 2069 6e76 6572  e:.        inver
+00009300: 7469 626c 6520 3d20 7e6e 702e 6973 636c  tible = ~np.iscl
+00009310: 6f73 6528 6e6c 612e 6465 7428 4d29 2c20  ose(nla.det(M), 
+00009320: 3029 0a20 2020 2065 6c73 653a 0a20 2020  0).    else:.   
+00009330: 2020 2020 2069 6e76 6572 7469 626c 6520       invertible 
+00009340: 3d20 6e70 2e61 7272 6179 2854 7275 6529  = np.array(True)
+00009350: 0a0a 2020 2020 5320 3d20 6e70 2e65 6d70  ..    S = np.emp
+00009360: 7479 2828 2a70 6861 7365 732e 7368 6170  ty((*phases.shap
+00009370: 652c 202a 746f 7461 6c5f 7072 6f70 6167  e, *total_propag
+00009380: 6174 6f72 5f6c 696f 7576 696c 6c65 2e73  ator_liouville.s
+00009390: 6861 7065 292c 2064 7479 7065 3d63 6f6d  hape), dtype=com
+000093a0: 706c 6578 290a 2020 2020 2320 536f 6c76  plex).    # Solv
+000093b0: 6520 4c53 4520 696e 7374 6561 6420 6f66  e LSE instead of
+000093c0: 2063 6f6d 7075 7469 6e67 2069 6e76 6572   computing inver
+000093d0: 7365 2c20 6661 7374 6572 202b 206e 756d  se, faster + num
+000093e0: 6572 6963 616c 6c79 206d 6f72 6520 7374  erically more st
+000093f0: 6162 6c65 0a20 2020 2053 5b69 6e76 6572  able.    S[inver
+00009400: 7469 626c 655d 203d 206e 6c61 2e73 6f6c  tible] = nla.sol
+00009410: 7665 284d 5b69 6e76 6572 7469 626c 655d  ve(M[invertible]
+00009420: 2c20 6579 6520 2d20 6e6c 612e 6d61 7472  , eye - nla.matr
+00009430: 6978 5f70 6f77 6572 2854 5b69 6e76 6572  ix_power(T[inver
+00009440: 7469 626c 655d 2c20 7265 7065 6174 7329  tible], repeats)
+00009450: 290a 2020 2020 6966 2028 7e69 6e76 6572  ).    if (~inver
+00009460: 7469 626c 6529 2e61 6e79 2829 3a0a 2020  tible).any():.  
+00009470: 2020 2020 2020 535b 7e69 6e76 6572 7469        S[~inverti
+00009480: 626c 655d 203d 2065 7965 202b 2073 756d  ble] = eye + sum
+00009490: 2861 6363 756d 756c 6174 6528 7265 7065  (accumulate(repe
+000094a0: 6174 2854 5b7e 696e 7665 7274 6962 6c65  at(T[~invertible
+000094b0: 5d2c 2072 6570 6561 7473 2d31 292c 206e  ], repeats-1), n
+000094c0: 702e 6d61 746d 756c 2929 0a0a 2020 2020  p.matmul))..    
+000094d0: 636f 6e74 726f 6c5f 6d61 7472 6978 5f74  control_matrix_t
+000094e0: 6f74 203d 2028 636f 6e74 726f 6c5f 6d61  ot = (control_ma
+000094f0: 7472 6978 2e74 7261 6e73 706f 7365 2832  trix.transpose(2
+00009500: 2c20 302c 2031 2920 4020 5329 2e74 7261  , 0, 1) @ S).tra
+00009510: 6e73 706f 7365 2831 2c20 322c 2030 290a  nspose(1, 2, 0).
+00009520: 2020 2020 7265 7475 726e 2063 6f6e 7472      return contr
+00009530: 6f6c 5f6d 6174 7269 785f 746f 740a 0a0a  ol_matrix_tot...
+00009540: 4075 7469 6c2e 7061 7273 655f 6f70 7469  @util.parse_opti
+00009550: 6f6e 616c 5f70 6172 616d 6574 6572 7328  onal_parameters(
+00009560: 7768 6963 683d 2827 746f 7461 6c27 2c20  which=('total', 
+00009570: 2763 6f72 7265 6c61 7469 6f6e 7327 2929  'correlations'))
+00009580: 0a64 6566 2063 616c 6375 6c61 7465 5f63  .def calculate_c
+00009590: 756d 756c 616e 745f 6675 6e63 7469 6f6e  umulant_function
+000095a0: 280a 2020 2020 2020 2020 7075 6c73 653a  (.        pulse:
+000095b0: 2027 5075 6c73 6553 6571 7565 6e63 6527   'PulseSequence'
+000095c0: 2c0a 2020 2020 2020 2020 7370 6563 7472  ,.        spectr
+000095d0: 756d 3a20 4f70 7469 6f6e 616c 5b6e 6461  um: Optional[nda
+000095e0: 7272 6179 5d20 3d20 4e6f 6e65 2c0a 2020  rray] = None,.  
+000095f0: 2020 2020 2020 6f6d 6567 613a 204f 7074        omega: Opt
+00009600: 696f 6e61 6c5b 436f 6566 6669 6369 656e  ional[Coefficien
+00009610: 7473 5d20 3d20 4e6f 6e65 2c0a 2020 2020  ts] = None,.    
+00009620: 2020 2020 6e5f 6f70 6572 5f69 6465 6e74      n_oper_ident
+00009630: 6966 6965 7273 3a20 4f70 7469 6f6e 616c  ifiers: Optional
+00009640: 5b53 6571 7565 6e63 655b 7374 725d 5d20  [Sequence[str]] 
+00009650: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00009660: 7768 6963 683a 2073 7472 203d 2027 746f  which: str = 'to
+00009670: 7461 6c27 2c0a 2020 2020 2020 2020 7365  tal',.        se
+00009680: 636f 6e64 5f6f 7264 6572 3a20 626f 6f6c  cond_order: bool
+00009690: 203d 2046 616c 7365 2c0a 2020 2020 2020   = False,.      
+000096a0: 2020 6465 6361 795f 616d 706c 6974 7564    decay_amplitud
+000096b0: 6573 3a20 4f70 7469 6f6e 616c 5b6e 6461  es: Optional[nda
+000096c0: 7272 6179 5d20 3d20 4e6f 6e65 2c0a 2020  rray] = None,.  
+000096d0: 2020 2020 2020 6672 6571 7565 6e63 795f        frequency_
+000096e0: 7368 6966 7473 3a20 4f70 7469 6f6e 616c  shifts: Optional
+000096f0: 5b6e 6461 7272 6179 5d20 3d20 4e6f 6e65  [ndarray] = None
+00009700: 2c0a 2020 2020 2020 2020 7368 6f77 5f70  ,.        show_p
+00009710: 726f 6772 6573 7362 6172 3a20 626f 6f6c  rogressbar: bool
+00009720: 203d 2046 616c 7365 2c0a 2020 2020 2020   = False,.      
+00009730: 2020 6d65 6d6f 7279 5f70 6172 7369 6d6f    memory_parsimo
+00009740: 6e69 6f75 733a 2062 6f6f 6c20 3d20 4661  nious: bool = Fa
+00009750: 6c73 652c 0a20 2020 2020 2020 2063 6163  lse,.        cac
+00009760: 6865 5f69 6e74 6572 6d65 6469 6174 6573  he_intermediates
+00009770: 3a20 4f70 7469 6f6e 616c 5b62 6f6f 6c5d  : Optional[bool]
+00009780: 203d 204e 6f6e 650a 2920 2d3e 206e 6461   = None.) -> nda
+00009790: 7272 6179 3a0a 2020 2020 7222 2222 4361  rray:.    r"""Ca
+000097a0: 6c63 756c 6174 6520 7468 6520 6375 6d75  lculate the cumu
+000097b0: 6c61 6e74 2066 756e 6374 696f 6e20 3a6d  lant function :m
+000097c0: 6174 683a 605c 6d61 7468 6361 6c7b 4b7d  ath:`\mathcal{K}
+000097d0: 285c 7461 7529 602e 0a0a 2020 2020 5468  (\tau)`...    Th
+000097e0: 6520 6572 726f 7220 7472 616e 7366 6572  e error transfer
+000097f0: 206d 6174 7269 7820 6973 206f 6274 6169   matrix is obtai
+00009800: 6e65 6420 6672 6f6d 2074 6865 2063 756d  ned from the cum
+00009810: 756c 616e 7420 6675 6e63 7469 6f6e 2062  ulant function b
+00009820: 790a 2020 2020 6578 706f 6e65 6e74 6961  y.    exponentia
+00009830: 7469 6f6e 2c0a 2020 2020 3a6d 6174 683a  tion,.    :math:
+00009840: 605c 6c61 6e67 6c65 5c74 696c 6465 7b5c  `\langle\tilde{\
+00009850: 6d61 7468 6361 6c7b 557d 7d5c 7261 6e67  mathcal{U}}\rang
+00009860: 6c65 203d 205c 6578 705c 6d61 7468 6361  le = \exp\mathca
+00009870: 6c7b 4b7d 285c 7461 7529 602e 0a0a 2020  l{K}(\tau)`...  
+00009880: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+00009890: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+000098a0: 7075 6c73 653a 2050 756c 7365 5365 7175  pulse: PulseSequ
+000098b0: 656e 6365 0a20 2020 2020 2020 2054 6865  ence.        The
+000098c0: 2060 6050 756c 7365 5365 7175 656e 6365   ``PulseSequence
+000098d0: 6060 2069 6e73 7461 6e63 6520 666f 7220  `` instance for 
+000098e0: 7768 6963 6820 746f 2063 6f6d 7075 7465  which to compute
+000098f0: 2074 6865 2063 756d 756c 616e 740a 2020   the cumulant.  
+00009900: 2020 2020 2020 6675 6e63 7469 6f6e 2e0a        function..
+00009910: 2020 2020 7370 6563 7472 756d 3a20 6172      spectrum: ar
+00009920: 7261 795f 6c69 6b65 2c20 7368 6170 6520  ray_like, shape 
+00009930: 285b 5b6e 5f6e 6f70 732c 5d20 6e5f 6e6f  ([[n_nops,] n_no
+00009940: 7073 2c5d 206e 5f6f 6d65 6761 292c 206f  ps,] n_omega), o
+00009950: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
+00009960: 5468 6520 6e6f 6973 6520 706f 7765 7220  The noise power 
+00009970: 7370 6563 7472 616c 2064 656e 7369 7479  spectral density
+00009980: 2069 6e20 756e 6974 7320 6f66 2069 6e76   in units of inv
+00009990: 6572 7365 2066 7265 7175 656e 6369 6573  erse frequencies
+000099a0: 0a20 2020 2020 2020 2061 7320 616e 2061  .        as an a
+000099b0: 7272 6179 206f 6620 7368 6170 6520 286e  rray of shape (n
+000099c0: 5f6f 6d65 6761 2c29 2c20 286e 5f6e 6f70  _omega,), (n_nop
+000099d0: 732c 206e 5f6f 6d65 6761 292c 206f 7220  s, n_omega), or 
+000099e0: 286e 5f6e 6f70 732c 0a20 2020 2020 2020  (n_nops,.       
+000099f0: 206e 5f6e 6f70 732c 206e 5f6f 6d65 6761   n_nops, n_omega
+00009a00: 292e 2049 6e20 7468 6520 6669 7273 7420  ). In the first 
+00009a10: 6361 7365 2c20 7468 6520 7361 6d65 2073  case, the same s
+00009a20: 7065 6374 7275 6d20 6973 2074 616b 656e  pectrum is taken
+00009a30: 0a20 2020 2020 2020 2066 6f72 2061 6c6c  .        for all
+00009a40: 206e 6f69 7365 206f 7065 7261 746f 7273   noise operators
+00009a50: 2c20 696e 2074 6865 2073 6563 6f6e 642c  , in the second,
+00009a60: 2069 7420 6973 2061 7373 756d 6564 2074   it is assumed t
+00009a70: 6861 7420 7468 6572 650a 2020 2020 2020  hat there.      
+00009a80: 2020 6172 6520 6e6f 2063 6f72 7265 6c61    are no correla
+00009a90: 7469 6f6e 7320 6265 7477 6565 6e20 6469  tions between di
+00009aa0: 6666 6572 656e 7420 6e6f 6973 6520 736f  fferent noise so
+00009ab0: 7572 6365 7320 616e 6420 7468 7573 0a20  urces and thus. 
+00009ac0: 2020 2020 2020 2074 6865 7265 2069 7320         there is 
+00009ad0: 6f6e 6520 7370 6563 7472 756d 2066 6f72  one spectrum for
+00009ae0: 2065 6163 6820 6e6f 6973 6520 6f70 6572   each noise oper
+00009af0: 6174 6f72 2e20 496e 2074 6865 2074 6869  ator. In the thi
+00009b00: 7264 2061 6e64 0a20 2020 2020 2020 206d  rd and.        m
+00009b10: 6f73 7420 6765 6e65 7261 6c20 6361 7365  ost general case
+00009b20: 2c20 7468 6572 6520 6d61 7920 6265 2061  , there may be a
+00009b30: 2073 7065 6374 7275 6d20 666f 7220 6561   spectrum for ea
+00009b40: 6368 2070 6169 7220 6f66 0a20 2020 2020  ch pair of.     
+00009b50: 2020 206e 6f69 7365 206f 7065 7261 746f     noise operato
+00009b60: 7273 2063 6f72 7265 7370 6f6e 6469 6e67  rs corresponding
+00009b70: 2074 6f20 7468 6520 636f 7272 656c 6174   to the correlat
+00009b80: 696f 6e73 2062 6574 7765 656e 2074 6865  ions between the
+00009b90: 6d2e 0a20 2020 2020 2020 206e 5f6e 6f70  m..        n_nop
+00009ba0: 7320 6973 2074 6865 206e 756d 6265 7220  s is the number 
+00009bb0: 6f66 206e 6f69 7365 206f 7065 7261 746f  of noise operato
+00009bc0: 7273 2063 6f6e 7369 6465 7265 6420 616e  rs considered an
+00009bd0: 6420 7368 6f75 6c64 2062 650a 2020 2020  d should be.    
+00009be0: 2020 2020 6571 7561 6c20 746f 2060 606c      equal to ``l
+00009bf0: 656e 286e 5f6f 7065 725f 6964 656e 7469  en(n_oper_identi
+00009c00: 6669 6572 7329 6060 2e0a 2020 2020 6f6d  fiers)``..    om
+00009c10: 6567 613a 2061 7272 6179 5f6c 696b 652c  ega: array_like,
+00009c20: 2073 6861 7065 2028 6e5f 6f6d 6567 612c   shape (n_omega,
+00009c30: 292c 206f 7074 696f 6e61 6c0a 2020 2020  ), optional.    
+00009c40: 2020 2020 5468 6520 6672 6571 7565 6e63      The frequenc
+00009c50: 6965 7320 6174 2077 6869 6368 2074 6f20  ies at which to 
+00009c60: 6576 616c 7561 7465 2074 6865 2066 696c  evaluate the fil
+00009c70: 7465 7220 6675 6e63 7469 6f6e 732e 0a20  ter functions.. 
+00009c80: 2020 206e 5f6f 7065 725f 6964 656e 7469     n_oper_identi
+00009c90: 6669 6572 733a 2061 7272 6179 5f6c 696b  fiers: array_lik
+00009ca0: 652c 206f 7074 696f 6e61 6c0a 2020 2020  e, optional.    
+00009cb0: 2020 2020 5468 6520 6964 656e 7469 6669      The identifi
+00009cc0: 6572 7320 6f66 2074 6865 206e 6f69 7365  ers of the noise
+00009cd0: 206f 7065 7261 746f 7273 2066 6f72 2077   operators for w
+00009ce0: 6869 6368 2074 6f20 6576 616c 7561 7465  hich to evaluate
+00009cf0: 2074 6865 0a20 2020 2020 2020 2063 756d   the.        cum
+00009d00: 756c 616e 7420 6675 6e63 7469 6f6e 2e20  ulant function. 
+00009d10: 5468 6520 6465 6661 756c 7420 6973 2061  The default is a
+00009d20: 6c6c 2e0a 2020 2020 7768 6963 683a 2073  ll..    which: s
+00009d30: 7472 2c20 6f70 7469 6f6e 616c 0a20 2020  tr, optional.   
+00009d40: 2020 2020 2057 6869 6368 2064 6563 6179       Which decay
+00009d50: 2061 6d70 6c69 7475 6465 7320 7368 6f75   amplitudes shou
+00009d60: 6c64 2062 6520 6361 6c63 756c 6174 6564  ld be calculated
+00009d70: 2c20 6d61 7920 6265 2065 6974 6865 720a  , may be either.
+00009d80: 2020 2020 2020 2020 2774 6f74 616c 2720          'total' 
+00009d90: 2864 6566 6175 6c74 2920 6f72 2027 636f  (default) or 'co
+00009da0: 7272 656c 6174 696f 6e73 272e 2053 6565  rrelations'. See
+00009db0: 203a 6675 6e63 3a60 696e 6669 6465 6c69   :func:`infideli
+00009dc0: 7479 6020 616e 640a 2020 2020 2020 2020  ty` and.        
+00009dd0: 3a72 6566 3a60 4e6f 7465 7320 3c6e 6f74  :ref:`Notes <not
+00009de0: 6573 3e60 2e20 4e6f 7465 2074 6861 7420  es>`. Note that 
+00009df0: 7468 6520 6c61 7474 6572 2069 7320 6e6f  the latter is no
+00009e00: 7420 6176 6169 6c61 626c 6520 666f 720a  t available for.
+00009e10: 2020 2020 2020 2020 7468 6520 7365 636f          the seco
+00009e20: 6e64 206f 7264 6572 2074 6572 6d73 2e0a  nd order terms..
+00009e30: 2020 2020 7365 636f 6e64 5f6f 7264 6572      second_order
+00009e40: 3a20 626f 6f6c 2c20 6f70 7469 6f6e 616c  : bool, optional
+00009e50: 0a20 2020 2020 2020 2041 6c73 6f20 7461  .        Also ta
+00009e60: 6b65 2069 6e74 6f20 6163 636f 756e 7420  ke into account 
+00009e70: 7468 6520 6672 6571 7565 6e63 7920 7368  the frequency sh
+00009e80: 6966 7473 203a 6d61 7468 3a60 5c44 656c  ifts :math:`\Del
+00009e90: 7461 6020 7468 6174 0a20 2020 2020 2020  ta` that.       
+00009ea0: 2063 6f72 7265 7370 6f6e 6420 746f 2073   correspond to s
+00009eb0: 6563 6f6e 6420 6f72 6465 7220 4d61 676e  econd order Magn
+00009ec0: 7573 2065 7870 616e 7369 6f6e 2061 6e64  us expansion and
+00009ed0: 2063 6f6e 7374 6974 7574 650a 2020 2020   constitute.    
+00009ee0: 2020 2020 756e 6974 6172 7920 7465 726d      unitary term
+00009ef0: 732e 2044 6566 6175 6c74 2060 6046 616c  s. Default ``Fal
+00009f00: 7365 6060 2e0a 2020 2020 6465 6361 795f  se``..    decay_
+00009f10: 616d 706c 6974 7564 6573 2c20 6172 7261  amplitudes, arra
+00009f20: 795f 6c69 6b65 2c20 7368 6170 6520 285b  y_like, shape ([
+00009f30: 5b6e 5f70 6c73 2c20 6e5f 706c 732c 5d20  [n_pls, n_pls,] 
+00009f40: 6e5f 6e6f 7073 2c5d 206e 5f6e 6f70 732c  n_nops,] n_nops,
+00009f50: 2064 2a2a 322c 2064 2a2a 3229 2c20 6f70   d**2, d**2), op
+00009f60: 7469 6f6e 616c 0a20 2020 2020 2020 2041  tional.        A
+00009f70: 2070 7265 636f 6d70 7574 6564 2063 756d   precomputed cum
+00009f80: 756c 616e 7420 6675 6e63 7469 6f6e 2e20  ulant function. 
+00009f90: 4966 2067 6976 656e 2c20 2a73 7065 6374  If given, *spect
+00009fa0: 7275 6d2a 2c20 2a6f 6d65 6761 2a0a 2020  rum*, *omega*.  
+00009fb0: 2020 2020 2020 6172 6520 6e6f 7420 7265        are not re
+00009fc0: 7175 6972 6564 2e0a 2020 2020 6672 6571  quired..    freq
+00009fd0: 7565 6e63 795f 7368 6966 7473 2c20 6172  uency_shifts, ar
+00009fe0: 7261 795f 6c69 6b65 2c20 7368 6170 6520  ray_like, shape 
+00009ff0: 285b 5b6e 5f70 6c73 2c20 6e5f 706c 732c  ([[n_pls, n_pls,
+0000a000: 5d20 6e5f 6e6f 7073 2c5d 206e 5f6e 6f70  ] n_nops,] n_nop
+0000a010: 732c 2064 2a2a 322c 2064 2a2a 3229 2c20  s, d**2, d**2), 
+0000a020: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
+0000a030: 2041 2070 7265 636f 6d70 7574 6564 2066   A precomputed f
+0000a040: 7265 7175 656e 6379 2073 6869 6674 2e20  requency shift. 
+0000a050: 4966 2067 6976 656e 2c20 2a73 7065 6374  If given, *spect
+0000a060: 7275 6d2a 2c20 2a6f 6d65 6761 2a0a 2020  rum*, *omega*.  
+0000a070: 2020 2020 2020 6172 6520 6e6f 7420 7265        are not re
+0000a080: 7175 6972 6564 2066 6f72 2073 6563 6f6e  quired for secon
+0000a090: 6420 6f72 6465 7220 7465 726d 732e 0a20  d order terms.. 
+0000a0a0: 2020 2073 686f 775f 7072 6f67 7265 7373     show_progress
+0000a0b0: 6261 723a 2062 6f6f 6c2c 206f 7074 696f  bar: bool, optio
+0000a0c0: 6e61 6c0a 2020 2020 2020 2020 5368 6f77  nal.        Show
+0000a0d0: 2061 2070 726f 6772 6573 7320 6261 7220   a progress bar 
+0000a0e0: 666f 7220 7468 6520 6361 6c63 756c 6174  for the calculat
+0000a0f0: 696f 6e20 6f66 2074 6865 2063 6f6e 7472  ion of the contr
+0000a100: 6f6c 206d 6174 7269 782e 0a20 2020 206d  ol matrix..    m
+0000a110: 656d 6f72 795f 7061 7273 696d 6f6e 696f  emory_parsimonio
+0000a120: 7573 3a20 626f 6f6c 2c20 6f70 7469 6f6e  us: bool, option
+0000a130: 616c 0a20 2020 2020 2020 2054 7261 6465  al.        Trade
+0000a140: 206d 656d 6f72 7920 666f 6f74 7072 696e   memory footprin
+0000a150: 7420 666f 7220 7065 7266 6f72 6d61 6e63  t for performanc
+0000a160: 652e 2053 6565 0a20 2020 2020 2020 203a  e. See.        :
+0000a170: 6675 6e63 3a60 7e6e 756d 6572 6963 2e63  func:`~numeric.c
+0000a180: 616c 6375 6c61 7465 5f64 6563 6179 5f61  alculate_decay_a
+0000a190: 6d70 6c69 7475 6465 7360 2e20 5468 6520  mplitudes`. The 
+0000a1a0: 6465 6661 756c 7420 6973 0a20 2020 2020  default is.     
+0000a1b0: 2020 2060 6046 616c 7365 6060 2e0a 2020     ``False``..  
+0000a1c0: 2020 6361 6368 655f 696e 7465 726d 6564    cache_intermed
+0000a1d0: 6961 7465 733a 2062 6f6f 6c2c 206f 7074  iates: bool, opt
+0000a1e0: 696f 6e61 6c0a 2020 2020 2020 2020 4b65  ional.        Ke
+0000a1f0: 6570 2061 6e64 2072 6574 7572 6e20 696e  ep and return in
+0000a200: 7465 726d 6564 6961 7465 2074 6572 6d73  termediate terms
+0000a210: 206f 6620 7468 6520 6361 6c63 756c 6174   of the calculat
+0000a220: 696f 6e20 6f66 2074 6865 0a20 2020 2020  ion of the.     
+0000a230: 2020 2063 6f6e 7472 6f6c 206d 6174 7269     control matri
+0000a240: 7820 7468 6174 2063 616e 2062 6520 7265  x that can be re
+0000a250: 7573 6564 2069 6e20 6f74 6865 7220 636f  used in other co
+0000a260: 6d70 7574 6174 696f 6e73 2028 7365 636f  mputations (seco
+0000a270: 6e64 0a20 2020 2020 2020 206f 7264 6572  nd.        order
+0000a280: 206f 7220 6772 6164 6965 6e74 7329 2e20   or gradients). 
+0000a290: 4f74 6865 7277 6973 6520 7468 6520 7375  Otherwise the su
+0000a2a0: 6d20 6973 2070 6572 666f 726d 6564 2069  m is performed i
+0000a2b0: 6e2d 706c 6163 652e 0a20 2020 2020 2020  n-place..       
+0000a2c0: 2044 6566 6175 6c74 2069 7320 5472 7565   Default is True
+0000a2d0: 2069 6620 7365 636f 6e64 5f6f 7264 6572   if second_order
+0000a2e0: 3d54 7275 652c 2065 6c73 6520 4661 6c73  =True, else Fals
+0000a2f0: 652e 0a0a 2020 2020 5265 7475 726e 730a  e...    Returns.
+0000a300: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
+0000a310: 6375 6d75 6c61 6e74 5f66 756e 6374 696f  cumulant_functio
+0000a320: 6e3a 206e 6461 7272 6179 2c20 7368 6170  n: ndarray, shap
+0000a330: 6520 285b 5b6e 5f70 6c73 2c20 6e5f 706c  e ([[n_pls, n_pl
+0000a340: 732c 5d20 6e5f 6e6f 7073 2c5d 206e 5f6e  s,] n_nops,] n_n
+0000a350: 6f70 732c 2064 2a2a 322c 2064 2a2a 3229  ops, d**2, d**2)
+0000a360: 0a20 2020 2020 2020 2054 6865 2063 756d  .        The cum
+0000a370: 756c 616e 7420 6675 6e63 7469 6f6e 2e20  ulant function. 
+0000a380: 5468 6520 696e 6469 7669 6475 616c 206e  The individual n
+0000a390: 6f69 7365 206f 7065 7261 746f 720a 2020  oise operator.  
+0000a3a0: 2020 2020 2020 636f 6e74 7269 6275 7469        contributi
+0000a3b0: 6f6e 7320 6368 6f73 656e 2062 7920 6060  ons chosen by ``
+0000a3c0: 6e5f 6f70 6572 5f69 6465 6e74 6966 6965  n_oper_identifie
+0000a3d0: 7273 6060 2061 7265 206f 6e20 7468 6520  rs`` are on the 
+0000a3e0: 7468 6972 640a 2020 2020 2020 2020 746f  third.        to
+0000a3f0: 206c 6173 7420 6178 6973 202f 2061 7865   last axis / axe
+0000a400: 732c 2064 6570 656e 6469 6e67 206f 6e20  s, depending on 
+0000a410: 7768 6574 6865 7220 7468 6520 6e6f 6973  whether the nois
+0000a420: 6520 6973 0a20 2020 2020 2020 2063 726f  e is.        cro
+0000a430: 7373 2d63 6f72 7265 6c61 7465 6420 6f72  ss-correlated or
+0000a440: 206e 6f74 2e20 4966 2060 6077 6869 6368   not. If ``which
+0000a450: 203d 3d20 2763 6f72 7265 6c61 7469 6f6e   == 'correlation
+0000a460: 7327 6060 2c20 7468 650a 2020 2020 2020  s'``, the.      
+0000a470: 2020 6669 7273 7420 7477 6f20 6178 6573    first two axes
+0000a480: 2063 6f72 7265 7370 6f6e 6420 746f 2074   correspond to t
+0000a490: 6865 2063 6f6e 7472 6962 7574 696f 6e73  he contributions
+0000a4a0: 206f 6620 7468 6520 7075 6c73 6573 2069   of the pulses i
+0000a4b0: 6e0a 2020 2020 2020 2020 7468 6520 7365  n.        the se
+0000a4c0: 7175 656e 6365 2e0a 0a20 2020 202e 2e20  quence...    .. 
+0000a4d0: 5f6e 6f74 6573 3a0a 0a20 2020 204e 6f74  _notes:..    Not
+0000a4e0: 6573 0a20 2020 202d 2d2d 2d2d 0a20 2020  es.    -----.   
+0000a4f0: 2054 6865 2063 756d 756c 616e 7420 6675   The cumulant fu
+0000a500: 6e63 7469 6f6e 2069 7320 6769 7665 6e20  nction is given 
+0000a510: 6279 0a0a 2020 2020 2e2e 206d 6174 683a  by..    .. math:
+0000a520: 3a0a 0a20 2020 2020 2020 204b 5f7b 5c61  :..        K_{\a
+0000a530: 6c70 6861 5c62 6574 612c 696a 7d28 5c74  lpha\beta,ij}(\t
+0000a540: 6175 2920 3d20 2d5c 6672 6163 7b31 7d7b  au) = -\frac{1}{
+0000a550: 327d 205c 7375 6d5f 7b6b 6c7d 5c62 6967  2} \sum_{kl}\big
+0000a560: 676c 280a 2020 2020 2020 2020 2020 2020  gl(.            
+0000a570: 265c 4465 6c74 615f 7b5c 616c 7068 615c  &\Delta_{\alpha\
+0000a580: 6265 7461 2c6b 6c7d 5c6c 6566 7428 0a20  beta,kl}\left(. 
+0000a590: 2020 2020 2020 2020 2020 2020 2020 2054                 T
+0000a5a0: 5f7b 6b6c 6a69 7d20 2d20 545f 7b6c 6b6a  _{klji} - T_{lkj
+0000a5b0: 697d 202d 2054 5f7b 6b6c 696a 7d20 2b20  i} - T_{klij} + 
+0000a5c0: 545f 7b6c 6b69 6a7d 0a20 2020 2020 2020  T_{lkij}.       
+0000a5d0: 2020 2020 205c 7269 6768 7429 205c 5c20       \right) \\ 
+0000a5e0: 2b20 265c 4761 6d6d 615f 7b5c 616c 7068  + &\Gamma_{\alph
+0000a5f0: 615c 6265 7461 2c6b 6c7d 5c6c 6566 7428  a\beta,kl}\left(
+0000a600: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a610: 2054 5f7b 6b6c 6a69 7d20 2d20 545f 7b6b   T_{klji} - T_{k
+0000a620: 6a6c 697d 202d 2054 5f7b 6b69 6c6a 7d20  jli} - T_{kilj} 
+0000a630: 2b20 545f 7b6b 696a 6c7d 0a20 2020 2020  + T_{kijl}.     
+0000a640: 2020 2020 2020 205c 7269 6768 7429 0a20         \right). 
+0000a650: 2020 2020 2020 205c 6269 6767 7229 0a0a         \biggr)..
+0000a660: 2020 2020 4865 7265 2c20 3a6d 6174 683a      Here, :math:
+0000a670: 6054 5f7b 696a 6b6c 7d20 3d20 5c6d 6174  `T_{ijkl} = \mat
+0000a680: 6872 6d7b 7472 7d28 435f 6920 435f 6a20  hrm{tr}(C_i C_j 
+0000a690: 435f 6b20 435f 6c29 6020 6973 2061 2074  C_k C_l)` is a t
+0000a6a0: 7269 7669 616c 0a20 2020 2066 756e 6374  rivial.    funct
+0000a6b0: 696f 6e20 6f66 2074 6865 2062 6173 6973  ion of the basis
+0000a6c0: 2065 6c65 6d65 6e74 7320 3a6d 6174 683a   elements :math:
+0000a6d0: 6043 5f69 602c 2061 6e64 0a20 2020 203a  `C_i`, and.    :
+0000a6e0: 6d61 7468 3a60 5c47 616d 6d61 5f7b 5c61  math:`\Gamma_{\a
+0000a6f0: 6c70 6861 5c62 6574 612c 6b6c 7d60 2061  lpha\beta,kl}` a
+0000a700: 6e64 203a 6d61 7468 3a60 5c44 656c 7461  nd :math:`\Delta
+0000a710: 5f7b 5c61 6c70 6861 5c62 6574 612c 6b6c  _{\alpha\beta,kl
+0000a720: 7d60 0a20 2020 2061 7265 2074 6865 2064  }`.    are the d
+0000a730: 6563 6179 2061 6d70 6c69 7475 6465 7320  ecay amplitudes 
+0000a740: 616e 6420 6672 6571 7565 6e63 7920 7368  and frequency sh
+0000a750: 6966 7473 2077 6869 6368 2063 6f72 7265  ifts which corre
+0000a760: 7370 6f6e 6420 746f 0a20 2020 2066 6972  spond to.    fir
+0000a770: 7374 2061 6e64 2073 6563 6f6e 6420 6f72  st and second or
+0000a780: 6465 7220 696e 2074 6865 204d 6167 6e75  der in the Magnu
+0000a790: 7320 6578 7061 6e73 696f 6e2c 2072 6573  s expansion, res
+0000a7a0: 7065 6374 6976 656c 792e 2053 696e 6365  pectively. Since
+0000a7b0: 0a20 2020 2074 6865 206c 6174 7465 7220  .    the latter 
+0000a7c0: 696e 6475 6365 2063 6f68 6572 656e 7420  induce coherent 
+0000a7d0: 6572 726f 7273 2c20 7765 2063 616e 2061  errors, we can a
+0000a7e0: 7070 726f 7869 6d61 7465 6c79 206e 6567  pproximately neg
+0000a7f0: 6c65 6374 2074 6865 6d0a 2020 2020 6966  lect them.    if
+0000a800: 2077 6520 6173 7375 6d65 2074 6861 7420   we assume that 
+0000a810: 7468 6520 7075 6c73 6520 6861 7320 6265  the pulse has be
+0000a820: 656e 2065 7870 6572 696d 656e 7461 6c6c  en experimentall
+0000a830: 7920 6361 6c69 6272 6174 6564 2e0a 0a20  y calibrated... 
+0000a840: 2020 2046 6f72 2061 2073 696e 676c 6520     For a single 
+0000a850: 7175 6269 7420 616e 6420 7265 7072 6573  qubit and repres
+0000a860: 656e 7465 6420 696e 2074 6865 2050 6175  ented in the Pau
+0000a870: 6c69 2062 6173 6973 2c20 7468 6520 6162  li basis, the ab
+0000a880: 6f76 650a 2020 2020 7265 6475 6365 7320  ove.    reduces 
+0000a890: 746f 0a0a 2020 2020 2e2e 206d 6174 683a  to..    .. math:
+0000a8a0: 3a0a 0a20 2020 2020 2020 204b 5f7b 5c61  :..        K_{\a
+0000a8b0: 6c70 6861 5c62 6574 612c 696a 7d28 5c74  lpha\beta,ij}(\t
+0000a8c0: 6175 2920 3d20 5c62 6567 696e 7b63 6173  au) = \begin{cas
+0000a8d0: 6573 7d0a 2020 2020 2020 2020 2020 2020  es}.            
+0000a8e0: 2d20 5c73 756d 5f7b 6b5c 6e65 7120 697d  - \sum_{k\neq i}
+0000a8f0: 5c47 616d 6d61 5f7b 5c61 6c70 6861 5c62  \Gamma_{\alpha\b
+0000a900: 6574 612c 6b6b 7d0a 2020 2020 2020 2020  eta,kk}.        
+0000a910: 2020 2020 2020 2020 265c 7175 6164 5c6d          &\quad\m
+0000a920: 6174 6872 6d7b 6966 7d5c 3a20 6920 3d20  athrm{if}\: i = 
+0000a930: 6a2c 2020 205c 5c0a 2020 2020 2020 2020  j,   \\.        
+0000a940: 2020 2020 2d20 5c44 656c 7461 5f7b 5c61      - \Delta_{\a
+0000a950: 6c70 6861 5c62 6574 612c 696a 7d20 2b20  lpha\beta,ij} + 
+0000a960: 5c44 656c 7461 5f7b 5c61 6c70 6861 5c62  \Delta_{\alpha\b
+0000a970: 6574 612c 6a69 7d0a 2020 2020 2020 2020  eta,ji}.        
+0000a980: 2020 2020 2b20 5c47 616d 6d61 5f7b 5c61      + \Gamma_{\a
+0000a990: 6c70 6861 5c62 6574 612c 696a 7d0a 2020  lpha\beta,ij}.  
+0000a9a0: 2020 2020 2020 2020 2020 2020 2020 265c                &\
+0000a9b0: 7175 6164 5c6d 6174 6872 6d7b 6966 7d5c  quad\mathrm{if}\
+0000a9c0: 3a20 695c 6e65 7120 6a2c 0a20 2020 2020  : i\neq j,.     
+0000a9d0: 2020 205c 656e 647b 6361 7365 737d 0a0a     \end{cases}..
+0000a9e0: 2020 2020 666f 7220 3a6d 6174 683a 6069      for :math:`i
+0000a9f0: 5c69 6e5c 7b31 2c32 2c33 5c7d 6020 616e  \in\{1,2,3\}` an
+0000aa00: 6420 3a6d 6174 683a 604b 5f7b 306a 7d20  d :math:`K_{0j} 
+0000aa10: 3d20 4b5f 7b69 307d 203d 2030 602e 0a0a  = K_{i0} = 0`...
+0000aa20: 2020 2020 4c61 7374 6c79 2c20 7468 6520      Lastly, the 
+0000aa30: 7075 6c73 6520 636f 7272 656c 6174 696f  pulse correlatio
+0000aa40: 6e20 6375 6d75 6c61 6e74 2066 756e 6374  n cumulant funct
+0000aa50: 696f 6e20 7265 736f 6c76 6573 0a20 2020  ion resolves.   
+0000aa60: 2063 6f72 7265 6c61 7469 6f6e 7320 696e   correlations in
+0000aa70: 2074 6865 2063 756d 756c 616e 7420 6675   the cumulant fu
+0000aa80: 6e63 7469 6f6e 206f 6620 6120 7365 7175  nction of a sequ
+0000aa90: 656e 6365 206f 6620 7075 6c73 6573 0a20  ence of pulses. 
+0000aaa0: 2020 203a 6d61 7468 3a60 6720 3d20 312c     :math:`g = 1,
+0000aab0: 5c64 6f74 7363 2c47 6020 7375 6368 2074  \dotsc,G` such t
+0000aac0: 6861 7420 7468 6520 666f 6c6c 6f77 696e  hat the followin
+0000aad0: 6720 686f 6c64 733a 0a0a 2020 2020 2e2e  g holds:..    ..
+0000aae0: 206d 6174 683a 3a0a 0a20 2020 2020 2020   math::..       
+0000aaf0: 204b 5f7b 5c61 6c70 6861 5c62 6574 612c   K_{\alpha\beta,
+0000ab00: 696a 7d28 5c74 6175 2920 3d20 5c73 756d  ij}(\tau) = \sum
+0000ab10: 5f7b 672c 6727 3d31 7d5e 470a 2020 2020  _{g,g'=1}^G.    
+0000ab20: 2020 2020 2020 2020 204b 5f7b 5c61 6c70           K_{\alp
+0000ab30: 6861 5c62 6574 612c 696a 7d5e 7b28 6767  ha\beta,ij}^{(gg
+0000ab40: 2729 7d28 5c74 6175 292e 0a0a 2020 2020  ')}(\tau)...    
+0000ab50: 5365 6520 416c 736f 0a20 2020 202d 2d2d  See Also.    ---
+0000ab60: 2d2d 2d2d 2d0a 2020 2020 6361 6c63 756c  -----.    calcul
+0000ab70: 6174 655f 6465 6361 795f 616d 706c 6974  ate_decay_amplit
+0000ab80: 7564 6573 3a20 4361 6c63 756c 6174 6520  udes: Calculate 
+0000ab90: 7468 6520 3a6d 6174 683a 605c 4761 6d6d  the :math:`\Gamm
+0000aba0: 615f 7b5c 616c 7068 615c 6265 7461 2c6b  a_{\alpha\beta,k
+0000abb0: 6c7d 600a 2020 2020 6572 726f 725f 7472  l}`.    error_tr
+0000abc0: 616e 7366 6572 5f6d 6174 7269 783a 2043  ansfer_matrix: C
+0000abd0: 616c 6375 6c61 7465 2074 6865 2065 7272  alculate the err
+0000abe0: 6f72 2074 7261 6e73 6665 7220 6d61 7472  or transfer matr
+0000abf0: 6978 203a 6d61 7468 3a60 5c65 7870 5c6d  ix :math:`\exp\m
+0000ac00: 6174 6863 616c 7b4b 7d60 2e0a 2020 2020  athcal{K}`..    
+0000ac10: 696e 6669 6465 6c69 7479 3a20 4361 6c63  infidelity: Calc
+0000ac20: 756c 6174 6520 6f6e 6c79 2069 6e66 6964  ulate only infid
+0000ac30: 656c 6974 7920 6f66 2061 2070 756c 7365  elity of a pulse
+0000ac40: 2e0a 2020 2020 7075 6c73 655f 7365 7175  ..    pulse_sequ
+0000ac50: 656e 6365 2e63 6f6e 6361 7465 6e61 7465  ence.concatenate
+0000ac60: 3a20 436f 6e63 6174 656e 6174 6520 6060  : Concatenate ``
+0000ac70: 5075 6c73 6553 6571 7565 6e63 6560 6020  PulseSequence`` 
+0000ac80: 6f62 6a65 6374 732e 0a20 2020 2063 616c  objects..    cal
+0000ac90: 6375 6c61 7465 5f70 756c 7365 5f63 6f72  culate_pulse_cor
+0000aca0: 7265 6c61 7469 6f6e 5f66 696c 7465 725f  relation_filter_
+0000acb0: 6675 6e63 7469 6f6e 0a0a 2020 2020 2222  function..    ""
+0000acc0: 220a 2020 2020 4e2c 2064 203d 2070 756c  ".    N, d = pul
+0000acd0: 7365 2e62 6173 6973 2e73 6861 7065 5b3a  se.basis.shape[:
+0000ace0: 325d 0a20 2020 2069 6620 7370 6563 7472  2].    if spectr
+0000acf0: 756d 2069 7320 4e6f 6e65 2061 6e64 206f  um is None and o
+0000ad00: 6d65 6761 2069 7320 4e6f 6e65 3a0a 2020  mega is None:.  
+0000ad10: 2020 2020 2020 6966 2064 6563 6179 5f61        if decay_a
+0000ad20: 6d70 6c69 7475 6465 7320 6973 204e 6f6e  mplitudes is Non
+0000ad30: 6520 6f72 2028 6672 6571 7565 6e63 795f  e or (frequency_
+0000ad40: 7368 6966 7473 2069 7320 4e6f 6e65 2061  shifts is None a
+0000ad50: 6e64 2073 6563 6f6e 645f 6f72 6465 7229  nd second_order)
+0000ad60: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+0000ad70: 6973 6520 5661 6c75 6545 7272 6f72 2827  ise ValueError('
+0000ad80: 5265 7175 6972 6520 6569 7468 6572 2073  Require either s
+0000ad90: 7065 6374 7275 6d20 616e 6420 6672 6571  pectrum and freq
+0000ada0: 7565 6e63 6965 7320 6f72 2070 7265 636f  uencies or preco
+0000adb0: 6d70 7574 6564 2027 0a20 2020 2020 2020  mputed '.       
+0000adc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000add0: 2020 2020 2020 2b20 2764 6563 6179 2061        + 'decay a
+0000ade0: 6d70 6c69 7475 6465 7320 2866 7265 7175  mplitudes (frequ
+0000adf0: 656e 6379 2073 6869 6674 7329 2729 0a0a  ency shifts)')..
+0000ae00: 2020 2020 6966 2077 6869 6368 203d 3d20      if which == 
+0000ae10: 2763 6f72 7265 6c61 7469 6f6e 7327 2061  'correlations' a
+0000ae20: 6e64 2073 6563 6f6e 645f 6f72 6465 723a  nd second_order:
+0000ae30: 0a20 2020 2020 2020 2072 6169 7365 2056  .        raise V
+0000ae40: 616c 7565 4572 726f 7228 2743 616e 6e6f  alueError('Canno
+0000ae50: 7420 636f 6d70 7574 6520 636f 7272 656c  t compute correl
+0000ae60: 6174 696f 6e20 6375 6d75 6c61 6e74 2066  ation cumulant f
+0000ae70: 756e 6374 696f 6e20 666f 7220 7365 636f  unction for seco
+0000ae80: 6e64 206f 7264 6572 2074 6572 6d73 2729  nd order terms')
+0000ae90: 0a0a 2020 2020 6966 2063 6163 6865 5f69  ..    if cache_i
+0000aea0: 6e74 6572 6d65 6469 6174 6573 2069 7320  ntermediates is 
+0000aeb0: 4e6f 6e65 3a0a 2020 2020 2020 2020 6361  None:.        ca
+0000aec0: 6368 655f 696e 7465 726d 6564 6961 7465  che_intermediate
+0000aed0: 7320 3d20 7365 636f 6e64 5f6f 7264 6572  s = second_order
+0000aee0: 0a0a 2020 2020 6966 2064 6563 6179 5f61  ..    if decay_a
+0000aef0: 6d70 6c69 7475 6465 7320 6973 204e 6f6e  mplitudes is Non
+0000af00: 653a 0a20 2020 2020 2020 2064 6563 6179  e:.        decay
+0000af10: 5f61 6d70 6c69 7475 6465 7320 3d20 6361  _amplitudes = ca
+0000af20: 6c63 756c 6174 655f 6465 6361 795f 616d  lculate_decay_am
+0000af30: 706c 6974 7564 6573 2870 756c 7365 2c20  plitudes(pulse, 
+0000af40: 7370 6563 7472 756d 2c20 6f6d 6567 612c  spectrum, omega,
+0000af50: 206e 5f6f 7065 725f 6964 656e 7469 6669   n_oper_identifi
+0000af60: 6572 732c 0a20 2020 2020 2020 2020 2020  ers,.           
+0000af70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000af80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000af90: 2020 2020 2020 2020 2020 2077 6869 6368             which
+0000afa0: 2c20 7368 6f77 5f70 726f 6772 6573 7362  , show_progressb
+0000afb0: 6172 2c20 6361 6368 655f 696e 7465 726d  ar, cache_interm
+0000afc0: 6564 6961 7465 732c 0a20 2020 2020 2020  ediates,.       
+0000afd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000afe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aff0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+0000b000: 656d 6f72 795f 7061 7273 696d 6f6e 696f  emory_parsimonio
+0000b010: 7573 290a 0a20 2020 2069 6620 7365 636f  us)..    if seco
+0000b020: 6e64 5f6f 7264 6572 3a0a 2020 2020 2020  nd_order:.      
+0000b030: 2020 6966 2066 7265 7175 656e 6379 5f73    if frequency_s
+0000b040: 6869 6674 7320 6973 204e 6f6e 653a 0a20  hifts is None:. 
+0000b050: 2020 2020 2020 2020 2020 2069 6620 6d65             if me
+0000b060: 6d6f 7279 5f70 6172 7369 6d6f 6e69 6f75  mory_parsimoniou
+0000b070: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+0000b080: 2020 2077 6172 6e28 274d 656d 6f72 7920     warn('Memory 
+0000b090: 7061 7273 696d 6f6e 696f 7573 2063 616c  parsimonious cal
+0000b0a0: 6375 6c61 7469 6f6e 206e 6f74 2069 6d70  culation not imp
+0000b0b0: 6c65 6d65 6e74 6564 2066 6f72 2066 7265  lemented for fre
+0000b0c0: 7175 656e 6379 2073 6869 6674 732e 2729  quency shifts.')
+0000b0d0: 0a0a 2020 2020 2020 2020 2020 2020 6672  ..            fr
+0000b0e0: 6571 7565 6e63 795f 7368 6966 7473 203d  equency_shifts =
+0000b0f0: 2063 616c 6375 6c61 7465 5f66 7265 7175   calculate_frequ
+0000b100: 656e 6379 5f73 6869 6674 7328 7075 6c73  ency_shifts(puls
+0000b110: 652c 2073 7065 6374 7275 6d2c 206f 6d65  e, spectrum, ome
+0000b120: 6761 2c0a 2020 2020 2020 2020 2020 2020  ga,.            
+0000b130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b150: 2020 2020 2020 2020 2020 2020 2020 6e5f                n_
+0000b160: 6f70 6572 5f69 6465 6e74 6966 6965 7273  oper_identifiers
+0000b170: 2c20 7368 6f77 5f70 726f 6772 6573 7362  , show_progressb
+0000b180: 6172 290a 0a20 2020 2020 2020 2069 6620  ar)..        if 
+0000b190: 6672 6571 7565 6e63 795f 7368 6966 7473  frequency_shifts
+0000b1a0: 2e73 6861 7065 2021 3d20 6465 6361 795f  .shape != decay_
+0000b1b0: 616d 706c 6974 7564 6573 2e73 6861 7065  amplitudes.shape
+0000b1c0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+0000b1d0: 6973 6520 5661 6c75 6545 7272 6f72 2827  ise ValueError('
+0000b1e0: 4672 6571 7565 6e63 7920 7368 6966 7473  Frequency shifts
+0000b1f0: 206e 6f74 2073 616d 6520 7368 6170 6520   not same shape 
+0000b200: 6173 2064 6563 6179 2061 6d70 6c69 7475  as decay amplitu
+0000b210: 6465 7327 290a 0a20 2020 2069 6620 6420  des')..    if d 
+0000b220: 3d3d 2032 2061 6e64 2070 756c 7365 2e62  == 2 and pulse.b
+0000b230: 6173 6973 2e62 7479 7065 2069 6e20 2827  asis.btype in ('
+0000b240: 5061 756c 6927 2c20 2747 474d 2729 3a0a  Pauli', 'GGM'):.
+0000b250: 2020 2020 2020 2020 2320 5369 6e67 6c65          # Single
+0000b260: 2071 7562 6974 2063 6173 652e 2043 616e   qubit case. Can
+0000b270: 2075 7365 2073 696d 706c 6966 6965 6420   use simplified 
+0000b280: 6578 7072 6573 7369 6f6e 0a20 2020 2020  expression.     
+0000b290: 2020 2063 756d 756c 616e 745f 6675 6e63     cumulant_func
+0000b2a0: 7469 6f6e 203d 206e 702e 7a65 726f 7328  tion = np.zeros(
+0000b2b0: 6465 6361 795f 616d 706c 6974 7564 6573  decay_amplitudes
+0000b2c0: 2e73 6861 7065 2c20 6465 6361 795f 616d  .shape, decay_am
+0000b2d0: 706c 6974 7564 6573 2e64 7479 7065 290a  plitudes.dtype).
+0000b2e0: 2020 2020 2020 2020 6469 6167 5f6d 6173          diag_mas
+0000b2f0: 6b20 3d20 6e70 2e7a 6572 6f73 2828 4e2c  k = np.zeros((N,
+0000b300: 204e 292c 2064 7479 7065 3d62 6f6f 6c29   N), dtype=bool)
+0000b310: 0a20 2020 2020 2020 2064 6961 675f 6d61  .        diag_ma
+0000b320: 736b 5b31 3a2c 2031 3a5d 203d 207e 6e70  sk[1:, 1:] = ~np
+0000b330: 2e65 7965 284e 2d31 2c20 6474 7970 653d  .eye(N-1, dtype=
+0000b340: 626f 6f6c 290a 0a20 2020 2020 2020 2023  bool)..        #
+0000b350: 204f 6666 6469 6167 6f6e 616c 2074 6572   Offdiagonal ter
+0000b360: 6d73 0a20 2020 2020 2020 2063 756d 756c  ms.        cumul
+0000b370: 616e 745f 6675 6e63 7469 6f6e 5b2e 2e2e  ant_function[...
+0000b380: 2c20 6469 6167 5f6d 6173 6b5d 203d 2064  , diag_mask] = d
+0000b390: 6563 6179 5f61 6d70 6c69 7475 6465 735b  ecay_amplitudes[
+0000b3a0: 2e2e 2e2c 2064 6961 675f 6d61 736b 5d0a  ..., diag_mask].
+0000b3b0: 0a20 2020 2020 2020 2023 2044 6961 676f  .        # Diago
+0000b3c0: 6e61 6c20 7465 726d 7320 4b5f 6969 2067  nal terms K_ii g
+0000b3d0: 6976 656e 2062 7920 7375 6d20 6f76 6572  iven by sum over
+0000b3e0: 2064 6961 676f 6e61 6c20 6f66 2047 616d   diagonal of Gam
+0000b3f0: 6d61 2065 7863 6c75 6469 6e67 0a20 2020  ma excluding.   
+0000b400: 2020 2020 2023 2047 616d 6d61 5f69 692e       # Gamma_ii.
+0000b410: 2053 696e 6365 2074 6865 2050 6175 6c69   Since the Pauli
+0000b420: 2062 6173 6973 2069 7320 7472 6163 656c   basis is tracel
+0000b430: 6573 732c 204b 5f30 3020 6973 207a 6572  ess, K_00 is zer
+0000b440: 6f2c 2074 6865 7265 666f 7265 0a20 2020  o, therefore.   
+0000b450: 2020 2020 2023 2073 7461 7274 2061 7420       # start at 
+0000b460: 4b5f 3131 2e0a 2020 2020 2020 2020 6469  K_11..        di
+0000b470: 6167 5f64 6571 7565 203d 2064 6571 7565  ag_deque = deque
+0000b480: 2828 4661 6c73 652c 2054 7275 652c 2054  ((False, True, T
+0000b490: 7275 6529 290a 2020 2020 2020 2020 666f  rue)).        fo
+0000b4a0: 7220 6920 696e 2072 616e 6765 2831 2c20  r i in range(1, 
+0000b4b0: 4e29 3a0a 2020 2020 2020 2020 2020 2020  N):.            
+0000b4c0: 6469 6167 5f69 6478 203d 205b 4661 6c73  diag_idx = [Fals
+0000b4d0: 655d 202b 206c 6973 7428 6469 6167 5f64  e] + list(diag_d
+0000b4e0: 6571 7565 290a 2020 2020 2020 2020 2020  eque).          
+0000b4f0: 2020 6375 6d75 6c61 6e74 5f66 756e 6374    cumulant_funct
+0000b500: 696f 6e5b 2e2e 2e2c 2069 2c20 695d 203d  ion[..., i, i] =
+0000b510: 202d 6465 6361 795f 616d 706c 6974 7564   -decay_amplitud
+0000b520: 6573 5b2e 2e2e 2c20 6469 6167 5f69 6478  es[..., diag_idx
+0000b530: 2c20 6469 6167 5f69 6478 5d2e 7375 6d28  , diag_idx].sum(
+0000b540: 6178 6973 3d2d 3129 0a20 2020 2020 2020  axis=-1).       
+0000b550: 2020 2020 2023 2073 6869 6674 2074 6865       # shift the
+0000b560: 2069 7465 6d20 6e6f 7420 7375 6d6d 6564   item not summed
+0000b570: 206f 7665 7220 6279 206f 6e65 0a20 2020   over by one.   
+0000b580: 2020 2020 2020 2020 2064 6961 675f 6465           diag_de
+0000b590: 7175 652e 726f 7461 7465 2829 0a0a 2020  que.rotate()..  
+0000b5a0: 2020 2020 2020 6966 2073 6563 6f6e 645f        if second_
+0000b5b0: 6f72 6465 723a 0a20 2020 2020 2020 2020  order:.         
+0000b5c0: 2020 2063 756d 756c 616e 745f 6675 6e63     cumulant_func
+0000b5d0: 7469 6f6e 5b2e 2e2e 2c20 313a 2c20 313a  tion[..., 1:, 1:
+0000b5e0: 5d20 2d3d 2066 7265 7175 656e 6379 5f73  ] -= frequency_s
+0000b5f0: 6869 6674 735b 2e2e 2e2c 2031 3a2c 2031  hifts[..., 1:, 1
+0000b600: 3a5d 0a20 2020 2020 2020 2020 2020 2063  :].            c
+0000b610: 756d 756c 616e 745f 6675 6e63 7469 6f6e  umulant_function
+0000b620: 5b2e 2e2e 2c20 313a 2c20 313a 5d20 2b3d  [..., 1:, 1:] +=
+0000b630: 2066 7265 7175 656e 6379 5f73 6869 6674   frequency_shift
+0000b640: 735b 2e2e 2e2c 2031 3a2c 2031 3a5d 2e73  s[..., 1:, 1:].s
+0000b650: 7761 7061 7865 7328 2d31 2c20 2d32 290a  wapaxes(-1, -2).
+0000b660: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000b670: 2020 2320 4d75 6c74 6920 7175 6269 7420    # Multi qubit 
+0000b680: 6361 7365 2e20 5573 6520 6765 6e65 7261  case. Use genera
+0000b690: 6c20 6578 7072 6573 7369 6f6e 2e20 4472  l expression. Dr
+0000b6a0: 6f70 2069 6d61 6769 6e61 7279 2070 6172  op imaginary par
+0000b6b0: 7420 7369 6e63 650a 2020 2020 2020 2020  t since.        
+0000b6c0: 2320 7265 7375 6c74 2069 7320 6775 6172  # result is guar
+0000b6d0: 616e 7465 6564 2074 6f20 6265 2072 6561  anteed to be rea
+0000b6e0: 6c20 2869 6620 7765 2064 6964 6e27 7420  l (if we didn't 
+0000b6f0: 646f 2061 6e79 7468 696e 6720 7772 6f6e  do anything wron
+0000b700: 6729 0a20 2020 2020 2020 2074 7261 6365  g).        trace
+0000b710: 7320 3d20 7075 6c73 652e 6261 7369 732e  s = pulse.basis.
+0000b720: 666f 7572 5f65 6c65 6d65 6e74 5f74 7261  four_element_tra
+0000b730: 6365 730a 2020 2020 2020 2020 6375 6d75  ces.        cumu
+0000b740: 6c61 6e74 5f66 756e 6374 696f 6e20 3d20  lant_function = 
+0000b750: 2d20 280a 2020 2020 2020 2020 2020 2020  - (.            
+0000b760: 2b20 6f65 2e63 6f6e 7472 6163 7428 272e  + oe.contract('.
+0000b770: 2e2e 6b6c 2c6b 6c6a 692d 3e2e 2e2e 696a  ..kl,klji->...ij
+0000b780: 272c 2064 6563 6179 5f61 6d70 6c69 7475  ', decay_amplitu
+0000b790: 6465 732c 2074 7261 6365 732c 2062 6163  des, traces, bac
+0000b7a0: 6b65 6e64 3d27 7370 6172 7365 2729 0a20  kend='sparse'). 
+0000b7b0: 2020 2020 2020 2020 2020 202d 206f 652e             - oe.
+0000b7c0: 636f 6e74 7261 6374 2827 2e2e 2e6b 6c2c  contract('...kl,
+0000b7d0: 6b6a 6c69 2d3e 2e2e 2e69 6a27 2c20 6465  kjli->...ij', de
+0000b7e0: 6361 795f 616d 706c 6974 7564 6573 2c20  cay_amplitudes, 
+0000b7f0: 7472 6163 6573 2c20 6261 636b 656e 643d  traces, backend=
+0000b800: 2773 7061 7273 6527 290a 2020 2020 2020  'sparse').      
+0000b810: 2020 2020 2020 2d20 6f65 2e63 6f6e 7472        - oe.contr
+0000b820: 6163 7428 272e 2e2e 6b6c 2c6b 696c 6a2d  act('...kl,kilj-
+0000b830: 3e2e 2e2e 696a 272c 2064 6563 6179 5f61  >...ij', decay_a
+0000b840: 6d70 6c69 7475 6465 732c 2074 7261 6365  mplitudes, trace
+0000b850: 732c 2062 6163 6b65 6e64 3d27 7370 6172  s, backend='spar
+0000b860: 7365 2729 0a20 2020 2020 2020 2020 2020  se').           
+0000b870: 202b 206f 652e 636f 6e74 7261 6374 2827   + oe.contract('
+0000b880: 2e2e 2e6b 6c2c 6b69 6a6c 2d3e 2e2e 2e69  ...kl,kijl->...i
+0000b890: 6a27 2c20 6465 6361 795f 616d 706c 6974  j', decay_amplit
+0000b8a0: 7564 6573 2c20 7472 6163 6573 2c20 6261  udes, traces, ba
+0000b8b0: 636b 656e 643d 2773 7061 7273 6527 290a  ckend='sparse').
+0000b8c0: 2020 2020 2020 2020 2920 2f20 320a 2020          ) / 2.  
+0000b8d0: 2020 2020 2020 6966 2073 6563 6f6e 645f        if second_
+0000b8e0: 6f72 6465 723a 0a20 2020 2020 2020 2020  order:.         
+0000b8f0: 2020 2063 756d 756c 616e 745f 6675 6e63     cumulant_func
+0000b900: 7469 6f6e 202d 3d20 280a 2020 2020 2020  tion -= (.      
+0000b910: 2020 2020 2020 2020 2020 2b20 6f65 2e63            + oe.c
+0000b920: 6f6e 7472 6163 7428 272e 2e2e 6b6c 2c6b  ontract('...kl,k
+0000b930: 6c6a 692d 3e2e 2e2e 696a 272c 2066 7265  lji->...ij', fre
+0000b940: 7175 656e 6379 5f73 6869 6674 732c 2074  quency_shifts, t
+0000b950: 7261 6365 732c 2062 6163 6b65 6e64 3d27  races, backend='
+0000b960: 7370 6172 7365 2729 0a20 2020 2020 2020  sparse').       
+0000b970: 2020 2020 2020 2020 202d 206f 652e 636f           - oe.co
+0000b980: 6e74 7261 6374 2827 2e2e 2e6b 6c2c 6c6b  ntract('...kl,lk
+0000b990: 6a69 2d3e 2e2e 2e69 6a27 2c20 6672 6571  ji->...ij', freq
+0000b9a0: 7565 6e63 795f 7368 6966 7473 2c20 7472  uency_shifts, tr
+0000b9b0: 6163 6573 2c20 6261 636b 656e 643d 2773  aces, backend='s
+0000b9c0: 7061 7273 6527 290a 2020 2020 2020 2020  parse').        
+0000b9d0: 2020 2020 2020 2020 2d20 6f65 2e63 6f6e          - oe.con
+0000b9e0: 7472 6163 7428 272e 2e2e 6b6c 2c6b 6c69  tract('...kl,kli
+0000b9f0: 6a2d 3e2e 2e2e 696a 272c 2066 7265 7175  j->...ij', frequ
+0000ba00: 656e 6379 5f73 6869 6674 732c 2074 7261  ency_shifts, tra
+0000ba10: 6365 732c 2062 6163 6b65 6e64 3d27 7370  ces, backend='sp
+0000ba20: 6172 7365 2729 0a20 2020 2020 2020 2020  arse').         
+0000ba30: 2020 2020 2020 202b 206f 652e 636f 6e74         + oe.cont
+0000ba40: 7261 6374 2827 2e2e 2e6b 6c2c 6c6b 696a  ract('...kl,lkij
+0000ba50: 2d3e 2e2e 2e69 6a27 2c20 6672 6571 7565  ->...ij', freque
+0000ba60: 6e63 795f 7368 6966 7473 2c20 7472 6163  ncy_shifts, trac
+0000ba70: 6573 2c20 6261 636b 656e 643d 2773 7061  es, backend='spa
+0000ba80: 7273 6527 290a 2020 2020 2020 2020 2020  rse').          
+0000ba90: 2020 2920 2f20 320a 0a20 2020 2072 6574    ) / 2..    ret
+0000baa0: 7572 6e20 6375 6d75 6c61 6e74 5f66 756e  urn cumulant_fun
+0000bab0: 6374 696f 6e2e 7265 616c 0a0a 0a40 7574  ction.real...@ut
+0000bac0: 696c 2e70 6172 7365 5f6f 7074 696f 6e61  il.parse_optiona
+0000bad0: 6c5f 7061 7261 6d65 7465 7273 2877 6869  l_parameters(whi
+0000bae0: 6368 3d28 2774 6f74 616c 272c 2027 636f  ch=('total', 'co
+0000baf0: 7272 656c 6174 696f 6e73 2729 290a 6465  rrelations')).de
+0000bb00: 6620 6361 6c63 756c 6174 655f 6465 6361  f calculate_deca
+0000bb10: 795f 616d 706c 6974 7564 6573 280a 2020  y_amplitudes(.  
+0000bb20: 2020 2020 2020 7075 6c73 653a 2027 5075        pulse: 'Pu
+0000bb30: 6c73 6553 6571 7565 6e63 6527 2c0a 2020  lseSequence',.  
+0000bb40: 2020 2020 2020 7370 6563 7472 756d 3a20        spectrum: 
+0000bb50: 6e64 6172 7261 792c 0a20 2020 2020 2020  ndarray,.       
+0000bb60: 206f 6d65 6761 3a20 436f 6566 6669 6369   omega: Coeffici
+0000bb70: 656e 7473 2c0a 2020 2020 2020 2020 6e5f  ents,.        n_
+0000bb80: 6f70 6572 5f69 6465 6e74 6966 6965 7273  oper_identifiers
+0000bb90: 3a20 4f70 7469 6f6e 616c 5b53 6571 7565  : Optional[Seque
+0000bba0: 6e63 655b 7374 725d 5d20 3d20 4e6f 6e65  nce[str]] = None
+0000bbb0: 2c0a 2020 2020 2020 2020 7768 6963 683a  ,.        which:
+0000bbc0: 2073 7472 203d 2027 746f 7461 6c27 2c0a   str = 'total',.
+0000bbd0: 2020 2020 2020 2020 7368 6f77 5f70 726f          show_pro
+0000bbe0: 6772 6573 7362 6172 3a20 626f 6f6c 203d  gressbar: bool =
+0000bbf0: 2046 616c 7365 2c0a 2020 2020 2020 2020   False,.        
+0000bc00: 6361 6368 655f 696e 7465 726d 6564 6961  cache_intermedia
+0000bc10: 7465 733a 2062 6f6f 6c20 3d20 4661 6c73  tes: bool = Fals
+0000bc20: 652c 0a20 2020 2020 2020 206d 656d 6f72  e,.        memor
+0000bc30: 795f 7061 7273 696d 6f6e 696f 7573 3a20  y_parsimonious: 
+0000bc40: 626f 6f6c 203d 2046 616c 7365 0a29 202d  bool = False.) -
+0000bc50: 3e20 6e64 6172 7261 793a 0a20 2020 2072  > ndarray:.    r
+0000bc60: 2222 220a 2020 2020 4765 7420 7468 6520  """.    Get the 
+0000bc70: 6465 6361 7920 616d 706c 6974 7564 6573  decay amplitudes
+0000bc80: 203a 6d61 7468 3a60 5c47 616d 6d61 5f7b   :math:`\Gamma_{
+0000bc90: 5c61 6c70 6861 5c62 6574 612c 206b 6c7d  \alpha\beta, kl}
+0000bca0: 6020 666f 7220 6e6f 6973 650a 2020 2020  ` for noise.    
+0000bcb0: 736f 7572 6365 7320 3a6d 6174 683a 605c  sources :math:`\
+0000bcc0: 616c 7068 612c 5c62 6574 6160 2061 6e64  alpha,\beta` and
+0000bcd0: 2062 6173 6973 2065 6c65 6d65 6e74 7320   basis elements 
+0000bce0: 3a6d 6174 683a 606b 2c6c 602e 0a0a 2020  :math:`k,l`...  
+0000bcf0: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+0000bd00: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+0000bd10: 7075 6c73 653a 2050 756c 7365 5365 7175  pulse: PulseSequ
+0000bd20: 656e 6365 0a20 2020 2020 2020 2054 6865  ence.        The
+0000bd30: 2060 6050 756c 7365 5365 7175 656e 6365   ``PulseSequence
+0000bd40: 6060 2069 6e73 7461 6e63 6520 666f 7220  `` instance for 
+0000bd50: 7768 6963 6820 746f 2063 6f6d 7075 7465  which to compute
+0000bd60: 2074 6865 2064 6563 6179 0a20 2020 2020   the decay.     
+0000bd70: 2020 2061 6d70 6c69 7475 6465 732e 0a20     amplitudes.. 
+0000bd80: 2020 2073 7065 6374 7275 6d3a 2061 7272     spectrum: arr
+0000bd90: 6179 5f6c 696b 652c 2073 6861 7065 2028  ay_like, shape (
+0000bda0: 5b5b 6e5f 6e6f 7073 2c5d 206e 5f6e 6f70  [[n_nops,] n_nop
+0000bdb0: 732c 5d20 6e5f 6f6d 6567 6129 0a20 2020  s,] n_omega).   
+0000bdc0: 2020 2020 2054 6865 206e 6f69 7365 2070       The noise p
+0000bdd0: 6f77 6572 2073 7065 6374 7261 6c20 6465  ower spectral de
+0000bde0: 6e73 6974 792e 2049 6620 312d 642c 2074  nsity. If 1-d, t
+0000bdf0: 6865 2073 616d 6520 7370 6563 7472 756d  he same spectrum
+0000be00: 2069 730a 2020 2020 2020 2020 7573 6564   is.        used
+0000be10: 2066 6f72 2061 6c6c 206e 6f69 7365 206f   for all noise o
+0000be20: 7065 7261 746f 7273 2e20 4966 2032 2d64  perators. If 2-d
+0000be30: 2c20 6f6e 6520 2873 656c 662d 2920 7370  , one (self-) sp
+0000be40: 6563 7472 756d 2066 6f72 0a20 2020 2020  ectrum for.     
+0000be50: 2020 2065 6163 6820 6e6f 6973 6520 6f70     each noise op
+0000be60: 6572 6174 6f72 2069 7320 6578 7065 6374  erator is expect
+0000be70: 6564 2e20 4966 2033 2d64 2c20 7368 6f75  ed. If 3-d, shou
+0000be80: 6c64 2062 6520 6120 6d61 7472 6978 206f  ld be a matrix o
+0000be90: 660a 2020 2020 2020 2020 6372 6f73 732d  f.        cross-
+0000bea0: 7370 6563 7472 6120 7375 6368 2074 6861  spectra such tha
+0000beb0: 740a 2020 2020 2020 2020 6060 7370 6563  t.        ``spec
+0000bec0: 7472 756d 5b69 2c20 6a5d 203d 3d20 7370  trum[i, j] == sp
+0000bed0: 6563 7472 756d 5b6a 2c20 695d 2e63 6f6e  ectrum[j, i].con
+0000bee0: 6a28 2960 602e 0a20 2020 206f 6d65 6761  j()``..    omega
+0000bef0: 3a20 6172 7261 795f 6c69 6b65 2c0a 2020  : array_like,.  
+0000bf00: 2020 2020 2020 5468 6520 6672 6571 7565        The freque
+0000bf10: 6e63 6965 7320 6174 2077 6869 6368 2074  ncies at which t
+0000bf20: 6f20 6361 6c63 756c 6174 6520 7468 6520  o calculate the 
+0000bf30: 6669 6c74 6572 2066 756e 6374 696f 6e73  filter functions
+0000bf40: 2e0a 2020 2020 6e5f 6f70 6572 5f69 6465  ..    n_oper_ide
+0000bf50: 6e74 6966 6965 7273 3a20 6172 7261 795f  ntifiers: array_
+0000bf60: 6c69 6b65 2c20 6f70 7469 6f6e 616c 0a20  like, optional. 
+0000bf70: 2020 2020 2020 2054 6865 2069 6465 6e74         The ident
+0000bf80: 6966 6965 7273 206f 6620 7468 6520 6e6f  ifiers of the no
+0000bf90: 6973 6520 6f70 6572 6174 6f72 7320 666f  ise operators fo
+0000bfa0: 7220 7768 6963 6820 746f 2063 616c 6375  r which to calcu
+0000bfb0: 6c61 7465 0a20 2020 2020 2020 2074 6865  late.        the
+0000bfc0: 2064 6563 6179 2061 6d70 6c69 7475 6465   decay amplitude
+0000bfd0: 732e 2054 6865 2064 6566 6175 6c74 2069  s. The default i
+0000bfe0: 7320 616c 6c2e 0a20 2020 2077 6869 6368  s all..    which
+0000bff0: 3a20 7374 722c 206f 7074 696f 6e61 6c0a  : str, optional.
+0000c000: 2020 2020 2020 2020 5768 6963 6820 6465          Which de
+0000c010: 6361 7920 616d 706c 6974 7564 6573 2073  cay amplitudes s
+0000c020: 686f 756c 6420 6265 2063 616c 6375 6c61  hould be calcula
+0000c030: 7465 642c 206d 6179 2062 6520 6569 7468  ted, may be eith
+0000c040: 6572 0a20 2020 2020 2020 2027 746f 7461  er.        'tota
+0000c050: 6c27 2028 6465 6661 756c 7429 206f 7220  l' (default) or 
+0000c060: 2763 6f72 7265 6c61 7469 6f6e 7327 2e20  'correlations'. 
+0000c070: 5365 6520 3a66 756e 633a 6069 6e66 6964  See :func:`infid
+0000c080: 656c 6974 7960 2061 6e64 0a20 2020 2020  elity` and.     
+0000c090: 2020 203a 7265 663a 604e 6f74 6573 203c     :ref:`Notes <
+0000c0a0: 6e6f 7465 733e 602e 0a20 2020 2073 686f  notes>`..    sho
+0000c0b0: 775f 7072 6f67 7265 7373 6261 723a 2062  w_progressbar: b
+0000c0c0: 6f6f 6c2c 206f 7074 696f 6e61 6c0a 2020  ool, optional.  
+0000c0d0: 2020 2020 2020 5368 6f77 2061 2070 726f        Show a pro
+0000c0e0: 6772 6573 7320 6261 7220 666f 7220 7468  gress bar for th
+0000c0f0: 6520 6361 6c63 756c 6174 696f 6e2e 0a20  e calculation.. 
+0000c100: 2020 2063 6163 6865 5f69 6e74 6572 6d65     cache_interme
+0000c110: 6469 6174 6573 3a20 626f 6f6c 2c20 6f70  diates: bool, op
+0000c120: 7469 6f6e 616c 0a20 2020 2020 2020 204b  tional.        K
+0000c130: 6565 7020 616e 6420 7265 7475 726e 2069  eep and return i
+0000c140: 6e74 6572 6d65 6469 6174 6520 7465 726d  ntermediate term
+0000c150: 7320 6f66 2074 6865 2063 616c 6375 6c61  s of the calcula
+0000c160: 7469 6f6e 2074 6861 7420 6172 650a 2020  tion that are.  
+0000c170: 2020 2020 2020 7573 6566 756c 2069 6e20        useful in 
+0000c180: 6f74 6865 7220 706c 6163 6573 2028 6966  other places (if
+0000c190: 2063 6f6e 7472 6f6c 206d 6174 7269 7820   control matrix 
+0000c1a0: 6e6f 7420 616c 7265 6164 7920 6361 6368  not already cach
+0000c1b0: 6564 292e 0a20 2020 206d 656d 6f72 795f  ed)..    memory_
+0000c1c0: 7061 7273 696d 6f6e 696f 7573 3a20 626f  parsimonious: bo
+0000c1d0: 6f6c 2c20 6f70 7469 6f6e 616c 0a20 2020  ol, optional.   
+0000c1e0: 2020 2020 2046 6f72 206c 6172 6765 2064       For large d
+0000c1f0: 696d 656e 7369 6f6e 732c 2074 6865 2069  imensions, the i
+0000c200: 6e74 6567 7261 6e64 0a0a 2020 2020 2020  ntegrand..      
+0000c210: 2020 2e2e 206d 6174 683a 3a0a 0a20 2020    .. math::..   
+0000c220: 2020 2020 2020 2020 205c 7469 6c64 657b           \tilde{
+0000c230: 5c6d 6174 6863 616c 7b42 7d7d 5e5c 6173  \mathcal{B}}^\as
+0000c240: 745f 7b5c 616c 7068 6120 6b7d 285c 6f6d  t_{\alpha k}(\om
+0000c250: 6567 6129 0a20 2020 2020 2020 2020 2020  ega).           
+0000c260: 2053 5f7b 5c61 6c70 6861 5c62 6574 617d   S_{\alpha\beta}
+0000c270: 285c 6f6d 6567 6129 5c74 696c 6465 7b5c  (\omega)\tilde{\
+0000c280: 6d61 7468 6361 6c7b 427d 7d5f 7b5c 6265  mathcal{B}}_{\be
+0000c290: 7461 206c 7d28 5c6f 6d65 6761 290a 0a20  ta l}(\omega).. 
+0000c2a0: 2020 2020 2020 2063 616e 2063 6f6e 7375         can consu
+0000c2b0: 6d65 2071 7569 7465 2061 206c 6172 6765  me quite a large
+0000c2c0: 2061 6d6f 756e 7420 6f66 206d 656d 6f72   amount of memor
+0000c2d0: 7920 6966 2073 6574 2075 7020 666f 7220  y if set up for 
+0000c2e0: 616c 6c0a 2020 2020 2020 2020 3a6d 6174  all.        :mat
+0000c2f0: 683a 605c 616c 7068 612c 5c62 6574 612c  h:`\alpha,\beta,
+0000c300: 6b2c 6c60 2061 7420 6f6e 6365 2e20 4966  k,l` at once. If
+0000c310: 2060 6054 7275 6560 602c 2069 7420 6973   ``True``, it is
+0000c320: 206f 6e6c 7920 7365 7420 7570 0a20 2020   only set up.   
+0000c330: 2020 2020 2061 6e64 2069 6e74 6567 7261       and integra
+0000c340: 7465 6420 666f 7220 6120 7369 6e67 6c65  ted for a single
+0000c350: 203a 6d61 7468 3a60 6b60 2061 7420 6120   :math:`k` at a 
+0000c360: 7469 6d65 2061 6e64 206c 6f6f 7065 6420  time and looped 
+0000c370: 6f76 6572 2e0a 2020 2020 2020 2020 5468  over..        Th
+0000c380: 6973 2069 7320 736c 6f77 6572 2062 7574  is is slower but
+0000c390: 2072 6571 7569 7265 7320 6d75 6368 206c   requires much l
+0000c3a0: 6573 7320 6d65 6d6f 7279 2e20 5468 6520  ess memory. The 
+0000c3b0: 6465 6661 756c 7420 6973 0a20 2020 2020  default is.     
+0000c3c0: 2020 2060 6046 616c 7365 6060 2e0a 0a20     ``False``... 
+0000c3d0: 2020 2052 6169 7365 730a 2020 2020 2d2d     Raises.    --
+0000c3e0: 2d2d 2d2d 0a20 2020 2056 616c 7565 4572  ----.    ValueEr
+0000c3f0: 726f 720a 2020 2020 2020 2020 4966 2073  ror.        If s
+0000c400: 7065 6374 7275 6d20 6861 7320 696e 636f  pectrum has inco
+0000c410: 6d70 6174 6962 6c65 2073 6861 7065 2e0a  mpatible shape..
+0000c420: 0a20 2020 2052 6574 7572 6e73 0a20 2020  .    Returns.   
+0000c430: 202d 2d2d 2d2d 2d2d 0a20 2020 2064 6563   -------.    dec
+0000c440: 6179 5f61 6d70 6c69 7475 6465 733a 206e  ay_amplitudes: n
+0000c450: 6461 7272 6179 2c20 7368 6170 6520 285b  darray, shape ([
+0000c460: 5b6e 5f70 6c73 2c20 6e5f 706c 732c 5d20  [n_pls, n_pls,] 
+0000c470: 6e5f 6e6f 7073 2c5d 206e 5f6e 6f70 732c  n_nops,] n_nops,
+0000c480: 2064 2a2a 322c 2064 2a2a 3229 0a20 2020   d**2, d**2).   
+0000c490: 2020 2020 2054 6865 2064 6563 6179 2061       The decay a
+0000c4a0: 6d70 6c69 7475 6465 732e 0a0a 2020 2020  mplitudes...    
+0000c4b0: 2e2e 205f 6e6f 7465 733a 0a0a 2020 2020  .. _notes:..    
+0000c4c0: 4e6f 7465 730a 2020 2020 2d2d 2d2d 2d0a  Notes.    -----.
+0000c4d0: 2020 2020 5468 6520 746f 7461 6c20 6465      The total de
+0000c4e0: 6361 7920 616d 706c 6974 7564 6573 2061  cay amplitudes a
+0000c4f0: 7265 2067 6976 656e 2062 790a 0a20 2020  re given by..   
+0000c500: 202e 2e20 6d61 7468 3a3a 0a0a 2020 2020   .. math::..    
+0000c510: 2020 2020 5c47 616d 6d61 5f7b 5c61 6c70      \Gamma_{\alp
+0000c520: 6861 5c62 6574 612c 206b 6c7d 203d 205c  ha\beta, kl} = \
+0000c530: 696e 745c 6672 6163 7b5c 6d61 7468 726d  int\frac{\mathrm
+0000c540: 7b64 7d5c 6f6d 6567 617d 7b32 5c70 697d  {d}\omega}{2\pi}
+0000c550: 0a20 2020 2020 2020 2020 2020 205c 7469  .            \ti
+0000c560: 6c64 657b 5c6d 6174 6863 616c 7b42 7d7d  lde{\mathcal{B}}
+0000c570: 5e5c 6173 745f 7b5c 616c 7068 6120 6b7d  ^\ast_{\alpha k}
+0000c580: 285c 6f6d 6567 6129 0a20 2020 2020 2020  (\omega).       
+0000c590: 2020 2020 2053 5f7b 5c61 6c70 6861 5c62       S_{\alpha\b
+0000c5a0: 6574 617d 285c 6f6d 6567 6129 5c74 696c  eta}(\omega)\til
+0000c5b0: 6465 7b5c 6d61 7468 6361 6c7b 427d 7d5f  de{\mathcal{B}}_
+0000c5c0: 7b5c 6265 7461 206c 7d28 5c6f 6d65 6761  {\beta l}(\omega
+0000c5d0: 292e 0a0a 2020 2020 4966 2070 756c 7365  )...    If pulse
+0000c5e0: 2063 6f72 7265 6c61 7469 6f6e 7320 6172   correlations ar
+0000c5f0: 6520 7461 6b65 6e20 696e 746f 2061 6363  e taken into acc
+0000c600: 6f75 6e74 2c20 7468 6579 2061 7265 2067  ount, they are g
+0000c610: 6976 656e 2062 790a 0a20 2020 202e 2e20  iven by..    .. 
+0000c620: 6d61 7468 3a3a 0a0a 2020 2020 2020 2020  math::..        
+0000c630: 5c47 616d 6d61 5f7b 5c61 6c70 6861 5c62  \Gamma_{\alpha\b
+0000c640: 6574 612c 206b 6c7d 5e7b 2867 6727 297d  eta, kl}^{(gg')}
+0000c650: 203d 205c 696e 740a 2020 2020 2020 2020   = \int.        
+0000c660: 2020 2020 5c66 7261 637b 5c6d 6174 6872      \frac{\mathr
+0000c670: 6d7b 647d 5c6f 6d65 6761 7d7b 325c 7069  m{d}\omega}{2\pi
+0000c680: 7d20 535f 7b5c 616c 7068 615c 6265 7461  } S_{\alpha\beta
+0000c690: 7d28 5c6f 6d65 6761 290a 2020 2020 2020  }(\omega).      
+0000c6a0: 2020 2020 2020 465f 7b5c 616c 7068 615c        F_{\alpha\
+0000c6b0: 6265 7461 2c20 6b6c 7d5e 7b28 6767 2729  beta, kl}^{(gg')
+0000c6c0: 7d28 5c6f 6d65 6761 292e 0a0a 2020 2020  }(\omega)...    
+0000c6d0: 5365 6520 416c 736f 0a20 2020 202d 2d2d  See Also.    ---
+0000c6e0: 2d2d 2d2d 2d0a 2020 2020 696e 6669 6465  -----.    infide
+0000c6f0: 6c69 7479 3a20 436f 6d70 7574 6520 7468  lity: Compute th
+0000c700: 6520 696e 6669 6465 6c69 7479 2064 6972  e infidelity dir
+0000c710: 6563 746c 792e 0a20 2020 2070 756c 7365  ectly..    pulse
+0000c720: 5f73 6571 7565 6e63 652e 636f 6e63 6174  _sequence.concat
+0000c730: 656e 6174 653a 2043 6f6e 6361 7465 6e61  enate: Concatena
+0000c740: 7465 2060 6050 756c 7365 5365 7175 656e  te ``PulseSequen
+0000c750: 6365 6060 206f 626a 6563 7473 2e0a 2020  ce`` objects..  
+0000c760: 2020 6361 6c63 756c 6174 655f 6672 6571    calculate_freq
+0000c770: 7565 6e63 795f 7368 6966 7473 3a20 5365  uency_shifts: Se
+0000c780: 636f 6e64 206f 7264 6572 2028 756e 6974  cond order (unit
+0000c790: 6172 7929 2074 6572 6d73 2e0a 2020 2020  ary) terms..    
+0000c7a0: 6361 6c63 756c 6174 655f 7075 6c73 655f  calculate_pulse_
+0000c7b0: 636f 7272 656c 6174 696f 6e5f 6669 6c74  correlation_filt
+0000c7c0: 6572 5f66 756e 6374 696f 6e0a 2020 2020  er_function.    
+0000c7d0: 2222 220a 2020 2020 2320 544f 444f 3a20  """.    # TODO: 
+0000c7e0: 5265 706c 6163 6520 696e 6669 6465 6c69  Replace infideli
+0000c7f0: 7479 2829 2062 7920 7468 6973 3f0a 2020  ty() by this?.  
+0000c800: 2020 2320 4e6f 6973 6520 6f70 6572 6174    # Noise operat
+0000c810: 6f72 2069 6e64 6963 6573 0a20 2020 2069  or indices.    i
+0000c820: 6478 203d 2075 7469 6c2e 6765 745f 696e  dx = util.get_in
+0000c830: 6469 6365 735f 6672 6f6d 5f69 6465 6e74  dices_from_ident
+0000c840: 6966 6965 7273 2870 756c 7365 2e6e 5f6f  ifiers(pulse.n_o
+0000c850: 7065 725f 6964 656e 7469 6669 6572 732c  per_identifiers,
+0000c860: 206e 5f6f 7065 725f 6964 656e 7469 6669   n_oper_identifi
+0000c870: 6572 7329 0a20 2020 2069 6620 7768 6963  ers).    if whic
+0000c880: 6820 3d3d 2027 746f 7461 6c27 3a0a 2020  h == 'total':.  
+0000c890: 2020 2020 2020 2320 4661 7374 6572 2074        # Faster t
+0000c8a0: 6f20 7573 6520 6669 6c74 6572 2066 756e  o use filter fun
+0000c8b0: 6374 696f 6e20 696e 7374 6561 6420 6f66  ction instead of
+0000c8c0: 2063 6f6e 7472 6f6c 206d 6174 7269 780a   control matrix.
+0000c8d0: 2020 2020 2020 2020 6966 2070 756c 7365          if pulse
+0000c8e0: 2e69 735f 6361 6368 6564 2827 6669 6c74  .is_cached('filt
+0000c8f0: 6572 5f66 756e 6374 696f 6e5f 6765 6e27  er_function_gen'
+0000c900: 293a 0a20 2020 2020 2020 2020 2020 2063  ):.            c
+0000c910: 6f6e 7472 6f6c 5f6d 6174 7269 7820 3d20  ontrol_matrix = 
+0000c920: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
+0000c930: 2066 696c 7465 725f 6675 6e63 7469 6f6e   filter_function
+0000c940: 203d 2070 756c 7365 2e67 6574 5f66 696c   = pulse.get_fil
+0000c950: 7465 725f 6675 6e63 7469 6f6e 286f 6d65  ter_function(ome
+0000c960: 6761 2c20 7768 6963 683d 2767 656e 6572  ga, which='gener
+0000c970: 616c 697a 6564 2729 0a20 2020 2020 2020  alized').       
+0000c980: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0000c990: 2020 2063 6f6e 7472 6f6c 5f6d 6174 7269     control_matri
+0000c9a0: 7820 3d20 7075 6c73 652e 6765 745f 636f  x = pulse.get_co
+0000c9b0: 6e74 726f 6c5f 6d61 7472 6978 286f 6d65  ntrol_matrix(ome
+0000c9c0: 6761 2c20 7368 6f77 5f70 726f 6772 6573  ga, show_progres
+0000c9d0: 7362 6172 2c20 6361 6368 655f 696e 7465  sbar, cache_inte
+0000c9e0: 726d 6564 6961 7465 7329 0a20 2020 2020  rmediates).     
+0000c9f0: 2020 2020 2020 2066 696c 7465 725f 6675         filter_fu
+0000ca00: 6e63 7469 6f6e 203d 204e 6f6e 650a 2020  nction = None.  
+0000ca10: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000ca20: 2320 7768 6963 6820 3d3d 2027 636f 7272  # which == 'corr
+0000ca30: 656c 6174 696f 6e73 270a 2020 2020 2020  elations'.      
+0000ca40: 2020 6966 2070 756c 7365 2e69 735f 6361    if pulse.is_ca
+0000ca50: 6368 6564 2827 6f6d 6567 6127 293a 0a20  ched('omega'):. 
+0000ca60: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+0000ca70: 7420 6e70 2e61 7272 6179 5f65 7175 616c  t np.array_equal
+0000ca80: 2870 756c 7365 2e6f 6d65 6761 2c20 6f6d  (pulse.omega, om
+0000ca90: 6567 6129 3a0a 2020 2020 2020 2020 2020  ega):.          
+0000caa0: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+0000cab0: 6545 7272 6f72 2827 5075 6c73 6520 636f  eError('Pulse co
+0000cac0: 7272 656c 6174 696f 6e20 6465 6361 7920  rrelation decay 
+0000cad0: 616d 706c 6974 7564 6573 2072 6571 7565  amplitudes reque
+0000cae0: 7374 6564 2062 7574 206f 6d65 6761 206e  sted but omega n
+0000caf0: 6f74 2027 0a20 2020 2020 2020 2020 2020  ot '.           
+0000cb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cb10: 2020 2020 2020 2b20 2765 7175 616c 2074        + 'equal t
+0000cb20: 6f20 6361 6368 6564 2066 7265 7175 656e  o cached frequen
+0000cb30: 6369 6573 2e27 290a 0a20 2020 2020 2020  cies.')..       
+0000cb40: 2069 6620 7075 6c73 652e 6973 5f63 6163   if pulse.is_cac
+0000cb50: 6865 6428 2766 696c 7465 725f 6675 6e63  hed('filter_func
+0000cb60: 7469 6f6e 5f70 635f 6765 6e27 293a 0a20  tion_pc_gen'):. 
+0000cb70: 2020 2020 2020 2020 2020 2063 6f6e 7472             contr
+0000cb80: 6f6c 5f6d 6174 7269 7820 3d20 4e6f 6e65  ol_matrix = None
+0000cb90: 0a20 2020 2020 2020 2020 2020 2066 696c  .            fil
+0000cba0: 7465 725f 6675 6e63 7469 6f6e 203d 2070  ter_function = p
+0000cbb0: 756c 7365 2e67 6574 5f70 756c 7365 5f63  ulse.get_pulse_c
+0000cbc0: 6f72 7265 6c61 7469 6f6e 5f66 696c 7465  orrelation_filte
+0000cbd0: 725f 6675 6e63 7469 6f6e 2877 6869 6368  r_function(which
+0000cbe0: 3d27 6765 6e65 7261 6c69 7a65 6427 290a  ='generalized').
+0000cbf0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0000cc00: 2020 2020 2020 2020 2020 636f 6e74 726f            contro
+0000cc10: 6c5f 6d61 7472 6978 203d 2070 756c 7365  l_matrix = pulse
+0000cc20: 2e67 6574 5f70 756c 7365 5f63 6f72 7265  .get_pulse_corre
+0000cc30: 6c61 7469 6f6e 5f63 6f6e 7472 6f6c 5f6d  lation_control_m
+0000cc40: 6174 7269 7828 290a 2020 2020 2020 2020  atrix().        
+0000cc50: 2020 2020 6669 6c74 6572 5f66 756e 6374      filter_funct
+0000cc60: 696f 6e20 3d20 4e6f 6e65 0a0a 2020 2020  ion = None..    
+0000cc70: 6966 206e 6f74 206d 656d 6f72 795f 7061  if not memory_pa
+0000cc80: 7273 696d 6f6e 696f 7573 3a0a 2020 2020  rsimonious:.    
+0000cc90: 2020 2020 696e 7465 6772 616e 6420 3d20      integrand = 
+0000cca0: 5f67 6574 5f69 6e74 6567 7261 6e64 2873  _get_integrand(s
+0000ccb0: 7065 6374 7275 6d2c 206f 6d65 6761 2c20  pectrum, omega, 
+0000ccc0: 6964 782c 2077 6869 6368 2c20 2767 656e  idx, which, 'gen
+0000ccd0: 6572 616c 697a 6564 272c 0a20 2020 2020  eralized',.     
+0000cce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ccf0: 2020 2020 2020 2020 2020 2020 2020 636f                co
+0000cd00: 6e74 726f 6c5f 6d61 7472 6978 3d63 6f6e  ntrol_matrix=con
+0000cd10: 7472 6f6c 5f6d 6174 7269 782c 0a20 2020  trol_matrix,.   
+0000cd20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cd30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cd40: 6669 6c74 6572 5f66 756e 6374 696f 6e3d  filter_function=
+0000cd50: 6669 6c74 6572 5f66 756e 6374 696f 6e29  filter_function)
+0000cd60: 0a20 2020 2020 2020 2064 6563 6179 5f61  .        decay_a
+0000cd70: 6d70 6c69 7475 6465 7320 3d20 7574 696c  mplitudes = util
+0000cd80: 2e69 6e74 6567 7261 7465 2869 6e74 6567  .integrate(integ
+0000cd90: 7261 6e64 2c20 6f6d 6567 6129 2f28 322a  rand, omega)/(2*
+0000cda0: 6e70 2e70 6929 0a20 2020 2020 2020 2072  np.pi).        r
+0000cdb0: 6574 7572 6e20 6465 6361 795f 616d 706c  eturn decay_ampl
+0000cdc0: 6974 7564 6573 0a0a 2020 2020 6e5f 6b6c  itudes..    n_kl
+0000cdd0: 203d 206c 656e 2870 756c 7365 2e62 6173   = len(pulse.bas
+0000cde0: 6973 290a 2020 2020 666f 7220 6b20 696e  is).    for k in
+0000cdf0: 2075 7469 6c2e 7072 6f67 7265 7373 6261   util.progressba
+0000ce00: 725f 7261 6e67 6528 6e5f 6b6c 2c20 7368  r_range(n_kl, sh
+0000ce10: 6f77 5f70 726f 6772 6573 7362 6172 3d73  ow_progressbar=s
+0000ce20: 686f 775f 7072 6f67 7265 7373 6261 722c  how_progressbar,
+0000ce30: 2064 6573 633d 2749 6e74 6567 7261 7469   desc='Integrati
+0000ce40: 6e67 2729 3a0a 2020 2020 2020 2020 6966  ng'):.        if
+0000ce50: 2063 6f6e 7472 6f6c 5f6d 6174 7269 7820   control_matrix 
+0000ce60: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0000ce70: 2020 2020 2020 2020 2069 6e74 6567 7261           integra
+0000ce80: 6e64 203d 205f 6765 745f 696e 7465 6772  nd = _get_integr
+0000ce90: 616e 6428 0a20 2020 2020 2020 2020 2020  and(.           
+0000cea0: 2020 2020 2073 7065 6374 7275 6d2c 206f       spectrum, o
+0000ceb0: 6d65 6761 2c20 6964 782c 2077 6869 6368  mega, idx, which
+0000cec0: 2c20 2767 656e 6572 616c 697a 6564 272c  , 'generalized',
+0000ced0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cee0: 2063 6f6e 7472 6f6c 5f6d 6174 7269 783d   control_matrix=
+0000cef0: 5b63 6f6e 7472 6f6c 5f6d 6174 7269 785b  [control_matrix[
+0000cf00: 2e2e 2e2c 206b 3a6b 2b31 2c20 3a5d 2c20  ..., k:k+1, :], 
+0000cf10: 636f 6e74 726f 6c5f 6d61 7472 6978 5d2c  control_matrix],
+0000cf20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cf30: 2066 696c 7465 725f 6675 6e63 7469 6f6e   filter_function
+0000cf40: 3d66 696c 7465 725f 6675 6e63 7469 6f6e  =filter_function
+0000cf50: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+0000cf60: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0000cf70: 2020 2020 2020 2020 2069 6e74 6567 7261           integra
+0000cf80: 6e64 203d 205f 6765 745f 696e 7465 6772  nd = _get_integr
+0000cf90: 616e 6428 0a20 2020 2020 2020 2020 2020  and(.           
+0000cfa0: 2020 2020 2073 7065 6374 7275 6d2c 206f       spectrum, o
+0000cfb0: 6d65 6761 2c20 6964 782c 2077 6869 6368  mega, idx, which
+0000cfc0: 2c20 2767 656e 6572 616c 697a 6564 272c  , 'generalized',
+0000cfd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cfe0: 2063 6f6e 7472 6f6c 5f6d 6174 7269 783d   control_matrix=
+0000cff0: 636f 6e74 726f 6c5f 6d61 7472 6978 2c0a  control_matrix,.
+0000d000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d010: 6669 6c74 6572 5f66 756e 6374 696f 6e3d  filter_function=
+0000d020: 6669 6c74 6572 5f66 756e 6374 696f 6e5b  filter_function[
+0000d030: 2e2e 2e2c 206b 3a6b 2b31 2c20 3a2c 203a  ..., k:k+1, :, :
+0000d040: 5d0a 2020 2020 2020 2020 2020 2020 290a  ].            ).
+0000d050: 0a20 2020 2020 2020 2069 6620 6b20 3d3d  .        if k ==
+0000d060: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
+0000d070: 6465 6361 795f 616d 706c 6974 7564 6573  decay_amplitudes
+0000d080: 203d 206e 702e 656d 7074 7928 696e 7465   = np.empty(inte
+0000d090: 6772 616e 642e 7368 6170 655b 3a2d 335d  grand.shape[:-3]
+0000d0a0: 202b 2028 6e5f 6b6c 2c29 2a32 290a 0a20   + (n_kl,)*2).. 
+0000d0b0: 2020 2020 2020 2064 6563 6179 5f61 6d70         decay_amp
+0000d0c0: 6c69 7475 6465 735b 2e2e 2e2c 206b 3a6b  litudes[..., k:k
+0000d0d0: 2b31 2c20 3a5d 203d 2075 7469 6c2e 696e  +1, :] = util.in
+0000d0e0: 7465 6772 6174 6528 696e 7465 6772 616e  tegrate(integran
+0000d0f0: 642c 206f 6d65 6761 292f 2832 2a6e 702e  d, omega)/(2*np.
+0000d100: 7069 290a 0a20 2020 2072 6574 7572 6e20  pi)..    return 
+0000d110: 6465 6361 795f 616d 706c 6974 7564 6573  decay_amplitudes
+0000d120: 0a0a 0a64 6566 2063 616c 6375 6c61 7465  ...def calculate
+0000d130: 5f66 7265 7175 656e 6379 5f73 6869 6674  _frequency_shift
+0000d140: 7328 0a20 2020 2020 2020 2070 756c 7365  s(.        pulse
+0000d150: 3a20 2750 756c 7365 5365 7175 656e 6365  : 'PulseSequence
+0000d160: 272c 0a20 2020 2020 2020 2073 7065 6374  ',.        spect
+0000d170: 7275 6d3a 206e 6461 7272 6179 2c0a 2020  rum: ndarray,.  
+0000d180: 2020 2020 2020 6f6d 6567 613a 2043 6f65        omega: Coe
+0000d190: 6666 6963 6965 6e74 732c 0a20 2020 2020  fficients,.     
+0000d1a0: 2020 206e 5f6f 7065 725f 6964 656e 7469     n_oper_identi
+0000d1b0: 6669 6572 733a 204f 7074 696f 6e61 6c5b  fiers: Optional[
+0000d1c0: 5365 7175 656e 6365 5b73 7472 5d5d 203d  Sequence[str]] =
+0000d1d0: 204e 6f6e 652c 0a20 2020 2020 2020 2073   None,.        s
+0000d1e0: 686f 775f 7072 6f67 7265 7373 6261 723a  how_progressbar:
+0000d1f0: 2062 6f6f 6c20 3d20 4661 6c73 650a 2920   bool = False.) 
+0000d200: 2d3e 206e 6461 7272 6179 3a0a 2020 2020  -> ndarray:.    
+0000d210: 7222 2222 0a20 2020 2047 6574 2074 6865  r""".    Get the
+0000d220: 2066 7265 7175 656e 6379 2073 6869 6674   frequency shift
+0000d230: 7320 3a6d 6174 683a 605c 4465 6c74 615f  s :math:`\Delta_
+0000d240: 7b5c 616c 7068 615c 6265 7461 2c20 6b6c  {\alpha\beta, kl
+0000d250: 7d60 2066 6f72 206e 6f69 7365 0a20 2020  }` for noise.   
+0000d260: 2073 6f75 7263 6573 203a 6d61 7468 3a60   sources :math:`
+0000d270: 5c61 6c70 6861 2c5c 6265 7461 6020 616e  \alpha,\beta` an
+0000d280: 6420 6261 7369 7320 656c 656d 656e 7473  d basis elements
+0000d290: 203a 6d61 7468 3a60 6b2c 6c60 2e0a 0a20   :math:`k,l`... 
+0000d2a0: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+0000d2b0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+0000d2c0: 2070 756c 7365 3a20 5075 6c73 6553 6571   pulse: PulseSeq
+0000d2d0: 7565 6e63 650a 2020 2020 2020 2020 5468  uence.        Th
+0000d2e0: 6520 6060 5075 6c73 6553 6571 7565 6e63  e ``PulseSequenc
+0000d2f0: 6560 6020 696e 7374 616e 6365 2066 6f72  e`` instance for
+0000d300: 2077 6869 6368 2074 6f20 636f 6d70 7574   which to comput
+0000d310: 6520 7468 650a 2020 2020 2020 2020 6672  e the.        fr
+0000d320: 6571 7565 6e63 7920 7368 6966 7473 2e0a  equency shifts..
+0000d330: 2020 2020 7370 6563 7472 756d 3a20 6172      spectrum: ar
+0000d340: 7261 795f 6c69 6b65 2c20 7368 6170 6520  ray_like, shape 
+0000d350: 285b 5b6e 5f6e 6f70 732c 5d20 6e5f 6e6f  ([[n_nops,] n_no
+0000d360: 7073 2c5d 206e 5f6f 6d65 6761 290a 2020  ps,] n_omega).  
+0000d370: 2020 2020 2020 5468 6520 7477 6f2d 7369        The two-si
+0000d380: 6465 6420 6e6f 6973 6520 706f 7765 7220  ded noise power 
+0000d390: 7370 6563 7472 616c 2064 656e 7369 7479  spectral density
+0000d3a0: 2e20 4966 2031 2d64 2c20 7468 6520 7361  . If 1-d, the sa
+0000d3b0: 6d65 0a20 2020 2020 2020 2073 7065 6374  me.        spect
+0000d3c0: 7275 6d20 6973 2075 7365 6420 666f 7220  rum is used for 
+0000d3d0: 616c 6c20 6e6f 6973 6520 6f70 6572 6174  all noise operat
+0000d3e0: 6f72 732e 2049 6620 322d 642c 206f 6e65  ors. If 2-d, one
+0000d3f0: 2028 7365 6c66 2d29 0a20 2020 2020 2020   (self-).       
+0000d400: 2073 7065 6374 7275 6d20 666f 7220 6561   spectrum for ea
+0000d410: 6368 206e 6f69 7365 206f 7065 7261 746f  ch noise operato
+0000d420: 7220 6973 2065 7870 6563 7465 642e 2049  r is expected. I
+0000d430: 6620 332d 642c 2073 686f 756c 6420 6265  f 3-d, should be
+0000d440: 0a20 2020 2020 2020 2061 206d 6174 7269  .        a matri
+0000d450: 7820 6f66 2063 726f 7373 2d73 7065 6374  x of cross-spect
+0000d460: 7261 2073 7563 6820 7468 6174 0a20 2020  ra such that.   
+0000d470: 2020 2020 2060 6073 7065 6374 7275 6d5b       ``spectrum[
+0000d480: 692c 206a 5d20 3d3d 2073 7065 6374 7275  i, j] == spectru
+0000d490: 6d5b 6a2c 2069 5d2e 636f 6e6a 2829 6060  m[j, i].conj()``
+0000d4a0: 2e0a 2020 2020 6f6d 6567 613a 2061 7272  ..    omega: arr
+0000d4b0: 6179 5f6c 696b 652c 0a20 2020 2020 2020  ay_like,.       
+0000d4c0: 2054 6865 2066 7265 7175 656e 6369 6573   The frequencies
+0000d4d0: 2e20 4e6f 7465 2074 6861 7420 7468 6520  . Note that the 
+0000d4e0: 6672 6571 7565 6e63 6965 7320 6172 6520  frequencies are 
+0000d4f0: 6173 7375 6d65 6420 746f 2062 650a 2020  assumed to be.  
+0000d500: 2020 2020 2020 7379 6d6d 6574 7269 6320        symmetric 
+0000d510: 6162 6f75 7420 7a65 726f 2e0a 2020 2020  about zero..    
+0000d520: 6e5f 6f70 6572 5f69 6465 6e74 6966 6965  n_oper_identifie
+0000d530: 7273 3a20 6172 7261 795f 6c69 6b65 2c20  rs: array_like, 
+0000d540: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
+0000d550: 2054 6865 2069 6465 6e74 6966 6965 7273   The identifiers
+0000d560: 206f 6620 7468 6520 6e6f 6973 6520 6f70   of the noise op
+0000d570: 6572 6174 6f72 7320 666f 7220 7768 6963  erators for whic
+0000d580: 6820 746f 2063 616c 6375 6c61 7465 0a20  h to calculate. 
+0000d590: 2020 2020 2020 2074 6865 2066 7265 7175         the frequ
+0000d5a0: 656e 6379 2073 6869 6674 732e 2054 6865  ency shifts. The
+0000d5b0: 2064 6566 6175 6c74 2069 7320 616c 6c2e   default is all.
+0000d5c0: 0a20 2020 2073 686f 775f 7072 6f67 7265  .    show_progre
+0000d5d0: 7373 6261 723a 2062 6f6f 6c2c 206f 7074  ssbar: bool, opt
+0000d5e0: 696f 6e61 6c0a 2020 2020 2020 2020 5368  ional.        Sh
+0000d5f0: 6f77 2061 2070 726f 6772 6573 7320 6261  ow a progress ba
+0000d600: 7220 666f 7220 7468 6520 6361 6c63 756c  r for the calcul
+0000d610: 6174 696f 6e2e 0a0a 2020 2020 5261 6973  ation...    Rais
+0000d620: 6573 0a20 2020 202d 2d2d 2d2d 2d0a 2020  es.    ------.  
+0000d630: 2020 5661 6c75 6545 7272 6f72 0a20 2020    ValueError.   
+0000d640: 2020 2020 2049 6620 7370 6563 7472 756d       If spectrum
+0000d650: 2068 6173 2069 6e63 6f6d 7061 7469 626c   has incompatibl
+0000d660: 6520 7368 6170 652e 0a0a 2020 2020 5265  e shape...    Re
+0000d670: 7475 726e 730a 2020 2020 2d2d 2d2d 2d2d  turns.    ------
+0000d680: 2d0a 2020 2020 4465 6c74 613a 206e 6461  -.    Delta: nda
+0000d690: 7272 6179 2c20 7368 6170 6520 285b 6e5f  rray, shape ([n_
+0000d6a0: 6e6f 7073 2c5d 206e 5f6e 6f70 732c 2064  nops,] n_nops, d
+0000d6b0: 2a2a 322c 2064 2a2a 3229 0a20 2020 2020  **2, d**2).     
+0000d6c0: 2020 2054 6865 2066 7265 7175 656e 6379     The frequency
+0000d6d0: 2073 6869 6674 732e 0a0a 2020 2020 2e2e   shifts...    ..
+0000d6e0: 205f 6e6f 7465 733a 0a0a 2020 2020 4e6f   _notes:..    No
+0000d6f0: 7465 730a 2020 2020 2d2d 2d2d 2d0a 2020  tes.    -----.  
+0000d700: 2020 5468 6520 746f 7461 6c20 6672 6571    The total freq
+0000d710: 7565 6e63 7920 7368 6966 7473 2061 7265  uency shifts are
+0000d720: 2067 6976 656e 2062 790a 0a20 2020 202e   given by..    .
+0000d730: 2e20 6d61 7468 3a3a 0a0a 2020 2020 2020  . math::..      
+0000d740: 2020 5c44 656c 7461 5f7b 5c61 6c70 6861    \Delta_{\alpha
+0000d750: 5c62 6574 612c 206b 6c7d 203d 205c 696e  \beta, kl} = \in
+0000d760: 745f 7b2d 5c69 6e66 7479 7d5e 5c69 6e66  t_{-\infty}^\inf
+0000d770: 7479 0a20 2020 2020 2020 2020 2020 205c  ty.            \
+0000d780: 6672 6163 7b5c 6d61 7468 726d 7b64 7d7b  frac{\mathrm{d}{
+0000d790: 5c6f 6d65 6761 7d7d 7b32 5c70 697d 2053  \omega}}{2\pi} S
+0000d7a0: 5f7b 5c61 6c70 6861 5c62 6574 617d 285c  _{\alpha\beta}(\
+0000d7b0: 6f6d 6567 6129 0a20 2020 2020 2020 2020  omega).         
+0000d7c0: 2020 2046 5f7b 5c61 6c70 6861 5c62 6574     F_{\alpha\bet
+0000d7d0: 612c 6b6c 7d5e 7b28 3229 7d28 5c6f 6d65  a,kl}^{(2)}(\ome
+0000d7e0: 6761 290a 0a20 2020 2077 6974 6820 3a6d  ga)..    with :m
+0000d7f0: 6174 683a 6046 5f7b 5c61 6c70 6861 5c62  ath:`F_{\alpha\b
+0000d800: 6574 612c 6b6c 7d5e 7b28 3229 7d28 5c6f  eta,kl}^{(2)}(\o
+0000d810: 6d65 6761 2960 2074 6865 2073 6563 6f6e  mega)` the secon
+0000d820: 6420 6f72 6465 7220 6669 6c74 6572 0a20  d order filter. 
+0000d830: 2020 2066 756e 6374 696f 6e2e 0a0a 2020     function...  
+0000d840: 2020 5365 6520 416c 736f 0a20 2020 202d    See Also.    -
+0000d850: 2d2d 2d2d 2d2d 2d0a 2020 2020 6361 6c63  -------.    calc
+0000d860: 756c 6174 655f 7365 636f 6e64 5f6f 7264  ulate_second_ord
+0000d870: 6572 5f66 696c 7465 725f 6675 6e63 7469  er_filter_functi
+0000d880: 6f6e 3a20 436f 7272 6573 706f 6e64 696e  on: Correspondin
+0000d890: 6720 6669 6c74 6572 2066 756e 6374 696f  g filter functio
+0000d8a0: 6e2e 0a20 2020 2063 616c 6375 6c61 7465  n..    calculate
+0000d8b0: 5f64 6563 6179 5f61 6d70 6c69 7475 6465  _decay_amplitude
+0000d8c0: 733a 2046 6972 7374 206f 7264 6572 2028  s: First order (
+0000d8d0: 6469 7373 6970 6174 6976 6529 2074 6572  dissipative) ter
+0000d8e0: 6d73 2e0a 2020 2020 696e 6669 6465 6c69  ms..    infideli
+0000d8f0: 7479 3a20 436f 6d70 7574 6520 7468 6520  ty: Compute the 
+0000d900: 696e 6669 6465 6c69 7479 2064 6972 6563  infidelity direc
+0000d910: 746c 792e 0a20 2020 2070 756c 7365 5f73  tly..    pulse_s
+0000d920: 6571 7565 6e63 652e 636f 6e63 6174 656e  equence.concaten
+0000d930: 6174 653a 2043 6f6e 6361 7465 6e61 7465  ate: Concatenate
+0000d940: 2060 6050 756c 7365 5365 7175 656e 6365   ``PulseSequence
+0000d950: 6060 206f 626a 6563 7473 2e0a 2020 2020  `` objects..    
+0000d960: 6361 6c63 756c 6174 655f 7075 6c73 655f  calculate_pulse_
+0000d970: 636f 7272 656c 6174 696f 6e5f 6669 6c74  correlation_filt
+0000d980: 6572 5f66 756e 6374 696f 6e0a 2020 2020  er_function.    
+0000d990: 2222 220a 2020 2020 6964 7820 3d20 7574  """.    idx = ut
+0000d9a0: 696c 2e67 6574 5f69 6e64 6963 6573 5f66  il.get_indices_f
+0000d9b0: 726f 6d5f 6964 656e 7469 6669 6572 7328  rom_identifiers(
+0000d9c0: 7075 6c73 652e 6e5f 6f70 6572 5f69 6465  pulse.n_oper_ide
+0000d9d0: 6e74 6966 6965 7273 2c20 6e5f 6f70 6572  ntifiers, n_oper
+0000d9e0: 5f69 6465 6e74 6966 6965 7273 290a 2020  _identifiers).  
+0000d9f0: 2020 6669 6c74 6572 5f66 756e 6374 696f    filter_functio
+0000da00: 6e5f 3220 3d20 7075 6c73 652e 6765 745f  n_2 = pulse.get_
+0000da10: 6669 6c74 6572 5f66 756e 6374 696f 6e28  filter_function(
+0000da20: 6f6d 6567 612c 206f 7264 6572 3d32 2c0a  omega, order=2,.
+0000da30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000da40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000da50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000da60: 2020 7368 6f77 5f70 726f 6772 6573 7362    show_progressb
+0000da70: 6172 3d73 686f 775f 7072 6f67 7265 7373  ar=show_progress
+0000da80: 6261 7229 0a20 2020 2069 6e74 6567 7261  bar).    integra
+0000da90: 6e64 203d 205f 6765 745f 696e 7465 6772  nd = _get_integr
+0000daa0: 616e 6428 7370 6563 7472 756d 2c20 6f6d  and(spectrum, om
+0000dab0: 6567 612c 2069 6478 2c20 7768 6963 685f  ega, idx, which_
+0000dac0: 7075 6c73 653d 2774 6f74 616c 272c 2077  pulse='total', w
+0000dad0: 6869 6368 5f46 463d 2767 656e 6572 616c  hich_FF='general
+0000dae0: 697a 6564 272c 0a20 2020 2020 2020 2020  ized',.         
+0000daf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db00: 2020 2020 2020 6669 6c74 6572 5f66 756e        filter_fun
+0000db10: 6374 696f 6e3d 6669 6c74 6572 5f66 756e  ction=filter_fun
+0000db20: 6374 696f 6e5f 3229 0a20 2020 2066 7265  ction_2).    fre
+0000db30: 7175 656e 6379 5f73 6869 6674 7320 3d20  quency_shifts = 
+0000db40: 7574 696c 2e69 6e74 6567 7261 7465 2869  util.integrate(i
+0000db50: 6e74 6567 7261 6e64 2c20 6f6d 6567 6129  ntegrand, omega)
+0000db60: 2f28 322a 6e70 2e70 6929 0a20 2020 2072  /(2*np.pi).    r
+0000db70: 6574 7572 6e20 6672 6571 7565 6e63 795f  eturn frequency_
+0000db80: 7368 6966 7473 0a0a 0a40 7574 696c 2e70  shifts...@util.p
+0000db90: 6172 7365 5f6f 7074 696f 6e61 6c5f 7061  arse_optional_pa
+0000dba0: 7261 6d65 7465 7273 2877 6869 6368 3d28  rameters(which=(
+0000dbb0: 2766 6964 656c 6974 7927 2c20 2767 656e  'fidelity', 'gen
+0000dbc0: 6572 616c 697a 6564 2729 290a 6465 6620  eralized')).def 
+0000dbd0: 6361 6c63 756c 6174 655f 6669 6c74 6572  calculate_filter
+0000dbe0: 5f66 756e 6374 696f 6e28 636f 6e74 726f  _function(contro
+0000dbf0: 6c5f 6d61 7472 6978 3a20 6e64 6172 7261  l_matrix: ndarra
+0000dc00: 792c 2077 6869 6368 3a20 7374 7220 3d20  y, which: str = 
+0000dc10: 2766 6964 656c 6974 7927 2920 2d3e 206e  'fidelity') -> n
+0000dc20: 6461 7272 6179 3a0a 2020 2020 7222 2222  darray:.    r"""
+0000dc30: 436f 6d70 7574 6520 7468 6520 6669 6c74  Compute the filt
+0000dc40: 6572 2066 756e 6374 696f 6e20 6672 6f6d  er function from
+0000dc50: 2074 6865 2063 6f6e 7472 6f6c 206d 6174   the control mat
+0000dc60: 7269 782e 0a0a 2020 2020 5061 7261 6d65  rix...    Parame
+0000dc70: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
+0000dc80: 2d2d 2d0a 2020 2020 636f 6e74 726f 6c5f  ---.    control_
+0000dc90: 6d61 7472 6978 3a20 6172 7261 795f 6c69  matrix: array_li
+0000dca0: 6b65 2c20 7368 6170 6520 286e 5f6e 6f70  ke, shape (n_nop
+0000dcb0: 732c 2064 2a2a 322c 206e 5f6f 6d65 6761  s, d**2, n_omega
+0000dcc0: 290a 2020 2020 2020 2020 5468 6520 636f  ).        The co
+0000dcd0: 6e74 726f 6c20 6d61 7472 6978 2e0a 2020  ntrol matrix..  
+0000dce0: 2020 7768 6963 6820 3a20 7374 722c 206f    which : str, o
+0000dcf0: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
+0000dd00: 5768 6963 6820 6669 6c74 6572 2066 756e  Which filter fun
+0000dd10: 6374 696f 6e20 746f 2072 6574 7572 6e2e  ction to return.
+0000dd20: 2045 6974 6865 7220 2766 6964 656c 6974   Either 'fidelit
+0000dd30: 7927 2028 6465 6661 756c 7429 206f 720a  y' (default) or.
+0000dd40: 2020 2020 2020 2020 2767 656e 6572 616c          'general
+0000dd50: 697a 6564 2720 2873 6565 203a 7265 663a  ized' (see :ref:
+0000dd60: 604e 6f74 6573 203c 6e6f 7465 733e 6029  `Notes <notes>`)
+0000dd70: 2e0a 0a20 2020 2052 6574 7572 6e73 0a20  ...    Returns. 
+0000dd80: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2066     -------.    f
+0000dd90: 696c 7465 725f 6675 6e63 7469 6f6e 3a20  ilter_function: 
+0000dda0: 6e64 6172 7261 792c 2073 6861 7065 2028  ndarray, shape (
+0000ddb0: 6e5f 6e6f 7073 2c20 6e5f 6e6f 7073 2c20  n_nops, n_nops, 
+0000ddc0: 5b64 2a2a 322c 2064 2a2a 322c 5d20 6e5f  [d**2, d**2,] n_
+0000ddd0: 6f6d 6567 6129 0a20 2020 2020 2020 2054  omega).        T
+0000dde0: 6865 2066 696c 7465 7220 6675 6e63 7469  he filter functi
+0000ddf0: 6f6e 7320 666f 7220 6561 6368 206e 6f69  ons for each noi
+0000de00: 7365 206f 7065 7261 746f 7220 636f 7272  se operator corr
+0000de10: 656c 6174 696f 6e2e 2054 6865 0a20 2020  elation. The.   
+0000de20: 2020 2020 2064 6961 676f 6e61 6c20 636f       diagonal co
+0000de30: 7272 6573 706f 6e64 7320 746f 2074 6865  rresponds to the
+0000de40: 2066 696c 7465 7220 6675 6e63 7469 6f6e   filter function
+0000de50: 7320 666f 7220 756e 636f 7272 656c 6174  s for uncorrelat
+0000de60: 6564 0a20 2020 2020 2020 206e 6f69 7365  ed.        noise
+0000de70: 2073 6f75 7263 6573 2e0a 0a20 2020 202e   sources...    .
+0000de80: 2e20 5f6e 6f74 6573 3a0a 0a20 2020 204e  . _notes:..    N
+0000de90: 6f74 6573 0a20 2020 202d 2d2d 2d2d 0a20  otes.    -----. 
+0000dea0: 2020 2054 6865 2067 656e 6572 616c 697a     The generaliz
+0000deb0: 6564 2066 696c 7465 7220 6675 6e63 7469  ed filter functi
+0000dec0: 6f6e 2069 7320 6769 7665 6e20 6279 0a0a  on is given by..
+0000ded0: 2020 2020 2e2e 206d 6174 683a 3a0a 0a20      .. math::.. 
+0000dee0: 2020 2020 2020 2046 5f7b 5c61 6c70 6861         F_{\alpha
+0000def0: 5c62 6574 612c 6b6c 7d28 5c6f 6d65 6761  \beta,kl}(\omega
+0000df00: 2920 3d0a 2020 2020 2020 2020 2020 2020  ) =.            
+0000df10: 5c74 696c 6465 7b5c 6d61 7468 6361 6c7b  \tilde{\mathcal{
+0000df20: 427d 7d5f 7b5c 616c 7068 6120 6b7d 5e5c  B}}_{\alpha k}^\
+0000df30: 6173 7428 5c6f 6d65 6761 290a 2020 2020  ast(\omega).    
+0000df40: 2020 2020 2020 2020 5c74 696c 6465 7b5c          \tilde{\
+0000df50: 6d61 7468 6361 6c7b 427d 7d5f 7b5c 6265  mathcal{B}}_{\be
+0000df60: 7461 206c 7d28 5c6f 6d65 6761 292c 0a0a  ta l}(\omega),..
+0000df70: 2020 2020 7768 6572 6520 3a6d 6174 683a      where :math:
+0000df80: 605c 616c 7068 612c 5c62 6574 6160 2061  `\alpha,\beta` a
+0000df90: 7265 2069 6e64 6963 6573 2063 6f75 6e74  re indices count
+0000dfa0: 696e 6720 7468 6520 6e6f 6973 6520 6f70  ing the noise op
+0000dfb0: 6572 6174 6f72 730a 2020 2020 3a6d 6174  erators.    :mat
+0000dfc0: 683a 6042 5f5c 616c 7068 6160 2061 6e64  h:`B_\alpha` and
+0000dfd0: 203a 6d61 7468 3a60 6b2c 6c60 2069 6e64   :math:`k,l` ind
+0000dfe0: 6963 6573 2063 6f75 6e74 696e 6720 7468  ices counting th
+0000dff0: 6520 6261 7369 7320 656c 656d 656e 7473  e basis elements
+0000e000: 0a20 2020 203a 6d61 7468 3a60 435f 6b60  .    :math:`C_k`
+0000e010: 2e0a 0a20 2020 2054 6865 2066 6964 656c  ...    The fidel
+0000e020: 6974 7920 6669 6c74 6572 2066 756e 6374  ity filter funct
+0000e030: 696f 6e20 6973 206f 6274 6169 6e65 6420  ion is obtained 
+0000e040: 6279 2074 7261 6369 6e67 206f 7665 7220  by tracing over 
+0000e050: 7468 6520 6261 7369 730a 2020 2020 696e  the basis.    in
+0000e060: 6469 6365 733a 0a0a 2020 2020 2e2e 206d  dices:..    .. m
+0000e070: 6174 683a 3a0a 0a20 2020 2020 2020 2046  ath::..        F
+0000e080: 5f7b 5c61 6c70 6861 5c62 6574 617d 285c  _{\alpha\beta}(\
+0000e090: 6f6d 6567 6129 203d 205c 7375 6d5f 7b6b  omega) = \sum_{k
+0000e0a0: 7d20 465f 7b5c 616c 7068 615c 6265 7461  } F_{\alpha\beta
+0000e0b0: 2c6b 6b7d 285c 6f6d 6567 6129 2e0a 0a20  ,kk}(\omega)... 
+0000e0c0: 2020 2053 6565 2041 6c73 6f0a 2020 2020     See Also.    
+0000e0d0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2063 616c  --------.    cal
+0000e0e0: 6375 6c61 7465 5f63 6f6e 7472 6f6c 5f6d  culate_control_m
+0000e0f0: 6174 7269 785f 6672 6f6d 5f73 6372 6174  atrix_from_scrat
+0000e100: 6368 3a20 436f 6e74 726f 6c20 6d61 7472  ch: Control matr
+0000e110: 6978 2066 726f 6d20 7363 7261 7463 682e  ix from scratch.
+0000e120: 0a20 2020 2063 616c 6375 6c61 7465 5f63  .    calculate_c
+0000e130: 6f6e 7472 6f6c 5f6d 6174 7269 785f 6672  ontrol_matrix_fr
+0000e140: 6f6d 5f61 746f 6d69 633a 2043 6f6e 7472  om_atomic: Contr
+0000e150: 6f6c 206d 6174 7269 7820 6672 6f6d 2063  ol matrix from c
+0000e160: 6f6e 6361 7465 6e61 7469 6f6e 2e0a 2020  oncatenation..  
+0000e170: 2020 6361 6c63 756c 6174 655f 7075 6c73    calculate_puls
+0000e180: 655f 636f 7272 656c 6174 696f 6e5f 6669  e_correlation_fi
+0000e190: 6c74 6572 5f66 756e 6374 696f 6e3a 2050  lter_function: P
+0000e1a0: 756c 7365 2063 6f72 7265 6c61 7469 6f6e  ulse correlation
+0000e1b0: 732e 0a20 2020 2022 2222 0a20 2020 2069  s..    """.    i
+0000e1c0: 6620 7768 6963 6820 3d3d 2027 6669 6465  f which == 'fide
+0000e1d0: 6c69 7479 273a 0a20 2020 2020 2020 2073  lity':.        s
+0000e1e0: 7562 7363 7269 7074 7320 3d20 2761 6b6f  ubscripts = 'ako
+0000e1f0: 2c62 6b6f 2d3e 6162 6f27 0a20 2020 2065  ,bko->abo'.    e
+0000e200: 6c73 653a 0a20 2020 2020 2020 2023 2077  lse:.        # w
+0000e210: 6869 6368 203d 3d20 2767 656e 6572 616c  hich == 'general
+0000e220: 697a 6564 270a 2020 2020 2020 2020 7375  ized'.        su
+0000e230: 6273 6372 6970 7473 203d 2027 616b 6f2c  bscripts = 'ako,
+0000e240: 626c 6f2d 3e61 626b 6c6f 270a 0a20 2020  blo->abklo'..   
+0000e250: 2072 6574 7572 6e20 6e70 2e65 696e 7375   return np.einsu
+0000e260: 6d28 7375 6273 6372 6970 7473 2c20 636f  m(subscripts, co
+0000e270: 6e74 726f 6c5f 6d61 7472 6978 2e63 6f6e  ntrol_matrix.con
+0000e280: 6a28 292c 2063 6f6e 7472 6f6c 5f6d 6174  j(), control_mat
+0000e290: 7269 7829 0a0a 0a64 6566 2063 616c 6375  rix)...def calcu
+0000e2a0: 6c61 7465 5f73 6563 6f6e 645f 6f72 6465  late_second_orde
+0000e2b0: 725f 6669 6c74 6572 5f66 756e 6374 696f  r_filter_functio
+0000e2c0: 6e28 0a20 2020 2020 2020 2065 6967 7661  n(.        eigva
+0000e2d0: 6c73 3a20 6e64 6172 7261 792c 0a20 2020  ls: ndarray,.   
+0000e2e0: 2020 2020 2065 6967 7665 6373 3a20 6e64       eigvecs: nd
+0000e2f0: 6172 7261 792c 0a20 2020 2020 2020 2070  array,.        p
+0000e300: 726f 7061 6761 746f 7273 3a20 6e64 6172  ropagators: ndar
+0000e310: 7261 792c 0a20 2020 2020 2020 206f 6d65  ray,.        ome
+0000e320: 6761 3a20 436f 6566 6669 6369 656e 7473  ga: Coefficients
+0000e330: 2c0a 2020 2020 2020 2020 6261 7369 733a  ,.        basis:
+0000e340: 2042 6173 6973 2c0a 2020 2020 2020 2020   Basis,.        
+0000e350: 6e5f 6f70 6572 733a 2053 6571 7565 6e63  n_opers: Sequenc
+0000e360: 655b 4f70 6572 6174 6f72 5d2c 0a20 2020  e[Operator],.   
+0000e370: 2020 2020 206e 5f63 6f65 6666 733a 2053       n_coeffs: S
+0000e380: 6571 7565 6e63 655b 436f 6566 6669 6369  equence[Coeffici
+0000e390: 656e 7473 5d2c 0a20 2020 2020 2020 2064  ents],.        d
+0000e3a0: 743a 2043 6f65 6666 6963 6965 6e74 732c  t: Coefficients,
+0000e3b0: 0a20 2020 2020 2020 2069 6e74 6572 6d65  .        interme
+0000e3c0: 6469 6174 6573 3a20 4f70 7469 6f6e 616c  diates: Optional
+0000e3d0: 5b44 6963 745b 7374 722c 206e 6461 7272  [Dict[str, ndarr
+0000e3e0: 6179 5d5d 203d 204e 6f6e 652c 0a20 2020  ay]] = None,.   
+0000e3f0: 2020 2020 2073 686f 775f 7072 6f67 7265       show_progre
+0000e400: 7373 6261 723a 2062 6f6f 6c20 3d20 4661  ssbar: bool = Fa
+0000e410: 6c73 650a 2920 2d3e 206e 6461 7272 6179  lse.) -> ndarray
+0000e420: 3a0a 2020 2020 7222 2222 4361 6c63 756c  :.    r"""Calcul
+0000e430: 6174 6520 7468 6520 7365 636f 6e64 206f  ate the second o
+0000e440: 7264 6572 2066 696c 7465 7220 6675 6e63  rder filter func
+0000e450: 7469 6f6e 2066 6f72 2066 7265 7175 656e  tion for frequen
+0000e460: 6379 2073 6869 6674 732e 0a0a 2020 2020  cy shifts...    
+0000e470: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
+0000e480: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6569  ---------.    ei
+0000e490: 6776 616c 733a 2061 7272 6179 5f6c 696b  gvals: array_lik
+0000e4a0: 652c 2073 6861 7065 2028 6e5f 6474 2c20  e, shape (n_dt, 
+0000e4b0: 6429 0a20 2020 2020 2020 2045 6967 656e  d).        Eigen
+0000e4c0: 7661 6c75 6520 7665 6374 6f72 7320 666f  value vectors fo
+0000e4d0: 7220 6561 6368 2074 696d 6520 7075 6c73  r each time puls
+0000e4e0: 6520 7365 676d 656e 7420 2a6c 2a20 7769  e segment *l* wi
+0000e4f0: 7468 2074 6865 0a20 2020 2020 2020 2066  th the.        f
+0000e500: 6972 7374 2061 7869 7320 636f 756e 7469  irst axis counti
+0000e510: 6e67 2074 6865 2070 756c 7365 2073 6567  ng the pulse seg
+0000e520: 6d65 6e74 2c20 692e 652e 0a20 2020 2020  ment, i.e..     
+0000e530: 2020 2060 6065 6967 7661 6c73 203d 3d20     ``eigvals == 
+0000e540: 6172 7261 7928 5b44 5f30 2c20 445f 312c  array([D_0, D_1,
+0000e550: 202e 2e2e 5d29 6060 2e0a 2020 2020 6569   ...])``..    ei
+0000e560: 6776 6563 733a 2061 7272 6179 5f6c 696b  gvecs: array_lik
+0000e570: 652c 2073 6861 7065 2028 6e5f 6474 2c20  e, shape (n_dt, 
+0000e580: 642c 2064 290a 2020 2020 2020 2020 4569  d, d).        Ei
+0000e590: 6765 6e76 6563 746f 7220 6d61 7472 6963  genvector matric
+0000e5a0: 6573 2066 6f72 2065 6163 6820 7469 6d65  es for each time
+0000e5b0: 2070 756c 7365 2073 6567 6d65 6e74 202a   pulse segment *
+0000e5c0: 6c2a 2077 6974 6820 7468 650a 2020 2020  l* with the.    
+0000e5d0: 2020 2020 6669 7273 7420 6178 6973 2063      first axis c
+0000e5e0: 6f75 6e74 696e 6720 7468 6520 7075 6c73  ounting the puls
+0000e5f0: 6520 7365 676d 656e 742c 2069 2e65 2e0a  e segment, i.e..
+0000e600: 2020 2020 2020 2020 6060 6569 6776 6563          ``eigvec
+0000e610: 7320 3d3d 2061 7272 6179 285b 565f 302c  s == array([V_0,
+0000e620: 2056 5f31 2c20 2e2e 2e5d 2960 602e 0a20   V_1, ...])``.. 
+0000e630: 2020 2070 726f 7061 6761 746f 7273 3a20     propagators: 
+0000e640: 6172 7261 795f 6c69 6b65 2c20 7368 6170  array_like, shap
+0000e650: 6520 286e 5f64 742b 312c 2064 2c20 6429  e (n_dt+1, d, d)
+0000e660: 0a20 2020 2020 2020 2054 6865 2070 726f  .        The pro
+0000e670: 7061 6761 746f 7273 203a 6d61 7468 3a60  pagators :math:`
+0000e680: 515f 6c20 3d20 505f 6c20 505f 7b6c 2d31  Q_l = P_l P_{l-1
+0000e690: 7d5c 6364 6f74 7320 505f 3060 2061 7320  }\cdots P_0` as 
+0000e6a0: 6120 2864 2c20 6429 0a20 2020 2020 2020  a (d, d).       
+0000e6b0: 2061 7272 6179 2077 6974 6820 2a64 2a20   array with *d* 
+0000e6c0: 7468 6520 6469 6d65 6e73 696f 6e20 6f66  the dimension of
+0000e6d0: 2074 6865 2048 696c 6265 7274 2073 7061   the Hilbert spa
+0000e6e0: 6365 2e0a 2020 2020 6f6d 6567 613a 2061  ce..    omega: a
+0000e6f0: 7272 6179 5f6c 696b 652c 2073 6861 7065  rray_like, shape
+0000e700: 2028 6e5f 6f6d 6567 612c 290a 2020 2020   (n_omega,).    
+0000e710: 2020 2020 4672 6571 7565 6e63 6965 7320      Frequencies 
+0000e720: 6174 2077 6869 6368 2074 6865 2070 756c  at which the pul
+0000e730: 7365 2063 6f6e 7472 6f6c 206d 6174 7269  se control matri
+0000e740: 7820 6973 2074 6f20 6265 0a20 2020 2020  x is to be.     
+0000e750: 2020 2065 7661 6c75 6174 6564 2e0a 2020     evaluated..  
+0000e760: 2020 6261 7369 733a 2042 6173 6973 2c20    basis: Basis, 
+0000e770: 7368 6170 6520 2864 2a2a 322c 2064 2c20  shape (d**2, d, 
+0000e780: 6429 0a20 2020 2020 2020 2054 6865 2062  d).        The b
+0000e790: 6173 6973 2065 6c65 6d65 6e74 7320 696e  asis elements in
+0000e7a0: 2077 6869 6368 2074 6865 2070 756c 7365   which the pulse
+0000e7b0: 2063 6f6e 7472 6f6c 206d 6174 7269 7820   control matrix 
+0000e7c0: 7769 6c6c 2062 650a 2020 2020 2020 2020  will be.        
+0000e7d0: 6578 7061 6e64 6564 2e0a 2020 2020 6e5f  expanded..    n_
+0000e7e0: 6f70 6572 733a 2061 7272 6179 5f6c 696b  opers: array_lik
+0000e7f0: 652c 2073 6861 7065 2028 6e5f 6e6f 7073  e, shape (n_nops
+0000e800: 2c20 642c 2064 290a 2020 2020 2020 2020  , d, d).        
+0000e810: 4e6f 6973 6520 6f70 6572 6174 6f72 7320  Noise operators 
+0000e820: 3a6d 6174 683a 6042 5f5c 616c 7068 6160  :math:`B_\alpha`
+0000e830: 2e0a 2020 2020 6e5f 636f 6566 6673 3a20  ..    n_coeffs: 
+0000e840: 6172 7261 795f 6c69 6b65 2c20 7368 6170  array_like, shap
+0000e850: 6520 286e 5f6e 6f70 732c 206e 5f64 7429  e (n_nops, n_dt)
+0000e860: 0a20 2020 2020 2020 2054 6865 2073 656e  .        The sen
+0000e870: 7369 7469 7669 7469 6573 206f 6620 7468  sitivities of th
+0000e880: 6520 7379 7374 656d 2074 6f20 7468 6520  e system to the 
+0000e890: 6e6f 6973 6520 6f70 6572 6174 6f72 7320  noise operators 
+0000e8a0: 6769 7665 6e20 6279 0a20 2020 2020 2020  given by.       
+0000e8b0: 202a 6e5f 6f70 6572 732a 2061 7420 7468   *n_opers* at th
+0000e8c0: 6520 6769 7665 6e20 7469 6d65 2073 7465  e given time ste
+0000e8d0: 702e 0a20 2020 2064 743a 2061 7272 6179  p..    dt: array
+0000e8e0: 5f6c 696b 652c 2073 6861 7065 2028 6e5f  _like, shape (n_
+0000e8f0: 6474 290a 2020 2020 2020 2020 5365 7175  dt).        Sequ
+0000e900: 656e 6365 2064 7572 6174 696f 6e2c 2069  ence duration, i
+0000e910: 2e65 2e20 666f 7220 7468 6520 3a6d 6174  .e. for the :mat
+0000e920: 683a 606c 602d 7468 2070 756c 7365 0a20  h:`l`-th pulse. 
+0000e930: 2020 2020 2020 203a 6d61 7468 3a60 745f         :math:`t_
+0000e940: 6c20 2d20 745f 7b6c 2d31 7d60 2e0a 2020  l - t_{l-1}`..  
+0000e950: 2020 696e 7465 726d 6564 6961 7465 733a    intermediates:
+0000e960: 2044 6963 745b 7374 722c 206e 6461 7272   Dict[str, ndarr
+0000e970: 6179 5d2c 206f 7074 696f 6e61 6c0a 2020  ay], optional.  
+0000e980: 2020 2020 2020 496e 7465 726d 6564 6961        Intermedia
+0000e990: 7465 2074 6572 6d73 206f 6620 7468 6520  te terms of the 
+0000e9a0: 6361 6c63 756c 6174 696f 6e20 6f66 2074  calculation of t
+0000e9b0: 6865 2063 6f6e 7472 6f6c 206d 6174 7269  he control matri
+0000e9c0: 7820 7468 6174 0a20 2020 2020 2020 2063  x that.        c
+0000e9d0: 616e 2062 6520 7265 7573 6564 2068 6572  an be reused her
+0000e9e0: 652e 2049 6620 4e6f 6e65 2028 6465 6661  e. If None (defa
+0000e9f0: 756c 7429 2c20 7468 6579 2061 7265 2063  ult), they are c
+0000ea00: 6f6d 7075 7465 6420 6672 6f6d 0a20 2020  omputed from.   
+0000ea10: 2020 2020 2073 6372 6174 6368 2e0a 2020       scratch..  
+0000ea20: 2020 7368 6f77 5f70 726f 6772 6573 7362    show_progressb
+0000ea30: 6172 3a20 626f 6f6c 2c20 6f70 7469 6f6e  ar: bool, option
+0000ea40: 616c 0a20 2020 2020 2020 2053 686f 7720  al.        Show 
+0000ea50: 6120 7072 6f67 7265 7373 2062 6172 2066  a progress bar f
+0000ea60: 6f72 2074 6865 2063 616c 6375 6c61 7469  or the calculati
+0000ea70: 6f6e 2e0a 0a20 2020 2052 6574 7572 6e73  on...    Returns
+0000ea80: 0a20 2020 202d 2d2d 2d2d 2d2d 0a20 2020  .    -------.   
+0000ea90: 2073 6563 6f6e 645f 6f72 6465 725f 6669   second_order_fi
+0000eaa0: 6c74 6572 5f66 756e 6374 696f 6e3a 206e  lter_function: n
+0000eab0: 6461 7272 6179 2c20 7368 6170 6520 286e  darray, shape (n
+0000eac0: 5f6e 6f70 732c 206e 5f6e 6f70 732c 2064  _nops, n_nops, d
+0000ead0: 2a2a 322c 2064 2a2a 322c 206e 5f6f 6d65  **2, d**2, n_ome
+0000eae0: 6761 290a 2020 2020 2020 2020 5468 6520  ga).        The 
+0000eaf0: 7365 636f 6e64 206f 7264 6572 2066 696c  second order fil
+0000eb00: 7465 7220 6675 6e63 7469 6f6e 2e0a 0a20  ter function... 
+0000eb10: 2020 202e 2e20 5f6e 6f74 6573 3a0a 0a20     .. _notes:.. 
+0000eb20: 2020 204e 6f74 6573 0a20 2020 202d 2d2d     Notes.    ---
+0000eb30: 2d2d 0a20 2020 2054 6865 2073 6563 6f6e  --.    The secon
+0000eb40: 6420 6f72 6465 7220 6669 6c74 6572 2066  d order filter f
+0000eb50: 756e 6374 696f 6e20 6973 2067 6976 656e  unction is given
+0000eb60: 2062 790a 0a20 2020 202e 2e20 6d61 7468   by..    .. math
+0000eb70: 3a3a 0a0a 2020 2020 2020 2020 465f 7b5c  ::..        F_{\
+0000eb80: 616c 7068 615c 6265 7461 2c20 6b6c 7d5e  alpha\beta, kl}^
+0000eb90: 7b28 3229 7d20 3d20 5c73 756d 5f7b 673d  {(2)} = \sum_{g=
+0000eba0: 317d 5e47 5c6c 6566 745b 0a20 2020 2020  1}^G\left[.     
+0000ebb0: 2020 2020 2020 2020 2020 205c 6d61 7468             \math
+0000ebc0: 6361 6c7b 477d 5f7b 5c61 6c70 6861 206b  cal{G}_{\alpha k
+0000ebd0: 7d5e 7b28 6729 5c61 7374 7d28 5c6f 6d65  }^{(g)\ast}(\ome
+0000ebe0: 6761 290a 2020 2020 2020 2020 2020 2020  ga).            
+0000ebf0: 2020 2020 5c73 756d 5f7b 6727 3d31 7d5e      \sum_{g'=1}^
+0000ec00: 7b67 2d31 7d5c 6d61 7468 6361 6c7b 477d  {g-1}\mathcal{G}
+0000ec10: 5f7b 5c62 6574 6120 6c7d 5e7b 2867 2729  _{\beta l}^{(g')
+0000ec20: 7d28 5c6f 6d65 6761 2920 2b0a 2020 2020  }(\omega) +.    
+0000ec30: 2020 2020 2020 2020 2020 2020 735f 5c61              s_\a
+0000ec40: 6c70 6861 5e7b 2867 297d 5c62 6172 7b42  lpha^{(g)}\bar{B
+0000ec50: 7d5f 7b5c 616c 7068 612c 696a 7d5e 7b28  }_{\alpha,ij}^{(
+0000ec60: 6729 7d5c 6261 727b 437d 5f7b 6b2c 6a69  g)}\bar{C}_{k,ji
+0000ec70: 7d5e 7b28 6729 7d0a 2020 2020 2020 2020  }^{(g)}.        
+0000ec80: 2020 2020 2020 2020 495f 7b69 6a6d 6e7d          I_{ijmn}
+0000ec90: 5e7b 2867 297d 285c 6f6d 6567 6129 5c62  ^{(g)}(\omega)\b
+0000eca0: 6172 7b43 7d5f 7b6c 2c6e 6d7d 5e7b 2867  ar{C}_{l,nm}^{(g
+0000ecb0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000ecc0: 2020 5c62 6172 7b42 7d5f 7b5c 6265 7461    \bar{B}_{\beta
+0000ecd0: 2c6d 6e7d 5e7b 2867 297d 735f 5c62 6574  ,mn}^{(g)}s_\bet
+0000ece0: 615e 7b28 6729 7d7d 0a20 2020 2020 2020  a^{(g)}}.       
+0000ecf0: 2020 2020 205c 7269 6768 745d 0a0a 2020       \right]..  
+0000ed00: 2020 7769 7468 0a0a 2020 2020 2e2e 206d    with..    .. m
+0000ed10: 6174 683a 3a0a 0a20 2020 2020 2020 205c  ath::..        \
+0000ed20: 6d61 7468 6361 6c7b 477d 5e7b 2867 297d  mathcal{G}^{(g)}
+0000ed30: 285c 6f6d 6567 6129 2026 3d0a 2020 2020  (\omega) &=.    
+0000ed40: 2020 2020 2020 2020 655e 7b69 5c6f 6d65          e^{i\ome
+0000ed50: 6761 2074 5f7b 672d 317d 7d5c 6d61 7468  ga t_{g-1}}\math
+0000ed60: 6361 6c7b 427d 5e7b 2867 297d 285c 6f6d  cal{B}^{(g)}(\om
+0000ed70: 6567 6129 0a20 2020 2020 2020 2020 2020  ega).           
+0000ed80: 205c 6d61 7468 6361 6c7b 517d 5e7b 2867   \mathcal{Q}^{(g
+0000ed90: 2d31 297d 2c20 5c5c 0a20 2020 2020 2020  -1)}, \\.       
+0000eda0: 2049 5f7b 696a 6d6e 7d5e 7b28 6729 7d28   I_{ijmn}^{(g)}(
+0000edb0: 5c6f 6d65 6761 2920 263d 0a20 2020 2020  \omega) &=.     
+0000edc0: 2020 2020 2020 205c 696e 745f 7b74 5f7b         \int_{t_{
+0000edd0: 672d 317d 7d5e 7b74 5f67 7d5c 6d61 7468  g-1}}^{t_g}\math
+0000ede0: 726d 7b64 7d7b 747d 0a20 2020 2020 2020  rm{d}{t}.       
+0000edf0: 2020 2020 2065 5e7b 695c 4f6d 6567 615f       e^{i\Omega_
+0000ee00: 7b69 6a7d 5e7b 2867 297d 2874 202d 2074  {ij}^{(g)}(t - t
+0000ee10: 5f7b 672d 317d 2920 2d20 695c 6f6d 6567  _{g-1}) - i\omeg
+0000ee20: 6120 747d 0a20 2020 2020 2020 2020 2020  a t}.           
+0000ee30: 205c 696e 745f 7b74 5f7b 672d 317d 7d5e   \int_{t_{g-1}}^
+0000ee40: 7b74 7d5c 6d61 7468 726d 7b64 7d7b 7427  {t}\mathrm{d}{t'
+0000ee50: 7d0a 2020 2020 2020 2020 2020 2020 655e  }.            e^
+0000ee60: 7b69 5c4f 6d65 6761 5f7b 6d6e 7d5e 7b28  {i\Omega_{mn}^{(
+0000ee70: 6729 7d28 7427 202d 2074 5f7b 672d 317d  g)}(t' - t_{g-1}
+0000ee80: 2920 2b20 695c 6f6d 6567 6120 7427 7d2e  ) + i\omega t'}.
+0000ee90: 0a0a 2020 2020 5365 6520 416c 736f 0a20  ..    See Also. 
+0000eea0: 2020 202d 2d2d 2d2d 2d2d 2d0a 2020 2020     --------.    
+0000eeb0: 6361 6c63 756c 6174 655f 6672 6571 7565  calculate_freque
+0000eec0: 6e63 795f 7368 6966 7473 3a20 496e 7465  ncy_shifts: Inte
+0000eed0: 6772 6174 6520 6f76 6572 2066 696c 7465  grate over filte
+0000eee0: 7220 6675 6e63 7469 6f6e 2074 696d 6573  r function times
+0000eef0: 2073 7065 6374 7275 6d2e 0a20 2020 2063   spectrum..    c
+0000ef00: 616c 6375 6c61 7465 5f64 6563 6179 5f61  alculate_decay_a
+0000ef10: 6d70 6c69 7475 6465 733a 2046 6972 7374  mplitudes: First
+0000ef20: 206f 7264 6572 2028 6469 7373 6970 6174   order (dissipat
+0000ef30: 6976 6529 2074 6572 6d73 2e0a 2020 2020  ive) terms..    
+0000ef40: 696e 6669 6465 6c69 7479 3a20 436f 6d70  infidelity: Comp
+0000ef50: 7574 6520 7468 6520 696e 6669 6465 6c69  ute the infideli
+0000ef60: 7479 2064 6972 6563 746c 792e 0a20 2020  ty directly..   
+0000ef70: 2070 756c 7365 5f73 6571 7565 6e63 652e   pulse_sequence.
+0000ef80: 636f 6e63 6174 656e 6174 653a 2043 6f6e  concatenate: Con
+0000ef90: 6361 7465 6e61 7465 2060 6050 756c 7365  catenate ``Pulse
+0000efa0: 5365 7175 656e 6365 6060 206f 626a 6563  Sequence`` objec
+0000efb0: 7473 2e0a 2020 2020 6361 6c63 756c 6174  ts..    calculat
+0000efc0: 655f 7075 6c73 655f 636f 7272 656c 6174  e_pulse_correlat
+0000efd0: 696f 6e5f 6669 6c74 6572 5f66 756e 6374  ion_filter_funct
+0000efe0: 696f 6e0a 2020 2020 2222 220a 2020 2020  ion.    """.    
+0000eff0: 6420 3d20 6569 6776 616c 732e 7368 6170  d = eigvals.shap
+0000f000: 655b 2d31 5d0a 2020 2020 2320 5765 2772  e[-1].    # We'r
+0000f010: 6520 6c61 7a79 0a20 2020 206e 5f63 6f65  e lazy.    n_coe
+0000f020: 6666 7320 3d20 6e70 2e61 7361 7272 6179  ffs = np.asarray
+0000f030: 286e 5f63 6f65 6666 7329 0a0a 2020 2020  (n_coeffs)..    
+0000f040: 2320 416c 6c6f 6361 7465 2072 6573 756c  # Allocate resul
+0000f050: 7420 616e 6420 6275 6666 6572 7320 666f  t and buffers fo
+0000f060: 7220 696e 7465 726d 6564 6961 7465 2061  r intermediate a
+0000f070: 7272 6179 730a 2020 2020 6445 5f62 7566  rrays.    dE_buf
+0000f080: 7320 3d20 286e 702e 656d 7074 7928 2864  s = (np.empty((d
+0000f090: 2c20 642c 2064 2c20 6429 2c20 6474 7970  , d, d, d), dtyp
+0000f0a0: 653d 666c 6f61 7429 2c0a 2020 2020 2020  e=float),.      
+0000f0b0: 2020 2020 2020 2020 206e 702e 656d 7074           np.empt
+0000f0c0: 7928 286c 656e 286f 6d65 6761 292c 2064  y((len(omega), d
+0000f0d0: 2c20 6429 2c20 6474 7970 653d 666c 6f61  , d), dtype=floa
+0000f0e0: 7429 2c0a 2020 2020 2020 2020 2020 2020  t),.            
+0000f0f0: 2020 206e 702e 656d 7074 7928 286c 656e     np.empty((len
+0000f100: 286f 6d65 6761 292c 2064 2c20 6429 2c20  (omega), d, d), 
+0000f110: 6474 7970 653d 666c 6f61 7429 290a 2020  dtype=float)).  
+0000f120: 2020 6578 705f 6275 6620 3d20 6e70 2e65    exp_buf = np.e
+0000f130: 6d70 7479 2828 6c65 6e28 6f6d 6567 6129  mpty((len(omega)
+0000f140: 2c20 642c 2064 292c 2064 7479 7065 3d63  , d, d), dtype=c
+0000f150: 6f6d 706c 6578 290a 2020 2020 6672 635f  omplex).    frc_
+0000f160: 6275 6673 203d 2028 6e70 2e65 6d70 7479  bufs = (np.empty
+0000f170: 2828 6c65 6e28 6f6d 6567 6129 2c20 642c  ((len(omega), d,
+0000f180: 2064 292c 2064 7479 7065 3d63 6f6d 706c   d), dtype=compl
+0000f190: 6578 292c 0a20 2020 2020 2020 2020 2020  ex),.           
+0000f1a0: 2020 2020 206e 702e 656d 7074 7928 2864       np.empty((d
+0000f1b0: 2c20 642c 2064 2c20 6429 2c20 6474 7970  , d, d, d), dtyp
+0000f1c0: 653d 636f 6d70 6c65 7829 290a 2020 2020  e=complex)).    
+0000f1d0: 696e 745f 6275 6620 3d20 6e70 2e65 6d70  int_buf = np.emp
+0000f1e0: 7479 2828 6c65 6e28 6f6d 6567 6129 2c20  ty((len(omega), 
+0000f1f0: 642c 2064 2c20 642c 2064 292c 2064 7479  d, d, d, d), dty
+0000f200: 7065 3d63 6f6d 706c 6578 290a 2020 2020  pe=complex).    
+0000f210: 6d73 6b5f 6275 6673 203d 206e 702e 656d  msk_bufs = np.em
+0000f220: 7074 7928 2832 2c20 6c65 6e28 6f6d 6567  pty((2, len(omeg
+0000f230: 6129 2c20 642c 2064 2c20 642c 2064 292c  a), d, d, d, d),
+0000f240: 2064 7479 7065 3d62 6f6f 6c29 0a20 2020   dtype=bool).   
+0000f250: 2063 7472 6c6d 6174 5f73 7465 705f 6375   ctrlmat_step_cu
+0000f260: 6d75 6c61 7469 7665 203d 206e 702e 7a65  mulative = np.ze
+0000f270: 726f 7328 286c 656e 286e 5f63 6f65 6666  ros((len(n_coeff
+0000f280: 7329 2c20 6c65 6e28 6261 7369 7329 2c20  s), len(basis), 
+0000f290: 6c65 6e28 6f6d 6567 6129 292c 2064 7479  len(omega)), dty
+0000f2a0: 7065 3d63 6f6d 706c 6578 290a 0a20 2020  pe=complex)..   
+0000f2b0: 2073 6861 7065 203d 2028 6c65 6e28 6e5f   shape = (len(n_
+0000f2c0: 636f 6566 6673 292c 206c 656e 286e 5f63  coeffs), len(n_c
+0000f2d0: 6f65 6666 7329 2c20 6c65 6e28 6261 7369  oeffs), len(basi
+0000f2e0: 7329 2c20 6c65 6e28 6261 7369 7329 2c20  s), len(basis), 
+0000f2f0: 6c65 6e28 6f6d 6567 6129 290a 2020 2020  len(omega)).    
+0000f300: 7374 6570 5f62 7566 203d 206e 702e 656d  step_buf = np.em
+0000f310: 7074 7928 7368 6170 652c 2064 7479 7065  pty(shape, dtype
+0000f320: 3d63 6f6d 706c 6578 290a 2020 2020 7265  =complex).    re
+0000f330: 7375 6c74 203d 206e 702e 7a65 726f 7328  sult = np.zeros(
+0000f340: 7368 6170 652c 2064 7479 7065 3d63 6f6d  shape, dtype=com
+0000f350: 706c 6578 290a 0a20 2020 2023 2069 6e74  plex)..    # int
+0000f360: 6572 6d65 6469 6174 6520 7265 7375 6c74  ermediate result
+0000f370: 7320 6672 6f6d 2063 616c 6375 6c61 7469  s from calculati
+0000f380: 6f6e 206f 6620 636f 6e74 726f 6c20 6d61  on of control ma
+0000f390: 7472 6978 0a20 2020 2069 6620 696e 7465  trix.    if inte
+0000f3a0: 726d 6564 6961 7465 7320 6973 204e 6f6e  rmediates is Non
+0000f3b0: 653a 0a20 2020 2020 2020 2069 6e74 6572  e:.        inter
+0000f3c0: 6d65 6469 6174 6573 203d 2064 6963 7428  mediates = dict(
+0000f3d0: 290a 0a20 2020 2023 2057 6f72 6b20 6172  )..    # Work ar
+0000f3e0: 6f75 6e64 2070 6f73 7369 626c 7920 706f  ound possibly po
+0000f3f0: 7075 6c61 7465 6420 696e 7465 726d 6564  pulated intermed
+0000f400: 6961 7465 7320 6469 6374 2077 6974 6820  iates dict with 
+0000f410: 6d69 7373 696e 6720 6b65 7973 0a20 2020  missing keys.   
+0000f420: 206e 5f6f 7065 7273 5f74 7261 6e73 666f   n_opers_transfo
+0000f430: 726d 6564 203d 2069 6e74 6572 6d65 6469  rmed = intermedi
+0000f440: 6174 6573 2e67 6574 2827 6e5f 6f70 6572  ates.get('n_oper
+0000f450: 735f 7472 616e 7366 6f72 6d65 6427 290a  s_transformed').
+0000f460: 2020 2020 6966 206e 5f6f 7065 7273 5f74      if n_opers_t
+0000f470: 7261 6e73 666f 726d 6564 2069 7320 4e6f  ransformed is No
+0000f480: 6e65 3a0a 2020 2020 2020 2020 6e5f 6f70  ne:.        n_op
+0000f490: 6572 735f 7472 616e 7366 6f72 6d65 6420  ers_transformed 
+0000f4a0: 3d20 5f74 7261 6e73 666f 726d 5f68 616d  = _transform_ham
+0000f4b0: 696c 746f 6e69 616e 2865 6967 7665 6373  iltonian(eigvecs
+0000f4c0: 2c20 6e5f 6f70 6572 732c 206e 5f63 6f65  , n_opers, n_coe
+0000f4d0: 6666 7329 0a0a 2020 2020 7472 793a 0a20  ffs)..    try:. 
+0000f4e0: 2020 2020 2020 2062 6173 6973 5f74 7261         basis_tra
+0000f4f0: 6e73 666f 726d 6564 5f63 6163 6865 203d  nsformed_cache =
+0000f500: 2069 6e74 6572 6d65 6469 6174 6573 5b27   intermediates['
+0000f510: 6261 7369 735f 7472 616e 7366 6f72 6d65  basis_transforme
+0000f520: 6427 5d0a 2020 2020 2020 2020 6374 726c  d'].        ctrl
+0000f530: 6d61 745f 7374 6570 5f63 6163 6865 203d  mat_step_cache =
+0000f540: 2069 6e74 6572 6d65 6469 6174 6573 5b27   intermediates['
+0000f550: 636f 6e74 726f 6c5f 6d61 7472 6978 5f73  control_matrix_s
+0000f560: 7465 7027 5d0a 2020 2020 2020 2020 6861  tep'].        ha
+0000f570: 7665 5f69 6e74 6572 6d65 6469 6174 6573  ve_intermediates
+0000f580: 203d 2054 7275 650a 2020 2020 6578 6365   = True.    exce
+0000f590: 7074 204b 6579 4572 726f 723a 0a20 2020  pt KeyError:.   
+0000f5a0: 2020 2020 2068 6176 655f 696e 7465 726d       have_interm
+0000f5b0: 6564 6961 7465 7320 3d20 4661 6c73 650a  ediates = False.
+0000f5c0: 2020 2020 2020 2020 2320 4e6f 2063 6163          # No cac
+0000f5d0: 6865 2e20 5072 6563 6f6d 7075 7465 2073  he. Precompute s
+0000f5e0: 6f6d 6520 7468 696e 6773 2061 6e64 2070  ome things and p
+0000f5f0: 6572 666f 726d 2074 6865 2063 6f73 746c  erform the costl
+0000f600: 7920 636f 6d70 7574 6174 696f 6e73 0a20  y computations. 
+0000f610: 2020 2020 2020 2023 2064 7572 696e 6720         # during 
+0000f620: 6561 6368 206c 6f6f 7020 6974 6572 6174  each loop iterat
+0000f630: 696f 6e20 6265 6c6f 770a 2020 2020 2020  ion below.      
+0000f640: 2020 7420 3d20 6e70 2e63 6f6e 6361 7465    t = np.concate
+0000f650: 6e61 7465 2828 5b30 5d2c 206e 702e 6173  nate(([0], np.as
+0000f660: 6172 7261 7928 6474 292e 6375 6d73 756d  array(dt).cumsum
+0000f670: 2829 2929 0a20 2020 2020 2020 2065 6967  ())).        eig
+0000f680: 7665 6373 5f70 726f 7061 6761 7465 6420  vecs_propagated 
+0000f690: 3d20 5f70 726f 7061 6761 7465 5f65 6967  = _propagate_eig
+0000f6a0: 656e 7665 6374 6f72 7328 7072 6f70 6167  envectors(propag
+0000f6b0: 6174 6f72 735b 3a2d 315d 2c20 6569 6776  ators[:-1], eigv
+0000f6c0: 6563 7329 0a20 2020 2020 2020 2062 6173  ecs).        bas
+0000f6d0: 6973 5f74 7261 6e73 666f 726d 6564 203d  is_transformed =
+0000f6e0: 206e 702e 656d 7074 7928 6261 7369 732e   np.empty(basis.
+0000f6f0: 7368 6170 652c 2064 7479 7065 3d63 6f6d  shape, dtype=com
+0000f700: 706c 6578 290a 2020 2020 2020 2020 6374  plex).        ct
+0000f710: 726c 6d61 745f 7374 6570 203d 206e 702e  rlmat_step = np.
+0000f720: 7a65 726f 7328 286c 656e 286e 5f63 6f65  zeros((len(n_coe
+0000f730: 6666 7329 2c20 6c65 6e28 6261 7369 7329  ffs), len(basis)
+0000f740: 2c20 6c65 6e28 6f6d 6567 6129 292c 2064  , len(omega)), d
+0000f750: 7479 7065 3d63 6f6d 706c 6578 290a 0a20  type=complex).. 
+0000f760: 2020 2073 7465 705f 6578 7072 203d 206f     step_expr = o
+0000f770: 652e 636f 6e74 7261 6374 5f65 7870 7265  e.contract_expre
+0000f780: 7373 696f 6e28 276f 696a 6d6e 2c61 6b69  ssion('oijmn,aki
+0000f790: 6a2c 626c 6d6e 2d3e 6162 6b6c 6f27 2c20  j,blmn->abklo', 
+0000f7a0: 696e 745f 6275 662e 7368 6170 652c 0a20  int_buf.shape,. 
+0000f7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f7d0: 2020 2020 2020 2a5b 286c 656e 286e 5f63        *[(len(n_c
+0000f7e0: 6f65 6666 7329 2c20 6c65 6e28 6261 7369  oeffs), len(basi
+0000f7f0: 7329 2c20 642c 2064 295d 2a32 2c0a 2020  s), d, d)]*2,.  
+0000f800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f820: 2020 2020 206f 7074 696d 697a 653d 5b28       optimize=[(
+0000f830: 302c 2031 292c 2028 302c 2031 295d 290a  0, 1), (0, 1)]).
+0000f840: 2020 2020 666f 7220 6720 696e 2075 7469      for g in uti
+0000f850: 6c2e 7072 6f67 7265 7373 6261 725f 7261  l.progressbar_ra
+0000f860: 6e67 6528 6c65 6e28 6474 292c 2073 686f  nge(len(dt), sho
+0000f870: 775f 7072 6f67 7265 7373 6261 723d 7368  w_progressbar=sh
+0000f880: 6f77 5f70 726f 6772 6573 7362 6172 2c0a  ow_progressbar,.
+0000f890: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000f8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f8b0: 2020 2020 2020 2020 2020 2020 6f70 7469              opti
-0000f8c0: 6d69 7a65 3d5b 2830 2c20 3129 2c20 2830  mize=[(0, 1), (0
-0000f8d0: 2c20 3129 5d29 0a20 2020 2066 6f72 2067  , 1)]).    for g
-0000f8e0: 2069 6e20 7574 696c 2e70 726f 6772 6573   in util.progres
-0000f8f0: 7362 6172 5f72 616e 6765 286c 656e 2864  sbar_range(len(d
-0000f900: 7429 2c20 7368 6f77 5f70 726f 6772 6573  t), show_progres
-0000f910: 7362 6172 3d73 686f 775f 7072 6f67 7265  sbar=show_progre
-0000f920: 7373 6261 722c 0a20 2020 2020 2020 2020  ssbar,.         
-0000f930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f940: 2020 2020 2020 2020 2020 2064 6573 633d             desc=
-0000f950: 2743 616c 6375 6c61 7469 6e67 2073 6563  'Calculating sec
-0000f960: 6f6e 6420 6f72 6465 7220 4646 2729 3a0a  ond order FF'):.
-0000f970: 2020 2020 2020 2020 6966 206e 6f74 2068          if not h
-0000f980: 6176 655f 696e 7465 726d 6564 6961 7465  ave_intermediate
-0000f990: 733a 0a20 2020 2020 2020 2020 2020 2062  s:.            b
-0000f9a0: 6173 6973 5f74 7261 6e73 666f 726d 6564  asis_transformed
-0000f9b0: 203d 205f 7472 616e 7366 6f72 6d5f 6279   = _transform_by
-0000f9c0: 5f75 6e69 7461 7279 2865 6967 7665 6373  _unitary(eigvecs
-0000f9d0: 5f70 726f 7061 6761 7465 645b 675d 2c20  _propagated[g], 
-0000f9e0: 6261 7369 732c 0a20 2020 2020 2020 2020  basis,.         
-0000f9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fa00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fa10: 2020 2020 2020 2020 2020 2020 206f 7574               out
-0000fa20: 3d62 6173 6973 5f74 7261 6e73 666f 726d  =basis_transform
-0000fa30: 6564 290a 2020 2020 2020 2020 2020 2020  ed).            
-0000fa40: 2320 4e65 6564 2074 6f20 636f 6d70 7574  # Need to comput
-0000fa50: 6520 475e 2867 2920 7369 6e63 6520 6e6f  e G^(g) since no
-0000fa60: 2063 6163 6865 2067 6976 656e 2e20 4669   cache given. Fi
-0000fa70: 7273 7420 696e 6974 6961 6c69 7a65 0a20  rst initialize. 
-0000fa80: 2020 2020 2020 2020 2020 2023 2062 7566             # buf
-0000fa90: 6665 7220 746f 207a 6572 6f2e 2054 6865  fer to zero. The
-0000faa0: 7265 2069 7320 6120 7072 6f62 6162 6c79  re is a probably
-0000fab0: 206c 6f74 7320 6f66 206f 7665 7268 6561   lots of overhea
-0000fac0: 6420 636f 6d70 7574 696e 670a 2020 2020  d computing.    
-0000fad0: 2020 2020 2020 2020 2320 7468 6973 2069          # this i
-0000fae0: 6e64 6976 6964 7561 6c6c 7920 666f 7220  ndividually for 
-0000faf0: 6576 6572 7920 7469 6d65 2073 7465 702e  every time step.
-0000fb00: 0a20 2020 2020 2020 2020 2020 2063 7472  .            ctr
-0000fb10: 6c6d 6174 5f73 7465 705b 3a5d 203d 2030  lmat_step[:] = 0
-0000fb20: 0a20 2020 2020 2020 2020 2020 2063 7472  .            ctr
-0000fb30: 6c6d 6174 5f73 7465 7020 3d20 6361 6c63  lmat_step = calc
-0000fb40: 756c 6174 655f 636f 6e74 726f 6c5f 6d61  ulate_control_ma
-0000fb50: 7472 6978 5f66 726f 6d5f 7363 7261 7463  trix_from_scratc
-0000fb60: 6828 0a20 2020 2020 2020 2020 2020 2020  h(.             
-0000fb70: 2020 2065 6967 7661 6c73 5b67 3a67 2b31     eigvals[g:g+1
-0000fb80: 5d2c 2065 6967 7665 6373 5b67 3a67 2b31  ], eigvecs[g:g+1
-0000fb90: 5d2c 2070 726f 7061 6761 746f 7273 5b67  ], propagators[g
-0000fba0: 3a67 2b32 5d2c 206f 6d65 6761 2c20 6261  :g+2], omega, ba
-0000fbb0: 7369 732c 206e 5f6f 7065 7273 2c0a 2020  sis, n_opers,.  
-0000fbc0: 2020 2020 2020 2020 2020 2020 2020 6e5f                n_
-0000fbd0: 636f 6566 6673 5b3a 2c20 673a 672b 315d  coeffs[:, g:g+1]
-0000fbe0: 2c20 6474 5b67 3a67 2b31 5d2c 2074 3d74  , dt[g:g+1], t=t
-0000fbf0: 5b67 3a67 2b31 5d2c 2073 686f 775f 7072  [g:g+1], show_pr
-0000fc00: 6f67 7265 7373 6261 723d 4661 6c73 652c  ogressbar=False,
-0000fc10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fc20: 2063 6163 6865 5f69 6e74 6572 6d65 6469   cache_intermedi
-0000fc30: 6174 6573 3d46 616c 7365 2c20 6f75 743d  ates=False, out=
-0000fc40: 6374 726c 6d61 745f 7374 6570 0a20 2020  ctrlmat_step.   
-0000fc50: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-0000fc60: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000fc70: 2020 2020 2023 2067 7261 6220 626f 7468       # grab both
-0000fc80: 2066 726f 6d20 6361 6368 650a 2020 2020   from cache.    
-0000fc90: 2020 2020 2020 2020 6261 7369 735f 7472          basis_tr
-0000fca0: 616e 7366 6f72 6d65 6420 3d20 6261 7369  ansformed = basi
-0000fcb0: 735f 7472 616e 7366 6f72 6d65 645f 6361  s_transformed_ca
-0000fcc0: 6368 655b 675d 0a20 2020 2020 2020 2020  che[g].         
-0000fcd0: 2020 2063 7472 6c6d 6174 5f73 7465 7020     ctrlmat_step 
-0000fce0: 3d20 6374 726c 6d61 745f 7374 6570 5f63  = ctrlmat_step_c
-0000fcf0: 6163 6865 5b67 5d0a 0a20 2020 2020 2020  ache[g]..       
-0000fd00: 2069 6e74 5f62 7566 203d 205f 7365 636f   int_buf = _seco
-0000fd10: 6e64 5f6f 7264 6572 5f69 6e74 6567 7261  nd_order_integra
-0000fd20: 6c28 6f6d 6567 612c 2065 6967 7661 6c73  l(omega, eigvals
-0000fd30: 5b67 5d2c 2064 745b 675d 2c20 696e 745f  [g], dt[g], int_
-0000fd40: 6275 662c 0a20 2020 2020 2020 2020 2020  buf,.           
-0000fd50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fd60: 2020 2020 2020 2020 2020 2020 2020 6672                fr
-0000fd70: 635f 6275 6673 2c20 6445 5f62 7566 732c  c_bufs, dE_bufs,
-0000fd80: 2065 7870 5f62 7566 2c20 6d73 6b5f 6275   exp_buf, msk_bu
-0000fd90: 6673 290a 2020 2020 2020 2020 6e5f 6f70  fs).        n_op
-0000fda0: 6572 735f 6261 7369 7320 3d20 6e70 2e65  ers_basis = np.e
-0000fdb0: 696e 7375 6d28 2761 6b6c 2c69 6c6b 2d3e  insum('akl,ilk->
-0000fdc0: 6169 6b6c 272c 206e 5f6f 7065 7273 5f74  aikl', n_opers_t
-0000fdd0: 7261 6e73 666f 726d 6564 5b3a 2c20 675d  ransformed[:, g]
-0000fde0: 2c20 6261 7369 735f 7472 616e 7366 6f72  , basis_transfor
-0000fdf0: 6d65 6429 0a20 2020 2020 2020 2023 2057  med).        # W
-0000fe00: 6520 7573 6520 7374 6570 5f62 7566 2061  e use step_buf a
-0000fe10: 7320 6120 6275 6666 6572 2066 6f72 2074  s a buffer for t
-0000fe20: 6865 206c 6173 7420 696e 7465 7276 616c  he last interval
-0000fe30: 2028 7769 7468 206e 6573 7465 6420 7469   (with nested ti
-0000fe40: 6d65 0a20 2020 2020 2020 2023 2064 6570  me.        # dep
-0000fe50: 656e 6465 6e63 6529 2061 6e64 2061 6674  endence) and aft
-0000fe60: 6572 7761 7264 7320 7468 6520 696e 7465  erwards the inte
-0000fe70: 7276 616c 7320 7570 2074 6f20 7468 6520  rvals up to the 
-0000fe80: 6c61 7374 2028 7768 6572 6520 7468 650a  last (where the.
-0000fe90: 2020 2020 2020 2020 2320 7469 6d65 2064          # time d
-0000fea0: 6570 656e 6465 6e63 6520 7365 7061 7261  ependence separa
-0000feb0: 7465 7320 616e 6420 7765 2063 616e 2075  tes and we can u
-0000fec0: 7365 2070 7265 7669 6f75 7320 7265 7375  se previous resu
-0000fed0: 6c74 2066 6f72 2074 6865 0a20 2020 2020  lt for the.     
-0000fee0: 2020 2023 2063 6f6e 7472 6f6c 206d 6174     # control mat
-0000fef0: 7269 7829 2e20 6f70 745f 6569 6e73 756d  rix). opt_einsum
-0000ff00: 2073 6565 6d73 2074 6f20 6265 2066 6173   seems to be fas
-0000ff10: 7465 7220 7468 616e 206e 756d 7079 2068  ter than numpy h
-0000ff20: 6572 652e 0a20 2020 2020 2020 2073 7465  ere..        ste
-0000ff30: 705f 6275 6620 3d20 7374 6570 5f65 7870  p_buf = step_exp
-0000ff40: 7228 696e 745f 6275 662c 206e 5f6f 7065  r(int_buf, n_ope
-0000ff50: 7273 5f62 6173 6973 2c20 6e5f 6f70 6572  rs_basis, n_oper
-0000ff60: 735f 6261 7369 732c 206f 7574 3d73 7465  s_basis, out=ste
-0000ff70: 705f 6275 6629 0a0a 2020 2020 2020 2020  p_buf)..        
-0000ff80: 7265 7375 6c74 202b 3d20 7374 6570 5f62  result += step_b
-0000ff90: 7566 2020 2320 6c61 7374 2069 6e74 6572  uf  # last inter
-0000ffa0: 7661 6c0a 2020 2020 2020 2020 6966 2067  val.        if g
-0000ffb0: 203e 2030 3a0a 2020 2020 2020 2020 2020   > 0:.          
-0000ffc0: 2020 7374 6570 5f62 7566 203d 206e 702e    step_buf = np.
-0000ffd0: 6569 6e73 756d 2827 616b 6f2c 626c 6f2d  einsum('ako,blo-
-0000ffe0: 3e61 626b 6c6f 272c 2063 7472 6c6d 6174  >abklo', ctrlmat
-0000fff0: 5f73 7465 702e 636f 6e6a 2829 2c20 6374  _step.conj(), ct
-00010000: 726c 6d61 745f 7374 6570 5f63 756d 756c  rlmat_step_cumul
-00010010: 6174 6976 652c 0a20 2020 2020 2020 2020  ative,.         
-00010020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010030: 2020 2020 2020 2020 6f75 743d 7374 6570          out=step
-00010040: 5f62 7566 290a 0a20 2020 2020 2020 2020  _buf)..         
-00010050: 2020 2072 6573 756c 7420 2b3d 2073 7465     result += ste
-00010060: 705f 6275 6620 2023 2061 6c6c 2069 6e74  p_buf  # all int
-00010070: 6572 7661 6c73 2075 7020 746f 206c 6173  ervals up to las
-00010080: 740a 0a20 2020 2020 2020 2069 6620 6720  t..        if g 
-00010090: 3c20 6c65 6e28 6474 2920 2d20 313a 0a20  < len(dt) - 1:. 
-000100a0: 2020 2020 2020 2020 2020 2023 2041 6464             # Add
-000100b0: 2047 5e28 672d 3129 2074 6f20 6375 6d75   G^(g-1) to cumu
-000100c0: 6c61 7469 7665 2073 756d 2066 6f72 2031  lative sum for 1
-000100d0: 203c 2067 203c 2047 2c20 666f 7220 673d   < g < G, for g=
-000100e0: 3020 6974 2773 0a20 2020 2020 2020 2020  0 it's.         
-000100f0: 2020 2023 207a 6572 6f2c 2066 6f72 2047     # zero, for G
-00010100: 2069 7427 7320 6e6f 7420 7265 7175 6972   it's not requir
-00010110: 6564 2061 7320 7468 6520 6c6f 6f70 2074  ed as the loop t
-00010120: 6572 6d69 6e61 7465 730a 2020 2020 2020  erminates.      
-00010130: 2020 2020 2020 6374 726c 6d61 745f 7374        ctrlmat_st
-00010140: 6570 5f63 756d 756c 6174 6976 6520 2b3d  ep_cumulative +=
-00010150: 2063 7472 6c6d 6174 5f73 7465 700a 0a20   ctrlmat_step.. 
-00010160: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
-00010170: 0a0a 0a40 7574 696c 2e70 6172 7365 5f6f  ...@util.parse_o
-00010180: 7074 696f 6e61 6c5f 7061 7261 6d65 7465  ptional_paramete
-00010190: 7273 2877 6869 6368 3d28 2766 6964 656c  rs(which=('fidel
-000101a0: 6974 7927 2c20 2767 656e 6572 616c 697a  ity', 'generaliz
-000101b0: 6564 2729 290a 6465 6620 6361 6c63 756c  ed')).def calcul
-000101c0: 6174 655f 7075 6c73 655f 636f 7272 656c  ate_pulse_correl
-000101d0: 6174 696f 6e5f 6669 6c74 6572 5f66 756e  ation_filter_fun
-000101e0: 6374 696f 6e28 636f 6e74 726f 6c5f 6d61  ction(control_ma
-000101f0: 7472 6978 3a20 6e64 6172 7261 792c 0a20  trix: ndarray,. 
-00010200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010220: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-00010230: 6869 6368 3a20 7374 7220 3d20 2766 6964  hich: str = 'fid
-00010240: 656c 6974 7927 2920 2d3e 206e 6461 7272  elity') -> ndarr
-00010250: 6179 3a0a 2020 2020 7222 2222 436f 6d70  ay:.    r"""Comp
-00010260: 7574 6520 7075 6c73 6520 636f 7272 656c  ute pulse correl
-00010270: 6174 696f 6e20 6669 6c74 6572 2066 756e  ation filter fun
-00010280: 6374 696f 6e20 6672 6f6d 2063 6f6e 7472  ction from contr
-00010290: 6f6c 206d 6174 7269 782e 0a0a 2020 2020  ol matrix...    
-000102a0: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
-000102b0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 636f  ---------.    co
-000102c0: 6e74 726f 6c5f 6d61 7472 6978 3a20 6172  ntrol_matrix: ar
-000102d0: 7261 795f 6c69 6b65 2c20 7368 6170 6520  ray_like, shape 
-000102e0: 286e 5f70 756c 7365 732c 206e 5f6e 6f70  (n_pulses, n_nop
-000102f0: 732c 2064 2a2a 322c 206e 5f6f 6d65 6761  s, d**2, n_omega
-00010300: 290a 2020 2020 2020 2020 5468 6520 636f  ).        The co
-00010310: 6e74 726f 6c20 6d61 7472 6978 2e0a 2020  ntrol matrix..  
-00010320: 2020 7768 6963 6820 3a20 7374 722c 206f    which : str, o
-00010330: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
-00010340: 5768 6963 6820 6669 6c74 6572 2066 756e  Which filter fun
-00010350: 6374 696f 6e20 746f 2072 6574 7572 6e2e  ction to return.
-00010360: 2045 6974 6865 7220 2766 6964 656c 6974   Either 'fidelit
-00010370: 7927 2028 6465 6661 756c 7429 206f 720a  y' (default) or.
-00010380: 2020 2020 2020 2020 2767 656e 6572 616c          'general
-00010390: 697a 6564 2720 2873 6565 203a 7265 663a  ized' (see :ref:
-000103a0: 604e 6f74 6573 203c 6e6f 7465 733e 6029  `Notes <notes>`)
-000103b0: 2e0a 0a20 2020 2052 6574 7572 6e73 0a20  ...    Returns. 
-000103c0: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2066     -------.    f
-000103d0: 696c 7465 725f 6675 6e63 7469 6f6e 5f70  ilter_function_p
-000103e0: 633a 206e 6461 7272 6179 2c20 7368 6170  c: ndarray, shap
-000103f0: 6520 286e 5f70 6c73 2c20 6e5f 706c 732c  e (n_pls, n_pls,
-00010400: 206e 5f6e 6f70 732c 206e 5f6e 6f70 732c   n_nops, n_nops,
-00010410: 205b 642a 2a32 2c20 642a 2a32 2c5d 206e   [d**2, d**2,] n
-00010420: 5f6f 6d65 6761 290a 2020 2020 2020 2020  _omega).        
-00010430: 5468 6520 7075 6c73 6520 636f 7272 656c  The pulse correl
-00010440: 6174 696f 6e20 6669 6c74 6572 2066 756e  ation filter fun
-00010450: 6374 696f 6e73 2066 6f72 2065 6163 6820  ctions for each 
-00010460: 7075 6c73 6520 616e 6420 6e6f 6973 650a  pulse and noise.
-00010470: 2020 2020 2020 2020 6f70 6572 6174 6f72          operator
-00010480: 2063 6f72 7265 6c61 7469 6f6e 732e 2054   correlations. T
-00010490: 6865 2066 6972 7374 2074 776f 2061 7865  he first two axe
-000104a0: 7320 686f 6c64 2074 6865 2070 756c 7365  s hold the pulse
-000104b0: 0a20 2020 2020 2020 2063 6f72 7265 6c61  .        correla
-000104c0: 7469 6f6e 732c 2074 6865 2073 6563 6f6e  tions, the secon
-000104d0: 6420 7477 6f20 7468 6520 6e6f 6973 6520  d two the noise 
-000104e0: 636f 7272 656c 6174 696f 6e73 2e0a 2020  correlations..  
-000104f0: 2020 7768 6963 6820 3a20 7374 722c 206f    which : str, o
-00010500: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
-00010510: 5768 6963 6820 6669 6c74 6572 2066 756e  Which filter fun
-00010520: 6374 696f 6e20 746f 2072 6574 7572 6e2e  ction to return.
-00010530: 2045 6974 6865 7220 2766 6964 656c 6974   Either 'fidelit
-00010540: 7927 2028 6465 6661 756c 7429 206f 720a  y' (default) or.
-00010550: 2020 2020 2020 2020 2767 656e 6572 616c          'general
-00010560: 697a 6564 2720 2873 6565 203a 7265 663a  ized' (see :ref:
-00010570: 604e 6f74 6573 203c 6e6f 7465 733e 6029  `Notes <notes>`)
-00010580: 2e0a 0a20 2020 202e 2e20 5f6e 6f74 6573  ...    .. _notes
-00010590: 3a0a 0a20 2020 204e 6f74 6573 0a20 2020  :..    Notes.   
-000105a0: 202d 2d2d 2d2d 0a20 2020 2054 6865 2067   -----.    The g
-000105b0: 656e 6572 616c 697a 6564 2070 756c 7365  eneralized pulse
-000105c0: 2063 6f72 7265 6c61 7469 6f6e 2066 696c   correlation fil
-000105d0: 7465 7220 6675 6e63 7469 6f6e 2069 7320  ter function is 
-000105e0: 6769 7665 6e20 6279 0a0a 2020 2020 2e2e  given by..    ..
-000105f0: 206d 6174 683a 3a0a 0a20 2020 2020 2020   math::..       
-00010600: 2046 5f7b 5c61 6c70 6861 5c62 6574 612c   F_{\alpha\beta,
-00010610: 6b6c 7d5e 7b28 6767 2729 7d28 5c6f 6d65  kl}^{(gg')}(\ome
-00010620: 6761 2920 3d20 5c62 6967 6c5b 0a20 2020  ga) = \bigl[.   
-00010630: 2020 2020 2020 2020 205c 6d61 7468 6361           \mathca
-00010640: 6c7b 517d 5e7b 2867 272d 3129 5c64 6167  l{Q}^{(g'-1)\dag
-00010650: 6765 727d 0a20 2020 2020 2020 2020 2020  ger}.           
-00010660: 205c 7469 6c64 657b 5c6d 6174 6863 616c   \tilde{\mathcal
-00010670: 7b42 7d7d 5e7b 2867 2729 5c64 6167 6765  {B}}^{(g')\dagge
-00010680: 727d 285c 6f6d 6567 6129 0a20 2020 2020  r}(\omega).     
-00010690: 2020 205c 6269 6772 5d5f 7b6b 5c61 6c70     \bigr]_{k\alp
-000106a0: 6861 7d20 5c62 6967 6c5b 0a20 2020 2020  ha} \bigl[.     
-000106b0: 2020 2020 2020 205c 7469 6c64 657b 5c6d         \tilde{\m
-000106c0: 6174 6863 616c 7b42 7d7d 5e7b 2867 297d  athcal{B}}^{(g)}
-000106d0: 285c 6f6d 6567 6129 5c6d 6174 6863 616c  (\omega)\mathcal
-000106e0: 7b51 7d5e 7b28 672d 3129 7d0a 2020 2020  {Q}^{(g-1)}.    
-000106f0: 2020 2020 5c62 6967 725d 5f7b 5c62 6574      \bigr]_{\bet
-00010700: 6120 6c7d 2065 5e7b 695c 6f6d 6567 6128  a l} e^{i\omega(
-00010710: 745f 7b67 2d31 7d20 2d20 745f 7b67 272d  t_{g-1} - t_{g'-
-00010720: 317d 297d 2c0a 0a20 2020 2077 6974 6820  1})},..    with 
-00010730: 3a6d 6174 683a 605c 7469 6c64 657b 5c6d  :math:`\tilde{\m
-00010740: 6174 6863 616c 7b42 7d7d 5e7b 2867 297d  athcal{B}}^{(g)}
-00010750: 6020 7468 6520 636f 6e74 726f 6c20 6d61  ` the control ma
-00010760: 7472 6978 206f 6620 7468 650a 2020 2020  trix of the.    
-00010770: 3a6d 6174 683a 6067 602d 7468 2070 756c  :math:`g`-th pul
-00010780: 7365 2e20 5468 6520 6669 6465 6c69 7479  se. The fidelity
-00010790: 2070 756c 7365 2063 6f72 7265 6c61 7469   pulse correlati
-000107a0: 6f6e 2066 756e 6374 696f 6e20 6973 0a20  on function is. 
-000107b0: 2020 206f 6274 6169 6e65 6420 6279 2074     obtained by t
-000107c0: 7261 6369 6e67 206f 7574 2074 6865 2062  racing out the b
-000107d0: 6173 6973 2069 6e64 6963 6573 2c0a 0a20  asis indices,.. 
-000107e0: 2020 202e 2e20 6d61 7468 3a3a 0a0a 2020     .. math::..  
-000107f0: 2020 2020 2020 465f 7b5c 616c 7068 615c        F_{\alpha\
-00010800: 6265 7461 7d5e 7b28 6767 2729 7d28 5c6f  beta}^{(gg')}(\o
-00010810: 6d65 6761 2920 3d0a 2020 2020 2020 2020  mega) =.        
-00010820: 2020 5c73 756d 5f7b 6b7d 2046 5f7b 5c61    \sum_{k} F_{\a
-00010830: 6c70 6861 5c62 6574 612c 6b6b 7d5e 7b28  lpha\beta,kk}^{(
-00010840: 6767 2729 7d28 5c6f 6d65 6761 290a 0a20  gg')}(\omega).. 
-00010850: 2020 2053 6565 2041 6c73 6f0a 2020 2020     See Also.    
-00010860: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2063 616c  --------.    cal
-00010870: 6375 6c61 7465 5f63 6f6e 7472 6f6c 5f6d  culate_control_m
-00010880: 6174 7269 785f 6672 6f6d 5f73 6372 6174  atrix_from_scrat
-00010890: 6368 3a20 436f 6e74 726f 6c20 6d61 7472  ch: Control matr
-000108a0: 6978 2066 726f 6d20 7363 7261 7463 682e  ix from scratch.
-000108b0: 0a20 2020 2063 616c 6375 6c61 7465 5f63  .    calculate_c
-000108c0: 6f6e 7472 6f6c 5f6d 6174 7269 785f 6672  ontrol_matrix_fr
-000108d0: 6f6d 5f61 746f 6d69 633a 2043 6f6e 7472  om_atomic: Contr
-000108e0: 6f6c 206d 6174 7269 7820 6672 6f6d 2063  ol matrix from c
-000108f0: 6f6e 6361 7465 6e61 7469 6f6e 2e0a 2020  oncatenation..  
-00010900: 2020 6361 6c63 756c 6174 655f 6669 6c74    calculate_filt
-00010910: 6572 5f66 756e 6374 696f 6e3a 2052 6567  er_function: Reg
-00010920: 756c 6172 2066 696c 7465 7220 6675 6e63  ular filter func
-00010930: 7469 6f6e 2e0a 2020 2020 2222 220a 2020  tion..    """.  
-00010940: 2020 6966 2063 6f6e 7472 6f6c 5f6d 6174    if control_mat
-00010950: 7269 782e 6e64 696d 2021 3d20 343a 0a20  rix.ndim != 4:. 
-00010960: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
-00010970: 7565 4572 726f 7228 2745 7870 6563 7465  ueError('Expecte
-00010980: 6420 636f 6e74 726f 6c5f 6d61 7472 6978  d control_matrix
-00010990: 2e6e 6469 6d20 3d3d 2034 2e27 290a 0a20  .ndim == 4.').. 
-000109a0: 2020 2069 6620 7768 6963 6820 3d3d 2027     if which == '
-000109b0: 6669 6465 6c69 7479 273a 0a20 2020 2020  fidelity':.     
-000109c0: 2020 2073 7562 7363 7269 7074 7320 3d20     subscripts = 
-000109d0: 2767 616b 6f2c 6862 6b6f 2d3e 6768 6162  'gako,hbko->ghab
-000109e0: 6f27 0a20 2020 2065 6c73 653a 0a20 2020  o'.    else:.   
-000109f0: 2020 2020 2023 2077 6869 6368 203d 3d20       # which == 
-00010a00: 2767 656e 6572 616c 697a 6564 270a 2020  'generalized'.  
-00010a10: 2020 2020 2020 7375 6273 6372 6970 7473        subscripts
-00010a20: 203d 2027 6761 6b6f 2c68 626c 6f2d 3e67   = 'gako,hblo->g
-00010a30: 6861 626b 6c6f 270a 0a20 2020 2072 6574  habklo'..    ret
-00010a40: 7572 6e20 6e70 2e65 696e 7375 6d28 7375  urn np.einsum(su
-00010a50: 6273 6372 6970 7473 2c20 636f 6e74 726f  bscripts, contro
-00010a60: 6c5f 6d61 7472 6978 2e63 6f6e 6a28 292c  l_matrix.conj(),
-00010a70: 2063 6f6e 7472 6f6c 5f6d 6174 7269 7829   control_matrix)
-00010a80: 0a0a 0a64 6566 2064 6961 676f 6e61 6c69  ...def diagonali
-00010a90: 7a65 2868 616d 696c 746f 6e69 616e 3a20  ze(hamiltonian: 
-00010aa0: 6e64 6172 7261 792c 2064 743a 2043 6f65  ndarray, dt: Coe
-00010ab0: 6666 6963 6965 6e74 7329 202d 3e20 5475  fficients) -> Tu
-00010ac0: 706c 655b 6e64 6172 7261 795d 3a0a 2020  ple[ndarray]:.  
-00010ad0: 2020 7222 2222 4469 6167 6f6e 616c 697a    r"""Diagonaliz
-00010ae0: 6520 6120 4861 6d69 6c74 6f6e 6961 6e2e  e a Hamiltonian.
-00010af0: 0a0a 2020 2020 4469 6167 6f6e 616c 697a  ..    Diagonaliz
-00010b00: 6520 7468 6520 4861 6d69 6c74 6f6e 6961  e the Hamiltonia
-00010b10: 6e20 7768 6963 6820 6973 2070 6965 6365  n which is piece
-00010b20: 7769 7365 2063 6f6e 7374 616e 7420 6475  wise constant du
-00010b30: 7269 6e67 2074 6865 0a20 2020 2074 696d  ring the.    tim
-00010b40: 6573 2067 6976 656e 2062 7920 2a64 742a  es given by *dt*
-00010b50: 2061 6e64 2072 6574 7572 6e20 6569 6765   and return eige
-00010b60: 6e76 616c 7565 732c 2065 6967 656e 7665  nvalues, eigenve
-00010b70: 6374 6f72 732c 2061 6e64 2074 6865 0a20  ctors, and the. 
-00010b80: 2020 2063 756d 756c 6174 6976 6520 7072     cumulative pr
-00010b90: 6f70 6167 6174 6f72 7320 3a6d 6174 683a  opagators :math:
-00010ba0: 6051 5f6c 602e 204e 6f74 6520 7468 6174  `Q_l`. Note that
-00010bb0: 2077 6520 6361 6c63 756c 6174 6520 696e   we calculate in
-00010bc0: 2075 6e69 7473 0a20 2020 2077 6865 7265   units.    where
-00010bd0: 203a 6d61 7468 3a60 5c68 6261 725c 6571   :math:`\hbar\eq
-00010be0: 7569 7620 3160 2073 6f20 7468 6174 0a0a  uiv 1` so that..
-00010bf0: 2020 2020 2e2e 206d 6174 683a 3a0a 0a20      .. math::.. 
-00010c00: 2020 2020 2020 2055 2874 2c20 745f 3029         U(t, t_0)
-00010c10: 203d 205c 6d61 7468 6361 6c7b 547d 5c65   = \mathcal{T}\e
-00010c20: 7870 5c6c 6566 7428 0a20 2020 2020 2020  xp\left(.       
-00010c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010c40: 202d 695c 696e 745f 7b74 5f30 7d5e 745c   -i\int_{t_0}^t\
-00010c50: 6d61 7468 726d 7b64 7d74 275c 6d61 7468  mathrm{d}t'\math
-00010c60: 6361 6c7b 487d 2874 2729 0a20 2020 2020  cal{H}(t').     
-00010c70: 2020 2020 2020 2020 2020 2020 2020 205c                 \
-00010c80: 7269 6768 7429 2e0a 0a20 2020 2050 6172  right)...    Par
-00010c90: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
-00010ca0: 2d2d 2d2d 2d2d 0a20 2020 2068 616d 696c  ------.    hamil
-00010cb0: 746f 6e69 616e 3a20 6172 7261 795f 6c69  tonian: array_li
-00010cc0: 6b65 2c20 7368 6170 6520 286e 5f64 742c  ke, shape (n_dt,
-00010cd0: 2064 2c20 6429 0a20 2020 2020 2020 2048   d, d).        H
-00010ce0: 616d 696c 746f 6e69 616e 206f 6620 7368  amiltonian of sh
-00010cf0: 6170 6520 286e 5f64 742c 2064 2c20 6429  ape (n_dt, d, d)
-00010d00: 2077 6974 6820 6420 7468 6520 6469 6d65   with d the dime
-00010d10: 6e73 696f 6e61 6c69 7479 206f 660a 2020  nsionality of.  
-00010d20: 2020 2020 2020 7468 6520 7379 7374 656d        the system
-00010d30: 0a20 2020 2064 743a 2061 7272 6179 5f6c  .    dt: array_l
-00010d40: 696b 650a 2020 2020 2020 2020 5468 6520  ike.        The 
-00010d50: 7469 6d65 2064 6966 6665 7265 6e63 6573  time differences
-00010d60: 0a0a 2020 2020 5265 7475 726e 730a 2020  ..    Returns.  
-00010d70: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 6569    -------.    ei
-00010d80: 6776 616c 733a 206e 6461 7272 6179 0a20  gvals: ndarray. 
-00010d90: 2020 2020 2020 2041 7272 6179 206f 6620         Array of 
-00010da0: 6569 6765 6e76 616c 7565 7320 6f66 2073  eigenvalues of s
-00010db0: 6861 7065 2028 6e5f 6474 2c20 6429 0a20  hape (n_dt, d). 
-00010dc0: 2020 2065 6967 7665 6373 3a20 6e64 6172     eigvecs: ndar
-00010dd0: 7261 790a 2020 2020 2020 2020 4172 7261  ray.        Arra
-00010de0: 7920 6f66 2065 6967 656e 7665 6374 6f72  y of eigenvector
-00010df0: 7320 6f66 2073 6861 7065 2028 6e5f 6474  s of shape (n_dt
-00010e00: 2c20 642c 2064 290a 2020 2020 7072 6f70  , d, d).    prop
-00010e10: 6167 6174 6f72 733a 206e 6461 7272 6179  agators: ndarray
-00010e20: 0a20 2020 2020 2020 2041 7272 6179 206f  .        Array o
-00010e30: 6620 6375 6d75 6c61 7469 7665 2070 726f  f cumulative pro
-00010e40: 7061 6761 746f 7273 206f 6620 7368 6170  pagators of shap
-00010e50: 6520 286e 5f64 742b 312c 2064 2c20 6429  e (n_dt+1, d, d)
-00010e60: 0a20 2020 2022 2222 0a20 2020 2064 203d  .    """.    d =
-00010e70: 2068 616d 696c 746f 6e69 616e 2e73 6861   hamiltonian.sha
-00010e80: 7065 5b2d 315d 0a20 2020 2023 2043 616c  pe[-1].    # Cal
-00010e90: 6375 6c61 7465 2045 6967 656e 7661 6c75  culate Eigenvalu
-00010ea0: 6573 2061 6e64 202d 7665 6374 6f72 730a  es and -vectors.
-00010eb0: 2020 2020 6569 6776 616c 732c 2065 6967      eigvals, eig
-00010ec0: 7665 6373 203d 206e 6c61 2e65 6967 6828  vecs = nla.eigh(
-00010ed0: 6861 6d69 6c74 6f6e 6961 6e29 0a20 2020  hamiltonian).   
-00010ee0: 2023 2050 726f 7061 6761 746f 7220 5020   # Propagator P 
-00010ef0: 3d20 5620 6578 7028 2d6a 2044 2064 7429  = V exp(-j D dt)
-00010f00: 2056 5e5c 6461 672e 204d 6964 646c 6520   V^\dag. Middle 
-00010f10: 7465 726d 2069 7320 6f66 2073 6861 7065  term is of shape
-00010f20: 0a20 2020 2023 2028 642c 206e 5f64 7429  .    # (d, n_dt)
-00010f30: 2064 7565 2074 6f20 7472 616e 7370 6f73   due to transpos
-00010f40: 652c 2073 6f20 7377 6974 6368 2061 726f  e, so switch aro
-00010f50: 756e 6420 696e 6469 6365 7320 696e 2065  und indices in e
-00010f60: 696e 7375 6d0a 2020 2020 2320 696e 7374  insum.    # inst
-00010f70: 6561 6420 6f66 2074 7261 6e73 706f 7369  ead of transposi
-00010f80: 6e67 2061 6761 696e 2e20 5361 6d65 2067  ng again. Same g
-00010f90: 6f65 7320 666f 7220 7468 6520 6c61 7374  oes for the last
-00010fa0: 2074 6572 6d2e 2054 6869 7320 7361 7665   term. This save
-00010fb0: 730a 2020 2020 2320 6120 6269 7420 6f66  s.    # a bit of
-00010fc0: 2074 696d 652e 2054 6865 2066 6f6c 6c6f   time. The follo
-00010fd0: 7769 6e67 2069 7320 6661 7374 6572 2066  wing is faster f
-00010fe0: 6f72 206c 6172 6765 7220 6469 6d65 6e73  or larger dimens
-00010ff0: 696f 6e73 2062 7574 206e 6f74 2066 6f72  ions but not for
-00011000: 0a20 2020 2023 206d 616e 7920 7469 6d65  .    # many time
-00011010: 2073 7465 7073 3a0a 2020 2020 2320 5020   steps:.    # P 
-00011020: 3d20 6e70 2e65 6d70 7479 2828 3530 302c  = np.empty((500,
-00011030: 2034 2c20 3429 2c20 6474 7970 653d 636f   4, 4), dtype=co
-00011040: 6d70 6c65 7829 0a20 2020 2023 2066 6f72  mplex).    # for
-00011050: 206c 2c20 2856 2c20 4429 2069 6e20 656e   l, (V, D) in en
-00011060: 756d 6572 6174 6528 7a69 7028 6569 6776  umerate(zip(eigv
-00011070: 6563 732c 206e 702e 6578 7028 2d31 6a2a  ecs, np.exp(-1j*
-00011080: 6474 2a65 6967 7661 6c73 2e54 292e 5429  dt*eigvals.T).T)
-00011090: 293a 0a20 2020 2023 2020 2020 2050 5b6c  ):.    #     P[l
-000110a0: 5d20 3d20 2856 202a 2044 2920 4020 562e  ] = (V * D) @ V.
-000110b0: 636f 6e6a 2829 2e54 0a20 2020 2070 6965  conj().T.    pie
-000110c0: 6365 7769 7365 203d 206e 702e 6569 6e73  cewise = np.eins
-000110d0: 756d 2827 6c69 6a2c 6a6c 2c6c 6b6a 2d3e  um('lij,jl,lkj->
-000110e0: 6c69 6b27 2c0a 2020 2020 2020 2020 2020  lik',.          
-000110f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011100: 6569 6776 6563 732c 2075 7469 6c2e 6365  eigvecs, util.ce
-00011110: 7870 282d 6e70 2e61 7361 7272 6179 2864  xp(-np.asarray(d
-00011120: 7429 2a65 6967 7661 6c73 2e54 292c 2065  t)*eigvals.T), e
-00011130: 6967 7665 6373 2e63 6f6e 6a28 2929 0a20  igvecs.conj()). 
-00011140: 2020 2023 2054 6865 2063 756d 756c 6174     # The cumulat
-00011150: 6976 6520 7072 6f70 6167 6174 6f72 2051  ive propagator Q
-00011160: 2077 6974 6820 7468 6520 6964 656e 7469   with the identi
-00011170: 7479 206f 7065 7261 746f 7220 6173 2066  ty operator as f
-00011180: 6972 7374 0a20 2020 2023 2065 6c65 6d65  irst.    # eleme
-00011190: 6e74 2028 515f 3020 3d20 505f 3020 3d20  nt (Q_0 = P_0 = 
-000111a0: 4929 2c20 692e 652e 0a20 2020 2023 2051  I), i.e..    # Q
-000111b0: 203d 205b 515f 302c 2051 5f31 2c20 2e2e   = [Q_0, Q_1, ..
-000111c0: 2e2c 2051 5f6e 5d20 3d20 5b50 5f30 2c20  ., Q_n] = [P_0, 
-000111d0: 505f 3120 4020 505f 302c 202e 2e2e 2c20  P_1 @ P_0, ..., 
-000111e0: 505f 6e20 4020 2e2e 2e20 4020 505f 305d  P_n @ ... @ P_0]
-000111f0: 0a20 2020 2063 756d 756c 6174 6976 6520  .    cumulative 
-00011200: 3d20 6e70 2e65 6d70 7479 2828 6c65 6e28  = np.empty((len(
-00011210: 6474 292b 312c 2064 2c20 6429 2c20 6474  dt)+1, d, d), dt
-00011220: 7970 653d 636f 6d70 6c65 7829 0a20 2020  ype=complex).   
-00011230: 2063 756d 756c 6174 6976 655b 305d 203d   cumulative[0] =
-00011240: 206e 702e 6964 656e 7469 7479 2864 290a   np.identity(d).
-00011250: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-00011260: 6765 286c 656e 2864 7429 293a 0a20 2020  ge(len(dt)):.   
-00011270: 2020 2020 2063 756d 756c 6174 6976 655b       cumulative[
-00011280: 692b 315d 203d 2070 6965 6365 7769 7365  i+1] = piecewise
-00011290: 5b69 5d20 4020 6375 6d75 6c61 7469 7665  [i] @ cumulative
-000112a0: 5b69 5d0a 0a20 2020 2072 6574 7572 6e20  [i]..    return 
-000112b0: 6569 6776 616c 732c 2065 6967 7665 6373  eigvals, eigvecs
-000112c0: 2c20 6375 6d75 6c61 7469 7665 0a0a 0a64  , cumulative...d
-000112d0: 6566 2065 7272 6f72 5f74 7261 6e73 6665  ef error_transfe
-000112e0: 725f 6d61 7472 6978 280a 2020 2020 2020  r_matrix(.      
-000112f0: 2020 7075 6c73 653a 204f 7074 696f 6e61    pulse: Optiona
-00011300: 6c5b 2750 756c 7365 5365 7175 656e 6365  l['PulseSequence
-00011310: 275d 203d 204e 6f6e 652c 0a20 2020 2020  '] = None,.     
-00011320: 2020 2073 7065 6374 7275 6d3a 204f 7074     spectrum: Opt
-00011330: 696f 6e61 6c5b 6e64 6172 7261 795d 203d  ional[ndarray] =
-00011340: 204e 6f6e 652c 0a20 2020 2020 2020 206f   None,.        o
-00011350: 6d65 6761 3a20 4f70 7469 6f6e 616c 5b43  mega: Optional[C
-00011360: 6f65 6666 6963 6965 6e74 735d 203d 204e  oefficients] = N
-00011370: 6f6e 652c 0a20 2020 2020 2020 206e 5f6f  one,.        n_o
-00011380: 7065 725f 6964 656e 7469 6669 6572 733a  per_identifiers:
-00011390: 204f 7074 696f 6e61 6c5b 5365 7175 656e   Optional[Sequen
-000113a0: 6365 5b73 7472 5d5d 203d 204e 6f6e 652c  ce[str]] = None,
-000113b0: 0a20 2020 2020 2020 2073 6563 6f6e 645f  .        second_
-000113c0: 6f72 6465 723a 2062 6f6f 6c20 3d20 4661  order: bool = Fa
-000113d0: 6c73 652c 0a20 2020 2020 2020 2063 756d  lse,.        cum
-000113e0: 756c 616e 745f 6675 6e63 7469 6f6e 3a20  ulant_function: 
-000113f0: 4f70 7469 6f6e 616c 5b6e 6461 7272 6179  Optional[ndarray
-00011400: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-00011410: 2020 7368 6f77 5f70 726f 6772 6573 7362    show_progressb
-00011420: 6172 3a20 626f 6f6c 203d 2046 616c 7365  ar: bool = False
-00011430: 2c0a 2020 2020 2020 2020 6d65 6d6f 7279  ,.        memory
-00011440: 5f70 6172 7369 6d6f 6e69 6f75 733a 2062  _parsimonious: b
-00011450: 6f6f 6c20 3d20 4661 6c73 652c 0a20 2020  ool = False,.   
-00011460: 2020 2020 2063 6163 6865 5f69 6e74 6572       cache_inter
-00011470: 6d65 6469 6174 6573 3a20 626f 6f6c 203d  mediates: bool =
-00011480: 2046 616c 7365 0a29 202d 3e20 6e64 6172   False.) -> ndar
-00011490: 7261 793a 0a20 2020 2072 2222 2243 6f6d  ray:.    r"""Com
-000114a0: 7075 7465 2074 6865 2065 7272 6f72 2074  pute the error t
-000114b0: 7261 6e73 6665 7220 6d61 7472 6978 2075  ransfer matrix u
-000114c0: 7020 746f 2075 6e69 7461 7279 2072 6f74  p to unitary rot
-000114d0: 6174 696f 6e73 2e0a 0a20 2020 2050 6172  ations...    Par
-000114e0: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
-000114f0: 2d2d 2d2d 2d2d 0a20 2020 2070 756c 7365  ------.    pulse
-00011500: 3a20 5075 6c73 6553 6571 7565 6e63 650a  : PulseSequence.
-00011510: 2020 2020 2020 2020 5468 6520 6060 5075          The ``Pu
-00011520: 6c73 6553 6571 7565 6e63 6560 6020 696e  lseSequence`` in
-00011530: 7374 616e 6365 2066 6f72 2077 6869 6368  stance for which
-00011540: 2074 6f20 636f 6d70 7574 6520 7468 6520   to compute the 
-00011550: 6572 726f 720a 2020 2020 2020 2020 7472  error.        tr
-00011560: 616e 7366 6572 206d 6174 7269 782e 0a20  ansfer matrix.. 
-00011570: 2020 2073 7065 6374 7275 6d3a 2061 7272     spectrum: arr
-00011580: 6179 5f6c 696b 652c 2073 6861 7065 2028  ay_like, shape (
-00011590: 5b5b 6e5f 6e6f 7073 2c5d 206e 5f6e 6f70  [[n_nops,] n_nop
-000115a0: 732c 5d20 6e5f 6f6d 6567 6129 0a20 2020  s,] n_omega).   
-000115b0: 2020 2020 2054 6865 2074 776f 2d73 6964       The two-sid
-000115c0: 6564 206e 6f69 7365 2070 6f77 6572 2073  ed noise power s
-000115d0: 7065 6374 7261 6c20 6465 6e73 6974 7920  pectral density 
-000115e0: 696e 2075 6e69 7473 206f 6620 696e 7665  in units of inve
-000115f0: 7273 650a 2020 2020 2020 2020 6672 6571  rse.        freq
-00011600: 7565 6e63 6965 7320 6173 2061 6e20 6172  uencies as an ar
-00011610: 7261 7920 6f66 2073 6861 7065 2028 6e5f  ray of shape (n_
-00011620: 6f6d 6567 612c 292c 2028 6e5f 6e6f 7073  omega,), (n_nops
-00011630: 2c20 6e5f 6f6d 6567 6129 2c0a 2020 2020  , n_omega),.    
-00011640: 2020 2020 6f72 2028 6e5f 6e6f 7073 2c20      or (n_nops, 
-00011650: 6e5f 6e6f 7073 2c20 6e5f 6f6d 6567 6129  n_nops, n_omega)
-00011660: 2e20 496e 2074 6865 2066 6972 7374 2063  . In the first c
-00011670: 6173 652c 2074 6865 2073 616d 650a 2020  ase, the same.  
-00011680: 2020 2020 2020 7370 6563 7472 756d 2069        spectrum i
-00011690: 7320 7461 6b65 6e20 666f 7220 616c 6c20  s taken for all 
-000116a0: 6e6f 6973 6520 6f70 6572 6174 6f72 732c  noise operators,
-000116b0: 2069 6e20 7468 6520 7365 636f 6e64 2c20   in the second, 
-000116c0: 6974 2069 730a 2020 2020 2020 2020 6173  it is.        as
-000116d0: 7375 6d65 6420 7468 6174 2074 6865 7265  sumed that there
-000116e0: 2061 7265 206e 6f20 636f 7272 656c 6174   are no correlat
-000116f0: 696f 6e73 2062 6574 7765 656e 2064 6966  ions between dif
-00011700: 6665 7265 6e74 206e 6f69 7365 0a20 2020  ferent noise.   
-00011710: 2020 2020 2073 6f75 7263 6573 2061 6e64       sources and
-00011720: 2074 6875 7320 7468 6572 6520 6973 206f   thus there is o
-00011730: 6e65 2073 7065 6374 7275 6d20 666f 7220  ne spectrum for 
-00011740: 6561 6368 206e 6f69 7365 206f 7065 7261  each noise opera
-00011750: 746f 722e 0a20 2020 2020 2020 2049 6e20  tor..        In 
-00011760: 7468 6520 7468 6972 6420 616e 6420 6d6f  the third and mo
-00011770: 7374 2067 656e 6572 616c 2063 6173 652c  st general case,
-00011780: 2074 6865 7265 206d 6179 2062 6520 6120   there may be a 
-00011790: 7370 6563 7472 756d 2066 6f72 0a20 2020  spectrum for.   
-000117a0: 2020 2020 2065 6163 6820 7061 6972 206f       each pair o
-000117b0: 6620 6e6f 6973 6520 6f70 6572 6174 6f72  f noise operator
-000117c0: 7320 636f 7272 6573 706f 6e64 696e 6720  s corresponding 
-000117d0: 746f 2074 6865 2063 6f72 7265 6c61 7469  to the correlati
-000117e0: 6f6e 730a 2020 2020 2020 2020 6265 7477  ons.        betw
-000117f0: 6565 6e20 7468 656d 2e20 6e5f 6e6f 7073  een them. n_nops
-00011800: 2069 7320 7468 6520 6e75 6d62 6572 206f   is the number o
-00011810: 6620 6e6f 6973 6520 6f70 6572 6174 6f72  f noise operator
-00011820: 7320 636f 6e73 6964 6572 6564 0a20 2020  s considered.   
-00011830: 2020 2020 2061 6e64 2073 686f 756c 6420       and should 
-00011840: 6265 2065 7175 616c 2074 6f20 6060 6c65  be equal to ``le
-00011850: 6e28 6e5f 6f70 6572 5f69 6465 6e74 6966  n(n_oper_identif
-00011860: 6965 7273 2960 602e 0a20 2020 206f 6d65  iers)``..    ome
-00011870: 6761 3a20 6172 7261 795f 6c69 6b65 2c20  ga: array_like, 
-00011880: 7368 6170 6520 286e 5f6f 6d65 6761 2c29  shape (n_omega,)
-00011890: 0a20 2020 2020 2020 2054 6865 2066 7265  .        The fre
-000118a0: 7175 656e 6369 6573 2061 7420 7768 6963  quencies at whic
-000118b0: 6820 746f 2063 616c 6375 6c61 7465 2074  h to calculate t
-000118c0: 6865 2066 696c 7465 7220 6675 6e63 7469  he filter functi
-000118d0: 6f6e 732e 0a20 2020 206e 5f6f 7065 725f  ons..    n_oper_
-000118e0: 6964 656e 7469 6669 6572 733a 2061 7272  identifiers: arr
-000118f0: 6179 5f6c 696b 652c 206f 7074 696f 6e61  ay_like, optiona
-00011900: 6c0a 2020 2020 2020 2020 5468 6520 6964  l.        The id
-00011910: 656e 7469 6669 6572 7320 6f66 2074 6865  entifiers of the
-00011920: 206e 6f69 7365 206f 7065 7261 746f 7273   noise operators
-00011930: 2066 6f72 2077 6869 6368 2074 6f20 6576   for which to ev
-00011940: 616c 7561 7465 2074 6865 0a20 2020 2020  aluate the.     
-00011950: 2020 2065 7272 6f72 2074 7261 6e73 6665     error transfe
-00011960: 7220 6d61 7472 6978 2e20 5468 6520 6465  r matrix. The de
-00011970: 6661 756c 7420 6973 2061 6c6c 2e20 4e6f  fault is all. No
-00011980: 7465 2074 6861 742c 2073 696e 6365 2069  te that, since i
-00011990: 6e0a 2020 2020 2020 2020 6765 6e65 7261  n.        genera
-000119a0: 6c20 636f 6e74 7269 6275 7469 6f6e 7320  l contributions 
-000119b0: 6672 6f6d 2064 6966 6665 7265 6e74 206e  from different n
-000119c0: 6f69 7365 206f 7065 7261 746f 7273 2077  oise operators w
-000119d0: 6f6e 2774 0a20 2020 2020 2020 2063 6f6d  on't.        com
-000119e0: 6d75 7465 2c20 6e6f 7420 7365 6c65 6374  mute, not select
-000119f0: 696e 6720 616c 6c20 6e6f 6973 6520 6f70  ing all noise op
-00011a00: 6572 6174 6f72 7320 7265 7375 6c74 7320  erators results 
-00011a10: 696e 206e 6567 6c65 6374 696e 670a 2020  in neglecting.  
-00011a20: 2020 2020 2020 7465 726d 7320 6f66 206f        terms of o
-00011a30: 7264 6572 203a 6d61 7468 3a60 5c78 695e  rder :math:`\xi^
-00011a40: 3460 2e0a 2020 2020 7365 636f 6e64 5f6f  4`..    second_o
-00011a50: 7264 6572 3a20 626f 6f6c 2c20 6f70 7469  rder: bool, opti
-00011a60: 6f6e 616c 0a20 2020 2020 2020 2041 6c73  onal.        Als
-00011a70: 6f20 7461 6b65 2069 6e74 6f20 6163 636f  o take into acco
-00011a80: 756e 7420 7468 6520 6672 6571 7565 6e63  unt the frequenc
-00011a90: 7920 7368 6966 7473 203a 6d61 7468 3a60  y shifts :math:`
-00011aa0: 5c44 656c 7461 6020 7468 6174 0a20 2020  \Delta` that.   
-00011ab0: 2020 2020 2063 6f72 7265 7370 6f6e 6420       correspond 
-00011ac0: 746f 2073 6563 6f6e 6420 6f72 6465 7220  to second order 
-00011ad0: 4d61 676e 7573 2065 7870 616e 7369 6f6e  Magnus expansion
-00011ae0: 2061 6e64 2063 6f6e 7374 6974 7574 650a   and constitute.
-00011af0: 2020 2020 2020 2020 756e 6974 6172 7920          unitary 
-00011b00: 7465 726d 732e 2044 6566 6175 6c74 2060  terms. Default `
-00011b10: 6046 616c 7365 6060 2e0a 2020 2020 6375  `False``..    cu
-00011b20: 6d75 6c61 6e74 5f66 756e 6374 696f 6e3a  mulant_function:
-00011b30: 206e 6461 7272 6179 2c20 7368 6170 6520   ndarray, shape 
-00011b40: 285b 5b6e 5f70 6c73 2c20 6e5f 706c 732c  ([[n_pls, n_pls,
-00011b50: 5d20 6e5f 6e6f 7073 2c5d 206e 5f6e 6f70  ] n_nops,] n_nop
-00011b60: 732c 2064 2a2a 322c 2064 2a2a 3229 0a20  s, d**2, d**2). 
-00011b70: 2020 2020 2020 2041 2070 7265 636f 6d70         A precomp
-00011b80: 7574 6564 2063 756d 756c 616e 7420 6675  uted cumulant fu
-00011b90: 6e63 7469 6f6e 2e20 4966 2067 6976 656e  nction. If given
-00011ba0: 2c20 2a70 756c 7365 2a2c 202a 7370 6563  , *pulse*, *spec
-00011bb0: 7472 756d 2a2c 0a20 2020 2020 2020 202a  trum*,.        *
-00011bc0: 6f6d 6567 612a 2061 7265 206e 6f74 2072  omega* are not r
-00011bd0: 6571 7569 7265 642e 0a20 2020 2073 686f  equired..    sho
-00011be0: 775f 7072 6f67 7265 7373 6261 723a 2062  w_progressbar: b
-00011bf0: 6f6f 6c2c 206f 7074 696f 6e61 6c0a 2020  ool, optional.  
-00011c00: 2020 2020 2020 5368 6f77 2061 2070 726f        Show a pro
-00011c10: 6772 6573 7320 6261 7220 666f 7220 7468  gress bar for th
-00011c20: 6520 6361 6c63 756c 6174 696f 6e20 6f66  e calculation of
-00011c30: 2074 6865 2063 6f6e 7472 6f6c 206d 6174   the control mat
-00011c40: 7269 782e 0a20 2020 206d 656d 6f72 795f  rix..    memory_
-00011c50: 7061 7273 696d 6f6e 696f 7573 3a20 626f  parsimonious: bo
-00011c60: 6f6c 2c20 6f70 7469 6f6e 616c 0a20 2020  ol, optional.   
-00011c70: 2020 2020 2054 7261 6465 206d 656d 6f72       Trade memor
-00011c80: 7920 666f 6f74 7072 696e 7420 666f 7220  y footprint for 
-00011c90: 7065 7266 6f72 6d61 6e63 652e 2053 6565  performance. See
-00011ca0: 0a20 2020 2020 2020 203a 6675 6e63 3a60  .        :func:`
-00011cb0: 7e6e 756d 6572 6963 2e63 616c 6375 6c61  ~numeric.calcula
-00011cc0: 7465 5f64 6563 6179 5f61 6d70 6c69 7475  te_decay_amplitu
-00011cd0: 6465 7360 2e20 5468 6520 6465 6661 756c  des`. The defaul
-00011ce0: 7420 6973 0a20 2020 2020 2020 2060 6046  t is.        ``F
-00011cf0: 616c 7365 6060 2e0a 2020 2020 6361 6368  alse``..    cach
-00011d00: 655f 696e 7465 726d 6564 6961 7465 733a  e_intermediates:
-00011d10: 2062 6f6f 6c2c 206f 7074 696f 6e61 6c0a   bool, optional.
-00011d20: 2020 2020 2020 2020 4b65 6570 2061 6e64          Keep and
-00011d30: 2072 6574 7572 6e20 696e 7465 726d 6564   return intermed
-00011d40: 6961 7465 2074 6572 6d73 206f 6620 7468  iate terms of th
-00011d50: 6520 6361 6c63 756c 6174 696f 6e20 6f66  e calculation of
-00011d60: 2074 6865 0a20 2020 2020 2020 2063 6f6e   the.        con
-00011d70: 7472 6f6c 206d 6174 7269 7820 2869 6620  trol matrix (if 
-00011d80: 6974 2069 7320 6e6f 7420 616c 7265 6164  it is not alread
-00011d90: 7920 6361 6368 6564 2920 7468 6174 2063  y cached) that c
-00011da0: 616e 2062 6520 7265 7573 6564 0a20 2020  an be reused.   
-00011db0: 2020 2020 2066 6f72 2073 6563 6f6e 6420       for second 
-00011dc0: 6f72 6465 7220 6f72 2067 7261 6469 656e  order or gradien
-00011dd0: 7473 2e20 4361 6e20 636f 6e73 756d 6520  ts. Can consume 
-00011de0: 6c61 7267 6520 616d 6f75 6e74 206f 660a  large amount of.
-00011df0: 2020 2020 2020 2020 6d65 6d6f 7279 2c20          memory, 
-00011e00: 6275 7420 7370 6565 6420 7570 2074 6865  but speed up the
-00011e10: 2063 616c 6375 6c61 7469 6f6e 2e0a 0a20   calculation... 
-00011e20: 2020 2052 6574 7572 6e73 0a20 2020 202d     Returns.    -
-00011e30: 2d2d 2d2d 2d2d 0a20 2020 2065 7272 6f72  ------.    error
-00011e40: 5f74 7261 6e73 6665 725f 6d61 7472 6978  _transfer_matrix
-00011e50: 3a20 6e64 6172 7261 792c 2073 6861 7065  : ndarray, shape
-00011e60: 2028 642a 2a32 2c20 642a 2a32 290a 2020   (d**2, d**2).  
-00011e70: 2020 2020 2020 5468 6520 6572 726f 7220        The error 
-00011e80: 7472 616e 7366 6572 206d 6174 7269 782e  transfer matrix.
-00011e90: 2054 6865 2069 6e64 6976 6964 7561 6c20   The individual 
-00011ea0: 6e6f 6973 6520 6f70 6572 6174 6f72 0a20  noise operator. 
-00011eb0: 2020 2020 2020 2063 6f6e 7472 6962 7574         contribut
-00011ec0: 696f 6e73 2061 7265 2073 756d 6d65 6420  ions are summed 
-00011ed0: 7570 2062 6566 6f72 6520 6578 706f 6e65  up before expone
-00011ee0: 6e74 6961 7469 6e67 2061 7320 7468 6579  ntiating as they
-00011ef0: 206d 6967 6874 0a20 2020 2020 2020 206e   might.        n
-00011f00: 6f74 2063 6f6d 6d75 7465 2e0a 0a20 2020  ot commute...   
-00011f10: 204e 6f74 6573 0a20 2020 202d 2d2d 2d2d   Notes.    -----
-00011f20: 0a20 2020 2054 6865 2065 7272 6f72 2074  .    The error t
-00011f30: 7261 6e73 6665 7220 6d61 7472 6978 2069  ransfer matrix i
-00011f40: 7320 6769 7665 6e20 6279 0a0a 2020 2020  s given by..    
-00011f50: 2e2e 206d 6174 683a 3a0a 0a20 2020 2020  .. math::..     
-00011f60: 2020 205c 7469 6c64 657b 5c6d 6174 6863     \tilde{\mathc
-00011f70: 616c 7b55 7d7d 203d 205c 6578 705c 6d61  al{U}} = \exp\ma
-00011f80: 7468 6361 6c7b 4b7d 285c 7461 7529 0a0a  thcal{K}(\tau)..
-00011f90: 2020 2020 7769 7468 203a 6d61 7468 3a60      with :math:`
-00011fa0: 5c6d 6174 6863 616c 7b4b 7d28 5c74 6175  \mathcal{K}(\tau
-00011fb0: 2960 2074 6865 2063 756d 756c 616e 7420  )` the cumulant 
-00011fc0: 6675 6e63 7469 6f6e 2028 7365 650a 2020  function (see.  
-00011fd0: 2020 3a66 756e 633a 6063 616c 6375 6c61    :func:`calcula
-00011fe0: 7465 5f63 756d 756c 616e 745f 6675 6e63  te_cumulant_func
-00011ff0: 7469 6f6e 6029 2e20 466f 7220 4761 7573  tion`). For Gaus
-00012000: 7369 616e 206e 6f69 7365 2074 6869 730a  sian noise this.
-00012010: 2020 2020 6578 7072 6573 7369 6f6e 2069      expression i
-00012020: 7320 6578 6163 7420 7768 656e 2074 616b  s exact when tak
-00012030: 696e 6720 696e 746f 2061 6363 6f75 6e74  ing into account
-00012040: 2074 6865 2064 6563 6179 2061 6d70 6c69   the decay ampli
-00012050: 7475 6465 730a 2020 2020 3a6d 6174 683a  tudes.    :math:
-00012060: 605c 4761 6d6d 6160 2061 6e64 2066 7265  `\Gamma` and fre
-00012070: 7175 656e 6379 2073 6869 6674 7320 3a6d  quency shifts :m
-00012080: 6174 683a 605c 4465 6c74 6160 2e20 4173  ath:`\Delta`. As
-00012090: 2074 6865 206c 6174 7465 720a 2020 2020   the latter.    
-000120a0: 6566 6665 6374 7320 636f 6865 7265 6e74  effects coherent
-000120b0: 2065 7272 6f72 7320 6974 2063 616e 2062   errors it can b
-000120c0: 6520 6e65 676c 6563 7465 6420 6966 2077  e neglected if w
-000120d0: 6520 6173 7375 6d65 2074 6861 7420 7468  e assume that th
-000120e0: 650a 2020 2020 6578 7065 7269 6d65 6e74  e.    experiment
-000120f0: 6572 2068 6173 2063 616c 6962 7261 7465  er has calibrate
-00012100: 6420 7468 6569 7220 7075 6c73 652e 0a0a  d their pulse...
-00012110: 2020 2020 466f 7220 6e6f 6e2d 4761 7573      For non-Gaus
-00012120: 7369 616e 206e 6f69 7365 2074 6865 2065  sian noise the e
-00012130: 7870 7265 7373 696f 6e20 6162 6f76 6520  xpression above 
-00012140: 6973 2070 6572 7475 7262 6174 6976 6520  is perturbative 
-00012150: 616e 640a 2020 2020 696e 636c 7564 6573  and.    includes
-00012160: 206e 6f69 7365 2075 7020 746f 206f 7264   noise up to ord
-00012170: 6572 203a 6d61 7468 3a60 5c78 695e 3260  er :math:`\xi^2`
-00012180: 2061 6e64 2068 656e 6365 0a20 2020 203a   and hence.    :
-00012190: 6d61 7468 3a60 5c74 696c 6465 7b5c 6d61  math:`\tilde{\ma
-000121a0: 7468 6361 6c7b 557d 7d20 3d20 5c6d 6174  thcal{U}} = \mat
-000121b0: 6862 627b 317d 202b 205c 6d61 7468 6361  hbb{1} + \mathca
-000121c0: 6c7b 4b7d 285c 7461 7529 202b 0a20 2020  l{K}(\tau) +.   
-000121d0: 205c 6d61 7468 6361 6c7b 4f7d 285c 7869   \mathcal{O}(\xi
-000121e0: 5e34 2960 0a20 2020 2028 616c 7468 6f75  ^4)`.    (althou
-000121f0: 6768 2069 7420 6973 2065 7661 6c75 6174  gh it is evaluat
-00012200: 6564 2061 7320 6120 6d61 7472 6978 2065  ed as a matrix e
-00012210: 7870 6f6e 656e 7469 616c 2069 6e20 616e  xponential in an
-00012220: 7920 6361 7365 292e 0a0a 2020 2020 4769  y case)...    Gi
-00012230: 7665 6e20 7468 6520 6162 6f76 6520 6578  ven the above ex
-00012240: 7072 6573 7369 6f6e 206f 6620 7468 6520  pression of the 
-00012250: 6572 726f 7220 7472 616e 7366 6572 206d  error transfer m
-00012260: 6174 7269 782c 2074 6865 0a20 2020 2065  atrix, the.    e
-00012270: 6e74 616e 676c 656d 656e 7420 6669 6465  ntanglement fide
-00012280: 6c69 7479 2069 7320 6769 7665 6e20 6279  lity is given by
-00012290: 0a0a 0a20 2020 202e 2e20 6d61 7468 3a3a  ...    .. math::
-000122a0: 0a0a 2020 2020 2020 2020 5c6d 6174 6863  ..        \mathc
-000122b0: 616c 7b46 7d5f 5c6d 6174 6872 6d7b 657d  al{F}_\mathrm{e}
-000122c0: 203d 0a20 2020 2020 2020 2020 2020 205c   =.            \
-000122d0: 6672 6163 7b31 7d7b 645e 327d 5c6d 6174  frac{1}{d^2}\mat
-000122e0: 6872 6d7b 7472 7d5c 2c5c 7469 6c64 657b  hrm{tr}\,\tilde{
-000122f0: 5c6d 6174 6863 616c 7b55 7d7d 2e0a 0a20  \mathcal{U}}... 
-00012300: 2020 2053 6565 2041 6c73 6f0a 2020 2020     See Also.    
-00012310: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2063 616c  --------.    cal
-00012320: 6375 6c61 7465 5f63 756d 756c 616e 745f  culate_cumulant_
-00012330: 6675 6e63 7469 6f6e 3a20 4361 6c63 756c  function: Calcul
-00012340: 6174 6520 7468 6520 6375 6d75 6c61 6e74  ate the cumulant
-00012350: 2066 756e 6374 696f 6e20 3a6d 6174 683a   function :math:
-00012360: 605c 6d61 7468 6361 6c7b 4b7d 600a 2020  `\mathcal{K}`.  
-00012370: 2020 6361 6c63 756c 6174 655f 6465 6361    calculate_deca
-00012380: 795f 616d 706c 6974 7564 6573 3a20 4361  y_amplitudes: Ca
-00012390: 6c63 756c 6174 6520 7468 6520 3a6d 6174  lculate the :mat
-000123a0: 683a 605c 4761 6d6d 615f 7b5c 616c 7068  h:`\Gamma_{\alph
-000123b0: 615c 6265 7461 2c6b 6c7d 600a 2020 2020  a\beta,kl}`.    
-000123c0: 696e 6669 6465 6c69 7479 3a20 4361 6c63  infidelity: Calc
-000123d0: 756c 6174 6520 6f6e 6c79 2069 6e66 6964  ulate only infid
-000123e0: 656c 6974 7920 6f66 2061 2070 756c 7365  elity of a pulse
-000123f0: 2e0a 2020 2020 2222 220a 2020 2020 6966  ..    """.    if
-00012400: 2063 756d 756c 616e 745f 6675 6e63 7469   cumulant_functi
-00012410: 6f6e 2069 7320 4e6f 6e65 3a0a 2020 2020  on is None:.    
-00012420: 2020 2020 6966 2070 756c 7365 2069 7320      if pulse is 
-00012430: 4e6f 6e65 206f 7220 7370 6563 7472 756d  None or spectrum
-00012440: 2069 7320 4e6f 6e65 206f 7220 6f6d 6567   is None or omeg
-00012450: 6120 6973 204e 6f6e 653a 0a20 2020 2020  a is None:.     
-00012460: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
-00012470: 7565 4572 726f 7228 2752 6571 7569 7265  ueError('Require
-00012480: 2065 6974 6865 7220 7072 6563 6f6d 7075   either precompu
-00012490: 7465 6420 6375 6d75 6c61 6e74 2066 756e  ted cumulant fun
-000124a0: 6374 696f 6e20 2720 2b0a 2020 2020 2020  ction ' +.      
+0000f8b0: 2020 2020 6465 7363 3d27 4361 6c63 756c      desc='Calcul
+0000f8c0: 6174 696e 6720 7365 636f 6e64 206f 7264  ating second ord
+0000f8d0: 6572 2046 4627 293a 0a20 2020 2020 2020  er FF'):.       
+0000f8e0: 2069 6620 6e6f 7420 6861 7665 5f69 6e74   if not have_int
+0000f8f0: 6572 6d65 6469 6174 6573 3a0a 2020 2020  ermediates:.    
+0000f900: 2020 2020 2020 2020 6261 7369 735f 7472          basis_tr
+0000f910: 616e 7366 6f72 6d65 6420 3d20 5f74 7261  ansformed = _tra
+0000f920: 6e73 666f 726d 5f62 795f 756e 6974 6172  nsform_by_unitar
+0000f930: 7928 6569 6776 6563 735f 7072 6f70 6167  y(eigvecs_propag
+0000f940: 6174 6564 5b67 5d2c 2062 6173 6973 2c0a  ated[g], basis,.
+0000f950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f980: 2020 2020 2020 6f75 743d 6261 7369 735f        out=basis_
+0000f990: 7472 616e 7366 6f72 6d65 6429 0a20 2020  transformed).   
+0000f9a0: 2020 2020 2020 2020 2023 204e 6565 6420           # Need 
+0000f9b0: 746f 2063 6f6d 7075 7465 2047 5e28 6729  to compute G^(g)
+0000f9c0: 2073 696e 6365 206e 6f20 6361 6368 6520   since no cache 
+0000f9d0: 6769 7665 6e2e 2046 6972 7374 2069 6e69  given. First ini
+0000f9e0: 7469 616c 697a 650a 2020 2020 2020 2020  tialize.        
+0000f9f0: 2020 2020 2320 6275 6666 6572 2074 6f20      # buffer to 
+0000fa00: 7a65 726f 2e20 5468 6572 6520 6973 2061  zero. There is a
+0000fa10: 2070 726f 6261 626c 7920 6c6f 7473 206f   probably lots o
+0000fa20: 6620 6f76 6572 6865 6164 2063 6f6d 7075  f overhead compu
+0000fa30: 7469 6e67 0a20 2020 2020 2020 2020 2020  ting.           
+0000fa40: 2023 2074 6869 7320 696e 6469 7669 6475   # this individu
+0000fa50: 616c 6c79 2066 6f72 2065 7665 7279 2074  ally for every t
+0000fa60: 696d 6520 7374 6570 2e0a 2020 2020 2020  ime step..      
+0000fa70: 2020 2020 2020 6374 726c 6d61 745f 7374        ctrlmat_st
+0000fa80: 6570 5b3a 5d20 3d20 300a 2020 2020 2020  ep[:] = 0.      
+0000fa90: 2020 2020 2020 6374 726c 6d61 745f 7374        ctrlmat_st
+0000faa0: 6570 203d 2063 616c 6375 6c61 7465 5f63  ep = calculate_c
+0000fab0: 6f6e 7472 6f6c 5f6d 6174 7269 785f 6672  ontrol_matrix_fr
+0000fac0: 6f6d 5f73 6372 6174 6368 280a 2020 2020  om_scratch(.    
+0000fad0: 2020 2020 2020 2020 2020 2020 6569 6776              eigv
+0000fae0: 616c 735b 673a 672b 315d 2c20 6569 6776  als[g:g+1], eigv
+0000faf0: 6563 735b 673a 672b 315d 2c20 7072 6f70  ecs[g:g+1], prop
+0000fb00: 6167 6174 6f72 735b 673a 672b 325d 2c20  agators[g:g+2], 
+0000fb10: 6f6d 6567 612c 2062 6173 6973 2c20 6e5f  omega, basis, n_
+0000fb20: 6f70 6572 732c 0a20 2020 2020 2020 2020  opers,.         
+0000fb30: 2020 2020 2020 206e 5f63 6f65 6666 735b         n_coeffs[
+0000fb40: 3a2c 2067 3a67 2b31 5d2c 2064 745b 673a  :, g:g+1], dt[g:
+0000fb50: 672b 315d 2c20 743d 745b 673a 672b 315d  g+1], t=t[g:g+1]
+0000fb60: 2c20 7368 6f77 5f70 726f 6772 6573 7362  , show_progressb
+0000fb70: 6172 3d46 616c 7365 2c0a 2020 2020 2020  ar=False,.      
+0000fb80: 2020 2020 2020 2020 2020 6361 6368 655f            cache_
+0000fb90: 696e 7465 726d 6564 6961 7465 733d 4661  intermediates=Fa
+0000fba0: 6c73 652c 206f 7574 3d63 7472 6c6d 6174  lse, out=ctrlmat
+0000fbb0: 5f73 7465 700a 2020 2020 2020 2020 2020  _step.          
+0000fbc0: 2020 290a 2020 2020 2020 2020 656c 7365    ).        else
+0000fbd0: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
+0000fbe0: 6772 6162 2062 6f74 6820 6672 6f6d 2063  grab both from c
+0000fbf0: 6163 6865 0a20 2020 2020 2020 2020 2020  ache.           
+0000fc00: 2062 6173 6973 5f74 7261 6e73 666f 726d   basis_transform
+0000fc10: 6564 203d 2062 6173 6973 5f74 7261 6e73  ed = basis_trans
+0000fc20: 666f 726d 6564 5f63 6163 6865 5b67 5d0a  formed_cache[g].
+0000fc30: 2020 2020 2020 2020 2020 2020 6374 726c              ctrl
+0000fc40: 6d61 745f 7374 6570 203d 2063 7472 6c6d  mat_step = ctrlm
+0000fc50: 6174 5f73 7465 705f 6361 6368 655b 675d  at_step_cache[g]
+0000fc60: 0a0a 2020 2020 2020 2020 696e 745f 6275  ..        int_bu
+0000fc70: 6620 3d20 5f73 6563 6f6e 645f 6f72 6465  f = _second_orde
+0000fc80: 725f 696e 7465 6772 616c 286f 6d65 6761  r_integral(omega
+0000fc90: 2c20 6569 6776 616c 735b 675d 2c20 6474  , eigvals[g], dt
+0000fca0: 5b67 5d2c 2069 6e74 5f62 7566 2c0a 2020  [g], int_buf,.  
+0000fcb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fcc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fcd0: 2020 2020 2020 2066 7263 5f62 7566 732c         frc_bufs,
+0000fce0: 2064 455f 6275 6673 2c20 6578 705f 6275   dE_bufs, exp_bu
+0000fcf0: 662c 206d 736b 5f62 7566 7329 0a20 2020  f, msk_bufs).   
+0000fd00: 2020 2020 206e 5f6f 7065 7273 5f62 6173       n_opers_bas
+0000fd10: 6973 203d 206e 702e 6569 6e73 756d 2827  is = np.einsum('
+0000fd20: 616b 6c2c 696c 6b2d 3e61 696b 6c27 2c20  akl,ilk->aikl', 
+0000fd30: 6e5f 6f70 6572 735f 7472 616e 7366 6f72  n_opers_transfor
+0000fd40: 6d65 645b 3a2c 2067 5d2c 2062 6173 6973  med[:, g], basis
+0000fd50: 5f74 7261 6e73 666f 726d 6564 290a 2020  _transformed).  
+0000fd60: 2020 2020 2020 2320 5765 2075 7365 2073        # We use s
+0000fd70: 7465 705f 6275 6620 6173 2061 2062 7566  tep_buf as a buf
+0000fd80: 6665 7220 666f 7220 7468 6520 6c61 7374  fer for the last
+0000fd90: 2069 6e74 6572 7661 6c20 2877 6974 6820   interval (with 
+0000fda0: 6e65 7374 6564 2074 696d 650a 2020 2020  nested time.    
+0000fdb0: 2020 2020 2320 6465 7065 6e64 656e 6365      # dependence
+0000fdc0: 2920 616e 6420 6166 7465 7277 6172 6473  ) and afterwards
+0000fdd0: 2074 6865 2069 6e74 6572 7661 6c73 2075   the intervals u
+0000fde0: 7020 746f 2074 6865 206c 6173 7420 2877  p to the last (w
+0000fdf0: 6865 7265 2074 6865 0a20 2020 2020 2020  here the.       
+0000fe00: 2023 2074 696d 6520 6465 7065 6e64 656e   # time dependen
+0000fe10: 6365 2073 6570 6172 6174 6573 2061 6e64  ce separates and
+0000fe20: 2077 6520 6361 6e20 7573 6520 7072 6576   we can use prev
+0000fe30: 696f 7573 2072 6573 756c 7420 666f 7220  ious result for 
+0000fe40: 7468 650a 2020 2020 2020 2020 2320 636f  the.        # co
+0000fe50: 6e74 726f 6c20 6d61 7472 6978 292e 206f  ntrol matrix). o
+0000fe60: 7074 5f65 696e 7375 6d20 7365 656d 7320  pt_einsum seems 
+0000fe70: 746f 2062 6520 6661 7374 6572 2074 6861  to be faster tha
+0000fe80: 6e20 6e75 6d70 7920 6865 7265 2e0a 2020  n numpy here..  
+0000fe90: 2020 2020 2020 7374 6570 5f62 7566 203d        step_buf =
+0000fea0: 2073 7465 705f 6578 7072 2869 6e74 5f62   step_expr(int_b
+0000feb0: 7566 2c20 6e5f 6f70 6572 735f 6261 7369  uf, n_opers_basi
+0000fec0: 732c 206e 5f6f 7065 7273 5f62 6173 6973  s, n_opers_basis
+0000fed0: 2c20 6f75 743d 7374 6570 5f62 7566 290a  , out=step_buf).
+0000fee0: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
+0000fef0: 2b3d 2073 7465 705f 6275 6620 2023 206c  += step_buf  # l
+0000ff00: 6173 7420 696e 7465 7276 616c 0a20 2020  ast interval.   
+0000ff10: 2020 2020 2069 6620 6720 3e20 303a 0a20       if g > 0:. 
+0000ff20: 2020 2020 2020 2020 2020 2073 7465 705f             step_
+0000ff30: 6275 6620 3d20 6e70 2e65 696e 7375 6d28  buf = np.einsum(
+0000ff40: 2761 6b6f 2c62 6c6f 2d3e 6162 6b6c 6f27  'ako,blo->abklo'
+0000ff50: 2c20 6374 726c 6d61 745f 7374 6570 2e63  , ctrlmat_step.c
+0000ff60: 6f6e 6a28 292c 2063 7472 6c6d 6174 5f73  onj(), ctrlmat_s
+0000ff70: 7465 705f 6375 6d75 6c61 7469 7665 2c0a  tep_cumulative,.
+0000ff80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ff90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ffa0: 206f 7574 3d73 7465 705f 6275 6629 0a0a   out=step_buf)..
+0000ffb0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+0000ffc0: 6c74 202b 3d20 7374 6570 5f62 7566 2020  lt += step_buf  
+0000ffd0: 2320 616c 6c20 696e 7465 7276 616c 7320  # all intervals 
+0000ffe0: 7570 2074 6f20 6c61 7374 0a0a 2020 2020  up to last..    
+0000fff0: 2020 2020 6966 2067 203c 206c 656e 2864      if g < len(d
+00010000: 7429 202d 2031 3a0a 2020 2020 2020 2020  t) - 1:.        
+00010010: 2020 2020 2320 4164 6420 475e 2867 2d31      # Add G^(g-1
+00010020: 2920 746f 2063 756d 756c 6174 6976 6520  ) to cumulative 
+00010030: 7375 6d20 666f 7220 3120 3c20 6720 3c20  sum for 1 < g < 
+00010040: 472c 2066 6f72 2067 3d30 2069 7427 730a  G, for g=0 it's.
+00010050: 2020 2020 2020 2020 2020 2020 2320 7a65              # ze
+00010060: 726f 2c20 666f 7220 4720 6974 2773 206e  ro, for G it's n
+00010070: 6f74 2072 6571 7569 7265 6420 6173 2074  ot required as t
+00010080: 6865 206c 6f6f 7020 7465 726d 696e 6174  he loop terminat
+00010090: 6573 0a20 2020 2020 2020 2020 2020 2063  es.            c
+000100a0: 7472 6c6d 6174 5f73 7465 705f 6375 6d75  trlmat_step_cumu
+000100b0: 6c61 7469 7665 202b 3d20 6374 726c 6d61  lative += ctrlma
+000100c0: 745f 7374 6570 0a0a 2020 2020 7265 7475  t_step..    retu
+000100d0: 726e 2072 6573 756c 740a 0a0a 4075 7469  rn result...@uti
+000100e0: 6c2e 7061 7273 655f 6f70 7469 6f6e 616c  l.parse_optional
+000100f0: 5f70 6172 616d 6574 6572 7328 7768 6963  _parameters(whic
+00010100: 683d 2827 6669 6465 6c69 7479 272c 2027  h=('fidelity', '
+00010110: 6765 6e65 7261 6c69 7a65 6427 2929 0a64  generalized')).d
+00010120: 6566 2063 616c 6375 6c61 7465 5f70 756c  ef calculate_pul
+00010130: 7365 5f63 6f72 7265 6c61 7469 6f6e 5f66  se_correlation_f
+00010140: 696c 7465 725f 6675 6e63 7469 6f6e 2863  ilter_function(c
+00010150: 6f6e 7472 6f6c 5f6d 6174 7269 783a 206e  ontrol_matrix: n
+00010160: 6461 7272 6179 2c0a 2020 2020 2020 2020  darray,.        
+00010170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010190: 2020 2020 2020 2020 7768 6963 683a 2073          which: s
+000101a0: 7472 203d 2027 6669 6465 6c69 7479 2729  tr = 'fidelity')
+000101b0: 202d 3e20 6e64 6172 7261 793a 0a20 2020   -> ndarray:.   
+000101c0: 2072 2222 2243 6f6d 7075 7465 2070 756c   r"""Compute pul
+000101d0: 7365 2063 6f72 7265 6c61 7469 6f6e 2066  se correlation f
+000101e0: 696c 7465 7220 6675 6e63 7469 6f6e 2066  ilter function f
+000101f0: 726f 6d20 636f 6e74 726f 6c20 6d61 7472  rom control matr
+00010200: 6978 2e0a 0a20 2020 2050 6172 616d 6574  ix...    Paramet
+00010210: 6572 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ers.    --------
+00010220: 2d2d 0a20 2020 2063 6f6e 7472 6f6c 5f6d  --.    control_m
+00010230: 6174 7269 783a 2061 7272 6179 5f6c 696b  atrix: array_lik
+00010240: 652c 2073 6861 7065 2028 6e5f 7075 6c73  e, shape (n_puls
+00010250: 6573 2c20 6e5f 6e6f 7073 2c20 642a 2a32  es, n_nops, d**2
+00010260: 2c20 6e5f 6f6d 6567 6129 0a20 2020 2020  , n_omega).     
+00010270: 2020 2054 6865 2063 6f6e 7472 6f6c 206d     The control m
+00010280: 6174 7269 782e 0a20 2020 2077 6869 6368  atrix..    which
+00010290: 203a 2073 7472 2c20 6f70 7469 6f6e 616c   : str, optional
+000102a0: 0a20 2020 2020 2020 2057 6869 6368 2066  .        Which f
+000102b0: 696c 7465 7220 6675 6e63 7469 6f6e 2074  ilter function t
+000102c0: 6f20 7265 7475 726e 2e20 4569 7468 6572  o return. Either
+000102d0: 2027 6669 6465 6c69 7479 2720 2864 6566   'fidelity' (def
+000102e0: 6175 6c74 2920 6f72 0a20 2020 2020 2020  ault) or.       
+000102f0: 2027 6765 6e65 7261 6c69 7a65 6427 2028   'generalized' (
+00010300: 7365 6520 3a72 6566 3a60 4e6f 7465 7320  see :ref:`Notes 
+00010310: 3c6e 6f74 6573 3e60 292e 0a0a 2020 2020  <notes>`)...    
+00010320: 5265 7475 726e 730a 2020 2020 2d2d 2d2d  Returns.    ----
+00010330: 2d2d 2d0a 2020 2020 6669 6c74 6572 5f66  ---.    filter_f
+00010340: 756e 6374 696f 6e5f 7063 3a20 6e64 6172  unction_pc: ndar
+00010350: 7261 792c 2073 6861 7065 2028 6e5f 706c  ray, shape (n_pl
+00010360: 732c 206e 5f70 6c73 2c20 6e5f 6e6f 7073  s, n_pls, n_nops
+00010370: 2c20 6e5f 6e6f 7073 2c20 5b64 2a2a 322c  , n_nops, [d**2,
+00010380: 2064 2a2a 322c 5d20 6e5f 6f6d 6567 6129   d**2,] n_omega)
+00010390: 0a20 2020 2020 2020 2054 6865 2070 756c  .        The pul
+000103a0: 7365 2063 6f72 7265 6c61 7469 6f6e 2066  se correlation f
+000103b0: 696c 7465 7220 6675 6e63 7469 6f6e 7320  ilter functions 
+000103c0: 666f 7220 6561 6368 2070 756c 7365 2061  for each pulse a
+000103d0: 6e64 206e 6f69 7365 0a20 2020 2020 2020  nd noise.       
+000103e0: 206f 7065 7261 746f 7220 636f 7272 656c   operator correl
+000103f0: 6174 696f 6e73 2e20 5468 6520 6669 7273  ations. The firs
+00010400: 7420 7477 6f20 6178 6573 2068 6f6c 6420  t two axes hold 
+00010410: 7468 6520 7075 6c73 650a 2020 2020 2020  the pulse.      
+00010420: 2020 636f 7272 656c 6174 696f 6e73 2c20    correlations, 
+00010430: 7468 6520 7365 636f 6e64 2074 776f 2074  the second two t
+00010440: 6865 206e 6f69 7365 2063 6f72 7265 6c61  he noise correla
+00010450: 7469 6f6e 732e 0a20 2020 2077 6869 6368  tions..    which
+00010460: 203a 2073 7472 2c20 6f70 7469 6f6e 616c   : str, optional
+00010470: 0a20 2020 2020 2020 2057 6869 6368 2066  .        Which f
+00010480: 696c 7465 7220 6675 6e63 7469 6f6e 2074  ilter function t
+00010490: 6f20 7265 7475 726e 2e20 4569 7468 6572  o return. Either
+000104a0: 2027 6669 6465 6c69 7479 2720 2864 6566   'fidelity' (def
+000104b0: 6175 6c74 2920 6f72 0a20 2020 2020 2020  ault) or.       
+000104c0: 2027 6765 6e65 7261 6c69 7a65 6427 2028   'generalized' (
+000104d0: 7365 6520 3a72 6566 3a60 4e6f 7465 7320  see :ref:`Notes 
+000104e0: 3c6e 6f74 6573 3e60 292e 0a0a 2020 2020  <notes>`)...    
+000104f0: 2e2e 205f 6e6f 7465 733a 0a0a 2020 2020  .. _notes:..    
+00010500: 4e6f 7465 730a 2020 2020 2d2d 2d2d 2d0a  Notes.    -----.
+00010510: 2020 2020 5468 6520 6765 6e65 7261 6c69      The generali
+00010520: 7a65 6420 7075 6c73 6520 636f 7272 656c  zed pulse correl
+00010530: 6174 696f 6e20 6669 6c74 6572 2066 756e  ation filter fun
+00010540: 6374 696f 6e20 6973 2067 6976 656e 2062  ction is given b
+00010550: 790a 0a20 2020 202e 2e20 6d61 7468 3a3a  y..    .. math::
+00010560: 0a0a 2020 2020 2020 2020 465f 7b5c 616c  ..        F_{\al
+00010570: 7068 615c 6265 7461 2c6b 6c7d 5e7b 2867  pha\beta,kl}^{(g
+00010580: 6727 297d 285c 6f6d 6567 6129 203d 205c  g')}(\omega) = \
+00010590: 6269 676c 5b0a 2020 2020 2020 2020 2020  bigl[.          
+000105a0: 2020 5c6d 6174 6863 616c 7b51 7d5e 7b28    \mathcal{Q}^{(
+000105b0: 6727 2d31 295c 6461 6767 6572 7d0a 2020  g'-1)\dagger}.  
+000105c0: 2020 2020 2020 2020 2020 5c74 696c 6465            \tilde
+000105d0: 7b5c 6d61 7468 6361 6c7b 427d 7d5e 7b28  {\mathcal{B}}^{(
+000105e0: 6727 295c 6461 6767 6572 7d28 5c6f 6d65  g')\dagger}(\ome
+000105f0: 6761 290a 2020 2020 2020 2020 5c62 6967  ga).        \big
+00010600: 725d 5f7b 6b5c 616c 7068 617d 205c 6269  r]_{k\alpha} \bi
+00010610: 676c 5b0a 2020 2020 2020 2020 2020 2020  gl[.            
+00010620: 5c74 696c 6465 7b5c 6d61 7468 6361 6c7b  \tilde{\mathcal{
+00010630: 427d 7d5e 7b28 6729 7d28 5c6f 6d65 6761  B}}^{(g)}(\omega
+00010640: 295c 6d61 7468 6361 6c7b 517d 5e7b 2867  )\mathcal{Q}^{(g
+00010650: 2d31 297d 0a20 2020 2020 2020 205c 6269  -1)}.        \bi
+00010660: 6772 5d5f 7b5c 6265 7461 206c 7d20 655e  gr]_{\beta l} e^
+00010670: 7b69 5c6f 6d65 6761 2874 5f7b 672d 317d  {i\omega(t_{g-1}
+00010680: 202d 2074 5f7b 6727 2d31 7d29 7d2c 0a0a   - t_{g'-1})},..
+00010690: 2020 2020 7769 7468 203a 6d61 7468 3a60      with :math:`
+000106a0: 5c74 696c 6465 7b5c 6d61 7468 6361 6c7b  \tilde{\mathcal{
+000106b0: 427d 7d5e 7b28 6729 7d60 2074 6865 2063  B}}^{(g)}` the c
+000106c0: 6f6e 7472 6f6c 206d 6174 7269 7820 6f66  ontrol matrix of
+000106d0: 2074 6865 0a20 2020 203a 6d61 7468 3a60   the.    :math:`
+000106e0: 6760 2d74 6820 7075 6c73 652e 2054 6865  g`-th pulse. The
+000106f0: 2066 6964 656c 6974 7920 7075 6c73 6520   fidelity pulse 
+00010700: 636f 7272 656c 6174 696f 6e20 6675 6e63  correlation func
+00010710: 7469 6f6e 2069 730a 2020 2020 6f62 7461  tion is.    obta
+00010720: 696e 6564 2062 7920 7472 6163 696e 6720  ined by tracing 
+00010730: 6f75 7420 7468 6520 6261 7369 7320 696e  out the basis in
+00010740: 6469 6365 732c 0a0a 2020 2020 2e2e 206d  dices,..    .. m
+00010750: 6174 683a 3a0a 0a20 2020 2020 2020 2046  ath::..        F
+00010760: 5f7b 5c61 6c70 6861 5c62 6574 617d 5e7b  _{\alpha\beta}^{
+00010770: 2867 6727 297d 285c 6f6d 6567 6129 203d  (gg')}(\omega) =
+00010780: 0a20 2020 2020 2020 2020 205c 7375 6d5f  .          \sum_
+00010790: 7b6b 7d20 465f 7b5c 616c 7068 615c 6265  {k} F_{\alpha\be
+000107a0: 7461 2c6b 6b7d 5e7b 2867 6727 297d 285c  ta,kk}^{(gg')}(\
+000107b0: 6f6d 6567 6129 0a0a 2020 2020 5365 6520  omega)..    See 
+000107c0: 416c 736f 0a20 2020 202d 2d2d 2d2d 2d2d  Also.    -------
+000107d0: 2d0a 2020 2020 6361 6c63 756c 6174 655f  -.    calculate_
+000107e0: 636f 6e74 726f 6c5f 6d61 7472 6978 5f66  control_matrix_f
+000107f0: 726f 6d5f 7363 7261 7463 683a 2043 6f6e  rom_scratch: Con
+00010800: 7472 6f6c 206d 6174 7269 7820 6672 6f6d  trol matrix from
+00010810: 2073 6372 6174 6368 2e0a 2020 2020 6361   scratch..    ca
+00010820: 6c63 756c 6174 655f 636f 6e74 726f 6c5f  lculate_control_
+00010830: 6d61 7472 6978 5f66 726f 6d5f 6174 6f6d  matrix_from_atom
+00010840: 6963 3a20 436f 6e74 726f 6c20 6d61 7472  ic: Control matr
+00010850: 6978 2066 726f 6d20 636f 6e63 6174 656e  ix from concaten
+00010860: 6174 696f 6e2e 0a20 2020 2063 616c 6375  ation..    calcu
+00010870: 6c61 7465 5f66 696c 7465 725f 6675 6e63  late_filter_func
+00010880: 7469 6f6e 3a20 5265 6775 6c61 7220 6669  tion: Regular fi
+00010890: 6c74 6572 2066 756e 6374 696f 6e2e 0a20  lter function.. 
+000108a0: 2020 2022 2222 0a20 2020 2069 6620 636f     """.    if co
+000108b0: 6e74 726f 6c5f 6d61 7472 6978 2e6e 6469  ntrol_matrix.ndi
+000108c0: 6d20 213d 2034 3a0a 2020 2020 2020 2020  m != 4:.        
+000108d0: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+000108e0: 2827 4578 7065 6374 6564 2063 6f6e 7472  ('Expected contr
+000108f0: 6f6c 5f6d 6174 7269 782e 6e64 696d 203d  ol_matrix.ndim =
+00010900: 3d20 342e 2729 0a0a 2020 2020 6966 2077  = 4.')..    if w
+00010910: 6869 6368 203d 3d20 2766 6964 656c 6974  hich == 'fidelit
+00010920: 7927 3a0a 2020 2020 2020 2020 7375 6273  y':.        subs
+00010930: 6372 6970 7473 203d 2027 6761 6b6f 2c68  cripts = 'gako,h
+00010940: 626b 6f2d 3e67 6861 626f 270a 2020 2020  bko->ghabo'.    
+00010950: 656c 7365 3a0a 2020 2020 2020 2020 2320  else:.        # 
+00010960: 7768 6963 6820 3d3d 2027 6765 6e65 7261  which == 'genera
+00010970: 6c69 7a65 6427 0a20 2020 2020 2020 2073  lized'.        s
+00010980: 7562 7363 7269 7074 7320 3d20 2767 616b  ubscripts = 'gak
+00010990: 6f2c 6862 6c6f 2d3e 6768 6162 6b6c 6f27  o,hblo->ghabklo'
+000109a0: 0a0a 2020 2020 7265 7475 726e 206e 702e  ..    return np.
+000109b0: 6569 6e73 756d 2873 7562 7363 7269 7074  einsum(subscript
+000109c0: 732c 2063 6f6e 7472 6f6c 5f6d 6174 7269  s, control_matri
+000109d0: 782e 636f 6e6a 2829 2c20 636f 6e74 726f  x.conj(), contro
+000109e0: 6c5f 6d61 7472 6978 290a 0a0a 6465 6620  l_matrix)...def 
+000109f0: 6469 6167 6f6e 616c 697a 6528 6861 6d69  diagonalize(hami
+00010a00: 6c74 6f6e 6961 6e3a 206e 6461 7272 6179  ltonian: ndarray
+00010a10: 2c20 6474 3a20 436f 6566 6669 6369 656e  , dt: Coefficien
+00010a20: 7473 2920 2d3e 2054 7570 6c65 5b6e 6461  ts) -> Tuple[nda
+00010a30: 7272 6179 5d3a 0a20 2020 2072 2222 2244  rray]:.    r"""D
+00010a40: 6961 676f 6e61 6c69 7a65 2061 2048 616d  iagonalize a Ham
+00010a50: 696c 746f 6e69 616e 2e0a 0a20 2020 2044  iltonian...    D
+00010a60: 6961 676f 6e61 6c69 7a65 2074 6865 2048  iagonalize the H
+00010a70: 616d 696c 746f 6e69 616e 2077 6869 6368  amiltonian which
+00010a80: 2069 7320 7069 6563 6577 6973 6520 636f   is piecewise co
+00010a90: 6e73 7461 6e74 2064 7572 696e 6720 7468  nstant during th
+00010aa0: 650a 2020 2020 7469 6d65 7320 6769 7665  e.    times give
+00010ab0: 6e20 6279 202a 6474 2a20 616e 6420 7265  n by *dt* and re
+00010ac0: 7475 726e 2065 6967 656e 7661 6c75 6573  turn eigenvalues
+00010ad0: 2c20 6569 6765 6e76 6563 746f 7273 2c20  , eigenvectors, 
+00010ae0: 616e 6420 7468 650a 2020 2020 6375 6d75  and the.    cumu
+00010af0: 6c61 7469 7665 2070 726f 7061 6761 746f  lative propagato
+00010b00: 7273 203a 6d61 7468 3a60 515f 6c60 2e20  rs :math:`Q_l`. 
+00010b10: 4e6f 7465 2074 6861 7420 7765 2063 616c  Note that we cal
+00010b20: 6375 6c61 7465 2069 6e20 756e 6974 730a  culate in units.
+00010b30: 2020 2020 7768 6572 6520 3a6d 6174 683a      where :math:
+00010b40: 605c 6862 6172 5c65 7175 6976 2031 6020  `\hbar\equiv 1` 
+00010b50: 736f 2074 6861 740a 0a20 2020 202e 2e20  so that..    .. 
+00010b60: 6d61 7468 3a3a 0a0a 2020 2020 2020 2020  math::..        
+00010b70: 5528 742c 2074 5f30 2920 3d20 5c6d 6174  U(t, t_0) = \mat
+00010b80: 6863 616c 7b54 7d5c 6578 705c 6c65 6674  hcal{T}\exp\left
+00010b90: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00010ba0: 2020 2020 2020 2020 2020 2d69 5c69 6e74            -i\int
+00010bb0: 5f7b 745f 307d 5e74 5c6d 6174 6872 6d7b  _{t_0}^t\mathrm{
+00010bc0: 647d 7427 5c6d 6174 6863 616c 7b48 7d28  d}t'\mathcal{H}(
+00010bd0: 7427 290a 2020 2020 2020 2020 2020 2020  t').            
+00010be0: 2020 2020 2020 2020 5c72 6967 6874 292e          \right).
+00010bf0: 0a0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
+00010c00: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
+00010c10: 2020 2020 6861 6d69 6c74 6f6e 6961 6e3a      hamiltonian:
+00010c20: 2061 7272 6179 5f6c 696b 652c 2073 6861   array_like, sha
+00010c30: 7065 2028 6e5f 6474 2c20 642c 2064 290a  pe (n_dt, d, d).
+00010c40: 2020 2020 2020 2020 4861 6d69 6c74 6f6e          Hamilton
+00010c50: 6961 6e20 6f66 2073 6861 7065 2028 6e5f  ian of shape (n_
+00010c60: 6474 2c20 642c 2064 2920 7769 7468 2064  dt, d, d) with d
+00010c70: 2074 6865 2064 696d 656e 7369 6f6e 616c   the dimensional
+00010c80: 6974 7920 6f66 0a20 2020 2020 2020 2074  ity of.        t
+00010c90: 6865 2073 7973 7465 6d0a 2020 2020 6474  he system.    dt
+00010ca0: 3a20 6172 7261 795f 6c69 6b65 0a20 2020  : array_like.   
+00010cb0: 2020 2020 2054 6865 2074 696d 6520 6469       The time di
+00010cc0: 6666 6572 656e 6365 730a 0a20 2020 2052  fferences..    R
+00010cd0: 6574 7572 6e73 0a20 2020 202d 2d2d 2d2d  eturns.    -----
+00010ce0: 2d2d 0a20 2020 2065 6967 7661 6c73 3a20  --.    eigvals: 
+00010cf0: 6e64 6172 7261 790a 2020 2020 2020 2020  ndarray.        
+00010d00: 4172 7261 7920 6f66 2065 6967 656e 7661  Array of eigenva
+00010d10: 6c75 6573 206f 6620 7368 6170 6520 286e  lues of shape (n
+00010d20: 5f64 742c 2064 290a 2020 2020 6569 6776  _dt, d).    eigv
+00010d30: 6563 733a 206e 6461 7272 6179 0a20 2020  ecs: ndarray.   
+00010d40: 2020 2020 2041 7272 6179 206f 6620 6569       Array of ei
+00010d50: 6765 6e76 6563 746f 7273 206f 6620 7368  genvectors of sh
+00010d60: 6170 6520 286e 5f64 742c 2064 2c20 6429  ape (n_dt, d, d)
+00010d70: 0a20 2020 2070 726f 7061 6761 746f 7273  .    propagators
+00010d80: 3a20 6e64 6172 7261 790a 2020 2020 2020  : ndarray.      
+00010d90: 2020 4172 7261 7920 6f66 2063 756d 756c    Array of cumul
+00010da0: 6174 6976 6520 7072 6f70 6167 6174 6f72  ative propagator
+00010db0: 7320 6f66 2073 6861 7065 2028 6e5f 6474  s of shape (n_dt
+00010dc0: 2b31 2c20 642c 2064 290a 2020 2020 2222  +1, d, d).    ""
+00010dd0: 220a 2020 2020 6420 3d20 6861 6d69 6c74  ".    d = hamilt
+00010de0: 6f6e 6961 6e2e 7368 6170 655b 2d31 5d0a  onian.shape[-1].
+00010df0: 2020 2020 2320 4361 6c63 756c 6174 6520      # Calculate 
+00010e00: 4569 6765 6e76 616c 7565 7320 616e 6420  Eigenvalues and 
+00010e10: 2d76 6563 746f 7273 0a20 2020 2065 6967  -vectors.    eig
+00010e20: 7661 6c73 2c20 6569 6776 6563 7320 3d20  vals, eigvecs = 
+00010e30: 6e6c 612e 6569 6768 2868 616d 696c 746f  nla.eigh(hamilto
+00010e40: 6e69 616e 290a 2020 2020 2320 5072 6f70  nian).    # Prop
+00010e50: 6167 6174 6f72 2050 203d 2056 2065 7870  agator P = V exp
+00010e60: 282d 6a20 4420 6474 2920 565e 5c64 6167  (-j D dt) V^\dag
+00010e70: 2e20 4d69 6464 6c65 2074 6572 6d20 6973  . Middle term is
+00010e80: 206f 6620 7368 6170 650a 2020 2020 2320   of shape.    # 
+00010e90: 2864 2c20 6e5f 6474 2920 6475 6520 746f  (d, n_dt) due to
+00010ea0: 2074 7261 6e73 706f 7365 2c20 736f 2073   transpose, so s
+00010eb0: 7769 7463 6820 6172 6f75 6e64 2069 6e64  witch around ind
+00010ec0: 6963 6573 2069 6e20 6569 6e73 756d 0a20  ices in einsum. 
+00010ed0: 2020 2023 2069 6e73 7465 6164 206f 6620     # instead of 
+00010ee0: 7472 616e 7370 6f73 696e 6720 6167 6169  transposing agai
+00010ef0: 6e2e 2053 616d 6520 676f 6573 2066 6f72  n. Same goes for
+00010f00: 2074 6865 206c 6173 7420 7465 726d 2e20   the last term. 
+00010f10: 5468 6973 2073 6176 6573 0a20 2020 2023  This saves.    #
+00010f20: 2061 2062 6974 206f 6620 7469 6d65 2e20   a bit of time. 
+00010f30: 5468 6520 666f 6c6c 6f77 696e 6720 6973  The following is
+00010f40: 2066 6173 7465 7220 666f 7220 6c61 7267   faster for larg
+00010f50: 6572 2064 696d 656e 7369 6f6e 7320 6275  er dimensions bu
+00010f60: 7420 6e6f 7420 666f 720a 2020 2020 2320  t not for.    # 
+00010f70: 6d61 6e79 2074 696d 6520 7374 6570 733a  many time steps:
+00010f80: 0a20 2020 2023 2050 203d 206e 702e 656d  .    # P = np.em
+00010f90: 7074 7928 2835 3030 2c20 342c 2034 292c  pty((500, 4, 4),
+00010fa0: 2064 7479 7065 3d63 6f6d 706c 6578 290a   dtype=complex).
+00010fb0: 2020 2020 2320 666f 7220 6c2c 2028 562c      # for l, (V,
+00010fc0: 2044 2920 696e 2065 6e75 6d65 7261 7465   D) in enumerate
+00010fd0: 287a 6970 2865 6967 7665 6373 2c20 6e70  (zip(eigvecs, np
+00010fe0: 2e65 7870 282d 316a 2a64 742a 6569 6776  .exp(-1j*dt*eigv
+00010ff0: 616c 732e 5429 2e54 2929 3a0a 2020 2020  als.T).T)):.    
+00011000: 2320 2020 2020 505b 6c5d 203d 2028 5620  #     P[l] = (V 
+00011010: 2a20 4429 2040 2056 2e63 6f6e 6a28 292e  * D) @ V.conj().
+00011020: 540a 2020 2020 7069 6563 6577 6973 6520  T.    piecewise 
+00011030: 3d20 6e70 2e65 696e 7375 6d28 276c 696a  = np.einsum('lij
+00011040: 2c6a 6c2c 6c6b 6a2d 3e6c 696b 272c 0a20  ,jl,lkj->lik',. 
+00011050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011060: 2020 2020 2020 2020 2065 6967 7665 6373           eigvecs
+00011070: 2c20 7574 696c 2e63 6578 7028 2d6e 702e  , util.cexp(-np.
+00011080: 6173 6172 7261 7928 6474 292a 6569 6776  asarray(dt)*eigv
+00011090: 616c 732e 5429 2c20 6569 6776 6563 732e  als.T), eigvecs.
+000110a0: 636f 6e6a 2829 290a 2020 2020 2320 5468  conj()).    # Th
+000110b0: 6520 6375 6d75 6c61 7469 7665 2070 726f  e cumulative pro
+000110c0: 7061 6761 746f 7220 5120 7769 7468 2074  pagator Q with t
+000110d0: 6865 2069 6465 6e74 6974 7920 6f70 6572  he identity oper
+000110e0: 6174 6f72 2061 7320 6669 7273 740a 2020  ator as first.  
+000110f0: 2020 2320 656c 656d 656e 7420 2851 5f30    # element (Q_0
+00011100: 203d 2050 5f30 203d 2049 292c 2069 2e65   = P_0 = I), i.e
+00011110: 2e0a 2020 2020 2320 5120 3d20 5b51 5f30  ..    # Q = [Q_0
+00011120: 2c20 515f 312c 202e 2e2e 2c20 515f 6e5d  , Q_1, ..., Q_n]
+00011130: 203d 205b 505f 302c 2050 5f31 2040 2050   = [P_0, P_1 @ P
+00011140: 5f30 2c20 2e2e 2e2c 2050 5f6e 2040 202e  _0, ..., P_n @ .
+00011150: 2e2e 2040 2050 5f30 5d0a 2020 2020 6375  .. @ P_0].    cu
+00011160: 6d75 6c61 7469 7665 203d 206e 702e 656d  mulative = np.em
+00011170: 7074 7928 286c 656e 2864 7429 2b31 2c20  pty((len(dt)+1, 
+00011180: 642c 2064 292c 2064 7479 7065 3d63 6f6d  d, d), dtype=com
+00011190: 706c 6578 290a 2020 2020 6375 6d75 6c61  plex).    cumula
+000111a0: 7469 7665 5b30 5d20 3d20 6e70 2e69 6465  tive[0] = np.ide
+000111b0: 6e74 6974 7928 6429 0a20 2020 2066 6f72  ntity(d).    for
+000111c0: 2069 2069 6e20 7261 6e67 6528 6c65 6e28   i in range(len(
+000111d0: 6474 2929 3a0a 2020 2020 2020 2020 6375  dt)):.        cu
+000111e0: 6d75 6c61 7469 7665 5b69 2b31 5d20 3d20  mulative[i+1] = 
+000111f0: 7069 6563 6577 6973 655b 695d 2040 2063  piecewise[i] @ c
+00011200: 756d 756c 6174 6976 655b 695d 0a0a 2020  umulative[i]..  
+00011210: 2020 7265 7475 726e 2065 6967 7661 6c73    return eigvals
+00011220: 2c20 6569 6776 6563 732c 2063 756d 756c  , eigvecs, cumul
+00011230: 6174 6976 650a 0a0a 6465 6620 6572 726f  ative...def erro
+00011240: 725f 7472 616e 7366 6572 5f6d 6174 7269  r_transfer_matri
+00011250: 7828 0a20 2020 2020 2020 2070 756c 7365  x(.        pulse
+00011260: 3a20 4f70 7469 6f6e 616c 5b27 5075 6c73  : Optional['Puls
+00011270: 6553 6571 7565 6e63 6527 5d20 3d20 4e6f  eSequence'] = No
+00011280: 6e65 2c0a 2020 2020 2020 2020 7370 6563  ne,.        spec
+00011290: 7472 756d 3a20 4f70 7469 6f6e 616c 5b6e  trum: Optional[n
+000112a0: 6461 7272 6179 5d20 3d20 4e6f 6e65 2c0a  darray] = None,.
+000112b0: 2020 2020 2020 2020 6f6d 6567 613a 204f          omega: O
+000112c0: 7074 696f 6e61 6c5b 436f 6566 6669 6369  ptional[Coeffici
+000112d0: 656e 7473 5d20 3d20 4e6f 6e65 2c0a 2020  ents] = None,.  
+000112e0: 2020 2020 2020 6e5f 6f70 6572 5f69 6465        n_oper_ide
+000112f0: 6e74 6966 6965 7273 3a20 4f70 7469 6f6e  ntifiers: Option
+00011300: 616c 5b53 6571 7565 6e63 655b 7374 725d  al[Sequence[str]
+00011310: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+00011320: 2020 7365 636f 6e64 5f6f 7264 6572 3a20    second_order: 
+00011330: 626f 6f6c 203d 2046 616c 7365 2c0a 2020  bool = False,.  
+00011340: 2020 2020 2020 6375 6d75 6c61 6e74 5f66        cumulant_f
+00011350: 756e 6374 696f 6e3a 204f 7074 696f 6e61  unction: Optiona
+00011360: 6c5b 6e64 6172 7261 795d 203d 204e 6f6e  l[ndarray] = Non
+00011370: 652c 0a20 2020 2020 2020 2073 686f 775f  e,.        show_
+00011380: 7072 6f67 7265 7373 6261 723a 2062 6f6f  progressbar: boo
+00011390: 6c20 3d20 4661 6c73 652c 0a20 2020 2020  l = False,.     
+000113a0: 2020 206d 656d 6f72 795f 7061 7273 696d     memory_parsim
+000113b0: 6f6e 696f 7573 3a20 626f 6f6c 203d 2046  onious: bool = F
+000113c0: 616c 7365 2c0a 2020 2020 2020 2020 6361  alse,.        ca
+000113d0: 6368 655f 696e 7465 726d 6564 6961 7465  che_intermediate
+000113e0: 733a 2062 6f6f 6c20 3d20 4661 6c73 650a  s: bool = False.
+000113f0: 2920 2d3e 206e 6461 7272 6179 3a0a 2020  ) -> ndarray:.  
+00011400: 2020 7222 2222 436f 6d70 7574 6520 7468    r"""Compute th
+00011410: 6520 6572 726f 7220 7472 616e 7366 6572  e error transfer
+00011420: 206d 6174 7269 7820 7570 2074 6f20 756e   matrix up to un
+00011430: 6974 6172 7920 726f 7461 7469 6f6e 732e  itary rotations.
+00011440: 0a0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
+00011450: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
+00011460: 2020 2020 7075 6c73 653a 2050 756c 7365      pulse: Pulse
+00011470: 5365 7175 656e 6365 0a20 2020 2020 2020  Sequence.       
+00011480: 2054 6865 2060 6050 756c 7365 5365 7175   The ``PulseSequ
+00011490: 656e 6365 6060 2069 6e73 7461 6e63 6520  ence`` instance 
+000114a0: 666f 7220 7768 6963 6820 746f 2063 6f6d  for which to com
+000114b0: 7075 7465 2074 6865 2065 7272 6f72 0a20  pute the error. 
+000114c0: 2020 2020 2020 2074 7261 6e73 6665 7220         transfer 
+000114d0: 6d61 7472 6978 2e0a 2020 2020 7370 6563  matrix..    spec
+000114e0: 7472 756d 3a20 6172 7261 795f 6c69 6b65  trum: array_like
+000114f0: 2c20 7368 6170 6520 285b 5b6e 5f6e 6f70  , shape ([[n_nop
+00011500: 732c 5d20 6e5f 6e6f 7073 2c5d 206e 5f6f  s,] n_nops,] n_o
+00011510: 6d65 6761 290a 2020 2020 2020 2020 5468  mega).        Th
+00011520: 6520 7477 6f2d 7369 6465 6420 6e6f 6973  e two-sided nois
+00011530: 6520 706f 7765 7220 7370 6563 7472 616c  e power spectral
+00011540: 2064 656e 7369 7479 2069 6e20 756e 6974   density in unit
+00011550: 7320 6f66 2069 6e76 6572 7365 0a20 2020  s of inverse.   
+00011560: 2020 2020 2066 7265 7175 656e 6369 6573       frequencies
+00011570: 2061 7320 616e 2061 7272 6179 206f 6620   as an array of 
+00011580: 7368 6170 6520 286e 5f6f 6d65 6761 2c29  shape (n_omega,)
+00011590: 2c20 286e 5f6e 6f70 732c 206e 5f6f 6d65  , (n_nops, n_ome
+000115a0: 6761 292c 0a20 2020 2020 2020 206f 7220  ga),.        or 
+000115b0: 286e 5f6e 6f70 732c 206e 5f6e 6f70 732c  (n_nops, n_nops,
+000115c0: 206e 5f6f 6d65 6761 292e 2049 6e20 7468   n_omega). In th
+000115d0: 6520 6669 7273 7420 6361 7365 2c20 7468  e first case, th
+000115e0: 6520 7361 6d65 0a20 2020 2020 2020 2073  e same.        s
+000115f0: 7065 6374 7275 6d20 6973 2074 616b 656e  pectrum is taken
+00011600: 2066 6f72 2061 6c6c 206e 6f69 7365 206f   for all noise o
+00011610: 7065 7261 746f 7273 2c20 696e 2074 6865  perators, in the
+00011620: 2073 6563 6f6e 642c 2069 7420 6973 0a20   second, it is. 
+00011630: 2020 2020 2020 2061 7373 756d 6564 2074         assumed t
+00011640: 6861 7420 7468 6572 6520 6172 6520 6e6f  hat there are no
+00011650: 2063 6f72 7265 6c61 7469 6f6e 7320 6265   correlations be
+00011660: 7477 6565 6e20 6469 6666 6572 656e 7420  tween different 
+00011670: 6e6f 6973 650a 2020 2020 2020 2020 736f  noise.        so
+00011680: 7572 6365 7320 616e 6420 7468 7573 2074  urces and thus t
+00011690: 6865 7265 2069 7320 6f6e 6520 7370 6563  here is one spec
+000116a0: 7472 756d 2066 6f72 2065 6163 6820 6e6f  trum for each no
+000116b0: 6973 6520 6f70 6572 6174 6f72 2e0a 2020  ise operator..  
+000116c0: 2020 2020 2020 496e 2074 6865 2074 6869        In the thi
+000116d0: 7264 2061 6e64 206d 6f73 7420 6765 6e65  rd and most gene
+000116e0: 7261 6c20 6361 7365 2c20 7468 6572 6520  ral case, there 
+000116f0: 6d61 7920 6265 2061 2073 7065 6374 7275  may be a spectru
+00011700: 6d20 666f 720a 2020 2020 2020 2020 6561  m for.        ea
+00011710: 6368 2070 6169 7220 6f66 206e 6f69 7365  ch pair of noise
+00011720: 206f 7065 7261 746f 7273 2063 6f72 7265   operators corre
+00011730: 7370 6f6e 6469 6e67 2074 6f20 7468 6520  sponding to the 
+00011740: 636f 7272 656c 6174 696f 6e73 0a20 2020  correlations.   
+00011750: 2020 2020 2062 6574 7765 656e 2074 6865       between the
+00011760: 6d2e 206e 5f6e 6f70 7320 6973 2074 6865  m. n_nops is the
+00011770: 206e 756d 6265 7220 6f66 206e 6f69 7365   number of noise
+00011780: 206f 7065 7261 746f 7273 2063 6f6e 7369   operators consi
+00011790: 6465 7265 640a 2020 2020 2020 2020 616e  dered.        an
+000117a0: 6420 7368 6f75 6c64 2062 6520 6571 7561  d should be equa
+000117b0: 6c20 746f 2060 606c 656e 286e 5f6f 7065  l to ``len(n_ope
+000117c0: 725f 6964 656e 7469 6669 6572 7329 6060  r_identifiers)``
+000117d0: 2e0a 2020 2020 6f6d 6567 613a 2061 7272  ..    omega: arr
+000117e0: 6179 5f6c 696b 652c 2073 6861 7065 2028  ay_like, shape (
+000117f0: 6e5f 6f6d 6567 612c 290a 2020 2020 2020  n_omega,).      
+00011800: 2020 5468 6520 6672 6571 7565 6e63 6965    The frequencie
+00011810: 7320 6174 2077 6869 6368 2074 6f20 6361  s at which to ca
+00011820: 6c63 756c 6174 6520 7468 6520 6669 6c74  lculate the filt
+00011830: 6572 2066 756e 6374 696f 6e73 2e0a 2020  er functions..  
+00011840: 2020 6e5f 6f70 6572 5f69 6465 6e74 6966    n_oper_identif
+00011850: 6965 7273 3a20 6172 7261 795f 6c69 6b65  iers: array_like
+00011860: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
+00011870: 2020 2054 6865 2069 6465 6e74 6966 6965     The identifie
+00011880: 7273 206f 6620 7468 6520 6e6f 6973 6520  rs of the noise 
+00011890: 6f70 6572 6174 6f72 7320 666f 7220 7768  operators for wh
+000118a0: 6963 6820 746f 2065 7661 6c75 6174 6520  ich to evaluate 
+000118b0: 7468 650a 2020 2020 2020 2020 6572 726f  the.        erro
+000118c0: 7220 7472 616e 7366 6572 206d 6174 7269  r transfer matri
+000118d0: 782e 2054 6865 2064 6566 6175 6c74 2069  x. The default i
+000118e0: 7320 616c 6c2e 204e 6f74 6520 7468 6174  s all. Note that
+000118f0: 2c20 7369 6e63 6520 696e 0a20 2020 2020  , since in.     
+00011900: 2020 2067 656e 6572 616c 2063 6f6e 7472     general contr
+00011910: 6962 7574 696f 6e73 2066 726f 6d20 6469  ibutions from di
+00011920: 6666 6572 656e 7420 6e6f 6973 6520 6f70  fferent noise op
+00011930: 6572 6174 6f72 7320 776f 6e27 740a 2020  erators won't.  
+00011940: 2020 2020 2020 636f 6d6d 7574 652c 206e        commute, n
+00011950: 6f74 2073 656c 6563 7469 6e67 2061 6c6c  ot selecting all
+00011960: 206e 6f69 7365 206f 7065 7261 746f 7273   noise operators
+00011970: 2072 6573 756c 7473 2069 6e20 6e65 676c   results in negl
+00011980: 6563 7469 6e67 0a20 2020 2020 2020 2074  ecting.        t
+00011990: 6572 6d73 206f 6620 6f72 6465 7220 3a6d  erms of order :m
+000119a0: 6174 683a 605c 7869 5e34 602e 0a20 2020  ath:`\xi^4`..   
+000119b0: 2073 6563 6f6e 645f 6f72 6465 723a 2062   second_order: b
+000119c0: 6f6f 6c2c 206f 7074 696f 6e61 6c0a 2020  ool, optional.  
+000119d0: 2020 2020 2020 416c 736f 2074 616b 6520        Also take 
+000119e0: 696e 746f 2061 6363 6f75 6e74 2074 6865  into account the
+000119f0: 2066 7265 7175 656e 6379 2073 6869 6674   frequency shift
+00011a00: 7320 3a6d 6174 683a 605c 4465 6c74 6160  s :math:`\Delta`
+00011a10: 2074 6861 740a 2020 2020 2020 2020 636f   that.        co
+00011a20: 7272 6573 706f 6e64 2074 6f20 7365 636f  rrespond to seco
+00011a30: 6e64 206f 7264 6572 204d 6167 6e75 7320  nd order Magnus 
+00011a40: 6578 7061 6e73 696f 6e20 616e 6420 636f  expansion and co
+00011a50: 6e73 7469 7475 7465 0a20 2020 2020 2020  nstitute.       
+00011a60: 2075 6e69 7461 7279 2074 6572 6d73 2e20   unitary terms. 
+00011a70: 4465 6661 756c 7420 6060 4661 6c73 6560  Default ``False`
+00011a80: 602e 0a20 2020 2063 756d 756c 616e 745f  `..    cumulant_
+00011a90: 6675 6e63 7469 6f6e 3a20 6e64 6172 7261  function: ndarra
+00011aa0: 792c 2073 6861 7065 2028 5b5b 6e5f 706c  y, shape ([[n_pl
+00011ab0: 732c 206e 5f70 6c73 2c5d 206e 5f6e 6f70  s, n_pls,] n_nop
+00011ac0: 732c 5d20 6e5f 6e6f 7073 2c20 642a 2a32  s,] n_nops, d**2
+00011ad0: 2c20 642a 2a32 290a 2020 2020 2020 2020  , d**2).        
+00011ae0: 4120 7072 6563 6f6d 7075 7465 6420 6375  A precomputed cu
+00011af0: 6d75 6c61 6e74 2066 756e 6374 696f 6e2e  mulant function.
+00011b00: 2049 6620 6769 7665 6e2c 202a 7075 6c73   If given, *puls
+00011b10: 652a 2c20 2a73 7065 6374 7275 6d2a 2c0a  e*, *spectrum*,.
+00011b20: 2020 2020 2020 2020 2a6f 6d65 6761 2a20          *omega* 
+00011b30: 6172 6520 6e6f 7420 7265 7175 6972 6564  are not required
+00011b40: 2e0a 2020 2020 7368 6f77 5f70 726f 6772  ..    show_progr
+00011b50: 6573 7362 6172 3a20 626f 6f6c 2c20 6f70  essbar: bool, op
+00011b60: 7469 6f6e 616c 0a20 2020 2020 2020 2053  tional.        S
+00011b70: 686f 7720 6120 7072 6f67 7265 7373 2062  how a progress b
+00011b80: 6172 2066 6f72 2074 6865 2063 616c 6375  ar for the calcu
+00011b90: 6c61 7469 6f6e 206f 6620 7468 6520 636f  lation of the co
+00011ba0: 6e74 726f 6c20 6d61 7472 6978 2e0a 2020  ntrol matrix..  
+00011bb0: 2020 6d65 6d6f 7279 5f70 6172 7369 6d6f    memory_parsimo
+00011bc0: 6e69 6f75 733a 2062 6f6f 6c2c 206f 7074  nious: bool, opt
+00011bd0: 696f 6e61 6c0a 2020 2020 2020 2020 5472  ional.        Tr
+00011be0: 6164 6520 6d65 6d6f 7279 2066 6f6f 7470  ade memory footp
+00011bf0: 7269 6e74 2066 6f72 2070 6572 666f 726d  rint for perform
+00011c00: 616e 6365 2e20 5365 650a 2020 2020 2020  ance. See.      
+00011c10: 2020 3a66 756e 633a 607e 6e75 6d65 7269    :func:`~numeri
+00011c20: 632e 6361 6c63 756c 6174 655f 6465 6361  c.calculate_deca
+00011c30: 795f 616d 706c 6974 7564 6573 602e 2054  y_amplitudes`. T
+00011c40: 6865 2064 6566 6175 6c74 2069 730a 2020  he default is.  
+00011c50: 2020 2020 2020 6060 4661 6c73 6560 602e        ``False``.
+00011c60: 0a20 2020 2063 6163 6865 5f69 6e74 6572  .    cache_inter
+00011c70: 6d65 6469 6174 6573 3a20 626f 6f6c 2c20  mediates: bool, 
+00011c80: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
+00011c90: 204b 6565 7020 616e 6420 7265 7475 726e   Keep and return
+00011ca0: 2069 6e74 6572 6d65 6469 6174 6520 7465   intermediate te
+00011cb0: 726d 7320 6f66 2074 6865 2063 616c 6375  rms of the calcu
+00011cc0: 6c61 7469 6f6e 206f 6620 7468 650a 2020  lation of the.  
+00011cd0: 2020 2020 2020 636f 6e74 726f 6c20 6d61        control ma
+00011ce0: 7472 6978 2028 6966 2069 7420 6973 206e  trix (if it is n
+00011cf0: 6f74 2061 6c72 6561 6479 2063 6163 6865  ot already cache
+00011d00: 6429 2074 6861 7420 6361 6e20 6265 2072  d) that can be r
+00011d10: 6575 7365 640a 2020 2020 2020 2020 666f  eused.        fo
+00011d20: 7220 7365 636f 6e64 206f 7264 6572 206f  r second order o
+00011d30: 7220 6772 6164 6965 6e74 732e 2043 616e  r gradients. Can
+00011d40: 2063 6f6e 7375 6d65 206c 6172 6765 2061   consume large a
+00011d50: 6d6f 756e 7420 6f66 0a20 2020 2020 2020  mount of.       
+00011d60: 206d 656d 6f72 792c 2062 7574 2073 7065   memory, but spe
+00011d70: 6564 2075 7020 7468 6520 6361 6c63 756c  ed up the calcul
+00011d80: 6174 696f 6e2e 0a0a 2020 2020 5265 7475  ation...    Retu
+00011d90: 726e 730a 2020 2020 2d2d 2d2d 2d2d 2d0a  rns.    -------.
+00011da0: 2020 2020 6572 726f 725f 7472 616e 7366      error_transf
+00011db0: 6572 5f6d 6174 7269 783a 206e 6461 7272  er_matrix: ndarr
+00011dc0: 6179 2c20 7368 6170 6520 2864 2a2a 322c  ay, shape (d**2,
+00011dd0: 2064 2a2a 3229 0a20 2020 2020 2020 2054   d**2).        T
+00011de0: 6865 2065 7272 6f72 2074 7261 6e73 6665  he error transfe
+00011df0: 7220 6d61 7472 6978 2e20 5468 6520 696e  r matrix. The in
+00011e00: 6469 7669 6475 616c 206e 6f69 7365 206f  dividual noise o
+00011e10: 7065 7261 746f 720a 2020 2020 2020 2020  perator.        
+00011e20: 636f 6e74 7269 6275 7469 6f6e 7320 6172  contributions ar
+00011e30: 6520 7375 6d6d 6564 2075 7020 6265 666f  e summed up befo
+00011e40: 7265 2065 7870 6f6e 656e 7469 6174 696e  re exponentiatin
+00011e50: 6720 6173 2074 6865 7920 6d69 6768 740a  g as they might.
+00011e60: 2020 2020 2020 2020 6e6f 7420 636f 6d6d          not comm
+00011e70: 7574 652e 0a0a 2020 2020 4e6f 7465 730a  ute...    Notes.
+00011e80: 2020 2020 2d2d 2d2d 2d0a 2020 2020 5468      -----.    Th
+00011e90: 6520 6572 726f 7220 7472 616e 7366 6572  e error transfer
+00011ea0: 206d 6174 7269 7820 6973 2067 6976 656e   matrix is given
+00011eb0: 2062 790a 0a20 2020 202e 2e20 6d61 7468   by..    .. math
+00011ec0: 3a3a 0a0a 2020 2020 2020 2020 5c74 696c  ::..        \til
+00011ed0: 6465 7b5c 6d61 7468 6361 6c7b 557d 7d20  de{\mathcal{U}} 
+00011ee0: 3d20 5c65 7870 5c6d 6174 6863 616c 7b4b  = \exp\mathcal{K
+00011ef0: 7d28 5c74 6175 290a 0a20 2020 2077 6974  }(\tau)..    wit
+00011f00: 6820 3a6d 6174 683a 605c 6d61 7468 6361  h :math:`\mathca
+00011f10: 6c7b 4b7d 285c 7461 7529 6020 7468 6520  l{K}(\tau)` the 
+00011f20: 6375 6d75 6c61 6e74 2066 756e 6374 696f  cumulant functio
+00011f30: 6e20 2873 6565 0a20 2020 203a 6675 6e63  n (see.    :func
+00011f40: 3a60 6361 6c63 756c 6174 655f 6375 6d75  :`calculate_cumu
+00011f50: 6c61 6e74 5f66 756e 6374 696f 6e60 292e  lant_function`).
+00011f60: 2046 6f72 2047 6175 7373 6961 6e20 6e6f   For Gaussian no
+00011f70: 6973 6520 7468 6973 0a20 2020 2065 7870  ise this.    exp
+00011f80: 7265 7373 696f 6e20 6973 2065 7861 6374  ression is exact
+00011f90: 2077 6865 6e20 7461 6b69 6e67 2069 6e74   when taking int
+00011fa0: 6f20 6163 636f 756e 7420 7468 6520 6465  o account the de
+00011fb0: 6361 7920 616d 706c 6974 7564 6573 0a20  cay amplitudes. 
+00011fc0: 2020 203a 6d61 7468 3a60 5c47 616d 6d61     :math:`\Gamma
+00011fd0: 6020 616e 6420 6672 6571 7565 6e63 7920  ` and frequency 
+00011fe0: 7368 6966 7473 203a 6d61 7468 3a60 5c44  shifts :math:`\D
+00011ff0: 656c 7461 602e 2041 7320 7468 6520 6c61  elta`. As the la
+00012000: 7474 6572 0a20 2020 2065 6666 6563 7473  tter.    effects
+00012010: 2063 6f68 6572 656e 7420 6572 726f 7273   coherent errors
+00012020: 2069 7420 6361 6e20 6265 206e 6567 6c65   it can be negle
+00012030: 6374 6564 2069 6620 7765 2061 7373 756d  cted if we assum
+00012040: 6520 7468 6174 2074 6865 0a20 2020 2065  e that the.    e
+00012050: 7870 6572 696d 656e 7465 7220 6861 7320  xperimenter has 
+00012060: 6361 6c69 6272 6174 6564 2074 6865 6972  calibrated their
+00012070: 2070 756c 7365 2e0a 0a20 2020 2046 6f72   pulse...    For
+00012080: 206e 6f6e 2d47 6175 7373 6961 6e20 6e6f   non-Gaussian no
+00012090: 6973 6520 7468 6520 6578 7072 6573 7369  ise the expressi
+000120a0: 6f6e 2061 626f 7665 2069 7320 7065 7274  on above is pert
+000120b0: 7572 6261 7469 7665 2061 6e64 0a20 2020  urbative and.   
+000120c0: 2069 6e63 6c75 6465 7320 6e6f 6973 6520   includes noise 
+000120d0: 7570 2074 6f20 6f72 6465 7220 3a6d 6174  up to order :mat
+000120e0: 683a 605c 7869 5e32 6020 616e 6420 6865  h:`\xi^2` and he
+000120f0: 6e63 650a 2020 2020 3a6d 6174 683a 605c  nce.    :math:`\
+00012100: 7469 6c64 657b 5c6d 6174 6863 616c 7b55  tilde{\mathcal{U
+00012110: 7d7d 203d 205c 6d61 7468 6262 7b31 7d20  }} = \mathbb{1} 
+00012120: 2b20 5c6d 6174 6863 616c 7b4b 7d28 5c74  + \mathcal{K}(\t
+00012130: 6175 2920 2b0a 2020 2020 5c6d 6174 6863  au) +.    \mathc
+00012140: 616c 7b4f 7d28 5c78 695e 3429 600a 2020  al{O}(\xi^4)`.  
+00012150: 2020 2861 6c74 686f 7567 6820 6974 2069    (although it i
+00012160: 7320 6576 616c 7561 7465 6420 6173 2061  s evaluated as a
+00012170: 206d 6174 7269 7820 6578 706f 6e65 6e74   matrix exponent
+00012180: 6961 6c20 696e 2061 6e79 2063 6173 6529  ial in any case)
+00012190: 2e0a 0a20 2020 2047 6976 656e 2074 6865  ...    Given the
+000121a0: 2061 626f 7665 2065 7870 7265 7373 696f   above expressio
+000121b0: 6e20 6f66 2074 6865 2065 7272 6f72 2074  n of the error t
+000121c0: 7261 6e73 6665 7220 6d61 7472 6978 2c20  ransfer matrix, 
+000121d0: 7468 650a 2020 2020 656e 7461 6e67 6c65  the.    entangle
+000121e0: 6d65 6e74 2066 6964 656c 6974 7920 6973  ment fidelity is
+000121f0: 2067 6976 656e 2062 790a 0a0a 2020 2020   given by...    
+00012200: 2e2e 206d 6174 683a 3a0a 0a20 2020 2020  .. math::..     
+00012210: 2020 205c 6d61 7468 6361 6c7b 467d 5f5c     \mathcal{F}_\
+00012220: 6d61 7468 726d 7b65 7d20 3d0a 2020 2020  mathrm{e} =.    
+00012230: 2020 2020 2020 2020 5c66 7261 637b 317d          \frac{1}
+00012240: 7b64 5e32 7d5c 6d61 7468 726d 7b74 727d  {d^2}\mathrm{tr}
+00012250: 5c2c 5c74 696c 6465 7b5c 6d61 7468 6361  \,\tilde{\mathca
+00012260: 6c7b 557d 7d2e 0a0a 2020 2020 5365 6520  l{U}}...    See 
+00012270: 416c 736f 0a20 2020 202d 2d2d 2d2d 2d2d  Also.    -------
+00012280: 2d0a 2020 2020 6361 6c63 756c 6174 655f  -.    calculate_
+00012290: 6375 6d75 6c61 6e74 5f66 756e 6374 696f  cumulant_functio
+000122a0: 6e3a 2043 616c 6375 6c61 7465 2074 6865  n: Calculate the
+000122b0: 2063 756d 756c 616e 7420 6675 6e63 7469   cumulant functi
+000122c0: 6f6e 203a 6d61 7468 3a60 5c6d 6174 6863  on :math:`\mathc
+000122d0: 616c 7b4b 7d60 0a20 2020 2063 616c 6375  al{K}`.    calcu
+000122e0: 6c61 7465 5f64 6563 6179 5f61 6d70 6c69  late_decay_ampli
+000122f0: 7475 6465 733a 2043 616c 6375 6c61 7465  tudes: Calculate
+00012300: 2074 6865 203a 6d61 7468 3a60 5c47 616d   the :math:`\Gam
+00012310: 6d61 5f7b 5c61 6c70 6861 5c62 6574 612c  ma_{\alpha\beta,
+00012320: 6b6c 7d60 0a20 2020 2069 6e66 6964 656c  kl}`.    infidel
+00012330: 6974 793a 2043 616c 6375 6c61 7465 206f  ity: Calculate o
+00012340: 6e6c 7920 696e 6669 6465 6c69 7479 206f  nly infidelity o
+00012350: 6620 6120 7075 6c73 652e 0a20 2020 2022  f a pulse..    "
+00012360: 2222 0a20 2020 2069 6620 6375 6d75 6c61  "".    if cumula
+00012370: 6e74 5f66 756e 6374 696f 6e20 6973 204e  nt_function is N
+00012380: 6f6e 653a 0a20 2020 2020 2020 2069 6620  one:.        if 
+00012390: 7075 6c73 6520 6973 204e 6f6e 6520 6f72  pulse is None or
+000123a0: 2073 7065 6374 7275 6d20 6973 204e 6f6e   spectrum is Non
+000123b0: 6520 6f72 206f 6d65 6761 2069 7320 4e6f  e or omega is No
+000123c0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000123d0: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+000123e0: 2827 5265 7175 6972 6520 6569 7468 6572  ('Require either
+000123f0: 2070 7265 636f 6d70 7574 6564 2063 756d   precomputed cum
+00012400: 756c 616e 7420 6675 6e63 7469 6f6e 2027  ulant function '
+00012410: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012420: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
+00012430: 276f 7220 7075 6c73 652c 2073 7065 6374  'or pulse, spect
+00012440: 7275 6d2c 2061 6e64 206f 6d65 6761 2061  rum, and omega a
+00012450: 7320 6172 6775 6d65 6e74 732e 2729 0a0a  s arguments.')..
+00012460: 2020 2020 2020 2020 6375 6d75 6c61 6e74          cumulant
+00012470: 5f66 756e 6374 696f 6e20 3d20 6361 6c63  _function = calc
+00012480: 756c 6174 655f 6375 6d75 6c61 6e74 5f66  ulate_cumulant_f
+00012490: 756e 6374 696f 6e28 7075 6c73 652c 2073  unction(pulse, s
+000124a0: 7065 6374 7275 6d2c 206f 6d65 6761 2c0a  pectrum, omega,.
 000124b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000124c0: 2020 2020 2020 2027 6f72 2070 756c 7365         'or pulse
-000124d0: 2c20 7370 6563 7472 756d 2c20 616e 6420  , spectrum, and 
-000124e0: 6f6d 6567 6120 6173 2061 7267 756d 656e  omega as argumen
-000124f0: 7473 2e27 290a 0a20 2020 2020 2020 2063  ts.')..        c
-00012500: 756d 756c 616e 745f 6675 6e63 7469 6f6e  umulant_function
-00012510: 203d 2063 616c 6375 6c61 7465 5f63 756d   = calculate_cum
-00012520: 756c 616e 745f 6675 6e63 7469 6f6e 2870  ulant_function(p
-00012530: 756c 7365 2c20 7370 6563 7472 756d 2c20  ulse, spectrum, 
-00012540: 6f6d 6567 612c 0a20 2020 2020 2020 2020  omega,.         
-00012550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012570: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00012580: 5f6f 7065 725f 6964 656e 7469 6669 6572  _oper_identifier
-00012590: 732c 2027 746f 7461 6c27 2c20 7365 636f  s, 'total', seco
-000125a0: 6e64 5f6f 7264 6572 2c0a 2020 2020 2020  nd_order,.      
-000125b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000125c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000124c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000124d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000124e0: 2020 2020 2020 2020 6e5f 6f70 6572 5f69          n_oper_i
+000124f0: 6465 6e74 6966 6965 7273 2c20 2774 6f74  dentifiers, 'tot
+00012500: 616c 272c 2073 6563 6f6e 645f 6f72 6465  al', second_orde
+00012510: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
+00012520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012540: 2020 2020 2020 2020 2020 2073 686f 775f             show_
+00012550: 7072 6f67 7265 7373 6261 723d 7368 6f77  progressbar=show
+00012560: 5f70 726f 6772 6573 7362 6172 2c0a 2020  _progressbar,.  
+00012570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000125a0: 2020 2020 2020 6d65 6d6f 7279 5f70 6172        memory_par
+000125b0: 7369 6d6f 6e69 6f75 733d 6d65 6d6f 7279  simonious=memory
+000125c0: 5f70 6172 7369 6d6f 6e69 6f75 732c 0a20  _parsimonious,. 
 000125d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000125e0: 2020 7368 6f77 5f70 726f 6772 6573 7362    show_progressb
-000125f0: 6172 3d73 686f 775f 7072 6f67 7265 7373  ar=show_progress
-00012600: 6261 722c 0a20 2020 2020 2020 2020 2020  bar,.           
-00012610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012630: 2020 2020 2020 2020 2020 2020 206d 656d               mem
-00012640: 6f72 795f 7061 7273 696d 6f6e 696f 7573  ory_parsimonious
-00012650: 3d6d 656d 6f72 795f 7061 7273 696d 6f6e  =memory_parsimon
-00012660: 696f 7573 2c0a 2020 2020 2020 2020 2020  ious,.          
-00012670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012690: 2020 2020 2020 2020 2020 2020 2020 6361                ca
-000126a0: 6368 655f 696e 7465 726d 6564 6961 7465  che_intermediate
-000126b0: 733d 6361 6368 655f 696e 7465 726d 6564  s=cache_intermed
-000126c0: 6961 7465 7329 0a0a 2020 2020 7472 793a  iates)..    try:
-000126d0: 0a20 2020 2020 2020 2023 2061 676e 6f73  .        # agnos
-000126e0: 7469 6320 6f66 2074 6865 2073 7065 6369  tic of the speci
-000126f0: 6669 6320 7368 6170 6520 6f66 2063 756d  fic shape of cum
-00012700: 756c 616e 745f 6675 6e63 7469 6f6e 2c20  ulant_function, 
-00012710: 6a75 7374 2073 756d 206f 7665 7220 6576  just sum over ev
-00012720: 6572 7974 6869 6e67 2065 7863 6570 7420  erything except 
-00012730: 666f 720a 2020 2020 2020 2020 2320 7468  for.        # th
-00012740: 6520 6261 7369 7320 656c 656d 656e 7473  e basis elements
-00012750: 2074 6861 7420 7369 7420 6f6e 2074 6865   that sit on the
-00012760: 206c 6173 7420 7477 6f20 6178 6573 0a20   last two axes. 
-00012770: 2020 2020 2020 2065 7272 6f72 5f74 7261         error_tra
-00012780: 6e73 6665 725f 6d61 7472 6978 203d 2073  nsfer_matrix = s
-00012790: 6c61 2e65 7870 6d28 0a20 2020 2020 2020  la.expm(.       
-000127a0: 2020 2020 2063 756d 756c 616e 745f 6675       cumulant_fu
-000127b0: 6e63 7469 6f6e 2e73 756d 2861 7869 733d  nction.sum(axis=
-000127c0: 7475 706c 6528 7261 6e67 6528 6375 6d75  tuple(range(cumu
-000127d0: 6c61 6e74 5f66 756e 6374 696f 6e2e 6e64  lant_function.nd
-000127e0: 696d 202d 2032 2929 290a 2020 2020 2020  im - 2))).      
-000127f0: 2020 290a 2020 2020 6578 6365 7074 2041    ).    except A
-00012800: 7474 7269 6275 7465 4572 726f 7220 6173  ttributeError as
-00012810: 2061 6572 723a 0a20 2020 2020 2020 2072   aerr:.        r
-00012820: 6169 7365 2054 7970 6545 7272 6f72 2866  aise TypeError(f
-00012830: 2763 756d 756c 616e 745f 6675 6e63 7469  'cumulant_functi
-00012840: 6f6e 2069 6e76 616c 6964 2074 7970 653a  on invalid type:
-00012850: 207b 7479 7065 2863 756d 756c 616e 745f   {type(cumulant_
-00012860: 6675 6e63 7469 6f6e 297d 2729 2066 726f  function)}') fro
-00012870: 6d20 6165 7272 0a20 2020 2065 7863 6570  m aerr.    excep
-00012880: 7420 5661 6c75 6545 7272 6f72 2061 7320  t ValueError as 
-00012890: 7665 7272 3a0a 2020 2020 2020 2020 7261  verr:.        ra
-000128a0: 6973 6520 5661 6c75 6545 7272 6f72 2866  ise ValueError(f
-000128b0: 2763 756d 756c 616e 745f 6675 6e63 7469  'cumulant_functi
-000128c0: 6f6e 2069 6e76 616c 6964 2073 6861 7065  on invalid shape
-000128d0: 3a20 7b63 756d 756c 616e 745f 6675 6e63  : {cumulant_func
-000128e0: 7469 6f6e 2e73 6861 7065 7d27 2920 6672  tion.shape}') fr
-000128f0: 6f6d 2076 6572 720a 0a20 2020 2072 6574  om verr..    ret
-00012900: 7572 6e20 6572 726f 725f 7472 616e 7366  urn error_transf
-00012910: 6572 5f6d 6174 7269 780a 0a0a 4075 7469  er_matrix...@uti
-00012920: 6c2e 7061 7273 655f 6f70 7469 6f6e 616c  l.parse_optional
-00012930: 5f70 6172 616d 6574 6572 7328 7768 6963  _parameters(whic
-00012940: 683d 2827 746f 7461 6c27 2c20 2763 6f72  h=('total', 'cor
-00012950: 7265 6c61 7469 6f6e 7327 2929 0a64 6566  relations')).def
-00012960: 2069 6e66 6964 656c 6974 7928 0a20 2020   infidelity(.   
-00012970: 2020 2020 2070 756c 7365 3a20 2750 756c       pulse: 'Pul
-00012980: 7365 5365 7175 656e 6365 272c 0a20 2020  seSequence',.   
-00012990: 2020 2020 2073 7065 6374 7275 6d3a 2055       spectrum: U
-000129a0: 6e69 6f6e 5b43 6f65 6666 6963 6965 6e74  nion[Coefficient
-000129b0: 732c 2043 616c 6c61 626c 655d 2c0a 2020  s, Callable],.  
-000129c0: 2020 2020 2020 6f6d 6567 613a 2055 6e69        omega: Uni
-000129d0: 6f6e 5b43 6f65 6666 6963 6965 6e74 732c  on[Coefficients,
-000129e0: 2044 6963 745b 7374 722c 2055 6e69 6f6e   Dict[str, Union
-000129f0: 5b69 6e74 2c20 7374 725d 5d5d 2c0a 2020  [int, str]]],.  
-00012a00: 2020 2020 2020 6e5f 6f70 6572 5f69 6465        n_oper_ide
-00012a10: 6e74 6966 6965 7273 3a20 4f70 7469 6f6e  ntifiers: Option
-00012a20: 616c 5b53 6571 7565 6e63 655b 7374 725d  al[Sequence[str]
-00012a30: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-00012a40: 2020 7768 6963 683a 2073 7472 203d 2027    which: str = '
-00012a50: 746f 7461 6c27 2c0a 2020 2020 2020 2020  total',.        
-00012a60: 7368 6f77 5f70 726f 6772 6573 7362 6172  show_progressbar
-00012a70: 3a20 626f 6f6c 203d 2046 616c 7365 2c0a  : bool = False,.
-00012a80: 2020 2020 2020 2020 6361 6368 655f 696e          cache_in
-00012a90: 7465 726d 6564 6961 7465 733a 2062 6f6f  termediates: boo
-00012aa0: 6c20 3d20 4661 6c73 652c 0a20 2020 2020  l = False,.     
-00012ab0: 2020 2072 6574 7572 6e5f 736d 616c 6c6e     return_smalln
-00012ac0: 6573 733a 2062 6f6f 6c20 3d20 4661 6c73  ess: bool = Fals
-00012ad0: 652c 0a20 2020 2020 2020 2074 6573 745f  e,.        test_
-00012ae0: 636f 6e76 6572 6765 6e63 653a 2062 6f6f  convergence: boo
-00012af0: 6c20 3d20 4661 6c73 650a 2920 2d3e 2055  l = False.) -> U
-00012b00: 6e69 6f6e 5b6e 6461 7272 6179 2c20 416e  nion[ndarray, An
-00012b10: 795d 3a0a 2020 2020 7222 2222 4361 6c63  y]:.    r"""Calc
-00012b20: 756c 6174 6520 7468 6520 6c65 6164 696e  ulate the leadin
-00012b30: 6720 6f72 6465 7220 656e 7461 6e67 6c65  g order entangle
-00012b40: 6d65 6e74 2069 6e66 6964 656c 6974 792e  ment infidelity.
-00012b50: 0a0a 2020 2020 5468 6973 2066 756e 6374  ..    This funct
-00012b60: 696f 6e20 6361 6c63 756c 6174 6573 2074  ion calculates t
-00012b70: 6865 2069 6e66 6964 656c 6974 7920 6170  he infidelity ap
-00012b80: 7072 6f78 696d 6174 656c 7920 6672 6f6d  proximately from
-00012b90: 2074 6865 0a20 2020 206c 6561 6469 6e67   the.    leading
-00012ba0: 2070 6574 7572 6261 7469 6f6e 2028 7365   peturbation (se
-00012bb0: 6520 3a72 6566 3a60 4e6f 7465 7320 3c6e  e :ref:`Notes <n
-00012bc0: 6f74 6573 3e60 292e 2054 6f20 636f 6d70  otes>`). To comp
-00012bd0: 7574 6520 6974 0a20 2020 2065 7861 6374  ute it.    exact
-00012be0: 6c79 2066 6f72 2047 6175 7373 6961 6e20  ly for Gaussian 
-00012bf0: 6e6f 6973 6520 616e 6420 7661 6e69 7368  noise and vanish
-00012c00: 696e 6720 636f 6865 7265 6e74 2065 7272  ing coherent err
-00012c10: 6f72 7320 2873 6563 6f6e 640a 2020 2020  ors (second.    
-00012c20: 6f72 6465 7220 4d61 676e 7573 2074 6572  order Magnus ter
-00012c30: 6d73 292c 2075 7365 203a 6675 6e63 3a60  ms), use :func:`
-00012c40: 6572 726f 725f 7472 616e 7366 6572 5f6d  error_transfer_m
-00012c50: 6174 7269 7860 2074 6f20 6f62 7461 696e  atrix` to obtain
-00012c60: 2069 740a 2020 2020 6672 6f6d 2074 6865   it.    from the
-00012c70: 2066 756c 6c20 7072 6f63 6573 7320 6d61   full process ma
-00012c80: 7472 6978 2e0a 0a20 2020 2050 6172 616d  trix...    Param
-00012c90: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
-00012ca0: 2d2d 2d2d 0a20 2020 2070 756c 7365 3a20  ----.    pulse: 
-00012cb0: 5075 6c73 6553 6571 7565 6e63 650a 2020  PulseSequence.  
-00012cc0: 2020 2020 2020 5468 6520 6060 5075 6c73        The ``Puls
-00012cd0: 6553 6571 7565 6e63 6560 6020 696e 7374  eSequence`` inst
-00012ce0: 616e 6365 2066 6f72 2077 6869 6368 2074  ance for which t
-00012cf0: 6f20 6361 6c63 756c 6174 6520 7468 650a  o calculate the.
-00012d00: 2020 2020 2020 2020 696e 6669 6465 6c69          infideli
-00012d10: 7479 2066 6f72 2e0a 2020 2020 7370 6563  ty for..    spec
-00012d20: 7472 756d 3a20 6172 7261 795f 6c69 6b65  trum: array_like
-00012d30: 2c20 7368 6170 6520 285b 5b6e 5f6e 6f70  , shape ([[n_nop
-00012d40: 732c 5d20 6e5f 6e6f 7073 2c5d 206f 6d65  s,] n_nops,] ome
-00012d50: 6761 2920 6f72 2063 616c 6c61 626c 650a  ga) or callable.
-00012d60: 2020 2020 2020 2020 5468 6520 7477 6f2d          The two-
-00012d70: 7369 6465 6420 6e6f 6973 6520 706f 7765  sided noise powe
-00012d80: 7220 7370 6563 7472 616c 2064 656e 7369  r spectral densi
-00012d90: 7479 2069 6e20 756e 6974 7320 6f66 2069  ty in units of i
-00012da0: 6e76 6572 7365 0a20 2020 2020 2020 2066  nverse.        f
-00012db0: 7265 7175 656e 6369 6573 2061 7320 616e  requencies as an
-00012dc0: 2061 7272 6179 206f 6620 7368 6170 6520   array of shape 
-00012dd0: 286e 5f6f 6d65 6761 2c29 2c20 286e 5f6e  (n_omega,), (n_n
-00012de0: 6f70 732c 206e 5f6f 6d65 6761 292c 0a20  ops, n_omega),. 
-00012df0: 2020 2020 2020 206f 7220 286e 5f6e 6f70         or (n_nop
-00012e00: 732c 206e 5f6e 6f70 732c 206e 5f6f 6d65  s, n_nops, n_ome
-00012e10: 6761 292e 2049 6e20 7468 6520 6669 7273  ga). In the firs
-00012e20: 7420 6361 7365 2c20 7468 6520 7361 6d65  t case, the same
-00012e30: 0a20 2020 2020 2020 2073 7065 6374 7275  .        spectru
-00012e40: 6d20 6973 2074 616b 656e 2066 6f72 2061  m is taken for a
-00012e50: 6c6c 206e 6f69 7365 206f 7065 7261 746f  ll noise operato
-00012e60: 7273 2c20 696e 2074 6865 2073 6563 6f6e  rs, in the secon
-00012e70: 642c 2069 7420 6973 0a20 2020 2020 2020  d, it is.       
-00012e80: 2061 7373 756d 6564 2074 6861 7420 7468   assumed that th
-00012e90: 6572 6520 6172 6520 6e6f 2063 6f72 7265  ere are no corre
-00012ea0: 6c61 7469 6f6e 7320 6265 7477 6565 6e20  lations between 
-00012eb0: 6469 6666 6572 656e 7420 6e6f 6973 650a  different noise.
-00012ec0: 2020 2020 2020 2020 736f 7572 6365 7320          sources 
-00012ed0: 616e 6420 7468 7573 2074 6865 7265 2069  and thus there i
-00012ee0: 7320 6f6e 6520 7370 6563 7472 756d 2066  s one spectrum f
-00012ef0: 6f72 2065 6163 6820 6e6f 6973 6520 6f70  or each noise op
-00012f00: 6572 6174 6f72 2e0a 2020 2020 2020 2020  erator..        
-00012f10: 496e 2074 6865 2074 6869 7264 2061 6e64  In the third and
-00012f20: 206d 6f73 7420 6765 6e65 7261 6c20 6361   most general ca
-00012f30: 7365 2c20 7468 6572 6520 6d61 7920 6265  se, there may be
-00012f40: 2061 2073 7065 6374 7275 6d20 666f 720a   a spectrum for.
-00012f50: 2020 2020 2020 2020 6561 6368 2070 6169          each pai
-00012f60: 7220 6f66 206e 6f69 7365 206f 7065 7261  r of noise opera
-00012f70: 746f 7273 2063 6f72 7265 7370 6f6e 6469  tors correspondi
-00012f80: 6e67 2074 6f20 7468 6520 636f 7272 656c  ng to the correl
-00012f90: 6174 696f 6e73 0a20 2020 2020 2020 2062  ations.        b
-00012fa0: 6574 7765 656e 2074 6865 6d2e 206e 5f6e  etween them. n_n
-00012fb0: 6f70 7320 6973 2074 6865 206e 756d 6265  ops is the numbe
-00012fc0: 7220 6f66 206e 6f69 7365 206f 7065 7261  r of noise opera
-00012fd0: 746f 7273 2063 6f6e 7369 6465 7265 640a  tors considered.
-00012fe0: 2020 2020 2020 2020 616e 6420 7368 6f75          and shou
-00012ff0: 6c64 2062 6520 6571 7561 6c20 746f 2060  ld be equal to `
-00013000: 606c 656e 286e 5f6f 7065 725f 6964 656e  `len(n_oper_iden
-00013010: 7469 6669 6572 7329 6060 2e0a 0a20 2020  tifiers)``...   
-00013020: 2020 2020 2049 6620 2a74 6573 745f 636f       If *test_co
-00013030: 6e76 6572 6765 6e63 652a 2069 7320 6060  nvergence* is ``
-00013040: 5472 7565 6060 2c20 6120 6675 6e63 7469  True``, a functi
-00013050: 6f6e 2068 616e 646c 6520 746f 0a20 2020  on handle to.   
-00013060: 2020 2020 2063 6f6d 7075 7465 2074 6865       compute the
-00013070: 2070 6f77 6572 2073 7065 6374 7261 6c20   power spectral 
-00013080: 6465 6e73 6974 7920 6672 6f6d 2061 2073  density from a s
-00013090: 6571 7565 6e63 6520 6f66 0a20 2020 2020  equence of.     
-000130a0: 2020 2066 7265 7175 656e 6369 6573 2069     frequencies i
-000130b0: 7320 6578 7065 6374 6564 2e0a 2020 2020  s expected..    
-000130c0: 6f6d 6567 613a 2061 7272 6179 5f6c 696b  omega: array_lik
-000130d0: 6520 6f72 2064 6963 740a 2020 2020 2020  e or dict.      
-000130e0: 2020 5468 6520 6672 6571 7565 6e63 6965    The frequencie
-000130f0: 7320 6174 2077 6869 6368 2074 6865 2069  s at which the i
-00013100: 6e74 6567 7261 7469 6f6e 2069 7320 746f  ntegration is to
-00013110: 2062 6520 6361 7272 6965 6420 6f75 742e   be carried out.
-00013120: 0a20 2020 2020 2020 2049 6620 2a74 6573  .        If *tes
-00013130: 745f 636f 6e76 6572 6765 6e63 652a 2069  t_convergence* i
-00013140: 7320 6060 5472 7565 6060 2c20 6120 6469  s ``True``, a di
-00013150: 6374 2077 6974 6820 706f 7373 6962 6c65  ct with possible
-00013160: 206b 6579 730a 2020 2020 2020 2020 2827   keys.        ('
-00013170: 6f6d 6567 615f 4952 272c 2027 6f6d 6567  omega_IR', 'omeg
-00013180: 615f 5556 272c 2027 7370 6163 696e 6727  a_UV', 'spacing'
-00013190: 2c20 276e 5f6d 696e 272c 2027 6e5f 6d61  , 'n_min', 'n_ma
-000131a0: 7827 2c0a 2020 2020 2020 2020 276e 5f70  x',.        'n_p
-000131b0: 6f69 6e74 7327 292c 2077 6865 7265 2061  oints'), where a
-000131c0: 6c6c 2065 6e74 7269 6573 2061 7265 2069  ll entries are i
-000131d0: 6e74 6567 6572 7320 6578 6365 7074 2066  ntegers except f
-000131e0: 6f72 0a20 2020 2020 2020 2060 6073 7061  or.        ``spa
-000131f0: 6369 6e67 6060 2077 6869 6368 2073 686f  cing`` which sho
-00013200: 756c 6420 6265 2061 2073 7472 696e 672c  uld be a string,
-00013210: 2065 6974 6865 7220 276c 696e 6561 7227   either 'linear'
-00013220: 206f 7220 276c 6f67 272e 0a20 2020 2020   or 'log'..     
-00013230: 2020 2027 6e5f 706f 696e 7473 2720 636f     'n_points' co
-00013240: 6e74 726f 6c73 2068 6f77 206d 616e 7920  ntrols how many 
-00013250: 7374 6570 7320 6172 6520 7461 6b65 6e2e  steps are taken.
-00013260: 0a20 2020 206e 5f6f 7065 725f 6964 656e  .    n_oper_iden
-00013270: 7469 6669 6572 733a 2061 7272 6179 5f6c  tifiers: array_l
-00013280: 696b 652c 206f 7074 696f 6e61 6c0a 2020  ike, optional.  
-00013290: 2020 2020 2020 5468 6520 6964 656e 7469        The identi
-000132a0: 6669 6572 7320 6f66 2074 6865 206e 6f69  fiers of the noi
-000132b0: 7365 206f 7065 7261 746f 7273 2066 6f72  se operators for
-000132c0: 2077 6869 6368 2074 6f20 6361 6c63 756c   which to calcul
-000132d0: 6174 650a 2020 2020 2020 2020 7468 6520  ate.        the 
-000132e0: 696e 6669 6465 6c69 7479 2020 636f 6e74  infidelity  cont
-000132f0: 7269 6275 7469 6f6e 2e20 4966 2067 6976  ribution. If giv
-00013300: 656e 2c20 7468 6520 696e 6669 6465 6c69  en, the infideli
-00013310: 7469 6573 2066 6f72 0a20 2020 2020 2020  ties for.       
-00013320: 2065 6163 6820 6e6f 6973 6520 6f70 6572   each noise oper
-00013330: 6174 6f72 2077 696c 6c20 6265 2072 6574  ator will be ret
-00013340: 7572 6e65 642e 204f 7468 6572 7769 7365  urned. Otherwise
-00013350: 2c20 616c 6c20 6e6f 6973 650a 2020 2020  , all noise.    
-00013360: 2020 2020 6f70 6572 6174 6f72 7320 7769      operators wi
-00013370: 6c6c 2062 6520 7461 6b65 6e20 696e 746f  ll be taken into
-00013380: 2061 6363 6f75 6e74 2e0a 2020 2020 7768   account..    wh
-00013390: 6963 683a 2073 7472 2c20 6f70 7469 6f6e  ich: str, option
-000133a0: 616c 0a20 2020 2020 2020 2057 6869 6368  al.        Which
-000133b0: 2069 6e66 6964 656c 6974 6965 7320 7368   infidelities sh
-000133c0: 6f75 6c64 2062 6520 6361 6c63 756c 6174  ould be calculat
-000133d0: 6564 2c20 6d61 7920 6265 2065 6974 6865  ed, may be eithe
-000133e0: 7220 2774 6f74 616c 270a 2020 2020 2020  r 'total'.      
-000133f0: 2020 2864 6566 6175 6c74 2920 6f72 2027    (default) or '
-00013400: 636f 7272 656c 6174 696f 6e73 272e 2049  correlations'. I
-00013410: 6e20 7468 6520 666f 726d 6572 2063 6173  n the former cas
-00013420: 652c 206f 6e65 2076 616c 7565 2069 730a  e, one value is.
-00013430: 2020 2020 2020 2020 7265 7475 726e 6564          returned
-00013440: 2066 6f72 2065 6163 6820 6e6f 6973 6520   for each noise 
-00013450: 6f70 6572 6174 6f72 2c20 636f 7272 6573  operator, corres
-00013460: 706f 6e64 696e 6720 746f 2074 6865 2074  ponding to the t
-00013470: 6f74 616c 0a20 2020 2020 2020 2069 6e66  otal.        inf
-00013480: 6964 656c 6974 7920 6f66 2074 6865 2070  idelity of the p
-00013490: 756c 7365 2028 6f72 2070 756c 7365 2073  ulse (or pulse s
-000134a0: 6571 7565 6e63 6529 2e20 496e 2074 6865  equence). In the
-000134b0: 206c 6174 7465 722c 2061 6e0a 2020 2020   latter, an.    
-000134c0: 2020 2020 6172 7261 7920 6f66 2069 6e66      array of inf
-000134d0: 6964 656c 6974 6965 7320 6973 2072 6574  idelities is ret
-000134e0: 7572 6e65 6420 7768 6572 6520 656c 656d  urned where elem
-000134f0: 656e 7420 2869 2c6a 290a 2020 2020 2020  ent (i,j).      
-00013500: 2020 636f 7272 6573 706f 6e64 7320 746f    corresponds to
-00013510: 2074 6865 2069 6e66 6964 656c 6974 7920   the infidelity 
-00013520: 636f 6e74 7269 6275 7469 6f6e 206f 6620  contribution of 
-00013530: 7468 6520 636f 7272 656c 6174 696f 6e73  the correlations
-00013540: 0a20 2020 2020 2020 2062 6574 7765 656e  .        between
-00013550: 2070 756c 7365 7320 6920 616e 6420 6a20   pulses i and j 
-00013560: 2873 6565 203a 7265 663a 604e 6f74 6573  (see :ref:`Notes
-00013570: 203c 6e6f 7465 733e 6029 2e20 4e6f 7465   <notes>`). Note
-00013580: 2074 6861 740a 2020 2020 2020 2020 7468   that.        th
-00013590: 6973 206f 7074 696f 6e20 6973 206f 6e6c  is option is onl
-000135a0: 7920 6176 6169 6c61 626c 6520 6966 2074  y available if t
-000135b0: 6865 2070 756c 7365 2063 6f72 7265 6c61  he pulse correla
-000135c0: 7469 6f6e 2066 696c 7465 720a 2020 2020  tion filter.    
-000135d0: 2020 2020 6675 6e63 7469 6f6e 7320 6861      functions ha
-000135e0: 7665 2062 6565 6e20 636f 6d70 7574 6564  ve been computed
-000135f0: 2064 7572 696e 6720 636f 6e63 6174 656e   during concaten
-00013600: 6174 696f 6e20 2873 6565 0a20 2020 2020  ation (see.     
-00013610: 2020 203a 6675 6e63 3a60 6361 6c63 756c     :func:`calcul
-00013620: 6174 655f 7075 6c73 655f 636f 7272 656c  ate_pulse_correl
-00013630: 6174 696f 6e5f 6669 6c74 6572 5f66 756e  ation_filter_fun
-00013640: 6374 696f 6e60 2061 6e64 0a20 2020 2020  ction` and.     
-00013650: 2020 203a 6675 6e63 3a60 7e66 696c 7465     :func:`~filte
-00013660: 725f 6675 6e63 7469 6f6e 732e 7075 6c73  r_functions.puls
-00013670: 655f 7365 7175 656e 6365 2e63 6f6e 6361  e_sequence.conca
-00013680: 7465 6e61 7465 6029 2e0a 2020 2020 7368  tenate`)..    sh
-00013690: 6f77 5f70 726f 6772 6573 7362 6172 3a20  ow_progressbar: 
-000136a0: 626f 6f6c 2c20 6f70 7469 6f6e 616c 0a20  bool, optional. 
-000136b0: 2020 2020 2020 2053 686f 7720 6120 7072         Show a pr
-000136c0: 6f67 7265 7373 6261 7220 666f 7220 7468  ogressbar for th
-000136d0: 6520 6361 6c63 756c 6174 696f 6e20 6f66  e calculation of
-000136e0: 2074 6865 2063 6f6e 7472 6f6c 206d 6174   the control mat
-000136f0: 7269 782e 0a20 2020 2063 6163 6865 5f69  rix..    cache_i
-00013700: 6e74 6572 6d65 6469 6174 6573 3a20 626f  ntermediates: bo
-00013710: 6f6c 2c20 6f70 7469 6f6e 616c 0a20 2020  ol, optional.   
-00013720: 2020 2020 204b 6565 7020 616e 6420 7265       Keep and re
-00013730: 7475 726e 2069 6e74 6572 6d65 6469 6174  turn intermediat
-00013740: 6520 7465 726d 7320 6f66 2074 6865 2063  e terms of the c
-00013750: 616c 6375 6c61 7469 6f6e 206f 6620 7468  alculation of th
-00013760: 650a 2020 2020 2020 2020 636f 6e74 726f  e.        contro
-00013770: 6c20 6d61 7472 6978 2028 6966 2069 7420  l matrix (if it 
-00013780: 6973 206e 6f74 2061 6c72 6561 6479 2063  is not already c
-00013790: 6163 6865 6429 2074 6861 7420 6361 6e20  ached) that can 
-000137a0: 6265 2072 6575 7365 640a 2020 2020 2020  be reused.      
-000137b0: 2020 666f 7220 7365 636f 6e64 206f 7264    for second ord
-000137c0: 6572 206f 7220 6772 6164 6965 6e74 732e  er or gradients.
-000137d0: 2054 6865 2064 6566 6175 6c74 2069 7320   The default is 
-000137e0: 4661 6c73 652e 0a20 2020 2072 6574 7572  False..    retur
-000137f0: 6e5f 736d 616c 6c6e 6573 733a 2062 6f6f  n_smallness: boo
-00013800: 6c2c 206f 7074 696f 6e61 6c0a 2020 2020  l, optional.    
-00013810: 2020 2020 5265 7475 726e 2074 6865 2073      Return the s
-00013820: 6d61 6c6c 6e65 7373 2070 6172 616d 6574  mallness paramet
-00013830: 6572 203a 6d61 7468 3a60 5c78 6960 2066  er :math:`\xi` f
-00013840: 6f72 2074 6865 2067 6976 656e 0a20 2020  or the given.   
-00013850: 2020 2020 2073 7065 6374 7275 6d2e 0a20       spectrum.. 
-00013860: 2020 2074 6573 745f 636f 6e76 6572 6765     test_converge
-00013870: 6e63 653a 2062 6f6f 6c2c 206f 7074 696f  nce: bool, optio
-00013880: 6e61 6c0a 2020 2020 2020 2020 5465 7374  nal.        Test
-00013890: 2074 6865 2063 6f6e 7665 7267 656e 6365   the convergence
-000138a0: 206f 6620 7468 6520 696e 7465 6772 616c   of the integral
-000138b0: 2077 6974 6820 7265 7370 6563 7420 746f   with respect to
-000138c0: 2074 6865 206e 756d 6265 720a 2020 2020   the number.    
-000138d0: 2020 2020 6f66 2066 7265 7175 656e 6379      of frequency
-000138e0: 2073 616d 706c 6573 2e20 5265 7475 726e   samples. Return
-000138f0: 7320 7468 6520 6e75 6d62 6572 206f 6620  s the number of 
-00013900: 6672 6571 7565 6e63 7920 7361 6d70 6c65  frequency sample
-00013910: 730a 2020 2020 2020 2020 616e 6420 7468  s.        and th
-00013920: 6520 636f 7272 6573 706f 6e64 696e 6720  e corresponding 
-00013930: 6669 6465 6c69 7469 6573 2e20 5365 6520  fidelities. See 
-00013940: 2a73 7065 6374 7275 6d2a 2061 6e64 202a  *spectrum* and *
-00013950: 6f6d 6567 612a 2066 6f72 0a20 2020 2020  omega* for.     
-00013960: 2020 206d 6f72 6520 696e 666f 726d 6174     more informat
-00013970: 696f 6e2e 0a0a 2020 2020 5265 7475 726e  ion...    Return
-00013980: 730a 2020 2020 2d2d 2d2d 2d2d 2d0a 2020  s.    -------.  
-00013990: 2020 696e 6669 643a 206e 6461 7272 6179    infid: ndarray
-000139a0: 2c20 7368 6170 6520 285b 5b6e 5f70 6c73  , shape ([[n_pls
-000139b0: 2c20 6e5f 706c 732c 5d2c 206e 5f6e 6f70  , n_pls,], n_nop
-000139c0: 732c 5d20 6e5f 6e6f 7073 290a 2020 2020  s,] n_nops).    
-000139d0: 2020 2020 4172 7261 7920 7769 7468 2074      Array with t
-000139e0: 6865 2069 6e66 6964 656c 6974 7920 636f  he infidelity co
-000139f0: 6e74 7269 6275 7469 6f6e 7320 666f 7220  ntributions for 
-00013a00: 6561 6368 2073 7065 6374 7275 6d0a 2020  each spectrum.  
-00013a10: 2020 2020 2020 2a73 7065 6374 7275 6d2a        *spectrum*
-00013a20: 206f 6e20 7468 6520 6c61 7374 2061 7869   on the last axi
-00013a30: 7320 6f72 2061 7865 732c 2064 6570 656e  s or axes, depen
-00013a40: 6469 6e67 206f 6e20 7468 6520 7368 6170  ding on the shap
-00013a50: 6520 6f66 0a20 2020 2020 2020 202a 7370  e of.        *sp
-00013a60: 6563 7472 756d 2a20 616e 6420 2a77 6869  ectrum* and *whi
-00013a70: 6368 2a2e 2049 6620 6060 7768 6963 6860  ch*. If ``which`
-00013a80: 6020 6973 2060 6063 6f72 7265 6c61 7469  ` is ``correlati
-00013a90: 6f6e 7360 602c 2074 6865 0a20 2020 2020  ons``, the.     
-00013aa0: 2020 2066 6972 7374 2074 776f 2061 7865     first two axe
-00013ab0: 7320 6172 6520 7468 6520 696e 6469 7669  s are the indivi
-00013ac0: 6475 616c 2070 756c 7365 2063 6f6e 7472  dual pulse contr
-00013ad0: 6962 7574 696f 6e73 2e20 4966 0a20 2020  ibutions. If.   
-00013ae0: 2020 2020 202a 7370 6563 7472 756d 2a20       *spectrum* 
-00013af0: 6973 2032 2d64 2028 332d 6429 2c20 7468  is 2-d (3-d), th
-00013b00: 6520 6c61 7374 2061 7869 7320 2874 776f  e last axis (two
-00013b10: 2061 7865 7329 2061 7265 2074 6865 0a20   axes) are the. 
-00013b20: 2020 2020 2020 2069 6e64 6976 6964 7561         individua
-00013b30: 6c20 7370 6563 7472 616c 2063 6f6e 7472  l spectral contr
-00013b40: 6962 7574 696f 6e73 2e20 4f6e 6c79 2069  ibutions. Only i
-00013b50: 6620 2a74 6573 745f 636f 6e76 6572 6765  f *test_converge
-00013b60: 6e63 652a 2069 730a 2020 2020 2020 2020  nce* is.        
-00013b70: 6060 4661 6c73 6560 602e 0a20 2020 206e  ``False``..    n
-00013b80: 5f73 616d 706c 6573 3a20 6172 7261 795f  _samples: array_
-00013b90: 6c69 6b65 0a20 2020 2020 2020 2041 7272  like.        Arr
-00013ba0: 6179 2077 6974 6820 6e75 6d62 6572 206f  ay with number o
-00013bb0: 6620 6672 6571 7565 6e63 7920 7361 6d70  f frequency samp
-00013bc0: 6c65 7320 7573 6564 2066 6f72 2063 6f6e  les used for con
-00013bd0: 7665 7267 656e 6365 0a20 2020 2020 2020  vergence.       
-00013be0: 2074 6573 742e 204f 6e6c 7920 6966 202a   test. Only if *
-00013bf0: 7465 7374 5f63 6f6e 7665 7267 656e 6365  test_convergence
-00013c00: 2a20 6973 2060 6054 7275 6560 602e 0a20  * is ``True``.. 
-00013c10: 2020 2063 6f6e 7665 7267 656e 6365 5f69     convergence_i
-00013c20: 6e66 6964 733a 2061 7272 6179 5f6c 696b  nfids: array_lik
-00013c30: 650a 2020 2020 2020 2020 4172 7261 7920  e.        Array 
-00013c40: 7769 7468 2069 6e66 6964 656c 6974 6965  with infidelitie
-00013c50: 7320 6361 6c63 756c 6174 6564 2069 6e20  s calculated in 
-00013c60: 636f 6e76 6572 6765 6e63 6520 7465 7374  convergence test
-00013c70: 2e0a 2020 2020 2020 2020 4f6e 6c79 2069  ..        Only i
-00013c80: 6620 2a74 6573 745f 636f 6e76 6572 6765  f *test_converge
-00013c90: 6e63 652a 2069 7320 6060 5472 7565 6060  nce* is ``True``
-00013ca0: 2e0a 0a20 2020 202e 2e20 5f6e 6f74 6573  ...    .. _notes
-00013cb0: 3a0a 0a20 2020 204e 6f74 6573 0a20 2020  :..    Notes.   
-00013cc0: 202d 2d2d 2d2d 0a20 2020 2054 6865 2069   -----.    The i
-00013cd0: 6e66 6964 656c 6974 7920 6973 2067 6976  nfidelity is giv
-00013ce0: 656e 2062 790a 0a20 2020 202e 2e20 6d61  en by..    .. ma
-00013cf0: 7468 3a3a 0a0a 2020 2020 2020 2020 5c6d  th::..        \m
-00013d00: 6174 6863 616c 7b49 7d5f 7b5c 616c 7068  athcal{I}_{\alph
-00013d10: 615c 6265 7461 7d0a 2020 2020 2020 2020  a\beta}.        
-00013d20: 2020 2020 263d 2031 202d 205c 6672 6163      &= 1 - \frac
-00013d30: 7b31 7d7b 645e 327d 5c6d 6174 6872 6d7b  {1}{d^2}\mathrm{
-00013d40: 7472 7d5c 3a5c 7469 6c64 657b 5c6d 6174  tr}\:\tilde{\mat
-00013d50: 6863 616c 7b55 7d7d 205c 5c0a 2020 2020  hcal{U}} \\.    
-00013d60: 2020 2020 2020 2020 263d 205c 6672 6163          &= \frac
-00013d70: 7b31 7d7b 647d 5c69 6e74 5f7b 2d5c 696e  {1}{d}\int_{-\in
-00013d80: 6674 797d 5e7b 5c69 6e66 7479 7d0a 2020  fty}^{\infty}.  
-00013d90: 2020 2020 2020 2020 2020 2020 2020 5c66                \f
-00013da0: 7261 637b 5c6d 6174 6872 6d7b 647d 5c6f  rac{\mathrm{d}\o
-00013db0: 6d65 6761 7d7b 325c 7069 7d53 5f7b 5c61  mega}{2\pi}S_{\a
-00013dc0: 6c70 6861 5c62 6574 617d 285c 6f6d 6567  lpha\beta}(\omeg
-00013dd0: 6129 0a20 2020 2020 2020 2020 2020 2020  a).             
-00013de0: 2020 2046 5f7b 5c61 6c70 6861 5c62 6574     F_{\alpha\bet
-00013df0: 617d 285c 6f6d 6567 6129 202b 205c 6d61  a}(\omega) + \ma
-00013e00: 7468 6361 6c7b 4f7d 5c62 6967 285c 7869  thcal{O}\big(\xi
-00013e10: 5e34 5c62 6967 2920 5c5c 0a20 2020 2020  ^4\big) \\.     
-00013e20: 2020 2020 2020 2026 3d20 5c73 756d 5f7b         &= \sum_{
-00013e30: 672c 6727 3d31 7d5e 4720 5c6d 6174 6863  g,g'=1}^G \mathc
-00013e40: 616c 7b49 7d5f 7b5c 616c 7068 615c 6265  al{I}_{\alpha\be
-00013e50: 7461 7d5e 7b28 6767 2729 7d0a 0a20 2020  ta}^{(gg')}..   
-00013e60: 2077 6974 6820 3a6d 6174 683a 6053 5f7b   with :math:`S_{
-00013e70: 5c61 6c70 6861 5c62 6574 617d 285c 6f6d  \alpha\beta}(\om
-00013e80: 6567 6129 6020 7468 6520 7477 6f2d 7369  ega)` the two-si
-00013e90: 6465 6420 6e6f 6973 6520 7370 6563 7472  ded noise spectr
-00013ea0: 616c 0a20 2020 2064 656e 7369 7479 2061  al.    density a
-00013eb0: 6e64 203a 6d61 7468 3a60 465f 7b5c 616c  nd :math:`F_{\al
-00013ec0: 7068 615c 6265 7461 7d28 5c6f 6d65 6761  pha\beta}(\omega
-00013ed0: 2960 2074 6865 2066 6972 7374 2d6f 7264  )` the first-ord
-00013ee0: 6572 2066 696c 7465 720a 2020 2020 6675  er filter.    fu
-00013ef0: 6e63 7469 6f6e 2066 6f72 206e 6f69 7365  nction for noise
-00013f00: 2073 6f75 7263 6573 203a 6d61 7468 3a60   sources :math:`
-00013f10: 5c61 6c70 6861 2c5c 6265 7461 602e 2054  \alpha,\beta`. T
-00013f20: 6865 206e 6f69 7365 2073 7065 6374 7275  he noise spectru
-00013f30: 6d0a 2020 2020 6d61 7920 696e 636c 7564  m.    may includ
-00013f40: 6520 636f 7272 656c 6174 6564 206e 6f69  e correlated noi
-00013f50: 7365 2073 6f75 7263 6573 2c20 7468 6174  se sources, that
-00013f60: 2069 732c 2069 7473 2065 6e74 7279 2061   is, its entry a
-00013f70: 740a 2020 2020 3a6d 6174 683a 6028 5c61  t.    :math:`(\a
-00013f80: 6c70 6861 2c5c 6265 7461 2960 2063 6f72  lpha,\beta)` cor
-00013f90: 7265 7370 6f6e 6473 2074 6f20 7468 6520  responds to the 
-00013fa0: 636f 7272 656c 6174 696f 6e73 2062 6574  correlations bet
-00013fb0: 7765 656e 0a20 2020 2073 6f75 7263 6573  ween.    sources
-00013fc0: 203a 6d61 7468 3a60 5c61 6c70 6861 6020   :math:`\alpha` 
-00013fd0: 616e 6420 3a6d 6174 683a 605c 6265 7461  and :math:`\beta
-00013fe0: 602e 0a20 2020 203a 6d61 7468 3a60 5c6d  `..    :math:`\m
-00013ff0: 6174 6863 616c 7b49 7d5f 7b5c 616c 7068  athcal{I}_{\alph
-00014000: 615c 6265 7461 7d5e 7b28 6767 2729 7d60  a\beta}^{(gg')}`
-00014010: 2061 7265 2074 6865 2063 6f72 7265 6c61   are the correla
-00014020: 7469 6f6e 0a20 2020 2069 6e66 6964 656c  tion.    infidel
-00014030: 6974 6965 7320 7468 6174 2063 616e 2062  ities that can b
-00014040: 6520 636f 6d70 7574 6564 2062 7920 7365  e computed by se
-00014050: 7474 696e 670a 2020 2020 6060 7768 6963  tting.    ``whic
-00014060: 683d 2763 6f72 7265 6c61 7469 6f6e 7327  h='correlations'
-00014070: 6060 2e0a 0a0a 2020 2020 546f 2063 6f6e  ``....    To con
-00014080: 7665 7274 2074 6f20 7468 6520 6176 6572  vert to the aver
-00014090: 6167 6520 6761 7465 2069 6e66 6964 656c  age gate infidel
-000140a0: 6974 792c 2075 7365 2074 6865 0a20 2020  ity, use the.   
-000140b0: 2066 6f6c 6c6f 7769 6e67 2072 656c 6174   following relat
-000140c0: 696f 6e20 6769 7665 6e20 6279 2048 6f72  ion given by Hor
-000140d0: 6f64 6563 6b69 2065 7420 616c 2e20 5b48  odecki et al. [H
-000140e0: 6f72 3939 5d5f 2061 6e64 0a20 2020 204e  or99]_ and.    N
-000140f0: 6965 6c73 656e 205b 4e69 6530 325d 5f3a  ielsen [Nie02]_:
-00014100: 0a0a 2020 2020 2e2e 206d 6174 683a 3a0a  ..    .. math::.
-00014110: 0a20 2020 2020 2020 205c 6d61 7468 6361  .        \mathca
-00014120: 6c7b 497d 5f5c 6d61 7468 726d 7b61 7667  l{I}_\mathrm{avg
-00014130: 7d20 3d20 5c66 7261 637b 647d 7b64 2b31  } = \frac{d}{d+1
-00014140: 7d5c 6d61 7468 6361 6c7b 497d 2e0a 0a20  }\mathcal{I}... 
-00014150: 2020 2054 6865 2073 6d61 6c6c 6e65 7373     The smallness
-00014160: 2070 6172 616d 6574 6572 2069 7320 6769   parameter is gi
-00014170: 7665 6e20 6279 0a0a 2020 2020 2e2e 206d  ven by..    .. m
-00014180: 6174 683a 3a0a 0a20 2020 2020 2020 205c  ath::..        \
-00014190: 7869 5e32 203d 205c 7375 6d5f 5c61 6c70  xi^2 = \sum_\alp
-000141a0: 6861 5c6c 6566 745b 0a20 2020 2020 2020  ha\left[.       
-000141b0: 2020 2020 2020 2020 2020 2020 205c 6c76               \lv
-000141c0: 6572 745c 6c76 6572 7420 425f 5c61 6c70  ert\lvert B_\alp
-000141d0: 6861 5c72 7665 7274 5c72 7665 7274 5e32  ha\rvert\rvert^2
-000141e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000141f0: 2020 2020 205c 696e 745f 7b2d 5c69 6e66       \int_{-\inf
-00014200: 7479 7d5e 5c69 6e66 7479 5c66 7261 637b  ty}^\infty\frac{
-00014210: 5c6d 6174 6872 6d7b 647d 5c6f 6d65 6761  \mathrm{d}\omega
-00014220: 7d7b 325c 7069 7d0a 2020 2020 2020 2020  }{2\pi}.        
-00014230: 2020 2020 2020 2020 2020 2020 535f 5c61              S_\a
-00014240: 6c70 6861 285c 6f6d 6567 6129 5c6c 6566  lpha(\omega)\lef
-00014250: 7428 5c73 756d 5f67 735f 5c61 6c70 6861  t(\sum_gs_\alpha
-00014260: 5e7b 2867 297d 5c44 656c 7461 2074 5f67  ^{(g)}\Delta t_g
-00014270: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014280: 2020 2020 205c 7269 6768 7429 5e32 0a20       \right)^2. 
-00014290: 2020 2020 2020 2020 2020 2020 2020 205c                 \
-000142a0: 7269 6768 745d 2e0a 0a20 2020 204e 6f74  right]...    Not
-000142b0: 6520 7468 6174 2069 6e20 7072 6163 7469  e that in practi
-000142c0: 6365 2c20 7468 6520 696e 7465 6772 616c  ce, the integral
-000142d0: 2069 7320 6f6e 6c79 2065 7661 6c75 6174   is only evaluat
-000142e0: 6564 206f 6e20 7468 650a 2020 2020 696e  ed on the.    in
-000142f0: 7465 7276 616c 203a 6d61 7468 3a60 5c6f  terval :math:`\o
-00014300: 6d65 6761 5c69 6e5b 5c6f 6d65 6761 5f5c  mega\in[\omega_\
-00014310: 6d61 7468 726d 7b6d 696e 7d2c 5c6f 6d65  mathrm{min},\ome
-00014320: 6761 5f5c 6d61 7468 726d 7b6d 6178 7d5d  ga_\mathrm{max}]
-00014330: 602e 0a0a 2020 2020 5365 6520 416c 736f  `...    See Also
-00014340: 0a20 2020 202d 2d2d 2d2d 2d2d 2d0a 2020  .    --------.  
-00014350: 2020 6361 6c63 756c 6174 655f 6465 6361    calculate_deca
-00014360: 795f 616d 706c 6974 7564 6573 3a20 4361  y_amplitudes: Ca
-00014370: 6c63 756c 6174 6520 7468 6520 6675 6c6c  lculate the full
-00014380: 206d 6174 7269 7820 6f66 2066 6972 7374   matrix of first
-00014390: 206f 7264 6572 2074 6572 6d73 2e0a 2020   order terms..  
-000143a0: 2020 6572 726f 725f 7472 616e 7366 6572    error_transfer
-000143b0: 5f6d 6174 7269 783a 2043 616c 6375 6c61  _matrix: Calcula
-000143c0: 7465 2074 6865 2066 756c 6c20 7072 6f63  te the full proc
-000143d0: 6573 7320 6d61 7472 6978 2e0a 2020 2020  ess matrix..    
-000143e0: 706c 6f74 7469 6e67 2e70 6c6f 745f 696e  plotting.plot_in
-000143f0: 6669 6465 6c69 7479 5f63 6f6e 7665 7267  fidelity_converg
-00014400: 656e 6365 3a20 436f 6e76 656e 6965 6e63  ence: Convenienc
-00014410: 6520 6675 6e63 7469 6f6e 2074 6f20 706c  e function to pl
-00014420: 6f74 2072 6573 756c 7473 2e0a 2020 2020  ot results..    
-00014430: 7075 6c73 655f 7365 7175 656e 6365 2e63  pulse_sequence.c
-00014440: 6f6e 6361 7465 6e61 7465 3a20 436f 6e63  oncatenate: Conc
-00014450: 6174 656e 6174 6520 6060 5075 6c73 6553  atenate ``PulseS
-00014460: 6571 7565 6e63 6560 6020 6f62 6a65 6374  equence`` object
-00014470: 732e 0a20 2020 2063 616c 6375 6c61 7465  s..    calculate
-00014480: 5f70 756c 7365 5f63 6f72 7265 6c61 7469  _pulse_correlati
-00014490: 6f6e 5f66 696c 7465 725f 6675 6e63 7469  on_filter_functi
-000144a0: 6f6e 2e0a 0a20 2020 2052 6566 6572 656e  on...    Referen
-000144b0: 6365 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ces.    --------
-000144c0: 2d2d 0a0a 2020 2020 2e2e 205b 486f 7239  --..    .. [Hor9
-000144d0: 395d 0a20 2020 2020 2020 2048 6f72 6f64  9].        Horod
-000144e0: 6563 6b69 2c20 4d2e 2c20 486f 726f 6465  ecki, M., Horode
-000144f0: 636b 692c 2050 2e2c 2026 2048 6f72 6f64  cki, P., & Horod
-00014500: 6563 6b69 2c20 522e 2028 3139 3939 292e  ecki, R. (1999).
-00014510: 2047 656e 6572 616c 0a20 2020 2020 2020   General.       
-00014520: 2074 656c 6570 6f72 7461 7469 6f6e 2063   teleportation c
-00014530: 6861 6e6e 656c 2c20 7369 6e67 6c65 7420  hannel, singlet 
-00014540: 6672 6163 7469 6f6e 2c20 616e 6420 7175  fraction, and qu
-00014550: 6173 6964 6973 7469 6c6c 6174 696f 6e2e  asidistillation.
-00014560: 0a20 2020 2020 2020 2050 6879 7369 6361  .        Physica
-00014570: 6c20 5265 7669 6577 2041 202d 2041 746f  l Review A - Ato
-00014580: 6d69 632c 204d 6f6c 6563 756c 6172 2c20  mic, Molecular, 
-00014590: 616e 6420 4f70 7469 6361 6c20 5068 7973  and Optical Phys
-000145a0: 6963 732c 0a20 2020 2020 2020 2036 3028  ics,.        60(
-000145b0: 3329 2c20 3138 3838 e280 9331 3839 382e  3), 1888...1898.
-000145c0: 2068 7474 7073 3a2f 2f64 6f69 2e6f 7267   https://doi.org
-000145d0: 2f31 302e 3131 3033 2f50 6879 7352 6576  /10.1103/PhysRev
-000145e0: 412e 3630 2e31 3838 380a 0a20 2020 202e  A.60.1888..    .
-000145f0: 2e20 5b4e 6965 3032 5d0a 2020 2020 2020  . [Nie02].      
-00014600: 2020 4e69 656c 7365 6e2c 204d 2e20 412e    Nielsen, M. A.
-00014610: 2028 3230 3032 292e 2041 2073 696d 706c   (2002). A simpl
-00014620: 6520 666f 726d 756c 6120 666f 7220 7468  e formula for th
-00014630: 6520 6176 6572 6167 6520 6761 7465 0a20  e average gate. 
-00014640: 2020 2020 2020 2066 6964 656c 6974 7920         fidelity 
-00014650: 6f66 2061 2071 7561 6e74 756d 2064 796e  of a quantum dyn
-00014660: 616d 6963 616c 206f 7065 7261 7469 6f6e  amical operation
-00014670: 2e20 5068 7973 6963 7320 4c65 7474 6572  . Physics Letter
-00014680: 732c 0a20 2020 2020 2020 2053 6563 7469  s,.        Secti
-00014690: 6f6e 2041 3a20 4765 6e65 7261 6c2c 2041  on A: General, A
-000146a0: 746f 6d69 6320 616e 6420 536f 6c69 6420  tomic and Solid 
-000146b0: 5374 6174 6520 5068 7973 6963 732c 2033  State Physics, 3
-000146c0: 3033 2834 292c 0a20 2020 2020 2020 2032  03(4),.        2
-000146d0: 3439 e280 9332 3532 2e20 6874 7470 733a  49...252. https:
-000146e0: 2f2f 646f 692e 6f72 672f 3130 2e31 3031  //doi.org/10.101
-000146f0: 362f 5330 3337 352d 3936 3031 2830 3229  6/S0375-9601(02)
-00014700: 3031 3237 322d 300a 2020 2020 2222 220a  01272-0.    """.
-00014710: 2020 2020 2320 4e6f 6973 6520 6f70 6572      # Noise oper
-00014720: 6174 6f72 2069 6e64 6963 6573 0a20 2020  ator indices.   
-00014730: 2069 6478 203d 2075 7469 6c2e 6765 745f   idx = util.get_
-00014740: 696e 6469 6365 735f 6672 6f6d 5f69 6465  indices_from_ide
-00014750: 6e74 6966 6965 7273 2870 756c 7365 2e6e  ntifiers(pulse.n
-00014760: 5f6f 7065 725f 6964 656e 7469 6669 6572  _oper_identifier
-00014770: 732c 206e 5f6f 7065 725f 6964 656e 7469  s, n_oper_identi
-00014780: 6669 6572 7329 0a0a 2020 2020 6966 2074  fiers)..    if t
-00014790: 6573 745f 636f 6e76 6572 6765 6e63 653a  est_convergence:
-000147a0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-000147b0: 6361 6c6c 6162 6c65 2873 7065 6374 7275  callable(spectru
-000147c0: 6d29 3a0a 2020 2020 2020 2020 2020 2020  m):.            
-000147d0: 7261 6973 6520 5479 7065 4572 726f 7228  raise TypeError(
-000147e0: 2753 7065 6374 7275 6d20 7368 6f75 6c64  'Spectrum should
-000147f0: 2062 6520 6361 6c6c 6162 6c65 2077 6865   be callable whe
-00014800: 6e20 7465 7374 5f63 6f6e 7665 7267 656e  n test_convergen
-00014810: 6365 203d 3d20 5472 7565 2e27 290a 0a20  ce == True.').. 
-00014820: 2020 2020 2020 2023 2050 6172 7365 2061         # Parse a
-00014830: 7267 756d 656e 7420 6469 6374 0a20 2020  rgument dict.   
-00014840: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-00014850: 2020 2020 2020 6f6d 6567 615f 4952 203d        omega_IR =
-00014860: 206f 6d65 6761 2e67 6574 2827 6f6d 6567   omega.get('omeg
-00014870: 615f 4952 272c 2032 2a6e 702e 7069 2f70  a_IR', 2*np.pi/p
-00014880: 756c 7365 2e74 6175 2a31 652d 3229 0a20  ulse.tau*1e-2). 
-00014890: 2020 2020 2020 2065 7863 6570 7420 4174         except At
-000148a0: 7472 6962 7574 6545 7272 6f72 3a0a 2020  tributeError:.  
-000148b0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-000148c0: 5479 7065 4572 726f 7228 276f 6d65 6761  TypeError('omega
-000148d0: 2073 686f 756c 6420 6265 2064 6963 7469   should be dicti
-000148e0: 6f6e 6172 7920 7769 7468 2070 6172 616d  onary with param
-000148f0: 6574 6572 7320 2720 2b0a 2020 2020 2020  eters ' +.      
-00014900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014910: 2020 2020 2020 2777 6865 6e20 7465 7374        'when test
-00014920: 5f63 6f6e 7665 7267 656e 6365 203d 3d20  _convergence == 
-00014930: 5472 7565 2e27 290a 0a20 2020 2020 2020  True.')..       
-00014940: 206f 6d65 6761 5f55 5620 3d20 6f6d 6567   omega_UV = omeg
-00014950: 612e 6765 7428 276f 6d65 6761 5f55 5627  a.get('omega_UV'
-00014960: 2c20 322a 6e70 2e70 692f 7075 6c73 652e  , 2*np.pi/pulse.
-00014970: 7461 752a 3165 2b32 290a 2020 2020 2020  tau*1e+2).      
-00014980: 2020 7370 6163 696e 6720 3d20 6f6d 6567    spacing = omeg
-00014990: 612e 6765 7428 2773 7061 6369 6e67 272c  a.get('spacing',
-000149a0: 2027 6c69 6e65 6172 2729 0a20 2020 2020   'linear').     
-000149b0: 2020 206e 5f6d 696e 203d 206f 6d65 6761     n_min = omega
-000149c0: 2e67 6574 2827 6e5f 6d69 6e27 2c20 3130  .get('n_min', 10
-000149d0: 3029 0a20 2020 2020 2020 206e 5f6d 6178  0).        n_max
-000149e0: 203d 206f 6d65 6761 2e67 6574 2827 6e5f   = omega.get('n_
-000149f0: 6d61 7827 2c20 3530 3029 0a20 2020 2020  max', 500).     
-00014a00: 2020 206e 5f70 6f69 6e74 7320 3d20 6f6d     n_points = om
-00014a10: 6567 612e 6765 7428 276e 5f70 6f69 6e74  ega.get('n_point
-00014a20: 7327 2c20 3130 290a 0a20 2020 2020 2020  s', 10)..       
-00014a30: 2023 2041 6c69 6173 206e 756d 7079 2773   # Alias numpy's
-00014a40: 206c 696e 7370 6163 6520 6f72 206c 6f67   linspace or log
-00014a50: 7370 6163 6520 6d65 7468 6f64 2064 6570  space method dep
-00014a60: 656e 6469 6e67 206f 6e20 7468 6520 7370  ending on the sp
-00014a70: 6163 696e 670a 2020 2020 2020 2020 2320  acing.        # 
-00014a80: 6f6d 6567 6120 6861 730a 2020 2020 2020  omega has.      
-00014a90: 2020 6966 2073 7061 6369 6e67 203d 3d20    if spacing == 
-00014aa0: 276c 696e 6561 7227 3a0a 2020 2020 2020  'linear':.      
-00014ab0: 2020 2020 2020 7873 7061 6365 203d 206e        xspace = n
-00014ac0: 702e 6c69 6e73 7061 6365 0a20 2020 2020  p.linspace.     
-00014ad0: 2020 2065 6c69 6620 7370 6163 696e 6720     elif spacing 
-00014ae0: 3d3d 2027 6c6f 6727 3a0a 2020 2020 2020  == 'log':.      
-00014af0: 2020 2020 2020 7873 7061 6365 203d 206e        xspace = n
-00014b00: 702e 6765 6f6d 7370 6163 650a 2020 2020  p.geomspace.    
-00014b10: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00014b20: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-00014b30: 6545 7272 6f72 2822 7370 6163 696e 6720  eError("spacing 
-00014b40: 7368 6f75 6c64 2062 6520 6569 7468 6572  should be either
-00014b50: 2027 6c69 6e65 6172 2720 6f72 2027 6c6f   'linear' or 'lo
-00014b60: 6727 2e22 290a 0a20 2020 2020 2020 2064  g'.")..        d
-00014b70: 656c 7461 5f6e 203d 2028 6e5f 6d61 7820  elta_n = (n_max 
-00014b80: 2d20 6e5f 6d69 6e29 2f2f 286e 5f70 6f69  - n_min)//(n_poi
-00014b90: 6e74 7320 2d20 3129 0a20 2020 2020 2020  nts - 1).       
-00014ba0: 206e 5f73 616d 706c 6573 203d 206e 702e   n_samples = np.
-00014bb0: 6172 616e 6765 286e 5f6d 696e 2c20 6e5f  arange(n_min, n_
-00014bc0: 6d61 7820 2b20 6465 6c74 615f 6e2c 2064  max + delta_n, d
-00014bd0: 656c 7461 5f6e 290a 0a20 2020 2020 2020  elta_n)..       
-00014be0: 2063 6f6e 7665 7267 656e 6365 5f69 6e66   convergence_inf
-00014bf0: 6964 7320 3d20 6e70 2e65 6d70 7479 2828  ids = np.empty((
-00014c00: 6c65 6e28 6e5f 7361 6d70 6c65 7329 2c20  len(n_samples), 
-00014c10: 6c65 6e28 6964 7829 2929 0a20 2020 2020  len(idx))).     
-00014c20: 2020 2066 6f72 2069 2c20 6e20 696e 2065     for i, n in e
-00014c30: 6e75 6d65 7261 7465 286e 5f73 616d 706c  numerate(n_sampl
-00014c40: 6573 293a 0a20 2020 2020 2020 2020 2020  es):.           
-00014c50: 2066 7265 7173 203d 2078 7370 6163 6528   freqs = xspace(
-00014c60: 6f6d 6567 615f 4952 2c20 6f6d 6567 615f  omega_IR, omega_
-00014c70: 5556 2c20 6e29 0a20 2020 2020 2020 2020  UV, n).         
-00014c80: 2020 2063 6f6e 7665 7267 656e 6365 5f69     convergence_i
-00014c90: 6e66 6964 735b 695d 203d 2069 6e66 6964  nfids[i] = infid
-00014ca0: 656c 6974 7928 7075 6c73 652c 2073 7065  elity(pulse, spe
-00014cb0: 6374 7275 6d28 6672 6571 7329 2c20 6672  ctrum(freqs), fr
-00014cc0: 6571 732c 0a20 2020 2020 2020 2020 2020  eqs,.           
-00014cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014cf0: 2020 2020 6e5f 6f70 6572 5f69 6465 6e74      n_oper_ident
-00014d00: 6966 6965 7273 3d6e 5f6f 7065 725f 6964  ifiers=n_oper_id
-00014d10: 656e 7469 6669 6572 732c 0a20 2020 2020  entifiers,.     
-00014d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014d40: 2020 2020 2020 2020 2020 7768 6963 683d            which=
-00014d50: 2774 6f74 616c 272c 2073 686f 775f 7072  'total', show_pr
-00014d60: 6f67 7265 7373 6261 723d 7368 6f77 5f70  ogressbar=show_p
-00014d70: 726f 6772 6573 7362 6172 2c0a 2020 2020  rogressbar,.    
-00014d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014da0: 2020 2020 2020 2020 2020 2063 6163 6865             cache
-00014db0: 5f69 6e74 6572 6d65 6469 6174 6573 3d46  _intermediates=F
-00014dc0: 616c 7365 2c20 7265 7475 726e 5f73 6d61  alse, return_sma
-00014dd0: 6c6c 6e65 7373 3d46 616c 7365 2c0a 2020  llness=False,.  
-00014de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014e00: 2020 2020 2020 2020 2020 2020 2074 6573               tes
-00014e10: 745f 636f 6e76 6572 6765 6e63 653d 4661  t_convergence=Fa
-00014e20: 6c73 6529 0a0a 2020 2020 2020 2020 7265  lse)..        re
-00014e30: 7475 726e 206e 5f73 616d 706c 6573 2c20  turn n_samples, 
-00014e40: 636f 6e76 6572 6765 6e63 655f 696e 6669  convergence_infi
-00014e50: 6473 0a0a 2020 2020 6966 2077 6869 6368  ds..    if which
-00014e60: 203d 3d20 2774 6f74 616c 273a 0a20 2020   == 'total':.   
-00014e70: 2020 2020 2069 6620 6e6f 7420 7075 6c73       if not puls
-00014e80: 652e 6261 7369 732e 6973 7472 6163 656c  e.basis.istracel
-00014e90: 6573 733a 0a20 2020 2020 2020 2020 2020  ess:.           
-00014ea0: 2023 2046 6964 656c 6974 7920 6e6f 7420   # Fidelity not 
-00014eb0: 7369 6d70 6c79 2073 756d 206f 6620 6469  simply sum of di
-00014ec0: 6167 6f6e 616c 206f 6620 6465 6361 7920  agonal of decay 
-00014ed0: 616d 706c 6974 7564 6573 2047 616d 6d61  amplitudes Gamma
-00014ee0: 5f6b 6b0a 2020 2020 2020 2020 2020 2020  _kk.            
-00014ef0: 2320 6275 7420 7472 6163 6520 7465 6e73  # but trace tens
-00014f00: 6f72 2070 6c61 7973 2061 2072 6f6c 652c  or plays a role,
-00014f10: 2063 6620 6571 2e20 2833 3929 2e20 466f   cf eq. (39). Fo
-00014f20: 7220 7472 6163 656c 6573 7320 6261 7365  r traceless base
-00014f30: 732c 0a20 2020 2020 2020 2020 2020 2023  s,.            #
-00014f40: 2074 6865 2074 7261 6365 2074 656e 736f   the trace tenso
-00014f50: 7220 7465 726d 2072 6564 7563 6573 2074  r term reduces t
-00014f60: 6f20 6465 6c74 615f 696a 2e0a 2020 2020  o delta_ij..    
-00014f70: 2020 2020 2020 2020 7472 6163 6573 203d          traces =
-00014f80: 2070 756c 7365 2e62 6173 6973 2e66 6f75   pulse.basis.fou
-00014f90: 725f 656c 656d 656e 745f 7472 6163 6573  r_element_traces
-00014fa0: 0a20 2020 2020 2020 2020 2020 2074 7261  .            tra
-00014fb0: 6365 735f 6469 6167 203d 2028 7370 6172  ces_diag = (spar
-00014fc0: 7365 2e64 6961 676f 6e61 6c28 7472 6163  se.diagonal(trac
-00014fd0: 6573 2c20 6178 6973 313d 322c 2061 7869  es, axis1=2, axi
-00014fe0: 7332 3d33 292e 7375 6d28 2d31 2920 2d0a  s2=3).sum(-1) -.
-00014ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015000: 2020 2020 2020 2020 2020 2073 7061 7273             spars
-00015010: 652e 6469 6167 6f6e 616c 2874 7261 6365  e.diagonal(trace
-00015020: 732c 2061 7869 7331 3d31 2c20 6178 6973  s, axis1=1, axis
-00015030: 323d 3329 2e73 756d 282d 3129 292e 746f  2=3).sum(-1)).to
-00015040: 6465 6e73 6528 290a 0a20 2020 2020 2020  dense()..       
-00015050: 2020 2020 2063 6f6e 7472 6f6c 5f6d 6174       control_mat
-00015060: 7269 7820 3d20 7075 6c73 652e 6765 745f  rix = pulse.get_
-00015070: 636f 6e74 726f 6c5f 6d61 7472 6978 286f  control_matrix(o
-00015080: 6d65 6761 2c20 7368 6f77 5f70 726f 6772  mega, show_progr
-00015090: 6573 7362 6172 2c20 6361 6368 655f 696e  essbar, cache_in
-000150a0: 7465 726d 6564 6961 7465 7329 0a20 2020  termediates).   
-000150b0: 2020 2020 2020 2020 2066 696c 7465 725f           filter_
-000150c0: 6675 6e63 7469 6f6e 203d 206e 702e 6569  function = np.ei
-000150d0: 6e73 756d 2827 616b 6f2c 626c 6f2c 6b6c  nsum('ako,blo,kl
-000150e0: 2d3e 6162 6f27 2c0a 2020 2020 2020 2020  ->abo',.        
-000150f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015110: 636f 6e74 726f 6c5f 6d61 7472 6978 2e63  control_matrix.c
-00015120: 6f6e 6a28 292c 2063 6f6e 7472 6f6c 5f6d  onj(), control_m
-00015130: 6174 7269 782c 2074 7261 6365 735f 6469  atrix, traces_di
-00015140: 6167 292f 7075 6c73 652e 640a 2020 2020  ag)/pulse.d.    
-00015150: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00015160: 2020 2020 2020 6669 6c74 6572 5f66 756e        filter_fun
-00015170: 6374 696f 6e20 3d20 7075 6c73 652e 6765  ction = pulse.ge
-00015180: 745f 6669 6c74 6572 5f66 756e 6374 696f  t_filter_functio
-00015190: 6e28 6f6d 6567 612c 2077 6869 6368 3d27  n(omega, which='
-000151a0: 6669 6465 6c69 7479 272c 0a20 2020 2020  fidelity',.     
-000151b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000151c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000151d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000151e0: 2020 2073 686f 775f 7072 6f67 7265 7373     show_progress
-000151f0: 6261 723d 7368 6f77 5f70 726f 6772 6573  bar=show_progres
-00015200: 7362 6172 2c0a 2020 2020 2020 2020 2020  sbar,.          
-00015210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015230: 2020 2020 2020 2020 2020 2020 2020 6361                ca
-00015240: 6368 655f 696e 7465 726d 6564 6961 7465  che_intermediate
-00015250: 733d 6361 6368 655f 696e 7465 726d 6564  s=cache_intermed
-00015260: 6961 7465 7329 0a20 2020 2065 6c73 653a  iates).    else:
-00015270: 0a20 2020 2020 2020 2023 2077 6869 6368  .        # which
-00015280: 203d 3d20 2763 6f72 7265 6c61 7469 6f6e   == 'correlation
-00015290: 7327 0a20 2020 2020 2020 2069 6620 6e6f  s'.        if no
-000152a0: 7420 7075 6c73 652e 6261 7369 732e 6973  t pulse.basis.is
-000152b0: 7472 6163 656c 6573 733a 0a20 2020 2020  traceless:.     
-000152c0: 2020 2020 2020 2077 6172 6e28 2743 616c         warn('Cal
-000152d0: 6375 6c61 7469 6e67 2070 756c 7365 2063  culating pulse c
-000152e0: 6f72 7265 6c61 7469 6f6e 2066 6964 656c  orrelation fidel
-000152f0: 6974 6965 7320 7769 7468 206e 6f6e 2d27  ities with non-'
-00015300: 202b 0a20 2020 2020 2020 2020 2020 2020   +.             
-00015310: 2020 2020 2774 7261 6365 6c65 7373 2062      'traceless b
-00015320: 6173 6973 2e20 5468 6520 7265 7375 6c74  asis. The result
-00015330: 7320 7769 6c6c 2062 6520 6f66 662e 2729  s will be off.')
-00015340: 0a0a 2020 2020 2020 2020 6966 2070 756c  ..        if pul
-00015350: 7365 2e69 735f 6361 6368 6564 2827 6f6d  se.is_cached('om
-00015360: 6567 6127 293a 0a20 2020 2020 2020 2020  ega'):.         
-00015370: 2020 2069 6620 6e6f 7420 6e70 2e61 7272     if not np.arr
-00015380: 6179 5f65 7175 616c 2870 756c 7365 2e6f  ay_equal(pulse.o
-00015390: 6d65 6761 2c20 6f6d 6567 6129 3a0a 2020  mega, omega):.  
-000153a0: 2020 2020 2020 2020 2020 2020 2020 7261                ra
-000153b0: 6973 6520 5661 6c75 6545 7272 6f72 2827  ise ValueError('
-000153c0: 5075 6c73 6520 636f 7272 656c 6174 696f  Pulse correlatio
-000153d0: 6e20 696e 6669 6465 6c69 7469 6573 2072  n infidelities r
-000153e0: 6571 7565 7374 6564 2027 202b 0a20 2020  equested ' +.   
-000153f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015400: 2020 2020 2020 2020 2020 2020 2020 2762                'b
-00015410: 7574 206f 6d65 6761 206e 6f74 2065 7175  ut omega not equ
-00015420: 616c 2074 6f20 6361 6368 6564 2066 7265  al to cached fre
-00015430: 7175 656e 6369 6573 2e27 290a 0a20 2020  quencies.')..   
-00015440: 2020 2020 2066 696c 7465 725f 6675 6e63       filter_func
-00015450: 7469 6f6e 203d 2070 756c 7365 2e67 6574  tion = pulse.get
-00015460: 5f70 756c 7365 5f63 6f72 7265 6c61 7469  _pulse_correlati
-00015470: 6f6e 5f66 696c 7465 725f 6675 6e63 7469  on_filter_functi
-00015480: 6f6e 2829 0a0a 2020 2020 696e 7465 6772  on()..    integr
-00015490: 616e 6420 3d20 5f67 6574 5f69 6e74 6567  and = _get_integ
-000154a0: 7261 6e64 2873 7065 6374 7275 6d2c 206f  rand(spectrum, o
-000154b0: 6d65 6761 2c20 6964 782c 2077 6869 6368  mega, idx, which
-000154c0: 2c20 2766 6964 656c 6974 7927 2c0a 2020  , 'fidelity',.  
-000154d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000154e0: 2020 2020 2020 2020 2020 2020 2066 696c               fil
-000154f0: 7465 725f 6675 6e63 7469 6f6e 3d66 696c  ter_function=fil
-00015500: 7465 725f 6675 6e63 7469 6f6e 290a 2020  ter_function).  
-00015510: 2020 696e 6669 6420 3d20 7574 696c 2e69    infid = util.i
-00015520: 6e74 6567 7261 7465 2869 6e74 6567 7261  ntegrate(integra
-00015530: 6e64 2c20 6f6d 6567 6129 2f28 322a 6e70  nd, omega)/(2*np
-00015540: 2e70 692a 7075 6c73 652e 6429 0a0a 2020  .pi*pulse.d)..  
-00015550: 2020 6966 2072 6574 7572 6e5f 736d 616c    if return_smal
-00015560: 6c6e 6573 733a 0a20 2020 2020 2020 2069  lness:.        i
-00015570: 6620 7370 6563 7472 756d 2e6e 6469 6d20  f spectrum.ndim 
-00015580: 3e20 323a 0a20 2020 2020 2020 2020 2020  > 2:.           
-00015590: 2072 6169 7365 204e 6f74 496d 706c 656d   raise NotImplem
-000155a0: 656e 7465 6445 7272 6f72 2827 536d 616c  entedError('Smal
-000155b0: 6c6e 6573 7320 7061 7261 6d65 7465 7220  lness parameter 
-000155c0: 6f6e 6c79 2069 6d70 6c65 6d65 6e74 6564  only implemented
-000155d0: 2027 202b 0a20 2020 2020 2020 2020 2020   ' +.           
-000155e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000155f0: 2020 2020 2020 2020 2020 2027 666f 7220             'for 
-00015600: 756e 636f 7272 656c 6174 6564 206e 6f69  uncorrelated noi
-00015610: 7365 2073 6f75 7263 6573 2729 0a0a 2020  se sources')..  
-00015620: 2020 2020 2020 5431 203d 2075 7469 6c2e        T1 = util.
-00015630: 696e 7465 6772 6174 6528 7370 6563 7472  integrate(spectr
-00015640: 756d 2c20 6f6d 6567 6129 2f28 322a 6e70  um, omega)/(2*np
-00015650: 2e70 6929 0a20 2020 2020 2020 2054 3220  .pi).        T2 
-00015660: 3d20 2870 756c 7365 2e64 742a 7075 6c73  = (pulse.dt*puls
-00015670: 652e 6e5f 636f 6566 6673 5b69 6478 5d29  e.n_coeffs[idx])
-00015680: 2e73 756d 2861 7869 733d 2d31 292a 2a32  .sum(axis=-1)**2
-00015690: 0a20 2020 2020 2020 2054 3320 3d20 7574  .        T3 = ut
-000156a0: 696c 2e61 6273 3228 7075 6c73 652e 6e5f  il.abs2(pulse.n_
-000156b0: 6f70 6572 735b 6964 785d 292e 7375 6d28  opers[idx]).sum(
-000156c0: 6178 6973 3d28 312c 2032 2929 0a20 2020  axis=(1, 2)).   
-000156d0: 2020 2020 2078 6920 3d20 6e70 2e73 7172       xi = np.sqr
-000156e0: 7428 2854 312a 5432 2a54 3329 2e73 756d  t((T1*T2*T3).sum
-000156f0: 2829 290a 0a20 2020 2020 2020 2072 6574  ())..        ret
-00015700: 7572 6e20 696e 6669 642c 2078 690a 0a20  urn infid, xi.. 
-00015710: 2020 2072 6574 7572 6e20 696e 6669 640a     return infid.
+000125e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000125f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012600: 2020 2020 2020 2063 6163 6865 5f69 6e74         cache_int
+00012610: 6572 6d65 6469 6174 6573 3d63 6163 6865  ermediates=cache
+00012620: 5f69 6e74 6572 6d65 6469 6174 6573 290a  _intermediates).
+00012630: 0a20 2020 2074 7279 3a0a 2020 2020 2020  .    try:.      
+00012640: 2020 2320 6167 6e6f 7374 6963 206f 6620    # agnostic of 
+00012650: 7468 6520 7370 6563 6966 6963 2073 6861  the specific sha
+00012660: 7065 206f 6620 6375 6d75 6c61 6e74 5f66  pe of cumulant_f
+00012670: 756e 6374 696f 6e2c 206a 7573 7420 7375  unction, just su
+00012680: 6d20 6f76 6572 2065 7665 7279 7468 696e  m over everythin
+00012690: 6720 6578 6365 7074 2066 6f72 0a20 2020  g except for.   
+000126a0: 2020 2020 2023 2074 6865 2062 6173 6973       # the basis
+000126b0: 2065 6c65 6d65 6e74 7320 7468 6174 2073   elements that s
+000126c0: 6974 206f 6e20 7468 6520 6c61 7374 2074  it on the last t
+000126d0: 776f 2061 7865 730a 2020 2020 2020 2020  wo axes.        
+000126e0: 6572 726f 725f 7472 616e 7366 6572 5f6d  error_transfer_m
+000126f0: 6174 7269 7820 3d20 736c 612e 6578 706d  atrix = sla.expm
+00012700: 280a 2020 2020 2020 2020 2020 2020 6375  (.            cu
+00012710: 6d75 6c61 6e74 5f66 756e 6374 696f 6e2e  mulant_function.
+00012720: 7375 6d28 6178 6973 3d74 7570 6c65 2872  sum(axis=tuple(r
+00012730: 616e 6765 2863 756d 756c 616e 745f 6675  ange(cumulant_fu
+00012740: 6e63 7469 6f6e 2e6e 6469 6d20 2d20 3229  nction.ndim - 2)
+00012750: 2929 0a20 2020 2020 2020 2029 0a20 2020  )).        ).   
+00012760: 2065 7863 6570 7420 4174 7472 6962 7574   except Attribut
+00012770: 6545 7272 6f72 2061 7320 6165 7272 3a0a  eError as aerr:.
+00012780: 2020 2020 2020 2020 7261 6973 6520 5479          raise Ty
+00012790: 7065 4572 726f 7228 6627 6375 6d75 6c61  peError(f'cumula
+000127a0: 6e74 5f66 756e 6374 696f 6e20 696e 7661  nt_function inva
+000127b0: 6c69 6420 7479 7065 3a20 7b74 7970 6528  lid type: {type(
+000127c0: 6375 6d75 6c61 6e74 5f66 756e 6374 696f  cumulant_functio
+000127d0: 6e29 7d27 2920 6672 6f6d 2061 6572 720a  n)}') from aerr.
+000127e0: 2020 2020 6578 6365 7074 2056 616c 7565      except Value
+000127f0: 4572 726f 7220 6173 2076 6572 723a 0a20  Error as verr:. 
+00012800: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+00012810: 7565 4572 726f 7228 6627 6375 6d75 6c61  ueError(f'cumula
+00012820: 6e74 5f66 756e 6374 696f 6e20 696e 7661  nt_function inva
+00012830: 6c69 6420 7368 6170 653a 207b 6375 6d75  lid shape: {cumu
+00012840: 6c61 6e74 5f66 756e 6374 696f 6e2e 7368  lant_function.sh
+00012850: 6170 657d 2729 2066 726f 6d20 7665 7272  ape}') from verr
+00012860: 0a0a 2020 2020 7265 7475 726e 2065 7272  ..    return err
+00012870: 6f72 5f74 7261 6e73 6665 725f 6d61 7472  or_transfer_matr
+00012880: 6978 0a0a 0a40 7574 696c 2e70 6172 7365  ix...@util.parse
+00012890: 5f6f 7074 696f 6e61 6c5f 7061 7261 6d65  _optional_parame
+000128a0: 7465 7273 2877 6869 6368 3d28 2774 6f74  ters(which=('tot
+000128b0: 616c 272c 2027 636f 7272 656c 6174 696f  al', 'correlatio
+000128c0: 6e73 2729 290a 6465 6620 696e 6669 6465  ns')).def infide
+000128d0: 6c69 7479 280a 2020 2020 2020 2020 7075  lity(.        pu
+000128e0: 6c73 653a 2027 5075 6c73 6553 6571 7565  lse: 'PulseSeque
+000128f0: 6e63 6527 2c0a 2020 2020 2020 2020 7370  nce',.        sp
+00012900: 6563 7472 756d 3a20 556e 696f 6e5b 436f  ectrum: Union[Co
+00012910: 6566 6669 6369 656e 7473 2c20 4361 6c6c  efficients, Call
+00012920: 6162 6c65 5d2c 0a20 2020 2020 2020 206f  able],.        o
+00012930: 6d65 6761 3a20 556e 696f 6e5b 436f 6566  mega: Union[Coef
+00012940: 6669 6369 656e 7473 2c20 4469 6374 5b73  ficients, Dict[s
+00012950: 7472 2c20 556e 696f 6e5b 696e 742c 2073  tr, Union[int, s
+00012960: 7472 5d5d 5d2c 0a20 2020 2020 2020 206e  tr]]],.        n
+00012970: 5f6f 7065 725f 6964 656e 7469 6669 6572  _oper_identifier
+00012980: 733a 204f 7074 696f 6e61 6c5b 5365 7175  s: Optional[Sequ
+00012990: 656e 6365 5b73 7472 5d5d 203d 204e 6f6e  ence[str]] = Non
+000129a0: 652c 0a20 2020 2020 2020 2077 6869 6368  e,.        which
+000129b0: 3a20 7374 7220 3d20 2774 6f74 616c 272c  : str = 'total',
+000129c0: 0a20 2020 2020 2020 2073 686f 775f 7072  .        show_pr
+000129d0: 6f67 7265 7373 6261 723a 2062 6f6f 6c20  ogressbar: bool 
+000129e0: 3d20 4661 6c73 652c 0a20 2020 2020 2020  = False,.       
+000129f0: 2063 6163 6865 5f69 6e74 6572 6d65 6469   cache_intermedi
+00012a00: 6174 6573 3a20 626f 6f6c 203d 2046 616c  ates: bool = Fal
+00012a10: 7365 2c0a 2020 2020 2020 2020 7265 7475  se,.        retu
+00012a20: 726e 5f73 6d61 6c6c 6e65 7373 3a20 626f  rn_smallness: bo
+00012a30: 6f6c 203d 2046 616c 7365 2c0a 2020 2020  ol = False,.    
+00012a40: 2020 2020 7465 7374 5f63 6f6e 7665 7267      test_converg
+00012a50: 656e 6365 3a20 626f 6f6c 203d 2046 616c  ence: bool = Fal
+00012a60: 7365 0a29 202d 3e20 556e 696f 6e5b 6e64  se.) -> Union[nd
+00012a70: 6172 7261 792c 2041 6e79 5d3a 0a20 2020  array, Any]:.   
+00012a80: 2072 2222 2243 616c 6375 6c61 7465 2074   r"""Calculate t
+00012a90: 6865 206c 6561 6469 6e67 206f 7264 6572  he leading order
+00012aa0: 2065 6e74 616e 676c 656d 656e 7420 696e   entanglement in
+00012ab0: 6669 6465 6c69 7479 2e0a 0a20 2020 2054  fidelity...    T
+00012ac0: 6869 7320 6675 6e63 7469 6f6e 2063 616c  his function cal
+00012ad0: 6375 6c61 7465 7320 7468 6520 696e 6669  culates the infi
+00012ae0: 6465 6c69 7479 2061 7070 726f 7869 6d61  delity approxima
+00012af0: 7465 6c79 2066 726f 6d20 7468 650a 2020  tely from the.  
+00012b00: 2020 6c65 6164 696e 6720 7065 7475 7262    leading peturb
+00012b10: 6174 696f 6e20 2873 6565 203a 7265 663a  ation (see :ref:
+00012b20: 604e 6f74 6573 203c 6e6f 7465 733e 6029  `Notes <notes>`)
+00012b30: 2e20 546f 2063 6f6d 7075 7465 2069 740a  . To compute it.
+00012b40: 2020 2020 6578 6163 746c 7920 666f 7220      exactly for 
+00012b50: 4761 7573 7369 616e 206e 6f69 7365 2061  Gaussian noise a
+00012b60: 6e64 2076 616e 6973 6869 6e67 2063 6f68  nd vanishing coh
+00012b70: 6572 656e 7420 6572 726f 7273 2028 7365  erent errors (se
+00012b80: 636f 6e64 0a20 2020 206f 7264 6572 204d  cond.    order M
+00012b90: 6167 6e75 7320 7465 726d 7329 2c20 7573  agnus terms), us
+00012ba0: 6520 3a66 756e 633a 6065 7272 6f72 5f74  e :func:`error_t
+00012bb0: 7261 6e73 6665 725f 6d61 7472 6978 6020  ransfer_matrix` 
+00012bc0: 746f 206f 6274 6169 6e20 6974 0a20 2020  to obtain it.   
+00012bd0: 2066 726f 6d20 7468 6520 6675 6c6c 2070   from the full p
+00012be0: 726f 6365 7373 206d 6174 7269 782e 0a0a  rocess matrix...
+00012bf0: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+00012c00: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+00012c10: 2020 7075 6c73 653a 2050 756c 7365 5365    pulse: PulseSe
+00012c20: 7175 656e 6365 0a20 2020 2020 2020 2054  quence.        T
+00012c30: 6865 2060 6050 756c 7365 5365 7175 656e  he ``PulseSequen
+00012c40: 6365 6060 2069 6e73 7461 6e63 6520 666f  ce`` instance fo
+00012c50: 7220 7768 6963 6820 746f 2063 616c 6375  r which to calcu
+00012c60: 6c61 7465 2074 6865 0a20 2020 2020 2020  late the.       
+00012c70: 2069 6e66 6964 656c 6974 7920 666f 722e   infidelity for.
+00012c80: 0a20 2020 2073 7065 6374 7275 6d3a 2061  .    spectrum: a
+00012c90: 7272 6179 5f6c 696b 652c 2073 6861 7065  rray_like, shape
+00012ca0: 2028 5b5b 6e5f 6e6f 7073 2c5d 206e 5f6e   ([[n_nops,] n_n
+00012cb0: 6f70 732c 5d20 6f6d 6567 6129 206f 7220  ops,] omega) or 
+00012cc0: 6361 6c6c 6162 6c65 0a20 2020 2020 2020  callable.       
+00012cd0: 2054 6865 2074 776f 2d73 6964 6564 206e   The two-sided n
+00012ce0: 6f69 7365 2070 6f77 6572 2073 7065 6374  oise power spect
+00012cf0: 7261 6c20 6465 6e73 6974 7920 696e 2075  ral density in u
+00012d00: 6e69 7473 206f 6620 696e 7665 7273 650a  nits of inverse.
+00012d10: 2020 2020 2020 2020 6672 6571 7565 6e63          frequenc
+00012d20: 6965 7320 6173 2061 6e20 6172 7261 7920  ies as an array 
+00012d30: 6f66 2073 6861 7065 2028 6e5f 6f6d 6567  of shape (n_omeg
+00012d40: 612c 292c 2028 6e5f 6e6f 7073 2c20 6e5f  a,), (n_nops, n_
+00012d50: 6f6d 6567 6129 2c0a 2020 2020 2020 2020  omega),.        
+00012d60: 6f72 2028 6e5f 6e6f 7073 2c20 6e5f 6e6f  or (n_nops, n_no
+00012d70: 7073 2c20 6e5f 6f6d 6567 6129 2e20 496e  ps, n_omega). In
+00012d80: 2074 6865 2066 6972 7374 2063 6173 652c   the first case,
+00012d90: 2074 6865 2073 616d 650a 2020 2020 2020   the same.      
+00012da0: 2020 7370 6563 7472 756d 2069 7320 7461    spectrum is ta
+00012db0: 6b65 6e20 666f 7220 616c 6c20 6e6f 6973  ken for all nois
+00012dc0: 6520 6f70 6572 6174 6f72 732c 2069 6e20  e operators, in 
+00012dd0: 7468 6520 7365 636f 6e64 2c20 6974 2069  the second, it i
+00012de0: 730a 2020 2020 2020 2020 6173 7375 6d65  s.        assume
+00012df0: 6420 7468 6174 2074 6865 7265 2061 7265  d that there are
+00012e00: 206e 6f20 636f 7272 656c 6174 696f 6e73   no correlations
+00012e10: 2062 6574 7765 656e 2064 6966 6665 7265   between differe
+00012e20: 6e74 206e 6f69 7365 0a20 2020 2020 2020  nt noise.       
+00012e30: 2073 6f75 7263 6573 2061 6e64 2074 6875   sources and thu
+00012e40: 7320 7468 6572 6520 6973 206f 6e65 2073  s there is one s
+00012e50: 7065 6374 7275 6d20 666f 7220 6561 6368  pectrum for each
+00012e60: 206e 6f69 7365 206f 7065 7261 746f 722e   noise operator.
+00012e70: 0a20 2020 2020 2020 2049 6e20 7468 6520  .        In the 
+00012e80: 7468 6972 6420 616e 6420 6d6f 7374 2067  third and most g
+00012e90: 656e 6572 616c 2063 6173 652c 2074 6865  eneral case, the
+00012ea0: 7265 206d 6179 2062 6520 6120 7370 6563  re may be a spec
+00012eb0: 7472 756d 2066 6f72 0a20 2020 2020 2020  trum for.       
+00012ec0: 2065 6163 6820 7061 6972 206f 6620 6e6f   each pair of no
+00012ed0: 6973 6520 6f70 6572 6174 6f72 7320 636f  ise operators co
+00012ee0: 7272 6573 706f 6e64 696e 6720 746f 2074  rresponding to t
+00012ef0: 6865 2063 6f72 7265 6c61 7469 6f6e 730a  he correlations.
+00012f00: 2020 2020 2020 2020 6265 7477 6565 6e20          between 
+00012f10: 7468 656d 2e20 6e5f 6e6f 7073 2069 7320  them. n_nops is 
+00012f20: 7468 6520 6e75 6d62 6572 206f 6620 6e6f  the number of no
+00012f30: 6973 6520 6f70 6572 6174 6f72 7320 636f  ise operators co
+00012f40: 6e73 6964 6572 6564 0a20 2020 2020 2020  nsidered.       
+00012f50: 2061 6e64 2073 686f 756c 6420 6265 2065   and should be e
+00012f60: 7175 616c 2074 6f20 6060 6c65 6e28 6e5f  qual to ``len(n_
+00012f70: 6f70 6572 5f69 6465 6e74 6966 6965 7273  oper_identifiers
+00012f80: 2960 602e 0a0a 2020 2020 2020 2020 4966  )``...        If
+00012f90: 202a 7465 7374 5f63 6f6e 7665 7267 656e   *test_convergen
+00012fa0: 6365 2a20 6973 2060 6054 7275 6560 602c  ce* is ``True``,
+00012fb0: 2061 2066 756e 6374 696f 6e20 6861 6e64   a function hand
+00012fc0: 6c65 2074 6f0a 2020 2020 2020 2020 636f  le to.        co
+00012fd0: 6d70 7574 6520 7468 6520 706f 7765 7220  mpute the power 
+00012fe0: 7370 6563 7472 616c 2064 656e 7369 7479  spectral density
+00012ff0: 2066 726f 6d20 6120 7365 7175 656e 6365   from a sequence
+00013000: 206f 660a 2020 2020 2020 2020 6672 6571   of.        freq
+00013010: 7565 6e63 6965 7320 6973 2065 7870 6563  uencies is expec
+00013020: 7465 642e 0a20 2020 206f 6d65 6761 3a20  ted..    omega: 
+00013030: 6172 7261 795f 6c69 6b65 206f 7220 6469  array_like or di
+00013040: 6374 0a20 2020 2020 2020 2054 6865 2066  ct.        The f
+00013050: 7265 7175 656e 6369 6573 2061 7420 7768  requencies at wh
+00013060: 6963 6820 7468 6520 696e 7465 6772 6174  ich the integrat
+00013070: 696f 6e20 6973 2074 6f20 6265 2063 6172  ion is to be car
+00013080: 7269 6564 206f 7574 2e0a 2020 2020 2020  ried out..      
+00013090: 2020 4966 202a 7465 7374 5f63 6f6e 7665    If *test_conve
+000130a0: 7267 656e 6365 2a20 6973 2060 6054 7275  rgence* is ``Tru
+000130b0: 6560 602c 2061 2064 6963 7420 7769 7468  e``, a dict with
+000130c0: 2070 6f73 7369 626c 6520 6b65 7973 0a20   possible keys. 
+000130d0: 2020 2020 2020 2028 276f 6d65 6761 5f49         ('omega_I
+000130e0: 5227 2c20 276f 6d65 6761 5f55 5627 2c20  R', 'omega_UV', 
+000130f0: 2773 7061 6369 6e67 272c 2027 6e5f 6d69  'spacing', 'n_mi
+00013100: 6e27 2c20 276e 5f6d 6178 272c 0a20 2020  n', 'n_max',.   
+00013110: 2020 2020 2027 6e5f 706f 696e 7473 2729       'n_points')
+00013120: 2c20 7768 6572 6520 616c 6c20 656e 7472  , where all entr
+00013130: 6965 7320 6172 6520 696e 7465 6765 7273  ies are integers
+00013140: 2065 7863 6570 7420 666f 720a 2020 2020   except for.    
+00013150: 2020 2020 6060 7370 6163 696e 6760 6020      ``spacing`` 
+00013160: 7768 6963 6820 7368 6f75 6c64 2062 6520  which should be 
+00013170: 6120 7374 7269 6e67 2c20 6569 7468 6572  a string, either
+00013180: 2027 6c69 6e65 6172 2720 6f72 2027 6c6f   'linear' or 'lo
+00013190: 6727 2e0a 2020 2020 2020 2020 276e 5f70  g'..        'n_p
+000131a0: 6f69 6e74 7327 2063 6f6e 7472 6f6c 7320  oints' controls 
+000131b0: 686f 7720 6d61 6e79 2073 7465 7073 2061  how many steps a
+000131c0: 7265 2074 616b 656e 2e0a 2020 2020 6e5f  re taken..    n_
+000131d0: 6f70 6572 5f69 6465 6e74 6966 6965 7273  oper_identifiers
+000131e0: 3a20 6172 7261 795f 6c69 6b65 2c20 6f70  : array_like, op
+000131f0: 7469 6f6e 616c 0a20 2020 2020 2020 2054  tional.        T
+00013200: 6865 2069 6465 6e74 6966 6965 7273 206f  he identifiers o
+00013210: 6620 7468 6520 6e6f 6973 6520 6f70 6572  f the noise oper
+00013220: 6174 6f72 7320 666f 7220 7768 6963 6820  ators for which 
+00013230: 746f 2063 616c 6375 6c61 7465 0a20 2020  to calculate.   
+00013240: 2020 2020 2074 6865 2069 6e66 6964 656c       the infidel
+00013250: 6974 7920 2063 6f6e 7472 6962 7574 696f  ity  contributio
+00013260: 6e2e 2049 6620 6769 7665 6e2c 2074 6865  n. If given, the
+00013270: 2069 6e66 6964 656c 6974 6965 7320 666f   infidelities fo
+00013280: 720a 2020 2020 2020 2020 6561 6368 206e  r.        each n
+00013290: 6f69 7365 206f 7065 7261 746f 7220 7769  oise operator wi
+000132a0: 6c6c 2062 6520 7265 7475 726e 6564 2e20  ll be returned. 
+000132b0: 4f74 6865 7277 6973 652c 2061 6c6c 206e  Otherwise, all n
+000132c0: 6f69 7365 0a20 2020 2020 2020 206f 7065  oise.        ope
+000132d0: 7261 746f 7273 2077 696c 6c20 6265 2074  rators will be t
+000132e0: 616b 656e 2069 6e74 6f20 6163 636f 756e  aken into accoun
+000132f0: 742e 0a20 2020 2077 6869 6368 3a20 7374  t..    which: st
+00013300: 722c 206f 7074 696f 6e61 6c0a 2020 2020  r, optional.    
+00013310: 2020 2020 5768 6963 6820 696e 6669 6465      Which infide
+00013320: 6c69 7469 6573 2073 686f 756c 6420 6265  lities should be
+00013330: 2063 616c 6375 6c61 7465 642c 206d 6179   calculated, may
+00013340: 2062 6520 6569 7468 6572 2027 746f 7461   be either 'tota
+00013350: 6c27 0a20 2020 2020 2020 2028 6465 6661  l'.        (defa
+00013360: 756c 7429 206f 7220 2763 6f72 7265 6c61  ult) or 'correla
+00013370: 7469 6f6e 7327 2e20 496e 2074 6865 2066  tions'. In the f
+00013380: 6f72 6d65 7220 6361 7365 2c20 6f6e 6520  ormer case, one 
+00013390: 7661 6c75 6520 6973 0a20 2020 2020 2020  value is.       
+000133a0: 2072 6574 7572 6e65 6420 666f 7220 6561   returned for ea
+000133b0: 6368 206e 6f69 7365 206f 7065 7261 746f  ch noise operato
+000133c0: 722c 2063 6f72 7265 7370 6f6e 6469 6e67  r, corresponding
+000133d0: 2074 6f20 7468 6520 746f 7461 6c0a 2020   to the total.  
+000133e0: 2020 2020 2020 696e 6669 6465 6c69 7479        infidelity
+000133f0: 206f 6620 7468 6520 7075 6c73 6520 286f   of the pulse (o
+00013400: 7220 7075 6c73 6520 7365 7175 656e 6365  r pulse sequence
+00013410: 292e 2049 6e20 7468 6520 6c61 7474 6572  ). In the latter
+00013420: 2c20 616e 0a20 2020 2020 2020 2061 7272  , an.        arr
+00013430: 6179 206f 6620 696e 6669 6465 6c69 7469  ay of infideliti
+00013440: 6573 2069 7320 7265 7475 726e 6564 2077  es is returned w
+00013450: 6865 7265 2065 6c65 6d65 6e74 2028 692c  here element (i,
+00013460: 6a29 0a20 2020 2020 2020 2063 6f72 7265  j).        corre
+00013470: 7370 6f6e 6473 2074 6f20 7468 6520 696e  sponds to the in
+00013480: 6669 6465 6c69 7479 2063 6f6e 7472 6962  fidelity contrib
+00013490: 7574 696f 6e20 6f66 2074 6865 2063 6f72  ution of the cor
+000134a0: 7265 6c61 7469 6f6e 730a 2020 2020 2020  relations.      
+000134b0: 2020 6265 7477 6565 6e20 7075 6c73 6573    between pulses
+000134c0: 2069 2061 6e64 206a 2028 7365 6520 3a72   i and j (see :r
+000134d0: 6566 3a60 4e6f 7465 7320 3c6e 6f74 6573  ef:`Notes <notes
+000134e0: 3e60 292e 204e 6f74 6520 7468 6174 0a20  >`). Note that. 
+000134f0: 2020 2020 2020 2074 6869 7320 6f70 7469         this opti
+00013500: 6f6e 2069 7320 6f6e 6c79 2061 7661 696c  on is only avail
+00013510: 6162 6c65 2069 6620 7468 6520 7075 6c73  able if the puls
+00013520: 6520 636f 7272 656c 6174 696f 6e20 6669  e correlation fi
+00013530: 6c74 6572 0a20 2020 2020 2020 2066 756e  lter.        fun
+00013540: 6374 696f 6e73 2068 6176 6520 6265 656e  ctions have been
+00013550: 2063 6f6d 7075 7465 6420 6475 7269 6e67   computed during
+00013560: 2063 6f6e 6361 7465 6e61 7469 6f6e 2028   concatenation (
+00013570: 7365 650a 2020 2020 2020 2020 3a66 756e  see.        :fun
+00013580: 633a 6063 616c 6375 6c61 7465 5f70 756c  c:`calculate_pul
+00013590: 7365 5f63 6f72 7265 6c61 7469 6f6e 5f66  se_correlation_f
+000135a0: 696c 7465 725f 6675 6e63 7469 6f6e 6020  ilter_function` 
+000135b0: 616e 640a 2020 2020 2020 2020 3a66 756e  and.        :fun
+000135c0: 633a 607e 6669 6c74 6572 5f66 756e 6374  c:`~filter_funct
+000135d0: 696f 6e73 2e70 756c 7365 5f73 6571 7565  ions.pulse_seque
+000135e0: 6e63 652e 636f 6e63 6174 656e 6174 6560  nce.concatenate`
+000135f0: 292e 0a20 2020 2073 686f 775f 7072 6f67  )..    show_prog
+00013600: 7265 7373 6261 723a 2062 6f6f 6c2c 206f  ressbar: bool, o
+00013610: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
+00013620: 5368 6f77 2061 2070 726f 6772 6573 7362  Show a progressb
+00013630: 6172 2066 6f72 2074 6865 2063 616c 6375  ar for the calcu
+00013640: 6c61 7469 6f6e 206f 6620 7468 6520 636f  lation of the co
+00013650: 6e74 726f 6c20 6d61 7472 6978 2e0a 2020  ntrol matrix..  
+00013660: 2020 6361 6368 655f 696e 7465 726d 6564    cache_intermed
+00013670: 6961 7465 733a 2062 6f6f 6c2c 206f 7074  iates: bool, opt
+00013680: 696f 6e61 6c0a 2020 2020 2020 2020 4b65  ional.        Ke
+00013690: 6570 2061 6e64 2072 6574 7572 6e20 696e  ep and return in
+000136a0: 7465 726d 6564 6961 7465 2074 6572 6d73  termediate terms
+000136b0: 206f 6620 7468 6520 6361 6c63 756c 6174   of the calculat
+000136c0: 696f 6e20 6f66 2074 6865 0a20 2020 2020  ion of the.     
+000136d0: 2020 2063 6f6e 7472 6f6c 206d 6174 7269     control matri
+000136e0: 7820 2869 6620 6974 2069 7320 6e6f 7420  x (if it is not 
+000136f0: 616c 7265 6164 7920 6361 6368 6564 2920  already cached) 
+00013700: 7468 6174 2063 616e 2062 6520 7265 7573  that can be reus
+00013710: 6564 0a20 2020 2020 2020 2066 6f72 2073  ed.        for s
+00013720: 6563 6f6e 6420 6f72 6465 7220 6f72 2067  econd order or g
+00013730: 7261 6469 656e 7473 2e20 5468 6520 6465  radients. The de
+00013740: 6661 756c 7420 6973 2046 616c 7365 2e0a  fault is False..
+00013750: 2020 2020 7265 7475 726e 5f73 6d61 6c6c      return_small
+00013760: 6e65 7373 3a20 626f 6f6c 2c20 6f70 7469  ness: bool, opti
+00013770: 6f6e 616c 0a20 2020 2020 2020 2052 6574  onal.        Ret
+00013780: 7572 6e20 7468 6520 736d 616c 6c6e 6573  urn the smallnes
+00013790: 7320 7061 7261 6d65 7465 7220 3a6d 6174  s parameter :mat
+000137a0: 683a 605c 7869 6020 666f 7220 7468 6520  h:`\xi` for the 
+000137b0: 6769 7665 6e0a 2020 2020 2020 2020 7370  given.        sp
+000137c0: 6563 7472 756d 2e0a 2020 2020 7465 7374  ectrum..    test
+000137d0: 5f63 6f6e 7665 7267 656e 6365 3a20 626f  _convergence: bo
+000137e0: 6f6c 2c20 6f70 7469 6f6e 616c 0a20 2020  ol, optional.   
+000137f0: 2020 2020 2054 6573 7420 7468 6520 636f       Test the co
+00013800: 6e76 6572 6765 6e63 6520 6f66 2074 6865  nvergence of the
+00013810: 2069 6e74 6567 7261 6c20 7769 7468 2072   integral with r
+00013820: 6573 7065 6374 2074 6f20 7468 6520 6e75  espect to the nu
+00013830: 6d62 6572 0a20 2020 2020 2020 206f 6620  mber.        of 
+00013840: 6672 6571 7565 6e63 7920 7361 6d70 6c65  frequency sample
+00013850: 732e 2052 6574 7572 6e73 2074 6865 206e  s. Returns the n
+00013860: 756d 6265 7220 6f66 2066 7265 7175 656e  umber of frequen
+00013870: 6379 2073 616d 706c 6573 0a20 2020 2020  cy samples.     
+00013880: 2020 2061 6e64 2074 6865 2063 6f72 7265     and the corre
+00013890: 7370 6f6e 6469 6e67 2066 6964 656c 6974  sponding fidelit
+000138a0: 6965 732e 2053 6565 202a 7370 6563 7472  ies. See *spectr
+000138b0: 756d 2a20 616e 6420 2a6f 6d65 6761 2a20  um* and *omega* 
+000138c0: 666f 720a 2020 2020 2020 2020 6d6f 7265  for.        more
+000138d0: 2069 6e66 6f72 6d61 7469 6f6e 2e0a 0a20   information... 
+000138e0: 2020 2052 6574 7572 6e73 0a20 2020 202d     Returns.    -
+000138f0: 2d2d 2d2d 2d2d 0a20 2020 2069 6e66 6964  ------.    infid
+00013900: 3a20 6e64 6172 7261 792c 2073 6861 7065  : ndarray, shape
+00013910: 2028 5b5b 6e5f 706c 732c 206e 5f70 6c73   ([[n_pls, n_pls
+00013920: 2c5d 2c20 6e5f 6e6f 7073 2c5d 206e 5f6e  ,], n_nops,] n_n
+00013930: 6f70 7329 0a20 2020 2020 2020 2041 7272  ops).        Arr
+00013940: 6179 2077 6974 6820 7468 6520 696e 6669  ay with the infi
+00013950: 6465 6c69 7479 2063 6f6e 7472 6962 7574  delity contribut
+00013960: 696f 6e73 2066 6f72 2065 6163 6820 7370  ions for each sp
+00013970: 6563 7472 756d 0a20 2020 2020 2020 202a  ectrum.        *
+00013980: 7370 6563 7472 756d 2a20 6f6e 2074 6865  spectrum* on the
+00013990: 206c 6173 7420 6178 6973 206f 7220 6178   last axis or ax
+000139a0: 6573 2c20 6465 7065 6e64 696e 6720 6f6e  es, depending on
+000139b0: 2074 6865 2073 6861 7065 206f 660a 2020   the shape of.  
+000139c0: 2020 2020 2020 2a73 7065 6374 7275 6d2a        *spectrum*
+000139d0: 2061 6e64 202a 7768 6963 682a 2e20 4966   and *which*. If
+000139e0: 2060 6077 6869 6368 6060 2069 7320 6060   ``which`` is ``
+000139f0: 636f 7272 656c 6174 696f 6e73 6060 2c20  correlations``, 
+00013a00: 7468 650a 2020 2020 2020 2020 6669 7273  the.        firs
+00013a10: 7420 7477 6f20 6178 6573 2061 7265 2074  t two axes are t
+00013a20: 6865 2069 6e64 6976 6964 7561 6c20 7075  he individual pu
+00013a30: 6c73 6520 636f 6e74 7269 6275 7469 6f6e  lse contribution
+00013a40: 732e 2049 660a 2020 2020 2020 2020 2a73  s. If.        *s
+00013a50: 7065 6374 7275 6d2a 2069 7320 322d 6420  pectrum* is 2-d 
+00013a60: 2833 2d64 292c 2074 6865 206c 6173 7420  (3-d), the last 
+00013a70: 6178 6973 2028 7477 6f20 6178 6573 2920  axis (two axes) 
+00013a80: 6172 6520 7468 650a 2020 2020 2020 2020  are the.        
+00013a90: 696e 6469 7669 6475 616c 2073 7065 6374  individual spect
+00013aa0: 7261 6c20 636f 6e74 7269 6275 7469 6f6e  ral contribution
+00013ab0: 732e 204f 6e6c 7920 6966 202a 7465 7374  s. Only if *test
+00013ac0: 5f63 6f6e 7665 7267 656e 6365 2a20 6973  _convergence* is
+00013ad0: 0a20 2020 2020 2020 2060 6046 616c 7365  .        ``False
+00013ae0: 6060 2e0a 2020 2020 6e5f 7361 6d70 6c65  ``..    n_sample
+00013af0: 733a 2061 7272 6179 5f6c 696b 650a 2020  s: array_like.  
+00013b00: 2020 2020 2020 4172 7261 7920 7769 7468        Array with
+00013b10: 206e 756d 6265 7220 6f66 2066 7265 7175   number of frequ
+00013b20: 656e 6379 2073 616d 706c 6573 2075 7365  ency samples use
+00013b30: 6420 666f 7220 636f 6e76 6572 6765 6e63  d for convergenc
+00013b40: 650a 2020 2020 2020 2020 7465 7374 2e20  e.        test. 
+00013b50: 4f6e 6c79 2069 6620 2a74 6573 745f 636f  Only if *test_co
+00013b60: 6e76 6572 6765 6e63 652a 2069 7320 6060  nvergence* is ``
+00013b70: 5472 7565 6060 2e0a 2020 2020 636f 6e76  True``..    conv
+00013b80: 6572 6765 6e63 655f 696e 6669 6473 3a20  ergence_infids: 
+00013b90: 6172 7261 795f 6c69 6b65 0a20 2020 2020  array_like.     
+00013ba0: 2020 2041 7272 6179 2077 6974 6820 696e     Array with in
+00013bb0: 6669 6465 6c69 7469 6573 2063 616c 6375  fidelities calcu
+00013bc0: 6c61 7465 6420 696e 2063 6f6e 7665 7267  lated in converg
+00013bd0: 656e 6365 2074 6573 742e 0a20 2020 2020  ence test..     
+00013be0: 2020 204f 6e6c 7920 6966 202a 7465 7374     Only if *test
+00013bf0: 5f63 6f6e 7665 7267 656e 6365 2a20 6973  _convergence* is
+00013c00: 2060 6054 7275 6560 602e 0a0a 2020 2020   ``True``...    
+00013c10: 2e2e 205f 6e6f 7465 733a 0a0a 2020 2020  .. _notes:..    
+00013c20: 4e6f 7465 730a 2020 2020 2d2d 2d2d 2d0a  Notes.    -----.
+00013c30: 2020 2020 5468 6520 696e 6669 6465 6c69      The infideli
+00013c40: 7479 2069 7320 6769 7665 6e20 6279 0a0a  ty is given by..
+00013c50: 2020 2020 2e2e 206d 6174 683a 3a0a 0a20      .. math::.. 
+00013c60: 2020 2020 2020 205c 6d61 7468 6361 6c7b         \mathcal{
+00013c70: 497d 5f7b 5c61 6c70 6861 5c62 6574 617d  I}_{\alpha\beta}
+00013c80: 0a20 2020 2020 2020 2020 2020 2026 3d20  .            &= 
+00013c90: 3120 2d20 5c66 7261 637b 317d 7b64 5e32  1 - \frac{1}{d^2
+00013ca0: 7d5c 6d61 7468 726d 7b74 727d 5c3a 5c74  }\mathrm{tr}\:\t
+00013cb0: 696c 6465 7b5c 6d61 7468 6361 6c7b 557d  ilde{\mathcal{U}
+00013cc0: 7d20 5c5c 0a20 2020 2020 2020 2020 2020  } \\.           
+00013cd0: 2026 3d20 5c66 7261 637b 317d 7b64 7d5c   &= \frac{1}{d}\
+00013ce0: 696e 745f 7b2d 5c69 6e66 7479 7d5e 7b5c  int_{-\infty}^{\
+00013cf0: 696e 6674 797d 0a20 2020 2020 2020 2020  infty}.         
+00013d00: 2020 2020 2020 205c 6672 6163 7b5c 6d61         \frac{\ma
+00013d10: 7468 726d 7b64 7d5c 6f6d 6567 617d 7b32  thrm{d}\omega}{2
+00013d20: 5c70 697d 535f 7b5c 616c 7068 615c 6265  \pi}S_{\alpha\be
+00013d30: 7461 7d28 5c6f 6d65 6761 290a 2020 2020  ta}(\omega).    
+00013d40: 2020 2020 2020 2020 2020 2020 465f 7b5c              F_{\
+00013d50: 616c 7068 615c 6265 7461 7d28 5c6f 6d65  alpha\beta}(\ome
+00013d60: 6761 2920 2b20 5c6d 6174 6863 616c 7b4f  ga) + \mathcal{O
+00013d70: 7d5c 6269 6728 5c78 695e 345c 6269 6729  }\big(\xi^4\big)
+00013d80: 205c 5c0a 2020 2020 2020 2020 2020 2020   \\.            
+00013d90: 263d 205c 7375 6d5f 7b67 2c67 273d 317d  &= \sum_{g,g'=1}
+00013da0: 5e47 205c 6d61 7468 6361 6c7b 497d 5f7b  ^G \mathcal{I}_{
+00013db0: 5c61 6c70 6861 5c62 6574 617d 5e7b 2867  \alpha\beta}^{(g
+00013dc0: 6727 297d 0a0a 2020 2020 7769 7468 203a  g')}..    with :
+00013dd0: 6d61 7468 3a60 535f 7b5c 616c 7068 615c  math:`S_{\alpha\
+00013de0: 6265 7461 7d28 5c6f 6d65 6761 2960 2074  beta}(\omega)` t
+00013df0: 6865 2074 776f 2d73 6964 6564 206e 6f69  he two-sided noi
+00013e00: 7365 2073 7065 6374 7261 6c0a 2020 2020  se spectral.    
+00013e10: 6465 6e73 6974 7920 616e 6420 3a6d 6174  density and :mat
+00013e20: 683a 6046 5f7b 5c61 6c70 6861 5c62 6574  h:`F_{\alpha\bet
+00013e30: 617d 285c 6f6d 6567 6129 6020 7468 6520  a}(\omega)` the 
+00013e40: 6669 7273 742d 6f72 6465 7220 6669 6c74  first-order filt
+00013e50: 6572 0a20 2020 2066 756e 6374 696f 6e20  er.    function 
+00013e60: 666f 7220 6e6f 6973 6520 736f 7572 6365  for noise source
+00013e70: 7320 3a6d 6174 683a 605c 616c 7068 612c  s :math:`\alpha,
+00013e80: 5c62 6574 6160 2e20 5468 6520 6e6f 6973  \beta`. The nois
+00013e90: 6520 7370 6563 7472 756d 0a20 2020 206d  e spectrum.    m
+00013ea0: 6179 2069 6e63 6c75 6465 2063 6f72 7265  ay include corre
+00013eb0: 6c61 7465 6420 6e6f 6973 6520 736f 7572  lated noise sour
+00013ec0: 6365 732c 2074 6861 7420 6973 2c20 6974  ces, that is, it
+00013ed0: 7320 656e 7472 7920 6174 0a20 2020 203a  s entry at.    :
+00013ee0: 6d61 7468 3a60 285c 616c 7068 612c 5c62  math:`(\alpha,\b
+00013ef0: 6574 6129 6020 636f 7272 6573 706f 6e64  eta)` correspond
+00013f00: 7320 746f 2074 6865 2063 6f72 7265 6c61  s to the correla
+00013f10: 7469 6f6e 7320 6265 7477 6565 6e0a 2020  tions between.  
+00013f20: 2020 736f 7572 6365 7320 3a6d 6174 683a    sources :math:
+00013f30: 605c 616c 7068 6160 2061 6e64 203a 6d61  `\alpha` and :ma
+00013f40: 7468 3a60 5c62 6574 6160 2e0a 2020 2020  th:`\beta`..    
+00013f50: 3a6d 6174 683a 605c 6d61 7468 6361 6c7b  :math:`\mathcal{
+00013f60: 497d 5f7b 5c61 6c70 6861 5c62 6574 617d  I}_{\alpha\beta}
+00013f70: 5e7b 2867 6727 297d 6020 6172 6520 7468  ^{(gg')}` are th
+00013f80: 6520 636f 7272 656c 6174 696f 6e0a 2020  e correlation.  
+00013f90: 2020 696e 6669 6465 6c69 7469 6573 2074    infidelities t
+00013fa0: 6861 7420 6361 6e20 6265 2063 6f6d 7075  hat can be compu
+00013fb0: 7465 6420 6279 2073 6574 7469 6e67 0a20  ted by setting. 
+00013fc0: 2020 2060 6077 6869 6368 3d27 636f 7272     ``which='corr
+00013fd0: 656c 6174 696f 6e73 2760 602e 0a0a 0a20  elations'``.... 
+00013fe0: 2020 2054 6f20 636f 6e76 6572 7420 746f     To convert to
+00013ff0: 2074 6865 2061 7665 7261 6765 2067 6174   the average gat
+00014000: 6520 696e 6669 6465 6c69 7479 2c20 7573  e infidelity, us
+00014010: 6520 7468 650a 2020 2020 666f 6c6c 6f77  e the.    follow
+00014020: 696e 6720 7265 6c61 7469 6f6e 2067 6976  ing relation giv
+00014030: 656e 2062 7920 486f 726f 6465 636b 6920  en by Horodecki 
+00014040: 6574 2061 6c2e 205b 486f 7239 395d 5f20  et al. [Hor99]_ 
+00014050: 616e 640a 2020 2020 4e69 656c 7365 6e20  and.    Nielsen 
+00014060: 5b4e 6965 3032 5d5f 3a0a 0a20 2020 202e  [Nie02]_:..    .
+00014070: 2e20 6d61 7468 3a3a 0a0a 2020 2020 2020  . math::..      
+00014080: 2020 5c6d 6174 6863 616c 7b49 7d5f 5c6d    \mathcal{I}_\m
+00014090: 6174 6872 6d7b 6176 677d 203d 205c 6672  athrm{avg} = \fr
+000140a0: 6163 7b64 7d7b 642b 317d 5c6d 6174 6863  ac{d}{d+1}\mathc
+000140b0: 616c 7b49 7d2e 0a0a 2020 2020 5468 6520  al{I}...    The 
+000140c0: 736d 616c 6c6e 6573 7320 7061 7261 6d65  smallness parame
+000140d0: 7465 7220 6973 2067 6976 656e 2062 790a  ter is given by.
+000140e0: 0a20 2020 202e 2e20 6d61 7468 3a3a 0a0a  .    .. math::..
+000140f0: 2020 2020 2020 2020 5c78 695e 3220 3d20          \xi^2 = 
+00014100: 5c73 756d 5f5c 616c 7068 615c 6c65 6674  \sum_\alpha\left
+00014110: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
+00014120: 2020 2020 2020 5c6c 7665 7274 5c6c 7665        \lvert\lve
+00014130: 7274 2042 5f5c 616c 7068 615c 7276 6572  rt B_\alpha\rver
+00014140: 745c 7276 6572 745e 320a 2020 2020 2020  t\rvert^2.      
+00014150: 2020 2020 2020 2020 2020 2020 2020 5c69                \i
+00014160: 6e74 5f7b 2d5c 696e 6674 797d 5e5c 696e  nt_{-\infty}^\in
+00014170: 6674 795c 6672 6163 7b5c 6d61 7468 726d  fty\frac{\mathrm
+00014180: 7b64 7d5c 6f6d 6567 617d 7b32 5c70 697d  {d}\omega}{2\pi}
+00014190: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000141a0: 2020 2020 2053 5f5c 616c 7068 6128 5c6f       S_\alpha(\o
+000141b0: 6d65 6761 295c 6c65 6674 285c 7375 6d5f  mega)\left(\sum_
+000141c0: 6773 5f5c 616c 7068 615e 7b28 6729 7d5c  gs_\alpha^{(g)}\
+000141d0: 4465 6c74 6120 745f 670a 2020 2020 2020  Delta t_g.      
+000141e0: 2020 2020 2020 2020 2020 2020 2020 5c72                \r
+000141f0: 6967 6874 295e 320a 2020 2020 2020 2020  ight)^2.        
+00014200: 2020 2020 2020 2020 5c72 6967 6874 5d2e          \right].
+00014210: 0a0a 2020 2020 4e6f 7465 2074 6861 7420  ..    Note that 
+00014220: 696e 2070 7261 6374 6963 652c 2074 6865  in practice, the
+00014230: 2069 6e74 6567 7261 6c20 6973 206f 6e6c   integral is onl
+00014240: 7920 6576 616c 7561 7465 6420 6f6e 2074  y evaluated on t
+00014250: 6865 0a20 2020 2069 6e74 6572 7661 6c20  he.    interval 
+00014260: 3a6d 6174 683a 605c 6f6d 6567 615c 696e  :math:`\omega\in
+00014270: 5b5c 6f6d 6567 615f 5c6d 6174 6872 6d7b  [\omega_\mathrm{
+00014280: 6d69 6e7d 2c5c 6f6d 6567 615f 5c6d 6174  min},\omega_\mat
+00014290: 6872 6d7b 6d61 787d 5d60 2e0a 0a20 2020  hrm{max}]`...   
+000142a0: 2053 6565 2041 6c73 6f0a 2020 2020 2d2d   See Also.    --
+000142b0: 2d2d 2d2d 2d2d 0a20 2020 2063 616c 6375  ------.    calcu
+000142c0: 6c61 7465 5f64 6563 6179 5f61 6d70 6c69  late_decay_ampli
+000142d0: 7475 6465 733a 2043 616c 6375 6c61 7465  tudes: Calculate
+000142e0: 2074 6865 2066 756c 6c20 6d61 7472 6978   the full matrix
+000142f0: 206f 6620 6669 7273 7420 6f72 6465 7220   of first order 
+00014300: 7465 726d 732e 0a20 2020 2065 7272 6f72  terms..    error
+00014310: 5f74 7261 6e73 6665 725f 6d61 7472 6978  _transfer_matrix
+00014320: 3a20 4361 6c63 756c 6174 6520 7468 6520  : Calculate the 
+00014330: 6675 6c6c 2070 726f 6365 7373 206d 6174  full process mat
+00014340: 7269 782e 0a20 2020 2070 6c6f 7474 696e  rix..    plottin
+00014350: 672e 706c 6f74 5f69 6e66 6964 656c 6974  g.plot_infidelit
+00014360: 795f 636f 6e76 6572 6765 6e63 653a 2043  y_convergence: C
+00014370: 6f6e 7665 6e69 656e 6365 2066 756e 6374  onvenience funct
+00014380: 696f 6e20 746f 2070 6c6f 7420 7265 7375  ion to plot resu
+00014390: 6c74 732e 0a20 2020 2070 756c 7365 5f73  lts..    pulse_s
+000143a0: 6571 7565 6e63 652e 636f 6e63 6174 656e  equence.concaten
+000143b0: 6174 653a 2043 6f6e 6361 7465 6e61 7465  ate: Concatenate
+000143c0: 2060 6050 756c 7365 5365 7175 656e 6365   ``PulseSequence
+000143d0: 6060 206f 626a 6563 7473 2e0a 2020 2020  `` objects..    
+000143e0: 6361 6c63 756c 6174 655f 7075 6c73 655f  calculate_pulse_
+000143f0: 636f 7272 656c 6174 696f 6e5f 6669 6c74  correlation_filt
+00014400: 6572 5f66 756e 6374 696f 6e2e 0a0a 2020  er_function...  
+00014410: 2020 5265 6665 7265 6e63 6573 0a20 2020    References.   
+00014420: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 0a20 2020   ----------..   
+00014430: 202e 2e20 5b48 6f72 3939 5d0a 2020 2020   .. [Hor99].    
+00014440: 2020 2020 486f 726f 6465 636b 692c 204d      Horodecki, M
+00014450: 2e2c 2048 6f72 6f64 6563 6b69 2c20 502e  ., Horodecki, P.
+00014460: 2c20 2620 486f 726f 6465 636b 692c 2052  , & Horodecki, R
+00014470: 2e20 2831 3939 3929 2e20 4765 6e65 7261  . (1999). Genera
+00014480: 6c0a 2020 2020 2020 2020 7465 6c65 706f  l.        telepo
+00014490: 7274 6174 696f 6e20 6368 616e 6e65 6c2c  rtation channel,
+000144a0: 2073 696e 676c 6574 2066 7261 6374 696f   singlet fractio
+000144b0: 6e2c 2061 6e64 2071 7561 7369 6469 7374  n, and quasidist
+000144c0: 696c 6c61 7469 6f6e 2e0a 2020 2020 2020  illation..      
+000144d0: 2020 5068 7973 6963 616c 2052 6576 6965    Physical Revie
+000144e0: 7720 4120 2d20 4174 6f6d 6963 2c20 4d6f  w A - Atomic, Mo
+000144f0: 6c65 6375 6c61 722c 2061 6e64 204f 7074  lecular, and Opt
+00014500: 6963 616c 2050 6879 7369 6373 2c0a 2020  ical Physics,.  
+00014510: 2020 2020 2020 3630 2833 292c 2031 3838        60(3), 188
+00014520: 38e2 8093 3138 3938 2e20 6874 7470 733a  8...1898. https:
+00014530: 2f2f 646f 692e 6f72 672f 3130 2e31 3130  //doi.org/10.110
+00014540: 332f 5068 7973 5265 7641 2e36 302e 3138  3/PhysRevA.60.18
+00014550: 3838 0a0a 2020 2020 2e2e 205b 4e69 6530  88..    .. [Nie0
+00014560: 325d 0a20 2020 2020 2020 204e 6965 6c73  2].        Niels
+00014570: 656e 2c20 4d2e 2041 2e20 2832 3030 3229  en, M. A. (2002)
+00014580: 2e20 4120 7369 6d70 6c65 2066 6f72 6d75  . A simple formu
+00014590: 6c61 2066 6f72 2074 6865 2061 7665 7261  la for the avera
+000145a0: 6765 2067 6174 650a 2020 2020 2020 2020  ge gate.        
+000145b0: 6669 6465 6c69 7479 206f 6620 6120 7175  fidelity of a qu
+000145c0: 616e 7475 6d20 6479 6e61 6d69 6361 6c20  antum dynamical 
+000145d0: 6f70 6572 6174 696f 6e2e 2050 6879 7369  operation. Physi
+000145e0: 6373 204c 6574 7465 7273 2c0a 2020 2020  cs Letters,.    
+000145f0: 2020 2020 5365 6374 696f 6e20 413a 2047      Section A: G
+00014600: 656e 6572 616c 2c20 4174 6f6d 6963 2061  eneral, Atomic a
+00014610: 6e64 2053 6f6c 6964 2053 7461 7465 2050  nd Solid State P
+00014620: 6879 7369 6373 2c20 3330 3328 3429 2c0a  hysics, 303(4),.
+00014630: 2020 2020 2020 2020 3234 39e2 8093 3235          249...25
+00014640: 322e 2068 7474 7073 3a2f 2f64 6f69 2e6f  2. https://doi.o
+00014650: 7267 2f31 302e 3130 3136 2f53 3033 3735  rg/10.1016/S0375
+00014660: 2d39 3630 3128 3032 2930 3132 3732 2d30  -9601(02)01272-0
+00014670: 0a20 2020 2022 2222 0a20 2020 2023 204e  .    """.    # N
+00014680: 6f69 7365 206f 7065 7261 746f 7220 696e  oise operator in
+00014690: 6469 6365 730a 2020 2020 6964 7820 3d20  dices.    idx = 
+000146a0: 7574 696c 2e67 6574 5f69 6e64 6963 6573  util.get_indices
+000146b0: 5f66 726f 6d5f 6964 656e 7469 6669 6572  _from_identifier
+000146c0: 7328 7075 6c73 652e 6e5f 6f70 6572 5f69  s(pulse.n_oper_i
+000146d0: 6465 6e74 6966 6965 7273 2c20 6e5f 6f70  dentifiers, n_op
+000146e0: 6572 5f69 6465 6e74 6966 6965 7273 290a  er_identifiers).
+000146f0: 0a20 2020 2069 6620 7465 7374 5f63 6f6e  .    if test_con
+00014700: 7665 7267 656e 6365 3a0a 2020 2020 2020  vergence:.      
+00014710: 2020 6966 206e 6f74 2063 616c 6c61 626c    if not callabl
+00014720: 6528 7370 6563 7472 756d 293a 0a20 2020  e(spectrum):.   
+00014730: 2020 2020 2020 2020 2072 6169 7365 2054           raise T
+00014740: 7970 6545 7272 6f72 2827 5370 6563 7472  ypeError('Spectr
+00014750: 756d 2073 686f 756c 6420 6265 2063 616c  um should be cal
+00014760: 6c61 626c 6520 7768 656e 2074 6573 745f  lable when test_
+00014770: 636f 6e76 6572 6765 6e63 6520 3d3d 2054  convergence == T
+00014780: 7275 652e 2729 0a0a 2020 2020 2020 2020  rue.')..        
+00014790: 2320 5061 7273 6520 6172 6775 6d65 6e74  # Parse argument
+000147a0: 2064 6963 740a 2020 2020 2020 2020 7472   dict.        tr
+000147b0: 793a 0a20 2020 2020 2020 2020 2020 206f  y:.            o
+000147c0: 6d65 6761 5f49 5220 3d20 6f6d 6567 612e  mega_IR = omega.
+000147d0: 6765 7428 276f 6d65 6761 5f49 5227 2c20  get('omega_IR', 
+000147e0: 322a 6e70 2e70 692f 7075 6c73 652e 7461  2*np.pi/pulse.ta
+000147f0: 752a 3165 2d32 290a 2020 2020 2020 2020  u*1e-2).        
+00014800: 6578 6365 7074 2041 7474 7269 6275 7465  except Attribute
+00014810: 4572 726f 723a 0a20 2020 2020 2020 2020  Error:.         
+00014820: 2020 2072 6169 7365 2054 7970 6545 7272     raise TypeErr
+00014830: 6f72 2827 6f6d 6567 6120 7368 6f75 6c64  or('omega should
+00014840: 2062 6520 6469 6374 696f 6e61 7279 2077   be dictionary w
+00014850: 6974 6820 7061 7261 6d65 7465 7273 2027  ith parameters '
+00014860: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014870: 2020 2020 2020 2020 2020 2020 202b 2027               + '
+00014880: 7768 656e 2074 6573 745f 636f 6e76 6572  when test_conver
+00014890: 6765 6e63 6520 3d3d 2054 7275 652e 2729  gence == True.')
+000148a0: 0a0a 2020 2020 2020 2020 6f6d 6567 615f  ..        omega_
+000148b0: 5556 203d 206f 6d65 6761 2e67 6574 2827  UV = omega.get('
+000148c0: 6f6d 6567 615f 5556 272c 2032 2a6e 702e  omega_UV', 2*np.
+000148d0: 7069 2f70 756c 7365 2e74 6175 2a31 652b  pi/pulse.tau*1e+
+000148e0: 3229 0a20 2020 2020 2020 2073 7061 6369  2).        spaci
+000148f0: 6e67 203d 206f 6d65 6761 2e67 6574 2827  ng = omega.get('
+00014900: 7370 6163 696e 6727 2c20 276c 696e 6561  spacing', 'linea
+00014910: 7227 290a 2020 2020 2020 2020 6e5f 6d69  r').        n_mi
+00014920: 6e20 3d20 6f6d 6567 612e 6765 7428 276e  n = omega.get('n
+00014930: 5f6d 696e 272c 2031 3030 290a 2020 2020  _min', 100).    
+00014940: 2020 2020 6e5f 6d61 7820 3d20 6f6d 6567      n_max = omeg
+00014950: 612e 6765 7428 276e 5f6d 6178 272c 2035  a.get('n_max', 5
+00014960: 3030 290a 2020 2020 2020 2020 6e5f 706f  00).        n_po
+00014970: 696e 7473 203d 206f 6d65 6761 2e67 6574  ints = omega.get
+00014980: 2827 6e5f 706f 696e 7473 272c 2031 3029  ('n_points', 10)
+00014990: 0a0a 2020 2020 2020 2020 2320 416c 6961  ..        # Alia
+000149a0: 7320 6e75 6d70 7927 7320 6c69 6e73 7061  s numpy's linspa
+000149b0: 6365 206f 7220 6c6f 6773 7061 6365 206d  ce or logspace m
+000149c0: 6574 686f 6420 6465 7065 6e64 696e 6720  ethod depending 
+000149d0: 6f6e 2074 6865 2073 7061 6369 6e67 0a20  on the spacing. 
+000149e0: 2020 2020 2020 2023 206f 6d65 6761 2068         # omega h
+000149f0: 6173 0a20 2020 2020 2020 2069 6620 7370  as.        if sp
+00014a00: 6163 696e 6720 3d3d 2027 6c69 6e65 6172  acing == 'linear
+00014a10: 273a 0a20 2020 2020 2020 2020 2020 2078  ':.            x
+00014a20: 7370 6163 6520 3d20 6e70 2e6c 696e 7370  space = np.linsp
+00014a30: 6163 650a 2020 2020 2020 2020 656c 6966  ace.        elif
+00014a40: 2073 7061 6369 6e67 203d 3d20 276c 6f67   spacing == 'log
+00014a50: 273a 0a20 2020 2020 2020 2020 2020 2078  ':.            x
+00014a60: 7370 6163 6520 3d20 6e70 2e67 656f 6d73  space = np.geoms
+00014a70: 7061 6365 0a20 2020 2020 2020 2065 6c73  pace.        els
+00014a80: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00014a90: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+00014aa0: 2273 7061 6369 6e67 2073 686f 756c 6420  "spacing should 
+00014ab0: 6265 2065 6974 6865 7220 276c 696e 6561  be either 'linea
+00014ac0: 7227 206f 7220 276c 6f67 272e 2229 0a0a  r' or 'log'.")..
+00014ad0: 2020 2020 2020 2020 6465 6c74 615f 6e20          delta_n 
+00014ae0: 3d20 286e 5f6d 6178 202d 206e 5f6d 696e  = (n_max - n_min
+00014af0: 292f 2f28 6e5f 706f 696e 7473 202d 2031  )//(n_points - 1
+00014b00: 290a 2020 2020 2020 2020 6e5f 7361 6d70  ).        n_samp
+00014b10: 6c65 7320 3d20 6e70 2e61 7261 6e67 6528  les = np.arange(
+00014b20: 6e5f 6d69 6e2c 206e 5f6d 6178 202b 2064  n_min, n_max + d
+00014b30: 656c 7461 5f6e 2c20 6465 6c74 615f 6e29  elta_n, delta_n)
+00014b40: 0a0a 2020 2020 2020 2020 636f 6e76 6572  ..        conver
+00014b50: 6765 6e63 655f 696e 6669 6473 203d 206e  gence_infids = n
+00014b60: 702e 656d 7074 7928 286c 656e 286e 5f73  p.empty((len(n_s
+00014b70: 616d 706c 6573 292c 206c 656e 2869 6478  amples), len(idx
+00014b80: 2929 290a 2020 2020 2020 2020 666f 7220  ))).        for 
+00014b90: 692c 206e 2069 6e20 656e 756d 6572 6174  i, n in enumerat
+00014ba0: 6528 6e5f 7361 6d70 6c65 7329 3a0a 2020  e(n_samples):.  
+00014bb0: 2020 2020 2020 2020 2020 6672 6571 7320            freqs 
+00014bc0: 3d20 7873 7061 6365 286f 6d65 6761 5f49  = xspace(omega_I
+00014bd0: 522c 206f 6d65 6761 5f55 562c 206e 290a  R, omega_UV, n).
+00014be0: 2020 2020 2020 2020 2020 2020 636f 6e76              conv
+00014bf0: 6572 6765 6e63 655f 696e 6669 6473 5b69  ergence_infids[i
+00014c00: 5d20 3d20 696e 6669 6465 6c69 7479 2870  ] = infidelity(p
+00014c10: 756c 7365 2c20 7370 6563 7472 756d 2866  ulse, spectrum(f
+00014c20: 7265 7173 292c 2066 7265 7173 2c0a 2020  reqs), freqs,.  
+00014c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014c50: 2020 2020 2020 2020 2020 2020 206e 5f6f               n_o
+00014c60: 7065 725f 6964 656e 7469 6669 6572 733d  per_identifiers=
+00014c70: 6e5f 6f70 6572 5f69 6465 6e74 6966 6965  n_oper_identifie
+00014c80: 7273 2c0a 2020 2020 2020 2020 2020 2020  rs,.            
+00014c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014cb0: 2020 2077 6869 6368 3d27 746f 7461 6c27     which='total'
+00014cc0: 2c20 7368 6f77 5f70 726f 6772 6573 7362  , show_progressb
+00014cd0: 6172 3d73 686f 775f 7072 6f67 7265 7373  ar=show_progress
+00014ce0: 6261 722c 0a20 2020 2020 2020 2020 2020  bar,.           
+00014cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014d10: 2020 2020 6361 6368 655f 696e 7465 726d      cache_interm
+00014d20: 6564 6961 7465 733d 4661 6c73 652c 2072  ediates=False, r
+00014d30: 6574 7572 6e5f 736d 616c 6c6e 6573 733d  eturn_smallness=
+00014d40: 4661 6c73 652c 0a20 2020 2020 2020 2020  False,.         
+00014d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014d70: 2020 2020 2020 7465 7374 5f63 6f6e 7665        test_conve
+00014d80: 7267 656e 6365 3d46 616c 7365 290a 0a20  rgence=False).. 
+00014d90: 2020 2020 2020 2072 6574 7572 6e20 6e5f         return n_
+00014da0: 7361 6d70 6c65 732c 2063 6f6e 7665 7267  samples, converg
+00014db0: 656e 6365 5f69 6e66 6964 730a 0a20 2020  ence_infids..   
+00014dc0: 2069 6620 7768 6963 6820 3d3d 2027 746f   if which == 'to
+00014dd0: 7461 6c27 3a0a 2020 2020 2020 2020 6966  tal':.        if
+00014de0: 206e 6f74 2070 756c 7365 2e62 6173 6973   not pulse.basis
+00014df0: 2e69 7374 7261 6365 6c65 7373 3a0a 2020  .istraceless:.  
+00014e00: 2020 2020 2020 2020 2020 2320 4669 6465            # Fide
+00014e10: 6c69 7479 206e 6f74 2073 696d 706c 7920  lity not simply 
+00014e20: 7375 6d20 6f66 2064 6961 676f 6e61 6c20  sum of diagonal 
+00014e30: 6f66 2064 6563 6179 2061 6d70 6c69 7475  of decay amplitu
+00014e40: 6465 7320 4761 6d6d 615f 6b6b 0a20 2020  des Gamma_kk.   
+00014e50: 2020 2020 2020 2020 2023 2062 7574 2074           # but t
+00014e60: 7261 6365 2074 656e 736f 7220 706c 6179  race tensor play
+00014e70: 7320 6120 726f 6c65 2c20 6366 2065 712e  s a role, cf eq.
+00014e80: 2028 3339 292e 2046 6f72 2074 7261 6365   (39). For trace
+00014e90: 6c65 7373 2062 6173 6573 2c0a 2020 2020  less bases,.    
+00014ea0: 2020 2020 2020 2020 2320 7468 6520 7472          # the tr
+00014eb0: 6163 6520 7465 6e73 6f72 2074 6572 6d20  ace tensor term 
+00014ec0: 7265 6475 6365 7320 746f 2064 656c 7461  reduces to delta
+00014ed0: 5f69 6a2e 0a20 2020 2020 2020 2020 2020  _ij..           
+00014ee0: 2074 7261 6365 7320 3d20 7075 6c73 652e   traces = pulse.
+00014ef0: 6261 7369 732e 666f 7572 5f65 6c65 6d65  basis.four_eleme
+00014f00: 6e74 5f74 7261 6365 730a 2020 2020 2020  nt_traces.      
+00014f10: 2020 2020 2020 7472 6163 6573 5f64 6961        traces_dia
+00014f20: 6720 3d20 2873 7061 7273 652e 6469 6167  g = (sparse.diag
+00014f30: 6f6e 616c 2874 7261 6365 732c 2061 7869  onal(traces, axi
+00014f40: 7331 3d32 2c20 6178 6973 323d 3329 2e73  s1=2, axis2=3).s
+00014f50: 756d 282d 3129 0a20 2020 2020 2020 2020  um(-1).         
+00014f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014f70: 2020 2d20 7370 6172 7365 2e64 6961 676f    - sparse.diago
+00014f80: 6e61 6c28 7472 6163 6573 2c20 6178 6973  nal(traces, axis
+00014f90: 313d 312c 2061 7869 7332 3d33 292e 7375  1=1, axis2=3).su
+00014fa0: 6d28 2d31 2929 2e74 6f64 656e 7365 2829  m(-1)).todense()
+00014fb0: 0a0a 2020 2020 2020 2020 2020 2020 636f  ..            co
+00014fc0: 6e74 726f 6c5f 6d61 7472 6978 203d 2070  ntrol_matrix = p
+00014fd0: 756c 7365 2e67 6574 5f63 6f6e 7472 6f6c  ulse.get_control
+00014fe0: 5f6d 6174 7269 7828 6f6d 6567 612c 2073  _matrix(omega, s
+00014ff0: 686f 775f 7072 6f67 7265 7373 6261 722c  how_progressbar,
+00015000: 2063 6163 6865 5f69 6e74 6572 6d65 6469   cache_intermedi
+00015010: 6174 6573 290a 2020 2020 2020 2020 2020  ates).          
+00015020: 2020 6669 6c74 6572 5f66 756e 6374 696f    filter_functio
+00015030: 6e20 3d20 6e70 2e65 696e 7375 6d28 2761  n = np.einsum('a
+00015040: 6b6f 2c62 6c6f 2c6b 6c2d 3e61 626f 272c  ko,blo,kl->abo',
+00015050: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015070: 2020 2020 2020 2020 2063 6f6e 7472 6f6c           control
+00015080: 5f6d 6174 7269 782e 636f 6e6a 2829 2c20  _matrix.conj(), 
+00015090: 636f 6e74 726f 6c5f 6d61 7472 6978 2c20  control_matrix, 
+000150a0: 7472 6163 6573 5f64 6961 6729 2f70 756c  traces_diag)/pul
+000150b0: 7365 2e64 0a20 2020 2020 2020 2065 6c73  se.d.        els
+000150c0: 653a 0a20 2020 2020 2020 2020 2020 2066  e:.            f
+000150d0: 696c 7465 725f 6675 6e63 7469 6f6e 203d  ilter_function =
+000150e0: 2070 756c 7365 2e67 6574 5f66 696c 7465   pulse.get_filte
+000150f0: 725f 6675 6e63 7469 6f6e 286f 6d65 6761  r_function(omega
+00015100: 2c20 7768 6963 683d 2766 6964 656c 6974  , which='fidelit
+00015110: 7927 2c0a 2020 2020 2020 2020 2020 2020  y',.            
+00015120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015140: 2020 2020 2020 2020 2020 2020 7368 6f77              show
+00015150: 5f70 726f 6772 6573 7362 6172 3d73 686f  _progressbar=sho
+00015160: 775f 7072 6f67 7265 7373 6261 722c 0a20  w_progressbar,. 
+00015170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000151a0: 2020 2020 2020 2063 6163 6865 5f69 6e74         cache_int
+000151b0: 6572 6d65 6469 6174 6573 3d63 6163 6865  ermediates=cache
+000151c0: 5f69 6e74 6572 6d65 6469 6174 6573 290a  _intermediates).
+000151d0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+000151e0: 2020 2320 7768 6963 6820 3d3d 2027 636f    # which == 'co
+000151f0: 7272 656c 6174 696f 6e73 270a 2020 2020  rrelations'.    
+00015200: 2020 2020 6966 2070 756c 7365 2e69 735f      if pulse.is_
+00015210: 6361 6368 6564 2827 6f6d 6567 6127 2920  cached('omega') 
+00015220: 616e 6420 6e6f 7420 6e70 2e61 7272 6179  and not np.array
+00015230: 5f65 7175 616c 2870 756c 7365 2e6f 6d65  _equal(pulse.ome
+00015240: 6761 2c20 6f6d 6567 6129 3a0a 2020 2020  ga, omega):.    
+00015250: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+00015260: 6c75 6545 7272 6f72 2827 5075 6c73 6520  lueError('Pulse 
+00015270: 636f 7272 656c 6174 696f 6e20 696e 6669  correlation infi
+00015280: 6465 6c69 7469 6573 2072 6571 7565 7374  delities request
+00015290: 6564 2027 0a20 2020 2020 2020 2020 2020  ed '.           
+000152a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000152b0: 2020 2b20 2762 7574 206f 6d65 6761 206e    + 'but omega n
+000152c0: 6f74 2065 7175 616c 2074 6f20 6361 6368  ot equal to cach
+000152d0: 6564 2066 7265 7175 656e 6369 6573 2e27  ed frequencies.'
+000152e0: 290a 0a20 2020 2020 2020 2066 696c 7465  )..        filte
+000152f0: 725f 6675 6e63 7469 6f6e 203d 2070 756c  r_function = pul
+00015300: 7365 2e67 6574 5f70 756c 7365 5f63 6f72  se.get_pulse_cor
+00015310: 7265 6c61 7469 6f6e 5f66 696c 7465 725f  relation_filter_
+00015320: 6675 6e63 7469 6f6e 2829 0a0a 2020 2020  function()..    
+00015330: 696e 7465 6772 616e 6420 3d20 5f67 6574  integrand = _get
+00015340: 5f69 6e74 6567 7261 6e64 2873 7065 6374  _integrand(spect
+00015350: 7275 6d2c 206f 6d65 6761 2c20 6964 782c  rum, omega, idx,
+00015360: 2077 6869 6368 2c20 2766 6964 656c 6974   which, 'fidelit
+00015370: 7927 2c0a 2020 2020 2020 2020 2020 2020  y',.            
+00015380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015390: 2020 2066 696c 7465 725f 6675 6e63 7469     filter_functi
+000153a0: 6f6e 3d66 696c 7465 725f 6675 6e63 7469  on=filter_functi
+000153b0: 6f6e 290a 2020 2020 696e 6669 6420 3d20  on).    infid = 
+000153c0: 7574 696c 2e69 6e74 6567 7261 7465 2869  util.integrate(i
+000153d0: 6e74 6567 7261 6e64 2c20 6f6d 6567 6129  ntegrand, omega)
+000153e0: 2f28 322a 6e70 2e70 692a 7075 6c73 652e  /(2*np.pi*pulse.
+000153f0: 6429 0a0a 2020 2020 6966 2072 6574 7572  d)..    if retur
+00015400: 6e5f 736d 616c 6c6e 6573 733a 0a20 2020  n_smallness:.   
+00015410: 2020 2020 2069 6620 7370 6563 7472 756d       if spectrum
+00015420: 2e6e 6469 6d20 3e20 323a 0a20 2020 2020  .ndim > 2:.     
+00015430: 2020 2020 2020 2072 6169 7365 204e 6f74         raise Not
+00015440: 496d 706c 656d 656e 7465 6445 7272 6f72  ImplementedError
+00015450: 2827 536d 616c 6c6e 6573 7320 7061 7261  ('Smallness para
+00015460: 6d65 7465 7220 6f6e 6c79 2069 6d70 6c65  meter only imple
+00015470: 6d65 6e74 6564 2027 0a20 2020 2020 2020  mented '.       
+00015480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015490: 2020 2020 2020 2020 2020 2020 2020 202b                 +
+000154a0: 2027 666f 7220 756e 636f 7272 656c 6174   'for uncorrelat
+000154b0: 6564 206e 6f69 7365 2073 6f75 7263 6573  ed noise sources
+000154c0: 2729 0a0a 2020 2020 2020 2020 5431 203d  ')..        T1 =
+000154d0: 2075 7469 6c2e 696e 7465 6772 6174 6528   util.integrate(
+000154e0: 7370 6563 7472 756d 2c20 6f6d 6567 6129  spectrum, omega)
+000154f0: 2f28 322a 6e70 2e70 6929 0a20 2020 2020  /(2*np.pi).     
+00015500: 2020 2054 3220 3d20 2870 756c 7365 2e64     T2 = (pulse.d
+00015510: 742a 7075 6c73 652e 6e5f 636f 6566 6673  t*pulse.n_coeffs
+00015520: 5b69 6478 5d29 2e73 756d 2861 7869 733d  [idx]).sum(axis=
+00015530: 2d31 292a 2a32 0a20 2020 2020 2020 2054  -1)**2.        T
+00015540: 3320 3d20 7574 696c 2e61 6273 3228 7075  3 = util.abs2(pu
+00015550: 6c73 652e 6e5f 6f70 6572 735b 6964 785d  lse.n_opers[idx]
+00015560: 292e 7375 6d28 6178 6973 3d28 312c 2032  ).sum(axis=(1, 2
+00015570: 2929 0a20 2020 2020 2020 2078 6920 3d20  )).        xi = 
+00015580: 6e70 2e73 7172 7428 2854 312a 5432 2a54  np.sqrt((T1*T2*T
+00015590: 3329 2e73 756d 2829 290a 0a20 2020 2020  3).sum())..     
+000155a0: 2020 2072 6574 7572 6e20 696e 6669 642c     return infid,
+000155b0: 2078 690a 0a20 2020 2072 6574 7572 6e20   xi..    return 
+000155c0: 696e 6669 640a                           infid.
```

### Comparing `filter_functions-1.1.1/filter_functions/plotting.py` & `filter_functions-1.1.2/filter_functions/plotting.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,16 +51,16 @@
 import matplotlib.pyplot as plt
 import numpy as np
 from matplotlib import cm, collections, colors, lines
 from mpl_toolkits import axes_grid1
 from numpy import ndarray
 
 from . import numeric, util
-from .types import (Axes, Coefficients, Colormap, Figure, FigureAxes, FigureAxesLegend, FigureGrid,
-                    Grid, Operator, State)
+from .types import (Axes, Coefficients, Colormap, Cycler, Figure, FigureAxes, FigureAxesLegend,
+                    FigureGrid, Grid, Operator, State)
 
 __all__ = ['plot_cumulant_function', 'plot_infidelity_convergence', 'plot_filter_function',
            'plot_pulse_correlation_filter_function', 'plot_pulse_train']
 
 try:
     import qutip as qt
     __all__.append('plot_bloch_vector_evolution')
@@ -125,50 +125,35 @@
         b.axes.set_box_aspect([1, 1, 1])
 
     b.xlabel = [r'$|+\rangle$', '']
     b.ylabel = [r'$|+_i\rangle$', '']
     return b
 
 
-@util.parse_optional_parameters(prop=('total', 'piecewise'))
-def get_states_from_prop(U: Sequence[Operator], psi0: Optional[State] = None,
-                         prop: str = 'total') -> ndarray:
+def get_states_from_prop(U: Sequence[Operator], psi0: Optional[State] = None) -> ndarray:
     r"""
     Get the the quantum state at time t from the propagator and the
     inital state:
 
     .. math::
 
         |\psi(t)\rangle = U(t, 0)|\psi(0)\rangle
 
-    If *prop* is 'piecewise', then it is assumed that *U* is the
-    propagator of a piecewise-constant control:
-
-    .. math::
-        |\psi(t)\rangle = \prod_{l=1}^n U(t_l, t_{l-1})|\psi(0)\rangle
-
-    with :math:`t_0\equiv 0` and :math:`t_n\equiv t`.
-
     """
     if psi0 is None:
-        psi0 = np.c_[1:-1:-1]  # |0>
+        # default to |0>
+        psi0 = np.c_[1:-1:-1]
+    elif hasattr(psi0, 'full'):
+        # qutip.Qobj
+        psi0 = psi0.full()
 
-    psi0 = psi0.full() if hasattr(psi0, 'full') else psi0  # qutip.Qobj
-    d = max(psi0.shape)
-    states = np.empty((len(U), d, 1), dtype=complex)
-    if prop == 'total':
-        for j in range(len(U)):
-            states[j] = U[j] @ psi0
-    else:
-        # prop == 'piecewise'
-        states[0] = U[0] @ psi0
-        for j in range(1, len(U)):
-            states[j] = U[j] @ states[j-1]
+    if psi0.shape[-2:] != (2, 1):
+        raise ValueError('Initial state should be shape (..., 2, 1)')
 
-    return states
+    return U @ psi0
 
 
 def plot_bloch_vector_evolution(
         pulse: 'PulseSequence',
         psi0: Optional[State] = None,
         b: Optional[qt.Bloch] = None,
         n_samples: Optional[int] = None,
@@ -285,15 +270,15 @@
 
 
 def plot_pulse_train(
         pulse: 'PulseSequence',
         c_oper_identifiers: Optional[Sequence[int]] = None,
         fig: Optional[Figure] = None,
         axes: Optional[Axes] = None,
-        cycler: Optional['cycler.Cycler'] = None,
+        cycler: Optional[Cycler] = None,
         plot_kw: Optional[dict] = {},
         subplot_kw: Optional[dict] = None,
         gridspec_kw: Optional[dict] = None,
         **figure_kw
 ) -> FigureAxesLegend:
     """
     Plot the pulsetrain of the ``PulseSequence`` *pulse*.
@@ -376,15 +361,15 @@
         omega: Optional[Coefficients] = None,
         n_oper_identifiers: Optional[Sequence[int]] = None,
         fig: Optional[Figure] = None,
         axes: Optional[Axes] = None,
         xscale: str = 'log',
         yscale: str = 'linear',
         omega_in_units_of_tau: bool = True,
-        cycler: Optional['cycler.Cycler'] = None,
+        cycler: Optional[Cycler] = None,
         plot_kw: dict = {},
         subplot_kw: Optional[dict] = None,
         gridspec_kw: Optional[dict] = None,
         **figure_kw
 ) -> FigureAxesLegend:
     r"""
     Plot the fidelity filter function(s) of the given PulseSequence for
@@ -506,15 +491,15 @@
 def plot_pulse_correlation_filter_function(
         pulse: 'PulseSequence',
         n_oper_identifiers: Optional[Sequence[int]] = None,
         fig: Optional[Figure] = None,
         xscale: str = 'log',
         yscale: str = 'linear',
         omega_in_units_of_tau: bool = True,
-        cycler: Optional['cycler.Cycler'] = None,
+        cycler: Optional[Cycler] = None,
         plot_kw: dict = {},
         subplot_kw: Optional[dict] = None,
         gridspec_kw: Optional[dict] = None,
         **figure_kw
 ) -> FigureAxesLegend:
     r"""
     Plot the fidelity pulse correlation filter functions of the given
@@ -727,15 +712,15 @@
     function is calculated for those parameters, or with a precomputed
     cumulant function.
 
     As of now, only auto-correlated spectra are implemented.
 
     Parameters
     ----------
-    pulse: 'PulseSequence'
+    pulse: PulseSequence
         The pulse sequence.
     spectrum: ndarray
         The two-sided noise spectrum.
     omega: array_like
         The frequencies for which to evaluate the error transfer matrix.
     cumulant_function: ndarray, shape (n_nops, d**2, d**2)
         A precomputed cumulant function. If given, *pulse*, *spectrum*,
@@ -797,21 +782,23 @@
         if n_oper_identifiers is None:
             if pulse is not None and len(pulse.n_oper_identifiers) == len(K):
                 n_oper_identifiers = pulse.n_oper_identifiers
             else:
                 n_oper_identifiers = [f'$B_{{{i}}}$' for i in range(len(n_oper_inds))]
         else:
             if len(n_oper_identifiers) != len(K):
-                raise ValueError('Both precomputed cumulant function and n_oper_identifiers ' +
-                                 f'given but not same len: {len(K)} != {len(n_oper_identifiers)}')
+                raise ValueError(
+                    'Both precomputed cumulant function and n_oper_identifiers '
+                    + f'given but not same len: {len(K)} != {len(n_oper_identifiers)}'
+                )
 
     else:
         if pulse is None or spectrum is None or omega is None:
-            raise ValueError('Require either precomputed cumulant function ' +
-                             'or pulse, spectrum, and omega as arguments.')
+            raise ValueError('Require either precomputed cumulant function '
+                             + 'or pulse, spectrum, and omega as arguments.')
 
         n_oper_inds = util.get_indices_from_identifiers(pulse.n_oper_identifiers,
                                                         n_oper_identifiers)
         n_oper_identifiers = pulse.n_oper_identifiers[n_oper_inds]
         K = numeric.calculate_cumulant_function(pulse, spectrum, omega, n_oper_identifiers,
                                                 'total', second_order)
         if K.ndim == 4:
@@ -848,16 +835,16 @@
         if fig is None:
             figsize = figure_kw.pop('figsize', (8*n_cols, 6*n_rows))
             fig = plt.figure(figsize=figsize, **figure_kw)
 
         grid = axes_grid1.ImageGrid(fig, **grid_kw)
     else:
         if len(grid) != len(n_oper_inds):
-            raise ValueError('Size of supplied ImageGrid instance does not ' +
-                             'match the number of n_oper_identifiers given!')
+            raise ValueError('Size of supplied ImageGrid instance does not '
+                             + 'match the number of n_oper_identifiers given!')
 
         fig = grid[0].get_figure()
 
     # Parse default arguments
     if cmap is not None:
         plt.get_cmap(cmap)
     else:
```

### Comparing `filter_functions-1.1.1/filter_functions/pulse_sequence.py` & `filter_functions-1.1.2/filter_functions/pulse_sequence.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,25 +156,31 @@
     >>> # Plot the resulting filter function:
     >>> from filter_functions import plotting
     >>> fig, ax, leg = plotting.plot_filter_function(pulse)
 
     Attributes
     ----------
     c_opers: ndarray, shape (n_cops, d, d)
-        Control operators
+        Control operators. Note that they are stored sorted by their
+        corresponding identifiers.
     n_opers: ndarray, shape (n_nops, d, d)
-        Noise operators
+        Noise operators. Note that they are stored sorted by their
+        corresponding identifiers.
     c_oper_identifers: sequence of str
-        Identifiers for the control operators of the system
+        Identifiers for the control operators of the system. Stored
+        sorted.
     n_oper_identifers: sequence of str
-        Identifiers for the noise operators of the system
+        Identifiers for the noise operators of the system. Stored
+        sorted.
     c_coeffs: ndarray, shape (n_cops, n_dt)
-        Control parameters in units of :math:`\hbar`
+        Control parameters in units of :math:`\hbar`. Note that they
+        are stored sorted by their corresponding identifiers.
     n_coeffs: ndarray, shape (n_nops, n_dt)
-        Noise sensitivities in units of :math:`\hbar`
+        Noise sensitivities in units of :math:`\hbar`. Note that they
+        are stored sorted by their corresponding identifiers.
     dt: ndarray, shape (n_dt,)
         Time steps
     t: ndarray, shape (n_dt + 1,)
         Absolute times taken to start at :math:`t_0\equiv 0`
     tau: float
         Total duration. Equal to t[-1].
     d: int
@@ -192,15 +198,15 @@
         Eigenvalues :math:`D^{(g)}`
     eigvecs: ndarray, shape (n_dt, d, d)
         Eigenvectors :math:`V^{(g)}`
     propagators: ndarray, shape (n_dt+1, d, d)
         Cumulative propagators :math:`Q_g`
     total_propagator: ndarray, shape (d, d)
         The total propagator :math:`Q` of the pulse alone. That is,
-        :math:`|\psi(\tau)\rangle = propagators|\psi(0)\rangle`.
+        :math:`|\psi(\tau)\rangle = Q|\psi(0)\rangle`.
     total_propagator_liouville: array_like, shape (d**2, d**2)
         The transfer matrix for the total propagator of the pulse. Given
         by
         ``liouville_representation(pulse.total_propagator, pulse.basis)``.
 
     Furthermore, when the filter function is calculated, the frequencies
     are cached as well as other relevant quantities.
@@ -243,27 +249,29 @@
         self.c_coeffs = None
         self.n_coeffs = None
         self.dt = None
         self.d = None
         self.basis = None
 
         # Parse the input arguments and set attributes
-        attributes = ('c_opers', 'c_oper_identifiers', 'c_coeffs', 'n_opers',
-                      'n_oper_identifiers', 'n_coeffs', 'dt', 'd', 'basis')
+        # TODO: Jesus, this is in need of refactoring.
+        attributes = ('c_opers', 'c_oper_identifiers', 'c_coeffs',
+                      'n_opers', 'n_oper_identifiers', 'n_coeffs',
+                      'dt', 'd', 'basis')
         if not args:
             # Bypass args parsing and directly set necessary attributes
             values = (kwargs[attr] for attr in attributes)
         else:
             if len(args) == 4:
                 # basis given as arg, not kwarg
                 kwargs['basis'] = args[-1]
             elif len(args) < 3:
                 posargs = ['H_c', 'H_n', 'dt']
-                raise TypeError(f'Missing {3 - len(args)} required positional argument(s): ' +
-                                f'{posargs[len(args):]}')
+                raise TypeError(f'Missing {3 - len(args)} required positional argument(s): '
+                                + f'{posargs[len(args):]}')
 
             values = _parse_args(*args[:3], **kwargs)
 
         for attr, value in zip(attributes, values):
             setattr(self, attr, value)
 
         # Initialize attributes that can be set by bound methods to None
@@ -582,18 +590,18 @@
 
     def get_pulse_correlation_control_matrix(self) -> ndarray:
         """Get the pulse correlation control matrix if it was cached."""
         if self.is_cached('control_matrix_pc'):
             return self._control_matrix_pc
 
         raise util.CalculationError(
-            "Could not get the pulse correlation control matrix since it " +
-            "was not computed during concatenation. Please run the " +
-            "concatenation again with 'calc_pulse_correlation_FF' set to " +
-            "True."
+            "Could not get the pulse correlation control matrix since it "
+            + "was not computed during concatenation. Please run the "
+            + "concatenation again with 'calc_pulse_correlation_FF' set to "
+            + "True."
         )
 
     @util.parse_optional_parameters(which=('fidelity', 'generalized'), order=(1, 2))
     def get_filter_function(
             self, omega: Coefficients,
             which: str = 'fidelity',
             order: int = 1,
@@ -842,53 +850,97 @@
             else:
                 # which == 'generalized'
                 self._filter_function_pc_gen = F_pc
 
             return F_pc
 
         raise util.CalculationError(
-            "Could not get the pulse correlation filter function since it " +
-            "was not computed during concatenation. Please run the " +
-            "concatenation again with 'calc_pulse_correlation_FF' set to True."
+            "Could not get the pulse correlation filter function since it "
+            + "was not computed during concatenation. Please run the "
+            + "concatenation again with 'calc_pulse_correlation_FF' set to True."
         )
 
     def get_filter_function_derivative(
             self,
             omega: Coefficients,
             control_identifiers: Optional[Sequence[str]] = None,
+            n_oper_identifiers: Optional[Sequence[str]] = None,
             n_coeffs_deriv: Optional[Sequence[Coefficients]] = None
     ) -> ndarray:
         r"""Calculate the pulse sequence's filter function derivative.
 
         Parameters
         ----------
         omega: array_like, shape (n_omega,)
             Frequencies at which the pulse control matrix is to be
             evaluated.
-        control_identifiers: Sequence[str]
-            Sequence of strings with the control identifiern to
+        control_identifiers: Sequence[str], shape (n_ctrl,)
+            Sequence of strings with the control identifiers to
             distinguish between control and drift Hamiltonian. The
-            default is None.
+            default is None, in which case the derivative is computed
+            for all known non-noise operators.
+        n_oper_identifiers: Sequence[str], shape (n_nops,)
+            Sequence of strings with the noise identifiers for which to
+            compute the derivative contribution. The default is None, in
+            which case it is computed for all known noise operators.
         n_coeffs_deriv: array_like, shape (n_nops, n_ctrl, n_dt)
             The derivatives of the noise susceptibilities by the control
-            amplitudes. Defaults to None.
+            amplitudes. The rows and columns should be in the same order
+            as the corresponding identifiers above. Defaults to None, in
+            which case the coefficients are assumed to be constant and
+            hence their derivative vanishing.
+
+            .. warning::
+
+                Internally, control and noise terms of the Hamiltonian
+                are stored alphanumerically sorted by their identifiers.
+                If the noise and/or control identifiers above are not
+                explicitly given, the rows and/or columns of this
+                parameter need to be sorted in the same fashion.
 
         Returns
         -------
         filter_function_deriv: ndarray, shape (n_nops, n_t, n_ctrl, n_omega)
             The regular filter functions' derivatives for variation in
-            each control contribution.
+            each control contribution. Sorted in the same fashion as
+            `n_coeffs_deriv` or, if not given, alphanumerically by the
+            identifiers.
 
         """
-        control_matrix = self.get_control_matrix(omega, cache_intermediates=True)
+        c_idx = util.get_indices_from_identifiers(self.c_oper_identifiers, control_identifiers)
+        n_idx = util.get_indices_from_identifiers(self.n_oper_identifiers, n_oper_identifiers)
 
+        if n_coeffs_deriv is not None:
+            # TODO 05/22: walrus once support for 3.7 is dropped.
+            actual_shape = np.shape(n_coeffs_deriv)
+            required_shape = (len(n_idx), len(c_idx), len(self))
+            if actual_shape != required_shape:
+                raise ValueError(f'Expected n_coeffs_deriv to be of shape {required_shape}, '
+                                 f'not {actual_shape}. Did you forget to specify identifiers?')
+            else:
+                # Do nothing; n_coeffs_deriv specifies the sorting order. If identifiers
+                # are given, we sort everything else by them. If not, n_coeffs_deriv is
+                # expected to be sorted in accordance with the opers and coeffs.
+                pass
+
+        # Check if we can pass on intermediates.
+        intermediates = dict()
+        # TODO 05/22: walrus once support for 3.7 is dropped.
+        n_opers_transformed = self._intermediates.get('n_opers_transformed')
+        first_order_integral = self._intermediates.get('first_order_integral')
+        if n_opers_transformed is not None:
+            intermediates['n_opers_transformed'] = n_opers_transformed[n_idx]
+        if first_order_integral is not None:
+            intermediates['first_order_integral'] = first_order_integral
+
+        control_matrix = self.get_control_matrix(omega, cache_intermediates=True)[n_idx]
         control_matrix_deriv = gradient.calculate_derivative_of_control_matrix_from_scratch(
             omega, self.propagators, self.eigvals, self.eigvecs, self.basis, self.t, self.dt,
-            self.n_opers, self.n_coeffs, self.c_opers, self.c_oper_identifiers,
-            control_identifiers, n_coeffs_deriv, self._intermediates
+            self.n_opers[n_idx], self.n_coeffs[n_idx], self.c_opers[c_idx], n_coeffs_deriv,
+            intermediates
         )
         return gradient.calculate_filter_function_derivative(control_matrix, control_matrix_deriv)
 
     def get_total_phases(self, omega: Coefficients) -> ndarray:
         """Get the (cached) total phase factors for this pulse and omega."""
         # Only calculate if not calculated before for the same frequencies
         if np.array_equal(self.omega, omega):
@@ -1156,36 +1208,36 @@
     basis = kwargs.pop('basis', None)
     if basis is None:
         # Use generalized Gell-Mann basis by default since we have a nice
         # expression for a basis expansion
         basis = Basis.ggm(d)
     else:
         if not hasattr(basis, 'btype'):
-            raise ValueError("Expected basis to be an instance of the " +
-                             f"'filter_functions.basis.Basis' class, not {type(basis)}!")
+            raise ValueError("Expected basis to be an instance of the "
+                             + f"'filter_functions.basis.Basis' class, not {type(basis)}!")
         if basis.shape[1:] != (d, d):
             # Make sure the basis has the correct dimension (we allow an
             # incomplete set)
-            raise ValueError("Expected basis elements to be of shape " +
-                             f"({d}, {d}), not {basis.shape[1:]}!")
+            raise ValueError("Expected basis elements to be of shape "
+                             + f"({d}, {d}), not {basis.shape[1:]}!")
 
     return (*control_args, *noise_args, dt, d, basis)
 
 
 def _parse_Hamiltonian(H: Hamiltonian, n_dt: int, H_str: str) -> Tuple[Sequence[Operator],
                                                                        Sequence[str],
                                                                        Sequence[Coefficients]]:
     """Helper function to parse the Hamiltonian in QuTiP format."""
     # Check correct types of the various levels of nestedness
     if not isinstance(H, (list, tuple)):
         raise TypeError(f'Expected {H_str} to be a list of lists, not of type {type(H)}!')
 
     if not all(isinstance(item, (list, tuple)) for item in H):
-        raise TypeError(f'Expected {H_str} to be a list of lists but found at least one item ' +
-                        'of H not of type list or tuple!')
+        raise TypeError(f'Expected {H_str} to be a list of lists but found at least one item '
+                        + 'of H not of type list or tuple!')
 
     # Unzip the nested lists into operators and coefficient arrays. Since
     # identifiers are optional, we need to perform a check if they were given.
     opers, *args = zip_longest(*H, fillvalue=None)
     if len(args) == 1:
         coeffs = args[0]
         identifiers = None
@@ -1310,16 +1362,16 @@
         op_to_id = oper_to_identifier_mapping.setdefault(oper, set())
         op_to_id.add(identifier)
         id_to_op = identifier_to_oper_mapping.setdefault(identifier, set())
         id_to_op.add(oper)
 
     if any(len(value) > 1 for value in oper_to_identifier_mapping.values()):
         # Clash: two different identifiers are assigned to the same operator
-        raise ValueError(f'Trying to concatenate pulses with equal {kind} operators but ' +
-                         f'different identifiers. Please choose unique {kind} identifiers!')
+        raise ValueError(f'Trying to concatenate pulses with equal {kind} operators but '
+                         + f'different identifiers. Please choose unique {kind} identifiers!')
 
     # A dict that maps the identifiers of each Hamiltonian to the identifiers
     # in the new Hamiltonian
     pulse_identifier_mapping = {p: {identifier: identifier for identifier in identifiers[p]}
                                 for p in range(len(pulse_idx))}
     for identifier, oper in identifier_to_oper_mapping.items():
         identifier_str = all_identifiers[hashed_identifiers.index(identifier)]
@@ -1362,16 +1414,16 @@
         test = nan_mask.any(axis=1)
         for i, (concat_coeff, mask) in enumerate(zip(concat_coeffs[test], nan_mask[test])):
             nonnan_coeff = concat_coeff[~mask]
             if (nonnan_coeff == nonnan_coeff[0]).all():
                 # Constant value, use for empty segment
                 concat_coeffs[i, mask] = nonnan_coeff[0]
             else:
-                raise ValueError('Not all pulses have the same noise operators and ' +
-                                 'non-trivial noise sensitivities so I cannot infer them.')
+                raise ValueError('Not all pulses have the same noise operators and '
+                                 + 'non-trivial noise sensitivities so I cannot infer them.')
     else:
         concat_coeffs[np.isnan(concat_coeffs)] = 0
 
     return concat_opers, concat_identifiers, concat_coeffs[sort_idx], pulse_identifier_mapping
 
 
 def _merge_attrs(old_attrs: List[ndarray], new_attrs: List[ndarray], d_per_qubit: int,
@@ -1526,16 +1578,16 @@
     if not all(hasattr(pls, 'c_opers') for pls in pulses):
         # Do awkward checking for type
         raise TypeError('Can only concatenate PulseSequences!')
 
     # Check if the Hamiltonians' shapes are compatible, ie the set of all
     # shapes has length 1
     if len(set(pulse.c_opers.shape[1:] for pulse in pulses)) != 1:
-        raise ValueError('Trying to concatenate two PulseSequence ' +
-                         'instances with incompatible Hamiltonian shapes')
+        raise ValueError('Trying to concatenate two PulseSequence '
+                         + 'instances with incompatible Hamiltonian shapes')
 
     # Check if the bases are the same by hashing them and creating a set
     if not util.all_array_equal((pulse.basis for pulse in pulses)):
         raise ValueError('Trying to concatenate two PulseSequence instances with different bases!')
 
     basis = pulses[0].basis
     control_keys = ('c_opers', 'c_oper_identifiers', 'c_coeffs')
@@ -1671,19 +1723,19 @@
         else:
             cached_omega = [pls.is_cached('omega') for pls in pulses]
             equal_omega = util.all_array_equal((pls.omega
                                                 for pls in compress(pulses, cached_omega)))
 
         if not equal_omega:
             if calc_filter_function:
-                raise ValueError("Calculation of filter function forced  but not all pulses " +
-                                 "have the same frequencies cached and none were supplied!")
+                raise ValueError("Calculation of filter function forced  but not all pulses "
+                                 + "have the same frequencies cached and none were supplied!")
             if calc_pulse_correlation_FF:
-                raise ValueError("Cannot compute the pulse correlation filter functions; do not " +
-                                 "have the frequencies at which to evaluate.")
+                raise ValueError("Cannot compute the pulse correlation filter functions; do not "
+                                 + "have the frequencies at which to evaluate.")
 
             return newpulse
 
         if calc_filter_function is None:
             # compute filter function only if at least one pulse has a control
             # matrix cached
             if not equal_n_opers or not any(cached_ctrl_mat):
@@ -1703,16 +1755,16 @@
         # Cannot reuse atomic filter functions
         newpulse.cache_filter_function(omega, which=which)
         return newpulse
 
     # Get the phase factors at the correct times (the individual gate
     # durations) which are just the total phase factors of the pulses cumprod'd
     phases = np.array(
-        [np.ones_like(omega)] +
-        [pls.get_total_phases(omega) for pls in pulses[:-1]]
+        [np.ones_like(omega)]
+        + [pls.get_total_phases(omega) for pls in pulses[:-1]]
     ).cumprod(axis=0)
 
     # Get the transfer matrices for the individual gates
     N = len(newpulse.basis)
     L = np.empty((len(pulses), N, N))
     L[0] = np.identity(N)
     for i in range(1, len(pulses)):
@@ -1838,15 +1890,16 @@
     control_matrix_at = pulse.get_control_matrix(pulse.omega)
     total_propagator_liouville_at = pulse.total_propagator_liouville
 
     newpulse.total_propagator = nla.matrix_power(pulse.total_propagator, repeats)
     newpulse.cache_total_phases(pulse.omega)
 
     control_matrix_tot = numeric.calculate_control_matrix_periodic(phases_at, control_matrix_at,
-                                                                   total_propagator_liouville_at, repeats)
+                                                                   total_propagator_liouville_at,
+                                                                   repeats)
 
     newpulse.cache_filter_function(pulse.omega, control_matrix_tot)
 
     return newpulse
 
 
 def remap(pulse: PulseSequence, order: Sequence[int], d_per_qubit: int = 2,
@@ -1958,16 +2011,16 @@
     if pulse.is_cached('filter_function'):
         remapped_filter_function = pulse.get_filter_function(omega)[n_sort_idx[:, None],
                                                                     n_sort_idx[None, :]]
         remapped_pulse.cache_filter_function(omega, filter_function=remapped_filter_function)
 
     if pulse.is_cached('total_propagator_liouville') or pulse.is_cached('control_matrix'):
         if pulse.basis.btype != 'Pauli':
-            warn('pulse does not have a separable basis which is needed to ' +
-                 'retain cached control matrices.')
+            warn('pulse does not have a separable basis which is needed to '
+                 + 'retain cached control matrices.')
 
             return remapped_pulse
 
         perm = remap_pauli_basis_elements(order, N)[None, :]
         if pulse.is_cached('total_propagator_liouville'):
             remapped_pulse.total_propagator_liouville = np.empty_like(
                 pulse.total_propagator_liouville
@@ -2162,30 +2215,30 @@
                     # No need to remap
                     sorted_pulse = pulse
                 else:
                     # remap the pulse in the given order
                     try:
                         sorted_pulse = remap(pulse, order, d_per_qubit)
                     except ValueError as err:
-                        raise ValueError(f'Could not remap {repr(pulse)} mapped ' +
-                                         f'to qubits {qubit}. Do the dimensions match?') from err
+                        raise ValueError(f'Could not remap {repr(pulse)} mapped '
+                                         + f'to qubits {qubit}. Do the dimensions match?') from err
 
                 multi_qubit_idx.append(list(sorted_qubit))
                 multi_qubit_pulses.append(sorted_pulse)
                 multi_qubit_identifier_mappings.append(id_mapping)
         except TypeError:
             # qubit is not iterable, ie single qubit
             active_qubits_list.append(int(qubit))
             single_qubit_idx.append(int(qubit))
             single_qubit_pulses.append(pulse)
             single_qubit_identifier_mappings.append(id_mapping)
 
     if not all(pulse.d == d_per_qubit for pulse in single_qubit_pulses):
-        raise ValueError('Not all single-qubit pulses have dimension ' +
-                         f'd_per_qubit = {d_per_qubit}.')
+        raise ValueError('Not all single-qubit pulses have dimension '
+                         + f'd_per_qubit = {d_per_qubit}.')
 
     if not all(pulse.d == d_per_qubit**len(qubits)
                for pulse, qubits in zip(multi_qubit_pulses, multi_qubit_idx)):
         raise ValueError('Not all multi-qubit pulses have correct dimension!')
 
     # Get lists of pulses in deterministic order
     pulses = multi_qubit_pulses + single_qubit_pulses
@@ -2199,28 +2252,28 @@
         raise ValueError('Qubit clash: multiple pulses mapped to same qubit!')
 
     last_qubit = max(active_qubits)
     if N is None:
         N = last_qubit + 1
     else:
         if last_qubit + 1 > N:
-            raise ValueError('Number of qubits N smaller than highest qubit ' +
-                             f'index + 1 = {last_qubit + 1}')
+            raise ValueError('Number of qubits N smaller than highest qubit '
+                             + f'index + 1 = {last_qubit + 1}')
 
     if len(pulse_to_qubit_mapping) == 1:
         # return input pulse if not mapped to another qubit
         if multi_qubit_idx:
             if N == len(multi_qubit_idx[0]):
-                warn('Single multi-qubit pulse given and mapped to its ' +
-                     'original qubits. Returning the same.')
+                warn('Single multi-qubit pulse given and mapped to its '
+                     + 'original qubits. Returning the same.')
                 return multi_qubit_pulses[0]
         if single_qubit_idx:
             if N == 1:
-                warn('Single single-qubit pulse given and mapped to its ' +
-                     'original qubit. Returning the same.')
+                warn('Single single-qubit pulse given and mapped to its '
+                     + 'original qubit. Returning the same.')
                 return single_qubit_pulses[0]
 
     if cache_filter_function is not False:
         # Cache filter function of extended pulse if cached before for the same
         # frequencies
         is_cached = all(pulse.is_cached('control_matrix') for pulse in pulses)
 
@@ -2234,33 +2287,33 @@
             cache_filter_function = is_cached and equal_omega
             if cache_filter_function:
                 omega = pulses[0].omega
         else:
             # cache_filter_function == True
             if omega is None:
                 if not equal_omega:
-                    raise ValueError('Filter function should be cached but omega was not ' +
-                                     'provided and could not be inferred.')
+                    raise ValueError('Filter function should be cached but omega was not '
+                                     + 'provided and could not be inferred.')
 
                 omega = pulses[0].omega
 
     if cache_diagonalization is None:
         if cache_filter_function and additional_noise_Hamiltonian is not None:
             # Need the diagonalization
             cache_diagonalization = True
         else:
             # Extend propagators, eigenvalue and -vector arrays if calculated
             attrs = ('eigvals', 'eigvecs', 'propagators')
             cache_diagonalization = all(pulse.is_cached(attr)
                                         for attr in attrs
                                         for pulse in pulses)
-    elif (cache_diagonalization is False and
-          additional_noise_Hamiltonian is not None):
-        raise ValueError('Additional noise Hamiltonian given and ' +
-                         'cache_diagonalization set to False but required.')
+    elif (cache_diagonalization is False
+          and additional_noise_Hamiltonian is not None):
+        raise ValueError('Additional noise Hamiltonian given and '
+                         + 'cache_diagonalization set to False but required.')
 
     # Multi-qubit opers and coeffs
     all_qubits = {q for q in range(N)}
     d = d_per_qubit**N
     n_dt = len(pulses[0].dt)
     ID = np.identity(d_per_qubit)
 
@@ -2310,16 +2363,16 @@
     if additional_noise_Hamiltonian is not None:
         noise_args = _parse_Hamiltonian(
             additional_noise_Hamiltonian, len(pulses[0].dt), 'H_n'
         )
         add_n_opers, add_n_oper_id, add_n_coeffs = noise_args
 
         if add_n_opers.shape[1:] != (d, d):
-            raise ValueError(f'Expected additional noise operators to have dimensions {(d, d)}, ' +
-                             f'not {add_n_opers.shape[1:]}.')
+            raise ValueError(f'Expected additional noise operators to have dimensions {(d, d)}, '
+                             + f'not {add_n_opers.shape[1:]}.')
         if any(n_oper_id in n_oper_identifiers for n_oper_id in add_n_oper_id):
             identifiers = set(n_oper_identifiers).intersection(add_n_oper_id)
             raise ValueError(f'Found duplicate noise operator identifiers: {identifiers}')
 
         n_opers.extend(add_n_opers)
         n_coeffs.extend(add_n_coeffs)
         n_oper_identifiers.extend(add_n_oper_id)
@@ -2327,16 +2380,16 @@
     pulse_btypes = list(set(pulse.basis.btype for pulse in pulses))
     if not len(pulse_btypes) == 1:
         warn('Not all pulses had the same basis type. Cannot retain cached control matrices.')
         basis = Basis.ggm(d_per_qubit**N)
     else:
         btype = pulse_btypes[0]
         if btype == 'GGM':
-            warn('Original pulses had GGM basis which is not separable into ' +
-                 'a tensor product. Cannot retain cached control matrices.')
+            warn('Original pulses had GGM basis which is not separable into '
+                 + 'a tensor product. Cannot retain cached control matrices.')
             basis = Basis.ggm(d_per_qubit**N)
         elif btype == 'Pauli':
             basis = Basis.pauli(N)
         else:
             warn('Original pulses had custom basis which I cannot extend.')
             basis = Basis.ggm(d_per_qubit**N)
```

### Comparing `filter_functions-1.1.1/filter_functions/superoperator.py` & `filter_functions-1.1.2/filter_functions/superoperator.py`

 * *Files identical despite different names*

### Comparing `filter_functions-1.1.1/filter_functions/types.py` & `filter_functions-1.1.2/filter_functions/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,22 +22,24 @@
 Defines custom types for the package.
 """
 from typing import Mapping, Optional, Sequence, Tuple, Union
 
 from numpy import ndarray
 
 try:
+    import cycler
     from matplotlib import axes, colors, figure, legend
     from mpl_toolkits import axes_grid1
 
     Axes = axes.Axes
     Colormap = Union[colors.Colormap, str]
     Figure = figure.Figure
     Grid = axes_grid1.ImageGrid
     Legend = legend.Legend
+    Cycler = cycler.Cycler
     FigureAxes = Tuple[Figure, Axes]
     FigureAxesLegend = Tuple[Figure, Axes, Legend]
     FigureGrid = Tuple[Figure, Grid]
 except ImportError:
     pass
 
 try:
```

### Comparing `filter_functions-1.1.1/filter_functions/util.py` & `filter_functions-1.1.2/filter_functions/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
 """
 import functools
 import inspect
 import operator
 import string
 from itertools import zip_longest
-from typing import Callable, Dict, Iterable, List, Optional, Sequence, Tuple, Union
+from typing import Callable, Iterable, List, Optional, Sequence, Tuple, Union
 
 import numpy as np
 from numpy import ndarray
 
 from .types import Operator, State
 
 try:
@@ -148,15 +148,15 @@
     """
     out = np.empty(x.shape, dtype=np.complex128) if out is None else out
     out.real = np.cos(x, out=out.real, where=where)
     out.imag = np.sin(x, out=out.imag, where=where)
     return out
 
 
-def parse_optional_parameters(**allowed_kwargs: Dict[str, Sequence]) -> Callable:
+def parse_optional_parameters(**allowed_kwargs: Sequence) -> Callable:
     """Decorator factory to parse optional parameter with certain legal
     values.
 
     For ``allowed_kwargs = {name: allowed, ...}``: If the parameter
     value corresponding to ``name`` (either in args or kwargs of the
     decorated function) is not contained in ``allowed`` a ``ValueError``
     is raised.
@@ -169,22 +169,38 @@
                 idx = tuple(parameters).index(name)
                 try:
                     value = args[idx]
                 except IndexError:
                     value = kwargs.get(name, parameters[name].default)
 
                 if value not in allowed:
-                    raise ValueError(f"Invalid value for {name}: {value}. " +
-                                     f"Should be one of {allowed}.")
+                    raise ValueError(f"Invalid value for {name}: {value}. "
+                                     + f"Should be one of {allowed}.")
 
             return func(*args, **kwargs)
         return wrapper
     return decorator
 
 
+def parse_spectrum(spectrum: Sequence, omega: Sequence, idx: Sequence) -> ndarray:
+    error = 'Spectrum should be of shape {}, not {}.'
+    shape = (len(idx),)*(spectrum.ndim - 1) + (len(omega),)
+    try:
+        spectrum = np.broadcast_to(spectrum, shape)
+    except ValueError as broadcast_error:
+        raise ValueError(error.format(shape, spectrum.shape)) from broadcast_error
+
+    if spectrum.ndim == 3 and not np.allclose(spectrum, spectrum.conj().swapaxes(0, 1)):
+        raise ValueError('Cross-spectra given but not Hermitian along first two axes')
+    elif spectrum.ndim > 3:
+        raise ValueError(f'Expected spectrum to have < 4 dimensions, not {spectrum.ndim}')
+
+    return spectrum
+
+
 def parse_operators(opers: Sequence[Operator], err_loc: str) -> List[ndarray]:
     """Parse a sequence of operators and convert to ndarray.
 
     Parameters
     ----------
     opers: Sequence[Operator]
         Sequence of operators.
@@ -216,22 +232,24 @@
             parsed_opers.append(oper.todense())
         elif hasattr(oper, 'data') and hasattr(oper, 'dexp'):
             # qopt DenseMatrix
             parsed_opers.append(oper.data)
         else:
             raise TypeError(f'Expected operators in {err_loc} to be NumPy arrays or QuTiP Qobjs!')
 
+    parsed_opers = np.asarray(parsed_opers, dtype=complex)
+
     # Check correct dimensions of the operators
-    if set(oper.ndim for oper in parsed_opers) != {2}:
-        raise ValueError(f'Expected all operators in {err_loc} to be two-dimensional!')
+    if parsed_opers.ndim > 3:
+        raise ValueError(f'Expected operators in {err_loc} to be two-dimensional!')
 
-    if len(set(*set(oper.shape for oper in parsed_opers))) != 1:
+    if len(set(parsed_opers.shape[-2:])) != 1:
         raise ValueError(f'Expected operators in {err_loc} to be square!')
 
-    return np.asarray(parsed_opers)
+    return parsed_opers
 
 
 def _tensor_product_shape(shape_A: Sequence[int], shape_B: Sequence[int], rank: int):
     """Get shape of the tensor product between A and B of rank rank"""
     broadcast_shape = ()
     # Loop over dimensions from last to first, filling the 'shorter' shape
     # with 1's once it is exhausted
@@ -239,16 +257,16 @@
         if 1 in dims:
             # Broadcast 1-d of argument to dimension of other
             broadcast_shape = (max(dims),) + broadcast_shape
         elif len(set(dims)) == 1:
             # Both arguments have same dimension on axis.
             broadcast_shape = dims[:1] + broadcast_shape
         else:
-            raise ValueError(f'Incompatible shapes {shape_A} and {shape_B} ' +
-                             f'for tensor product of rank {rank}.')
+            raise ValueError(f'Incompatible shapes {shape_A} and {shape_B} '
+                             + f'for tensor product of rank {rank}.')
 
     # Shape of the actual tensor product is product of each dimension,
     # again broadcasting if need be
     tensor_shape = tuple(
         functools.reduce(operator.mul, dimensions)
         for dimensions in zip_longest(shape_A[:-rank-1:-1],
                                       shape_B[:-rank-1:-1],
@@ -287,16 +305,16 @@
         try:
             if isinstance(identifiers, str):
                 inds = np.array([identifier_to_index_table[identifiers]])
             else:
                 inds = np.array([identifier_to_index_table[identifier]
                                  for identifier in identifiers])
         except KeyError:
-            raise ValueError('Invalid identifiers given. All available ones ' +
-                             f'are: {all_identifiers}')
+            raise ValueError('Invalid identifiers given. All available ones '
+                             + f'are: {all_identifiers}')
 
     return inds
 
 
 def tensor(*args, rank: int = 2, optimize: Union[bool, str] = False) -> ndarray:
     """
     Fast, flexible tensor product using einsum. The product is taken
@@ -510,16 +528,16 @@
         if len(args) > 1:
             # Inserting all args at same position, perform their tensor product
             # using tensor and insert the result instead of iteratively insert
             # one by one
             args = (tensor(*args, rank=rank, optimize=optimize),)
     else:
         if not len(pos) == len(args):
-            raise ValueError('Expected pos to be either an int or a sequence of the same length ' +
-                             f'as the number of args, not length {len(pos)}')
+            raise ValueError('Expected pos to be either an int or a sequence of the same length '
+                             + f'as the number of args, not length {len(pos)}')
 
     _parse_dims_arg('arr', arr_dims, rank)
 
     def _tensor_insert_subscripts(ndim, pos, rank):
         """Get einsum string for the contraction"""
         ins_chars = string.ascii_letters[:rank]
         arr_chars = string.ascii_letters[rank:(ndim+1)*rank]
@@ -555,24 +573,24 @@
     ndim = len(arr_dims[0])
     divs, pos = zip(*[divmod(p, ndim) if p != ndim else (0, p) for p in pos])
     for i, (p, div, arg, arg_counter) in enumerate(sorted(
             zip_longest(pos, divs, args, range(len(args)), fillvalue=pos[0]),
             key=operator.itemgetter(0))):
 
         if div not in (-1, 0):
-            raise IndexError(f'Invalid position {cpos[i]} specified. Must ' +
-                             f'be between -{ndim} and {ndim}.')
+            raise IndexError(f'Invalid position {cpos[i]} specified. Must '
+                             + f'be between -{ndim} and {ndim}.')
 
         # Insert argument arg at position p+i (since every iteration the index
         # shifts by 1)
         try:
             result = single_tensor_insert(result, arg, carr_dims, p+i)
         except ValueError as err:
-            raise ValueError(f'Could not insert arg {arg_counter} with shape {result.shape} ' +
-                             f'into the array with shape {arg.shape} at position {p}.') from err
+            raise ValueError(f'Could not insert arg {arg_counter} with shape {result.shape} '
+                             + f'into the array with shape {arg.shape} at position {p}.') from err
 
         # Update arr_dims
         for axis, d in zip(carr_dims, arg.shape[-rank:]):
             axis.insert(p, d)
 
     return result
 
@@ -685,16 +703,16 @@
     for r in range(rank):
         arr_part = arr_chars[r*arr_ndim:(r+1)*arr_ndim]
         ins_part = ins_chars[r*ins_ndim:(r+1)*ins_ndim]
         for i, (p, ins_p) in enumerate(sorted(zip(pos, ins_part))):
             if p != arr_ndim:
                 div, p = divmod(p, arr_ndim)
                 if div not in (-1, 0):
-                    raise IndexError(f'Invalid position {pos[i]} specified. Must be between ' +
-                                     f'-{arr_ndim} and {arr_ndim}.')
+                    raise IndexError(f'Invalid position {pos[i]} specified. Must be between '
+                                     + f'-{arr_ndim} and {arr_ndim}.')
             arr_part = arr_part[:p+i] + ins_p + arr_part[p+i:]
 
         out_chars += arr_part
 
     subscripts = f'...{ins_chars},...{arr_chars}->...{out_chars}'
 
     outshape = _tensor_product_shape(ins.shape, arr.shape, rank)
@@ -703,21 +721,21 @@
     flat_arr_dims = [dim for axis in arr_dims for dim in axis]
     flat_ins_dims = [dim for axis in ins_dims for dim in axis]
 
     # Catch exceptions from wrong ins/arr_dims arguments
     try:
         ins_reshaped = ins.reshape(*ins.shape[:-rank], *flat_ins_dims)
     except ValueError as err:
-        raise ValueError('ins_dims not compatible with ins.shape[-rank:] = ' +
-                         f'{ins.shape[-rank:]}') from err
+        raise ValueError('ins_dims not compatible with ins.shape[-rank:] = '
+                         + f'{ins.shape[-rank:]}') from err
     try:
         arr_reshaped = arr.reshape(*arr.shape[:-rank], *flat_arr_dims)
     except ValueError as err:
-        raise ValueError('arr_dims not compatible with arr.shape[-rank:] = ' +
-                         f'{arr.shape[-rank:]}') from err
+        raise ValueError('arr_dims not compatible with arr.shape[-rank:] = '
+                         + f'{arr.shape[-rank:]}') from err
 
     result = np.einsum(subscripts, ins_reshaped, arr_reshaped, optimize=optimize).reshape(outshape)
 
     return result
 
 
 def tensor_transpose(arr: ndarray, order: Sequence[int], arr_dims: Sequence[Sequence[int]],
@@ -770,36 +788,36 @@
     tensor_merge: Merge tensor product chains.
     """
     _parse_dims_arg('arr', arr_dims, rank)
 
     ndim = len(arr_dims[0])
     # Number of axes that are broadcast over
     n_broadcast = len(arr.shape[:-rank])
-    transpose_axes = ([i for i in range(n_broadcast)] +
-                      [n_broadcast + r*ndim + o for r in range(rank) for o in order])
+    transpose_axes = ([i for i in range(n_broadcast)]
+                      + [n_broadcast + r*ndim + o for r in range(rank) for o in order])
 
     # Need to reshape arr to the rank*ndim-dimensional shape that's the
     # output of the regular tensor einsum call
     flat_arr_dims = [dim for axis in arr_dims for dim in axis]
 
     # Catch exceptions from wrong arr_dims argument
     try:
         arr_reshaped = arr.reshape(*arr.shape[:-rank], *flat_arr_dims)
     except ValueError as err:
-        raise ValueError('arr_dims not compatible with arr.shape[-rank:] = ' +
-                         f'{arr.shape[-rank:]}') from err
+        raise ValueError('arr_dims not compatible with arr.shape[-rank:] = '
+                         + f'{arr.shape[-rank:]}') from err
 
     try:
         result = arr_reshaped.transpose(*transpose_axes).reshape(arr.shape)
     except TypeError as type_err:
-        raise TypeError("Could not transpose the order. Are all elements of " +
-                        "'order' integers?") from type_err
+        raise TypeError("Could not transpose the order. Are all elements of "
+                        + "'order' integers?") from type_err
     except ValueError as val_err:
-        raise ValueError("Could not transpose the order. Are all elements " +
-                         "of 'order' unique and match the array?") from val_err
+        raise ValueError("Could not transpose the order. Are all elements "
+                         + "of 'order' unique and match the array?") from val_err
 
     return result
 
 
 def mdot(arr: Sequence, axis: int = 0) -> ndarray:
     """Multiple matrix products along axis"""
     return functools.reduce(np.matmul, np.swapaxes(arr, 0, axis))
@@ -901,16 +919,16 @@
     # Convert qutip.Qobj's to numpy arrays
     psi, phi = [obj.full() if hasattr(obj, 'full') else obj for obj in (psi, phi)]
     psi, phi = np.atleast_2d(psi, phi)
 
     if eps is None:
         # Tolerance the floating point eps times the # of flops for the matrix
         # multiplication, i.e. for psi and phi n x m matrices 2*n**2*m
-        eps = (max(np.finfo(psi.dtype).eps, np.finfo(phi.dtype).eps) *
-               np.prod(psi.shape)*phi.shape[-1]*2)
+        eps = (max(np.finfo(psi.dtype).eps, np.finfo(phi.dtype).eps)
+               * np.prod(psi.shape)*phi.shape[-1]*2)
         if not normalized:
             # normalization introduces more floating point error
             eps *= (np.prod(psi.shape[-2:])*phi.shape[-1]*2)**2
 
     try:
         # Don't need to round at this point
         inner_product = dot_HS(psi, phi, eps=0)
@@ -924,15 +942,16 @@
 
     phase = np.angle(inner_product)
     modulus = abs(inner_product)
 
     return abs(norm - modulus) <= eps, phase
 
 
-def dot_HS(U: Operator, V: Operator, eps: Optional[float] = None) -> float:
+def dot_HS(U: Operator, V: Operator, eps: Optional[float] = None) -> Union[float, complex,
+                                                                           ndarray]:
     r"""Return the Hilbert-Schmidt inner product of U and V,
 
     .. math::
         \langle U, V\rangle_\mathrm{HS} := \mathrm{tr}(U^\dagger V).
 
     Parameters
     ----------
@@ -976,18 +995,19 @@
         res = np.around(np.einsum('...ij,...ij', U.conj(), V), decimals=abs(int(np.log10(eps))))
 
     return res if res.imag.any() else res.real
 
 
 @parse_optional_parameters(spacing=('log', 'linear'))
 def get_sample_frequencies(pulse: 'PulseSequence', n_samples: int = 300, spacing: str = 'log',
-                           include_quasistatic: bool = False) -> ndarray:
-    """Get *n_samples* sample frequencies spaced 'linear' or 'log'.
+                           include_quasistatic: bool = False, omega_min: Optional[float] = None,
+                           omega_max: Optional[float] = None) -> ndarray:
+    r"""Get *n_samples* sample frequencies spaced 'linear' or 'log'.
 
-    The ultraviolet cutoff is taken to be two orders of magnitude larger
+    The ultraviolet cutoff is taken to be one order of magnitude larger
     than the timescale of the pulse tau. In the case of log spacing, the
     values are clipped in the infrared at two orders of magnitude below
     the timescale of the pulse.
 
     Parameters
     ----------
     pulse: PulseSequence
@@ -995,33 +1015,32 @@
     n_samples: int, optional
         The number of frequency samples. Default is 300.
     spacing: str, optional
         The spacing of the frequencies. Either 'log' or 'linear',
         default is 'log'.
     include_quasistatic: bool, optional
         Include zero frequency. Default is False.
+    omega_min, omega_max: float, optional
+        Minimum and maximum angular frequencies included (DC
+        notwithstanding). Default to :math:`2\pi\times 10^{-2}/\tau` and
+        :math:`2\pi\times 10^{+1}/\Delta t_{\mathrm{min}}`.
 
     Returns
     -------
     omega: ndarray
-        The frequencies.
+        The angular frequencies.
     """
-    if spacing == 'linear':
-        xspace = np.linspace
-    else:
-        # spacing == 'log'
-        xspace = np.geomspace
+    xspace = np.geomspace if spacing == 'log' else np.linspace
+    omega_min = 2*np.pi*1e-2/pulse.tau if omega_min is None else omega_min
+    omega_max = 2*np.pi*1e+1/pulse.dt.min() if omega_max is None else omega_max
+    omega = xspace(omega_min, omega_max, n_samples - include_quasistatic)
 
     if include_quasistatic:
-        freqs = xspace(1e-2/pulse.tau, 1e2/pulse.tau, n_samples - 1)
-        freqs = np.insert(freqs, 0, 0)
-    else:
-        freqs = xspace(1e-2/pulse.tau, 1e2/pulse.tau, n_samples)
-
-    return 2*np.pi*freqs
+        return np.insert(omega, 0, 0)
+    return omega
 
 
 def hash_array_along_axis(arr: ndarray, axis: int = 0) -> List[int]:
     """Return the hashes of arr along the first axis"""
     return [hash(arr.tobytes()) for arr in np.swapaxes(arr, 0, axis)]
 
 
@@ -1060,18 +1079,16 @@
 
     Returns
     -------
     it: Iterator
         Range iterator dressed with a progressbar if
         ``show_progressbar=True``.
     """
-    if show_progressbar:
-        return progressbar(range(*args), **kwargs)
-
-    return range(*args)
+    return progressbar(range(*args), disable=kwargs.pop('disable', not show_progressbar),
+                       **kwargs)
 
 
 class CalculationError(Exception):
     """Indicates a quantity could not be computed."""
 
     def __init__(self, message: str) -> None:
         super().__init__(message)
```

### Comparing `filter_functions-1.1.1/filter_functions.egg-info/PKG-INFO` & `filter_functions-1.1.2/filter_functions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filter-functions
-Version: 1.1.1
+Version: 1.1.2
 Summary: Package for efficient calculation of generalized filter functions
 Home-page: https://github.com/qutech/filter_functions
 Author: Quantum Technology Group, RWTH Aachen University
 Author-email: tobias.hangleiter@rwth-aachen.de
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `filter_functions-1.1.1/filter_functions.egg-info/SOURCES.txt` & `filter_functions-1.1.2/filter_functions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `filter_functions-1.1.1/setup.py` & `filter_functions-1.1.2/setup.py`

 * *Files identical despite different names*

