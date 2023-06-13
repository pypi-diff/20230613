# Comparing `tmp/BaseDeploy-0.0.1.tar.gz` & `tmp/BaseDeploy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/BaseDeploy-0.0.1.tar", last modified: Thu Jun  8 08:28:20 2023, max compression
+gzip compressed data, was "dist/BaseDeploy-0.0.2.tar", last modified: Tue Jun 13 08:04:20 2023, max compression
```

## Comparing `BaseDeploy-0.0.1.tar` & `BaseDeploy-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-06-08 08:28:20.000000 BaseDeploy-0.0.1/
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-06-08 08:28:20.000000 BaseDeploy-0.0.1/BaseDeploy/
--rw-rw-r--   0 user      (1001) user      (1001)    16218 2023-06-06 05:57:34.000000 BaseDeploy-0.0.1/BaseDeploy/BaseDeploy.py
--rw-rw-r--   0 user      (1001) user      (1001)      174 2023-06-05 14:43:36.000000 BaseDeploy-0.0.1/BaseDeploy/__init__.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-06-08 08:28:20.000000 BaseDeploy-0.0.1/BaseDeploy.egg-info/
--rw-rw-r--   0 user      (1001) user      (1001)      299 2023-06-08 08:28:20.000000 BaseDeploy-0.0.1/BaseDeploy.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1001) user      (1001)      287 2023-06-08 08:28:20.000000 BaseDeploy-0.0.1/BaseDeploy.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1001) user      (1001)        1 2023-06-08 08:28:20.000000 BaseDeploy-0.0.1/BaseDeploy.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1001) user      (1001)       60 2023-06-08 08:28:20.000000 BaseDeploy-0.0.1/BaseDeploy.egg-info/requires.txt
--rw-rw-r--   0 user      (1001) user      (1001)       11 2023-06-08 08:28:20.000000 BaseDeploy-0.0.1/BaseDeploy.egg-info/top_level.txt
--rw-rw-r--   0 user      (1001) user      (1001)        1 2023-06-07 11:34:56.000000 BaseDeploy-0.0.1/BaseDeploy.egg-info/zip-safe
--rw-rw-r--   0 user      (1001) user      (1001)       40 2023-04-06 03:45:54.000000 BaseDeploy-0.0.1/MANIFEST.in
--rw-rw-r--   0 user      (1001) user      (1001)      299 2023-06-08 08:28:20.000000 BaseDeploy-0.0.1/PKG-INFO
--rw-rw-r--   0 user      (1001) user      (1001)       59 2023-06-08 08:27:27.000000 BaseDeploy-0.0.1/install_requires.txt
--rw-rw-r--   0 user      (1001) user      (1001)       38 2023-06-08 08:28:20.000000 BaseDeploy-0.0.1/setup.cfg
--rw-rw-r--   0 user      (1001) user      (1001)     4230 2023-06-08 08:28:12.000000 BaseDeploy-0.0.1/setup.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-06-13 08:04:20.000000 BaseDeploy-0.0.2/
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-06-13 08:04:20.000000 BaseDeploy-0.0.2/BaseDeploy/
+-rw-rw-r--   0 user      (1001) user      (1001)    21811 2023-06-13 07:43:46.000000 BaseDeploy-0.0.2/BaseDeploy/BaseDeploy.py
+-rw-rw-r--   0 user      (1001) user      (1001)      206 2023-06-13 08:04:12.000000 BaseDeploy-0.0.2/BaseDeploy/__init__.py
+-rw-rw-r--   0 user      (1001) user      (1001)     1298 2023-06-13 07:57:10.000000 BaseDeploy-0.0.2/BaseDeploy/version.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-06-13 08:04:20.000000 BaseDeploy-0.0.2/BaseDeploy.egg-info/
+-rw-rw-r--   0 user      (1001) user      (1001)      299 2023-06-13 08:04:20.000000 BaseDeploy-0.0.2/BaseDeploy.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1001) user      (1001)      346 2023-06-13 08:04:20.000000 BaseDeploy-0.0.2/BaseDeploy.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        1 2023-06-13 08:04:20.000000 BaseDeploy-0.0.2/BaseDeploy.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       57 2023-06-13 08:04:20.000000 BaseDeploy-0.0.2/BaseDeploy.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       60 2023-06-13 08:04:20.000000 BaseDeploy-0.0.2/BaseDeploy.egg-info/requires.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       11 2023-06-13 08:04:20.000000 BaseDeploy-0.0.2/BaseDeploy.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        1 2023-06-07 11:34:56.000000 BaseDeploy-0.0.2/BaseDeploy.egg-info/zip-safe
+-rw-rw-r--   0 user      (1001) user      (1001)       40 2023-04-06 03:45:54.000000 BaseDeploy-0.0.2/MANIFEST.in
+-rw-rw-r--   0 user      (1001) user      (1001)      299 2023-06-13 08:04:20.000000 BaseDeploy-0.0.2/PKG-INFO
+-rw-rw-r--   0 user      (1001) user      (1001)       59 2023-06-08 08:27:27.000000 BaseDeploy-0.0.2/install_requires.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       38 2023-06-13 08:04:20.000000 BaseDeploy-0.0.2/setup.cfg
+-rw-rw-r--   0 user      (1001) user      (1001)     4238 2023-06-13 07:53:50.000000 BaseDeploy-0.0.2/setup.py
```

### Comparing `BaseDeploy-0.0.1/BaseDeploy/BaseDeploy.py` & `BaseDeploy-0.0.2/BaseDeploy/BaseDeploy.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 import BaseDT
 from BaseDT.data import ModelData, ImageData
 import numpy as np
 from typing import Union, List
 import os
 import cv2
 import matplotlib.pyplot as plt
