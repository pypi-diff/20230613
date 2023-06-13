# Comparing `tmp/swifter-1.3.4.tar.gz` & `tmp/swifter-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swifter-1.3.4.tar", last modified: Tue Aug 16 23:30:20 2022, max compression
+gzip compressed data, was "dist/swifter-1.3.5.tar", last modified: Tue Jun 13 03:04:35 2023, max compression
```

## Comparing `swifter-1.3.4.tar` & `swifter-1.3.5.tar`

### file list

```diff
@@ -1,49 +1,38 @@
-drwxr-xr-x   0 jmcarpenter   (501) staff       (20)        0 2022-08-16 23:30:20.788413 swifter-1.3.4/
--rw-------   0 jmcarpenter   (501) staff       (20)     1072 2018-08-21 19:54:00.000000 swifter-1.3.4/LICENSE
--rw-------   0 jmcarpenter   (501) staff       (20)       56 2020-07-26 20:36:18.000000 swifter-1.3.4/MANIFEST.in
--rw-r--r--   0 jmcarpenter   (501) staff       (20)      510 2022-08-16 23:30:20.788690 swifter-1.3.4/PKG-INFO
--rw-r--r--   0 jmcarpenter   (501) staff       (20)     4813 2022-08-03 20:19:56.000000 swifter-1.3.4/README.md
-drwxr-xr-x   0 jmcarpenter   (501) staff       (20)        0 2022-08-16 23:30:20.367029 swifter-1.3.4/assets/
--rw-r--r--   0 jmcarpenter   (501) staff       (20)    25427 2022-08-16 20:06:27.000000 swifter-1.3.4/assets/groupby_parallel_v_single_log10.png
--rw-r--r--   0 jmcarpenter   (501) staff       (20)    21371 2022-08-16 20:06:27.000000 swifter-1.3.4/assets/groupby_parallel_v_single_real.png
--rw-r--r--   0 jmcarpenter   (501) staff       (20)    22263 2022-07-24 04:45:29.000000 swifter-1.3.4/assets/groupby_parallel_v_single_text_log10.png
--rw-r--r--   0 jmcarpenter   (501) staff       (20)    19696 2022-07-24 04:45:29.000000 swifter-1.3.4/assets/groupby_parallel_v_single_text_real.png
--rw-------   0 jmcarpenter   (501) staff       (20)    19922 2020-09-19 23:37:53.000000 swifter-1.3.4/assets/modin_swifter_performance_benchmark_log10.png
--rw-------   0 jmcarpenter   (501) staff       (20)    17220 2020-09-19 23:37:53.000000 swifter-1.3.4/assets/modin_swifter_performance_benchmark_real.png
--rw-------   0 jmcarpenter   (501) staff       (20)    22488 2020-07-26 20:36:18.000000 swifter-1.3.4/assets/multiprocessing_v_single_log10.png
--rw-------   0 jmcarpenter   (501) staff       (20)    17977 2020-07-26 20:36:18.000000 swifter-1.3.4/assets/multiprocessing_v_single_real.png
--rw-------   0 jmcarpenter   (501) staff       (20)    20448 2020-07-26 20:36:18.000000 swifter-1.3.4/assets/vectorizes_when_possible_log10.png
--rw-------   0 jmcarpenter   (501) staff       (20)    18628 2020-07-26 20:36:18.000000 swifter-1.3.4/assets/vectorizes_when_possible_real.png
-drwxr-xr-x   0 jmcarpenter   (501) staff       (20)        0 2022-08-16 23:30:20.370228 swifter-1.3.4/docs/
--rw-r--r--   0 jmcarpenter   (501) staff       (20)    10574 2022-08-16 23:30:12.000000 swifter-1.3.4/docs/changelog.md
--rw-r--r--   0 jmcarpenter   (501) staff       (20)     9651 2022-07-24 04:45:29.000000 swifter-1.3.4/docs/documentation.md
-drwxr-xr-x   0 jmcarpenter   (501) staff       (20)        0 2022-08-16 23:30:20.379620 swifter-1.3.4/examples/
-drwxr-xr-x   0 jmcarpenter   (501) staff       (20)        0 2022-08-16 23:30:20.622911 swifter-1.3.4/examples/.ipynb_checkpoints/
--rw-r--r--   0 jmcarpenter   (501) staff       (20)    11549 2022-07-28 20:00:33.000000 swifter-1.3.4/examples/.ipynb_checkpoints/Untitled-checkpoint.ipynb
--rw-r--r--   0 jmcarpenter   (501) staff       (20)       72 2022-04-12 17:18:09.000000 swifter-1.3.4/examples/.ipynb_checkpoints/bug-checkpoint.ipynb
--rw-------   0 jmcarpenter   (501) staff       (20)    52404 2020-08-03 18:49:01.000000 swifter-1.3.4/examples/.ipynb_checkpoints/modin_performance_benchmark-checkpoint.ipynb
--rw-r--r--   0 jmcarpenter   (501) staff       (20)    15945 2022-07-28 21:40:32.000000 swifter-1.3.4/examples/.ipynb_checkpoints/quick_demo-checkpoint.ipynb
--rw-r--r--   0 jmcarpenter   (501) staff       (20)    48413 2022-07-24 03:42:55.000000 swifter-1.3.4/examples/.ipynb_checkpoints/swifter_apply_examples-checkpoint.ipynb
--rw-r--r--   0 jmcarpenter   (501) staff       (20)    49408 2022-07-23 00:16:46.000000 swifter-1.3.4/examples/.ipynb_checkpoints/swifter_groupby_example-checkpoint.ipynb
--rw-------   0 jmcarpenter   (501) staff       (20)   230137 2020-08-03 19:50:22.000000 swifter-1.3.4/examples/.ipynb_checkpoints/swifter_speed_comparison-Copy1-checkpoint.ipynb
--rw-r--r--   0 jmcarpenter   (501) staff       (20)   212635 2022-02-05 00:30:50.000000 swifter-1.3.4/examples/.ipynb_checkpoints/swifter_speed_comparison-checkpoint.ipynb
--rw-r--r--   0 jmcarpenter   (501) staff       (20)    19328 2022-08-02 22:15:40.000000 swifter-1.3.4/examples/Untitled.ipynb
--rw-------   0 jmcarpenter   (501) staff       (20)    52404 2020-09-19 23:37:53.000000 swifter-1.3.4/examples/modin_dataframe_swifter_performance_benchmark.ipynb
--rw-r--r--   0 jmcarpenter   (501) staff       (20)    15945 2022-07-28 21:40:32.000000 swifter-1.3.4/examples/quick_demo.ipynb
--rw-r--r--   0 jmcarpenter   (501) staff       (20)    48413 2022-07-24 04:45:29.000000 swifter-1.3.4/examples/swifter_apply_examples.ipynb
--rw-r--r--   0 jmcarpenter   (501) staff       (20)   348083 2022-07-26 00:02:58.000000 swifter-1.3.4/examples/swifter_speed_comparison.ipynb
--rw-------   0 jmcarpenter   (501) staff       (20)       79 2022-08-16 23:30:20.794983 swifter-1.3.4/setup.cfg
--rw-r--r--   0 jmcarpenter   (501) staff       (20)      931 2022-08-16 23:30:12.000000 swifter-1.3.4/setup.py
-drwxr-xr-x   0 jmcarpenter   (501) staff       (20)        0 2022-08-16 23:30:20.631481 swifter-1.3.4/swifter/
--rw-r--r--   0 jmcarpenter   (501) staff       (20)      600 2022-08-16 23:30:12.000000 swifter-1.3.4/swifter/__init__.py
--rw-r--r--   0 jmcarpenter   (501) staff       (20)     1907 2022-07-24 04:45:29.000000 swifter-1.3.4/swifter/base.py
--rw-r--r--   0 jmcarpenter   (501) staff       (20)     5915 2022-07-07 00:19:34.000000 swifter-1.3.4/swifter/parallel_accessor.py
--rw-r--r--   0 jmcarpenter   (501) staff       (20)    34409 2022-08-16 23:30:12.000000 swifter-1.3.4/swifter/swifter.py
--rw-r--r--   0 jmcarpenter   (501) staff       (20)    47785 2022-08-16 23:30:12.000000 swifter-1.3.4/swifter/swifter_tests.py
--rw-r--r--   0 jmcarpenter   (501) staff       (20)     1160 2022-04-13 00:28:39.000000 swifter-1.3.4/swifter/tqdm_dask_progressbar.py
-drwxr-xr-x   0 jmcarpenter   (501) staff       (20)        0 2022-08-16 23:30:20.787630 swifter-1.3.4/swifter.egg-info/
--rw-r--r--   0 jmcarpenter   (501) staff       (20)      510 2022-08-16 23:30:19.000000 swifter-1.3.4/swifter.egg-info/PKG-INFO
--rw-r--r--   0 jmcarpenter   (501) staff       (20)     1539 2022-08-16 23:30:19.000000 swifter-1.3.4/swifter.egg-info/SOURCES.txt
--rw-r--r--   0 jmcarpenter   (501) staff       (20)        1 2022-08-16 23:30:19.000000 swifter-1.3.4/swifter.egg-info/dependency_links.txt
--rw-r--r--   0 jmcarpenter   (501) staff       (20)      150 2022-08-16 23:30:19.000000 swifter-1.3.4/swifter.egg-info/requires.txt
--rw-r--r--   0 jmcarpenter   (501) staff       (20)        8 2022-08-16 23:30:19.000000 swifter-1.3.4/swifter.egg-info/top_level.txt
+drwxr-xr-x   0 jmcarpenter   (501) staff       (20)        0 2023-06-13 03:04:35.815509 swifter-1.3.5/
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)     1072 2021-06-25 15:03:32.000000 swifter-1.3.5/LICENSE
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)       56 2021-06-25 15:03:32.000000 swifter-1.3.5/MANIFEST.in
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)      499 2023-06-13 03:04:35.815761 swifter-1.3.5/PKG-INFO
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)     4813 2023-06-13 03:00:36.000000 swifter-1.3.5/README.md
+drwxr-xr-x   0 jmcarpenter   (501) staff       (20)        0 2023-06-13 03:04:35.808362 swifter-1.3.5/assets/
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)    25427 2023-06-13 03:00:36.000000 swifter-1.3.5/assets/groupby_parallel_v_single_log10.png
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)    21371 2023-06-13 03:00:36.000000 swifter-1.3.5/assets/groupby_parallel_v_single_real.png
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)    22263 2023-06-13 03:00:36.000000 swifter-1.3.5/assets/groupby_parallel_v_single_text_log10.png
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)    19696 2023-06-13 03:00:36.000000 swifter-1.3.5/assets/groupby_parallel_v_single_text_real.png
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)    19922 2021-06-25 15:03:32.000000 swifter-1.3.5/assets/modin_swifter_performance_benchmark_log10.png
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)    17220 2021-06-25 15:03:32.000000 swifter-1.3.5/assets/modin_swifter_performance_benchmark_real.png
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)    22488 2021-06-25 15:03:32.000000 swifter-1.3.5/assets/multiprocessing_v_single_log10.png
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)    17977 2021-06-25 15:03:32.000000 swifter-1.3.5/assets/multiprocessing_v_single_real.png
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)    20448 2021-06-25 15:03:32.000000 swifter-1.3.5/assets/vectorizes_when_possible_log10.png
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)    18628 2021-06-25 15:03:32.000000 swifter-1.3.5/assets/vectorizes_when_possible_real.png
+drwxr-xr-x   0 jmcarpenter   (501) staff       (20)        0 2023-06-13 03:04:35.809083 swifter-1.3.5/docs/
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)    10684 2023-06-13 03:03:47.000000 swifter-1.3.5/docs/changelog.md
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)     9651 2023-06-13 03:00:36.000000 swifter-1.3.5/docs/documentation.md
+drwxr-xr-x   0 jmcarpenter   (501) staff       (20)        0 2023-06-13 03:04:35.810269 swifter-1.3.5/examples/
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)    52404 2021-06-25 15:03:32.000000 swifter-1.3.5/examples/modin_dataframe_swifter_performance_benchmark.ipynb
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)    48413 2023-06-13 03:00:36.000000 swifter-1.3.5/examples/swifter_apply_examples.ipynb
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)   348083 2023-06-13 03:00:36.000000 swifter-1.3.5/examples/swifter_speed_comparison.ipynb
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)       79 2023-06-13 03:04:35.816673 swifter-1.3.5/setup.cfg
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)      931 2023-06-13 03:03:47.000000 swifter-1.3.5/setup.py
+drwxr-xr-x   0 jmcarpenter   (501) staff       (20)        0 2023-06-13 03:04:35.813217 swifter-1.3.5/swifter/
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)      600 2023-06-13 03:03:47.000000 swifter-1.3.5/swifter/__init__.py
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)     1907 2023-06-13 03:00:36.000000 swifter-1.3.5/swifter/base.py
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)     5915 2023-06-13 03:00:36.000000 swifter-1.3.5/swifter/parallel_accessor.py
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)    33450 2023-06-13 03:00:36.000000 swifter-1.3.5/swifter/swifter.py
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)    48584 2023-06-13 03:00:36.000000 swifter-1.3.5/swifter/swifter_tests.py
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)     1160 2023-06-13 03:00:36.000000 swifter-1.3.5/swifter/tqdm_dask_progressbar.py
+drwxr-xr-x   0 jmcarpenter   (501) staff       (20)        0 2023-06-13 03:04:35.815127 swifter-1.3.5/swifter.egg-info/
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)      499 2023-06-13 03:04:35.000000 swifter-1.3.5/swifter.egg-info/PKG-INFO
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)      974 2023-06-13 03:04:35.000000 swifter-1.3.5/swifter.egg-info/SOURCES.txt
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)        1 2023-06-13 03:04:35.000000 swifter-1.3.5/swifter.egg-info/dependency_links.txt
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)      150 2023-06-13 03:04:35.000000 swifter-1.3.5/swifter.egg-info/requires.txt
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)        8 2023-06-13 03:04:35.000000 swifter-1.3.5/swifter.egg-info/top_level.txt
```

### Comparing `swifter-1.3.4/LICENSE` & `swifter-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `swifter-1.3.4/README.md` & `swifter-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `swifter-1.3.4/assets/groupby_parallel_v_single_log10.png` & `swifter-1.3.5/assets/groupby_parallel_v_single_log10.png`

 * *Files identical despite different names*

### Comparing `swifter-1.3.4/assets/groupby_parallel_v_single_real.png` & `swifter-1.3.5/assets/groupby_parallel_v_single_real.png`

 * *Files identical despite different names*

### Comparing `swifter-1.3.4/assets/groupby_parallel_v_single_text_log10.png` & `swifter-1.3.5/assets/groupby_parallel_v_single_text_log10.png`

 * *Files identical despite different names*

### Comparing `swifter-1.3.4/assets/groupby_parallel_v_single_text_real.png` & `swifter-1.3.5/assets/groupby_parallel_v_single_text_real.png`

 * *Files identical despite different names*

### Comparing `swifter-1.3.4/assets/modin_swifter_performance_benchmark_log10.png` & `swifter-1.3.5/assets/modin_swifter_performance_benchmark_log10.png`

 * *Files identical despite different names*

### Comparing `swifter-1.3.4/assets/modin_swifter_performance_benchmark_real.png` & `swifter-1.3.5/assets/modin_swifter_performance_benchmark_real.png`

 * *Files identical despite different names*

### Comparing `swifter-1.3.4/assets/multiprocessing_v_single_log10.png` & `swifter-1.3.5/assets/multiprocessing_v_single_log10.png`

 * *Files identical despite different names*

### Comparing `swifter-1.3.4/assets/multiprocessing_v_single_real.png` & `swifter-1.3.5/assets/multiprocessing_v_single_real.png`

 * *Files identical despite different names*

### Comparing `swifter-1.3.4/assets/vectorizes_when_possible_log10.png` & `swifter-1.3.5/assets/vectorizes_when_possible_log10.png`

 * *Files identical despite different names*

### Comparing `swifter-1.3.4/assets/vectorizes_when_possible_real.png` & `swifter-1.3.5/assets/vectorizes_when_possible_real.png`

 * *Files identical despite different names*

### Comparing `swifter-1.3.4/docs/changelog.md` & `swifter-1.3.5/docs/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changelog
 
+## Version 1.3.5 -- 2023-06-12
+* Add secondary fallback for series applies
+* Code refactoring for simplicity
+
 ## Version 1.3.4 -- 2022-08-16
 * Enable indexing after a groupby, e.g. `df.swifter.groupby(by)[key].apply(func)`
 * Improve groupby apply progress bar
   - Previously, the groupby apply progress bar only appeared after the data was distributed across the cores.
   - Now, the groupby apply progress bar appears before the data is distributed for a more realistic reflection of how long it took
 * Additional groupby apply code refactoring and optimizations, including removing the mutability of the data within `ray`
