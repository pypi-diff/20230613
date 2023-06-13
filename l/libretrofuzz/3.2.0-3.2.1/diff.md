# Comparing `tmp/libretrofuzz-3.2.0.tar.gz` & `tmp/libretrofuzz-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libretrofuzz-3.2.0.tar", max compression
+gzip compressed data, was "libretrofuzz-3.2.1.tar", max compression
```

## Comparing `libretrofuzz-3.2.0.tar` & `libretrofuzz-3.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1063 2023-06-13 02:12:10.975272 libretrofuzz-3.2.0/LICENSE
--rw-r--r--   0        0        0     7733 2023-06-13 02:12:10.975272 libretrofuzz-3.2.0/README.rst
--rw-r--r--   0        0        0       22 2023-06-13 02:12:10.975272 libretrofuzz-3.2.0/libretrofuzz/__init__.py
--rw-r--r--   0        0        0    55816 2023-06-13 02:12:10.975272 libretrofuzz-3.2.0/libretrofuzz/__main__.py
--rw-r--r--   0        0        0     1275 2023-06-13 02:12:10.975272 libretrofuzz-3.2.0/pyproject.toml
--rw-r--r--   0        0        0     8911 2023-06-13 02:12:21.071689 libretrofuzz-3.2.0/setup.py
--rw-r--r--   0        0        0     8921 2023-06-13 02:12:21.072764 libretrofuzz-3.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-13 16:18:57.774312 libretrofuzz-3.2.1/LICENSE
+-rw-r--r--   0        0        0     7471 2023-06-13 16:18:57.774312 libretrofuzz-3.2.1/README.rst
+-rw-r--r--   0        0        0       22 2023-06-13 16:18:57.774312 libretrofuzz-3.2.1/libretrofuzz/__init__.py
+-rw-r--r--   0        0        0    55734 2023-06-13 16:18:57.774312 libretrofuzz-3.2.1/libretrofuzz/__main__.py
+-rw-r--r--   0        0        0     1275 2023-06-13 16:18:57.774312 libretrofuzz-3.2.1/pyproject.toml
+-rw-r--r--   0        0        0     8651 2023-06-13 16:19:09.019950 libretrofuzz-3.2.1/setup.py
+-rw-r--r--   0        0        0     8659 2023-06-13 16:19:09.021023 libretrofuzz-3.2.1/PKG-INFO
```

### Comparing `libretrofuzz-3.2.0/LICENSE` & `libretrofuzz-3.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `libretrofuzz-3.2.0/README.rst` & `libretrofuzz-3.2.1/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 **Fuzzy Retroarch thumbnail downloader**
 ========================================
 
 In Retroarch, when you use the manual scanner to get nonstandard games or hacks in playlists, thumbnails often fail to download.
 
 These programs, for each game label on a playlist, download the most similar named image to display in retroarch.
 
-There are several options to fit unusual labels and increase fuzziness, but you can just run them to get the most restrictive default (require exact matches after the standard heuristics). If you still want more thumbnails, using ``libretro-fuzz --min 100 --delay 5 --delay 5`` works (lowering ``--min`` increases fuzz), with some delays introduced before and after downloading to check if you want to keep the game selected for the thumbnails.
+There are several options to fit unusual labels and increase fuzziness, but you can just run them to get a adequate default that is neither too strict or lax.
+
+If you still want more thumbnails, using ``libretro-fuzz --min 80 --delay 5 --delay 5`` works (smaller ``--min`` increases fuzz), with some delays introduced to check if you want to keep the game selected for the thumbnails. If you prefer only exact matches, use `--min 100`.
 
 If you use ``libretro-fuzz``, it will download for a single playlist by asking for the playlist and system if they're not provided.
 If you use ``libretro-fuzzall``, it will download for all playlists with standard libretro names, and will skip custom playlists.
 
 Besides those differences, if no retroarch.cfg is provided, both programs try to use the default retroarch.cfg.
 
 If `chafa <https://github.com/hpjansson/chafa>`_ is installed, the program will display new thumbnails of a game, with gray border for images already in use and with green border for new images. Chafa works better with a recent release and on a `sixel <https://en.wikipedia.org/wiki/Sixel>`_ or `kitty <https://sw.kovidgoyal.net/kitty/graphics-protocol/>`_ compatible shell.
