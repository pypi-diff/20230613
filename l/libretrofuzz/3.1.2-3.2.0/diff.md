# Comparing `tmp/libretrofuzz-3.1.2.tar.gz` & `tmp/libretrofuzz-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libretrofuzz-3.1.2.tar", max compression
+gzip compressed data, was "libretrofuzz-3.2.0.tar", max compression
```

## Comparing `libretrofuzz-3.1.2.tar` & `libretrofuzz-3.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1063 2023-06-11 22:20:04.187282 libretrofuzz-3.1.2/LICENSE
--rw-r--r--   0        0        0     7681 2023-06-11 22:20:04.187282 libretrofuzz-3.1.2/README.rst
--rw-r--r--   0        0        0       22 2023-06-11 22:20:04.187282 libretrofuzz-3.1.2/libretrofuzz/__init__.py
--rw-r--r--   0        0        0    53876 2023-06-11 22:20:04.187282 libretrofuzz-3.1.2/libretrofuzz/__main__.py
--rw-r--r--   0        0        0     1275 2023-06-11 22:20:04.191282 libretrofuzz-3.1.2/pyproject.toml
--rw-r--r--   0        0        0     8858 2023-06-11 22:20:14.565938 libretrofuzz-3.1.2/setup.py
--rw-r--r--   0        0        0     8869 2023-06-11 22:20:14.567036 libretrofuzz-3.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-13 02:12:10.975272 libretrofuzz-3.2.0/LICENSE
+-rw-r--r--   0        0        0     7733 2023-06-13 02:12:10.975272 libretrofuzz-3.2.0/README.rst
+-rw-r--r--   0        0        0       22 2023-06-13 02:12:10.975272 libretrofuzz-3.2.0/libretrofuzz/__init__.py
+-rw-r--r--   0        0        0    55816 2023-06-13 02:12:10.975272 libretrofuzz-3.2.0/libretrofuzz/__main__.py
+-rw-r--r--   0        0        0     1275 2023-06-13 02:12:10.975272 libretrofuzz-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0     8911 2023-06-13 02:12:21.071689 libretrofuzz-3.2.0/setup.py
+-rw-r--r--   0        0        0     8921 2023-06-13 02:12:21.072764 libretrofuzz-3.2.0/PKG-INFO
```

### Comparing `libretrofuzz-3.1.2/LICENSE` & `libretrofuzz-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `libretrofuzz-3.1.2/README.rst` & `libretrofuzz-3.2.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -54,24 +54,25 @@
   --system <NAME libretro-fuzz only>
                         Directory name in the server to download thumbnails. If not provided, asked from the user.
   --delay-after FLOAT   | Seconds after download to skip replacing thumbnails, enter continues. No-op with ``--no-image``.
                         | [1<=x<=60]
   --delay FLOAT         | Seconds to skip thumbnails download, enter continues.
                         | [1<=x<=60]
   --filter GLOB         Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, ``--filter '*'`` redownloads all.
-  --min SCORE           | 0=any, 100=fuzzy match,default 200=equal. No-op with ``--no-fail``.
-                        | [default: 100; 0<=x<=200]
+  --min SCORE           | 0=any, 100≃equal, 99=default. No-op with ``--no-fail``.
+                        | [default: 99; 0<=x<=100]
   --no-fail             Download any score. Equivalent to ``--min 0``.
   --no-image            Don't show images even with chafa installed.
   --no-merge            Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with ``--filter``.
   --no-meta             Ignores () delimited metadata and may cause false positives. Forced with ``--before``.
   --hack                Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with ``--before``.
   --before TEXT         Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.
   --address URL         | URL with libretro-thumbnails server. For local files, git clone/unzip packs, run ``'python3 -m http.server'`` in parent dir, and use ``--address 'http://localhost:8000'``.
                         | [default: https://thumbnails.libretro.com]
+  --dry-run             Print results only, no image download.
   --verbose N           | Show length N list: score, name, emoji hyperlinks.
                         | [x>=1]
   --install-completion  Install completion for the current shell.
   --show-completion     Show completion for the current shell, to copy it or customize the installation.
   --help                Show this message and exit.
```

### Comparing `libretrofuzz-3.1.2/libretrofuzz/__main__.py` & `libretrofuzz-3.2.0/libretrofuzz/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 import shutil
 import unicodedata
 import asyncio
 import subprocess
 import configparser
 import platform
 
+
 # external libraries
 from PIL import Image, ImageOps
 from rapidfuzz import process, fuzz
 from bs4 import BeautifulSoup
 from questionary import Style, select
 from httpx import RequestError, HTTPStatusError, Client, AsyncClient
 from tqdm import trange, tqdm
@@ -59,16 +60,16 @@
 
 
 ###########################################
 ########### SCRIPT SETTINGS ###############
 ###########################################
 
 ADDRESS = "https://thumbnails.libretro.com"