@@ -93,30 +92,45 @@
                 img = cv2.imread(input_data)
                 _, encoded_image = cv2.imencode('.jpg', img)
                 encoded_string = base64.b64encode(encoded_image).decode('utf-8')
                 self.siot.publish(IOT_Topic, encoded_string)
 
                 self.siot.subscribe(IOT_Result_Topic, rec_cb)
         if self.backend == 'ort':
-            if isinstance(input_data, str):
-                if os.path.isfile(input_data):
+            if self.backbone == '':
+                input_shape = self.model.get_inputs()[0].shape
+                if input_shape[0] == 'unk__606':
+                    img_size = tuple(input_shape[1:3])
+                else:
+                    img_size = tuple(input_shape[-2:])
+                if isinstance(input_data, str):
+                    if os.path.isfile(input_data):
+                        input_data = ImageData(input_data, size = img_size)
+                    elif os.path.isdir(input_data):
+                        input_data = [ImageData(os.path.join(input_data, f), size = img_size) for f in os.listdir(input_data) if os.path.isfile(os.path.join(input_data, f))]
+                if isinstance(input_data, np.ndarray):
+                    input_data = ImageData(input_data, size = img_size)
+            else:
+                if isinstance(input_data, str):
+                    if os.path.isfile(input_data):
+                        input_data = ImageData(input_data, backbone = self.backbone)
+                    elif os.path.isdir(input_data):
+                        input_data = [ImageData(os.path.join(input_data, f), backbone = self.backbone) for f in os.listdir(input_data) if os.path.isfile(os.path.join(input_data, f))]
+                if isinstance(input_data, np.ndarray):
                     input_data = ImageData(input_data, backbone = self.backbone)
-                elif os.path.isdir(input_data):
-                    input_data = [ImageData(os.path.join(input_data, f), backbone = self.backbone) for f in os.listdir(input_data) if os.path.isfile(os.path.join(input_data, f))]
-            if isinstance(input_data, np.ndarray):
-                input_data = ImageData(input_data, backbone = self.backbone)
             if isinstance(input_data, ImageData):
                 input_data = [input_data]
             assert isinstance(input_data, list)
             input_name = self.model.get_inputs()[0].name
             output_names = [o.name for o in self.model.get_outputs()]
             results = []
             for dt in input_data:
                 assert isinstance(dt, ImageData)
                 if self.codebase == 'MMCls':
