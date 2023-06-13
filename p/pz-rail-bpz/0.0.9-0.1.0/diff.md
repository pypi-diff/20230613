# Comparing `tmp/pz-rail-bpz-0.0.9.tar.gz` & `tmp/pz-rail-bpz-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz-rail-bpz-0.0.9.tar", last modified: Thu May  4 05:26:18 2023, max compression
+gzip compressed data, was "pz-rail-bpz-0.1.0.tar", last modified: Tue Jun 13 20:03:20 2023, max compression
```

## Comparing `pz-rail-bpz-0.0.9.tar` & `pz-rail-bpz-0.1.0.tar`

### file list

```diff
@@ -1,35 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 05:26:18.000789 pz-rail-bpz-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (122)      123 2023-05-04 05:26:01.000000 pz-rail-bpz-0.0.9/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 05:26:18.000789 pz-rail-bpz-0.0.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 05:26:18.000789 pz-rail-bpz-0.0.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     2066 2023-05-04 05:26:01.000000 pz-rail-bpz-0.0.9/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (122)      548 2023-05-04 05:26:01.000000 pz-rail-bpz-0.0.9/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1828 2023-05-04 05:26:01.000000 pz-rail-bpz-0.0.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1102 2023-05-04 05:26:01.000000 pz-rail-bpz-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     1936 2023-05-04 05:26:18.000789 pz-rail-bpz-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1604 2023-05-04 05:26:01.000000 pz-rail-bpz-0.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     3070 2023-05-04 05:26:01.000000 pz-rail-bpz-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-04 05:26:18.000789 pz-rail-bpz-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)       71 2023-05-04 05:26:01.000000 pz-rail-bpz-0.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 05:26:18.000789 pz-rail-bpz-0.0.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 05:26:18.000789 pz-rail-bpz-0.0.9/src/pz_rail_bpz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1936 2023-05-04 05:26:17.000000 pz-rail-bpz-0.0.9/src/pz_rail_bpz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      529 2023-05-04 05:26:17.000000 pz-rail-bpz-0.0.9/src/pz_rail_bpz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-04 05:26:17.000000 pz-rail-bpz-0.0.9/src/pz_rail_bpz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       90 2023-05-04 05:26:17.000000 pz-rail-bpz-0.0.9/src/pz_rail_bpz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-04 05:26:17.000000 pz-rail-bpz-0.0.9/src/pz_rail_bpz.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 05:26:18.000789 pz-rail-bpz-0.0.9/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 05:26:18.000789 pz-rail-bpz-0.0.9/src/rail/bpz/
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-05-04 05:26:01.000000 pz-rail-bpz-0.0.9/src/rail/bpz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-05-04 05:26:17.000000 pz-rail-bpz-0.0.9/src/rail/bpz/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)      147 2023-05-04 05:26:01.000000 pz-rail-bpz-0.0.9/src/rail/bpz/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 05:26:18.000789 pz-rail-bpz-0.0.9/src/rail/estimation/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 05:26:18.000789 pz-rail-bpz-0.0.9/src/rail/estimation/algos/
--rw-r--r--   0 runner    (1001) docker     (122)    26631 2023-05-04 05:26:01.000000 pz-rail-bpz-0.0.9/src/rail/estimation/algos/bpz_lite.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 05:26:18.000789 pz-rail-bpz-0.0.9/src/rail/examples_data/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 05:26:18.000789 pz-rail-bpz-0.0.9/src/rail/examples_data/estimation_data/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 05:26:18.000789 pz-rail-bpz-0.0.9/src/rail/examples_data/estimation_data/configs/
--rw-r--r--   0 runner    (1001) docker     (122)      701 2023-05-04 05:26:01.000000 pz-rail-bpz-0.0.9/src/rail/examples_data/estimation_data/configs/test_bpz.columns
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 05:26:18.000789 pz-rail-bpz-0.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     6104 2023-05-04 05:26:01.000000 pz-rail-bpz-0.0.9/tests/test_algos.py
--rw-r--r--   0 runner    (1001) docker     (122)    10624 2023-05-04 05:26:01.000000 pz-rail-bpz-0.0.9/tests/validation_10gal.pq
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:03:20.530973 pz-rail-bpz-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      123 2023-06-13 20:03:02.000000 pz-rail-bpz-0.1.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:03:20.518972 pz-rail-bpz-0.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:03:20.522972 pz-rail-bpz-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     2066 2023-06-13 20:03:02.000000 pz-rail-bpz-0.1.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      548 2023-06-13 20:03:02.000000 pz-rail-bpz-0.1.0/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1828 2023-06-13 20:03:02.000000 pz-rail-bpz-0.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1102 2023-06-13 20:03:02.000000 pz-rail-bpz-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1936 2023-06-13 20:03:20.530973 pz-rail-bpz-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1604 2023-06-13 20:03:02.000000 pz-rail-bpz-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:03:20.526972 pz-rail-bpz-0.1.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (122)    33291 2023-06-13 20:03:02.000000 pz-rail-bpz-0.1.0/examples/BPZ_lite_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)    22127 2023-06-13 20:03:02.000000 pz-rail-bpz-0.1.0/examples/BPZ_lite_with_custom_SEDs.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)   460800 2023-06-13 20:03:02.000000 pz-rail-bpz-0.1.0/examples/nonphysical_dc2_templates.tar
+-rw-r--r--   0 runner    (1001) docker     (122)    83848 2023-06-13 20:03:02.000000 pz-rail-bpz-0.1.0/examples/test_dc2_train_customtemp_broadttypes.hdf5
+-rw-r--r--   0 runner    (1001) docker     (122)    83848 2023-06-13 20:03:02.000000 pz-rail-bpz-0.1.0/examples/test_dc2_training_9816_broadtypes.hdf5
+-rw-r--r--   0 runner    (1001) docker     (122)     3129 2023-06-13 20:03:02.000000 pz-rail-bpz-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-13 20:03:20.530973 pz-rail-bpz-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)       71 2023-06-13 20:03:02.000000 pz-rail-bpz-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:03:20.518972 pz-rail-bpz-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:03:20.526972 pz-rail-bpz-0.1.0/src/pz_rail_bpz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1936 2023-06-13 20:03:20.000000 pz-rail-bpz-0.1.0/src/pz_rail_bpz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      738 2023-06-13 20:03:20.000000 pz-rail-bpz-0.1.0/src/pz_rail_bpz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-13 20:03:20.000000 pz-rail-bpz-0.1.0/src/pz_rail_bpz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       97 2023-06-13 20:03:20.000000 pz-rail-bpz-0.1.0/src/pz_rail_bpz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-13 20:03:20.000000 pz-rail-bpz-0.1.0/src/pz_rail_bpz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:03:20.518972 pz-rail-bpz-0.1.0/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:03:20.526972 pz-rail-bpz-0.1.0/src/rail/bpz/
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-06-13 20:03:02.000000 pz-rail-bpz-0.1.0/src/rail/bpz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-06-13 20:03:19.000000 pz-rail-bpz-0.1.0/src/rail/bpz/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)      147 2023-06-13 20:03:02.000000 pz-rail-bpz-0.1.0/src/rail/bpz/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:03:20.518972 pz-rail-bpz-0.1.0/src/rail/estimation/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:03:20.530973 pz-rail-bpz-0.1.0/src/rail/estimation/algos/
+-rw-r--r--   0 runner    (1001) docker     (122)    26630 2023-06-13 20:03:02.000000 pz-rail-bpz-0.1.0/src/rail/estimation/algos/bpz_lite.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:03:20.522972 pz-rail-bpz-0.1.0/src/rail/examples_data/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:03:20.522972 pz-rail-bpz-0.1.0/src/rail/examples_data/estimation_data/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:03:20.530973 pz-rail-bpz-0.1.0/src/rail/examples_data/estimation_data/configs/
+-rw-r--r--   0 runner    (1001) docker     (122)      701 2023-06-13 20:03:02.000000 pz-rail-bpz-0.1.0/src/rail/examples_data/estimation_data/configs/test_bpz.columns
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:03:20.530973 pz-rail-bpz-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     6092 2023-06-13 20:03:02.000000 pz-rail-bpz-0.1.0/tests/test_algos.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10624 2023-06-13 20:03:02.000000 pz-rail-bpz-0.1.0/tests/validation_10gal.pq
```

### Comparing `pz-rail-bpz-0.0.9/.github/workflows/main.yml` & `pz-rail-bpz-0.1.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-bpz-0.0.9/.github/workflows/pypi.yaml` & `pz-rail-bpz-0.1.0/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `pz-rail-bpz-0.0.9/.gitignore` & `pz-rail-bpz-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pz-rail-bpz-0.0.9/LICENSE` & `pz-rail-bpz-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pz-rail-bpz-0.0.9/PKG-INFO` & `pz-rail-bpz-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-bpz
-Version: 0.0.9
+Version: 0.1.0
 Summary: RAIL BPZ Interface
 Author-email: The LSST DESC PZ WG <samuel.j.schmidt@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pz-rail-bpz-0.0.9/README.md` & `pz-rail-bpz-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pz-rail-bpz-0.0.9/pyproject.toml` & `pz-rail-bpz-0.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -17,25 +17,25 @@
     "Programming Language :: Python :: 3.10",
     "Natural Language :: English",
     "Operating System :: POSIX"
 ]
 dynamic = ["version"]
 dependencies = [
     "desc-bpz",
-    "pandas",
-    "pz-rail",
-    "tables-io[full]",
+    "pz-rail-base",
+    "qp-prob[full]",
 ]
 
 [project.optional-dependencies]
 dev = [
     "coverage",
     "pylint",
     "pytest",
     "pytest-cov",
+    "pre-commit", # Used to run checks before finalizing a git commit
     "yamllint",
 ]
 
 [build-system]
 requires = ["setuptools>=61", "wheel", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
```

