# Comparing `tmp/gggifcheck-0.0.3.tar.gz` & `tmp/gggifcheck-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gggifcheck-0.0.3.tar", last modified: Wed Apr 26 11:05:12 2023, max compression
+gzip compressed data, was "gggifcheck-0.0.4.tar", last modified: Tue Jun 13 10:35:15 2023, max compression
```

## Comparing `gggifcheck-0.0.3.tar` & `gggifcheck-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 11:05:12.592520 gggifcheck-0.0.3/
--rw-rw-rw-   0        0        0     1088 2023-03-27 06:45:03.000000 gggifcheck-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     5394 2023-04-26 11:05:12.593519 gggifcheck-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     4684 2023-04-26 10:42:11.000000 gggifcheck-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-26 11:05:12.587380 gggifcheck-0.0.3/gggifcheck/
--rw-rw-rw-   0        0        0       86 2023-04-13 04:29:58.000000 gggifcheck-0.0.3/gggifcheck/__init__.py
--rw-rw-rw-   0        0        0    11566 2023-04-25 02:42:29.000000 gggifcheck-0.0.3/gggifcheck/fields.py
--rw-rw-rw-   0        0        0     7101 2023-04-26 10:39:56.000000 gggifcheck-0.0.3/gggifcheck/items.py
--rw-rw-rw-   0        0        0     3331 2023-04-24 11:22:06.000000 gggifcheck-0.0.3/gggifcheck/scrapy_ifcheck.py
-drwxrwxrwx   0        0        0        0 2023-04-26 11:05:12.592520 gggifcheck-0.0.3/gggifcheck.egg-info/
--rw-rw-rw-   0        0        0     5394 2023-04-26 11:05:12.000000 gggifcheck-0.0.3/gggifcheck.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-04-26 11:05:12.000000 gggifcheck-0.0.3/gggifcheck.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 11:05:12.000000 gggifcheck-0.0.3/gggifcheck.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-26 11:05:12.000000 gggifcheck-0.0.3/gggifcheck.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      770 2023-04-26 11:05:12.598405 gggifcheck-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      164 2023-04-13 03:43:33.000000 gggifcheck-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 10:35:15.330286 gggifcheck-0.0.4/
+-rw-rw-rw-   0        0        0     1088 2023-03-27 06:45:03.000000 gggifcheck-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     4570 2023-06-13 10:35:15.330286 gggifcheck-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3854 2023-06-13 09:33:39.000000 gggifcheck-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 10:35:15.325299 gggifcheck-0.0.4/gggifcheck/
+-rw-rw-rw-   0        0        0       86 2023-04-13 04:29:58.000000 gggifcheck-0.0.4/gggifcheck/__init__.py
+-rw-rw-rw-   0        0        0    12065 2023-06-13 09:17:54.000000 gggifcheck-0.0.4/gggifcheck/fields.py
+-rw-rw-rw-   0        0        0     7132 2023-06-13 09:29:52.000000 gggifcheck-0.0.4/gggifcheck/items.py
+-rw-rw-rw-   0        0        0     2631 2023-06-13 09:29:52.000000 gggifcheck-0.0.4/gggifcheck/scrapy_ifcheck.py
+drwxrwxrwx   0        0        0        0 2023-06-13 10:35:15.329289 gggifcheck-0.0.4/gggifcheck.egg-info/
+-rw-rw-rw-   0        0        0     4570 2023-06-13 10:35:15.000000 gggifcheck-0.0.4/gggifcheck.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-06-13 10:35:15.000000 gggifcheck-0.0.4/gggifcheck.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 10:35:15.000000 gggifcheck-0.0.4/gggifcheck.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-13 10:35:15.000000 gggifcheck-0.0.4/gggifcheck.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      774 2023-06-13 10:35:15.332280 gggifcheck-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      164 2023-04-13 03:43:33.000000 gggifcheck-0.0.4/setup.py
```

### Comparing `gggifcheck-0.0.3/LICENSE` & `gggifcheck-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gggifcheck-0.0.3/PKG-INFO` & `gggifcheck-0.0.4/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: gggifcheck
-Version: 0.0.3
-Summary: 通用、便捷、准确的字符串时间解析工具
-Home-page: https://github.com/kusen-alpha/gggifcheck
-Author: kusen
-Author-email: hu1194542196@qq.com
-License: MIT
-Project-URL: Bug Tracker, https://github.com/kusen-alpha/gggifcheck/issues
-Project-URL: Documentation, https://github.com/kusen-alpha/gggifcheck/blob/master/README.md
-Project-URL: Source Code, https://github.com/kusen-alpha/gggifcheck
-Platform: any
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # gggifcheck
 
 通用条目字段检查(General General General Item Field Check)
 ，是基于Python编写通用检查工具，适应于各种场景的使用，只需要略微进行适配。
 
 ## 使用方法
 
