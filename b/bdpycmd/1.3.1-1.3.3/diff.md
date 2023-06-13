# Comparing `tmp/bdpycmd-1.3.1.tar.gz` & `tmp/bdpycmd-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bdpycmd-1.3.1.tar", last modified: Tue Jun 13 10:01:53 2023, max compression
+gzip compressed data, was "bdpycmd-1.3.3.tar", last modified: Tue Jun 13 12:27:18 2023, max compression
```

## Comparing `bdpycmd-1.3.1.tar` & `bdpycmd-1.3.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 10:01:53.492786 bdpycmd-1.3.1/
--rw-r--r--   0 zhicheng   (501) staff       (20)     2066 2023-06-13 10:01:53.492886 bdpycmd-1.3.1/PKG-INFO
--rw-r--r--   0 zhicheng   (501) staff       (20)     1406 2023-06-13 08:32:29.000000 bdpycmd-1.3.1/README.md
--rw-r--r--   0 zhicheng   (501) staff       (20)       80 2022-09-04 10:23:26.000000 bdpycmd-1.3.1/pyproject.toml
--rw-r--r--   0 zhicheng   (501) staff       (20)      784 2023-06-13 10:01:53.493231 bdpycmd-1.3.1/setup.cfg
-drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 10:01:53.490308 bdpycmd-1.3.1/src/
-drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 10:01:53.491314 bdpycmd-1.3.1/src/bdpycmd/
--rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 08:19:55.000000 bdpycmd-1.3.1/src/bdpycmd/__init__.py
-drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 10:01:53.492005 bdpycmd-1.3.1/src/bdpycmd/cmd/
--rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 08:12:26.000000 bdpycmd-1.3.1/src/bdpycmd/cmd/__init__.py
-drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 10:01:53.492252 bdpycmd-1.3.1/src/bdpycmd/cmd/camp/
--rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 08:12:26.000000 bdpycmd-1.3.1/src/bdpycmd/cmd/camp/__init__.py
--rw-r--r--   0 zhicheng   (501) staff       (20)     2560 2023-06-13 08:12:26.000000 bdpycmd-1.3.1/src/bdpycmd/cmd/camp/assistant.py
-drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 10:01:53.492620 bdpycmd-1.3.1/src/bdpycmd/cmd/factory/
--rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 08:12:26.000000 bdpycmd-1.3.1/src/bdpycmd/cmd/factory/__init__.py
--rw-r--r--   0 zhicheng   (501) staff       (20)     3918 2023-06-13 08:12:26.000000 bdpycmd-1.3.1/src/bdpycmd/cmd/factory/base.py
--rw-r--r--   0 zhicheng   (501) staff       (20)      716 2023-06-13 08:12:26.000000 bdpycmd-1.3.1/src/bdpycmd/cmd/factory/cmd.py
--rw-r--r--   0 zhicheng   (501) staff       (20)     7614 2023-06-13 09:58:29.000000 bdpycmd-1.3.1/src/bdpycmd/pycmd.py
-drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 10:01:53.491754 bdpycmd-1.3.1/src/bdpycmd.egg-info/
--rw-r--r--   0 zhicheng   (501) staff       (20)     2066 2023-06-13 10:01:53.000000 bdpycmd-1.3.1/src/bdpycmd.egg-info/PKG-INFO
--rw-r--r--   0 zhicheng   (501) staff       (20)      413 2023-06-13 10:01:53.000000 bdpycmd-1.3.1/src/bdpycmd.egg-info/SOURCES.txt
--rw-r--r--   0 zhicheng   (501) staff       (20)        1 2023-06-13 10:01:53.000000 bdpycmd-1.3.1/src/bdpycmd.egg-info/dependency_links.txt
--rw-r--r--   0 zhicheng   (501) staff       (20)        8 2023-06-13 10:01:53.000000 bdpycmd-1.3.1/src/bdpycmd.egg-info/top_level.txt
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:27:18.167132 bdpycmd-1.3.3/
+-rw-r--r--   0 zhicheng   (501) staff       (20)     2066 2023-06-13 12:27:18.167203 bdpycmd-1.3.3/PKG-INFO
+-rw-r--r--   0 zhicheng   (501) staff       (20)     1406 2023-06-13 08:32:29.000000 bdpycmd-1.3.3/README.md
+-rw-r--r--   0 zhicheng   (501) staff       (20)       80 2022-09-04 10:23:26.000000 bdpycmd-1.3.3/pyproject.toml
+-rw-r--r--   0 zhicheng   (501) staff       (20)      784 2023-06-13 12:27:18.167477 bdpycmd-1.3.3/setup.cfg
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:27:18.164726 bdpycmd-1.3.3/src/
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:27:18.165523 bdpycmd-1.3.3/src/bdpycmd/
+-rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 08:19:55.000000 bdpycmd-1.3.3/src/bdpycmd/__init__.py
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:27:18.166400 bdpycmd-1.3.3/src/bdpycmd/cmd/
+-rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:25:21.000000 bdpycmd-1.3.3/src/bdpycmd/cmd/__init__.py
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:27:18.166641 bdpycmd-1.3.3/src/bdpycmd/cmd/camp/
+-rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:25:21.000000 bdpycmd-1.3.3/src/bdpycmd/cmd/camp/__init__.py
+-rw-r--r--   0 zhicheng   (501) staff       (20)     2560 2023-06-13 12:25:21.000000 bdpycmd-1.3.3/src/bdpycmd/cmd/camp/assistant.py
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:27:18.167033 bdpycmd-1.3.3/src/bdpycmd/cmd/factory/
+-rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:25:21.000000 bdpycmd-1.3.3/src/bdpycmd/cmd/factory/__init__.py
+-rw-r--r--   0 zhicheng   (501) staff       (20)     4110 2023-06-13 12:25:21.000000 bdpycmd-1.3.3/src/bdpycmd/cmd/factory/base.py
+-rw-r--r--   0 zhicheng   (501) staff       (20)      937 2023-06-13 12:25:21.000000 bdpycmd-1.3.3/src/bdpycmd/cmd/factory/cmd.py
+-rw-r--r--   0 zhicheng   (501) staff       (20)     8247 2023-06-13 12:25:21.000000 bdpycmd-1.3.3/src/bdpycmd/pycmd.py
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:27:18.166121 bdpycmd-1.3.3/src/bdpycmd.egg-info/
+-rw-r--r--   0 zhicheng   (501) staff       (20)     2066 2023-06-13 12:27:18.000000 bdpycmd-1.3.3/src/bdpycmd.egg-info/PKG-INFO
+-rw-r--r--   0 zhicheng   (501) staff       (20)      413 2023-06-13 12:27:18.000000 bdpycmd-1.3.3/src/bdpycmd.egg-info/SOURCES.txt
+-rw-r--r--   0 zhicheng   (501) staff       (20)        1 2023-06-13 12:27:18.000000 bdpycmd-1.3.3/src/bdpycmd.egg-info/dependency_links.txt
+-rw-r--r--   0 zhicheng   (501) staff       (20)        8 2023-06-13 12:27:18.000000 bdpycmd-1.3.3/src/bdpycmd.egg-info/top_level.txt
```

### Comparing `bdpycmd-1.3.1/PKG-INFO` & `bdpycmd-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdpycmd
-Version: 1.3.1
+Version: 1.3.3
 Summary: Run Python`s file as command line
 Home-page: https://github.com/biandoucheng/bd-py-cmd
 Author: biandoucheng
 Author-email: biandoucheng@outlook.com
 Project-URL: Bug Tracker, https://github.com/biandoucheng/bd-py-cmd/issues
 Project-URL: Use Example, https://github.com/biandoucheng/open-example/tree/main/bdpycmd-example
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `bdpycmd-1.3.1/README.md` & `bdpycmd-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `bdpycmd-1.3.1/setup.cfg` & `bdpycmd-1.3.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = bdpycmd
-version = 1.3.1
+version = 1.3.3
 author = biandoucheng
 author_email = biandoucheng@outlook.com
 description = Run Python`s file as command line
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/biandoucheng/bd-py-cmd
 project_urls =
