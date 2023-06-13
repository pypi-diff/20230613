# Comparing `tmp/myl-0.7.1.tar.gz` & `tmp/myl-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myl-0.7.1.tar", last modified: Tue Jun 13 17:24:06 2023, max compression
+gzip compressed data, was "myl-0.8.0.tar", last modified: Tue Jun 13 19:05:39 2023, max compression
```

## Comparing `myl-0.7.1.tar` & `myl-0.8.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:24:06.231727 myl-0.7.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:24:06.227728 myl-0.7.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-13 17:23:37.000000 myl-0.7.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:24:06.227728 myl-0.7.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-13 17:23:37.000000 myl-0.7.1/.github/workflows/lint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-13 17:23:37.000000 myl-0.7.1/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-13 17:23:37.000000 myl-0.7.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-13 17:23:37.000000 myl-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    40931 2023-06-13 17:24:06.231727 myl-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-13 17:23:37.000000 myl-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:24:06.231727 myl-0.7.1/myl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    40931 2023-06-13 17:24:06.000000 myl-0.7.1/myl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-13 17:24:06.000000 myl-0.7.1/myl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 17:24:06.000000 myl-0.7.1/myl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-13 17:24:06.000000 myl-0.7.1/myl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-13 17:24:06.000000 myl-0.7.1/myl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-13 17:24:06.000000 myl-0.7.1/myl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-06-13 17:23:37.000000 myl-0.7.1/myl.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-13 17:23:37.000000 myl-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 17:24:06.231727 myl-0.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:05:39.712104 myl-0.8.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:05:39.712104 myl-0.8.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-13 19:05:25.000000 myl-0.8.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:05:39.712104 myl-0.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-13 19:05:25.000000 myl-0.8.0/.github/workflows/lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-13 19:05:25.000000 myl-0.8.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-13 19:05:25.000000 myl-0.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-13 19:05:25.000000 myl-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    40931 2023-06-13 19:05:39.712104 myl-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-13 19:05:25.000000 myl-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:05:39.712104 myl-0.8.0/myl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    40931 2023-06-13 19:05:39.000000 myl-0.8.0/myl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-13 19:05:39.000000 myl-0.8.0/myl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 19:05:39.000000 myl-0.8.0/myl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-13 19:05:39.000000 myl-0.8.0/myl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-13 19:05:39.000000 myl-0.8.0/myl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-13 19:05:39.000000 myl-0.8.0/myl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7599 2023-06-13 19:05:25.000000 myl-0.8.0/myl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-13 19:05:25.000000 myl-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 19:05:39.712104 myl-0.8.0/setup.cfg
```

### Comparing `myl-0.7.1/.github/workflows/release.yaml` & `myl-0.8.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `myl-0.7.1/LICENSE` & `myl-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `myl-0.7.1/PKG-INFO` & `myl-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myl
-Version: 0.7.1
+Version: 0.8.0
 Summary: Dead simple IMAP CLI client
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `myl-0.7.1/myl.egg-info/PKG-INFO` & `myl-0.8.0/myl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myl
-Version: 0.7.1
+Version: 0.8.0
 Summary: Dead simple IMAP CLI client
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `myl-0.7.1/myl.py` & `myl-0.8.0/myl.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import argparse
 import logging
+import re
 import sys
 
+import dns.resolver
 import imap_tools
+import requests
+import xmltodict
 from rich import print
 from rich.console import Console
 from rich.table import Table
 
 LOGGER = logging.getLogger(__name__)
 GMAIL_IMAP_SERVER = "imap.gmail.com"
 GMAIL_IMAP_PORT = 993
