# Comparing `tmp/laserdato-0.0.12.tar.gz` & `tmp/laserdato-0.0.13.tar.gz`

## Comparing `laserdato-0.0.12.tar` & `laserdato-0.0.13.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 laserdato-0.0.12/main.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 laserdato-0.0.12/laserdato/__init__.py
--rw-r--r--   0        0        0    20534 2020-02-02 00:00:00.000000 laserdato-0.0.12/laserdato/embed.py
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 laserdato-0.0.12/laserdato/get_model.py
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 laserdato-0.0.12/laserdato/laser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 laserdato-0.0.12/laserdato/lib/__init__.py
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 laserdato-0.0.12/laserdato/lib/constants.py
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 laserdato-0.0.12/laserdato/lib/text_processing.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 laserdato-0.0.12/settings.json/settings.json
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 laserdato-0.0.12/LICENSE
--rw-r--r--   0        0        0     8059 2020-02-02 00:00:00.000000 laserdato-0.0.12/README.md
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 laserdato-0.0.12/pyproject.toml
--rw-r--r--   0        0        0     8577 2020-02-02 00:00:00.000000 laserdato-0.0.12/PKG-INFO
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 laserdato-0.0.13/main.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 laserdato-0.0.13/laserdato/__init__.py
+-rw-r--r--   0        0        0    20675 2020-02-02 00:00:00.000000 laserdato-0.0.13/laserdato/embed.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 laserdato-0.0.13/laserdato/get_model.py
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 laserdato-0.0.13/laserdato/laser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 laserdato-0.0.13/laserdato/lib/__init__.py
+-rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 laserdato-0.0.13/laserdato/lib/constants.py
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 laserdato-0.0.13/laserdato/lib/text_processing.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 laserdato-0.0.13/settings.json/settings.json
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 laserdato-0.0.13/LICENSE
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 laserdato-0.0.13/README.md
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 laserdato-0.0.13/pyproject.toml
+-rw-r--r--   0        0        0     3298 2020-02-02 00:00:00.000000 laserdato-0.0.13/PKG-INFO
```

### Comparing `laserdato-0.0.12/laserdato/embed.py` & `laserdato-0.0.13/laserdato/embed.py`

 * *Files 0% similar despite different names*

```diff
@@ -504,14 +504,18 @@
     max_tokens: int = 12000,
     max_sentences: Optional[int] = None,
     cpu: bool = False,
     fp16: bool = False,
     sort_kind: str = "quicksort",
     target_devices: Optional[list[int]] = None,
 ):
+    if verbose:
+        logging.getLogger().setLevel(logging.INFO)
+    else:
+        logging.getLogger().setLevel(logging.ERROR)
     assert encoder or encoder_path, "Provide initialised encoder or encoder_path"
     buffer_size = max(buffer_size, 1)
     assert (
         not max_sentences or max_sentences <= buffer_size
     ), "--max-sentences/--batch-size cannot be larger than --buffer-size"
     assert not cpu or target_devices == None, "Cannot use cpu and target_devices"
     if encoder_path:
@@ -523,15 +527,15 @@
             max_sentences=max_sentences,
             max_tokens=max_tokens,
             sort_kind=sort_kind,
         )
     tSMP = time.time()
     embeddings = SPMApply(sentences, spm_model, spm_lang)
     if verbose:
-        logger.info(f" - SPMApply time {time.time() - tSMP}")
+        logger.info(f" - Preprocessing finished at {time.time() - tSMP}")
     return EncodeText(
         encoder, embeddings, fp16=fp16, verbose=verbose, devices=target_devices
     )
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(description="LASER: Embed sentences")
```

### Comparing `laserdato-0.0.12/laserdato/get_model.py` & `laserdato-0.0.13/laserdato/get_model.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import os
 import requests
 from pathlib import Path
 
 MODEL_DIR = Path(__file__).parent / "models"
 LASER_2_URL = "https://tinyurl.com/nllblaser2"
 SPM_NAME = "laser2.spm"
 S3 = "https://dl.fbaipublicfiles.com/nllb/laser"  # available encoders
@@ -15,25 +14,15 @@
     else:
         response = requests.get(f"{S3}/{file}")
     file_path = MODEL_DIR / file
     with file_path.open(mode="wb") as f:
         f.write(response.content)
 
 
-def load_or_download_file(file) -> os:
+def load_or_download_file(file) -> Path:
     """Download file if not present in MODEL_DIR and return path to file"""
     if not MODEL_DIR.is_dir():
         MODEL_DIR.mkdir(parents=True)
     file_path = MODEL_DIR / file
     if not file_path.exists():
         download(file)
     return file_path
-
-
-# directory_path.mkdir()
-
-
-# # def load_model():
-# #     if not os.path.isdir(MODEL_DIR):
-# #         print(f" - creating model directory: {MODEL_DIR}")
-# #         os.makedirs(MODEL_DIR)
-# # return os.path.join(MODEL_DIR, LASER_MODEL[0])
```

### Comparing `laserdato-0.0.12/laserdato/laser.py` & `laserdato-0.0.13/laserdato/laser.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,53 @@
 from .embed import embed_sentences
 import numpy as np
