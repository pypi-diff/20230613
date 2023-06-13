# Comparing `tmp/ansible-anonymizer-1.3.0.tar.gz` & `tmp/ansible-anonymizer-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-anonymizer-1.3.0.tar", last modified: Wed May 24 20:28:16 2023, max compression
+gzip compressed data, was "ansible-anonymizer-1.4.0.tar", last modified: Tue Jun 13 18:36:14 2023, max compression
```

## Comparing `ansible-anonymizer-1.3.0.tar` & `ansible-anonymizer-1.4.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-05-24 20:28:16.838947 ansible-anonymizer-1.3.0/
--rw-r--r--   0 goneri    (1002) goneri    (1002)      292 2023-03-10 14:59:31.000000 ansible-anonymizer-1.3.0/.editorconfig
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-05-24 20:28:16.836947 ansible-anonymizer-1.3.0/.github/
--rw-r--r--   0 goneri    (1002) goneri    (1002)      321 2023-03-23 15:13:37.000000 ansible-anonymizer-1.3.0/.github/ISSUE_TEMPLATE.md
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-05-24 20:28:16.836947 ansible-anonymizer-1.3.0/.github/workflows/
--rw-r--r--   0 goneri    (1002) goneri    (1002)      551 2023-03-10 14:59:31.000000 ansible-anonymizer-1.3.0/.github/workflows/tox.yml
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1204 2023-03-10 14:59:31.000000 ansible-anonymizer-1.3.0/.gitignore
--rw-r--r--   0 goneri    (1002) goneri    (1002)      142 2023-05-24 20:00:02.000000 ansible-anonymizer-1.3.0/.gitleaks.toml
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1208 2023-05-24 17:40:23.000000 ansible-anonymizer-1.3.0/.pre-commit-config.yaml
--rw-r--r--   0 goneri    (1002) goneri    (1002)     2075 2023-05-24 20:00:16.000000 ansible-anonymizer-1.3.0/CHANGELOG.rst
--rw-r--r--   0 goneri    (1002) goneri    (1002)     2478 2023-03-23 15:13:37.000000 ansible-anonymizer-1.3.0/CONTRIBUTING.rst
--rw-r--r--   0 goneri    (1002) goneri    (1002)       63 2023-03-10 14:59:31.000000 ansible-anonymizer-1.3.0/HISTORY.rst
--rw-r--r--   0 goneri    (1002) goneri    (1002)      588 2023-03-22 17:41:29.000000 ansible-anonymizer-1.3.0/LICENSE
--rw-r--r--   0 goneri    (1002) goneri    (1002)      168 2023-04-05 18:22:37.000000 ansible-anonymizer-1.3.0/MANIFEST.in
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1671 2023-05-24 20:28:16.838947 ansible-anonymizer-1.3.0/PKG-INFO
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1227 2023-05-05 17:28:31.000000 ansible-anonymizer-1.3.0/README.rst
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-05-24 20:28:16.836947 ansible-anonymizer-1.3.0/ansible_anonymizer/
--rw-r--r--   0 goneri    (1002) goneri    (1002)       90 2023-05-24 20:00:16.000000 ansible-anonymizer-1.3.0/ansible_anonymizer/__init__.py
--rw-r--r--   0 goneri    (1002) goneri    (1002)     9368 2023-05-24 17:40:09.000000 ansible-anonymizer-1.3.0/ansible_anonymizer/anonymizer.py
--rw-r--r--   0 goneri    (1002) goneri    (1002)      724 2023-05-24 17:21:14.000000 ansible-anonymizer-1.3.0/ansible_anonymizer/cli.py
--rw-r--r--   0 goneri    (1002) goneri    (1002)     2071 2023-05-24 17:21:14.000000 ansible-anonymizer-1.3.0/ansible_anonymizer/field_checks.py
--rw-r--r--   0 goneri    (1002) goneri    (1002)      327 2023-05-24 17:21:14.000000 ansible-anonymizer-1.3.0/ansible_anonymizer/jinja2.py
--rw-r--r--   0 goneri    (1002) goneri    (1002)    13085 2023-05-24 20:02:45.000000 ansible-anonymizer-1.3.0/ansible_anonymizer/parser.py
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-05-24 20:28:16.837947 ansible-anonymizer-1.3.0/ansible_anonymizer.egg-info/
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1671 2023-05-24 20:28:16.000000 ansible-anonymizer-1.3.0/ansible_anonymizer.egg-info/PKG-INFO
--rw-r--r--   0 goneri    (1002) goneri    (1002)      743 2023-05-24 20:28:16.000000 ansible-anonymizer-1.3.0/ansible_anonymizer.egg-info/SOURCES.txt
--rw-r--r--   0 goneri    (1002) goneri    (1002)        1 2023-05-24 20:28:16.000000 ansible-anonymizer-1.3.0/ansible_anonymizer.egg-info/dependency_links.txt
--rw-r--r--   0 goneri    (1002) goneri    (1002)       67 2023-05-24 20:28:16.000000 ansible-anonymizer-1.3.0/ansible_anonymizer.egg-info/entry_points.txt
--rw-r--r--   0 goneri    (1002) goneri    (1002)       12 2023-05-24 20:28:16.000000 ansible-anonymizer-1.3.0/ansible_anonymizer.egg-info/requires.txt
--rw-r--r--   0 goneri    (1002) goneri    (1002)       19 2023-05-24 20:28:16.000000 ansible-anonymizer-1.3.0/ansible_anonymizer.egg-info/top_level.txt
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1683 2023-05-24 20:00:02.000000 ansible-anonymizer-1.3.0/pyproject.toml
--rw-r--r--   0 goneri    (1002) goneri    (1002)       38 2023-05-24 20:28:16.838947 ansible-anonymizer-1.3.0/setup.cfg
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-05-24 20:28:16.837947 ansible-anonymizer-1.3.0/tests/
--rw-r--r--   0 goneri    (1002) goneri    (1002)    11265 2023-05-24 20:00:02.000000 ansible-anonymizer-1.3.0/tests/test_anonymizer.py
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1648 2023-05-24 20:00:02.000000 ansible-anonymizer-1.3.0/tests/test_field_checks.py
--rw-r--r--   0 goneri    (1002) goneri    (1002)      294 2023-05-24 20:00:02.000000 ansible-anonymizer-1.3.0/tests/test_jinja2.py
--rw-r--r--   0 goneri    (1002) goneri    (1002)     9281 2023-05-24 20:21:16.000000 ansible-anonymizer-1.3.0/tests/test_parser.py
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1430 2023-05-24 20:00:16.000000 ansible-anonymizer-1.3.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:36:14.595428 ansible-anonymizer-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-13 18:35:55.000000 ansible-anonymizer-1.4.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:36:14.587428 ansible-anonymizer-1.4.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-13 18:35:55.000000 ansible-anonymizer-1.4.0/.github/ISSUE_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:36:14.587428 ansible-anonymizer-1.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-13 18:35:55.000000 ansible-anonymizer-1.4.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-13 18:35:55.000000 ansible-anonymizer-1.4.0/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-13 18:35:55.000000 ansible-anonymizer-1.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-13 18:35:55.000000 ansible-anonymizer-1.4.0/.gitleaks.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-13 18:35:55.000000 ansible-anonymizer-1.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-06-13 18:35:55.000000 ansible-anonymizer-1.4.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-06-13 18:35:55.000000 ansible-anonymizer-1.4.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-13 18:35:55.000000 ansible-anonymizer-1.4.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-13 18:35:55.000000 ansible-anonymizer-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-13 18:35:55.000000 ansible-anonymizer-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-06-13 18:36:14.595428 ansible-anonymizer-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-06-13 18:35:55.000000 ansible-anonymizer-1.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:36:14.587428 ansible-anonymizer-1.4.0/ansible_anonymizer/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-13 18:35:55.000000 ansible-anonymizer-1.4.0/ansible_anonymizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10454 2023-06-13 18:35:55.000000 ansible-anonymizer-1.4.0/ansible_anonymizer/anonymizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-13 18:35:55.000000 ansible-anonymizer-1.4.0/ansible_anonymizer/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-13 18:35:55.000000 ansible-anonymizer-1.4.0/ansible_anonymizer/field_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-13 18:35:55.000000 ansible-anonymizer-1.4.0/ansible_anonymizer/jinja2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13245 2023-06-13 18:35:55.000000 ansible-anonymizer-1.4.0/ansible_anonymizer/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:36:14.591428 ansible-anonymizer-1.4.0/ansible_anonymizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-06-13 18:36:14.000000 ansible-anonymizer-1.4.0/ansible_anonymizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-13 18:36:14.000000 ansible-anonymizer-1.4.0/ansible_anonymizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 18:36:14.000000 ansible-anonymizer-1.4.0/ansible_anonymizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-13 18:36:14.000000 ansible-anonymizer-1.4.0/ansible_anonymizer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 18:36:14.000000 ansible-anonymizer-1.4.0/ansible_anonymizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-13 18:36:14.000000 ansible-anonymizer-1.4.0/ansible_anonymizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-06-13 18:35:55.000000 ansible-anonymizer-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 18:36:14.595428 ansible-anonymizer-1.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:36:14.591428 ansible-anonymizer-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-06-13 18:35:55.000000 ansible-anonymizer-1.4.0/tests/test_anonymizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-06-13 18:35:55.000000 ansible-anonymizer-1.4.0/tests/test_field_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-13 18:35:55.000000 ansible-anonymizer-1.4.0/tests/test_jinja2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12040 2023-06-13 18:35:55.000000 ansible-anonymizer-1.4.0/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-13 18:35:55.000000 ansible-anonymizer-1.4.0/tox.ini
```

### Comparing `ansible-anonymizer-1.3.0/.github/workflows/tox.yml` & `ansible-anonymizer-1.4.0/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.3.0/.gitignore` & `ansible-anonymizer-1.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.3.0/.pre-commit-config.yaml` & `ansible-anonymizer-1.4.0/.pre-commit-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -44,10 +44,11 @@
 - repo: local
   hooks:
     - id: mypy
       name: mypy
       entry: mypy
       language: python
       types: [python]