@@ -45,19 +27,17 @@
 ### 使用CheckItem
 
 ```python
 from gggifcheck import fields, items
 
 
 class TestCheckItem(items.CheckItem):
-    a = items.BuildCheckField(
-        check_field_class=fields.StringCheckField, min_length=1, 
+    a = fields.StringCheckField(min_length=1, 
         max_length=2, contains=['a'], excludes=['b'])
-    b = items.BuildCheckField(
-        check_field_class=fields.StringCheckField, min_length=1, 
+    b = fields.StringCheckField(min_length=1, 
         max_length=2, contains=['a'], excludes=['c'])
 
 
 item = TestCheckItem()
 item['a'] = 'aa'
 item['b'] = 'ab'
 print(dict(item))
@@ -67,22 +47,22 @@
 
 ### 结合scrapy
 
 ```python
 # 对scrapy Item进行改写
 import scrapy
 from gggifcheck import fields
-from gggifcheck.items import CheckItem, BuildCheckField
+from gggifcheck.items import CheckItem
 
 
 class ScrapyCheckItem(scrapy.Item, CheckItem):
 
     def __init__(self, *args, **kwargs):
         self._values = {}
-        self.check_fields = {}
+        self._base_values = {}
         if args or kwargs:
             for k, v in dict(*args, **kwargs).items():
                 self[k] = v
 
     def __getitem__(self, key):
         if key in self.fields and key not in self._values:
             value = None
@@ -90,28 +70,29 @@
                 value = self[field2]
                 break
             self[key] = value
         return self._values[key]
 
     def __setitem__(self, key, value):
         if key in self.fields:
+            self._base_values[key] = value
             field = self.fields[key]
-            build_check_field = field.get('build_check_field')
-            if build_check_field:
-                check_field = build_check_field.build(key=key, value=value)
-                self.check_fields[key] = check_field
-                self._values[key] = check_field.value
+            check_field = field.get('check_field')
+            if isinstance(check_field, fields.CheckField):
+                fe = check_field.from_instance()
+                fe.input(key, value)
+                self._values[key] = fe.value
             else:
                 self._values[key] = value
         else:
             raise KeyError(
                 f"{self.__class__.__name__} does not support field: {key}")
 
     def __setattr__(self, name, value):
