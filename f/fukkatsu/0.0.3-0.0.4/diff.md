# Comparing `tmp/fukkatsu-0.0.3.tar.gz` & `tmp/fukkatsu-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fukkatsu-0.0.3.tar", last modified: Mon Jun  5 00:23:53 2023, max compression
+gzip compressed data, was "fukkatsu-0.0.4.tar", last modified: Tue Jun 13 00:18:39 2023, max compression
```

## Comparing `fukkatsu-0.0.3.tar` & `fukkatsu-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 00:23:53.512154 fukkatsu-0.0.3/
--rw-rw-rw-   0        0        0      519 2023-06-04 23:17:03.000000 fukkatsu-0.0.3/CHANGELOG.md
--rw-rw-rw-   0        0        0     1089 2023-04-28 00:39:24.000000 fukkatsu-0.0.3/LICENSE
--rw-rw-rw-   0        0        0       58 2022-10-31 01:25:26.000000 fukkatsu-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0    10488 2023-06-05 00:23:53.506492 fukkatsu-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     9849 2023-06-05 00:14:18.000000 fukkatsu-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 00:23:53.422550 fukkatsu-0.0.3/fukkatsu/
--rw-rw-rw-   0        0        0     7833 2023-06-05 00:09:44.000000 fukkatsu-0.0.3/fukkatsu/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 00:23:53.469382 fukkatsu-0.0.3/fukkatsu/memory/
--rw-rw-rw-   0        0        0       75 2023-05-20 04:07:03.000000 fukkatsu-0.0.3/fukkatsu/memory/__init__.py
--rw-rw-rw-   0        0        0      663 2023-05-20 04:07:01.000000 fukkatsu-0.0.3/fukkatsu/memory/manage.py
--rw-rw-rw-   0        0        0       23 2023-05-20 04:07:01.000000 fukkatsu-0.0.3/fukkatsu/memory/short.py
-drwxrwxrwx   0        0        0        0 2023-06-05 00:23:53.494481 fukkatsu-0.0.3/fukkatsu/utils/
--rw-rw-rw-   0        0        0      110 2023-05-18 05:17:09.000000 fukkatsu-0.0.3/fukkatsu/utils/__init__.py
--rw-rw-rw-   0        0        0     3617 2023-06-04 21:33:13.000000 fukkatsu-0.0.3/fukkatsu/utils/helper.py
--rw-rw-rw-   0        0        0     2241 2023-06-05 00:09:44.000000 fukkatsu-0.0.3/fukkatsu/utils/medic.py
--rw-rw-rw-   0        0        0     1583 2023-05-20 04:08:40.000000 fukkatsu-0.0.3/fukkatsu/utils/prompt.py
-drwxrwxrwx   0        0        0        0 2023-06-05 00:23:53.453760 fukkatsu-0.0.3/fukkatsu.egg-info/
--rw-rw-rw-   0        0        0    10488 2023-06-05 00:23:52.000000 fukkatsu-0.0.3/fukkatsu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      411 2023-06-05 00:23:53.000000 fukkatsu-0.0.3/fukkatsu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 00:23:52.000000 fukkatsu-0.0.3/fukkatsu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-06-05 00:23:52.000000 fukkatsu-0.0.3/fukkatsu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-05 00:23:53.000000 fukkatsu-0.0.3/fukkatsu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 00:23:53.512154 fukkatsu-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1086 2023-06-04 21:25:11.000000 fukkatsu-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 00:18:39.891733 fukkatsu-0.0.4/
+-rw-rw-rw-   0        0        0      914 2023-06-12 23:03:57.000000 fukkatsu-0.0.4/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1089 2023-04-28 00:39:24.000000 fukkatsu-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0       58 2022-10-31 01:25:26.000000 fukkatsu-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0    12611 2023-06-13 00:18:39.884718 fukkatsu-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0    11970 2023-06-12 23:37:54.000000 fukkatsu-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 00:18:39.807747 fukkatsu-0.0.4/fukkatsu/
+-rw-rw-rw-   0        0        0     8008 2023-06-13 00:03:15.000000 fukkatsu-0.0.4/fukkatsu/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 00:18:39.851079 fukkatsu-0.0.4/fukkatsu/memory/
+-rw-rw-rw-   0        0        0       75 2023-05-20 04:07:03.000000 fukkatsu-0.0.4/fukkatsu/memory/__init__.py
+-rw-rw-rw-   0        0        0      663 2023-05-20 04:07:01.000000 fukkatsu-0.0.4/fukkatsu/memory/manage.py
+-rw-rw-rw-   0        0        0       23 2023-05-20 04:07:01.000000 fukkatsu-0.0.4/fukkatsu/memory/short.py
+drwxrwxrwx   0        0        0        0 2023-06-13 00:18:39.870986 fukkatsu-0.0.4/fukkatsu/utils/
+-rw-rw-rw-   0        0        0      110 2023-05-18 05:17:09.000000 fukkatsu-0.0.4/fukkatsu/utils/__init__.py
+-rw-rw-rw-   0        0        0     4082 2023-06-12 22:53:43.000000 fukkatsu-0.0.4/fukkatsu/utils/helper.py
+-rw-rw-rw-   0        0        0     2241 2023-06-13 00:03:15.000000 fukkatsu-0.0.4/fukkatsu/utils/medic.py
+-rw-rw-rw-   0        0        0     1531 2023-06-07 22:47:31.000000 fukkatsu-0.0.4/fukkatsu/utils/prompt.py
+drwxrwxrwx   0        0        0        0 2023-06-13 00:18:39.837747 fukkatsu-0.0.4/fukkatsu.egg-info/
+-rw-rw-rw-   0        0        0    12611 2023-06-13 00:18:39.000000 fukkatsu-0.0.4/fukkatsu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      411 2023-06-13 00:18:39.000000 fukkatsu-0.0.4/fukkatsu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 00:18:39.000000 fukkatsu-0.0.4/fukkatsu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-06-13 00:18:39.000000 fukkatsu-0.0.4/fukkatsu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-13 00:18:39.000000 fukkatsu-0.0.4/fukkatsu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 00:18:39.892730 fukkatsu-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1086 2023-06-12 22:59:04.000000 fukkatsu-0.0.4/setup.py
```

### Comparing `fukkatsu-0.0.3/LICENSE` & `fukkatsu-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fukkatsu-0.0.3/PKG-INFO` & `fukkatsu-0.0.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: fukkatsu
-Version: 0.0.3
-Summary: A python library for runtime LLM supported code corrections.
-Home-page: https://github.com/maxmekiska/fukkatsu
-Author: Maximilian Mekiska
-Author-email: maxmekiska@gmail.com
-Keywords: machinelearning,llm,runtime,codecorrection
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # fukkatsu 復活 [![Downloads](https://pepy.tech/badge/fukkatsu)](https://pepy.tech/project/fukkatsu) [![PyPi](https://img.shields.io/pypi/v/fukkatsu.svg?color=blue)](https://pypi.org/project/fukkatsu/) [![GitHub license](https://img.shields.io/github/license/maxmekiska/fukkatsu?color=black)](https://github.com/maxmekiska/fukkatsu/blob/main/LICENSE) [![PyPI pyversions](https://img.shields.io/pypi/pyversions/fukkatsu.svg)](https://pypi.python.org/project/fukkatsu/)
 
 <br>
 
 | Build | Status|
 |---|---|
 | `MAIN BUILD`  |  ![master](https://github.com/maxmekiska/fukkatsu/actions/workflows/main.yml/badge.svg?branch=main) |
@@ -253,7 +237,58 @@
 
 ### `mutate`
 ```python
 def mutate(request: str = "", allow_installs: bool = False):
   ...
 ```
 </details>
+
+## Testing Capabilities
+
+This section will conduct a series of simulations to better understand fukkatsu's potential capabilities. To achieve this, multiple error types will be tested. Each error type and scenario will consist of a total of 25 runs under the same conditions. We will test the following hypotheses:
+
+### Hypotheses testing
+
+- H<sub>0</sub>: "The proportion of errors solved is not significantly greater than 0.5."
+- H<sub>1</sub>: "The proportion of errors solved is significantly greater than 0.5."
+
+We will consider a confidence interval of 0.05 and utilize a binomial distribution.
+
+```python
+import scipy.stats as stats
+
+successes = # number of successful repairs
+
+alpha = 0.05
+
+p_value = stats.binom_test(successes, n=25, p=0.5, alternative='greater')
+
+print(f"p_value: {p_value}")
+
+if p_value < alpha:
+    print("Reject the null hypothesis")
+    print("The proportion of errors solved is significantly greater than 0.5.")
+else:
+    print("Fail to reject the null hypothesis")
+    print("The proportion of errors solved is not significantly greater than 0.5.")
+```
+
+
+fukkatsu will utilize the `gpt-3.5-turbo` model in all simulations. For each simulation, 3 lives will be allocated. The functions will also be provided with sufficient context. 
+
+After conducting all the tests, we will finally apply a `chi-square test`. This test will help determine whether there is a statistically significant difference in the fukkatsu's performance across the error types. If the test results indicate a significant association, it suggests that the effectiveness of fukkatsu varies depending on the error type.
+
+```python
+import numpy as np
+from scipy.stats import chi2_contingency
+
+observed_counts = np.array([[10, 20], [15, 25], [5, 30]])
+
+chi2, p_value, dof, expected = chi2_contingency(observed_counts)
+
+print("Chi-square statistic:", chi2)
+print("P-value:", p_value)
+print("Degrees of freedom:", dof)
+print("Expected counts:", expected)
+```
+
+You can see each simulation recored in the different jupyter notebooks contained within the `research` directory.
```

### Comparing `fukkatsu-0.0.3/README.md` & `fukkatsu-0.0.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: fukkatsu
+Version: 0.0.4
+Summary: A python library for runtime LLM supported code corrections.
+Home-page: https://github.com/maxmekiska/fukkatsu
+Author: Maximilian Mekiska
+Author-email: maxmekiska@gmail.com
+Keywords: machinelearning,llm,runtime,codecorrection
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # fukkatsu 復活 [![Downloads](https://pepy.tech/badge/fukkatsu)](https://pepy.tech/project/fukkatsu) [![PyPi](https://img.shields.io/pypi/v/fukkatsu.svg?color=blue)](https://pypi.org/project/fukkatsu/) [![GitHub license](https://img.shields.io/github/license/maxmekiska/fukkatsu?color=black)](https://github.com/maxmekiska/fukkatsu/blob/main/LICENSE) [![PyPI pyversions](https://img.shields.io/pypi/pyversions/fukkatsu.svg)](https://pypi.python.org/project/fukkatsu/)
 
 <br>
 
 | Build | Status|
 |---|---|
 | `MAIN BUILD`  |  ![master](https://github.com/maxmekiska/fukkatsu/actions/workflows/main.yml/badge.svg?branch=main) |
@@ -237,7 +253,58 @@
 
 ### `mutate`
 ```python
 def mutate(request: str = "", allow_installs: bool = False):
   ...
 ```
 </details>
+
+## Testing Capabilities
+
+This section will conduct a series of simulations to better understand fukkatsu's potential capabilities. To achieve this, multiple error types will be tested. Each error type and scenario will consist of a total of 25 runs under the same conditions. We will test the following hypotheses:
+
+### Hypotheses testing
+
+- H<sub>0</sub>: "The proportion of errors solved is not significantly greater than 0.5."
+- H<sub>1</sub>: "The proportion of errors solved is significantly greater than 0.5."
+
+We will consider a confidence interval of 0.05 and utilize a binomial distribution.
+
+```python
+import scipy.stats as stats
+
+successes = # number of successful repairs
+
+alpha = 0.05
+
+p_value = stats.binom_test(successes, n=25, p=0.5, alternative='greater')
+
+print(f"p_value: {p_value}")
+
+if p_value < alpha:
+    print("Reject the null hypothesis")
+    print("The proportion of errors solved is significantly greater than 0.5.")
+else:
+    print("Fail to reject the null hypothesis")
+    print("The proportion of errors solved is not significantly greater than 0.5.")
+```
+
+
+fukkatsu will utilize the `gpt-3.5-turbo` model in all simulations. For each simulation, 3 lives will be allocated. The functions will also be provided with sufficient context. 
+
+After conducting all the tests, we will finally apply a `chi-square test`. This test will help determine whether there is a statistically significant difference in the fukkatsu's performance across the error types. If the test results indicate a significant association, it suggests that the effectiveness of fukkatsu varies depending on the error type.
+
+```python
+import numpy as np
+from scipy.stats import chi2_contingency
+
+observed_counts = np.array([[10, 20], [15, 25], [5, 30]])
+
+chi2, p_value, dof, expected = chi2_contingency(observed_counts)
+
+print("Chi-square statistic:", chi2)
+print("P-value:", p_value)
+print("Degrees of freedom:", dof)
+print("Expected counts:", expected)
+```
+
+You can see each simulation recored in the different jupyter notebooks contained within the `research` directory.
```

### Comparing `fukkatsu-0.0.3/fukkatsu/__init__.py` & `fukkatsu-0.0.4/fukkatsu/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,41 @@
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
+import copy
 import functools
 import logging
 import traceback
 
 from fukkatsu.memory import SHORT_TERM_MEMORY
 from fukkatsu.utils import (check_and_install_libraries, extract_imports,
-                            extract_text_between_backticks,
+                            extract_text_between_pipes,
                             insert_string_after_colon, remove_trace_lines,
                             remove_wrapper_name, return_input_arguments,
                             return_source_code)
 from fukkatsu.utils.medic import defibrillate, enhance
 
 
 def resurrect(lives: int = 1, additional_req: str = "", allow_installs: bool = False):
     def _resurrect(func):
         @functools.wraps(func)
         def wrapper(*args, **kwargs):
+            input_args = return_input_arguments(func, *args, **kwargs)
 
             try:
-                result = func(*args, **kwargs)
+                args_copy = copy.deepcopy(args)
+                kwargs_copy = copy.deepcopy(kwargs)
+                result = func(*args_copy, **kwargs_copy)
+
                 return result
 
             except Exception as e:
                 logging.exception(e)
                 trace = traceback.format_exc()
                 trace = remove_trace_lines(trace)
 
-                input_args = return_input_arguments(func, *args, **kwargs)
                 source = return_source_code(func)
                 source = remove_wrapper_name(source)
 
                 logging.warning(f"Input arguments: {input_args}\n")
                 logging.warning(f"\nSource Code: \n {source}\n")
 
                 if trace in SHORT_TERM_MEMORY.keys():
@@ -48,15 +52,15 @@
                         faulty_function=source,
                         error_trace=trace,
                         additional_req=additional_req,
                     )
                     logging.warning(
                         f"Received INITIAL RAW suggestion: {suggested_code}\n"
                     )
-                    suggested_code = extract_text_between_backticks(suggested_code)
+                    suggested_code = extract_text_between_pipes(suggested_code)
                     logging.warning(
                         f"Received INITIAL CLEANED suggestion: {suggested_code}\n"
                     )
 
                     import_block = extract_imports(suggested_code)
                     if allow_installs == True:
                         check_and_install_libraries(import_statements=import_block)
@@ -82,15 +86,19 @@
 
                         SHORT_TERM_MEMORY[trace] = suggested_code
                         logging.warning(
                             f"Reanimation successful, using {suggested_code}\n"
                         )
                         locals()[func.__name__] = new_function
 
-                        return new_function(*args, **kwargs)
+                        args_copy = copy.deepcopy(args)
+                        kwargs_copy = copy.deepcopy(kwargs)
+
+                        return new_function(*args_copy, **kwargs_copy)
+
                     except:
                         logging.exception(e)
                         trace = traceback.format_exc()
                         trace = remove_trace_lines(trace)
                         logging.warning(
                             "Reanimation failed, requesting new correction\n"
                         )
@@ -108,17 +116,15 @@
                                 faulty_function=suggested_code,
                                 error_trace=trace,
                                 additional_req=additional_req,
                             )
                             logging.warning(
                                 f"Received attempt RAW suggestion: {suggested_code}\n"
                             )
