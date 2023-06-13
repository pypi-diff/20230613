# Comparing `tmp/pythonic-toolbox-1.1.8.tar.gz` & `tmp/pythonic-toolbox-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pythonic-toolbox-1.1.8.tar", last modified: Tue Jan 25 13:08:26 2022, max compression
+gzip compressed data, was "dist/pythonic-toolbox-1.1.9.tar", last modified: Fri Jan 28 08:24:59 2022, max compression
```

## Comparing `pythonic-toolbox-1.1.8.tar` & `pythonic-toolbox-1.1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 limenglong   (501) staff       (20)        0 2022-01-25 13:08:26.309385 pythonic-toolbox-1.1.8/
--rw-r--r--   0 limenglong   (501) staff       (20)      785 2022-01-25 13:08:26.309539 pythonic-toolbox-1.1.8/PKG-INFO
--rw-r--r--   0 limenglong   (501) staff       (20)      141 2022-01-11 03:06:51.000000 pythonic-toolbox-1.1.8/README.md
-drwxr-xr-x   0 limenglong   (501) staff       (20)        0 2022-01-25 13:08:26.305663 pythonic-toolbox-1.1.8/pythonic_toolbox/
--rw-r--r--   0 limenglong   (501) staff       (20)        0 2021-12-27 12:37:55.000000 pythonic-toolbox-1.1.8/pythonic_toolbox/__init__.py
-drwxr-xr-x   0 limenglong   (501) staff       (20)        0 2022-01-25 13:08:26.307756 pythonic-toolbox-1.1.8/pythonic_toolbox/tests/
--rw-r--r--   0 limenglong   (501) staff       (20)        0 2021-12-28 12:15:27.000000 pythonic-toolbox-1.1.8/pythonic_toolbox/tests/__init__.py
--rw-r--r--   0 limenglong   (501) staff       (20)     6553 2022-01-25 13:04:03.000000 pythonic-toolbox-1.1.8/pythonic_toolbox/tests/test_dict_utils.py
--rw-r--r--   0 limenglong   (501) staff       (20)     3278 2021-12-28 12:18:29.000000 pythonic-toolbox-1.1.8/pythonic_toolbox/tests/test_list_utils.py
-drwxr-xr-x   0 limenglong   (501) staff       (20)        0 2022-01-25 13:08:26.308932 pythonic-toolbox-1.1.8/pythonic_toolbox/utils/
--rw-r--r--   0 limenglong   (501) staff       (20)        0 2021-12-27 12:37:55.000000 pythonic-toolbox-1.1.8/pythonic_toolbox/utils/__init__.py
--rw-r--r--   0 limenglong   (501) staff       (20)     7632 2022-01-25 13:04:03.000000 pythonic-toolbox-1.1.8/pythonic_toolbox/utils/dict_utils.py
--rw-r--r--   0 limenglong   (501) staff       (20)     3360 2022-01-10 12:19:33.000000 pythonic-toolbox-1.1.8/pythonic_toolbox/utils/list_utils.py
-drwxr-xr-x   0 limenglong   (501) staff       (20)        0 2022-01-25 13:08:26.306981 pythonic-toolbox-1.1.8/pythonic_toolbox.egg-info/
--rw-r--r--   0 limenglong   (501) staff       (20)      785 2022-01-25 13:08:26.000000 pythonic-toolbox-1.1.8/pythonic_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 limenglong   (501) staff       (20)      484 2022-01-25 13:08:26.000000 pythonic-toolbox-1.1.8/pythonic_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 limenglong   (501) staff       (20)        1 2022-01-25 13:08:26.000000 pythonic-toolbox-1.1.8/pythonic_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 limenglong   (501) staff       (20)        7 2022-01-25 13:08:26.000000 pythonic-toolbox-1.1.8/pythonic_toolbox.egg-info/requires.txt
--rw-r--r--   0 limenglong   (501) staff       (20)       17 2022-01-25 13:08:26.000000 pythonic-toolbox-1.1.8/pythonic_toolbox.egg-info/top_level.txt
--rw-r--r--   0 limenglong   (501) staff       (20)       67 2022-01-25 13:08:26.310067 pythonic-toolbox-1.1.8/setup.cfg
--rw-r--r--   0 limenglong   (501) staff       (20)     2480 2022-01-25 13:08:05.000000 pythonic-toolbox-1.1.8/setup.py
+drwxr-xr-x   0 limenglong   (501) staff       (20)        0 2022-01-28 08:24:59.000000 pythonic-toolbox-1.1.9/
+-rw-r--r--   0 limenglong   (501) staff       (20)      774 2022-01-28 08:24:59.000000 pythonic-toolbox-1.1.9/PKG-INFO
+drwxr-xr-x   0 limenglong   (501) staff       (20)        0 2022-01-28 08:24:59.000000 pythonic-toolbox-1.1.9/pythonic_toolbox/
+drwxr-xr-x   0 limenglong   (501) staff       (20)        0 2022-01-28 08:24:59.000000 pythonic-toolbox-1.1.9/pythonic_toolbox/tests/
+-rw-r--r--   0 limenglong   (501) staff       (20)        0 2021-12-28 12:15:27.000000 pythonic-toolbox-1.1.9/pythonic_toolbox/tests/__init__.py
+-rw-r--r--   0 limenglong   (501) staff       (20)     3278 2021-12-28 12:18:29.000000 pythonic-toolbox-1.1.9/pythonic_toolbox/tests/test_list_utils.py
+-rw-r--r--   0 limenglong   (501) staff       (20)     7341 2022-01-28 08:09:09.000000 pythonic-toolbox-1.1.9/pythonic_toolbox/tests/test_dict_utils.py
+-rw-r--r--   0 limenglong   (501) staff       (20)        0 2021-12-27 12:37:55.000000 pythonic-toolbox-1.1.9/pythonic_toolbox/__init__.py
+drwxr-xr-x   0 limenglong   (501) staff       (20)        0 2022-01-28 08:24:59.000000 pythonic-toolbox-1.1.9/pythonic_toolbox/utils/
+-rw-r--r--   0 limenglong   (501) staff       (20)     8146 2022-01-28 08:16:04.000000 pythonic-toolbox-1.1.9/pythonic_toolbox/utils/dict_utils.py
+-rw-r--r--   0 limenglong   (501) staff       (20)     3360 2022-01-10 12:19:33.000000 pythonic-toolbox-1.1.9/pythonic_toolbox/utils/list_utils.py
+-rw-r--r--   0 limenglong   (501) staff       (20)        0 2021-12-27 12:37:55.000000 pythonic-toolbox-1.1.9/pythonic_toolbox/utils/__init__.py
+drwxr-xr-x   0 limenglong   (501) staff       (20)        0 2022-01-28 08:24:59.000000 pythonic-toolbox-1.1.9/pythonic_toolbox.egg-info/
+-rw-r--r--   0 limenglong   (501) staff       (20)      774 2022-01-28 08:24:59.000000 pythonic-toolbox-1.1.9/pythonic_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 limenglong   (501) staff       (20)      484 2022-01-28 08:24:59.000000 pythonic-toolbox-1.1.9/pythonic_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 limenglong   (501) staff       (20)        7 2022-01-28 08:24:59.000000 pythonic-toolbox-1.1.9/pythonic_toolbox.egg-info/requires.txt
+-rw-r--r--   0 limenglong   (501) staff       (20)       17 2022-01-28 08:24:59.000000 pythonic-toolbox-1.1.9/pythonic_toolbox.egg-info/top_level.txt
+-rw-r--r--   0 limenglong   (501) staff       (20)        1 2022-01-28 08:24:59.000000 pythonic-toolbox-1.1.9/pythonic_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 limenglong   (501) staff       (20)      141 2022-01-11 03:06:51.000000 pythonic-toolbox-1.1.9/README.md
+-rw-r--r--   0 limenglong   (501) staff       (20)     2480 2022-01-28 08:10:15.000000 pythonic-toolbox-1.1.9/setup.py
+-rw-r--r--   0 limenglong   (501) staff       (20)       67 2022-01-28 08:24:59.000000 pythonic-toolbox-1.1.9/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `pythonic-toolbox-1.1.8/PKG-INFO` & `pythonic-toolbox-1.1.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pythonic-toolbox
-Version: 1.1.8
+Version: 1.1.9
 Summary: a toolbox with pythonic utils, tools
 Home-page: https://github.com/albertmenglongli/pythonic-toolbox
 Author: menglong.li
 Author-email: albert.menglongli@gmail.com
 License: Apache2.0
-Description: A toolbox containing multi useful pythonic utils, functions, decorators etc.
 Keywords: toolbox
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+
+A toolbox containing multi useful pythonic utils, functions, decorators etc.
+
```

