# Comparing `tmp/attacus-0.1.5-cp310-cp310-win_amd64.whl.zip` & `tmp/attacus-0.1.6-cp310-cp310-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,23 @@
-Zip file size: 902751 bytes, number of entries: 21
+Zip file size: 975466 bytes, number of entries: 21
 -rw-rw-rw-  2.0 fat       23 b- defN 23-May-26 10:35 attacus/__about__.py
 -rw-rw-rw-  2.0 fat      165 b- defN 23-May-27 06:52 attacus/__init__.py
 -rw-rw-rw-  2.0 fat      189 b- defN 23-May-26 08:44 attacus/app.py
 -rw-rw-rw-  2.0 fat     3168 b- defN 23-May-28 18:19 attacus/artifacts.py
 -rw-rw-rw-  2.0 fat      139 b- defN 23-Jun-01 08:36 attacus/assets.py
--rw-rw-rw-  2.0 fat  2277376 b- defN 23-May-31 13:06 attacus/attacus.pyd
+-rw-rw-rw-  2.0 fat  2463744 b- defN 23-Jun-13 11:19 attacus/attacus.pyd
 -rw-rw-rw-  2.0 fat      397 b- defN 23-May-28 18:02 attacus/build.py
 -rw-rw-rw-  2.0 fat      267 b- defN 23-Jun-01 09:42 attacus/cli.py
 -rw-rw-rw-  2.0 fat      518 b- defN 23-Jun-01 08:36 attacus/flutter_config.py
 -rw-rw-rw-  2.0 fat      355 b- defN 23-May-27 08:23 attacus/flutter_view.py
 -rw-rw-rw-  2.0 fat      590 b- defN 23-Jun-01 09:05 attacus/install.py
 -rw-rw-rw-  2.0 fat      636 b- defN 23-May-28 12:49 attacus/post_build.py
 -rw-rw-rw-  2.0 fat      829 b- defN 23-Jun-01 09:07 attacus/project.py
--rw-rw-rw-  2.0 fat      668 b- defN 23-Jun-01 07:47 attacus/pyproject.py
+-rw-rw-rw-  2.0 fat      739 b- defN 23-Jun-03 11:12 attacus/pyproject.py
 -rw-rw-rw-  2.0 fat      186 b- defN 23-May-28 06:30 attacus/uninstall.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-Jun-01 09:53 attacus-0.1.5.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     4252 b- defN 23-Jun-01 09:53 attacus-0.1.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat      102 b- defN 23-Jun-01 09:53 attacus-0.1.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       44 b- defN 23-Jun-01 09:53 attacus-0.1.5.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-01 09:53 attacus-0.1.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1609 b- defN 23-Jun-01 09:53 attacus-0.1.5.dist-info/RECORD
-21 files, 2292612 bytes uncompressed, 900167 bytes compressed:  60.8%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Jun-13 11:19 attacus-0.1.6.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     4252 b- defN 23-Jun-13 11:19 attacus-0.1.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      102 b- defN 23-Jun-13 11:19 attacus-0.1.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       44 b- defN 23-Jun-13 11:19 attacus-0.1.6.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-13 11:19 attacus-0.1.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1609 b- defN 23-Jun-13 11:19 attacus-0.1.6.dist-info/RECORD
+21 files, 2479051 bytes uncompressed, 972882 bytes compressed:  60.8%
```

## zipnote {}

```diff
@@ -39,26 +39,26 @@
 
 Filename: attacus/pyproject.py
 Comment: 
 
 Filename: attacus/uninstall.py
 Comment: 
 
-Filename: attacus-0.1.5.dist-info/LICENSE
+Filename: attacus-0.1.6.dist-info/LICENSE
 Comment: 
 
-Filename: attacus-0.1.5.dist-info/METADATA
+Filename: attacus-0.1.6.dist-info/METADATA
 Comment: 
 
-Filename: attacus-0.1.5.dist-info/WHEEL
+Filename: attacus-0.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: attacus-0.1.5.dist-info/entry_points.txt
+Filename: attacus-0.1.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: attacus-0.1.5.dist-info/top_level.txt
+Filename: attacus-0.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: attacus-0.1.5.dist-info/RECORD
+Filename: attacus-0.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## attacus/pyproject.py

```diff
@@ -10,16 +10,18 @@
             setattr(self, key, value)
 
 class PyProject(Config):
     def __init__(self, config) -> None:
         super().__init__(config)
 
     @classmethod
-    def load(cls, path: Path):
+    def load(cls, path: Path) -> 'PyProject':
         path = path / 'pyproject.toml'
+        if not path.exists():
+            return None
         with open(path, "rb") as f:
             config = tomli.load(f)
             return PyProject(config)
 
     @property
     def name(self):
         return self.project.name
```

