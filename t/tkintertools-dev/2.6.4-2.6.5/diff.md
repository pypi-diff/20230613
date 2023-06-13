# Comparing `tmp/tkintertools-dev-2.6.4.tar.gz` & `tmp/tkintertools-dev-2.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkintertools-dev-2.6.4.tar", last modified: Sat Jun 10 16:31:18 2023, max compression
+gzip compressed data, was "tkintertools-dev-2.6.5.tar", last modified: Tue Jun 13 06:31:05 2023, max compression
```

## Comparing `tkintertools-dev-2.6.4.tar` & `tkintertools-dev-2.6.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 16:31:18.703807 tkintertools-dev-2.6.4/
--rw-rw-rw-   0        0        0     7548 2023-05-27 20:59:02.000000 tkintertools-dev-2.6.4/LICENSE
--rw-rw-rw-   0        0        0    28017 2023-06-10 16:31:18.701772 tkintertools-dev-2.6.4/PKG-INFO
--rw-rw-rw-   0        0        0    27512 2023-06-10 16:21:28.000000 tkintertools-dev-2.6.4/README.md
--rw-rw-rw-   0        0        0       42 2023-06-10 16:31:18.704774 tkintertools-dev-2.6.4/setup.cfg
--rw-rw-rw-   0        0        0     1216 2023-06-10 06:50:22.000000 tkintertools-dev-2.6.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-10 16:31:18.690328 tkintertools-dev-2.6.4/tkintertools/
--rw-rw-rw-   0        0        0     2352 2023-06-10 12:13:26.000000 tkintertools-dev-2.6.4/tkintertools/__init__.py
--rw-rw-rw-   0        0        0    62557 2023-06-10 12:15:00.000000 tkintertools-dev-2.6.4/tkintertools/__main__.py
--rw-rw-rw-   0        0        0     2066 2023-06-10 13:59:58.000000 tkintertools-dev-2.6.4/tkintertools/constants.py
--rw-rw-rw-   0        0        0    18105 2023-06-10 15:12:51.000000 tkintertools-dev-2.6.4/tkintertools/tools_3d.py
-drwxrwxrwx   0        0        0        0 2023-06-10 16:31:18.700770 tkintertools-dev-2.6.4/tkintertools_dev.egg-info/
--rw-rw-rw-   0        0        0    28017 2023-06-10 16:31:18.000000 tkintertools-dev-2.6.4/tkintertools_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2023-06-10 16:31:18.000000 tkintertools-dev-2.6.4/tkintertools_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 16:31:18.000000 tkintertools-dev-2.6.4/tkintertools_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-10 16:31:18.000000 tkintertools-dev-2.6.4/tkintertools_dev.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 06:31:05.390830 tkintertools-dev-2.6.5/
+-rw-rw-rw-   0        0        0     9257 2023-06-12 07:55:24.000000 tkintertools-dev-2.6.5/LICENSE
+-rw-rw-rw-   0        0        0    29158 2023-06-13 06:31:05.388835 tkintertools-dev-2.6.5/PKG-INFO
+-rw-rw-rw-   0        0        0    28593 2023-06-13 06:28:48.000000 tkintertools-dev-2.6.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-13 06:31:05.390830 tkintertools-dev-2.6.5/setup.cfg
+-rw-rw-rw-   0        0        0     1294 2023-06-13 06:30:22.000000 tkintertools-dev-2.6.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 06:31:05.370833 tkintertools-dev-2.6.5/tkintertools/
+-rw-rw-rw-   0        0        0     2845 2023-06-12 15:57:49.000000 tkintertools-dev-2.6.5/tkintertools/__init__.py
+-rw-rw-rw-   0        0        0    62557 2023-06-10 12:15:00.000000 tkintertools-dev-2.6.5/tkintertools/__main__.py
+-rw-rw-rw-   0        0        0     2066 2023-06-10 13:59:58.000000 tkintertools-dev-2.6.5/tkintertools/constants.py
+-rw-rw-rw-   0        0        0    21168 2023-06-13 06:16:52.000000 tkintertools-dev-2.6.5/tkintertools/tools_3d.py
+drwxrwxrwx   0        0        0        0 2023-06-13 06:31:05.384833 tkintertools-dev-2.6.5/tkintertools_dev.egg-info/
+-rw-rw-rw-   0        0        0    29158 2023-06-13 06:31:05.000000 tkintertools-dev-2.6.5/tkintertools_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-06-13 06:31:05.000000 tkintertools-dev-2.6.5/tkintertools_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 06:31:05.000000 tkintertools-dev-2.6.5/tkintertools_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-13 06:31:05.000000 tkintertools-dev-2.6.5/tkintertools_dev.egg-info/top_level.txt
```

### Comparing `tkintertools-dev-2.6.4/LICENSE` & `tkintertools-dev-2.6.5/LICENSE`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-木兰宽松许可证, 第2版
+木兰宽松许可证, 第2版 木兰宽松许可证， 第2版
 
 2020年1月 http://license.coscl.org.cn/MulanPSL2
 
 您对"软件"的复制、使用、修改及分发受木兰宽松许可证，第2版（"本许可证"）的如下条款的约束：
 
    0. 定义
 
@@ -38,15 +38,45 @@
 
    6. 语言
 
    "本许可证"以中英文双语表述，中英文版本具有同等法律效力。如果中英文版本存在任何冲突不一致，以中文版为准。
 
 条款结束
 
-Mulan Permissive Software License，Version 2 (Mulan PSL v2)
+如何将木兰宽松许可证，第2版，应用到您的软件
+
+如果您希望将木兰宽松许可证，第2版，应用到您的新软件，为了方便接收者查阅，建议您完成如下三步：
+
+   1， 请您补充如下声明中的空白，包括软件名、软件的首次发表年份以及您作为版权人的名字；
+
+   2， 请您在软件包的一级目录下创建以"LICENSE"为名的文件，将整个许可证文本放入该文件中；
+
+   3， 请将如下声明文本放入每个源文件的头部注释中。
+
+Copyright (c) 2022 小康2022
+
+tkintertools is licensed under Mulan PSL v2.
+
+You can use this software according to the terms and conditions of the Mulan PSL v2.
+
+You may obtain a copy of Mulan PSL v2 at:
+
+http://license.coscl.org.cn/MulanPSL2
+
+THIS SOFTWARE IS PROVIDED ON AN "AS IS" BASIS, WITHOUT WARRANTIES OF ANY KIND,
+
+EITHER EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO NON-INFRINGEMENT,
+
+MERCHANTABILITY OR FIT FOR A PARTICULAR PURPOSE.
+
+See the Mulan PSL v2 for more details.
+
+
+
+Mulan Permissive Software License，Version 2 Mulan Permissive Software License，Version 2 (Mulan PSL v2)
 
 January 2020 http://license.coscl.org.cn/MulanPSL2
 
 Your reproduction, use, modification and distribution of the Software shall be subject to Mulan PSL v2 (this License) with the following terms and conditions:
 
    0. Definition
 
@@ -82,26 +112,34 @@
 
    6. Language
 
    THIS LICENSE IS WRITTEN IN BOTH CHINESE AND ENGLISH, AND THE CHINESE VERSION AND ENGLISH VERSION SHALL HAVE THE SAME LEGAL EFFECT. IN THE CASE OF DIVERGENCE BETWEEN THE CHINESE AND ENGLISH VERSIONS, THE CHINESE VERSION SHALL PREVAIL.
 
 END OF THE TERMS AND CONDITIONS
 
-=======================================================================================
+How to Apply the Mulan Permissive Software License，Version 2 (Mulan PSL v2) to Your Software
+
+To apply the Mulan PSL v2 to your work, for easy identification by recipients, you are suggested to complete following three steps:
+
+   i. Fill in the blanks in following statement, including insert your software name, the year of the first publication of your software, and your name identified as the copyright owner;
+
+   ii. Create a file named "LICENSE" which contains the whole context of this License in the first directory of your software package;
+
+   iii. Attach the statement to the appropriate annotated syntax at the beginning of each source file.
 
-Copyright (c) 2022-2023 小康2022
+Copyright (c) 2022 Xiaokang2022
 
-[tkintertools] is licensed under Mulan PSL v2.
+tkintertools is licensed under Mulan PSL v2.
 
 You can use this software according to the terms and conditions of the Mulan PSL v2.
 
 You may obtain a copy of Mulan PSL v2 at:
 
 http://license.coscl.org.cn/MulanPSL2
 
 THIS SOFTWARE IS PROVIDED ON AN "AS IS" BASIS, WITHOUT WARRANTIES OF ANY KIND,
 
 EITHER EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO NON-INFRINGEMENT,
 
 MERCHANTABILITY OR FIT FOR A PARTICULAR PURPOSE.
 
-See the Mulan PSL v2 for more details. 
+See the Mulan PSL v2 for more details.
```

