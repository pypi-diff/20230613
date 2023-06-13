# Comparing `tmp/err_hunter-0.8.1-py2.py3-none-any.whl.zip` & `tmp/err_hunter-0.8.2-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 26884 bytes, number of entries: 20
--rw-rw-rw-  2.0 fat      614 b- defN 23-Jun-13 02:49 err_hunter/__init__.py
+Zip file size: 26886 bytes, number of entries: 20
+-rw-rw-rw-  2.0 fat      613 b- defN 23-Jun-13 03:16 err_hunter/__init__.py
 -rw-rw-rw-  2.0 fat     5182 b- defN 17-Jul-23 11:11 err_hunter/attr.py
 -rw-rw-rw-  2.0 fat     2775 b- defN 17-Jul-25 11:36 err_hunter/frame_operations.py
 -rw-rw-rw-  2.0 fat     1964 b- defN 17-Jul-23 11:14 err_hunter/myinspect.py
 -rw-rw-rw-  2.0 fat     4448 b- defN 20-Aug-05 02:22 err_hunter/mylogger.py
 -rw-rw-rw-  2.0 fat     7357 b- defN 20-Aug-05 02:19 err_hunter/mylogging.py
 -rw-rw-rw-  2.0 fat     1273 b- defN 17-Jul-25 11:32 err_hunter/traceback2.py
 -rw-rw-rw-  2.0 fat       42 b- defN 17-Jul-23 06:18 err_hunter/third_party/__init__.py
 -rw-rw-rw-  2.0 fat      270 b- defN 22-Nov-03 19:01 err_hunter/third_party/colorama/__init__.py
 -rw-rw-rw-  2.0 fat     2522 b- defN 22-Nov-03 19:01 err_hunter/third_party/colorama/ansi.py
 -rw-rw-rw-  2.0 fat    11128 b- defN 22-Nov-03 19:01 err_hunter/third_party/colorama/ansitowin32.py
 -rw-rw-rw-  2.0 fat     3325 b- defN 22-Nov-03 19:01 err_hunter/third_party/colorama/initialise.py
 -rw-rw-rw-  2.0 fat     6181 b- defN 22-Nov-03 19:01 err_hunter/third_party/colorama/win32.py
 -rw-rw-rw-  2.0 fat     7168 b- defN 22-Nov-03 19:01 err_hunter/third_party/colorama/winterm.py
--rw-rw-rw-  2.0 fat    18461 b- defN 17-Sep-20 03:44 err_hunter/third_party/logzero/__init__.py
+-rw-rw-rw-  2.0 fat    18465 b- defN 23-Jun-13 03:15 err_hunter/third_party/logzero/__init__.py
 -rw-rw-rw-  2.0 fat     2226 b- defN 17-Jul-23 06:09 err_hunter/third_party/logzero/colors.py
--rw-rw-rw-  2.0 fat      529 b- defN 23-Jun-13 02:58 err_hunter-0.8.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Jun-13 02:58 err_hunter-0.8.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Jun-13 02:58 err_hunter-0.8.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1753 b- defN 23-Jun-13 02:58 err_hunter-0.8.1.dist-info/RECORD
-20 files, 77339 bytes uncompressed, 23996 bytes compressed:  69.0%
+-rw-rw-rw-  2.0 fat      531 b- defN 23-Jun-13 03:16 err_hunter-0.8.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Jun-13 03:16 err_hunter-0.8.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Jun-13 03:16 err_hunter-0.8.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1753 b- defN 23-Jun-13 03:16 err_hunter-0.8.2.dist-info/RECORD
+20 files, 77344 bytes uncompressed, 23998 bytes compressed:  69.0%
```

## zipnote {}

```diff
@@ -42,20 +42,20 @@
 
 Filename: err_hunter/third_party/logzero/__init__.py
 Comment: 
 
 Filename: err_hunter/third_party/logzero/colors.py
 Comment: 
 
-Filename: err_hunter-0.8.1.dist-info/METADATA
+Filename: err_hunter-0.8.2.dist-info/METADATA
 Comment: 
 
-Filename: err_hunter-0.8.1.dist-info/WHEEL
+Filename: err_hunter-0.8.2.dist-info/WHEEL
 Comment: 
 
-Filename: err_hunter-0.8.1.dist-info/top_level.txt
+Filename: err_hunter-0.8.2.dist-info/top_level.txt
 Comment: 
 
-Filename: err_hunter-0.8.1.dist-info/RECORD
+Filename: err_hunter-0.8.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## err_hunter/__init__.py

```diff
@@ -12,12 +12,12 @@
 from .traceback2 import format_exc, print_exc
 from .mylogger import MyHTTPHandler, apply_handler, MultiprocessRotatingFileHandler
 from .mylogging import (
     basicConfig, colorConfig, getLogger, FILE_LOG_FORMAT,
     VERBOSE, TRACE, NOISE, LOWEST,
 )
 
-VERSION = (0, 8, 1)
+VERSION = (0, 8, 2)
 VERSION_STR = "{}.{}.{}".format(*VERSION)
 
 __version__ = VERSION
-__author__ = "Aploium<i@z.codes>"
+__author__ = "Ap<meow@meow.cat>"
```