```

### Comparing `swifter-1.3.4/docs/documentation.md` & `swifter-1.3.5/docs/documentation.md`

 * *Files identical despite different names*

### Comparing `swifter-1.3.4/examples/.ipynb_checkpoints/modin_performance_benchmark-checkpoint.ipynb` & `swifter-1.3.5/examples/modin_dataframe_swifter_performance_benchmark.ipynb`

 * *Files identical despite different names*

### Comparing `swifter-1.3.4/examples/.ipynb_checkpoints/swifter_apply_examples-checkpoint.ipynb` & `swifter-1.3.5/examples/swifter_apply_examples.ipynb`

 * *Files identical despite different names*

### Comparing `swifter-1.3.4/examples/.ipynb_checkpoints/swifter_speed_comparison-checkpoint.ipynb` & `swifter-1.3.5/examples/swifter_speed_comparison.ipynb`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9550144300144301%*

 * *Differences: {"'cells'": "{4: {'execution_count': 3, 'source': ['data = "*

 * *            'pd.read_feather("../../swifter_data/data/status")\']}, 12: {\'source\': {insert: [(1, '*

 * *            "'This function performs an operation on a string column.')], delete: [1]}}, insert: "*

 * *            "[(14, OrderedDict([('cell_type', 'markdown'), ('metadata', OrderedDict()), ('source', "*

 * *            "['## Group By Apply aggregation functions\\n', 'This function performs a group by "*

 * *            "operation on numeric columns.'])])), (15 […]*

```diff
@@ -50,49 +50,24 @@
             "source": [
                 "These data (~71 million rows) were taken from https://www.kaggle.com/benhamner/sf-bay-area-bike-share/data.\n",
                 "In order to run the speed comparisons in this notebook yourself, you will need to download the data from that location, and unzip the file into the the `examples` directory."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
-            "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "Collecting pyarrow\n",
-                        "  Downloading pyarrow-7.0.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (26.7 MB)\n",
-                        "\u001b[K     |\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 26.7 MB 4.6 MB/s eta 0:00:01\n",
-                        "\u001b[?25hRequirement already satisfied: numpy>=1.16.6 in /usr/local/lib/python3.10/site-packages (from pyarrow) (1.22.2)\n",
-                        "Installing collected packages: pyarrow\n",
-                        "Successfully installed pyarrow-7.0.0\n",
-                        "\u001b[33mWARNING: Running pip as the 'root' user can result in broken permissions and conflicting behaviour with the system package manager. It is recommended to use a virtual environment instead: https://pip.pypa.io/warnings/venv\u001b[0m\n",
-                        "\u001b[33mWARNING: You are using pip version 21.2.4; however, version 22.0.3 is available.\n",
-                        "You should consider upgrading via the '/usr/local/bin/python -m pip install --upgrade pip' command.\u001b[0m\n"
-                    ]
-                }
-            ],
-            "source": [
-                "!pip install pyarrow"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 3,
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2020-08-03T23:54:58.848056Z",
                     "start_time": "2020-08-03T23:54:46.674387Z"
                 }
             },
             "outputs": [],
             "source": [
-                "data = pd.read_feather(\"../data/status\")"
+                "data = pd.read_feather(\"../../swifter_data/data/status\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "metadata": {
                 "ExecuteTime": {
@@ -284,15 +259,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Non-vectorized string functions\n",
-                "This function performs an operation on a string column, and therefore leverages modin dataframes."
+                "This function performs an operation on a string column."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
             "metadata": {
                 "ExecuteTime": {
@@ -306,14 +281,50 @@
                 "    return f\"Station ID {row['station_id']} had {row['bikes_available']} bikes available at {row['time']}. This is {np.where(row['bikes_available'] > row['docks_available'], 'more', 'less')} than the number of docks available ({row['docks_available']}).\""
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "## Group By Apply aggregation functions\n",
+                "This function performs a group by operation on numeric columns."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 3,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "def agg_func(x):\n",
+                "    return x[\"normal\"].mean() / x[\"exponential\"].var()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## Group By Apply text functions\n",
+                "This function performs a group by operation on string columns."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 4,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "def join_text_func(x):\n",
+                "    return \" \".join([name for name in x[\"first\"].values.tolist() + x[\"last\"].values.tolist()])"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
                 "# Perfplot\n",
                 "[Perfplot](https://github.com/unutbu/perfplot) is a library for performing speed comparisons of various functions.\n",
                 "\n",
                 "Here we use perfplot to compare pandas apply, dask apply, vectorized functions, and swifter apply."
             ]
         },
         {
@@ -881,14 +892,465 @@
                 "fig = plt.figure()\n",
                 "nonvectorized_string_comparison.xlabel = 'log10(n_rows)'\n",
                 "nonvectorized_string_comparison.title = 'Non-Vectorized String Function Speed Comparison [LogLog Plot]'\n",
                 "nonvectorized_string_comparison.plot(logx=True, logy=True, time_unit='s')\n",
                 "plt.ylabel(\"Runtime [log10(s)]\")\n",
                 "plt.savefig(\"nonvectorized_string_axis1_speed_comparison_loglog.png\")"
             ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "# Groupby Apply aggregation function speed comparison"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 5,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "SIZE = 100000000\n",
+                "data = pd.DataFrame({\n",
+                "    \"groups\": np.random.choice(np.arange(100000), size=SIZE),\n",
+                "    \"normal\": np.random.normal(size=SIZE),\n",
+                "    \"exponential\": np.random.exponential(size=SIZE),\n",
+                "})"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 6,
+            "metadata": {
+                "scrolled": true
+            },
+            "outputs": [
+                {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "  0% 0/11 [00:00<?, ?it/s]\n",
+                        "  0% 0/3 [00:00<?, ?it/s]\u001b[A\n",
+                        " 33% 1/3 [00:00<00:00,  2.12it/s]\u001b[A/tmp/ipykernel_31702/2989292544.py:2: RuntimeWarning: divide by zero encountered in double_scalars\n",
+                        "  return x[\"normal\"].mean() / x[\"exponential\"].var()\n",
+                        "/tmp/ipykernel_31702/2277446876.py:5: UserWarning: `meta` is not specified, inferred from partial data. Please provide `meta` if the result is unexpected.\n",
+                        "  Before: .apply(func)\n",
+                        "  After:  .apply(func, meta={'x': 'f8', 'y': 'f8'}) for dataframe result\n",
+                        "  or:     .apply(func, meta=('x', 'f8'))            for series result\n",
+                        "  lambda df: dd.from_pandas(df, npartitions=npartitions).groupby(\"groups\").apply(agg_func).compute(scheduler=\"processes\").sort_values(ascending=False),\n",
+                        "\n",
+                        " 67% 2/3 [00:01<00:00,  1.14it/s]\u001b[A\n",
+                        "100% 3/3 [00:02<00:00,  1.42it/s]\u001b[A\n",
+                        "  9% 1/11 [00:02<00:21,  2.14s/it][A\n",
+                        "  0% 0/3 [00:00<?, ?it/s]\u001b[A\n",
+                        " 33% 1/3 [00:00<00:01,  1.22it/s]\u001b[A/tmp/ipykernel_31702/2989292544.py:2: RuntimeWarning: divide by zero encountered in double_scalars\n",
+                        "  return x[\"normal\"].mean() / x[\"exponential\"].var()\n",
+                        "/tmp/ipykernel_31702/2277446876.py:5: UserWarning: `meta` is not specified, inferred from partial data. Please provide `meta` if the result is unexpected.\n",
+                        "  Before: .apply(func)\n",
+                        "  After:  .apply(func, meta={'x': 'f8', 'y': 'f8'}) for dataframe result\n",
+                        "  or:     .apply(func, meta=('x', 'f8'))            for series result\n",
+                        "  lambda df: dd.from_pandas(df, npartitions=npartitions).groupby(\"groups\").apply(agg_func).compute(scheduler=\"processes\").sort_values(ascending=False),\n",
+                        "\n",
+                        " 67% 2/3 [00:01<00:00,  1.01it/s]\u001b[A\n",
+                        "100% 3/3 [00:02<00:00,  1.19it/s]\u001b[A\n",
+                        " 18% 2/11 [00:04<00:21,  2.41s/it][A\n",
+                        "  0% 0/3 [00:00<?, ?it/s]\u001b[A\n",
+                        " 33% 1/3 [00:00<00:01,  1.26it/s]\u001b[A/tmp/ipykernel_31702/2989292544.py:2: RuntimeWarning: divide by zero encountered in double_scalars\n",
+                        "  return x[\"normal\"].mean() / x[\"exponential\"].var()\n",
+                        "/tmp/ipykernel_31702/2277446876.py:5: UserWarning: `meta` is not specified, inferred from partial data. Please provide `meta` if the result is unexpected.\n",
+                        "  Before: .apply(func)\n",
+                        "  After:  .apply(func, meta={'x': 'f8', 'y': 'f8'}) for dataframe result\n",
+                        "  or:     .apply(func, meta=('x', 'f8'))            for series result\n",
+                        "  lambda df: dd.from_pandas(df, npartitions=npartitions).groupby(\"groups\").apply(agg_func).compute(scheduler=\"processes\").sort_values(ascending=False),\n",
+                        "\n",
+                        " 67% 2/3 [00:02<00:01,  1.06s/it]\u001b[A\n",
+                        "100% 3/3 [00:02<00:00,  1.09it/s]\u001b[A\n",
+                        " 27% 3/11 [00:07<00:20,  2.59s/it][A\n",
+                        "  0% 0/3 [00:00<?, ?it/s]\u001b[A\n",
+                        " 33% 1/3 [00:00<00:01,  1.03it/s]\u001b[A/tmp/ipykernel_31702/2989292544.py:2: RuntimeWarning: divide by zero encountered in double_scalars\n",
+                        "  return x[\"normal\"].mean() / x[\"exponential\"].var()\n",
+                        "/tmp/ipykernel_31702/2277446876.py:5: UserWarning: `meta` is not specified, inferred from partial data. Please provide `meta` if the result is unexpected.\n",
+                        "  Before: .apply(func)\n",
+                        "  After:  .apply(func, meta={'x': 'f8', 'y': 'f8'}) for dataframe result\n",
+                        "  or:     .apply(func, meta=('x', 'f8'))            for series result\n",
+                        "  lambda df: dd.from_pandas(df, npartitions=npartitions).groupby(\"groups\").apply(agg_func).compute(scheduler=\"processes\").sort_values(ascending=False),\n",
+                        "\n",
+                        " 67% 2/3 [00:02<00:01,  1.24s/it]\u001b[A\n",
+                        "100% 3/3 [00:03<00:00,  1.09s/it]\u001b[A\n",
+                        " 36% 4/11 [00:10<00:20,  2.88s/it][A\n",
+                        "  0% 0/3 [00:00<?, ?it/s]\u001b[A\n",
+                        " 33% 1/3 [00:01<00:02,  1.00s/it]\u001b[A/tmp/ipykernel_31702/2989292544.py:2: RuntimeWarning: divide by zero encountered in double_scalars\n",
+                        "  return x[\"normal\"].mean() / x[\"exponential\"].var()\n",
+                        "/tmp/ipykernel_31702/2277446876.py:5: UserWarning: `meta` is not specified, inferred from partial data. Please provide `meta` if the result is unexpected.\n",
+                        "  Before: .apply(func)\n",
+                        "  After:  .apply(func, meta={'x': 'f8', 'y': 'f8'}) for dataframe result\n",
+                        "  or:     .apply(func, meta=('x', 'f8'))            for series result\n",
+                        "  lambda df: dd.from_pandas(df, npartitions=npartitions).groupby(\"groups\").apply(agg_func).compute(scheduler=\"processes\").sort_values(ascending=False),\n",
+                        "\n",
+                        " 67% 2/3 [00:02<00:01,  1.43s/it]\u001b[A\n",
+                        "100% 3/3 [00:03<00:00,  1.23s/it]\u001b[A\n",
+                        " 45% 5/11 [00:14<00:19,  3.19s/it][A\n",
+                        "  0% 0/3 [00:00<?, ?it/s]\u001b[A\n",
+                        " 33% 1/3 [00:00<00:01,  1.39it/s]\u001b[A/tmp/ipykernel_31702/2989292544.py:2: RuntimeWarning: divide by zero encountered in double_scalars\n",
+                        "  return x[\"normal\"].mean() / x[\"exponential\"].var()\n",
+                        "/tmp/ipykernel_31702/2277446876.py:5: UserWarning: `meta` is not specified, inferred from partial data. Please provide `meta` if the result is unexpected.\n",
+                        "  Before: .apply(func)\n",
+                        "  After:  .apply(func, meta={'x': 'f8', 'y': 'f8'}) for dataframe result\n",
+                        "  or:     .apply(func, meta=('x', 'f8'))            for series result\n",
+                        "  lambda df: dd.from_pandas(df, npartitions=npartitions).groupby(\"groups\").apply(agg_func).compute(scheduler=\"processes\").sort_values(ascending=False),\n",
+                        "\n",
+                        " 67% 2/3 [00:03<00:01,  1.69s/it]\u001b[A\n",
+                        "100% 3/3 [00:03<00:00,  1.25s/it]\u001b[A\n",
+                        " 55% 6/11 [00:18<00:17,  3.40s/it][A\n",
+                        "  0% 0/3 [00:00<?, ?it/s]\u001b[A\n",
+                        " 33% 1/3 [00:01<00:02,  1.38s/it]\u001b[A/tmp/ipykernel_31702/2989292544.py:2: RuntimeWarning: divide by zero encountered in double_scalars\n",
+                        "  return x[\"normal\"].mean() / x[\"exponential\"].var()\n",
+                        "/tmp/ipykernel_31702/2277446876.py:5: UserWarning: `meta` is not specified, inferred from partial data. Please provide `meta` if the result is unexpected.\n",
+                        "  Before: .apply(func)\n",
+                        "  After:  .apply(func, meta={'x': 'f8', 'y': 'f8'}) for dataframe result\n",
+                        "  or:     .apply(func, meta=('x', 'f8'))            for series result\n",
+                        "  lambda df: dd.from_pandas(df, npartitions=npartitions).groupby(\"groups\").apply(agg_func).compute(scheduler=\"processes\").sort_values(ascending=False),\n",
+                        "\n",
+                        " 67% 2/3 [00:04<00:02,  2.45s/it]\u001b[A\n",
+                        "100% 3/3 [00:06<00:00,  2.01s/it]\u001b[A\n",
+                        " 64% 7/11 [00:24<00:17,  4.27s/it][A\n",
+                        "  0% 0/3 [00:00<?, ?it/s]\u001b[A\n",
+                        " 33% 1/3 [00:05<00:10,  5.22s/it]\u001b[A/tmp/ipykernel_31702/2989292544.py:2: RuntimeWarning: divide by zero encountered in double_scalars\n",
+                        "  return x[\"normal\"].mean() / x[\"exponential\"].var()\n",
+                        "/tmp/ipykernel_31702/2277446876.py:5: UserWarning: `meta` is not specified, inferred from partial data. Please provide `meta` if the result is unexpected.\n",
+                        "  Before: .apply(func)\n",
+                        "  After:  .apply(func, meta={'x': 'f8', 'y': 'f8'}) for dataframe result\n",
+                        "  or:     .apply(func, meta=('x', 'f8'))            for series result\n",
+                        "  lambda df: dd.from_pandas(df, npartitions=npartitions).groupby(\"groups\").apply(agg_func).compute(scheduler=\"processes\").sort_values(ascending=False),\n",
+                        "\n",
+                        " 67% 2/3 [00:09<00:04,  4.49s/it]\u001b[A2022-07-24 03:25:03,657\tWARNING services.py:2002 -- WARNING: The object store is using /tmp instead of /dev/shm because /dev/shm has only 67104768 bytes available. This will harm performance! You may be able to free up space by deleting files in /dev/shm. If you are inside a Docker container, you can increase /dev/shm size by passing '--shm-size=10.24gb' to 'docker run' (or add it to the run_options list in a Ray cluster config). Make sure to set this to more than 30% of available RAM.\n",
+                        "\n",
+                        "100% 3/3 [00:14<00:00,  4.90s/it]\u001b[A\n",
+                        " 73% 8/11 [00:39<00:22,  7.56s/it][A\n",
+                        "  0% 0/3 [00:00<?, ?it/s]\u001b[A\n",
+                        " 33% 1/3 [00:18<00:36, 18.27s/it]\u001b[A/tmp/ipykernel_31702/2989292544.py:2: RuntimeWarning: divide by zero encountered in double_scalars\n",
+                        "  return x[\"normal\"].mean() / x[\"exponential\"].var()\n",
+                        "/tmp/ipykernel_31702/2277446876.py:5: UserWarning: `meta` is not specified, inferred from partial data. Please provide `meta` if the result is unexpected.\n",
+                        "  Before: .apply(func)\n",
+                        "  After:  .apply(func, meta={'x': 'f8', 'y': 'f8'}) for dataframe result\n",
+                        "  or:     .apply(func, meta=('x', 'f8'))            for series result\n",
+                        "  lambda df: dd.from_pandas(df, npartitions=npartitions).groupby(\"groups\").apply(agg_func).compute(scheduler=\"processes\").sort_values(ascending=False),\n",
+                        "\n",
+                        " 67% 2/3 [00:24<00:11, 11.18s/it]\u001b[A\n",
+                        "100% 3/3 [00:26<00:00,  7.04s/it]\u001b[A\n",
+                        " 82% 9/11 [01:05<00:27, 13.52s/it][A\n",
+                        "  0% 0/3 [00:00<?, ?it/s]\u001b[A\n",
+                        " 33% 1/3 [00:34<01:09, 34.77s/it]\u001b[A/tmp/ipykernel_31702/2989292544.py:2: RuntimeWarning: divide by zero encountered in double_scalars\n",
+                        "  return x[\"normal\"].mean() / x[\"exponential\"].var()\n",
+                        "/tmp/ipykernel_31702/2277446876.py:5: UserWarning: `meta` is not specified, inferred from partial data. Please provide `meta` if the result is unexpected.\n",
+                        "  Before: .apply(func)\n",
+                        "  After:  .apply(func, meta={'x': 'f8', 'y': 'f8'}) for dataframe result\n",
+                        "  or:     .apply(func, meta=('x', 'f8'))            for series result\n",
+                        "  lambda df: dd.from_pandas(df, npartitions=npartitions).groupby(\"groups\").apply(agg_func).compute(scheduler=\"processes\").sort_values(ascending=False),\n"
+                    ]
+                },
+                {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "\n",
+                        " 67% 2/3 [00:44<00:19, 19.76s/it]\u001b[A\n",
+                        "100% 3/3 [00:48<00:00, 12.68s/it]\u001b[A\n",
+                        " 91% 10/11 [01:53<00:24, 24.25s/it]A\n",
+                        "  0% 0/3 [00:00<?, ?it/s]\u001b[A\n",
+                        " 33% 1/3 [00:38<01:16, 38.35s/it]\u001b[A/tmp/ipykernel_31702/2989292544.py:2: RuntimeWarning: divide by zero encountered in double_scalars\n",
+                        "  return x[\"normal\"].mean() / x[\"exponential\"].var()\n",
+                        "/tmp/ipykernel_31702/2277446876.py:5: UserWarning: `meta` is not specified, inferred from partial data. Please provide `meta` if the result is unexpected.\n",
+                        "  Before: .apply(func)\n",
+                        "  After:  .apply(func, meta={'x': 'f8', 'y': 'f8'}) for dataframe result\n",
+                        "  or:     .apply(func, meta=('x', 'f8'))            for series result\n",
+                        "  lambda df: dd.from_pandas(df, npartitions=npartitions).groupby(\"groups\").apply(agg_func).compute(scheduler=\"processes\").sort_values(ascending=False),\n",
+                        "\n",
+                        " 67% 2/3 [00:48<00:21, 21.68s/it]\u001b[A\n",
+                        "100% 3/3 [00:54<00:00, 18.10s/it]\u001b[A\n",
+                        "100% 11/11 [02:48<00:00, 15.30s/it]\n"
+                    ]
+                }
+            ],
+            "source": [
+                "vectorized_comparison = perfplot.bench(\n",
+                "    setup=lambda n: data.iloc[:n],\n",
+                "    kernels=[\n",
+                "        lambda df: df.groupby(\"groups\").apply(agg_func),\n",
+                "        lambda df: dd.from_pandas(df, npartitions=npartitions).groupby(\"groups\").apply(agg_func).compute(scheduler=\"processes\").sort_values(ascending=False),\n",
+                "        lambda df: df.swifter.progress_bar(False).groupby(\"groups\").apply(agg_func),\n",
+                "    ],\n",
+                "    labels=['Pandas Apply', 'Dask Apply', 'Swifter Apply'],\n",
+                "    n_range=[2**k for k in range(0, 22, 2)],\n",
+                "    xlabel='n_rows',\n",
+                "    equality_check=None\n",
+                ")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 7,
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAYEAAAEWCAYAAACAOivfAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjUuMiwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy8qNh9FAAAACXBIWXMAAAsTAAALEwEAmpwYAABJZUlEQVR4nO2dd3xUVfbAvye9EUICRHrvHQKoFIOgou7qKjasWH+66q7r6uoWFdvu2t2i62LfVcGyrgV1XRWyNhRBaVKkG6SXhAQIaef3x3sJk2EymYRMZjJzvp/P+8wrt5z73ptz7j33vntFVTEMwzCik5hQC2AYhmGEDjMChmEYUYwZAcMwjCjGjIBhGEYUY0bAMAwjijEjYBiGEcWYEYhgROQ5Ebkn1HKEGyLynohcEmo5goGIFItI91DLESxEJE9Ergi1HMEgVM+uWRgBETlPRL4UkX0ist3d/6mISAhkmSYiFe4DKxaRdSJyzRGmmeam9V5jydkYiEg3EakUkb+FWpaGIiLTReQFz3OqerKqPh+EvJ4TkVKPd6NYRM5t7Hw88jtMIapqmqquC0JeY0XkcxEpFJHdIvKZiIxs7HyOFBHpLSKvishOV9YlInKjiMSGWra6CNazq4uwNwIi8kvgT8ADwFFANnA1MAZIqCVOsB/4PPeBpQFTgPtFZNgRpDcFOAicICJHNYqEjcPFwB7gXBFJDEYG4hD272E9uL/q3XC3l0Mt0JEiIunAbOAvQCbQAbgT550NG0SkB/AlkA8MUtWWwNlADtAilLL5Q0TiQiqAqobtBrQE9gFT6gj3HPA34F03/CSgH5AHFADfAqd5hM8DrvA4ngZ86nGswM+AdcBOHAMU4yuse24+cL67/w5wvdf1JcAZfuSfA9wLfA3c5HVtA/BrYDmOQn4WSHKv5QKbgN+4cm4ALvC6L/e4+8uAH3tci3fjDKtFJgHWAtcA24CzvK6fCKwCCoHHgf9V3VMgFnjITX89cJ17T+M87v+9wGfAAaAn0Bf4ANjtpnuOR15ZwNvAXuAr4B6v5/UnnD/+XmAhMM49PxkoBcqAYmCx9/PHqQj9DtgIbAf+AbR0r3V15b4E+N4tz2/reA/vqet81XPzesY3ue9JIfBy1TN2r58OLHLLt9Yt171ABVDilu2vHu9uT4//zz+AHW75fofXeww8iPNerQdOrqVcOUCBn3JPc5/lX135VwITvf7HTwNbgB/c5xfrcf0yYIUrx/tAF49rJ7jpFbrpV79nPuR4AXinDl1xGo4+KHDfg35ez+Fm9znsc2XOBt4DioAPgVZe78ZVwGa3bDd5pDUKmOfms8WVPcFLx1wLrAbW+3h2p+D854vce+aZ9pXAGpz/yltAe690r3bTLQAeA8TvPfF3MdSb+7KX4yqPOv58hTitgxgcq78GRzkmAMe7N7OPtxLw/EN43ci5OLWezsB3HFIa3mFHuje7t3t8DvClx/UhwC7PF8BL9i5AJdAf+CWwxOv6BhwF3smV5zMOKfZc9/48DCQCx7kvbx+P+1IV9lfAy16KZamfezoOp6bXCqcG+LbHtdY4CulMIA74OY6irbpHV7svcEc3/occbgS+Bwa48VviKPFL3eNhOAq3vxt+lruluPcp3+sZXIhjKOLce7iVQ4ZyOvCCV9mqnz+OAloDdAfSgNeBf3r90Z8Ekt1neRAPxeHjPWyoEZgPtHef8Qrgag9lUoijDGNwauF9fb3HPhTJP4A3cf4PXXHe48s93uMyHIUSi2PsN+NDYQDpOO/w88DJuIrQ6/9TDvwCp3Jxritzpnv938DfgVSgrVvW//N4D9fgVNricAzV5x7vWRFwlpvuL9x8ajMCW4FL/bzTvXH+Hye46f3KzTvB4zl8gaP4O+BUCr7GeR+TcCprd3i9GzPdcg3CMbaT3OsjgKPdMnV1n+kNXs/pA/d5J/t4dls4VJlpBQx394/H+W8Mx/nP/wX42Cvd2UAGju7aAUz2qz8bS2EHY8P5c2/1Ovc5jtI9AIz3+JP9w0uBbcWt9bjnZgLTff158G0EJnsc/xT4yOuFL3BfUHUfhLjXk3BqNL3c4weBx/2U8XfAIne/A07tbpjH9Q24CsE9PgVY66FMyoFUj+uvALd5Kx8cBVMEpLvHrwG/8iPXU8Ab7v4xOAqjrXt8MY5LrCqs4CjmKsU6B/dP7h5P4nAjcJfH9XOBT7zy/ztwB46CKsM1bO61Gi0BH7LvAYa4+9PxbwQ+An7qca2Pm1/Vn1eBjh7X5wPn1ZLvczg18wJ32+n9HDyem7cRuNDj+H7gCY/78Egt+VWXw+vd7enet1JcQ+pe+z8gz+M9XuNxLcWNe1QtefVzy7EJ5517C8j2SKuGAXHv00U4CvUgrqJzr00F5rr77+EaJvc4BtiPUzm6GPjC6z3b5F1mj+tl+FF4wG3AK155/QDkejwHz5b0v4C/eRxfz6H/RNW70dfruT1dS943AP/2ek7H+3p27v737vNK9wrzNI7Lseo4zS13V480xnrpg1truyeqGvZ9AruA1p4+M1U9VlUz3Gue8ud77LcH8lW10uPcRhwlGyie6W1006ziC1XNUNUWOP0UA4Dfu/KV4DTnL3R93VOBf/rJ52LgRTfuDzjN3UvqIcseVd3n5zpu2ptxWhFTRCQDp0b3oi+BRCQZx5daJdc8nJfyfDdIe0+Z1HnbNnkkUeO6176vc12A0SJSULUBF+Dc2zY4CrnW9ETkJhFZ4XYEFuC0LFr7KpsP2uPcsyo2uvlle5zb6rG/H+ePVxsPuu9GhqoGKoO/PDrhuIDqS2uc2q532Tz/A9V5qup+d9dn2VR1hapOU9WOwECc+/aoR5Af3PfAM6/2OM82Htji8Wz/jtMiwL3+J49ru3GUfQd8v2e+3qUqdgHt/Fyv8axd/ZBPzXuyzWP/gI9j7/vj87/pdlDPFpGtIrIXRz94vw/+yjIFp8K3UUT+JyLH1FKGYpxy+3yu1P2+hr0RmIdTizg9gLCeL+BmoJNXh2NnHKsPTpMwxeOar87YTl5xN/vMVHUbTo3hxx6nn8dRYhOB/a4SPQwRORboBfzafVm2AqOB8706i/zJ0kpEUgOR1ZXrQhwFP881Or44A8cF8LiHXB04ZJy24Lh6qsohnsfe173kr8LzeeUD//NQnhnqdKpeg9OcLa8tPREZh9OsPwfHTZGB44qoGjnmmY8vNuMooio6u/lt8x28QQTyvtVGPtCjlmv+yrYTp4boXbbannnAqOpKnFbBQI/THbxG61W9h/k4/+HWHs82XVUHuOHycVqNns8+WVU/x3mPPJ+14PtdquJDHOVZGzWetUd6R3JPavtv/g2nL6OXqqbjuKa9RzPW+vxU9StVPR3HWL6BU6OHw8uQiuMKbXAZwtoIqGoBziiEx0XkLBFpISIxIjIUxw9XG1/iWMBfiUi8iOTiKOlZ7vVFwJkikiIiPYHLfaRxs4i0EpFOOD5vn6M8RCQLR2l+6yH3PBw//0P4bwVcguMX7A8MdbeBOP7nkz3CXSsiHUUkE/itD1nuFJEEVyH+CHi1lvzewPEl/hzHX+xPrmdw/JxVco0BhojIIJzO70Ei8hPXWF1LTcX2CvBzEengtjpu8ZMXOD7M3iJykfu84kVkpIj0U9UKHD/9dPd59cVpPVXRAkdp7wDiROR2HANWxTagq58RSDOBX7jDYdNwamwvq2p5HTLXh0XAKSKS6Y7+uqEecZ8GLhWRie6738G9B+CUzee4cve+vQLc6/5vugA34nSe1gsR6SsivxSRju5xJ5wW7hcewdoCP3Of3dk47qN3VXUL8F/gIRFJd8vQQ0SOc+M9gVMJGuCm3dKND857NkBEznTfs5/h34DeARwrIg9UjbITkZ4i8oL7Hr4CnOrey3ic/qODOC7mhnKb+14OwOnTqvpvtsDpNyt2n1fAw8jd//IFItJSVcvcdKq8GjNx3oeh7oi93+P0QW5oaAHC2ggAqOr9OC/vr3Be+m04zclbqOXhqWopjtI/GadG9DhwsVuDAXgEx1+6Dad27Mst8ibOSJNFOC/j0x7XjhF3HDhOh88OHH+hJ//AUaI+/3QikoRTe/2Lqm712NbjGA5Pl9BLOH+kdTiuAc8PwLbi+MA3u+W42qOcNVDVAzitlm44itWXXB1wWjCPesm1EPgPcImq7sRpTdyP0xTtDyzg0JDBJ115lwDf4IzaKsfp7/AlVxHOaKPz3HJsBe7D6fgCZ3RRS/f8P3H+CFV5ve/K9R1OM7mEms3sKoO4S0S+9pH9M26aH+OMkCnh8Gd5pPwTWIzjc/4vtVQofKGq83GUyyM4LZz/cagm+CfgLBHZIyJ/9hH9epxWyDqckUAv4ZS3vhThtFC/FJF9OMp/GY4SreJLnFbtTpyRS2ep6i732sU4AzSqRri9huu2UdV/4zzrWa7bZBluBcjjPfsjznvWC8el6RNVXYvTf9UV+FZECnHe9wVAkaquwmkJ/8WV88c4I+ZKG3BPqvgfTufyRziuwP+652/CcZ8W4fwf6jtU+CJgg3tPrsbxLKCqH+L0bfwLp6XUA+d/02CqOjMND0REcZpxa44gjYuBq1R17BHKsgGnI+xDH9dycTo9O3pf85Pe7TgjmS48Erm80ozB6RO4QFXn+rh+Mk5HZ5fDIjcsv/twOjC9+06MECAi03De0SN615sTItIVp9IQ38itxiYn7FsCzRERScEZUTQj1LJ44rqTLqcR5BKRk0Qkw22SVvk7v3CvJYvIKSIS57Ys7sAZJtjQvPqKyGBxGOWWocHpGYZxCDMCjYyInITjHtqG0/wOC0TkShw3yXuq+nEjJHkMjmuqqln9E9fdBI5BuBOn6f8Njsvs9iPIqwWO+2ofTrP6IRx3nWEYR4i5gwzDMKKYoLcERCRWRL4RkdnucTdxJoBbIyIvi4jP+X8MwzCM4BP0loCI3Igz90i6qv5IRF4BXlfVWSLyBM58Ln5nqWzdurV27dq1Qfnv27eP1FR/o0kjAytnZGHljCxCVc6FCxfuVNU2fgP5+5z4SDecD3w+wpnvYjaOr3gnh6YPOAZ4v650RowYoQ1l7ty5DY7bnLByRhZWzsgiVOUEFmgd+jWoLQEReQ34A07H3k04c4x8oao93eudcDoqB/qIexXODH1kZ2ePmDVrlneQgCguLiYtze9X0xGBlTOysHJGFqEq54QJExaqao6/MEGbx1pEfgRsV9WF7nj2eqGqM3CHMubk5Ghubr2TACAvL4+Gxm1OWDkjCytnZBHO5QzmYgZjgNNE5BScmTXTcb5wzBCROHU+sOhII8xlYhiGYTSMoI0OUtVfq2pHVe2K81nzHFW9AGee/rPcYJdg470NwzBCRig+FrsFuFFE1uDMfvd0HeENwzCMINEka1uqah7OAhios5DyqKbI1zAMw/CPTRthGIYRxYR2lXvDMAyD0vJKdu8rrd527TvIHnd/yoiOdMkK3odmZgQMwzAaEVWl+GB5DaX++aYyVv1vravgS9nj/u5294sO+p6NWgSGdWllRsAwDCNUVFQqe/aXetXUS6tr6jWV+kH27CujtKLy8ISWrSQhLoas1AQy3a1LVgqZqQlkpSbQyv3NTE0kMzWezNREWibHExvjvSpl42JGwDCMqKKkrMJR2MWl7N7vKO5dxaXVir5qv6qmXnigjNomVkhPiqtW6B0ykhnUIZ3M1EQvpZ7Ad0u/5pSJ40lJiEUkuEq9vpgRMAyj2aKq7D1Q7vjQ9zsKfPc+V7l77nso9/2lPlc5JS5GaJWaQGaKo7j7tUuv3s9KS6BViqvU05wwrVITiI8NbGzNnrUxpCaGp7oNT6kMw4hKyioqq10rnn5zX9uufY5Sr6j0XU1PSYitrqVnpibQs22ao9TTXPdLiqPcM1MTyUxJID05Luxq6U2BGQHDMIKCqrK/tMKn33z3vjJ27zvIdxtL+PPyz6rDFJXU3kGakRxf7WLp2jqF4V0yXAV/uPslMzWBpPjYJi5x88SMgGEYAVFRqRQeKKvhQ6/pWz+8pl5a7qODFEiIjSEzNYF4Vbq0jKNjq5QatfaqrUq5ZyTHExeg68WoH2YEDCNKKSmrqOFHr8unXrC/lFo8L7RIjCPT9ZsflZ5E/3bptSj1RFqlxpOW6LhenNk1RzdtwY0amBEwjAhAVdlbUn7Y+HNv94ungt9XSwdpjFCttFulJNA7O805djtJM9MSa3SYZqTEkxhnrpfmihkBwwhDKiqV7UUl7NlXxi5XefvrKN2zv5SyCt/V9KT4GLJSEx2lnppA9zZpPmvpVe6X9KR4YoI8Nt0IH8wIGEYTsL+0nLo/NDq0FR4og/9+5DOtlsnx1b7yTpkpDO2UUaNT1HM/KzWR5ASrpRu1Y0bAMOpJZVUHqdf488M/NDpYXZMvKfPdQRofK7RKOVQTH9A+nazUBAp3bGbEgN5kuj70qpp8Rkp8wGPTDSMQzAgYUY+/ybuqxqJ7dp7u2V9W69j01IRY52Oi1ETapCXSJzu95odGnjX1tARaJPoem56Xt5PcY7oGueSGYUbAiDB8Td7lz/1S1+RdnrX0Hm3SfHxodGi/VYqNTTeaH8FcaD4J+BhIdPN5TVXvEJHngOOAQjfoNFVdFCw5jOaN9+RdX20tJ/+LjfWfvAvCcvIuwwg1wWwJHASOV9ViEYkHPhWR99xrN6vqa0HM2whTGmXyrkXLAGiRFFet1DtkJFVP3lWlxL2/Ig3HybsMI9QEzQioqgLF7mG8u9XyqYnRHGnMybtiY6SG37zfUYd/bJSVmsDaFUs46bhjyUhJICHOOkgN40gRrW2O1MZIXCQWWAj0BB5T1Vtcd9AxOC2Fj4BbVfWgj7hXAVcBZGdnj5g1a1aDZCguLiYtLa1hBWhGNFY5Cw8qe0uVIu+tzPktdo/3lkJxmdb6BWliLKTFC+kJQosEIS1BaJEALRKEFvHOOc8tJY6Aaun2PCMLK2dwmTBhwkJVzfEXJqhGoDoTkQzg38D1wC5gK5AAzADWqupd/uLn5OToggULGpS381l6boPiNicao5yPfvgdj364+rDz3pN31ayh+3a/BKuD1J5nZGHlDC4iUqcRaJLRQapaICJzgcmq+qB7+qCIPAvc1BQyGP755vs9/Pmj1Zw0IJvTh3aooeht8i7DiFyCOTqoDVDmGoBk4ATgPhFpp6pbxGn7/wRYFiwZjMAoKavgplcXc1R6Eg+cPYT0pPhQi2QYRhMRzJZAO+B5t18gBnhFVWeLyBzXQAiwCLg6iDIYAfDwB9+xdsc+/nn5KDMAhhFlBHN00BJgmI/zxwcrT6P+LNy4myc/Wcf5ozszrlebUItjGEYTY47eKOZAaQU3vbqE9i2T+c0p/UItjmEYIcCmjYhiHvzvKtbv3MdLV4wmLUwXwTYMI7hYSyBKmb9+N898tp6Lju7CsT1bh1ocwzBChBmBKGR/aTm/em0xHVslc+vJfUMtjmEYIcR8AFHI/f9ZxYZd+5l11dGkmhvIMKIaawlEGV+s28Vzn29g2rFdObp7VqjFMQwjxJgRiCL2HSzn5tcW0yUrhV9N7hNqcQzDCAPMFxBF3PeflWzac4CXrzqGlAR79IZhWEsgavh8zU7+MW8jl43pxqhumaEWxzCMMMGMQBRQfLCcm19bQrfWqdx0ormBDMM4hPkEooDfv7uCzYUHeO3qY0hOsDVwDcM4hLUEIpxPVu/gpS+/58px3RnRxdxAhmHUxIxABFNUUsYtry2hR5tUbjyhd6jFMQwjDDF3UARz7zsr2Lq3hH9dc2zQVvoyDKN5Yy2BCCVv1XZmfZXPVeN7MKxzq1CLYxhGmGJGIAIpPFDGrf9aSq+2adwwqVeoxTEMI4wxd1AEcs/s5ewoPsjfLxphbiDDMPwStJaAiCSJyHwRWSwi34rIne75biLypYisEZGXRSQhWDJEI3NWbuPVhZu45rgeDOmUEWpxDMMIc4LpDjoIHK+qQ4ChwGQRORq4D3hEVXsCe4DLgyhDVFG433ED9cluwfUTe4ZaHMMwmgFBMwLqUOwexrubAscDr7nnnwd+EiwZoo073/6WXftKeeicISTGmRvIMIy6EVUNXuIiscBCoCfwGPAA8IXbCkBEOgHvqepAH3GvAq4CyM7OHjFr1qwGyVBcXExaWlrDCtCM+HxjMTNWCKf3iOeMXpHrYYuW52nljCxCVc4JEyYsVNUcf2GC2jGsqhXAUBHJAP4NBLyMlarOAGYA5OTkaG5uboNkyMvLo6Fxmwt79pXy87kf0q9dCx64dAwJcZE76CsanidYOSONcC5nk2gLVS0A5gLHABkiUmV8OgI/NIUMkcz0t7+luFR58OzBEW0ADMNofII5OqiN2wJARJKBE4AVOMbgLDfYJcCbwZIhGvjPsi28uWgzp/WIZ0D7lqEWxzCMZkYw3UHtgOfdfoEY4BVVnS0iy4FZInIP8A3wdBBliGh27yvld28sY0D7dE7tXh5qcQzDaIYEzQio6hJgmI/z64BRwco3mrj9zWUUHijjhStGs3Xl16EWxzCMZog5kJsp7yzZwuwlW/j5xF70PSo91OIYhtFMMSPQDNlZfJDb3lzGoA4tufq4HqEWxzCMZowZgWaGqnLbG8soLinnoXOGEBdrj9AwjIZjGqSZMXvJFt5btpVfnNCb3tktQi2OYRjNHDMCzYjtRSXc9uYyhnbK4Mpx3UItjmEYEYAZgWaCqvLbfy9jf2kFD55tbiDDMBoH0yTNhDcXbeaD5du46cTe9Gwb+XOtGIbRNJgRaAZs31vCHW99y/DOGVw+tnuoxTEMI4IwIxDmqCq/+fdSSsocN1BsjIRaJMMwIggzAmHO61//wIcrtnPzSX3o3sbcQIZhNC5mBMKYrYUlTH/7W0Z2bcWlY2w0kGEYjY8ZgTBFVbn19SWUVVTywFnmBjIMIziYEQhTXl24ibxVO7h1cl+6tk4NtTiGYUQoZgTCkM0FB7j77eWM7pbJxcd0DbU4hmFEMGYEwgxV5ZZ/LaFClQfOGkKMuYEMwwgiZgTCjFlf5fPJ6p38+uS+dM5KCbU4hmFEOGYEwohNe/Zz7zsrOLZHFheM7hJqcQzDiAKCucZwJxGZKyLLReRbEfm5e366iPwgIovc7ZRgydCcqHIDqSr3TRlsbiDDMJqEYK4xXA78UlW/FpEWwEIR+cC99oiqPhjEvJsdL375PZ+t2cW9ZwykU6a5gQzDaBqCucbwFmCLu18kIiuADsHKrzmTv3s/v393BWN7tub8UZ1DLY5hGFGEqGrwMxHpCnwMDARuBKYBe4EFOK2FPT7iXAVcBZCdnT1i1qxZDcq7uLiYtLTwnW6hUpX7vyphQ2El945NJiu5YR66cC9nY2HljCysnMFlwoQJC1U1x28gVQ3qBqQBC4Ez3eNsIBanP+Je4Jm60hgxYoQ2lLlz5zY4blPw/Ofrtcsts3XW/I1HlE64l7OxsHJGFlbO4AIs0Dr0a1BHB4lIPPAv4EVVfd01OttUtUJVK4EngVHBlCGc2bhrH394dyXH9W7DOTmdQi2OYRhRiN8+ARHJDCCNSlUt8BFXgKeBFar6sMf5dur0FwCcASwLXNzIobJSufnVJcTFCn+cMgjndhmGYTQtdXUMb3Y3fxoqFvDVmzkGuAhYKiKL3HO/AaaKyFBAgQ3A/wUubuTw3OcbmL9hNw+cNZh2LZNDLY5hGFFKXUZghaoO8xdARL7xdV5VP8W38Xg3QNkilvU793H/+ys5vm9bzhrRMdTiGIYRxdRlBI4JII1AwhguFZXKza8uJiE2hj+caW4go3lRVlbGpk2bKCkpaZT0WrZsyYoVKxolrXAm2OVMSkqiY8eOxMfH1zuuXyOgqiUAItID2KSqB0UkFxgM/ENVC6rCGIHx7GfrWbBxDw+fM4Ts9KRQi2MY9WLTpk20aNGCrl27NkoFpqioiBYtWjSCZOFNMMupquzatYtNmzbRrVv9F58KdHTQv4AKEekJzAA6AS/VO7coZ832Yh54fxWT+mVzxjD7bs5ofpSUlJCVlWUt2DBCRMjKympw6yxQI1CpquU4o3n+oqo3A+0alGOUUlGp3PzaYpITYvn9mQPtT2Q0W+zdDT+O5JkEagTKRGQqcAkw2z1Xf+dTFPPUJ+v45vsC7jxtAG1bmBvIMIzwIFAjcClOB/C9qrpeRLoB/wyeWJHF6m1FPPTBd5w0IJvThrQPtTiG0ayJjY1l6NChDBw4kLPPPpv9+/cfcZrTp0/nwQcbZ07LRx99lKSkJAoLC48ondzcXBYsWNAoMvkjICOgqstV9WeqOtM9Xq+q9wVXtMigvKKSm15dTGpCLPf8xEYDGcaRkpyczKJFi1i2bBkJCQk88cQToRapBjNnzmTkyJG8/vrroRYlIPwaARGZUVcCgYSJZv7+8ToWbyrk7p8MpE2LxFCLYxgRxbhx41izZg1vv/02o0ePZtiwYUyaNIlt27YBTg3/sssuIzc3l+7du/PnP/+5Ou69995L7969GTt2LKtWrao+/+STTzJy5EiGDBnClClTqlsar776KgMHDmTIkCGMHz/epzxr166luLiYe+65h5kzZ1aff/HFFzn99NPJzc2lV69e3HnnnQBs2LCBvn37csEFF9CvXz/OOuusw1o2zzzzDDfccEMN+X7xi18c2Y3zoK7vBH4iIv66nAWY0GjSRBirthbxpw9Xc8qgo/jRYHMDGZHFnW9/y/LNe48ojYqKCmJjY6uP+7dP544fDwgobnl5Oe+99x6TJ09m7NixfPHFF4gITz31FPfffz8PPfQQACtXrmTu3LkUFRXRp08frrnmGpYsWcKsWbNYtGgR5eXlDB8+nBEjRgBw5plncuWVVwLwu9/9jqeffprrr7+eu+66i/fff58OHTpQUFDgU6ZZs2Zx3nnnMW7cOFatWsW2bdvIzs4GYP78+SxbtoyUlBRGjhzJqaeeSuvWrVm1ahVPP/00Y8aM4bLLLuPxxx/npptuqk7znHPO4d577+WBBx4gPj6eZ599lr///e/1vte1UZc76GacGUBr2xYAv200aSKIMtcN1CIpjrtPHxhqcQwjYjhw4ABDhw4lJyeHzp07c/nll7Np0yZOOukkBg0axAMPPMC3335bHf7UU08lMTGR1q1b07ZtW7Zt28Ynn3zCGWecQUpKCunp6Zx22mnV4ZctW8a4ceMYNGgQL774YnVaY8aMYdq0aTz55JNUVFT4lG3mzJmcd955xMTEMGXKFF599dXqayeccAJZWVkkJydz5pln8umnnwLQqVMnxowZA8CFF15Yfb6KtLQ0jj/+eGbPns3KlSspKytj0KBBjXMzqftjsecbLaco44m8tSz9oZC/XTCcrDRzAxmRR6A1dn805COqqj4BT66//npuvPFGTjvtNPLy8pg+fXr1tcTEQ/+/2NhYysvL/aY/bdo03njjDYYMGcJzzz1HXl4eAE888QRffvkl77zzDiNGjGDhwoVkZWVVx1u6dCmrV6/mhBNOAKC0tJRu3bpx3XXXAYcP46w6ru28J1dccQW///3v6du3L5deeqlf+euLLTQfBFZs2cuf56zmx0Pac/Ig+5zCMIJNYWEhHTo4H2A+/3zdddfx48fzxhtvcODAAYqKinj77berrxUVFdGuXTvKysp48cUXq8+vXbuW0aNHc9ddd9GmTRvy8/NrpDlz5kymT5/Ohg0b2LBhA5s3b2bz5s1s3LgRgA8++IDdu3dz4MAB3njjjera//fff8+8efMAeOmllxg7duxh8o4ePZr8/Hxeeuklpk6dWs+74x8zAo1MWUUlv3xlMS2TE7jrtCOvKRmGUTfTp0/n7LPPZsSIEbRu3brO8MOHD+fcc89lyJAhnHzyyYwcObL62t13383o0aMZM2YMffv2rT5/8803M2jQIAYOHMixxx7LkCFDaqQ5a9YszjjjjBrnzjjjDKpWRRw1ahRTpkxh8ODBTJkyhZwcZ8GvPn368Nhjj9GvXz/27NnDNddc41Pmc845hzFjxtCqVavAbkqg1LXqjNZcJSylPuEba2tOK4s98sEq7XLLbP3Psi1Nmq+t0BRZhGs5ly9f3qjp7d27t1HTC1f+9re/6bXXXnvY+fXr1+uAAQMCSuPUU0/VDz/8sNbrvp4NjbWymIgcKyLLgZXu8RARebxxzVHzZ9kPhfx1zhp+MrQ9Jw04KtTiGIYRARQUFNC7d2+Sk5OZOHFio6df1xDRKh4BTgLeAlDVxSLie6BslFJa7owGapWawHRzAxmG4cEFF1zgswO8a9euLFvmf3HFjIwMvvvuu2CJFnifgKrme53yPUYqSvnLnNWs3FrEH84YREZKQqjFMQzDCIhAjUC+iBwLqIjEi8hNgN8VEkSkk4jMFZHlIvKtiPzcPZ8pIh+IyGr3t5F7OZqepZsKeTxvLWcO78Ck/tmhFscwDCNgAjUCVwPXAh2AH4Ch7rE/yoFfqmp/4GjgWhHpD9wKfKSqvYCP3ONmy8HyCn756iJapyVwx4/MDWQYRvMioD4BVd0JXFCfhFV1C7DF3S8SkRU4RuR0INcN9jyQB9xSn7TDiT99uJrvthXz7LSRtEyx2bUNw2heiDOKqI5AztTR1wNd8TAcqnpabXG84ncFPgYGAt+raoZ7XoA9Vcdeca4CrgLIzs4eUTXWtr4UFxeTlpbWoLh1sa6ggru/KGFshzguHxTar4KDWc5wwsoZWlq2bEnPnj0bLT3vuYMCISMjgwEDBlBWVkZcXBxTp07l2muvJSam/p89tWvXji1bttQZbvbs2Zx//vksWLCA3r171zufqnJeffXVTJ48mZ/85Cf1TqMu1qxZc9j01RMmTFioqjn+4gU6OugN4GngbaCyPoKJSBrO8pQ3qOpez0+iVVVFxKcVUtUZOEtZkpOTo7m5ufXJtpq8vDwaGtcfJWUV3POXTzmqZRKPXTme9KTQtgKCVc5ww8oZWlasWNGoa+U2dNqIJUuWALB9+3bOP/98Dh48WD0zZ30JJP833niDsWPH8tZbbzUon6pyxsfHk5ycHJT1hpOSkhg2bFi94wVqOktU9c+qOldV/1e11RVJROJxDMCLqlo1ufY2EWnnXm8HbK+31GHAIx9+x5rtxfxxyuCQGwDDiFbatm3LjBkz+Otf/4qqsmHDBsaNG8fw4cMZPnw4n3/+OQBbtmxh/Pjx1YvRfPLJJzXS2blzJ8cccwzvvPPOYXkUFxfz6aef8vTTT+PpkcjLy2P8+PGceuqp9OnTh6uvvprKSqeOnJaWxi9+8QsGDBjAxIkT2blzZ40058yZU6M18MEHHxz2tXFTEWhL4E8icgfwX+Bg1UlV/bq2CK6r52lghao+7HHpLZxlKv/o/r5ZX6FDzcKNe3jy43VMHdWJ43q3CbU4hhEa3rsVti49oiSSK8oh1kMNHTUITv5jvdLo3r07FRUVbN++nbZt2/LBBx+QlJTE6tWrmTp1KgsWLOCll17ipJNO4re//S0VFRU15uzftm0bp512Gvfcc0/15G+evPnmm0yePJnevXuTlZXFwoULq6ednj9/PsuXL6dLly5MnjyZ119/nbPOOot9+/aRk5PDI488wl133cUf/vAHZsw4tPTKhAkT+OlPf8qOHTto06YNzz77LJdddlk9717jEGhLYBBwJY7ifsjd6lqLbQxwEXC8iCxyt1PcNE4QkdXAJPe42VBSVsHNry6mXctkfnNKv1CLYxiGB2VlZVx55ZUMGjSIs88+m+XLlwMwcuRInn32WaZPn87SpUur3TFlZWVMnDiR+++/36cBgEPTQwOcd955NRaLGTVqFN27dyc2NpapU6dWTwMdExPDueeeCzjTQ3/xxRc10hQRLrroIl544QUKCgqYN28eJ598cuPejAAJtCVwNtBdVUsDTVhVP8VZdMYXjf/tcxPx4PurWLdzHy9cPpoW5gYyopl61th9caABfQLerFu3jtjYWNq2bcudd95JdnY2ixcvprKykqSkJMCZNfTjjz/mnXfeYdq0adx4441cfPHFxMXFMWLECN5//32OO+64w9LevXs3c+bMYenSpYgIFRUViAgPPPAAENg00LWdv/TSS/nxj39MUlISZ599NnFxgarjxiXQlsAyICOIcjQLFmzYzdOfreeC0Z0Z26vumQoNwwguO3bs4Oqrr+a6665DRCgsLKRdu3bExMTwz3/+s3rxl40bN5Kdnc2VV17JFVdcwddfO55sEeGZZ55h5cqV3Hff4cumv/baa1x00UVs3LiRDRs2kJ+fT7du3ar7FObPn8/69euprKzk5Zdfrp4GurKyktdeew1wpoc++uijD0u7ffv2tG/fnnvuuafR1wioD4EagQxgpYi8LyJvVW1BlCvsOFBawU2vLqZDRjK/NjeQYYSMqpXFBgwYwKRJkzjxxBO54447APjpT3/K888/z5AhQ1i5ciWpqamA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\n",
+                        "text/plain": [
+                            "<Figure size 432x288 with 1 Axes>"
+                        ]
+                    },
+                    "metadata": {
+                        "needs_background": "light"
+                    },
+                    "output_type": "display_data"
+                }
+            ],
+            "source": [
+                "fig = plt.figure()\n",
+                "vectorized_comparison.title = \"GroupBy Apply Aggregation Function Speed Comparison\"\n",
+                "vectorized_comparison.xlabel = \"n_rows\"\n",
+                "vectorized_comparison.plot(logx=False, logy=False)\n",
+                "plt.savefig(\"groupby_apply_agg_func_speed_comparison.png\")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 8,
+            "metadata": {
+                "scrolled": true
+            },
+            "outputs": [
+                {
+                    "data": {
+                        "image/png": "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\n",
+                        "text/plain": [
+                            "<Figure size 432x288 with 1 Axes>"
+                        ]
+                    },
+                    "metadata": {
+                        "needs_background": "light"
+                    },
+                    "output_type": "display_data"
+                }
+            ],
+            "source": [
+                "fig = plt.figure()\n",
+                "vectorized_comparison.xlabel = 'log10(n_rows)'\n",
+                "vectorized_comparison.title = 'GroupBy Apply Aggregation Function Speed Comparison [LogLog Plot]'\n",
+                "vectorized_comparison.plot(logx=True, logy=True, time_unit='s')\n",
+                "plt.ylabel(\"Runtime [log10(s)]\")\n",
+                "plt.savefig(\"groupby_apply_agg_func_speed_comparison_loglog.png\")"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "# Groupby Apply text function speed comparison"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 9,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "SIZE = 100000000\n",
+                "data = pd.DataFrame({\n",
+                "    \"groups\": np.random.choice(np.arange(100000), size=SIZE),\n",
+                "    \"first\": np.random.choice([\"JACK\", \"JILL\"], size=SIZE),\n",
+                "    \"last\": np.random.choice([\"SMITH\", \"JOHNSON\"], size=SIZE),\n",
+                "})"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 10,
+            "metadata": {
+                "scrolled": true
+            },
+            "outputs": [
+                {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "  0% 0/10 [00:00<?, ?it/s]\n",
+                        "  0% 0/3 [00:00<?, ?it/s]\u001b[A\n",
+                        " 33% 1/3 [00:00<00:00,  3.45it/s]\u001b[A/tmp/ipykernel_31702/386866890.py:5: UserWarning: `meta` is not specified, inferred from partial data. Please provide `meta` if the result is unexpected.\n",
+                        "  Before: .apply(func)\n",
+                        "  After:  .apply(func, meta={'x': 'f8', 'y': 'f8'}) for dataframe result\n",
+                        "  or:     .apply(func, meta=('x', 'f8'))            for series result\n",
+                        "  lambda df: dd.from_pandas(df, npartitions=npartitions).groupby(\"groups\").apply(join_text_func).compute(scheduler=\"processes\").sort_values(ascending=False),\n",
+                        "\n",
+                        " 67% 2/3 [00:01<00:00,  1.11it/s]\u001b[A\n",
+                        "100% 3/3 [00:02<00:00,  1.39it/s]\u001b[A\n",
+                        " 10% 1/10 [00:02<00:19,  2.13s/it][A\n",
+                        "  0% 0/3 [00:00<?, ?it/s]\u001b[A\n",
+                        " 33% 1/3 [00:00<00:01,  1.66it/s]\u001b[A/tmp/ipykernel_31702/386866890.py:5: UserWarning: `meta` is not specified, inferred from partial data. Please provide `meta` if the result is unexpected.\n",
+                        "  Before: .apply(func)\n",
+                        "  After:  .apply(func, meta={'x': 'f8', 'y': 'f8'}) for dataframe result\n",
+                        "  or:     .apply(func, meta=('x', 'f8'))            for series result\n",
+                        "  lambda df: dd.from_pandas(df, npartitions=npartitions).groupby(\"groups\").apply(join_text_func).compute(scheduler=\"processes\").sort_values(ascending=False),\n",
+                        "\n",
+                        " 67% 2/3 [00:01<00:01,  1.03s/it]\u001b[A\n",
+                        "100% 3/3 [00:02<00:00,  1.21it/s]\u001b[A\n",
+                        " 20% 2/10 [00:04<00:18,  2.36s/it][A\n",
+                        "  0% 0/3 [00:00<?, ?it/s]\u001b[A\n",
+                        " 33% 1/3 [00:00<00:01,  1.39it/s]\u001b[A/tmp/ipykernel_31702/386866890.py:5: UserWarning: `meta` is not specified, inferred from partial data. Please provide `meta` if the result is unexpected.\n",
+                        "  Before: .apply(func)\n",
+                        "  After:  .apply(func, meta={'x': 'f8', 'y': 'f8'}) for dataframe result\n",
+                        "  or:     .apply(func, meta=('x', 'f8'))            for series result\n",
+                        "  lambda df: dd.from_pandas(df, npartitions=npartitions).groupby(\"groups\").apply(join_text_func).compute(scheduler=\"processes\").sort_values(ascending=False),\n",
+                        "\n",
+                        " 67% 2/3 [00:02<00:01,  1.22s/it]\u001b[A\n",
+                        "100% 3/3 [00:02<00:00,  1.06it/s]\u001b[A\n",
+                        " 30% 3/10 [00:07<00:18,  2.62s/it][A\n",
+                        "  0% 0/3 [00:00<?, ?it/s]\u001b[A\n",
+                        " 33% 1/3 [00:00<00:01,  1.12it/s]\u001b[A/tmp/ipykernel_31702/386866890.py:5: UserWarning: `meta` is not specified, inferred from partial data. Please provide `meta` if the result is unexpected.\n",
+                        "  Before: .apply(func)\n",
+                        "  After:  .apply(func, meta={'x': 'f8', 'y': 'f8'}) for dataframe result\n",
+                        "  or:     .apply(func, meta=('x', 'f8'))            for series result\n",
+                        "  lambda df: dd.from_pandas(df, npartitions=npartitions).groupby(\"groups\").apply(join_text_func).compute(scheduler=\"processes\").sort_values(ascending=False),\n",
+                        "\n",
+                        " 67% 2/3 [00:02<00:01,  1.56s/it]\u001b[A\n",
+                        "100% 3/3 [00:03<00:00,  1.17s/it]\u001b[A\n",
+                        " 40% 4/10 [00:11<00:18,  3.02s/it][A\n",
+                        "  0% 0/3 [00:00<?, ?it/s]\u001b[A\n",
+                        " 33% 1/3 [00:00<00:01,  1.06it/s]\u001b[A/tmp/ipykernel_31702/386866890.py:5: UserWarning: `meta` is not specified, inferred from partial data. Please provide `meta` if the result is unexpected.\n",
+                        "  Before: .apply(func)\n",
+                        "  After:  .apply(func, meta={'x': 'f8', 'y': 'f8'}) for dataframe result\n",
+                        "  or:     .apply(func, meta=('x', 'f8'))            for series result\n",
+                        "  lambda df: dd.from_pandas(df, npartitions=npartitions).groupby(\"groups\").apply(join_text_func).compute(scheduler=\"processes\").sort_values(ascending=False),\n",
+                        "\n",
+                        " 67% 2/3 [00:03<00:01,  1.70s/it]\u001b[A\n",
+                        "100% 3/3 [00:04<00:00,  1.32s/it]\u001b[A\n",
+                        " 50% 5/10 [00:15<00:16,  3.40s/it][A\n",
+                        "  0% 0/3 [00:00<?, ?it/s]\u001b[A\n",
+                        " 33% 1/3 [00:00<00:01,  1.01it/s]\u001b[A/tmp/ipykernel_31702/386866890.py:5: UserWarning: `meta` is not specified, inferred from partial data. Please provide `meta` if the result is unexpected.\n",
+                        "  Before: .apply(func)\n",
+                        "  After:  .apply(func, meta={'x': 'f8', 'y': 'f8'}) for dataframe result\n",
+                        "  or:     .apply(func, meta=('x', 'f8'))            for series result\n",
+                        "  lambda df: dd.from_pandas(df, npartitions=npartitions).groupby(\"groups\").apply(join_text_func).compute(scheduler=\"processes\").sort_values(ascending=False),\n",
+                        "\n",
+                        " 67% 2/3 [00:03<00:02,  2.11s/it]\u001b[A\n",
+                        "100% 3/3 [00:04<00:00,  1.55s/it]\u001b[A\n",
+                        " 60% 6/10 [00:20<00:15,  3.86s/it][A\n",
+                        "  0% 0/3 [00:00<?, ?it/s]\u001b[A\n",
+                        " 33% 1/3 [00:00<00:01,  1.03it/s]\u001b[A/tmp/ipykernel_31702/386866890.py:5: UserWarning: `meta` is not specified, inferred from partial data. Please provide `meta` if the result is unexpected.\n",
+                        "  Before: .apply(func)\n",
+                        "  After:  .apply(func, meta={'x': 'f8', 'y': 'f8'}) for dataframe result\n",
+                        "  or:     .apply(func, meta=('x', 'f8'))            for series result\n",
+                        "  lambda df: dd.from_pandas(df, npartitions=npartitions).groupby(\"groups\").apply(join_text_func).compute(scheduler=\"processes\").sort_values(ascending=False),\n",
+                        "\n",
+                        " 67% 2/3 [00:04<00:02,  2.51s/it]\u001b[A\n",
+                        "100% 3/3 [00:05<00:00,  1.82s/it]\u001b[A\n",
+                        " 70% 7/10 [00:25<00:13,  4.42s/it][A\n",
+                        "  0% 0/3 [00:00<?, ?it/s]\u001b[A\n",
+                        " 33% 1/3 [00:01<00:03,  1.89s/it]\u001b[A/tmp/ipykernel_31702/386866890.py:5: UserWarning: `meta` is not specified, inferred from partial data. Please provide `meta` if the result is unexpected.\n",
+                        "  Before: .apply(func)\n",
+                        "  After:  .apply(func, meta={'x': 'f8', 'y': 'f8'}) for dataframe result\n",
+                        "  or:     .apply(func, meta=('x', 'f8'))            for series result\n",
+                        "  lambda df: dd.from_pandas(df, npartitions=npartitions).groupby(\"groups\").apply(join_text_func).compute(scheduler=\"processes\").sort_values(ascending=False),\n",
+                        "\n",
+                        " 67% 2/3 [00:05<00:03,  3.02s/it]\u001b[A\n",
+                        "100% 3/3 [00:06<00:00,  1.88s/it]\u001b[A\n",
+                        " 80% 8/10 [00:31<00:09,  5.00s/it][A\n",
+                        "  0% 0/3 [00:00<?, ?it/s]\u001b[A\n",
+                        " 33% 1/3 [00:05<00:11,  5.91s/it]\u001b[A/tmp/ipykernel_31702/386866890.py:5: UserWarning: `meta` is not specified, inferred from partial data. Please provide `meta` if the result is unexpected.\n",
+                        "  Before: .apply(func)\n",
+                        "  After:  .apply(func, meta={'x': 'f8', 'y': 'f8'}) for dataframe result\n",
+                        "  or:     .apply(func, meta=('x', 'f8'))            for series result\n",
+                        "  lambda df: dd.from_pandas(df, npartitions=npartitions).groupby(\"groups\").apply(join_text_func).compute(scheduler=\"processes\").sort_values(ascending=False),\n",
+                        "\n",
+                        " 67% 2/3 [00:10<00:05,  5.12s/it]\u001b[A\n",
+                        "100% 3/3 [00:11<00:00,  3.47s/it]\u001b[A\n",
+                        " 90% 9/10 [00:43<00:07,  7.19s/it][A\n",
+                        "  0% 0/3 [00:00<?, ?it/s]\u001b[A\n",
+                        " 33% 1/3 [00:11<00:22, 11.32s/it]\u001b[A/tmp/ipykernel_31702/386866890.py:5: UserWarning: `meta` is not specified, inferred from partial data. Please provide `meta` if the result is unexpected.\n",
+                        "  Before: .apply(func)\n",
+                        "  After:  .apply(func, meta={'x': 'f8', 'y': 'f8'}) for dataframe result\n",
+                        "  or:     .apply(func, meta=('x', 'f8'))            for series result\n",
+                        "  lambda df: dd.from_pandas(df, npartitions=npartitions).groupby(\"groups\").apply(join_text_func).compute(scheduler=\"processes\").sort_values(ascending=False),\n",
+                        "\n",
+                        " 67% 2/3 [00:17<00:08,  8.12s/it]\u001b[A\n",
+                        "100% 3/3 [00:22<00:00,  7.39s/it]\u001b[A\n",
+                        "100% 10/10 [01:06<00:00,  6.60s/it]\n"
+                    ]
+                }
+            ],
+            "source": [
+                "vectorized_comparison = perfplot.bench(\n",
+                "    setup=lambda n: data.iloc[:n],\n",
+                "    kernels=[\n",
+                "        lambda df: df.groupby(\"groups\").apply(join_text_func),\n",
+                "        lambda df: dd.from_pandas(df, npartitions=npartitions).groupby(\"groups\").apply(join_text_func).compute(scheduler=\"processes\").sort_values(ascending=False),\n",
+                "        lambda df: df.swifter.progress_bar(False).groupby(\"groups\").apply(join_text_func),\n",
+                "    ],\n",
+                "    labels=['Pandas Apply', 'Dask Apply', 'Swifter Apply'],\n",
+                "    n_range=[2**k for k in range(0, 20, 2)],\n",
+                "    xlabel='n_rows',\n",
+                "    equality_check=None\n",
+                ")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 11,
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "image/png": "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UqpfrdWXA4nm79eBJOBeR9ngaKpn4Kruznnttddyzz33AHDrrbcyb9483njjDWbOnElAQABgNMRWT10YGBhYw63i6enJmjVruOyyywgKCuLWW2+1bVuzZg333lvzVM2bN481a9Ywf/58xo8fz+23387evXuZNm2arYE2ICCAjRs38thjj9GzZ0/efvvtOsuyaNEijh49yvDhw1v1HAmCo3CVuDnOQBmROx2UuCH8n9i5egq11sHmbwWcqF6u49jlwHKA0NDQaPteLABdunRh0KBBjdrQ3Dl3OxIbNmzgr3/9q61mb094eDg5OTmNpvGrX/2KsWPHsmTJkhbbs3fvXoqKilqcTl2UlJQQGBjokLTbE1LO+jlYVMW3WZWkHKmkwgqDgj04v683MaGe+Hi2T9+9s67ntGnT0rXWMbXXO82Zq7XWSql6/3W01iuBlQAxMTE6MTGxxvadO3c2yXfvyKkX2wv+/v4opeotZ2Plj46OJiAggOeff77G9JDNxdfXl3HjxrU4nbpISkqi9r3gikg5a1Izbs4p/Lw9mRfTp8PEzWlv17OthT9PKRWutc5RSoUD+W2cv0uSmJho691Tm6aMBk5PT29tkwShVXCHuDnOoK2F/z/AdcCT5vdHbZy/IAjtHHeLm+MMHNmdcw1GQ26IUiobeBhD8N9RSt0AHAKudlT+giB0LNw1bo4zcGSvnoX1bJI5+wRBAIyumOmHjrt13BxnICN1BEFoc06druSjjCP8/Ydysr5IJqiTF9fE9WVxfF8G9XTtzhjtAfk7bQGPP/44I0eOZMyYMURFRZGamtqk4x566CG+/vprwOiKOXLkSKKiokhOTuazzz5rFds+/PBDlFLs2rWrReksXbq0zm6igtAc9uQV8/BH24n/wzfc/+9tKOCJK0aT+vvprLhspIh+GyE1/maSnJzMJ598wubNm+nUqRPHjh2joqKiScc++uijtt9vvvkm9913H4sXL+a1114jLS2NSy65pMl2VFZW1hliQcI3C+2FhuLmnNyfwbQJfZ1totshNf5mkpOTQ0hIiK3fe0hICL169WLTpk22QGgfffQRfn5+VFRUUF5ebguiVl2Lfumll3jnnXd48MEHWbhwIQ899BBvv/02UVFRvP3225w6dYply5YxYcIExo0bx0cfGZ2gXnvtNS677DLOP/98pk8/u8mkofDNCQkJ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\n",
+                        "text/plain": [
+                            "<Figure size 432x288 with 1 Axes>"
+                        ]
+                    },
+                    "metadata": {
+                        "needs_background": "light"
+                    },
+                    "output_type": "display_data"
+                }
+            ],
+            "source": [
+                "fig = plt.figure()\n",
+                "vectorized_comparison.title = \"GroupBy Apply Text Function Speed Comparison\"\n",
+                "vectorized_comparison.xlabel = \"n_rows\"\n",
+                "vectorized_comparison.plot(logx=False, logy=False)\n",
+                "plt.savefig(\"groupby_apply_text_func_speed_comparison.png\")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 12,
+            "metadata": {
+                "scrolled": true
+            },
+            "outputs": [
+                {
+                    "data": {
+                        "image/png": "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b71FUFAQ8fHxpdpOVFQUK1euLJOYXEmTjipzmdmZTF03laHzhnLg1CGqxI9i09prGHVxG74fdwmt6rplVAylAKhUqRJr1qxh/fr1VKhQgQ8+yHdILo+Jjo6ma9euzJ4929OhuIUmHVWmdsbvZMRPI3h79ds0qNiFI5vuITupLV+O6saEq1vrvTfKo3r06MH27duZO3cu3bp1o2PHjvTp04cjR44AVg3mtttuIyoqiiZNmvDOO6eH8nrhhRdo3rw53bt3Z8uWLbnzP/roI7p27Ur79u0ZNGhQbk3qm2++oW3btrRv356ePXvmG8+OHTtITEzk+eefJzo6Onf+9OnTufbaa4mKiqJZs2Y888wzAOzevZuWLVty44030qpVKwYPHnxWzW3atGncf//9Z8T3wAMPlO6FK0M+dU1HGxJ4TlZ2Fl9s+oJ3Vr9DRf8g6qSOYu2mpvRvX0+bQisAnpm7gY0HE4pcLysrC39/536ctK5XhaevaePUupmZmfz000/069eP7t278/fffyMiTJ06lVdffZVJkyYBsHnzZhYtWsSpU6do0aIFd955J2vXrmXmzJmsWbOGzMxMOnXqROfOnQG47rrrGD3auow8YcIEPv74Y+655x6effZZFixYQP369YmLi8s3ppkzZzJs2DB69OjBli1bOHLkCOHh1ii4y5cvZ/369QQHB9O1a1euuuoqatasyZYtW/j444+55JJLuO2223j//fd58MEHc7d5/fXX88ILL/Daa68RGBjIJ598wocffujUa+QOPlXT0W5wPGNPwh5uXXArr698nYiQTsRvu4/Dh1ry9rAOvDO8oyYc5VEpKSl06NCBLl260KhRI26//Xb2799P3759adeuHa+99hobNpweXeWqq66iYsWK1KxZk9q1a3PkyBGWLFnCwIEDCQ4OpkqVKvTv3z93/fXr19OjRw/atWvHjBkzcrd1ySWXMHLkSD766COysrLyjS06Opphw4bh5+fHoEGD+Oabb3KXXX755dSoUYNKlSpx3XXXsXTpUgAaNmzIJZdcAsBNN92UOz9HaGgol112GfPmzWPz5s1kZGTQrl27snkxy4BP1XSUe2WbbKI3R/PWqrcI8AukKaNZtbwJFzapwaTrO2hTaHUGZ2skZX3zZM41HUf33HMP48ePp3///sTExDBx4sTcZRUrVsx97O/vT2ZmZqHb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\n",
+                        "text/plain": [
+                            "<Figure size 432x288 with 1 Axes>"
+                        ]
+                    },
+                    "metadata": {
+                        "needs_background": "light"
+                    },
+                    "output_type": "display_data"
+                }
+            ],
+            "source": [
+                "fig = plt.figure()\n",
+                "vectorized_comparison.xlabel = 'log10(n_rows)'\n",
+                "vectorized_comparison.title = 'GroupBy Apply Text Function Speed Comparison [LogLog Plot]'\n",
+                "vectorized_comparison.plot(logx=True, logy=True, time_unit='s')\n",
+                "plt.ylabel(\"Runtime [log10(s)]\")\n",
+                "plt.savefig(\"groupby_apply_text_func_speed_comparison_loglog.png\")"
+            ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
@@ -899,15 +1361,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.2"
+            "version": "3.9.13"
         },
         "toc": {
             "base_numbering": 1,
             "nav_menu": {},
             "number_sections": true,
             "sideBar": true,
             "skip_h1_title": false,
```

### Comparing `swifter-1.3.4/setup.py` & `swifter-1.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup
 
 setup(
     name="swifter",
     packages=["swifter"],  # this must be the same as the name above
-    version="1.3.4",
+    version="1.3.5",
     description="A package which efficiently applies any function to a pandas dataframe or series in the fastest available manner",
     author="Jason Carpenter",
     author_email="jcarpenter@manifold.ai",
     url="https://github.com/jmcarpenter2/swifter",  # use the URL to the github repo
-    download_url=f"https://github.com/jmcarpenter2/swifter/archive/1.3.4.tar.gz",
+    download_url=f"https://github.com/jmcarpenter2/swifter/archive/1.3.5.tar.gz",
     keywords=["pandas", "dask", "apply", "function", "parallelize", "vectorize"],
     install_requires=[
         "pandas>=1.0.0",
         "psutil>=5.6.6",
         "dask[dataframe]>=2.10.0",
         "tqdm>=4.33.0",
         "ipywidgets>=7.0.0",
```

### Comparing `swifter-1.3.4/swifter/__init__.py` & `swifter-1.3.5/swifter/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,8 +18,8 @@
     "set_defaults",
     "SeriesAccessor",
     "DataFrameAccessor",
     "register_parallel_dataframe_accessor",
     "register_parallel_series_accessor",
     "register_modin",
 ]
-__version__ = "1.3.4"
+__version__ = "1.3.5"
```

### Comparing `swifter-1.3.4/swifter/base.py` & `swifter-1.3.5/swifter/base.py`

 * *Files identical despite different names*

### Comparing `swifter-1.3.4/swifter/parallel_accessor.py` & `swifter-1.3.5/swifter/parallel_accessor.py`

 * *Files identical despite different names*

### Comparing `swifter-1.3.4/swifter/swifter.py` & `swifter-1.3.5/swifter/swifter.py`

 * *Files 10% similar despite different names*

```diff
@@ -224,80 +224,81 @@
     def _wrapped_apply(self, func, convert_dtype=True, args=(), **kwds):
         def wrapped():
             with suppress_stdout_stderr_logging():
                 self._obj.iloc[self._SAMPLE_INDEX].apply(func, convert_dtype=convert_dtype, args=args, **kwds)
 
         return wrapped
 
-    def _dask_apply(self, func, convert_dtype, *args, **kwds):
+    def _pandas_apply(self, df, func, convert_dtype, *args, **kwds):
+        if self._progress_bar:
+            tqdm.pandas(desc=self._progress_bar_desc or "Pandas Apply")
+            return df.progress_apply(func, convert_dtype=convert_dtype, args=args, **kwds)
+        else:
+            return df.apply(func, convert_dtype=convert_dtype, args=args, **kwds)
+
+    def _dask_map_partitions(self, df, func, meta, *args, **kwds):
+        return (
+            dd.from_pandas(df, npartitions=self._npartitions)
+            .map_partitions(func, *args, meta=meta, **kwds)
+            .compute(scheduler=self._scheduler)
+        )
+
+    def _dask_apply(self, df, func, convert_dtype, meta, *args, **kwds):
+        return (
+            dd.from_pandas(df, npartitions=self._npartitions)
+            .apply(
+                lambda x: func(x, *args, **kwds),
+                convert_dtype=convert_dtype,
+                meta=meta,
+            )
+            .compute(scheduler=self._scheduler)
+        )
+
+    def _parallel_apply(self, func, convert_dtype, *args, **kwds):
         sample = self._obj.iloc[self._SAMPLE_INDEX]
         with suppress_stdout_stderr_logging():
             meta = sample.apply(func, convert_dtype=convert_dtype, args=args, **kwds)
         try:
             # check that the dask map partitions matches the pandas apply
             with suppress_stdout_stderr_logging():
-                tmp_df = (
-                    dd.from_pandas(sample, npartitions=self._npartitions)
-                    .map_partitions(func, *args, meta=meta, **kwds)
-                    .compute(scheduler=self._scheduler)
-                )
+                tmp_df = self._dask_map_partitions(sample, func, meta, *args, **kwds)
                 self._validate_apply(
                     tmp_df.equals(meta),
                     error_message=("Dask map-partitions sample does not match pandas apply sample."),
                 )
             if self._progress_bar:
                 with TQDMDaskProgressBar(desc=self._progress_bar_desc or "Dask Apply"):
-                    return (
-                        dd.from_pandas(self._obj, npartitions=self._npartitions)
-                        .map_partitions(func, *args, meta=meta, **kwds)
-                        .compute(scheduler=self._scheduler)
-                    )
+                    return self._dask_map_partitions(self._obj, func, meta, *args, **kwds)
             else:
-                return (
-                    dd.from_pandas(self._obj, npartitions=self._npartitions)
-                    .map_partitions(func, *args, meta=meta, **kwds)
-                    .compute(scheduler=self._scheduler)
-                )
+                return self._dask_map_partitions(self._obj, func, meta, *args, **kwds)
         except ERRORS_TO_HANDLE:
             # if map partitions doesn't match pandas apply,
             # we can use dask apply, but it will be a bit slower
-            if self._progress_bar:
-                with TQDMDaskProgressBar(desc=self._progress_bar_desc or "Dask Apply"):
-                    return (
-                        dd.from_pandas(self._obj, npartitions=self._npartitions)
-                        .apply(
-                            lambda x: func(x, *args, **kwds),
-                            convert_dtype=convert_dtype,
-                            meta=meta,
-                        )
-                        .compute(scheduler=self._scheduler)
-                    )
-            else:
-                return (
-                    dd.from_pandas(self._obj, npartitions=self._npartitions)
-                    .apply(
-                        lambda x: func(x, *args, **kwds),
-                        convert_dtype=convert_dtype,
-                        meta=meta,
-                    )
-                    .compute(scheduler=self._scheduler)
-                )
+            try:
+                if self._progress_bar:
+                    with TQDMDaskProgressBar(desc=self._progress_bar_desc or "Dask Apply"):
+                        return self._dask_apply(self._obj, func, convert_dtype, meta, *args, **kwds)
+                else:
+                    return self._dask_apply(self._obj, func, convert_dtype, meta, *args, **kwds)
+            except ERRORS_TO_HANDLE:
+                # Second fallback to pandas if dask apply fails
+                return self._pandas_apply(self._obj, func, convert_dtype, *args, **kwds)
 
     def apply(self, func, convert_dtype=True, args=(), **kwds):
         """
         Apply the function to the Series using swifter
         """
 
         # if the series is empty, return early using Pandas
         if not self._nrows:
             return self._obj.apply(func, convert_dtype=convert_dtype, args=args, **kwds)
 
         # If parallel processing is forced by the user, then skip the logic and apply dask
         if self._force_parallel:
-            return self._dask_apply(func, convert_dtype, *args, **kwds)
+            return self._parallel_apply(func, convert_dtype, *args, **kwds)
 
         sample = self._obj.iloc[self._SAMPLE_INDEX]
         # check if input is string or
         # if the user is overriding the string processing default
         allow_dask_processing = True if self._allow_dask_on_strings else (sample.dtype != "object")
 
         if "axis" in kwds.keys():
@@ -318,35 +319,55 @@
             timed = timeit.timeit(wrapped, number=N_REPEATS)
             sample_proc_est = timed / N_REPEATS
             est_apply_duration = sample_proc_est / self._SAMPLE_SIZE * self._nrows
 
             # if pandas sample apply takes too long and not performing str processing
             # then use dask
             if (est_apply_duration > self._dask_threshold) and allow_dask_processing:
-                return self._dask_apply(func, convert_dtype, *args, **kwds)
+                return self._parallel_apply(func, convert_dtype, *args, **kwds)
             else:  # use pandas
-                if self._progress_bar:
-                    tqdm.pandas(desc=self._progress_bar_desc or "Pandas Apply")
-                    return self._obj.progress_apply(func, convert_dtype=convert_dtype, args=args, **kwds)
-                else:
-                    return self._obj.apply(func, convert_dtype=convert_dtype, args=args, **kwds)
+                return self._pandas_apply(self._obj, func, convert_dtype, *args, **kwds)
 
 
 @pd.api.extensions.register_dataframe_accessor("swifter")
 class DataFrameAccessor(_SwifterObject):
     def _wrapped_apply(self, func, axis=0, raw=None, result_type=None, args=(), **kwds):
         def wrapped():
             with suppress_stdout_stderr_logging():
                 self._obj.iloc[self._SAMPLE_INDEX].apply(
                     func, axis=axis, raw=raw, result_type=result_type, args=args, **kwds
                 )
 
         return wrapped
 
-    def _dask_apply(self, func, axis=0, raw=None, result_type=None, *args, **kwds):
+    def _pandas_apply(self, df, func, axis, raw, result_type, *args, **kwds):
+        if self._progress_bar:
+            tqdm.pandas(desc=self._progress_bar_desc or "Pandas Apply")
+            apply_func = df.progress_apply
+        else:
+            apply_func = df.apply
+
+        return apply_func(func, axis=axis, raw=raw, result_type=result_type, args=args, **kwds)
+
+    def _dask_apply(self, df, func, axis, raw, result_type, meta, *args, **kwds):
+        return (
+            dd.from_pandas(df, npartitions=self._npartitions)
+            .apply(
+                func,
+                *args,
+                axis=axis,
+                raw=raw,
+                result_type=result_type,
+                meta=meta,
+                **kwds,
+            )
+            .compute(scheduler=self._scheduler)
+        )
+
+    def _parallel_apply(self, func, axis=0, raw=None, result_type=None, *args, **kwds):
         sample = self._obj.iloc[self._SAMPLE_INDEX]
         with suppress_stdout_stderr_logging():
             meta = sample.apply(func, axis=axis, raw=raw, result_type=result_type, args=args, **kwds)
         try:
             with suppress_stdout_stderr_logging():
                 # check that the dask apply matches the pandas apply
                 tmp_df = (
@@ -364,62 +385,32 @@
                 )
                 self._validate_apply(
                     tmp_df.equals(meta),
                     error_message="Dask apply sample does not match pandas apply sample.",
                 )
             if self._progress_bar:
                 with TQDMDaskProgressBar(desc=self._progress_bar_desc or "Dask Apply"):
-                    return (
-                        dd.from_pandas(self._obj, npartitions=self._npartitions)
-                        .apply(
-                            func,
-                            *args,
-                            axis=axis,
-                            raw=raw,
-                            result_type=result_type,
-                            meta=meta,
-                            **kwds,
-                        )
-                        .compute(scheduler=self._scheduler)
-                    )
+                    return self._dask_apply(self._obj, func, axis, raw, result_type, meta, *args, **kwds)
             else:
-                return (
-                    dd.from_pandas(self._obj, npartitions=self._npartitions)
-                    .apply(
-                        func,
-                        *args,
-                        axis=axis,
-                        raw=raw,
-                        result_type=result_type,
-                        meta=meta,
-                        **kwds,
-                    )
-                    .compute(scheduler=self._scheduler)
-                )
+                return self._dask_apply(self._obj, func, axis, raw, result_type, meta, *args, **kwds)
         except ERRORS_TO_HANDLE:
             # if dask apply doesn't match pandas apply, fallback to pandas
-            if self._progress_bar:
-                tqdm.pandas(desc=self._progress_bar_desc or "Pandas Apply")
-                apply_func = self._obj.progress_apply
-            else:
-                apply_func = self._obj.apply
-
-            return apply_func(func, axis=axis, raw=raw, result_type=result_type, args=args, **kwds)
+            return self._pandas_apply(self._obj, func, axis, raw, result_type, *args, **kwds)
 
     def apply(self, func, axis=0, raw=False, result_type=None, args=(), **kwds):
         """
         Apply the function to the DataFrame using swifter
         """
         # If there are no rows return early using Pandas
         if not self._nrows:
             return self._obj.apply(func, axis=axis, raw=raw, result_type=result_type, args=args, **kwds)
 
         # If parallel processing is forced by the user, then skip the logic and apply dask
         if self._force_parallel:
-            return self._dask_apply(func, axis, raw, result_type, *args, **kwds)
+            return self._parallel_apply(func, axis, raw, result_type, *args, **kwds)
 
         sample = self._obj.iloc[self._SAMPLE_INDEX]
         # check if input is string
         # or if the user is overriding the string processing default
         allow_dask_processing = True if self._allow_dask_on_strings else ("object" not in sample.dtypes.values)
 
         try:  # try to vectorize
@@ -436,82 +427,74 @@
             timed = timeit.timeit(wrapped, number=N_REPEATS)
             sample_proc_est = timed / N_REPEATS
             est_apply_duration = sample_proc_est / self._SAMPLE_SIZE * self._nrows
 
             # if pandas sample apply takes too long
             # and not performing str processing, use dask
             if (est_apply_duration > self._dask_threshold) and allow_dask_processing and axis == 1:
-                return self._dask_apply(func, axis, raw, result_type, *args, **kwds)
+                return self._parallel_apply(func, axis, raw, result_type, *args, **kwds)
             else:  # use pandas
-                if self._progress_bar:
-                    tqdm.pandas(desc=self._progress_bar_desc or "Pandas Apply")
-                    apply_func = self._obj.progress_apply
-                else:
-                    apply_func = self._obj.apply
-
-                return apply_func(func, axis=axis, raw=raw, result_type=result_type, args=args, **kwds)
+                return self._pandas_apply(self._obj, func, axis, raw, result_type, *args, **kwds)
 
     def _wrapped_applymap(self, func):
         def wrapped():
             with suppress_stdout_stderr_logging():
                 self._obj.iloc[self._SAMPLE_INDEX].applymap(func)
 
         return wrapped
 
-    def _dask_applymap(self, func):
+    def _pandas_applymap(self, df, func):
+        if self._progress_bar:
+            tqdm.pandas(desc=self._progress_bar_desc or "Pandas Apply")
+            applymap_func = df.progress_applymap
+        else:
+            applymap_func = df.applymap
+
+        return applymap_func(func)
+
+    def _dask_applymap(self, df, func, meta):
+        return (
+            dd.from_pandas(df, npartitions=self._npartitions)
+            .applymap(func, meta=meta)
+            .compute(scheduler=self._scheduler)
+        )
+
+    def _parallel_applymap(self, func):
         sample = self._obj.iloc[self._SAMPLE_INDEX]
         with suppress_stdout_stderr_logging():
             meta = sample.applymap(func)
         try:
             with suppress_stdout_stderr_logging():
                 # check that the dask apply matches the pandas apply
-                tmp_df = (
-                    dd.from_pandas(sample, npartitions=self._npartitions)
-                    .applymap(func, meta=meta)
-                    .compute(scheduler=self._scheduler)
-                )
+                tmp_df = self._dask_applymap(sample, func, meta)
                 self._validate_apply(
                     tmp_df.equals(meta),
                     error_message=("Dask applymap sample does not match pandas applymap sample."),
                 )
             if self._progress_bar:
                 with TQDMDaskProgressBar(desc=self._progress_bar_desc or "Dask Applymap"):
-                    return (
-                        dd.from_pandas(self._obj, npartitions=self._npartitions)
-                        .applymap(func, meta=meta)
-                        .compute(scheduler=self._scheduler)
-                    )
+                    return self._dask_applymap(self._obj, func, meta)
             else:
-                return (
-                    dd.from_pandas(self._obj, npartitions=self._npartitions)
-                    .applymap(func, meta=meta)
-                    .compute(scheduler=self._scheduler)
-                )
+                return self._dask_applymap(self._obj, func, meta)
         except ERRORS_TO_HANDLE:
             # if dask apply doesn't match pandas apply, fallback to pandas
-            if self._progress_bar:
-                tqdm.pandas(desc=self._progress_bar_desc or "Pandas Apply")
-                applymap_func = self._obj.progress_applymap
-            else:
-                applymap_func = self._obj.applymap
-
-            return applymap_func(func)
+            return self._pandas_applymap(self._obj, func)
 
     def applymap(self, func):
         """
         Applymap the function to the DataFrame using swifter
         """
 
         # If there are no rows return early using Pandas
         if not self._nrows:
             return self._obj.applymap(func)
 
         # If parallel processing is forced by the user, then skip the logic and apply dask
         if self._force_parallel:
-            return self._dask_applymap(func)
+            return self._parallel_applymap(func)
 
         sample = self._obj.iloc[self._SAMPLE_INDEX]
         # check if input is string
         # or if the user is overriding the string processing default
         allow_dask_processing = True if self._allow_dask_on_strings else ("object" not in sample.dtypes.values)
 
         try:  # try to vectorize
@@ -528,23 +511,17 @@
             timed = timeit.timeit(wrapped, number=N_REPEATS)
             sample_proc_est = timed / N_REPEATS
             est_apply_duration = sample_proc_est / self._SAMPLE_SIZE * self._nrows
 
             # if pandas sample apply takes too long
             # and not performing str processing, use dask
             if (est_apply_duration > self._dask_threshold) and allow_dask_processing:
-                return self._dask_applymap(func)
+                return self._parallel_applymap(func)
             else:  # use pandas
-                if self._progress_bar:
-                    tqdm.pandas(desc=self._progress_bar_desc or "Pandas Apply")
-                    applymap_func = self._obj.progress_applymap
-                else:
-                    applymap_func = self._obj.applymap
-
-                return applymap_func(func)
+                return self._pandas_applymap(self._obj, func)
 
     def groupby(
         self, by=None, axis=0, level=None, as_index=True, sort=True, group_keys=True, observed=False, dropna=True
     ):
         """
         Create a swifter groupby object
         """
@@ -692,39 +669,39 @@
         def wrapped():
             with suppress_stdout_stderr_logging():
                 self._sample_pd.apply(func, *args, **kwds)
 
         return wrapped
 
     @abstractmethod
-    def _dask_apply(self, func, *args, **kwds):
-        raise NotImplementedError("Transformation class does not implement _dask_apply")
+    def _parallel_apply(self, func, *args, **kwds):
+        raise NotImplementedError("Transformation class does not implement _parallel_apply")
 
     def apply(self, func, *args, **kwds):
         """
         Apply the function to the transformed swifter object
         """
         # if the transformed dataframe is empty, return early using Pandas
         if not self._nrows:
             return self._obj_pd.apply(func, *args, **kwds)
 
         # If parallel processing is forced by the user, then skip the logic and apply dask
         if self._force_parallel:
-            return self._dask_apply(func, *args, **kwds)
+            return self._parallel_apply(func, *args, **kwds)
 
         # estimate time to pandas apply
         wrapped = self._wrapped_apply(func, *args, **kwds)
         timed = timeit.timeit(wrapped, number=N_REPEATS)
         sample_proc_est = timed / N_REPEATS
         est_apply_duration = sample_proc_est / self._SAMPLE_SIZE * self._nrows
 
         # No `allow_dask_processing` variable here,
         # because we don't know the dtypes of the transformation
         if est_apply_duration > self._dask_threshold:
-            return self._dask_apply(func, *args, **kwds)
+            return self._parallel_apply(func, *args, **kwds)
         else:  # use pandas
             if self._progress_bar and hasattr(self._obj_pd, "progress_apply"):
                 tqdm.pandas(desc=self._progress_bar_desc or "Pandas Apply")
                 return self._obj_pd.progress_apply(func, *args, **kwds)
             else:
                 return self._obj_pd.apply(func, *args, **kwds)
 
@@ -754,15 +731,15 @@
         )
         self._rolling_kwds = kwds.copy()
         self._comparison_pd = self._obj_pd.iloc[: self._SAMPLE_SIZE]
         self._sample_pd = self._sample_pd.rolling(**kwds)
         self._obj_pd = self._obj_pd.rolling(**kwds)
         self._obj_dd = self._obj_dd.rolling(**{k: v for k, v in kwds.items() if k not in ["on", "closed"]})
 
-    def _dask_apply(self, func, *args, **kwds):
+    def _parallel_apply(self, func, *args, **kwds):
         try:
             # check that the dask rolling apply matches the pandas apply
             with suppress_stdout_stderr_logging():
                 tmp_df = (
                     dd.from_pandas(self._comparison_pd, npartitions=self._npartitions)
                     .rolling(**{k: v for k, v in self._rolling_kwds.items() if k not in ["on", "closed"]})
                     .apply(func, *args, **kwds)
@@ -817,15 +794,15 @@
         # function if there are 0 `self._nrows`
         self._obj_dd = (
             self._obj_dd.resample(**{k: v for k, v in kwds.items() if k in ["rule", "closed", "label"]})
             if self._nrows
             else None
         )
 
-    def _dask_apply(self, func, *args, **kwds):
+    def _parallel_apply(self, func, *args, **kwds):
         try:
             # check that the dask resampler apply matches the pandas apply
             with suppress_stdout_stderr_logging():
                 tmp_df = (
                     dd.from_pandas(self._comparison_pd, npartitions=self._npartitions)
                     .resample(**{k: v for k, v in self._resampler_kwds.items() if k in ["rule", "closed", "label"]})
                     .agg(func, *args, **kwds)
```

### Comparing `swifter-1.3.4/swifter/swifter_tests.py` & `swifter-1.3.5/swifter/swifter_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,28 @@
+import os
 import sys
 import importlib
 import unittest
 import subprocess
 import time
 import logging
 import warnings
 from psutil import cpu_count
 
 import numpy as np
 import numpy.testing as npt
 import pandas as pd
 import swifter
 
-from .swifter import GROUPBY_MAX_ROWS_PANDAS_DEFAULT
+from .swifter import RAY_INSTALLED, GROUPBY_MAX_ROWS_PANDAS_DEFAULT
+
 from tqdm.auto import tqdm
 
+WINDOWS_CI = "windows" in os.environ.get("CIRCLE_JOB", "")
+
 
 LOG = logging.getLogger(__name__)
 LOG.setLevel(logging.INFO)
 ch = logging.StreamHandler()
 ch.setLevel(logging.INFO)
 formatter = logging.Formatter("%(asctime)-8s.%(msecs)03d %(levelname)-8s %(name)s:%(lineno)-3s %(message)s")
 ch.setFormatter(formatter)
@@ -69,15 +73,29 @@
     # if modin is installed, run the test/test suite
     if importlib.util.find_spec("modin") is not None:
         return cls
     else:  # if modin isnt installed just skip the test(s)
         return True
 
 
+def run_if_ray_installed(func):
+    # if ray is installed, run the test/test suite
+    if RAY_INSTALLED:
+        return func
+    else:  # if ray isnt installed just skip the test(s)
+        return True
+
+
 class TestSwifter(unittest.TestCase):
+    def assertLessLinux(self, a, b, msg=None):
+        if WINDOWS_CI:
+            pass
+        else:
+            super().assertLess(a, b, msg=msg)
+
     def assertSeriesEqual(self, a, b, msg):
         try:
             pd.testing.assert_series_equal(a, b)
         except AssertionError as e:
             raise self.failureException(msg) from e
 
     def assertDataFrameEqual(self, a, b, msg):
@@ -406,15 +424,15 @@
             series.swifter.set_npartitions(4).progress_bar(desc="Vec math apply ~ Series").apply(math_vec_square)
         )
         end_swifter = time.time()
         swifter_time = end_swifter - start_swifter
 
         self.assertEqual(pd_val, swifter_val)  # equality test
         if self.ncores > 1:  # speed test
-            self.assertLess(swifter_time, pd_time)
+            self.assertLessLinux(swifter_time, pd_time)
 
     def test_nonvectorized_math_apply_on_large_series(self):
         LOG.info("test_nonvectorized_math_apply_on_large_series")
         df = pd.DataFrame({"x": np.random.normal(size=10_000_000)})
         series = df["x"]
 
         tqdm.pandas(desc="Pandas Nonvec math apply ~ Series")
@@ -430,15 +448,15 @@
             .apply(math_foo, compare_to=1)
         )
         end_swifter = time.time()
         swifter_time = end_swifter - start_swifter
 
         self.assertEqual(pd_val, swifter_val)  # equality test
         if self.ncores > 1:  # speed test
-            self.assertLess(swifter_time, pd_time)
+            self.assertLessLinux(swifter_time, pd_time)
 
     def test_vectorized_force_parallel_math_apply_on_large_series(self):
         LOG.info("test_vectorized_force_parallel_math_apply_on_large_series")
         df = pd.DataFrame({"x": np.random.normal(size=2_000_000)})
         series = df["x"]
 
         tqdm.pandas(desc="Pandas Vec math apply ~ Series")
@@ -455,15 +473,15 @@
             .apply(math_vec_square)
         )
         end_swifter = time.time()
         swifter_time = end_swifter - start_swifter
 
         self.assertEqual(pd_val, swifter_val)  # equality test
         if self.ncores > 1:  # speed test
-            self.assertLess(swifter_time, pd_time)
+            self.assertLessLinux(swifter_time, pd_time)
 
 
 class TestPandasDataFrame(TestSwifter):
     def test_apply_on_empty_dataframe(self):
         LOG.info("test_apply_on_empty_dataframe")
         df = pd.DataFrame(columns=["x", "y"])
         pd_val = df.apply(math_vec_multiply, axis=1)
@@ -473,21 +491,23 @@
     def test_applymap_on_empty_dataframe(self):
         LOG.info("test_applymap_on_empty_dataframe")
         df = pd.DataFrame(columns=["x", "y"])
         pd_val = df.applymap(math_vec_square)
         swifter_val = df.swifter.applymap(math_vec_square)
         self.assertEqual(pd_val, swifter_val)  # equality test
 
+    @run_if_ray_installed
     def test_groupby_apply_on_empty_dataframe(self):
         LOG.info("test_groupby_apply_on_empty_dataframe")
         df = pd.DataFrame(columns=["x", "y"])
         pd_val = df.groupby("x").apply(math_vec_square)
         swifter_val = df.swifter.groupby("x").apply(math_vec_square)
         self.assertEqual(pd_val, swifter_val)  # equality test
 
+    @run_if_ray_installed
     def test_groupby_index_apply(self):
         LOG.info("test_groupby_index_apply")
         SIZE = GROUPBY_MAX_ROWS_PANDAS_DEFAULT * 2
         df = pd.DataFrame(
             {
                 "x": np.random.normal(size=SIZE),
                 "y": np.random.uniform(size=SIZE),
@@ -533,15 +553,15 @@
             df.swifter.set_npartitions(4).progress_bar(desc="Vec math apply ~ DF").apply(math_vec_multiply, axis=1)
         )
         end_swifter = time.time()
         swifter_time = end_swifter - start_swifter
 
         self.assertEqual(pd_val, swifter_val)  # equality test
         if self.ncores > 1:  # speed test
-            self.assertLess(swifter_time, pd_time)
+            self.assertLessLinux(swifter_time, pd_time)
 
     def test_nonvectorized_math_apply_on_large_dataframe_broadcast(self):
         LOG.info("test_nonvectorized_math_apply_on_large_dataframe_broadcast")
         df = pd.DataFrame({"x": np.random.normal(size=500_000), "y": np.random.uniform(size=500_000)})
 
         tqdm.pandas(desc="Pandas Nonvec math apply + broadcast ~ DF")
         start_pd = time.time()
@@ -556,15 +576,15 @@
             .apply(math_agg_foo, axis=1, result_type="broadcast")
         )
         end_swifter = time.time()
         swifter_time = end_swifter - start_swifter
 
         self.assertEqual(pd_val, swifter_val)  # equality test
         if self.ncores > 1:  # speed test
-            self.assertLess(swifter_time, pd_time)
+            self.assertLessLinux(swifter_time, pd_time)
 
     def test_nonvectorized_math_apply_on_large_dataframe_reduce(self):
         LOG.info("test_nonvectorized_math_apply_on_large_dataframe_reduce")
         df = pd.DataFrame({"x": np.random.normal(size=250_000), "y": np.random.uniform(size=250_000)})
 
         tqdm.pandas(desc="Pandas Nonvec math apply + reduce ~ DF")
         start_pd = time.time()
@@ -579,15 +599,15 @@
             .apply(math_agg_foo, axis=1, result_type="reduce")
         )
         end_swifter = time.time()
         swifter_time = end_swifter - start_swifter
 
         self.assertEqual(pd_val, swifter_val)  # equality test
         if self.ncores > 1:  # speed test