+                    score = 0
                     pred_onx = self.model.run(output_names, {input_name: dt.to_tensor()})
                     if pred_onx[0].ndim == 1:
                         pred_onx[0] = pred_onx[0][np.newaxis,:]
                     idx = np.argmax(pred_onx[0], axis=1)[0]
                     result = {'标签':idx, '置信度':pred_onx[0][0][idx], 
                                    '预测结果':self.class_names[idx]}
                     if show_path:
@@ -150,14 +164,15 @@
                             result.append(tmp_dict)
                     results.append(result)
                     if show:
                         from BaseDT.plot import show_det
                         show_det([dt], [result])        
                         print(result)
                 elif self.codebase == 'TFJS':
+                    score = 0
                     import copy
                     copy_dt = copy.deepcopy(dt)
                     input_tensor = copy_dt.to_tensor()
                     input_data_tfjs = np.transpose(input_tensor, (0, 2, 3, 1))
                     output_data = self.model.run(output_names, {input_name: input_data_tfjs})[0]
                     idx = np.argmax(output_data)
                     acc = output_data[0][idx]
@@ -173,15 +188,88 @@
                             print(result)
                         else:
                             print("The accuracy is lower than the preset value, "
                                   "if you want to draw a picture, "
                                   "please set score={:.2f}, or lower.".format(result['置信度']))
                     #pred_onx = self.model.run(output_names, {input_name: dt.to_tensor()})
                 else:
-                    print(f'CodeBase {self.codebase} will be supported latter')
+                    input_shape = self.model.get_inputs()[0].shape
+                    print('The onnx model is not exported by the XEdu tool.'\
+						' BaseDeploy calls BaseDT to adapt the input to {}.'\
+						' \'mean\': [123.675, 116.28, 103.53], \'std\': [58.395, 57.12, 57.375], \'normalize\': True'.format(input_shape))
+                    if input_shape[0] == 'unk__606':
+                        score = 0
+                        import copy
+                        copy_dt = copy.deepcopy(dt)
+                        input_tensor = copy_dt.to_tensor()
+                        input_data_tfjs = np.transpose(input_tensor, (0, 2, 3, 1))
+                        output_data = self.model.run(output_names, {input_name: input_data_tfjs})[0]
+                        idx = np.argmax(output_data)
+                        acc = output_data[0][idx]
+                        result = {'标签':idx, '置信度':acc}
+                        if show_path:
+                            result['路径'] = dt.data_source
+                        results.append(result)
+                        if show:
+                            if result['置信度'] >= score:
+                                from BaseDT.plot import show_cls
+                                show_cls([dt], [result])
+                                print(result)
+                            else:
+                                print("The accuracy is lower than the preset value, "
+                                    "if you want to draw a picture, "
+                                    "please set score={:.2f}, or lower.".format(result['置信度']))
+                    else:
+                        pred_onx = self.model.run(output_names, {input_name: dt.to_tensor()})
+                        if len(pred_onx) == 1:
+                            # consider as cls
+                            score = 0
+                            if pred_onx[0].ndim == 1:
+                                pred_onx[0] = pred_onx[0][np.newaxis,:]
+                            idx = np.argmax(pred_onx[0], axis=1)[0]
+                            result = {'标签':idx, '置信度':pred_onx[0][0][idx]}
+                            if show_path:
+                                result['路径'] = dt.data_source
+                            results.append(result)
+                            if show:
+                                if result['置信度'] >= score:
+                                    from BaseDT.plot import show_cls
+                                    show_cls([dt], [result])
+                                    print(result)
+                                else:
+                                    print("The accuracy is lower than the preset value, "
+                                        "if you want to draw a picture, "
+                                        "please set score={:.2f}, or lower.".format(result['置信度']))
+                        elif len(pred_onx) == 2:
+                            # consider as det
+                            pred_onx = self.model.run(output_names, {input_name: dt.to_tensor()})
+                            boxes = dt.map_orig_coords(pred_onx[0][0])
+                            labels = pred_onx[1][0]
+                            result = []
+
+                            for box, label in zip(boxes, labels):
+                                if box[4] >= score:
+                                    box_int = box.astype(np.int32)
+                                    tmp_dict = {'标签':label, '置信度':box[4], 
+                                                '坐标': {'x1':box_int[0], 
+                                                        'y1':box_int[1],
+                                                        'x2':box_int[2],
+                                                        'y2':box_int[3]}}
+                                    if show_path:
+                                        tmp_dict['路径'] = dt.data_source
+                                    result.append(tmp_dict)
+                            results.append(result)
+                            print(result)
+                            if show:
+                                from BaseDT.plot import show_det
+                                show_det([dt], [result])        
+                                print(result)
+                        else:
+                            return pred_onx
+                    #print(f'CodeBase {self.codebase} will be supported latter')
             if get_img == 'pil':
                 results, imgs = self._get_img(input_data, results, score, show)
                 results = results[0] if len(results) == 1 else results
                 imgs = imgs[0] if len(imgs) == 1 else imgs
                 return results, imgs
             elif get_img == 'cv2':
                 results, imgs = self._get_img(input_data, results, score, show)
