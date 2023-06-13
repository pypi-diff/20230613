# Comparing `tmp/kotan-0.1.4.tar.gz` & `tmp/kotan-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kotan-0.1.4.tar", max compression
+gzip compressed data, was "kotan-1.0.0.tar", max compression
```

## Comparing `kotan-0.1.4.tar` & `kotan-1.0.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0        0 2023-05-16 05:09:07.710676 kotan-0.1.4/README.md
--rw-r--r--   0        0        0       45 2023-05-17 23:24:18.924115 kotan-0.1.4/kotan/__init__.py
--rw-r--r--   0        0        0      299 2023-05-16 05:09:07.710676 kotan-0.1.4/kotan/const.py
--rw-r--r--   0        0        0     2122 2023-05-17 23:24:17.844189 kotan-0.1.4/kotan/job.py
--rw-r--r--   0        0        0      112 2023-05-16 05:09:07.710676 kotan-0.1.4/kotan/tasks/__init__.py
--rw-r--r--   0        0        0     3251 2023-05-16 06:06:15.311045 kotan-0.1.4/kotan/tasks/data_augmentation.py
--rw-r--r--   0        0        0     2590 2023-05-16 05:25:58.316875 kotan-0.1.4/kotan/tasks/machine_translation.py
--rw-r--r--   0        0        0      327 2023-05-17 23:24:23.783782 kotan-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      555 1970-01-01 00:00:00.000000 kotan-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     3310 2023-06-13 07:25:27.501181 kotan-1.0.0/README.md
+-rw-r--r--   0        0        0       45 2023-06-13 06:01:56.207576 kotan-1.0.0/kotan/__init__.py
+-rw-r--r--   0        0        0      749 2023-06-13 06:01:56.207576 kotan-1.0.0/kotan/const.py
+-rw-r--r--   0        0        0     2727 2023-06-13 06:01:56.207576 kotan-1.0.0/kotan/job.py
+-rw-r--r--   0        0        0      168 2023-06-13 06:01:56.207576 kotan-1.0.0/kotan/tasks/__init__.py
+-rw-r--r--   0        0        0     4309 2023-06-13 07:21:43.612245 kotan-1.0.0/kotan/tasks/data_augmentation.py
+-rw-r--r--   0        0        0     2071 2023-06-13 06:01:56.207576 kotan-1.0.0/kotan/tasks/machine_translation.py
+-rw-r--r--   0        0        0     2214 2023-06-13 06:01:56.207576 kotan-1.0.0/kotan/tasks/style_convert.py
+-rw-r--r--   0        0        0      383 2023-06-13 07:30:22.773181 kotan-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3921 1970-01-01 00:00:00.000000 kotan-1.0.0/PKG-INFO
```

### Comparing `kotan-0.1.4/kotan/job.py` & `kotan-1.0.0/kotan/job.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 import torch
 
 from .tasks import (
     KoTANTranslationFactory,
-    KoTANAugmentationFactory
+    KoTANAugmentationFactory,
+    KoTANStyleConversiontFactory
 )
 
-from .const import LANG_ALIASES, LEVEL
+from .const import LANG_ALIASES, LEVEL, STYLE
 
 
 # Task list
 SUPPORTED_TASKS = {
     "mt": KoTANTranslationFactory,
     "translation": KoTANTranslationFactory,
     "aug": KoTANAugmentationFactory,
-    "augmentation": KoTANAugmentationFactory
+    "augmentation": KoTANAugmentationFactory,
+    "style": KoTANStyleConversiontFactory,
+    "convert": KoTANStyleConversiontFactory
 }
 
 
 class KoTAN:
     def __new__(
             cls,
             task,
             tgt="en",
-            level="fine"
+            level="fine",
+            style="formal"
             ):
         
         if task not in SUPPORTED_TASKS:
             raise KeyError("Unknown task {}, available tasks are {}".format(
                 task,
                 list(SUPPORTED_TASKS.keys()),
             ))