## Comparing `attacus-0.1.5.dist-info/LICENSE` & `attacus-0.1.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `attacus-0.1.5.dist-info/METADATA` & `attacus-0.1.6.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: attacus
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python Flutter Extension
 Author-email: Kurtis Fields <kurtisfields@gmail.com>
 License: MIT License        
         Copyright (c) 2023 Kurtis Fields        
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

## Comparing `attacus-0.1.5.dist-info/RECORD` & `attacus-0.1.6.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 attacus/__about__.py,sha256=ryAfvAaW7VM8g1gnCrFCPrXmcbbm99Xw44aLkwGZzaI,23
 attacus/__init__.py,sha256=aJCUEMMOC7CoN0HXU20S5egMwzY1teojhDwcDsSWfCU,165
 attacus/app.py,sha256=qdfUm8sRao1JsrGJplAVsa5xVeqco2LRQO0PzbBuFHU,189
 attacus/artifacts.py,sha256=cdlqf-RfIt8xgFQsp74YWDViW7AycRzd3fkT9xX0quI,3168
 attacus/assets.py,sha256=k1y0TXyFqH2rvm9yaGuIy_mFHFJILECScJPtgjrNtgE,139
-attacus/attacus.pyd,sha256=xsv0ooCh8dGrX7CDoxHFnGrye5yLJUiU5rozhI_XFlU,2277376
+attacus/attacus.pyd,sha256=cf_61znYi-7VlG1wqMhQGLW4FeL85OsbixC7L0n0U6Y,2463744
 attacus/build.py,sha256=bc8NoYTNFU5sH1-fGRvbi0XPOII8tXnm1Qu0i_de6IE,397
 attacus/cli.py,sha256=V8k7Dy7NKDEn6l_fWRf__u_ggmuGfqtk9meB-RTafMQ,267
 attacus/flutter_config.py,sha256=4-iwoLmiznQ_e7OTRf5ACkhiadfqQHEcNHs-Ijv447Q,518
 attacus/flutter_view.py,sha256=lFA-0N8qlBcyogR_aHvVUETf_F6YBIboYSW5b8UXBQU,355
 attacus/install.py,sha256=hqja0lcgIqrFQDF2zR2UT4f93FcvTKtExP02Rqf1lKs,590
 attacus/post_build.py,sha256=YAH74QJnJpRBrmqxoluuLOIcAKdorWQ7l_5wPRwiZQI,636
 attacus/project.py,sha256=GOafEhy5h9a2jDrwBVRoO6vqvoF23BZRT6dGo9Ill14,829
-attacus/pyproject.py,sha256=AEs-9_1E-G7OsdqIOhZFrZ-F-mzuxCb5vw4buDalTmY,668
+attacus/pyproject.py,sha256=lqnaqjOknHh4qInTXJtylGfqNJsL73j48tNfFAFYMFo,739
 attacus/uninstall.py,sha256=lSIo76H7g5Bb33Nva8nIzua-yqhXAwpQEa_kG3-dI_4,186
-attacus-0.1.5.dist-info/LICENSE,sha256=_66BWzWzllOL6nPR0Jn9JDr5IFHvfOCeTUBcY-IAOR8,1091
-attacus-0.1.5.dist-info/METADATA,sha256=epJBU9DoT0O92qmljhUWfKUr4wnOyYq5IfsMs2iykQk,4252
-attacus-0.1.5.dist-info/WHEEL,sha256=W26pYN7HLsBT1jrDSL9udgf_mdNKJmYmL23sIP-FcgM,102
-attacus-0.1.5.dist-info/entry_points.txt,sha256=oe8OVlAMzQUiONOSKXmCHVFS3t4wf4tHxYAGIulrBbQ,44
-attacus-0.1.5.dist-info/top_level.txt,sha256=MzO2IQ9x5yLfi1noaf99pmzxRu3h7OczbuZKytaFjUI,8
-attacus-0.1.5.dist-info/RECORD,,
+attacus-0.1.6.dist-info/LICENSE,sha256=_66BWzWzllOL6nPR0Jn9JDr5IFHvfOCeTUBcY-IAOR8,1091
+attacus-0.1.6.dist-info/METADATA,sha256=ZyBuF5CZrVwwGvSoeuZ7-LgTq8upmofMeRt0lW-t5-o,4252
+attacus-0.1.6.dist-info/WHEEL,sha256=W26pYN7HLsBT1jrDSL9udgf_mdNKJmYmL23sIP-FcgM,102
+attacus-0.1.6.dist-info/entry_points.txt,sha256=oe8OVlAMzQUiONOSKXmCHVFS3t4wf4tHxYAGIulrBbQ,44
+attacus-0.1.6.dist-info/top_level.txt,sha256=MzO2IQ9x5yLfi1noaf99pmzxRu3h7OczbuZKytaFjUI,8
+attacus-0.1.6.dist-info/RECORD,,
```