-                            suggested_code = extract_text_between_backticks(
-                                suggested_code
-                            )
+                            suggested_code = extract_text_between_pipes(suggested_code)
                             logging.warning(
                                 f"Received attempt CLEANED suggestion: {suggested_code}\n"
                             )
 
                             import_block = extract_imports(suggested_code)
                             if allow_installs == True:
                                 check_and_install_libraries(
@@ -154,15 +160,15 @@
             logging.warning("Requesting mutation\n")
             suggested_code = enhance(
                 inputs=input_args,
                 target_function=source,
                 request=request,
             )
             logging.warning(f"Received RAW suggestion mutation: {suggested_code}\n")
-            suggested_code = extract_text_between_backticks(suggested_code)
+            suggested_code = extract_text_between_pipes(suggested_code)
             logging.warning(f"Received CLEANED suggestion mutation: {suggested_code}\n")
 
             global_dict = globals()
             local_dict = locals()
 
             import_block = extract_imports(suggested_code)
             if allow_installs == True:
```

### Comparing `fukkatsu-0.0.3/fukkatsu/memory/manage.py` & `fukkatsu-0.0.4/fukkatsu/memory/manage.py`

 * *Files identical despite different names*

### Comparing `fukkatsu-0.0.3/fukkatsu/utils/helper.py` & `fukkatsu-0.0.4/fukkatsu/utils/helper.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,15 +15,32 @@
 
 def remove_wrapper_name(source_code: str) -> str:
     start_index = source_code.index("def")
     source_code = source_code[start_index:]
     return source_code
 
 
-def extract_text_between_backticks(message: str) -> str:
+def standardize_delimiters(code_block: str) -> str:
+    pattern = r"\|*\s*(?:python):?\|*"
+    return re.sub(pattern, "|||", code_block)
+
+
+def add_delimiters(message: str) -> str:
+    message = message.rstrip()
+    if message.endswith("|||"):
+        return message
+    elif message.count("|||") == 2:
+        return message
+    else:
+        return message + "|||"
+
+
+def extract_text_between_pipes(message: str) -> str:
+    message = standardize_delimiters(message)
+    message = add_delimiters(message)
     start_idx = message.find("|||") + 3
     end_idx = message.rfind("|||")
     if start_idx == -1 or end_idx == -1 or start_idx >= end_idx:
         return ""
     return message[start_idx:end_idx].strip()
```

### Comparing `fukkatsu-0.0.3/fukkatsu/utils/medic.py` & `fukkatsu-0.0.4/fukkatsu/utils/medic.py`

 * *Files identical despite different names*

### Comparing `fukkatsu-0.0.3/fukkatsu/utils/prompt.py` & `fukkatsu-0.0.4/fukkatsu/utils/prompt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 # Tokens: 29
 CONTEXT = (
     "You are a helpful large language model focusing on repairing and improving faulty code. "
     "Repair and improve the following faulty function: "
 )
 # Tokens: 27
 CONTEXT_MUTATE = (
-    "You are a helpful large language model focusing on improving and changing functions based on a Users request. "
+    "You are a helpful large language model focusing on improving and mutating functions based on a Users request. "
     "Improve and change the following function: "
 )
-# Tokens: 131
+# Tokens: 105
 OUTPUT_CONSTRAINTS = (
     "Your response needs to strictly follow the following requierements:\n"
     "1. Respond with exactly one code box.\n"
     "2. Provide only the code of the corrected function.\n"
-    "3. Do not import any additional libraries.\n"
-    "4. Do not provide examples or comments.\n"
-    "5. Make sure to prefix the requested python code with: ||| exactly and suffix the code with: ||| exactly.\n"
-    "6. When providing the corrected function, make sure to implement all additional logic explained in the faulty functions docstring.\n"
+    "3. Do not provide examples or comments.\n"
+    "4. Make sure to prefix the requested python code with: ||| exactly and suffix the code with: ||| exactly.\n"
+    "5. When providing the corrected function, make sure to implement all additional logic explained in the faulty functions docstring.\n"
 )
 # Tokens: 123
 OUTPUT_CONSTRAINTS_MUTATE = (
     "Your response needs to strictly follow the following requierements:\n"
     "1. Respond with exactly one code box.\n"
     "2. Provide only the code of the changed function.\n"
     "3. Do not provide examples or comments.\n"
```

### Comparing `fukkatsu-0.0.3/fukkatsu.egg-info/PKG-INFO` & `fukkatsu-0.0.4/fukkatsu.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fukkatsu
-Version: 0.0.3
+Version: 0.0.4
 Summary: A python library for runtime LLM supported code corrections.
 Home-page: https://github.com/maxmekiska/fukkatsu
 Author: Maximilian Mekiska
 Author-email: maxmekiska@gmail.com
 Keywords: machinelearning,llm,runtime,codecorrection
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -253,7 +253,58 @@
 
 ### `mutate`
 ```python
 def mutate(request: str = "", allow_installs: bool = False):
   ...
 ```
 </details>
+
+## Testing Capabilities
+
+This section will conduct a series of simulations to better understand fukkatsu's potential capabilities. To achieve this, multiple error types will be tested. Each error type and scenario will consist of a total of 25 runs under the same conditions. We will test the following hypotheses:
+
+### Hypotheses testing
+
+- H<sub>0</sub>: "The proportion of errors solved is not significantly greater than 0.5."
+- H<sub>1</sub>: "The proportion of errors solved is significantly greater than 0.5."
+
+We will consider a confidence interval of 0.05 and utilize a binomial distribution.
+
+```python
+import scipy.stats as stats
+
+successes = # number of successful repairs
+
+alpha = 0.05
+
+p_value = stats.binom_test(successes, n=25, p=0.5, alternative='greater')
+
+print(f"p_value: {p_value}")
+
+if p_value < alpha:
+    print("Reject the null hypothesis")
+    print("The proportion of errors solved is significantly greater than 0.5.")
+else:
+    print("Fail to reject the null hypothesis")
+    print("The proportion of errors solved is not significantly greater than 0.5.")
+```
+
+
+fukkatsu will utilize the `gpt-3.5-turbo` model in all simulations. For each simulation, 3 lives will be allocated. The functions will also be provided with sufficient context. 
+
+After conducting all the tests, we will finally apply a `chi-square test`. This test will help determine whether there is a statistically significant difference in the fukkatsu's performance across the error types. If the test results indicate a significant association, it suggests that the effectiveness of fukkatsu varies depending on the error type.
+
+```python
+import numpy as np
+from scipy.stats import chi2_contingency
+
+observed_counts = np.array([[10, 20], [15, 25], [5, 30]])
+
+chi2, p_value, dof, expected = chi2_contingency(observed_counts)
+
+print("Chi-square statistic:", chi2)
+print("P-value:", p_value)
+print("Degrees of freedom:", dof)
+print("Expected counts:", expected)
+```
+
+You can see each simulation recored in the different jupyter notebooks contained within the `research` directory.
```

### Comparing `fukkatsu-0.0.3/setup.py` & `fukkatsu-0.0.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     author="Maximilian Mekiska",
     author_email="maxmekiska@gmail.com",
     url="https://github.com/maxmekiska/fukkatsu",
     description="A python library for runtime LLM supported code corrections.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     name="fukkatsu",
-    version="0.0.3",
+    version="0.0.4",
     packages=find_packages(include=["fukkatsu", "fukkatsu.*"]),
     install_requires=[
         "setuptools >= 41.0.0",
         "openai >= 0.27.5, <= 0.28",
     ],
     classifiers=[
         "Programming Language :: Python :: 3.8",
```