@@ -201,15 +289,15 @@
         def predict(input_img, score):
             dt = ImageData(input_img, backbone=self.backbone)
             result, img = self.inference(dt, score=score, get_img='pil')
             return img, result
         gr_infer = gr.Interface(
             fn=predict,
             inputs=[gr.Image(type="filepath"),
-                    gr.Slider(minimum=0, maximum=1, value=0.65, step=0.01, label="Score")],
+                    gr.Slider(minimum=0, maximum=1, value=0.0, step=0.01, label="Score")],
             outputs = [gr.Image(type="numpy"), "text"]
         )
         gr_infer.launch()
 
     def run_fastapi(self, 
                     port: int = 1956,
                     mode: str = 'json',
@@ -359,12 +447,17 @@
                         dt.init_plt()
                     else:
                         from BaseDT.plot import show_cls
                         show_cls(dt, results[i])
                 imgs.append(dt.get_image())
         return results, imgs
     
+    def diy_inference(self, input_data):
+        assert isinstance(input_data, np.ndarray)
+        input_name = self.model.get_inputs()[0].name
+        output_names = [o.name for o in self.model.get_outputs()]
+        pred_onx = self.model.run(output_names, {input_name: input_data})
+        return pred_onx
+    
     def print_result(self, result):
         print('推理结果如下：')
-        print(result)
-
-            
+        print(result)
```

### Comparing `BaseDeploy-0.0.1/setup.py` & `BaseDeploy-0.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,15 +75,15 @@
                 yield item
 
     packages = list(gen_packages_items())
     return packages
 
 setup(
     name='BaseDeploy',
-    version='0.0.1',
+    version='0.0.2',
     # version='0.0.1rc1',
     description='BaseDeploy is a simple deployment tool made by XEdu.',
     license='MIT License',
     author='OpenXLab',
     author_email='wangbolun@pjlab.org.cn',
     url='https://github.com/OpenXLab-Edu/OpenMMLab-Edu',
     packages=find_packages(),
@@ -96,13 +96,13 @@
     # ],
     # classifiers=[
     #     # 'Operating System :: Linux',
     #     'Programming Language :: Python :: 3.8',
     # ],
     python_requires='>=3.6',
     zip_safe=True,
-    # entry_points= {'console_scripts': ['MMEdu = MMEdu.version:hello',]},
+    entry_points= {'console_scripts': ['BaseDeploy = BaseDeploy.version:hello',]},
     # build_scripts
     # dependency_links = [
     #     " https://download.pytorch.org/whl/cu101/torch-1.8.1%2Bcu101-cp38-cp38-linux_x86_64.whl#egg=torch-1.8.1+cu101",
     # ],
 )
```