+      args: [--no-strict-optional]
       additional_dependencies:
         - mypy
         - types-PyYAML
```

### Comparing `ansible-anonymizer-1.3.0/CHANGELOG.rst` & `ansible-anonymizer-1.4.0/CHANGELOG.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Changelog
 =========
 
+Version 1.4.0 (2023-06-13)
+-------------
+
+- fix the parser when a string is an empty quoted string (``""``)
+- refactoring to properly isolate the parsing in ``ansible_anonymizer.parser``
+- add ability to customize the secret substitution
+- README: minor adjustments and a new "limitations" section
+
 Version 1.3.0 (2023-05-24)
 -------------
 
 - tests: split up test_anonymizer.py
 - pre-commit: only check ansible_anonymizer
 - pre-commit: mypy needs types-PyYAML
 - pylint: various fixes to get pylint to pass
```

### Comparing `ansible-anonymizer-1.3.0/CONTRIBUTING.rst` & `ansible-anonymizer-1.4.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.3.0/LICENSE` & `ansible-anonymizer-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.3.0/PKG-INFO` & `ansible-anonymizer-1.4.0/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: ansible-anonymizer
-Version: 1.3.0
-Summary: Ansible Anonymizer
-Author-email: Gonéri Le Bouder <goneri@lebouder.net>
-Project-URL: Homepage, https://github.com/ansible/anonymizer
-Keywords: pii,anonymize
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
-Description-Content-Type: text/x-rst
-Provides-Extra: test
-License-File: LICENSE
-
 ==========
 Anonymizer
 ==========
 
 
 .. image:: https://img.shields.io/pypi/v/ansible-anonymizer.svg
         :target: https://pypi.python.org/pypi/ansible-anonymizer
@@ -26,38 +12,64 @@
 
 Library to clean up Ansible tasks from any Personally Identifiable Information (PII)
 
 
 * Free software: Apache Software License 2.0
 
 
-Features
---------
+Usage
+-----
 
 The library can be used to remove the PII from a multi level structure:
 
-.. code-block::
+.. code-block:: python
+
+    from ansible_anonymizer.anonymizer import anonymize_struct
 
-   $ python3
-   >>> from ansible_anonymizer import anonymizer
-   >>> example = [{"name": "foo bar", "email": "my-email@address.com"}]
-   >>> anonymizer.anonymize_struct(example)
-   ['- email: lucas27@example.com\n  name: foo bar\n']
+    example = [{"name": "foo bar", "email": "my-email@address.com"}]
+
+    anonymize_struct(example)
+    # [{'name': 'foo bar', 'email': 'noah2@example.com'}]
 
 But you can also anonymize a block of text:
 
-.. code-block::
+.. code-block:: python
+
+    from ansible_anonymizer.anonymizer import anonymize_text_block
 
-   >>> from ansible_anonymizer import anonymizer
-   >>> some_text = """
-   ... - name: a task
-   ...   a_module:
-   ...     secret: foobar
-   ... """
-   >>> anonymizer.anonymize_text_block(some_text)
-   '\n- name: a task\n  a_module:\n    secret: {{ }}\n'
+    some_text = """
+    - name: a task
+      a_module:
+        secret: foobar
+    """
+
+    anonymize_text_block(some_text)
+    # '\n- name: a task\n  a_module:\n    secret: "{{ secret }}"\n'
 
 You can also use the ``ansible-anonymizer`` command:
 
 .. code-block:: console
 
    ansible-anonymizer my-secret-file
+
+Customize the anonymized strings
+================================
+
+By default, the variables are anonymized with a string based on the name of the field.
+You can customize it with the ``value_template`` parameter:
+
+.. code-block:: python
+
+    from ansible_anonymizer.anonymizer import anonymize_struct
+    from string import Template
+
+    original = {"password": "$RvEDSRW#R"}
+    value_template = Template("_${variable_name}_")
+    anonymize_struct(original, value_template=value_template)
+    #  {'password': '_password_'}
+
+
+Limitations
+-----------
+
+- ``anonymize_text_block()`` relies on its own text parser which only support a subset of YAML features. Because of this, it may not be able to identify some PII. When possible, use ``anonymize_struct`` which accepts a Python structure instead.
+- The Anonymizer is not a silver bullet and it's still possible to see PII going through the filters.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ansible-anonymizer-1.3.0/ansible_anonymizer/anonymizer.py` & `ansible-anonymizer-1.4.0/ansible_anonymizer/anonymizer.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,25 +3,26 @@
 # pylint: disable=missing-function-docstring
 # pylint: disable=invalid-name
 import ipaddress
 import re
 from collections.abc import Generator
 from ipaddress import IPv4Address, IPv6Address
 from re import Match
