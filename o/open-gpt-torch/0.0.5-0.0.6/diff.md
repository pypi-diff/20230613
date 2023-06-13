# Comparing `tmp/open_gpt_torch-0.0.5.tar.gz` & `tmp/open_gpt_torch-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_gpt_torch-0.0.5.tar", max compression
+gzip compressed data, was "open_gpt_torch-0.0.6.tar", max compression
```

## Comparing `open_gpt_torch-0.0.5.tar` & `open_gpt_torch-0.0.6.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0    10825 2023-06-12 10:13:36.643150 open_gpt_torch-0.0.5/LICENSE
--rw-r--r--   0        0        0     7611 2023-06-12 10:13:36.643150 open_gpt_torch-0.0.5/README.md
--rw-r--r--   0        0        0      929 2023-06-12 10:13:36.671151 open_gpt_torch-0.0.5/open_gpt/__init__.py
--rw-r--r--   0        0        0      107 2023-06-12 10:13:36.671151 open_gpt_torch-0.0.5/open_gpt/__main__.py
--rw-r--r--   0        0        0        0 2023-06-12 10:13:36.671151 open_gpt_torch-0.0.5/open_gpt/cli/__init__.py
--rw-r--r--   0        0        0     1057 2023-06-12 10:13:36.671151 open_gpt_torch-0.0.5/open_gpt/cli/application.py
--rw-r--r--   0        0        0      508 2023-06-12 10:13:36.671151 open_gpt_torch-0.0.5/open_gpt/cli/command_loader.py
--rw-r--r--   0        0        0        0 2023-06-12 10:13:36.671151 open_gpt_torch-0.0.5/open_gpt/cli/commands/__init__.py
--rw-r--r--   0        0        0      567 2023-06-12 10:13:36.671151 open_gpt_torch-0.0.5/open_gpt/cli/commands/about.py
--rw-r--r--   0        0        0      953 2023-06-12 10:13:36.671151 open_gpt_torch-0.0.5/open_gpt/cli/commands/playground.py
--rw-r--r--   0        0        0     2223 2023-06-12 10:13:36.671151 open_gpt_torch-0.0.5/open_gpt/cli/commands/serve.py
--rw-r--r--   0        0        0     5326 2023-06-12 10:13:36.671151 open_gpt_torch-0.0.5/open_gpt/factory.py
--rw-r--r--   0        0        0     2523 2023-06-12 10:13:36.671151 open_gpt_torch-0.0.5/open_gpt/helper.py
--rw-r--r--   0        0        0      490 2023-06-12 10:13:36.671151 open_gpt_torch-0.0.5/open_gpt/logs.py
--rw-r--r--   0        0        0        0 2023-06-12 10:13:36.671151 open_gpt_torch-0.0.5/open_gpt/models/__init__.py
--rw-r--r--   0        0        0     2420 2023-06-12 10:13:36.671151 open_gpt_torch-0.0.5/open_gpt/models/embedding.py
--rw-r--r--   0        0        0        0 2023-06-12 10:13:36.671151 open_gpt_torch-0.0.5/open_gpt/models/flamingo/__init__.py
--rw-r--r--   0        0        0     6038 2023-06-12 10:13:36.671151 open_gpt_torch-0.0.5/open_gpt/models/flamingo/flamingo_lm.py
--rw-r--r--   0        0        0     9040 2023-06-12 10:13:36.671151 open_gpt_torch-0.0.5/open_gpt/models/flamingo/flamingo_model.py
--rw-r--r--   0        0        0     5647 2023-06-12 10:13:36.671151 open_gpt_torch-0.0.5/open_gpt/models/flamingo/loading.py
--rw-r--r--   0        0        0     2545 2023-06-12 10:13:36.671151 open_gpt_torch-0.0.5/open_gpt/models/flamingo/modeling.py
--rw-r--r--   0        0        0    11346 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/open_gpt/models/generation.py
--rw-r--r--   0        0        0        0 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/open_gpt/models/llama/__init__.py
--rw-r--r--   0        0        0     2877 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/open_gpt/models/llama/loading.py
--rw-r--r--   0        0        0      943 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/open_gpt/models/llama/modeling.py
--rw-r--r--   0        0        0     2856 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/open_gpt/models/loading.py
--rw-r--r--   0        0        0     2564 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/open_gpt/models/modeling.py
--rw-r--r--   0        0        0        0 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/open_gpt/models/moss/__init__.py
--rw-r--r--   0        0        0     3504 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/open_gpt/models/moss/modeling.py
--rw-r--r--   0        0        0        0 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/open_gpt/models/pythia/__init__.py
--rw-r--r--   0        0        0      653 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/open_gpt/models/pythia/modeling.py
--rw-r--r--   0        0        0        0 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/open_gpt/models/rwkv/__init__.py
--rw-r--r--   0        0        0      659 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/open_gpt/models/rwkv/modeling.py
--rw-r--r--   0        0        0        0 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/open_gpt/models/stablelm/__init__.py
--rw-r--r--   0        0        0     2608 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/open_gpt/models/stablelm/modeling.py
--rw-r--r--   0        0        0        0 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/open_gpt/models/vicuna/__init__.py
--rw-r--r--   0        0        0     7439 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/open_gpt/models/vicuna/loading.py
--rw-r--r--   0        0        0     1521 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/open_gpt/models/vicuna/modeling.py
--rw-r--r--   0        0        0     3507 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/open_gpt/profile.py
--rw-r--r--   0        0        0        0 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/open_gpt/serve/__init__.py
--rw-r--r--   0        0        0       36 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/open_gpt/serve/executors/__init__.py
--rw-r--r--   0        0        0     1977 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/open_gpt/serve/executors/base.py
--rw-r--r--   0        0        0     2373 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/open_gpt/serve/executors/flamingo.py
--rw-r--r--   0        0        0      171 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/open_gpt/serve/executors/utils.py
--rw-r--r--   0        0        0     3429 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/open_gpt/serve/gateway.py
--rw-r--r--   0        0        0        0 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/open_gpt/serve/playground/__init__.py
--rw-r--r--   0        0        0     4686 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/open_gpt/serve/playground/gradio.py
--rw-r--r--   0        0        0     7396 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/open_gpt/serve/playground/gradio_chatbot.py
--rw-r--r--   0        0        0     2714 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/open_gpt/serve/playground/gradio_css.py
--rw-r--r--   0        0        0     3094 2023-06-12 10:13:36.675150 open_gpt_torch-0.0.5/pyproject.toml
--rw-r--r--   0        0        0    20700 1970-01-01 00:00:00.000000 open_gpt_torch-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    10825 2023-06-13 06:23:11.272000 open_gpt_torch-0.0.6/LICENSE
+-rw-r--r--   0        0        0     7610 2023-06-13 06:23:11.272000 open_gpt_torch-0.0.6/README.md
+-rw-r--r--   0        0        0      929 2023-06-13 06:23:11.300001 open_gpt_torch-0.0.6/open_gpt/__init__.py
+-rw-r--r--   0        0        0      107 2023-06-13 06:23:11.300001 open_gpt_torch-0.0.6/open_gpt/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:23:11.300001 open_gpt_torch-0.0.6/open_gpt/cli/__init__.py
+-rw-r--r--   0        0        0     1057 2023-06-13 06:23:11.300001 open_gpt_torch-0.0.6/open_gpt/cli/application.py
+-rw-r--r--   0        0        0      508 2023-06-13 06:23:11.300001 open_gpt_torch-0.0.6/open_gpt/cli/command_loader.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:23:11.300001 open_gpt_torch-0.0.6/open_gpt/cli/commands/__init__.py
+-rw-r--r--   0        0        0      567 2023-06-13 06:23:11.300001 open_gpt_torch-0.0.6/open_gpt/cli/commands/about.py
+-rw-r--r--   0        0        0      953 2023-06-13 06:23:11.300001 open_gpt_torch-0.0.6/open_gpt/cli/commands/playground.py
+-rw-r--r--   0        0        0     2223 2023-06-13 06:23:11.300001 open_gpt_torch-0.0.6/open_gpt/cli/commands/serve.py
+-rw-r--r--   0        0        0     5293 2023-06-13 06:23:11.300001 open_gpt_torch-0.0.6/open_gpt/factory.py
+-rw-r--r--   0        0        0     2523 2023-06-13 06:23:11.300001 open_gpt_torch-0.0.6/open_gpt/helper.py
+-rw-r--r--   0        0        0      490 2023-06-13 06:23:11.300001 open_gpt_torch-0.0.6/open_gpt/logs.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:23:11.304000 open_gpt_torch-0.0.6/open_gpt/models/__init__.py
+-rw-r--r--   0        0        0     2420 2023-06-13 06:23:11.304000 open_gpt_torch-0.0.6/open_gpt/models/embedding.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:23:11.304000 open_gpt_torch-0.0.6/open_gpt/models/flamingo/__init__.py
+-rw-r--r--   0        0        0     6038 2023-06-13 06:23:11.304000 open_gpt_torch-0.0.6/open_gpt/models/flamingo/flamingo_lm.py
+-rw-r--r--   0        0        0     9040 2023-06-13 06:23:11.304000 open_gpt_torch-0.0.6/open_gpt/models/flamingo/flamingo_model.py
+-rw-r--r--   0        0        0     5523 2023-06-13 06:23:11.304000 open_gpt_torch-0.0.6/open_gpt/models/flamingo/loading.py
+-rw-r--r--   0        0        0     2545 2023-06-13 06:23:11.304000 open_gpt_torch-0.0.6/open_gpt/models/flamingo/modeling.py
+-rw-r--r--   0        0        0    11346 2023-06-13 06:23:11.304000 open_gpt_torch-0.0.6/open_gpt/models/generation.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:23:11.304000 open_gpt_torch-0.0.6/open_gpt/models/llama/__init__.py
+-rw-r--r--   0        0        0     2877 2023-06-13 06:23:11.304000 open_gpt_torch-0.0.6/open_gpt/models/llama/loading.py
+-rw-r--r--   0        0        0      863 2023-06-13 06:23:11.304000 open_gpt_torch-0.0.6/open_gpt/models/llama/modeling.py
+-rw-r--r--   0        0        0     2856 2023-06-13 06:23:11.304000 open_gpt_torch-0.0.6/open_gpt/models/loading.py
+-rw-r--r--   0        0        0     2564 2023-06-13 06:23:11.304000 open_gpt_torch-0.0.6/open_gpt/models/modeling.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:23:11.304000 open_gpt_torch-0.0.6/open_gpt/models/moss/__init__.py
+-rw-r--r--   0        0        0     3504 2023-06-13 06:23:11.304000 open_gpt_torch-0.0.6/open_gpt/models/moss/modeling.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:23:11.304000 open_gpt_torch-0.0.6/open_gpt/models/pythia/__init__.py
+-rw-r--r--   0        0        0      653 2023-06-13 06:23:11.304000 open_gpt_torch-0.0.6/open_gpt/models/pythia/modeling.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:23:11.304000 open_gpt_torch-0.0.6/open_gpt/models/rwkv/__init__.py
+-rw-r--r--   0        0        0     1233 2023-06-13 06:23:11.304000 open_gpt_torch-0.0.6/open_gpt/models/rwkv/modeling.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:23:11.304000 open_gpt_torch-0.0.6/open_gpt/models/stablelm/__init__.py
+-rw-r--r--   0        0        0     2608 2023-06-13 06:23:11.304000 open_gpt_torch-0.0.6/open_gpt/models/stablelm/modeling.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:23:11.304000 open_gpt_torch-0.0.6/open_gpt/models/vicuna/__init__.py
+-rw-r--r--   0        0        0     7439 2023-06-13 06:23:11.304000 open_gpt_torch-0.0.6/open_gpt/models/vicuna/loading.py
+-rw-r--r--   0        0        0     1428 2023-06-13 06:23:11.304000 open_gpt_torch-0.0.6/open_gpt/models/vicuna/modeling.py
+-rw-r--r--   0        0        0     3507 2023-06-13 06:23:11.304000 open_gpt_torch-0.0.6/open_gpt/profile.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:23:11.304000 open_gpt_torch-0.0.6/open_gpt/serve/__init__.py
+-rw-r--r--   0        0        0       36 2023-06-13 06:23:11.304000 open_gpt_torch-0.0.6/open_gpt/serve/executors/__init__.py
+-rw-r--r--   0        0        0     1977 2023-06-13 06:23:11.304000 open_gpt_torch-0.0.6/open_gpt/serve/executors/base.py
+-rw-r--r--   0        0        0     2373 2023-06-13 06:23:11.304000 open_gpt_torch-0.0.6/open_gpt/serve/executors/flamingo.py
+-rw-r--r--   0        0        0      171 2023-06-13 06:23:11.304000 open_gpt_torch-0.0.6/open_gpt/serve/executors/utils.py
+-rw-r--r--   0        0        0     3429 2023-06-13 06:23:11.304000 open_gpt_torch-0.0.6/open_gpt/serve/gateway.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:23:11.304000 open_gpt_torch-0.0.6/open_gpt/serve/playground/__init__.py
+-rw-r--r--   0        0        0     4686 2023-06-13 06:23:11.304000 open_gpt_torch-0.0.6/open_gpt/serve/playground/gradio.py
+-rw-r--r--   0        0        0     7396 2023-06-13 06:23:11.304000 open_gpt_torch-0.0.6/open_gpt/serve/playground/gradio_chatbot.py
+-rw-r--r--   0        0        0     2714 2023-06-13 06:23:11.304000 open_gpt_torch-0.0.6/open_gpt/serve/playground/gradio_css.py
+-rw-r--r--   0        0        0     3237 2023-06-13 06:23:11.304000 open_gpt_torch-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0    20866 1970-01-01 00:00:00.000000 open_gpt_torch-0.0.6/PKG-INFO
```

### Comparing `open_gpt_torch-0.0.5/LICENSE` & `open_gpt_torch-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.5/README.md` & `open_gpt_torch-0.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # ☄️ OpenGPT
 
 <p align="center">
