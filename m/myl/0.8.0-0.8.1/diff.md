# Comparing `tmp/myl-0.8.0.tar.gz` & `tmp/myl-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myl-0.8.0.tar", last modified: Tue Jun 13 19:05:39 2023, max compression
+gzip compressed data, was "myl-0.8.1.tar", last modified: Tue Jun 13 19:29:31 2023, max compression
```

## Comparing `myl-0.8.0.tar` & `myl-0.8.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:05:39.712104 myl-0.8.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:05:39.712104 myl-0.8.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-13 19:05:25.000000 myl-0.8.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:05:39.712104 myl-0.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-13 19:05:25.000000 myl-0.8.0/.github/workflows/lint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-13 19:05:25.000000 myl-0.8.0/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-13 19:05:25.000000 myl-0.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-13 19:05:25.000000 myl-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    40931 2023-06-13 19:05:39.712104 myl-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-13 19:05:25.000000 myl-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:05:39.712104 myl-0.8.0/myl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    40931 2023-06-13 19:05:39.000000 myl-0.8.0/myl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-13 19:05:39.000000 myl-0.8.0/myl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 19:05:39.000000 myl-0.8.0/myl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-13 19:05:39.000000 myl-0.8.0/myl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-13 19:05:39.000000 myl-0.8.0/myl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-13 19:05:39.000000 myl-0.8.0/myl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7599 2023-06-13 19:05:25.000000 myl-0.8.0/myl.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-13 19:05:25.000000 myl-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 19:05:39.712104 myl-0.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:29:31.050301 myl-0.8.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:29:31.050301 myl-0.8.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-13 19:29:19.000000 myl-0.8.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:29:31.050301 myl-0.8.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-13 19:29:19.000000 myl-0.8.1/.github/workflows/lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-13 19:29:19.000000 myl-0.8.1/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-13 19:29:19.000000 myl-0.8.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-13 19:29:19.000000 myl-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    40931 2023-06-13 19:29:31.050301 myl-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-13 19:29:19.000000 myl-0.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:29:31.050301 myl-0.8.1/myl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    40931 2023-06-13 19:29:31.000000 myl-0.8.1/myl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-13 19:29:31.000000 myl-0.8.1/myl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 19:29:31.000000 myl-0.8.1/myl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-13 19:29:31.000000 myl-0.8.1/myl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-13 19:29:31.000000 myl-0.8.1/myl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-13 19:29:31.000000 myl-0.8.1/myl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8368 2023-06-13 19:29:19.000000 myl-0.8.1/myl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-13 19:29:19.000000 myl-0.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 19:29:31.050301 myl-0.8.1/setup.cfg
```

### Comparing `myl-0.8.0/.github/workflows/release.yaml` & `myl-0.8.1/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `myl-0.8.0/LICENSE` & `myl-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `myl-0.8.0/PKG-INFO` & `myl-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myl
-Version: 0.8.0
+Version: 0.8.1
 Summary: Dead simple IMAP CLI client
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `myl-0.8.0/myl.egg-info/PKG-INFO` & `myl-0.8.1/myl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myl
-Version: 0.8.0
+Version: 0.8.1
 Summary: Dead simple IMAP CLI client
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `myl-0.8.0/myl.py` & `myl-0.8.1/myl.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,29 +5,32 @@
 
 import dns.resolver
 import imap_tools
 import requests
 import xmltodict
 from rich import print
 from rich.console import Console
+from rich.logging import RichHandler
 from rich.table import Table
 
 LOGGER = logging.getLogger(__name__)
+IMAP_PORT = 993
 GMAIL_IMAP_SERVER = "imap.gmail.com"
-GMAIL_IMAP_PORT = 993
+GMAIL_IMAP_PORT = IMAP_PORT
 GMAIL_SENT_FOLDER = "[Gmail]/Sent Mail"
 # GMAIL_ALL_FOLDER = "[Gmail]/All Mail"
 
 
 def error_msg(msg):
     print(f"[red]{msg}[/red]", file=sys.stderr)
 
 
 def parse_args():
     parser = argparse.ArgumentParser()
+    parser.add_argument("-d", "--debug", help="Debug", action="store_true")
     parser.add_argument(
         "-s", "--server", help="IMAP server address", required=False
     )
     parser.add_argument(
         "--google",
         "--gmail",
         help="Use Google IMAP settings (overrides --port, --server etc.)",
@@ -37,16 +40,20 @@
     parser.add_argument(
         "-a",
         "--auto",
         help="Autodiscovery of the required server and port",
         action="store_true",
         default=False,
     )
-    parser.add_argument("-P", "--port", help="IMAP server port", default=143)
-    parser.add_argument("--starttls", help="Start TLS", action="store_true")
+    parser.add_argument(
+        "-P", "--port", help="IMAP server port", default=IMAP_PORT
+    )
+    parser.add_argument(
+        "--starttls", help="Start TLS", action="store_true", default=False
+    )
     parser.add_argument(
         "-c",
         "--count",
         help="Number of messages to fetch",
         default=10,
         type=int,
     )
@@ -79,40 +86,15 @@
         default=False,
     )
     parser.add_argument("MAILID", help="Mail ID to fetch", nargs="?")
     parser.add_argument(
         "ATTACHMENT", help="Name of the attachment to fetch", nargs="?"
     )
 
