# Comparing `tmp/dataclass_bakery_patched-0.3.0.tar.gz` & `tmp/dataclass_bakery_patched-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataclass_bakery_patched-0.3.0.tar", max compression
+gzip compressed data, was "dataclass_bakery_patched-0.4.0.tar", max compression
```

## Comparing `dataclass_bakery_patched-0.3.0.tar` & `dataclass_bakery_patched-0.4.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0        0 2023-06-13 08:43:13.493926 dataclass_bakery_patched-0.3.0/dataclass_bakery_patched/__init__.py
--rw-r--r--   0        0        0      691 2023-06-13 08:43:13.493926 dataclass_bakery_patched-0.3.0/dataclass_bakery_patched/baker.py
--rw-r--r--   0        0        0        0 2023-06-13 08:43:13.493926 dataclass_bakery_patched-0.3.0/dataclass_bakery_patched/generators/__init__.py
--rw-r--r--   0        0        0     2868 2023-06-13 08:43:13.495241 dataclass_bakery_patched-0.3.0/dataclass_bakery_patched/generators/defaults.py
--rw-r--r--   0        0        0      145 2023-06-13 08:43:13.495241 dataclass_bakery_patched-0.3.0/dataclass_bakery_patched/generators/generators_exceptions.py
--rw-r--r--   0        0        0      326 2023-06-13 08:43:13.496524 dataclass_bakery_patched-0.3.0/dataclass_bakery_patched/generators/random_bool_generator.py
--rw-r--r--   0        0        0      876 2023-06-13 08:43:13.496524 dataclass_bakery_patched-0.3.0/dataclass_bakery_patched/generators/random_complex_generator.py
--rw-r--r--   0        0        0     3072 2023-06-13 10:21:54.299061 dataclass_bakery_patched-0.3.0/dataclass_bakery_patched/generators/random_data_class_generator.py
--rw-r--r--   0        0        0      796 2023-06-13 08:43:13.497964 dataclass_bakery_patched-0.3.0/dataclass_bakery_patched/generators/random_decimal_generator.py
--rw-r--r--   0        0        0     1796 2023-06-13 08:43:13.499432 dataclass_bakery_patched-0.3.0/dataclass_bakery_patched/generators/random_dict_generator.py
--rw-r--r--   0        0        0      708 2023-06-13 08:43:13.499432 dataclass_bakery_patched-0.3.0/dataclass_bakery_patched/generators/random_float_generator.py
--rw-r--r--   0        0        0      178 2023-06-13 08:43:13.499432 dataclass_bakery_patched-0.3.0/dataclass_bakery_patched/generators/random_generator.py
--rw-r--r--   0        0        0      571 2023-06-13 08:43:13.500705 dataclass_bakery_patched-0.3.0/dataclass_bakery_patched/generators/random_int_generator.py
--rw-r--r--   0        0        0     1195 2023-06-13 08:43:13.500705 dataclass_bakery_patched-0.3.0/dataclass_bakery_patched/generators/random_list_generator.py
--rw-r--r--   0        0        0      546 2023-06-13 08:43:13.501776 dataclass_bakery_patched-0.3.0/dataclass_bakery_patched/generators/random_option_generator.py
--rw-r--r--   0        0        0      612 2023-06-13 08:43:13.501776 dataclass_bakery_patched-0.3.0/dataclass_bakery_patched/generators/random_path_generator.py
--rw-r--r--   0        0        0      681 2023-06-13 08:43:13.503015 dataclass_bakery_patched-0.3.0/dataclass_bakery_patched/generators/random_range_generator.py
--rw-r--r--   0        0        0      810 2023-06-13 08:43:13.503015 dataclass_bakery_patched-0.3.0/dataclass_bakery_patched/generators/random_set_generator.py
--rw-r--r--   0        0        0      596 2023-06-13 08:43:13.504423 dataclass_bakery_patched-0.3.0/dataclass_bakery_patched/generators/random_str_generator.py
--rw-r--r--   0        0        0     1210 2023-06-13 08:43:13.505433 dataclass_bakery_patched-0.3.0/dataclass_bakery_patched/generators/random_tuple_generator.py
--rw-r--r--   0        0        0      277 2023-06-13 08:43:13.505433 dataclass_bakery_patched-0.3.0/dataclass_bakery_patched/generators/random_uuid_generator.py
--rw-r--r--   0        0        0    11558 2023-06-13 08:43:13.449996 dataclass_bakery_patched-0.3.0/LICENSE
--rw-r--r--   0        0        0      539 2023-06-13 11:20:10.612156 dataclass_bakery_patched-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1218 2023-06-13 08:43:13.451303 dataclass_bakery_patched-0.3.0/README.md
--rw-r--r--   0        0        0     1559 1970-01-01 00:00:00.000000 dataclass_bakery_patched-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-13 08:43:13.493926 dataclass_bakery_patched-0.4.0/dataclass_bakery_patched/__init__.py
+-rw-r--r--   0        0        0      650 2023-06-13 11:22:33.735622 dataclass_bakery_patched-0.4.0/dataclass_bakery_patched/baker.py
+-rw-r--r--   0        0        0        0 2023-06-13 08:43:13.493926 dataclass_bakery_patched-0.4.0/dataclass_bakery_patched/generators/__init__.py
+-rw-r--r--   0        0        0     2980 2023-06-13 11:23:25.696246 dataclass_bakery_patched-0.4.0/dataclass_bakery_patched/generators/defaults.py
+-rw-r--r--   0        0        0      145 2023-06-13 08:43:13.495241 dataclass_bakery_patched-0.4.0/dataclass_bakery_patched/generators/generators_exceptions.py
+-rw-r--r--   0        0        0      334 2023-06-13 11:23:34.985109 dataclass_bakery_patched-0.4.0/dataclass_bakery_patched/generators/random_bool_generator.py
+-rw-r--r--   0        0        0      892 2023-06-13 11:23:37.746882 dataclass_bakery_patched-0.4.0/dataclass_bakery_patched/generators/random_complex_generator.py
+-rw-r--r--   0        0        0     3080 2023-06-13 11:23:39.750171 dataclass_bakery_patched-0.4.0/dataclass_bakery_patched/generators/random_data_class_generator.py
+-rw-r--r--   0        0        0      812 2023-06-13 11:23:52.467563 dataclass_bakery_patched-0.4.0/dataclass_bakery_patched/generators/random_decimal_generator.py
+-rw-r--r--   0        0        0     1820 2023-06-13 11:23:54.182632 dataclass_bakery_patched-0.4.0/dataclass_bakery_patched/generators/random_dict_generator.py
+-rw-r--r--   0        0        0      724 2023-06-13 11:23:57.623576 dataclass_bakery_patched-0.4.0/dataclass_bakery_patched/generators/random_float_generator.py
+-rw-r--r--   0        0        0      178 2023-06-13 08:43:13.499432 dataclass_bakery_patched-0.4.0/dataclass_bakery_patched/generators/random_generator.py
+-rw-r--r--   0        0        0      587 2023-06-13 11:24:01.861372 dataclass_bakery_patched-0.4.0/dataclass_bakery_patched/generators/random_int_generator.py
+-rw-r--r--   0        0        0     1219 2023-06-13 11:24:04.043714 dataclass_bakery_patched-0.4.0/dataclass_bakery_patched/generators/random_list_generator.py
+-rw-r--r--   0        0        0      562 2023-06-13 11:24:06.361799 dataclass_bakery_patched-0.4.0/dataclass_bakery_patched/generators/random_option_generator.py
+-rw-r--r--   0        0        0      636 2023-06-13 11:24:08.697490 dataclass_bakery_patched-0.4.0/dataclass_bakery_patched/generators/random_path_generator.py
+-rw-r--r--   0        0        0      697 2023-06-13 11:24:10.611366 dataclass_bakery_patched-0.4.0/dataclass_bakery_patched/generators/random_range_generator.py
+-rw-r--r--   0        0        0      826 2023-06-13 11:24:12.802182 dataclass_bakery_patched-0.4.0/dataclass_bakery_patched/generators/random_set_generator.py
+-rw-r--r--   0        0        0      619 2023-06-13 11:24:35.759623 dataclass_bakery_patched-0.4.0/dataclass_bakery_patched/generators/random_str_generator.py
+-rw-r--r--   0        0        0     1234 2023-06-13 11:24:17.288064 dataclass_bakery_patched-0.4.0/dataclass_bakery_patched/generators/random_tuple_generator.py
+-rw-r--r--   0        0        0      285 2023-06-13 11:24:19.756139 dataclass_bakery_patched-0.4.0/dataclass_bakery_patched/generators/random_uuid_generator.py
+-rw-r--r--   0        0        0    11558 2023-06-13 08:43:13.449996 dataclass_bakery_patched-0.4.0/LICENSE
+-rw-r--r--   0        0        0      539 2023-06-13 11:24:50.856739 dataclass_bakery_patched-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1218 2023-06-13 08:43:13.451303 dataclass_bakery_patched-0.4.0/README.md
+-rw-r--r--   0        0        0     1559 1970-01-01 00:00:00.000000 dataclass_bakery_patched-0.4.0/PKG-INFO
```

### Comparing `dataclass_bakery_patched-0.3.0/dataclass_bakery_patched/baker.py` & `dataclass_bakery_patched-0.4.0/dataclass_bakery_patched/baker.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 from typing import Any, Dict, List, Optional, Union
 
