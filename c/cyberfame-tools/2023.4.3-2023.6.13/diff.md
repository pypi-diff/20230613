# Comparing `tmp/cyberfame-tools-2023.4.3.tar.gz` & `tmp/cyberfame-tools-2023.6.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyberfame-tools-2023.4.3.tar", last modified: Mon Apr  3 14:46:16 2023, max compression
+gzip compressed data, was "cyberfame-tools-2023.6.13.tar", last modified: Mon Jun 12 22:42:28 2023, max compression
```

## Comparing `cyberfame-tools-2023.4.3.tar` & `cyberfame-tools-2023.6.13.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 kittyandrew  (1000) kittyandrew  (1000)        0 2023-04-03 14:46:16.081524 cyberfame-tools-2023.4.3/
--rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)       39 2023-02-11 15:59:23.000000 cyberfame-tools-2023.4.3/MANIFEST.in
--rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)      651 2023-04-03 14:46:16.081524 cyberfame-tools-2023.4.3/PKG-INFO
--rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)      123 2023-02-16 16:35:41.000000 cyberfame-tools-2023.4.3/README.md
-drwxrwxr-x   0 kittyandrew  (1000) kittyandrew  (1000)        0 2023-04-03 14:46:16.077524 cyberfame-tools-2023.4.3/cyberfame_tools.egg-info/
--rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)      651 2023-04-03 14:46:15.000000 cyberfame-tools-2023.4.3/cyberfame_tools.egg-info/PKG-INFO
--rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)      349 2023-04-03 14:46:16.000000 cyberfame-tools-2023.4.3/cyberfame_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)        1 2023-04-03 14:46:15.000000 cyberfame-tools-2023.4.3/cyberfame_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)       15 2023-04-03 14:46:15.000000 cyberfame-tools-2023.4.3/cyberfame_tools.egg-info/top_level.txt
-drwxrwxr-x   0 kittyandrew  (1000) kittyandrew  (1000)        0 2023-04-03 14:46:16.081524 cyberfame-tools-2023.4.3/cyberfametools/
--rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)      151 2023-04-03 14:46:07.000000 cyberfame-tools-2023.4.3/cyberfametools/__init__.py
--rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)      729 2023-02-16 16:37:02.000000 cyberfame-tools-2023.4.3/cyberfametools/__main__.py
--rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)     2057 2023-04-03 14:44:52.000000 cyberfame-tools-2023.4.3/cyberfametools/basic.py
-drwxrwxr-x   0 kittyandrew  (1000) kittyandrew  (1000)        0 2023-04-03 14:46:16.081524 cyberfame-tools-2023.4.3/cyberfametools/data/
--rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)   341846 2023-02-13 21:39:19.000000 cyberfame-tools-2023.4.3/cyberfametools/data/packed.bin
--rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)    17903 2023-03-30 14:11:09.000000 cyberfame-tools-2023.4.3/cyberfametools/gh.py
--rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)     9008 2023-02-13 21:39:37.000000 cyberfame-tools-2023.4.3/cyberfametools/identification.py
--rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)       38 2023-04-03 14:46:16.081524 cyberfame-tools-2023.4.3/setup.cfg
--rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)     1054 2023-02-16 16:35:11.000000 cyberfame-tools-2023.4.3/setup.py
+drwxrwxr-x   0 kittyandrew  (1000) kittyandrew  (1000)        0 2023-06-12 22:42:28.156998 cyberfame-tools-2023.6.13/
+-rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)       39 2023-02-11 15:59:23.000000 cyberfame-tools-2023.6.13/MANIFEST.in
+-rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)      652 2023-06-12 22:42:28.156998 cyberfame-tools-2023.6.13/PKG-INFO
+-rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)      123 2023-02-16 16:35:41.000000 cyberfame-tools-2023.6.13/README.md
+drwxrwxr-x   0 kittyandrew  (1000) kittyandrew  (1000)        0 2023-06-12 22:42:28.148998 cyberfame-tools-2023.6.13/cyberfame_tools.egg-info/
+-rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)      652 2023-06-12 22:42:28.000000 cyberfame-tools-2023.6.13/cyberfame_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)      349 2023-06-12 22:42:28.000000 cyberfame-tools-2023.6.13/cyberfame_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)        1 2023-06-12 22:42:28.000000 cyberfame-tools-2023.6.13/cyberfame_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)       15 2023-06-12 22:42:28.000000 cyberfame-tools-2023.6.13/cyberfame_tools.egg-info/top_level.txt
+drwxrwxr-x   0 kittyandrew  (1000) kittyandrew  (1000)        0 2023-06-12 22:42:28.152998 cyberfame-tools-2023.6.13/cyberfametools/
+-rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)      152 2023-06-12 22:41:50.000000 cyberfame-tools-2023.6.13/cyberfametools/__init__.py
+-rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)      729 2023-02-16 16:37:02.000000 cyberfame-tools-2023.6.13/cyberfametools/__main__.py
+-rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)     2057 2023-04-03 14:51:16.000000 cyberfame-tools-2023.6.13/cyberfametools/basic.py
+drwxrwxr-x   0 kittyandrew  (1000) kittyandrew  (1000)        0 2023-06-12 22:42:28.152998 cyberfame-tools-2023.6.13/cyberfametools/data/
+-rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)   341846 2023-02-13 21:39:19.000000 cyberfame-tools-2023.6.13/cyberfametools/data/packed.bin
+-rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)    19090 2023-06-12 19:14:57.000000 cyberfame-tools-2023.6.13/cyberfametools/gh.py
+-rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)     9008 2023-02-13 21:39:37.000000 cyberfame-tools-2023.6.13/cyberfametools/identification.py
+-rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)       38 2023-06-12 22:42:28.156998 cyberfame-tools-2023.6.13/setup.cfg
+-rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)     1054 2023-02-16 16:35:11.000000 cyberfame-tools-2023.6.13/setup.py
```

### Comparing `cyberfame-tools-2023.4.3/PKG-INFO` & `cyberfame-tools-2023.6.13/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberfame-tools
-Version: 2023.4.3
+Version: 2023.6.13
 Summary: Answering interesting cybersecurity questions with graph theory.
 Author: Cyberfame Team
 Author-email: contact@morphysm.com
 Keywords: cyberfame tools
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cyberfame-tools-2023.4.3/cyberfame_tools.egg-info/PKG-INFO` & `cyberfame-tools-2023.6.13/cyberfame_tools.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberfame-tools
-Version: 2023.4.3
+Version: 2023.6.13
 Summary: Answering interesting cybersecurity questions with graph theory.
 Author: Cyberfame Team
 Author-email: contact@morphysm.com
 Keywords: cyberfame tools
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cyberfame-tools-2023.4.3/cyberfametools/__main__.py` & `cyberfame-tools-2023.6.13/cyberfametools/__main__.py`

 * *Files identical despite different names*

### Comparing `cyberfame-tools-2023.4.3/cyberfametools/basic.py` & `cyberfame-tools-2023.6.13/cyberfametools/basic.py`

 * *Files identical despite different names*

### Comparing `cyberfame-tools-2023.4.3/cyberfametools/data/packed.bin` & `cyberfame-tools-2023.6.13/cyberfametools/data/packed.bin`

 * *Files identical despite different names*

### Comparing `cyberfame-tools-2023.4.3/cyberfametools/gh.py` & `cyberfame-tools-2023.6.13/cyberfametools/gh.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from pprint import pprint
 from uuid import uuid4
 from io import BytesIO
 import itertools
 import argparse
 import aiohttp
 import asyncio
