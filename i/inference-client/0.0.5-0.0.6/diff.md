# Comparing `tmp/inference_client-0.0.5.tar.gz` & `tmp/inference_client-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inference_client-0.0.5.tar", max compression
+gzip compressed data, was "inference_client-0.0.6.tar", max compression
```

## Comparing `inference_client-0.0.5.tar` & `inference_client-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    11357 2023-06-01 08:40:10.429325 inference_client-0.0.5/LICENSE
--rw-r--r--   0        0        0     7312 2023-06-01 08:40:10.429325 inference_client-0.0.5/README.md
--rw-r--r--   0        0        0      256 2023-06-01 08:40:10.481326 inference_client-0.0.5/inference_client/__init__.py
--rw-r--r--   0        0        0     2349 2023-06-01 08:40:10.481326 inference_client-0.0.5/inference_client/__version__.py
--rw-r--r--   0        0        0     1546 2023-06-01 08:40:10.481326 inference_client-0.0.5/inference_client/client.py
--rw-r--r--   0        0        0      719 2023-06-01 08:40:10.481326 inference_client-0.0.5/inference_client/config.py
--rw-r--r--   0        0        0     3129 2023-06-01 08:40:10.481326 inference_client-0.0.5/inference_client/helper.py
--rw-r--r--   0        0        0      250 2023-06-01 08:40:10.481326 inference_client-0.0.5/inference_client/logging.py
--rw-r--r--   0        0        0      551 2023-06-01 08:40:10.481326 inference_client-0.0.5/inference_client/model.py
--rw-r--r--   0        0        0     3541 2023-06-01 08:40:10.481326 inference_client-0.0.5/inference_client/tasks/caption.py
--rw-r--r--   0        0        0     5855 2023-06-01 08:40:10.481326 inference_client-0.0.5/inference_client/tasks/encode.py
--rw-r--r--   0        0        0     3664 2023-06-01 08:40:10.481326 inference_client-0.0.5/inference_client/tasks/generate.py
--rw-r--r--   0        0        0     2389 2023-06-01 08:40:10.481326 inference_client-0.0.5/inference_client/tasks/helper.py
--rw-r--r--   0        0        0     6174 2023-06-01 08:40:10.481326 inference_client-0.0.5/inference_client/tasks/rank.py
--rw-r--r--   0        0        0    11539 2023-06-01 08:40:10.481326 inference_client-0.0.5/inference_client/tasks/upscale.py
--rw-r--r--   0        0        0     3929 2023-06-01 08:40:10.481326 inference_client-0.0.5/inference_client/tasks/vqa.py
--rw-r--r--   0        0        0     1355 2023-06-01 08:40:10.481326 inference_client-0.0.5/pyproject.toml
--rw-r--r--   0        0        0    19692 1970-01-01 00:00:00.000000 inference_client-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-13 13:35:39.484234 inference_client-0.0.6/LICENSE
+-rw-r--r--   0        0        0     5030 2023-06-13 13:35:39.484234 inference_client-0.0.6/README.md
+-rw-r--r--   0        0        0      256 2023-06-13 13:35:39.536234 inference_client-0.0.6/inference_client/__init__.py
+-rw-r--r--   0        0        0     2349 2023-06-13 13:35:39.536234 inference_client-0.0.6/inference_client/__version__.py
+-rw-r--r--   0        0        0     1546 2023-06-13 13:35:39.536234 inference_client-0.0.6/inference_client/client.py
+-rw-r--r--   0        0        0      719 2023-06-13 13:35:39.536234 inference_client-0.0.6/inference_client/config.py
+-rw-r--r--   0        0        0     3129 2023-06-13 13:35:39.536234 inference_client-0.0.6/inference_client/helper.py
+-rw-r--r--   0        0        0      250 2023-06-13 13:35:39.536234 inference_client-0.0.6/inference_client/logging.py
+-rw-r--r--   0        0        0      551 2023-06-13 13:35:39.536234 inference_client-0.0.6/inference_client/model.py
+-rw-r--r--   0        0        0     3541 2023-06-13 13:35:39.536234 inference_client-0.0.6/inference_client/tasks/caption.py
+-rw-r--r--   0        0        0     5855 2023-06-13 13:35:39.536234 inference_client-0.0.6/inference_client/tasks/encode.py
+-rw-r--r--   0        0        0     3664 2023-06-13 13:35:39.536234 inference_client-0.0.6/inference_client/tasks/generate.py
+-rw-r--r--   0        0        0     2389 2023-06-13 13:35:39.536234 inference_client-0.0.6/inference_client/tasks/helper.py
+-rw-r--r--   0        0        0     6174 2023-06-13 13:35:39.536234 inference_client-0.0.6/inference_client/tasks/rank.py
+-rw-r--r--   0        0        0    13226 2023-06-13 13:35:39.536234 inference_client-0.0.6/inference_client/tasks/upscale.py
+-rw-r--r--   0        0        0     3929 2023-06-13 13:35:39.536234 inference_client-0.0.6/inference_client/tasks/vqa.py
+-rw-r--r--   0        0        0     1355 2023-06-13 13:35:39.536234 inference_client-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0    17410 1970-01-01 00:00:00.000000 inference_client-0.0.6/PKG-INFO
```

### Comparing `inference_client-0.0.5/LICENSE` & `inference_client-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `inference_client-0.0.5/inference_client/__version__.py` & `inference_client-0.0.6/inference_client/__version__.py`

 * *Files identical despite different names*