-        if name.startswith('_') or name in ['check_fields']:
+        if name.startswith('_'):
             self.__dict__[name] = value
         else:
             raise AttributeError(
                 f"Use item[{name!r}] = {value!r} to set field value")
 
     def check_all(self):
         """
@@ -125,44 +106,27 @@
         # 不能放在此处验证的原因是scrapy item进入pipeline前有日志打印等操作导致进行
         # 此处验证，导致如果在pipeline里进行透传时验证不生效，提前检查报错，此处验证放
         # 在check_all方法中，因此需要手动调用
         # self._process_and_check()
         # _ = [self[field] for field in self.fields]  # 进行所有字段检查
         return self._values.keys()
 
-    def get_base_value(self, key):
-        if key in self.check_fields:
-            return self.check_fields[key].base_value
-        elif key in self.fields:
-            field = self.fields[key]
-            build_check_field = field.get('build_check_field')
-            if build_check_field:
-                return build_check_field.build_default(
-                    key=key, value=None).base_value
-            return self.fields[key] or None
-        else:
-            raise KeyError(
-                f"{self.__class__.__name__} does not support field: {key}")
-
-
 # 示例
 class PostItem(ScrapyCheckItem):
     id = scrapy.Field(
-        build_check_field=BuildCheckField(
-            check_field_class=fields.MD5CheckField, nullable=False))
+        check_field=fields.MD5CheckField(nullable=False))
     channel = scrapy.Field(
-        build_check_field=BuildCheckField(
-            check_field_class=fields.IntegerCheckField,
+        check_field=fields.IntegerCheckField(
             nullable=False, min_value=1, max_value=6))
 
 
 item = PostItem()
 item['id'] = '81dc9bdb52d04dc20036dbd8313ed055'
 item['channel'] = 1
 print(dict(item))
 ```
 
 ## 关于作者
 
 1. 邮箱：1194542196@qq.com
 2. 微信：hu1194542196
-3. 目前还需要很多需要改进的地方，可以私信作者，你们的提供越多，本库才能更完善。
+3. 目前还需要很多需要改进的地方，可以私信作者，你们的提供越多，本库才能更完善。
```

### Comparing `gggifcheck-0.0.3/gggifcheck/fields.py` & `gggifcheck-0.0.4/gggifcheck/fields.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 # -*- coding:utf-8 -*-
 # author: kusen
 # email: 1194542196@qq.com
 # date: 2023/4/13
-
-
+import copy
 import re
 import sys
 import datetime
 
 
-class CheckField(object):
+class Filed(object):
+    """
+    普通Field，不进行检查
+    """
+    pass
+
+
+class CheckField(Filed):
     def __init__(self, key=None, value=None, default=None,
                  nullable=True, choices=None, types=None):
         """
 
         :param default: 默认值
         :param nullable: 是否能为None
         :param choices: 必须为其中一个
@@ -28,14 +34,26 @@
         if not isinstance(types, (tuple, list)):
             types = (types,)
         self.types = types
         self._check_args()  # 检查初始参数合法性
         self._type_checked = True  # 类型是否检查
         self._input_checked = False  # input方法对_value进行检查与否
 
+    def from_instance(self):
+        """
+        使用场景：开始创建一个实例模板，后续通过该模板进行多次独立进行检查
+        :return:
+        """
+        new = copy.deepcopy(self)
+        new.key = None
+        new._value = None
+        new._type_checked = True
+        new._input_checked = False
+        return new
+
     def input(self, key, value=None):
         self.key = key
         self._value = value
         self.check()
         self._input_checked = True
 
     def output(self):
@@ -73,15 +91,16 @@
     def _check_types(self):
         if self._value is None:
             return []
         if not isinstance(self._value, self.types):
             self._type_checked = False
             error_msg = ('Field %s input: %s, the type is %s, is not '
                          'types: %s') % (
-                self.key, self._value, type(self._value), self.types)
+                            self.key, self._value, type(self._value),
+                            self.types)
             return [Exception(error_msg)]
         return []
 
     def _check_choices(self):
         if self.choices and self._value not in self.choices:
             error_msg = 'Field %s intput: %s, is not in choices: %s' % (
                 self.key, self._value, self.choices)
```

### Comparing `gggifcheck-0.0.3/gggifcheck/items.py` & `gggifcheck-0.0.4/gggifcheck/items.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,55 +3,58 @@
 # email: 1194542196@qq.com
 # date: 2023/4/13
 
 
 import itertools
 from collections.abc import MutableMapping
 
+from .fields import Filed, CheckField
+
 
 class ItemMeta(object):
     def __new__(cls, *args, **kwargs):
-        build_fields = {}
+        fields = {}
         for n in dir(cls):
             v = getattr(cls, n)
-            if isinstance(v, BuildCheckField):
-                build_fields[n] = v
-        cls.build_fields = build_fields
+            if isinstance(v, Filed):
+                fields[n] = v
+        cls.fields = fields
         return super().__new__(cls)
 
 
 class CheckItem(MutableMapping, ItemMeta):
     relate_process_default = []  # 关联处理字段间互相取默认值
     relate_check_null = []  # 关联检查字段间互相是否为None
     relate_check_sequence_length = []  # 关联检查序列字段间互相长度判断
     relate_check_startswith = []  # 关联检查字符串字段间互相startswith关系
     relate_check_endswith = []  # 关联检查字符串字段间互相endswith关系
     relate_check_contains = []  # 关联检查字符串字段间互相包含关系
     bundle_errors = []  # 是否一次性返回所有错误，暂时没有使用该字段
 
     def __init__(self, *args, **kwargs):
