# Comparing `tmp/tedeous-0.1.2.tar.gz` & `tmp/tedeous-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tedeous-0.1.2.tar", last modified: Thu May 11 09:26:33 2023, max compression
+gzip compressed data, was "tedeous-0.2.0.tar", last modified: Tue Jun 13 14:33:23 2023, max compression
```

## Comparing `tedeous-0.1.2.tar` & `tedeous-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:26:33.396173 tedeous-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-11 09:26:26.000000 tedeous-0.1.2/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-11 09:26:33.396173 tedeous-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-05-11 09:26:26.000000 tedeous-0.1.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 09:26:33.396173 tedeous-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-11 09:26:26.000000 tedeous-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:26:33.392173 tedeous-0.1.2/tedeous/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-11 09:26:26.000000 tedeous-0.1.2/tedeous/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14794 2023-05-11 09:26:26.000000 tedeous-0.1.2/tedeous/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-05-11 09:26:26.000000 tedeous-0.1.2/tedeous/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11410 2023-05-11 09:26:26.000000 tedeous-0.1.2/tedeous/derivative.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-11 09:26:26.000000 tedeous-0.1.2/tedeous/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     9417 2023-05-11 09:26:26.000000 tedeous-0.1.2/tedeous/finite_diffs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24639 2023-05-11 09:26:26.000000 tedeous-0.1.2/tedeous/input_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)    12431 2023-05-11 09:26:26.000000 tedeous-0.1.2/tedeous/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-05-11 09:26:26.000000 tedeous-0.1.2/tedeous/points_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    15634 2023-05-11 09:26:26.000000 tedeous-0.1.2/tedeous/solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:26:33.396173 tedeous-0.1.2/tedeous.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-11 09:26:33.000000 tedeous-0.1.2/tedeous.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-11 09:26:33.000000 tedeous-0.1.2/tedeous.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 09:26:33.000000 tedeous-0.1.2/tedeous.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-11 09:26:33.000000 tedeous-0.1.2/tedeous.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:33:23.857148 tedeous-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-13 14:33:17.000000 tedeous-0.2.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-13 14:33:23.857148 tedeous-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-06-13 14:33:17.000000 tedeous-0.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 14:33:23.857148 tedeous-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-13 14:33:17.000000 tedeous-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:33:23.857148 tedeous-0.2.0/tedeous/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-13 14:33:17.000000 tedeous-0.2.0/tedeous/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15995 2023-06-13 14:33:17.000000 tedeous-0.2.0/tedeous/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-06-13 14:33:17.000000 tedeous-0.2.0/tedeous/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11410 2023-06-13 14:33:17.000000 tedeous-0.2.0/tedeous/derivative.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-13 14:33:17.000000 tedeous-0.2.0/tedeous/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9417 2023-06-13 14:33:17.000000 tedeous-0.2.0/tedeous/finite_diffs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24639 2023-06-13 14:33:17.000000 tedeous-0.2.0/tedeous/input_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15481 2023-06-13 14:33:17.000000 tedeous-0.2.0/tedeous/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-06-13 14:33:17.000000 tedeous-0.2.0/tedeous/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-06-13 14:33:17.000000 tedeous-0.2.0/tedeous/points_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16472 2023-06-13 14:33:17.000000 tedeous-0.2.0/tedeous/solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:33:23.857148 tedeous-0.2.0/tedeous.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-13 14:33:23.000000 tedeous-0.2.0/tedeous.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-13 14:33:23.000000 tedeous-0.2.0/tedeous.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 14:33:23.000000 tedeous-0.2.0/tedeous.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 14:33:23.000000 tedeous-0.2.0/tedeous.egg-info/top_level.txt
```

### Comparing `tedeous-0.1.2/LICENCE` & `tedeous-0.2.0/LICENCE`

 * *Files identical despite different names*

### Comparing `tedeous-0.1.2/PKG-INFO` & `tedeous-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tedeous
-Version: 0.1.2
+Version: 0.2.0
 Summary: TEDEouS - Torch Exhaustive Differential Equations Solver. Differential equation solver, based on pytorch library
 Author: Alexander Hvatov
 Author-email: itmo.nss.team@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tedeous-0.1.2/README.rst` & `tedeous-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `tedeous-0.1.2/setup.py` & `tedeous-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 def get_requirements():
     requirements = extract_requirements('requirements.txt')
     return requirements
 
 setup(
     name = 'tedeous',
-    version= '0.1.2' ,
+    version= '0.2.0' ,
     description = 'TEDEouS - Torch Exhaustive Differential Equations Solver. Differential equation solver, based on pytorch library',
     long_description = 'Combine power of pytorch, numerical methods and math overall to conquer and solve ALL {O,P}DEs. There are some examples to provide a little insight to an operator form',
     author = 'Alexander Hvatov',
     author_email = 'itmo.nss.team@gmail.com', # add email
     classifiers = [      
               'Development Status :: 3 - Alpha',
               'Programming Language :: Python :: 3',
```