-    args = parser.parse_args()
-
-    if args.google:
-        args.server = GMAIL_IMAP_SERVER
-        args.port = GMAIL_IMAP_PORT
-        args.starttls = False
-
-        if args.sent or args.folder == "Sent":
-            args.folder = GMAIL_SENT_FOLDER
-        # elif args.folder == "INBOX":
-        #     args.folder = GMAIL_ALL_FOLDER
-    else:
-        if args.auto:
-            settings = autodiscover(args.username)
-            args.server = settings.get("server")
-            args.port = settings.get("port")
-            args.starttls = settings.get("starttls")
-        if args.sent:
-            args.folder = "Sent"
-
-    if not args.server:
-        error_msg("No server specified")
-        parser.print_help()
-        sys.exit(2)
-
-    return args
+    return parser.parse_args()
 
 
 def resolve_txt(domain, criteria="^mailconf="):
     regex = re.compile(criteria)
     answers = dns.resolver.resolve(domain, "TXT")
     for rdata in answers:
         for txt_string in rdata.strings:
@@ -171,37 +153,74 @@
         "port": imap.get("port"),
         "starttls": imap.get("socketType") == "STARTTLS",
     }
 
 
 def main():
     console = Console()
+    args = parse_args()
+    logging.basicConfig(
+        format="%(message)s",
+        handlers=[RichHandler(console=console)],
+        level=logging.DEBUG if args.debug else logging.INFO,
+    )
+    LOGGER.debug(args)
 
-    try:
-        args = parse_args()
+    if args.google:
+        args.server = GMAIL_IMAP_SERVER
+        args.port = GMAIL_IMAP_PORT
+        args.starttls = False
 
-        table = Table(
-            expand=True,
-            show_header=not args.no_title,
-            header_style="bold",
-            show_lines=False,
-            box=None,
-        )
-        table.add_column(
-            "ID", style="red", no_wrap=not args.wrap, max_width=10
-        )
-        table.add_column(
-            "Subject", style="green", no_wrap=not args.wrap, max_width=30
-        )
-        table.add_column(
-            "From", style="blue", no_wrap=not args.wrap, max_width=30
+        if args.sent or args.folder == "Sent":
+            args.folder = GMAIL_SENT_FOLDER
+        # elif args.folder == "INBOX":
+        #     args.folder = GMAIL_ALL_FOLDER
+    else:
+        if args.auto:
+            try:
+                settings = autodiscover(args.username)
+            except Exception:
+                error_msg("Failed to autodiscover IMAP settings")
+                if args.debug:
+                    console.print_exception(show_locals=True)
+                return 1
+            LOGGER.debug(f"Discovered settings: {settings})")
+            args.server = settings.get("server")
+            args.port = settings.get("port", IMAP_PORT)
+            args.starttls = settings.get("starttls")
+        if args.sent:
+            args.folder = "Sent"
+
+    if not args.server:
+        error_msg(
+            "No server specified\n"
+            "You need to either:\n"
+            "- specify a server using --server HOSTNAME\n"
+            "- set --google if you are using a Gmail account\n"
+            "- use --auto to attempt autodiscovery"
         )
-        table.add_column("Date", style="cyan", no_wrap=not args.wrap)
-        mb = imap_tools.MailBoxTls if args.starttls else imap_tools.MailBox
+        return 2
+
+    table = Table(
+        expand=True,
+        show_header=not args.no_title,
+        header_style="bold",
+        show_lines=False,
+        box=None,
+    )
+    table.add_column("ID", style="red", no_wrap=not args.wrap, max_width=10)
+    table.add_column(
+        "Subject", style="green", no_wrap=not args.wrap, max_width=30
+    )
+    table.add_column("From", style="blue", no_wrap=not args.wrap, max_width=30)
+    table.add_column("Date", style="cyan", no_wrap=not args.wrap)
+
+    mb = imap_tools.MailBoxTls if args.starttls else imap_tools.MailBox
 
+    try:
         with mb(args.server, port=args.port).login(
             args.username, args.password, args.folder
         ) as mailbox:
             if args.MAILID:
                 msg = next(
                     mailbox.fetch(
                         f"UID {args.MAILID}", mark_seen=args.mark_seen
```

### Comparing `myl-0.8.0/pyproject.toml` & `myl-0.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,14 @@
 dependencies = [
   "dnspython",
   "imap_tools",
   "requests",
   "rich",
   "xmltodict"
 ]
-version = "0.8.0"
+version = "0.8.1"
 
 [tool.black]
 line-length = 79
 
 [project.scripts]
 myl = "myl:main"
```