```

### Comparing `bdpycmd-1.3.1/src/bdpycmd/cmd/camp/assistant.py` & `bdpycmd-1.3.3/src/bdpycmd/cmd/camp/assistant.py`

 * *Files identical despite different names*

### Comparing `bdpycmd-1.3.1/src/bdpycmd/cmd/factory/base.py` & `bdpycmd-1.3.3/src/bdpycmd/cmd/factory/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,20 +20,18 @@
         
         :param alias: str #alias for the command
         :param description: str #a description of the function of the command
         """
         self.name = name.split('.')[-1] + '.Command'
         self.alias = alias + 'command'
         self.description = description
-        self.info = """
-        {name}  {alias} {description}
-        """.format(
-            name=self.name,
-            alias=self.alias,
-            description=self.description
+        self.info = CmdMeta(
+            name=name,
+            alias=alias,
+            desc=description
         )
         #Methods not shown in the help information
         self.protected_methods = {'__init__','as_cmder'}
 
 
     def help(self,m=''):
         """
@@ -41,15 +39,15 @@
         """
         tab = """
         """
         if not isinstance(m,str):
             m = ''
 
         #help output command
-        hps = [self.info]
+        hps = []
 
         #Handling inheritance of command classes
         class_objects = [self.__class__]
         self.deep_clss(self.__class__,class_objects)
 
         #Traverse the object members of the command class and the parent class
         # inherited by the command class to find the command method
@@ -59,14 +57,15 @@
                 k = k.replace(class_name + '_', '')
                 if k in self.protected_methods:
                     continue
                 
                 if not k.startswith('_') and isinstance(v,FunctionType) and v.__name__.endswith('___bdcmder'):
                     hps.append(tab + k + '  ' + str(v.__doc__).lstrip(tab))
 
+        print(self.info.info())
         self.format_print(infos=hps)
 
     def deep_clss(self,obj:object,clss:list):
         """
         Recursively complete inherited class query
         
         :param obj: object #initial class