-DEF_SCORE = 100
-MAX_SCORE = 200
+DEF_SCORE = 90
+MAX_SCORE = 100
 MAX_RETRIES = 3
 MAX_WAIT_SECS = 60
 # 00-1f are ascii control codes, rest are illegal windows filename chars according to powershell + &
 forbidden = regex.compile(
     r"[\u0022\u003c\u003e\u007c\u0000\u0001\u0002\u0003\u0004\u0005\u0006\u0007\u0008"
     + r"\u0009\u000a\u000b\u000c\u000d\u000e\u000f\u0010\u0011\u0012\u0013\u0014\u0015"
     + r"\u0016\u0017\u0018\u0019\u001a\u001b\u001c\u001d\u001e\u001f\u003a\u002a\u003f\u005c\u002f\u0026]"
@@ -235,14 +236,22 @@
     if label is None:
         label = uri
     # OSC 8 ; params ; URI ST <name> OSC 8 ;; ST
     escape_mask = "\033]8;{};{}\033\\{}\033]8;;\033\\"
     return escape_mask.format(parameters, uri, label)
 
 
+def extdigits(input_str):
+    result = ""
+    for ch in input_str:
+        if ch.isdigit():
+            result += ch
+    return result
+
+
 def removeparenthesis(input_str, open_p="(", close_p=")"):
     result = ""
     paren_level = 0
     for ch in input_str:
         if ch == open_p:
             paren_level += 1
         elif (ch == close_p) and paren_level:
@@ -277,14 +286,19 @@
 
 def removeprefix(name: str, pre: str):
     if name.startswith(pre):
         return name[len(pre) :]
     return name
 
 
+def replaceRoman(source, romana, number):
+    source = regex.sub(rf"([\s']){romana}([\s,]|$)", rf"\g<1>{number}\g<2>", source)
+    return source
+
+
 # Used to check the existence of a sixtel compatible terminal image viewer
 def which(executable):
     flips = shutil.which(executable)
     if not flips:
         flips = shutil.which(executable, path=os.path.dirname(__file__))
     if not flips:
         flips = shutil.which(executable, path=os.getcwd())
@@ -292,50 +306,57 @@
 
 
 # -------------------------------------------------------------------
 # The heart of the program, what orders titles to be 'more similar'
 # or less to the local labels (after the normalization)
 # -------------------------------------------------------------------
 class TitleScorer(object):
-    def __init__(self, normcache, normcache2):
-        # rapidfuzz says to use range 0-100, but this doesn't (it's much easier that way)
-        # so it uses internal api to prevent a possible early exit at == 100
-        self._RF_ScorerPy = {
-            "get_scorer_flags": lambda **kwargs: {
-                "optimal_score": MAX_SCORE,
-                "worst_score": 0,
-                "flags": (1 << 6),
-            }
-        }
+    def __init__(self, normcache, normcache2, hack):
         self.normcache = normcache
         self.normcache2 = normcache2
+        self.hack = hack
 
     def __call__(self, name, other, processor=None, score_cutoff=None):
         if name == other:
-            return 200
-        (_, name_ns, _, _) = self.normcache[name]
-        (_, other_ns, other_subs, other_ns_subs) = self.normcache2[other]
+            return MAX_SCORE
+        (_, name_ns, _, _, digits) = self.normcache[name]
+        (_, other_ns, other_subs, other_ns_subs, other_digits) = self.normcache2[other]
         if name_ns == other_ns:
-            return 200
-        # If a playlist has 'other name' that means 'other name' is
-        # a perfect match to another game on the playlist.
-        # That probably means it's not the right game.
-        if other in self.normcache or other_ns in self.normcache:
-            perfect_for_another = 0.1
-        else:
-            perfect_for_another = 0
-        candidates = []
-        for sub, sub2 in zip(other_subs, other_ns_subs):
-            if name == sub or name_ns == sub2:
-                candidates.append(200 - perfect_for_another)
-                break
-            else:
-                candidates.append(fuzz.token_ratio(name, sub) - perfect_for_another)
-        candidates.append(fuzz.token_ratio(name, other) - perfect_for_another)
-        return max(candidates)
+            return MAX_SCORE
+
+        remaining = MAX_SCORE - DEF_SCORE
+
+        cnbrs = fuzz.ratio(digits, other_digits)  # normalized to 0-100
+        # 2 heuristics (this time), however they don't both have the same weight
+        increment_common_number = remaining * 0.03
+        increment_common_length = remaining * 0.97
+
+        rest_of_score = increment_common_number * 0.01 * cnbrs  # 100 gives 1
+        common_prop = len(os.path.commonprefix([name_ns, other_ns])) / len(name_ns)
+        rest_of_score += increment_common_length * common_prop
+        sum_ns = ""
+        for sub, sub_ns in zip(other_subs, other_ns_subs):
+            # if you find a exact match on either a subtitle
+            # or a sequence of subtitles from the start, give
+            # a 'winning' score but distingish them by the rest
+            # by name ratio and digits ratio
+            if name_ns == (sum_ns := sum_ns + sub_ns) or name_ns == sub_ns:
+                # reset increment and rest of score
+                rest_of_score = increment_common_number * 0.01 * cnbrs
+                rest_of_score += increment_common_length * 0.01 * fuzz.WRatio(name, other)
+                return DEF_SCORE + rest_of_score
+
+        # give a penality if you got here and the name you're checking against
+        # already has a perfect match in the playlist being processed. This usually
+        # penalizes hack names but removes a lot of inane false positives
+        # (depending on the playlist completeness). Disable it when processing hacks
+        # TODO remove this when a feature to choose when waiting happens
+        if not self.hack and other_ns in self.normcache:
+            rest_of_score -= remaining * 0.65
+        return fuzz.WRatio(name, other) * (DEF_SCORE / 100) + rest_of_score
 
 
 # ---------------------------------------------------------------
 # Normalization functions, part of the functions that change both
 # local labels and remote names to be more similar to compare
 # ---------------------------------------------------------------
 # word splitter regex, wont even attempt to explain how and why
@@ -349,19 +370,20 @@
 
 
 def normalizer(nometa, hack, t):
     if nometa:
         t = removeparenthesis(t, "(", ")")
     if not hack:
         t = removeparenthesis(t, "[", "]")
+
     # replace the default character representing illegal chars
     # in the libretro database by space
     t = t.replace("_", " ")
     # remove any number of leading 0s that ends in a digit
-    t = regex.sub(zero_lead_pattern, r"\1\2", t)
+    t = regex.sub(zero_lead_pattern, r"\g<1>\g<2>", t)
     # split subtitles. ': ' is forbidden in server names
     # but may occur in the local name. Do this before camelcase
     # split because its hard to do a regex that allows splitting
     # Word-Word or Word:Word without creating new subtitle
     # and removing articles from subtitles is helpful anyway
     subtitles = t.split(" - ")
     if len(subtitles) == 1:
@@ -371,14 +393,38 @@
         # remove all symbols, except, ',' and '''
         # this needs to be here for all the names
         # to be operating on the same base for definite articles
         st = regex.sub(almost_symbols_pattern, "", st)
         # CamelCaseNames for local labels are common when there are no spaces
         # do this to normalize for definite articles
         st = " ".join([a for s in regex.split(camelcase_pattern, st) if s and (a := s.strip())])
+        # Tries to make roman numerals in the range 1-20 equivalent to normal numbers.
+        # If both str tested have roman numerals little harm done if XXIV gets turned into 204.
+        st = replaceRoman(st, "XVIII", "18")
+        st = replaceRoman(st, "XVII", "17")
+        st = replaceRoman(st, "XVI", "16")
+        st = replaceRoman(st, "XIII", "13")
+        st = replaceRoman(st, "XII", "12")
+        st = replaceRoman(st, "XIV", "14")
+        st = replaceRoman(st, "XV", "15")
+        st = replaceRoman(st, "XIX", "19")
+        st = replaceRoman(st, "XX", "20")
+        st = replaceRoman(st, "XI", "11")
+        st = replaceRoman(st, "VIII", "8")
+        st = replaceRoman(st, "VII", "7")
+        st = replaceRoman(st, "VI", "6")
+        st = replaceRoman(st, "III", "3")
+        st = replaceRoman(st, "II", "2")
+        st = replaceRoman(st, "IV", "4")
+        st = replaceRoman(st, "V", "5")
+        st = replaceRoman(st, "IX", "9")
+        st = replaceRoman(st, "X", "10")
+        st = replaceRoman(st, "I", "1")
+        # such a common variant i zoom in on it
+        st = st.replace("Center", "Centre")
         # normalize case
         st = st.lower()
         # beginning and end definite articles in several european languages (people move them)
         # make sure we're only removing the start and end forms with spaces
         st = removefirst(st, ", the")
         st = removeprefix(st, "the ")
         st = removefirst(st, ", los")
@@ -412,42 +458,22 @@
         st = removeprefix(st, "a ")
         # finally get rid of the rest
         st = replacemany(st, ",'", "")
         # if a remote name has ' and ' instead of ' _ ' to replace ' & ' make it work
         st = st.replace(" and ", " ")
         # and why not
         st = st.replace(" the ", " ")
-        # Tries to make roman numerals in the range 1-20 equivalent to normal numbers.
-        # If both str tested have roman numerals no harm done if XXIV gets turned into 204.
-        st = st.replace("xviii", "18")
-        st = st.replace("xvii", "17")
-        st = st.replace("xvi", "16")
-        st = st.replace("xiii", "13")
-        st = st.replace("xii", "12")
-        st = st.replace("xiv", "14")
-        st = st.replace("xv", "15")
-        st = st.replace("xix", "19")
-        st = st.replace("xx", "20")
-        st = st.replace("xi", "11")
-        st = st.replace("viii", "8")
-        st = st.replace("vii", "7")
-        st = st.replace("vi", "6")
-        st = st.replace("iii", "3")
-        st = st.replace("ii", "2")
-        st = st.replace("iv", "4")
-        st = st.replace("v", "5")
-        st = st.replace("ix", "9")
-        st = st.replace("x", "10")
-        st = st.replace("i", "1")
         # remove diacritics (not to asian languages diacritics, only for 2 to 1 character combinations)
         st = "".join([c for c in unicodedata.normalize("NFKD", st) if not unicodedata.combining(c)])
         st = st.strip().split()
         subtitles[i] = " ".join(st)
         subtitles2[i] = "".join(st)
-    return " ".join(subtitles), "".join(subtitles2), subtitles, subtitles2
+    nspaces = "".join(subtitles2)
+    ext_digits = extdigits(nspaces)
+    return " ".join(subtitles), nspaces, subtitles, subtitles2, ext_digits
 
 
 # ---------------------------------------------------------------------------------
 # Initalization functions, since there are two main programs so the code is reused
 # ---------------------------------------------------------------------------------
 class RzipReader(object):
     """used to abstract the libretro compressed playlist format"""
@@ -660,15 +686,15 @@
     ),
     score: int = Option(
         DEF_SCORE,
         "--min",
         min=0,
         max=MAX_SCORE,
         metavar="SCORE",
-        help=f"0=any, {DEF_SCORE}=fuzzy match,default, {MAX_SCORE}=equal. No-op with --no-fail.",
+        help=f"0=any, {MAX_SCORE}≃equal, {DEF_SCORE}=default. No-op with --no-fail.",
     ),
     nofail: bool = Option(False, "--no-fail", help="Download any score. Equivalent to --score 0."),
     noimage: bool = Option(False, "--no-image", help="Don't show images even with chafa installed."),
     nomerge: bool = Option(
         False,
         "--no-merge",
         help="Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with --filter.",
@@ -688,26 +714,25 @@
         help="Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.",
     ),
     address: Optional[str] = Option(
         ADDRESS,
         metavar="URL",
         help="URL with libretro-thumbnails server. For local files, git clone/unzip packs, run 'python3 -m http.server' in parent dir, and use --address 'http://localhost:8000'.",
     ),