-            self.assertLess(swifter_time, pd_time)
+            self.assertLessLinux(swifter_time, pd_time)
 
     def test_nonvectorized_text_dask_apply_on_large_dataframe(self):
         LOG.info("test_nonvectorized_text_dask_apply_on_large_dataframe")
         df = pd.DataFrame(
             {
                 "letter": ["A", "B", "C", "D", "E"] * 200_000,
                 "value": np.random.normal(size=1_000_000),
@@ -608,15 +628,15 @@
             .apply(text_foo, axis=1)
         )
         end_swifter = time.time()
         swifter_time = end_swifter - start_swifter
 
         self.assertEqual(pd_val, swifter_val)  # equality test
         if self.ncores > 1:  # speed test
-            self.assertLess(swifter_time, pd_time)
+            self.assertLessLinux(swifter_time, pd_time)
 
     def test_vectorized_force_parallel_math_apply_on_large_dataframe(self):
         LOG.info("test_vectorized_force_parallel_math_apply_on_large_dataframe")
         df = pd.DataFrame(
             {
                 "x": np.random.normal(size=1_000_000),
                 "y": np.random.uniform(size=1_000_000),
@@ -637,15 +657,15 @@
             .apply(math_vec_multiply, axis=1)
         )
         end_swifter = time.time()
         swifter_time = end_swifter - start_swifter
 
         self.assertEqual(pd_val, swifter_val)  # equality test
         if self.ncores > 1:  # speed test
-            self.assertLess(swifter_time, pd_time)
+            self.assertLessLinux(swifter_time, pd_time)
 
     def test_vectorized_math_applymap_on_large_dataframe(self):
         LOG.info("test_vectorized_math_applymap_on_large_dataframe")
         df = pd.DataFrame(
             {
                 "x": np.random.normal(size=2_000_000),
                 "y": np.random.uniform(size=2_000_000),
@@ -663,15 +683,15 @@
             df.swifter.set_npartitions(4).progress_bar(desc="Vec math applymap ~ DF").applymap(math_vec_square)
         )
         end_swifter = time.time()
         swifter_time = end_swifter - start_swifter
 
         self.assertEqual(pd_val, swifter_val)  # equality test
         if self.ncores > 1:  # speed test
-            self.assertLess(swifter_time, pd_time)
+            self.assertLessLinux(swifter_time, pd_time)
 
     def test_vectorized_force_parallel_math_applymap_on_large_dataframe(self):
         LOG.info("test_vectorized_force_parallel_math_applymap_on_large_dataframe")
         df = pd.DataFrame(
             {
                 "x": np.random.normal(size=2_000_000),
                 "y": np.random.uniform(size=2_000_000),
@@ -692,15 +712,15 @@
             .applymap(math_vec_square)
         )
         end_swifter = time.time()
         swifter_time = end_swifter - start_swifter
 
         self.assertEqual(pd_val, swifter_val)  # equality test
         if self.ncores > 1:  # speed test
-            self.assertLess(swifter_time, pd_time)
+            self.assertLessLinux(swifter_time, pd_time)
 
     def test_nonvectorized_math_applymap_on_large_dataframe(self):
         LOG.info("test_nonvectorized_math_applymap_on_large_dataframe")
         df = pd.DataFrame(
             {
                 "x": np.random.normal(size=5_000_000),
                 "y": np.random.uniform(size=5_000_000),
@@ -716,15 +736,15 @@
         start_swifter = time.time()
         swifter_val = df.swifter.set_npartitions(4).progress_bar(desc="Nonvec math applymap ~ DF").applymap(math_foo)
         end_swifter = time.time()
         swifter_time = end_swifter - start_swifter
 
         self.assertEqual(pd_val, swifter_val)  # equality test
         if self.ncores > 1:  # speed test
-            self.assertLess(swifter_time, pd_time)
+            self.assertLessLinux(swifter_time, pd_time)
 
     def test_nonvectorized_math_applymap_on_small_dataframe(self):
         LOG.info("test_nonvectorized_math_applymap_on_small_dataframe")
         df = pd.DataFrame({"x": np.random.normal(size=1000), "y": np.random.uniform(size=1000)})
         pd_val = df.applymap(math_foo)
         swifter_val = df.swifter.set_npartitions(4).applymap(math_foo)
         self.assertEqual(pd_val, swifter_val)  # equality test
@@ -732,109 +752,118 @@
     def test_nonvectorized_math_applymap_on_small_dataframe_no_progress_bar(self):
         LOG.info("test_nonvectorized_math_applymap_on_small_dataframe_no_progress_bar")
         df = pd.DataFrame({"x": np.random.normal(size=1000), "y": np.random.uniform(size=1000)})
         pd_val = df.applymap(math_foo)
         swifter_val = df.swifter.progress_bar(enable=False).applymap(math_foo)
         self.assertEqual(pd_val, swifter_val)  # equality test
 
+    @run_if_ray_installed
     def test_vectorized_math_groupby_apply_on_small_dataframe(self):
         LOG.info("test_vectorized_math_groupby_apply_on_small_dataframe")
         df = pd.DataFrame(
             {
                 "g": np.random.choice([0, 1, 2], size=500),
                 "x": np.random.normal(size=500),
                 "y": np.random.uniform(size=500),
             }
         )
         pd_val = df.groupby("g").apply(numeric_func)
         swifter_val = df.swifter.groupby("g").apply(numeric_func)
         self.assertSeriesEqual(pd_val, swifter_val, "Swifter output does not equal Pandas output")  # equality test
 
+    @run_if_ray_installed
     def test_vectorized_force_parallel_math_groupby_apply_on_small_dataframe(self):
         LOG.info("test_vectorized_force_parallel_math_groupby_apply_on_small_dataframe")
         df = pd.DataFrame(
             {
                 "g": np.random.choice([0, 1, 2], size=500),
                 "x": np.random.normal(size=500),
                 "y": np.random.uniform(size=500),
             }
         )
         pd_val = df.groupby("g").apply(numeric_func)
         swifter_val = df.swifter.force_parallel(True).groupby("g").apply(numeric_func)
         self.assertSeriesEqual(pd_val, swifter_val, "Swifter output does not equal Pandas output")  # equality test
 
+    @run_if_ray_installed
     def test_vectorized_math_groupby_apply_on_large_dataframe(self):
         LOG.info("test_vectorized_math_groupby_apply_on_large_dataframe")
         df = pd.DataFrame(
             {
                 "g": np.random.choice(np.arange(50000), size=500000),
                 "x": np.random.normal(size=500000),
                 "y": np.random.uniform(size=500000),
             }
         )
         pd_val = df.groupby("g").apply(numeric_func)
         swifter_val = df.swifter.groupby("g").apply(numeric_func)
         self.assertSeriesEqual(pd_val, swifter_val, "Swifter output does not equal Pandas output")  # equality test
 
+    @run_if_ray_installed
     def test_vectorized_math_groupby_apply_on_large_dataframe_index(self):
         LOG.info("test_vectorized_math_groupby_apply_on_large_dataframe_index")
         df = pd.DataFrame(
             {
                 "x": np.random.normal(size=500000),
                 "y": np.random.uniform(size=500000),
             },
             index=np.random.choice(np.arange(50000), size=500000),
         )
         pd_val = df.groupby(df.index).apply(numeric_func)
         swifter_val = df.swifter.groupby(df.index).apply(numeric_func)
         self.assertSeriesEqual(pd_val, swifter_val, "Swifter output does not equal Pandas output")  # equality test
 
+    @run_if_ray_installed
     def test_vectorized_force_parallel_math_groupby_apply_on_large_dataframe(self):
         LOG.info("test_vectorized_force_parallel_math_groupby_apply_on_large_dataframe")
         df = pd.DataFrame(
             {
                 "g": np.random.choice(np.arange(50000), size=500000),
                 "x": np.random.normal(size=500000),
                 "y": np.random.uniform(size=500000),
             }
         )
         pd_val = df.groupby("g").apply(numeric_func)
         swifter_val = df.swifter.force_parallel(True).groupby("g").apply(numeric_func)
         self.assertSeriesEqual(pd_val, swifter_val, "Swifter output does not equal Pandas output")  # equality test
 
+    @run_if_ray_installed
     def test_vectorized_text_groupby_apply_on_small_dataframe(self):
         LOG.info("test_vectorized_text_groupby_apply_on_small_dataframe")
         df = pd.DataFrame(
             {"g": np.random.choice([0, 1, 2], size=500), "text": np.random.choice(["A", "B", "C"], size=500)}
         )
         pd_val = df.groupby("g").apply(clean_text_foo)
         swifter_val = df.swifter.groupby("g").apply(clean_text_foo)
         self.assertSeriesEqual(pd_val, swifter_val, "Swifter output does not equal Pandas output")  # equality test
 
+    @run_if_ray_installed
     def test_vectorized_force_parallel_text_groupby_apply_on_small_dataframe(self):
         LOG.info("test_vectorized_force_parallel_text_groupby_apply_on_small_dataframe")
         df = pd.DataFrame(
             {"g": np.random.choice([0, 1, 2], size=500), "text": np.random.choice(["A", "B", "C"], size=500)}
         )
         pd_val = df.groupby("g").apply(clean_text_foo)
         swifter_val = df.swifter.force_parallel(True).groupby("g").apply(clean_text_foo)
         self.assertSeriesEqual(pd_val, swifter_val, "Swifter output does not equal Pandas output")  # equality test
 
+    @run_if_ray_installed
     def test_vectorized_text_groupby_apply_on_large_dataframe(self):
         LOG.info("test_vectorized_text_groupby_apply_on_large_dataframe")
         df = pd.DataFrame(
             {
                 "g": np.random.choice(np.arange(50000), size=500000),
                 "text": np.random.choice(["A", "B", "C"], size=500000),
             }
         )
         pd_val = df.groupby("g").apply(clean_text_foo)
         swifter_val = df.swifter.groupby("g").apply(clean_text_foo)
         self.assertSeriesEqual(pd_val, swifter_val, "Swifter output does not equal Pandas output")  # equality test
 
+    @run_if_ray_installed
     def test_vectorized_force_parallel_text_groupby_apply_on_large_dataframe(self):
         LOG.info("test_vectorized_force_parallel_text_groupby_apply_on_large_dataframe")
         df = pd.DataFrame(
             {
                 "g": np.random.choice(np.arange(50000), size=500000),
                 "text": np.random.choice(["A", "B", "C"], size=500000),
             }
@@ -921,15 +950,15 @@
             .apply(math_agg_foo, raw=True)
         )
         end_swifter = time.time()
         swifter_time = end_swifter - start_swifter
 
         self.assertEqual(pd_val, swifter_val)  # equality test
         if self.ncores > 1:  # speed test
-            self.assertLess(swifter_time, pd_time)
+            self.assertLessLinux(swifter_time, pd_time)
 
     def test_vectorized_force_parallel_math_apply_on_large_rolling_dataframe(self):
         LOG.info("test_vectorized_force_parallel_math_apply_on_large_rolling_dataframe")
         df = pd.DataFrame(
             {"x": np.arange(0, 1_000_000)},
             index=pd.date_range("2019-01-1", "2020-01-1", periods=1_000_000),
         )
@@ -978,15 +1007,15 @@
             .apply(math_agg_foo)
         )
         end_swifter = time.time()
         swifter_time = end_swifter - start_swifter
 
         self.assertEqual(pd_val, swifter_val)  # equality test
         if self.ncores > 1:  # speed test
-            self.assertLess(swifter_time, pd_time)
+            self.assertLessLinux(swifter_time, pd_time)
 
     def test_nonvectorized_force_parallel_math_apply_on_large_resampler_dataframe(self):
         LOG.info("test_nonvectorized_force_parallel_math_apply_on_large_resampler_dataframe")
         df = pd.DataFrame(
             {"x": np.arange(0, 1_000_000)},
             index=pd.date_range("2019-01-1", "2020-01-1", periods=1_000_000),
         )
@@ -1005,15 +1034,15 @@
             .apply(math_agg_foo)
         )
         end_swifter = time.time()
         swifter_time = end_swifter - start_swifter
 
         self.assertEqual(pd_val, swifter_val)  # equality test
         if self.ncores > 1:  # speed test
-            self.assertLess(swifter_time, pd_time)
+            self.assertLessLinux(swifter_time, pd_time)
 
 
 @run_if_modin_installed
 class TestModinSeries(TestSwifter):
     def test_modin_series_warns_on_missing_attributes(self):
         LOG.info("test_modin_series_warns_on_missing_attributes")
         md = self.modinSetUp()
@@ -1169,8 +1198,8 @@
             swifter_val._to_pandas()
         )  # We have to bring it into pandas to confirm swifter apply speed is quicker
         end_swifter = time.time()
         swifter_time = end_swifter - start_swifter
 
         self.assertEqual(md_val, swifter_val)  # equality test
         self.assertEqual(md_pd_val, swifter_pd_val)  # equality test after converting to pandas
-        self.assertLess(swifter_time, md_time)  # speed test
+        self.assertLessLinux(swifter_time, md_time)  # speed test
```

### Comparing `swifter-1.3.4/swifter/tqdm_dask_progressbar.py` & `swifter-1.3.5/swifter/tqdm_dask_progressbar.py`

 * *Files identical despite different names*