@@ -111,16 +110,26 @@
         """
         @wraps(fun)
         def wrapper(self,**kwargs):
             args_regex = re.compile(r':param\s([\w]+):',re.DOTALL)
             dc = fun.__doc__
             if not dc:
                 dc = ''
+            
+            fn = f"""
+        {fun.__name__}
+            """
+            print(fn + dc)
+            
             all_arg_names = args_regex.findall(dc)
             target = {}
             for k in all_arg_names:
                 if k in kwargs:
                     target[k] = kwargs[k]
+                else:
+                    vl = input(k + " = ")
+                    if vl:
+                        target[k] = vl
             return fun(self,**target)
 
         wrapper.__name__ = wrapper.__name__ + '___bdcmder'
         return wrapper
```

### Comparing `bdpycmd-1.3.1/src/bdpycmd/cmd/factory/cmd.py` & `bdpycmd-1.3.3/src/bdpycmd/cmd/factory/cmd.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,7 +28,17 @@
         """
         return f"""
         {self.name} ----------------------
                     {self.alias}
                     {self.desc}
                     Number: {self.number}
         """
+
+    def info(self,) -> str:
+        """
+        Describe information
+        """
+        return f"""
+        {self.name} ++++++++++++++++++++++
+                    {self.alias}
+                    {self.desc}
+        """
```

### Comparing `bdpycmd-1.3.1/src/bdpycmd/pycmd.py` & `bdpycmd-1.3.3/src/bdpycmd/pycmd.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,16 +61,14 @@
         
         :param cmd:      parent command name  If this parameter is omitted, the help is called
         :param son:      subcommand name  If this parameter is omitted, help is called
         :param **kwargs: Subcommand arguments Unsupported arguments are filtered out
         """
         tab = """
         """
-        headers = [str(cls.help.__doc__).lstrip(tab),tab+'List of available commands:']
-        
         cmders = []
         for _,v in cls.__INNER_CMD.items():
             cmders.append(v)
         
         numb = 1
         for fh in os.listdir(cls.__CMD_ROOT_DIR):
             if fh.endswith('.py') and os.path.isfile(cls.__CMD_ROOT_DIR+'/'+fh) and fh not in ['__init__.py']:
@@ -84,28 +82,48 @@
                         "alias":n,
                         "desc":n
                     }
                 info["number"] = numb
                 numb += 1
                 cmders.append(CmdMeta(**info))
         
-        print(*headers)
-        cls.search(cms=cmders)
+        print(str(cls.help.__doc__).lstrip(tab))
+        print(tab+'List of available commands:')
+
+        _cmd = cls.search(cms=cmders)
+
+        if not _cmd:
+            msg = """
+        Target command not found
+            """
+            print(msg)
+        else:
+            cls.run(dic_args={
+                "cmd":_cmd
+            })
     
     @classmethod
-    def search(cls,cms:list[CmdMeta]):
+    def search(cls,cms:list) -> str:
         """
         Retrieve command list based on keywords
 
         :param cms: list[CmdMeta] Command Meta Information List
