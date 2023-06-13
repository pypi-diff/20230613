# Comparing `tmp/zdxtools-0.0.8.tar.gz` & `tmp/zdxtools-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "F:\python\pyqt5\pypi_update\dist\tmpnlq366ng\zdxtools-0.0.8.tar", last modified: Tue Jun 28 23:10:07 2022, max compression
+gzip compressed data, was "F:\python\pyqt5\pypi_update\dist\tmpv0zh9sdg\zdxtools-0.0.9.tar", last modified: Mon Jul  4 02:15:11 2022, max compression
```

## Comparing `zdxtools-0.0.8.tar` & `zdxtools-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2022-06-28 23:10:07.988790 zdxtools-0.0.8/
--rw-rw-rw-   0        0        0     1091 2022-06-17 14:49:43.000000 zdxtools-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      685 2022-06-28 23:10:07.989790 zdxtools-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      174 2022-06-17 14:49:43.000000 zdxtools-0.0.8/README.md
--rw-rw-rw-   0        0        0       86 2022-06-17 14:49:43.000000 zdxtools-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-06-28 23:10:07.990790 zdxtools-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      926 2022-06-28 23:09:42.000000 zdxtools-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2022-06-28 23:10:07.928777 zdxtools-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2022-06-28 23:10:07.954781 zdxtools-0.0.8/src/zdxtools/
--rw-rw-rw-   0        0        0        0 2022-04-01 16:49:03.000000 zdxtools-0.0.8/src/zdxtools/__init__.py
--rw-rw-rw-   0        0        0    13567 2022-04-01 16:43:31.000000 zdxtools-0.0.8/src/zdxtools/dx_tools.py
--rw-rw-rw-   0        0        0      926 2022-06-17 15:48:12.000000 zdxtools-0.0.8/src/zdxtools/setup.py
-drwxrwxrwx   0        0        0        0 2022-06-28 23:10:07.985788 zdxtools-0.0.8/src/zdxtools/winrar/
--rw-rw-rw-   0        0        0        0 2022-06-28 22:48:30.000000 zdxtools-0.0.8/src/zdxtools/winrar/__init__.py
--rw-rw-rw-   0        0        0       34 2022-05-30 07:53:04.000000 zdxtools-0.0.8/src/zdxtools/winrar/comment.txt
--rw-rw-rw-   0        0        0       35 2022-05-30 09:57:48.000000 zdxtools-0.0.8/src/zdxtools/winrar/comment_card.txt
--rw-rw-rw-   0        0        0    12505 2022-06-28 23:07:55.000000 zdxtools-0.0.8/src/zdxtools/winrar/winrar_yasuo.py
--rw-rw-rw-   0        0        0      920 2022-06-28 22:29:15.000000 zdxtools-0.0.8/src/zdxtools/winrar/winrar_yasuo_setting.py
-drwxrwxrwx   0        0        0        0 2022-06-28 23:10:07.969785 zdxtools-0.0.8/src/zdxtools.egg-info/
--rw-rw-rw-   0        0        0      685 2022-06-28 23:10:07.000000 zdxtools-0.0.8/src/zdxtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      448 2022-06-28 23:10:07.000000 zdxtools-0.0.8/src/zdxtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-28 23:10:07.000000 zdxtools-0.0.8/src/zdxtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2022-06-28 23:10:07.000000 zdxtools-0.0.8/src/zdxtools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-07-04 02:15:11.931136 zdxtools-0.0.9/
+-rw-rw-rw-   0        0        0     1091 2022-06-17 14:49:43.000000 zdxtools-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      685 2022-07-04 02:15:11.931136 zdxtools-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2022-06-17 14:49:43.000000 zdxtools-0.0.9/README.md
+-rw-rw-rw-   0        0        0       86 2022-06-17 14:49:43.000000 zdxtools-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2022-07-04 02:15:11.932136 zdxtools-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      926 2022-07-04 02:10:11.000000 zdxtools-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2022-07-04 02:15:11.874123 zdxtools-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2022-07-04 02:15:11.901130 zdxtools-0.0.9/src/zdxtools/
+-rw-rw-rw-   0        0        0        0 2022-04-01 16:49:03.000000 zdxtools-0.0.9/src/zdxtools/__init__.py
+-rw-rw-rw-   0        0        0    13567 2022-04-01 16:43:31.000000 zdxtools-0.0.9/src/zdxtools/dx_tools.py
+-rw-rw-rw-   0        0        0      926 2022-07-04 02:09:57.000000 zdxtools-0.0.9/src/zdxtools/setup.py
+drwxrwxrwx   0        0        0        0 2022-07-04 02:15:11.927135 zdxtools-0.0.9/src/zdxtools/winrar/
+-rw-rw-rw-   0        0        0        0 2022-06-28 22:48:30.000000 zdxtools-0.0.9/src/zdxtools/winrar/__init__.py
+-rw-rw-rw-   0        0        0       34 2022-05-30 07:53:04.000000 zdxtools-0.0.9/src/zdxtools/winrar/comment.txt
+-rw-rw-rw-   0        0        0       35 2022-05-30 09:57:48.000000 zdxtools-0.0.9/src/zdxtools/winrar/comment_card.txt
+-rw-rw-rw-   0        0        0    12624 2022-06-30 01:14:27.000000 zdxtools-0.0.9/src/zdxtools/winrar/winrar_yasuo.py
+-rw-rw-rw-   0        0        0     1059 2022-06-30 01:13:48.000000 zdxtools-0.0.9/src/zdxtools/winrar/winrar_yasuo_setting.py
+drwxrwxrwx   0        0        0        0 2022-07-04 02:15:11.913133 zdxtools-0.0.9/src/zdxtools.egg-info/
+-rw-rw-rw-   0        0        0      685 2022-07-04 02:15:11.000000 zdxtools-0.0.9/src/zdxtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      448 2022-07-04 02:15:11.000000 zdxtools-0.0.9/src/zdxtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-07-04 02:15:11.000000 zdxtools-0.0.9/src/zdxtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2022-07-04 02:15:11.000000 zdxtools-0.0.9/src/zdxtools.egg-info/top_level.txt
```

### Comparing `zdxtools-0.0.8/LICENSE` & `zdxtools-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `zdxtools-0.0.8/setup.py` & `zdxtools-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="zdxtools",
-    version="0.0.8",
+    version="0.0.9",
     author="zhou",
     author_email="1057129097@qq.com",
     description="来自21世纪最伟大的科学家",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pypa/sampleproject",
     project_urls={
```

