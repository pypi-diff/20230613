# Comparing `tmp/xgo-pythonlib-0.1.4.tar.gz` & `tmp/xgo-pythonlib-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xgo-pythonlib-0.1.4.tar", last modified: Sun Jun 11 07:50:18 2023, max compression
+gzip compressed data, was "xgo-pythonlib-0.1.5.tar", last modified: Mon Jun 12 13:16:27 2023, max compression
```

## Comparing `xgo-pythonlib-0.1.4.tar` & `xgo-pythonlib-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 07:50:18.975680 xgo-pythonlib-0.1.4/
--rw-rw-rw-   0        0        0     1733 2023-06-11 07:50:18.974681 xgo-pythonlib-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1106 2023-06-08 09:16:07.000000 xgo-pythonlib-0.1.4/README.md
--rw-rw-rw-   0        0        0       42 2023-06-11 07:50:18.976679 xgo-pythonlib-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     3684 2023-06-11 07:47:55.000000 xgo-pythonlib-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-11 07:50:18.957679 xgo-pythonlib-0.1.4/xgo_pythonlib.egg-info/
--rw-rw-rw-   0        0        0     1733 2023-06-11 07:50:18.000000 xgo-pythonlib-0.1.4/xgo_pythonlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2023-06-11 07:50:18.000000 xgo-pythonlib-0.1.4/xgo_pythonlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 07:50:18.000000 xgo-pythonlib-0.1.4/xgo_pythonlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-06-11 07:50:18.000000 xgo-pythonlib-0.1.4/xgo_pythonlib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-11 07:50:18.960678 xgo-pythonlib-0.1.4/xgoedu/
--rw-rw-rw-   0        0        0    37176 2023-06-11 07:45:57.000000 xgo-pythonlib-0.1.4/xgoedu/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-11 07:50:18.963680 xgo-pythonlib-0.1.4/xgolib/
--rw-rw-rw-   0        0        0    26384 2023-06-08 09:11:58.000000 xgo-pythonlib-0.1.4/xgolib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-11 07:50:18.971680 xgo-pythonlib-0.1.4/xgoscreen/
--rw-rw-rw-   0        0        0     5339 2023-06-07 11:44:32.000000 xgo-pythonlib-0.1.4/xgoscreen/LCD_2inch.py
--rw-rw-rw-   0        0        0        0 2023-06-06 11:56:39.000000 xgo-pythonlib-0.1.4/xgoscreen/__init__.py
--rw-rw-rw-   0        0        0     2214 2023-06-06 01:30:25.000000 xgo-pythonlib-0.1.4/xgoscreen/lcdconfig.py
+drwxrwxrwx   0        0        0        0 2023-06-12 13:16:27.876812 xgo-pythonlib-0.1.5/
+-rw-rw-rw-   0        0        0     1733 2023-06-12 13:16:27.874733 xgo-pythonlib-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1106 2023-06-11 07:56:34.000000 xgo-pythonlib-0.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-12 13:16:27.876812 xgo-pythonlib-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     3684 2023-06-12 13:15:50.000000 xgo-pythonlib-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 13:16:27.866732 xgo-pythonlib-0.1.5/xgo_pythonlib.egg-info/
+-rw-rw-rw-   0        0        0     1733 2023-06-12 13:16:27.000000 xgo-pythonlib-0.1.5/xgo_pythonlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-06-12 13:16:27.000000 xgo-pythonlib-0.1.5/xgo_pythonlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 13:16:27.000000 xgo-pythonlib-0.1.5/xgo_pythonlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-06-12 13:16:27.000000 xgo-pythonlib-0.1.5/xgo_pythonlib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 13:16:27.868037 xgo-pythonlib-0.1.5/xgoedu/
+-rw-rw-rw-   0        0        0    37464 2023-06-12 13:15:04.000000 xgo-pythonlib-0.1.5/xgoedu/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 13:16:27.870046 xgo-pythonlib-0.1.5/xgolib/
+-rw-rw-rw-   0        0        0    26384 2023-06-08 09:11:58.000000 xgo-pythonlib-0.1.5/xgolib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 13:16:27.873576 xgo-pythonlib-0.1.5/xgoscreen/
+-rw-rw-rw-   0        0        0     5339 2023-06-07 11:44:32.000000 xgo-pythonlib-0.1.5/xgoscreen/LCD_2inch.py
+-rw-rw-rw-   0        0        0        0 2023-06-06 11:56:39.000000 xgo-pythonlib-0.1.5/xgoscreen/__init__.py
+-rw-rw-rw-   0        0        0     2214 2023-06-06 01:30:25.000000 xgo-pythonlib-0.1.5/xgoscreen/lcdconfig.py
```

### Comparing `xgo-pythonlib-0.1.4/PKG-INFO` & `xgo-pythonlib-0.1.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xgo-pythonlib
-Version: 0.1.4
+Version: 0.1.5
 Summary: PythonLib for XGO2-DOG
 Home-page: https://github.com/Xgorobot/XGO-PythonLib
 Author: luwudynamics
 Author-email: hello@xgorobot.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -26,15 +26,15 @@
 
 [PythonLib-WIKI](https://www.yuque.com/luwudynamics/cn/mxkaodwpo2h5zmvw)
 
 
 
 ## Install instructions 
 
-1 Burn the official 0608 img image 
+1 Burn the official 0609 img image 
 
 2 Copy all files from the "model" directory to `\home\pi\model`
 
 3 Run this command:
 
 ```
 pip install --upgrade xgo-pythonlib
@@ -56,15 +56,15 @@
 ```
 xgolib library example
 ```python
 from xgolib import XGO
 dog = XGO('/dev/ttyAMA0')
 dog.action(1)
 ```
-### Lastest Verion:0.1.3
+### Lastest Verion:0.1.4
 
 ### xgolib_version=1.3.0
 
-### xgoedu_version=1.2.1
+### xgoedu_version=1.2.2
```

### Comparing `xgo-pythonlib-0.1.4/README.md` & `xgo-pythonlib-0.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 [PythonLib-WIKI](https://www.yuque.com/luwudynamics/cn/mxkaodwpo2h5zmvw)
 
 
 
 ## Install instructions 
 
-1 Burn the official 0608 img image 
+1 Burn the official 0609 img image 
 
 2 Copy all files from the "model" directory to `\home\pi\model`
 
 3 Run this command:
 
 ```
 pip install --upgrade xgo-pythonlib
@@ -38,15 +38,15 @@
 ```
 xgolib library example
 ```python
 from xgolib import XGO
 dog = XGO('/dev/ttyAMA0')
 dog.action(1)
 ```
-### Lastest Verion:0.1.3
+### Lastest Verion:0.1.4
 
 ### xgolib_version=1.3.0
 
-### xgoedu_version=1.2.1
+### xgoedu_version=1.2.2
```

### Comparing `xgo-pythonlib-0.1.4/setup.py` & `xgo-pythonlib-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 NAME = 'xgo-pythonlib'
 DESCRIPTION = 'PythonLib for XGO2-DOG'
 URL = 'https://github.com/Xgorobot/XGO-PythonLib'
 EMAIL = 'hello@xgorobot.com'
 AUTHOR = 'luwudynamics'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.4'
+VERSION = '0.1.5'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

### Comparing `xgo-pythonlib-0.1.4/xgo_pythonlib.egg-info/PKG-INFO` & `xgo-pythonlib-0.1.5/xgo_pythonlib.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xgo-pythonlib
-Version: 0.1.4
+Version: 0.1.5
 Summary: PythonLib for XGO2-DOG
 Home-page: https://github.com/Xgorobot/XGO-PythonLib
 Author: luwudynamics
 Author-email: hello@xgorobot.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -26,15 +26,15 @@
 
 [PythonLib-WIKI](https://www.yuque.com/luwudynamics/cn/mxkaodwpo2h5zmvw)
 
 
 
 ## Install instructions 
 
-1 Burn the official 0608 img image 
+1 Burn the official 0609 img image 
 
 2 Copy all files from the "model" directory to `\home\pi\model`
 
 3 Run this command:
 
 ```
 pip install --upgrade xgo-pythonlib
@@ -56,15 +56,15 @@
 ```
 xgolib library example
 ```python
 from xgolib import XGO
 dog = XGO('/dev/ttyAMA0')
 dog.action(1)
 ```
-### Lastest Verion:0.1.3
+### Lastest Verion:0.1.4
 
 ### xgolib_version=1.3.0
 
-### xgoedu_version=1.2.1
+### xgoedu_version=1.2.2
```

### Comparing `xgo-pythonlib-0.1.4/xgoedu/__init__.py` & `xgo-pythonlib-0.1.5/xgoedu/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 import json
 import threading
 # from xgolib import XGO
 # from keras.preprocessing import image
 # import _thread  使用_thread会报错，坑！
 
 
-__versinon__ = '1.2.2'
-__last_modified__ = '2023/6/11'
+__versinon__ = '1.2.3'
+__last_modified__ = '2023/6/12'
 
 GPIO.setwarnings(False)
 GPIO.setmode(GPIO.BCM)
 
 camera_still=False
 
 
@@ -158,15 +158,16 @@
         self.splash = Image.new("RGB",(320,240),"black")
         self.display.ShowImage(self.splash)
     #显示图片
     '''
     图片的大小为320*240,jpg格式
     '''
     def lcd_picture(self,filename,x=0,y=0):
-        image = Image.open(filename)
+        path="/home/pi/xgoPictures/"
+        image = Image.open(path+filename)
         self.splash.paste(image,(x,y))
         self.display.ShowImage(self.splash)
     #显示文字
     '''
     x1,y1为初始点坐标,content为内容
     '''
     def lcd_text(self,x,y,content,color="WHITE",fontsize=15):
@@ -200,26 +201,29 @@
             time.sleep(0.02)
             return(not last_state_d)
     #speaker
     '''
     filename 文件名 字符串
     '''
     def xgoSpeaker(self,filename):
-        os.system("mplayer"+" "+filename)
+        path="/home/pi/xgoMusic/"
+        os.system("mplayer"+" "+path+filename)
 
     def xgoVedioAudio(self,filename):
-        time.sleep(0.1)  #音画速度同步了 但是时间轴可能不同步 这里调试一下
-        cmd="sudo mplayer "+filename+" -novideo"
+        path="/home/pi/xgoVideos/"
+        time.sleep(0.2)  #音画速度同步了 但是时间轴可能不同步 这里调试一下
+        cmd="sudo mplayer "+path+filename+" -novideo"
         os.system(cmd)
 
     def xgoVedio(self,filename):
+        path="/home/pi/xgoVideos/"
         x=threading.Thread(target=self.xgoVedioAudio,args=(filename,))
         x.start()
         global counter
-        video=cv2.VideoCapture(filename)
+        video=cv2.VideoCapture(path+filename)
         fps = video.get(cv2.CAP_PROP_FPS) 
         print(fps)
         init_time=time.time()
         counter=0
         while True:
             grabbed, dst = video.read()
             b,g,r = cv2.split(dst)
@@ -239,21 +243,22 @@
         
     #audio_record
     '''
     filename 文件名 字符串
     seconds 录制时间S 字符串
     '''
     def xgoAudioRecord(self,filename="record",seconds=5):
+        path="/home/pi/xgoMusic/"
         command1 = "sudo arecord -d"
         command2 = "-f S32_LE -r 16000 -c 1 -t wav"
-        cmd=command1+" "+str(seconds)+" "+command2+" "+filename+".wav"
+        cmd=command1+" "+str(seconds)+" "+command2+" "+path+filename+".wav"
         print(cmd)
         os.system(cmd)
 
-    def cameraOn(self,switch):
+    def xgoCamera(self,switch):
         global camera_still
         if switch:
             self.open_camera()
             self.camera_still=True
             t = threading.Thread(target=self.camera_mode)  
             t.start() 
         else:
@@ -271,22 +276,23 @@
             image = cv2.flip(image,1)
             imgok = Image.fromarray(image)
             self.display.ShowImage(imgok)
             if not self.camera_still:
                 break
 
     def xgoVedioRecord(self,filename="record",seconds=5):
+        path="/home/pi/xgoVideos/"
         self.camera_still=False
         time.sleep(0.6)
         self.open_camera()
         FPS=15
         fourcc = cv2.VideoWriter_fourcc(*'mp4v')
         width = int(self.cap.get(cv2.CAP_PROP_FRAME_WIDTH))
         height = int(self.cap.get(cv2.CAP_PROP_FRAME_HEIGHT))
-        videoWrite = cv2.VideoWriter(filename+'.mp4', fourcc, FPS, (width,height))
+        videoWrite = cv2.VideoWriter(path+filename+'.mp4', fourcc, FPS, (width,height))
         starttime=time.time()
         while 1:
             print('recording...')
             ret, image = self.cap.read()
             if not ret:
                 break
             videoWrite.write(image)
@@ -294,33 +300,34 @@
             image = cv2.merge((r,g,b))
             image = cv2.flip(image,1)
             imgok = Image.fromarray(image)
             self.display.ShowImage(imgok)
             if time.time()-starttime>seconds:
                 break
         print('recording done')
-        self.cameraOn(True)
+        self.xgoCamera(True)
         videoWrite.release()
 
-    def xgoTakePhoto(self,filename="photo.jpg"):
+    def xgoTakePhoto(self,filename="photo"):
+        path="/home/pi/xgoPictures/"
         self.camera_still=False
         time.sleep(0.6)
         self.open_camera()
         success,image = self.cap.read()
         if not success:
             print("Ignoring empty camera frame")
         b,g,r = cv2.split(image)
         image = cv2.merge((r,g,b))
         image = cv2.flip(image,1)
         imgok = Image.fromarray(image)
         self.display.ShowImage(imgok)
-        cv2.imwrite(filename+'.jpg',image)
+        cv2.imwrite(path+filename+'.jpg',image)
         print('photo writed!')
         time.sleep(0.7)
-        self.cameraOn(True)
+        self.xgoCamera(True)
 
 
     '''
     开启摄像头  A键拍照 B键录像 C键退出
     '''
     def camera(self,filename="camera"):
         font = ImageFont.truetype("/home/pi/model/msyh.ttc",20)
```

### Comparing `xgo-pythonlib-0.1.4/xgolib/__init__.py` & `xgo-pythonlib-0.1.5/xgolib/__init__.py`

 * *Files identical despite different names*

### Comparing `xgo-pythonlib-0.1.4/xgoscreen/LCD_2inch.py` & `xgo-pythonlib-0.1.5/xgoscreen/LCD_2inch.py`

 * *Files identical despite different names*

### Comparing `xgo-pythonlib-0.1.4/xgoscreen/lcdconfig.py` & `xgo-pythonlib-0.1.5/xgoscreen/lcdconfig.py`

 * *Files identical despite different names*

