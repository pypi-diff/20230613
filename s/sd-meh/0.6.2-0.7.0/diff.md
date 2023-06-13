# Comparing `tmp/sd_meh-0.6.2.tar.gz` & `tmp/sd_meh-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sd_meh-0.6.2.tar", max compression
+gzip compressed data, was "sd_meh-0.7.0.tar", max compression
```

## Comparing `sd_meh-0.6.2.tar` & `sd_meh-0.7.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1062 2023-06-13 18:59:51.908244 sd_meh-0.6.2/LICENSE.txt
--rw-r--r--   0        0        0     1878 2023-06-13 18:59:51.908244 sd_meh-0.6.2/README.md
--rw-r--r--   0        0        0      390 2023-06-13 18:59:51.908244 sd_meh-0.6.2/pyproject.toml
--rw-r--r--   0        0        0       22 2023-06-13 18:59:51.912244 sd_meh-0.6.2/sd_meh/__init__.py
--rw-r--r--   0        0        0    11653 2023-06-13 18:59:51.912244 sd_meh-0.6.2/sd_meh/merge.py
--rw-r--r--   0        0        0     6626 2023-06-13 18:59:51.912244 sd_meh-0.6.2/sd_meh/merge_methods.py
--rw-r--r--   0        0        0     1521 2023-06-13 18:59:51.912244 sd_meh-0.6.2/sd_meh/model.py
--rw-r--r--   0        0        0    83404 2023-06-13 18:59:51.912244 sd_meh-0.6.2/sd_meh/rebasin.py
--rw-r--r--   0        0        0     2402 1970-01-01 00:00:00.000000 sd_meh-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-13 19:20:47.976472 sd_meh-0.7.0/LICENSE.txt
+-rw-r--r--   0        0        0     1002 2023-06-13 19:20:47.976472 sd_meh-0.7.0/README.md
+-rw-r--r--   0        0        0      390 2023-06-13 19:20:47.980473 sd_meh-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-06-13 19:20:47.980473 sd_meh-0.7.0/sd_meh/__init__.py
+-rw-r--r--   0        0        0    13082 2023-06-13 19:20:47.980473 sd_meh-0.7.0/sd_meh/merge.py
+-rw-r--r--   0        0        0     6626 2023-06-13 19:20:47.980473 sd_meh-0.7.0/sd_meh/merge_methods.py
+-rw-r--r--   0        0        0     1521 2023-06-13 19:20:47.980473 sd_meh-0.7.0/sd_meh/model.py
+-rw-r--r--   0        0        0    10306 2023-06-13 19:20:47.980473 sd_meh-0.7.0/sd_meh/presets.py
+-rw-r--r--   0        0        0    83404 2023-06-13 19:20:47.980473 sd_meh-0.7.0/sd_meh/rebasin.py
+-rw-r--r--   0        0        0     1526 1970-01-01 00:00:00.000000 sd_meh-0.7.0/PKG-INFO
```

### Comparing `sd_meh-0.6.2/LICENSE.txt` & `sd_meh-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sd_meh-0.6.2/sd_meh/merge.py` & `sd_meh-0.7.0/sd_meh/merge.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import gc
 import os
 import re
+from concurrent.futures import ThreadPoolExecutor
 from contextlib import contextmanager
 from pathlib import Path
 from typing import Dict, Optional, Tuple
 
 import safetensors.torch
 import torch
 from tqdm import tqdm
@@ -131,40 +132,47 @@
     bases: Dict,
     merge_mode: str,
     precision: int = 16,
     weights_clip: bool = False,
     re_basin: bool = False,
     iterations: int = 1,
     device: str = "cpu",
+    work_device: Optional[str] = None,
     prune: bool = False,
+    threads: int = 1,
 ) -> Dict:
     thetas = load_thetas(models, prune, device, precision)
 
     if re_basin:
         merged = rebasin_merge(
             thetas,
             weights,
             bases,
             merge_mode,
             precision=precision,
             weights_clip=False,
             iterations=iterations,
             device=device,
+            work_device=work_device,
+            threads=threads,
         )
         # clip only after the last re-basin iteration
         if weights_clip:
             merged = clip_weights(thetas, merged)
     else:
         merged = simple_merge(
             thetas,
             weights,
             bases,
             merge_mode,
             precision=precision,
             weights_clip=weights_clip,
+            device=device,
+            work_device=work_device,
+            threads=threads,
         )
 
     return un_prune_model(merged, thetas, models, device, prune, precision)
 
 
 def un_prune_model(
     merged: Dict,
@@ -205,21 +213,39 @@
 def simple_merge(
     thetas: Dict[str, Dict],
     weights: Dict,
     bases: Dict,
     merge_mode: str,
     precision: int = 16,
     weights_clip: bool = False,
+    device: str = "cpu",
+    work_device: Optional[str] = None,
+    threads: int = 1,
 ) -> Dict:
-    for key in tqdm(thetas["model_a"].keys(), desc="stage 1"):
-        with merge_key_context(
-            key, thetas, weights, bases, merge_mode, precision, weights_clip
-        ) as result:
-            if result is not None:
-                thetas["model_a"].update({key: result.detach().clone()})
+    futures = []
+    with tqdm(thetas["model_a"].keys(), desc="stage 1") as progress:
+        with ThreadPoolExecutor(max_workers=threads) as executor:
+            for key in thetas["model_a"].keys():
+                future = executor.submit(
+                    simple_merge_key,
+                    progress,
+                    key,
+                    thetas,
+                    weights,
+                    bases,
+                    merge_mode,
+                    precision,
+                    weights_clip,
+                    device,
+                    work_device,
+                )
+                futures.append(future)
+
+        for res in futures:
+            res.result()
 
     log_vram("after stage 1")
 
     for key in tqdm(thetas["model_b"].keys(), desc="stage 2"):
         if KEY_POSITION_IDS in key:
             continue
         if "model" in key and key not in thetas["model_a"].keys():
@@ -237,14 +263,16 @@
     weights: Dict,
     bases: Dict,
     merge_mode: str,
     precision: int = 16,
     weights_clip: bool = False,
     iterations: int = 1,
     device="cpu",
+    work_device=None,
+    threads: int = 1,
 ):
     # WARNING: not sure how this does when 3 models are involved...
 
     model_a = thetas["model_a"].clone()
     perm_spec = sdunet_permutation_spec()
 
     print("permuting")