+import logging
 import tarfile
 import random
 import time
 import json
 import sys
 import os
 
@@ -124,40 +125,41 @@
             async with session.post(self.endpoint, json={"query": query}, headers=headers) as r:
                 data = await r.json()
 
                 if data.get("message"):
                     error = data["message"].lower()
                     if "you have exceeded a secondary rate limit" in error:
                         raise GithubRateLimitError
+
+                    logging.error("ERROR: message present: %s", json.dumps(data, indent=4))
+
                     raise GithubUnknownError("unknown github error..")
 
                 if "errors" in data:
                     error = data["errors"][0]["message"].lower()
 
                     if "could not resolve to a repository with the name" in error:
                         raise GithubNotFoundError
 
-                    print(f"ERROR: bad data:")
-                    pprint(data)
+                    logging.error("ERROR: bad data: %s", json.dumps(data, indent=4))
 
                     # @NOTE: Github sometimes errors out like this, maybe internal systems
                     #        there return a timeout or something like that, because response
                     #        contains 'data: None' and the following error:
                     if error == "timedout" or "something went wrong while executing your query" in error:
                         if not retries:
                             raise GithubInternalError("github missbehaving..")
 
                         await asyncio.sleep(err_sleep)
                         return await self.run_query(query, err_sleep, retries=retries-1)
 
                     raise GithubUnknownError("unknown github error..")
 
                 if not data.get("data"):