### Comparing `inference_client-0.0.5/inference_client/client.py` & `inference_client-0.0.6/inference_client/client.py`

 * *Files identical despite different names*

### Comparing `inference_client-0.0.5/inference_client/config.py` & `inference_client-0.0.6/inference_client/config.py`

 * *Files identical despite different names*

### Comparing `inference_client-0.0.5/inference_client/helper.py` & `inference_client-0.0.6/inference_client/helper.py`

 * *Files identical despite different names*

### Comparing `inference_client-0.0.5/inference_client/model.py` & `inference_client-0.0.6/inference_client/model.py`

 * *Files identical despite different names*

### Comparing `inference_client-0.0.5/inference_client/tasks/caption.py` & `inference_client-0.0.6/inference_client/tasks/caption.py`

 * *Files identical despite different names*

### Comparing `inference_client-0.0.5/inference_client/tasks/encode.py` & `inference_client-0.0.6/inference_client/tasks/encode.py`

 * *Files identical despite different names*

### Comparing `inference_client-0.0.5/inference_client/tasks/generate.py` & `inference_client-0.0.6/inference_client/tasks/generate.py`

 * *Files identical despite different names*

### Comparing `inference_client-0.0.5/inference_client/tasks/helper.py` & `inference_client-0.0.6/inference_client/tasks/helper.py`

 * *Files identical despite different names*

### Comparing `inference_client-0.0.5/inference_client/tasks/rank.py` & `inference_client-0.0.6/inference_client/tasks/rank.py`

 * *Files identical despite different names*

### Comparing `inference_client-0.0.5/inference_client/tasks/upscale.py` & `inference_client-0.0.6/inference_client/tasks/upscale.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     def upscale(
         self,
         *,
         image: Union[str, bytes, 'ArrayType'],
         scale: Optional[str] = None,
         image_format: Optional[str] = None,
         output_path: Optional[str] = None,