-from dataclass_bakery.generators.random_data_class_generator import (
+from generators.random_data_class_generator import (
     RandomDataClassGenerator,
 )
 
 
 def make(
     _data_class: Any,
     _quantity: Optional[int] = 1,
     _attr_defaults: Optional[Dict] = {},
 ) -> Union[List, Any]:
     random_data_class_generator = RandomDataClassGenerator()
 
     data_class_objects = []
     for _ in range(_quantity):
-        data_class_object = random_data_class_generator.generate(
-            _data_class, **_attr_defaults
-        )
+        data_class_object = random_data_class_generator.generate(_data_class, **_attr_defaults)
         data_class_objects.append(data_class_object)
 
     if _quantity > 1:
         return data_class_objects
 
     return data_class_object
```

### Comparing `dataclass_bakery_patched-0.3.0/dataclass_bakery_patched/generators/defaults.py` & `dataclass_bakery_patched-0.4.0/dataclass_bakery_patched/generators/defaults.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from decimal import Decimal
 from pathlib import Path
 from typing import Literal
 from uuid import UUID
 
-from dataclass_bakery.generators.random_bool_generator import RandomBoolGenerator
-from dataclass_bakery.generators.random_complex_generator import RandomComplexGenerator
-from dataclass_bakery.generators.random_decimal_generator import RandomDecimalGenerator
-from dataclass_bakery.generators.random_dict_generator import RandomDictGenerator
-from dataclass_bakery.generators.random_float_generator import RandomFloatGenerator
-from dataclass_bakery.generators.random_int_generator import RandomIntGenerator
-from dataclass_bakery.generators.random_list_generator import RandomListGenerator
-from dataclass_bakery.generators.random_option_generator import RandomOptionGenerator
-from dataclass_bakery.generators.random_path_generator import RandomPathGenerator
-from dataclass_bakery.generators.random_range_generator import RandomRangeGenerator
-from dataclass_bakery.generators.random_set_generator import RandomSetGenerator
-from dataclass_bakery.generators.random_str_generator import RandomStrGenerator
-from dataclass_bakery.generators.random_tuple_generator import RandomTupleGenerator
-from dataclass_bakery.generators.random_uuid_generator import RandomUuidGenerator
+from dataclass_bakery_patched.generators.random_bool_generator import RandomBoolGenerator
+from dataclass_bakery_patched.generators.random_complex_generator import RandomComplexGenerator
+from dataclass_bakery_patched.generators.random_decimal_generator import RandomDecimalGenerator
+from dataclass_bakery_patched.generators.random_dict_generator import RandomDictGenerator
+from dataclass_bakery_patched.generators.random_float_generator import RandomFloatGenerator
+from dataclass_bakery_patched.generators.random_int_generator import RandomIntGenerator
+from dataclass_bakery_patched.generators.random_list_generator import RandomListGenerator
+from dataclass_bakery_patched.generators.random_option_generator import RandomOptionGenerator
+from dataclass_bakery_patched.generators.random_path_generator import RandomPathGenerator
+from dataclass_bakery_patched.generators.random_range_generator import RandomRangeGenerator
+from dataclass_bakery_patched.generators.random_set_generator import RandomSetGenerator
+from dataclass_bakery_patched.generators.random_str_generator import RandomStrGenerator
+from dataclass_bakery_patched.generators.random_tuple_generator import RandomTupleGenerator
+from dataclass_bakery_patched.generators.random_uuid_generator import RandomUuidGenerator
 
 # Generators
 TYPING_GENERATORS = {
     str: RandomStrGenerator,
     int: RandomIntGenerator,
     float: RandomFloatGenerator,
     complex: RandomComplexGenerator,
```

### Comparing `dataclass_bakery_patched-0.3.0/dataclass_bakery_patched/generators/random_complex_generator.py` & `dataclass_bakery_patched-0.4.0/dataclass_bakery_patched/generators/random_complex_generator.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import random
 
-from dataclass_bakery.generators import defaults
-from dataclass_bakery.generators.random_generator import RandomGenerator
+from dataclass_bakery_patched.generators import defaults
+from dataclass_bakery_patched.generators.random_generator import RandomGenerator
 
 
 class RandomComplexGenerator(RandomGenerator):
     """
     Class to generate random complex number
     """
```

### Comparing `dataclass_bakery_patched-0.3.0/dataclass_bakery_patched/generators/random_data_class_generator.py` & `dataclass_bakery_patched-0.4.0/dataclass_bakery_patched/generators/random_data_class_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from dataclasses import is_dataclass
 from typing import _GenericAlias, Any, Literal, Union, Dict
 
-from dataclass_bakery.generators import defaults
+from dataclass_bakery_patched.generators import defaults
 
 
 def collect_all_attributes(dclass: Any) -> Dict:
     if not is_dataclass(dclass):
         return {}
     attrs = dict(dclass.__annotations__.items())
     for pclass in dclass.__bases__:
```

### Comparing `dataclass_bakery_patched-0.3.0/dataclass_bakery_patched/generators/random_decimal_generator.py` & `dataclass_bakery_patched-0.4.0/dataclass_bakery_patched/generators/random_decimal_generator.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import random
 from decimal import Decimal
 
-from dataclass_bakery.generators import defaults
-from dataclass_bakery.generators.random_generator import RandomGenerator
+from dataclass_bakery_patched.generators import defaults
+from dataclass_bakery_patched.generators.random_generator import RandomGenerator
 
 
 class RandomDecimalGenerator(RandomGenerator):
     """
     Class to generate random decimal number
     """
```

### Comparing `dataclass_bakery_patched-0.3.0/dataclass_bakery_patched/generators/random_dict_generator.py` & `dataclass_bakery_patched-0.4.0/dataclass_bakery_patched/generators/random_dict_generator.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import is_dataclass
 
-from dataclass_bakery.generators import defaults
-from dataclass_bakery.generators import random_data_class_generator
-from dataclass_bakery.generators.random_generator import RandomGenerator
+from dataclass_bakery_patched.generators import defaults
+from dataclass_bakery_patched.generators import random_data_class_generator
+from dataclass_bakery_patched.generators.random_generator import RandomGenerator
 
 
 class RandomDictGenerator(RandomGenerator):
     """
     Class to generate random dict
     """
```

### Comparing `dataclass_bakery_patched-0.3.0/dataclass_bakery_patched/generators/random_float_generator.py` & `dataclass_bakery_patched-0.4.0/dataclass_bakery_patched/generators/random_range_generator.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import random
 
-from dataclass_bakery.generators import defaults
-from dataclass_bakery.generators.random_generator import RandomGenerator
+from dataclass_bakery_patched.generators import defaults
+from dataclass_bakery_patched.generators.random_generator import RandomGenerator
 
 
-class RandomFloatGenerator(RandomGenerator):
+class RandomRangeGenerator(RandomGenerator):
     """
-    Class to generate random float number
+    Class to generate random range
     """
 
-    def generate(self, *args, **kwargs) -> float:
+    def generate(self, *args, **kwargs) -> range:
         min_limit = kwargs.get(defaults.NUMBER_MIN_LIMIT_ARG, defaults.NUMBER_MIN_LIMIT)
         max_limit = kwargs.get(defaults.NUMBER_MAX_LIMIT_ARG, defaults.NUMBER_MAX_LIMIT)
-        decimals = kwargs.get(defaults.DECIMALS_ARG, defaults.DECIMALS)
-        random_number = random.uniform(min_limit, max_limit)
-        rounded_number = round(random_number, decimals)
-        return rounded_number
+        range_start = random.randint(min_limit, max_limit)
+        range_end = random.randint(range_start, max_limit)
+        random_range = range(range_start, range_end)
+        return random_range
```

### Comparing `dataclass_bakery_patched-0.3.0/dataclass_bakery_patched/generators/random_int_generator.py` & `dataclass_bakery_patched-0.4.0/dataclass_bakery_patched/generators/random_int_generator.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import random
 
-from dataclass_bakery.generators import defaults
-from dataclass_bakery.generators.random_generator import RandomGenerator
+from dataclass_bakery_patched.generators import defaults
+from dataclass_bakery_patched.generators.random_generator import RandomGenerator
 
 
 class RandomIntGenerator(RandomGenerator):
     """
     Class to generate random int number
     """
```

### Comparing `dataclass_bakery_patched-0.3.0/dataclass_bakery_patched/generators/random_list_generator.py` & `dataclass_bakery_patched-0.4.0/dataclass_bakery_patched/generators/random_list_generator.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import is_dataclass
 
-from dataclass_bakery.generators import defaults
-from dataclass_bakery.generators import random_data_class_generator
-from dataclass_bakery.generators.random_generator import RandomGenerator
+from dataclass_bakery_patched.generators import defaults
+from dataclass_bakery_patched.generators import random_data_class_generator
+from dataclass_bakery_patched.generators.random_generator import RandomGenerator
 
 
 class RandomListGenerator(RandomGenerator):
     """
     Class to generate random list
     """
```

### Comparing `dataclass_bakery_patched-0.3.0/dataclass_bakery_patched/generators/random_option_generator.py` & `dataclass_bakery_patched-0.4.0/dataclass_bakery_patched/generators/random_option_generator.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import random
 from typing import Any
 
-from dataclass_bakery.generators import defaults
-from dataclass_bakery.generators.random_generator import RandomGenerator
+from dataclass_bakery_patched.generators import defaults
+from dataclass_bakery_patched.generators.random_generator import RandomGenerator
 
 
 class RandomOptionGenerator(RandomGenerator):
     """
     Class to generate random option
     """
```

### Comparing `dataclass_bakery_patched-0.3.0/dataclass_bakery_patched/generators/random_path_generator.py` & `dataclass_bakery_patched-0.4.0/dataclass_bakery_patched/generators/random_path_generator.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
 
-from dataclass_bakery.generators import defaults
-from dataclass_bakery.generators.random_generator import RandomGenerator
-from dataclass_bakery.generators.random_str_generator import RandomStrGenerator
+from dataclass_bakery_patched.generators import defaults
+from dataclass_bakery_patched.generators.random_generator import RandomGenerator
+from dataclass_bakery_patched.generators.random_str_generator import RandomStrGenerator
 
 
 class RandomPathGenerator(RandomGenerator):
     def generate(self, *args, **kwargs) -> Path:
         generator = RandomStrGenerator()
         max_path_length = kwargs.get(defaults.MAX_LENGTH_ARG, defaults.MAX_PATH_LENGTH)
         folders = [generator.generate() for _ in range(max_path_length)]
```

### Comparing `dataclass_bakery_patched-0.3.0/dataclass_bakery_patched/generators/random_range_generator.py` & `dataclass_bakery_patched-0.4.0/dataclass_bakery_patched/generators/random_set_generator.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,25 @@
-import random
+from dataclass_bakery_patched.generators import defaults
+from dataclass_bakery_patched.generators.random_generator import RandomGenerator
 
-from dataclass_bakery.generators import defaults
-from dataclass_bakery.generators.random_generator import RandomGenerator
 
-
-class RandomRangeGenerator(RandomGenerator):
+class RandomSetGenerator(RandomGenerator):
     """
-    Class to generate random range
+    Class to generate random set
     """
 
-    def generate(self, *args, **kwargs) -> range:
-        min_limit = kwargs.get(defaults.NUMBER_MIN_LIMIT_ARG, defaults.NUMBER_MIN_LIMIT)
-        max_limit = kwargs.get(defaults.NUMBER_MAX_LIMIT_ARG, defaults.NUMBER_MAX_LIMIT)
-        range_start = random.randint(min_limit, max_limit)
-        range_end = random.randint(range_start, max_limit)
-        random_range = range(range_start, range_end)
-        return random_range
+    def generate(self, *args, **kwargs) -> set:
+        max_length = kwargs.get(defaults.MAX_LENGTH_ARG, defaults.MAX_SET_LENGTH)
+
+        default_value_type = kwargs.get(
+            defaults.DEFAULT_VALUE_TYPE_ARG, defaults.DEFAULT_VALUE_TYPE
+        )
+
+        value_type = kwargs.get(defaults.VALUE_TYPE_ARG, default_value_type)
+        generator = defaults.TYPING_GENERATORS[value_type]()
+
+        random_set = set()
+        for _ in range(max_length):
+            set_value = generator.generate()
+            random_set.add(set_value)
+
+        return random_set
```

### Comparing `dataclass_bakery_patched-0.3.0/dataclass_bakery_patched/generators/random_set_generator.py` & `dataclass_bakery_patched-0.4.0/dataclass_bakery_patched/generators/random_tuple_generator.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,35 @@
-from dataclass_bakery.generators import defaults
-from dataclass_bakery.generators.random_generator import RandomGenerator
+from dataclasses import is_dataclass
 
+from dataclass_bakery_patched.generators import defaults
+from dataclass_bakery_patched.generators import random_data_class_generator
+from dataclass_bakery_patched.generators.random_generator import RandomGenerator
 
-class RandomSetGenerator(RandomGenerator):
+
+class RandomTupleGenerator(RandomGenerator):
     """
-    Class to generate random set
+    Class to generate random tuple
     """
 
-    def generate(self, *args, **kwargs) -> set:
-        max_length = kwargs.get(defaults.MAX_LENGTH_ARG, defaults.MAX_SET_LENGTH)
+    def generate(self, *args, **kwargs) -> tuple:
+        max_length = kwargs.get(defaults.MAX_LENGTH_ARG, defaults.MAX_TUPLE_LENGTH)
 
         default_value_type = kwargs.get(
             defaults.DEFAULT_VALUE_TYPE_ARG, defaults.DEFAULT_VALUE_TYPE
         )
 
         value_type = kwargs.get(defaults.VALUE_TYPE_ARG, default_value_type)
-        generator = defaults.TYPING_GENERATORS[value_type]()
 
-        random_set = set()
+        if is_dataclass(value_type):
+            generator = random_data_class_generator.RandomDataClassGenerator()
+        else:
+            generator = defaults.TYPING_GENERATORS[value_type]()
+
+        random_tuple = []
         for _ in range(max_length):
-            set_value = generator.generate()
-            random_set.add(set_value)
+            if is_dataclass(value_type):
+                tuple_value = generator.generate(value_type)
+            else:
+                tuple_value = generator.generate()
+            random_tuple.append(tuple_value)
 
-        return random_set
+        return tuple(random_tuple)
```

### Comparing `dataclass_bakery_patched-0.3.0/dataclass_bakery_patched/generators/random_str_generator.py` & `dataclass_bakery_patched-0.4.0/dataclass_bakery_patched/generators/random_str_generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-import random, string
+import random
+import string
 
-from dataclass_bakery.generators import defaults
-from dataclass_bakery.generators.random_generator import RandomGenerator
+from dataclass_bakery_patched.generators import defaults
+from dataclass_bakery_patched.generators.random_generator import RandomGenerator
 
 
 class RandomStrGenerator(RandomGenerator):
     """
     Class to generate random string
     """
```

### Comparing `dataclass_bakery_patched-0.3.0/LICENSE` & `dataclass_bakery_patched-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dataclass_bakery_patched-0.3.0/pyproject.toml` & `dataclass_bakery_patched-0.4.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dataclass-bakery-patched"
-version = "0.3.0"
+version = "0.4.0"
 description = "A fork from dataclass-bakery, with a tweak to consider inherited attributes when creating dataclasses."
 authors = ["Adam Ruman <469068@muni.cz>"]
 readme = "README.md"
 packages = [{include = "dataclass_bakery_patched"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `dataclass_bakery_patched-0.3.0/README.md` & `dataclass_bakery_patched-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `dataclass_bakery_patched-0.3.0/PKG-INFO` & `dataclass_bakery_patched-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataclass-bakery-patched
-Version: 0.3.0
+Version: 0.4.0
 Summary: A fork from dataclass-bakery, with a tweak to consider inherited attributes when creating dataclasses.
 Author: Adam Ruman
 Author-email: 469068@muni.cz
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