-                    print(f"ERROR: bad data:")
-                    pprint(data)
+                    logging.error("ERROR: bad data: %s", json.dumps(data, indent=4))
                     raise GithubUnknownError("unknown github error..")
 
                 return data
 
     async def rate_limit(self):
         query = """{
             rateLimit
@@ -168,15 +170,15 @@
                 resetAt
             }
         }"""
         response = await self.run_query(query)
         try:
             return response["data"]["rateLimit"]
         except KeyError:
-            print("ERROR in rate limits:", response)
+            logging.error("ERROR in rate limits: %s", json.dumps(response, indent=4))
 
     async def top_user_repos(self, user: str) -> dict:
         query = """{
             user(login: \"%s\") {
                 repositories(first: 10, orderBy: {field: STARGAZERS, direction: DESC}, isFork: false) {
                     nodes {
                         name
@@ -198,15 +200,20 @@
                     }
                 }
             }
         }""" % (org)
         response = await self.run_query(query)
         return response["data"]["organization"]
 
-    async def _shallow_dependencies(self, repo: str, mpsize: int = 10, dpsize: int = 100) -> dict:
+    async def _shallow_dependencies(self, repo: str, mpsize: int = 1, dpsize: int = 40) -> dict:
+        # TODO: Rewrite this function, possibly implement some complex heuristical algorithm
+        #       to guess/change 'dpsize' based on response success to maximize payload size,
+        #       and therefore speed/efficiency.
+        assert mpsize == 1, "mpsize>1 is broken atm, it won't work!"
+
         # Since we are using async requests, we need to apply lock per repo here,
         # so when we request two same repos in a row, the second request gets blocked
         # here and then immediatelly gets fullfilled from the cache.
         async with self.locks[repo]:
             # NOTE: Before making an actual request, we want to check our local cache to
             #       avoid wasting API quotas. Notice that this is not a regular dict but
             #       our custom 'Cache' class, where calling '__getitem__' on non-existing
@@ -219,46 +226,56 @@
             # print("", "~" * 50, f"Making a request into GH API for '{repo}'!", "~" * 50, "", sep="\n")
             owner, name = repo.split("/")
             mhas_next, mnext = True, ""
             result = {"manifests": []}
             while mhas_next:
                 dhas_next, dnext = True, ""
                 manifests = {}
-                while dhas_next:
+                skip_manifest = False
+                while dhas_next and not skip_manifest:
                     r = await self.run_query(self.DEPENDENCY_QUERY % (owner, name, mpsize, mnext, dpsize, dnext))
                     data = r["data"]["repository"]["dependencyGraphManifests"]
 
                     # Reset has_next here as a default case.
                     dhas_next = False
                     for manifest in data["nodes"]:
                         # Properly parsing filepath to the manifest:
                         #     path schema: /<resource>/<repo>/blob/<branch>/<...path/to/manifest/file.ext>
                         _prefix, branched_path = manifest["blobPath"].split("/blob/")
                         _branch, *paths, fname = branched_path.split("/")
+                        mname = "/".join((*paths, fname))
+                        logging.debug("Processing manifest: '%s' ...", mname)
 
                         # SKIP all kinds of lock files: they contain full trees instead of just first-order.
-                        if "lock" in fname:
-                            # print(f"Warn: skipped manifest '{fname}'!")
+                        if "lock" in fname or fname == "go.sum":
+                            skip_manifest = True
+                            logging.warning("Warn: skipped manifest '%s'!", mname)
                             continue
 