-from pathlib import Path
 from .get_model import load_or_download_file
-import time
-from .lib.constants import langs
+from .lib.constants import laser3_langs, langs_with_specific_vocab
 
 
 class Laser:
-    def embed_sentences(
-        self, sentences: list[str], target_devices: list[int] = None, lang: str = None
+    def __init__(
+        self, target_devices: list[int] = None, lang: str = None, cpu: bool = True
     ):
+        """
+        :param target_devices: list of GPU ids to use for embedding, if None, will use the first GPU available
+        :param lang: only to be specified if using laser3, must be in laser3_langs. If None, will use laser2
+        :param cpu: if True, will use CPU for embedding and ignore target_devices
+        """
+        self.lang = lang
+        self.target_devices = target_devices
+        self.cpu = cpu
+
+    def embed_sentences(
+        self, sentences: list[str], verbose: bool = False
+    ) -> list[np.ndarray]:
+        """
+        :param sentences: list of sentences to embed
+        :param verbose: if True, will print progress
+        :return: list of embeddings
+        """
         version = 0
-        if lang is not None:
-            if lang not in langs:
-                raise ValueError(f"Language {lang} not supported")
+        if self.lang is not None:
+            if self.lang not in laser3_langs:
+                raise ValueError(f"Language {self.lang} not supported")
             version = 1
-            pt = load_or_download_file(f"laser3-{lang}.{version}.pt")
+            pt = load_or_download_file(f"laser3-{self.lang}.v{version}.pt")
+            if self.lang in langs_with_specific_vocab:
+                spm = load_or_download_file(
+                    f"laser3-{self.lang}.v{version}.spm"
+                ).as_posix()
+                vocab = load_or_download_file(f"laser3-{self.lang}.v{version}.cvocab")
         else:
             pt = load_or_download_file("laser2.pt")
         spm = load_or_download_file("laser2.spm").as_posix()
         vocab = load_or_download_file("laser2.cvocab")
         embeddings = embed_sentences(
             sentences=sentences,
             encoder_path=str(pt),
             spm_model=str(spm),
-            verbose=True,
+            verbose=verbose,
             max_tokens=12000,
             buffer_size=10000,
-            target_devices=target_devices,
+            target_devices=self.target_devices,
+            cpu=self.cpu,
         )
         return embeddings
-
-
-if __name__ == "__main__":
-    laser = Laser()
-    # sentences = ["This is a sentence", "this is another sentences."] * 1000000
-    sentences = ["This is a sentence", "this is another sentences."] * 10
-
-    t = time.time()
-    # print(sentences)
-    # embeddings = laser.embed_sentences(sentences=sentences, target_devices=[0, 1])
-    embeddings = laser.embed_sentences(sentences=sentences)
-    # dim = 1024
-    # embeddings.resize(embeddings.shape[0] // dim, dim)
-    print(embeddings)
-    print(embeddings.shape)
-    print(type(embeddings))
-    print(len(embeddings))
-    print(time.time() - t)
```

### Comparing `laserdato-0.0.12/laserdato/lib/constants.py` & `laserdato-0.0.13/laserdato/lib/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-langs = [
+laser3_langs = [
     "ace_Latn",
     "aka_Latn",
     "als_Latn",
     "amh_Ethi",
     "asm_Beng",
     "awa_Deva",
     "ayr_Latn",
@@ -143,7 +143,44 @@
     "wol_Latn",
     "xho_Latn",
     "ydd_Hebr",
     "yor_Latn",
     "zsm_Latn",
     "zul_Latn",
 ]
+langs_with_specific_vocab = [
+    "amh_Ethi",
+    "ayr_Latn",
+    "azj_Latn",
+    "bak_Cyrl",
+    "bel_Cyrl",
+    "bod_Tibt",
+    "ckb_Arab",
+    "crh_Latn",
+    "dik_Latn",
+    "dzo_Tibt",
+    "fur_Latn",
+    "fuv_Latn",
+    "grn_Latn",
+    "kab_Latn",
+    "kac_Latn",
+    "kaz_Cyrl",
+    "kir_Cyrl",
+    "kmr_Latn",
+    "lij_Latn",
+    "lim_Latn",
+    "lmo_Latn",
+    "ltg_Latn",
+    "mya_Mymr",
+    "pbt_Arab",
+    "pes_Arab",
+    "prs_Arab",
+    "sat_Beng",
+    "scn_Latn",
+    "srd_Latn",
+    "szl_Latn",
+    "taq_Latn",
+    "tgk_Cyrl",
+    "tir_Ethi",
+    "tzm_Tfng",
+    "vec_Latn",
+]
```

### Comparing `laserdato-0.0.12/laserdato/lib/text_processing.py` & `laserdato-0.0.13/laserdato/lib/text_processing.py`

 * *Files identical despite different names*

### Comparing `laserdato-0.0.12/LICENSE` & `laserdato-0.0.13/LICENSE`

 * *Files identical despite different names*

### Comparing `laserdato-0.0.12/pyproject.toml` & `laserdato-0.0.13/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "laserdato"
-version = "0.0.12"
+version = "0.0.13"
 authors = [
   { name="Lingua Custodia", email="" },
 ]
 description = "A small example package"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

