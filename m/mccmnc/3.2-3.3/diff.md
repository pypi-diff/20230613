# Comparing `tmp/mccmnc-3.2.tar.gz` & `tmp/mccmnc-3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mccmnc-3.2.tar", last modified: Mon May 29 16:41:35 2023, max compression
+gzip compressed data, was "mccmnc-3.3.tar", last modified: Tue Jun 13 04:48:32 2023, max compression
```

## Comparing `mccmnc-3.2.tar` & `mccmnc-3.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 16:41:35.864893 mccmnc-3.2/
--rw-rw-rw-   0        0        0     1092 2022-08-18 19:13:34.000000 mccmnc-3.2/LICENSE
--rw-rw-rw-   0        0        0     2909 2023-05-29 16:41:35.864893 mccmnc-3.2/PKG-INFO
--rw-rw-rw-   0        0        0     2432 2023-05-29 16:38:35.000000 mccmnc-3.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 16:41:35.849882 mccmnc-3.2/mccmnc/
--rw-rw-rw-   0        0        0        0 2022-08-18 15:56:50.000000 mccmnc-3.2/mccmnc/__init__.py
--rw-rw-rw-   0        0        0     1191 2023-05-29 16:38:12.000000 mccmnc-3.2/mccmnc/cli.py
--rw-rw-rw-   0        0        0     3615 2023-05-29 16:17:14.000000 mccmnc-3.2/mccmnc/mccmnc.py
-drwxrwxrwx   0        0        0        0 2023-05-29 16:41:35.864893 mccmnc-3.2/mccmnc.egg-info/
--rw-rw-rw-   0        0        0     2909 2023-05-29 16:41:35.000000 mccmnc-3.2/mccmnc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-05-29 16:41:35.000000 mccmnc-3.2/mccmnc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 16:41:35.000000 mccmnc-3.2/mccmnc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-05-29 16:41:35.000000 mccmnc-3.2/mccmnc.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2023-05-29 16:41:35.000000 mccmnc-3.2/mccmnc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-29 16:41:35.000000 mccmnc-3.2/mccmnc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-29 16:41:35.864893 mccmnc-3.2/setup.cfg
--rw-rw-rw-   0        0        0      894 2023-05-29 16:41:27.000000 mccmnc-3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 04:48:32.811653 mccmnc-3.3/
+-rw-rw-rw-   0        0        0     1092 2022-08-18 19:13:34.000000 mccmnc-3.3/LICENSE
+-rw-rw-rw-   0        0        0     2909 2023-06-13 04:48:32.811653 mccmnc-3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2432 2023-05-29 16:38:35.000000 mccmnc-3.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 04:48:32.811653 mccmnc-3.3/mccmnc/
+-rw-rw-rw-   0        0        0       57 2023-06-13 04:44:25.000000 mccmnc-3.3/mccmnc/__init__.py
+-rw-rw-rw-   0        0        0     1274 2023-06-13 04:46:19.000000 mccmnc-3.3/mccmnc/cli.py
+-rw-rw-rw-   0        0        0     3667 2023-06-13 04:46:19.000000 mccmnc-3.3/mccmnc/mccmnc.py
+drwxrwxrwx   0        0        0        0 2023-06-13 04:48:32.811653 mccmnc-3.3/mccmnc.egg-info/
+-rw-rw-rw-   0        0        0     2909 2023-06-13 04:48:32.000000 mccmnc-3.3/mccmnc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-06-13 04:48:32.000000 mccmnc-3.3/mccmnc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 04:48:32.000000 mccmnc-3.3/mccmnc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-06-13 04:48:32.000000 mccmnc-3.3/mccmnc.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2023-06-13 04:48:32.000000 mccmnc-3.3/mccmnc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-13 04:48:32.000000 mccmnc-3.3/mccmnc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 04:48:32.811653 mccmnc-3.3/setup.cfg
+-rw-rw-rw-   0        0        0      894 2023-06-13 04:48:30.000000 mccmnc-3.3/setup.py
```

### Comparing `mccmnc-3.2/LICENSE` & `mccmnc-3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mccmnc-3.2/PKG-INFO` & `mccmnc-3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mccmnc
-Version: 3.2
+Version: 3.3
 Summary: A tool for matching and retrieving information about MCC-MNC combinations.
 Home-page: https://github.com/jbjulia/mcc-mnc
 Author: Joseph Julian
 Author-email: jbjulian@pm.me
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mccmnc-3.2/README.md` & `mccmnc-3.3/README.md`

 * *Files identical despite different names*

### Comparing `mccmnc-3.2/mccmnc/cli.py` & `mccmnc-3.3/mccmnc/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,20 +4,30 @@
 from .mccmnc import find_matches, print_matches, update
 
 
 def get_args():
     """
     Parse command-line arguments.
     """