### Comparing `tedeous-0.1.2/tedeous/cache.py` & `tedeous-0.2.0/tedeous/cache.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,25 +68,52 @@
                 torch.nn.Tanh(),
                 torch.nn.Linear(100, 100),
                 torch.nn.Tanh(),
                 torch.nn.Linear(100, 1)
             )
         return NN_grid, cache_model
 
+    @staticmethod
+    def model_reform(init_model, model):
+        """
+        As some models are nn.Sequential class objects,
+        but another models are nn.Module class objects.
+        This method does checking the solver model (init_model)
+        and the cache model (model).
+        Args:
+            init_model: [nn.Sequential or class(nn.Module)].
+            model: [nn.Sequential or class(nn.Module)].
+        Returns:
+            * **init_model** -- [nn.Sequential or nn.ModuleList] \n
+            * **model** -- [nn.Sequential or nn.ModuleList].
+        """
+        try:
+            model[0]
+        except:
+            model = model.model
+        
+        try:
+            init_model[0]
+        except:
+            init_model = init_model.model
+        
+        return init_model, model
+        
+
     def cache_lookup(self, lambda_bound: float = 0.001, weak_form: None = None, cache_dir: str = '../cache/',
                 nmodels: Union[int, None] = None, cache_verbose: bool = False) -> Tuple[dict, torch.Tensor]:
         """
         Looking for a saved cache.
         Args:
             lambda_bound: an arbitrary chosen constant, influence only convergence speed.
             cache_dir: directory where saved cache in.
-            nmodels: smth
+            nmodels: maximal number of models that are looked before optimization
             cache_verbose: more detailed info about models in cache.
         Returns:
-            * **best_checkpoint** -- smth.\n
+            * **best_checkpoint** -- best model with optimizator state.\n
             * **min_loss** -- minimum error in pre-trained error.
         """
         files = glob.glob(cache_dir + '*.tar')
         if len(files) == 0:
             best_checkpoint = None
             min_loss = np.inf
             return best_checkpoint, min_loss
@@ -100,18 +127,21 @@
 
         for i in cache_n:
             file = files[i]
             checkpoint = torch.load(file)
             model = checkpoint['model']
             model.load_state_dict(checkpoint['model_state_dict'])
             # this one for the input shape fix if needed
-            if model[0].in_features != self.model[0].in_features:
+            
+            solver_model, cache_model = self.model_reform(self.model, model)
+
+            if cache_model[0].in_features != solver_model[0].in_features:
                 continue
             try:
-                if model[-1].out_features != self.model[-1].out_features:
+                if cache_model[-1].out_features != solver_model[-1].out_features:
                     continue
             except Exception:
                 continue
             model = model.to(device)
             l = Solution(self.grid, self.equal_cls, model, self.mode). \
                 loss_evaluation(lambda_bound=lambda_bound, weak_form=weak_form)
             if l < min_loss:
@@ -224,16 +254,19 @@
             * **optimizer_state** -- smth
         """
 
         # do nothing if cache is empty
         if cache_checkpoint == None:
             optimizer_state = None
             return self.model, optimizer_state
-        # if models have the same structure use the cache model state
-        if str(cache_checkpoint['model']) == str(self.model):
+        # if models have the same structure use the cache model state,
+        # and the cache model has ordinary structure
+        if str(cache_checkpoint['model']) == str(self.model) and \
+                 isinstance(self.model, torch.nn.Sequential) and \
+                 isinstance(self.model[0], torch.nn.Linear):
             self.model = cache_checkpoint['model']
             self.model.load_state_dict(cache_checkpoint['model_state_dict'])
             self.model.train()
             optimizer_state = cache_checkpoint['optimizer_state_dict']
             if cache_verbose:
                 print('Using model from cache')
         # else retrain the input model using the cache model
@@ -267,14 +300,15 @@
        """
         r = create_random_fn(model_randomize_parameter)
         cache_checkpoint, min_loss = self.cache_lookup(cache_dir=cache_dir,
                                                        nmodels=nmodels,
                                                        cache_verbose=cache_verbose,
                                                        lambda_bound=lambda_bound,
                                                        weak_form=weak_form)
+        
         self.model, optimizer_state = self.cache_retrain(cache_checkpoint,
                                                          cache_verbose=cache_verbose)
 
         self.model.apply(r)
 
         return self.model, min_loss