@@ -252,15 +280,23 @@
         # print(it)
         log_vram(f"{it} iteration start")
         new_weights, new_bases = step_weights_and_bases(weights, bases, it, iterations)
         log_vram("weights & bases, before simple merge")
 
         # normal block merge we already know and love
         thetas["model_a"] = simple_merge(
-            thetas, new_weights, new_bases, merge_mode, precision, weights_clip
+            thetas,
+            new_weights,
+            new_bases,
+            merge_mode,
+            precision,
+            weights_clip,
+            device,
+            work_device,
+            threads,
         )
 
         log_vram("simple merge done")
 
         # find permutations
         perm_1, y = weight_matching(
             perm_spec,
@@ -298,23 +334,36 @@
         )
 
         log_vram("model a updated")
 
     return thetas["model_a"]
 
 
+def simple_merge_key(progress, key, thetas, *args, **kwargs):
+    with merge_key_context(key, thetas, *args, **kwargs) as result:
+        if result is not None:
+            thetas["model_a"].update({key: result.detach().clone()})
+
+        progress.update()
+
+
 def merge_key(
     key: str,
     thetas: Dict,
     weights: Dict,
     bases: Dict,
     merge_mode: str,
     precision: int = 16,
     weights_clip: bool = False,
+    storage_device: str = "cpu",
+    work_device: Optional[str] = None,
 ) -> Optional[Tuple[str, Dict]]:
+    if work_device is None:
+        work_device = storage_device
+
     if KEY_POSITION_IDS in key:
         return
 
     for theta in thetas.values():
         if key not in theta.keys():
             return
 
@@ -346,16 +395,16 @@
                 current_bases = {k: w[weight_index] for k, w in weights.items()}
 
         try:
             merge_method = getattr(merge_methods, merge_mode)
         except AttributeError as e:
             raise ValueError(f"{merge_mode} not implemented, aborting merge!") from e
 
-        merge_args = get_merge_method_args(current_bases, thetas, key)
-        merged_key = merge_method(**merge_args)
+        merge_args = get_merge_method_args(current_bases, thetas, key, work_device)
+        merged_key = merge_method(**merge_args).to(storage_device)
 
         if weights_clip:
             t0 = thetas["model_a"][key]
             t1 = thetas["model_b"][key]
             threshold = torch.maximum(torch.abs(t0), torch.abs(t1))
             merged_key = torch.minimum(torch.maximum(merged_key, -threshold), threshold)
 
@@ -379,23 +428,28 @@
     try:
         yield result
     finally:
         if result is not None:
             del result
 
 
-def get_merge_method_args(current_bases: Dict, thetas: Dict, key: str) -> Dict:
+def get_merge_method_args(
+    current_bases: Dict,
+    thetas: Dict,
+    key: str,
+    work_device: str,
+) -> Dict:
     merge_method_args = {
-        "a": thetas["model_a"][key],
-        "b": thetas["model_b"][key],
+        "a": thetas["model_a"][key].to(work_device),
+        "b": thetas["model_b"][key].to(work_device),
         **current_bases,
     }
 
     if "model_c" in thetas:
-        merge_method_args["c"] = thetas["model_c"][key]
+        merge_method_args["c"] = thetas["model_c"][key].to(work_device)
 
     return merge_method_args
 
 
 def save_model(model, output_file, file_format) -> None:
     print(f"saving {output_file}")
     if file_format == "safetensors":
```

### Comparing `sd_meh-0.6.2/sd_meh/merge_methods.py` & `sd_meh-0.7.0/sd_meh/merge_methods.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-import torch
-from torch import Tensor
 import math
 from typing import Tuple
 
+import torch
+from torch import Tensor
 
 __all__ = [
     "weighted_sum",
     "weighted_subtraction",
     "tensor_sum",
     "add_difference",
     "sum_twice",
```

### Comparing `sd_meh-0.6.2/sd_meh/model.py` & `sd_meh-0.7.0/sd_meh/model.py`

 * *Files identical despite different names*

### Comparing `sd_meh-0.6.2/sd_meh/rebasin.py` & `sd_meh-0.7.0/sd_meh/rebasin.py`

 * *Files identical despite different names*