@@ -25,17 +27,17 @@
 
 Example:
  ``libretro-fuzz --no-meta --no-merge``
 
  After downloading ``ScummVM`` thumbnails (and not before, to minimize false positives), we'd like to try to pickup a few covers from ``DOS`` thumbnails and skip download if there a risk of mixing thumbnails from ``DOS`` and ``ScummVM`` for a single game.
  Choose the ScummVM playlist and DOS system name, and covers would be downloaded with risk of false positives: CD vs floppy covers, USA vs Japan covers, or another platform vs DOS.
 
-Because of this increased risk of false positives with options, the default is to count everything except hack metadata as part of the match, only select the names that match exactly (after 'safe' heuristics like removing spaces) and the default pre-selected system name to be the same as the playlist name, which is safest.
+Because of this increased risk of false positives with options, the default is to count everything except hack metadata as part of the match and the default pre-selected system name to be the same as the playlist name, which is safest.
 
-False positives will then be from using ``--min`` (allows inexact matches) or/and one of the commands that do not count metadata (``--before`` and ``--no-meta``). A common scenario is the thumbnail server not having a single thumbnail of the game, and the program selecting the best match it can which is still good enough to pass, like a sequel, prequel, or different release, most often regions/languages. It's not recommended to use ``--min`` less than 100 without ``--filter`` to a specific game, or at least ``--delay/--delay-after`` to be able to cancel.
+A common scenario is the thumbnail server not having a single thumbnail of the game, and the program selecting the best match it can which is still good enough to pass, like a sequel, prequel, or different release, most often regions/languages. It's not recommended to use ``--min`` less than 90 without ``--filter`` to a specific game, or at least ``--delay/--delay-after`` to be able to cancel.
 
 Example:
   ``libretro-fuzz --system 'Commodore - Amiga' --before '_' --filter '[Ii]shar*'``
 
   The best way to solve these issues is to upload the right cover to the respective libretro-thumbnail subproject with the correct name of the game variant. Then you can redownload just the updated thumbnails with a label, in this example, because of ``--filter``, the Ishar series in the WHDLoad playlist would redownload.
 
 To debug why a game is not being matched, SHORT=1 before the command will display the simplified names checked for similarity.
@@ -54,16 +56,16 @@
   --system <NAME libretro-fuzz only>
                         Directory name in the server to download thumbnails. If not provided, asked from the user.
   --delay-after FLOAT   | Seconds after download to skip replacing thumbnails, enter continues. No-op with ``--no-image``.
                         | [1<=x<=60]
   --delay FLOAT         | Seconds to skip thumbnails download, enter continues.
                         | [1<=x<=60]
   --filter GLOB         Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, ``--filter '*'`` redownloads all.
-  --min SCORE           | 0=any, 100≃equal, 99=default. No-op with ``--no-fail``.
-                        | [default: 99; 0<=x<=100]
+  --min SCORE           | 0=any, 100≃equal, 90=default. No-op with ``--no-fail``.
+                        | [default: 90; 0<=x<=100]
   --no-fail             Download any score. Equivalent to ``--min 0``.
   --no-image            Don't show images even with chafa installed.
   --no-merge            Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with ``--filter``.
   --no-meta             Ignores () delimited metadata and may cause false positives. Forced with ``--before``.
   --hack                Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with ``--before``.
   --before TEXT         Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.
   --address URL         | URL with libretro-thumbnails server. For local files, git clone/unzip packs, run ``'python3 -m http.server'`` in parent dir, and use ``--address 'http://localhost:8000'``.
```

### Comparing `libretrofuzz-3.2.0/libretrofuzz/__main__.py` & `libretrofuzz-3.2.1/libretrofuzz/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -254,16 +254,14 @@
     for ch in input_str:
         if ch == open_p:
             paren_level += 1
         elif (ch == close_p) and paren_level:
             paren_level -= 1
         elif not paren_level:
             result += ch
