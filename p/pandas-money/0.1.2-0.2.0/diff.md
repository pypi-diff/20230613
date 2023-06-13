# Comparing `tmp/pandas_money-0.1.2.tar.gz` & `tmp/pandas_money-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas_money-0.1.2.tar", max compression
+gzip compressed data, was "pandas_money-0.2.0.tar", max compression
```

## Comparing `pandas_money-0.1.2.tar` & `pandas_money-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1070 2023-06-09 03:17:36.171096 pandas_money-0.1.2/LICENSE
--rw-r--r--   0        0        0      857 2023-06-12 06:16:13.622825 pandas_money-0.1.2/README.md
--rw-r--r--   0        0        0      152 2023-06-12 00:16:34.192150 pandas_money-0.1.2/pandas_money/__init__.py
--rw-r--r--   0        0        0     7411 2023-06-12 03:40:40.766131 pandas_money-0.1.2/pandas_money/money_dtype.py
--rw-r--r--   0        0        0        0 2023-06-12 04:25:47.563979 pandas_money-0.1.2/pandas_money/tests/__init__.py
--rw-r--r--   0        0        0    10506 2023-06-12 03:34:06.593176 pandas_money-0.1.2/pandas_money/tests/test_money_dtype.py
--rw-r--r--   0        0        0     1434 2023-06-12 06:16:29.822713 pandas_money-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1543 1970-01-01 00:00:00.000000 pandas_money-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-09 03:17:36.171096 pandas_money-0.2.0/LICENSE
+-rw-r--r--   0        0        0      859 2023-06-12 22:53:26.115878 pandas_money-0.2.0/README.md
+-rw-r--r--   0        0        0      152 2023-06-12 00:16:34.192150 pandas_money-0.2.0/pandas_money/__init__.py
+-rw-r--r--   0        0        0     8531 2023-06-12 22:53:26.115878 pandas_money-0.2.0/pandas_money/money_dtype.py
+-rw-r--r--   0        0        0        0 2023-06-12 04:25:47.563979 pandas_money-0.2.0/pandas_money/tests/__init__.py
+-rw-r--r--   0        0        0    12730 2023-06-12 23:58:17.114508 pandas_money-0.2.0/pandas_money/tests/test_money_dtype.py
+-rw-r--r--   0        0        0     1434 2023-06-12 22:53:26.115878 pandas_money-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1545 1970-01-01 00:00:00.000000 pandas_money-0.2.0/PKG-INFO
```

### Comparing `pandas_money-0.1.2/LICENSE` & `pandas_money-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pandas_money-0.1.2/README.md` & `pandas_money-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -10,44 +10,46 @@
 or with pip/pipenv
 ```
 pipenv install pandas-money
 ```
 
 ### Example
 ```py
+from decimal import Decimal
+
 import pandas as pd
+
 import pandas_money as pm
-from decimal import Decimal
 
-s = pd.Series(["1.11", "2.22", "3.33"], dtype="money64")
+s = pd.Series(["1.11", "2.22", "3.33"], dtype="Money64")
 
 print(s)
 print(s + s)
 print(s * Decimal("1.5"))
 print(s / 2)
 print(s.iloc[0], type(s.iloc[0]))
 ```
 outputs
 ```
 0    $1.11
 1    $2.22
 2    $3.33
-dtype: money64
+dtype: Money64
 0    $2.22
 1    $4.44
 2    $6.66
-dtype: money64
+dtype: Money64
 0    $1.66
 1    $3.33
 2    $5.00
-dtype: money64
+dtype: Money64
 0    $0.56
 1    $1.11
 2    $1.66
-dtype: money64
+dtype: Money64
 $1.11 <class 'moneyed.classes.Money'>
 ```
 
 ## Setup
 - Clone repo
 - `poetry install`
```

### Comparing `pandas_money-0.1.2/pandas_money/money_dtype.py` & `pandas_money-0.2.0/pandas_money/money_dtype.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,92 +1,107 @@
 from decimal import Decimal
 
 import numpy as np
 import pandas as pd
 from moneyed import USD, Money