-    parser = argparse.ArgumentParser(description='MCC-MNC match and update tool.')
-    parser.add_argument('-cc', metavar='CC', type=str, help='Country Code (CC)')
-    parser.add_argument('-mcc', metavar='MCC', type=str, help='Mobile Country Code (MCC)')
-    parser.add_argument('-mnc', metavar='MNC', type=str, help='Mobile Network Code (MNC)')
-    parser.add_argument('-plmn', metavar='PLMN', type=str, help='Public Land Mobile Network (PLMN)')
-    parser.add_argument('-update', action='store_true', help='Downloads and refreshes local CSV and JSON')
+    parser = argparse.ArgumentParser(description="MCC-MNC match and update tool.")
+    parser.add_argument("-cc", metavar="CC", type=str, help="Country Code (CC)")
+    parser.add_argument(
+        "-mcc", metavar="MCC", type=str, help="Mobile Country Code (MCC)"
+    )
+    parser.add_argument(
+        "-mnc", metavar="MNC", type=str, help="Mobile Network Code (MNC)"
+    )
+    parser.add_argument(
+        "-plmn", metavar="PLMN", type=str, help="Public Land Mobile Network (PLMN)"
+    )
+    parser.add_argument(
+        "-update",
+        action="store_true",
+        help="Downloads and refreshes local CSV and JSON",
+    )
     return parser.parse_args()
 
 
 def main():
     args = get_args()
     try:
         if args.update:
```

### Comparing `mccmnc-3.2/mccmnc/mccmnc.py` & `mccmnc-3.3/mccmnc/mccmnc.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,31 +69,35 @@
 
         if os.path.exists(JSON_PATH):
             print(f"Removing old JSON dictionary {JSON_PATH}.")
             os.remove(JSON_PATH)
 
         print(f"Creating new JSON dictionary {JSON_PATH}.")
         json_data = {}
-        table = soup.find('table')
-        rows = table.find_all('tr')[1:]  # Skip the header
+        table = soup.find("table")
+        rows = table.find_all("tr")[1:]  # Skip the header
         total_rows = len(rows)
-        progress_bar = tqdm(total=total_rows, bar_format='{l_bar}{bar}| {n_fmt}/{total_fmt}', colour="blue")
+        progress_bar = tqdm(
+            total=total_rows,
+            bar_format="{l_bar}{bar}| {n_fmt}/{total_fmt}",
+            colour="blue",
+        )
 
         for i, row in enumerate(rows, start=1):
-            cols = row.find_all('td')
+            cols = row.find_all("td")
             mcc = cols[0].text
             mnc = cols[1].text
             plmn = mcc + mnc  # MCC + MNC
             json_data[plmn] = {
                 "MCC": mcc,
                 "MNC": mnc,
                 "ISO": cols[2].text,
                 "COUNTRY": cols[3].text,
                 "CC": cols[4].text,
-                "NETWORK": cols[5].text.strip() if cols[5].text else "unknown"
+                "NETWORK": cols[5].text.strip() if cols[5].text else "unknown",
             }
             progress_bar.set_description(f"Processing row {i}/{total_rows}")
             progress_bar.update(1)
 
         progress_bar.close()
 
         with open(JSON_PATH, "w+") as json_file:
```

### Comparing `mccmnc-3.2/mccmnc.egg-info/PKG-INFO` & `mccmnc-3.3/mccmnc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mccmnc
-Version: 3.2
+Version: 3.3
 Summary: A tool for matching and retrieving information about MCC-MNC combinations.
 Home-page: https://github.com/jbjulia/mcc-mnc
 Author: Joseph Julian
 Author-email: jbjulian@pm.me
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mccmnc-3.2/setup.py` & `mccmnc-3.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="mccmnc",
-    version="3.2",
+    version="3.3",
     author="Joseph Julian",
     author_email="jbjulian@pm.me",
     description="A tool for matching and retrieving information about MCC-MNC combinations.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jbjulia/mcc-mnc",
     packages=find_packages(),
     include_package_data=True,
-    python_requires='>=3.6',
+    python_requires=">=3.6",
     install_requires=["beautifulsoup4", "tqdm"],
     entry_points={
-        'console_scripts': [
-            'mccmnc=mccmnc.cli:main',
+        "console_scripts": [
+            "mccmnc=mccmnc.cli:main",
         ],
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

