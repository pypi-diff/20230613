# Comparing `tmp/xiaoranli-7.1.1-py3-none-any.whl.zip` & `tmp/xiaoranli-7.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 13602 bytes, number of entries: 20
+Zip file size: 13570 bytes, number of entries: 20
 -rw-r--r--  2.0 unx     3808 b- defN 23-Jun-13 09:02 xiaoranli/__init__.py
--rw-r--r--  2.0 unx     1920 b- defN 23-Jun-12 07:32 xiaoranli/data/rc_files/alias
+-rw-r--r--  2.0 unx     1854 b- defN 23-Jun-13 09:06 xiaoranli/data/rc_files/alias
 -rw-r--r--  2.0 unx       75 b- defN 23-Jun-12 07:32 xiaoranli/data/rc_files/dockerignore
 -rw-r--r--  2.0 unx      393 b- defN 23-Jun-12 07:32 xiaoranli/data/rc_files/gdbinit
 -rw-r--r--  2.0 unx      124 b- defN 23-Jun-12 07:32 xiaoranli/data/rc_files/gitconfig
 -rw-r--r--  2.0 unx      561 b- defN 23-Jun-12 07:32 xiaoranli/data/rc_files/inputrc
 -rw-r--r--  2.0 unx      903 b- defN 23-Jun-12 07:32 xiaoranli/data/rc_files/tmux.config
 -rw-r--r--  2.0 unx      452 b- defN 23-Jun-12 07:33 xiaoranli/data/rc_files/vimrc
 -rw-r--r--  2.0 unx      188 b- defN 23-Jun-12 07:32 xiaoranli/scripts/install_golang.sh
 -rw-r--r--  2.0 unx     1874 b- defN 23-Jun-13 08:27 xiaoranli/scripts/install_useful_tools.sh
 -rw-r--r--  2.0 unx      451 b- defN 23-Jun-13 08:02 xiaoranli/scripts/install_zsh.sh
 -rw-r--r--  2.0 unx      480 b- defN 23-Jun-12 07:32 xiaoranli/zhijiang/scripts/enhance_python.sh
 -rw-r--r--  2.0 unx     1150 b- defN 23-Jun-12 07:32 xiaoranli/zhijiang/scripts/install_useful_tools.sh
 -rw-r--r--  2.0 unx     7953 b- defN 23-Jun-13 05:36 xiaoranli/zhijiang/scripts/useful_func.py
--rw-r--r--  2.0 unx     1081 b- defN 23-Jun-13 09:06 xiaoranli-7.1.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      923 b- defN 23-Jun-13 09:06 xiaoranli-7.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-13 09:06 xiaoranli-7.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       45 b- defN 23-Jun-13 09:06 xiaoranli-7.1.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 23-Jun-13 09:06 xiaoranli-7.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1772 b- defN 23-Jun-13 09:06 xiaoranli-7.1.1.dist-info/RECORD
-20 files, 24255 bytes uncompressed, 10654 bytes compressed:  56.1%
+-rw-r--r--  2.0 unx     1081 b- defN 23-Jun-13 09:07 xiaoranli-7.1.2.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      923 b- defN 23-Jun-13 09:07 xiaoranli-7.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-13 09:07 xiaoranli-7.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       45 b- defN 23-Jun-13 09:07 xiaoranli-7.1.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-13 09:07 xiaoranli-7.1.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1772 b- defN 23-Jun-13 09:07 xiaoranli-7.1.2.dist-info/RECORD
+20 files, 24189 bytes uncompressed, 10622 bytes compressed:  56.1%
```

## zipnote {}

```diff
@@ -36,26 +36,26 @@
 
 Filename: xiaoranli/zhijiang/scripts/install_useful_tools.sh
 Comment: 
 
 Filename: xiaoranli/zhijiang/scripts/useful_func.py
 Comment: 
 
-Filename: xiaoranli-7.1.1.dist-info/LICENSE.txt
+Filename: xiaoranli-7.1.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xiaoranli-7.1.1.dist-info/METADATA
+Filename: xiaoranli-7.1.2.dist-info/METADATA
 Comment: 
 
-Filename: xiaoranli-7.1.1.dist-info/WHEEL
+Filename: xiaoranli-7.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: xiaoranli-7.1.1.dist-info/entry_points.txt
+Filename: xiaoranli-7.1.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: xiaoranli-7.1.1.dist-info/top_level.txt
+Filename: xiaoranli-7.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: xiaoranli-7.1.1.dist-info/RECORD
+Filename: xiaoranli-7.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xiaoranli/data/rc_files/alias

```diff
@@ -1,9 +1,7 @@
-alias ls='exa --group-directories-first'
-alias ll="exa -abghHliS"
 alias cat="batcat"
 alias grep='grep --color=auto'
 alias less='less -i' # ignore case when searching
 alias ps='ps auxf|peco' # process tree
 alias top='top c'
 alias sudo="sudo env \"PATH=$PATH\""
 alias j='autojump'
```

