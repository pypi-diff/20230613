# Comparing `tmp/pandas_money-0.2.0.tar.gz` & `tmp/pandas_money-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas_money-0.2.0.tar", max compression
+gzip compressed data, was "pandas_money-0.2.1.tar", max compression
```

## Comparing `pandas_money-0.2.0.tar` & `pandas_money-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1070 2023-06-09 03:17:36.171096 pandas_money-0.2.0/LICENSE
--rw-r--r--   0        0        0      859 2023-06-12 22:53:26.115878 pandas_money-0.2.0/README.md
--rw-r--r--   0        0        0      152 2023-06-12 00:16:34.192150 pandas_money-0.2.0/pandas_money/__init__.py
--rw-r--r--   0        0        0     8531 2023-06-12 22:53:26.115878 pandas_money-0.2.0/pandas_money/money_dtype.py
--rw-r--r--   0        0        0        0 2023-06-12 04:25:47.563979 pandas_money-0.2.0/pandas_money/tests/__init__.py
--rw-r--r--   0        0        0    12730 2023-06-12 23:58:17.114508 pandas_money-0.2.0/pandas_money/tests/test_money_dtype.py
--rw-r--r--   0        0        0     1434 2023-06-12 22:53:26.115878 pandas_money-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1545 1970-01-01 00:00:00.000000 pandas_money-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-09 03:17:36.171096 pandas_money-0.2.1/LICENSE
+-rw-r--r--   0        0        0      859 2023-06-12 22:53:26.115878 pandas_money-0.2.1/README.md
+-rw-r--r--   0        0        0      207 2023-06-13 19:32:02.941024 pandas_money-0.2.1/pandas_money/__init__.py
+-rw-r--r--   0        0        0     8652 2023-06-13 20:29:44.806189 pandas_money-0.2.1/pandas_money/money_dtype.py
+-rw-r--r--   0        0        0        0 2023-06-12 04:25:47.563979 pandas_money-0.2.1/pandas_money/tests/__init__.py
+-rw-r--r--   0        0        0    13160 2023-06-13 20:23:58.449518 pandas_money-0.2.1/pandas_money/tests/test_money_dtype.py
+-rw-r--r--   0        0        0     1434 2023-06-13 20:31:03.509546 pandas_money-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1545 1970-01-01 00:00:00.000000 pandas_money-0.2.1/PKG-INFO
```

### Comparing `pandas_money-0.2.0/LICENSE` & `pandas_money-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pandas_money-0.2.0/README.md` & `pandas_money-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pandas_money-0.2.0/pandas_money/money_dtype.py` & `pandas_money-0.2.1/pandas_money/money_dtype.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
             [self._clean_value(v, to_cents) for v in values],
             dtype=pd.Int64Dtype(),
         )
 
     def _clean_value(
         self, v: InputScalar | NAType, to_cents: bool
     ) -> int | Decimal | NAType:
-        if pd.isna(v):
+        if pd.isna(v) or v == np.inf:
             return pd.NA
 
         factor = money_factor if to_cents else 1
         round_to = money_decimals if to_cents else 0
         cleaned: int | np.integer | Decimal
         if isinstance(v, (int, np.integer)):
             cleaned = v
@@ -248,7 +248,11 @@
 ops_overrides_patches = {
     f"__{op}__": getattr(MoneyArray, f"__{op}__") for op in ops_overrides
 }
 MoneyArray._add_arithmetic_ops()
 MoneyArray._add_comparison_ops()
 for attr, patch in ops_overrides_patches.items():
     setattr(MoneyArray, attr, patch)
+
+
+def money_series(data, **kwargs) -> pd.Series:
+    return pd.Series(data, dtype=MoneyDtype(), **kwargs)
```

### Comparing `pandas_money-0.2.0/pandas_money/tests/test_money_dtype.py` & `pandas_money-0.2.1/pandas_money/tests/test_money_dtype.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,22 @@
 
 def test_money_scalar(money_scalar):
     m = pd.Series(money_scalar, dtype="Money64")
     assert isinstance(m.dtype, pm.MoneyDtype)
     assert m.iloc[0] == money_scalar
 
 
+def test_money_series_in_dataframe(money_scalar):
+    df = pd.DataFrame(index=range(2))
+    df["m"] = pm.money_series(money_scalar)
+    assert isinstance(df["m"].dtype, pm.MoneyDtype)
+    assert df["m"].iloc[0] == money_scalar
+    assert pd.isna(df["m"].iloc[1])
+
+
 def test_decimal_scalar(decimal_scalar):
     m = pd.Series(decimal_scalar, dtype="Money64")
     assert isinstance(m.dtype, pm.MoneyDtype)
     assert m.iloc[0] == Money(decimal_scalar, USD)
 
 
 def test_str_scalar(str_scalar):
@@ -271,14 +279,21 @@
     assert isinstance(m.dtype, pm.MoneyDtype)
     # DeprecationWarning: Multiplying Money instances with floats is deprecated
     # so cast floats to Decimal
     assert m.iloc[0] == (money_list[0] / Decimal(float_scalar)).round(pm.money_decimals)
     assert m.iloc[1] == (money_list[1] / Decimal(float_scalar)).round(pm.money_decimals)
 
 
+def test_truediv_by_zero(money_list):
+    m1 = pm.money_series(money_list)
+    m = m1 / [0, 1]
+    assert pd.isna(m.iloc[0])
+    assert m.iloc[1] == money_list[1]
+
+
 def test_badscalar():
     with pytest.raises(InvalidOperation):
         pd.Series("asdf", dtype="Money64")
 
 
 def test_astype(money_list):
     m1 = pd.Series(money_list, dtype="Money64")
```

### Comparing `pandas_money-0.2.0/pyproject.toml` & `pandas_money-0.2.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pandas-money"
-version = "0.2.0"
+version = "0.2.1"
 description = "A Pandas ArrayExtension for handling currency with int64 performance"
 authors = ["Rod Morison <rmorison@users.noreply.github.com>"]
 repository = "https://github.com/rmorison/pandas-money"
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandas_money"}]
```

### Comparing `pandas_money-0.2.0/PKG-INFO` & `pandas_money-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-money
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Pandas ArrayExtension for handling currency with int64 performance
 Home-page: https://github.com/rmorison/pandas-money
 License: MIT
 Author: Rod Morison
 Author-email: rmorison@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