@@ -39,21 +43,27 @@
         
         if level not in LEVEL:
             raise KeyError("Unknown level {}, available levels are {}".format(
                 task,
                 list(LEVEL.keys()),
             ))
         
+        if style not in STYLE:
+            raise KeyError("Unknown style {}, available levels are {}".format(
+                task,
+                list(STYLE.keys()),
+            ))
+        
         device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 
         task_module = SUPPORTED_TASKS[task](
             task,
             LANG_ALIASES[tgt],
-            LANG_ALIASES,
-            LEVEL[level]
+            LEVEL[level],
+            STYLE[style]
         ).load(device)
 
         return task_module
 
     @staticmethod
     def available_tasks():
         """
@@ -81,8 +91,19 @@
         """
         Returns available level in KoTAN project
 
         Returns:
             str: Supported level names
 
         """
-        return "Available tasks are {}".format(list(LEVEL.keys()))
+        return "Available tasks are {}".format(list(LEVEL.keys()))
+    
+    @staticmethod
+    def available_style():
+        """
+        Returns available convert style in KoTAN project
+
+        Returns:
+            str: Supported style names
+
+        """
+        return "Available tasks are {}".format(list(STYLE.keys()))
```

### Comparing `kotan-0.1.4/kotan/tasks/machine_translation.py` & `kotan-1.0.0/kotan/tasks/machine_translation.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,68 +17,60 @@
     Examples:
         >>> mt = KoTAN(task="translation", tgt="en")
     """
     def __init__(
             self,
             task,
             tgt,
-            LANG_ALIASES,
-            level
+            level,
+            style
             ):
         super().__init__()
         self.task = task
         self.tgt = tgt
-        self.LANG_ALIASES = LANG_ALIASES
 
     def load(self, device: str):
         if self.tgt == "kor_Hang":
             tokenizer = AutoTokenizer.from_pretrained("KoJLabs/nllb-finetuned-en2ko")
             model = AutoModelForSeq2SeqLM.from_pretrained("KoJLabs/nllb-finetuned-en2ko").to(device)
             
         if self.tgt == "eng_Latn":
             tokenizer = AutoTokenizer.from_pretrained("KoJLabs/nllb-finetuned-ko2en")
             model = AutoModelForSeq2SeqLM.from_pretrained("KoJLabs/nllb-finetuned-ko2en").to(device)
 
         return KoTANTranslation(
             model,
             tokenizer,
             device,
-            self.LANG_ALIASES
+            self.tgt
         )
     
 
 class KoTANTranslation:
-    def __init__(self, model, tokenizer, device, LANG_ALIASES):
+    def __init__(self, model, tokenizer, device, tgt):
         self.model = model
         self.tokenizer = tokenizer
         self.device = device
-        self.LANG_ALIASES = LANG_ALIASES
+        self.tgt = tgt
 
-    def predict(self, text, tgt):
+    def predict(self, text):
         """
         Predict a translation result
 
         Args:
             text (str): input text
-            tgt (str): target language
 
         Returns:
             output (list): Translation results
         """
         
         inputs = self.tokenizer(text, padding=True, truncation=True, return_tensors="pt")
-
-        if isinstance(inputs['input_ids'], list):
-            input_dict = {}            
-            input_dict['input_ids'] = torch.LongTensor(inputs['input_ids']).reshape(1,len(inputs['input_ids']))
-            input_dict['attention_mask'] = torch.LongTensor(inputs['attention_mask']).reshape(1,len(inputs['attention_mask']))
-            inputs = BatchEncoding(input_dict)
             
         translated_tokens = self.model.generate(
-            **inputs.to(self.device), forced_bos_token_id=self.tokenizer.lang_code_to_id[self.LANG_ALIASES[tgt]], max_length=128
+            **inputs.to(self.device), forced_bos_token_id=self.tokenizer.lang_code_to_id[self.tgt], max_length=128
         )
 
         output = self.tokenizer.batch_decode(translated_tokens, skip_special_tokens=True)
             
         return output
```

