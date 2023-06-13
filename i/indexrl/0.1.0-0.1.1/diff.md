# Comparing `tmp/indexrl-0.1.0.tar.gz` & `tmp/indexrl-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indexrl-0.1.0.tar", max compression
+gzip compressed data, was "indexrl-0.1.1.tar", max compression
```

## Comparing `indexrl-0.1.0.tar` & `indexrl-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,9 @@
--rw-r--r--   0        0        0     1841 2023-06-13 03:49:55.027190 indexrl-0.1.0/indexrl/configs/config_transfomer.py
--rw-r--r--   0        0        0     9844 2023-06-13 03:49:55.027190 indexrl-0.1.0/indexrl/environment.py
--rw-r--r--   0        0        0     2162 2023-06-13 03:49:55.028190 indexrl-0.1.0/indexrl/expression_handler.py
--rw-r--r--   0        0        0     1315 2023-06-13 03:49:55.028190 indexrl-0.1.0/indexrl/get_expression.py
--rw-r--r--   0        0        0    19716 2023-06-13 03:49:55.029190 indexrl-0.1.0/indexrl/gpt.py
--rw-r--r--   0        0        0     4572 2023-06-13 03:49:55.029190 indexrl-0.1.0/indexrl/mcts.py
--rw-r--r--   0        0        0     3834 2023-06-13 03:49:55.030196 indexrl-0.1.0/indexrl/overfit.py
--rw-r--r--   0        0        0     5464 2023-06-13 03:49:55.030196 indexrl-0.1.0/indexrl/pretrain_transformer.py
--rw-r--r--   0        0        0     1120 2023-06-13 03:49:55.033221 indexrl-0.1.0/indexrl/utils.py
--rw-r--r--   0        0        0      436 2023-06-13 04:02:10.002507 indexrl-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      105 2023-05-08 06:25:52.428525 indexrl-0.1.0/README.md
--rw-r--r--   0        0        0      767 1970-01-01 00:00:00.000000 indexrl-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1841 2023-06-13 03:49:55.027190 indexrl-0.1.1/indexrl/configs/config_transfomer.py
+-rw-r--r--   0        0        0    10243 2023-06-13 04:43:46.500329 indexrl-0.1.1/indexrl/environment.py
+-rw-r--r--   0        0        0     2162 2023-06-13 03:49:55.028190 indexrl-0.1.1/indexrl/expression_handler.py
+-rw-r--r--   0        0        0    19716 2023-06-13 03:49:55.029190 indexrl-0.1.1/indexrl/gpt.py
+-rw-r--r--   0        0        0     4572 2023-06-13 03:49:55.029190 indexrl-0.1.1/indexrl/mcts.py
+-rw-r--r--   0        0        0     1120 2023-06-13 03:49:55.033221 indexrl-0.1.1/indexrl/utils.py
+-rw-r--r--   0        0        0      458 2023-06-13 05:00:44.818915 indexrl-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      105 2023-05-08 06:25:52.428525 indexrl-0.1.1/README.md
+-rw-r--r--   0        0        0      803 1970-01-01 00:00:00.000000 indexrl-0.1.1/PKG-INFO
```

### Comparing `indexrl-0.1.0/indexrl/configs/config_transfomer.py` & `indexrl-0.1.1/indexrl/configs/config_transfomer.py`

 * *Files identical despite different names*

### Comparing `indexrl-0.1.0/indexrl/environment.py` & `indexrl-0.1.1/indexrl/environment.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from glob import glob
 import os
-import cv2
 import gym
 from copy import deepcopy
 import numpy as np
 from tqdm import tqdm
 import pickle
 
 from sklearn.metrics import roc_curve, auc
 