-        self.check_fields = {}
+        self._values = {}
+        self._base_values = {}
         if args or kwargs:
             for k, v in dict(*args, **kwargs).items():
                 self[k] = v
 
     def process(self):
         for key in itertools.chain(self._get_config_attr_names(),
-                                   self.build_fields.keys()):
+                                   self.fields.keys()):
             field_name = key
             if not key.startswith('_'):
                 field_name = '_' + field_name
             process_method_name = '_process' + field_name
             if not hasattr(self, process_method_name):
                 continue
             getattr(self, process_method_name)()
 
     def check(self):
         for key in itertools.chain(self._get_config_attr_names(),
-                                   self.build_fields.keys()):
+                                   self.fields.keys()):
             field_name = key
             if not key.startswith('_'):
                 field_name = '_' + field_name
             check_method_name = '_check' + field_name
             if not hasattr(self, check_method_name):
                 continue
             getattr(self, check_method_name)()
@@ -117,70 +120,69 @@
         for k in dir(self.__class__):
             if k.startswith('relate_process_') or k.startswith(
                     'relate_check_') or k == 'bundle_errors':
                 attr_names.append(k)
         return attr_names
 
     def __setitem__(self, key, value):
-        if key in self.build_fields:
-            self.check_fields[key] = self.build_fields[key].build(
-                key=key, value=value)
+        self._base_values[key] = value
+        if key in self.fields:
+            if isinstance(self.fields[key], CheckField):
+                fe = self.fields[key].from_instance()
+                fe.input(key, value)
+                self._values[key] = fe.value
+            else:
+                self._values[key] = value
         else:
             raise KeyError(
                 f"{self.__class__.__name__} does not support field: {key}")
 
     def __getitem__(self, key):
-        if key in self.check_fields:
-            field = self.check_fields[key]
-            if not field.key:
-                field.key = key
-            return self.check_fields[key].value
+        if key in self._values:
+            return self._values[key]
+        elif key in self.fields:
+            self[key] = None
+            return self[key]
         elif key in self.__dict__:
             return self.__dict__[key]
         else:
             raise KeyError(
                 f"{self.__class__.__name__} does not have field: {key}")
 
     def __delitem__(self, key):
-        del self.check_fields[key]
+        del self._values[key]
 
     def __len__(self):
         return len(self.__dict__.keys())
 
     def __iter__(self):
         self._process_and_check()
-        return iter(self.build_fields)
+        return iter(self.fields)
 
     def _process_and_check(self):
         self.process()
         self.check()
 
     def __getattr__(self, name):
         if name in self.__dict__:
             return self.__dict__[name]
         raise AttributeError(f"Use item[{name!r}] to get field value")
 
     def __setattr__(self, name, value):
-        if name in self.__dict__ or name in ['check_fields']:
+        if name in self.__dict__ or name in ['_values', '_base_values']:
             self.__dict__[name] = value
         else:
             raise AttributeError(
                 f"Use item[{name!r}] = {value!r} to set field value")
 
     def keys(self):  # to dict时优先调用，不会调用__iter__和__len__，但必须实现
         self._process_and_check()
-        return self.build_fields.keys()
-
-
-class BuildCheckField(object):
-    def __init__(self, check_field_class, **kwargs):
-        self.check_field_class = check_field_class
-        self.kwargs = kwargs
-
-    def build(self, key, value):
-        check_field = self.check_field_class(**self.kwargs)
-        check_field.input(key, value)
-        return check_field
-
-    def build_default(self, key, value=None):
-        return self.check_field_class(
-            key=key, value=value, **self.kwargs)
+        keys = self.fields.keys()
+        _ = [self[field] for field in keys]  # 补全所有字段数据
+        return keys
+
+    def get_base_value(self, key):
+        if key in self._base_values:
+            return self._base_values[key]
+        else:
+            raise KeyError(
+                f"{self.__class__.__name__} does not support field: {key}")
```

### Comparing `gggifcheck-0.0.3/gggifcheck/scrapy_ifcheck.py` & `gggifcheck-0.0.4/gggifcheck/scrapy_ifcheck.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,17 @@
-# -*- coding:utf-8 -*-
-# author: kusen
-# email: 1194542196@qq.com
-# date: 2023/4/13
-
-
 import scrapy