### Comparing `tkintertools-dev-2.6.4/PKG-INFO` & `tkintertools-dev-2.6.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,98 +1,120 @@
 Metadata-Version: 2.1
 Name: tkintertools-dev
-Version: 2.6.4
+Version: 2.6.5
 Summary: An auxiliary module of the tkinder module
 Home-page: https://github.com/Xiaokang2022/tkintertools
 Author: Xiaokang2022
 Author-email: 2951256653@qq.com
 License: MulanPSL-2.0
+Keywords: tkinter,tkintertools,GUI
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
 Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
     <h1>🚀tkintertools🚀</h1>
-    <p><img height="120px" alt="logo.png"
-        src="tkintertools.png" />
+    <p><img height="128px" alt="logo.png" src="tkt.png" /></p>
+    <p>
+    The <code>tkintertools</code> module is an auxiliary module of the <code>tkinter</code> module
+    <br />
+    <code>tkintertools</code> 模块是 <code>tkinter</code> 模块的辅助模块
     </p>
-    <p>The <code>tkintertools</code> module is an auxiliary module of the <code>tkinter</code> module</p>
-    <p><code>tkintertools</code> 模块是 <code>tkinter</code> 模块的辅助模块</p>
     <p>
         <a href="tkintertools/__init__.py">
-            <img src="https://img.shields.io/badge/Version-2.6.4(dev)-blue" alt="latest version" />
+            <img src="https://img.shields.io/badge/Version-2.6.5(dev)-blue" alt="latest version" />
         </a>
         <a href="LICENSE">
             <img src="https://img.shields.io/badge/License-Mulan PSL v2-green" alt="License" />
         </a>
         <a href="CHANGELOG.md">
-            <img src="https://img.shields.io/badge/ChangeLog-2023/06/11-orange" alt="ChangeLog" />
+            <img src="https://img.shields.io/badge/ChangeLog-2023/06/13-orange" alt="ChangeLog" />
         </a>
         <a href="TODO.md">
-            <img src="https://img.shields.io/badge/ToDos-14-yellow" alt="ToDos" />
+            <img src="https://img.shields.io/badge/ToDo-14-yellow?logo=cachet" alt="ToDos" />
         </a>
         <a href="https://pypistats.org/packages/tkintertools">
-            <img src="https://img.shields.io/badge/Downloads-4k-purple" alt="Downloads" />
+            <img src="https://img.shields.io/badge/Download-4k-purple?logo=pypi" alt="Downloads" />
         </a>
-    </p>
-    <p>
+        <br />
         <a href="mailto:2951256653@qq.com">
             <img src="https://img.shields.io/badge/Email-2951256653@qq.com-cyan" alt="Email" />
         </a>
-        <a href="https://xiaokang2022.blog.csdn.net">
-            <img src="https://img.shields.io/badge/Blog-小康2022@CSDN-red" alt="Blog" />
-        </a>
         <a href="https://github.com/Xiaokang2022">
             <img src="https://img.shields.io/badge/Author-小康2022-white" alt="Author" />
         </a>
+        <a href="https://xiaokang2022.blog.csdn.net">
+            <img src="https://img.shields.io/badge/Blog-小康2022@CSDN-red" alt="Blog" />
+        </a>
     </p>
 </div>
 
-Installation/模块安装
---------------------
+Install/模块安装
+---------------
 
 ### Stable version/稳定版本
 
-* Version/版本 : 2.6.3
-* Release Date/发布日期 : 2023/06/07
-
-```
-pip install tkintertools==2.6.3
-或者
-pip install tkintertools
-```
+* Version/版本 : 2.6.4
+* Release Date/发布日期 : 2023/06/12
 
 这个是目前的最新稳定版，比较稳定，bug （可能）没有那么多，推荐使用这个。  
 关于稳定版有 Issue 的话，我会去查看并尝试解决 Issue。
 
-### Development version/开发版本
-
-* Version/版本 : 2.6.4
-* Release Date/发布日期 : 2023/06/11
-
 ```
-pip install tkintertools-dev==2.6.4
-或者
-pip install tkintertools-dev
+pip install tkintertools==2.6.4
 ```
 
+### Development version/开发版本
+
+* Version/版本 : 2.6.5
+* Release Date/发布日期 : 2023/06/13
+
 这个是我正在开发的版本，可能有新功能，bug 也可能会比较多，但也可能会比原来的版本更加稳定。  
 大家可以在 Issue 中提出一些建议，我会适当采纳一些并在开发版本中更改或实现。
 
-**特别注意**
+```
+pip install tkintertools-dev==2.6.5
+```
+
+**Attention/特别注意**
 * 开发版仅作示例，各函数或类的API并非最终确定结果，直接使用开发版可能导致后续无法与正式版兼容！
 * 若要使用开发版，请先卸载正式版后再进行pip安装，再次使用正式版时也是一样，先卸载开发版再安装正式版！