### Comparing `pythonic-toolbox-1.1.8/pythonic_toolbox/tests/test_dict_utils.py` & `pythonic-toolbox-1.1.9/pythonic_toolbox/tests/test_dict_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -107,36 +107,56 @@
     expected = [{'name': 'lml', 'age': 66}, {'name': 'albert', 'age': 36}]
     assert walk_leaves(data, trans_fun=lambda x: x * 2 if isinstance(x, int) else x) == expected
     assert walk_leaves(data, trans_fun=lambda x: x * 2 if isinstance(x, int) else x, inplace=True) is None
     assert data == expected
 
 
 def test_dict_obj():
+    import pytest
     from pythonic_toolbox.utils.dict_utils import DictObj
 
+    naive_dct = {
+        'key1': 'val1',
+        'key2': 'val2',
+    }
+
+    obj = DictObj(naive_dct)
+    # same behavior like ordinary dict according to the python version (FILO for popitem for 3.6+)
+    assert obj.popitem() == ('key2', 'val2')
+    assert obj.popitem() == ('key1', 'val1')
+    with pytest.raises(KeyError) as __:
+        obj.popitem()
+    obj.key3 = 'val3'
+    assert obj.pop('key3', None) == 'val3'
+    assert obj.pop('key4', None) is None
+
     person_dct = {'name': 'Albert', 'age': '34', 'sex': 'Male', 'languages': ['Chinese', 'English']}
 
     person = DictObj(person_dct)
     assert person.to_dict() == person_dct
     assert set(person.keys()) == {'name', 'age', 'sex', 'languages'}
