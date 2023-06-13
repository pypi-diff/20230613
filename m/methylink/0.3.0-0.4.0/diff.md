# Comparing `tmp/methylink-0.3.0.tar.gz` & `tmp/methylink-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "methylink-0.3.0.tar", last modified: Mon May 22 23:57:37 2023, max compression
+gzip compressed data, was "methylink-0.4.0.tar", last modified: Tue Jun 13 17:48:25 2023, max compression
```

## Comparing `methylink-0.3.0.tar` & `methylink-0.4.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 uwmei      (503) staff       (20)        0 2023-05-22 23:57:37.312929 methylink-0.3.0/
--rw-r--r--   0 uwmei      (503) staff       (20)     1063 2023-05-17 16:49:14.000000 methylink-0.3.0/LICENSE
--rw-r--r--   0 uwmei      (503) staff       (20)      130 2023-05-22 14:54:33.000000 methylink-0.3.0/MANIFEST.in
--rw-r--r--   0 uwmei      (503) staff       (20)     2523 2023-05-22 23:57:37.312739 methylink-0.3.0/PKG-INFO
--rw-r--r--   0 uwmei      (503) staff       (20)     2037 2023-05-22 23:50:52.000000 methylink-0.3.0/README.md
-drwxr-xr-x   0 uwmei      (503) staff       (20)        0 2023-05-22 23:57:37.266250 methylink-0.3.0/methylink/
--rw-r--r--   0 uwmei      (503) staff       (20)       22 2023-05-22 23:52:47.000000 methylink-0.3.0/methylink/__init__.py
--rw-r--r--   0 uwmei      (503) staff       (20)     5879 2023-05-22 01:48:24.000000 methylink-0.3.0/methylink/append_mod_tags.py
-drwxr-xr-x   0 uwmei      (503) staff       (20)        0 2023-05-22 23:57:37.307006 methylink-0.3.0/methylink/cli/
--rw-r--r--   0 uwmei      (503) staff       (20)        0 2023-05-21 02:47:41.000000 methylink-0.3.0/methylink/cli/__init__.py
--rw-r--r--   0 uwmei      (503) staff       (20)     2667 2023-05-22 23:32:26.000000 methylink-0.3.0/methylink/cli/core.py
-drwxr-xr-x   0 uwmei      (503) staff       (20)        0 2023-05-22 23:57:37.312321 methylink-0.3.0/methylink/database/
--rw-r--r--   0 uwmei      (503) staff       (20)        0 2023-05-21 02:47:41.000000 methylink-0.3.0/methylink/database/__init__.py
--rw-r--r--   0 uwmei      (503) staff       (20)     1193 2023-05-21 02:47:41.000000 methylink-0.3.0/methylink/database/crud.py
--rw-r--r--   0 uwmei      (503) staff       (20)      159 2023-05-21 02:47:41.000000 methylink-0.3.0/methylink/main.py
-drwxr-xr-x   0 uwmei      (503) staff       (20)        0 2023-05-22 23:57:37.287411 methylink-0.3.0/methylink.egg-info/
--rw-r--r--   0 uwmei      (503) staff       (20)     2523 2023-05-22 23:57:37.000000 methylink-0.3.0/methylink.egg-info/PKG-INFO
--rw-r--r--   0 uwmei      (503) staff       (20)      428 2023-05-22 23:57:37.000000 methylink-0.3.0/methylink.egg-info/SOURCES.txt
--rw-r--r--   0 uwmei      (503) staff       (20)        1 2023-05-22 23:57:37.000000 methylink-0.3.0/methylink.egg-info/dependency_links.txt
--rw-r--r--   0 uwmei      (503) staff       (20)       50 2023-05-22 23:57:37.000000 methylink-0.3.0/methylink.egg-info/entry_points.txt
--rw-r--r--   0 uwmei      (503) staff       (20)       34 2023-05-22 23:57:37.000000 methylink-0.3.0/methylink.egg-info/requires.txt
--rw-r--r--   0 uwmei      (503) staff       (20)       10 2023-05-22 23:57:37.000000 methylink-0.3.0/methylink.egg-info/top_level.txt
--rw-r--r--   0 uwmei      (503) staff       (20)       80 2023-05-22 01:46:41.000000 methylink-0.3.0/pyproject.toml
--rw-r--r--   0 uwmei      (503) staff       (20)       38 2023-05-22 23:57:37.312981 methylink-0.3.0/setup.cfg
--rw-r--r--   0 uwmei      (503) staff       (20)     1197 2023-05-22 23:52:47.000000 methylink-0.3.0/setup.py
+drwxr-xr-x   0 uwmei      (503) staff       (20)        0 2023-06-13 17:48:25.950362 methylink-0.4.0/
+-rw-r--r--   0 uwmei      (503) staff       (20)     1063 2023-05-17 16:49:14.000000 methylink-0.4.0/LICENSE
+-rw-r--r--   0 uwmei      (503) staff       (20)      130 2023-06-13 17:35:54.000000 methylink-0.4.0/MANIFEST.in
+-rw-r--r--   0 uwmei      (503) staff       (20)     2523 2023-06-13 17:48:25.950098 methylink-0.4.0/PKG-INFO
+-rw-r--r--   0 uwmei      (503) staff       (20)     2037 2023-06-13 17:35:54.000000 methylink-0.4.0/README.md
+drwxr-xr-x   0 uwmei      (503) staff       (20)        0 2023-06-13 17:48:25.908465 methylink-0.4.0/methylink/
+-rw-r--r--   0 uwmei      (503) staff       (20)       22 2023-06-13 17:46:05.000000 methylink-0.4.0/methylink/__init__.py
+-rw-r--r--   0 uwmei      (503) staff       (20)     5926 2023-06-13 17:43:25.000000 methylink-0.4.0/methylink/append_mod_tags.py
+drwxr-xr-x   0 uwmei      (503) staff       (20)        0 2023-06-13 17:48:25.928305 methylink-0.4.0/methylink/cli/
+-rw-r--r--   0 uwmei      (503) staff       (20)        0 2023-05-21 02:47:41.000000 methylink-0.4.0/methylink/cli/__init__.py
+-rw-r--r--   0 uwmei      (503) staff       (20)     2690 2023-06-13 17:43:25.000000 methylink-0.4.0/methylink/cli/core.py
+drwxr-xr-x   0 uwmei      (503) staff       (20)        0 2023-06-13 17:48:25.949697 methylink-0.4.0/methylink/database/
+-rw-r--r--   0 uwmei      (503) staff       (20)        0 2023-05-21 02:47:41.000000 methylink-0.4.0/methylink/database/__init__.py
+-rw-r--r--   0 uwmei      (503) staff       (20)     1193 2023-05-21 02:47:41.000000 methylink-0.4.0/methylink/database/crud.py
+-rw-r--r--   0 uwmei      (503) staff       (20)      159 2023-05-21 02:47:41.000000 methylink-0.4.0/methylink/main.py
+drwxr-xr-x   0 uwmei      (503) staff       (20)        0 2023-06-13 17:48:25.927327 methylink-0.4.0/methylink.egg-info/
+-rw-r--r--   0 uwmei      (503) staff       (20)     2523 2023-06-13 17:48:25.000000 methylink-0.4.0/methylink.egg-info/PKG-INFO
+-rw-r--r--   0 uwmei      (503) staff       (20)      428 2023-06-13 17:48:25.000000 methylink-0.4.0/methylink.egg-info/SOURCES.txt
+-rw-r--r--   0 uwmei      (503) staff       (20)        1 2023-06-13 17:48:25.000000 methylink-0.4.0/methylink.egg-info/dependency_links.txt
+-rw-r--r--   0 uwmei      (503) staff       (20)       50 2023-06-13 17:48:25.000000 methylink-0.4.0/methylink.egg-info/entry_points.txt
+-rw-r--r--   0 uwmei      (503) staff       (20)       34 2023-06-13 17:48:25.000000 methylink-0.4.0/methylink.egg-info/requires.txt
+-rw-r--r--   0 uwmei      (503) staff       (20)       10 2023-06-13 17:48:25.000000 methylink-0.4.0/methylink.egg-info/top_level.txt
+-rw-r--r--   0 uwmei      (503) staff       (20)       80 2023-06-13 17:35:54.000000 methylink-0.4.0/pyproject.toml
+-rw-r--r--   0 uwmei      (503) staff       (20)       38 2023-06-13 17:48:25.950414 methylink-0.4.0/setup.cfg
+-rw-r--r--   0 uwmei      (503) staff       (20)     1197 2023-06-13 17:46:05.000000 methylink-0.4.0/setup.py
```

### Comparing `methylink-0.3.0/LICENSE` & `methylink-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `methylink-0.3.0/PKG-INFO` & `methylink-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: methylink
-Version: 0.3.0
+Version: 0.4.0
 Summary: methylink is a tool to link methylation tags between SAM/BAM files.
 Home-page: https://github.com/projectoriented/methylink
 Author: Mei Wu
 License: MIT
 Keywords: methylation nanopore bioinformatics
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `methylink-0.3.0/README.md` & `methylink-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `methylink-0.3.0/methylink/append_mod_tags.py` & `methylink-0.4.0/methylink/append_mod_tags.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,16 +142,17 @@
                 bam_file_list.append(f"{self.prefix}_tmp.{subset_idx}.bam")
 
             # Write the current read to the current subset file
             current_subset.write(read)
             subset_size_bytes = os.path.getsize(current_subset.filename.decode())
 
         # Close the last subset file
-        current_subset.close()
-        pysam.index(current_subset.filename.decode())
+        if current_subset is not None:
+            current_subset.close()
+            pysam.index(current_subset.filename.decode())
 
         self.aln_obj.close()
 
         return bam_file_list
 
     def combine_the_chunked(self, linked_bam_output_fp):
         # Read in the chunked bams
```