```

### Comparing `tedeous-0.1.2/tedeous/config.py` & `tedeous-0.2.0/tedeous/config.py`

 * *Files identical despite different names*

### Comparing `tedeous-0.1.2/tedeous/derivative.py` & `tedeous-0.2.0/tedeous/derivative.py`

 * *Files identical despite different names*

### Comparing `tedeous-0.1.2/tedeous/device.py` & `tedeous-0.2.0/tedeous/device.py`

 * *Files identical despite different names*

### Comparing `tedeous-0.1.2/tedeous/finite_diffs.py` & `tedeous-0.2.0/tedeous/finite_diffs.py`

 * *Files identical despite different names*

### Comparing `tedeous-0.1.2/tedeous/input_preprocessing.py` & `tedeous-0.2.0/tedeous/input_preprocessing.py`

 * *Files identical despite different names*

### Comparing `tedeous-0.1.2/tedeous/metrics.py` & `tedeous-0.2.0/tedeous/metrics.py`

 * *Files 12% similar despite different names*

```diff
@@ -48,22 +48,22 @@
         return U, 0.
     else:
         result.append(U)
         grid = grid[index, :-1]
         return result, grid
 
 
-class Solution():
-    def __init__(self, grid: torch.Tensor, equal_cls: Union[tedeous.input_preprocessing.Equation_NN,
-                                                            tedeous.input_preprocessing.Equation_mat, tedeous.input_preprocessing.Equation_autograd],
+class DE_operator():
+    """
+    Class for differential equation calculation.
+    """
+    def __init__(self, grid: torch.Tensor, prepared_operator: dict,
                  model: Union[torch.nn.Sequential, torch.Tensor], mode: str):
         self.grid = check_device(grid)
-        equal_copy = deepcopy(equal_cls)
-        self.prepared_operator = equal_copy.operator_prepare()
-        self.prepared_bconds = equal_copy.bnd_prepare()
+        self.prepared_operator = prepared_operator
         self.model = model.to(device_type())
         self.mode = mode
         if self.mode == 'NN':
             self.grid_dict = Points_type(self.grid).grid_sort()
             self.sorted_grid = torch.cat(list(self.grid_dict.values()))
         elif self.mode == 'autograd' or self.mode == 'mat':
             self.sorted_grid = self.grid
@@ -85,14 +85,79 @@
             dif = derivative(term, grid_points)
             try:
                 total += dif
             except NameError:
                 total = dif
         return total
 
+    def pde_compute(self) -> torch.Tensor:
+        """
+        Computes PDE residual.
+
+        Returns:
+            PDE residual.
+        """
+
+        num_of_eq = len(self.prepared_operator)
+        if num_of_eq == 1:
+            op = self.apply_operator(
+                self.prepared_operator[0], self.sorted_grid)
+        else:
+            op_list = []
+            for i in range(num_of_eq):
+                op_list.append(self.apply_operator(
+                    self.prepared_operator[i], self.sorted_grid))
+            op = torch.cat(op_list, 1)
+        return op
+
+    def weak_pde_compute(self, weak_form) -> torch.Tensor:
+        """
+        Computes PDE residual in weak form.
+
+        Args:
+            weak_form: list of basis functions
+        Returns:
+            weak PDE residual.
+        """
+        device = device_type()
+        if self.mode == 'NN':
+            grid_central = self.grid_dict['central']
+        elif self.mode == 'autograd':
+            grid_central = self.grid
+
+        op = self.pde_compute()
+        sol_list = []
+        for i in range(op.shape[-1]):
+            sol = op[:, i]
+            for func in weak_form:
+                sol = sol * func(grid_central).to(device).reshape(-1)
+            grid_central1 = torch.clone(grid_central)
+            for k in range(grid_central.shape[-1]):
+                sol, grid_central1 = integration(sol, grid_central1)
+            sol_list.append(sol.reshape(-1, 1))
+        if len(sol_list) == 1:
+            return sol_list[0]
+        else:
+            return torch.cat(sol_list)
+
+
+class Bounds():
+    """
+    class for boundary and initial conditions calculation.
+    """
+    def __init__(self, grid: torch.Tensor, prepared_bconds: dict,
+                 model: Union[torch.nn.Sequential, torch.Tensor], mode: str):
+        self.grid = check_device(grid)
+        self.prepared_bconds = prepared_bconds
+        self.model = model.to(device_type())
+        self.mode = mode
+        self.apply_operator = DE_operator(self.grid, self.prepared_bconds,
+                                          self.model, self.mode).apply_operator
+
+
     def apply_bconds_set(self, operator_set: list) -> torch.Tensor:
         """
         Deciphers equation in a whole grid to a field.
         Args:
             operator_set: Multiple (len(subset)>=1) operators in input form. See
             input_preprocessing.operator_prepare().
         Returns:
@@ -212,120 +277,131 @@
             b_val_list.append(b_op_val)
 
         true_b_val = torch.cat(true_b_val_list)
         b_val = torch.cat(b_val_list).reshape(-1, 1)
 
         return b_val, true_b_val
 
-    def pde_compute(self) -> torch.Tensor:
-        """
-        Computes PDE residual.
 
-        Returns:
-            PDE residual.
-        """
-
-        num_of_eq = len(self.prepared_operator)
-        if num_of_eq == 1:
-            op = self.apply_operator(
-                self.prepared_operator[0], self.sorted_grid)
-        else:
-            op_list = []
-            for i in range(num_of_eq):
-                op_list.append(self.apply_operator(
-                    self.prepared_operator[i], self.sorted_grid))
-            op = torch.cat(op_list, 1)
-        return op
+class Solution():
+    """
+    class for different loss functions calculation.
+    """
+    def __init__(self, grid: torch.Tensor, equal_cls: Union[tedeous.input_preprocessing.Equation_NN,
+                                                            tedeous.input_preprocessing.Equation_mat,
+                                                            tedeous.input_preprocessing.Equation_autograd],
+                 model: Union[torch.nn.Sequential, torch.Tensor], mode: str):
+        self.grid = check_device(grid)
+        if mode == 'NN':
+            sorted_grid = Points_type(self.grid).grid_sort()
+            self.n_t = len(sorted_grid['central'][:, 0].unique())
+        elif mode == 'autograd':
+            self.n_t = len(self.grid[:, 0].unique())
+        equal_copy = deepcopy(equal_cls)
+        self.prepared_operator = equal_copy.operator_prepare()
+        self.prepared_bconds = equal_copy.bnd_prepare()
+        self.model = model.to(device_type())
+        self.mode = mode
+        self.operator = DE_operator(self.grid, self.prepared_operator, self.model,
+                                   self.mode)
+        self.bconds = Bounds(self.grid, self.prepared_bconds, self.model,
+                                   self.mode)
 
-    def weak_pde_compute(self, weak_form) -> torch.Tensor:
+    def default_loss(self, lambda_bound:  Union[int, float] = 10):
         """
-        Computes PDE residual in weak form.
-
+        Computes l2 loss.
         Args:
-            weak_form: list of basis functions
+            lambda_bound: an arbitrary chosen constant, influence only convergence speed.
         Returns:
-            weak PDE residual.
+            model loss.
         """
-        device = device_type()
-        if self.mode == 'NN':
-            grid_central = self.grid_dict['central']
-        elif self.mode == 'autograd':
-            grid_central = self.grid
+        op = self.operator.pde_compute()
 
-        op = self.pde_compute()
-        sol_list = []
-        for i in range(op.shape[-1]):
-            sol = op[:, i]
-            for func in weak_form:
-                sol = sol * func(grid_central).to(device).reshape(-1)
-            grid_central1 = torch.clone(grid_central)
-            for k in range(grid_central.shape[-1]):
-                sol, grid_central1 = integration(sol, grid_central1)
-            sol_list.append(sol.reshape(-1, 1))
-        if len(sol_list) == 1:
-            return sol_list[0]
+        if self.prepared_bconds == None:
+            return torch.sum(torch.mean((op) ** 2, 0))
+
+        b_val, true_b_val = self.bconds.apply_bconds_operator()
+
+        if self.mode == 'mat':
+            loss = torch.mean((op) ** 2) + \
+                   lambda_bound * torch.mean((b_val - true_b_val) ** 2)
         else:
-            return torch.cat(sol_list)
+            loss = torch.sum(torch.mean((op) ** 2, 0)) + \
+                   lambda_bound * torch.sum(torch.mean((b_val - true_b_val) ** 2, 0))
+        return loss
 
-    def l2_loss(self, lambda_bound:  Union[int, float] = 10) -> torch.Tensor:
+    def casual_loss(self, lambda_bound:  Union[int, float] = 10, tol: float = 0) -> torch.Tensor:
         """
-        Computes l2 loss.
+        Computes casual loss, which is caclulated with weights matrix:
+        W = exp(-tol*(Loss_i)) where Loss_i is sum of the L2 loss from 0
+        to t_i moment of time. This loss function should be used when one
+        of the DE independent parameter is time.
+
         Args:
             lambda_bound: an arbitrary chosen constant, influence only convergence speed.
+            tol: float constant, influences on error penalty. 
         Returns:
             model loss.
         """
-        op = self.pde_compute()
+        
+        op = self.operator.pde_compute()**2
+
         if self.prepared_bconds == None:
             return torch.sum(torch.mean((op) ** 2, 0))
 
-        b_val, true_b_val = self.apply_bconds_operator()
+        b_val, true_b_val = self.bconds.apply_bconds_operator()
 
+        res = torch.sum(op, dim=1).reshape(self.n_t, -1)
+        res = torch.mean(res, axis=1).reshape(self.n_t, 1)
+        M = torch.triu(torch.ones((self.n_t, self.n_t)), diagonal=1).T
+        with torch.no_grad():
+            W = torch.exp(- tol * (M @ res))
+        #plt.plot(W.detach().cpu().numpy())
+        #plt.show()
+        loss = torch.mean(W*res) + \
+                lambda_bound * torch.sum(torch.mean((b_val - true_b_val) ** 2, 0))
 
-        if self.mode == 'mat':
-            loss = torch.mean((op) ** 2) + \
-                   lambda_bound * torch.mean((b_val - true_b_val) ** 2)
-        else:
-            loss = torch.sum(torch.mean((op) ** 2, 0)) + \
-                   lambda_bound * torch.sum(torch.mean((b_val - true_b_val) ** 2, 0))
         return loss
 
     def weak_loss(self, weak_form: Union[None, list], lambda_bound: Union[int, float] = 10) -> torch.Tensor:
         """
         Weak solution of O/PDE problem.
         Args:
             weak_form: list of basis functions.
             lambda_bound: const regularization parameter.
         Returns:
             model loss.
         """
-        op = self.weak_pde_compute(weak_form)
+        op = self.operator.weak_pde_compute(weak_form)
         if self.prepared_bconds == None:
             return torch.sum(op)
 
         # we apply no  boundary conditions operators if they are all None
 
-        b_val, true_b_val = self.apply_bconds_operator()
+        b_val, true_b_val = self.bconds.apply_bconds_operator()
 
         loss = torch.sum(op) + \
                lambda_bound * torch.sum(torch.mean((b_val - true_b_val) ** 2, 0))
 
         return loss
 
-    def loss_evaluation(self, lambda_bound: Union[int, float] = 10, weak_form: Union[None, list] = None) -> Union[l2_loss, weak_loss]:
+    def loss_evaluation(self, lambda_bound: Union[int, float] = 10, weak_form: Union[None, list] = None, tol=0) -> Union[default_loss, weak_loss, casual_loss]:
         """
         Setting the required loss calculation method.
         Args:
             lambda_bound: an arbitrary chosen constant, influence only convergence speed.
             weak_form: list of basis functions.
+            tol: float constant, influences on error penalty. 
         Returns:
             A given calculation method.
         """
         if self.mode == 'mat' or self.mode == 'autograd':
             if self.prepared_bconds == None:
                 print('No bconds is not possible, returning infinite loss')
                 return np.inf
 
-        if weak_form == None or weak_form == []:
-            return self.l2_loss(lambda_bound=lambda_bound)
+        if weak_form != None and weak_form != []:
+            return self.weak_loss(weak_form, lambda_bound=lambda_bound)
+        elif tol != 0:
+            return self.casual_loss(lambda_bound=lambda_bound, tol=tol)
         else:
-            return self.weak_loss(weak_form, lambda_bound=lambda_bound)
+            return self.default_loss(lambda_bound=lambda_bound)
```

### Comparing `tedeous-0.1.2/tedeous/points_type.py` & `tedeous-0.2.0/tedeous/points_type.py`

 * *Files identical despite different names*

### Comparing `tedeous-0.1.2/tedeous/solver.py` & `tedeous-0.2.0/tedeous/solver.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import torch
 import numpy as np
 import matplotlib.pyplot as plt
 from matplotlib import cm
 import os
 import datetime
 from typing import Union
+from torch.optim.lr_scheduler import ExponentialLR
 
 from tedeous.cache import *
 from tedeous.device import check_device, device_type
 from tedeous.metrics import Solution
 import tedeous.input_preprocessing
 
 
@@ -41,81 +42,42 @@
             grid=torch.cartesian_prod(*coord_list_tensor)
     elif mode=='mat':
         grid = np.meshgrid(*coord_list)
         grid = torch.tensor(np.array(grid)).to(device)
     return grid
 
 
-class Solver():
-    """
-    High-level interface for solving equations.
-    """
-    def __init__(self, grid: torch.Tensor, equal_cls: Union[tedeous.input_preprocessing.Equation_NN,
-                                                            tedeous.input_preprocessing.Equation_mat, tedeous.input_preprocessing.Equation_autograd],
-                 model: Any, mode: str, weak_form: Union[None, list] = None):
-        """
-        High-level interface for solving equations.
-        Args:
-            grid: array of a n-D points.
-            equal_cls: object from input_preprocessing (see input_preprocessing.Equation).
-            model: neural network.
-            mode: calculation method. (i.e., "NN", "autograd", "mat").
-            weak_form: list of basis functions.
-        """
-        self.grid = check_device(grid)
-        self.equal_cls = equal_cls
+class Plots():
+    def __init__(self, model, grid, mode):
         self.model = model
+        self.grid = grid
         self.mode = mode
-        self.weak_form = weak_form
-
-    def optimizer_choice(self, optimizer: str, learning_rate: float)-> \
-            Union[torch.optim.Adam, torch.optim.SGD, torch.optim.LBFGS]:
-        """
-        Setting optimizer.
-
-        Args:
-           optimizer: optimizer choice (Adam, SGD, LBFGS).
-           learning_rate: determines the step size at each iteration while moving toward a minimum of a loss function.
-        Returns:
-           torch.optimizer object as is.
-        """
-        if optimizer=='Adam':
-            torch_optim = torch.optim.Adam
-        elif optimizer=='SGD':
-            torch_optim = torch.optim.SGD
-        elif optimizer=='LBFGS':
-            torch_optim = torch.optim.LBFGS
-        else:
-            print('Wrong optimizer chosen, optimization was not performed')
-            return self.model
-
-        if self.mode =='NN' or self.mode == 'autograd':
-            optimizer = torch_optim(self.model.parameters(), lr=learning_rate)
-        elif self.mode =='mat':
-            optimizer = torch_optim([self.model.requires_grad_()], lr=learning_rate)
-       
-        return optimizer
 
     def print_nn(self, title: str):
         """
         Solution plot for NN method.
 
         Args:
             title: title
         """
-        nvars_model = self.model[-1].out_features
+        try:
+            nvars_model = self.model[-1].out_features
+        except:
+            nvars_model = self.model.model[-1].out_features
+
         nparams = self.grid.shape[1]
-        fig = plt.figure()
+        fig = plt.figure(figsize=(15,8))
         for i in range(nvars_model):
             if nparams == 1:
                 ax1 = fig.add_subplot(1,nvars_model,i+1)
                 if title != None:
                     ax1.set_title(title+' variable {}'.format(i))
                 ax1.scatter(self.grid.detach().cpu().numpy().reshape(-1),
                             self.model(self.grid)[:,i].detach().cpu().numpy())
+                
             else:
                 ax1 = fig.add_subplot(1, nvars_model, i+1, projection='3d')
                 if title != None:
                     ax1.set_title(title+' variable {}'.format(i))
                 ax1.plot_trisurf(self.grid[:, 0].detach().cpu().numpy(), 
                             self.grid[:, 1].detach().cpu().numpy(),
                             self.model(self.grid)[:,i].detach().cpu().numpy(),
@@ -183,30 +145,86 @@
             self.print_nn(title)
         if solution_save:
             plt.savefig(directory)
         if solution_print:
             plt.show()
         plt.close()
 
-    def solve(self, lambda_bound: Union[int, float] = 10, verbose: bool = False, learning_rate: float = 1e-4,
-              eps: float = 1e-5, tmin: int = 1000, tmax: float = 1e5, nmodels: Union[int, None] = None,
-              name: Union[str, None] = None, abs_loss: Union[None, float] = None, use_cache: bool = True,
-              cache_dir: str = '../cache/', cache_verbose: bool = False, save_always: bool = False,
-              print_every: Union[int, None] = 100, cache_model: Union[torch.nn.Sequential, None] = None,
-              patience: int = 5, loss_oscillation_window: int = 100, no_improvement_patience: int = 1000,
-              model_randomize_parameter: Union[int, float] = 0, optimizer_mode: str = 'Adam',
-              step_plot_print: Union[bool, int] = False, step_plot_save: Union[bool, int] = False,
-              image_save_dir: Union[str, None] = None) -> Any:
+
+class Solver():
+    """
+    High-level interface for solving equations.
+    """
+    def __init__(self, grid: torch.Tensor, equal_cls,
+                 model: Any, mode: str, weak_form: Union[None, list] = None):
+        """
+        High-level interface for solving equations.
+        Args:
+            grid: array of a n-D points.
+            equal_cls: object from input_preprocessing (see input_preprocessing.Equation).
+            model: neural network.
+            mode: calculation method. (i.e., "NN", "autograd", "mat").
+            weak_form: list of basis functions.
+        """
+        self.grid = check_device(grid)
+        self.equal_cls = equal_cls
+        self.model = model
+        self.mode = mode
+        self.weak_form = weak_form
+
+    def optimizer_choice(self, optimizer: str, learning_rate: float)-> \
+            Union[torch.optim.Adam, torch.optim.SGD, torch.optim.LBFGS]:
+        """
+        Setting optimizer.
+
+        Args:
+           optimizer: optimizer choice (Adam, SGD, LBFGS).
+           learning_rate: determines the step size at each iteration while moving toward a minimum of a loss function.
+        Returns:
+           torch.optimizer object as is.
+        """
+        if optimizer=='Adam':
+            torch_optim = torch.optim.Adam
+        elif optimizer=='SGD':
+            torch_optim = torch.optim.SGD
+        elif optimizer=='LBFGS':
+            torch_optim = torch.optim.LBFGS
+        else:
+            print('Wrong optimizer chosen, optimization was not performed')
+            return self.model
+
+        if self.mode =='NN' or self.mode == 'autograd':
+            optimizer = torch_optim(self.model.parameters(), lr=learning_rate)
+        elif self.mode =='mat':
+            optimizer = torch_optim([self.model.requires_grad_()], lr=learning_rate)
+       
+        return optimizer
+
+
+    def solve(self, lambda_bound: Union[int, float] = 10,
+              verbose: bool = False, learning_rate: float = 1e-4, gamma=None, lr_change=1000,
+              eps: float = 1e-5, tmin: int = 1000, tmax: float = 1e5,
+              nmodels: Union[int, None] = None, name: Union[str, None] = None,
+              abs_loss: Union[None, float] = None, use_cache: bool = True,
+              cache_dir: str = '../cache/', cache_verbose: bool = False,
+              save_always: bool = False, print_every: Union[int, None] = 100,
+              cache_model: Union[torch.nn.Sequential, None] = None,
+              patience: int = 5, loss_oscillation_window: int = 100,
+              no_improvement_patience: int = 1000,  model_randomize_parameter: Union[int, float] = 0,
+              optimizer_mode: str = 'Adam', step_plot_print: Union[bool, int] = False,
+              step_plot_save: Union[bool, int] = False, image_save_dir: Union[str, None] = None, tol:float=0) -> Any:
         """
         High-level interface for solving equations.
 
         Args:
             lambda_bound: an arbitrary chosen constant, influence only convergence speed.
             verbose: detailed info about training process.
             learning_rate: determines the step size at each iteration while moving toward a minimum of a loss function.
+            gamma: multiplicative factor of learning rate decay.
+            lr_change: the number of epochs after which the learning_rate change occurs
             eps: arbitrarily small number that uses for loss comparison criterion.
             tmax: maximum execution time.
             nmodels: smth
             name: model name if saved.
             abs_loss: absolute loss.
             use_cache: as is.
             cache_dir: directory where saved cache in.
@@ -218,67 +236,76 @@
             loss_oscillation_window: smth
             no_improvement_patience: smth
             model_randomize_parameter: creates a random model parameters (weights, biases) multiplied with a given randomize parameter.
             optimizer_mode: optimizer choice (Adam, SGD, LBFGS).
             step_plot_print: draws a figure through each given step.
             step_plot_save: saves a figure through each given step.
             image_save_dir: a directory where saved figure in.
+            tol: float constant, influences on error penalty in casual_loss algorithm. 
 
         Returns:
             model.
         """
         
 
         Cache_class = Model_prepare(self.grid, self.equal_cls,
                                                         self.model, self.mode)
 
         # prepare input data to uniform format 
         r = create_random_fn(model_randomize_parameter)
+
+
         #  use cache if needed
         if use_cache:
             self.model, min_loss = Cache_class.cache(cache_dir, nmodels,
                                                      lambda_bound,
                                                      cache_verbose,
                                                      model_randomize_parameter,
                                                      cache_model,
-                                                     weak_form=self.weak_form,)
+                                                     weak_form=self.weak_form)
             
             Solution_class = Solution(self.grid, self.equal_cls,
                                       self.model, self.mode)
         else:
             Solution_class = Solution(self.grid, self.equal_cls,
                                       self.model, self.mode)
             min_loss = Solution_class.loss_evaluation(lambda_bound=lambda_bound,
-                                                      weak_form=self.weak_form)
+                                                      weak_form=self.weak_form,
+                                                      tol=tol)
         
+        self.plot = Plots(self.model, self.grid, self.mode)
+
         optimizer = self.optimizer_choice(optimizer_mode, learning_rate)
-    
+        if gamma != None:
+            scheduler = ExponentialLR(optimizer, gamma=gamma)
+
         # standard NN stuff
         if verbose:
             print('[{}] initial (min) loss is {}'.format(
                 datetime.datetime.now(), min_loss))
     
         t = 0
     
         last_loss = np.zeros(loss_oscillation_window) + float(min_loss)
         line = np.polyfit(range(loss_oscillation_window), last_loss, 1)
 
         def closure():
             nonlocal cur_loss
             optimizer.zero_grad()
             loss = Solution_class.loss_evaluation(
-                lambda_bound = lambda_bound, weak_form=self.weak_form)
+                lambda_bound = lambda_bound, weak_form=self.weak_form,
+                                                            tol=tol)
             loss.backward()
             cur_loss = loss.item()
             return loss
 
         stop_dings = 0
         t_imp_start = 0
         # to stop train proceduce we fit the line in the loss data
-        # if line is flat enough 5 times, we stop the procedure
+        # if line is flat enough "patience" times, we stop the procedure
         cur_loss = min_loss
         while stop_dings <= patience:
             optimizer.step(closure)
 
             if cur_loss != cur_loss:
                 print(f'Loss is equal to NaN, something went wrong (LBFGS+high'
                  f'leraning rate and pytorch<1.12 could be the problem)')
@@ -291,64 +318,68 @@
                 min_loss = cur_loss
                 t_imp_start = t
 
             if verbose:
                 info_string='Step = {} loss = {:.6f} normalized loss line= {:.6f}x+{:.6f}. There was {} stop dings already.'.format(
                                                                         t, cur_loss, line[0]/cur_loss, line[1]/cur_loss, stop_dings+1)
 
+            if gamma != None and t % lr_change == 0:
+                 scheduler.step()
+
+
             if t%loss_oscillation_window == 0:
                 line = np.polyfit(range(loss_oscillation_window), last_loss, 1)
                 if abs(line[0]/cur_loss) < eps and t > 0:
                     stop_dings += 1
                     if self.mode =='NN' or self.mode =='autograd':
                         self.model.apply(r)
                     if verbose:
                         print('[{}] Oscillation near the same loss'.format(
                             datetime.datetime.now()))
                         print(info_string)
                         if step_plot_print or step_plot_save:
-                            self.solution_print(title='Iteration = ' + str(t),
+                            self.plot.solution_print(title='Iteration = ' + str(t),
                                                 solution_print=step_plot_print,
                                                 solution_save=step_plot_save,
                                                 save_dir=image_save_dir)
 
             if (t-t_imp_start) == no_improvement_patience:
                 if verbose:
                     print('[{}] No improvement in {} steps'.format(
                         datetime.datetime.now(),no_improvement_patience))
                     print(info_string)
                     if step_plot_print or step_plot_save:
-                        self.solution_print(title='Iteration = ' + str(t),
+                        self.plot.solution_print(title='Iteration = ' + str(t),
                                                 solution_print=step_plot_print,
                                                 solution_save=step_plot_save,
                                                 save_dir=image_save_dir)
                 t_imp_start = t
                 stop_dings += 1
                 if self.mode == 'NN' or self.mode == 'autograd':
                         self.model.apply(r)
 
 
             if abs_loss != None and cur_loss < abs_loss:
                 if verbose:
                     print('[{}] Absolute value of loss is lower than threshold'.format(datetime.datetime.now()))
                     print(info_string)
                     if step_plot_print or step_plot_save:
-                        self.solution_print(title='Iteration = ' + str(t),
+                        self.plot.solution_print(title='Iteration = ' + str(t),
                                                 solution_print=step_plot_print,
                                                 solution_save=step_plot_save,
                                                 save_dir=image_save_dir)
                 stop_dings += 1
 
 
             if print_every != None and (t % print_every == 0) and verbose:
                 print('[{}] Print every {} step'.format(
                     datetime.datetime.now(),print_every))
                 print(info_string)
                 if step_plot_print or step_plot_save:
-                    self.solution_print(title='Iteration = ' + str(t),
+                    self.plot.solution_print(title='Iteration = ' + str(t),
                                                 solution_print=step_plot_print,
                                                 solution_save=step_plot_save,
                                                 save_dir=image_save_dir)
             t += 1
             if t > tmax:
                 break
         if save_always:
```

### Comparing `tedeous-0.1.2/tedeous.egg-info/PKG-INFO` & `tedeous-0.2.0/tedeous.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tedeous
-Version: 0.1.2
+Version: 0.2.0
 Summary: TEDEouS - Torch Exhaustive Differential Equations Solver. Differential equation solver, based on pytorch library
 Author: Alexander Hvatov
 Author-email: itmo.nss.team@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