-
 from gggifcheck import fields
 from gggifcheck.items import CheckItem
 
 
 class ScrapyCheckItem(scrapy.Item, CheckItem):
 
     def __init__(self, *args, **kwargs):
         self._values = {}
-        self.check_fields = {}
+        self._base_values = {}
         if args or kwargs:
             for k, v in dict(*args, **kwargs).items():
                 self[k] = v
 
     def __getitem__(self, key):
         if key in self.fields and key not in self._values:
             value = None
@@ -26,28 +19,29 @@
                 value = self[field2]
                 break
             self[key] = value
         return self._values[key]
 
     def __setitem__(self, key, value):
         if key in self.fields:
+            self._base_values[key] = value
             field = self.fields[key]
-            build_check_field = field.get('build_check_field')
-            if build_check_field:
-                check_field = build_check_field.build(key=key, value=value)
-                self.check_fields[key] = check_field
-                self._values[key] = check_field.value
+            check_field = field.get('check_field')
+            if isinstance(check_field, fields.CheckField):
+                fe = check_field.from_instance()
+                fe.input(key, value)
+                self._values[key] = fe.value
             else:
                 self._values[key] = value
         else:
             raise KeyError(
                 f"{self.__class__.__name__} does not support field: {key}")
 
     def __setattr__(self, name, value):