### Comparing `methylink-0.3.0/methylink/cli/core.py` & `methylink-0.4.0/methylink/cli/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     multiple=True,
     help="Unmapped bam files with methylation tags.",
 )
 @click.option("--aln", required=True, help="Aligned bam to map the meth tags to.")
 @click.option(
     "--sample",
     required=True,
-    help="Sample name.",
+    help="Sample name to use in the prefixing",
 )
 @click.option(
     "--output",
     required=True,
     help="Output file.",
 )
 def base(sample, threads, methyl_bams, aln, output, log_level, tmp=None):
```

### Comparing `methylink-0.3.0/methylink/database/crud.py` & `methylink-0.4.0/methylink/database/crud.py`

 * *Files identical despite different names*

### Comparing `methylink-0.3.0/methylink.egg-info/PKG-INFO` & `methylink-0.4.0/methylink.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: methylink
-Version: 0.3.0
+Version: 0.4.0
 Summary: methylink is a tool to link methylation tags between SAM/BAM files.
 Home-page: https://github.com/projectoriented/methylink
 Author: Mei Wu
 License: MIT
 Keywords: methylation nanopore bioinformatics
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `methylink-0.3.0/setup.py` & `methylink-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     with io.open(os.path.join(HERE, "README.md"), encoding="utf-8") as f:
         LONG_DESCRIPTION = "\n" + f.read()
 except FileNotFoundError:
     LONG_DESCRIPTION = DESCRIPTION
 
 setup(
     name=NAME,
-    version="0.3.0",
+    version="0.4.0",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     keywords="methylation nanopore bioinformatics",
     license="MIT",
     author=AUTHOR,
     packages=find_packages(),
```