### Comparing `zdxtools-0.0.8/src/zdxtools/dx_tools.py` & `zdxtools-0.0.9/src/zdxtools/dx_tools.py`

 * *Files identical despite different names*

### Comparing `zdxtools-0.0.8/src/zdxtools/setup.py` & `zdxtools-0.0.9/src/zdxtools/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="zdxtools",
-    version="0.0.6",
+    version="0.0.9",
     author="zhou",
     author_email="1057129097@qq.com",
     description="来自21世纪最伟大的科学家",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pypa/sampleproject",
     project_urls={
```

### Comparing `zdxtools-0.0.8/src/zdxtools/winrar/winrar_yasuo.py` & `zdxtools-0.0.9/src/zdxtools/winrar/winrar_yasuo.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,19 +64,22 @@
     @classmethod
     def choice_zijieya_text(cls,f):
 
         if setting.zijieya_text:
             n = 1
             print('请选择默认要打开的网址')
             for i in setting.zijieya_text:
-                newpath = os.path.join(os.path.dirname(__file__),i)
+                newpath = os.path.join(os.path.dirname(__file__),i[0])
                 print(f'''{n} {zuj.get_url(newpath)}''')
                 n += 1
             choice = int(input('请输入编号：'))-1
-            setting.zijieya_text = setting.zijieya_text[choice]
+            peizhi = setting.zijieya_text[choice]
+            if len(peizhi)>1 :
+                setting.other_add_file = peizhi[1]
+            setting.zijieya_text = peizhi[0]
         def inner(*args, **kwargs):  # *代表聚合
             ret = f(*args, **kwargs)  # *代表打散
             return ret
         return inner
 
 #压缩模式0，先压缩，再添加附加文件
 def winrar_plyasuo(path):
```

### Comparing `zdxtools-0.0.8/src/zdxtools/winrar/winrar_yasuo_setting.py` & `zdxtools-0.0.9/src/zdxtools/winrar/winrar_yasuo_setting.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,26 +16,33 @@
 yasuo_after_delet = True
 #压缩文件输出路径
 # outinput_path = None
 
 #随机生成文件，防止压缩包md5相同
 suijishu = False
 
+other_add_file = [
+    r'F:\python\pyqt5\manager\winrar_yasuo\fujia\更多游戏下载.url',
+]
+other_add_file1= [
+    r'F:\python\pyqt5\manager\winrar_yasuo\path\更多人物卡下载.url',
+]
+
+
+
 #自解压选择
 zijieya_text = [
-    ('comment.txt'),
-    ('comment_card.txt')
+    ('comment.txt',other_add_file),
+    ('comment_card.txt',other_add_file1)
 ]
 
 
 #要额外附加的宣传文件
 # other_add_file = [
 #     r'F:\python\pyqt5\tools\fujia\更多游戏下载.url',
 #
 # ]
-other_add_file = [
-    r'F:\python\pyqt5\manager\winrar_yasuo\fujia\更多游戏下载.url',
-]
+
 
 if __name__ == '__main__':
     import os
     print(os.path.dirname(other_add_file[0]))
```