-        if name.startswith('_') or name in ['check_fields']:
+        if name.startswith('_'):
             self.__dict__[name] = value
         else:
             raise AttributeError(
                 f"Use item[{name!r}] = {value!r} to set field value")
 
     def check_all(self):
         """
@@ -61,36 +55,24 @@
         # 不能放在此处验证的原因是scrapy item进入pipeline前有日志打印等操作导致进行
         # 此处验证，导致如果在pipeline里进行透传时验证不生效，提前检查报错，此处验证放
         # 在check_all方法中，因此需要手动调用
         # self._process_and_check()
         # _ = [self[field] for field in self.fields]  # 进行所有字段检查
         return self._values.keys()
 
-    def get_base_value(self, key):
-        if key in self.check_fields:
-            return self.check_fields[key].base_value
-        elif key in self.fields:
-            field = self.fields[key]
-            build_check_field = field.get('build_check_field')
-            if build_check_field:
-                return build_check_field.build_default(
-                    key=key, value=None).base_value
-            return self.fields[key] or None
-        else:
-            raise KeyError(
-                f"{self.__class__.__name__} does not support field: {key}")
-
-
-if __name__ == '__main__':
-    class PostItem(ScrapyCheckItem):
-        id = scrapy.Field(
-            check_field=fields.MD5CheckField(
-                nullable=False))
-        channel = scrapy.Field(
-            check_field=fields.IntegerCheckField(nullable=False, min_value=1,
-                                                 max_value=6))
-
 
-    item = PostItem()
-    item['id'] = '81dc9bdb52d04dc20036dbd8313ed055'
-    item['channel'] = 1
-    print(dict(item))
+# 示例
+class PostItem(ScrapyCheckItem):
+    relate_process_default = [('channel', 'id')]
+    id = scrapy.Field(
+        check_field=fields.MD5CheckField(nullable=False))
+    channel = scrapy.Field(
+        check_field=fields.IntegerCheckField(
+            nullable=False, min_value=1, max_value=6))
+
+
+item = PostItem()
+item['id'] = '81dc9bdb52d04dc20036dbd8313ed055'
+item['channel'] = 1
+item.check_all()
+print(dict(item))
+print(item.get_base_value('id'))
```

### Comparing `gggifcheck-0.0.3/setup.cfg` & `gggifcheck-0.0.4/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2067 6767 6966 6368 6563 6b0d 0a76   = gggifcheck..v
-00000020: 6572 7369 6f6e 203d 2030 2e30 2e33 0d0a  ersion = 0.0.3..
+00000020: 6572 7369 6f6e 203d 2030 2e30 2e34 0d0a  ersion = 0.0.4..
 00000030: 6175 7468 6f72 203d 206b 7573 656e 0d0a  author = kusen..
 00000040: 6175 7468 6f72 5f65 6d61 696c 203d 2068  author_email = h
 00000050: 7531 3139 3435 3432 3139 3640 7171 2e63  u1194542196@qq.c
 00000060: 6f6d 0d0a 6465 7363 7269 7074 696f 6e20  om..description 
-00000070: 3d20 cda8 d3c3 a1a2 b1e3 bddd a1a2 d7bc  = ..............
-00000080: c8b7 b5c4 d7d6 b7fb b4ae cab1 bce4 bde2  ................
-00000090: cef6 b9a4 bedf 0d0a 6c6f 6e67 5f64 6573  ........long_des
-000000a0: 6372 6970 7469 6f6e 203d 2066 696c 653a  cription = file:
-000000b0: 2052 4541 444d 452e 6d64 0d0a 6c6f 6e67   README.md..long
-000000c0: 5f64 6573 6372 6970 7469 6f6e 5f63 6f6e  _description_con
-000000d0: 7465 6e74 5f74 7970 6520 3d20 7465 7874  tent_type = text
-000000e0: 2f6d 6172 6b64 6f77 6e0d 0a6c 6963 656e  /markdown..licen
-000000f0: 7365 203d 204d 4954 0d0a 6c69 6365 6e73  se = MIT..licens
-00000100: 655f 6669 6c65 7320 3d20 4c49 4345 4e53  e_files = LICENS
-00000110: 450d 0a75 726c 203d 2068 7474 7073 3a2f  E..url = https:/
-00000120: 2f67 6974 6875 622e 636f 6d2f 6b75 7365  /github.com/kuse
-00000130: 6e2d 616c 7068 612f 6767 6769 6663 6865  n-alpha/gggifche
-00000140: 636b 0d0a 706c 6174 666f 726d 7320 3d20  ck..platforms = 
-00000150: 616e 790d 0a70 726f 6a65 6374 5f75 726c  any..project_url
-00000160: 7320 3d20 0d0a 0942 7567 2054 7261 636b  s = ...Bug Track
-00000170: 6572 203d 2068 7474 7073 3a2f 2f67 6974  er = https://git
-00000180: 6875 622e 636f 6d2f 6b75 7365 6e2d 616c  hub.com/kusen-al
-00000190: 7068 612f 6767 6769 6663 6865 636b 2f69  pha/gggifcheck/i
-000001a0: 7373 7565 730d 0a09 446f 6375 6d65 6e74  ssues...Document
-000001b0: 6174 696f 6e20 3d20 6874 7470 733a 2f2f  ation = https://
-000001c0: 6769 7468 7562 2e63 6f6d 2f6b 7573 656e  github.com/kusen
-000001d0: 2d61 6c70 6861 2f67 6767 6966 6368 6563  -alpha/gggifchec
-000001e0: 6b2f 626c 6f62 2f6d 6173 7465 722f 5245  k/blob/master/RE
-000001f0: 4144 4d45 2e6d 640d 0a09 536f 7572 6365  ADME.md...Source
-00000200: 2043 6f64 6520 3d20 6874 7470 733a 2f2f   Code = https://
-00000210: 6769 7468 7562 2e63 6f6d 2f6b 7573 656e  github.com/kusen
-00000220: 2d61 6c70 6861 2f67 6767 6966 6368 6563  -alpha/gggifchec
-00000230: 6b0d 0a63 6c61 7373 6966 6965 7273 203d  k..classifiers =
-00000240: 200d 0a09 5072 6f67 7261 6d6d 696e 6720   ...Programming 
-00000250: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000260: 6f6e 203a 3a20 330d 0a09 4c69 6365 6e73  on :: 3...Licens
-00000270: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
-00000280: 6420 3a3a 204d 4954 204c 6963 656e 7365  d :: MIT License
-00000290: 0d0a 094f 7065 7261 7469 6e67 2053 7973  ...Operating Sys
-000002a0: 7465 6d20 3a3a 204f 5320 496e 6465 7065  tem :: OS Indepe
-000002b0: 6e64 656e 740d 0a0d 0a5b 6f70 7469 6f6e  ndent....[option
-000002c0: 735d 0d0a 7061 636b 6167 6573 203d 2066  s]..packages = f
-000002d0: 696e 643a 0d0a 0d0a 5b65 6767 5f69 6e66  ind:....[egg_inf
-000002e0: 6f5d 0d0a 7461 675f 6275 696c 6420 3d20  o]..tag_build = 
-000002f0: 0d0a 7461 675f 6461 7465 203d 2030 0d0a  ..tag_date = 0..
-00000300: 0d0a                                     ..
+00000070: 3d20 cda8 d3c3 ccf5 c4bf d7d6 b6ce bcec  = ..............
+00000080: b2e9 a3ac caca d3a6 d3da b8f7 d6d6 b3a1  ................
+00000090: beb0 b5c4 cab9 d3c3 a1a3 0d0a 6c6f 6e67  ............long
+000000a0: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
+000000b0: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
+000000c0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
+000000d0: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
+000000e0: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a6c  text/markdown..l
+000000f0: 6963 656e 7365 203d 204d 4954 0d0a 6c69  icense = MIT..li
+00000100: 6365 6e73 655f 6669 6c65 7320 3d20 4c49  cense_files = LI
+00000110: 4345 4e53 450d 0a75 726c 203d 2068 7474  CENSE..url = htt
+00000120: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000130: 6b75 7365 6e2d 616c 7068 612f 6767 6769  kusen-alpha/gggi
+00000140: 6663 6865 636b 0d0a 706c 6174 666f 726d  fcheck..platform
+00000150: 7320 3d20 616e 790d 0a70 726f 6a65 6374  s = any..project
+00000160: 5f75 726c 7320 3d20 0d0a 0942 7567 2054  _urls = ...Bug T
+00000170: 7261 636b 6572 203d 2068 7474 7073 3a2f  racker = https:/
+00000180: 2f67 6974 6875 622e 636f 6d2f 6b75 7365  /github.com/kuse
+00000190: 6e2d 616c 7068 612f 6767 6769 6663 6865  n-alpha/gggifche
+000001a0: 636b 2f69 7373 7565 730d 0a09 446f 6375  ck/issues...Docu
+000001b0: 6d65 6e74 6174 696f 6e20 3d20 6874 7470  mentation = http
+000001c0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6b  s://github.com/k
+000001d0: 7573 656e 2d61 6c70 6861 2f67 6767 6966  usen-alpha/gggif
+000001e0: 6368 6563 6b2f 626c 6f62 2f6d 6173 7465  check/blob/maste
+000001f0: 722f 5245 4144 4d45 2e6d 640d 0a09 536f  r/README.md...So
+00000200: 7572 6365 2043 6f64 6520 3d20 6874 7470  urce Code = http
+00000210: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6b  s://github.com/k
+00000220: 7573 656e 2d61 6c70 6861 2f67 6767 6966  usen-alpha/gggif
+00000230: 6368 6563 6b0d 0a63 6c61 7373 6966 6965  check..classifie
+00000240: 7273 203d 200d 0a09 5072 6f67 7261 6d6d  rs = ...Programm
+00000250: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000260: 5079 7468 6f6e 203a 3a20 330d 0a09 4c69  Python :: 3...Li
+00000270: 6365 6e73 6520 3a3a 204f 5349 2041 7070  cense :: OSI App
+00000280: 726f 7665 6420 3a3a 204d 4954 204c 6963  roved :: MIT Lic
+00000290: 656e 7365 0d0a 094f 7065 7261 7469 6e67  ense...Operating
+000002a0: 2053 7973 7465 6d20 3a3a 204f 5320 496e   System :: OS In
+000002b0: 6465 7065 6e64 656e 740d 0a0d 0a5b 6f70  dependent....[op
+000002c0: 7469 6f6e 735d 0d0a 7061 636b 6167 6573  tions]..packages
+000002d0: 203d 2066 696e 643a 0d0a 0d0a 5b65 6767   = find:....[egg
+000002e0: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
+000002f0: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
+00000300: 2030 0d0a 0d0a                            0....
```