+        :return: str Target Command
         """
         keyword = ""
+        tag_cmd = ""
+        checked = "/"
+        exited = "."
         
         while True:
-            if keyword == "/":
+            if keyword == exited:
+                tag_cmd = ""
+                break
+            
+            if keyword == checked:
                 break
             
             if not keyword:
                 for _cmd in cms:
                     keyword = input(_cmd.say()).strip()
                     if not keyword:
                         continue
@@ -120,14 +138,16 @@
                         keyword = input(_cmd.say()).strip()
                         if not keyword or keyword == _word:
                             continue
                         else:
                             break
                 else:
                     break
+        
+        return tag_cmd
 
     @classmethod
     def chunk_list(cls,ls:list,size:int):
         """
         Group the list by seize
         
         :param ls: list
@@ -205,36 +225,38 @@
             print('command not exists')
             print(traceback.format_exc())
         except Exception as e:
             print('run command failed: %s ' % str(e))
             print(traceback.format_exc())
 
     @classmethod
-    def run(cls):
+    def run(cls,dic_args:dict=None):
         """
         Receive command line arguments and execute commands
         
+        :param dic_args: dict 参数字典
         :return:
         """
         help_list = ['help', 'h', 'hp', 'hlp']
-        dic_args = {}
         args = sys.argv
 
-        # parameter to dictionary
-        if len(args) < 2:
-            dic_args['cmd'] = 'help'
-        else:
-            for it in args[1:]:
-                its = str(it).split('=')
-                if len(its) >= 2:
-                    k = its[0].lstrip('-')
-                    dic_args[k] = '='.join(its[1:]).strip('=')
+        # dictionary parameter determination and input parameter analysis
+        if not isinstance(dic_args,dict) or "cmd" not in dic_args:
+            dic_args = {}
+            if len(args) < 2:
+                dic_args['cmd'] = 'help'
+            else:
+                for it in args[1:]:
+                    its = str(it).split('=')
+                    if len(its) >= 2:
+                        k = its[0].lstrip('-')
+                        dic_args[k] = '='.join(its[1:]).strip('=')
 
-        if 'cmd' not in dic_args:
-            dic_args['cmd'] = 'help'
+            if 'cmd' not in dic_args:
+                dic_args['cmd'] = 'help'
 
         if dic_args['cmd'] in help_list:
             cls.help()
         else:
             if 'son' not in dic_args or dic_args['son'] in help_list or not dic_args['son']:
                 dic_args['son'] = 'help'
                 if 'm' not in dic_args:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bdpycmd-1.3.1/src/bdpycmd.egg-info/PKG-INFO` & `bdpycmd-1.3.3/src/bdpycmd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdpycmd
-Version: 1.3.1
+Version: 1.3.3
 Summary: Run Python`s file as command line
 Home-page: https://github.com/biandoucheng/bd-py-cmd
 Author: biandoucheng
 Author-email: biandoucheng@outlook.com
 Project-URL: Bug Tracker, https://github.com/biandoucheng/bd-py-cmd/issues
 Project-URL: Use Example, https://github.com/biandoucheng/open-example/tree/main/bdpycmd-example
 Classifier: Programming Language :: Python :: 3.5
```