+        quality: Optional[int] = None,
         **kwargs,
     ):
         """
         Upscale plain input images. Return an image bytes in the format of `image_format`. If `output_path` is
         provided, the image will also be saved to the specified path.
 
         :param image: the image to upscale, can be a `ndarray`, 'bytes' or uri of the image
@@ -44,24 +45,28 @@
                 values being set to 0 as previously detailed. Default: None.
         :param image_format: the format of the output image, could be either `jpeg` or `png`. If not provided, the
                 same format as the input image will be used. Default: None.
         :param output_path: the complete file path to save the output image if provided in addition to returning it.
                 The path should end with the file extension of the output format, and could be either '.jpeg' or '.png'.
                 If both `output_path` and `image_format` are provided, the `image_format` will be ignored, and the
                 output image will be saved in the format of the file extension of `output_path`. Default: None.
+        :param quality: The image quality for JPEG output, on a scale from 0 (worst) to 95 (best). Values above 95
+                should be avoided; 100 disables portions of the JPEG compression algorithm, and results in large files
+                with hardly any gain in image quality. This parameter is ignored for PNG files. Default: None.
         :param kwargs: additional arguments to pass to the model.
         """
         ...
 
     @overload
     def upscale(
         self,
         *,
         docs: Union[Iterable['Document'], 'DocumentArray'],
         scale: Optional[str] = None,
+        quality: Optional[int] = None,
         **kwargs,
     ):
         """
         Upscale image documents. The result will be stored in the `blob` attribute of the document in the format of
         `image_format` specified in the `tags` attribute. If `output_path` is provided in the `tags` attribute, the
         image will also be saved to the specified path.
 
@@ -76,27 +81,31 @@
                 scale should be in the format of `width:height`, e.g. `100:200`. Both width and height should be
                 integers. If the width is 0, the input width is used for the output. If the height is 0, the input
                 height is used for the output. If one and only one of the values is -n with n >= 1, the scale filter
                 will use a value that maintains the aspect ratio of the input image, calculated from the other specified
                 dimension. After that it will, however, make sure that the calculated dimension is divisible by n and
                 adjust the value if necessary. If both values are -n with n >= 1, the behavior will be identical to both
                 values being set to 0 as previously detailed. Default: None.
+        :param quality: The image quality for JPEG output, on a scale from 0 (worst) to 95 (best). Values above 95
+                should be avoided; 100 disables portions of the JPEG compression algorithm, and results in large files
+                with hardly any gain in image quality. This parameter is ignored for PNG files. Default: None.
         :param kwargs: additional arguments to pass to the model
         """
         ...
 
     @overload
     def upscale(
         self,
         *,
         docs: Optional[Union[Iterable['Document'], 'DocumentArray']] = None,
         image: Optional[Union[str, bytes, 'ArrayType']] = None,
         scale: Optional[str] = None,
         image_format: Optional[str] = None,
         output_path: Optional[str] = None,
+        quality: Optional[int] = None,
         **kwargs,
     ):
         """
         Upscale an image or a set of image documents using a pre-trained model.
 
         :param docs: the image documents to upscale. The `image_format` and `output_path` should be provided in the
                 `tags` attribute of each document. The `image_format` specifies the format of the output image, could
@@ -116,14 +125,17 @@
                 values being set to 0 as previously detailed. Default: None.
         :param image_format: the format of the output image, could be either `jpeg` or `png`. If not provided, the
                 same format as the input image will be used. Default: None.
         :param output_path: the complete file path to save the output image if provided in addition to returning it.
                 The path should end with the file extension of the output format, and could be either '.jpeg' or '.png'.
                 If both `output_path` and `image_format` are provided, the `image_format` will be ignored, and the
                 output image will be saved in the format of the file extension of `output_path`. Default: None.
+        :param quality: The image quality for JPEG output, on a scale from 0 (worst) to 95 (best). Values above 95
+                should be avoided; 100 disables portions of the JPEG compression algorithm, and results in large files
+                with hardly any gain in image quality. This parameter is ignored for PNG files. Default: None.
         :param kwargs: additional arguments to pass to the model.
         """
         ...
 
     def upscale(self, **kwargs):
         """
         Upscale the image documents using the model.
@@ -159,22 +171,22 @@
             content_type = 'plain'
             image_content = kwargs.pop('image')
             if isinstance(image_content, (str, bytes, numpy.ndarray)):
                 image_doc = load_plain_into_document(image_content, mime_type='image')
 
                 if kwargs.get('output_path', None) is not None:
                     output_path = kwargs.pop('output_path')
-                    image_format = os.path.splitext(output_path)[1].lower()
+                    image_format = os.path.splitext(output_path)[1].strip().lower()
                     if image_format not in ('.jpeg', '.jpg', '.png'):
                         raise ValueError(
                             'Output path should end with either `.jpeg` or `.png`.'
                         )
                     image_doc.tags['output_path'] = output_path
-
-                if kwargs.get('image_format', None) is not None:
+                    image_doc.tags['image_format'] = image_format.split('.')[-1]
+                elif kwargs.get('image_format', None) is not None:
                     image_format = kwargs.pop('image_format').lower()
                     if image_format not in ('jpeg', 'jpg', 'png'):
                         raise ValueError('Output format should be either jpeg or png.')
                     image_doc.tags['image_format'] = image_format
 
                 payload.update(inputs=DocumentArray([image_doc]))
                 payload.update(total_docs=1)
@@ -187,14 +199,22 @@
         if kwargs.get('scale', None) is not None:
             scale = kwargs.pop('scale')
             self._scale_checker(scale)
             if parameters := payload.get('parameters'):
                 parameters.update(scale=scale)
             else:
                 payload.update(parameters={'scale': scale})
+        if kwargs.get('quality', None) is not None:
+            quality = kwargs.pop('quality')
+            if isinstance(quality, int) and (quality < 0 or quality > 100):
+                raise ValueError('Quality should be an integer between 0 and 100.')
+            if parameters := payload.get('parameters'):
+                parameters.update(quality=quality)
+            else:
+                payload.update(parameters={'quality': quality})
 
         return payload, content_type
 
     def _unbox_upscale_result(
         self,
         result: 'DocumentArray' = None,
         content_type: str = 'docarray',
```

### Comparing `inference_client-0.0.5/inference_client/tasks/vqa.py` & `inference_client-0.0.6/inference_client/tasks/vqa.py`

 * *Files identical despite different names*

### Comparing `inference_client-0.0.5/pyproject.toml` & `inference_client-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "inference_client"
-version = "0.0.5"
+version = "0.0.6"
 description = "Python Client for Jina Inference API"
 
 license = "Apache-2.0"
 
 authors = [
     "Jina AI <hello@jina.ai>"
 ]
```

### Comparing `inference_client-0.0.5/PKG-INFO` & `inference_client-0.0.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inference-client
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python Client for Jina Inference API
 Home-page: https://inference-api.jina.ai
 License: Apache-2.0
 Keywords: jina,inference,api,client
 Author: Jina AI
 Author-email: hello@jina.ai
 Requires-Python: >=3.8,<4.0.0
@@ -31,214 +31,141 @@
 <br>
 </p>
 
 [![PyPI](https://img.shields.io/pypi/v/inference-client)](https://pypi.org/project/inference-client/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/inference-client)](https://pypi.org/project/inference-client/)
 [![PyPI - License](https://img.shields.io/pypi/l/inference-client)](https://pypi.org/project/inference-client/)
 
-Inference Client is a library that provides a simple and efficient way to use Jina AI's Inference, a powerful platform that offers a range of AI models for common tasks such as visual reasoning, question answering, and embedding modalities like texts and images. 
-With Inference Client, you can easily select the task and model of your choice and integrate the API call into your workflow with zero technical overhead. 
+Inference-Client is a Python library that allows you to interact with the [Jina AI Inference](https://cloud.jina.ai/user/inference). 
+It provides a simple and intuitive API to perform various tasks such as image captioning, encoding, ranking, visual 
+question answering (VQA), and image upscaling.
 
 The current version of Inference Client includes methods to call the following tasks:
 
+📷 **Caption**: Generate captions for images 
+
 📈 **Encode**: Encode data into embeddings using various models 
 
 🔍 **Rank**: Re-rank cross-modal matches according to their joint likelihood
 
-📷 **Caption**: Generate captions for images 
+🆙 **Upscale**: Increasing the resolution while preserving the quality and details
 
 🤔 **VQA**: Answer questions related to images 
 
 
 ## Installation
 
 Inference Client is available on PyPI and can be installed using pip:
 
 ```bash
 pip install inference-client
 ```
 
 ## Getting Started
 
-Before using Inference Client, please create an inference on [Jina AI Cloud](https://cloud.jina.ai/user/inference).
+Before using the Inference-Client, please create an inference on [Jina AI Cloud](https://cloud.jina.ai/user/inference).
 
-After login with your Jina AI Cloud account, you can create an inference by clicking the "Create" button in the inference page.
-From there, you can select the model you want to use.
-
-After the inference is created and the status is "Serving", you can use Inference Client to connect to it.
+After the inference is created and the status is "Serving", you can use the Inference-Client to connect to it.
 This could take a few minutes, depending on the model you selected.
 
-<p align="center">
-    <img src=".github/README-img/jac.png" width="100%">
-</p>
-
 ### Client Initialization
 
-To use Inference Client, you need to initialize a Client object with the authentication token of your Jina AI Cloud account:
+To use the Inference-Client, you first need to import the `Client` class and create a new instance of it. 
 
 ```python
 from inference_client import Client
 
 client = Client(token='<your auth token>')
 ```
 
-The token can be generated at the [Jina AI Cloud](https://cloud.jina.ai/settings/tokens), or via CLI as described in [this guide](https://docs.jina.ai/jina-ai-cloud/login/#create-a-new-pat):
+You will need to provide your access token when creating the client. The token can be generated at the [Jina AI Cloud](https://cloud.jina.ai/settings/tokens), or via CLI as described in [this guide](https://docs.jina.ai/jina-ai-cloud/login/#create-a-new-pat):
 ```bash
 jina auth token create <name of PAT> -e <expiration days>
 ```
 
-
-### Connecting to Models
-
-Once you have initialized the Client object, you can connect to the models you want to use by calling the `get_model` method, which takes the name of the model as it appears in Jina AI Cloud as an argument.
+You can then use the `get_model` method of the `Client` object to get a specific model.
 
 ```python
-# connect to a CLIP model
-model = client.get_model('ViT-B-32::openai')
+model = client.get_model('<model of your selection>')
 ```
-As example, the above code connects to the CLIP model named "ViT-B-32::openai" on Jina AI Cloud.
-
 You can connect to as many inference models as you want once they have been created on Jina AI Cloud, and you can use them for multiple tasks.
 
-
-### Performing tasks
+## Performing tasks
 
 Now that you have connected to the models, you can use them to perform the tasks they support.
 
+### Image Captioning
 
-#### 1. Encoding
+The `caption` method of the `Model` object takes an image as input and returns a caption as output.
 
-The encode task is used to encode data into embeddings using various models.
-For example, you can use the CLIP model to encode text or images into embeddings:
-    
 ```python
-model = client.get_model(
-    '<name of the model that supports encode>'
-)  # e.g. ViT-B-32::openai
-
-# encode text
-result = model.encode(text='hello world')
-
-# encode image
-result = model.encode(image='hello_world.jpg')
-
-# encode image RGB tensor
-from PIL import Image
-from numpy import asarray
-
-image_bytes = Image.open('hello_world.jpg')
-image_tensor = asarray(image_bytes)
-result = model.encode(image=image_tensor)
+image = 'path/to/image.jpg'
+caption = model.caption(image=image)
 ```
 
-The output of the encode method is a DocumentArray, which contains the embeddings of the input data.
+### Encoding
 
-```bash
-# print(result[0].embedding)
+The `encode` method of the `Model` object takes text or image data as input and returns an embedding as output.
+
+```python
+text = 'a sentence describing the beautiful nature'
+embedding = model.encode(text=text)
 
-[-5.48706055e-02 -1.10717773e-01  5.13671875e-01 -3.22509766e-01
- -1.40380859e-01  6.23535156e-01  3.07617188e-01  4.26025391e-01
-  ...
-  8.04443359e-02  8.53515625e-01 -5.96008301e-02  3.61633301e-02]
+# OR
+image = 'path/to/image.jpg'
+embedding = model.encode(image=image)
 ```
 
-### 2. Ranking
+### Ranking
 
-To perform similarity-based ranking of candidate matches, you can use the `rank` method of an inference model. 
-The rank method takes a reference input and a list of candidates, and reorder that list of candidates based on their similarity to the reference input. 
-You can also construct a cross-modal Document where the root contains an image or text and `.matches` contain images or sentences to rerank.
+The `rank` method of the `Model` object takes a text or image data as query and a list of candidates as input and returns a list of reordered candidates as well as their scores as output.
 
 ```python
-# Connect to a model
-model = client.get_model('<name of the model that supports rank>')
-
-reference = 'singapore.jpg'
 candidates = [
-    'a colorful photo of nature',
-    'a photo of blue scenery',
-    'a black and white photo of a cat',
+    'an image about dogs',
+    'an image about cats',
+    'an image about birds',
 ]
-response = model.rank(reference=reference, candidates=candidates)
-
-# Access the matches
-for match in not response[0]:
-    print(match.text)
+image = 'path/to/image.jpg'
+result = model.rank(image=image, candidates=candidates)
 ```
 
-```bash
-a photo of blue scenery
-a colorful photo of nature
-a black and white photo of a cat
-```
-You may also input images as bytes or tensors similarly to the encode method.
-
-**NOTICE**: The following tasks Caption and VQA are BLIP2 exclusive. Calling these methods on other models will fall back to the default encode method.
-
-### 3. Captioning
-
-You can use caption method to generate natural language descriptions of images.
+### Image Upscaling
 
-
-The caption method takes a DocumentArray containing images or a single plain image as input.
-The plain input image can be in the form of a URL string, an image blob, or an image tensor.
-
-For example, you can use the BLIP2 model to generate captions for images:
+The `upscale` method of the `Model` object takes an image and optional configurations as input, and returns the upscaled image bytes as output.
 
 ```python
-# Initialize model
-model = client.get_model('Salesforce/blip2-opt-2.7b')
-
-response = model.caption(image='singapore.jpg')
-
-# Access the captions
-print(response[0].tags['response'])
-```
-
-```bash
-the merlion fountain in singapore at night
+image = 'path/to/image.jpg'
+result = model.upscale(image=image, output_path='upscaled_image.png', scale='800:600')
 ```
 
+### Visual Question Answering (VQA)
 
-### 4. VQA (Visual Question Answering)
-
-Visual Question Answering (VQA) is a task that involves answering natural language questions about visual content such as images. 
-Given an image and a question, the goal of VQA is to provide a natural language answer.
-The VQA method takes either a DocumentArray of images and questions, or a single plain image and question.
-
+The `vqa` method of the `Model` object takes an image and a question as input and returns an answer as output.
 
 ```python
-# Initialize model
-model = client.get_model('Salesforce/blip2-opt-2.7b')
-
-image = 'singapore.jpg'
-question = 'Question: What is this photo about? Answer:'
-
-response = model.vqa(image=image, question=question)
-
-# Access the answers
-print(response[0].tags['response'])
-```
-
-```bash
-the merlion fountain in singapore
+image = 'path/to/image.jpg'
+question = 'Question: What is the name of this place? Answer:'
+answer = model.vqa(image=image, question=question)
 ```
 
-## Documentation
+## Advanced Usage
 
-For more information about advanced usage of Inference Client, please refer to the [documentation](https://jina.readme.io/docs/inference).
+In addition to the basic usage, the Inference-Client also supports advanced features such as handling DocumentArray inputs, customizing the task parameters, and more. 
+Please refer to the [official documentation](https://jina.readme.io/docs/inference) for more details.
 
 ## Support
 
-- Join our [Slack community](https://slack.jina.ai) and chat with other community members about ideas.
+- Join our [Discord community](https://discord.jina.ai) and chat with other community members about ideas.
 - Watch our [Engineering All Hands](https://youtube.com/playlist?list=PL3UBBWOUVhFYRUa_gpYYKBqEAkO4sxmne) to learn Jina's new features and stay up-to-date with the latest AI techniques.
 - Subscribe to the latest video tutorials on our [YouTube channel](https://youtube.com/c/jina-ai)
 
 ## License
 
-Inference Client is backed by [Jina AI](https://jina.ai) and licensed under [Apache-2.0](./LICENSE). 
+Inference-Client is backed by [Jina AI](https://jina.ai) and licensed under [Apache-2.0](./LICENSE). 
                                  Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
 
    TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
 
    1. Definitions.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: inference-client Version: 0.0.5 Summary: Python
+Metadata-Version: 2.1 Name: inference-client Version: 0.0.6 Summary: Python
 Client for Jina Inference API Home-page: https://inference-api.jina.ai License:
 Apache-2.0 Keywords: jina,inference,api,client Author: Jina AI Author-email:
 hello@jina.ai Requires-Python: >=3.8,<4.0.0 Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Provides-Extra: pytorch
@@ -14,99 +14,71 @@
 Description-Content-Type: text/markdown
 
 
 [![PyPI](https://img.shields.io/pypi/v/inference-client)](https://pypi.org/
 project/inference-client/) [![PyPI - Python Version](https://img.shields.io/
 pypi/pyversions/inference-client)](https://pypi.org/project/inference-client/)
 [![PyPI - License](https://img.shields.io/pypi/l/inference-client)](https://
-pypi.org/project/inference-client/) Inference Client is a library that provides
-a simple and efficient way to use Jina AI's Inference, a powerful platform that
-offers a range of AI models for common tasks such as visual reasoning, question
-answering, and embedding modalities like texts and images. With Inference
-Client, you can easily select the task and model of your choice and integrate
-the API call into your workflow with zero technical overhead. The current
-version of Inference Client includes methods to call the following tasks: ð
-**Encode**: Encode data into embeddings using various models ð **Rank**: Re-
-rank cross-modal matches according to their joint likelihood ð· **Caption**:
-Generate captions for images ð¤ **VQA**: Answer questions related to images
-## Installation Inference Client is available on PyPI and can be installed
-using pip: ```bash pip install inference-client ``` ## Getting Started Before
-using Inference Client, please create an inference on [Jina AI Cloud](https://
-cloud.jina.ai/user/inference). After login with your Jina AI Cloud account, you
-can create an inference by clicking the "Create" button in the inference page.
-From there, you can select the model you want to use. After the inference is
-created and the status is "Serving", you can use Inference Client to connect to
-it. This could take a few minutes, depending on the model you selected.
-                         [.github/README-img/jac.png]
-### Client Initialization To use Inference Client, you need to initialize a
-Client object with the authentication token of your Jina AI Cloud account:
-```python from inference_client import Client client = Client(token='') ``` The
-token can be generated at the [Jina AI Cloud](https://cloud.jina.ai/settings/
-tokens), or via CLI as described in [this guide](https://docs.jina.ai/jina-ai-
-cloud/login/#create-a-new-pat): ```bash jina auth token create  -e  ``` ###
-Connecting to Models Once you have initialized the Client object, you can
-connect to the models you want to use by calling the `get_model` method, which
-takes the name of the model as it appears in Jina AI Cloud as an argument.
-```python # connect to a CLIP model model = client.get_model('ViT-B-32::
-openai') ``` As example, the above code connects to the CLIP model named "ViT-
-B-32::openai" on Jina AI Cloud. You can connect to as many inference models as
-you want once they have been created on Jina AI Cloud, and you can use them for
-multiple tasks. ### Performing tasks Now that you have connected to the models,
-you can use them to perform the tasks they support. #### 1. Encoding The encode
-task is used to encode data into embeddings using various models. For example,
-you can use the CLIP model to encode text or images into embeddings: ```python
-model = client.get_model( '' ) # e.g. ViT-B-32::openai # encode text result =
-model.encode(text='hello world') # encode image result = model.encode
-(image='hello_world.jpg') # encode image RGB tensor from PIL import Image from
-numpy import asarray image_bytes = Image.open('hello_world.jpg') image_tensor =
-asarray(image_bytes) result = model.encode(image=image_tensor) ``` The output
-of the encode method is a DocumentArray, which contains the embeddings of the
-input data. ```bash # print(result[0].embedding) [-5.48706055e-02 -1.10717773e-
-01 5.13671875e-01 -3.22509766e-01 -1.40380859e-01 6.23535156e-01 3.07617188e-01
-4.26025391e-01 ... 8.04443359e-02 8.53515625e-01 -5.96008301e-02 3.61633301e-
-02] ``` ### 2. Ranking To perform similarity-based ranking of candidate
-matches, you can use the `rank` method of an inference model. The rank method
-takes a reference input and a list of candidates, and reorder that list of
-candidates based on their similarity to the reference input. You can also
-construct a cross-modal Document where the root contains an image or text and
-`.matches` contain images or sentences to rerank. ```python # Connect to a
-model model = client.get_model('') reference = 'singapore.jpg' candidates =
-[ 'a colorful photo of nature', 'a photo of blue scenery', 'a black and white
-photo of a cat', ] response = model.rank(reference=reference,
-candidates=candidates) # Access the matches for match in not response[0]: print
-(match.text) ``` ```bash a photo of blue scenery a colorful photo of nature a
-black and white photo of a cat ``` You may also input images as bytes or
-tensors similarly to the encode method. **NOTICE**: The following tasks Caption
-and VQA are BLIP2 exclusive. Calling these methods on other models will fall
-back to the default encode method. ### 3. Captioning You can use caption method
-to generate natural language descriptions of images. The caption method takes a
-DocumentArray containing images or a single plain image as input. The plain
-input image can be in the form of a URL string, an image blob, or an image
-tensor. For example, you can use the BLIP2 model to generate captions for
-images: ```python # Initialize model model = client.get_model('Salesforce/
-blip2-opt-2.7b') response = model.caption(image='singapore.jpg') # Access the
-captions print(response[0].tags['response']) ``` ```bash the merlion fountain
-in singapore at night ``` ### 4. VQA (Visual Question Answering) Visual
-Question Answering (VQA) is a task that involves answering natural language
-questions about visual content such as images. Given an image and a question,
-the goal of VQA is to provide a natural language answer. The VQA method takes
-either a DocumentArray of images and questions, or a single plain image and
-question. ```python # Initialize model model = client.get_model('Salesforce/
-blip2-opt-2.7b') image = 'singapore.jpg' question = 'Question: What is this
-photo about? Answer:' response = model.vqa(image=image, question=question) #
-Access the answers print(response[0].tags['response']) ``` ```bash the merlion
-fountain in singapore ``` ## Documentation For more information about advanced
-usage of Inference Client, please refer to the [documentation](https://
-jina.readme.io/docs/inference). ## Support - Join our [Slack community](https:/
-/slack.jina.ai) and chat with other community members about ideas. - Watch our
-[Engineering All Hands](https://youtube.com/
+pypi.org/project/inference-client/) Inference-Client is a Python library that
+allows you to interact with the [Jina AI Inference](https://cloud.jina.ai/user/
+inference). It provides a simple and intuitive API to perform various tasks
+such as image captioning, encoding, ranking, visual question answering (VQA),
+and image upscaling. The current version of Inference Client includes methods
+to call the following tasks: ð· **Caption**: Generate captions for images
+ð **Encode**: Encode data into embeddings using various models ð
+**Rank**: Re-rank cross-modal matches according to their joint likelihood ð
+**Upscale**: Increasing the resolution while preserving the quality and details
+ð¤ **VQA**: Answer questions related to images ## Installation Inference
+Client is available on PyPI and can be installed using pip: ```bash pip install
+inference-client ``` ## Getting Started Before using the Inference-Client,
+please create an inference on [Jina AI Cloud](https://cloud.jina.ai/user/
+inference). After the inference is created and the status is "Serving", you can
+use the Inference-Client to connect to it. This could take a few minutes,
+depending on the model you selected. ### Client Initialization To use the
+Inference-Client, you first need to import the `Client` class and create a new
+instance of it. ```python from inference_client import Client client = Client
+(token='') ``` You will need to provide your access token when creating the
+client. The token can be generated at the [Jina AI Cloud](https://
+cloud.jina.ai/settings/tokens), or via CLI as described in [this guide](https:/
+/docs.jina.ai/jina-ai-cloud/login/#create-a-new-pat): ```bash jina auth token
+create  -e  ``` You can then use the `get_model` method of the `Client` object
+to get a specific model. ```python model = client.get_model('') ``` You can
+connect to as many inference models as you want once they have been created on
+Jina AI Cloud, and you can use them for multiple tasks. ## Performing tasks Now
+that you have connected to the models, you can use them to perform the tasks
+they support. ### Image Captioning The `caption` method of the `Model` object
+takes an image as input and returns a caption as output. ```python image =
+'path/to/image.jpg' caption = model.caption(image=image) ``` ### Encoding The
+`encode` method of the `Model` object takes text or image data as input and
+returns an embedding as output. ```python text = 'a sentence describing the
+beautiful nature' embedding = model.encode(text=text) # OR image = 'path/to/
+image.jpg' embedding = model.encode(image=image) ``` ### Ranking The `rank`
+method of the `Model` object takes a text or image data as query and a list of
+candidates as input and returns a list of reordered candidates as well as their
+scores as output. ```python candidates = [ 'an image about dogs', 'an image
+about cats', 'an image about birds', ] image = 'path/to/image.jpg' result =
+model.rank(image=image, candidates=candidates) ``` ### Image Upscaling The
+`upscale` method of the `Model` object takes an image and optional
+configurations as input, and returns the upscaled image bytes as output.
+```python image = 'path/to/image.jpg' result = model.upscale(image=image,
+output_path='upscaled_image.png', scale='800:600') ``` ### Visual Question
+Answering (VQA) The `vqa` method of the `Model` object takes an image and a
+question as input and returns an answer as output. ```python image = 'path/to/
+image.jpg' question = 'Question: What is the name of this place? Answer:
+' answer = model.vqa(image=image, question=question) ``` ## Advanced Usage In
+addition to the basic usage, the Inference-Client also supports advanced
+features such as handling DocumentArray inputs, customizing the task
+parameters, and more. Please refer to the [official documentation](https://
+jina.readme.io/docs/inference) for more details. ## Support - Join our [Discord
+community](https://discord.jina.ai) and chat with other community members about
+ideas. - Watch our [Engineering All Hands](https://youtube.com/
 playlist?list=PL3UBBWOUVhFYRUa_gpYYKBqEAkO4sxmne) to learn Jina's new features
 and stay up-to-date with the latest AI techniques. - Subscribe to the latest
 video tutorials on our [YouTube channel](https://youtube.com/c/jina-ai) ##
-License Inference Client is backed by [Jina AI](https://jina.ai) and licensed
+License Inference-Client is backed by [Jina AI](https://jina.ai) and licensed
 under [Apache-2.0](./LICENSE). Apache License Version 2.0, January 2004 http://
 www.apache.org/licenses/ TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND
 DISTRIBUTION 1. Definitions. "License" shall mean the terms and conditions for
 use, reproduction, and distribution as defined by Sections 1 through 9 of this
 document. "Licensor" shall mean the copyright owner or entity authorized by the
 copyright owner that is granting the License. "Legal Entity" shall mean the
 union of the acting entity and all other entities that control, are controlled
```