+    dryrun: bool = Option(False, "--dry-run", help="Print results only, no image download."),
     verbose: Optional[int] = Option(
         None, "--verbose", min=1, metavar="N", help="Show length N list: score, name, emoji hyperlinks."
     ),
 ):
     if playlist and not playlist.lower().endswith(".lpl"):
         playlist = playlist + ".lpl"
 
     (nub_verbose, playlist_dir, thumbnails_dir, playlists, systems) = common_errors(
         cfg, playlist, system, address
     )
-    if nub_verbose:
-        noimage = True
 
     custom_style = Style([("answer", "fg:green bold")])
 
     # ask user for these 2 arguments if they're still not set
     if not playlist:
         display_playlists = list(map(os.path.basename, playlists))
         playlist = select(
@@ -746,14 +771,15 @@
                     )
                     await downloader(
                         names,
                         system,
                         wait_before,
                         wait_after,
                         filters,
+                        dryrun,
                         score,
                         noimage,
                         nomerge,
                         nofail,
                         nometa,
                         hack,
                         verbose,
@@ -801,15 +827,15 @@
     ),
     score: int = Option(
         DEF_SCORE,
         "--min",
         min=0,
         max=MAX_SCORE,
         metavar="SCORE",
-        help=f"0=any, {DEF_SCORE}=fuzzy match,default, {MAX_SCORE}=equal. No-op with --no-fail.",
+        help=f"0=any, {MAX_SCORE}≃equal, {DEF_SCORE}=default. No-op with --no-fail.",
     ),
     nofail: bool = Option(False, "--no-fail", help="Download any score. Equivalent to --score 0."),
     noimage: bool = Option(False, "--no-image", help="Don't show images even with chafa installed."),
     nomerge: bool = Option(
         False,
         "--no-merge",
         help="Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with --filter.",
@@ -829,21 +855,20 @@
         help="Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.",
     ),
     address: Optional[str] = Option(
         ADDRESS,
         metavar="URL",
         help="URL with libretro-thumbnails server. For local files, git clone/unzip packs, run 'python3 -m http.server' in parent dir, and use --address 'http://localhost:8000'.",
     ),