-<a href="https://github.com/jina-ai/opengpt"><img src="https://github.com/jina-ai/opengpt/blob/main/.github/images/logo.png?" alt="OpenGPT: An open-source cloud-native large-scale multimodal model serving framework" width="300px"></a>
+<a href="https://github.com/jina-ai/opengpt"><img src="https://github.com/jina-ai/opengpt/blob/main/.github/images/logo.png" alt="OpenGPT: An open-source cloud-native large-scale multimodal model serving framework" width="300px"></a>
 <br>
 </p>
 
 > "A playful and whimsical vector art of a Stochastic Tigger, wearing a t-shirt with a "GPT" text printed logo, surrounded by colorful geometric shapes.  –ar 1:1 –upbeta"
 >
 > — Prompts and logo art was produced with  [PromptPerfect](https://promptperfect.jina.ai/) & [Stable Diffusion X](https://clipdrop.co/stable-diffusion)
```

### Comparing `open_gpt_torch-0.0.5/open_gpt/__init__.py` & `open_gpt_torch-0.0.6/open_gpt/__init__.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.5/open_gpt/cli/application.py` & `open_gpt_torch-0.0.6/open_gpt/cli/application.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.5/open_gpt/cli/commands/about.py` & `open_gpt_torch-0.0.6/open_gpt/cli/commands/about.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.5/open_gpt/cli/commands/playground.py` & `open_gpt_torch-0.0.6/open_gpt/cli/commands/playground.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.5/open_gpt/cli/commands/serve.py` & `open_gpt_torch-0.0.6/open_gpt/cli/commands/serve.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.5/open_gpt/factory.py` & `open_gpt_torch-0.0.6/open_gpt/factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,19 +97,17 @@
         return FlamingoModel(
             model_name,
             device=device,
             precision=precision,
             device_map=device_map,
             **kwargs,
         )
-    elif model_name.startswith('RWKV/rwkv'):
+    elif model_name.startswith('sgugger/rwkv') or model_name.startswith('ybelkada/rwkv'):
         from .models.rwkv.modeling import RWKVModel
 
-        assert adapter_name_or_path is None, 'RWKV does not support adapter'
-
         return RWKVModel(
             model_name,
             device=device,
             precision=precision,
             device_map=device_map,
             **kwargs,
         )
```

### Comparing `open_gpt_torch-0.0.5/open_gpt/helper.py` & `open_gpt_torch-0.0.6/open_gpt/helper.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.5/open_gpt/models/embedding.py` & `open_gpt_torch-0.0.6/open_gpt/models/embedding.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.5/open_gpt/models/flamingo/flamingo_lm.py` & `open_gpt_torch-0.0.6/open_gpt/models/flamingo/flamingo_lm.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.5/open_gpt/models/flamingo/flamingo_model.py` & `open_gpt_torch-0.0.6/open_gpt/models/flamingo/flamingo_model.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.5/open_gpt/models/flamingo/loading.py` & `open_gpt_torch-0.0.6/open_gpt/models/flamingo/loading.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,46 +9,54 @@
 
 def load_model_and_transforms(
     model_name_or_path: str,
     vision_model_name_or_path: str,
     lang_model_name_or_path: str,
     tokenizer_name_or_path: Optional[str] = None,
     decoder_layers_attr_name: Optional[str] = None,
-    device: 'torch.device' = torch.device('cuda'),
-    dtype: 'torch.dtype' = torch.float16,
+    device: Optional[torch.device] = None,
+    precision: Optional[str] = None,
+    dtype: Optional[torch.dtype] = None,
     device_map: Optional[Union[str, List[int]]] = None,
-    no_split_module_classes: Optional[List[str]] = None,
     **kwargs,
 ):
     """Load a Flamingo model and its associated image and text processors.
 
     :param model_name_or_path: The name or path of the model to load.
     :param vision_model_name_or_path: The name or path of the vision model to use.
     :param lang_model_name_or_path: The name or path of the language model to use.
     :param tokenizer_name_or_path: The name or path of the tokenizer to use. If not specified, the tokenizer associated with the model will be used.
     :param decoder_layers_attr_name: The name of the attribute that specifies the decoder layers.
+    :param precision: The precision to load the model with.
     :param device: The device to load the model on.
     :param dtype: The dtype to load the model with.
     """
 
-    from ...helper import cast_to_precision
-    from ..loading import load_model_and_tokenizer as load_llama_model_and_tokenizer
+    import os
+
+    from ..llama.loading import (
+        load_model_and_tokenizer as load_llama_model_and_tokenizer,
+    )
     from .flamingo_lm import FlamingoLMMixin
     from .flamingo_model import FlamingoLMModel
 
+    hf_token = os.environ.get("HF_TOKEN")
+    assert (
+        hf_token is not None
+    ), "Please set HF_TOKEN environment variable to download model from HuggingFace Hub"
+
     assert (
         device_map is None
     ), f"`device_map={device_map}` is not supported for Flamingo models"
 
     # load the vision model
-    precision = cast_to_precision(dtype)
     model_name, *pretrained = vision_model_name_or_path.split("::")
     pretrained = pretrained[0] if len(pretrained) == 1 else 'openai'
     clip_model, _, image_processor = open_clip.create_model_and_transforms(
-        model_name, pretrained=pretrained, device=device, precision=precision
+        model_name, pretrained=pretrained
     )
     # set the vision encoder to output the visual features
     clip_model.visual.output_tokens = True
 
     # remove text encoder to save footprint and memory
     if hasattr(clip_model, 'text'):
         del clip_model.text
@@ -66,15 +74,14 @@
     # load the language model
     lang_model, tokenizer = load_llama_model_and_tokenizer(
         model_name_or_path=lang_model_name_or_path,
         tokenizer_name_or_path=tokenizer_name_or_path,
         device=device,
         dtype=dtype,
         device_map=device_map,
-        no_split_module_classes=no_split_module_classes,
     )
 
     # add Flamingo special tokens to the tokenizer
     tokenizer.add_special_tokens(
         {"additional_special_tokens": ["<|endofchunk|>", "<image>"]}
     )
 
@@ -113,23 +120,16 @@
     model.lang_encoder.get_input_embeddings().requires_grad_(True)
 
     logger.debug(
         f"Flamingo model initialized with {sum(p.numel() for p in model.parameters() if p.requires_grad)} trainable parameters"
     )
 
     # grab model checkpoint from huggingface hub
-    import os
-
     from huggingface_hub import hf_hub_download
 
-    hf_token = os.environ.get("HF_TOKEN")
-    assert (
-        hf_token is not None
-    ), "Please set HF_TOKEN environment variable to download model from HuggingFace Hub"
-
     checkpoint_path = hf_hub_download(
         model_name_or_path, "checkpoint.pt", token=hf_token
     )
     model.load_state_dict(torch.load(checkpoint_path), strict=False)
 
     return model, tokenizer, image_processor
```

### Comparing `open_gpt_torch-0.0.5/open_gpt/models/flamingo/modeling.py` & `open_gpt_torch-0.0.6/open_gpt/models/flamingo/modeling.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.5/open_gpt/models/generation.py` & `open_gpt_torch-0.0.6/open_gpt/models/generation.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.5/open_gpt/models/llama/loading.py` & `open_gpt_torch-0.0.6/open_gpt/models/llama/loading.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.5/open_gpt/models/llama/modeling.py` & `open_gpt_torch-0.0.6/open_gpt/models/llama/modeling.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 
 import torch
 
 from open_gpt.models.modeling import BaseModel
 
 
 class LlamaModel(BaseModel):
-    no_split_module_classes = ["LlamaDecoderLayer"]
-
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def load_model_and_transforms(
         self,
         model_name_or_path: str,
         adapter_name_or_path: Optional[str] = None,
@@ -27,9 +25,7 @@
             precision=self._precision,
             device=self._device,
             device_map=self._device_map,
         )
 
         if adapter_name_or_path:
             self.load_adapter(adapter_name_or_path)
-
-        self.model.eval()
```

### Comparing `open_gpt_torch-0.0.5/open_gpt/models/loading.py` & `open_gpt_torch-0.0.6/open_gpt/models/loading.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.5/open_gpt/models/modeling.py` & `open_gpt_torch-0.0.6/open_gpt/models/modeling.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -42,14 +42,18 @@
 
         self.load_model_and_transforms(
             model_name_or_path,
             adapter_name_or_path=adapter_name_or_path,
             tokenizer_name_or_path=tokenizer_name_or_path,
         )
 
+        # turn the eval mode off `eval_mode=False` in training
+        if self._eval_mode:
+            self.model.eval()
+
         self.post_init(**kwargs)
 
     def load_model_and_transforms(
         self,
         model_name_or_path: str,
         adapter_name_or_path: Optional[str] = None,
         tokenizer_name_or_path: Optional[str] = None,
@@ -64,18 +68,14 @@
             device=self._device,
             device_map=self._device_map,
         )
 
         if adapter_name_or_path is not None:
             self.load_adapter(adapter_name_or_path)
 
-        # turn the eval mode off `eval_mode=False` in training
-        if self._eval_mode:
-            self.model.eval()
-
     def post_init(self, **kwargs):
         pass
 
     def load_adapter(self, adapter_name_or_path: str):
         from peft import PeftModel
 
         self.model = PeftModel.from_pretrained(
```

### Comparing `open_gpt_torch-0.0.5/open_gpt/models/moss/modeling.py` & `open_gpt_torch-0.0.6/open_gpt/models/moss/modeling.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.5/open_gpt/models/pythia/modeling.py` & `open_gpt_torch-0.0.6/open_gpt/models/pythia/modeling.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.5/open_gpt/models/stablelm/modeling.py` & `open_gpt_torch-0.0.6/open_gpt/models/stablelm/modeling.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.5/open_gpt/models/vicuna/loading.py` & `open_gpt_torch-0.0.6/open_gpt/models/vicuna/loading.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.5/open_gpt/models/vicuna/modeling.py` & `open_gpt_torch-0.0.6/open_gpt/models/vicuna/modeling.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,11 +44,8 @@
         self.model, self.tokenizer = load_model_and_tokenizer(
             model_name_or_path,
             tokenizer_name_or_path=tokenizer_name_or_path,
             dtype=self._dtype,
             precision=self._precision,
             device=self._device,
             device_map=self._device_map,
-            no_split_module_classes=self.no_split_module_classes,
         )
-
-        self.model.eval()
```

### Comparing `open_gpt_torch-0.0.5/open_gpt/profile.py` & `open_gpt_torch-0.0.6/open_gpt/profile.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.5/open_gpt/serve/executors/base.py` & `open_gpt_torch-0.0.6/open_gpt/serve/executors/base.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.5/open_gpt/serve/executors/flamingo.py` & `open_gpt_torch-0.0.6/open_gpt/serve/executors/flamingo.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.5/open_gpt/serve/gateway.py` & `open_gpt_torch-0.0.6/open_gpt/serve/gateway.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.5/open_gpt/serve/playground/gradio.py` & `open_gpt_torch-0.0.6/open_gpt/serve/playground/gradio.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.5/open_gpt/serve/playground/gradio_chatbot.py` & `open_gpt_torch-0.0.6/open_gpt/serve/playground/gradio_chatbot.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.5/open_gpt/serve/playground/gradio_css.py` & `open_gpt_torch-0.0.6/open_gpt/serve/playground/gradio_css.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.5/pyproject.toml` & `open_gpt_torch-0.0.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "open_gpt_torch"
-version = "0.0.5"
+version = "0.0.6"
 description = "An open-source cloud-native of large multi-modal models (LMMs) serving framework."
 
 license = "Apache-2.0"
 
 authors = [
     "Jina AI <hello@jina.ai>"
 ]
@@ -42,40 +42,43 @@
 [build-system]
 requires = ["poetry-core>=1.1.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.dependencies]
 # Compatible Python versions
 python = ">=3.8,<4.0"
-jina = "^3.15.0"
+jina = "^3.17.0"
 docarray = "^0.21.0"
 inference-client = "^0.0.4"
 pydantic = "^1.10.0"
 loguru = "^0.5"
 cleo = "^2.0.0"
 click = "^8.1.3"
 numpy = "^1.21.2"
 einops = "^0.6.0"
+tensorboard = "^2.11.2"
 transformers = "^4.30.1"
-open_clip_torch = ">2.16.0"
-bitsandbytes = ">=0.39.0"
+bitsandbytes = "^0.39.0"
 accelerate = "^0.20.3"
 tqdm = "^4.62.3"
 peft = "^0.3.0"
 
 # A list of all of the optional dependencies, some of which are included in the
 # below `extras`. They can be opted into by apps.
+psutil = { version = "^5.8.0", optional = true }
 open-flamingo = { version = "^0.0.2", optional = true }
+open_clip_torch = { version = "^2.20.0", optional = true }
 gradio = { version = "^3.30.0", optional = true }
 mdtex2html = { version = "^1.2.0", optional = true }
 markdown2 = { version = "^2.4.0", optional = true }
 
 [tool.poetry.extras]
-flamingo = ["open-flamingo"]
+flamingo = ["open-flamingo", "open_clip_torch"]
 playground = ["gradio", "mdtex2html", "markdown2"]
+profile = ["psutil"]
 
 
 # Dependency groups are supported for organizing your dependencies
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.0.262"
 mypy = "^1.2.0"
 pre-commit = ">=2.15.0"
```

### Comparing `open_gpt_torch-0.0.5/PKG-INFO` & `open_gpt_torch-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-gpt-torch
-Version: 0.0.5
+Version: 0.0.6
 Summary: An open-source cloud-native of large multi-modal models (LMMs) serving framework.
 Home-page: https://github.com/jina-ai/opengpt
 License: Apache-2.0
 Keywords: Pytorch,LMM,GPT,LLM,multi-modality,cloud-native,model-serving,model-inference,llama,vicuna,stabellm
 Author: Jina AI
 Author-email: hello@jina.ai
 Requires-Python: >=3.8,<4.0
@@ -22,40 +22,43 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: flamingo
 Provides-Extra: playground
+Provides-Extra: profile
 Requires-Dist: accelerate (>=0.20.3,<0.21.0)
-Requires-Dist: bitsandbytes (>=0.39.0)
+Requires-Dist: bitsandbytes (>=0.39.0,<0.40.0)
 Requires-Dist: cleo (>=2.0.0,<3.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: docarray (>=0.21.0,<0.22.0)
 Requires-Dist: einops (>=0.6.0,<0.7.0)
 Requires-Dist: gradio (>=3.30.0,<4.0.0) ; extra == "playground"
 Requires-Dist: inference-client (>=0.0.4,<0.0.5)
-Requires-Dist: jina (>=3.15.0,<4.0.0)
+Requires-Dist: jina (>=3.17.0,<4.0.0)
 Requires-Dist: loguru (>=0.5,<0.6)
 Requires-Dist: markdown2 (>=2.4.0,<3.0.0) ; extra == "playground"
 Requires-Dist: mdtex2html (>=1.2.0,<2.0.0) ; extra == "playground"
 Requires-Dist: numpy (>=1.21.2,<2.0.0)
 Requires-Dist: open-flamingo (>=0.0.2,<0.0.3) ; extra == "flamingo"
-Requires-Dist: open_clip_torch (>2.16.0)
+Requires-Dist: open_clip_torch (>=2.20.0,<3.0.0) ; extra == "flamingo"
 Requires-Dist: peft (>=0.3.0,<0.4.0)
+Requires-Dist: psutil (>=5.8.0,<6.0.0) ; extra == "profile"
 Requires-Dist: pydantic (>=1.10.0,<2.0.0)
+Requires-Dist: tensorboard (>=2.11.2,<3.0.0)
 Requires-Dist: tqdm (>=4.62.3,<5.0.0)
 Requires-Dist: transformers (>=4.30.1,<5.0.0)
 Project-URL: Repository, https://github.com/jina-ai/opengpt
 Description-Content-Type: text/markdown
 
 # ☄️ OpenGPT
 
 <p align="center">
-<a href="https://github.com/jina-ai/opengpt"><img src="https://github.com/jina-ai/opengpt/blob/main/.github/images/logo.png?" alt="OpenGPT: An open-source cloud-native large-scale multimodal model serving framework" width="300px"></a>
+<a href="https://github.com/jina-ai/opengpt"><img src="https://github.com/jina-ai/opengpt/blob/main/.github/images/logo.png" alt="OpenGPT: An open-source cloud-native large-scale multimodal model serving framework" width="300px"></a>
 <br>
 </p>
 
 > "A playful and whimsical vector art of a Stochastic Tigger, wearing a t-shirt with a "GPT" text printed logo, surrounded by colorful geometric shapes.  –ar 1:1 –upbeta"
 >
 > — Prompts and logo art was produced with  [PromptPerfect](https://promptperfect.jina.ai/) & [Stable Diffusion X](https://clipdrop.co/stable-diffusion)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: open-gpt-torch Version: 0.0.5 Summary: An open-
+Metadata-Version: 2.1 Name: open-gpt-torch Version: 0.0.6 Summary: An open-
 source cloud-native of large multi-modal models (LMMs) serving framework. Home-
 page: https://github.com/jina-ai/opengpt License: Apache-2.0 Keywords:
 Pytorch,LMM,GPT,LLM,multi-modality,cloud-native,model-serving,model-
 inference,llama,vicuna,stabellm Author: Jina AI Author-email: hello@jina.ai
 Requires-Python: >=3.8,<4.0 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: Apache Software License
@@ -11,28 +11,30 @@
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Topic :: Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Classifier: Topic :: Scientific/Engineering ::
 Mathematics Classifier: Topic :: Software Development Classifier: Topic ::
 Software Development :: Libraries Classifier: Topic :: Software Development ::
 Libraries :: Python Modules Provides-Extra: flamingo Provides-Extra: playground
-Requires-Dist: accelerate (>=0.20.3,<0.21.0) Requires-Dist: bitsandbytes
-(>=0.39.0) Requires-Dist: cleo (>=2.0.0,<3.0.0) Requires-Dist: click
-(>=8.1.3,<9.0.0) Requires-Dist: docarray (>=0.21.0,<0.22.0) Requires-Dist:
-einops (>=0.6.0,<0.7.0) Requires-Dist: gradio (>=3.30.0,<4.0.0) ; extra ==
-"playground" Requires-Dist: inference-client (>=0.0.4,<0.0.5) Requires-Dist:
-jina (>=3.15.0,<4.0.0) Requires-Dist: loguru (>=0.5,<0.6) Requires-Dist:
-markdown2 (>=2.4.0,<3.0.0) ; extra == "playground" Requires-Dist: mdtex2html
-(>=1.2.0,<2.0.0) ; extra == "playground" Requires-Dist: numpy (>=1.21.2,<2.0.0)
-Requires-Dist: open-flamingo (>=0.0.2,<0.0.3) ; extra == "flamingo" Requires-
-Dist: open_clip_torch (>2.16.0) Requires-Dist: peft (>=0.3.0,<0.4.0) Requires-
-Dist: pydantic (>=1.10.0,<2.0.0) Requires-Dist: tqdm (>=4.62.3,<5.0.0)
-Requires-Dist: transformers (>=4.30.1,<5.0.0) Project-URL: Repository, https://
-github.com/jina-ai/opengpt Description-Content-Type: text/markdown # âï¸
-OpenGPT
+Provides-Extra: profile Requires-Dist: accelerate (>=0.20.3,<0.21.0) Requires-
+Dist: bitsandbytes (>=0.39.0,<0.40.0) Requires-Dist: cleo (>=2.0.0,<3.0.0)
+Requires-Dist: click (>=8.1.3,<9.0.0) Requires-Dist: docarray
+(>=0.21.0,<0.22.0) Requires-Dist: einops (>=0.6.0,<0.7.0) Requires-Dist: gradio
+(>=3.30.0,<4.0.0) ; extra == "playground" Requires-Dist: inference-client
+(>=0.0.4,<0.0.5) Requires-Dist: jina (>=3.17.0,<4.0.0) Requires-Dist: loguru
+(>=0.5,<0.6) Requires-Dist: markdown2 (>=2.4.0,<3.0.0) ; extra == "playground"
+Requires-Dist: mdtex2html (>=1.2.0,<2.0.0) ; extra == "playground" Requires-
+Dist: numpy (>=1.21.2,<2.0.0) Requires-Dist: open-flamingo (>=0.0.2,<0.0.3) ;
+extra == "flamingo" Requires-Dist: open_clip_torch (>=2.20.0,<3.0.0) ; extra ==
+"flamingo" Requires-Dist: peft (>=0.3.0,<0.4.0) Requires-Dist: psutil
+(>=5.8.0,<6.0.0) ; extra == "profile" Requires-Dist: pydantic (>=1.10.0,<2.0.0)
+Requires-Dist: tensorboard (>=2.11.2,<3.0.0) Requires-Dist: tqdm
+(>=4.62.3,<5.0.0) Requires-Dist: transformers (>=4.30.1,<5.0.0) Project-URL:
+Repository, https://github.com/jina-ai/opengpt Description-Content-Type: text/
+markdown # âï¸ OpenGPT
   [OpenGPT:_An_open-source_cloud-native_large-scale_multimodal_model_serving
                                   framework]
 > "A playful and whimsical vector art of a Stochastic Tigger, wearing a t-shirt
 with a "GPT" text printed logo, surrounded by colorful geometric shapes. âar
 1:1 âupbeta" > > â Prompts and logo art was produced with [PromptPerfect]
 (https://promptperfect.jina.ai/) & [Stable Diffusion X](https://clipdrop.co/
 stable-diffusion) ![](https://img.shields.io/badge/Made%20with-JinaAI-
```