## Comparing `xiaoranli-7.1.1.dist-info/LICENSE.txt` & `xiaoranli-7.1.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `xiaoranli-7.1.1.dist-info/METADATA` & `xiaoranli-7.1.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xiaoranli
-Version: 7.1.1
+Version: 7.1.2
 Summary: setup linux env, such as bashrc etc.
 Home-page: https://github.com/xiaoranliMS/env-setup.git
 Author: Li Xiaoran
 Author-email: 1240897116@qq.com
 Project-URL: Funding,  https://github.com/xiaoranliMS
 Project-URL: Source, https://github.com/xiaoranliMS/env-setup.git
 Keywords: env setup,development,xiaoranli
```

## Comparing `xiaoranli-7.1.1.dist-info/RECORD` & `xiaoranli-7.1.2.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 xiaoranli/__init__.py,sha256=h1E19jN92KaWNDe55BGV6PZHC7Bl2Wxn1NW8qfroYEs,3808
-xiaoranli/data/rc_files/alias,sha256=kxHI2nOHQLggc-GLAS3mgKBZXe_D54IlrYSvQOB8j3E,1920
+xiaoranli/data/rc_files/alias,sha256=14B42RVy8JjFnp-EnIwDU6Iix0eJRTbxRJAC92uhZIw,1854
 xiaoranli/data/rc_files/dockerignore,sha256=fNTcMXrdUU9h9Y0tkLpfQKbLhwRwaVNd-MyP-ycI3sE,75
 xiaoranli/data/rc_files/gdbinit,sha256=Om1pIhhf-_lIfLgx8Gt730W2R4vvZLr05hbgnhNy0Hs,393
 xiaoranli/data/rc_files/gitconfig,sha256=sSooqGwfXpEHUvL047wvYQOMl1zQUgN8GVWWMhRLYII,124
 xiaoranli/data/rc_files/inputrc,sha256=yl22z2lj2jWLaE85I9QpV9NjoYoOhpmPemNxEsxMC5Y,561
 xiaoranli/data/rc_files/tmux.config,sha256=kk88x2Skt6csucriayhCNORaufCV8FsLMycVzEkrwHA,903
 xiaoranli/data/rc_files/vimrc,sha256=z4s0auYUgfiGZ5lZPLpcGhJqVoU8sz2SMxMxxSqyuV8,452
 xiaoranli/scripts/install_golang.sh,sha256=sR2H-HL-Bj6dj9bTD0apJsRLlEQaLoD0Ay5S3qUycxc,188
 xiaoranli/scripts/install_useful_tools.sh,sha256=3hq21Dqrvm6dEVsmXpW5SgA_dviJbX4jZwN8dzKEyuY,1874
 xiaoranli/scripts/install_zsh.sh,sha256=zdgMuJi8a0-5RapD01oSXoQvErMsCDktz9uMCdAUTWo,451
 xiaoranli/zhijiang/scripts/enhance_python.sh,sha256=l9YzkTTMLRzUV_nkCi8PS029QqIx8__bKmD3HCkEycE,480
 xiaoranli/zhijiang/scripts/install_useful_tools.sh,sha256=7C287YLb57j0hxKWLWeM2KIZcI6cM1L4DDHGIlju9UE,1150
 xiaoranli/zhijiang/scripts/useful_func.py,sha256=jgQgWXUkBYSNqC88yOymtlW2MLkL9MYHDnFpiJLKNqk,7953
-xiaoranli-7.1.1.dist-info/LICENSE.txt,sha256=ceC9ZJOV9H6CtQDcYmHOS46NA3dHJ_WD4J9blH513pc,1081
-xiaoranli-7.1.1.dist-info/METADATA,sha256=GloL7whoyukWImyDzN7KOgEMpj9slrsV9hhhZIgi39Y,923
-xiaoranli-7.1.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-xiaoranli-7.1.1.dist-info/entry_points.txt,sha256=T3ZBwdXMY38i4JvMaIXq1WIMdrDEDrVkaWIgKfVsrTc,45
-xiaoranli-7.1.1.dist-info/top_level.txt,sha256=DjwPuFyAkwL8uNM0Z41wNraAt9-71lDJ8SRwYTqRRcs,10
-xiaoranli-7.1.1.dist-info/RECORD,,
+xiaoranli-7.1.2.dist-info/LICENSE.txt,sha256=ceC9ZJOV9H6CtQDcYmHOS46NA3dHJ_WD4J9blH513pc,1081
+xiaoranli-7.1.2.dist-info/METADATA,sha256=AsJUG3Qkxqm09IWt4DFYc0B4lB2xrO6aYU-rL9kxcR0,923
+xiaoranli-7.1.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+xiaoranli-7.1.2.dist-info/entry_points.txt,sha256=T3ZBwdXMY38i4JvMaIXq1WIMdrDEDrVkaWIgKfVsrTc,45
+xiaoranli-7.1.2.dist-info/top_level.txt,sha256=DjwPuFyAkwL8uNM0Z41wNraAt9-71lDJ8SRwYTqRRcs,10
+xiaoranli-7.1.2.dist-info/RECORD,,
```