+    assert hasattr(person, 'name') is True
     assert person.name == 'Albert'
     assert person['name'] == 'Albert'
     person.languages.append('Japanese')
     assert person.languages == ['Chinese', 'English', 'Japanese']
 
     person.height = '170'
     assert person['height'] == '170'
     assert 'height' in person
     assert 'height' in person.keys()
+    assert hasattr(person, 'height') is True
     del person['height']
     assert 'height' not in person
     assert 'height' not in person.keys()
     person['height'] = '170cm'
 
     person.update({'weight': '50'})
+    weight_val = person.pop('weight')
+    assert weight_val == '50'
     person.update(DictObj({'weight': '50kg'}))
     assert person.weight == '50kg'
 
     expected = {
         'name': 'Albert', 'age': '34', 'sex': 'Male',
         'languages': ['Chinese', 'English', 'Japanese'],  # appended new language
         'height': '170cm',  # new added attribute
@@ -160,14 +180,20 @@
     assert fixed_person.name == 'Albert'
 
     with pytest.raises(RuntimeError) as exec_info:
         fixed_person.name = 'Steve'
     expected_error_str = 'Not allowed to assign attribute name with value Steve for an initialized FinalDictObj'
     assert exec_info.value.args[0] == expected_error_str
 
+    with pytest.raises(RuntimeError) as __:
+        fixed_person.popitem()
+
+    with pytest.raises(RuntimeError) as __:
+        fixed_person.pop('name')
+
     assert type(fixed_person.languages) == tuple
     with pytest.raises(AttributeError) as exec_info:
         # list values are changed into tuple to avoid being modified
         fixed_person.languages.append('Japanese')
     expected_error_str = "'tuple' object has no attribute 'append'"
     assert exec_info.value.args[0] == expected_error_str
     assert fixed_person.to_dict() == person_dct
```

### Comparing `pythonic-toolbox-1.1.8/pythonic_toolbox/tests/test_list_utils.py` & `pythonic-toolbox-1.1.9/pythonic_toolbox/tests/test_list_utils.py`

 * *Files identical despite different names*

### Comparing `pythonic-toolbox-1.1.8/pythonic_toolbox/utils/dict_utils.py` & `pythonic-toolbox-1.1.9/pythonic_toolbox/utils/dict_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -115,14 +115,20 @@
             lst_factory = object.__getattribute__(self, f'_{self.__class__.__name__}__lst_factory')
             self.data[key] = lst_factory(self.__class__(x) if isinstance(x, dict) else x for x in item)
         elif isinstance(item, dict):
             self.data[key] = self.__class__(item)
         else:
             self.data[key] = item
 
+    def popitem(self):
+        """
+        Override popitem from MutableMapping, make behavior popitem FILO like ordinary dict since 3.6
+        """
+        return self.data.popitem()
+
     def __getattribute__(self, item):
         if item == 'data':
             return self.__dict__['data']
         else:
             return super(DictObj, self).__getattribute__(item)
 
     def __delitem__(self, key):
@@ -191,14 +197,22 @@
         super(FinalDictObj, self).__setitem__(key, value)
 
     def __delitem__(self, key):
         if self.__is_frozen is True:
             raise RuntimeError(f'Cannot del attribute or item {key} in an initialized FinalDictObj')
         super(FinalDictObj, self).__delitem__(key)
 
+    def popitem(self):
+        """
+        Override popitem from MutableMapping, make behavior popitem FILO like ordinary dict since 3.6
+        """
+        if self.__is_frozen is True:
+            raise RuntimeError(f'Cannot popitem attribute/item in initialed FinalDictObj')
+        return super(FinalDictObj, self).popitem()
+
     def __setattr__(self, key, value):
         """DictObj that cannot change attribute"""
         if key == '_FinalDictObj__is_frozen' and value is True:
             # __is_frozen can only be assigned once
             object.__setattr__(self, key, value)
         else:
             if self.__is_frozen:
```

### Comparing `pythonic-toolbox-1.1.8/pythonic_toolbox/utils/list_utils.py` & `pythonic-toolbox-1.1.9/pythonic_toolbox/utils/list_utils.py`

 * *Files identical despite different names*

### Comparing `pythonic-toolbox-1.1.8/pythonic_toolbox.egg-info/PKG-INFO` & `pythonic-toolbox-1.1.9/pythonic_toolbox.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pythonic-toolbox
-Version: 1.1.8
+Version: 1.1.9
 Summary: a toolbox with pythonic utils, tools
 Home-page: https://github.com/albertmenglongli/pythonic-toolbox
 Author: menglong.li
 Author-email: albert.menglongli@gmail.com
 License: Apache2.0
-Description: A toolbox containing multi useful pythonic utils, functions, decorators etc.
 Keywords: toolbox
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+
+A toolbox containing multi useful pythonic utils, functions, decorators etc.
+
```

### Comparing `pythonic-toolbox-1.1.8/setup.py` & `pythonic-toolbox-1.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 setup(
     name='pythonic-toolbox',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='1.1.8',
+    version='1.1.9',
 
     description='a toolbox with pythonic utils, tools',
     long_description=long_description,
 
     # The project's main homepage.
     url='https://github.com/albertmenglongli/pythonic-toolbox',
```

