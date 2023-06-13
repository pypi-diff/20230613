# Comparing `tmp/lesscode_tag-0.0.3.tar.gz` & `tmp/lesscode_tag-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lesscode_tag-0.0.3.tar", last modified: Mon Jun  5 03:35:05 2023, max compression
+gzip compressed data, was "dist/lesscode_tag-0.0.4.tar", last modified: Tue Jun 13 03:18:59 2023, max compression
```

## Comparing `lesscode_tag-0.0.3.tar` & `lesscode_tag-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-06-05 03:35:05.000000 lesscode_tag-0.0.3/
--rw-r--r--   0 baai       (501) staff       (20)      379 2023-06-05 03:35:05.000000 lesscode_tag-0.0.3/PKG-INFO
--rw-r--r--   0 baai       (501) staff       (20)       52 2023-05-25 01:34:02.000000 lesscode_tag-0.0.3/README.md
-drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-06-05 03:35:05.000000 lesscode_tag-0.0.3/lesscode_tag/
--rw-r--r--   0 baai       (501) staff       (20)        0 2023-05-25 01:04:19.000000 lesscode_tag-0.0.3/lesscode_tag/__init__.py
--rw-r--r--   0 baai       (501) staff       (20)     1807 2023-05-25 02:53:36.000000 lesscode_tag-0.0.3/lesscode_tag/aes.py
--rw-r--r--   0 baai       (501) staff       (20)     8049 2023-06-05 03:35:02.000000 lesscode_tag-0.0.3/lesscode_tag/business.py
--rw-r--r--   0 baai       (501) staff       (20)     9603 2023-05-25 02:53:36.000000 lesscode_tag-0.0.3/lesscode_tag/es_util.py
--rw-r--r--   0 baai       (501) staff       (20)       22 2023-06-05 03:35:02.000000 lesscode_tag-0.0.3/lesscode_tag/version.py
-drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-06-05 03:35:05.000000 lesscode_tag-0.0.3/lesscode_tag.egg-info/
--rw-r--r--   0 baai       (501) staff       (20)      379 2023-06-05 03:35:05.000000 lesscode_tag-0.0.3/lesscode_tag.egg-info/PKG-INFO
--rw-r--r--   0 baai       (501) staff       (20)      280 2023-06-05 03:35:05.000000 lesscode_tag-0.0.3/lesscode_tag.egg-info/SOURCES.txt
--rw-r--r--   0 baai       (501) staff       (20)        1 2023-06-05 03:35:05.000000 lesscode_tag-0.0.3/lesscode_tag.egg-info/dependency_links.txt
--rw-r--r--   0 baai       (501) staff       (20)       13 2023-06-05 03:35:05.000000 lesscode_tag-0.0.3/lesscode_tag.egg-info/top_level.txt
--rw-r--r--   0 baai       (501) staff       (20)       38 2023-06-05 03:35:05.000000 lesscode_tag-0.0.3/setup.cfg
--rw-r--r--   0 baai       (501) staff       (20)     1273 2023-05-25 07:46:43.000000 lesscode_tag-0.0.3/setup.py
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-06-13 03:18:59.000000 lesscode_tag-0.0.4/
+-rw-r--r--   0 baai       (501) staff       (20)      379 2023-06-13 03:18:59.000000 lesscode_tag-0.0.4/PKG-INFO
+-rw-r--r--   0 baai       (501) staff       (20)       52 2023-05-25 01:34:02.000000 lesscode_tag-0.0.4/README.md
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-06-13 03:18:59.000000 lesscode_tag-0.0.4/lesscode_tag/
+-rw-r--r--   0 baai       (501) staff       (20)        0 2023-05-25 01:04:19.000000 lesscode_tag-0.0.4/lesscode_tag/__init__.py
+-rw-r--r--   0 baai       (501) staff       (20)     1807 2023-05-25 02:53:36.000000 lesscode_tag-0.0.4/lesscode_tag/aes.py
+-rw-r--r--   0 baai       (501) staff       (20)     8078 2023-06-13 03:18:47.000000 lesscode_tag-0.0.4/lesscode_tag/business.py
+-rw-r--r--   0 baai       (501) staff       (20)     9603 2023-05-25 02:53:36.000000 lesscode_tag-0.0.4/lesscode_tag/es_util.py
+-rw-r--r--   0 baai       (501) staff       (20)       22 2023-06-13 03:18:47.000000 lesscode_tag-0.0.4/lesscode_tag/version.py
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-06-13 03:18:59.000000 lesscode_tag-0.0.4/lesscode_tag.egg-info/
+-rw-r--r--   0 baai       (501) staff       (20)      379 2023-06-13 03:18:59.000000 lesscode_tag-0.0.4/lesscode_tag.egg-info/PKG-INFO
+-rw-r--r--   0 baai       (501) staff       (20)      280 2023-06-13 03:18:59.000000 lesscode_tag-0.0.4/lesscode_tag.egg-info/SOURCES.txt
+-rw-r--r--   0 baai       (501) staff       (20)        1 2023-06-13 03:18:59.000000 lesscode_tag-0.0.4/lesscode_tag.egg-info/dependency_links.txt
+-rw-r--r--   0 baai       (501) staff       (20)       13 2023-06-13 03:18:59.000000 lesscode_tag-0.0.4/lesscode_tag.egg-info/top_level.txt
+-rw-r--r--   0 baai       (501) staff       (20)       38 2023-06-13 03:18:59.000000 lesscode_tag-0.0.4/setup.cfg
+-rw-r--r--   0 baai       (501) staff       (20)     1273 2023-05-25 07:46:43.000000 lesscode_tag-0.0.4/setup.py
```

### Comparing `lesscode_tag-0.0.3/lesscode_tag/aes.py` & `lesscode_tag-0.0.4/lesscode_tag/aes.py`

 * *Files identical despite different names*

### Comparing `lesscode_tag-0.0.3/lesscode_tag/business.py` & `lesscode_tag-0.0.4/lesscode_tag/business.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,14 +112,14 @@
 
 
 def format_special_tag_list(special_tag_list=None):
     bool_should_list = []
     if special_tag_list:
         for special_tag in special_tag_list:
             if isinstance(special_tag, list):
-                bool_should = []
+                bool_must_list = []
                 for _tag in special_tag:
-                    bool_should.append(get_single_tag_condition(_tag))
-                bool_should_list.append(bool_should)
+                    bool_must_list.append(get_single_tag_condition(_tag))
+                bool_should_list.append({"bool": {"must": bool_must_list}})
             else:
                 bool_should_list.append(get_single_tag_condition(special_tag))
     return {"bool": {"should": bool_should_list}}
```

### Comparing `lesscode_tag-0.0.3/lesscode_tag/es_util.py` & `lesscode_tag-0.0.4/lesscode_tag/es_util.py`

 * *Files identical despite different names*

### Comparing `lesscode_tag-0.0.3/setup.py` & `lesscode_tag-0.0.4/setup.py`

 * *Files identical despite different names*

