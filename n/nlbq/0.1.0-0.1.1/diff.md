# Comparing `tmp/nlbq-0.1.0.tar.gz` & `tmp/nlbq-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlbq-0.1.0.tar", last modified: Thu Jun  8 14:26:08 2023, max compression
+gzip compressed data, was "nlbq-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `nlbq-0.1.0.tar` & `nlbq-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      505 2023-06-08 14:24:49.437083 nlbq-0.1.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      878 2023-06-08 14:24:49.437218 nlbq-0.1.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0     3108 2023-06-07 18:05:27.275604 nlbq-0.1.0/.gitignore
--rw-r--r--   0        0        0      258 2023-06-07 18:05:27.275843 nlbq-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1065 2023-05-25 16:02:19.967434 nlbq-0.1.0/LICENSE
--rw-r--r--   0        0        0     1039 2023-06-07 18:05:27.275969 nlbq-0.1.0/README.md
--rw-r--r--   0        0        0       58 2023-06-08 14:25:02.093118 nlbq-0.1.0/nlbq/__init__.py
--rw-r--r--   0        0        0     2395 2023-06-08 13:58:02.567130 nlbq-0.1.0/nlbq/api.py
--rw-r--r--   0        0        0     3679 2023-06-08 14:24:49.437473 nlbq-0.1.0/nlbq/cli.py
--rw-r--r--   0        0        0      435 2023-06-07 18:05:27.276859 nlbq-0.1.0/nlbq/config.py
--rw-r--r--   0        0        0     4333 2023-06-08 13:50:23.774181 nlbq-0.1.0/nlbq/core.py
--rw-r--r--   0        0        0     1476 2023-06-08 14:24:49.437699 nlbq-0.1.0/nlbq/helpers.py
--rw-r--r--   0        0        0      103 2023-06-07 18:05:27.277574 nlbq-0.1.0/nlbq/templates/Dockerfile
--rw-r--r--   0        0        0     7354 2023-06-08 13:58:02.567625 nlbq-0.1.0/nlbq/templates/index.html
--rw-r--r--   0        0        0     1460 2023-06-07 18:05:27.278013 nlbq-0.1.0/nlbq/templates/prompt.txt
--rw-r--r--   0        0        0      760 2023-06-07 18:05:27.278181 nlbq-0.1.0/nlbq/templates/prompt_template.txt
--rw-r--r--   0        0        0     1191 2023-06-07 18:05:27.278495 nlbq-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1607 1970-01-01 00:00:00.000000 nlbq-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      505 2023-06-13 15:46:24.829925 nlbq-0.1.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      878 2023-06-13 15:46:24.829925 nlbq-0.1.1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     3108 2023-06-13 15:46:24.829925 nlbq-0.1.1/.gitignore
+-rw-r--r--   0        0        0      258 2023-06-13 15:46:24.829925 nlbq-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1065 2023-06-13 15:46:24.829925 nlbq-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1039 2023-06-13 15:46:24.829925 nlbq-0.1.1/README.md
+-rw-r--r--   0        0        0       58 2023-06-13 15:46:24.829925 nlbq-0.1.1/nlbq/__init__.py
+-rw-r--r--   0        0        0     2431 2023-06-13 15:46:24.829925 nlbq-0.1.1/nlbq/api.py
+-rw-r--r--   0        0        0     3675 2023-06-13 15:46:24.829925 nlbq-0.1.1/nlbq/cli.py
+-rw-r--r--   0        0        0      631 2023-06-13 15:46:24.829925 nlbq-0.1.1/nlbq/config.py
+-rw-r--r--   0        0        0     4333 2023-06-13 15:46:24.829925 nlbq-0.1.1/nlbq/core.py
+-rw-r--r--   0        0        0     1476 2023-06-13 15:46:24.829925 nlbq-0.1.1/nlbq/helpers.py
+-rw-r--r--   0        0        0      103 2023-06-13 15:46:24.833925 nlbq-0.1.1/nlbq/templates/Dockerfile
+-rw-r--r--   0        0        0     7354 2023-06-13 15:46:24.833925 nlbq-0.1.1/nlbq/templates/index.html
+-rw-r--r--   0        0        0     1460 2023-06-13 15:46:24.833925 nlbq-0.1.1/nlbq/templates/prompt.txt
+-rw-r--r--   0        0        0      760 2023-06-13 15:46:24.833925 nlbq-0.1.1/nlbq/templates/prompt_template.txt
+-rw-r--r--   0        0        0     1191 2023-06-13 15:46:24.833925 nlbq-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1607 1970-01-01 00:00:00.000000 nlbq-0.1.1/PKG-INFO
```

### Comparing `nlbq-0.1.0/.github/workflows/publish.yml` & `nlbq-0.1.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `nlbq-0.1.0/.gitignore` & `nlbq-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `nlbq-0.1.0/LICENSE` & `nlbq-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nlbq-0.1.0/README.md` & `nlbq-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nlbq-0.1.0/nlbq/api.py` & `nlbq-0.1.1/nlbq/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,23 +8,21 @@
 from nlbq.config import get_settings
 from nlbq.core import NLBQ
 
 settings = get_settings()
 
 app = FastAPI()
 
-# Allow all origins
-origins = ["*"]
 
 app.add_middleware(
     CORSMiddleware,
-    allow_origins=origins,
-    allow_credentials=False,
-    allow_methods=["*"],
-    allow_headers=["*"],
+    allow_origins=settings.cors_origins,
+    allow_methods=settings.cors_methods,
+    allow_headers=settings.cors_headers,
+    allow_credentials=settings.cors_allow_credentials,
 )
 
 
 class DryRunRequest(BaseModel):
     question: str
     model: str
```

### Comparing `nlbq-0.1.0/nlbq/cli.py` & `nlbq-0.1.1/nlbq/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     if input("Do you want to run it? (Y/n) ").lower() not in ["y", ""]:
         sys.exit(0)
     fields, rows = nlbq.execute(statement)
     print("\n" + tabulate(rows, headers=fields, tablefmt="pipe") + "\n")
 
 
 def validate_table_format(table_in_dataset: str) -> str:
-    """Validate dataset format"""    
+    """Validate dataset format"""
     if table_in_dataset and "." not in table_in_dataset:
         raise typer.BadParameter(
             "The target table value must be in the format dataset.table_id"
         )
     return table_in_dataset
```

### Comparing `nlbq-0.1.0/nlbq/core.py` & `nlbq-0.1.1/nlbq/core.py`

 * *Files identical despite different names*

### Comparing `nlbq-0.1.0/nlbq/helpers.py` & `nlbq-0.1.1/nlbq/helpers.py`

 * *Files identical despite different names*

### Comparing `nlbq-0.1.0/nlbq/templates/index.html` & `nlbq-0.1.1/nlbq/templates/index.html`

 * *Files identical despite different names*

### Comparing `nlbq-0.1.0/nlbq/templates/prompt.txt` & `nlbq-0.1.1/nlbq/templates/prompt.txt`

 * *Files identical despite different names*

### Comparing `nlbq-0.1.0/nlbq/templates/prompt_template.txt` & `nlbq-0.1.1/nlbq/templates/prompt_template.txt`

 * *Files identical despite different names*

### Comparing `nlbq-0.1.0/pyproject.toml` & `nlbq-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nlbq-0.1.0/PKG-INFO` & `nlbq-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlbq
-Version: 0.1.0
+Version: 0.1.1
 Summary: Natural language to BigQuery
 Author: Tom Dyson, Dan Braghis
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: openai
 Requires-Dist: fastapi
```