-    if paren_level != 0:
-        error(f"'{input_str}' has a unclosed parenthesis")
     return result
 
 
 def extractbefore(name, before):
     if before:
         # Ignore metadata and get the string before it
         name_without_meta = regex.search(r"(^[^\[({]*)", name)
@@ -287,15 +285,15 @@
 def removeprefix(name: str, pre: str):
     if name.startswith(pre):
         return name[len(pre) :]
     return name
 
 
 def replaceRoman(source, romana, number):
-    source = regex.sub(rf"([\s']){romana}([\s,]|$)", rf"\g<1>{number}\g<2>", source)
+    source = regex.sub(rf"([\s']|^){romana}([\s,]|$)", rf"\g<1>{number}\g<2>", source)
     return source
 
 
 # Used to check the existence of a sixtel compatible terminal image viewer
 def which(executable):
     flips = shutil.which(executable)
     if not flips:
```

### Comparing `libretrofuzz-3.2.0/pyproject.toml` & `libretrofuzz-3.2.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "libretrofuzz"
-version = "3.2.0"
+version = "3.2.1"
 description = "Fuzzy Retroarch thumbnail downloader"
 authors = ["i30817 <i30817@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/i30817/libretrofuzz"
 
 [tool.poetry.dependencies]
```

### Comparing `libretrofuzz-3.2.0/setup.py` & `libretrofuzz-3.2.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 
 entry_points = \
 {'console_scripts': ['libretro-fuzz = libretrofuzz.__main__:fuzzsingle',
                      'libretro-fuzzall = libretrofuzz.__main__:fuzzall']}
 
 setup_kwargs = {
     'name': 'libretrofuzz',
-    'version': '3.2.0',
+    'version': '3.2.1',
     'description': 'Fuzzy Retroarch thumbnail downloader',
-    'long_description': "**Fuzzy Retroarch thumbnail downloader**\n========================================\n\nIn Retroarch, when you use the manual scanner to get nonstandard games or hacks in playlists, thumbnails often fail to download.\n\nThese programs, for each game label on a playlist, download the most similar named image to display in retroarch.\n\nThere are several options to fit unusual labels and increase fuzziness, but you can just run them to get the most restrictive default (require exact matches after the standard heuristics). If you still want more thumbnails, using ``libretro-fuzz --min 100 --delay 5 --delay 5`` works (lowering ``--min`` increases fuzz), with some delays introduced before and after downloading to check if you want to keep the game selected for the thumbnails.\n\nIf you use ``libretro-fuzz``, it will download for a single playlist by asking for the playlist and system if they're not provided.\nIf you use ``libretro-fuzzall``, it will download for all playlists with standard libretro names, and will skip custom playlists.\n\nBesides those differences, if no retroarch.cfg is provided, both programs try to use the default retroarch.cfg.\n\nIf `chafa <https://github.com/hpjansson/chafa>`_ is installed, the program will display new thumbnails of a game, with gray border for images already in use and with green border for new images. Chafa works better with a recent release and on a `sixel <https://en.wikipedia.org/wiki/Sixel>`_ or `kitty <https://sw.kovidgoyal.net/kitty/graphics-protocol/>`_ compatible shell.\n\nExample:\n | ``libretro-fuzz --system 'Commodore - Amiga' --no-merge --before '_'``\n\n The Retroplay WHDLoad set has labels like ``MonkeyIsland2_v1.3_0020`` after a manual scan. These labels *often* don't have subtitles (but not always) and all the metadata is not separated from the name by brackets. Select the playlist that contains those whdloads to download from the libretro amiga thumbnails.\n\nNote that the system name you download from doesn't have to be the same as the playlist name.\n\nIf the thumbnail server contains games from multiple releases for the system (like ``ScummVM``), be careful using extra options since it is easy to end up with 'slightly wrong' covers.\n\nExample:\n ``libretro-fuzz --no-meta --no-merge``\n\n After downloading ``ScummVM`` thumbnails (and not before, to minimize false positives), we'd like to try to pickup a few covers from ``DOS`` thumbnails and skip download if there a risk of mixing thumbnails from ``DOS`` and ``ScummVM`` for a single game.\n Choose the ScummVM playlist and DOS system name, and covers would be downloaded with risk of false positives: CD vs floppy covers, USA vs Japan covers, or another platform vs DOS.\n\nBecause of this increased risk of false positives with options, the default is to count everything except hack metadata as part of the match, only select the names that match exactly (after 'safe' heuristics like removing spaces) and the default pre-selected system name to be the same as the playlist name, which is safest.\n\nFalse positives will then be from using ``--min`` (allows inexact matches) or/and one of the commands that do not count metadata (``--before`` and ``--no-meta``). A common scenario is the thumbnail server not having a single thumbnail of the game, and the program selecting the best match it can which is still good enough to pass, like a sequel, prequel, or different release, most often regions/languages. It's not recommended to use ``--min`` less than 100 without ``--filter`` to a specific game, or at least ``--delay/--delay-after`` to be able to cancel.\n\nExample:\n  ``libretro-fuzz --system 'Commodore - Amiga' --before '_' --filter '[Ii]shar*'``\n\n  The best way to solve these issues is to upload the right cover to the respective libretro-thumbnail subproject with the correct name of the game variant. Then you can redownload just the updated thumbnails with a label, in this example, because of ``--filter``, the Ishar series in the WHDLoad playlist would redownload.\n\nTo debug why a game is not being matched, SHORT=1 before the command will display the simplified names checked for similarity.\n\nlibretro-fuzzall/libretro-fuzz [OPTIONS] [CFG]\n  :CFG:                 Path to the retroarch cfg file. If not default, asked from the user.\n\n                        Linux default:   ``~/.config/retroarch/retroarch.cfg``\n\n                        Windows default: ``%APPDATA%/RetroArch/retroarch.cfg``\n\n                        MacOS default:   ``~/Library/Application Support/RetroArch/config/retroarch.cfg``\n\n  --playlist <NAME libretro-fuzz only>\n                        Playlist name with labels used for thumbnail fuzzy matching. If not provided, asked from the user.\n  --system <NAME libretro-fuzz only>\n                        Directory name in the server to download thumbnails. If not provided, asked from the user.\n  --delay-after FLOAT   | Seconds after download to skip replacing thumbnails, enter continues. No-op with ``--no-image``.\n                        | [1<=x<=60]\n  --delay FLOAT         | Seconds to skip thumbnails download, enter continues.\n                        | [1<=x<=60]\n  --filter GLOB         Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, ``--filter '*'`` redownloads all.\n  --min SCORE           | 0=any, 100≃equal, 99=default. No-op with ``--no-fail``.\n                        | [default: 99; 0<=x<=100]\n  --no-fail             Download any score. Equivalent to ``--min 0``.\n  --no-image            Don't show images even with chafa installed.\n  --no-merge            Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with ``--filter``.\n  --no-meta             Ignores () delimited metadata and may cause false positives. Forced with ``--before``.\n  --hack                Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with ``--before``.\n  --before TEXT         Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.\n  --address URL         | URL with libretro-thumbnails server. For local files, git clone/unzip packs, run ``'python3 -m http.server'`` in parent dir, and use ``--address 'http://localhost:8000'``.\n                        | [default: https://thumbnails.libretro.com]\n  --dry-run             Print results only, no image download.\n  --verbose N           | Show length N list: score, name, emoji hyperlinks.\n                        | [x>=1]\n  --install-completion  Install completion for the current shell.\n  --show-completion     Show completion for the current shell, to copy it or customize the installation.\n  --help                Show this message and exit.\n\n\n\nTo install the program, type on the cmd line\n\n+----------------+---------------------------------------------------------------------------------------------+\n| Latest release | ``pip install --force-reinstall libretrofuzz``                                              |\n+----------------+---------------------------------------------------------------------------------------------+\n| Current code   | ``pip install --force-reinstall https://github.com/i30817/libretrofuzz/archive/master.zip`` |\n+----------------+---------------------------------------------------------------------------------------------+\n\nIn windows, you'll want to check the option to “Add Python to PATH” when installing python, to be able to install and execute the script from any path of the cmd line.\n",
+    'long_description': "**Fuzzy Retroarch thumbnail downloader**\n========================================\n\nIn Retroarch, when you use the manual scanner to get nonstandard games or hacks in playlists, thumbnails often fail to download.\n\nThese programs, for each game label on a playlist, download the most similar named image to display in retroarch.\n\nThere are several options to fit unusual labels and increase fuzziness, but you can just run them to get a adequate default that is neither too strict or lax.\n\nIf you still want more thumbnails, using ``libretro-fuzz --min 80 --delay 5 --delay 5`` works (smaller ``--min`` increases fuzz), with some delays introduced to check if you want to keep the game selected for the thumbnails. If you prefer only exact matches, use `--min 100`.\n\nIf you use ``libretro-fuzz``, it will download for a single playlist by asking for the playlist and system if they're not provided.\nIf you use ``libretro-fuzzall``, it will download for all playlists with standard libretro names, and will skip custom playlists.\n\nBesides those differences, if no retroarch.cfg is provided, both programs try to use the default retroarch.cfg.\n\nIf `chafa <https://github.com/hpjansson/chafa>`_ is installed, the program will display new thumbnails of a game, with gray border for images already in use and with green border for new images. Chafa works better with a recent release and on a `sixel <https://en.wikipedia.org/wiki/Sixel>`_ or `kitty <https://sw.kovidgoyal.net/kitty/graphics-protocol/>`_ compatible shell.\n\nExample:\n | ``libretro-fuzz --system 'Commodore - Amiga' --no-merge --before '_'``\n\n The Retroplay WHDLoad set has labels like ``MonkeyIsland2_v1.3_0020`` after a manual scan. These labels *often* don't have subtitles (but not always) and all the metadata is not separated from the name by brackets. Select the playlist that contains those whdloads to download from the libretro amiga thumbnails.\n\nNote that the system name you download from doesn't have to be the same as the playlist name.\n\nIf the thumbnail server contains games from multiple releases for the system (like ``ScummVM``), be careful using extra options since it is easy to end up with 'slightly wrong' covers.\n\nExample:\n ``libretro-fuzz --no-meta --no-merge``\n\n After downloading ``ScummVM`` thumbnails (and not before, to minimize false positives), we'd like to try to pickup a few covers from ``DOS`` thumbnails and skip download if there a risk of mixing thumbnails from ``DOS`` and ``ScummVM`` for a single game.\n Choose the ScummVM playlist and DOS system name, and covers would be downloaded with risk of false positives: CD vs floppy covers, USA vs Japan covers, or another platform vs DOS.\n\nBecause of this increased risk of false positives with options, the default is to count everything except hack metadata as part of the match and the default pre-selected system name to be the same as the playlist name, which is safest.\n\nA common scenario is the thumbnail server not having a single thumbnail of the game, and the program selecting the best match it can which is still good enough to pass, like a sequel, prequel, or different release, most often regions/languages. It's not recommended to use ``--min`` less than 90 without ``--filter`` to a specific game, or at least ``--delay/--delay-after`` to be able to cancel.\n\nExample:\n  ``libretro-fuzz --system 'Commodore - Amiga' --before '_' --filter '[Ii]shar*'``\n\n  The best way to solve these issues is to upload the right cover to the respective libretro-thumbnail subproject with the correct name of the game variant. Then you can redownload just the updated thumbnails with a label, in this example, because of ``--filter``, the Ishar series in the WHDLoad playlist would redownload.\n\nTo debug why a game is not being matched, SHORT=1 before the command will display the simplified names checked for similarity.\n\nlibretro-fuzzall/libretro-fuzz [OPTIONS] [CFG]\n  :CFG:                 Path to the retroarch cfg file. If not default, asked from the user.\n\n                        Linux default:   ``~/.config/retroarch/retroarch.cfg``\n\n                        Windows default: ``%APPDATA%/RetroArch/retroarch.cfg``\n\n                        MacOS default:   ``~/Library/Application Support/RetroArch/config/retroarch.cfg``\n\n  --playlist <NAME libretro-fuzz only>\n                        Playlist name with labels used for thumbnail fuzzy matching. If not provided, asked from the user.\n  --system <NAME libretro-fuzz only>\n                        Directory name in the server to download thumbnails. If not provided, asked from the user.\n  --delay-after FLOAT   | Seconds after download to skip replacing thumbnails, enter continues. No-op with ``--no-image``.\n                        | [1<=x<=60]\n  --delay FLOAT         | Seconds to skip thumbnails download, enter continues.\n                        | [1<=x<=60]\n  --filter GLOB         Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, ``--filter '*'`` redownloads all.\n  --min SCORE           | 0=any, 100≃equal, 90=default. No-op with ``--no-fail``.\n                        | [default: 90; 0<=x<=100]\n  --no-fail             Download any score. Equivalent to ``--min 0``.\n  --no-image            Don't show images even with chafa installed.\n  --no-merge            Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with ``--filter``.\n  --no-meta             Ignores () delimited metadata and may cause false positives. Forced with ``--before``.\n  --hack                Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with ``--before``.\n  --before TEXT         Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.\n  --address URL         | URL with libretro-thumbnails server. For local files, git clone/unzip packs, run ``'python3 -m http.server'`` in parent dir, and use ``--address 'http://localhost:8000'``.\n                        | [default: https://thumbnails.libretro.com]\n  --dry-run             Print results only, no image download.\n  --verbose N           | Show length N list: score, name, emoji hyperlinks.\n                        | [x>=1]\n  --install-completion  Install completion for the current shell.\n  --show-completion     Show completion for the current shell, to copy it or customize the installation.\n  --help                Show this message and exit.\n\n\n\nTo install the program, type on the cmd line\n\n+----------------+---------------------------------------------------------------------------------------------+\n| Latest release | ``pip install --force-reinstall libretrofuzz``                                              |\n+----------------+---------------------------------------------------------------------------------------------+\n| Current code   | ``pip install --force-reinstall https://github.com/i30817/libretrofuzz/archive/master.zip`` |\n+----------------+---------------------------------------------------------------------------------------------+\n\nIn windows, you'll want to check the option to “Add Python to PATH” when installing python, to be able to install and execute the script from any path of the cmd line.\n",
     'author': 'i30817',
     'author_email': 'i30817@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/i30817/libretrofuzz',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `libretrofuzz-3.2.0/PKG-INFO` & `libretrofuzz-3.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libretrofuzz
-Version: 3.2.0
+Version: 3.2.1
 Summary: Fuzzy Retroarch thumbnail downloader
 Home-page: https://github.com/i30817/libretrofuzz
 License: MIT
 Author: i30817
 Author-email: i30817@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -30,15 +30,17 @@
 **Fuzzy Retroarch thumbnail downloader**
 ========================================
 
 In Retroarch, when you use the manual scanner to get nonstandard games or hacks in playlists, thumbnails often fail to download.
 
 These programs, for each game label on a playlist, download the most similar named image to display in retroarch.
 
-There are several options to fit unusual labels and increase fuzziness, but you can just run them to get the most restrictive default (require exact matches after the standard heuristics). If you still want more thumbnails, using ``libretro-fuzz --min 100 --delay 5 --delay 5`` works (lowering ``--min`` increases fuzz), with some delays introduced before and after downloading to check if you want to keep the game selected for the thumbnails.
+There are several options to fit unusual labels and increase fuzziness, but you can just run them to get a adequate default that is neither too strict or lax.
+
+If you still want more thumbnails, using ``libretro-fuzz --min 80 --delay 5 --delay 5`` works (smaller ``--min`` increases fuzz), with some delays introduced to check if you want to keep the game selected for the thumbnails. If you prefer only exact matches, use `--min 100`.
 
 If you use ``libretro-fuzz``, it will download for a single playlist by asking for the playlist and system if they're not provided.
 If you use ``libretro-fuzzall``, it will download for all playlists with standard libretro names, and will skip custom playlists.
 
 Besides those differences, if no retroarch.cfg is provided, both programs try to use the default retroarch.cfg.
 
 If `chafa <https://github.com/hpjansson/chafa>`_ is installed, the program will display new thumbnails of a game, with gray border for images already in use and with green border for new images. Chafa works better with a recent release and on a `sixel <https://en.wikipedia.org/wiki/Sixel>`_ or `kitty <https://sw.kovidgoyal.net/kitty/graphics-protocol/>`_ compatible shell.
@@ -54,17 +56,17 @@
 
 Example:
  ``libretro-fuzz --no-meta --no-merge``
 
  After downloading ``ScummVM`` thumbnails (and not before, to minimize false positives), we'd like to try to pickup a few covers from ``DOS`` thumbnails and skip download if there a risk of mixing thumbnails from ``DOS`` and ``ScummVM`` for a single game.
  Choose the ScummVM playlist and DOS system name, and covers would be downloaded with risk of false positives: CD vs floppy covers, USA vs Japan covers, or another platform vs DOS.
 
-Because of this increased risk of false positives with options, the default is to count everything except hack metadata as part of the match, only select the names that match exactly (after 'safe' heuristics like removing spaces) and the default pre-selected system name to be the same as the playlist name, which is safest.
+Because of this increased risk of false positives with options, the default is to count everything except hack metadata as part of the match and the default pre-selected system name to be the same as the playlist name, which is safest.
 
-False positives will then be from using ``--min`` (allows inexact matches) or/and one of the commands that do not count metadata (``--before`` and ``--no-meta``). A common scenario is the thumbnail server not having a single thumbnail of the game, and the program selecting the best match it can which is still good enough to pass, like a sequel, prequel, or different release, most often regions/languages. It's not recommended to use ``--min`` less than 100 without ``--filter`` to a specific game, or at least ``--delay/--delay-after`` to be able to cancel.
+A common scenario is the thumbnail server not having a single thumbnail of the game, and the program selecting the best match it can which is still good enough to pass, like a sequel, prequel, or different release, most often regions/languages. It's not recommended to use ``--min`` less than 90 without ``--filter`` to a specific game, or at least ``--delay/--delay-after`` to be able to cancel.
 
 Example:
   ``libretro-fuzz --system 'Commodore - Amiga' --before '_' --filter '[Ii]shar*'``
 
   The best way to solve these issues is to upload the right cover to the respective libretro-thumbnail subproject with the correct name of the game variant. Then you can redownload just the updated thumbnails with a label, in this example, because of ``--filter``, the Ishar series in the WHDLoad playlist would redownload.
 
 To debug why a game is not being matched, SHORT=1 before the command will display the simplified names checked for similarity.
@@ -83,16 +85,16 @@
   --system <NAME libretro-fuzz only>
                         Directory name in the server to download thumbnails. If not provided, asked from the user.
   --delay-after FLOAT   | Seconds after download to skip replacing thumbnails, enter continues. No-op with ``--no-image``.
                         | [1<=x<=60]
   --delay FLOAT         | Seconds to skip thumbnails download, enter continues.
                         | [1<=x<=60]
   --filter GLOB         Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, ``--filter '*'`` redownloads all.
-  --min SCORE           | 0=any, 100≃equal, 99=default. No-op with ``--no-fail``.
-                        | [default: 99; 0<=x<=100]
+  --min SCORE           | 0=any, 100≃equal, 90=default. No-op with ``--no-fail``.
+                        | [default: 90; 0<=x<=100]
   --no-fail             Download any score. Equivalent to ``--min 0``.
   --no-image            Don't show images even with chafa installed.
   --no-merge            Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with ``--filter``.
   --no-meta             Ignores () delimited metadata and may cause false positives. Forced with ``--before``.
   --hack                Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with ``--before``.
   --before TEXT         Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.
   --address URL         | URL with libretro-thumbnails server. For local files, git clone/unzip packs, run ``'python3 -m http.server'`` in parent dir, and use ``--address 'http://localhost:8000'``.
```