+from pandas._libs.hashtable import object_hash  # type: ignore[import]
+from pandas._libs.missing import NAType
 from pandas._typing import Dtype
+from pandas._typing import Scalar as InputScalar
 from pandas.api.extensions import (
     ExtensionArray,
     ExtensionScalarOpsMixin,
     register_extension_dtype,
 )
 from pandas.core.dtypes.base import ExtensionDtype
 from pandas.core.dtypes.common import is_dtype_equal, pandas_dtype
 from pandas.core.dtypes.dtypes import PandasExtensionDtype
 
 money_decimals = 2
 money_factor = 10**money_decimals
 decimal_quantize = Decimal(f".{'0'*(money_decimals-1)}1")
 
-InputScalar = int | Money | Decimal | str | float | np.integer | np.floating
-
 
 @register_extension_dtype
 class MoneyDtype(PandasExtensionDtype):
     """DType class for MoneyArray extension"""
 
     type = Money
-    name = "money64"
+    name = "Money64"
+    _metadata: tuple[str, ...] = ()
 
     @classmethod
     def construct_array_type(cls):
         """
         Return array type associated with this dtype
         """
         return MoneyArray
 
+    def __hash__(self) -> int:
+        # for python>=3.10, different nan objects have different hashes
+        # we need to avoid that and thus use hash function with old behavior
+        return object_hash(tuple(getattr(self, attr) for attr in self._metadata))
+
 
 class MoneyArray(ExtensionScalarOpsMixin, ExtensionArray):
     """A Pandas ExtensionArray of int64 for fixed decimal currency math
 
     Operator type rules
 
     MoneyArray ± (MoneyArray | Money) = MoneyArray
     MoneyArray * (int | float | Decimal | Iterable[int | float | Decimal]) = MoneyArray
     MoneyArray / (int | float | Decimal | Iterable[int | float | Decimal]) = MoneyArray
     MoneyArray / (MoneyArray | Money) = FloatArray
     """
 
     def __init__(self, values, copy=False, to_cents=True):
-        self.values = np.array(
-            [self._clean_value(v, to_cents) for v in values], dtype=np.int64
+        self.values = pd.array(
+            [self._clean_value(v, to_cents) for v in values],
+            dtype=pd.Int64Dtype(),
         )
 
-    def _clean_value(self, v: InputScalar, to_cents: bool) -> int | Decimal:
+    def _clean_value(
+        self, v: InputScalar | NAType, to_cents: bool
+    ) -> int | Decimal | NAType:
+        if pd.isna(v):
+            return pd.NA
+
         factor = money_factor if to_cents else 1
         round_to = money_decimals if to_cents else 0
-
         cleaned: int | np.integer | Decimal
         if isinstance(v, (int, np.integer)):
             cleaned = v
         elif isinstance(v, Money):
             cleaned = v.amount
         elif isinstance(v, Decimal):
             cleaned = round(v, round_to)
         elif isinstance(v, str):
             cleaned = round(Decimal(v), round_to)
         elif isinstance(v, (float, np.floating)):
             cleaned = round(Decimal(float(v)), round_to)
         else:
-            raise TypeError(f"{v} cannot be converted to a Money type")
+            raise TypeError(f"{type(v)} cannot be converted to a Money type")
         return factor * cleaned
 
     @classmethod
     def _from_sequence(cls, scalars, *, dtype: Dtype | None = None, copy: bool = False):
         return MoneyArray(scalars, copy=copy)
 
     @classmethod
     def _from_sequence_of_strings(
         cls, strings, *, dtype: Dtype | None = None, copy: bool = False
     ):
         return cls._from_sequence(strings, dtype=dtype, copy=copy)
 
     def __getitem__(self, item):
         if isinstance(item, int):
-            return Money(self.values[item], USD) / money_factor
+            val = self.values[item]
+            if pd.isna(val):
+                return val
+            return Money(val, USD) / money_factor
         else:
             return MoneyArray(self.values[item], to_cents=False)
 
     def __eq__(self, other):
         if isinstance(other, (pd.Index, pd.Series, pd.DataFrame)):
             return NotImplemented
         if not isinstance(other, MoneyArray):
@@ -98,18 +113,18 @@
         return MoneyDtype()
 
     @property
     def nbytes(self):
         return self.values.nbytes
 
     def __len__(self):
-        return self.values.size
+        return len(self.values)
 
     def isna(self):
-        return np.isnan(self.values)
+        return pd.isna(self.values)
 
     def take(self, indices, *, allow_fill=False, fill_value=None):
         from pandas.core.algorithms import take
 
         if allow_fill and fill_value is None:
             fill_value = self.dtype.na_value
 
@@ -118,95 +133,109 @@
             indices,
             fill_value=fill_value,
             allow_fill=allow_fill,
         )
         return MoneyArray(result, to_cents=False)
 
     def copy(self):