-from typing import Any, Callable, Union
+from string import Template
+from typing import Any, Callable, Optional, Union
 from zlib import crc32
 
 from ansible_anonymizer.field_checks import (
     is_jinja2_expression,
     is_password_field_name,
     is_path,
     is_uuid_string,
 )
 from ansible_anonymizer.jinja2 import str_jinja2_variable_name
-from ansible_anonymizer.parser import hide_secrets
+from ansible_anonymizer.parser import NodeType, flatten, parse_raw_block
 
 
 def gen_email_address(original: Match[str]) -> str:
     samples = [
         "liam",
         "olivia",
         "noah",
@@ -114,41 +115,47 @@
     if not value or len(value) < 2:
         return value
     if value[0] == value[-1] and value[0] in ('"', "'"):
         return value[1:-1]
     return value
 
 
-def anonymize_field(value: str, name: str) -> str:
+def anonymize_field(value: str, name: str, value_template: Template) -> str:
     v = value.strip()
     if is_uuid_string(v):
         return value
     if is_password_field_name(name):
         if is_path(v):
             return value
         if is_jinja2_expression(unquote(v)):
             return unquote(v)
         variable_name = str_jinja2_variable_name(name)
-        return f"{{{{ { variable_name } }}}}"
+        return value_template.substitute(variable_name=variable_name)
     return anonymize_text_block(value)
 
 
-def anonymize_struct(o: Any, key_name: str = "") -> Any:
+def anonymize_struct(o: Any, key_name: str = "", value_template: Optional[Template] = None) -> Any:
+    if not value_template:
+        value_template = Template("{{ $variable_name }}")
+
     def key_name_str(k: Any) -> str:
         return k if isinstance(k, str) else ""
 
     if key_name and not isinstance(key_name, str):
         key_name = str(key_name)
 
     if isinstance(o, dict):
-        return {k: anonymize_struct(v, key_name=key_name_str(k)) for k, v in o.items()}
+        return {
+            k: anonymize_struct(v, key_name=key_name_str(k), value_template=value_template)
+            for k, v in o.items()
+        }
     if isinstance(o, list):
-        return [anonymize_struct(v, key_name=key_name) for v in o]
+        return [anonymize_struct(v, key_name=key_name, value_template=value_template) for v in o]
     if isinstance(o, str):
-        return anonymize_field(o, key_name)
+        return anonymize_field(o, key_name, value_template)
     return o
 
 
 def anonymize(o: Any, key_name: str = "") -> Any:
     """Deprecated: use anonymize_struct() instead."""
     return anonymize_struct(o, key_name=key_name)
 
@@ -299,23 +306,39 @@
         r"(?P<before>/(home|Users)/)(?P<user_name>[a-z0-9_-]{,255})",
     ]
     for regex in user_regexes:
         block = re.sub(regex, _rewrite, block, flags=flags)
     return block
 
 
-def anonymize_text_block(block: str) -> str:
-    transformation = [
-        hide_comments,
-        hide_secrets,
-        hide_emails,
-        hide_ip_addresses,
-        hide_us_ssn,
-        hide_mac_addresses,
-        hide_us_phone_numbers,
-        hide_credit_cards,
-        hide_user_name,
-    ]
+def hide_secrets(block: str, value_template: Template) -> str:
+    root_node = parse_raw_block(block)
+
+    output = ""
+    for node in flatten(root_node):
+        if node.type is NodeType.secret:
+            if node.previous.type is node.holder:  # type: ignore[comparison-overlap]
+                # Already quoted
+                quote = ""
+            else:
+                quote = "" if node.holder.text else '"'
+            output += quote + anonymize_field("", node.secret_value_of.text, value_template) + quote
+        else:
+            output += node.text
+    return output
+
+
+def anonymize_text_block(block: str, value_template: Optional[Template] = None) -> str:
+    if not value_template:
+        value_template = Template("{{ $variable_name }}")
+
+    block = hide_comments(block)
+    block = hide_secrets(block, value_template)
+    block = hide_emails(block)
+    block = hide_ip_addresses(block)
+    block = hide_us_ssn(block)
+    block = hide_mac_addresses(block)
+    block = hide_us_phone_numbers(block)
+    block = hide_credit_cards(block)
+    block = hide_user_name(block)
 
-    for t in transformation:
-        block = t(block)
     return block
```

### Comparing `ansible-anonymizer-1.3.0/ansible_anonymizer/cli.py` & `ansible-anonymizer-1.4.0/ansible_anonymizer/cli.py`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.3.0/ansible_anonymizer/field_checks.py` & `ansible-anonymizer-1.4.0/ansible_anonymizer/field_checks.py`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.3.0/ansible_anonymizer/parser.py` & `ansible-anonymizer-1.4.0/ansible_anonymizer/parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python3
 """Parser for YAML-like structure that is error tolerant."""
 from collections.abc import Generator
 from enum import Enum
 from typing import Optional, Union
 
 from ansible_anonymizer.field_checks import is_password_field_name
-from ansible_anonymizer.jinja2 import str_jinja2_variable_name
 
 
 class NodeType(Enum):
     """The different type of Node returned by the parser."""
 
     # pylint: disable=invalid-name
 
@@ -19,14 +18,15 @@
     quoted_string_holder = 3
     quoted_string_closing = 4
     new_line = 5
     space = 6
     securized = 7
     backslash = 8
     deleted = 9
+    secret = 10
 
 
 class ParserError(Exception):
     """Unexpected behaviour."""
 
 
 class Node:
@@ -37,14 +37,16 @@
         self.previous: Optional["Node"] = None
         self.next: Optional["Node"] = None
         self.begin_at: int = begin_at
         self.end_at: int
         self.text: str = ""
         self.type: NodeType = NodeType.unknown
         self.holder: Optional["Node"] = None
+        # Node of the field that point on this secret
+        self.secret_value_of: Optional["Node"] = None
 
         # NOTE: Fields only used with quoted strings (called `holder`)
         self.closed_by: Optional["Node"] = None
         self.sub: list["Node"] = []
         self.is_protected: bool = False
 
     def attach(self, previous: "Node") -> None:
@@ -120,104 +122,107 @@
 
 
 def is_field_value_sep(char: str) -> bool:
     """Return True if the character is : or =."""
     return char in [":", "="]
 
 
-def parser(block: str) -> Node:
+def breakup_elements(block: str) -> Node:
     # pylint: disable=too-many-branches
     # pylint: disable=too-many-statements
     """Digest a text block an return a list of Nodes that will be simplified later."""
     root_node = Node(0)
     root_node.type = NodeType.quoted_string_holder
     current_node = root_node
     for pos, c in enumerate(block):  # pylint: disable=invalid-name