@@ -24,14 +28,22 @@
         "-s", "--server", help="IMAP server address", required=False
     )
     parser.add_argument(
         "--google",
         "--gmail",
         help="Use Google IMAP settings (overrides --port, --server etc.)",
         action="store_true",
+        default=False,
+    )
+    parser.add_argument(
+        "-a",
+        "--auto",
+        help="Autodiscovery of the required server and port",
+        action="store_true",
+        default=False,
     )
     parser.add_argument("-P", "--port", help="IMAP server port", default=143)
     parser.add_argument("--starttls", help="Start TLS", action="store_true")
     parser.add_argument(
         "-c",
         "--count",
         help="Number of messages to fetch",
@@ -79,43 +91,115 @@
         args.starttls = False
 
         if args.sent or args.folder == "Sent":
             args.folder = GMAIL_SENT_FOLDER
         # elif args.folder == "INBOX":
         #     args.folder = GMAIL_ALL_FOLDER
     else:
+        if args.auto:
+            settings = autodiscover(args.username)
+            args.server = settings.get("server")
+            args.port = settings.get("port")
+            args.starttls = settings.get("starttls")
         if args.sent:
             args.folder = "Sent"
 
     if not args.server:
         error_msg("No server specified")
         parser.print_help()
         sys.exit(2)
 
     return args
 
 
-def main():
-    args = parse_args()
+def resolve_txt(domain, criteria="^mailconf="):
+    regex = re.compile(criteria)
+    answers = dns.resolver.resolve(domain, "TXT")
+    for rdata in answers:
+        for txt_string in rdata.strings:
+            txt_record = txt_string.decode("utf-8")
+            if re.search(regex, txt_record):
+                return txt_record
+
+
+def resolve_srv(domain):
+    answers = dns.resolver.resolve(domain, "SRV")
+    data = []
+    for rdata in answers:
+        entry = {
+            "hostname": ".".join(
+                [
+                    x.decode("utf-8")
+                    for x in rdata.target.labels
+                    if x.decode("utf-8") != ""
+                ]
+            ),
+            "port": rdata.port,
+        }
+        data.append(entry)
+
+    return data
+
+
+# TODO export this a separate library
+def autodiscover(email_addr):
+    domain = email_addr.split("@")[-1]
+    if not domain:
+        raise ValueError(f"Invalid email address {email_addr}")
+
+    autoconfig = None  # resolve_txt(domain)
+
+    if not autoconfig:
+        srv = resolve_srv(f"_imaps._tcp.{domain}")
+        return {
+            "server": srv[0].get("hostname"),
+            "port": srv[0].get("port"),
+            "starttls": False,
+        }
+
+    res = requests.get(autoconfig)
+    res.raise_for_status()
+
+    data = xmltodict.parse(res.text)
+    imap = (
+        data.get("clientConfig", {})
+        .get("emailProvider", {})
+        .get("incomingServer")
+    )
+    assert imap is not None
+    return {
+        "server": imap.get("hostname"),
+        "port": imap.get("port"),
+        "starttls": imap.get("socketType") == "STARTTLS",
+    }
 
-    table = Table(
-        expand=True,
-        show_header=not args.no_title,
-        header_style="bold",
-        show_lines=False,
-        box=None,
-    )
-    table.add_column("ID", style="red", no_wrap=not args.wrap, max_width=10)
-    table.add_column(
-        "Subject", style="green", no_wrap=not args.wrap, max_width=30
-    )
-    table.add_column("From", style="blue", no_wrap=not args.wrap, max_width=30)
-    table.add_column("Date", style="cyan", no_wrap=not args.wrap)
+
+def main():
+    console = Console()
 
     try:
+        args = parse_args()
+
+        table = Table(
+            expand=True,
+            show_header=not args.no_title,
+            header_style="bold",
+            show_lines=False,
+            box=None,
+        )
+        table.add_column(
+            "ID", style="red", no_wrap=not args.wrap, max_width=10
+        )
+        table.add_column(
+            "Subject", style="green", no_wrap=not args.wrap, max_width=30
+        )
+        table.add_column(
+            "From", style="blue", no_wrap=not args.wrap, max_width=30
+        )
+        table.add_column("Date", style="cyan", no_wrap=not args.wrap)
         mb = imap_tools.MailBoxTls if args.starttls else imap_tools.MailBox
 
         with mb(args.server, port=args.port).login(
             args.username, args.password, args.folder
         ) as mailbox:
             if args.MAILID:
                 msg = next(
@@ -157,17 +241,16 @@
                     + (msg.subject if msg.subject else "<no-subject>"),
                     msg.from_,
                     msg.date.strftime("%H:%M %d/%m/%Y") if msg.date else "???",
                 )
                 if len(table.rows) >= args.count:
                     break
 
-        console = Console()
         console.print(table)
         return 0
-    except Exception as e:
-        LOGGER.error(e)
+    except Exception:
+        console.print_exception(show_locals=True)
         return 1
 
 
 if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `myl-0.7.1/pyproject.toml` & `myl-0.8.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -12,17 +12,20 @@
 requires-python = ">=3.8"
 keywords = ["imap", "email"]
 license = {file = "LICENSE"}
 classifiers = [
   "Programming Language :: Python :: 3",
 ]
 dependencies = [
+  "dnspython",
   "imap_tools",
-  "rich"
+  "requests",
+  "rich",
+  "xmltodict"
 ]
-version = "0.7.1"
+version = "0.8.0"
 
 [tool.black]
 line-length = 79
 
 [project.scripts]
 myl = "myl:main"
```