-        return MoneyArray(np.copy(self.values))
+        return MoneyArray(self.values.copy(), to_cents=False)
 
     @classmethod
     def _concat_same_type(cls, to_concat):
         return MoneyArray(np.concatenate(to_concat))
 
     def astype(self, dtype, copy: bool = True):
         dtype = pandas_dtype(dtype)
         if is_dtype_equal(dtype, self.dtype):
             if not copy:
                 return self
             else:
                 return self.copy()
 
-        decimals = [Decimal(int(v)) / money_factor for v in self.values]
+        decimals = [
+            v if pd.isna(v) else Decimal(int(v)) / money_factor for v in self.values
+        ]
 
         if isinstance(dtype, ExtensionDtype):
             cls = dtype.construct_array_type()
-            return cls._from_sequence(decimals, dtype=dtype, copy=False)  # type: ignore
+            return cls._from_sequence(decimals, dtype=dtype, copy=False)  # type: ignore[attr-defined]
 
-        return np.array(decimals, dtype=dtype, copy=False)
+        return pd.array(decimals, dtype=dtype, copy=False)
 
     def __add__(self, other):
         if isinstance(other, Money):
             return MoneyArray(
-                self.values + np.int64(other.amount * money_factor),
+                self.values + other.amount * money_factor,
                 to_cents=False,
             )
         elif isinstance(other, MoneyArray) and len(self) == len(other):
-            return MoneyArray(self.values + other.values, to_cents=False)
+            return MoneyArray(self.values + other.values, to_cents=False)  # type: ignore[operator]
         else:
             raise TypeError(f"Cannot add money to {other}")
 
     def __radd__(self, other):
-        raise NotImplemented
+        raise NotImplemented  # noqa: F901
 
     def __sub__(self, other):
         if isinstance(other, Money):
             return MoneyArray(
-                self.values - np.int64(other.amount * money_factor),
+                self.values - int(other.amount * money_factor),  # type: ignore[operator]
                 to_cents=False,
             )
         elif isinstance(other, MoneyArray) and len(self) == len(other):
-            return MoneyArray(self.values - other.values, to_cents=False)
+            return MoneyArray(self.values - other.values, to_cents=False)  # type: ignore[operator]
         else:
             raise TypeError(f"Cannot subtract money with {other}")
 
     def __rsub__(self, other):
-        raise NotImplemented
+        raise NotImplemented  # noqa: F901
 
     def __mul__(self, other):
         if isinstance(other, (Money, MoneyArray)):
             raise TypeError(f"Cannot multiply money by money {other}")
         elif isinstance(other, Decimal):
-            return MoneyArray(self.values * float(other), to_cents=False)
+            return MoneyArray(self.values * float(other), to_cents=False)  # type: ignore[operator]
         elif isinstance(other, (np.number, int, float)):
-            return MoneyArray(self.values * other, to_cents=False)
-        elif isinstance(other, (list, np.ndarray)) and len(self) == len(other):
-            return MoneyArray(self.values * other, to_cents=False)
+            return MoneyArray(self.values * other, to_cents=False)  # type: ignore[operator,arg-type]
+        elif isinstance(other, (list, np.ndarray, ExtensionArray)) and len(self) == len(
+            other
+        ):
+            return MoneyArray(self.values * other, to_cents=False)  # type: ignore[operator]
         else:
             raise TypeError(f"Cannot multiply money by {other}")
 
     def __rmul__(self, other):