+        previous_node = current_node
+        current_node = Node(-1)  # -1 == undef, the variable will be reset
         if c == "\\":
             new_node = Node(pos)
-            new_node.attach(previous=current_node)
+            new_node.attach(previous=previous_node)
             new_node.type = NodeType.backslash
             current_node = new_node
         elif c in ["'", '"']:
-            is_protected = current_node.type is NodeType.backslash
+            is_protected = previous_node.type is NodeType.backslash
 
-            holder = current_node.holder
+            holder: Optional[Node] = previous_node
             while holder:
                 if (
                     holder.text == c
                     and holder.is_protected is is_protected
                     and not holder.closed_by
                 ):
                     break
                 holder = holder.holder
 
             if holder:
                 new_node = Node(pos)
-                new_node.attach(previous=current_node)
+                new_node.attach(previous=previous_node)
                 new_node.type = NodeType.quoted_string_closing
                 holder.closed_by = new_node
                 current_node = new_node
             else:
                 new_node = Node(pos)
                 new_node.type = NodeType.quoted_string_holder
                 new_node.is_protected = is_protected
-                new_node.attach(previous=current_node)
+                new_node.attach(previous=previous_node)
                 current_node = new_node
         elif is_valid_first_character_for_a_variable(c):
-            if current_node.type is NodeType.field:
-                pass
+            if previous_node.type is NodeType.field:
+                current_node = previous_node
             else:
                 new_node = Node(pos)
-                new_node.attach(previous=current_node)
+                new_node.attach(previous=previous_node)
                 new_node.type = NodeType.field
                 current_node = new_node
         elif is_valid_variable_character(c):
-            if current_node.type is NodeType.field:
-                pass
-            elif current_node.type is not NodeType.unknown:
+            if previous_node.type is NodeType.field:
+                current_node = previous_node
+            else:
                 new_node = Node(pos)
-                new_node.attach(previous=current_node)
+                new_node.attach(previous=previous_node)
+                new_node.type = NodeType.field
                 current_node = new_node
         elif is_field_value_sep(c):
             new_node = Node(pos)
-            new_node.attach(previous=current_node)
+            new_node.attach(previous=previous_node)
             new_node.type = NodeType.separator
             current_node = new_node
         elif c == "\n":
             new_node = Node(pos)
-            new_node.attach(previous=current_node)
+            new_node.attach(previous=previous_node)
             new_node.type = NodeType.new_line
             current_node = new_node
         elif c == " ":
             new_node = Node(pos)
-            new_node.attach(previous=current_node)
+            new_node.attach(previous=previous_node)
             new_node.type = NodeType.space
             current_node = new_node
+        elif previous_node.type is not NodeType.unknown:
+            new_node = Node(pos)
+            new_node.attach(previous=previous_node)
+            current_node = new_node
         else:
-            if current_node.type is not NodeType.unknown:
-                new_node = Node(pos)
-                new_node.attach(previous=current_node)
-                current_node = new_node
+            # Should never happend
+            new_node = Node(pos)
+            new_node.attach(previous=previous_node)
+            current_node = new_node
 
         current_node.text += c
     return root_node
 
 
-def hide_secrets(block: str) -> str:
+def parse_raw_block(block: str) -> Node:
     """Return block without any potential secrets."""
-    root_node = parser(block)
+    root_node = breakup_elements(block)
     close_quotes(root_node)
     handle_backslashes(root_node)
     combinate_value_fields(root_node)
-    hide_secret_fields(root_node)
-
-    output = ""
-    for node in flatten(root_node):
-        output += node.text
-    return output
+    identify_secrets(root_node)
+    return root_node
 
 
 def close_quotes(root_node: Node) -> None:
     """Close the quotes that are still opened."""
     current_node = root_node.next
     while current_node:
         if current_node.type is NodeType.quoted_string_holder and not current_node.closed_by:
@@ -298,15 +303,14 @@
         secret_content_ptr = current_node.get_secret()
         if not secret_content_ptr:
             continue
         separator = _find_separator_node(current_node)
         if not separator:
             continue
         if secret_content_ptr.type is NodeType.quoted_string_holder:
