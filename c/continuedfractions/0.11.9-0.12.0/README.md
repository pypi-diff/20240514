# Comparing `tmp/continuedfractions-0.11.9.tar.gz` & `tmp/continuedfractions-0.12.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "continuedfractions-0.11.9.tar", last modified: Wed Mar 13 17:14:39 2024, max compression
+gzip compressed data, was "continuedfractions-0.12.0.tar", last modified: Tue May 14 16:34:51 2024, max compression
```

## Comparing `continuedfractions-0.11.9.tar` & `continuedfractions-0.12.0.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0    16725 2024-02-18 16:26:08.292887 continuedfractions-0.11.9/LICENSE
--rw-r--r--   0        0        0    16725 2024-02-18 16:26:08.292887 continuedfractions-0.11.9/LICENSE
--rw-r--r--   0        0        0     2373 2024-03-11 09:44:12.799400 continuedfractions-0.11.9/README.md
--rw-r--r--   0        0        0     2373 2024-03-11 09:44:12.799400 continuedfractions-0.11.9/README.md
--rw-r--r--   0        0        0     3367 2024-03-13 17:14:39.962031 continuedfractions-0.11.9/pyproject.toml
--rw-r--r--   0        0        0    26842 2024-03-11 21:09:01.173920 continuedfractions-0.11.9/src/continuedfractions/continuedfraction.py
--rw-r--r--   0        0        0    12656 2024-03-13 09:49:11.510796 continuedfractions-0.11.9/src/continuedfractions/lib.py
--rw-r--r--   0        0        0       23 2024-03-13 16:50:36.027926 continuedfractions-0.11.9/src/continuedfractions/version.py
--rw-r--r--   0        0        0    23285 1970-01-01 00:00:00.000000 continuedfractions-0.11.9/PKG-INFO
+-rw-r--r--   0        0        0    16725 2024-02-18 16:26:08.292887 continuedfractions-0.12.0/LICENSE
+-rw-r--r--   0        0        0    16725 2024-02-18 16:26:08.292887 continuedfractions-0.12.0/LICENSE
+-rw-r--r--   0        0        0     3162 2024-05-14 16:22:41.742134 continuedfractions-0.12.0/README.md
+-rw-r--r--   0        0        0     3162 2024-05-14 16:22:41.742134 continuedfractions-0.12.0/README.md
+-rw-r--r--   0        0        0     3506 2024-05-14 16:34:51.929492 continuedfractions-0.12.0/pyproject.toml
+-rw-r--r--   0        0        0    31312 2024-03-28 15:58:08.840824 continuedfractions-0.12.0/src/continuedfractions/continuedfraction.py
+-rw-r--r--   0        0        0    15791 2024-03-28 16:02:15.530704 continuedfractions-0.12.0/src/continuedfractions/lib.py
+-rw-r--r--   0        0        0    40644 2024-05-14 15:35:07.292234 continuedfractions-0.12.0/src/continuedfractions/sequences.py
+-rw-r--r--   0        0        0     2077 2024-04-15 22:05:26.859297 continuedfractions-0.12.0/src/continuedfractions/utils.py
+-rw-r--r--   0        0        0       23 2024-04-12 12:56:49.382276 continuedfractions-0.12.0/src/continuedfractions/version.py
+-rw-r--r--   0        0        0    24146 1970-01-01 00:00:00.000000 continuedfractions-0.12.0/PKG-INFO
```

### Comparing `continuedfractions-0.11.9/LICENSE` & `continuedfractions-0.12.0/LICENSE`

 * *Files identical despite different names*

### Comparing `continuedfractions-0.11.9/README.md` & `continuedfractions-0.12.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,41 @@
 <div align="center">
   
 [![CI](https://github.com/sr-murthy/continuedfractions/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/sr-murthy/continuedfractions/actions/workflows/ci.yml)
+[![CodeQL Analysis](https://github.com/sr-murthy/continuedfractions/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/sr-murthy/continuedfractions/actions/workflows/codeql-analysis.yml)
 [![Codecov](https://codecov.io/gh/sr-murthy/continuedfractions/graph/badge.svg?token=GWQ08T4P5J)](https://codecov.io/gh/sr-murthy/continuedfractions)
-[![PyPI version](https://badge.fury.io/py/continuedfractions.svg)](https://badge.fury.io/py/continuedfractions)
 [![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm-project.org)
 [![License: MPL
 2.0](https://img.shields.io/badge/License-MPL_2.0-brightgreen.svg)](https://opensource.org/licenses/MPL-2.0)
 [![Docs](https://readthedocs.org/projects/continuedfractions/badge/?version=latest)](https://continuedfractions.readthedocs.io/en/latest/?badge=latest)
 <a href="https://trackgit.com">
 <img src="https://us-central1-trackgit-analytics.cloudfunctions.net/token/ping/lsudelfvcxb7f1xm6i4l" alt="trackgit-views" />
 </a>
+[![PyPI version](https://badge.fury.io/py/continuedfractions.svg)](https://badge.fury.io/py/continuedfractions)
 [![Downloads](https://static.pepy.tech/badge/continuedfractions/week)](https://pepy.tech/project/continuedfractions)
 
 </div>
 
 # continuedfractions
 
 A simple extension of the Python [`fractions`](https://docs.python.org/3/library/fractions.html) standard library for working with [continued fractions](https://en.wikipedia.org/wiki/Continued_fraction) as Python objects.
 
+The [PyPI package](https://pypi.org/project/continuedfractions/) only uses standard libraries and can be installed on any **Linux**, **Mac OS** or **Windows** system supporting **Python 3.10**, **3.11**, or **3.12**.
+```shell
+pip install continuedfractions
+```
+
+See the [project docs](https://continuedfractions.readthedocs.io/en/latest/) for more details, which includes the [API reference](https://continuedfractions.readthedocs.io/en/latest/sources/api-reference.html).
+
 [Continued fractions](https://en.wikipedia.org/wiki/Continued_fraction) are beautiful and interesting mathematical objects, with many connections in [number theory](https://en.wikipedia.org/wiki/Number_theory) and also very useful practical applications, including the [rational approximation of real numbers](https://en.wikipedia.org/wiki/Continued_fraction#Best_rational_approximations).
 
 The `continuedfractions` package is designed to:
 
-* make it easy to construct (finite) continued fractions as Python objects
+* make it easy to work with (finite) continued fractions as Python objects
 * explore their key properties, such as elements/coefficients, convergents, segments, remainders, and others
 * operate on them as rationals and instances of the standard library [`fractions.Fraction`](https://docs.python.org/3/library/fractions.html#fractions.Fraction) class
+* support approximations and experimental computations for irrational numbers
+* explore other objects related to continued fractions, such as mediants, sequences of coprime integers, and Farey sequences
 
 The project is [licensed](LICENSE) under the [Mozilla Public License 2.0](https://opensource.org/licenses/MPL-2.0).
 
-See the [project docs](https://continuedfractions.readthedocs.io/en/latest) for more details.
+
```

#### html2text {}

```diff
@@ -1,30 +1,41 @@
    [![CI](https://github.com/sr-murthy/continuedfractions/actions/workflows/
 ci.yml/badge.svg?branch=main)](https://github.com/sr-murthy/continuedfractions/
-    actions/workflows/ci.yml) [![Codecov](https://codecov.io/gh/sr-murthy/
-continuedfractions/graph/badge.svg?token=GWQ08T4P5J)](https://codecov.io/gh/sr-
-     murthy/continuedfractions) [![PyPI version](https://badge.fury.io/py/
- continuedfractions.svg)](https://badge.fury.io/py/continuedfractions) [![pdm-
-  managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm-
-project.org) [![License: MPL 2.0](https://img.shields.io/badge/License-MPL_2.0-
- brightgreen.svg)](https://opensource.org/licenses/MPL-2.0) [![Docs](https://
- readthedocs.org/projects/continuedfractions/badge/?version=latest)](https://
- continuedfractions.readthedocs.io/en/latest/?badge=latest) _[_t_r_a_c_k_g_i_t_-_v_i_e_w_s_][!
+  actions/workflows/ci.yml) [![CodeQL Analysis](https://github.com/sr-murthy/
+ continuedfractions/actions/workflows/codeql-analysis.yml/badge.svg)](https://
+github.com/sr-murthy/continuedfractions/actions/workflows/codeql-analysis.yml)
+     [![Codecov](https://codecov.io/gh/sr-murthy/continuedfractions/graph/
+         badge.svg?token=GWQ08T4P5J)](https://codecov.io/gh/sr-murthy/
+ continuedfractions) [![pdm-managed](https://img.shields.io/badge/pdm-managed-
+      blueviolet)](https://pdm-project.org) [![License: MPL 2.0](https://
+img.shields.io/badge/License-MPL_2.0-brightgreen.svg)](https://opensource.org/
+licenses/MPL-2.0) [![Docs](https://readthedocs.org/projects/continuedfractions/
+ badge/?version=latest)](https://continuedfractions.readthedocs.io/en/latest/
+   ?badge=latest) _[_t_r_a_c_k_g_i_t_-_v_i_e_w_s_][![PyPI version](https://badge.fury.io/py/
+   continuedfractions.svg)](https://badge.fury.io/py/continuedfractions) [!
  [Downloads](https://static.pepy.tech/badge/continuedfractions/week)](https://
                      pepy.tech/project/continuedfractions)
 # continuedfractions A simple extension of the Python [`fractions`](https://
 docs.python.org/3/library/fractions.html) standard library for working with
 [continued fractions](https://en.wikipedia.org/wiki/Continued_fraction) as
-Python objects. [Continued fractions](https://en.wikipedia.org/wiki/
-Continued_fraction) are beautiful and interesting mathematical objects, with
-many connections in [number theory](https://en.wikipedia.org/wiki/
+Python objects. The [PyPI package](https://pypi.org/project/continuedfractions/
+) only uses standard libraries and can be installed on any **Linux**, **Mac
+OS** or **Windows** system supporting **Python 3.10**, **3.11**, or **3.12**.
+```shell pip install continuedfractions ``` See the [project docs](https://
+continuedfractions.readthedocs.io/en/latest/) for more details, which includes
+the [API reference](https://continuedfractions.readthedocs.io/en/latest/
+sources/api-reference.html). [Continued fractions](https://en.wikipedia.org/
+wiki/Continued_fraction) are beautiful and interesting mathematical objects,
+with many connections in [number theory](https://en.wikipedia.org/wiki/
 Number_theory) and also very useful practical applications, including the
 [rational approximation of real numbers](https://en.wikipedia.org/wiki/
 Continued_fraction#Best_rational_approximations). The `continuedfractions`
-package is designed to: * make it easy to construct (finite) continued
+package is designed to: * make it easy to work with (finite) continued
 fractions as Python objects * explore their key properties, such as elements/
 coefficients, convergents, segments, remainders, and others * operate on them
 as rationals and instances of the standard library [`fractions.Fraction`]
-(https://docs.python.org/3/library/fractions.html#fractions.Fraction) class The
-project is [licensed](LICENSE) under the [Mozilla Public License 2.0](https://
-opensource.org/licenses/MPL-2.0). See the [project docs](https://
-continuedfractions.readthedocs.io/en/latest) for more details.
+(https://docs.python.org/3/library/fractions.html#fractions.Fraction) class *
+support approximations and experimental computations for irrational numbers *
+explore other objects related to continued fractions, such as mediants,
+sequences of coprime integers, and Farey sequences The project is [licensed]
+(LICENSE) under the [Mozilla Public License 2.0](https://opensource.org/
+licenses/MPL-2.0).
```

### Comparing `continuedfractions-0.11.9/pyproject.toml` & `continuedfractions-0.12.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,59 @@
 [project]
 name = "continuedfractions"
-description = "Continued fractions with Python"
+description = "Object-oriented continued fractions with Python."
 authors = [
     { name = "S. R. Murthy", email = "s.murthy@tutanota.com" },
 ]
 maintainers = [
     { name = "S. R. Murthy", email = "s.murthy@tutanota.com" },
 ]
 dynamic = []
 requires-python = ">=3.10"
 dependencies = []
 readme = "README.md"
 keywords = [
+    "computational number theory",
+    "coprime integers",
     "continued fractions",
+    "farey sequences",
+    "irrational numbers",
+    "mediants",
+    "number theory",
+    "rational approximation",
     "rational numbers",
     "real numbers",
-    "irrational numbers",
-    "approximation",
 ]
 classifiers = [
-    "Development Status :: 4 - Beta",
     "Environment :: Console",
     "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Development Status :: 5 - Production/Stable",
     "Operating System :: POSIX :: Linux",
     "Operating System :: MacOS",
     "Operating System :: Microsoft :: Windows",
 ]
-version = "0.11.9"
+version = "0.12.0"
 
 [project.license]
 file = "LICENSE"
 
 [project.optional-dependencies]
 user = [
     "jupyter",
 ]
 
 [project.scripts]
 
 [project.urls]
 Homepage = "https://github.com/sr-murthy/continuedfractions"
-Documentation = "https://continuedfractions.readthedocs.io/en/latest"
+Documentation = "https://continuedfractions.readthedocs.io/en/latest/"
 Repository = "https://github.com/sr-murthy/continuedfractions"
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
@@ -84,14 +88,15 @@
 ]
 dev = [
     "ipython",
     "ipdb",
     "virtualenv",
 ]
 docs = [
+    "myst-parser",
     "pydata-sphinx-theme",
     "Sphinx",
     "sphinx-autobuild",
     "sphinx-copybutton",
     "pylint>=2.17.5",
     "nb2plots>=0.7.1",
     "sphinx-gallery>=0.14.0",
@@ -103,23 +108,24 @@
     "ruff",
 ]
 test = [
     "coverage[toml]",
     "pytest",
     "pytest-cov",
     "pytest-xdist",
+    "sympy",
 ]
 tox = []
 deploy = [
     "twine>=4.0.2",
 ]
 
 [tool.pdm.scripts.lint]
 shell = "make lint"
-help = "Linting code with Ruff"
+help = "Lint source with Ruff"
 
 [tool.pdm.scripts.doctests]
 shell = "make doctests"
 help = "Run doctests"
 
 [tool.pdm.scripts.unittests]
 shell = "make unittests"
```

### Comparing `continuedfractions-0.11.9/src/continuedfractions/continuedfraction.py` & `continuedfractions-0.12.0/src/continuedfractions/continuedfraction.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,114 +1,78 @@
+from __future__ import annotations
+
+
 __all__ = [
     'ContinuedFraction',
 ]
 
 
 # -- IMPORTS --
 
 # -- Standard libraries --
-import math
+import decimal
+import functools
 import statistics
 import sys
 
 from decimal import Decimal
-from fractions import Fraction, _RATIONAL_FORMAT
-from functools import partial
+from fractions import Fraction
 from pathlib import Path
 from types import MappingProxyType
 from typing import Any
 
 # -- 3rd party libraries --
 
 # -- Internal libraries --
 sys.path.insert(0, str(Path(__file__).parent.parent))
 
 from continuedfractions.lib import (
     continued_fraction_rational,
-    continued_fraction_real,
-    fraction_from_elements,
     convergent,
-    mediant,
+    fraction_from_elements,
+    left_mediant,
+    right_mediant,
 )
 
 
 class ContinuedFraction(Fraction):
-    """
-    A simple implementation of continued fractions as Python objects and
-    instances of the standard library ``fractions.Fraction`` class, with
+    """An object-oriented representation of a (finite) simple continued fraction.
+
+    An implementation of simple continued fractions as Python objects and
+    instances of the standard library :py:class:`fractions.Fraction` class, with
     various properties for the continued fraction, including its elements
-    (or coefficients), the order, convergents, segments, and remainders.
+    (or coefficients), the order, convergents, and remainders.
 
-    Attributes
-    ----------
-    elements : tuple[int]
-        The ordered sequence of elements of the continued fraction.
-
-    order : int
-        The order of the continued fraction, defined as the number of
-        elements - 1.
-
-    khinchin_mean : decimal.Decimal
-        The geometric mean of all elements of the continued fraction, starting
-        from ``a_1``, excluding the leading element ``a_0``.
-
-    convergents : types.MappingProxyType[int, Fraction]
-        An immutable map of all the `k`-order convergents of the continued
-        fraction, keyed by `k`.
-
-    Methods
-    -------
-    as_float()
-        The `float` value of the fraction, as given by standard division of
-        the numerator by the denominator.
-
-    segment(k: int)
-        The `k`th segment of the continued fraction, defined as the continued
-        fraction given by its `k`-order convergent, whose elements consist of
-        the first `k + 1` two elements of the original continued fraction.
-
-    remainder(k: int)
-        The `k`th remainder of the continued fraction, defined as the continued
-        fraction given by the difference between the original continued
-        fraction and its `(k - 1)`-order convergent (equivalently, the
-        `(k - 1)` order segment, as defined above).
-
-    mediant(other: Fraction)
-        The continued fraction of the rational number formed by taking the
-        pairwise sum of the numerators and denominators of the original
-        continued fraction and a second fraction (`other`). The resulting
-        fraction has the property that its value lies between the two
-        constituents.
+    The term "simple continued fraction" denotes a specific type of continued
+    fraction where the fractional terms only have numerators of :math:`1`.
 
     Examples
     --------
     Construct the continued fraction for the rational `649/200`.
 
     >>> cf = ContinuedFraction(649, 200)
     >>> cf
     ContinuedFraction(649, 200)
     >>> cf.as_float()
     3.245
 
-    Inspect the elements, order, convergents, segments and remainders
+    Inspect the elements, order, convergents, and remainders.
 
     >>> cf.elements
     (3, 4, 12, 4)
     >>> cf.order
     3
-    >>> cf.convergents
-    mappingproxy({0: Fraction(3, 1), 1: Fraction(13, 4), 2: Fraction(159, 49), 3: Fraction(649, 200)})
-    >>> cf.segment(1)
-    ContinuedFraction(13, 4)
-    >>> cf.remainder(1)
-    ContinuedFraction(200, 49)
+    >>> cf.convergent(0), cf.convergent(1), cf.convergent(2), cf.convergent(3)
+    (ContinuedFraction(3, 1), ContinuedFraction(13, 4), ContinuedFraction(159, 49), ContinuedFraction(649, 200))
+    >>> cf.remainder(0), cf.remainder(1), cf.remainder(2), cf.remainder(3)
+    (ContinuedFraction(649, 200), ContinuedFraction(200, 49), ContinuedFraction(49, 4), ContinuedFraction(4, 1))
 
-    Check some properties of the segments and remainders
+    Check some properties of the convergents and remainders.
 
-    >>> assert cf.remainder(1) == 1 / (cf - cf.convergents[0])
+    >>> assert cf.remainder(1) == 1 / (cf - cf.convergent(0))
 
     Construct continued fractions from element sequences.
 
     >>> cf_inverse = ContinuedFraction.from_elements(0, 3, 4, 12, 4)
     >>> cf_inverse
     ContinuedFraction(200, 649)
     >>> assert cf_inverse == 1/cf
@@ -116,636 +80,764 @@
     >>> cf_negative_inverse = ContinuedFraction.from_elements(-1, 1, 2, 4, 12, 4)
     >>> cf_negative_inverse
     ContinuedFraction(-200, 649)
     >>> assert cf_negative_inverse == -1/cf
     >>> assert cf * cf_negative_inverse == -1
     """
 
-    # Class attribute to store an error message for input errors
-    __valid_inputs_msg__ = (
-        "Only single integers, non-nan floats, numeric strings, \n"
-        "`fractions.Fraction`, or `decimal.Decimal` objects; or two \n"
-        "integers or two `fractions.Fraction` objects or a pairwise \n"
-        "combination of these, representing the numerator and non-zero \n"
-        "denominator, respectively, of a rational fraction, are valid."
-    )
-
-    @classmethod
-    def validate(cls, *args: int | float | str | Fraction | Decimal, **kwargs: Any) -> None:
-        """
-        Checks whether the arguments are one of the following types:
-
-        * a single integer or a non-nan float
-        * a single numeric string
-        * a single `fractions.Fraction` or `decimal.Decimal` object
-        * two integers or `fractions.Fraction` objects, or a combination of an
-          integer and a `fractions.Fraction` object, representing the numerator
-          and non-zero denominator of a rational fraction
-
-        Parameters
-        ----------
-        *args: int or float or str or fractions.Fraction or decimal.Decimal
-            Arguments of the type described above.
-
-        Raises
-        ------
-        ValueError
-            If validation fails.
+    # Slots - ATM only ``_elements`` to store the continued fraction elements sequence
+    __slots__ = ['_elements',]
 
-        Notes
-        -----
-        To avoid recursion errors validation excludes `ContinuedFraction`
-        instances, and for the same reason convergents of a
-        `ContinuedFraction` instance are given as `fractions.Fraction`
-        instances.
-
-        Examples
-        --------
-        >>> ContinuedFraction.validate(100)
-        >>> ContinuedFraction.validate(3, -2)
-
-        >>> ContinuedFraction.validate(1, -2.0)
-        Traceback (most recent call last):
-        ...
-        ValueError: Only single integers, non-nan floats, numeric strings, 
-        `fractions.Fraction`, or `decimal.Decimal` objects; or two 
-        integers or two `fractions.Fraction` objects or a pairwise 
-        combination of these, representing the numerator and non-zero 
-        denominator, respectively, of a rational fraction, are valid.
-
-        >>> ContinuedFraction.validate(-.123456789)
-        >>> ContinuedFraction.validate('-.123456789')
-        >>> ContinuedFraction.validate('-649/200')
-        >>> ContinuedFraction.validate(-3/2)
-
-        >>> ContinuedFraction.validate(-3, 0)
-        Traceback (most recent call last):
-        ...
-        ValueError: Only single integers, non-nan floats, numeric strings, 
-        `fractions.Fraction`, or `decimal.Decimal` objects; or two 
-        integers or two `fractions.Fraction` objects or a pairwise 
-        combination of these, representing the numerator and non-zero 
-        denominator, respectively, of a rational fraction, are valid.
-
-        >>> ContinuedFraction.validate(Fraction(-415, 93))
-        >>> ContinuedFraction.validate(Decimal('12345.6789'))
-        >>> ContinuedFraction.validate(Decimal(12345.6789))
-
-        >>> ContinuedFraction.validate(Fraction(3, 2), 2.5)
-        Traceback (most recent call last):
-        ...
-        ValueError: Only single integers, non-nan floats, numeric strings, 
-        `fractions.Fraction`, or `decimal.Decimal` objects; or two 
-        integers or two `fractions.Fraction` objects or a pairwise 
-        combination of these, representing the numerator and non-zero 
-        denominator, respectively, of a rational fraction, are valid.
-        """
-        if len(args) not in [1, 2]:
-            raise ValueError(cls.__valid_inputs_msg__)
-
-        if (
-            len(args) == 1 and
-            not set(map(type, args)).issubset(
-                [int, float, str, Fraction, Decimal]
-            )
-        ):
-            raise ValueError(cls.__valid_inputs_msg__)
-
-        if any(isinstance(arg, float) and math.isnan(arg) for arg in args):
-            raise ValueError(cls.__valid_inputs_msg__)
-
-        if len(args) == 1 and isinstance(args[0], str) and not _RATIONAL_FORMAT.match(args[0]):
-            raise ValueError(cls.__valid_inputs_msg__)
-
-        if len(args) == 2 and not set(map(type, args)).issubset([int, Fraction]):
-            raise ValueError(cls.__valid_inputs_msg__)
-
-        if len(args) == 2 and args[1] == 0:
-            raise ValueError(cls.__valid_inputs_msg__)
-
-    def __new__(cls, *args:  int | float | str | Fraction | Decimal, **kwargs: Any) -> Fraction:
-        """
-        Creates instances of this class, which represent finite, simple
-        continued fractions.
-
-        Arguments must be one of the following types:
-
-        * a single integer or a non-nan float
-        * a single numeric string
-        * a single `fractions.Fraction` or `decimal.Decimal` object
-        * two integers or `fractions.Fraction` objects, or a combination of an
-          integer and a `fractions.Fraction` object, representing the numerator
-          and non-zero denominator of a rational fraction
-
-        Parameters
-        ----------
-        *args: int or float or str or fractions.Fraction or decimal.Decimal
-            Arguments of the type described above.
-
-        **kwargs
-            Any valid keyword arguments for the superclass
-            `fractions.Fraction`.
+    # Declare all instances to have an ``_elements`` attribute, which must be
+    # a ``tuple`` of ``int``s.
+    _elements: tuple[int]
+
+    def __new__(cls, *args: Any, **kwargs: Any) -> ContinuedFraction:
+        """Creates, initialises and returns instances of this class.
+
+        Arguments can be any which are valid for creating objects of the
+        :py:class:`fractions.Fraction` superclass.
+
+        For clarification, valid arguments can be one of the following:
+
+        * a single instance of :py:class:`numbers.Rational`, including
+          :py:class:`int`, :py:class:`fractions.Fraction` or
+          :py:class:`ContinuedFraction`, named or unnamed
+        * a pair of  :py:class:`numbers.Rational` instances, including
+          :py:class:`int`, :py:class:`fractions.Fraction` and
+          :py:class:`ContinuedFraction`, named or unnamed
+        * a single :py:class:`float` or :py:class:`decimal.Decimal` value
+          that is not a special value such as :py:data:`math.nan`,
+          ``float('inf')``, or ``Decimal('infinity')``
+        * a single numeric valid string (:py:class:`str`) - validity is
+          determined in the superclass by the
+          :py:data:`fractions._RATIONAL_FORMAT` test
 
         Returns
         -------
         ContinuedFraction
-            A new instance of `ContinuedFraction`, but not yet initialised with
-            the class-specific attributes and properties.
+            A full instance of :py:class:`ContinuedFraction`.
 
         Examples
         --------
-        >>> ContinuedFraction(100, 2)
-        ContinuedFraction(50, 1)
-
-        >>> ContinuedFraction(1, -2.0)
-        Traceback (most recent call last):
-        ...
-        ValueError: Only single integers, non-nan floats, numeric strings, 
-        `fractions.Fraction`, or `decimal.Decimal` objects; or two 
-        integers or two `fractions.Fraction` objects or a pairwise 
-        combination of these, representing the numerator and non-zero 
-        denominator, respectively, of a rational fraction, are valid.
+        Several example are given below of constructing the simple continued
+        fraction for the number :math:`\\frac{-649}{200}` in different ways.
 
-        >>> ContinuedFraction('-.123456789')
-        ContinuedFraction(-123456789, 1000000000)
+        >>> ContinuedFraction(-649, 200)
+        ContinuedFraction(-649, 200)
+        >>> ContinuedFraction('-3.245')
+        ContinuedFraction(-649, 200)
+        >>> ContinuedFraction(Decimal('-3.245'))
+        ContinuedFraction(-649, 200)
+        >>> ContinuedFraction('-649/200')
+        ContinuedFraction(-649, 200)
+        >>> ContinuedFraction(Fraction(-649, 200))
+        ContinuedFraction(-649, 200)
+        >>> ContinuedFraction(ContinuedFraction(649, -200))
+        ContinuedFraction(-649, 200)
+        >>> ContinuedFraction(Fraction(-649), 200)
+        ContinuedFraction(-649, 200)
+        >>> ContinuedFraction(649, Fraction(-200))
+        ContinuedFraction(-649, 200)
+        >>> ContinuedFraction(Fraction(-649), ContinuedFraction(200))
+        ContinuedFraction(-649, 200)
+
+        In each of the examples above, the minus sign can be removed from
+        the arguments to the :py:class:`numbers.Rational` instance and
+        instead attached to the outer class, e.g.:
+
+        >>> -ContinuedFraction(649, 200)
+        ContinuedFraction(-649, 200)
+        >>> -ContinuedFraction('3.245')
+        ContinuedFraction(-649, 200)
+        >>> -ContinuedFraction('649/200')
+        ContinuedFraction(-649, 200)
+
+        Invalid arguments will raise errors in the
+        :py:class:`fractions.Fraction` superclass.
+        """
+        # Get the ``fractions.Fraction`` instance from the superclass constructor
+        self = super().__new__(cls, *args, **kwargs)
+
+        # Call ``lib.continued_fraction_rational`` with the fraction to get
+        # get the elements, and assign back to the instance
+        self._elements = tuple(continued_fraction_rational(self))
 
-        >>> ContinuedFraction(.3, -2)
-        Traceback (most recent call last):
-        ...
-        ValueError: Only single integers, non-nan floats, numeric strings, 
-        `fractions.Fraction`, or `decimal.Decimal` objects; or two 
-        integers or two `fractions.Fraction` objects or a pairwise 
-        combination of these, representing the numerator and non-zero 
-        denominator, respectively, of a rational fraction, are valid.
-
-        >>> ContinuedFraction(Fraction(-415, 93))
-        ContinuedFraction(-415, 93)
-        """
-        try:
-            cls.validate(*args, **kwargs)
-        except ValueError:
-            raise
-
-        return super().__new__(cls, *args, **kwargs)
+        return self
 
     @classmethod
-    def from_elements(cls, *elements: int) -> Fraction:
-        """
-        Returns a `ContinuedFraction` instance from a sequence of (integer)
-        elements of a continued fraction.
+    def from_elements(cls, *elements: int) -> ContinuedFraction:
+        """Returns a :py:class:`ContinuedFraction` instance from a sequence of (integer) elements of a (finite) simple continued fraction.
+
+        Invalid elements will trigger a :py:class:`ValueError`.
 
         Parameters
         ----------
-        *elements: int
-            An ordered sequence of elements of a (finite) continued fraction.
+        *elements : int
+            An ordered sequence of integer elements of a (finite) simple
+            continued fraction.
 
         Returns
         -------
         ContinuedFraction
-            A new and fully initialised instance of `ContinuedFraction` with
+            A new and fully initialised instance of :py:class:`ContinuedFraction` with
             the given element sequence.
 
+        Raises
+        ------
+        ValueError
+            If any elements are not integers, or any elements after the 1st
+            are not positive.
+
         Examples
         --------
-        Constructing a continued fraction for the rational `649/200` using the
-        element sequence `(3, 4, 12, 4)`.
+        Constructing a continued fraction for the rational :math:`\\frac{649}{200}` using
+        the element sequence :math:`3, 4, 12, 4`.
 
         >>> c1 = ContinuedFraction.from_elements(3, 4, 12, 4)
         >>> c1
         ContinuedFraction(649, 200)
 
-        Constructing the continued fraction of the inverse rational `200/649`
-        using the element sequence `(0, 3, 4, 12, 4)`.
+        Constructing the continued fraction of the (multiplicative) inverse :math:`\\frac{200}{649}`
+        using the element sequence :math:`0, 3, 4, 12, 4`.
 
         >>> c2 = ContinuedFraction.from_elements(0, 3, 4, 12, 4)
         >>> c2
         ContinuedFraction(200, 649)
-        """
-        return cls(fraction_from_elements(*elements))
 
-    def __init__(self, *args:  int | float | str | Fraction | Decimal, **kwargs: Any) -> None:
-        """
-        Initialises new `ContinuedFraction` instances with attributes and
-        properties for their elements, order, convergents, segments and
-        remainders.
-
-        Parameters
-        ----------
-        *args : int or float or str or fractions.Fraction or decimal.Decimal
-            Arguments of the type described above.
-
-        **kwargs
-            Any valid keyword arguments for the superclass fractions.Fraction
-
-        Raises
-        ------
-        ValueError
-            If there are arguments that have somehow passed the validation
-            check, but do not fall into one of the types described above.
+        Validation for elements containing non-integers or negative integers.
 
-        Examples
-        --------
-        Construct the continued fraction for the rational `415/93`.
-
-        >>> cf = ContinuedFraction(415, 93)
-        >>> cf
-        ContinuedFraction(415, 93)
+        >>> ContinuedFraction.from_elements('0', 1)
+        Traceback (most recent call last):
+        ...
+        ValueError: Continued fraction elements must be integers, and all elements after the 1st must be positive
+        >>> ContinuedFraction.from_elements(0, 1, 2.5)
+        Traceback (most recent call last):
+        ...
+        ValueError: Continued fraction elements must be integers, and all elements after the 1st must be positive
+        >>> ContinuedFraction.from_elements(1, 0)
+        Traceback (most recent call last):
+        ...
+        ValueError: Continued fraction elements must be integers, and all elements after the 1st must be positive
+        >>> ContinuedFraction.from_elements(1, -1)
+        Traceback (most recent call last):
+        ...
+        ValueError: Continued fraction elements must be integers, and all elements after the 1st must be positive
 
-        Inspect the elements, order, convergents, segments and remainders
+        """
+        # Create a new ``ContinuedFraction`` instance from the given elements
+        # and initialise with elements only - no need to initialise via
+        # ``__init__``
+        if any(not isinstance(elem, int) or (elem <= 0 and i > 0) for i, elem in enumerate(elements)):
+            raise ValueError(
+                "Continued fraction elements must be integers, and all "
+                "elements after the 1st must be positive"
+            )
 
-        >>> cf.elements
-        (4, 2, 6, 7)
-        >>> cf.order
-        3
-        >>> cf.convergents
-        mappingproxy({0: Fraction(4, 1), 1: Fraction(9, 2), 2: Fraction(58, 13), 3: Fraction(415, 93)})
-        >>> cf.segment(0), cf.segment(1), cf.segment(2), cf.segment(3)
-        (ContinuedFraction(4, 1), ContinuedFraction(9, 2), ContinuedFraction(58, 13), ContinuedFraction(415, 93))
-        >>> cf.remainder(0), cf.remainder(1), cf.remainder(2), cf.remainder(3)
-        (ContinuedFraction(415, 93), ContinuedFraction(93, 43), ContinuedFraction(43, 7), ContinuedFraction(7, 1))
-
-        Check some properties of the segments and remainders
-
-        >>> assert cf.remainder(1) == 1 / (cf - cf.convergents[0])
-        """
-        super().__init__()
-
-        if len(args) == 1 and isinstance(args[0], int):
-            self._elements = tuple(continued_fraction_rational(Fraction(args[0])))
-        elif len(args) == 1 and isinstance(args[0], float):
-            self._elements = tuple(continued_fraction_real(args[0]))
-        elif len(args) == 1 and isinstance(args[0], str) and _RATIONAL_FORMAT.match(args[0]) and '/' in args[0]:
-            self._elements = tuple(continued_fraction_rational(Fraction(*self.as_integer_ratio())))
-        elif len(args) == 1 and isinstance(args[0], str) and _RATIONAL_FORMAT.match(args[0]) and '/' not in args[0]:
-            self._elements = tuple(continued_fraction_real(args[0]))
-        elif len(args) == 1 and (isinstance(args[0], Fraction) or isinstance(args[0], Decimal)):
-            self._elements = tuple(continued_fraction_rational(Fraction(*args[0].as_integer_ratio())))
-        elif len(args) == 2 and set(map(type, args)) == set([int]):
-            self._elements = tuple(continued_fraction_rational(Fraction(args[0], args[1])))
-        elif len(args) == 2 and set(map(type, args)).issubset([int, Fraction]):
-            self._elements = tuple(continued_fraction_rational(Fraction(*self.as_integer_ratio())))
-        else:      # pragma: no cover
-            raise ValueError(self.__class__.__valid_inputs_msg__)
-
-        _convergent = partial(convergent, *self._elements)
-        self._convergents = MappingProxyType(
-            {
-                k: _convergent(k=k)
-                for k in range(len(self._elements))
-            }
-        )
+        # A step to ensure uniqueness of the simple form of the continued
+        # fraction - if the last element is ``1`` it can be "removed" by
+        # adding it to the second last element, thereby shortening the
+        # sequence by one element. The resulting simple continued
+        # fraction becomes unique for the number that is represented.
+        if len(elements) > 1 and elements[-1] == 1:
+            elements = elements[:-2] + (elements[-2] + 1,)
+
+        # Call the superclass constructor with the ``fractions.Fraction``
+        # instance returned by ``lib.fraction_from_elements`` - this will
+        # be the highest-order convergent of the simple continued
+        # fraction represented by the given sequence of elements
+        self = super().__new__(cls, fraction_from_elements(*elements))
+
+        # Assign the given elements back to the instance - note that we
+        # have avoided going through the division algorithm in
+        # ``lib.continued_fraction_rational``
+        self._elements = elements
+    
+        return self
 
-    def __add__(self, other: Fraction, /) -> Fraction:
+    def __add__(self, other, /):
         return self.__class__(super().__add__(other))
 
-    def __radd__(self, other: Fraction, /) -> Fraction:
+    def __radd__(self, other, /):
         return self.__class__(super().__radd__(other))
 
-    def __sub__(self, other: Fraction, /) -> Fraction:
+    def __sub__(self, other, /):
         return self.__class__(super().__sub__(other))
 
-    def __rsub__(self, other: Fraction, /) -> Fraction:
+    def __rsub__(self, other, /):
         return self.__class__(super().__rsub__(other))
 
-    def __mul__(self, other: Fraction, /) -> Fraction:
+    def __mul__(self, other, /):
         return self.__class__(super().__mul__(other))
 
-    def __rmul__(self, other: Fraction, /) -> Fraction:
+    def __rmul__(self, other, /):
         return self.__class__(super().__rmul__(other))
 
-    def __truediv__(self, other: Fraction, /) -> Fraction:
+    def __truediv__(self, other, /):
         return self.__class__(super().__truediv__(other))
 
-    def __rtruediv__(self, other: Fraction, /) -> Fraction:
+    def __rtruediv__(self, other, /):
         return self.__class__(super().__rtruediv__(other))
 
-    def __floordiv__(self, other: Fraction, /) -> Fraction:
+    def __floordiv__(self, other, /):
         return self.__class__(super().__floordiv__(other))
 
-    def __rfloordiv__(self, other: Fraction, /) -> Fraction:
+    def __rfloordiv__(self, other, /):
         return self.__class__(super().__rfloordiv__(other))
 
-    def __divmod__(self, other: Fraction, /) -> Fraction:
+    def __divmod__(self, other, /):
         quo, rem = super().__divmod__(other)
 
         return self.__class__(quo), self.__class__(rem)
 
-    def __rdivmod__(self, other: Fraction, /) -> Fraction:
+    def __rdivmod__(self, other, /):
         quo, rem = super().__rdivmod__(other)
         
         return self.__class__(quo), self.__class__(rem)
 
-    def __pow__(self, other: Fraction, /) -> Fraction:
+    def __pow__(self, other, /) -> ContinuedFraction:
         return self.__class__(super().__pow__(other))
 
-    def __rpow__(self, other: Fraction, /) -> Fraction:
-        return self.__class__(Fraction(other).__pow__(self))
+    def __rpow__(self, other, /):
+        return self.__class__(Fraction(other).__rpow__(self))
 
-    def __pos__(self) -> Fraction:
+    def __pos__(self) -> ContinuedFraction:
         return self.__class__(super().__pos__())
 
-    def __neg__(self) -> Fraction:
-        return self.__class__(super().__neg__())
+    def __neg__(self) -> ContinuedFraction:
+        """
+        Division-free negation for a finite simple continued fraction, as
+        described `documentation <https://continuedfractions.readthedocs.io/en/latest/sources/creating-continued-fractions.html#negative-continued-fractions>`_.
 
-    def __abs__(self) -> Fraction:
-        return self.__class__(super().__abs__())
+        The basic algorithm can be described as follows: if
+        :math:`[a_0; a_1,\\ldots, a_n]` is the simple continued fraction of a
+        **positive** rational number :math:`\\frac{a}{b}` of finite order
+        :math:`n` then  :math:`-\\frac{a}{b}` has the simple continued
+        fraction:
+
+        .. math::
+
+           \\begin{cases}
+           [-a_0;]                                      \\hskip{3em} & n = 0 \\\\
+           [-(a_0 + 1); 2]                              \\hskip{3em} & n = 1 \\text{ and } a_1 = 2 \\\\
+           [-(a_0 + 1); a_2 + 1, a_3,\\ldots, a_n]      \\hskip{3em} & n \\geq 2 \\text{ and } a_1 = 1 \\\\
+           [-(a_0 + 1); 1, a_1 - 1, a_2, \\ldots,a_n]   \\hskip{3em} & n \\geq 2 \\text{ and } a_1 \\geq 2
+           \\end{cases}
+
+        In applying this algorithm there is an assumption that the last element
+        :math:`a_n > 1`, as any simple continued fraction of type
+        :math:`[a_0; a_1,\\ldots, a_{n} = 1]` can be reduced to the simple
+        continued fraction :math:`[a_0; a_1,\\ldots, a_{n - 1} + 1]`.
+        """
+        cls_ = self.__class__
+        elms = self._elements
+
+        if len(elms) == 1:
+            # Case (1) of the algorithm
+            neg_elms = (-elms[0],)
+        elif len(elms) == 2 and elms[1] == 2:
+            # Case (2) of the algorithm
+            neg_elms = (-(elms[0] + 1), 2)
+        elif len(elms) > 1 and elms[1] == 1:
+            # Case (3) of the algorithm
+            neg_elms = (-(elms[0] + 1), elms[2] + 1, *elms[3:])
+        else:
+            # Case (4) of the algorithm
+            neg_elms = (-(elms[0] + 1), 1, elms[1] - 1, *elms[2:])
+
+        neg_self = cls_.__new__(cls_, *convergent(len(neg_elms) - 1, *neg_elms).as_integer_ratio())
+        neg_self._elements = neg_elms
+
+        return neg_self
 
+    def __abs__(self) -> ContinuedFraction:
+        return self.__class__(super().__abs__())
 
     def as_float(self) -> float:
-        """
-        Returns the `float` value of the continued fraction, using standard
-        division (`/`) of the numerator by the denominator.
+        """Returns the :py:class:`float` value of the continued fraction.
 
         Returns
         -------
         float
-            The `float` representation of the continued fraction.
+            The :py:class:`float` value of the continued fraction.
 
         Examples
         --------
+        Note that the default :py:mod:`decimal` context precision of :math:`28`
+        is used in these examples.
+
         >>> import math
         >>> math.pi
         3.141592653589793
 
-        Now construct a `ContinuedFraction` object from it, and check the 
-        `float` value.
+        Now construct a :py:class:`ContinuedFraction` instance from it, and check the 
+        :py:class:`float` value.
 
         >>> cf = ContinuedFraction(math.pi)
         >>> cf
         ContinuedFraction(884279719003555, 281474976710656)
         >>> cf.as_float()
         3.141592653589793
         """
         return self.numerator / self.denominator
 
     def as_decimal(self) -> Decimal:
-        """
-        Returns the `float` value of the continued fraction, using standard
-        division (`/`) of the numerator by the denominator.
+        """Returns the :py:class:`decimal.Decimal` value of the continued fraction.
 
         Returns
         -------
-        float
-            The `float` representation of the continued fraction.
+        decimal.Decimal
+            The :py:class:`decimal.Decimal` representation of the continued fraction.
 
         Examples
         --------
+        Note that the default :py:mod:`decimal` context precision of :math:`28`
+        is used in these examples.
+
         >>> import math
         >>> math.pi
         3.141592653589793
 
-        Now construct a `ContinuedFraction` object from it, and check the 
-        `float` value.
+        Now construct a :py:class:`ContinuedFraction` instance from it, and check the 
+        :py:class:`float` value.
 
         >>> cf = ContinuedFraction(math.pi)
         >>> cf
         ContinuedFraction(884279719003555, 281474976710656)
-        >>> cf.as_float()
-        3.141592653589793
+        >>> cf.as_decimal()
+        Decimal('3.141592653589793115997963469')
         """
         return Decimal(self.numerator) / Decimal(self.denominator)
 
     @property
     def elements(self) -> tuple[int]:
-        """
-        Property: the element sequence of the continued fraction.
-
-        Returns
-        -------
-        tuple[int]
-            The element sequence of the continued fraction.
+        """:py:class:`tuple`: The sequence of elements of the continued fraction.
 
         Examples
         --------
         >>> cf = ContinuedFraction('.12345')
         >>> cf
         ContinuedFraction(2469, 20000)
         >>> cf.elements
         (0, 8, 9, 1, 21, 1, 1, 5)
         """
         return self._elements
 
     @property
     def order(self) -> int:
-        """
-        Property: the order of the continued fraction, which is the number
-                  of its elements + `1`.
-
-        Returns
-        -------
-        int
-            The order of the continued fraction, which is the number of its
-            elements + `1`.
+        """:py:class:`int`: The order of the continued fraction, which is the number of its elements minus :math:`1`.
 
         Examples
         --------
         >>> cf = ContinuedFraction('.12345')
         >>> cf
         ContinuedFraction(2469, 20000)
+        >>> len(cf.elements)
+        8
         >>> cf.order
         7
         """
         return len(self._elements[1:])
 
     @property
     def khinchin_mean(self) -> Decimal | None:
-        """
-        Property: the Khinchin mean of the continued fraction, which we define
-                  as the geometric mean of all its elements starting from
-                  ``a_1``, so that is,:
-                  ::
-
-                    a_1, a_2, ...
-
-                  The leading element ``a_0`` is excluded.
-
-                  As in practice all ``ContinuedFraction`` objects will have a
-                  finite sequence of elements the Khinchin mean as defined
-                  above will always have a computable value.
-
-                  In the special case of integers or fractions representing
-                  integers, whose continued fraction representations consist of
-                  only a single element, a null value is returned.
+        """:py:class:`decimal.Decimal` or :py:data:`None`: The Khinchin mean of the continued fraction, which is defined as the geometric mean of all its elements after the 1st.
 
-        Returns
-        -------
-        decimal.Decimal
-            The geometric mean of all elements of the continued fraction,
-            excluding the leading term ``a_0``, so the geometric mean of
-            the sequence ``a_1, a2, ...``.
+        We define the Khinchin mean :math:`K_n` of a simple continued fraction
+        :math:`[a_0; a_1, a_2, \\ldots, a_n]` as:
+
+        .. math::
+
+           K_n := \\sqrt[n]{a_1a_2 \\cdots a_n} = \\left( a_1a_2 \\cdots a_n \\right)^{\\frac{1}{n}}, \\hskip{3em} n \\geq 1
+
+        This property is intended to make it easier to study the limit of
+        :math:`K_n` as :math:`n \\to \\infty`.  See the `documentation <https://continuedfractions.readthedocs.io/en/latest/sources/exploring-continued-fractions.html#khinchin-means-khinchin-s-constant>`_
+        for more details.
+
+        In the special case of integers or fractions representing integers,
+        whose continued fraction representations consist of only a single
+        element, a null value is returned.
 
         Examples
         --------
+        Note that the default :py:mod:`decimal` context precision of :math:`28`
+        is used in these examples.
+
         >>> ContinuedFraction(649, 200).elements
         (3, 4, 12, 4)
         >>> ContinuedFraction(649, 200).khinchin_mean
         Decimal('5.76899828122963409526846589869819581508636474609375')
         >>> ContinuedFraction(415, 93).elements
         (4, 2, 6, 7)
         >>> ContinuedFraction(415, 93).khinchin_mean
         Decimal('4.37951913988788898990378584130667150020599365234375')
         >>> (ContinuedFraction(649, 200) + ContinuedFraction(415, 93)).elements
         (7, 1, 2, 2, 2, 1, 1, 11, 1, 2, 12)
         >>> (ContinuedFraction(649, 200) + ContinuedFraction(415, 93)).khinchin_mean
         Decimal('2.15015313349074244086978069390170276165008544921875')
         >>> ContinuedFraction(5000).khinchin_mean
-        
-        """
-        try:
-            return Decimal(statistics.geometric_mean(self.elements[1:]))
-        except statistics.StatisticsError:
-            return
 
-    @property
-    def convergents(self) -> MappingProxyType[int, Fraction]:
         """
-        Property: the map of all the (simple) convergents of the continued
-                  fraction, keyed by the orders `0`,`1`,...,`n`, where `n` is
-                  the order of the continued fraction.
+        match self.order:
+            case 0:
+                return None
+            case 1:
+                return Decimal(self.elements[-1])
+            case _:
+                return Decimal(statistics.geometric_mean(self.elements[1:]))
+
+    @functools.cache
+    def convergent(self, k: int, /) -> ContinuedFraction:
+        """Returns the :math:`k`-th (simple) convergent of the continued fraction.
 
-        Returns
-        -------
-        types.MappingProxyType[int, fractions.Fraction]
-            The map of all convergents of the continued fraction, keyed
-            by their orders.
+        Given a simple continued fraction  :math:`[a_0;a_1,a_2,\\ldots]` the
+        :math:`k`-th convergent is defined as:
 
-        Examples
-        --------
-        >>> cf = ContinuedFraction('.12345')
-        >>> cf
-        ContinuedFraction(2469, 20000)
-        >>> cf.convergents
-        mappingproxy({0: Fraction(0, 1), 1: Fraction(1, 8), 2: Fraction(9, 73), 3: Fraction(10, 81), 4: Fraction(219, 1774), 5: Fraction(229, 1855), 6: Fraction(448, 3629), 7: Fraction(2469, 20000)})
-        """
-        return self._convergents
+        .. math::
 
-    def segment(self, k: int, /) -> Fraction:
-        """
-        Returns a ``ContinuedFraction`` object for the `k`-th segment of
-        the continued fraction, which is defined as the sequence of its
-        first ``k + 1`` elements ``a_0, a_1, ... , a_k``. As this sequence
-        uniquely determines the ``k``-th convergent of the continued
-        fraction, the ``k``-th segments may be used as a proxy for the
-        convergents, which in this implementation are represented using
-        ``fractions.Fraction``.
+           C_k = a_0 + \\cfrac{1}{a_1 + \\cfrac{1}{a_2 \\ddots \\cfrac{1}{a_{k-1} + \\cfrac{1}{a_k}}}}
+
+        The result is a :py:class:`fractions.Fraction` instance.
+        
+        The integer :math:`k` is called the order of the convergent, and if 
+        :math:`[a_0;a_1,a_2,\\ldots]` is finite of order :math:`n` then it has
+        exactly :math:`n + 1` convergents :math:`C_0,C_1,C_2,\\ldots,C_n` where
+        the :math:`k`-th convergent :math:`C_k = \\frac{p_k}{q_k}` is given by
+        the recurrence relation:
+
+        .. math::
+           
+           \\begin{align}
+           p_k &= a_kp_{k - 1} + p_{k - 2} \\\\
+           q_k &= a_kq_{k - 1} + q_{k - 2},        \\hskip{3em}    k \\geq 3
+           \\end{align}
+
+        where :math:`p_0 = a_0`, :math:`q_0 = 1`, :math:`p_1 = p_1p_0 + 1`,
+        and :math:`q_1 = p_1`.
+
+        The method is cached (with :py:func:`functools.cache`), which makes
+        calls after the initial call much faster.
 
         Parameters
         ----------
         k : int
-            The index of the segment, as described above.
+            The order of the convergent, as described above.
 
         Returns
         -------
         ContinuedFraction
-            A new `ContinuedFraction` instance representing the `k`-th segment
-            of the original continued fraction, as described above.
+            A new :py:class:`ContinuedFraction` instance representing the :math:`k`-th
+            (simple) convergent of the original continued fraction, as
+            described above.
 
         Examples
         --------
         >>> cf = ContinuedFraction('.12345')
         >>> cf
         ContinuedFraction(2469, 20000)
-        >>> cf.segment(2)
+        >>> cf.convergent(0)
+        ContinuedFraction(0, 1)
+        >>> cf.convergent(2)
         ContinuedFraction(9, 73)
+        >>> cf.convergent(6)
+        ContinuedFraction(448, 3629)
+        >>> cf.convergent(7)
+        ContinuedFraction(2469, 20000)
         """
-        return self.__class__.from_elements(*self._elements[:k + 1])
+        return self.__class__(convergent(k, *self._elements))
+
+    @property
+    @functools.lru_cache
+    def convergents(self) -> MappingProxyType[int, ContinuedFraction]:
+        """:py:class:`types.MappingProxyType`: An immutable dict of all :math:`k`-order convergents of the continued fraction, keyed by order.
+
+        Each convergent is indexed by its order and is also a
+        :py:class:`ContinuedFraction` instance.
 
-    def remainder(self, k: int, /) -> Fraction:
+        The property is cached (with :py:func:`functools.lru_cache`), which makes
+        calls after the initial call much faster.
+
+        Examples
+        --------
+        >>> cf = ContinuedFraction('3.245')
+        >>> cf.convergents
+        mappingproxy({0: ContinuedFraction(3, 1), 1: ContinuedFraction(13, 4), 2: ContinuedFraction(159, 49), 3: ContinuedFraction(649, 200)})
+        >>> cf.convergents[0], cf.convergents[2]
+        (ContinuedFraction(3, 1), ContinuedFraction(159, 49))
+        """
+        return MappingProxyType({
+            k: self.convergent(k)
+            for k in range(self.order + 1)
+        })
+
+    @property
+    @functools.lru_cache
+    def even_order_convergents(self) -> MappingProxyType[int, ContinuedFraction]:
+        """:py:class:`types.MappingProxyType`: An immutable dict of all even-order convergents of the continued fraction, keyed by order.
+
+        Each convergent is indexed by its order and is also a
+        :py:class:`ContinuedFraction` instance.
+
+        The property is cached (with :py:func:`functools.lru_cache`), which makes
+        calls after the initial call much faster.
+
+        Examples
+        --------
+        >>> ContinuedFraction('3.245').even_order_convergents
+        mappingproxy({0: ContinuedFraction(3, 1), 2: ContinuedFraction(159, 49)})
+        """
+        return MappingProxyType({
+            k: self.convergents[k]
+            for k in range(0, self.order + 1, 2)
+        })
+
+    @property
+    @functools.lru_cache
+    def odd_order_convergents(self) -> MappingProxyType[int, ContinuedFraction]:
+        """:py:class:`types.MappingProxyType`: An immutable dict of all odd-order convergents of the continued fraction, keyed by order.
+
+        Each convergent is indexed by its order and is also a
+        :py:class:`ContinuedFraction` instance.
+
+        The property is cached (with :py:func:`functools.lru_cache`), which makes
+        calls after the initial call much faster.
+
+        Examples
+        --------
+        >>> ContinuedFraction('3.245').odd_order_convergents
+        mappingproxy({1: ContinuedFraction(13, 4), 3: ContinuedFraction(649, 200)})
         """
-        The `k`-th remainder of the continued fraction, defined as the continued
-        fraction given by the difference between the original continued
-        fraction and its `(k - 1)`-order convergent (equivalently, the
-        `(k - 1)`-order segment, as defined above).
+        return MappingProxyType({
+            k: self.convergents[k]
+            for k in range(1, self.order + 1, 2)
+        })
+
+    @functools.cache
+    def remainder(self, k: int, /) -> ContinuedFraction:
+        """Returns the :math:`k`-th remainder of the continued fraction.
+
+        The :math:`k`-th remainder :math:`R_k` of a (simple) continued fraction
+        :math:`[a_0; a_1,\\ldots]` as the continued fraction :math:`[a_k;a_{k + 1},\\ldots]`,
+        obtained from the original by "removing" the elements of the :math:`(k - 1)`-st
+        convergent :math:`C_{k - 1} = (a_0,a_1,\\ldots,a_{k - 1})`.
+
+        .. math::
+
+            R_k = a_k + \\cfrac{1}{a_{k + 1} + \\cfrac{1}{a_{k + 2} \\ddots }}
+
+        The method is cached (with :py:func:`functools.cache`), which makes calls
+        after the initial call much faster.
 
         Parameters
         ----------
         k : int
             The index of the remainder, as described above.
 
         Returns
         -------
         ContinuedFraction
-            A new `ContinuedFraction` instance representing the `k`-th remainder
-            of the original continued fraction, as described above.
+            A new :py:class:`ContinuedFraction` instance representing the :math:`k`-th
+            remainder of the original continued fraction, as described above.
 
         Examples
         --------
         >>> cf = ContinuedFraction('.12345')
         >>> cf
         ContinuedFraction(2469, 20000)
+        >>> cf.remainder(0)
+        ContinuedFraction(2469, 20000)
         >>> cf.remainder(2)
         ContinuedFraction(2469, 248)
+        >>> cf.remainder(6)
+        ContinuedFraction(6, 5)
+        >>> cf.remainder(7)
+        ContinuedFraction(5, 1)
         """
         return self.__class__.from_elements(*self._elements[k:])
 
-    def mediant(self, other: Fraction, /, *, dir='right', k: int = 1) -> Fraction:
+    @property
+    @functools.lru_cache
+    def remainders(self) -> MappingProxyType[int, ContinuedFraction]:
+        """:py:class:`types.MappingProxyType`: An immutable dict of all :math:`k`-th remainders of the continued fraction, keyed by order.
+
+        Each remainder is indexed by its order and is also a
+        :py:class:`ContinuedFraction` instance.
+
+        The property is cached (with :py:func:`functools.lru_cache`), which makes
+        calls after the initial call much faster.
+
+        Examples
+        --------
+        >>> cf = ContinuedFraction('3.245')
+        >>> cf.remainders
+        mappingproxy({0: ContinuedFraction(649, 200), 1: ContinuedFraction(200, 49), 2: ContinuedFraction(49, 4), 3: ContinuedFraction(4, 1)})
+        >>> cf.remainders[0], cf.remainders[2]
+        (ContinuedFraction(649, 200), ContinuedFraction(49, 4))
         """
-        Returns the `k`-th left- or right-mediant of this `ContinuedFraction`
-        object with another `fractions.Fraction` object. The "direction" of the
-        mediant is specified with `dir`, and can only be one of `"left"` or 
-        `"right"`.
+        return MappingProxyType({
+            k: self.remainder(k)
+            for k in range(self.order + 1)
+        })
+
+    @functools.cache
+    def left_mediant(self, other: Fraction, /, *, k: int = 1) -> ContinuedFraction:
+        """Returns the :math:`k`-th left-mediant of the continued fraction with another rational number.
+        
+        For a positive integer :math:`k`, the :math:`k`-th left-mediant of two
+        rational numbers :math:`r = \\frac{a}{b}` and :math:`s = \\frac{c}{d}`,
+        where :math:`b, d, b + d \\neq 0`, is defined as:
+        
+        .. math::
+
+           \\frac{ka + c}{kb + d}, \\hskip{3em}    k \\geq 1
+
+        while the :math:`k`-th right mediant is defined as:
+        
+        .. math::
+
+           \\frac{a + kc}{b + kd}, \\hskip{3em}    k \\geq 1
+
+        If we assume that :math:`r < s` and :math:`bd > 0` then these mediants
+        have the property that:
+       
+        .. math::
+
+           \\frac{a}{b} < \\frac{ka + c}{kb + d} \\leq \\frac{a + kc}{b + kd} < \\frac{c}{d},   \\hskip{3em} k \\geq 1
+
+        where equality holds for :math:`k = 1`. If we let :math:`k \\to \\infty`
+        then the mediants converge to opposite limits:
+
+        .. math::
+
+          \\begin{align}
+          \\lim_{k \\to \\infty} \\frac{ka + c}{kb + d} &= \\frac{a}{b} \\\\
+          \\lim_{k \\to \\infty} \\frac{a + kc}{b + kd} &= \\frac{c}{d}
+          \\end{align}
+
+        For more information consult the
+        `documentation <https://continuedfractions.readthedocs.io/en/latest/sources/mediants.html>`_.
+
+        The method is cached (with :py:func:`functools.cache`), which makes calls
+        after the initial call much faster.
+
+        Parameters
+        ----------
+        other : fractions.Fraction, ContinuedFraction
+            The second fraction to use to calculate the :math:`k`-th mediant with
+            the first.
+        
+        k : int, default=1
+            The order of the mediant, as defined above.        
+
+        Returns
+        -------
+        ContinuedFraction
+            The :math:`k`-th left-mediant of the original fraction and the second
+            fraction, as a :py:class:`ContinuedFraction` instance.
+
+        Examples
+        --------
+        >>> c1 = ContinuedFraction('1/2')
+        >>> c2 = ContinuedFraction(3, 5)
+        >>> c1, c2
+        (ContinuedFraction(1, 2), ContinuedFraction(3, 5))
+        >>> c1.left_mediant(c2)
+        ContinuedFraction(4, 7)
+        >>> c1.left_mediant(c2, k=2)
+        ContinuedFraction(5, 9)
+        >>> c1.left_mediant(c2, k=3)
+        ContinuedFraction(6, 11)
+        >>> c1.left_mediant(c2, k=100)
+        ContinuedFraction(103, 205)
+        >>> assert c1.left_mediant(c2, k=2) < c1.right_mediant(c2, k=2)
+        >>> assert c1.left_mediant(c2, k=3) < c1.right_mediant(c2, k=3)
+        >>> assert c1.left_mediant(c2, k=100) < c1.right_mediant(c2, k=100)
+        """
+        return self.__class__(left_mediant(self, other, k=k))
+
+    @functools.cache
+    def right_mediant(self, other: Fraction, /, *, k: int = 1) -> ContinuedFraction:
+        """Returns the :math:`k`-th right-mediant of the continued fraction with another rational number.
+        
+        For a positive integer :math:`k`, the :math:`k`-th right-mediant of two
+        rational numbers :math:`r = \\frac{a}{b}` and :math:`s = \\frac{c}{d}`,
+        where :math:`b, d, b + d \\neq 0`, is defined as:
+        
+        .. math::
+
+           \\frac{a + kc}{b + kd}, \\hskip{3em}    k \\geq 1
+
+        while the :math:`k`-th left-mediant is defined as:
+        
+        .. math::
 
-        For a positive integer `k`, the `k`-th left-mediant of rational numbers
-        `r = a / b` and `s = c / d`, where `b` and `d` are non-zero, can be defined
-        as:
-        ::
+           \\frac{ka + c}{kb + d}, \\hskip{3em}    k \\geq 1
 
-            (ka + c) / (kb + d)
+        If we assume that :math:`r < s` and :math:`bd > 0` then these mediants
+        have the property that:
+       
+        .. math::
 
-        while the `k`-th right mediant can be defined as:
-        ::
+           \\frac{a}{b} < \\frac{ka + c}{kb + d} \\leq \\frac{a + kc}{b + kd} < \\frac{c}{d},   \\hskip{3em} k \\geq 1
 
-            (a + kc) / (b + kd)
+        where equality holds for :math:`k = 1`. If we let :math:`k \\to \\infty`
+        then the mediants converge to opposite limits:
 
-        If we assume that `r < s` and `bd > 0` then the `k`-th left mediants have
-        the property that:
-        ::
+        .. math::
 
-            a / b < ... < (3a + c) / (3b + d) < (2a + c) / (2b + d) < (a + c) / (b + d) < c / d
-            a / b < (a + c) / (b + d) < (a + 2c) / (b + 2d) < (a + 3c) / (b + 3d) < ... c / d
+          \\begin{align}
+          \\lim_{k \\to \\infty} \\frac{ka + c}{kb + d} &= \\frac{a}{b} \\\\
+          \\lim_{k \\to \\infty} \\frac{a + kc}{b + kd} &= \\frac{c}{d}
+          \\end{align}
 
-        That is, the left mediants form a strictly decreasing sequence, actually
-        converging to `a / b`, while the right mediants form a strictly increasing
-        sequence of, actually converging to `c / d`.
+        For more information consult the
+        `documentation <https://continuedfractions.readthedocs.io/en/latest/sources/mediants.html>`_.
 
-        For the left mediant use `dir='left'`, while for the right use
-        `dir='right'`. The default is `dir='right'`. For `k = 1` the left and right
-        mediants are the same.
+        The method is cached (with :py:func:`functools.cache`), which makes calls
+        after the initial call much faster.
 
         Parameters
         ----------
-        other : fractions.Fraction or ContinuedFraction
-            The second fraction to use to calculate the `k`-th mediant with
+        other : fractions.Fraction, ContinuedFraction
+            The second fraction to use to calculate the :math:`k`-th mediant with
             the first.
         
         k : int, default=1
             The order of the mediant, as defined above.        
 
         Returns
         -------
         ContinuedFraction
-            The `k`-th mediant of the original fraction and the second
-            fraction, as a `ContinuedFraction` instance.
+            The :math:`k`-th right-mediant of the original fraction and the second
+            fraction, as a :py:class:`ContinuedFraction` instance.
 
         Examples
         --------
-        >>> c1 = ContinuedFraction('.5')
+        >>> c1 = ContinuedFraction('1/2')
         >>> c2 = ContinuedFraction(3, 5)
         >>> c1, c2
         (ContinuedFraction(1, 2), ContinuedFraction(3, 5))
-        >>> c1.mediant(c2)
+        >>> c1.right_mediant(c2)
         ContinuedFraction(4, 7)
-        >>> c1.mediant(c2, k=2)
+        >>> c1.right_mediant(c2, k=2)
         ContinuedFraction(7, 12)
-        >>> c1.mediant(c2, k=3)
+        >>> c1.right_mediant(c2, k=3)
         ContinuedFraction(10, 17)
+        >>> c1.right_mediant(c2, k=100)
+        ContinuedFraction(301, 502)
+        >>> assert c1.left_mediant(c2, k=2) < c1.right_mediant(c2, k=2)
+        >>> assert c1.left_mediant(c2, k=3) < c1.right_mediant(c2, k=3)
+        >>> assert c1.left_mediant(c2, k=100) < c1.right_mediant(c2, k=100)
         """
-        return self.__class__(mediant(self, other, dir=dir, k=k))
+        return self.__class__(right_mediant(self, other, k=k))
 
 
 if __name__ == "__main__":      # pragma: no cover
     # Doctest the module from the project root using
     #
     #     python -m doctest -v src/continuedfractions/continuedfraction.py
     #
+    # NOTE: the doctest examples using where `float` or ``decimal.Decimal``
+            # values assume a context precision of 28 digits
+    decimal.getcontext().prec = 28
     import doctest
     doctest.testmod()
```

### Comparing `continuedfractions-0.11.9/src/continuedfractions/lib.py` & `continuedfractions-0.12.0/src/continuedfractions/lib.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,356 +1,415 @@
 __all__ = [
     'continued_fraction_real',
     'continued_fraction_rational',
-    'fraction_from_elements',
     'convergent',
+    'fraction_from_elements',
+    'left_mediant',
     'mediant',
+    'right_mediant',
 ]
 
 
 # -- IMPORTS --
 
 # -- Standard libraries --
-from collections import deque
+import decimal
+import functools
+import re
+
 from decimal import Decimal
-from itertools import accumulate
 from fractions import Fraction
 from typing import Generator
 
 # -- 3rd party libraries --
 
 # -- Internal libraries --
 
 
+# A private copy of ``fractions._RATIONAL_FORMAT`` to support debugging
+_RATIONAL_FORMAT = re.compile(r"""
+    \A\s*                                  # optional whitespace at the start,
+    (?P<sign>[-+]?)                        # an optional sign, then
+    (?=\d|\.\d)                            # lookahead for digit or .digit
+    (?P<num>\d*|\d+(_\d+)*)                # numerator (possibly empty)
+    (?:                                    # followed by
+       (?:\s*/\s*(?P<denom>\d+(_\d+)*))?   # an optional denominator
+    |                                      # or
+       (?:\.(?P<decimal>\d*|\d+(_\d+)*))?  # an optional fractional part
+       (?:E(?P<exp>[-+]?\d+(_\d+)*))?      # and optional exponent
+    )
+    \s*\Z                                  # and optional whitespace to finish
+""", re.VERBOSE | re.IGNORECASE)
+
+
 def continued_fraction_rational(r: Fraction, /) -> Generator[int, None, None]:
-    """
-    Generates the (integer) elements (also called coefficient or terms) of a
-    unique, finite, "simple" continued fraction representation of the
-    rational fraction `x/y` with numerator `x` and non-zero denominator `y`,
-    given as a `fractions.Fraction` object.
-
-    The number of elements generated minus 1 is called the order of the
-    continued fraction, and as the function applies only to rational fractions
-    the order will always be finite.
-
-    Negative rational fractions can be represented, but in accordance with
-    convention and to ensure uniqueness only the numerator can be negative,
-    while the denominator cannot - in case of inputs such as `x/-y`, where
-    `x` and `y` are positive integers, the negative sign is "transferred" from
-    the denominator `y` to the numerator `x`.
+    """Generates elements/coefficients of the finite, simple continued fraction for the given rational number.
 
-    For a definition of "continued fraction", "element", "order",
-    "finite continued fraction", "simple continued fraction", please consult:
+    The resulting sequence of elements defines a continued fraction of the form:
+
+    .. math::
+
+       a_0 + \\cfrac{1}{a_1 + \\cfrac{1}{a_2 + \\ddots\\cfrac{1}{a_{n - 1} + \\cfrac{1}{a_n}}}}
+
+    which is also written more compactly as:
+
+    .. math::
+
+       [a_0; a_1, a_2\\ldots, a_n]
+
+    The order of the continued fraction is said to be :math:`n`.
 
-        https://en.wikipedia.org/wiki/Continued_fraction
-        https://mathcenter.oxford.emory.edu/site/math125/continuedFractions/
+    Negative rational numbers can also be represented in this way, provided we
+    use the `Euclidean division lemma <https://en.wikipedia.org/wiki/Euclid%27s_lemma>`_.
+    This is described in more detail in the `documentation <https://continuedfractions.readthedocs.io/en/latest/sources/creating-continued-fractions.html#negative-continued-fractions>`_.
+
+    For a definition of "continued fraction", "element", "order",
+    "finite continued fraction", "simple continued fraction", please consult
+    the `package documentation <https://continuedfractions.readthedocs.io/en/stable>`_,
+    or any online resource such as `Wikipedia <https://en.wikipedia.org/wiki/Continued_fraction>`_,
+    or suitable books on number theory.
 
     Parameters
     ----------
-    r : fractions.Fraction
+    r : `fractions.Fraction`
         The rational number to represented as a continued fraction.
 
     Yields
     ------
     int
         Elements of a unique, finite "simple" continued fraction representation
-        of the given rational fraction `x/y` (where `y` is non-zero).
+        of the given rational number.
 
     Examples
     --------
     A few examples are given below of how this function can be used.
 
     >>> for e in continued_fraction_rational(Fraction(649, 200)):
     ...     print(e)
     ... 
     3
     4
     12
     4
-
     >>> list(continued_fraction_rational(Fraction(415, 93)))
     [4, 2, 6, 7]
-
     >>> list(continued_fraction_rational(Fraction(-649, 200)))
     [-4, 1, 3, 12, 4]
-
     >>> list(continued_fraction_rational(Fraction(123235, 334505)))
     [0, 2, 1, 2, 1, 1, 250, 1, 13]
 
     Notes
     -----
-    It is known that every rational number has exactly two finite continued
-    fraction representations, one of which has an additional element of `1`
-    as its last element. Any such continued fraction can be translated into a
-    shorter continued fraction whose last element is 1 + its second last
-    element.
-
-    The continued fraction representation generated by this function is the
-    shorter version, and is thus unique.
-
-    A continued fraction is called "simple" if all of its fractional terms
-    have the numerator `1`, and it is the simple version that is generated by
-    the function.
+    Every rational number has exactly two simple continued fractions, one of
+    which has an additional element of :math:`1` as its last element,
+    i.e. :math:`[a_0;a_1,a_2,\\ldots,a_{n - 1}, 1]`. But this form can be
+    reduced by adding the :math:`1` to the second last element, :math:`a_{n - 1}`,
+    producing the shorter form :math:`[a_0;a_1,a_2,\\ldots, a_{n - 1} + 1]`,
+    where the last element is now :math:`> 1`.
+
+    The simple continued fraction representation generated by this function is
+    the shorter version, and is thus unique.
     """
     num, denom = r.as_integer_ratio()
 
     quo, rem = divmod(num, denom)
     yield quo
 
     while rem > 0:
         num, denom = denom, rem
         quo, rem = divmod(num, denom)
         yield quo
 
 
-def continued_fraction_real(x: int | float | str, /) -> Generator[int, None, None]:
-    """
-    Generates the (integer) elements of a "simple" continued fraction
-    representation of `x`, which can be either an integer, float or an
-    equivalent string representation, except for nans and non-numeric strings.
-
-    As floats are finite precision representations of real numbers, if `x`
-    is a float representing a real number with a fractional part containing
-    an infinite periodic sequence of digits, or is an irrational number, the
-    continued fraction representation of `x`, as given by the elements
-    generated by the function, will necessarily be finite, but not necessarily
-    unique.
-
-    No attempt is made to raise exceptions or errors directly - if `x` is not
-    an `int` or `float`, or is a `nan` or a non-numeric string, either the
-    `decimal.Decimal` conversion or the call to `continued_fraction_rational`
-    will trigger upstream error(s).
+def continued_fraction_real(x: int | float | str | Decimal, /) -> Generator[int, None, None]:
+    """Generates elements/coefficients of a simple continued fraction of the given real number.
+
+    The simple continued fraction representation of :math:`x` is a number of
+    the form
+
+    .. math::
+
+       a_0 + \\cfrac{1}{a_1 + \\cfrac{1}{a_2 + \\ddots}}
+
+    where :math:`a_0 = [x]` is the integer part of :math:`x`, and the
+    :math:`a_1,a_2\\ldots` are the (non-negative) quotients obtained by a
+    repeated application of `Euclidean division <https://en.wikipedia.org/wiki/Euclidean_division>`_
+    to the fractional part :math:`x - [x]`, which is called the remainder.
+
+    As Python :py:class:`float` values, like all floating point
+    implementations, are `finite precision representations <https://docs.python.org/3/tutorial/floatingpoint.html>`_
+    of real numbers, the resulting simple continued fraction  of :math:`x`
+    generated by this function may be approximate, not exact, and also not
+    necessarily unique.
+
+    For non-rational real numbers it is best to pass :py:class:`decimal.Decimal`
+    values, with the `context precision <https://docs.python.org/3.12/library/decimal.html#context-objects>`_
+    set to the highest level possible.
+
+    The results for rational numbers are guaranteed to be exact however large
+    the number, subject to memory and hardware limitations of the running
+    environment.
+
+    Invalid values will generate an error in either the
+    :py:class:`fractions.Fraction` or :py:class:`decimal.Decimal` classes -
+    no errors are raised directly in the function itself.
 
     Parameters
     ----------
-    x : int or float or str
-        The number to represent as a continued fraction. It can be any `int` or
-        `float`, or an equivalent string representation of an `int` or `float`,
-        except for nans (`float("nan")`) and non-numeric strings.
+    x : int, float, str, decimal.Decimal
+        The real number to represent as a simple continued fraction.
 
     Yields
     ------
     int
-        Elements of a unique "simple" continued fraction representation of
-        the given `int` or `float`.
+        Elements of a simple continued fraction of the given real number.
 
     Examples
     --------
     A few examples are given below of how this function can be used.
 
+    >>> list(continued_fraction_real(5000))
+    [5000]
+    >>> list(continued_fraction_real(-5000.0))
+    [-5000]
     >>> list(continued_fraction_real(2/5))
+    [0, 2, 2, 1801439850948198]
+    >>> list(continued_fraction_real('2/5'))
     [0, 2, 2]
-
-    >>> list(continued_fraction_real(2984.0495684))
-    [2984, 20, 5, 1, 2, 1, 7, 2, 9, 6, 1, 4]
-
+    >>> list(continued_fraction_real('-1/3'))
+    [-1, 1, 2]
     >>> list(continued_fraction_real(1/1j))
     Traceback (most recent call last):
     ...
-    decimal.InvalidOperation: [<class 'decimal.ConversionSyntax'>]
-
-    >>> list(continued_fraction_real('-1/3'))
+    TypeError: conversion from complex to Decimal is not supported
+    >>> list(continued_fraction_real("not a numeric string"))
     Traceback (most recent call last):
     ...
     decimal.InvalidOperation: [<class 'decimal.ConversionSyntax'>]
-
     >>> list(continued_fraction_real(-649/200))
+    [-4, 1, 3, 12, 3, 1, 234562480591, 2, 5, 2]
+    >>> list(continued_fraction_real('-649/200'))
     [-4, 1, 3, 12, 4]
+    >>> list(continued_fraction_real('-649/-200'))
+    Traceback (most recent call last):
+    ...
+    ValueError: Invalid literal for Fraction: '-649/-200'
+    >>> list(continued_fraction_real(Decimal('0.3333')))
+    [0, 3, 3333]
+    """
+    if isinstance(x, int):
+        yield x
+    elif isinstance(x, str) and '/' in x:
+        yield from continued_fraction_rational(Fraction(x))
+    elif isinstance(x, float):
+        yield from continued_fraction_rational(Fraction(*Decimal.from_float(x).as_integer_ratio()))
+    else:
+        yield from continued_fraction_rational(Fraction(*(Decimal(x).as_integer_ratio())))
 
-    Notes
-    -----
-    It might be expected that numeric strings expressing rational fractions,
-    such as `"1/3"`, would be processed succesfully, but this is not the case,
-    as the key step in the function is to use the string representation of `x`
-    to construct a `decimal.Decimal` object, which, however, does not treat
-    strings such as `"x/y"` where `x` and `y` are integers or floats, as
-    numeric.
-
-    See the CPython library source for more information:
 
-    https://github.com/python/cpython/blob/main/Lib/_pydecimal.py#L557
+def convergent(k: int, *elements: int) -> Fraction:
+    """Returns the :math:`k`-th convergent of a simple continued fraction from a sequence of its elements.
 
-    But actual fractions where the numerator and denominator are `int` or
-    `float`, e.g. `-1/4` or `5.6/2`, can be processed successfully.
-    """
-    num, denum = Decimal(str(x)).as_integer_ratio()
+    Given a simple continued fraction  :math:`[a_0;a_1,a_2,\\ldots]` the
+    :math:`k`-th convergent is defined as:
 
-    for elem in continued_fraction_rational(Fraction(num, denum)):
-        yield elem
+    .. math::
 
+       C_k = a_0 + \\cfrac{1}{a_1 + \\cfrac{1}{a_2 \\ddots \\cfrac{1}{a_{k-1} + \\cfrac{1}{a_k}}}}
 
-def fraction_from_elements(*elements: int) -> Fraction:
-    """
-    Returns a `fractions.Fraction` object representing the rational fraction
-    constructed from an ordered sequence of the (integer) elements of a
-    continued fraction.
-
-    The element sequence must be given as positional arguments, which means
-    that if they are contained in an iterable then they must be unpacked
-    using the unpacking operator `*`, as described in the examples below.
+    The result is a :py:class:`fractions.Fraction` instance.
+    
+    The integer :math:`k` is called the order of the convergent, and if 
+    :math:`[a_0;a_1,a_2,\\ldots]` is finite of order :math:`n` then it has
+    exactly :math:`n + 1` convergents :math:`C_0,C_1,C_2,\\ldots,C_n` where
+    the :math:`k`-th convergent :math:`C_k = \\frac{p_k}{q_k}` is given by
+    the recurrence relation:
+
+    .. math::
+       
+       \\begin{align}
+       p_k &= a_kp_{k - 1} + p_{k - 2} \\\\
+       q_k &= a_kq_{k - 1} + q_{k - 2},        \\hskip{3em}    k \\geq 3
+       \\end{align}
+
+    where :math:`p_0 = a_0`, :math:`q_0 = 1`, :math:`p_1 = p_1p_0 + 1`,
+    and :math:`q_1 = p_1`.
+
+    This function is a faithful implementation of this algorithm.
+
+    A :py:class:`ValueError` is raised if :math:`k` is not an integer or is an
+    integer greater than the number of elements, or if any of the elements are
+    not integers.
 
     Parameters
     ----------
-    *elements : int
+    k : `int`
+        The order of the convergent. Must be a non-negative integer less than
+        the number of elements.
+
+    *elements : `int`
         A variable-length sequence of integer elements of a continued fraction.
 
     Returns
     -------
     fractions.Fraction
         A rational fraction constructed from the given sequence of elements of
-        a continued fraction.
+        a continued fraction, representing the :math:`k`-order convergent of a
+        (finite) simple continued fraction as given by a sequence of elements.
 
     Raises
     ------
     ValueError
-        If any elements are not integers.
+        If :math:`k` is not a non-negative integer less than the number of
+        elements, or if any of the elements are not integers.
 
     Examples
     --------
-    >>> fraction_from_elements(3, 4, 12, 4)
+    >>> convergent(0, 3, 4, 12, 4)
+    Fraction(3, 1)
+    >>> convergent(1, 3, 4, 12, 4)
+    Fraction(13, 4)
+    >>> convergent(2, 3, 4, 12, 4)
+    Fraction(159, 49)
+    >>> convergent(3, 3, 4, 12, 4)
     Fraction(649, 200)
+    >>> convergent(-1, 3, 4, 12, 4)
+    Traceback (most recent call last):
+    ...
+    ValueError: `k` must be a non-negative integer less than the number of
+    elements of the continued fraction.
+    >>> convergent(4, 3, 4, 12, 4)
+    Traceback (most recent call last):
+    ...
+    ValueError: `k` must be a non-negative integer less than the number of
+    elements of the continued fraction.
+    """
+    if not isinstance(k, int) or k < 0 or k >= len(elements) or any(not isinstance(e, int) for e in elements):
+        raise ValueError(
+            "`k` must be a non-negative integer less than the number of\n"
+            "elements of the continued fraction."
+        )
 
-    >>> fraction_from_elements(-4, 1, 3, 12, 4)
-    Fraction(-649, 200)
+    a, b = elements[0], 1
+    
+    if k == 0:
+        return Fraction(a, b)
 
-    >>> fraction_from_elements(4, 2, 6, 7)
-    Fraction(415, 93)
+    c, d = (elements[1] * a) + b, elements[1]
 
-    >>> fraction_from_elements(*[4, 2, 6, 7])
-    Fraction(415, 93)
+    if k == 1:
+        return Fraction(c, d)
 
-    >>> fraction_from_elements(4.5, 2, 6, 7)
-    Traceback (most recent call last):
-    ...
-    ValueError: Continued fraction elements must be integers
-    """
-    if any(not isinstance(elem, int) for elem in elements):
-        raise ValueError("Continued fraction elements must be integers")
+    for e in elements[2:k + 1]:
+        p, q = (e * c) + a, (e * d) + b
+        a, b = c, d
+        c, d = p, q
 
-    return Fraction(
-        deque(
-            accumulate(reversed(elements), func=lambda x, y: Fraction(1, x) + y)
-        ).pop()
-    )
+    return Fraction(p, q)
 
 
-def convergent(*elements: int, k: int = 1) -> Fraction:
-    """
-    Returns a `fractions.Fraction` object representing the `k`-th convergent of
-    a (finite) continued fraction given by an ordered sequence of its (integer)
-    elements.
-    
-    The integer `k` is called the order of the convergent, and a continued
-    fraction of order `n` has exactly `n + 1` convergents of orders `0`, `1`,
-    ... `n`.
-
-    Each convergent has its own continued fraction representation, which occurs
-    as a partial sum in the continued fraction representation of the number
-    represented by the continued fraction given by the element sequence.
+def fraction_from_elements(*elements: int) -> Fraction:
+    """Returns the rational number represented by a simple (finite) continued fraction from a sequence of its elements.
 
-    It is assumed that `k` < the number of elements, otherwise a `ValueError`
-    is raised.
+    The elements must be given as positional arguments, which means that if
+    they are contained in an iterable then they must be unpacked using the
+    unpacking operator ``*``, as described in the examples below.
 
     Parameters
     ----------
-    *elements : int
-        A variable-length sequence of integer elements of a continued fraction.
-
-    k : int, default=1
-        The order of the convergent.
+    *elements : `int`
+        A variable-length sequence of integer elements of a simple continued
+        fraction.
 
     Returns
     -------
     fractions.Fraction
-        A rational fraction constructed from the given sequence of elements of
-        a continued fraction, representing the `k`-order convergent of a
-        (finite) continued fraction represented by the given element sequence.
+        A rational number constructed from a sequence of elements of a simple
+        continued fraction which represents the number.
 
     Raises
     ------
     ValueError
-        If `k` < the number of elements.
+        If any of the elements are not integers.
 
     Examples
     --------
-    >>> convergent(3, 4, 12, 4, k=0)
-    Fraction(3, 1)
+    >>> fraction_from_elements(3, 4, 12, 4)
+    Fraction(649, 200)
+    >>> fraction_from_elements(-4, 1, 3, 12, 4)
+    Fraction(-649, 200)
+    >>> fraction_from_elements(4, 2, 6, 7)
+    Fraction(415, 93)
+    >>> fraction_from_elements(*[4, 2, 6, 7])
+    Fraction(415, 93)
+    >>> fraction_from_elements(4.5, 2, 6, 7)
+    Traceback (most recent call last):
+    ...
+    ValueError: Continued fraction elements must be integers
+    """
+    if any(not isinstance(elem, int) for elem in elements):
+        raise ValueError("Continued fraction elements must be integers")
 
-    >>> convergent(3, 4, 12, 4, k=1)
-    Fraction(13, 4)
+    return convergent(len(elements) - 1, *elements)
 
-    >>> convergent(3, 4, 12, 4, k=2)
-    Fraction(159, 49)
 
-    >>> convergent(3, 4, 12, 4, k=3)
-    Fraction(649, 200)
+def mediant(r: Fraction, s: Fraction, /, *, dir: str = 'right', k: int = 1) -> Fraction:
+    """Returns the :math:`k`-th left- or right-mediant of two rational numbers.
 
-    >>> convergent(3, 4, 12, 4, k=-1)
-    Traceback (most recent call last):
-    ...
-    ValueError: `k` must be a non-negative integer less than the number of elements of the continued fraction
+    For a positive integer :math:`k`, the :math:`k`-th left-mediant of two
+    rational numbers :math:`r = \\frac{a}{b}` and :math:`s = \\frac{c}{d}`,
+    where :math:`b, d, b + d \\neq 0`, is defined as:
+    
+    .. math::
 
-    >>> convergent(3, 4, 12, 4, k=4)
-    Traceback (most recent call last):
-    ...
-    ValueError: `k` must be a non-negative integer less than the number of elements of the continued fraction
-    """
-    if not isinstance(k, int) or k < 0 or k >= len(elements):
-        raise ValueError(
-            "`k` must be a non-negative integer less than the number of "
-            "elements of the continued fraction"
-        )
+       \\frac{ka + c}{kb + d}, \\hskip{3em}    k \\geq 1
 
-    return fraction_from_elements(*elements[:k + 1])
+    while the :math:`k`-th right mediant is defined as:
+    
+    .. math::
 
+       \\frac{a + kc}{b + kd}, \\hskip{3em}    k \\geq 1
 
-def mediant(r: Fraction, s: Fraction, /, *, dir='right', k: int = 1) -> Fraction:
-    """
-    Returns the `k`-th left- or right-mediant of two rational numbers, given as
-    `fractions.Fraction` objects.
+    If we assume that :math:`r < s` and :math:`bd > 0` then these mediants
+    have the property that:
+   
+    .. math::
+
+       \\frac{a}{b} < \\frac{ka + c}{kb + d} \\leq \\frac{a + kc}{b + kd} < \\frac{c}{d},   \\hskip{3em} k \\geq 1
+
+    where equality holds for :math:`k = 1`. If we let :math:`k \\to \\infty`
+    then the mediants converge to opposite limits:
 
-    For a positive integer `k`, the `k`-th left-mediant of rational numbers
-    `r = a / b` and `s = c / d`, where `b` and `d` are non-zero, can be defined
-    as:
-    ::
-
-        (ka + c) / (kb + d)
-
-    while the `k`-th right mediant can be defined as:
-    ::
-
-        (a + kc) / (b + kd)
-
-    If we assume that `r < s` and `bd > 0` then the `k`-th left mediants have
-    the property that:
-    ::
-        a / b < ... < (3a + c) / (3b + d) < (2a + c) / (2b + d) < (a + c) / (b + d) < c / d
-        a / b < (a + c) / (b + d) < (a + 2c) / (b + 2d) < (a + 3c) / (b + 3d) < ... c / d
-
-    That is, the left mediants form a strictly decreasing sequence, actually
-    converging to `a / b`, while the right mediants form a strictly increasing
-    sequence of, actually converging to `c / d`.
-
-    For the left mediant use `dir='left'`, while for the right use
-    `dir='right'`. The default is `dir='right'`. For `k = 1` the left and right
-    mediants are the same.
+    .. math::
+
+      \\begin{align}
+      \\lim_{k \\to \\infty} \\frac{ka + c}{kb + d} &= \\frac{a}{b} \\\\
+      \\lim_{k \\to \\infty} \\frac{a + kc}{b + kd} &= \\frac{c}{d}
+      \\end{align}
+
+    For more information consult the
+    `documentation <https://continuedfractions.readthedocs.io/en/latest/sources/mediants.html>`_.
+
+    For the left mediant use ``dir="left"``, while for the right use
+    ``dir="right"``. The default is ``dir="right"``. For ``k = 1`` the left and
+    right mediants are identical to the simple mediant :math:`\\frac{a + c}{b + d}`.
 
     Parameters
     ----------
-    r : fractions.Fraction
+    r : `fractions.Fraction`
         The first rational number.
 
-    s : fractions.Fraction
+    s : `fractions.Fraction`
         The second rational number.
 
-    dir : str, default='right'
+    dir : `str`, default='right'
         The "direction" of the mediant - `'left'` or `'right'`, as defined
         above.
 
-    k : int, default=1
+    k : `int`, default=1
         The order of the mediant, as defined above.
 
     Returns
     -------
     fractions.Fraction
         The `k`-th left- or right-mediant of the two given rational numbers.
 
@@ -380,14 +439,25 @@
 
     if dir == 'left':
         return Fraction(k * a + c, k * b + d)
 
     return Fraction(a + k * c, b + k * d)
 
 
+#: A :py:func:`functools.partial` binding of :py:func:`mediant` for left-mediants.
+left_mediant = functools.partial(mediant, dir="left")
+
+
+#: A :py:func:`functools.partial` binding of :py:func:`mediant` for right-mediants.
+right_mediant = functools.partial(mediant, dir="right")
+
+
 if __name__ == "__main__":      # pragma: no cover
     # Doctest the module from the project root using
     #
     #     python -m doctest -v src/continuedfractions/lib.py
     #
+    # NOTE: the doctest examples using where `float` or ``decimal.Decimal``
+            # values assume a context precision of 28 digits
+    decimal.getcontext().prec = 28
     import doctest
     doctest.testmod()
```

### Comparing `continuedfractions-0.11.9/PKG-INFO` & `continuedfractions-0.12.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: continuedfractions
-Version: 0.11.9
-Summary: Continued fractions with Python
-Keywords: continued fractions rational numbers real numbers irrational numbers approximation
-Author-Email: S. R. Murthy <s.murthy@tutanota.com>
-Maintainer-Email: S. R. Murthy <s.murthy@tutanota.com>
+Version: 0.12.0
+Summary: Object-oriented continued fractions with Python.
+Keywords: computational number theory,coprime integers,continued fractions,farey sequences,irrational numbers,mediants,number theory,rational approximation,rational numbers,real numbers
+Author-Email: "S. R. Murthy" <s.murthy@tutanota.com>
+Maintainer-Email: "S. R. Murthy" <s.murthy@tutanota.com>
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
         
         1.1. "Contributor"
@@ -374,57 +374,66 @@
         You may add additional accurate notices of copyright ownership.
         
         Exhibit B - "Incompatible With Secondary Licenses" Notice
         ---------------------------------------------------------
         
           This Source Code Form is "Incompatible With Secondary Licenses", as
           defined by the Mozilla Public License, v. 2.0.
-Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Project-URL: Homepage, https://github.com/sr-murthy/continuedfractions
-Project-URL: Documentation, https://continuedfractions.readthedocs.io/en/latest
+Project-URL: Documentation, https://continuedfractions.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/sr-murthy/continuedfractions
 Requires-Python: >=3.10
 Provides-Extra: user
 Requires-Dist: jupyter; extra == "user"
 Description-Content-Type: text/markdown
 
 <div align="center">
   
 [![CI](https://github.com/sr-murthy/continuedfractions/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/sr-murthy/continuedfractions/actions/workflows/ci.yml)
+[![CodeQL Analysis](https://github.com/sr-murthy/continuedfractions/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/sr-murthy/continuedfractions/actions/workflows/codeql-analysis.yml)
 [![Codecov](https://codecov.io/gh/sr-murthy/continuedfractions/graph/badge.svg?token=GWQ08T4P5J)](https://codecov.io/gh/sr-murthy/continuedfractions)
-[![PyPI version](https://badge.fury.io/py/continuedfractions.svg)](https://badge.fury.io/py/continuedfractions)
 [![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm-project.org)
 [![License: MPL
 2.0](https://img.shields.io/badge/License-MPL_2.0-brightgreen.svg)](https://opensource.org/licenses/MPL-2.0)
 [![Docs](https://readthedocs.org/projects/continuedfractions/badge/?version=latest)](https://continuedfractions.readthedocs.io/en/latest/?badge=latest)
 <a href="https://trackgit.com">
 <img src="https://us-central1-trackgit-analytics.cloudfunctions.net/token/ping/lsudelfvcxb7f1xm6i4l" alt="trackgit-views" />
 </a>
+[![PyPI version](https://badge.fury.io/py/continuedfractions.svg)](https://badge.fury.io/py/continuedfractions)
 [![Downloads](https://static.pepy.tech/badge/continuedfractions/week)](https://pepy.tech/project/continuedfractions)
 
 </div>
 
 # continuedfractions
 
 A simple extension of the Python [`fractions`](https://docs.python.org/3/library/fractions.html) standard library for working with [continued fractions](https://en.wikipedia.org/wiki/Continued_fraction) as Python objects.
 
+The [PyPI package](https://pypi.org/project/continuedfractions/) only uses standard libraries and can be installed on any **Linux**, **Mac OS** or **Windows** system supporting **Python 3.10**, **3.11**, or **3.12**.
+```shell
+pip install continuedfractions
+```
+
+See the [project docs](https://continuedfractions.readthedocs.io/en/latest/) for more details, which includes the [API reference](https://continuedfractions.readthedocs.io/en/latest/sources/api-reference.html).
+
 [Continued fractions](https://en.wikipedia.org/wiki/Continued_fraction) are beautiful and interesting mathematical objects, with many connections in [number theory](https://en.wikipedia.org/wiki/Number_theory) and also very useful practical applications, including the [rational approximation of real numbers](https://en.wikipedia.org/wiki/Continued_fraction#Best_rational_approximations).
 
 The `continuedfractions` package is designed to:
 
-* make it easy to construct (finite) continued fractions as Python objects
+* make it easy to work with (finite) continued fractions as Python objects
 * explore their key properties, such as elements/coefficients, convergents, segments, remainders, and others
 * operate on them as rationals and instances of the standard library [`fractions.Fraction`](https://docs.python.org/3/library/fractions.html#fractions.Fraction) class
+* support approximations and experimental computations for irrational numbers
+* explore other objects related to continued fractions, such as mediants, sequences of coprime integers, and Farey sequences
 
 The project is [licensed](LICENSE) under the [Mozilla Public License 2.0](https://opensource.org/licenses/MPL-2.0).
 
-See the [project docs](https://continuedfractions.readthedocs.io/en/latest) for more details.
+
```