-        raise NotImplemented
+        raise NotImplemented  # noqa: F901
 
     def __truediv__(self, other):
         if isinstance(other, Money):
-            return self.values / (np.float64(other.amount) * money_factor)
+            return self.values / float(other.amount * money_factor)  # type: ignore[operator]
         elif isinstance(other, MoneyArray) and len(self) == len(other):
-            return self.values / other.values.astype(np.float64)
+            return self.values / other.values.astype("Float64")
         elif isinstance(other, Decimal):
-            return MoneyArray(self.values / np.float64(float(other)), to_cents=False)
+            return MoneyArray(
+                self.values / float(other),  # type: ignore[operator]
+                to_cents=False,
+            )
         elif isinstance(other, (np.number, int, float)):
-            return MoneyArray(self.values / np.float64(other), to_cents=False)
-        elif isinstance(other, (list, np.ndarray)) and len(self) == len(other):
-            return MoneyArray(self.values / other, to_cents=False)
+            return MoneyArray(
+                self.values / float(other),  # type: ignore[operator]
+                to_cents=False,
+            )
+        elif isinstance(other, (list, np.ndarray, ExtensionArray)) and len(self) == len(
+            other
+        ):
+            return MoneyArray(
+                self.values / other, to_cents=False  # type: ignore[operator]
+            )
         else:
             raise TypeError(f"Cannot divide money by {other}")
 
     def __rtruediv__(self, other):