-                        mname = "/".join((*paths, fname))
                         if mname not in manifests:
                             manifests[mname] = {"path": mname, "dependencies": manifest["dependencies"]["nodes"]}
                         else:
                             manifests[mname]["dependencies"].extend(manifest["dependencies"]["nodes"])
 
                         # Looking for the next cursor:
                         meta = manifest["dependencies"]["pageInfo"]
                         if not dhas_next and meta["hasNextPage"]:
                             dhas_next, dnext = True, meta["endCursor"]
-                    # print(dhas_next, dnext)
+
+                    if skip_manifest: break
+
+                    logging.debug("DHAS_NEXT: %s, DNEXT: %s", dhas_next, dnext)
+                    # exit(0)
 
                 mhas_next, mnext = data["pageInfo"]["hasNextPage"], data["pageInfo"]["endCursor"]
                 result["manifests"].extend(list(manifests.values()))
-                # print(mhas_next, mnext)
+                logging.debug(
+                    "MHAS_NEXT: %s, MNEXT: %s | TOTAL deps total - %s", mhas_next, mnext,
+                    sum(map(lambda o: len(o["dependencies"]), list(manifests.values())))
+                )
 
             self.cache[repo] = result
             return result
 
     async def dependency_tree(self, repo: str, limit: int, depth: int = 0, results: list = None) -> dict:
         batch = []
 
@@ -318,15 +335,15 @@
         repo = f"{owner}/{name}"
 
         main_repo, *repos = await self.dependency_tree(repo, limit=recursion_depth, results=[])
 
         # Generating cypher for main entity:
         main_cipher = (
             "WITH $data as data\n"
-            "MATCH (e:repo {url: data.url})\n"
+            "MATCH (e:Entity|repo {url: data.url})\n"
             "SET e.name = data.name\n"
             "WITH e, data\n"
             "UNWIND data.manifests as manifest\n"
             "WITH e, manifest\n"
             "UNWIND manifest.dependencies as dep\n"
             "MERGE (d:repo {url: dep.url})\n"
             "SET d.name = dep.name\n"
@@ -380,21 +397,26 @@
         tfile.addfile(tinfo, BytesIO(encoded))
 
 
 async def main():
     parser = argparse.ArgumentParser(description="Generate dependency graph")
     parser.add_argument("repository", help="the GitHub owner/repository", nargs="?", default="")
     parser.add_argument("-r", "--recursion-depth", type=int, default=0)
-    parser.add_argument("-o", "--output", type=str, default="output.json")
+    parser.add_argument("-o", "--output", type=str, default="")
     parser.add_argument("--docker", action=argparse.BooleanOptionalAction, default=True)
     parser.add_argument("--rate-limits", action=argparse.BooleanOptionalAction, default=False)
     parser.add_argument("--top-user-repos", action=argparse.BooleanOptionalAction, default=False)
     parser.add_argument("--top-org-repos", action=argparse.BooleanOptionalAction, default=False)
     args = parser.parse_args()
 
+    logging.basicConfig(
+        format="%(asctime)s - %(filename)7s:%(lineno)-3s - %(levelname)-7s - %(message)s",
+        level=logging.INFO,
+    )
+
     api = GithubTool(token=os.environ["GITHUB_TOKEN"])
 
     if args.docker:
         # Opening entity file from TC.
         with open("entity.json") as f:
             entity = json.load(f)
 
@@ -416,14 +438,18 @@
 
         if args.top_org_repos:
             data = await api.top_org_repos(args.repository)
             print(*(repo["nameWithOwner"] for repo in data["repositories"]["nodes"]), sep="\n")
             exit(0)
 
         data = await api.dependency_tree(args.repository, limit = args.recursion_depth, results = [])
+        if not args.output:
+            print(data)
+            exit(0)
+
         with open(args.output, "w+") as f:
             # json.dump(data, f, indent=4)
             json.dump(data, f)
 
     else:
         print("You have to provide 'repository' argument (or '--docker' flag)!")
```

### Comparing `cyberfame-tools-2023.4.3/cyberfametools/identification.py` & `cyberfame-tools-2023.6.13/cyberfametools/identification.py`

 * *Files identical despite different names*

### Comparing `cyberfame-tools-2023.4.3/setup.py` & `cyberfame-tools-2023.6.13/setup.py`

 * *Files identical despite different names*