-from expression_handler import check_unitless_validity, eval_expression
-from utils import min_max_normalize, standardize
+from indexrl.expression_handler import check_unitless_validity, eval_expression
+from indexrl.utils import standardize
 
 
 class IndexRLEnv(gym.Env):
     def __init__(
         self,
         discrete_actions: list,
         max_exp_len: int = 100,
@@ -44,17 +43,17 @@
     def save_seen(self, seen_path):
         print("Seen length:", len(self.seen))
         with open(seen_path, "wb") as fp:
             pickle.dump(self.seen, fp)
 
     def get_cur_state(self):
         if self.ohe:
-            cur_exp_indices = [self.actions.index(act) for act in self.cur_exp] + [0] * (
-                self.max_exp_len - len(self.cur_exp)
-            )
+            cur_exp_indices = [self.actions.index(act) for act in self.cur_exp] + [
+                0
+            ] * (self.max_exp_len - len(self.cur_exp))
             enc_state = np.zeros((self.max_exp_len, len(self.actions)))
             enc_state[np.arange(self.max_exp_len), cur_exp_indices] = 1
             return enc_state.flatten()
         else:
             cur_exp_indices = [self.actions.index(act) for act in self.cur_exp]
             return np.array(cur_exp_indices)
 
@@ -114,15 +113,20 @@
             self.best_reward = max(self.best_reward, reward)
             self.best_exp = self.cur_exp
             return reward
         else:  # Pretraining stage
             # Motivate longer expressions
             if len(self.cur_exp) < self.max_exp_len // 3 or "(" not in self.cur_exp:
                 return -1
-            return 0.5 + 0.05 * len(self.cur_exp) + 0.01 * self.cur_exp.count(")") + 1 * unitless
+            return (
+                0.5
+                + 0.05 * len(self.cur_exp)
+                + 0.01 * self.cur_exp.count(")")
+                + 1 * unitless
+            )
 
     def take_action(self, action_idx: int) -> bool:
         action = self.actions[action_idx]
         if action == "(":
             self.parentheses_level += 1
         elif action == ")":
             self.parentheses_level -= 1
@@ -204,36 +208,51 @@
     assert len(image_paths) == len(mask_paths)
 
     unitless = check_unitless_validity(exp)
     if unitless is False:
         return -1
 
     tot_reward = 0
-    for image_path, mask_path in tqdm(zip(image_paths, mask_paths), "Calculating reward"):
+    for image_path, mask_path in tqdm(
+        zip(image_paths, mask_paths), "Calculating reward"
+    ):
         image = np.load(image_path)
         mask = np.load(mask_path)
 
         result = eval_expression(exp, image.squeeze())
         if result is False:
             tot_reward -= 1
         elif len(mask) > 2:
             norm_result = standardize(result, 3, (0, 1))
             if rew_type == "corr":
                 tot_reward += abs(get_correlation(1 - norm_result, mask > 0))
             elif rew_type == "f1":
-                tot_reward += min(get_f1_score(norm_result, mask > 0), get_f1_score(1 - norm_result, mask > 0))
+                tot_reward += min(
+                    get_f1_score(norm_result, mask > 0),
+                    get_f1_score(1 - norm_result, mask > 0),
+                )
             elif rew_type == "auc":
-                tot_reward += min(get_auc_score(norm_result, mask > 0), get_auc_score(1 - norm_result, mask > 0))
+                tot_reward += min(
+                    get_auc_score(norm_result, mask > 0),
+                    get_auc_score(1 - norm_result, mask > 0),
+                )
             elif rew_type == "sim":
-                tot_reward += min(get_similarity(norm_result, mask > 0), get_similarity(1 - norm_result, mask > 0))
+                tot_reward += min(
+                    get_similarity(norm_result, mask > 0),
+                    get_similarity(1 - norm_result, mask > 0),
+                )
             elif rew_type == "iou":
-                tot_reward += min(get_jaccard(norm_result, mask > 0), get_jaccard(1 - norm_result, mask > 0))
+                tot_reward += min(
+                    get_jaccard(norm_result, mask > 0),
+                    get_jaccard(1 - norm_result, mask > 0),
+                )
             else:  # AUC F1
                 tot_reward += min(
-                    get_auc_f1(standardize(result), mask > 0), get_auc_f1(1 - standardize(result), mask > 0)
+                    get_auc_f1(standardize(result), mask > 0),
+                    get_auc_f1(1 - standardize(result), mask > 0),
                 )
         else:  # Pretraining stage
             tot_reward += 0.5 + 0.02 * len(exp) + 0.2 * exp.count(")") + 1 * unitless
 
     return tot_reward / len(image_paths)
 
 
@@ -266,13 +285,18 @@
 
 
 def get_correlation(result: np.ndarray, mask: np.ndarray):
     return np.abs(np.corrcoef(result.flatten(), mask.flatten())[0, 1])
 
 
 def get_similarity(result: np.ndarray, mask: np.ndarray):
-    return np.dot(result.flatten(), mask.flatten()) / (np.linalg.norm(result) * np.linalg.norm(mask))
+    return np.dot(result.flatten(), mask.flatten()) / (
+        np.linalg.norm(result) * np.linalg.norm(mask)
+    )
 
 
 def get_jaccard(pred, target, threshold=0.5):
     pred_thresh = pred > threshold
-    return np.logical_and(pred_thresh, target).sum() / np.logical_or(pred_thresh, target).sum()
+    return (
+        np.logical_and(pred_thresh, target).sum()
+        / np.logical_or(pred_thresh, target).sum()
+    )
```

### Comparing `indexrl-0.1.0/indexrl/expression_handler.py` & `indexrl-0.1.1/indexrl/expression_handler.py`

 * *Files identical despite different names*

### Comparing `indexrl-0.1.0/indexrl/gpt.py` & `indexrl-0.1.1/indexrl/gpt.py`

 * *Files identical despite different names*

### Comparing `indexrl-0.1.0/indexrl/mcts.py` & `indexrl-0.1.1/indexrl/mcts.py`

 * *Files identical despite different names*

### Comparing `indexrl-0.1.0/indexrl/utils.py` & `indexrl-0.1.1/indexrl/utils.py`

 * *Files identical despite different names*

### Comparing `indexrl-0.1.0/PKG-INFO` & `indexrl-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: indexrl
-Version: 0.1.0
+Version: 0.1.1
 Summary: Generate remote sensing indices using image-mask pairs.
 Author: Dilith Jayakody
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: gym (==0.26.1)
 Requires-Dist: numpy (==1.20.3)
+Requires-Dist: scikit-learn (==1.0)
 Requires-Dist: torch (==1.13.1)
 Requires-Dist: torchvision (==0.14.1)
 Requires-Dist: transformers (==4.26.1)
 Requires-Dist: treelib (==1.6.1)
 Description-Content-Type: text/markdown
 
 # IndexRL
```

