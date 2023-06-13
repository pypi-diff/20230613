# Comparing `tmp/jsonfmt-0.2.5.tar.gz` & `tmp/jsonfmt-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonfmt-0.2.5.tar", last modified: Tue Jun  6 11:11:38 2023, max compression
+gzip compressed data, was "jsonfmt-0.2.6.tar", last modified: Tue Jun 13 09:59:35 2023, max compression
```

## Comparing `jsonfmt-0.2.5.tar` & `jsonfmt-0.2.6.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:11:38.462554 jsonfmt-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-06 11:11:17.000000 jsonfmt-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13703 2023-06-06 11:11:38.458554 jsonfmt-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12581 2023-06-06 11:11:17.000000 jsonfmt-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:11:38.458554 jsonfmt-0.2.5/jsonfmt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13703 2023-06-06 11:11:38.000000 jsonfmt-0.2.5/jsonfmt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-06 11:11:38.000000 jsonfmt-0.2.5/jsonfmt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 11:11:38.000000 jsonfmt-0.2.5/jsonfmt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-06 11:11:38.000000 jsonfmt-0.2.5/jsonfmt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-06 11:11:38.000000 jsonfmt-0.2.5/jsonfmt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-06 11:11:38.000000 jsonfmt-0.2.5/jsonfmt.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    10544 2023-06-06 11:11:17.000000 jsonfmt-0.2.5/jsonfmt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-06 11:11:17.000000 jsonfmt-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 11:11:38.462554 jsonfmt-0.2.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:11:38.458554 jsonfmt-0.2.5/test/
--rw-r--r--   0 runner    (1001) docker     (123)    15677 2023-06-06 11:11:17.000000 jsonfmt-0.2.5/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:59:35.915504 jsonfmt-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-13 09:59:18.000000 jsonfmt-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16213 2023-06-13 09:59:35.915504 jsonfmt-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15091 2023-06-13 09:59:18.000000 jsonfmt-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:59:35.915504 jsonfmt-0.2.6/jsonfmt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16213 2023-06-13 09:59:35.000000 jsonfmt-0.2.6/jsonfmt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-13 09:59:35.000000 jsonfmt-0.2.6/jsonfmt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 09:59:35.000000 jsonfmt-0.2.6/jsonfmt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-13 09:59:35.000000 jsonfmt-0.2.6/jsonfmt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-13 09:59:35.000000 jsonfmt-0.2.6/jsonfmt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 09:59:35.000000 jsonfmt-0.2.6/jsonfmt.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12198 2023-06-13 09:59:18.000000 jsonfmt-0.2.6/jsonfmt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-06-13 09:59:18.000000 jsonfmt-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-13 09:59:18.000000 jsonfmt-0.2.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 09:59:35.915504 jsonfmt-0.2.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:59:35.915504 jsonfmt-0.2.6/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    17709 2023-06-13 09:59:18.000000 jsonfmt-0.2.6/test/test.py
```

### Comparing `jsonfmt-0.2.5/LICENSE` & `jsonfmt-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonfmt-0.2.5/PKG-INFO` & `jsonfmt-0.2.6/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,66 +1,42 @@
-Metadata-Version: 2.1
-Name: jsonfmt
-Version: 0.2.5
-Summary: A simple tool for formatting JSON object.
-Author-email: Seamile <lanhuermao@gmail.com>
-License: MIT License
-Project-URL: homepage, https://github.com/seamile/jsonfmt
-Project-URL: repository, https://github.com/seamile/jsonfmt
-Project-URL: documentation, https://seamile.github.io/jsonfmt/
-Keywords: json,formatter,pretty-print,highlight,jmespath
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Topic :: File Formats :: JSON
-Classifier: Topic :: Printing
-Classifier: Topic :: Utilities
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # JSON Formatter
 
 [![Build Status](https://github.com/seamile/jsonfmt/actions/workflows/python-package.yml/badge.svg)](https://github.com/seamile/jsonfmt/actions)
 [![PyPI Version](https://img.shields.io/pypi/v/jsonfmt?color=blue&label=Version&logo=python&logoColor=white)](https://pypi.org/project/jsonfmt/)
 [![Installs](https://static.pepy.tech/personalized-badge/jsonfmt?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Installs)](https://pepy.tech/project/jsonfmt)
 [![Code Grade](https://app.codacy.com/project/badge/Grade/1e12e3cd8c8342bca68db4caf5b6a31d)](https://app.codacy.com/gh/seamile/jsonfmt/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 [![Test Coverage](https://app.codacy.com/project/badge/Coverage/1e12e3cd8c8342bca68db4caf5b6a31d)](https://app.codacy.com/gh/seamile/jsonfmt/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage)
 
-**jsonfmt** is a powerful tool for handling JSON document.
+**jsonfmt** is a powerful tool for pretty-printing, querying and conversion JSON documents.
 
-It is as powerful as [jq](https://github.com/jqlang/jq), but simpler.
+It is as powerful as [jq](https://github.com/jqlang/jq), but easier to use.
 
 
 ## Features
 
 - [1. Pretty print JSON document.](#1-pretty-print-json-document)
     - [Syntax hight and indenation.](#syntax-hight-and-indenation)
     - [Read JSON from pipeline.](#read-json-from-pipeline)
 - [2. Features for handling large JSON document.](#2-features-for-handling-large-json-document)
     - [View a large JSON with pager-mode.](#view-a-large-json-with-pager-mode)
     - [Show the overview of a large JSON.](#show-the-overview-of-a-large-json)
     - [Copy the result to clipboard.](#copy-the-result-to-clipboard)
 - [3. Minimize the JSON document.](#3-minimize-the-json-document)
-- [4. Pick out parts of a large JSON via JmesPath.](#4-pick-out-parts-of-a-large-json-via-jmespath)
+- [4. Pick out parts of a large JSON via JMESPath or JSONPath.](#4-pick-out-parts-of-a-large-json-via-jmespath-or-jsonpath)
+    - [JMESPath examples](#jmespath-examples)
+    - [JSONPath examples](#jsonpath-examples)
+    - [Query for TOML and YAML](#query-for-toml-and-yaml)
 - [5. Convert formats between JSON, TOML and YAML.](#5-convert-formats-between-json-toml-and-yaml)
     - [JSON to TOML and YAML](#json-to-toml-and-yaml)
     - [TOML to JSON and YAML](#toml-to-json-and-yaml)
     - [YAML to JSON and TOML](#yaml-to-json-and-toml)
 - [6. Modify some values in the input data.](#6-modify-some-values-in-the-input-data)
-    - [Add and modify some items.](#add-and-modify-some-items)
-    - [Pop some items.](#pop-some-items)
+    - [Add items](#add-items)
+    - [Modify items](#modify-items)
+    - [Pop items](#pop-items)
 - [7. Output to file.](#7-output-to-file)
 
 
 ## Install
 
 ```shell
 $ pip install jsonfmt
@@ -79,19 +55,20 @@
 
 - Options:
 
     - `-h, --help`: show this help message and exit
     - `-c`: suppress all whitespace separation
     - `-C`: copy the result to clipboard
     - `-e`: escape non-ASCII characters
-    - `-f {json,toml,yaml}`: the format to output (default: None)
+    - `-f {json,toml,yaml}`: the format to output (default: same as input)
     - `-i {0-8,t}`: number of spaces for indentation (default: 2)
     - `-o`: show data structure overview
     - `-O`: overwrite the formated text to original file
-    - `-p JSONPATH`: output part of the object via jmespath
+    - `-l {jmespath,jsonpath}`: the language for querying (default: jmespath)
+    - `-p QUERYPATH`: the path for querying
     - `-s`: sort keys of objects on output
     - `--set 'foo.k1=v1;k2[i]=v2'`: set the keys to values (seperated by `;`)
     - `--pop 'k1;foo.k2;k3[i]'`: pop the specified keys (seperated by `;`)
     - `-v`: show the version
 
 
 ## Example
@@ -160,19 +137,26 @@
 
 The pager-mode is similar to the command `more`.
 
 *jsonfmt* will automatically present the result in pager-mode when the JSON document is too large to overflow the window display area.
 
 The key-binding of the pager-mode is same as command `more`:
 
-- <kbd>j</kbd> / <kbd>k</kbd> to forward / backward by line.
-- <kbd>f</kbd> or <kbd>ctrl</kbd>+<kbd>f</kbd> to forward by page.
-- <kbd>b</kbd> or <kbd>ctrl</kbd>+<kbd>b</kbd> to backward by page.
-- <kbd>g</kbd> to go to the top of the page, and <kbd>G</kbd> to the bottom.
-- <kbd>q</kbd> to exit.
+| key                          | description               |
+|------------------------------|---------------------------|
+| <kbd>j</kbd>                 | forward  by line          |
+| <kbd>k</kbd>                 | backward by line          |
+| <kbd>f</kbd>                 | forward by page           |
+| <kbd>ctrl</kbd>+<kbd>f</kbd> | forward by page           |
+| <kbd>b</kbd>                 | backward by page          |
+| <kbd>ctrl</kbd>+<kbd>b</kbd> | backward by page          |
+| <kbd>g</kbd>                 | go to the top of the page |
+| <kbd>G</kbd>                 | go to the bottom          |
+| <kbd>/</kbd>                 | search mode               |
+| <kbd>q</kbd>                 | quit pager-mode           |
 
 There is a big JSON from GitHub, you can paste this command into terminal to try the pager-mode:
 
 ```shell
 curl -s 'https://api.github.com/repos/seamile/jsonfmt/commits?per_page=10' | jsonfmt
 ```
 
@@ -238,25 +222,23 @@
 
 *Output:*
 
 ```json
 {"age":21,"items":["pen","phone"],"name":"alex"}
 ```
 
-### 4. Pick out parts of a large JSON via JmesPath.
+### 4. Pick out parts of a large JSON via JMESPath or JSONPath.
 
-Unlike from jq's private solution, `jsonfmt` uses [JmesPath](https://jmespath.org/) as its query language.
+Unlike from jq's private solution, `jsonfmt` uses both [JMESPath](https://jmespath.org/) and [JSONPath](https://datatracker.ietf.org/doc/id/draft-goessner-dispatch-jsonpath-00.html) as its query language.
 
-Among the many JSON query languages, `JmesPath` is the most popular one ([compared here](https://npmtrends.com/JSONPath-vs-jmespath-vs-jq-vs-json-path-vs-json-query-vs-jsonata-vs-jsonpath-vs-jsonpath-plus-vs-node-jq)).
-It is more general than `jq`, and more intuitive and powerful than `JsonPath`.
+Among the many JSON query languages, `JMESPath` is the most popular one ([compared here](https://npmtrends.com/JSONPath-vs-jmespath-vs-jq-vs-json-path-vs-json-query-vs-jsonata-vs-jsonpath-vs-jsonpath-plus-vs-node-jq)). It is more general than `jq`, and more intuitive and powerful than `JSONPath`. So I prefer to use it.
 
-Like the XPath for xml, `JmesPath` can elegantly extract parts of a given JSON document with simple syntax.
-See the tutorial [here](https://jmespath.org/tutorial.html).
+Like the XPath for xml, `JMESPath` can elegantly extract parts of a given JSON document with simple syntax. The official tutorial of JMESPath is [here](https://jmespath.org/tutorial.html).
 
-Some examples:
+#### JMESPath examples
 
 - pick out the first actions in `example.json`
 
     ```shell
     $ jsonfmt -p 'actions[0]' test/example.json
     ```
 
@@ -287,15 +269,15 @@
         }
     ]
     ```
 
 - Show all the keys and actions' length.
 
     ```shell
-    $ jsonfmt  -p '{all_keys:keys(@), actions_len:length(actions)}' test/example.json
+    $ jsonfmt -p '{all_keys:keys(@), actions_len:length(actions)}' test/example.json
     ```
 
     *Output:*
 
     ```json
     {
         "all_keys": [
@@ -326,35 +308,82 @@
         {
             "name": "eat",
             "calorie": 294.9
         }
     ]
     ```
 
-- [More examples](https://jmespath.org/examples.html).
+[More examples of JMESPath](https://jmespath.org/examples.html).
 
+#### JSONPath examples
 
-**Amazingly**, you can do the same with YAML and TOML using JmesPath, and convert the result format arbitrarily.
+The syntax of `JSONPath` is very similar to that of `JMESPath`. Everything that `JSONPath` can do `JMESPath` can also do, except using relative path querying. So `JSONPath` can be used as a supplementary query method of `JMESPath`.
 
-```shell
-# read the data from toml file, and convert the result to yaml
-$ jsonfmt  -p '{all_keys:keys(@), actions_len:length(actions)}' test/example.yaml -f toml
-```
+- Filter all `name` fields by relative path:
 
-*Output:*
+    ```shell
+    # use `-l` to specify the query language of JSON
+    $ jsonfmt.py -l jsonpath -p '$..name' test/example.json
+    ```
 
-```yaml
-all_keys:
-- age
-- gender
-- money
-- name
-- actions
-actions_len: 2
-```
+    *Output:*
+
+    ```json
+    [
+        "Bob",
+        "eat",
+        "sport"
+    ]
+    ```
+
+#### Query for TOML and YAML
+
+**Amazingly**, you can do all of the above with TOML and YAML in the same way, and convert the result format arbitrarily. It is even possible to process all three formats simultaneously in a single command.
+
+- Read the data from toml file, and convert the result to yaml
+
+    ```shell
+    $ jsonfmt -p '{all_keys:keys(@), actions_len:length(actions)}' test/example.toml -f yaml
+    ```
+
+    *Output:*
+
+    ```yaml
+    all_keys:
+    - age
+    - gender
+    - money
+    - name
+    - actions
+    actions_len: 2
+    ```
+
+- Handle three formats simultaneously
+
+    ```shell
+    $ jsonfmt.py -p 'actions[0]' test/example.json test/example.toml test/example.yaml
+    ```
+
+    *Output:*
+
+    ```
+    {
+        "calorie": 294.9,
+        "date": "2021-03-02",
+        "name": "eat"
+    }
+
+    calorie = 294.9
+    date = "2021-03-02"
+    name = "eat"
+
+    calorie: 294.9
+    date: '2021-03-02'
+    name: eat
+    ```
 
 
 ### 5. Convert formats between JSON, TOML and YAML.
 
 The *jsonfmt* can recognize any format of JSON, TOML and YAML from files or `stdin`. Either formats can be converted to the other by specifying the "-f" option.
 
 <div style="color: orange"><strong>Note that:</strong></div>
@@ -423,23 +452,23 @@
 $ jsonfmt test/example.yaml -f toml
 ```
 
 ### 6. Modify some values in the input data.
 
 Use the `--set` and `--pop` options when you want to change something in the input documents.
 
-The format is `--set 'key1=value1'`. When you need to modify multiple values ​​you can use `;` to separate: `--set 'k1=v1;k2=v2'`. If the key-value pair dose not exist, it will be added.
+The format is `--set 'key=value'`. When you need to modify multiple values ​​you can use `;` to separate: `--set 'k1=v1;k2=v2'`. If the key-value pair dose not exist, it will be added.
 
-For the items in list, use `key[i]` or `key.i` to specify. But it doesn't support adding new elements.
+For the items in list, use `key[i]` or `key.i` to specify. If the index is greater than or equal to the number of elements, the value will be appended.
 
-#### Add and modify some items.
+#### Add items
 
 ```shell
-# add a key-value pair and modify the money field
-$ jsonfmt --set 'skills=["Django","Flask"];money=1000' test/example.json
+# add `country` key and append one item for `actions`
+$ jsonfmt --set 'country=China; actions[2]={"name": "drink"}' test/example.json
 ```
 
 *Output:*
 
 ```json
 {
     "actions": [
@@ -448,32 +477,62 @@
             "date": "2021-03-02",
             "name": "eat"
         },
         {
             "calorie": -375,
             "date": "2023-04-27",
             "name": "sport"
+        },
+        {
+            "name": "drink"
+        }
+    ],
+    "age": 23,
+    "country": "China",
+    "gender": "纯爷们",
+    "money": 3.1415926,
+    "name": "Bob"
+}
+```
+
+#### Modify items
+
+```shell
+# modify money and actions[1]["name"]
+$ jsonfmt --set 'money=1000; actions[1].name=swim' test/example.json
+```
+
+*Output:*
+
+```json
+{
+    "actions": [
+        {
+            "calorie": 294.9,
+            "date": "2021-03-02",
+            "name": "eat"
+        },
+        {
+            "calorie": -375,
+            "date": "2023-04-27",
+            "name": "swim"
         }
     ],
     "age": 23,
     "gender": "纯爷们",
     "money": 1000,
-    "name": "Bob",
-    "skills": [
-        "Django",
-        "Flask"
-    ]
+    "name": "Bob"
 }
 ```
 
-#### Pop some items.
+#### Pop items
 
 ```shell
-# remove the gender field and actions[1]
-$ jsonfmt --pop 'gender;actions[1]' test/example.json
+# pop `gender` and actions[1]
+$ jsonfmt --pop 'gender; actions[1]' test/example.json
 ```
 
 *Output:*
 
 ```json
 {
     "actions": [
@@ -492,15 +551,15 @@
 Of course you can use `--set` and `--pop` together.
 
 ```shell
 jsonfmt --set 'skills=["Django","Flask"];money=1000' --pop 'gender;actions[1]' test/example.json
 ```
 
 **Note**, however, that the above command will not modify the original JSON file.
-If you want to do this, then please read below.
+If you want to do this, read below please.
 
 ### 7. Output to file.
 
 - use the `-O` parameter to overwrite the file with the result.
 
     This option will be forced to close when `-o` is specified
```

### Comparing `jsonfmt-0.2.5/README.md` & `jsonfmt-0.2.6/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,70 @@
+Metadata-Version: 2.1
+Name: jsonfmt
+Version: 0.2.6
+Summary: A simple tool for formatting JSON object.
+Author-email: Seamile <lanhuermao@gmail.com>
+License: MIT License
+Project-URL: homepage, https://github.com/seamile/jsonfmt
+Project-URL: repository, https://github.com/seamile/jsonfmt
+Project-URL: documentation, https://seamile.github.io/jsonfmt/
+Keywords: json,formatter,pretty-print,highlight,jmespath
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: File Formats :: JSON
+Classifier: Topic :: Printing
+Classifier: Topic :: Utilities
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # JSON Formatter
 
 [![Build Status](https://github.com/seamile/jsonfmt/actions/workflows/python-package.yml/badge.svg)](https://github.com/seamile/jsonfmt/actions)
 [![PyPI Version](https://img.shields.io/pypi/v/jsonfmt?color=blue&label=Version&logo=python&logoColor=white)](https://pypi.org/project/jsonfmt/)
 [![Installs](https://static.pepy.tech/personalized-badge/jsonfmt?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Installs)](https://pepy.tech/project/jsonfmt)
 [![Code Grade](https://app.codacy.com/project/badge/Grade/1e12e3cd8c8342bca68db4caf5b6a31d)](https://app.codacy.com/gh/seamile/jsonfmt/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 [![Test Coverage](https://app.codacy.com/project/badge/Coverage/1e12e3cd8c8342bca68db4caf5b6a31d)](https://app.codacy.com/gh/seamile/jsonfmt/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage)
 
-**jsonfmt** is a powerful tool for handling JSON document.
+**jsonfmt** is a powerful tool for pretty-printing, querying and conversion JSON documents.
 
-It is as powerful as [jq](https://github.com/jqlang/jq), but simpler.
+It is as powerful as [jq](https://github.com/jqlang/jq), but easier to use.
 
 
 ## Features
 
 - [1. Pretty print JSON document.](#1-pretty-print-json-document)
     - [Syntax hight and indenation.](#syntax-hight-and-indenation)
     - [Read JSON from pipeline.](#read-json-from-pipeline)
 - [2. Features for handling large JSON document.](#2-features-for-handling-large-json-document)
     - [View a large JSON with pager-mode.](#view-a-large-json-with-pager-mode)
     - [Show the overview of a large JSON.](#show-the-overview-of-a-large-json)
     - [Copy the result to clipboard.](#copy-the-result-to-clipboard)
 - [3. Minimize the JSON document.](#3-minimize-the-json-document)
-- [4. Pick out parts of a large JSON via JmesPath.](#4-pick-out-parts-of-a-large-json-via-jmespath)
+- [4. Pick out parts of a large JSON via JMESPath or JSONPath.](#4-pick-out-parts-of-a-large-json-via-jmespath-or-jsonpath)
+    - [JMESPath examples](#jmespath-examples)
+    - [JSONPath examples](#jsonpath-examples)
+    - [Query for TOML and YAML](#query-for-toml-and-yaml)
 - [5. Convert formats between JSON, TOML and YAML.](#5-convert-formats-between-json-toml-and-yaml)
     - [JSON to TOML and YAML](#json-to-toml-and-yaml)
     - [TOML to JSON and YAML](#toml-to-json-and-yaml)
     - [YAML to JSON and TOML](#yaml-to-json-and-toml)
 - [6. Modify some values in the input data.](#6-modify-some-values-in-the-input-data)
-    - [Add and modify some items.](#add-and-modify-some-items)
-    - [Pop some items.](#pop-some-items)
+    - [Add items](#add-items)
+    - [Modify items](#modify-items)
+    - [Pop items](#pop-items)
 - [7. Output to file.](#7-output-to-file)
 
 
 ## Install
 
 ```shell
 $ pip install jsonfmt
@@ -51,19 +83,20 @@
 
 - Options:
 
     - `-h, --help`: show this help message and exit
     - `-c`: suppress all whitespace separation
     - `-C`: copy the result to clipboard
     - `-e`: escape non-ASCII characters
-    - `-f {json,toml,yaml}`: the format to output (default: None)
+    - `-f {json,toml,yaml}`: the format to output (default: same as input)
     - `-i {0-8,t}`: number of spaces for indentation (default: 2)
     - `-o`: show data structure overview
     - `-O`: overwrite the formated text to original file
-    - `-p JSONPATH`: output part of the object via jmespath
+    - `-l {jmespath,jsonpath}`: the language for querying (default: jmespath)
+    - `-p QUERYPATH`: the path for querying
     - `-s`: sort keys of objects on output
     - `--set 'foo.k1=v1;k2[i]=v2'`: set the keys to values (seperated by `;`)
     - `--pop 'k1;foo.k2;k3[i]'`: pop the specified keys (seperated by `;`)
     - `-v`: show the version
 
 
 ## Example
@@ -132,19 +165,26 @@
 
 The pager-mode is similar to the command `more`.
 
 *jsonfmt* will automatically present the result in pager-mode when the JSON document is too large to overflow the window display area.
 
 The key-binding of the pager-mode is same as command `more`:
 
-- <kbd>j</kbd> / <kbd>k</kbd> to forward / backward by line.
-- <kbd>f</kbd> or <kbd>ctrl</kbd>+<kbd>f</kbd> to forward by page.
-- <kbd>b</kbd> or <kbd>ctrl</kbd>+<kbd>b</kbd> to backward by page.
-- <kbd>g</kbd> to go to the top of the page, and <kbd>G</kbd> to the bottom.
-- <kbd>q</kbd> to exit.
+| key                          | description               |
+|------------------------------|---------------------------|
+| <kbd>j</kbd>                 | forward  by line          |
+| <kbd>k</kbd>                 | backward by line          |
+| <kbd>f</kbd>                 | forward by page           |
+| <kbd>ctrl</kbd>+<kbd>f</kbd> | forward by page           |
+| <kbd>b</kbd>                 | backward by page          |
+| <kbd>ctrl</kbd>+<kbd>b</kbd> | backward by page          |
+| <kbd>g</kbd>                 | go to the top of the page |
+| <kbd>G</kbd>                 | go to the bottom          |
+| <kbd>/</kbd>                 | search mode               |
+| <kbd>q</kbd>                 | quit pager-mode           |
 
 There is a big JSON from GitHub, you can paste this command into terminal to try the pager-mode:
 
 ```shell
 curl -s 'https://api.github.com/repos/seamile/jsonfmt/commits?per_page=10' | jsonfmt
 ```
 
@@ -210,25 +250,23 @@
 
 *Output:*
 
 ```json
 {"age":21,"items":["pen","phone"],"name":"alex"}
 ```
 
-### 4. Pick out parts of a large JSON via JmesPath.
+### 4. Pick out parts of a large JSON via JMESPath or JSONPath.
 
-Unlike from jq's private solution, `jsonfmt` uses [JmesPath](https://jmespath.org/) as its query language.
+Unlike from jq's private solution, `jsonfmt` uses both [JMESPath](https://jmespath.org/) and [JSONPath](https://datatracker.ietf.org/doc/id/draft-goessner-dispatch-jsonpath-00.html) as its query language.
 
-Among the many JSON query languages, `JmesPath` is the most popular one ([compared here](https://npmtrends.com/JSONPath-vs-jmespath-vs-jq-vs-json-path-vs-json-query-vs-jsonata-vs-jsonpath-vs-jsonpath-plus-vs-node-jq)).
-It is more general than `jq`, and more intuitive and powerful than `JsonPath`.
+Among the many JSON query languages, `JMESPath` is the most popular one ([compared here](https://npmtrends.com/JSONPath-vs-jmespath-vs-jq-vs-json-path-vs-json-query-vs-jsonata-vs-jsonpath-vs-jsonpath-plus-vs-node-jq)). It is more general than `jq`, and more intuitive and powerful than `JSONPath`. So I prefer to use it.
 
-Like the XPath for xml, `JmesPath` can elegantly extract parts of a given JSON document with simple syntax.
-See the tutorial [here](https://jmespath.org/tutorial.html).
+Like the XPath for xml, `JMESPath` can elegantly extract parts of a given JSON document with simple syntax. The official tutorial of JMESPath is [here](https://jmespath.org/tutorial.html).
 
-Some examples:
+#### JMESPath examples
 
 - pick out the first actions in `example.json`
 
     ```shell
     $ jsonfmt -p 'actions[0]' test/example.json
     ```
 
@@ -259,15 +297,15 @@
         }
     ]
     ```
 
 - Show all the keys and actions' length.
 
     ```shell
-    $ jsonfmt  -p '{all_keys:keys(@), actions_len:length(actions)}' test/example.json
+    $ jsonfmt -p '{all_keys:keys(@), actions_len:length(actions)}' test/example.json
     ```
 
     *Output:*
 
     ```json
     {
         "all_keys": [
@@ -298,35 +336,82 @@
         {
             "name": "eat",
             "calorie": 294.9
         }
     ]
     ```
 
-- [More examples](https://jmespath.org/examples.html).
+[More examples of JMESPath](https://jmespath.org/examples.html).
 
+#### JSONPath examples
 
-**Amazingly**, you can do the same with YAML and TOML using JmesPath, and convert the result format arbitrarily.
+The syntax of `JSONPath` is very similar to that of `JMESPath`. Everything that `JSONPath` can do `JMESPath` can also do, except using relative path querying. So `JSONPath` can be used as a supplementary query method of `JMESPath`.
 
-```shell
-# read the data from toml file, and convert the result to yaml
-$ jsonfmt  -p '{all_keys:keys(@), actions_len:length(actions)}' test/example.yaml -f toml
-```
+- Filter all `name` fields by relative path:
 
-*Output:*
+    ```shell
+    # use `-l` to specify the query language of JSON
+    $ jsonfmt.py -l jsonpath -p '$..name' test/example.json
+    ```
 
-```yaml
-all_keys:
-- age
-- gender
-- money
-- name
-- actions
-actions_len: 2
-```
+    *Output:*
+
+    ```json
+    [
+        "Bob",
+        "eat",
+        "sport"
+    ]
+    ```
+
+#### Query for TOML and YAML
+
+**Amazingly**, you can do all of the above with TOML and YAML in the same way, and convert the result format arbitrarily. It is even possible to process all three formats simultaneously in a single command.
+
+- Read the data from toml file, and convert the result to yaml
+
+    ```shell
+    $ jsonfmt -p '{all_keys:keys(@), actions_len:length(actions)}' test/example.toml -f yaml
+    ```
+
+    *Output:*
+
+    ```yaml
+    all_keys:
+    - age
+    - gender
+    - money
+    - name
+    - actions
+    actions_len: 2
+    ```
+
+- Handle three formats simultaneously
+
+    ```shell
+    $ jsonfmt.py -p 'actions[0]' test/example.json test/example.toml test/example.yaml
+    ```
+
+    *Output:*
+
+    ```
+    {
+        "calorie": 294.9,
+        "date": "2021-03-02",
+        "name": "eat"
+    }
+
+    calorie = 294.9
+    date = "2021-03-02"
+    name = "eat"
+
+    calorie: 294.9
+    date: '2021-03-02'
+    name: eat
+    ```
 
 
 ### 5. Convert formats between JSON, TOML and YAML.
 
 The *jsonfmt* can recognize any format of JSON, TOML and YAML from files or `stdin`. Either formats can be converted to the other by specifying the "-f" option.
 
 <div style="color: orange"><strong>Note that:</strong></div>
@@ -395,23 +480,23 @@
 $ jsonfmt test/example.yaml -f toml
 ```
 
 ### 6. Modify some values in the input data.
 
 Use the `--set` and `--pop` options when you want to change something in the input documents.
 
-The format is `--set 'key1=value1'`. When you need to modify multiple values ​​you can use `;` to separate: `--set 'k1=v1;k2=v2'`. If the key-value pair dose not exist, it will be added.
+The format is `--set 'key=value'`. When you need to modify multiple values ​​you can use `;` to separate: `--set 'k1=v1;k2=v2'`. If the key-value pair dose not exist, it will be added.
 
-For the items in list, use `key[i]` or `key.i` to specify. But it doesn't support adding new elements.
+For the items in list, use `key[i]` or `key.i` to specify. If the index is greater than or equal to the number of elements, the value will be appended.
 
-#### Add and modify some items.
+#### Add items
 
 ```shell
-# add a key-value pair and modify the money field
-$ jsonfmt --set 'skills=["Django","Flask"];money=1000' test/example.json
+# add `country` key and append one item for `actions`
+$ jsonfmt --set 'country=China; actions[2]={"name": "drink"}' test/example.json
 ```
 
 *Output:*
 
 ```json
 {
     "actions": [
@@ -420,32 +505,62 @@
             "date": "2021-03-02",
             "name": "eat"
         },
         {
             "calorie": -375,
             "date": "2023-04-27",
             "name": "sport"
+        },
+        {
+            "name": "drink"
+        }
+    ],
+    "age": 23,
+    "country": "China",
+    "gender": "纯爷们",
+    "money": 3.1415926,
+    "name": "Bob"
+}
+```
+
+#### Modify items
+
+```shell
+# modify money and actions[1]["name"]
+$ jsonfmt --set 'money=1000; actions[1].name=swim' test/example.json
+```
+
+*Output:*
+
+```json
+{
+    "actions": [
+        {
+            "calorie": 294.9,
+            "date": "2021-03-02",
+            "name": "eat"
+        },
+        {
+            "calorie": -375,
+            "date": "2023-04-27",
+            "name": "swim"
         }
     ],
     "age": 23,
     "gender": "纯爷们",
     "money": 1000,
-    "name": "Bob",
-    "skills": [
-        "Django",
-        "Flask"
-    ]
+    "name": "Bob"
 }
 ```
 
-#### Pop some items.
+#### Pop items
 
 ```shell
-# remove the gender field and actions[1]
-$ jsonfmt --pop 'gender;actions[1]' test/example.json
+# pop `gender` and actions[1]
+$ jsonfmt --pop 'gender; actions[1]' test/example.json
 ```
 
 *Output:*
 
 ```json
 {
     "actions": [
@@ -464,15 +579,15 @@
 Of course you can use `--set` and `--pop` together.
 
 ```shell
 jsonfmt --set 'skills=["Django","Flask"];money=1000' --pop 'gender;actions[1]' test/example.json
 ```
 
 **Note**, however, that the above command will not modify the original JSON file.
-If you want to do this, then please read below.
+If you want to do this, read below please.
 
 ### 7. Output to file.
 
 - use the `-O` parameter to overwrite the file with the result.
 
     This option will be forced to close when `-o` is specified
```

### Comparing `jsonfmt-0.2.5/jsonfmt.egg-info/PKG-INFO` & `jsonfmt-0.2.6/jsonfmt.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonfmt
-Version: 0.2.5
+Version: 0.2.6
 Summary: A simple tool for formatting JSON object.
 Author-email: Seamile <lanhuermao@gmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/seamile/jsonfmt
 Project-URL: repository, https://github.com/seamile/jsonfmt
 Project-URL: documentation, https://seamile.github.io/jsonfmt/
 Keywords: json,formatter,pretty-print,highlight,jmespath
@@ -18,49 +18,53 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: File Formats :: JSON
 Classifier: Topic :: Printing
 Classifier: Topic :: Utilities
-Requires-Python: >=3.8
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # JSON Formatter
 
 [![Build Status](https://github.com/seamile/jsonfmt/actions/workflows/python-package.yml/badge.svg)](https://github.com/seamile/jsonfmt/actions)
 [![PyPI Version](https://img.shields.io/pypi/v/jsonfmt?color=blue&label=Version&logo=python&logoColor=white)](https://pypi.org/project/jsonfmt/)
 [![Installs](https://static.pepy.tech/personalized-badge/jsonfmt?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Installs)](https://pepy.tech/project/jsonfmt)
 [![Code Grade](https://app.codacy.com/project/badge/Grade/1e12e3cd8c8342bca68db4caf5b6a31d)](https://app.codacy.com/gh/seamile/jsonfmt/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 [![Test Coverage](https://app.codacy.com/project/badge/Coverage/1e12e3cd8c8342bca68db4caf5b6a31d)](https://app.codacy.com/gh/seamile/jsonfmt/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage)
 
-**jsonfmt** is a powerful tool for handling JSON document.
+**jsonfmt** is a powerful tool for pretty-printing, querying and conversion JSON documents.
 
-It is as powerful as [jq](https://github.com/jqlang/jq), but simpler.
+It is as powerful as [jq](https://github.com/jqlang/jq), but easier to use.
 
 
 ## Features
 
 - [1. Pretty print JSON document.](#1-pretty-print-json-document)
     - [Syntax hight and indenation.](#syntax-hight-and-indenation)
     - [Read JSON from pipeline.](#read-json-from-pipeline)
 - [2. Features for handling large JSON document.](#2-features-for-handling-large-json-document)
     - [View a large JSON with pager-mode.](#view-a-large-json-with-pager-mode)
     - [Show the overview of a large JSON.](#show-the-overview-of-a-large-json)
     - [Copy the result to clipboard.](#copy-the-result-to-clipboard)
 - [3. Minimize the JSON document.](#3-minimize-the-json-document)
-- [4. Pick out parts of a large JSON via JmesPath.](#4-pick-out-parts-of-a-large-json-via-jmespath)
+- [4. Pick out parts of a large JSON via JMESPath or JSONPath.](#4-pick-out-parts-of-a-large-json-via-jmespath-or-jsonpath)
+    - [JMESPath examples](#jmespath-examples)
+    - [JSONPath examples](#jsonpath-examples)
+    - [Query for TOML and YAML](#query-for-toml-and-yaml)
 - [5. Convert formats between JSON, TOML and YAML.](#5-convert-formats-between-json-toml-and-yaml)
     - [JSON to TOML and YAML](#json-to-toml-and-yaml)
     - [TOML to JSON and YAML](#toml-to-json-and-yaml)
     - [YAML to JSON and TOML](#yaml-to-json-and-toml)
 - [6. Modify some values in the input data.](#6-modify-some-values-in-the-input-data)
-    - [Add and modify some items.](#add-and-modify-some-items)
-    - [Pop some items.](#pop-some-items)
+    - [Add items](#add-items)
+    - [Modify items](#modify-items)
+    - [Pop items](#pop-items)
 - [7. Output to file.](#7-output-to-file)
 
 
 ## Install
 
 ```shell
 $ pip install jsonfmt
@@ -79,19 +83,20 @@
 
 - Options:
 
     - `-h, --help`: show this help message and exit
     - `-c`: suppress all whitespace separation
     - `-C`: copy the result to clipboard
     - `-e`: escape non-ASCII characters
-    - `-f {json,toml,yaml}`: the format to output (default: None)
+    - `-f {json,toml,yaml}`: the format to output (default: same as input)
     - `-i {0-8,t}`: number of spaces for indentation (default: 2)
     - `-o`: show data structure overview
     - `-O`: overwrite the formated text to original file
-    - `-p JSONPATH`: output part of the object via jmespath
+    - `-l {jmespath,jsonpath}`: the language for querying (default: jmespath)
+    - `-p QUERYPATH`: the path for querying
     - `-s`: sort keys of objects on output
     - `--set 'foo.k1=v1;k2[i]=v2'`: set the keys to values (seperated by `;`)
     - `--pop 'k1;foo.k2;k3[i]'`: pop the specified keys (seperated by `;`)
     - `-v`: show the version
 
 
 ## Example
@@ -160,19 +165,26 @@
 
 The pager-mode is similar to the command `more`.
 
 *jsonfmt* will automatically present the result in pager-mode when the JSON document is too large to overflow the window display area.
 
 The key-binding of the pager-mode is same as command `more`:
 
-- <kbd>j</kbd> / <kbd>k</kbd> to forward / backward by line.
-- <kbd>f</kbd> or <kbd>ctrl</kbd>+<kbd>f</kbd> to forward by page.
-- <kbd>b</kbd> or <kbd>ctrl</kbd>+<kbd>b</kbd> to backward by page.
-- <kbd>g</kbd> to go to the top of the page, and <kbd>G</kbd> to the bottom.
-- <kbd>q</kbd> to exit.
+| key                          | description               |
+|------------------------------|---------------------------|
+| <kbd>j</kbd>                 | forward  by line          |
+| <kbd>k</kbd>                 | backward by line          |
+| <kbd>f</kbd>                 | forward by page           |
+| <kbd>ctrl</kbd>+<kbd>f</kbd> | forward by page           |
+| <kbd>b</kbd>                 | backward by page          |
+| <kbd>ctrl</kbd>+<kbd>b</kbd> | backward by page          |
+| <kbd>g</kbd>                 | go to the top of the page |
+| <kbd>G</kbd>                 | go to the bottom          |
+| <kbd>/</kbd>                 | search mode               |
+| <kbd>q</kbd>                 | quit pager-mode           |
 
 There is a big JSON from GitHub, you can paste this command into terminal to try the pager-mode:
 
 ```shell
 curl -s 'https://api.github.com/repos/seamile/jsonfmt/commits?per_page=10' | jsonfmt
 ```
 
@@ -238,25 +250,23 @@
 
 *Output:*
 
 ```json
 {"age":21,"items":["pen","phone"],"name":"alex"}
 ```
 
-### 4. Pick out parts of a large JSON via JmesPath.
+### 4. Pick out parts of a large JSON via JMESPath or JSONPath.
 
-Unlike from jq's private solution, `jsonfmt` uses [JmesPath](https://jmespath.org/) as its query language.
+Unlike from jq's private solution, `jsonfmt` uses both [JMESPath](https://jmespath.org/) and [JSONPath](https://datatracker.ietf.org/doc/id/draft-goessner-dispatch-jsonpath-00.html) as its query language.
 
-Among the many JSON query languages, `JmesPath` is the most popular one ([compared here](https://npmtrends.com/JSONPath-vs-jmespath-vs-jq-vs-json-path-vs-json-query-vs-jsonata-vs-jsonpath-vs-jsonpath-plus-vs-node-jq)).
-It is more general than `jq`, and more intuitive and powerful than `JsonPath`.
+Among the many JSON query languages, `JMESPath` is the most popular one ([compared here](https://npmtrends.com/JSONPath-vs-jmespath-vs-jq-vs-json-path-vs-json-query-vs-jsonata-vs-jsonpath-vs-jsonpath-plus-vs-node-jq)). It is more general than `jq`, and more intuitive and powerful than `JSONPath`. So I prefer to use it.
 
-Like the XPath for xml, `JmesPath` can elegantly extract parts of a given JSON document with simple syntax.
-See the tutorial [here](https://jmespath.org/tutorial.html).
+Like the XPath for xml, `JMESPath` can elegantly extract parts of a given JSON document with simple syntax. The official tutorial of JMESPath is [here](https://jmespath.org/tutorial.html).
 
-Some examples:
+#### JMESPath examples
 
 - pick out the first actions in `example.json`
 
     ```shell
     $ jsonfmt -p 'actions[0]' test/example.json
     ```
 
@@ -287,15 +297,15 @@
         }
     ]
     ```
 
 - Show all the keys and actions' length.
 
     ```shell
-    $ jsonfmt  -p '{all_keys:keys(@), actions_len:length(actions)}' test/example.json
+    $ jsonfmt -p '{all_keys:keys(@), actions_len:length(actions)}' test/example.json
     ```
 
     *Output:*
 
     ```json
     {
         "all_keys": [
@@ -326,35 +336,82 @@
         {
             "name": "eat",
             "calorie": 294.9
         }
     ]
     ```
 
-- [More examples](https://jmespath.org/examples.html).
+[More examples of JMESPath](https://jmespath.org/examples.html).
 
+#### JSONPath examples
 
-**Amazingly**, you can do the same with YAML and TOML using JmesPath, and convert the result format arbitrarily.
+The syntax of `JSONPath` is very similar to that of `JMESPath`. Everything that `JSONPath` can do `JMESPath` can also do, except using relative path querying. So `JSONPath` can be used as a supplementary query method of `JMESPath`.
 
-```shell
-# read the data from toml file, and convert the result to yaml
-$ jsonfmt  -p '{all_keys:keys(@), actions_len:length(actions)}' test/example.yaml -f toml
-```
+- Filter all `name` fields by relative path:
 
-*Output:*
+    ```shell
+    # use `-l` to specify the query language of JSON
+    $ jsonfmt.py -l jsonpath -p '$..name' test/example.json
+    ```
 
-```yaml
-all_keys:
-- age
-- gender
-- money
-- name
-- actions
-actions_len: 2
-```
+    *Output:*
+
+    ```json
+    [
+        "Bob",
+        "eat",
+        "sport"
+    ]
+    ```
+
+#### Query for TOML and YAML
+
+**Amazingly**, you can do all of the above with TOML and YAML in the same way, and convert the result format arbitrarily. It is even possible to process all three formats simultaneously in a single command.
+
+- Read the data from toml file, and convert the result to yaml
+
+    ```shell
+    $ jsonfmt -p '{all_keys:keys(@), actions_len:length(actions)}' test/example.toml -f yaml
+    ```
+
+    *Output:*
+
+    ```yaml
+    all_keys:
+    - age
+    - gender
+    - money
+    - name
+    - actions
+    actions_len: 2
+    ```
+
+- Handle three formats simultaneously
+
+    ```shell
+    $ jsonfmt.py -p 'actions[0]' test/example.json test/example.toml test/example.yaml
+    ```
+
+    *Output:*
+
+    ```
+    {
+        "calorie": 294.9,
+        "date": "2021-03-02",
+        "name": "eat"
+    }
+
+    calorie = 294.9
+    date = "2021-03-02"
+    name = "eat"
+
+    calorie: 294.9
+    date: '2021-03-02'
+    name: eat
+    ```
 
 
 ### 5. Convert formats between JSON, TOML and YAML.
 
 The *jsonfmt* can recognize any format of JSON, TOML and YAML from files or `stdin`. Either formats can be converted to the other by specifying the "-f" option.
 
 <div style="color: orange"><strong>Note that:</strong></div>
@@ -423,23 +480,23 @@
 $ jsonfmt test/example.yaml -f toml
 ```
 
 ### 6. Modify some values in the input data.
 
 Use the `--set` and `--pop` options when you want to change something in the input documents.
 
-The format is `--set 'key1=value1'`. When you need to modify multiple values ​​you can use `;` to separate: `--set 'k1=v1;k2=v2'`. If the key-value pair dose not exist, it will be added.
+The format is `--set 'key=value'`. When you need to modify multiple values ​​you can use `;` to separate: `--set 'k1=v1;k2=v2'`. If the key-value pair dose not exist, it will be added.
 
-For the items in list, use `key[i]` or `key.i` to specify. But it doesn't support adding new elements.
+For the items in list, use `key[i]` or `key.i` to specify. If the index is greater than or equal to the number of elements, the value will be appended.
 
-#### Add and modify some items.
+#### Add items
 
 ```shell
-# add a key-value pair and modify the money field
-$ jsonfmt --set 'skills=["Django","Flask"];money=1000' test/example.json
+# add `country` key and append one item for `actions`
+$ jsonfmt --set 'country=China; actions[2]={"name": "drink"}' test/example.json
 ```
 
 *Output:*
 
 ```json
 {
     "actions": [
@@ -448,32 +505,62 @@
             "date": "2021-03-02",
             "name": "eat"
         },
         {
             "calorie": -375,
             "date": "2023-04-27",
             "name": "sport"
+        },
+        {
+            "name": "drink"
+        }
+    ],
+    "age": 23,
+    "country": "China",
+    "gender": "纯爷们",
+    "money": 3.1415926,
+    "name": "Bob"
+}
+```
+
+#### Modify items
+
+```shell
+# modify money and actions[1]["name"]
+$ jsonfmt --set 'money=1000; actions[1].name=swim' test/example.json
+```
+
+*Output:*
+
+```json
+{
+    "actions": [
+        {
+            "calorie": 294.9,
+            "date": "2021-03-02",
+            "name": "eat"
+        },
+        {
+            "calorie": -375,
+            "date": "2023-04-27",
+            "name": "swim"
         }
     ],
     "age": 23,
     "gender": "纯爷们",
     "money": 1000,
-    "name": "Bob",
-    "skills": [
-        "Django",
-        "Flask"
-    ]
+    "name": "Bob"
 }
 ```
 
-#### Pop some items.
+#### Pop items
 
 ```shell
-# remove the gender field and actions[1]
-$ jsonfmt --pop 'gender;actions[1]' test/example.json
+# pop `gender` and actions[1]
+$ jsonfmt --pop 'gender; actions[1]' test/example.json
 ```
 
 *Output:*
 
 ```json
 {
     "actions": [
@@ -492,15 +579,15 @@
 Of course you can use `--set` and `--pop` together.
 
 ```shell
 jsonfmt --set 'skills=["Django","Flask"];money=1000' --pop 'gender;actions[1]' test/example.json
 ```
 
 **Note**, however, that the above command will not modify the original JSON file.
-If you want to do this, then please read below.
+If you want to do this, read below please.
 
 ### 7. Output to file.
 
 - use the `-O` parameter to overwrite the file with the result.
 
     This option will be forced to close when `-o` is specified
```

### Comparing `jsonfmt-0.2.5/jsonfmt.py` & `jsonfmt-0.2.6/jsonfmt.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,27 +10,32 @@
 from io import TextIOBase
 from pydoc import pager
 from shutil import get_terminal_size
 from sys import stdin, stdout, stderr, exit as sys_exit
 from typing import Any, List, IO, Optional, Sequence, Tuple, Union
 from unittest.mock import patch
 
-import jmespath
 import pyperclip
+from jmespath import compile as jcompile
 from jmespath.exceptions import JMESPathError
-from jmespath.parser import ParsedResult
+from jmespath.parser import ParsedResult as JMESPath
+from jsonpath_ng import JSONPath
+from jsonpath_ng import parse as jparse
+from jsonpath_ng.exceptions import JSONPathError
 from pygments import highlight
 from pygments.formatters import TerminalFormatter
 from pygments.lexers import JsonLexer, TOMLLexer, YamlLexer
 
-__version__ = '0.2.5'
+__version__ = '0.2.6'
 
 NUMERIC = re.compile(r'-?\d+$|-?\d+\.\d+$|^-?\d+\.?\d+e-?\d+$')
 DICT_OR_LIST = re.compile(r'^\{.*\}$|^\[.*\]$')
 
+QueryPath = Union[JMESPath, JSONPath]
+
 
 def print_inf(msg: Any):
     print(f'\033[1;94mjsonfmt:\033[0m \033[0;94m{msg}\033[0m', file=stderr)
 
 
 def print_err(msg: Any):
     print(f'\033[1;91mjsonfmt:\033[0m \033[0;91m{msg}\033[0m', file=stderr)
@@ -43,15 +48,30 @@
 def is_clipboard_available() -> bool:
     '''check if the clipboard available'''
     copy_fn, paste_fn = pyperclip.determine_clipboard()
     return copy_fn.__class__.__name__ != 'ClipboardUnavailable' \
         and paste_fn.__class__.__name__ != 'ClipboardUnavailable'
 
 
-def parse_to_pyobj(text: str, jpath: Optional[ParsedResult]) -> Tuple[Any, str]:
+def extract_elements(qpath: QueryPath, py_obj: Any) -> Any:
+    '''find and extract elements via JMESPath or JSONPath'''
+    if isinstance(qpath, JMESPath):
+        return qpath.search(py_obj)
+    else:
+        items = [matched.value for matched in qpath.find(py_obj)]
+        n_items = len(items)
+        if n_items == 0:
+            return None
+        elif n_items == 1:
+            return items[0]
+        else:
+            return items
+
+
+def parse_to_pyobj(text: str, qpath: Optional[QueryPath]) -> Tuple[Any, str]:
     '''read json, toml or yaml from IO and then match sub-element by jmespath'''
     # parse json, toml or yaml to python object
     loads_methods = {
         'json': json.loads,
         'toml': toml.loads,
         'yaml': partial(yaml.load, Loader=yaml.Loader),
     }
@@ -62,29 +82,34 @@
             py_obj = fn_loads(text)
             break
         except Exception:
             continue
     else:
         raise FormatError("no json, toml or yaml found in the text")
 
-    if jpath is None:
+    if qpath is None:
         return py_obj, fmt
     else:
-        # match sub-elements via jmespath
-        return jpath.search(py_obj), fmt
+        # match sub-elements via jmespath or jsonpath
+        return extract_elements(qpath, py_obj), fmt
 
 
-def forward_by_keys(py_obj: Any, keys: str) -> Tuple[Any, Union[str, int]]:
-    next_k = lambda obj, k: int(k) if isinstance(obj, list) else k
+def traverse_to_bottom(py_obj: Any, keys: str) -> Tuple[Any, Union[str, int]]:
+    '''traverse the nested py_obj to bottom by keys'''
+    def key_or_idx(obj: Any, key: str):
+        '''return str for dict and int for list'''
+        return int(key) if isinstance(obj, list) else key
 
+    # make sure the keys joined by `.`, and then split
     _keys = keys.replace(']', '').replace('[', '.').split('.')
+
     for k in _keys[:-1]:
-        py_obj = py_obj[next_k(py_obj, k)]
+        py_obj = py_obj[key_or_idx(py_obj, k)]
     else:
-        return py_obj, next_k(py_obj, _keys[-1])
+        return py_obj, key_or_idx(py_obj, _keys[-1])
 
 
 def load_value(value: str):
     if NUMERIC.match(value):
         return eval(value)
     elif DICT_OR_LIST.match(value):
         try:
@@ -92,26 +117,30 @@
         except Exception:
             return value
     else:
         return value
 
 
 def modify_pyobj(py_obj: Any, sets: List[str], pops: List[str]):
+    '''add, modify or pop items for PyObj'''
     for kv in sets:
         try:
             keys, value = kv.split('=')
-            bottom, last_k = forward_by_keys(py_obj, keys)
-            bottom[last_k] = load_value(value)
-        except (IndexError, KeyError, ValueError):
+            bottom, last_k = traverse_to_bottom(py_obj, keys)
+            if isinstance(bottom, list) and len(bottom) <= last_k:  # type: ignore
+                bottom.append(load_value(value))
+            else:
+                bottom[last_k] = load_value(value)  # type: ignore
+        except (IndexError, KeyError, ValueError, TypeError):
             print_err(f'invalid key path: {kv}')
             continue
 
     for keys in pops:
         try:
-            bottom, last_k = forward_by_keys(py_obj, keys)
+            bottom, last_k = traverse_to_bottom(py_obj, keys)
             bottom.pop(last_k)
         except (IndexError, KeyError):
             print_err(f'invalid key path: {keys}')
             continue
 
 
 def get_overview(py_obj: Any):
@@ -134,18 +163,18 @@
 def format_to_text(py_obj: Any, fmt: str, *,
                    compact: bool, escape: bool,
                    indent: Union[int, str], sort_keys: bool) -> str:
     '''format the py_obj to text'''
     if fmt == 'json':
         if compact:
             return json.dumps(py_obj, ensure_ascii=escape, sort_keys=sort_keys,
-                              separators=(',', ':'))
+                              separators=(',', ':')) + '\n'
         else:
             return json.dumps(py_obj, ensure_ascii=escape, sort_keys=sort_keys,
-                              indent=indent)
+                              indent=indent) + '\n'
 
     elif fmt == 'toml':
         if not isinstance(py_obj, dict):
             msg = 'the pyobj must be a Mapping when format to toml'
             raise FormatError(msg)
         return toml.dumps(py_obj)
 
@@ -172,68 +201,74 @@
         # use pager when line-hight > screen hight or
         if text.count('\n') >= win_h or len(text) > win_w * (win_h - 1):
             with patch("sys.stdin.isatty", lambda *_: True):
                 pager(colored_text)
         else:
             output_fp.write(colored_text)
     else:
-        output_fp.seek(0)
-        output_fp.truncate()
+        if output_fp.fileno() > 2:
+            output_fp.seek(0)
+            output_fp.truncate()
+
         output_fp.write(text)
+
         if output_fp.fileno() > 2:
             print_inf(f'result written to {output_fp.name}')
 
 
-def process(input_fp: IO, jpath: Optional[ParsedResult], convert_fmt: Optional[str],
+def process(input_fp: IO, qpath: Optional[QueryPath], to_fmt: Optional[str],
             *, compact: bool, cp2clip: bool, escape: bool, indent: Union[int, str],
             overview: bool, overwrite: bool, sort_keys: bool,
             sets: Optional[list], pops: Optional[list]):
     # parse and format
     input_text = input_fp.read()
-    py_obj, fmt = parse_to_pyobj(input_text, jpath)
+    py_obj, fmt = parse_to_pyobj(input_text, qpath)
 
     if sets or pops:
         modify_pyobj(py_obj, sets, pops)  # type: ignore
 
     if overview:
         py_obj = get_overview(py_obj)
 
-    convert_fmt = convert_fmt or fmt
-    formated_text = format_to_text(py_obj, convert_fmt,
+    to_fmt = to_fmt or fmt
+    formated_text = format_to_text(py_obj, to_fmt,
                                    compact=compact, escape=escape,
                                    indent=indent, sort_keys=sort_keys)
 
     # output the result
     if input_fp.name == '<stdin>' or not overwrite:
         output_fp = stdout
     else:
         # truncate file to zero length before overwrite
         output_fp = input_fp
-    output(output_fp, formated_text, convert_fmt, cp2clip)
+    output(output_fp, formated_text, to_fmt, cp2clip)
 
 
 def parse_cmdline_args(args: Optional[Sequence[str]] = None):
     parser = ArgumentParser('jsonfmt')
     parser.add_argument('-c', dest='compact', action='store_true',
                         help='suppress all whitespace separation')
     parser.add_argument('-C', dest='cp2clip', action='store_true',
                         help='copy the result to clipboard')
     parser.add_argument('-e', dest='escape', action='store_true',
                         help='escape non-ASCII characters')
     parser.add_argument('-f', dest='format', choices=['json', 'toml', 'yaml'],
-                        help='the format to output ''(default: %(default)s)')
+                        help='the format to output (default: same as input)')
     parser.add_argument('-i', dest='indent', metavar='{0-8,t}',
                         choices='012345678t', default='2',
                         help='number of spaces for indentation (default: %(default)s)')
     parser.add_argument('-o', dest='overview', action='store_true',
                         help='show data structure overview')
     parser.add_argument('-O', dest='overwrite', action='store_true',
                         help='overwrite the formated text to original file')
-    parser.add_argument('-p', dest='jmespath', type=str,
-                        help='output part of the object via jmespath')
+    parser.add_argument('-l', dest='querylang', default='jmespath',
+                        choices=['jmespath', 'jsonpath'],
+                        help='the language for querying (default: %(default)s)')
+    parser.add_argument('-p', dest='querypath', type=str,
+                        help='the path for querying')
     parser.add_argument('-s', dest='sort_keys', action='store_true',
                         help='sort keys of objects on output')
     parser.add_argument('--set', metavar="'foo.k1=v1;k2[i]=v2'",
                         help='set the keys to values (seperated by `;`)')
     parser.add_argument('--pop', metavar="'k1;foo.k2;k3[i]'",
                         help='pop the specified keys (seperated by `;`)')
     parser.add_argument(dest='files', nargs='*',
@@ -242,19 +277,23 @@
                         version=__version__, help="show the version")
     return parser.parse_args(args)
 
 
 def main():
     args = parse_cmdline_args()
 
-    try:
-        jpath = None if args.jmespath is None else jmespath.compile(args.jmespath)
-    except JMESPathError:
-        print_err(f'invalid JMESPath expression: {args.jmespath}')
-        sys_exit(1)
+    if args.querypath is None:
+        querypath = None
+    else:
+        parse_path = {'jmespath': jcompile, 'jsonpath': jparse}[args.querylang]
+        try:
+            querypath = parse_path(args.querypath)
+        except (JMESPathError, JSONPathError, AttributeError):
+            print_err(f'invalid querypath expression: "{args.querypath}"')
+            sys_exit(1)
 
     # check if the clipboard is available
     cp2clip = args.cp2clip and is_clipboard_available()
     if args.cp2clip and not cp2clip:
         print_err('clipboard unavailable')
 
     # check the indent
@@ -264,34 +303,36 @@
     overwrite = False if args.overview else args.overwrite
 
     # get sets and pops
     sets = [k.strip() for k in args.set.split(';')] if args.set else []
     pops = [k.strip() for k in args.pop.split(';')] if args.pop else []
 
     files = args.files or [stdin]
+    files_cnt = len(files)
 
-    for file in files:
+    for num, file in enumerate(files, start=1):
         try:
             # read from file
             input_fp = open(file, 'r+') if isinstance(file, str) else file
             process(input_fp,
-                    jpath,
+                    querypath,
                     args.format,
                     compact=args.compact,
                     cp2clip=cp2clip,
                     escape=args.escape,
                     indent=indent,
                     overview=args.overview,
                     overwrite=overwrite,
                     sort_keys=args.sort_keys,
                     sets=sets,
                     pops=pops)
-        except FormatError as err:
-            print_err(err)
-        except JMESPathError as err:
+            # output a line to separate multiple results
+            if num < files_cnt:
+                print('----------------', file=stdout)
+        except (FormatError, JMESPathError, JSONPathError) as err:
             print_err(err)
         except FileNotFoundError:
             print_err(f'no such file: {file}')
         except PermissionError:
             print_err(f'permission denied: {file}')
         finally:
             input_fp = locals().get('input_fp')
```

### Comparing `jsonfmt-0.2.5/pyproject.toml` & `jsonfmt-0.2.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,20 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jsonfmt"
-dynamic = ["version"]
-requires-python = ">=3.8"
+dynamic = ["dependencies", "version"]
+requires-python = ">=3.6"
 license = {text = "MIT License"}
 description = "A simple tool for formatting JSON object."
 readme = "README.md"
 keywords = ["json", "formatter", "pretty-print", "highlight", "jmespath"]
 authors = [{name = "Seamile", email = "lanhuermao@gmail.com"}]
-dependencies = [
-    "jmespath >= 1.0.1",
-    "Pygments >= 2.13.0",
-    "pyperclip >= 1.8.2",
-    "pyyaml >= 6.0",
-    "toml >= 0.10.2"
-]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
@@ -37,11 +30,12 @@
 
 [project.urls]
 homepage = "https://github.com/seamile/jsonfmt"
 repository = "https://github.com/seamile/jsonfmt"
 documentation = "https://seamile.github.io/jsonfmt/"
 
 [tool.setuptools.dynamic]
+dependencies = {file = ["requirements.txt"]}
 version = {attr = "jsonfmt.__version__" }
 
 [project.scripts]
 jsonfmt = "jsonfmt:main"
```

### Comparing `jsonfmt-0.2.5/test/test.py` & `jsonfmt-0.2.6/test/test.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import tempfile
 import unittest
 import pyperclip
 from argparse import Namespace
 from copy import deepcopy
 from functools import partial
 from io import StringIO
-from jmespath import compile as jp_compile
+from jmespath import compile as jcompile
+from jsonpath_ng import parse as jparse
 from pygments import highlight
 from pygments.formatters import TerminalFormatter
 from pygments.lexers import JsonLexer, YamlLexer, TOMLLexer
 from unittest.mock import patch
 
 BASE_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 sys.path.insert(0, BASE_DIR)
@@ -90,53 +91,66 @@
         self.maxDiff = None
         self.py_obj = json.loads(JSON_TEXT)
 
     def test_is_clipboard_available(self):
         available = jsonfmt.is_clipboard_available()
         self.assertIsInstance(available, bool)
 
-    def test_parse_to_pyobj(self):
+    def test_parse_to_pyobj_with_jmespath(self):
         # normal parameters test
-        matched_obj = jsonfmt.parse_to_pyobj(JSON_TEXT, jp_compile("actions[:].calorie"))
+        matched_obj = jsonfmt.parse_to_pyobj(JSON_TEXT, jcompile("actions[:].calorie"))
         self.assertEqual(matched_obj, ([294.9, -375], 'json'))
-        matched_obj = jsonfmt.parse_to_pyobj(TOML_TEXT, jp_compile("actions[*].name"))
+        matched_obj = jsonfmt.parse_to_pyobj(TOML_TEXT, jcompile("actions[*].name"))
         self.assertEqual(matched_obj, (['eat', 'sport'], 'toml'))
-        matched_obj = jsonfmt.parse_to_pyobj(YAML_TEXT, jp_compile("actions[*].date"))
+        matched_obj = jsonfmt.parse_to_pyobj(YAML_TEXT, jcompile("actions[*].date"))
         self.assertEqual(matched_obj, (['2021-03-02', '2023-04-27'], 'yaml'))
         # test not exists key
-        matched_obj = jsonfmt.parse_to_pyobj(TOML_TEXT, jp_compile("not_exist_key"))
+        matched_obj = jsonfmt.parse_to_pyobj(TOML_TEXT, jcompile("not_exist_key"))
         self.assertEqual(matched_obj, (None, 'toml'))
         # test index out of range
-        matched_obj = jsonfmt.parse_to_pyobj(YAML_TEXT, jp_compile('actions[7]'))
+        matched_obj = jsonfmt.parse_to_pyobj(YAML_TEXT, jcompile('actions[7]'))
         self.assertEqual(matched_obj, (None, 'yaml'))
 
-        # test empty jmespath
-        with patch('jsonfmt.stderr', FakeStdErr()), self.assertRaises(jsonfmt.JMESPathError):
-            matched_obj = jsonfmt.parse_to_pyobj(JSON_TEXT, jp_compile(""))
+    def test_parse_to_pyobj_with_jsonpath(self):
+        # normal parameters test
+        matched_obj = jsonfmt.parse_to_pyobj(JSON_TEXT, jparse("age"))
+        self.assertEqual(matched_obj, (23, 'json'))
+        matched_obj = jsonfmt.parse_to_pyobj(TOML_TEXT, jparse("$..name"))
+        self.assertEqual(matched_obj, (['Bob', 'eat', 'sport'], 'toml'))
+        matched_obj = jsonfmt.parse_to_pyobj(YAML_TEXT, jparse("actions[*].date"))
+        self.assertEqual(matched_obj, (['2021-03-02', '2023-04-27'], 'yaml'))
+        # test not exists key
+        matched_obj = jsonfmt.parse_to_pyobj(TOML_TEXT, jparse("not_exist_key"))
+        self.assertEqual(matched_obj, (None, 'toml'))
+        # test index out of range
+        matched_obj = jsonfmt.parse_to_pyobj(YAML_TEXT, jparse('actions[7]'))
+        self.assertEqual(matched_obj, (None, 'yaml'))
 
-        # test for unsupported format
+    def test_parse_to_pyobj_with_wrong_fmt(self):
         with self.assertRaises(jsonfmt.FormatError), open(__file__) as fp:
-            text = fp.read()
-            matched_obj = jsonfmt.parse_to_pyobj(text, jp_compile("actions[0].calorie"))
+            jsonfmt.parse_to_pyobj(fp.read(), jcompile("actions[0].calorie"))
 
     def test_modify_pyobj_for_adding(self):
         # test empty sets and pops
         obj = deepcopy(self.py_obj)
         jsonfmt.modify_pyobj(obj, [], [])
         self.assertEqual(obj, self.py_obj)
 
         # test add new value
         obj = deepcopy(self.py_obj)
-        # add single value
-        jsonfmt.modify_pyobj(obj, ['new1=value1'], [])
-        self.assertEqual(obj['new1'], 'value1')
+        # add single value to dict
+        jsonfmt.modify_pyobj(obj, ['new=value'], [])
+        self.assertEqual(obj['new'], 'value')
+        # add single value to list
+        jsonfmt.modify_pyobj(obj, ['actions[20]={"K":"V"}'], [])
+        self.assertEqual(obj['actions'][2], {"K": "V"})
         # add multiple values at once
-        jsonfmt.modify_pyobj(obj, ['new2={}', 'new3=[1,2,3]'], [])
-        self.assertEqual(obj['new2'], {})
-        self.assertEqual(obj['new3'], [1, 2, 3])
+        jsonfmt.modify_pyobj(obj, ['new=[1,2,3]', 'actions[50]={"K":"V"}'], [])
+        self.assertEqual(obj['new'], [1, 2, 3])
+        self.assertEqual(obj['actions'][2], {"K": "V"})
 
     def test_modify_pyobj_for_modifying(self):
         # test modify values
         obj = deepcopy(self.py_obj)
         # modify single value
         jsonfmt.modify_pyobj(obj, ['name=Alex'], [])
         self.assertEqual(obj['name'], 'Alex')
@@ -175,43 +189,56 @@
             jsonfmt.modify_pyobj(obj, ['aa.bb=empty'], [])
             self.assertIn('invalid key path', jsonfmt.stderr.read())
             # popping
             jsonfmt.modify_pyobj(obj, [], ['actions[3]'])
             self.assertIn('invalid key path', jsonfmt.stderr.read())
 
     def test_get_overview(self):
+        # test dict obj
         obj = deepcopy(self.py_obj)
         obj['dict'] = {"a": 7758, "b": [1, 2, 3]}
-        expected = {
+        expected_1 = {
             'actions': [],
             'age': 23,
             'gender': '...',
             'money': 3.1415926,
             'name': '...',
             'dict': {
                 'a': 7758,
                 'b': []
             }
         }
         overview = jsonfmt.get_overview(obj)
-        self.assertEqual(overview, expected)
+        self.assertEqual(overview, expected_1)
+
+        # test list obj
+        obj = deepcopy(self.py_obj['actions'])
+        expected_2 = [
+            {
+                "calorie": 294.9,
+                "date": "...",
+                "name": "..."
+            }
+        ]
+        overview = jsonfmt.get_overview(obj)
+        self.assertEqual(overview, expected_2)
 
     def test_format_to_text(self):
         py_obj = {"name": "约翰", "age": 30}
         # format to json (compacted)
         j_compacted = jsonfmt.format_to_text(py_obj, 'json',
                                              compact=True, escape=True,
                                              indent=4, sort_keys=False)
-        self.assertEqual(j_compacted, '{"name":"\\u7ea6\\u7ff0","age":30}')
+        self.assertEqual(j_compacted.strip(), '{"name":"\\u7ea6\\u7ff0","age":30}')
 
         # format to json (indentation)
         j_indented = jsonfmt.format_to_text(py_obj, 'json',
                                             compact=False, escape=False,
                                             indent=4, sort_keys=True)
-        self.assertEqual(j_indented, '{\n    "age": 30,\n    "name": "约翰"\n}')
+        self.assertEqual(j_indented.strip(), '{\n    "age": 30,\n    "name": "约翰"\n}')
 
         # format to toml
         toml_text = jsonfmt.format_to_text(self.py_obj, 'toml',
                                            compact=False, escape=False,
                                            indent=4, sort_keys=False)
         self.assertEqual(toml_text.strip(), TOML_TEXT.strip())
 
@@ -260,15 +287,16 @@
             compact=False,
             cp2clip=False,
             escape=False,
             format=None,
             indent='2',
             overview=False,
             overwrite=False,
-            jmespath=None,
+            querylang='jmespath',
+            querypath=None,
             sort_keys=False,
             set=None,
             pop=None,
             files=[]
         )
         actual_args = jsonfmt.parse_cmdline_args(args=[])
         self.assertEqual(actual_args, default_args)
@@ -278,14 +306,15 @@
             '-c',
             '-C',
             '-e',
             '-f', 'toml',
             '-i', '4',
             '-o',
             '-O',
+            '-l', 'jsonpath',
             '-p', 'path.to.json',
             '--set', 'a; b',
             '--pop', 'c; d',
             '-s',
             'file1.json',
             'file2.json'
         ]
@@ -293,29 +322,36 @@
             compact=True,
             cp2clip=True,
             escape=True,
             format='toml',
             indent='4',
             overview=True,
             overwrite=True,
-            jmespath='path.to.json',
+            querylang='jsonpath',
+            querypath='path.to.json',
             sort_keys=True,
             set='a; b',
             pop='c; d',
             files=['file1.json', 'file2.json']
         )
 
         actual_args = jsonfmt.parse_cmdline_args(args=args)
         self.assertEqual(actual_args, expected_args)
 
+    ############################################################################
+    #                                 main test                                #
+    ############################################################################
+
     @patch.multiple(sys, argv=['jsonfmt', '-i', 't', '-p', 'actions[*].name',
-                               JSON_FILE])
+                               JSON_FILE, YAML_FILE])
     @patch.multiple(jsonfmt, stdout=FakeStdOut())
     def test_main_with_file(self):
         expected_output = color('[\n\t"eat",\n\t"sport"\n]', 'json')
+        expected_output += '----------------\n'
+        expected_output += color('- eat\n- sport', 'yaml')
         jsonfmt.main()
         self.assertEqual(jsonfmt.stdout.read(), expected_output)
 
     @patch.multiple(sys, argv=['jsonfmt', '-f', 'yaml'])
     @patch.multiple(jsonfmt, stdin=FakeStdIn('["a", "b"]'), stdout=FakeStdOut())
     def test_main_with_stdin(self):
         expected_output = color('- a\n- b', 'yaml')
@@ -327,19 +363,27 @@
         # test not exist file and wrong format
         with patch.multiple(sys, argv=['jsonfmt', 'not_exist_file.json', __file__]):
             jsonfmt.main()
             errmsg = jsonfmt.stderr.read()
             self.assertIn('no such file: not_exist_file.json', errmsg)
             self.assertIn('no json, toml or yaml found', errmsg)
 
-        # test wrong jmespath
+    @patch.multiple(jsonfmt, stderr=FakeStdErr())
+    def test_main_querying(self):
+        # test empty jmespath
         with patch('sys.argv', ['jsonfmt', JSON_FILE, '-p', '$.-[=]']),\
                 self.assertRaises(SystemExit):
             jsonfmt.main()
-        self.assertIn('invalid JMESPath expression', jsonfmt.stderr.read())
+        self.assertIn('invalid querypath expression', jsonfmt.stderr.read())
+
+        # test empty jmespath
+        with patch('sys.argv', ['jsonfmt', JSON_FILE, '-l', 'jsonpath', '-p', ' ']),\
+                self.assertRaises(SystemExit):
+            jsonfmt.main()
+        self.assertIn('invalid querypath expression', jsonfmt.stderr.read())
 
     @patch('jsonfmt.stdout', FakeStdOut())
     def test_main_convert(self):
         # test json to toml
         with patch.multiple(sys, argv=['jsonfmt', '-f', 'toml', JSON_FILE]):
             colored_output = color(TOML_TEXT, 'toml')
             jsonfmt.main()
@@ -357,15 +401,15 @@
             jsonfmt.main()
             self.assertEqual(jsonfmt.stdout.read(), colored_output)
 
     @patch.multiple(sys, argv=['jsonfmt', '-oc'])
     @patch.multiple(jsonfmt, stdin=FakeStdIn('{"a": "asfd", "b": [1, 2, 3]}'), stdout=FakeStdOut(tty=False))
     def test_main_overview(self):
         jsonfmt.main()
-        self.assertEqual(jsonfmt.stdout.read(), '{"a":"...","b":[]}')
+        self.assertEqual(jsonfmt.stdout.read().strip(), '{"a":"...","b":[]}')
 
     @patch('sys.argv', ['jsonfmt', '-Ocsf', 'json', TOML_FILE])
     def test_main_overwrite_to_original_file(self):
         try:
             jsonfmt.main()
             with open(TOML_FILE) as toml_fp:
                 new_content = toml_fp.read().strip()
```