+    dryrun: bool = Option(False, "--dry-run", help="Print results only, no image download."),
     verbose: Optional[int] = Option(
         None, "--verbose", min=1, metavar="N", help="Show length N list: score, name, emoji hyperlinks."
     ),
 ):
     (nub_verbose, _, thumbnails_dir, playlists, systems) = common_errors(cfg, None, None, address)
-    if nub_verbose:
-        noimage = True
 
     notInSystems = [
         (playlist, os.path.basename(playlist)[:-4])
         for playlist in playlists
         if os.path.basename(playlist)[:-4] not in systems
     ]
     for playlist, system in notInSystems:
@@ -865,14 +890,15 @@
                         try:
                             await downloader(
                                 names,
                                 system,
                                 wait_before,
                                 wait_after,
                                 filters,
+                                dryrun,
                                 score,
                                 noimage,
                                 nomerge,
                                 nofail,
                                 nometa,
                                 hack,
                                 verbose,
@@ -929,14 +955,15 @@
 
 async def downloader(
     names: [(str, str)],
     system: str,
     wait_before: Optional[float],
     wait_after: Optional[float],
     filters: Optional[List[str]],
+    dryrun: bool,
     score: int,
     noimage: bool,
     nomerge: bool,
     nofail: bool,
     nometa: bool,
     hack: bool,
     verbose: Optional[int],
@@ -953,14 +980,19 @@
     # so the hack and meta matching must be disabled
     if before:
         hack = False
         nometa = True
     # no-fail is equivalent to max fuzz
     if nofail:
         score = 0
+    # besides the explicit setting these two need to disable images,
+    # one because the console is not ready to print images (or emoji)
+    # the other to prevent unpleasant empty space.
+    if nub_verbose or dryrun:
+        noimage = True
 
     # build the function that will be called to print data,
     # filling in some fixed arguments
     short_names = os.getenv("SHORT")
     short_names = True if short_names and short_names != "0" else False
     strfy_runtime = partial(strfy, score, short_names, nub_verbose)
     norm = partial(normalizer, nometa, hack)
@@ -996,15 +1028,15 @@
     tmpdict = dict()
     normcache2 = dict()
     for x in remote_names:
         normtuple = norm(x)
         normcache2[normtuple[0]] = normtuple  # normalized only
         tmpdict[x] = normtuple[0]
     remote_names = tmpdict
-    scorer = TitleScorer(normcache, normcache2)
+    scorer = TitleScorer(normcache, normcache2, hack)
     for name, destination in names:
         await asyncio.sleep(0)  # update key status
         checkEscape()  # check key status
         # if the user used filters, filter everything that doesn't match any of the globs
         if filters and not any(map(lambda x: fnmatch.fnmatch(name, x), filters)):
             continue
         # cached normalized name
@@ -1081,14 +1113,15 @@
                                     url,
                                     temp,
                                     getting_format,
                                     waiting_format,
                                     first_wait,
                                     wait_before,
                                     MAX_RETRIES,
+                                    dryrun,
                                 ):
                                     first_wait = False
                                     downloaded_once = True
                                     urls[(dirname, winner)] = url
                                     break
                     # Delete old images in the case of --filter.
                     # internet not available will exit the program
@@ -1162,15 +1195,15 @@
     linked1 = style(link(url1, "🎴")) if url1 else ""
     linked2 = style(link(url2, "🎬")) if url2 else ""
     linked3 = style(link(url3, "📸")) if url3 else ""
     return f"{score_text} {thumb_text}{linked1}{linked2}{linked3}"
 
 
 async def download(
-    client, url, destination, getting_format, waiting_format, first_wait, wait_before, max_retries
+    client, url, destination, getting_format, waiting_format, first_wait, wait_before, max_retries, dryrun
 ):
     """returns True if downloaded. To download, it must have waited, if first_wait is True.
     Exceptions may happen instead of returning False, but they are all caught outside
     the caller loop of thumbnail types that downloads, so the first_wait guard gets
     reset again and only waits once per game
     """
     while True:
@@ -1180,24 +1213,30 @@
                     raise StopPlaylist()
                 if r.status_code == 404:  # broken image or symlink link, skip just this thumb
                     return False
                 r.raise_for_status()  # error before reading the header goes into retrying
                 length = int(r.headers["Content-Length"])
                 if length < 100:  # obviously corrupt 'thumbnail', skip this thumb
                     return False
-                with open(destination, "w+b") as f:
-                    if first_wait:
-                        await printwait(wait_before, waiting_format)
-                    with tqdm.wrapattr(
-                        f, "write", total=length, dynamic_ncols=True, bar_format=getting_format, leave=False
-                    ) as w:
-                        async for chunk in r.aiter_raw(4096):
-                            with handleContinueDownload():
-                                checkDownload()
-                            w.write(chunk)
+                if not dryrun:  # test
+                    with open(destination, "w+b") as f:
+                        if first_wait:
+                            await printwait(wait_before, waiting_format)
+                        with tqdm.wrapattr(
+                            f,
+                            "write",
+                            total=length,
+                            dynamic_ncols=True,
+                            bar_format=getting_format,
+                            leave=False,
+                        ) as w:
+                            async for chunk in r.aiter_raw(4096):
+                                with handleContinueDownload():
+                                    checkDownload()
+                                w.write(chunk)
             return True
         except (RequestError, HTTPStatusError):
             if max_retries <= 0:
                 error("Download max retries exceeded, exiting")
                 raise Exit(code=1)
             max_retries -= 1
```

### Comparing `libretrofuzz-3.1.2/pyproject.toml` & `libretrofuzz-3.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "libretrofuzz"
-version = "3.1.2"
+version = "3.2.0"
 description = "Fuzzy Retroarch thumbnail downloader"
 authors = ["i30817 <i30817@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/i30817/libretrofuzz"
 
 [tool.poetry.dependencies]
```

### Comparing `libretrofuzz-3.1.2/setup.py` & `libretrofuzz-3.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 
 entry_points = \
 {'console_scripts': ['libretro-fuzz = libretrofuzz.__main__:fuzzsingle',
                      'libretro-fuzzall = libretrofuzz.__main__:fuzzall']}
 
 setup_kwargs = {
     'name': 'libretrofuzz',
-    'version': '3.1.2',
+    'version': '3.2.0',
     'description': 'Fuzzy Retroarch thumbnail downloader',
-    'long_description': "**Fuzzy Retroarch thumbnail downloader**\n========================================\n\nIn Retroarch, when you use the manual scanner to get nonstandard games or hacks in playlists, thumbnails often fail to download.\n\nThese programs, for each game label on a playlist, download the most similar named image to display in retroarch.\n\nThere are several options to fit unusual labels and increase fuzziness, but you can just run them to get the most restrictive default (require exact matches after the standard heuristics). If you still want more thumbnails, using ``libretro-fuzz --min 100 --delay 5 --delay 5`` works (lowering ``--min`` increases fuzz), with some delays introduced before and after downloading to check if you want to keep the game selected for the thumbnails.\n\nIf you use ``libretro-fuzz``, it will download for a single playlist by asking for the playlist and system if they're not provided.\nIf you use ``libretro-fuzzall``, it will download for all playlists with standard libretro names, and will skip custom playlists.\n\nBesides those differences, if no retroarch.cfg is provided, both programs try to use the default retroarch.cfg.\n\nIf `chafa <https://github.com/hpjansson/chafa>`_ is installed, the program will display new thumbnails of a game, with gray border for images already in use and with green border for new images. Chafa works better with a recent release and on a `sixel <https://en.wikipedia.org/wiki/Sixel>`_ or `kitty <https://sw.kovidgoyal.net/kitty/graphics-protocol/>`_ compatible shell.\n\nExample:\n | ``libretro-fuzz --system 'Commodore - Amiga' --no-merge --before '_'``\n\n The Retroplay WHDLoad set has labels like ``MonkeyIsland2_v1.3_0020`` after a manual scan. These labels *often* don't have subtitles (but not always) and all the metadata is not separated from the name by brackets. Select the playlist that contains those whdloads to download from the libretro amiga thumbnails.\n\nNote that the system name you download from doesn't have to be the same as the playlist name.\n\nIf the thumbnail server contains games from multiple releases for the system (like ``ScummVM``), be careful using extra options since it is easy to end up with 'slightly wrong' covers.\n\nExample:\n ``libretro-fuzz --no-meta --no-merge``\n\n After downloading ``ScummVM`` thumbnails (and not before, to minimize false positives), we'd like to try to pickup a few covers from ``DOS`` thumbnails and skip download if there a risk of mixing thumbnails from ``DOS`` and ``ScummVM`` for a single game.\n Choose the ScummVM playlist and DOS system name, and covers would be downloaded with risk of false positives: CD vs floppy covers, USA vs Japan covers, or another platform vs DOS.\n\nBecause of this increased risk of false positives with options, the default is to count everything except hack metadata as part of the match, only select the names that match exactly (after 'safe' heuristics like removing spaces) and the default pre-selected system name to be the same as the playlist name, which is safest.\n\nFalse positives will then be from using ``--min`` (allows inexact matches) or/and one of the commands that do not count metadata (``--before`` and ``--no-meta``). A common scenario is the thumbnail server not having a single thumbnail of the game, and the program selecting the best match it can which is still good enough to pass, like a sequel, prequel, or different release, most often regions/languages. It's not recommended to use ``--min`` less than 100 without ``--filter`` to a specific game, or at least ``--delay/--delay-after`` to be able to cancel.\n\nExample:\n  ``libretro-fuzz --system 'Commodore - Amiga' --before '_' --filter '[Ii]shar*'``\n\n  The best way to solve these issues is to upload the right cover to the respective libretro-thumbnail subproject with the correct name of the game variant. Then you can redownload just the updated thumbnails with a label, in this example, because of ``--filter``, the Ishar series in the WHDLoad playlist would redownload.\n\nTo debug why a game is not being matched, SHORT=1 before the command will display the simplified names checked for similarity.\n\nlibretro-fuzzall/libretro-fuzz [OPTIONS] [CFG]\n  :CFG:                 Path to the retroarch cfg file. If not default, asked from the user.\n\n                        Linux default:   ``~/.config/retroarch/retroarch.cfg``\n\n                        Windows default: ``%APPDATA%/RetroArch/retroarch.cfg``\n\n                        MacOS default:   ``~/Library/Application Support/RetroArch/config/retroarch.cfg``\n\n  --playlist <NAME libretro-fuzz only>\n                        Playlist name with labels used for thumbnail fuzzy matching. If not provided, asked from the user.\n  --system <NAME libretro-fuzz only>\n                        Directory name in the server to download thumbnails. If not provided, asked from the user.\n  --delay-after FLOAT   | Seconds after download to skip replacing thumbnails, enter continues. No-op with ``--no-image``.\n                        | [1<=x<=60]\n  --delay FLOAT         | Seconds to skip thumbnails download, enter continues.\n                        | [1<=x<=60]\n  --filter GLOB         Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, ``--filter '*'`` redownloads all.\n  --min SCORE           | 0=any, 100=fuzzy match,default 200=equal. No-op with ``--no-fail``.\n                        | [default: 100; 0<=x<=200]\n  --no-fail             Download any score. Equivalent to ``--min 0``.\n  --no-image            Don't show images even with chafa installed.\n  --no-merge            Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with ``--filter``.\n  --no-meta             Ignores () delimited metadata and may cause false positives. Forced with ``--before``.\n  --hack                Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with ``--before``.\n  --before TEXT         Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.\n  --address URL         | URL with libretro-thumbnails server. For local files, git clone/unzip packs, run ``'python3 -m http.server'`` in parent dir, and use ``--address 'http://localhost:8000'``.\n                        | [default: https://thumbnails.libretro.com]\n  --verbose N           | Show length N list: score, name, emoji hyperlinks.\n                        | [x>=1]\n  --install-completion  Install completion for the current shell.\n  --show-completion     Show completion for the current shell, to copy it or customize the installation.\n  --help                Show this message and exit.\n\n\n\nTo install the program, type on the cmd line\n\n+----------------+---------------------------------------------------------------------------------------------+\n| Latest release | ``pip install --force-reinstall libretrofuzz``                                              |\n+----------------+---------------------------------------------------------------------------------------------+\n| Current code   | ``pip install --force-reinstall https://github.com/i30817/libretrofuzz/archive/master.zip`` |\n+----------------+---------------------------------------------------------------------------------------------+\n\nIn windows, you'll want to check the option to “Add Python to PATH” when installing python, to be able to install and execute the script from any path of the cmd line.\n",
+    'long_description': "**Fuzzy Retroarch thumbnail downloader**\n========================================\n\nIn Retroarch, when you use the manual scanner to get nonstandard games or hacks in playlists, thumbnails often fail to download.\n\nThese programs, for each game label on a playlist, download the most similar named image to display in retroarch.\n\nThere are several options to fit unusual labels and increase fuzziness, but you can just run them to get the most restrictive default (require exact matches after the standard heuristics). If you still want more thumbnails, using ``libretro-fuzz --min 100 --delay 5 --delay 5`` works (lowering ``--min`` increases fuzz), with some delays introduced before and after downloading to check if you want to keep the game selected for the thumbnails.\n\nIf you use ``libretro-fuzz``, it will download for a single playlist by asking for the playlist and system if they're not provided.\nIf you use ``libretro-fuzzall``, it will download for all playlists with standard libretro names, and will skip custom playlists.\n\nBesides those differences, if no retroarch.cfg is provided, both programs try to use the default retroarch.cfg.\n\nIf `chafa <https://github.com/hpjansson/chafa>`_ is installed, the program will display new thumbnails of a game, with gray border for images already in use and with green border for new images. Chafa works better with a recent release and on a `sixel <https://en.wikipedia.org/wiki/Sixel>`_ or `kitty <https://sw.kovidgoyal.net/kitty/graphics-protocol/>`_ compatible shell.\n\nExample:\n | ``libretro-fuzz --system 'Commodore - Amiga' --no-merge --before '_'``\n\n The Retroplay WHDLoad set has labels like ``MonkeyIsland2_v1.3_0020`` after a manual scan. These labels *often* don't have subtitles (but not always) and all the metadata is not separated from the name by brackets. Select the playlist that contains those whdloads to download from the libretro amiga thumbnails.\n\nNote that the system name you download from doesn't have to be the same as the playlist name.\n\nIf the thumbnail server contains games from multiple releases for the system (like ``ScummVM``), be careful using extra options since it is easy to end up with 'slightly wrong' covers.\n\nExample:\n ``libretro-fuzz --no-meta --no-merge``\n\n After downloading ``ScummVM`` thumbnails (and not before, to minimize false positives), we'd like to try to pickup a few covers from ``DOS`` thumbnails and skip download if there a risk of mixing thumbnails from ``DOS`` and ``ScummVM`` for a single game.\n Choose the ScummVM playlist and DOS system name, and covers would be downloaded with risk of false positives: CD vs floppy covers, USA vs Japan covers, or another platform vs DOS.\n\nBecause of this increased risk of false positives with options, the default is to count everything except hack metadata as part of the match, only select the names that match exactly (after 'safe' heuristics like removing spaces) and the default pre-selected system name to be the same as the playlist name, which is safest.\n\nFalse positives will then be from using ``--min`` (allows inexact matches) or/and one of the commands that do not count metadata (``--before`` and ``--no-meta``). A common scenario is the thumbnail server not having a single thumbnail of the game, and the program selecting the best match it can which is still good enough to pass, like a sequel, prequel, or different release, most often regions/languages. It's not recommended to use ``--min`` less than 100 without ``--filter`` to a specific game, or at least ``--delay/--delay-after`` to be able to cancel.\n\nExample:\n  ``libretro-fuzz --system 'Commodore - Amiga' --before '_' --filter '[Ii]shar*'``\n\n  The best way to solve these issues is to upload the right cover to the respective libretro-thumbnail subproject with the correct name of the game variant. Then you can redownload just the updated thumbnails with a label, in this example, because of ``--filter``, the Ishar series in the WHDLoad playlist would redownload.\n\nTo debug why a game is not being matched, SHORT=1 before the command will display the simplified names checked for similarity.\n\nlibretro-fuzzall/libretro-fuzz [OPTIONS] [CFG]\n  :CFG:                 Path to the retroarch cfg file. If not default, asked from the user.\n\n                        Linux default:   ``~/.config/retroarch/retroarch.cfg``\n\n                        Windows default: ``%APPDATA%/RetroArch/retroarch.cfg``\n\n                        MacOS default:   ``~/Library/Application Support/RetroArch/config/retroarch.cfg``\n\n  --playlist <NAME libretro-fuzz only>\n                        Playlist name with labels used for thumbnail fuzzy matching. If not provided, asked from the user.\n  --system <NAME libretro-fuzz only>\n                        Directory name in the server to download thumbnails. If not provided, asked from the user.\n  --delay-after FLOAT   | Seconds after download to skip replacing thumbnails, enter continues. No-op with ``--no-image``.\n                        | [1<=x<=60]\n  --delay FLOAT         | Seconds to skip thumbnails download, enter continues.\n                        | [1<=x<=60]\n  --filter GLOB         Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, ``--filter '*'`` redownloads all.\n  --min SCORE           | 0=any, 100≃equal, 99=default. No-op with ``--no-fail``.\n                        | [default: 99; 0<=x<=100]\n  --no-fail             Download any score. Equivalent to ``--min 0``.\n  --no-image            Don't show images even with chafa installed.\n  --no-merge            Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with ``--filter``.\n  --no-meta             Ignores () delimited metadata and may cause false positives. Forced with ``--before``.\n  --hack                Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with ``--before``.\n  --before TEXT         Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.\n  --address URL         | URL with libretro-thumbnails server. For local files, git clone/unzip packs, run ``'python3 -m http.server'`` in parent dir, and use ``--address 'http://localhost:8000'``.\n                        | [default: https://thumbnails.libretro.com]\n  --dry-run             Print results only, no image download.\n  --verbose N           | Show length N list: score, name, emoji hyperlinks.\n                        | [x>=1]\n  --install-completion  Install completion for the current shell.\n  --show-completion     Show completion for the current shell, to copy it or customize the installation.\n  --help                Show this message and exit.\n\n\n\nTo install the program, type on the cmd line\n\n+----------------+---------------------------------------------------------------------------------------------+\n| Latest release | ``pip install --force-reinstall libretrofuzz``                                              |\n+----------------+---------------------------------------------------------------------------------------------+\n| Current code   | ``pip install --force-reinstall https://github.com/i30817/libretrofuzz/archive/master.zip`` |\n+----------------+---------------------------------------------------------------------------------------------+\n\nIn windows, you'll want to check the option to “Add Python to PATH” when installing python, to be able to install and execute the script from any path of the cmd line.\n",
     'author': 'i30817',
     'author_email': 'i30817@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/i30817/libretrofuzz',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `libretrofuzz-3.1.2/PKG-INFO` & `libretrofuzz-3.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libretrofuzz
-Version: 3.1.2
+Version: 3.2.0
 Summary: Fuzzy Retroarch thumbnail downloader
 Home-page: https://github.com/i30817/libretrofuzz
 License: MIT
 Author: i30817
 Author-email: i30817@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -83,24 +83,25 @@
   --system <NAME libretro-fuzz only>
                         Directory name in the server to download thumbnails. If not provided, asked from the user.
   --delay-after FLOAT   | Seconds after download to skip replacing thumbnails, enter continues. No-op with ``--no-image``.
                         | [1<=x<=60]
   --delay FLOAT         | Seconds to skip thumbnails download, enter continues.
                         | [1<=x<=60]
   --filter GLOB         Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, ``--filter '*'`` redownloads all.
-  --min SCORE           | 0=any, 100=fuzzy match,default 200=equal. No-op with ``--no-fail``.
-                        | [default: 100; 0<=x<=200]
+  --min SCORE           | 0=any, 100≃equal, 99=default. No-op with ``--no-fail``.
+                        | [default: 99; 0<=x<=100]
   --no-fail             Download any score. Equivalent to ``--min 0``.
   --no-image            Don't show images even with chafa installed.
   --no-merge            Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with ``--filter``.
   --no-meta             Ignores () delimited metadata and may cause false positives. Forced with ``--before``.
   --hack                Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with ``--before``.
   --before TEXT         Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.
   --address URL         | URL with libretro-thumbnails server. For local files, git clone/unzip packs, run ``'python3 -m http.server'`` in parent dir, and use ``--address 'http://localhost:8000'``.
                         | [default: https://thumbnails.libretro.com]
+  --dry-run             Print results only, no image download.
   --verbose N           | Show length N list: score, name, emoji hyperlinks.
                         | [x>=1]
   --install-completion  Install completion for the current shell.
   --show-completion     Show completion for the current shell, to copy it or customize the installation.
   --help                Show this message and exit.
```