-            assert secret_content_ptr.closed_by  # for mypy # noqa: S101
             current_node = secret_content_ptr.closed_by
             continue
         while (
             secret_content_ptr.next
             and (
                 (secret_content_ptr.next.type in mergable_types)
                 or (
@@ -325,44 +329,41 @@
     while current:
         yield current
         if not current.next:
             break
         current = current.next
 
 
-def hide_secret_fields(root_node: Node) -> None:
+def identify_secrets(root_node: Node) -> None:
     """Remove the secret fields from a series of nodes."""
 
-    def hide_quoted_string(node: Node, secret_node: Node) -> None:
+    def identify_quoted_string(node: Node, secret_node: Node) -> None:
         assert secret_node.closed_by  # for mypy # noqa: S101
-        secret_node.next = secret_node.closed_by.next
-        secret_node.type = NodeType.securized
-        secret_node.text = (
-            f"{secret_node.text}{{{{ {str_jinja2_variable_name(node.text)} }}}}{secret_node.text}"
-        )
+        cursor = secret_node.next
+        while cursor and cursor != secret_node.closed_by and cursor.next != secret_node.closed_by:
+            cursor.merge_with_next()
+        if secret_node.next and secret_node.next != secret_node.closed_by:
+            secret_node.next.secret_value_of = node
+            secret_node.next.type = NodeType.secret
         if secret_node.next:
-            hide_secret_fields(secret_node.next)
+            identify_secrets(secret_node.next)
 
-    def hide_regular_field(node: Node, secret_node: Node) -> None:
-        secret_node.type = NodeType.securized
+    def identify_regular_field(node: Node, secret_node: Node) -> None:
         assert secret_node.holder  # for mypy # noqa: S101
-        quote = "" if secret_node.holder.text else '"'
-        secret_node.text = f"{quote}{{{{ {str_jinja2_variable_name(node.text)} }}}}{quote}"
+        secret_node.secret_value_of = node
+        secret_node.type = NodeType.secret
         if secret_node.next:
-            hide_secret_fields(secret_node.next)
+            identify_secrets(secret_node.next)
 
     for node in flatten(root_node):
         if node.type is not NodeType.field:
             continue
         if not node.is_password_field_name():
             continue
 
         secret_node = node.get_secret()
         if not secret_node:
             continue
 
-        # pylint: disable=inconsistent-return-statements
-        # pylint: disable=no-else-return
         if secret_node.type is NodeType.quoted_string_holder:
-            return hide_quoted_string(node, secret_node)
-        else:
-            return hide_regular_field(node, secret_node)
+            return identify_quoted_string(node, secret_node)
+        return identify_regular_field(node, secret_node)
```

### Comparing `ansible-anonymizer-1.3.0/ansible_anonymizer.egg-info/SOURCES.txt` & `ansible-anonymizer-1.4.0/ansible_anonymizer.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 HISTORY.rst
 LICENSE
 MANIFEST.in
 README.rst
 pyproject.toml
 tox.ini
 .github/ISSUE_TEMPLATE.md
+.github/workflows/release.yml
 .github/workflows/tox.yml
 ansible_anonymizer/__init__.py
 ansible_anonymizer/anonymizer.py
 ansible_anonymizer/cli.py
 ansible_anonymizer/field_checks.py
 ansible_anonymizer/jinja2.py
 ansible_anonymizer/parser.py
```

### Comparing `ansible-anonymizer-1.3.0/pyproject.toml` & `ansible-anonymizer-1.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -60,14 +60,14 @@
     "S",  # bandit
     "SIM",  # flake8-simplify
     "TRY",  # tryceratops
     "UP",  # pyupgrade
     "W",  # Warning
     "YTT", # flake8-2020
 ]
-ignore = ["D107", "D203", "D212", "D100", "D103", "PGH003", "D401", "SIM114", "ISC003"]
+ignore = ["D107", "D203", "D212", "D100", "D103", "PGH003", "D401", "SIM114", "ISC003", "SIM108"]
 
 [tool.ruff.per-file-ignores]
 "tests/test_anonymizer.py" = ["S101", "S105"]
 "tests/test_field_checks.py" = ["S101", "S105"]
 "tests/test_jinja2.py" = ["S101", "S105"]
 "tests/test_parser.py" = ["S101", "S105"]
```

### Comparing `ansible-anonymizer-1.3.0/tests/test_anonymizer.py` & `ansible-anonymizer-1.4.0/tests/test_anonymizer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python3
 # pylint: disable=missing-module-docstring
 # pylint: disable=missing-function-docstring
 from ipaddress import IPv4Address, IPv4Network, IPv6Address
+from string import Template
 from textwrap import dedent
 
 from ansible_anonymizer.anonymizer import (
     anonymize,
     anonymize_field,
     anonymize_struct,
     anonymize_text_block,
@@ -38,38 +39,44 @@
 
 
 def test_redact_ip_address():
     assert redact_ip_address("2001:4860:4860::8888") == "2001:4860:4860::8888"
     assert IPv4Address(redact_ip_address("8.8.8.9"))
 
 
-def test_anonymize_struct():
+def test_anonymize_struct_nested_struct():
     in_ = {
         "name": "Install nginx and nodejs 12",
         "apt": {"name": ["nginx", "nodejs"], "state": "latest"},
         "a_set": {1, 2, 3},
         "dict_wit_with_int_as_index": {1: "1", 2: "2", 3: "3"},
     }
     assert anonymize_struct(in_) == in_
 
+
+def test_anonymize_struct_ip_addresses():
     in_ = {
         "name": "foo@montreal.ca",
         "a_module": {
             "ip": ["2001:460:48::888", "192.168.1.1"],
             "password": "@This-should-disapear!",
         },
     }
     changed = anonymize_struct(in_)
     assert "foo@montreal.ca" not in changed["name"]
     assert "2001:460:48::888" not in changed["a_module"]["ip"]
     assert changed["a_module"]["password"] == "{{ password }}"
 
+
+def test_anonymize_multiple_passwords():
     in_ = {"password": ["first_password", "second_password"]}
     assert anonymize_struct(in_) == {"password": ["{{ password }}", "{{ password }}"]}
 
+
+def test_anonymize_email():
     # Str
     in_ = "my-email-address@somewhe.re"
     changed = anonymize_struct(in_)
     assert in_ not in changed
     assert isinstance(changed, str)
     assert "@" in changed
 
@@ -77,15 +84,22 @@
     in_ = ["my-email-address@somewhe.re"]
     changed = anonymize_struct(in_)
     assert in_ != changed
     assert isinstance(changed[0], str)
     assert "@" in changed[0]
 
 
-def test_anonymize():
+def test_anonymize_with_special_template():
+    original = {"password": ["first_password", "second_password"]}
+    expected = {"password": ["ö", "ö"]}
+    value_template = Template("ö")
+    assert anonymize_struct(original, value_template=value_template) == expected
+
+
+def test_anonymize_deprecated_function():
     in_ = ["my-email-address@somewhe.re"]
     changed = anonymize(in_)
     assert in_ != changed
 
 
 def test_anonymize_text_block_no_change():
     source = """
@@ -382,26 +396,116 @@
     assert anonymize_text_block(source) == expectation
     assert hide_user_name(dedent(source)) == dedent(expectation)
 
 
 def test_anonymize_field():
     field = "my_field"
     value = "     a    "
-    assert anonymize_field(value, field) == value
+
+    value_template = Template("{{ $variable_name }}")
+    assert anonymize_field(value, field, value_template) == value
 
 
 def test_unquote():
     assert unquote("'a'") == "a"
     assert unquote('"a"') == "a"
     assert unquote('"a\'') == '"a\''
     assert unquote("a") == "a"
     assert unquote("''") == ""
     assert unquote("'") == "'"
 
 
 def test_anonymize_uuid_field():
     field = "uuid_field"
     value = "ce34efc1-f5e3-4b0f-bb2c-5272319589a7"
-    assert anonymize_field(value, field) == value
+    value_template = Template("{{ $variable_name }}")
+    assert anonymize_field(value, field, value_template) == value
 
     value = "CE34EFC1-F5E3-4B0F-BB2C-5272319589A7"
-    assert anonymize_field(value, field) == value
+    value_template = Template("{{ $variable_name }}")
+    assert anonymize_field(value, field, value_template) == value
+
+
+def test_anonymize_special_template():
+    field = "secret"
+    value = "to_hide"
+
+    value_template = Template("--${variable_name}--")
+    assert anonymize_field(value, field, value_template) == "--secret--"
+
+
+def test_hide_secrets_aws_profile():
+    origin = """
+    [my-secret-account]
+    aws_access_key_id = BJIA5UUFYYOOKZQODC3F
+    aws_secret_access_key = NeTL/2vPPnlnb/8RBtsw3EwnNjflDbgZiDmRskhb
+    """
+
+    expectation = """
+    [my-secret-account]
+    aws_access_key_id = "{{ aws_access_key_id }}"
+    aws_secret_access_key = "{{ aws_secret_access_key }}"
+    """
+    assert anonymize_text_block(dedent(origin)) == dedent(expectation)
+
+
+def test_hide_secrets_multi_secrets():
+    origin = """
+    '(?i)password1:': "{{ _iosxr_password }}"
+    "this is somethingpass: password2: else my_password3: 'password4: _Agaim': barfoo"
+    password5: maxplus
+    password6: "maxplus"
+    password7: "my_password8: maxplus"
+    "password9": "my_password10: maxplus"
+    password11: "my_password12:
+              maxplus"
+
+    passwd: $6$j212wezy$7H/1LT4f9/N3wpgNunhsIqtMj62OKiS3nyNwuizouQc3u7MbYCarYeAHWYPYb2FT.lbioDm2RrkJPb9BZMN1O/
+    """  # noqa: E501
+    expectation = """
+    '(?i)password1:': "{{ _iosxr_password }}"
+    "this is somethingpass: {{ somethingpass }}: else my_password3: '{{ my_password3 }}': barfoo"
+    password5: "{{ password5 }}"
+    password6: "{{ password6 }}"
+    password7: "{{ password7 }}"
+    "password9": "{{ password9 }}"
+    password11: "{{ password11 }}"
+
+    passwd: "{{ passwd }}"
+    """
+    assert anonymize_text_block(origin) == expectation
+
+
+def test_hide_secret_sudo_line():
+    source = 'line="%wheel\tALL=(ALL)\tNOPASSWD: ALL"'
+    assert anonymize_text_block(source) == source
+
+
+def test_anonymize_text_block_quoted():
+    assert (
+        anonymize_text_block("ansible: 'ALL=(ALL) PASSWD: \\\"{{NOPASSWD'")
+        == "ansible: 'ALL=(ALL) PASSWD: {{ passwd }}'"
+    )
+    assert (
+        anonymize_text_block("ansible: 'ALL=(ALL) PASSWD: \\\"{{NOPASSWD'")
+        == "ansible: 'ALL=(ALL) PASSWD: {{ passwd }}'"
+    )
+    assert (
+        anonymize_text_block("password1: 'foobar'\npassword: 'barfoo'")
+        == "password1: '{{ password1 }}'\npassword: '{{ password }}'"
+    )
+    assert (
+        anonymize_text_block('%wheel	ALL=(ALL)	PASSWD: "ALL"')
+        == '%wheel	ALL=(ALL)	PASSWD: "{{ passwd }}"'  # noqa: E501
+    )
+
+
+def test_anonymize_text_block_special_template():
+    value_template = Template("--")
+    assert anonymize_text_block('my_secret: "ÓÐG™ÉÓÖ"', value_template) == 'my_secret: "--"'
+
+
+def test_anonymize_text_block_preserve_protected_quotes():
+    assert (
+        anonymize_text_block('line: "%ansible password=\'foobar\'"')
+        == 'line: "%ansible password=\'{{ password }}\'"'
+    )
```

### Comparing `ansible-anonymizer-1.3.0/tests/test_field_checks.py` & `ansible-anonymizer-1.4.0/tests/test_field_checks.py`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.3.0/tests/test_parser.py` & `ansible-anonymizer-1.4.0/tests/test_parser.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,212 +2,186 @@
 # pylint: disable=missing-module-docstring
 # pylint: disable=missing-function-docstring
 
 from textwrap import dedent
 
 from ansible_anonymizer.parser import (
     NodeType,
+    breakup_elements,
     combinate_value_fields,
     flatten,
-    hide_secrets,
-    parser,
+    parse_raw_block,
 )
 
 
-def test_hide_secret_sudo_line():
-    source = 'line="%wheel\tALL=(ALL)\tNOPASSWD: ALL"'
-    assert hide_secrets(source) == source
-
-
-def test_hide_secrets_quoted():
-    assert (
-        hide_secrets("ansible: 'ALL=(ALL) PASSWD: \\\"{{NOPASSWD'")
-        == "ansible: 'ALL=(ALL) PASSWD: {{ passwd }}'"
-    )
-    assert (
-        hide_secrets("ansible: 'ALL=(ALL) PASSWD: \\\"{{NOPASSWD'")
-        == "ansible: 'ALL=(ALL) PASSWD: {{ passwd }}'"
-    )
-    assert (
-        hide_secrets("password1: 'foobar'\npassword: 'barfoo'")
-        == "password1: '{{ password1 }}'\npassword: '{{ password }}'"
-    )
-    assert (
-        hide_secrets('%wheel	ALL=(ALL)	PASSWD: "ALL"')
-        == '%wheel	ALL=(ALL)	PASSWD: "{{ passwd }}"'  # noqa: E501
-    )
-
-
-def test_hide_secrets_preserve_protected_quotes():
-    assert (
-        hide_secrets('line: "%ansible password=\'foobar\'"')
-        == 'line: "%ansible password=\'{{ password }}\'"'
-    )
-
-
 def test_hide_secrets_trailing_secret():
-    origin = "password1: foobar\npassword: barfoo"
-    expectation = 'password1: "{{ password1 }}"\npassword: "{{ password }}"'
-    assert hide_secrets(origin) == expectation
+    sample = "password1: foobar\npassword: barfoo"
+    root_node = parse_raw_block(sample)
+    passwords = {
+        t.secret_value_of.text: t.text for t in flatten(root_node) if t.type is NodeType.secret
+    }
+    assert passwords == {"password1": "foobar", "password": "barfoo"}
 
 
 def test_hide_secrets_quoted_field():
-    origin = """
+    sample = """
     "password9": "my_password10: maxplus"
     """
-    expectation = """
-    "password9": "{{ password9 }}"
-    """
-    assert hide_secrets(origin) == expectation
+    root_node = parse_raw_block(sample)
+    passwords = {
+        t.secret_value_of.text: t.text for t in flatten(root_node) if t.type is NodeType.secret
+    }
+    assert passwords == {"password9": "my_password10: maxplus"}
 
 
-def test_hide_secrets_unquoted_field():
-    origin = """
+def test_parse_secrets_unquoted_field():
+    sample = """
     password9: "my_password10: maxplus"
     """
-    expectation = """
-    password9: "{{ password9 }}"
-    """
-    assert hide_secrets(origin) == expectation
+    root_node = parse_raw_block(sample)
+    passwords = {
+        t.secret_value_of.text: t.text for t in flatten(root_node) if t.type is NodeType.secret
+    }
+    assert passwords == {"password9": "my_password10: maxplus"}
 
 
-def test_hide_secrets_pattern_within_quoted_string():
-    origin = """
+def test_parse_secrets_pattern_within_quoted_string():
+    sample = """
     'password9: "my_password10: maxplus"'
     """
-    expectation = """
-    'password9: "{{ password9 }}"'
-    """
-    assert hide_secrets(origin) == expectation
+    root_node = parse_raw_block(sample)
+    passwords = {
+        t.secret_value_of.text: t.text for t in flatten(root_node) if t.type is NodeType.secret
+    }
+    assert passwords == {"password9": "my_password10: maxplus"}
 
 
-def test_hide_secrets_long_string():
-    origin = """
+def test_parse_secrets_long_string():
+    sample = """
     passwd: $6$j212wezy$7H/1LT4f9/N3wpgNunhsIqtMj62OKiS3nyNwuizouQc3u7MbYCarYeAHWYPYb2FT.lbioDm2RrkJPb9BZMN1O/
     """  # noqa: E501
-    expectation = """
-    passwd: "{{ passwd }}"
-    """
-    assert hide_secrets(origin) == expectation
+    root_node = parse_raw_block(sample)
+    passwords = {
+        t.secret_value_of.text: t.text for t in flatten(root_node) if t.type is NodeType.secret
+    }
+    assert passwords == {
+        "passwd": (
+            "$6$j212wezy$7H/1LT4f9/N3wpgNunhsIqtMj62OKiS3nyNwuizo"
+            "uQc3u7MbYCarYeAHWYPYb2FT.lbioDm2RrkJPb9BZMN1O/"
+        )
+    }
 
 
-def test_hide_secrets_2_level_of_quotes():
-    origin = """
+def test_parse_secrets_2_level_of_quotes():
+    sample = """
     "aaa'
        passwd: bob'"
     """
-    expectation = """
-    "aaa'
-       passwd: {{ passwd }}'"
-    """
-    assert hide_secrets(origin) == expectation
+    root_node = parse_raw_block(sample)
+    passwords = {
+        t.secret_value_of.text: t.text for t in flatten(root_node) if t.type is NodeType.secret
+    }
+    assert passwords == {"passwd": "bob"}
 
 
-def test_hide_secrets_protected_double_quotes():
-    origin = """
+def test_parse_secrets_protected_double_quotes():
+    sample = """
     "aaa
        \\"passwd: bob\\""
     """
-    expectation = """
-    "aaa
-       \\"passwd: {{ passwd }}\\""
-    """
-    assert hide_secrets(origin) == expectation
+    root_node = parse_raw_block(sample)
+    passwords = {
+        t.secret_value_of.text: t.text for t in flatten(root_node) if t.type is NodeType.secret
+    }
+    assert passwords == {"passwd": "bob"}
 
 
-def test_hide_secrets_empty():
-    origin = ""
-    expectation = ""
-    assert hide_secrets(origin) == expectation
+def test_parse_secrets_empty():
+    sample = ""
+    root_node = parse_raw_block(sample)
+    nodes = list(flatten(root_node))
+    assert len(nodes) == 1
 
 
-def test_hide_secrets_field_only():
-    origin = "passwd"
-    expectation = "passwd"
-    assert hide_secrets(origin) == expectation
+def test_parse_secrets_field_only():
+    sample = "passwd"
+    root_node = parse_raw_block(sample)
+    nodes = list(flatten(root_node))
+    assert len(nodes) == 2
+    assert nodes[-1].text == sample
 
 
-def test_hide_secrets_vars_file():
-    origin = """
+def test_parse_secrets_vars_file():
+    sample = """
     ansible_user: root
     ansible_host: esxi1-gw.ws.testing.ansible.com
     ansible_password: '!234AaAa56'
     """
-    expectation = """
-    ansible_user: root
-    ansible_host: esxi1-gw.ws.testing.ansible.com
-    ansible_password: '{{ ansible_password }}'
-    """
-    assert hide_secrets(dedent(origin)) == dedent(expectation)
+    root_node = parse_raw_block(sample)
+    passwords = {
+        t.secret_value_of.text: t.text for t in flatten(root_node) if t.type is NodeType.secret
+    }
+    assert passwords == {"ansible_password": "!234AaAa56"}
 
 
-def test_hide_secrets_unquoted_string():
-    origin = """
+def test_parse_secrets_unquoted_string():
+    sample = """
     ansible_password: an unquoted string
     """
-    expectation = """
-    ansible_password: "{{ ansible_password }}"
-    """
-    assert hide_secrets(dedent(origin)) == dedent(expectation)
+    root_node = parse_raw_block(dedent(sample))
+    nodes = list(flatten(root_node))
+    assert nodes[-2].text == "an unquoted string"
+    assert nodes[-2].secret_value_of.text == "ansible_password"
 
 
-def test_hide_secrets_multi_secrets():
-    origin = """
+def test_parse_secrets_multi_secrets():
+    sample = """
     '(?i)password1:': "{{ _iosxr_password }}"
     "this is somethingpass: password2: else my_password3: 'password4: _Agaim': barfoo"
     password5: maxplus
     password6: "maxplus"
     password7: "my_password8: maxplus"
     "password9": "my_password10: maxplus"
     password11: "my_password12:
               maxplus"
 
     passwd: $6$j212wezy$7H/1LT4f9/N3wpgNunhsIqtMj62OKiS3nyNwuizouQc3u7MbYCarYeAHWYPYb2FT.lbioDm2RrkJPb9BZMN1O/
     """  # noqa: E501
-    expectation = """
-    '(?i)password1:': "{{ _iosxr_password }}"
-    "this is somethingpass: {{ somethingpass }}: else my_password3: '{{ my_password3 }}': barfoo"
-    password5: "{{ password5 }}"
-    password6: "{{ password6 }}"
-    password7: "{{ password7 }}"
-    "password9": "{{ password9 }}"
-    password11: "{{ password11 }}"
-
-    passwd: "{{ passwd }}"
-    """
-    assert hide_secrets(origin) == expectation
-
-
-def test_hide_secrets_aws_profile():
-    origin = """
-    [my-secret-account]
-    aws_access_key_id = BJIA5UUFYYOOKZQODC3F
-    aws_secret_access_key = NeTL/2vPPnlnb/8RBtsw3EwnNjflDbgZiDmRskhb
-    """
-
-    expectation = """
-    [my-secret-account]
-    aws_access_key_id = "{{ aws_access_key_id }}"
-    aws_secret_access_key = "{{ aws_secret_access_key }}"
-    """
-    assert hide_secrets(dedent(origin)) == dedent(expectation)
+    root_node = parse_raw_block(sample)
+    passwords = {
+        t.secret_value_of.text: t.text for t in flatten(root_node) if t.type is NodeType.secret
+    }
+    assert passwords == {
+        "somethingpass": "password2",
+        "my_password3": "password4: _Agaim",
+        "password5": "maxplus",
+        "password6": "maxplus",
+        "password7": "my_password8: maxplus",
+        "password9": "my_password10: maxplus",
+        "password11": "my_password12:\n              maxplus",
+        "passwd": (
+            "$6$j212wezy$7H/1LT4f9/N3wpgNunhsIqtMj62OKiS3n"
+            "yNwuizouQc3u7MbYCarYeAHWYPYb2FT.lbioDm2RrkJPb9"
+            "BZMN1O/"
+        ),
+    }
 
 
 def test_parser_simple_key_value_string():
     sample = 'config_reverseproxy_oauth_password: "passw0rd"'
     expectation = [
         ("", NodeType.quoted_string_holder),
         ("config_reverseproxy_oauth_password", NodeType.field),
         (":", NodeType.separator),
         (" ", NodeType.space),
         ('"', NodeType.quoted_string_holder),
         ("passw0rd", NodeType.field),
         ('"', NodeType.quoted_string_closing),
     ]
-    root_node = parser(sample)
+    root_node = breakup_elements(sample)
     expanded = [(c.text, c.type) for c in flatten(root_node)]
     assert expanded == expectation
 
 
 def test_parser_multi_spaces_before_simple_key_value_string():
     sample = 'config_reverseproxy_oauth_password:      "passw0rd"'
     expectation = [
@@ -220,91 +194,187 @@
         (" ", NodeType.space),
         (" ", NodeType.space),
         (" ", NodeType.space),
         ('"', NodeType.quoted_string_holder),
         ("passw0rd", NodeType.field),
         ('"', NodeType.quoted_string_closing),
     ]
-    root_node = parser(sample)
+    root_node = breakup_elements(sample)
     expanded = [(c.text, c.type) for c in flatten(root_node)]
     assert expanded == expectation
 
 
 def test_parser_get_secret():
     sample = "config_reverseproxy_oauth_password: my_secret"
-    root_node = parser(sample)
+    root_node = breakup_elements(sample)
     list_of_nodes = list(flatten(root_node))
     field_name_node = list_of_nodes[1]
     assert field_name_node.text == "config_reverseproxy_oauth_password"
     assert field_name_node.get_secret().text == "my_secret"
 
 
 def test_parser_get_secret_with_unquoted_special_chars():
     sample = "config_reverseproxy_oauth_password: %$#my_secret&"
-    root_node = parser(sample)
+    root_node = breakup_elements(sample)
     field_name_node = root_node.next
     assert field_name_node.text == "config_reverseproxy_oauth_password"
     # Without combinate_value_fields we only get the first node of the secret
-    assert field_name_node.get_secret().text == "%$#"
+    assert field_name_node.get_secret().text == "%"
     combinate_value_fields(root_node)
     assert field_name_node.get_secret().text == "%$#my_secret&"
 
 
 def test_parser_get_secret_with_ini_file():
     sample = """
     [default]
     foo = bar
     key=value
     turbo_secret=@#%$%^&^^ 645
 
     [section.bar]
     George = # a comment
     """
-    root_node = parser(dedent(sample))
+    root_node = breakup_elements(dedent(sample))
     secret_node = [n for n in flatten(root_node) if n.text == "turbo_secret"][0]
     # Without combinate_value_fields we only get the first node of the secret
     combinate_value_fields(root_node)
     assert secret_node.get_secret().text == "@#%$%^&^^ 645"
 
 
 def test_combinate_value_fields():
     sample = "config_reverseproxy_oauth_password: my!secret%$!"
-    root_node = parser(sample)
-    assert len(list(flatten(root_node))) == 8
+    root_node = breakup_elements(sample)
+    assert len(list(flatten(root_node))) == 10
     combinate_value_fields(root_node)
     assert len(list(flatten(root_node))) == 5
 
 
 def test_hide_secrets_multi_spaces_before_simple_key_value_string():
     sample = 'config_reverseproxy_oauth_password:      "passw0rd"'
-    assert (
-        hide_secrets(sample)
-        == 'config_reverseproxy_oauth_password:      "{{ config_reverseproxy_oauth_password }}"'
-    )
+    root_node = parse_raw_block(sample)
+    nodes = list(flatten(root_node))
+    assert nodes[-2].text == "passw0rd"
+    assert nodes[-2].type is NodeType.secret
 
 
 def test_parser_unquoted_password_with_special_chars():
     sample = 'my_password=      !pass w0rd"'
-    assert hide_secrets(sample) == 'my_password=      "{{ my_password }}"'
+    root_node = parse_raw_block(sample)
+    nodes = list(flatten(root_node))
+    assert [t.type for t in nodes] == [
+        NodeType.quoted_string_holder,
+        NodeType.field,
+        NodeType.separator,
+        NodeType.space,
+        NodeType.space,
+        NodeType.space,
+        NodeType.space,
+        NodeType.space,
+        NodeType.space,
+        NodeType.secret,
+    ]
+    assert nodes[-1].type is NodeType.secret
+    assert nodes[-1].text == '!pass w0rd"'
 
 
 def test_parser_two_passwords_on_same_line():
     sample = 'my_password:      !pass w0rd  another_password: hide_thís "'
-    assert (
-        hide_secrets(sample)
-        == 'my_password:      "{{ my_password }}"  another_password: "{{ another_password }}"'
-    )
+    root_node = parse_raw_block(sample)
+    nodes = list(flatten(root_node))
+    assert [t.type for t in nodes] == [
+        NodeType.quoted_string_holder,
+        NodeType.field,
+        NodeType.separator,
+        NodeType.space,
+        NodeType.space,
+        NodeType.space,
+        NodeType.space,
+        NodeType.space,
+        NodeType.space,
+        NodeType.secret,
+        NodeType.space,
+        NodeType.space,
+        NodeType.field,
+        NodeType.separator,
+        NodeType.space,
+        NodeType.secret,
+    ]
+    assert nodes[9].type is NodeType.secret
+    assert nodes[9].text == "!pass w0rd"
+
+    assert nodes[-1].type is NodeType.secret
+    assert nodes[-1].text == 'hide_thís "'
 
 
 def test_parser_one_password_and_one_regular_kv_on_same_line():
     sample = "my_password:      !pass w0rd  some-key: show-this"
-    assert hide_secrets(sample) == 'my_password:      "{{ my_password }}"  some-key: show-this'
+    root_node = parse_raw_block(sample)
+    nodes = list(flatten(root_node))
+    assert [t.type for t in nodes] == [
+        NodeType.quoted_string_holder,
+        NodeType.field,
+        NodeType.separator,
+        NodeType.space,
+        NodeType.space,
+        NodeType.space,
+        NodeType.space,
+        NodeType.space,
+        NodeType.space,
+        NodeType.secret,
+        NodeType.space,
+        NodeType.space,
+        NodeType.field,
+        NodeType.separator,
+        NodeType.space,
+        NodeType.field,
+    ]
+    assert nodes[9].type is NodeType.secret
+    assert nodes[9].text == "!pass w0rd"
 
 
 def test_parser_yaml_unquoted_password_with_a_equal_sign():
     sample = 'my_password:     !pass=w0rd"'
-    assert hide_secrets(sample) == 'my_password:     "{{ my_password }}"'
+    root_node = parse_raw_block(sample)
+    nodes = list(flatten(root_node))
+    assert nodes[-1].secret_value_of is nodes[1]
+    assert nodes[-1].type is NodeType.secret
+    assert nodes[-1].text == '!pass=w0rd"'
 
 
 def test_parser_ini_unquoted_password_with_a_colon_sign():
     sample = 'my_password = !pass:w0rd"'
-    assert hide_secrets(sample) == 'my_password = "{{ my_password }}"'
+    root_node = parse_raw_block(sample)
+    nodes = list(flatten(root_node))
+    assert nodes[-1].secret_value_of is nodes[1]
+    assert nodes[-1].type is NodeType.secret
+    assert nodes[-1].text == '!pass:w0rd"'
+
+
+def test_parser_empty_quoted_secret():
+    sample = 'password=""'
+    root_node = breakup_elements(sample)
+    node_types_found = [n.type for n in flatten(root_node)]
+    assert node_types_found == [
+        NodeType.quoted_string_holder,
+        NodeType.field,
+        NodeType.separator,
+        NodeType.quoted_string_holder,
+        NodeType.quoted_string_closing,
+    ]
+    nodes_found = list(flatten(root_node))
+    assert nodes_found[-2].closed_by == nodes_found[-1]
+
+
+def test_parser_one_character_quoted_secret():
+    sample = 'password="a"'
+    root_node = breakup_elements(sample)
+    node_types_found = [n.type for n in flatten(root_node)]
+    assert node_types_found == [
+        NodeType.quoted_string_holder,
+        NodeType.field,
+        NodeType.separator,
+        NodeType.quoted_string_holder,
+        NodeType.field,
+        NodeType.quoted_string_closing,
+    ]
+    nodes_found = list(flatten(root_node))
+    assert nodes_found[-3].closed_by == nodes_found[-1]
```

### Comparing `ansible-anonymizer-1.3.0/tox.ini` & `ansible-anonymizer-1.4.0/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 [testenv:mypy]
 basepython = python3.11
 skip_install = true
 deps =
     {[testenv]deps}
     mypy
     types-PyYAML
-commands = mypy --strict ansible_anonymizer
+commands = mypy --no-strict-optional --strict ansible_anonymizer
 
 [testenv:black]
 basepython = python3.11
 deps =
     {[testenv]deps}
     black
 commands = black --check --line-length 100 ansible_anonymizer tests
```