-* 需要 **Python3.8** 及更高版本才能运行 tkintertools！
+
+### Environmental requirements/环境需求
+
+没有任何额外的依赖包（除了tkinter），但只支持以下 Python 版本:
+
+![Python3.8](https://img.shields.io/badge/Python-3.8.*-blue?logo=python)
+![Python3.9](https://img.shields.io/badge/Python-3.9.*-blue?logo=python)
+![Python3.10](https://img.shields.io/badge/Python-3.10.*-blue?logo=python)
+![Python3.11](https://img.shields.io/badge/Python-3.11.*-blue?logo=python)
+![Python3.12](https://img.shields.io/badge/Python-3.12.*-blue?logo=python)
+
+可能在某些操作系统上也可运行，但目前以下操作系统已经测试通过:
+
+![Windows10](https://img.shields.io/badge/Windows-10-green?logo=windows)
+![Windows11](https://img.shields.io/badge/Windows-11-green?logo=windows11)
+![Ubuntu22.04](https://img.shields.io/badge/Ubuntu-22.04-green?logo=ubuntu)
 
 <a name="news">News/最新功能</a>
 ------------
 
-最新版的 tkintertools **开发版**(2.6.4-dev)新增了对3d几何体空间位置排序的支持，使得几何体不再只有粗略的线条，而拥有丰富的颜色。
+最新开发版（2.6.5-dev）新内容:
+
+- [X] 子模块`tools_3d`新增类`Space`可以直接提供对3D对象进行平移、旋转和缩放等操作的功能
+- [X] 修复了类`Cuboid`和类`Tetrahedron`没有将实例添加到父类`Canvas_3D`的bug
+- [X] 修复了当3D对象出现在相机位置后面时会显示错误的bug
+- [X] 修复了部分错误的类型提示
+
+最新稳定版（2.6.4）新内容:
+
+新增了对3d几何体空间位置排序的支持，使得几何体不再只有粗略的线条，而拥有丰富的颜色。
 
 在 Windows 系统下运行下面的示例程序时，其拥有以下功能：
 * 按住鼠标左键拖动可以旋转这多个几何体；
 * 按住鼠标右键拖动可以移动这些几何体在空间中的位置；
 * 按“=”和“-”键分别可以放大和缩小几何体的大小；
 * 滚动鼠标中键可以放大和缩小画面。
```

#### html2text {}

```diff
@@ -1,39 +1,55 @@
-Metadata-Version: 2.1 Name: tkintertools-dev Version: 2.6.4 Summary: An
+Metadata-Version: 2.1 Name: tkintertools-dev Version: 2.6.5 Summary: An
 auxiliary module of the tkinder module Home-page: https://github.com/
 Xiaokang2022/tkintertools Author: Xiaokang2022 Author-email: 2951256653@qq.com
-License: MulanPSL-2.0 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Mulan Permissive Software License v2
-(MulanPSL-2.0) Classifier: Operating System :: OS Independent Description-
-Content-Type: text/markdown License-File: LICENSE
+License: MulanPSL-2.0 Keywords: tkinter,tkintertools,GUI Classifier:
+Programming Language :: Python :: 3 Classifier: License :: OSI Approved ::
+Mulan Permissive Software License v2 (MulanPSL-2.0) Classifier: Operating
+System :: OS Independent Requires-Python: >=3.8 Description-Content-Type: text/
+markdown License-File: LICENSE
                       ****** ðtkintertoolsð ******
                                   [logo.png]
      The tkintertools module is an auxiliary module of the tkinter module
              tkintertools æ¨¡åæ¯ tkinter æ¨¡åçè¾å©æ¨¡å
           [latest_version] [License] [ChangeLog] [ToDos] [Downloads]
-                            [Email] [Blog] [Author]
-Installation/æ¨¡åå®è£ -------------------- ### Stable version/ç¨³å®çæ¬
-* Version/çæ¬ : 2.6.3 * Release Date/åå¸æ¥æ : 2023/06/07 ``` pip
-install tkintertools==2.6.3 æè pip install tkintertools ```
+                            [Email] [Author] [Blog]
+Install/æ¨¡åå®è£ --------------- ### Stable version/ç¨³å®çæ¬ * Version/
+çæ¬ : 2.6.4 * Release Date/åå¸æ¥æ : 2023/06/12
 è¿ä¸ªæ¯ç®åçææ°ç¨³å®çï¼æ¯è¾ç¨³å®ï¼bug
 ï¼å¯è½ï¼æ²¡æé£ä¹å¤ï¼æ¨èä½¿ç¨è¿ä¸ªã å³äºç¨³å®çæ Issue
-çè¯ï¼æä¼å»æ¥çå¹¶å°è¯è§£å³ Issueã ### Development version/
-å¼åçæ¬ * Version/çæ¬ : 2.6.4 * Release Date/åå¸æ¥æ : 2023/06/11
-``` pip install tkintertools-dev==2.6.4 æè pip install tkintertools-dev ```
+çè¯ï¼æä¼å»æ¥çå¹¶å°è¯è§£å³ Issueã ``` pip install
+tkintertools==2.6.4 ``` ### Development version/å¼åçæ¬ * Version/çæ¬ :
+2.6.5 * Release Date/åå¸æ¥æ : 2023/06/13
 è¿ä¸ªæ¯ææ­£å¨å¼åççæ¬ï¼å¯è½ææ°åè½ï¼bug
 ä¹å¯è½ä¼æ¯è¾å¤ï¼ä½ä¹å¯è½ä¼æ¯åæ¥ççæ¬æ´å ç¨³å®ã
 å¤§å®¶å¯ä»¥å¨ Issue
 ä¸­æåºä¸äºå»ºè®®ï¼æä¼éå½éçº³ä¸äºå¹¶å¨å¼åçæ¬ä¸­æ´æ¹æå®ç°ã
-**ç¹å«æ³¨æ** *
+``` pip install tkintertools-dev==2.6.5 ``` **Attention/ç¹å«æ³¨æ** *
 å¼åçä»ä½ç¤ºä¾ï¼åå½æ°æç±»çAPIå¹¶éæç»ç¡®å®ç»æï¼ç´æ¥ä½¿ç¨å¼åçå¯è½å¯¼è´åç»­æ æ³ä¸æ­£å¼çå¼å®¹ï¼
 *
 è¥è¦ä½¿ç¨å¼åçï¼è¯·åå¸è½½æ­£å¼çååè¿è¡pipå®è£ï¼åæ¬¡ä½¿ç¨æ­£å¼çæ¶ä¹æ¯ä¸æ ·ï¼åå¸è½½å¼åçåå®è£æ­£å¼çï¼
-* éè¦ **Python3.8** åæ´é«çæ¬æè½è¿è¡ tkintertoolsï¼ News/
-ææ°åè½ ------------ ææ°çç tkintertools **å¼åç**(2.6.4-
-dev)æ°å¢äºå¯¹3då ä½ä½ç©ºé´ä½ç½®æåºçæ¯æï¼ä½¿å¾å ä½ä½ä¸ååªæç²ç¥ççº¿æ¡ï¼èæ¥æä¸°å¯çé¢è²ã
+### Environmental requirements/ç¯å¢éæ±
+æ²¡æä»»ä½é¢å¤çä¾èµåï¼é¤äºtkinterï¼ï¼ä½åªæ¯æä»¥ä¸ Python
+çæ¬: ![Python3.8](https://img.shields.io/badge/Python-3.8.*-
+blue?logo=python) ![Python3.9](https://img.shields.io/badge/Python-3.9.*-
+blue?logo=python) ![Python3.10](https://img.shields.io/badge/Python-3.10.*-
+blue?logo=python) ![Python3.11](https://img.shields.io/badge/Python-3.11.*-
+blue?logo=python) ![Python3.12](https://img.shields.io/badge/Python-3.12.*-
+blue?logo=python)
+å¯è½å¨æäºæä½ç³»ç»ä¸ä¹å¯è¿è¡ï¼ä½ç®åä»¥ä¸æä½ç³»ç»å·²ç»æµè¯éè¿:
+![Windows10](https://img.shields.io/badge/Windows-10-green?logo=windows) !
+[Windows11](https://img.shields.io/badge/Windows-11-green?logo=windows11) !
+[Ubuntu22.04](https://img.shields.io/badge/Ubuntu-22.04-green?logo=ubuntu)
+News/ææ°åè½ ------------ ææ°å¼åçï¼2.6.5-devï¼æ°åå®¹: - [X]
+å­æ¨¡å`tools_3d`æ°å¢ç±»`Space`å¯ä»¥ç´æ¥æä¾å¯¹3Då¯¹è±¡è¿è¡å¹³ç§»ãæè½¬åç¼©æ¾ç­æä½çåè½
+- [X]
+ä¿®å¤äºç±»`Cuboid`åç±»`Tetrahedron`æ²¡æå°å®ä¾æ·»å å°ç¶ç±»`Canvas_3D`çbug
+- [X] ä¿®å¤äºå½3Då¯¹è±¡åºç°å¨ç¸æºä½ç½®åé¢æ¶ä¼æ¾ç¤ºéè¯¯çbug -
+[X] ä¿®å¤äºé¨åéè¯¯çç±»åæç¤º ææ°ç¨³å®çï¼2.6.4ï¼æ°åå®¹:
+æ°å¢äºå¯¹3då ä½ä½ç©ºé´ä½ç½®æåºçæ¯æï¼ä½¿å¾å ä½ä½ä¸ååªæç²ç¥ççº¿æ¡ï¼èæ¥æä¸°å¯çé¢è²ã
 å¨ Windows ç³»ç»ä¸è¿è¡ä¸é¢çç¤ºä¾ç¨åºæ¶ï¼å¶æ¥æä»¥ä¸åè½ï¼
 * æä½é¼ æ å·¦é®æå¨å¯ä»¥æè½¬è¿å¤ä¸ªå ä½ä½ï¼ *
 æä½é¼ æ å³é®æå¨å¯ä»¥ç§»å¨è¿äºå ä½ä½å¨ç©ºé´ä¸­çä½ç½®ï¼ *
 æâ=âåâ-âé®åå«å¯ä»¥æ¾å¤§åç¼©å°å ä½ä½çå¤§å°ï¼ *
 æ»å¨é¼ æ ä¸­é®å¯ä»¥æ¾å¤§åç¼©å°ç»é¢ã
 ä¸é¢æ¯ç¤ºä¾ç¨åºçææå¾ï¼ ![news.png](news.png) æºä»£ç  ```python
 from tkinter import Event import tkintertools as tkt from tkintertools import
```

### Comparing `tkintertools-dev-2.6.4/README.md` & `tkintertools-dev-2.6.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,84 +1,104 @@
 <div align="center">
     <h1>🚀tkintertools🚀</h1>
-    <p><img height="120px" alt="logo.png"
-        src="tkintertools.png" />
+    <p><img height="128px" alt="logo.png" src="tkt.png" /></p>
+    <p>
+    The <code>tkintertools</code> module is an auxiliary module of the <code>tkinter</code> module
+    <br />
+    <code>tkintertools</code> 模块是 <code>tkinter</code> 模块的辅助模块
     </p>
-    <p>The <code>tkintertools</code> module is an auxiliary module of the <code>tkinter</code> module</p>
-    <p><code>tkintertools</code> 模块是 <code>tkinter</code> 模块的辅助模块</p>
     <p>
         <a href="tkintertools/__init__.py">
-            <img src="https://img.shields.io/badge/Version-2.6.4(dev)-blue" alt="latest version" />
+            <img src="https://img.shields.io/badge/Version-2.6.5(dev)-blue" alt="latest version" />
         </a>
         <a href="LICENSE">
             <img src="https://img.shields.io/badge/License-Mulan PSL v2-green" alt="License" />
         </a>
         <a href="CHANGELOG.md">
-            <img src="https://img.shields.io/badge/ChangeLog-2023/06/11-orange" alt="ChangeLog" />
+            <img src="https://img.shields.io/badge/ChangeLog-2023/06/13-orange" alt="ChangeLog" />
         </a>
         <a href="TODO.md">
-            <img src="https://img.shields.io/badge/ToDos-14-yellow" alt="ToDos" />
+            <img src="https://img.shields.io/badge/ToDo-14-yellow?logo=cachet" alt="ToDos" />
         </a>
         <a href="https://pypistats.org/packages/tkintertools">
-            <img src="https://img.shields.io/badge/Downloads-4k-purple" alt="Downloads" />
+            <img src="https://img.shields.io/badge/Download-4k-purple?logo=pypi" alt="Downloads" />
         </a>
-    </p>
-    <p>
+        <br />
         <a href="mailto:2951256653@qq.com">
             <img src="https://img.shields.io/badge/Email-2951256653@qq.com-cyan" alt="Email" />
         </a>
-        <a href="https://xiaokang2022.blog.csdn.net">
-            <img src="https://img.shields.io/badge/Blog-小康2022@CSDN-red" alt="Blog" />
-        </a>
         <a href="https://github.com/Xiaokang2022">
             <img src="https://img.shields.io/badge/Author-小康2022-white" alt="Author" />
         </a>
+        <a href="https://xiaokang2022.blog.csdn.net">
+            <img src="https://img.shields.io/badge/Blog-小康2022@CSDN-red" alt="Blog" />
+        </a>
     </p>
 </div>
 
-Installation/模块安装
---------------------
+Install/模块安装
+---------------
 
 ### Stable version/稳定版本
 
-* Version/版本 : 2.6.3
-* Release Date/发布日期 : 2023/06/07
-
-```
-pip install tkintertools==2.6.3
-或者
-pip install tkintertools
-```
+* Version/版本 : 2.6.4
+* Release Date/发布日期 : 2023/06/12
 
 这个是目前的最新稳定版，比较稳定，bug （可能）没有那么多，推荐使用这个。  
 关于稳定版有 Issue 的话，我会去查看并尝试解决 Issue。
 
-### Development version/开发版本
-
-* Version/版本 : 2.6.4
-* Release Date/发布日期 : 2023/06/11
-
 ```
-pip install tkintertools-dev==2.6.4
-或者
-pip install tkintertools-dev
+pip install tkintertools==2.6.4
 ```
 
+### Development version/开发版本
+
+* Version/版本 : 2.6.5
+* Release Date/发布日期 : 2023/06/13
+
 这个是我正在开发的版本，可能有新功能，bug 也可能会比较多，但也可能会比原来的版本更加稳定。  
 大家可以在 Issue 中提出一些建议，我会适当采纳一些并在开发版本中更改或实现。
 
-**特别注意**
+```
+pip install tkintertools-dev==2.6.5
+```
+
+**Attention/特别注意**
 * 开发版仅作示例，各函数或类的API并非最终确定结果，直接使用开发版可能导致后续无法与正式版兼容！
 * 若要使用开发版，请先卸载正式版后再进行pip安装，再次使用正式版时也是一样，先卸载开发版再安装正式版！
-* 需要 **Python3.8** 及更高版本才能运行 tkintertools！
+
+### Environmental requirements/环境需求
+
+没有任何额外的依赖包（除了tkinter），但只支持以下 Python 版本:
+
+![Python3.8](https://img.shields.io/badge/Python-3.8.*-blue?logo=python)
+![Python3.9](https://img.shields.io/badge/Python-3.9.*-blue?logo=python)
+![Python3.10](https://img.shields.io/badge/Python-3.10.*-blue?logo=python)
+![Python3.11](https://img.shields.io/badge/Python-3.11.*-blue?logo=python)
+![Python3.12](https://img.shields.io/badge/Python-3.12.*-blue?logo=python)
+
+可能在某些操作系统上也可运行，但目前以下操作系统已经测试通过:
+
+![Windows10](https://img.shields.io/badge/Windows-10-green?logo=windows)
+![Windows11](https://img.shields.io/badge/Windows-11-green?logo=windows11)
+![Ubuntu22.04](https://img.shields.io/badge/Ubuntu-22.04-green?logo=ubuntu)
 
 <a name="news">News/最新功能</a>
 ------------
 
-最新版的 tkintertools **开发版**(2.6.4-dev)新增了对3d几何体空间位置排序的支持，使得几何体不再只有粗略的线条，而拥有丰富的颜色。
+最新开发版（2.6.5-dev）新内容:
+
+- [X] 子模块`tools_3d`新增类`Space`可以直接提供对3D对象进行平移、旋转和缩放等操作的功能
+- [X] 修复了类`Cuboid`和类`Tetrahedron`没有将实例添加到父类`Canvas_3D`的bug
+- [X] 修复了当3D对象出现在相机位置后面时会显示错误的bug
+- [X] 修复了部分错误的类型提示
+
+最新稳定版（2.6.4）新内容:
+
+新增了对3d几何体空间位置排序的支持，使得几何体不再只有粗略的线条，而拥有丰富的颜色。
 
 在 Windows 系统下运行下面的示例程序时，其拥有以下功能：
 * 按住鼠标左键拖动可以旋转这多个几何体；
 * 按住鼠标右键拖动可以移动这些几何体在空间中的位置；
 * 按“=”和“-”键分别可以放大和缩小几何体的大小；
 * 滚动鼠标中键可以放大和缩小画面。
```

#### html2text {}

```diff
@@ -1,32 +1,47 @@
                       ****** ðtkintertoolsð ******
                                   [logo.png]
      The tkintertools module is an auxiliary module of the tkinter module
              tkintertools æ¨¡åæ¯ tkinter æ¨¡åçè¾å©æ¨¡å
           [latest_version] [License] [ChangeLog] [ToDos] [Downloads]
-                            [Email] [Blog] [Author]
-Installation/æ¨¡åå®è£ -------------------- ### Stable version/ç¨³å®çæ¬
-* Version/çæ¬ : 2.6.3 * Release Date/åå¸æ¥æ : 2023/06/07 ``` pip
-install tkintertools==2.6.3 æè pip install tkintertools ```
+                            [Email] [Author] [Blog]
+Install/æ¨¡åå®è£ --------------- ### Stable version/ç¨³å®çæ¬ * Version/
+çæ¬ : 2.6.4 * Release Date/åå¸æ¥æ : 2023/06/12
 è¿ä¸ªæ¯ç®åçææ°ç¨³å®çï¼æ¯è¾ç¨³å®ï¼bug
 ï¼å¯è½ï¼æ²¡æé£ä¹å¤ï¼æ¨èä½¿ç¨è¿ä¸ªã å³äºç¨³å®çæ Issue
-çè¯ï¼æä¼å»æ¥çå¹¶å°è¯è§£å³ Issueã ### Development version/
-å¼åçæ¬ * Version/çæ¬ : 2.6.4 * Release Date/åå¸æ¥æ : 2023/06/11
-``` pip install tkintertools-dev==2.6.4 æè pip install tkintertools-dev ```
+çè¯ï¼æä¼å»æ¥çå¹¶å°è¯è§£å³ Issueã ``` pip install
+tkintertools==2.6.4 ``` ### Development version/å¼åçæ¬ * Version/çæ¬ :
+2.6.5 * Release Date/åå¸æ¥æ : 2023/06/13
 è¿ä¸ªæ¯ææ­£å¨å¼åççæ¬ï¼å¯è½ææ°åè½ï¼bug
 ä¹å¯è½ä¼æ¯è¾å¤ï¼ä½ä¹å¯è½ä¼æ¯åæ¥ççæ¬æ´å ç¨³å®ã
 å¤§å®¶å¯ä»¥å¨ Issue
 ä¸­æåºä¸äºå»ºè®®ï¼æä¼éå½éçº³ä¸äºå¹¶å¨å¼åçæ¬ä¸­æ´æ¹æå®ç°ã
-**ç¹å«æ³¨æ** *
+``` pip install tkintertools-dev==2.6.5 ``` **Attention/ç¹å«æ³¨æ** *
 å¼åçä»ä½ç¤ºä¾ï¼åå½æ°æç±»çAPIå¹¶éæç»ç¡®å®ç»æï¼ç´æ¥ä½¿ç¨å¼åçå¯è½å¯¼è´åç»­æ æ³ä¸æ­£å¼çå¼å®¹ï¼
 *
 è¥è¦ä½¿ç¨å¼åçï¼è¯·åå¸è½½æ­£å¼çååè¿è¡pipå®è£ï¼åæ¬¡ä½¿ç¨æ­£å¼çæ¶ä¹æ¯ä¸æ ·ï¼åå¸è½½å¼åçåå®è£æ­£å¼çï¼
-* éè¦ **Python3.8** åæ´é«çæ¬æè½è¿è¡ tkintertoolsï¼ News/
-ææ°åè½ ------------ ææ°çç tkintertools **å¼åç**(2.6.4-
-dev)æ°å¢äºå¯¹3då ä½ä½ç©ºé´ä½ç½®æåºçæ¯æï¼ä½¿å¾å ä½ä½ä¸ååªæç²ç¥ççº¿æ¡ï¼èæ¥æä¸°å¯çé¢è²ã
+### Environmental requirements/ç¯å¢éæ±
+æ²¡æä»»ä½é¢å¤çä¾èµåï¼é¤äºtkinterï¼ï¼ä½åªæ¯æä»¥ä¸ Python
+çæ¬: ![Python3.8](https://img.shields.io/badge/Python-3.8.*-
+blue?logo=python) ![Python3.9](https://img.shields.io/badge/Python-3.9.*-
+blue?logo=python) ![Python3.10](https://img.shields.io/badge/Python-3.10.*-
+blue?logo=python) ![Python3.11](https://img.shields.io/badge/Python-3.11.*-
+blue?logo=python) ![Python3.12](https://img.shields.io/badge/Python-3.12.*-
+blue?logo=python)
+å¯è½å¨æäºæä½ç³»ç»ä¸ä¹å¯è¿è¡ï¼ä½ç®åä»¥ä¸æä½ç³»ç»å·²ç»æµè¯éè¿:
+![Windows10](https://img.shields.io/badge/Windows-10-green?logo=windows) !
+[Windows11](https://img.shields.io/badge/Windows-11-green?logo=windows11) !
+[Ubuntu22.04](https://img.shields.io/badge/Ubuntu-22.04-green?logo=ubuntu)
+News/ææ°åè½ ------------ ææ°å¼åçï¼2.6.5-devï¼æ°åå®¹: - [X]
+å­æ¨¡å`tools_3d`æ°å¢ç±»`Space`å¯ä»¥ç´æ¥æä¾å¯¹3Då¯¹è±¡è¿è¡å¹³ç§»ãæè½¬åç¼©æ¾ç­æä½çåè½
+- [X]
+ä¿®å¤äºç±»`Cuboid`åç±»`Tetrahedron`æ²¡æå°å®ä¾æ·»å å°ç¶ç±»`Canvas_3D`çbug
+- [X] ä¿®å¤äºå½3Då¯¹è±¡åºç°å¨ç¸æºä½ç½®åé¢æ¶ä¼æ¾ç¤ºéè¯¯çbug -
+[X] ä¿®å¤äºé¨åéè¯¯çç±»åæç¤º ææ°ç¨³å®çï¼2.6.4ï¼æ°åå®¹:
+æ°å¢äºå¯¹3då ä½ä½ç©ºé´ä½ç½®æåºçæ¯æï¼ä½¿å¾å ä½ä½ä¸ååªæç²ç¥ççº¿æ¡ï¼èæ¥æä¸°å¯çé¢è²ã
 å¨ Windows ç³»ç»ä¸è¿è¡ä¸é¢çç¤ºä¾ç¨åºæ¶ï¼å¶æ¥æä»¥ä¸åè½ï¼
 * æä½é¼ æ å·¦é®æå¨å¯ä»¥æè½¬è¿å¤ä¸ªå ä½ä½ï¼ *
 æä½é¼ æ å³é®æå¨å¯ä»¥ç§»å¨è¿äºå ä½ä½å¨ç©ºé´ä¸­çä½ç½®ï¼ *
 æâ=âåâ-âé®åå«å¯ä»¥æ¾å¤§åç¼©å°å ä½ä½çå¤§å°ï¼ *
 æ»å¨é¼ æ ä¸­é®å¯ä»¥æ¾å¤§åç¼©å°ç»é¢ã
 ä¸é¢æ¯ç¤ºä¾ç¨åºçææå¾ï¼ ![news.png](news.png) æºä»£ç  ```python
 from tkinter import Event import tkintertools as tkt from tkintertools import
```

### Comparing `tkintertools-dev-2.6.4/setup.py` & `tkintertools-dev-2.6.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 """ 上传 pypi """
 
 import setuptools
 
-
 setuptools.setup(
     name='tkintertools-dev',
-    version="2.6.4",
+    version='2.6.5',
     author='Xiaokang2022',
     license='MulanPSL-2.0',
     author_email='2951256653@qq.com',
     description='An auxiliary module of the tkinder module',
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/Xiaokang2022/tkintertools',
     packages=setuptools.find_packages(),
+    python_requires='>=3.8',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)',
         'Operating System :: OS Independent',
     ],
+    keywords=['tkinter', 'tkintertools', 'GUI'],
 )
 
 # python -m pip install --user --upgrade setuptools wheel [检查更新]
 
 # python setup.py sdist bdist_wheel [打包]
 # python -m twine upload dist/* [上传]
```

### Comparing `tkintertools-dev-2.6.4/tkintertools/__init__.py` & `tkintertools-dev-2.6.5/tkintertools/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,50 +1,60 @@
+# Copyright (c) 2022 Xiaokang2022
+# tkintertools is licensed under Mulan PSL v2.
+# You can use this software according to the terms and conditions of the Mulan PSL v2.
+# You may obtain a copy of Mulan PSL v2 at: http://license.coscl.org.cn/MulanPSL2
+# THIS SOFTWARE IS PROVIDED ON AN "AS IS" BASIS, WITHOUT WARRANTIES OF ANY KIND,
+# EITHER EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO NON-INFRINGEMENT,
+# MERCHANTABILITY OR FIT FOR A PARTICULAR PURPOSE.
+# See the Mulan PSL v2 for more details.
+
 """
 tkintertools
 ============
 The tkindertools module is an auxiliary module of the tkinder module.
 
 Provides
 --------
 * Transparent, rounded and customized widgets
 * Automatic control of picture size and widget size
 * Scalable png pictures and playable gif pictures
 * Regular mobile widgets and canvas interfaces
 * Gradient colors and contrast colors
 * Text with controllable length and alignment
 * Convenient, inheritable singleton pattern class
-* Display clear window and its contents
+* 3D drawing
 
 Contents
 --------
 * Container Widgets: `Tk`, `Toplevel`, `Canvas`
 * Virtual Canvas Widgets: `Label`, `Button`, `CheckButton`, `Entry`, `Text`, `Progressbar`
 * Tool Classes: `PhotoImage`, `Singleton`
 * Tool Functions: `move`, `text`, `color`, `askfont`, `SetProcessDpiAwareness`
+* Tool Submodules: `tool_3d`
 
 More
 ----
-* GitCode: https://gitcode.net/weixin_62651706/tkintertools
-* GitHub(Mirror): https://github.com/XiaoKang2022-CSDN/tkintertools
-* Tutorials: https://xiaokang2022.blog.csdn.net/article/details/127374661
+* GitHub: https://github.com/Xiaokang2022/tkintertools
+* Gitee(Mirror): https://gitee.com/xiaokang-2022/tkintertools
+* GitCode(Mirror): https://gitcode.net/weixin_62651706/tkintertools
 """
 
 import sys
 
 if sys.version_info < (3, 8):  # Version Check
-    error_info = '\n\033[31mOperation Requirements: \033[32m\nPython version shall not be less than\033[33m 3.7.0 !\033[0m'
+    error_info = '\n\033[31mOperation Requirements: \033[32m\nPython version shall not be less than\033[33m 3.8 !\033[0m'
     raise RuntimeError(error_info)
 
 from .__main__ import (Button, Canvas, CheckButton, Entry, Label, PhotoImage,
                        Progressbar, SetProcessDpiAwareness, Singleton, Text,
                        Tk, Toplevel, askfont, color, move, text)
 from .constants import *
 
 __author__ = 'Xiaokang2022<2951256653@qq.com>'
-__version__ = '2.6.4'
+__version__ = '2.6.5'
 __all__ = [
     # Container Widgets
     'Tk', 'Toplevel', 'Canvas',
     # Virtual Canvas Widgets
     'Label', 'Button', 'CheckButton', 'Entry', 'Text', 'Progressbar',
     # Tool Classes
     'PhotoImage', 'Singleton',
```

### Comparing `tkintertools-dev-2.6.4/tkintertools/__main__.py` & `tkintertools-dev-2.6.5/tkintertools/__main__.py`

 * *Files identical despite different names*

### Comparing `tkintertools-dev-2.6.4/tkintertools/constants.py` & `tkintertools-dev-2.6.5/tkintertools/constants.py`

 * *Files identical despite different names*

### Comparing `tkintertools-dev-2.6.4/tkintertools/tools_3d.py` & `tkintertools-dev-2.6.5/tkintertools/tools_3d.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """ 3D support """
 
 import math  # 数学支持
 import statistics  # 数据统计
+from tkinter import Event  # 类型提示
 from typing import Iterable  # 类型提示
 
 from .__main__ import Canvas, Tk, Toplevel  # 继承和类型提示
 from .constants import *
 
 
 def translate(coords, dx=0, dy=0, dz=0):
@@ -20,15 +21,15 @@
     `dz`: z方向位移\n
     """
     coords[0] += dx
     coords[1] += dy
     coords[2] += dz
 
 
-def rotate(coords, dx=1, dy=1, dz=1, *, center=[0, 0, 0]):
+def rotate(coords, dx=0, dy=0, dz=0, *, center=[0, 0, 0]):
     # type: (list[float], float, float, float, ..., Iterable[float]) -> None
     """
     ### 旋转
     将一个空间三维中的点以另一个点为旋转中心进行旋转\n
     ---
     `coords`: 被旋转点的空间坐标列表\n
     `dx`: x方向旋转弧度\n
@@ -113,46 +114,119 @@
 
     def geos(self):  # type: () -> tuple[Geometry]
         """ 返回`Canvas_3d`类的`geos`元组 """
         return tuple(self._geos)
 
     def space_sort(self):  # type: () -> None
         """ 空间位置排序 """
-        items = [item for item in self._items_3d]
-        items.sort(key=lambda item: item.camera_distance())
-        for item in items:
+        self._items_3d.sort(key=lambda item: item.camera_distance())
+        for item in self._items_3d:
             self.lower(item.item)
 
 
-class _Point():
+class Space(Canvas_3D):
+    """ 三维空间 """
+
+    def __init__(
+        self,
+        master,  # type: Tk | Toplevel
+        width,  # type: int
+        height,  # type: int
+        x=None,  # type: int | None
+        y=None,  # type: int | None
+        *,
+        lock=True,  # type: bool
+        expand=True,  # type: bool
+        keep=True,  # type: bool
+        camera_distance=CAMERA_DISTANCE,  # type: float
+        dx=None,  # type: float | None
+        dy=None,  # type: float | None
+        origin_color='',  # type: str
+        **kw
+    ):  # type: (...) -> None
+        Canvas_3D.__init__(self, master, width, height, x, y, lock=lock, expand=expand,
+                           keep=keep, camera_distance=camera_distance, dx=dx, dy=dy, **kw)
+        self._origin = Point(self, [0, 0, 0], size=1,
+                             fill=origin_color, outline=origin_color)
+        self.space_sort()
+        self.bind('<B3-Motion>', self._translate)
+        self.bind('<Button-3>', lambda _: self._translate(_, True))
+        self.bind('<ButtonRelease-3>', lambda _: self._translate(_, False))
+        self.bind('<B1-Motion>', self._rotate)
+        self.bind('<Button-1>', lambda _: self._rotate(_, True))
+        self.bind('<ButtonRelease-1>', lambda _: self._rotate(_, False))
+        self.bind('<MouseWheel>', self._zoom)
+        # NOTE: https://www.tcl.tk/man/tcl8.6/TkCmd/cursors.html
+
+    def _translate(self, event, flag=None, cache=[]):
+        # type: (Event, bool | None, list[float]) -> None
+        """ 平移视角 """
+        if flag is True:  # 按下
+            cache[:] = [event.x, event.y]
+            return self.configure(cursor='size')
+        elif flag is False:  # 松开
+            return self.configure(cursor='arrow')
+        dx, dy = event.x-cache[0], event.y-cache[1]
+        cache[:] = [event.x, event.y]
+        for item in self._geos+[self._origin]:
+            item.translate(0, dx, dy)
+            item.update()
+        self.space_sort()
+
+    def _rotate(self, event, flag=None, cache=[]):
+        # type: (Event, bool | None, list[float]) -> None
+        """ 旋转视角 """
+        if flag is True:
+            cache[:] = [event.x, event.y]
+            return self.configure(cursor='size')
+        elif flag is False:
+            return self.configure(cursor='arrow')
+        dx, dy = event.x-cache[0], event.y-cache[1]
+        cache[:] = [event.x, event.y]
+        for item in self._geos+[self._origin]:
+            item.rotate(0, -dy/self.dx*math.pi, dx /
+                        self.dy*math.pi, center=self._origin.coords)
+            item.update()
+        self.space_sort()
+
+    def _zoom(self, event):  # type: (Event) -> None
+        """ 缩放视角 """
+        k = 1.1 if event.delta > 0 else 0.9
+        for item in self.geos():
+            item.scale(k, k, k, center=self._origin.coords)
+            item.update()
+        self.space_sort()
+
+
+class _Point:
     """ 点 """
 
     def __init__(self, coords):  # type: (list[float]) -> None
         self.coords = coords  # 利用列表引用
 
     def translate(self, dx=0, dy=0, dz=0):  # type: (float, float, float) -> None
         """ 平移 """
         translate(self.coords, dx, dy, dz)
 
-    def rotate(self, dx=1, dy=1, dz=1, *, center=[0, 0, 0]):
+    def rotate(self, dx=0, dy=0, dz=0, *, center=[0, 0, 0]):
         # type: (float, float, float, ..., Iterable[float]) -> None
         """ 旋转 """
         rotate(self.coords, dx, dy, dz, center=center)
 
     def scale(self, kx=1, ky=1, kz=1, *, center=None):
         # type: (float, float, float, ..., Iterable[float] | None) -> None
         """ 缩放 """
         scale(self.coords, kx, ky, kz, center=center)
 
     def project(self, distance):  # type: (float) -> list[float]
         """ 投影 """
-        try:
-            k = distance/(distance - self.coords[0])
-        except ZeroDivisionError:
-            return [distance*10, distance*10]
+        relative_dis = distance - self.coords[0]
+        if relative_dis <= 1e-16:
+            return [float('INF')]*2  # BUG
+        k = distance/relative_dis
         return [self.coords[1]*k, self.coords[2]*k]
 
 
 class _Line:
     """ 线 """
 
     def __init__(
@@ -164,15 +238,15 @@
         self.points = [_Point(point) for point in self.coords]
 
     def translate(self, dx=0, dy=0, dz=0):  # type: (float, float, float) -> None
         """ 平移 """
         for coord in self.coords:
             translate(coord, dx, dy, dz)
 
-    def rotate(self, dx=1, dy=1, dz=1, *, center=[0, 0, 0]):
+    def rotate(self, dx=0, dy=0, dz=0, *, center=[0, 0, 0]):
         # type: (float, float, float, ..., Iterable[float]) -> None
         """ 旋转 """
         for coord in self.coords:
             rotate(coord, dx, dy, dz, center=center)
 
     def scale(self, kx=1, ky=1, kz=1, *, center=None):
         # type: (float, float, float, ..., Iterable[float] | None) -> None
@@ -196,15 +270,15 @@
                       for ind in range(len(points))]
 
     def translate(self, dx=0, dy=0, dz=0):  # type: (float, float, float) -> None
         """ 平移 """
         for coord in self.coords:
             translate(coord, dx, dy, dz)
 
-    def rotate(self, dx=1, dy=1, dz=1, *, center=[0, 0, 0]):
+    def rotate(self, dx=0, dy=0, dz=0, *, center=[0, 0, 0]):
         # type: (float, float, float, ..., Iterable[float]) -> None
         """ 旋转 """
         for coord in self.coords:
             rotate(coord, dx, dy, dz, center=center)
 
     def scale(self, kx=1, ky=1, kz=1, *, center=None):
         # type: (float, float, float, ..., Iterable[float] | None) -> None
@@ -373,21 +447,21 @@
         `dz`: z轴方向位移距离\n
         """
         coords = [coord for side in self.sides for coord in side.coords]
         for ind, coord in enumerate(coords):
             if coord not in coords[:ind]:
                 translate(coord, dx, dy, dz)
 
-    def rotate(self, dx=1, dy=1, dz=1, *, center=[0, 0, 0]):
+    def rotate(self, dx=0, dy=0, dz=0, *, center=[0, 0, 0]):
         # type: (float, float, float, ..., Iterable[float]) -> None
         """
         旋转\n
-        `dx`: 绕x轴方向旋转角度\n
-        `dy`: 绕y轴方向旋转角度\n
-        `dz`: 绕z轴方向旋转角度\n
+        `dx`: 绕x轴方向旋转弧度\n
+        `dy`: 绕y轴方向旋转弧度\n
+        `dz`: 绕z轴方向旋转弧度\n
         `center`: 旋转中心\n
         """
         coords = [coord for side in self.sides for coord in side.coords]
         for ind, coord in enumerate(coords):
             if coord not in coords[:ind]:
                 rotate(coord, dx, dy, dz, center=center)
 
@@ -456,14 +530,15 @@
         `color_up`: 上表面颜色\n
         `color_down`: 下表面颜色\n
         `color_left`: 左侧面颜色\n
         `color_right`: 右侧面颜色\n
         `color_front`: 正面颜色\n
         `color_back`: 后面颜色\n
         """
+        canvas._geos.append(self)
         self.canvas = canvas
         self.coords = [[x+l, y+w, z+h]
                        for l in (0, length)
                        for w in (0, width)
                        for h in (0, height)]
         self.sides = [
             Side(canvas, self.coords[0], self.coords[1],
@@ -498,14 +573,15 @@
         `canvas`: 父画布\n
         `p1`: 第一个顶点\n
         `p2`: 第二个顶点\n
         `p3`: 第三个顶点\n
         `p4`: 第四个顶点\n
         `colors`: 颜色序列\n
         """
+        canvas._geos.append(self)
         self.canvas = canvas
         self.coords = [list(p1), list(p2), list(p3), list(p4)]
         self.sides = [
             Side(canvas, self.coords[0], self.coords[1],
                  self.coords[2], fill=colors[0]),
             Side(canvas, self.coords[0], self.coords[1],
                  self.coords[3], fill=colors[1]),
```

### Comparing `tkintertools-dev-2.6.4/tkintertools_dev.egg-info/PKG-INFO` & `tkintertools-dev-2.6.5/tkintertools_dev.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,98 +1,120 @@
 Metadata-Version: 2.1
 Name: tkintertools-dev
-Version: 2.6.4
+Version: 2.6.5
 Summary: An auxiliary module of the tkinder module
 Home-page: https://github.com/Xiaokang2022/tkintertools
 Author: Xiaokang2022
 Author-email: 2951256653@qq.com
 License: MulanPSL-2.0
+Keywords: tkinter,tkintertools,GUI
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
 Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
     <h1>🚀tkintertools🚀</h1>
-    <p><img height="120px" alt="logo.png"
-        src="tkintertools.png" />
+    <p><img height="128px" alt="logo.png" src="tkt.png" /></p>
+    <p>
+    The <code>tkintertools</code> module is an auxiliary module of the <code>tkinter</code> module
+    <br />
+    <code>tkintertools</code> 模块是 <code>tkinter</code> 模块的辅助模块
     </p>
-    <p>The <code>tkintertools</code> module is an auxiliary module of the <code>tkinter</code> module</p>
-    <p><code>tkintertools</code> 模块是 <code>tkinter</code> 模块的辅助模块</p>
     <p>
         <a href="tkintertools/__init__.py">
-            <img src="https://img.shields.io/badge/Version-2.6.4(dev)-blue" alt="latest version" />
+            <img src="https://img.shields.io/badge/Version-2.6.5(dev)-blue" alt="latest version" />
         </a>
         <a href="LICENSE">
             <img src="https://img.shields.io/badge/License-Mulan PSL v2-green" alt="License" />
         </a>
         <a href="CHANGELOG.md">
-            <img src="https://img.shields.io/badge/ChangeLog-2023/06/11-orange" alt="ChangeLog" />
+            <img src="https://img.shields.io/badge/ChangeLog-2023/06/13-orange" alt="ChangeLog" />
         </a>
         <a href="TODO.md">
-            <img src="https://img.shields.io/badge/ToDos-14-yellow" alt="ToDos" />
+            <img src="https://img.shields.io/badge/ToDo-14-yellow?logo=cachet" alt="ToDos" />
         </a>
         <a href="https://pypistats.org/packages/tkintertools">
-            <img src="https://img.shields.io/badge/Downloads-4k-purple" alt="Downloads" />
+            <img src="https://img.shields.io/badge/Download-4k-purple?logo=pypi" alt="Downloads" />
         </a>
-    </p>
-    <p>
+        <br />
         <a href="mailto:2951256653@qq.com">
             <img src="https://img.shields.io/badge/Email-2951256653@qq.com-cyan" alt="Email" />
         </a>
-        <a href="https://xiaokang2022.blog.csdn.net">
-            <img src="https://img.shields.io/badge/Blog-小康2022@CSDN-red" alt="Blog" />
-        </a>
         <a href="https://github.com/Xiaokang2022">
             <img src="https://img.shields.io/badge/Author-小康2022-white" alt="Author" />
         </a>
+        <a href="https://xiaokang2022.blog.csdn.net">
+            <img src="https://img.shields.io/badge/Blog-小康2022@CSDN-red" alt="Blog" />
+        </a>
     </p>
 </div>
 
-Installation/模块安装
---------------------
+Install/模块安装
+---------------
 
 ### Stable version/稳定版本
 
-* Version/版本 : 2.6.3
-* Release Date/发布日期 : 2023/06/07
-
-```
-pip install tkintertools==2.6.3
-或者
-pip install tkintertools
-```
+* Version/版本 : 2.6.4
+* Release Date/发布日期 : 2023/06/12
 
 这个是目前的最新稳定版，比较稳定，bug （可能）没有那么多，推荐使用这个。  
 关于稳定版有 Issue 的话，我会去查看并尝试解决 Issue。
 
-### Development version/开发版本
-
-* Version/版本 : 2.6.4
-* Release Date/发布日期 : 2023/06/11
-
 ```
-pip install tkintertools-dev==2.6.4
-或者
-pip install tkintertools-dev
+pip install tkintertools==2.6.4
 ```
 
+### Development version/开发版本
+
+* Version/版本 : 2.6.5
+* Release Date/发布日期 : 2023/06/13
+
 这个是我正在开发的版本，可能有新功能，bug 也可能会比较多，但也可能会比原来的版本更加稳定。  
 大家可以在 Issue 中提出一些建议，我会适当采纳一些并在开发版本中更改或实现。
 
-**特别注意**
+```
+pip install tkintertools-dev==2.6.5
+```
+
+**Attention/特别注意**
 * 开发版仅作示例，各函数或类的API并非最终确定结果，直接使用开发版可能导致后续无法与正式版兼容！
 * 若要使用开发版，请先卸载正式版后再进行pip安装，再次使用正式版时也是一样，先卸载开发版再安装正式版！
-* 需要 **Python3.8** 及更高版本才能运行 tkintertools！
+
+### Environmental requirements/环境需求
+
+没有任何额外的依赖包（除了tkinter），但只支持以下 Python 版本:
+
+![Python3.8](https://img.shields.io/badge/Python-3.8.*-blue?logo=python)
+![Python3.9](https://img.shields.io/badge/Python-3.9.*-blue?logo=python)
+![Python3.10](https://img.shields.io/badge/Python-3.10.*-blue?logo=python)
+![Python3.11](https://img.shields.io/badge/Python-3.11.*-blue?logo=python)
+![Python3.12](https://img.shields.io/badge/Python-3.12.*-blue?logo=python)
+
+可能在某些操作系统上也可运行，但目前以下操作系统已经测试通过:
+
+![Windows10](https://img.shields.io/badge/Windows-10-green?logo=windows)
+![Windows11](https://img.shields.io/badge/Windows-11-green?logo=windows11)
+![Ubuntu22.04](https://img.shields.io/badge/Ubuntu-22.04-green?logo=ubuntu)
 
 <a name="news">News/最新功能</a>
 ------------
 
-最新版的 tkintertools **开发版**(2.6.4-dev)新增了对3d几何体空间位置排序的支持，使得几何体不再只有粗略的线条，而拥有丰富的颜色。
+最新开发版（2.6.5-dev）新内容:
+
+- [X] 子模块`tools_3d`新增类`Space`可以直接提供对3D对象进行平移、旋转和缩放等操作的功能
+- [X] 修复了类`Cuboid`和类`Tetrahedron`没有将实例添加到父类`Canvas_3D`的bug
+- [X] 修复了当3D对象出现在相机位置后面时会显示错误的bug
+- [X] 修复了部分错误的类型提示
+
+最新稳定版（2.6.4）新内容:
+
+新增了对3d几何体空间位置排序的支持，使得几何体不再只有粗略的线条，而拥有丰富的颜色。
 
 在 Windows 系统下运行下面的示例程序时，其拥有以下功能：
 * 按住鼠标左键拖动可以旋转这多个几何体；
 * 按住鼠标右键拖动可以移动这些几何体在空间中的位置；
 * 按“=”和“-”键分别可以放大和缩小几何体的大小；
 * 滚动鼠标中键可以放大和缩小画面。
```

#### html2text {}

```diff
@@ -1,39 +1,55 @@
-Metadata-Version: 2.1 Name: tkintertools-dev Version: 2.6.4 Summary: An
+Metadata-Version: 2.1 Name: tkintertools-dev Version: 2.6.5 Summary: An
 auxiliary module of the tkinder module Home-page: https://github.com/
 Xiaokang2022/tkintertools Author: Xiaokang2022 Author-email: 2951256653@qq.com
-License: MulanPSL-2.0 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Mulan Permissive Software License v2
-(MulanPSL-2.0) Classifier: Operating System :: OS Independent Description-
-Content-Type: text/markdown License-File: LICENSE
+License: MulanPSL-2.0 Keywords: tkinter,tkintertools,GUI Classifier:
+Programming Language :: Python :: 3 Classifier: License :: OSI Approved ::
+Mulan Permissive Software License v2 (MulanPSL-2.0) Classifier: Operating
+System :: OS Independent Requires-Python: >=3.8 Description-Content-Type: text/
+markdown License-File: LICENSE
                       ****** ðtkintertoolsð ******
                                   [logo.png]
      The tkintertools module is an auxiliary module of the tkinter module
              tkintertools æ¨¡åæ¯ tkinter æ¨¡åçè¾å©æ¨¡å
           [latest_version] [License] [ChangeLog] [ToDos] [Downloads]
-                            [Email] [Blog] [Author]
-Installation/æ¨¡åå®è£ -------------------- ### Stable version/ç¨³å®çæ¬
-* Version/çæ¬ : 2.6.3 * Release Date/åå¸æ¥æ : 2023/06/07 ``` pip
-install tkintertools==2.6.3 æè pip install tkintertools ```
+                            [Email] [Author] [Blog]
+Install/æ¨¡åå®è£ --------------- ### Stable version/ç¨³å®çæ¬ * Version/
+çæ¬ : 2.6.4 * Release Date/åå¸æ¥æ : 2023/06/12
 è¿ä¸ªæ¯ç®åçææ°ç¨³å®çï¼æ¯è¾ç¨³å®ï¼bug
 ï¼å¯è½ï¼æ²¡æé£ä¹å¤ï¼æ¨èä½¿ç¨è¿ä¸ªã å³äºç¨³å®çæ Issue
-çè¯ï¼æä¼å»æ¥çå¹¶å°è¯è§£å³ Issueã ### Development version/
-å¼åçæ¬ * Version/çæ¬ : 2.6.4 * Release Date/åå¸æ¥æ : 2023/06/11
-``` pip install tkintertools-dev==2.6.4 æè pip install tkintertools-dev ```
+çè¯ï¼æä¼å»æ¥çå¹¶å°è¯è§£å³ Issueã ``` pip install
+tkintertools==2.6.4 ``` ### Development version/å¼åçæ¬ * Version/çæ¬ :
+2.6.5 * Release Date/åå¸æ¥æ : 2023/06/13
 è¿ä¸ªæ¯ææ­£å¨å¼åççæ¬ï¼å¯è½ææ°åè½ï¼bug
 ä¹å¯è½ä¼æ¯è¾å¤ï¼ä½ä¹å¯è½ä¼æ¯åæ¥ççæ¬æ´å ç¨³å®ã
 å¤§å®¶å¯ä»¥å¨ Issue
 ä¸­æåºä¸äºå»ºè®®ï¼æä¼éå½éçº³ä¸äºå¹¶å¨å¼åçæ¬ä¸­æ´æ¹æå®ç°ã
-**ç¹å«æ³¨æ** *
+``` pip install tkintertools-dev==2.6.5 ``` **Attention/ç¹å«æ³¨æ** *
 å¼åçä»ä½ç¤ºä¾ï¼åå½æ°æç±»çAPIå¹¶éæç»ç¡®å®ç»æï¼ç´æ¥ä½¿ç¨å¼åçå¯è½å¯¼è´åç»­æ æ³ä¸æ­£å¼çå¼å®¹ï¼
 *
 è¥è¦ä½¿ç¨å¼åçï¼è¯·åå¸è½½æ­£å¼çååè¿è¡pipå®è£ï¼åæ¬¡ä½¿ç¨æ­£å¼çæ¶ä¹æ¯ä¸æ ·ï¼åå¸è½½å¼åçåå®è£æ­£å¼çï¼
-* éè¦ **Python3.8** åæ´é«çæ¬æè½è¿è¡ tkintertoolsï¼ News/
-ææ°åè½ ------------ ææ°çç tkintertools **å¼åç**(2.6.4-
-dev)æ°å¢äºå¯¹3då ä½ä½ç©ºé´ä½ç½®æåºçæ¯æï¼ä½¿å¾å ä½ä½ä¸ååªæç²ç¥ççº¿æ¡ï¼èæ¥æä¸°å¯çé¢è²ã
+### Environmental requirements/ç¯å¢éæ±
+æ²¡æä»»ä½é¢å¤çä¾èµåï¼é¤äºtkinterï¼ï¼ä½åªæ¯æä»¥ä¸ Python
+çæ¬: ![Python3.8](https://img.shields.io/badge/Python-3.8.*-
+blue?logo=python) ![Python3.9](https://img.shields.io/badge/Python-3.9.*-
+blue?logo=python) ![Python3.10](https://img.shields.io/badge/Python-3.10.*-
+blue?logo=python) ![Python3.11](https://img.shields.io/badge/Python-3.11.*-
+blue?logo=python) ![Python3.12](https://img.shields.io/badge/Python-3.12.*-
+blue?logo=python)
+å¯è½å¨æäºæä½ç³»ç»ä¸ä¹å¯è¿è¡ï¼ä½ç®åä»¥ä¸æä½ç³»ç»å·²ç»æµè¯éè¿:
+![Windows10](https://img.shields.io/badge/Windows-10-green?logo=windows) !
+[Windows11](https://img.shields.io/badge/Windows-11-green?logo=windows11) !
+[Ubuntu22.04](https://img.shields.io/badge/Ubuntu-22.04-green?logo=ubuntu)
+News/ææ°åè½ ------------ ææ°å¼åçï¼2.6.5-devï¼æ°åå®¹: - [X]
+å­æ¨¡å`tools_3d`æ°å¢ç±»`Space`å¯ä»¥ç´æ¥æä¾å¯¹3Då¯¹è±¡è¿è¡å¹³ç§»ãæè½¬åç¼©æ¾ç­æä½çåè½
+- [X]
+ä¿®å¤äºç±»`Cuboid`åç±»`Tetrahedron`æ²¡æå°å®ä¾æ·»å å°ç¶ç±»`Canvas_3D`çbug
+- [X] ä¿®å¤äºå½3Då¯¹è±¡åºç°å¨ç¸æºä½ç½®åé¢æ¶ä¼æ¾ç¤ºéè¯¯çbug -
+[X] ä¿®å¤äºé¨åéè¯¯çç±»åæç¤º ææ°ç¨³å®çï¼2.6.4ï¼æ°åå®¹:
+æ°å¢äºå¯¹3då ä½ä½ç©ºé´ä½ç½®æåºçæ¯æï¼ä½¿å¾å ä½ä½ä¸ååªæç²ç¥ççº¿æ¡ï¼èæ¥æä¸°å¯çé¢è²ã
 å¨ Windows ç³»ç»ä¸è¿è¡ä¸é¢çç¤ºä¾ç¨åºæ¶ï¼å¶æ¥æä»¥ä¸åè½ï¼
 * æä½é¼ æ å·¦é®æå¨å¯ä»¥æè½¬è¿å¤ä¸ªå ä½ä½ï¼ *
 æä½é¼ æ å³é®æå¨å¯ä»¥ç§»å¨è¿äºå ä½ä½å¨ç©ºé´ä¸­çä½ç½®ï¼ *
 æâ=âåâ-âé®åå«å¯ä»¥æ¾å¤§åç¼©å°å ä½ä½çå¤§å°ï¼ *
 æ»å¨é¼ æ ä¸­é®å¯ä»¥æ¾å¤§åç¼©å°ç»é¢ã
 ä¸é¢æ¯ç¤ºä¾ç¨åºçææå¾ï¼ ![news.png](news.png) æºä»£ç  ```python
 from tkinter import Event import tkintertools as tkt from tkintertools import
```