## err_hunter/third_party/logzero/__init__.py

```diff
@@ -190,15 +190,15 @@
         """
         logging.Formatter.__init__(self, datefmt=datefmt)
 
         self._fmt = fmt
         self._colors = {}
         self._normal = ''
 
-        if color and _stderr_supports_color():
+        if color:  # and _stderr_supports_color():
             self._colors = colors
             self._normal = ForegroundColors.RESET
 
     def format(self, record):
         try:
             message = record.getMessage()
             assert isinstance(message,
```

## Comparing `err_hunter-0.8.1.dist-info/RECORD` & `err_hunter-0.8.2.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-err_hunter/__init__.py,sha256=7o1k5lTB6AroUqlJgDrEWcQ8qM1E_nGwmagzhZJ1M6g,614
+err_hunter/__init__.py,sha256=qgf8r0wVA_bXwS2dgCIyg9XHG_PMRs1ylT5jqg9uwP4,613
 err_hunter/attr.py,sha256=I1HzYS9-dmfIKKuQRCcWqJ2UhghTmyvKMlc9rSrvxoM,5182
 err_hunter/frame_operations.py,sha256=wtEGv2vAt9mrR0PUCJZuNBvq0HKuosqKJRRwcD4BOZs,2775
 err_hunter/myinspect.py,sha256=zyIJiZDW9WvxNFsgs1GUd5YCLjf-UCTuGLdjNNOPzjc,1964
 err_hunter/mylogger.py,sha256=AqZwyx1Y_S87NxNfmMwA5UlWI-Zb9L1vesCY1ByQYGw,4448
 err_hunter/mylogging.py,sha256=Utvcs8D9ET3Gtru7mkujmWZMhldQnM8lrXjCQwQWK_0,7357
 err_hunter/traceback2.py,sha256=_FJBBYyEg5eUNyVKsZFqQR2KxvtoRPRGZg6deHxR9kI,1273
 err_hunter/third_party/__init__.py,sha256=tTpcZyWtHea_pWTUz4bLHtq5jvl-3DEjhNGT41oZQlU,42
 err_hunter/third_party/colorama/__init__.py,sha256=Pc8QRY_W_6TZTyd8hv_LzkNTSh2ri0W5B0sTS86NEhY,270
 err_hunter/third_party/colorama/ansi.py,sha256=Top4EeEuaQdBWdteKMEcGOTeKeF19Q-Wo_6_Cj5kOzQ,2522
 err_hunter/third_party/colorama/ansitowin32.py,sha256=vPNYa3OZbxjbuFyaVo0Tmhmy1FZ1lKMWCnT7odXpItk,11128
 err_hunter/third_party/colorama/initialise.py,sha256=-hIny86ClXo39ixh5iSCfUIa2f_h_bgKRDW7gqs-KLU,3325
 err_hunter/third_party/colorama/win32.py,sha256=YQOKwMTwtGBbsY4dL5HYTvwTeP9wIQra5MvPNddpxZs,6181
 err_hunter/third_party/colorama/winterm.py,sha256=s0cT0jlXaJ-7t62xh1fzpGSmdJp6aXg-rKm8haOBjhI,7168
-err_hunter/third_party/logzero/__init__.py,sha256=mqg3AolyUjb_80kKSneEQpdTM6VAb1yF_sx4AnMrYf0,18461
+err_hunter/third_party/logzero/__init__.py,sha256=7mYpKx2l57Y4cZKzcgyrltQ1dm88Kcj2Fov0We2bHdw,18465
 err_hunter/third_party/logzero/colors.py,sha256=i4yHz9ZbZM8fCOo8znHOCtLlNlv7qIFUUlMIGr38VzI,2226
-err_hunter-0.8.1.dist-info/METADATA,sha256=lTf5uk12jZgCj0Xm-peaTVQyr0td9_nV_wCUFh2v7-8,529
-err_hunter-0.8.1.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-err_hunter-0.8.1.dist-info/top_level.txt,sha256=_-P2NbkqROCnUnbHohuBGvl1NQzgpaqRXn_g8vEzIWM,11
-err_hunter-0.8.1.dist-info/RECORD,,
+err_hunter-0.8.2.dist-info/METADATA,sha256=4GQlsi2tpA_yTy4WFQsePXladl2y1z38-gK9u2nkiHg,531
+err_hunter-0.8.2.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+err_hunter-0.8.2.dist-info/top_level.txt,sha256=_-P2NbkqROCnUnbHohuBGvl1NQzgpaqRXn_g8vEzIWM,11
+err_hunter-0.8.2.dist-info/RECORD,,
```

