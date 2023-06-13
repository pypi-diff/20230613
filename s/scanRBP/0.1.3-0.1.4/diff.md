# Comparing `tmp/scanRBP-0.1.3.tar.gz` & `tmp/scanRBP-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scanRBP-0.1.3.tar", last modified: Thu May 25 13:58:27 2023, max compression
+gzip compressed data, was "scanRBP-0.1.4.tar", last modified: Tue Jun 13 13:29:47 2023, max compression
```

## Comparing `scanRBP-0.1.3.tar` & `scanRBP-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwsr-x   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)        0 2023-05-25 13:58:27.110922 scanRBP-0.1.3/
--rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)     4160 2023-05-25 13:58:27.110504 scanRBP-0.1.3/PKG-INFO
--rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)     3830 2023-05-11 12:29:25.000000 scanRBP-0.1.3/README.md
-drwxrwsr-x   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)        0 2023-05-25 13:58:27.104206 scanRBP-0.1.3/scanRBP/
--rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)      507 2023-05-09 14:06:00.000000 scanRBP-0.1.3/scanRBP/__init__.py
-drwxrwsr-x   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)        0 2023-05-25 13:58:27.108231 scanRBP-0.1.3/scanRBP/config/
--rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)     1389 2023-05-16 13:54:58.000000 scanRBP-0.1.3/scanRBP/config/__init__.py
-drwxrwsr-x   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)        0 2023-05-25 13:58:27.109134 scanRBP-0.1.3/scanRBP/database/
--rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)      795 2023-05-16 12:49:53.000000 scanRBP-0.1.3/scanRBP/database/__init__.py
-drwxrwsr-x   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)        0 2023-05-25 13:58:27.109837 scanRBP-0.1.3/scanRBP/pwm/
--rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)     1465 2023-05-10 10:55:50.000000 scanRBP-0.1.3/scanRBP/pwm/__init__.py
--rwxrwxr-x   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)     8874 2023-05-16 13:54:19.000000 scanRBP-0.1.3/scanRBP/scanRBP
--rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)      104 2023-05-09 11:28:18.000000 scanRBP-0.1.3/scanRBP/scanRBP.config.example
--rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)        6 2023-05-25 13:57:50.000000 scanRBP-0.1.3/scanRBP/version
-drwxrwsr-x   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)        0 2023-05-25 13:58:27.107298 scanRBP-0.1.3/scanRBP.egg-info/
--rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)     4160 2023-05-25 13:58:26.000000 scanRBP-0.1.3/scanRBP.egg-info/PKG-INFO
--rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)      365 2023-05-25 13:58:26.000000 scanRBP-0.1.3/scanRBP.egg-info/SOURCES.txt
--rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)        1 2023-05-25 13:58:26.000000 scanRBP-0.1.3/scanRBP.egg-info/dependency_links.txt
--rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)        1 2023-05-09 11:24:46.000000 scanRBP-0.1.3/scanRBP.egg-info/not-zip-safe
--rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)       41 2023-05-25 13:58:26.000000 scanRBP-0.1.3/scanRBP.egg-info/requires.txt
--rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)        8 2023-05-25 13:58:26.000000 scanRBP-0.1.3/scanRBP.egg-info/top_level.txt
--rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)       38 2023-05-25 13:58:27.111017 scanRBP-0.1.3/setup.cfg
--rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)     1041 2023-04-28 08:24:39.000000 scanRBP-0.1.3/setup.py
+drwxrwsr-x   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)        0 2023-06-13 13:29:47.967780 scanRBP-0.1.4/
+-rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)     4936 2023-06-13 13:29:47.967057 scanRBP-0.1.4/PKG-INFO
+-rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)     4606 2023-06-08 12:22:17.000000 scanRBP-0.1.4/README.md
+drwxrwsr-x   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)        0 2023-06-13 13:29:47.961959 scanRBP-0.1.4/scanRBP/
+-rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)      507 2023-05-09 14:06:00.000000 scanRBP-0.1.4/scanRBP/__init__.py
+drwxrwsr-x   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)        0 2023-06-13 13:29:47.965434 scanRBP-0.1.4/scanRBP/config/
+-rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)     1478 2023-06-13 13:24:29.000000 scanRBP-0.1.4/scanRBP/config/__init__.py
+drwxrwsr-x   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)        0 2023-06-13 13:29:47.966075 scanRBP-0.1.4/scanRBP/database/
+-rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)      795 2023-05-16 12:49:53.000000 scanRBP-0.1.4/scanRBP/database/__init__.py
+drwxrwsr-x   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)        0 2023-06-13 13:29:47.966464 scanRBP-0.1.4/scanRBP/pwm/
+-rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)     1465 2023-05-10 10:55:50.000000 scanRBP-0.1.4/scanRBP/pwm/__init__.py
+-rwxrwxr-x   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)     8939 2023-06-13 13:24:47.000000 scanRBP-0.1.4/scanRBP/scanRBP
+-rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)      104 2023-05-09 11:28:18.000000 scanRBP-0.1.4/scanRBP/scanRBP.config.example
+-rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)        6 2023-06-13 13:29:28.000000 scanRBP-0.1.4/scanRBP/version
+drwxrwsr-x   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)        0 2023-06-13 13:29:47.964789 scanRBP-0.1.4/scanRBP.egg-info/
+-rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)     4936 2023-06-13 13:29:47.962392 scanRBP-0.1.4/scanRBP.egg-info/PKG-INFO
+-rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)      365 2023-06-13 13:29:47.962773 scanRBP-0.1.4/scanRBP.egg-info/SOURCES.txt
+-rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)        1 2023-06-13 13:29:47.963232 scanRBP-0.1.4/scanRBP.egg-info/dependency_links.txt
+-rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)        1 2023-05-09 11:24:46.000000 scanRBP-0.1.4/scanRBP.egg-info/not-zip-safe
+-rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)       41 2023-06-13 13:29:47.964386 scanRBP-0.1.4/scanRBP.egg-info/requires.txt
+-rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)        8 2023-06-13 13:29:47.964865 scanRBP-0.1.4/scanRBP.egg-info/top_level.txt
+-rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)       38 2023-06-13 13:29:47.967896 scanRBP-0.1.4/setup.cfg
+-rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)     1041 2023-04-28 08:24:39.000000 scanRBP-0.1.4/setup.py
```

### Comparing `scanRBP-0.1.3/PKG-INFO` & `scanRBP-0.1.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-Metadata-Version: 2.1
-Name: scanRBP
-Version: 0.1.3
-Summary: scanRBP: RNA-protein binding toolkit
-Home-page: https://github.com/grexor/scanRBP
-Author: Gregor Rot
-Author-email: gregor.rot@gmail.com
-Keywords: scanRBP,bioinformatics,RBP,RNA-protein binding,toolkit
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-
+### What is scanRBP?
 
 scanRBP loads RNA-protein binding motif PWM and computes the log-odds scores for all the loaded RBPs across a given genomic sequence + draws a heatmap of the scores.
 
 The scores can be described as follows ([biopython docs](http://biopython.org/DIST/docs/tutorial/Tutorial.html)):
 
 > Here we can see positive values for symbols more frequent in the motif than in the background and negative for symbols more frequent in the background. 0.0 means that it's equally likely to see a symbol in the background and in the motif.
 
 > Using the background distribution and PWM with pseudo-counts added, it's easy to compute the log-odds ratios, telling us what are the log odds of a particular symbol to be coming from a motif against the background.
 
 For more information, see the [biopython docs](http://biopython.org/DIST/docs/tutorial/Tutorial.html).
 
+### Installation <a name="initial_setup"></a>
+
+The easiest way to install scanRBP is to simply run:
+
+`$ pip install scanRBP`
+
+Note that on some systems, pip is installing the executable scripts under `~/.local/bin`. However this folder is not in the PATH which will result in `command not found` if you try to run `$ scanRBP` on the command line. To fix this, please execute `export PATH="$PATH:~/.local/bin"` (and add this to your `.profile`). Another suggestion is to install inside a virtual environment (using `virtualenv`).
+
+If you would like to install scanRBP directly from this repository, clone the repository into a folder, for example `~/software/scanRBP`. Add the `~/software/scanRBP` folder to $PYTHONPATH (`export PYTHONPATH=$PYTHONPATH:~/software/scanRBP`).
+
 ### Example run
 
 scanRBP quick start:
 
 ```
 Usage for single sequence: scanRBP sequence output [options]
      * one sequence provided on the command line, generates output.png/pdf + output.tab
@@ -67,23 +67,23 @@
 To download the PWMs:
 
 ```
 wget http://zhanglab.c2b2.columbia.edu/data/mCross/eCLIP_mCross_PWM.tgz --no-check-certificate
 tar xfz eCLIP_mCross_PWM.tgz
 ```
 
-### Additional PWM dataset
+### Additional PWM datasets
 
 https://genomebiology.biomedcentral.com/articles/10.1186/s13059-023-02913-0
 https://static-content.springer.com/esm/art%3A10.1186%2Fs13059-023-02913-0/MediaObjects/13059_2023_2913_MOESM6_ESM.txt
 
-### CLIP dataset
+### CLIP datasets
 
 bedGraph files list from:
 
 https://www.encodeproject.org/metadata/?status=released&internal_tags=ENCORE&assay_title=eCLIP&biosample_ontology.term_name=K562&biosample_ontology.term_name=HepG2&type=Experiment&files.analyses.status=released&files.preferred_default=true
 
 Any other bedGraph CLIP peak called file for a specific genome can be added to the database.
 
 ### Gene data
 
-Gene metadata (names, aliases) donwloaded from https://www.ncbi.nlm.nih.gov/gene/?term=human[organism]   
+Gene metadata (names, aliases) donwloaded from https://www.ncbi.nlm.nih.gov/gene/?term=human[organism]
```

### Comparing `scanRBP-0.1.3/README.md` & `scanRBP-0.1.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,39 @@
-### What is scanRBP?
+Metadata-Version: 2.1
+Name: scanRBP
+Version: 0.1.4
+Summary: scanRBP: RNA-protein binding toolkit
+Home-page: https://github.com/grexor/scanRBP
+Author: Gregor Rot
+Author-email: gregor.rot@gmail.com
+Keywords: scanRBP,bioinformatics,RBP,RNA-protein binding,toolkit
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+
 
 scanRBP loads RNA-protein binding motif PWM and computes the log-odds scores for all the loaded RBPs across a given genomic sequence + draws a heatmap of the scores.
 
 The scores can be described as follows ([biopython docs](http://biopython.org/DIST/docs/tutorial/Tutorial.html)):
 
 > Here we can see positive values for symbols more frequent in the motif than in the background and negative for symbols more frequent in the background. 0.0 means that it's equally likely to see a symbol in the background and in the motif.
 
 > Using the background distribution and PWM with pseudo-counts added, it's easy to compute the log-odds ratios, telling us what are the log odds of a particular symbol to be coming from a motif against the background.
 
 For more information, see the [biopython docs](http://biopython.org/DIST/docs/tutorial/Tutorial.html).
 
+### Installation <a name="initial_setup"></a>
+
+The easiest way to install scanRBP is to simply run:
+
+`$ pip install scanRBP`
+
+Note that on some systems, pip is installing the executable scripts under `~/.local/bin`. However this folder is not in the PATH which will result in `command not found` if you try to run `$ scanRBP` on the command line. To fix this, please execute `export PATH="$PATH:~/.local/bin"` (and add this to your `.profile`). Another suggestion is to install inside a virtual environment (using `virtualenv`).
+
+If you would like to install scanRBP directly from this repository, clone the repository into a folder, for example `~/software/scanRBP`. Add the `~/software/scanRBP` folder to $PYTHONPATH (`export PYTHONPATH=$PYTHONPATH:~/software/scanRBP`).
+
 ### Example run
 
 scanRBP quick start:
 
 ```
 Usage for single sequence: scanRBP sequence output [options]
      * one sequence provided on the command line, generates output.png/pdf + output.tab
@@ -57,23 +77,23 @@
 To download the PWMs:
 
 ```
 wget http://zhanglab.c2b2.columbia.edu/data/mCross/eCLIP_mCross_PWM.tgz --no-check-certificate
 tar xfz eCLIP_mCross_PWM.tgz
 ```
 
-### Additional PWM dataset
+### Additional PWM datasets
 
 https://genomebiology.biomedcentral.com/articles/10.1186/s13059-023-02913-0
 https://static-content.springer.com/esm/art%3A10.1186%2Fs13059-023-02913-0/MediaObjects/13059_2023_2913_MOESM6_ESM.txt
 
-### CLIP dataset
+### CLIP datasets
 
 bedGraph files list from:
 
 https://www.encodeproject.org/metadata/?status=released&internal_tags=ENCORE&assay_title=eCLIP&biosample_ontology.term_name=K562&biosample_ontology.term_name=HepG2&type=Experiment&files.analyses.status=released&files.preferred_default=true
 
 Any other bedGraph CLIP peak called file for a specific genome can be added to the database.
 
 ### Gene data
 
-Gene metadata (names, aliases) donwloaded from https://www.ncbi.nlm.nih.gov/gene/?term=human[organism]   
+Gene metadata (names, aliases) donwloaded from https://www.ncbi.nlm.nih.gov/gene/?term=human[organism]
```

### Comparing `scanRBP-0.1.3/scanRBP/config/__init__.py` & `scanRBP-0.1.4/scanRBP/config/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 import os
 import sys
 
+# scanRBP config file stored to ~/.pybio
+def config_fname():
+    config_fname = os.path.expanduser("~/.scanRBP")
+    return config_fname
+
 def init(data_folder=None):
     config_module = sys.modules[__name__]
     scanRBP_folder = os.path.abspath(os.path.join(os.path.abspath(__file__), "..", "..")) 
-    config_file = os.path.abspath(os.path.join(scanRBP_folder, "scanRBP.config"))
+    config_file = config_fname()
     config_example_file = os.path.abspath(os.path.join(scanRBP_folder, "scanRBP.config.example"))
     if not os.path.exists(config_file):
         config_example_file = os.path.abspath(os.path.join(scanRBP_folder, "scanRBP.config.example"))
         os.system(f"cp {config_example_file} {config_file}")
     config_lines = open(config_file).readlines()
     new_config = []
     for cline in config_lines:
```

### Comparing `scanRBP-0.1.3/scanRBP/database/__init__.py` & `scanRBP-0.1.4/scanRBP/database/__init__.py`

 * *Files identical despite different names*

### Comparing `scanRBP-0.1.3/scanRBP/pwm/__init__.py` & `scanRBP-0.1.4/scanRBP/pwm/__init__.py`

 * *Files identical despite different names*

### Comparing `scanRBP-0.1.3/scanRBP/scanRBP` & `scanRBP-0.1.4/scanRBP/scanRBP`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,15 @@
 parser.add_argument("-heatmap", "--heatmap", default=False)
 parser.add_argument("-output_folder", "--output_folder", default=".")
 parser.add_argument("-version", "--version", help="Print version", action="store_true")
 
 args = parser.parse_args()
 
 print(f"[scanRBP] v{scanRBP.version}, https://github.com/grexor/scanRBP")
+print(f"[scanRBP] config file: {scanRBP.config.config_fname()}")
 print(f"[scanRBP] data folder: {scanRBP.config.data_folder}")
 print()
 
 # find all proteins with search
 def find_proteins(search):
     results, results_data = [], []
     for scan_id, data in scanRBP.database.proteins.items():
```

### Comparing `scanRBP-0.1.3/scanRBP.egg-info/PKG-INFO` & `scanRBP-0.1.4/scanRBP.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scanRBP
-Version: 0.1.3
+Version: 0.1.4
 Summary: scanRBP: RNA-protein binding toolkit
 Home-page: https://github.com/grexor/scanRBP
 Author: Gregor Rot
 Author-email: gregor.rot@gmail.com
 Keywords: scanRBP,bioinformatics,RBP,RNA-protein binding,toolkit
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -16,14 +16,24 @@
 
 > Here we can see positive values for symbols more frequent in the motif than in the background and negative for symbols more frequent in the background. 0.0 means that it's equally likely to see a symbol in the background and in the motif.
 
 > Using the background distribution and PWM with pseudo-counts added, it's easy to compute the log-odds ratios, telling us what are the log odds of a particular symbol to be coming from a motif against the background.
 
 For more information, see the [biopython docs](http://biopython.org/DIST/docs/tutorial/Tutorial.html).
 
+### Installation <a name="initial_setup"></a>
+
+The easiest way to install scanRBP is to simply run:
+
+`$ pip install scanRBP`
+
+Note that on some systems, pip is installing the executable scripts under `~/.local/bin`. However this folder is not in the PATH which will result in `command not found` if you try to run `$ scanRBP` on the command line. To fix this, please execute `export PATH="$PATH:~/.local/bin"` (and add this to your `.profile`). Another suggestion is to install inside a virtual environment (using `virtualenv`).
+
+If you would like to install scanRBP directly from this repository, clone the repository into a folder, for example `~/software/scanRBP`. Add the `~/software/scanRBP` folder to $PYTHONPATH (`export PYTHONPATH=$PYTHONPATH:~/software/scanRBP`).
+
 ### Example run
 
 scanRBP quick start:
 
 ```
 Usage for single sequence: scanRBP sequence output [options]
      * one sequence provided on the command line, generates output.png/pdf + output.tab
@@ -67,20 +77,20 @@
 To download the PWMs:
 
 ```
 wget http://zhanglab.c2b2.columbia.edu/data/mCross/eCLIP_mCross_PWM.tgz --no-check-certificate
 tar xfz eCLIP_mCross_PWM.tgz
 ```
 
-### Additional PWM dataset
+### Additional PWM datasets
 
 https://genomebiology.biomedcentral.com/articles/10.1186/s13059-023-02913-0
 https://static-content.springer.com/esm/art%3A10.1186%2Fs13059-023-02913-0/MediaObjects/13059_2023_2913_MOESM6_ESM.txt
 
-### CLIP dataset
+### CLIP datasets
 
 bedGraph files list from:
 
 https://www.encodeproject.org/metadata/?status=released&internal_tags=ENCORE&assay_title=eCLIP&biosample_ontology.term_name=K562&biosample_ontology.term_name=HepG2&type=Experiment&files.analyses.status=released&files.preferred_default=true
 
 Any other bedGraph CLIP peak called file for a specific genome can be added to the database.
```

### Comparing `scanRBP-0.1.3/setup.py` & `scanRBP-0.1.4/setup.py`

 * *Files identical despite different names*