-        raise NotImplemented
+        raise NotImplemented  # noqa: F901
 
 
 ops_overrides = [
     "eq",
     "add",
     "radd",
     "sub",
```

### Comparing `pandas_money-0.1.2/pandas_money/tests/test_money_dtype.py` & `pandas_money-0.2.0/pandas_money/tests/test_money_dtype.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import contextlib
+import io
+import re
 import string
 from decimal import Decimal, InvalidOperation
 
 import numpy as np
 import pandas as pd
 import pytest
 from moneyed import USD, Money
@@ -57,260 +60,260 @@
     return 314
 
 
 @pytest.fixture
 def slice_series():
     return pd.Series(
         {label: i for i, label in enumerate(string.ascii_lowercase[:10])},
-        dtype="money64",
+        dtype="Money64",
     )
 
 
 def test_money_dict(money_dict):
-    m = pd.Series(money_dict, dtype="money64")
+    m = pd.Series(money_dict, dtype="Money64")
     assert isinstance(m.dtype, pm.MoneyDtype)
     assert m["a"] == money_dict["a"]
     assert m["b"] == money_dict["b"]
 
 
 def test_money_list(money_list):
-    m = pd.Series(money_list, dtype="money64")
+    m = pd.Series(money_list, dtype="Money64")
     assert isinstance(m.dtype, pm.MoneyDtype)
     assert m.iloc[0] == money_list[0]
     assert m.iloc[1] == money_list[1]
 
 
 def test_money_scalar(money_scalar):
-    m = pd.Series(money_scalar, dtype="money64")
+    m = pd.Series(money_scalar, dtype="Money64")
     assert isinstance(m.dtype, pm.MoneyDtype)
     assert m.iloc[0] == money_scalar
 
 
 def test_decimal_scalar(decimal_scalar):
-    m = pd.Series(decimal_scalar, dtype="money64")
+    m = pd.Series(decimal_scalar, dtype="Money64")
     assert isinstance(m.dtype, pm.MoneyDtype)
     assert m.iloc[0] == Money(decimal_scalar, USD)
 
 
 def test_str_scalar(str_scalar):
-    m = pd.Series(str_scalar, dtype="money64")
+    m = pd.Series(str_scalar, dtype="Money64")
     assert isinstance(m.dtype, pm.MoneyDtype)
     assert m.iloc[0] == Money(str_scalar, USD)
 
 
 def test_int_scalar(int_scalar):
-    m = pd.Series(int_scalar, dtype="money64")
+    m = pd.Series(int_scalar, dtype="Money64")
     assert isinstance(m.dtype, pm.MoneyDtype)
     assert m.iloc[0] == Money(int_scalar, USD)
 
 
 def test_rounding():
     down = Decimal("1.444999")
     up = Decimal("1.445000")
-    m = pd.Series([down, up], dtype="money64")
+    m = pd.Series([down, up], dtype="Money64")
     assert m.iloc[0] == Money(down.quantize(Decimal(".01")), USD)
     assert m.iloc[1] == Money(up.quantize(Decimal(".01")), USD)
 
 
 def test_add_money(money_list, money_scalar):
-    m1 = pd.Series(money_list, dtype="money64")
+    m1 = pd.Series(money_list, dtype="Money64")
     m2 = money_scalar
     m = m1 + m2
     assert isinstance(m.dtype, pm.MoneyDtype)
     assert m.iloc[0] == money_list[0] + money_scalar
     assert m.iloc[1] == money_list[1] + money_scalar
 
 
 def test_add_money_array(money_list):
-    m1 = pd.Series(money_list, dtype="money64")
-    m2 = pd.Series(money_list, dtype="money64")
+    m1 = pd.Series(money_list, dtype="Money64")
+    m2 = pd.Series(money_list, dtype="Money64")
     m = m1 + m2
     assert isinstance(m.dtype, pm.MoneyDtype)
     assert m.iloc[0] == money_list[0] + money_list[0]
     assert m.iloc[1] == money_list[1] + money_list[1]
 
 
 def test_sub_money(money_list, money_scalar):
-    m1 = pd.Series(money_list, dtype="money64")
+    m1 = pd.Series(money_list, dtype="Money64")
     m2 = money_scalar
     m = m1 - m2
     assert isinstance(m.dtype, pm.MoneyDtype)
     assert m.iloc[0] == money_list[0] - money_scalar
     assert m.iloc[1] == money_list[1] - money_scalar
 
 
 def test_sub_money_array(money_list):
-    m1 = pd.Series(money_list, dtype="money64")
-    m2 = pd.Series(money_list, dtype="money64")
+    m1 = pd.Series(money_list, dtype="Money64")
+    m2 = pd.Series(money_list, dtype="Money64")
     m = m1 - m2
     assert isinstance(m.dtype, pm.MoneyDtype)
     assert m.iloc[0] == money_list[0] - money_list[0]
     assert m.iloc[1] == money_list[1] - money_list[1]
 
 
 def test_mul_money_array_money_array(money_list):
-    m1 = pd.Series(money_list, dtype="money64")
+    m1 = pd.Series(money_list, dtype="Money64")
     with pytest.raises(TypeError):
         m1 * m1
 
 
 def test_mul_money_array_money(money_list, money_scalar):
-    m1 = pd.Series(money_list, dtype="money64")
+    m1 = pd.Series(money_list, dtype="Money64")
     with pytest.raises(TypeError):
         m1 * money_scalar
 
 
 def test_mul_money_array_decimal_array(money_list, decimal_list):
-    m1 = pd.Series(money_list, dtype="money64")
+    m1 = pd.Series(money_list, dtype="Money64")
     m2 = pd.Series(decimal_list)
     m = m1 * m2
     assert isinstance(m.dtype, pm.MoneyDtype)
     assert m.iloc[0] == (money_list[0] * decimal_list[0]).round(pm.money_decimals)
     assert m.iloc[1] == (money_list[1] * decimal_list[1]).round(pm.money_decimals)
 
 
 def test_mul_money_array_decimal(money_list, decimal_scalar):
-    m1 = pd.Series(money_list, dtype="money64")
+    m1 = pd.Series(money_list, dtype="Money64")
     m = m1 * decimal_scalar
     assert isinstance(m.dtype, pm.MoneyDtype)
     assert m.iloc[0] == (money_list[0] * decimal_scalar).round(pm.money_decimals)
     assert m.iloc[1] == (money_list[1] * decimal_scalar).round(pm.money_decimals)
 
 
 def test_mul_money_array_float_array(money_list, float_list):
-    m1 = pd.Series(money_list, dtype="money64")
+    m1 = pd.Series(money_list, dtype="Money64")
     m2 = pd.Series(float_list)
     m = m1 * m2
     assert isinstance(m.dtype, pm.MoneyDtype)
     # DeprecationWarning: Multiplying Money instances with floats is deprecated
     # so cast floats to Decimal
     assert m.iloc[0] == (money_list[0] * Decimal(float_list[0])).round(
         pm.money_decimals
     )
     assert m.iloc[1] == (money_list[1] * Decimal(float_list[1])).round(
         pm.money_decimals
     )
 
 
 def test_mul_money_array_float(money_list, float_scalar):
-    m1 = pd.Series(money_list, dtype="money64")
+    m1 = pd.Series(money_list, dtype="Money64")
     m = m1 * float_scalar
     assert isinstance(m.dtype, pm.MoneyDtype)
     # DeprecationWarning: Multiplying Money instances with floats is deprecated
     # so cast floats to Decimal
     assert m.iloc[0] == (money_list[0] * Decimal(float_scalar)).round(pm.money_decimals)
     assert m.iloc[1] == (money_list[1] * Decimal(float_scalar)).round(pm.money_decimals)
 
 
 def test_truediv_money_array_money_array(money_list):
-    m1 = pd.Series(money_list, dtype="money64")
-    m2 = pd.Series(reversed(money_list), dtype="money64")
+    m1 = pd.Series(money_list, dtype="Money64")
+    m2 = pd.Series(reversed(money_list), dtype="Money64")
     m = m1 / m2
-    assert np.issubdtype(m.dtype, np.floating)  # type: ignore
+    assert isinstance(m.dtype, pd.Float64Dtype)
     assert round(m.iloc[0], ratio_precision) == round(
         float(money_list[0].amount) / float(money_list[1].amount),
         ratio_precision,
     )
     assert round(m.iloc[1], ratio_precision) == round(
         float(money_list[1].amount) / float(money_list[0].amount),
         ratio_precision,
     )
 
 
 def test_truediv_money_array_money(money_list, money_scalar):
-    m1 = pd.Series(money_list, dtype="money64")
+    m1 = pd.Series(money_list, dtype="Money64")
     m = m1 / money_scalar
-    assert np.issubdtype(m.dtype, np.floating)
+    assert isinstance(m.dtype, pd.Float64Dtype)
     assert round(m.iloc[0], ratio_precision) == round(
         float(money_list[0].amount) / float(money_scalar.amount),
         ratio_precision,
     )
     assert round(m.iloc[1], ratio_precision) == round(
         float(money_list[1].amount) / float(money_scalar.amount),
         ratio_precision,
     )
 
 
 def test_truediv_money_array_decimal_array(money_list, decimal_list):
-    m1 = pd.Series(money_list, dtype="money64")
+    m1 = pd.Series(money_list, dtype="Money64")
     m2 = pd.Series(reversed(decimal_list))
     m = m1 / m2
     assert isinstance(m.dtype, pm.MoneyDtype)
     assert m.iloc[0] == (money_list[0] / decimal_list[1]).round(pm.money_decimals)
     assert m.iloc[1] == (money_list[1] / decimal_list[0]).round(pm.money_decimals)
 
 
 def test_truediv_money_array_decimal(money_list, decimal_scalar):
-    m1 = pd.Series(money_list, dtype="money64")
+    m1 = pd.Series(money_list, dtype="Money64")
     m = m1 / decimal_scalar
     assert isinstance(m.dtype, pm.MoneyDtype)
     assert m.iloc[0] == (money_list[0] / decimal_scalar).round(pm.money_decimals)
     assert m.iloc[1] == (money_list[1] / decimal_scalar).round(pm.money_decimals)
 
 
 def test_truediv_money_array_float_array(money_list, float_list):
-    m1 = pd.Series(money_list, dtype="money64")
+    m1 = pd.Series(money_list, dtype="Money64")
     m2 = pd.Series(reversed(float_list))
     m = m1 / m2
     assert isinstance(m.dtype, pm.MoneyDtype)
     # DeprecationWarning: Multiplying Money instances with floats is deprecated
     # so cast floats to Decimal
     assert m.iloc[0] == (money_list[0] / Decimal(float_list[1])).round(
         pm.money_decimals
     )
     assert m.iloc[1] == (money_list[1] / Decimal(float_list[0])).round(
         pm.money_decimals
     )
 
 
 def test_truediv_money_array_float(money_list, float_scalar):
-    m1 = pd.Series(money_list, dtype="money64")
+    m1 = pd.Series(money_list, dtype="Money64")
     m = m1 / float_scalar
     assert isinstance(m.dtype, pm.MoneyDtype)
     # DeprecationWarning: Multiplying Money instances with floats is deprecated
     # so cast floats to Decimal
     assert m.iloc[0] == (money_list[0] / Decimal(float_scalar)).round(pm.money_decimals)
     assert m.iloc[1] == (money_list[1] / Decimal(float_scalar)).round(pm.money_decimals)
 
 
 def test_badscalar():
     with pytest.raises(InvalidOperation):
-        pd.Series("asdf", dtype="money64")
+        pd.Series("asdf", dtype="Money64")
 
 
 def test_astype(money_list):
-    m1 = pd.Series(money_list, dtype="money64")
-    m = m1.astype(np.float64)
-    assert np.issubdtype(m.dtype, np.floating)
+    m1 = pd.Series(money_list, dtype="Money64")
+    m = m1.astype("Float64")
+    assert isinstance(m.dtype, pd.Float64Dtype)
     assert round(m.iloc[0], pm.money_decimals) == round(
         float(money_list[0].amount),
         pm.money_decimals,
     )
     assert round(m.iloc[1], pm.money_decimals) == round(
         float(money_list[1].amount),
         pm.money_decimals,
     )
 
 
 def test_eq(money_list):
-    m1 = pd.Series(money_list, dtype="money64")
-    m2 = pd.Series(reversed(money_list), dtype="money64")
+    m1 = pd.Series(money_list, dtype="Money64")
+    m2 = pd.Series(reversed(money_list), dtype="Money64")
     assert list(m1 == m1) == [True, True]
-    assert list(m1 == pd.Series(money_list, dtype="money64")) == [True, True]
+    assert list(m1 == pd.Series(money_list, dtype="Money64")) == [True, True]
     assert list(m1 != m2) == [True, True]
 
 
 def test_eq_not_money(money_list):
-    m = pd.Series(money_list, dtype="money64")
+    m = pd.Series(money_list, dtype="Money64")
     assert list(m == money_list) == [True, True]
 
 
 def test_bad_money_type():
     with pytest.raises(TypeError):
-        pd.Series(object(), dtype="money64")
+        pd.Series(object(), dtype="Money64")
 
 
 def test_slice_head(slice_series):
     slen = len(slice_series)
     s = slice_series[: slen // 2]
     assert len(s) == slen // 2
     for i, item in enumerate(s):
@@ -339,10 +342,88 @@
     assert len(s) == len(select)
     for idx, v in zip(select, s):
         assert slice_series[idx] == v
 
 
 def test_from_strings():
     strings = "3.14 2.72".split()
-    m = pd.Series(strings, dtype="money64")
+    m = pd.Series(strings, dtype="Money64")
     assert m.iloc[0] == Money(strings[0], USD)
     assert m.iloc[1] == Money(strings[1], USD)
+
+
+def test_nan():
+    m = pd.Series(np.nan, dtype="Money64")
+    assert pd.isna(m.iloc[0])
+
+
+def test_reindex(money_list):
+    m = pd.Series(money_list, dtype="Money64").reindex(range(len(money_list) + 1))
+    assert not any(map(pd.isna, m.iloc[:-1]))
+    assert pd.isna(m.iloc[-1])
+
+
+def test_isna(money_list):
+    m = pd.Series(money_list, dtype="Money64").reindex(range(len(money_list) + 1))
+    nas = m.isna()
+    assert not any(nas.iloc[:-1])
+    assert nas.iloc[-1]
+
+
+def test_na_astype(money_list):
+    m = (
+        pd.Series(money_list, dtype="Money64")
+        .reindex(range(len(money_list) + 1))
+        .astype("Float64")
+    )
+    nas = m.isna()
+    assert not any(nas.iloc[:-1])
+    assert nas.iloc[-1]
+
+
+def test_na_arithmetic(money_list):
+    m1 = pd.Series(money_list, dtype="Money64").reindex(range(len(money_list) + 1))
+    m2 = m1.iloc[::-1].reset_index(drop=True)
+    for oper, func in [
+        ("+", lambda x, y: x + y),
+        ("-", lambda x, y: x - y),
+        ("*", lambda x, y: x * y),
+        ("/", lambda x, y: x / y),
+    ]:
+        if oper == "*":
+            # builtins.TypeError: Cannot multiply money by money <MoneyArray>
+            nas = func(m1, m2.astype("Float64")).isna()
+        else:
+            nas = func(m1, m2).isna()
+        assert nas.iloc[0]
+        assert nas.iloc[-1]
+        assert not any(nas.iloc[1:-1])
+
+
+def test_copy(money_list):
+    m1 = pd.Series(money_list, dtype="Money64")
+    m2 = m1.copy()
+    assert all(m1 == m2)
+
+
+def test_concat(money_list):
+    m1 = pd.Series(money_list, dtype="Money64")
+    m2 = m1.copy()
+
+    m = pd.concat([m1, m2])
+    for item, expect in zip(m, money_list + money_list):
+        assert item == expect
+
+
+def test_print_with_na(money_list):
+    f = io.StringIO()
+    m = pd.Series(money_list, dtype="Money64").reindex(range(len(money_list) + 1))
+
+    with contextlib.redirect_stdout(f):
+        print(m)
+
+    lines = f.getvalue().splitlines()
+    # adjust for slightly different formatting in GH Actions container
+    assert re.match(r"\d\s+\$\s*3.14\s*", lines[0])
+    assert re.match(r"\d\s+\$\s*2.72\s*", lines[1])
+    assert re.match(r"\d\s+\<NA\>\s*", lines[2])
+    assert "dtype: Money64" in lines[3]
```

### Comparing `pandas_money-0.1.2/pyproject.toml` & `pandas_money-0.2.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pandas-money"
-version = "0.1.2"
+version = "0.2.0"
 description = "A Pandas ArrayExtension for handling currency with int64 performance"
 authors = ["Rod Morison <rmorison@users.noreply.github.com>"]
 repository = "https://github.com/rmorison/pandas-money"
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandas_money"}]
```

### Comparing `pandas_money-0.1.2/PKG-INFO` & `pandas_money-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-money
-Version: 0.1.2
+Version: 0.2.0
 Summary: A Pandas ArrayExtension for handling currency with int64 performance
 Home-page: https://github.com/rmorison/pandas-money
 License: MIT
 Author: Rod Morison
 Author-email: rmorison@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -28,44 +28,46 @@
 or with pip/pipenv
 ```
 pipenv install pandas-money
 ```
 
 ### Example
 ```py
+from decimal import Decimal
+
 import pandas as pd
+
 import pandas_money as pm
-from decimal import Decimal
 
-s = pd.Series(["1.11", "2.22", "3.33"], dtype="money64")
+s = pd.Series(["1.11", "2.22", "3.33"], dtype="Money64")
 
 print(s)
 print(s + s)
 print(s * Decimal("1.5"))
 print(s / 2)
 print(s.iloc[0], type(s.iloc[0]))
 ```
 outputs
 ```
 0    $1.11
 1    $2.22
 2    $3.33
-dtype: money64
+dtype: Money64
 0    $2.22
 1    $4.44
 2    $6.66
-dtype: money64
+dtype: Money64
 0    $1.66
 1    $3.33
 2    $5.00
-dtype: money64
+dtype: Money64
 0    $0.56
 1    $1.11
 2    $1.66
-dtype: money64
+dtype: Money64
 $1.11 <class 'moneyed.classes.Money'>
 ```
 
 ## Setup
 - Clone repo
 - `poetry install`
```

