# Comparing `tmp/sd_meh-0.6.1.tar.gz` & `tmp/sd_meh-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sd_meh-0.6.1.tar", max compression
+gzip compressed data, was "sd_meh-0.6.2.tar", max compression
```

## Comparing `sd_meh-0.6.1.tar` & `sd_meh-0.6.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1062 2023-06-09 08:30:05.757563 sd_meh-0.6.1/LICENSE.txt
--rw-r--r--   0        0        0     1878 2023-06-09 08:30:05.757563 sd_meh-0.6.1/README.md
--rw-r--r--   0        0        0      390 2023-06-09 08:30:05.757563 sd_meh-0.6.1/pyproject.toml
--rw-r--r--   0        0        0       22 2023-06-09 08:30:05.757563 sd_meh-0.6.1/sd_meh/__init__.py
--rw-r--r--   0        0        0    11653 2023-06-09 08:30:05.757563 sd_meh-0.6.1/sd_meh/merge.py
--rw-r--r--   0        0        0     6566 2023-06-09 08:30:05.757563 sd_meh-0.6.1/sd_meh/merge_methods.py
--rw-r--r--   0        0        0     1521 2023-06-09 08:30:05.757563 sd_meh-0.6.1/sd_meh/model.py
--rw-r--r--   0        0        0    83404 2023-06-09 08:30:05.757563 sd_meh-0.6.1/sd_meh/rebasin.py
--rw-r--r--   0        0        0     2402 1970-01-01 00:00:00.000000 sd_meh-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-13 18:59:51.908244 sd_meh-0.6.2/LICENSE.txt
+-rw-r--r--   0        0        0     1878 2023-06-13 18:59:51.908244 sd_meh-0.6.2/README.md
+-rw-r--r--   0        0        0      390 2023-06-13 18:59:51.908244 sd_meh-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-06-13 18:59:51.912244 sd_meh-0.6.2/sd_meh/__init__.py
+-rw-r--r--   0        0        0    11653 2023-06-13 18:59:51.912244 sd_meh-0.6.2/sd_meh/merge.py
+-rw-r--r--   0        0        0     6626 2023-06-13 18:59:51.912244 sd_meh-0.6.2/sd_meh/merge_methods.py
+-rw-r--r--   0        0        0     1521 2023-06-13 18:59:51.912244 sd_meh-0.6.2/sd_meh/model.py
+-rw-r--r--   0        0        0    83404 2023-06-13 18:59:51.912244 sd_meh-0.6.2/sd_meh/rebasin.py
+-rw-r--r--   0        0        0     2402 1970-01-01 00:00:00.000000 sd_meh-0.6.2/PKG-INFO
```

### Comparing `sd_meh-0.6.1/LICENSE.txt` & `sd_meh-0.6.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sd_meh-0.6.1/README.md` & `sd_meh-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `sd_meh-0.6.1/sd_meh/merge.py` & `sd_meh-0.6.2/sd_meh/merge.py`

 * *Files identical despite different names*

### Comparing `sd_meh-0.6.1/sd_meh/merge_methods.py` & `sd_meh-0.6.2/sd_meh/merge_methods.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,16 +68,16 @@
 
 
 def euclidean_add_difference(
     a: Tensor, b: Tensor, c: Tensor, alpha: float, **kwargs
 ) -> Tensor:
     a_diff = a.float() - c.float()
     b_diff = b.float() - c.float()
-    a_diff /= torch.linalg.norm(a_diff)
-    b_diff /= torch.linalg.norm(b_diff)
+    a_diff = torch.nan_to_num(a_diff / torch.linalg.norm(a_diff))
+    b_diff = torch.nan_to_num(b_diff / torch.linalg.norm(b_diff))
 
     distance = (1 - alpha) * a_diff**2 + alpha * b_diff**2
     distance = torch.sqrt(distance)
     sum_diff = weighted_sum(a.float(), b.float(), alpha) - c.float()
     distance = torch.copysign(distance, sum_diff)
 
     target_norm = torch.linalg.norm(sum_diff)
@@ -115,15 +115,15 @@
     return a_redist.reshape_as(a)
 
 
 def kth_abs_value(a: Tensor, k: int) -> Tensor:
     if k <= 0:
         return torch.tensor(-1, device=a.device)
     else:
-        return torch.kthvalue(torch.abs(a), k)[0]
+        return torch.kthvalue(torch.abs(a.float()), k)[0]
 
 
 def ratio_to_region(width: float, offset: float, n: int) -> Tuple[int, int, bool]:
     if width < 0:
         offset += width
         width = -width
     width = min(width, 1)
```

### Comparing `sd_meh-0.6.1/sd_meh/model.py` & `sd_meh-0.6.2/sd_meh/model.py`

 * *Files identical despite different names*

### Comparing `sd_meh-0.6.1/sd_meh/rebasin.py` & `sd_meh-0.6.2/sd_meh/rebasin.py`

 * *Files identical despite different names*

### Comparing `sd_meh-0.6.1/PKG-INFO` & `sd_meh-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sd-meh
-Version: 0.6.1
+Version: 0.6.2
 Summary: stable diffusion merging execution helper
 Home-page: https://github.com/s1dlx/meh
 License: MIT
 Author: s1dlx
 Author-email: s1dlx@proton.me
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

