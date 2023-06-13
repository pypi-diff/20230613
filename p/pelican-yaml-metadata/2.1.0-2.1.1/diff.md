# Comparing `tmp/pelican_yaml_metadata-2.1.0.tar.gz` & `tmp/pelican_yaml_metadata-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Fri Jun  9 12:34:31 2023, max compression
+gzip compressed data, last modified: Tue Jun 13 01:19:33 2023, max compression
```

## Comparing `pelican_yaml_metadata-2.1.0.tar` & `pelican_yaml_metadata-2.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      201 2023-06-09 12:34:31.000000 pelican_yaml_metadata-2.1.0/.editorconfig
--rw-r--r--   0        0        0      741 2023-06-09 12:34:31.000000 pelican_yaml_metadata-2.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      636 2023-06-09 12:34:31.000000 pelican_yaml_metadata-2.1.0/CHANGELOG.md
--rw-r--r--   0        0        0      566 2023-06-09 12:34:31.000000 pelican_yaml_metadata-2.1.0/CONTRIBUTING.md
--rw-r--r--   0        0        0       60 2023-06-09 12:34:31.000000 pelican_yaml_metadata-2.1.0/RELEASE.md
--rw-r--r--   0        0        0     3130 2023-06-09 12:34:31.000000 pelican_yaml_metadata-2.1.0/tasks.py
--rw-r--r--   0        0        0     1460 2023-06-09 12:34:31.000000 pelican_yaml_metadata-2.1.0/.github/workflows/main.yml
--rw-r--r--   0        0        0       45 2023-06-09 12:34:31.000000 pelican_yaml_metadata-2.1.0/pelican/plugins/yaml_metadata/__init__.py
--rw-r--r--   0        0        0     5576 2023-06-09 12:34:31.000000 pelican_yaml_metadata-2.1.0/pelican/plugins/yaml_metadata/yaml_metadata.py
--rw-r--r--   0        0        0       44 2023-06-09 12:34:31.000000 pelican_yaml_metadata-2.1.0/.gitignore
--rw-r--r--   0        0        0     2568 2023-06-09 12:34:31.000000 pelican_yaml_metadata-2.1.0/README.md
--rw-r--r--   0        0        0     2701 2023-06-09 12:34:31.000000 pelican_yaml_metadata-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     3845 2023-06-09 12:34:31.000000 pelican_yaml_metadata-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0      201 2023-06-13 01:19:33.000000 pelican_yaml_metadata-2.1.1/.editorconfig
+-rw-r--r--   0        0        0      741 2023-06-13 01:19:33.000000 pelican_yaml_metadata-2.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      789 2023-06-13 01:19:33.000000 pelican_yaml_metadata-2.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0      566 2023-06-13 01:19:33.000000 pelican_yaml_metadata-2.1.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      135 2023-06-13 01:19:33.000000 pelican_yaml_metadata-2.1.1/RELEASE.md
+-rw-r--r--   0        0        0     3130 2023-06-13 01:19:33.000000 pelican_yaml_metadata-2.1.1/tasks.py
+-rw-r--r--   0        0        0     1460 2023-06-13 01:19:33.000000 pelican_yaml_metadata-2.1.1/.github/workflows/main.yml
+-rw-r--r--   0        0        0       45 2023-06-13 01:19:33.000000 pelican_yaml_metadata-2.1.1/pelican/plugins/yaml_metadata/__init__.py
+-rw-r--r--   0        0        0     5873 2023-06-13 01:19:33.000000 pelican_yaml_metadata-2.1.1/pelican/plugins/yaml_metadata/yaml_metadata.py
+-rw-r--r--   0        0        0       44 2023-06-13 01:19:33.000000 pelican_yaml_metadata-2.1.1/.gitignore
+-rw-r--r--   0        0        0     2568 2023-06-13 01:19:33.000000 pelican_yaml_metadata-2.1.1/README.md
+-rw-r--r--   0        0        0     2701 2023-06-13 01:19:33.000000 pelican_yaml_metadata-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3845 2023-06-13 01:19:33.000000 pelican_yaml_metadata-2.1.1/PKG-INFO
```

### Comparing `pelican_yaml_metadata-2.1.0/.pre-commit-config.yaml` & `pelican_yaml_metadata-2.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pelican_yaml_metadata-2.1.0/CONTRIBUTING.md` & `pelican_yaml_metadata-2.1.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pelican_yaml_metadata-2.1.0/tasks.py` & `pelican_yaml_metadata-2.1.1/tasks.py`

 * *Files identical despite different names*

### Comparing `pelican_yaml_metadata-2.1.0/.github/workflows/main.yml` & `pelican_yaml_metadata-2.1.1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `pelican_yaml_metadata-2.1.0/pelican/plugins/yaml_metadata/yaml_metadata.py` & `pelican_yaml_metadata-2.1.1/pelican/plugins/yaml_metadata/yaml_metadata.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,18 +16,21 @@
 with contextlib.suppress(ImportError):
     from markdown import Markdown
     import yaml
 
     ENABLED = True
 
 
-logger = logging.getLogger(__name__)
+__log__ = logging.getLogger(__name__)
 
 HEADER_RE = re.compile(
-    r"^---$" r"(?P<metadata>.+?)" r"^(?:---|\.\.\.)$" r"(?P<content>.*)",
+    r"\s*^---$"  # File starts with a line of "---" (preceeding blank lines accepted)
+    r"(?P<metadata>.+?)"
+    r"^(?:---|\.\.\.)$"  # metadata section ends with a line of "---" or "..."
+    r"(?P<content>.*)",
     re.MULTILINE | re.DOTALL,
 )
 
 DUPES_NOT_ALLOWED = set(
     k for k, v in DUPLICATES_DEFINITIONS_ALLOWED.items() if not v
 ) - {"tags", "authors"}
 
@@ -48,15 +51,15 @@
 
 def _strip(obj):
     return str(obj if obj is not None else "").strip()
 
 
 def _to_list(obj):
     """Make object into a list."""
-    return [obj] if not isinstance(obj, list) else obj
+    return [obj] if not isinstance(obj, (tuple, list)) else obj
 
 
 def _parse_date(obj):
     """Return a string representing a date."""
     # If it's already a date object, make it a string so Pelican can parse it
     # and make sure it has a timezone
     if isinstance(obj, datetime.date):
@@ -71,87 +74,93 @@
     enabled = ENABLED
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         # Don't use default Markdown metadata extension for parsing. Leave self.settings
         # alone in case we have to fall back to normal Markdown parsing.
-        self._md_settings = copy.deepcopy(self.settings["MARKDOWN"])
+        md_settings = copy.deepcopy(self.settings["MARKDOWN"])
         with contextlib.suppress(KeyError, ValueError):
-            self._md_settings["extensions"].remove("markdown.extensions.meta")
+            md_settings["extensions"].remove("markdown.extensions.meta")
+        self._md = Markdown(**md_settings)
 
     def read(self, source_path):
         """Parse content and YAML metadata of Markdown files."""
-        self._source_path = source_path
-        self._md = Markdown(**self._md_settings)
-
         with pelican_open(source_path) as text:
             m = HEADER_RE.fullmatch(text)
 
         if not m:
-            logger.info(
+            __log__.info(
                 (
-                    "No YAML metadata header found in '%s' - falling back to Markdown"
-                    " metadata parsing."
+                    "No YAML metadata header found in '%s' - "
+                    "falling back to Markdown metadata parsing."
                 ),
                 source_path,
             )
             return super().read(source_path)
 
         return (
-            self._md.convert(m.group("content")),
-            self._load_yaml_metadata(m.group("metadata")),
+            self._md.reset().convert(m.group("content")),
+            self._load_yaml_metadata(m.group("metadata"), source_path),
         )
 
-    def _load_yaml_metadata(self, text):
-        """Load Pelican metadata from the specified text."""
+    def _load_yaml_metadata(self, text, source_path):
+        """Load Pelican metadata from the specified text.
+
+        Returns an empty dict if the data fails to parse properly.
+        """
         try:
             metadata = yaml.safe_load(text)
-            if not isinstance(metadata, dict):
-                logger.error(
-                    "YAML header didn't parse as a dict for file '%s'",
-                    self._source_path,
-                )
-                logger.debug("YAML data: %r", metadata)
-                return {}
-        except Exception as e:  # NOQA: BLE001, RUF100
-            logger.exception(
-                "Error parsing YAML for file '%s': %s: %s",
-                self._source_path,
-                type(e).__name__,
-                e,
+        except Exception:  # NOQA: BLE001, RUF100
+            __log__.error(
+                "Error parsing YAML for file '%s",
+                source_path,
+                exc_info=True,
             )
             return {}
 
-        return self._parse_yaml_metadata(metadata)
+        if not isinstance(metadata, dict):
+            __log__.error(
+                "YAML header didn't parse as a dict for file '%s'",
+                source_path,
+            )
+            __log__.debug("YAML data: %r", metadata)
+            return {}
 
-    def _parse_yaml_metadata(self, meta):
+        return self._parse_yaml_metadata(metadata, source_path)
+
+    def _parse_yaml_metadata(self, meta, source_path):
         """Parse YAML-provided data into Pelican metadata.
 
         Based on MarkdownReader._parse_metadata.
         """
         output = {}
         for name, value in meta.items():
             name = name.lower()
             is_list = isinstance(value, list)
 
             if name in self.settings["FORMATTED_FIELDS"]:
                 # join mutliple formatted fields before parsing them as markdown
-                self._md.reset()
-                value = self._md.convert("\n".join(value) if is_list else str(value))
+                value = self._md.reset().convert(
+                    "\n".join(value) if is_list else str(value)
+                )
             elif is_list and len(value) > 1 and name == "author":
                 # special case: upconvert multiple "author" values to "authors"
                 name = "authors"
             elif is_list and name in DUPES_NOT_ALLOWED:
                 if len(value) > 1:
-                    logger.warning(
-                        "Duplicate definition of `%s` for %s (%s). Using first one.",
+                    __log__.warning(
+                        (
+                            "Duplicate definition of '%s' for '%s' ('%r') - "
+                            "using the first one ('%s')"
+                        ),
                         name,
-                        self._source_path,
+                        source_path,
                         value,
+                        value[0],
                     )
                 value = value[0]
 
             # Need to do our own metadata processing as YAML loads data in a
             # different way than the markdown metadata extension.
             if name in YAML_METADATA_PROCESSORS:
                 value = YAML_METADATA_PROCESSORS[name](value, self.settings)
```

### Comparing `pelican_yaml_metadata-2.1.0/README.md` & `pelican_yaml_metadata-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pelican_yaml_metadata-2.1.0/pyproject.toml` & `pelican_yaml_metadata-2.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pelican-yaml-metadata"
-version = "2.1.0"
+version = "2.1.1"
 description = "Pelican plugin for YAML-formatted Markdown metadata headers"
 authors = [
     {name = "Carey Metcalfe", email = "carey@cmetcalfe.ca"},
     {name = "Justin Mayer", email = "entroP@gmail.com"}
 ]
 readme = "README.md"
 license = {text = "MIT"}
```

### Comparing `pelican_yaml_metadata-2.1.0/PKG-INFO` & `pelican_yaml_metadata-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pelican-yaml-metadata
-Version: 2.1.0
+Version: 2.1.1
 Summary: Pelican plugin for YAML-formatted Markdown metadata headers
 Project-URL: Homepage, https://github.com/pelican-plugins/yaml-metadata
 Project-URL: Funding, https://donate.getpelican.com/
 Project-URL: Issue Tracker, https://github.com/pelican-plugins/yaml-metadata/issues
 Author-email: Carey Metcalfe <carey@cmetcalfe.ca>, Justin Mayer <entroP@gmail.com>
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
```

