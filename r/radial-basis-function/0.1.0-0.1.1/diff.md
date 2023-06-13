# Comparing `tmp/radial_basis_function-0.1.0.tar.gz` & `tmp/radial_basis_function-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radial_basis_function-0.1.0.tar", max compression
+gzip compressed data, was "radial_basis_function-0.1.1.tar", max compression
```

## Comparing `radial_basis_function-0.1.0.tar` & `radial_basis_function-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      605 2023-06-13 07:26:51.422763 radial_basis_function-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      142 2023-06-13 06:43:23.447317 radial_basis_function-0.1.0/radial_basis_function/__init__.py
--rw-r--r--   0        0        0     1652 2023-06-13 05:31:49.224159 radial_basis_function-0.1.0/radial_basis_function/pseudo_inversa.py
--rw-r--r--   0        0        0     5367 2023-06-13 05:34:34.426617 radial_basis_function-0.1.0/radial_basis_function/rbf.py
--rw-r--r--   0        0        0       46 2023-06-13 06:44:22.333854 radial_basis_function-0.1.0/README.md
--rw-r--r--   0        0        0      679 1970-01-01 00:00:00.000000 radial_basis_function-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      605 2023-06-13 09:16:03.814602 radial_basis_function-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      142 2023-06-13 09:16:08.875203 radial_basis_function-0.1.1/radial_basis_function/__init__.py
+-rw-r--r--   0        0        0     1652 2023-06-13 05:31:49.224159 radial_basis_function-0.1.1/radial_basis_function/pseudo_inversa.py
+-rw-r--r--   0        0        0     5368 2023-06-13 09:02:03.281223 radial_basis_function-0.1.1/radial_basis_function/rbf.py
+-rw-r--r--   0        0        0       46 2023-06-13 06:44:22.333854 radial_basis_function-0.1.1/README.md
+-rw-r--r--   0        0        0      679 1970-01-01 00:00:00.000000 radial_basis_function-0.1.1/PKG-INFO
```

### Comparing `radial_basis_function-0.1.0/pyproject.toml` & `radial_basis_function-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "radial-basis-function"
-version = "0.1.0"
+version = "0.1.1"
 description = "Radial Basis Function e Multiplicação de Matriz Pseudo-Inversa, para modelos de Regressão e Multi-Classificatórios."
 authors = ["Victor Venites <contato@victorvenites.com>"]
 readme = "README.md"
 packages = [{include = "radial_basis_function"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `radial_basis_function-0.1.0/radial_basis_function/pseudo_inversa.py` & `radial_basis_function-0.1.1/radial_basis_function/pseudo_inversa.py`

 * *Files identical despite different names*

### Comparing `radial_basis_function-0.1.0/radial_basis_function/rbf.py` & `radial_basis_function-0.1.1/radial_basis_function/rbf.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Classe e métodos para implementar a Regressão por Radial Basis Function
 
 Original Author: Victor Venites
 """
 
 import numpy as np
 import pandas as pd
-from pseudo_inversa import PseudoInversa
+from .pseudo_inversa import PseudoInversa
 
 
 class RadialBasisFunction:
     """Radial Basis Function
     Original Author: Victor Venites
     """
     def __init__(self, funcao = 'Gaussiana',
```

### Comparing `radial_basis_function-0.1.0/PKG-INFO` & `radial_basis_function-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radial-basis-function
-Version: 0.1.0
+Version: 0.1.1
 Summary: Radial Basis Function e Multiplicação de Matriz Pseudo-Inversa, para modelos de Regressão e Multi-Classificatórios.
 Author: Victor Venites
 Author-email: contato@victorvenites.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