### Comparing `pz-rail-bpz-0.0.9/src/pz_rail_bpz.egg-info/PKG-INFO` & `pz-rail-bpz-0.1.0/src/pz_rail_bpz.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-bpz
-Version: 0.0.9
+Version: 0.1.0
 Summary: RAIL BPZ Interface
 Author-email: The LSST DESC PZ WG <samuel.j.schmidt@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pz-rail-bpz-0.0.9/src/rail/estimation/algos/bpz_lite.py` & `pz-rail-bpz-0.1.0/src/rail/estimation/algos/bpz_lite.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
                           data_path=Param(str, "None",
                                           msg="data_path (str): file path to the "
                                           "SED, FILTER, and AB directories.  If left to "
                                           "default `None` it will use the install "
                                           "directory for rail + rail/examples_data/estimation_data/data"),
                           columns_file=Param(str, os.path.join(RAIL_BPZ_DIR, "rail/examples_data/estimation_data/configs/test_bpz.columns"),
                                              msg="name of the file specifying the columns"),
-                          spectra_file=Param(str, "SED/CWWSB4.list",
+                          spectra_file=Param(str, "CWWSB4.list",
                                              msg="name of the file specifying the list of SEDs to use"),
                           m0=Param(float, 20.0, msg="reference apparent mag, used in prior param"),
                           nt_array=Param(list, [1, 2, 3], msg="list of integer number of templates per 'broad type', "
                                          "must be in same order as the template set, and must sum to the same number "
                                          "as the # of templates in the spectra file"),
                           mmin=Param(float, 18.0, msg="lowest apparent mag in ref band, lower values ignored"),
                           mmax=Param(float, 29.0, msg="highest apparent mag in ref band, higher values ignored"),
@@ -259,15 +259,15 @@
                           data_path=Param(str, "None",
                                           msg="data_path (str): file path to the "
                                           "SED, FILTER, and AB directories.  If left to "
                                           "default `None` it will use the install "
                                           "directory for rail + ../examples_data/estimation_data/data"),
                           columns_file=Param(str, os.path.join(RAIL_BPZ_DIR, "rail/examples_data/estimation_data/configs/test_bpz.columns"),
                                              msg="name of the file specifying the columns"),
-                          spectra_file=Param(str, "SED/CWWSB4.list",
+                          spectra_file=Param(str, "CWWSB4.list",
                                              msg="name of the file specifying the list of SEDs to use"),
                           madau_flag=Param(str, "no",
                                            msg="set to 'yes' or 'no' to set whether to include intergalactic "
                                                "Madau reddening when constructing model fluxes"),
                           no_prior=Param(bool, "False", msg="set to True if you want to run with no prior"),
                           p_min=Param(float, 0.005,
                                       msg="BPZ sets all values of "
@@ -341,15 +341,15 @@
         z = self.zgrid
 
         data_path = self.data_path
         columns_file = self.config.columns_file
         ignore_rows = ["M_0", "OTHER", "ID", "Z_S"]
         filters = [f for f in get_str(columns_file, 0) if f not in ignore_rows]
 
-        spectra_file = os.path.join(data_path, self.config.spectra_file)
+        spectra_file = os.path.join(data_path, "SED", self.config.spectra_file)
         spectra = [s[:-4] for s in get_str(spectra_file)]
 
         nt = len(spectra)
         nf = len(filters)
         nz = len(z)
         flux_templates = np.zeros((nz, nt, nf))
```

### Comparing `pz-rail-bpz-0.0.9/src/rail/examples_data/estimation_data/configs/test_bpz.columns` & `pz-rail-bpz-0.1.0/src/rail/examples_data/estimation_data/configs/test_bpz.columns`

 * *Files identical despite different names*

### Comparing `pz-rail-bpz-0.0.9/tests/test_algos.py` & `pz-rail-bpz-0.1.0/tests/test_algos.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 def test_bpz_lite():
     train_config_dict = {}
     estim_config_dict = {'zmin': 0.0, 'zmax': 3.0,
                          'dz': 0.01,
                          'nzbins': 301,
                          'data_path': None,
                          'columns_file': os.path.join(RAIL_BPZ_DIR, "rail/examples_data/estimation_data/configs/test_bpz.columns"),
-                         'spectra_file': "SED/CWWSB4.list",
+                         'spectra_file': "CWWSB4.list",
                          'madau_flag': 'no',
                          'no_prior': False,
                          'ref_band': 'mag_i_lsst',
                          'prior_file': 'hdfn_gen',
                          'p_min': 0.005,
                          'gauss_kernel': 0.0,
                          'zp_errors': np.array([0.01, 0.01, 0.01, 0.01, 0.01, 0.01]),
@@ -87,15 +87,15 @@
 )
 def test_bpz_wHDFN_prior(inputdata, groupname):
     estim_config_dict = {'zmin': 0.0, 'zmax': 3.0,
                          'dz': 0.01,
                          'nzbins': 301,
                          'data_path': None,
                          'columns_file': os.path.join(RAIL_BPZ_DIR, "rail/examples_data/estimation_data/configs/test_bpz.columns"),
-                         'spectra_file': "SED/CWWSB4.list",
+                         'spectra_file': "CWWSB4.list",
                          'madau_flag': 'no',
                          'ref_band': 'mag_i_lsst',
                          'prior_file': 'flat',
                          'p_min': 0.005,
                          'gauss_kernel': 0.1,
                          'zp_errors': np.array([0.01, 0.01, 0.01, 0.01, 0.01, 0.01]),
                          'mag_err_min': 0.005,
@@ -116,15 +116,15 @@
 def test_bpz_lite_wkernel_flatprior():
     train_config_dict = {}
     estim_config_dict = {'zmin': 0.0, 'zmax': 3.0,
                          'dz': 0.01,
                          'nzbins': 301,
                          'data_path': None,
                          'columns_file': os.path.join(RAIL_BPZ_DIR, "rail/examples_data/estimation_data/configs/test_bpz.columns"),
-                         'spectra_file': "SED/CWWSB4.list",
+                         'spectra_file': "CWWSB4.list",
                          'madau_flag': 'no',
                          'ref_band': 'mag_i_lsst',
                          'prior_file': 'flat',
                          'p_min': 0.005,
                          'gauss_kernel': 0.1,
                          'zp_errors': np.array([0.01, 0.01, 0.01, 0.01, 0.01, 0.01]),
                          'mag_err_min': 0.005,
```

### Comparing `pz-rail-bpz-0.0.9/tests/validation_10gal.pq` & `pz-rail-bpz-0.1.0/tests/validation_10gal.pq`

 * *Files identical despite different names*

