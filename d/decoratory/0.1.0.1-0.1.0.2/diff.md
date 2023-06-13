# Comparing `tmp/decoratory-0.1.0.1.tar.gz` & `tmp/decoratory-0.1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decoratory-0.1.0.1.tar", last modified: Mon Jun 12 12:50:24 2023, max compression
+gzip compressed data, was "decoratory-0.1.0.2.tar", last modified: Tue Jun 13 16:28:40 2023, max compression
```

## Comparing `decoratory-0.1.0.1.tar` & `decoratory-0.1.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 12:50:24.058247 decoratory-0.1.0.1/
--rw-rw-rw-   0        0        0     2550 2023-06-02 20:50:35.000000 decoratory-0.1.0.1/License.txt
--rw-rw-rw-   0        0        0    16170 2023-06-12 12:50:24.058247 decoratory-0.1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    14568 2023-06-12 11:38:10.000000 decoratory-0.1.0.1/Readme.rst
--rw-rw-rw-   0        0        0        0 2023-06-10 04:00:34.000000 decoratory-0.1.0.1/Requirements.txt
-drwxrwxrwx   0        0        0        0 2023-06-12 12:50:23.757437 decoratory-0.1.0.1/Sources/
-drwxrwxrwx   0        0        0        0 2023-06-12 12:50:24.011380 decoratory-0.1.0.1/Sources/decoratory/
--rw-rw-rw-   0        0        0      249 2023-06-07 18:32:49.000000 decoratory-0.1.0.1/Sources/decoratory/__init__.py
--rw-rw-rw-   0        0        0     5084 2023-06-12 12:49:52.000000 decoratory-0.1.0.1/Sources/decoratory/__main__.py
--rw-rw-rw-   0        0        0     4938 2023-06-12 12:49:52.000000 decoratory-0.1.0.1/Sources/decoratory/banner.py
--rw-rw-rw-   0        0        0    14035 2023-06-12 12:49:52.000000 decoratory-0.1.0.1/Sources/decoratory/basic.py
--rw-rw-rw-   0        0        0    20586 2023-06-12 12:49:52.000000 decoratory-0.1.0.1/Sources/decoratory/multiton.py
--rw-rw-rw-   0        0        0    38553 2023-06-12 12:49:52.000000 decoratory-0.1.0.1/Sources/decoratory/observer.py
--rw-rw-rw-   0        0        0     7107 2023-06-12 12:49:52.000000 decoratory-0.1.0.1/Sources/decoratory/singleton.py
--rw-rw-rw-   0        0        0    12164 2023-06-12 12:49:52.000000 decoratory-0.1.0.1/Sources/decoratory/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-06-12 12:50:24.058247 decoratory-0.1.0.1/Sources/decoratory.egg-info/
--rw-rw-rw-   0        0        0    16170 2023-06-12 12:50:23.000000 decoratory-0.1.0.1/Sources/decoratory.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      459 2023-06-12 12:50:23.000000 decoratory-0.1.0.1/Sources/decoratory.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 12:50:23.000000 decoratory-0.1.0.1/Sources/decoratory.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-12 12:50:23.000000 decoratory-0.1.0.1/Sources/decoratory.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 12:50:24.058247 decoratory-0.1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     3929 2023-06-12 12:49:52.000000 decoratory-0.1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 16:28:40.070139 decoratory-0.1.0.2/
+-rw-rw-rw-   0        0        0     2550 2023-06-02 20:50:35.000000 decoratory-0.1.0.2/License.txt
+-rw-rw-rw-   0        0        0    18742 2023-06-13 16:28:40.070139 decoratory-0.1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    17129 2023-06-13 16:02:11.000000 decoratory-0.1.0.2/Readme.rst
+-rw-rw-rw-   0        0        0        0 2023-06-10 04:00:34.000000 decoratory-0.1.0.2/Requirements.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 16:28:40.038891 decoratory-0.1.0.2/Sources/
+drwxrwxrwx   0        0        0        0 2023-06-13 16:28:40.070139 decoratory-0.1.0.2/Sources/decoratory/
+-rw-rw-rw-   0        0        0      249 2023-06-07 18:32:49.000000 decoratory-0.1.0.2/Sources/decoratory/__init__.py
+-rw-rw-rw-   0        0        0     4621 2023-06-13 16:28:13.000000 decoratory-0.1.0.2/Sources/decoratory/__main__.py
+-rw-rw-rw-   0        0        0     4855 2023-06-13 16:03:52.000000 decoratory-0.1.0.2/Sources/decoratory/banner.py
+-rw-rw-rw-   0        0        0    14154 2023-06-13 16:03:52.000000 decoratory-0.1.0.2/Sources/decoratory/basic.py
+-rw-rw-rw-   0        0        0    20586 2023-06-12 14:51:04.000000 decoratory-0.1.0.2/Sources/decoratory/multiton.py
+-rw-rw-rw-   0        0        0    38553 2023-06-12 12:49:52.000000 decoratory-0.1.0.2/Sources/decoratory/observer.py
+-rw-rw-rw-   0        0        0     7107 2023-06-13 15:03:41.000000 decoratory-0.1.0.2/Sources/decoratory/singleton.py
+-rw-rw-rw-   0        0        0    14020 2023-06-13 16:23:56.000000 decoratory-0.1.0.2/Sources/decoratory/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-06-13 16:28:40.070139 decoratory-0.1.0.2/Sources/decoratory.egg-info/
+-rw-rw-rw-   0        0        0    18742 2023-06-13 16:28:40.000000 decoratory-0.1.0.2/Sources/decoratory.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      459 2023-06-13 16:28:40.000000 decoratory-0.1.0.2/Sources/decoratory.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 16:28:40.000000 decoratory-0.1.0.2/Sources/decoratory.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-13 16:28:40.000000 decoratory-0.1.0.2/Sources/decoratory.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 16:28:40.070139 decoratory-0.1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     3944 2023-06-13 16:28:13.000000 decoratory-0.1.0.2/setup.py
```

### Comparing `decoratory-0.1.0.1/License.txt` & `decoratory-0.1.0.2/License.txt`

 * *Files identical despite different names*

### Comparing `decoratory-0.1.0.1/PKG-INFO` & `decoratory-0.1.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: decoratory
-Version: 0.1.0.1
+Version: 0.1.0.2
 Summary: Decorators: Singleton, Multiton, Observer, generic Wrapper.
 Home-page: http://evation.eu
 Download-URL: http://evation.eu
 Author: Martin Abel
 Author-email: Martin Abel <python@evation.eu>
 Maintainer: Martin Abel
 Maintainer-email: Martin Abel <python@evation.eu>
 License: PSF
 Project-URL: Projekt, http://evation.eu
 Project-URL: Release Notes, http://evation.eu
 Project-URL: Download, http://evation.eu
-Keywords: decorator singleton multiton observer wrapper
+Keywords: decorator singleton multiton observer observable wrapper
 Platform: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
 Classifier: Natural Language :: English
@@ -44,66 +44,66 @@
 Decoratory
 ==============================================================================
 
 
 **Introduction**
 
 The "decoratory" package is based on the `Decorator Arguments Pattern`_, an 
-integrated concept for Python decorators with and without parameters. Thus 
-all decorators created with it support complex arguments, e.g. lists of 
-values and functions, without unnecessarily complicating the decoration of 
-simple cases by these extensions. All implementation details are described 
-on the `project homepage`_.
+integrated concept for Python decorators with and without parameters. In
+addition, all decorators created with it support complex arguments, e.g. 
+lists of values and functions, without unnecessarily complicating the 
+decoration of simple cases by these extensions. All implementation details 
+are described on the `project homepage`_.
 
 
 **Installation** ::
 
-    pip install decoratory
+    pip install --upgrade decoratory
 
 After installation, basic information about the package, the individual 
 modules and their methods is also available from the command line. ::
 
     python -m decoratory --help
 
 
-**Content**
+**Package Content**
 
-The "decoratory" package available here includes some classic decorators
+The decoratory package available here includes some classic decorators
 implemented and functionally extended with this concept, e.g.
 
 * `Singleton`_
 * `Multiton`_
 * `Wrapper`_
 * `Observer`_   (coming soon...)
 
-This is an open list that will grow over time.
+This is an open list that possibly will grow over time.
 
 
 **Description**
 
 To illustrate the functionality of each module, a simple as well as a 
-possibly more complex example is presented. Even if only one particular module 
+more complex example is presented. Even if only one particular module 
 is needed, it is recommended to view the preceding examples as well. For even
-more examples of the full range of possibilities, again, please refer to the 
+more examples of the full range of possibilities, please refer to the 
 `project homepage`_.
 
 
 ******************************************************************************
 Singleton
 ******************************************************************************
 
 A `singleton pattern`_ is a design pattern that limits the instantiation of 
 a class to a single (unique) instance. This is useful when exactly one unique 
 object is needed i.e. to manage an expensive resource or coordinate actions 
 across modules.
 
-As a simple example serves the decoration of the class  ``Animal`` as singleton. 
-In the context of the `Decorator Arguments Pattern`_, this can be done both 
-without brackets (class) and with brackets (object, instance), because both 
-notations describe the same functionality.
+As a simple example serves the decoration of the class  ``Animal`` as 
+singleton. In the context of the `Decorator Arguments Pattern`_, this can be 
+done both without brackets (decorator class) and with brackets (decorator 
+instance), meaning both notations describe the same functional situation.
 
 .. code-block:: python
    
     # *** example_singleton.py - class Animal with Singleton decoration
 
     from decoratory.singleton import Singleton
 
@@ -111,42 +111,36 @@
     class Animal:
         def __init__(self, name):
             self.name = name
 
         def __repr__(self):
             return f"{self.__class__.__name__}('{self.name}')"
 
-If instances of the class ``Animal`` are now created, this is only done for the 
-very first instantiation, and for all further instantiations always this 
-"primary instance" is given back.
-            
-.. code-block:: python
-   
-    # *** example_singleton.py - creation of instances
-
     # Create Instances
     a = Animal(name='Bello')        # Creates Bello
     b = Animal(name='Tessa')        # Returns Bello
 
-This can be verified by the following comparisons.
-
+If instances of the class ``Animal`` are now created, this is only done for the 
+very first instantiation, and for all further instantiations always this 
+"primary instance" is given back.
+            
 .. code-block:: python
 
     # *** example_singleton.py - verfication of the unique instance
 
     # Case 1: Static decoration using @Singleton or @Singleton()
     print(f"a = {a}")               # a = Animal('Bello')
     print(f"b = {b}")               # b = Animal('Bello')
     print(f"a is b: {a is b}")      # a is b: True
     print(f"a == b: {a == b}")      # a == b: True
 
 If instead of the above "static decoration" using pie-notation, i.e. with 
-@-notation at the class declaration, the "dynamic decoration" in Python code 
-is used, additional parameters can be passed to the decorator for passing 
-to the class constructor.
+@-notation at the class declaration, the "dynamic decoration" within Python 
+code is used, additional parameters can be passed to the decorator for 
+passing to the class constructor.
 
 .. code-block:: python
 
     # *** example_singleton.py - dynamic decoration with extra parameters
 
     # Case 2: Dynamic decoration providing extra initial default values 
     Animal = Singleton(Animal, 'Bello')
@@ -154,18 +148,19 @@
     Animal(name='Tessa')            # Returns Bello
     print(Animal.instance)          # Animal('Bello')
 
 Quite generally, for all the following decorators based on this 
 `Decorator Arguments Pattern`_, these two properties are always fulfilled:
 
 .. note::
+
     * Decoration as a class (without parentheses) and Decoration as an instance 
       (with empty parentheses) are equivalent
-    * For dynamic decoration, extra parameters can be passed, e.g. for the class 
-      constructor
+    * For dynamic decoration, extra parameters can be passed, e.g. for the 
+      class constructor
 
 
 ******************************************************************************
 Multiton
 ******************************************************************************
 
 A `multiton pattern`_ is a design pattern that extends the singleton pattern.
@@ -175,18 +170,18 @@
 In this implementation the key parameter can be either any immutable type
 or a callable returning such an immutable type which can be used as a key
 of a dictionary. In case of an invalid key, key is set ``None`` and with only 
 one key value the multiton simply collapses to a singleton, therefore the 
 decoration ``@Multiton`` resp. ``@Multiton()`` or even ``@Multiton(key=17)`` 
 or  ``@Multiton(key='some fixed value')`` and so on always creates a singleton.
 
-Sometimes the key is independent of the classified object, but in many cases 
-it is part of the classified object itself, as in the following example where
-the key string matches the parameter ``name`` of the constructor of the 
-class ``Animal``.
+Usually the key is independent of the classified object. However, it is not 
+uncommon for it to be part of the classified object itself, as in the 
+following example, where the key string matches the parameter ``name`` of 
+the constructor of the class ``Animal``.
 
 .. code-block:: python
    
     # *** example_multitonton.py - class Animal with Multiton decoration
 
     from decoratory.multiton import Multiton
 
@@ -195,30 +190,24 @@
         def __init__(self, spec, name):
             self.spec = spec
             self.name = name
 
         def __repr__(self):
             return f"{self.__class__.__name__}('{self.spec}', '{self.name}')"
 
-When instances of the class ``Animal`` are now created, this only happens for 
-the *first instantiation per key value*, the initial name of the animal. For 
-all subsequent instantiations, this "primary instance per key value" is 
-returned. But for each new key value, a new ``Animal`` instance is created 
-and stored in the internal directory.
-
-.. code-block:: python
-   
-    # *** example_multitonton.py - creation of instances
-
     # Create Instances
     a = Animal('dog', name='Bello')
     b = Animal('cat', name='Mausi')
     c = Animal('dog', name='Tessa')
 
-This can be verified by the following comparisons.
+When instances of the class ``Animal`` are now created, this only happens for 
+the *first instantiation per key value*, the initial name of the animal. For 
+all subsequent instantiations, this "primary instance per key value" is 
+returned. But for each new key value, a new ``Animal`` instance is created 
+and stored in the internal directory.
 
 .. code-block:: python
 
     # *** example_multitonton.py - One unique instance per name
 
     # Case 1: key='name' references kwargs['name'] from __init__(..,name)
     print(a)                        # Animal('dog', 'Bello')
@@ -253,14 +242,24 @@
 generally is not recommended. 
 
 For this reason, each object knows its multiton: Setting ``Multiton``'s ``attrib`` 
 parameter while decoration to a valid attribute name string the multiton is 
 attributed in the new instantiated substitute object, is the chosen name 
 invalid or missing, the default attribute name ``multiton`` is chosen. 
 
+.. code-block:: python
+
+    # *** example_multitonton.py - One unique instance per equivalence class
+
+    # Case 3: with decoration @Multiton(key=lambda spec, name: 'a' in name)
+    print(a)                        # Animal('dog', 'Bello')
+    print(a.multiton)               # <decoratory.multiton.Multiton object..>
+    print(a.multiton.instances())   # {False: Animal('dog', 'Bello'), 
+                                    #   True: Animal('cat', 'Mausi')}
+
 Thus, in the above example, ``a.multiton`` would be the multiton of ``a`` 
 ('Bello') and ``a.multiton.instances()`` would be the directory of equivalence 
 classes to which it belongs.
 
 .. warning::
  
     Classifications into the multiton directory are done only once on
@@ -283,25 +282,25 @@
 
 * (optional) ``after`` call functionality.
 
 This implementation additionally supports an 
 
 * (optional) ``replace`` call functionality.
 
-The wrapper is all the more useful and broadly applicable the more flexible 
+This generic Wrapper is all the more broadly applicable, the more flexibly 
 these three activities can be formulated. All three decorator parameters, 
 ``before``, ``after`` and ``replace``, can be combined with each other and 
-support both single callables and (nested) lists of F-types 
+support both single callables and (nested) lists of ``F``-types 
 (imported from module decoratory.basic, see below for details). 
 In addition, ``replace`` supports passing results from successive 
 replacement calls through an optional keyword argument named ``result`` 
-(defaut value is None).
+(defaut value is ``None``).
 
-Even without any of these arguments, the wrapper can be used to "overwrite" 
-default values, for example.
+Even without any of these arguments, such a "do nothing wrapper" can be used 
+to "overwrite" default values, for example.
 
 .. code-block:: python
 
     # *** example_wrapper.py - overwrite default parameter values
 
     from decoratory.wrapper import Wrapper
 
@@ -314,14 +313,15 @@
     some_function = Wrapper(some_function, value="changed")
     some_function()                 # value = 'changed'
 
 The functionality of ``some_function()`` itself remains unchanged. A typical 
 scenario for a wrapper is, of course, the execution of additional functionality 
 before and/or after a given functionality, which itself remains unchanged, 
 such as ``enter/leave`` markers, call data caches, runtime measurements, etc.
+Here is a typical example:
 
 .. code-block:: python
 
     # *** example_wrapper.py - enclose original function
 
     from decoratory.wrapper import Wrapper
     from decoratory.basic import F
@@ -338,63 +338,132 @@
                                     # value = 'original'
                                     # LEAVE
 
 While ``before`` calls ``print_message`` with its default parameters the 
 ``after`` parameter uses the ``F``-function from ``decoratory.basic``. 
 It has a signature ``F(callable, *args, **kwargs)`` and encapsulates the 
 passing of any function with optional positional and keyword parameters. 
+Accordingly, the keyword variant ``after=F(print_message, message="LEAVE")`` 
+would also be possible.
 
-Finally, a more complex example illustrates the replacement of the original 
+A rather more complex example illustrates the replacement of the original 
 functionality with a sequence of replacement functionalities, passing a 
 ``result`` object of type ``int`` between successive calls.
 
 .. code-block:: python
 
     # *** example_wrapper.py - enclose and replacing original function
 
     from decoratory.wrapper import Wrapper
     from decoratory.basic import F
 
     # Case 3: Decoration with before, after and multiple replacements
-    def print_message(message: str = "BEFORE"):
+    def print_message(message: str = "UNDEFINED"):
         print(message)
 
     def replacement_printer(add: int = 1, *, result=None):
         result += add if isinstance(result, int) else 0
         print(f"result = {result}")
         return result
 
-    @Wrapper(before=F(print_message, "ENTER"),
+    @Wrapper(before=F(print, "ENTER"), # Python's print()
              replace=[F(replacement_printer, 1, result=0),
                       F(replacement_printer, 3),
                       F(replacement_printer, 5)],
              after=F(print_message, "LEAVE"))
-    def default_printer(message: str = "DEFAULT"):
+    def result_printer(message: str = "UNKNOWN"):
         print(message)
 
-    default_printer()               # ENTER         (before)
+    result_printer()                # ENTER         (before)
                                     # result = 1    (replacement_printer, 1)
                                     # result = 4    (replacement_printer, 3)
                                     # result = 9    (replacement_printer, 5)
                                     # LEAVE         (after)
                                     # 9             (output default_printer)
 
-The absence of the outputs of ``BEFORE`` and ``DEFAULT`` reflects the correct 
-replacements by the decoration, and the order of execution is exactly as 
-expected: ``before`` then ``replace`` then ``after`` and in each of these 
+The absence of the outputs of ``UNDEFINED`` and ``UNKNOWN`` reflects the 
+correct replacements by the decoration, and the order of execution is exactly 
+as expected: ``before`` then ``replace`` then ``after`` and in each of these 
 variables the lists are processed in ascending order.
 
+The *decoration of a class* always refers to the constructor of the class, e.g.
+
+.. code-block:: python
+
+    # *** example_wrapper.py - class decoration
+
+    from decoratory.wrapper import Wrapper
+    from decoratory.basic import F
+
+    @Wrapper(before=F(print, "BEFORE init"), after=F(print, "AFTER init"))
+    class Animal:
+        def __init__(self, name):
+            self.name = name
+            print("RUNNING init")
+    
+    # Case 4: Decoration of a class always refers to __init__
+    a = Animal(name='Bello')        # BEFORE init
+                                    # RUNNING init
+                                    # AFTER init
+
+
+For all other methods applies:
+
+.. note::
+
+    Decorations to ``@staticmethod`` or ``@classmethod`` can be done 
+    analogously to the function decorations above, since they already exist 
+    at compile time. Instance methods, on the other hand, do not exist until 
+    an object instance is created and must be handled differently.
+
+With ``Wrapper`` and custom service functions, a "private wrapper library" 
+can be built and reused.
+
+.. code-block:: python
+
+    # *** example_wrapper.py - private wrapper library
+
+    from decoratory.wrapper import Wrapper
+    from decoratory.basic import F
+
+    # Case 5: Define a private wrapper library
+    before_wrapper = Wrapper(before=F(print, "BEFORE"))
+    after_wrapper = Wrapper(after=F(print, "AFTER"))
+
+    # Multiple decorations for specialized functionality encapsulation
+    @before_wrapper
+    @after_wrapper
+    def some_function(value: str = "original"):
+        print(f"value = '{value}'")
+
+    some_function()                 # BEFORE
+                                    # value = 'original'
+                                    # AFTER
+
 
 ******************************************************************************
 Observer
 ******************************************************************************
 
 coming soon...
 
 
+******************************************************************************
+Version History
+******************************************************************************
+
+**Version: 0.1.0.2, Build: 2023-06-13**
+
+- Documentation enhancements
+
+**Version: 0.1.0.1, Build: 2023-06-12**
+
+- Initial version with Singleton, Multiton and Wrapper
+
+
 .. ===========================================================================
 .. _project homepage: http://evation.eu
 .. _singleton pattern: https://en.wikipedia.org/wiki/Singleton_pattern
 .. _multiton pattern: https://en.wikipedia.org/wiki/Multiton_pattern
 .. _Decorator Arguments Pattern: http://evation.eu
 
 `back to top <#top>`_
```

### Comparing `decoratory-0.1.0.1/Readme.rst` & `decoratory-0.1.0.2/Readme.rst`

 * *Files 6% similar despite different names*

```diff
@@ -5,66 +5,66 @@
 Decoratory
 ==============================================================================
 
 
 **Introduction**
 
 The "decoratory" package is based on the `Decorator Arguments Pattern`_, an 
-integrated concept for Python decorators with and without parameters. Thus 
-all decorators created with it support complex arguments, e.g. lists of 
-values and functions, without unnecessarily complicating the decoration of 
-simple cases by these extensions. All implementation details are described 
-on the `project homepage`_.
+integrated concept for Python decorators with and without parameters. In
+addition, all decorators created with it support complex arguments, e.g. 
+lists of values and functions, without unnecessarily complicating the 
+decoration of simple cases by these extensions. All implementation details 
+are described on the `project homepage`_.
 
 
 **Installation** ::
 
-    pip install decoratory
+    pip install --upgrade decoratory
 
 After installation, basic information about the package, the individual 
 modules and their methods is also available from the command line. ::
 
     python -m decoratory --help
 
 
-**Content**
+**Package Content**
 
-The "decoratory" package available here includes some classic decorators
+The decoratory package available here includes some classic decorators
 implemented and functionally extended with this concept, e.g.
 
 * `Singleton`_
 * `Multiton`_
 * `Wrapper`_
 * `Observer`_   (coming soon...)
 
-This is an open list that will grow over time.
+This is an open list that possibly will grow over time.
 
 
 **Description**
 
 To illustrate the functionality of each module, a simple as well as a 
-possibly more complex example is presented. Even if only one particular module 
+more complex example is presented. Even if only one particular module 
 is needed, it is recommended to view the preceding examples as well. For even
-more examples of the full range of possibilities, again, please refer to the 
+more examples of the full range of possibilities, please refer to the 
 `project homepage`_.
 
 
 ******************************************************************************
 Singleton
 ******************************************************************************
 
 A `singleton pattern`_ is a design pattern that limits the instantiation of 
 a class to a single (unique) instance. This is useful when exactly one unique 
 object is needed i.e. to manage an expensive resource or coordinate actions 
 across modules.
 
-As a simple example serves the decoration of the class  ``Animal`` as singleton. 
-In the context of the `Decorator Arguments Pattern`_, this can be done both 
-without brackets (class) and with brackets (object, instance), because both 
-notations describe the same functionality.
+As a simple example serves the decoration of the class  ``Animal`` as 
+singleton. In the context of the `Decorator Arguments Pattern`_, this can be 
+done both without brackets (decorator class) and with brackets (decorator 
+instance), meaning both notations describe the same functional situation.
 
 .. code-block:: python
    
     # *** example_singleton.py - class Animal with Singleton decoration
 
     from decoratory.singleton import Singleton
 
@@ -72,42 +72,36 @@
     class Animal:
         def __init__(self, name):
             self.name = name
 
         def __repr__(self):
             return f"{self.__class__.__name__}('{self.name}')"
 
-If instances of the class ``Animal`` are now created, this is only done for the 
-very first instantiation, and for all further instantiations always this 
-"primary instance" is given back.
-            
-.. code-block:: python
-   
-    # *** example_singleton.py - creation of instances
-
     # Create Instances
     a = Animal(name='Bello')        # Creates Bello
     b = Animal(name='Tessa')        # Returns Bello
 
-This can be verified by the following comparisons.
-
+If instances of the class ``Animal`` are now created, this is only done for the 
+very first instantiation, and for all further instantiations always this 
+"primary instance" is given back.
+            
 .. code-block:: python
 
     # *** example_singleton.py - verfication of the unique instance
 
     # Case 1: Static decoration using @Singleton or @Singleton()
     print(f"a = {a}")               # a = Animal('Bello')
     print(f"b = {b}")               # b = Animal('Bello')
     print(f"a is b: {a is b}")      # a is b: True
     print(f"a == b: {a == b}")      # a == b: True
 
 If instead of the above "static decoration" using pie-notation, i.e. with 
-@-notation at the class declaration, the "dynamic decoration" in Python code 
-is used, additional parameters can be passed to the decorator for passing 
-to the class constructor.
+@-notation at the class declaration, the "dynamic decoration" within Python 
+code is used, additional parameters can be passed to the decorator for 
+passing to the class constructor.
 
 .. code-block:: python
 
     # *** example_singleton.py - dynamic decoration with extra parameters
 
     # Case 2: Dynamic decoration providing extra initial default values 
     Animal = Singleton(Animal, 'Bello')
@@ -115,18 +109,19 @@
     Animal(name='Tessa')            # Returns Bello
     print(Animal.instance)          # Animal('Bello')
 
 Quite generally, for all the following decorators based on this 
 `Decorator Arguments Pattern`_, these two properties are always fulfilled:
 
 .. note::
+
     * Decoration as a class (without parentheses) and Decoration as an instance 
       (with empty parentheses) are equivalent
-    * For dynamic decoration, extra parameters can be passed, e.g. for the class 
-      constructor
+    * For dynamic decoration, extra parameters can be passed, e.g. for the 
+      class constructor
 
 
 ******************************************************************************
 Multiton
 ******************************************************************************
 
 A `multiton pattern`_ is a design pattern that extends the singleton pattern.
@@ -136,18 +131,18 @@
 In this implementation the key parameter can be either any immutable type
 or a callable returning such an immutable type which can be used as a key
 of a dictionary. In case of an invalid key, key is set ``None`` and with only 
 one key value the multiton simply collapses to a singleton, therefore the 
 decoration ``@Multiton`` resp. ``@Multiton()`` or even ``@Multiton(key=17)`` 
 or  ``@Multiton(key='some fixed value')`` and so on always creates a singleton.
 
-Sometimes the key is independent of the classified object, but in many cases 
-it is part of the classified object itself, as in the following example where
-the key string matches the parameter ``name`` of the constructor of the 
-class ``Animal``.
+Usually the key is independent of the classified object. However, it is not 
+uncommon for it to be part of the classified object itself, as in the 
+following example, where the key string matches the parameter ``name`` of 
+the constructor of the class ``Animal``.
 
 .. code-block:: python
    
     # *** example_multitonton.py - class Animal with Multiton decoration
 
     from decoratory.multiton import Multiton
 
@@ -156,30 +151,24 @@
         def __init__(self, spec, name):
             self.spec = spec
             self.name = name
 
         def __repr__(self):
             return f"{self.__class__.__name__}('{self.spec}', '{self.name}')"
 
-When instances of the class ``Animal`` are now created, this only happens for 
-the *first instantiation per key value*, the initial name of the animal. For 
-all subsequent instantiations, this "primary instance per key value" is 
-returned. But for each new key value, a new ``Animal`` instance is created 
-and stored in the internal directory.
-
-.. code-block:: python
-   
-    # *** example_multitonton.py - creation of instances
-
     # Create Instances
     a = Animal('dog', name='Bello')
     b = Animal('cat', name='Mausi')
     c = Animal('dog', name='Tessa')
 
-This can be verified by the following comparisons.
+When instances of the class ``Animal`` are now created, this only happens for 
+the *first instantiation per key value*, the initial name of the animal. For 
+all subsequent instantiations, this "primary instance per key value" is 
+returned. But for each new key value, a new ``Animal`` instance is created 
+and stored in the internal directory.
 
 .. code-block:: python
 
     # *** example_multitonton.py - One unique instance per name
 
     # Case 1: key='name' references kwargs['name'] from __init__(..,name)
     print(a)                        # Animal('dog', 'Bello')
@@ -214,14 +203,24 @@
 generally is not recommended. 
 
 For this reason, each object knows its multiton: Setting ``Multiton``'s ``attrib`` 
 parameter while decoration to a valid attribute name string the multiton is 
 attributed in the new instantiated substitute object, is the chosen name 
 invalid or missing, the default attribute name ``multiton`` is chosen. 
 
+.. code-block:: python
+
+    # *** example_multitonton.py - One unique instance per equivalence class
+
+    # Case 3: with decoration @Multiton(key=lambda spec, name: 'a' in name)
+    print(a)                        # Animal('dog', 'Bello')
+    print(a.multiton)               # <decoratory.multiton.Multiton object..>
+    print(a.multiton.instances())   # {False: Animal('dog', 'Bello'), 
+                                    #   True: Animal('cat', 'Mausi')}
+
 Thus, in the above example, ``a.multiton`` would be the multiton of ``a`` 
 ('Bello') and ``a.multiton.instances()`` would be the directory of equivalence 
 classes to which it belongs.
 
 .. warning::
  
     Classifications into the multiton directory are done only once on
@@ -244,25 +243,25 @@
 
 * (optional) ``after`` call functionality.
 
 This implementation additionally supports an 
 
 * (optional) ``replace`` call functionality.
 
-The wrapper is all the more useful and broadly applicable the more flexible 
+This generic Wrapper is all the more broadly applicable, the more flexibly 
 these three activities can be formulated. All three decorator parameters, 
 ``before``, ``after`` and ``replace``, can be combined with each other and 
-support both single callables and (nested) lists of F-types 
+support both single callables and (nested) lists of ``F``-types 
 (imported from module decoratory.basic, see below for details). 
 In addition, ``replace`` supports passing results from successive 
 replacement calls through an optional keyword argument named ``result`` 
-(defaut value is None).
+(defaut value is ``None``).
 
-Even without any of these arguments, the wrapper can be used to "overwrite" 
-default values, for example.
+Even without any of these arguments, such a "do nothing wrapper" can be used 
+to "overwrite" default values, for example.
 
 .. code-block:: python
 
     # *** example_wrapper.py - overwrite default parameter values
 
     from decoratory.wrapper import Wrapper
 
@@ -275,14 +274,15 @@
     some_function = Wrapper(some_function, value="changed")
     some_function()                 # value = 'changed'
 
 The functionality of ``some_function()`` itself remains unchanged. A typical 
 scenario for a wrapper is, of course, the execution of additional functionality 
 before and/or after a given functionality, which itself remains unchanged, 
 such as ``enter/leave`` markers, call data caches, runtime measurements, etc.
+Here is a typical example:
 
 .. code-block:: python
 
     # *** example_wrapper.py - enclose original function
 
     from decoratory.wrapper import Wrapper
     from decoratory.basic import F
@@ -299,63 +299,132 @@
                                     # value = 'original'
                                     # LEAVE
 
 While ``before`` calls ``print_message`` with its default parameters the 
 ``after`` parameter uses the ``F``-function from ``decoratory.basic``. 
 It has a signature ``F(callable, *args, **kwargs)`` and encapsulates the 
 passing of any function with optional positional and keyword parameters. 
+Accordingly, the keyword variant ``after=F(print_message, message="LEAVE")`` 
+would also be possible.
 
-Finally, a more complex example illustrates the replacement of the original 
+A rather more complex example illustrates the replacement of the original 
 functionality with a sequence of replacement functionalities, passing a 
 ``result`` object of type ``int`` between successive calls.
 
 .. code-block:: python
 
     # *** example_wrapper.py - enclose and replacing original function
 
     from decoratory.wrapper import Wrapper
     from decoratory.basic import F
 
     # Case 3: Decoration with before, after and multiple replacements
-    def print_message(message: str = "BEFORE"):
+    def print_message(message: str = "UNDEFINED"):
         print(message)
 
     def replacement_printer(add: int = 1, *, result=None):
         result += add if isinstance(result, int) else 0
         print(f"result = {result}")
         return result
 
-    @Wrapper(before=F(print_message, "ENTER"),
+    @Wrapper(before=F(print, "ENTER"), # Python's print()
              replace=[F(replacement_printer, 1, result=0),
                       F(replacement_printer, 3),
                       F(replacement_printer, 5)],
              after=F(print_message, "LEAVE"))
-    def default_printer(message: str = "DEFAULT"):
+    def result_printer(message: str = "UNKNOWN"):
         print(message)
 
-    default_printer()               # ENTER         (before)
+    result_printer()                # ENTER         (before)
                                     # result = 1    (replacement_printer, 1)
                                     # result = 4    (replacement_printer, 3)
                                     # result = 9    (replacement_printer, 5)
                                     # LEAVE         (after)
                                     # 9             (output default_printer)
 
-The absence of the outputs of ``BEFORE`` and ``DEFAULT`` reflects the correct 
-replacements by the decoration, and the order of execution is exactly as 
-expected: ``before`` then ``replace`` then ``after`` and in each of these 
+The absence of the outputs of ``UNDEFINED`` and ``UNKNOWN`` reflects the 
+correct replacements by the decoration, and the order of execution is exactly 
+as expected: ``before`` then ``replace`` then ``after`` and in each of these 
 variables the lists are processed in ascending order.
 
+The *decoration of a class* always refers to the constructor of the class, e.g.
+
+.. code-block:: python
+
+    # *** example_wrapper.py - class decoration
+
+    from decoratory.wrapper import Wrapper
+    from decoratory.basic import F
+
+    @Wrapper(before=F(print, "BEFORE init"), after=F(print, "AFTER init"))
+    class Animal:
+        def __init__(self, name):
+            self.name = name
+            print("RUNNING init")
+    
+    # Case 4: Decoration of a class always refers to __init__
+    a = Animal(name='Bello')        # BEFORE init
+                                    # RUNNING init
+                                    # AFTER init
+
+
+For all other methods applies:
+
+.. note::
+
+    Decorations to ``@staticmethod`` or ``@classmethod`` can be done 
+    analogously to the function decorations above, since they already exist 
+    at compile time. Instance methods, on the other hand, do not exist until 
+    an object instance is created and must be handled differently.
+
+With ``Wrapper`` and custom service functions, a "private wrapper library" 
+can be built and reused.
+
+.. code-block:: python
+
+    # *** example_wrapper.py - private wrapper library
+
+    from decoratory.wrapper import Wrapper
+    from decoratory.basic import F
+
+    # Case 5: Define a private wrapper library
+    before_wrapper = Wrapper(before=F(print, "BEFORE"))
+    after_wrapper = Wrapper(after=F(print, "AFTER"))
+
+    # Multiple decorations for specialized functionality encapsulation
+    @before_wrapper
+    @after_wrapper
+    def some_function(value: str = "original"):
+        print(f"value = '{value}'")
+
+    some_function()                 # BEFORE
+                                    # value = 'original'
+                                    # AFTER
+
 
 ******************************************************************************
 Observer
 ******************************************************************************
 
 coming soon...
 
 
+******************************************************************************
+Version History
+******************************************************************************
+
+**Version: 0.1.0.2, Build: 2023-06-13**
+
+- Documentation enhancements
+
+**Version: 0.1.0.1, Build: 2023-06-12**
+
+- Initial version with Singleton, Multiton and Wrapper
+
+
 .. ===========================================================================
 .. _project homepage: http://evation.eu
 .. _singleton pattern: https://en.wikipedia.org/wiki/Singleton_pattern
 .. _multiton pattern: https://en.wikipedia.org/wiki/Multiton_pattern
 .. _Decorator Arguments Pattern: http://evation.eu
 
 `back to top <#top>`_
```

### Comparing `decoratory-0.1.0.1/Sources/decoratory/__main__.py` & `decoratory-0.1.0.2/Sources/decoratory/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.0.1"
-__date__ = "2023-06-12"
-__time__ = "14:49:52"
+__version__ = "0.1.0.2"
+__date__ = "2023-06-13"
+__time__ = "18:28:13"
 __state__ = "Beta"
 __license__ = "PSF"
 
 __all__ = []
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
@@ -47,31 +47,22 @@
     elif arg in "--copyright":
         print(f"{__copyright__}")
     elif arg in "--license" or arg in "--licence":
         print(f"\n{'-' * 79}")
         print(f"{__title__} ships under the license: {__license__}".center(79))
         print(f"{'-' * 79}")
         try:
-            with open(join(dirname(__file__), "License.txt"), "r") as f:
+            with open(join(dirname(__file__), "data", "License.txt"),
+                      "r") as f:
                 txt = f.read()
             print("\n" + txt)
         except (FileNotFoundError, Exception):
             print("*** No additional data accessible. "
                   f"Please look for file 'License.txt' ***".center(79, " "))
         print(f"{'-' * 79}")
-    elif arg in "--documentation":
-        print(f"\n{'-' * 79}")
-        try:
-            with open(join(dirname(__file__), "Readme.rst"), "r") as f:
-                txt = f.read()
-            print("\n" + txt)
-        except (FileNotFoundError, Exception):
-            print("*** No additional data accessible. "
-                  f"Please look for file 'Readme.rst' ***".center(79, " "))
-        print(f"{'-' * 79}")
     elif arg in "--information":
         print(f"\nPeople and contact information for package {module}:\n")
         print(f"Author    : {__author__}")
         print(f"Maintainer: {__maintainer__}")
         print(f"Company   : {__company__}")
         print(f"Email     : {__email__}")
         print(f"Web       : {__url__}")
@@ -109,15 +100,14 @@
 Possible options are:
 
   -h, --help            show this help message
   -v, --version         show {module}[.module] version information      
   -c, --copyright       show {module}[.module] copyright statement
   -l, --license         show {module}[.module] license statement (License.txt)
       --licence         an alias to --license
-  -d, --documentation   display content of the Readme.rst file
   -i, --info            people and contact information
 
 Example: Display license statement for the multiton module:
 
 {'python -m decoratory.multiton --license': ^79s}
          
 -------------------------------------------------------------------------------
```

### Comparing `decoratory-0.1.0.1/Sources/decoratory/banner.py` & `decoratory-0.1.0.2/Sources/decoratory/banner.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.0.1"
-__date__ = "2023-06-12"
-__time__ = "14:49:52"
+__version__ = "0.1.0.3"
+__date__ = "2023-06-13"
+__time__ = "18:03:50"
 __state__ = "Beta"
 __license__ = "PSF"
 
 __all__ = ["__banner"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
@@ -38,20 +38,19 @@
              maintainer: str = __maintainer__,
              company: str = __company__,
              email: str = __email__,
              url: str = __url__,
              copyright: str = __copyright__,
              state: str = __state__,
              license: str = __license__,
-             file_license: str = "License.txt"):
+             file_license: str = join("data", "License.txt")):
     """**Banner**
 
-    Banner is a helper module displaying package/module information. It is
-    designed private because it is very special and therefore not intended
-    for general or public use.
+    Banner is an auxiliary module for displaying package and module
+    information.
     """
     module = title.lower()
     name = title.capitalize()
 
     arg = argv[1].strip().lower() if len(argv) > 1 else "message"
     if arg in "--version":
         print(f"{module}: Version {version}, "
```

### Comparing `decoratory-0.1.0.1/Sources/decoratory/basic.py` & `decoratory-0.1.0.2/Sources/decoratory/basic.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,24 +9,24 @@
     decorator arguments. It generates and resolves (nested) lists of tuples of
     decorator argument objects between their native forms and F/X structure
     representations.
 
     Attributes
     ----------
     Activation: IntFlag
-        Relative point in time flags for callback activation.
+        Relative time flags for activity control.
 
     F: Type
         A wrapper for callee(*callee_args, **callee_kwargs) semantics.
 
     X: Type(F)
-        A cross-wrapper for callee and *callee_args as well as **callee_kwargs.
+        A cross-wrapper for callee vs. *callee_args and/or **callee_kwargs.
 
     Parser: Type
-        Function and Class Constructor Parser.
+        Parser to resolve the function/class decoration argument language.
 
     Methods
     -------
     None.
 """
 
 # -----------------------------------------------------------------------------
@@ -37,32 +37,32 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.0.1"
-__date__ = "2023-06-12"
-__time__ = "14:49:52"
+__version__ = "0.1.0.2"
+__date__ = "2023-06-13"
+__time__ = "18:03:50"
 __state__ = "Beta"
 __license__ = "PSF"
 
 __all__ = ["Activation", "Parser", "F", "X"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 from enum import IntFlag
 from typing import Union
 
 
 # -----------------------------------------------------------------------------
 # Classes
 class Activation(IntFlag):
-    """Relative point in time flags for action activation.
+    """Relative time flags for activity control.
 
     NONE                    No activation
     BEFORE                  Activation before action
     AFTER                   Activation after action
     BEFORE_AND_AFTER        Activation before and after action
     """
     NONE = 0x00
@@ -71,70 +71,70 @@
     BEFORE_AND_AFTER = BEFORE | AFTER
 
 
 class F:
     """A wrapper for callee(*callee_args, **callee_kwargs) semantics.
 
     The caller is designed as a read-only property, since it is used as a key
-    used to collect F objects in sets.
+    to collect F objects in sets.
 
     The eval() method applies the callee property to its callee_args and/or
     callee_kwargs:
       - If callee is a callable, it is applied directly to the arguments,
       - If callee is a string, eval() is applied to the same-named method of
         the object passed to eval().
 
     Attributes
     ----------
-        callee: callable or str (getter)
-        callee_kwargs: object
+        callee: callable or str     (getter property)
+        callee_args: object
         callee_kwargs: object
 
     Methods
     -------
     eval(self, obj=None)
-        Evaluate the callee(callee_args, callee_kwargs)
+        Evaluate the value of callee(callee_args, callee_kwargs)
 
     Example
     -------
 
     from decoratory.basic import F
 
     # Define a callable
-    def sandwich(anything="", toast:str="|"):
+    def sandwich(anything="", toast: str = "|"):
         return f"{toast}{anything}{toast}"
 
     # Case 1: Function argument is a callable
-    f = F(sandwich)         # F(sandwich), sandwich(): ||
-    print(f"{repr(f)}, {str(f)}: {f.eval()}")
-    f = F(sandwich, 3)      # F(sandwich, 3), sandwich(3): |3|
+    f = F(sandwich)                 # F(sandwich), sandwich(): ||
     print(f"{repr(f)}, {str(f)}: {f.eval()}")
-    f = F(sandwich, 'A')    # F(sandwich, "A"), sandwich("A"): |A|
+    f = F(sandwich, 3)              # F(sandwich, 3), sandwich(3): |3|
     print(f"{repr(f)}, {str(f)}: {f.eval()}")
-    f = F(sandwich, 3, '*') # F(sandwich, 3, "*"), sandwich(3, "*"): *3*
+    f = F(sandwich, 'A')            # F(sandwich, "A"), sandwich("A"): |A|
     print(f"{repr(f)}, {str(f)}: {f.eval()}")
-    f = F(sandwich, 3, toast='*') # F(sandwich, 3, toast="*"), sandwich(
+    f = F(sandwich, 3, '*')         # F(sandwich, 3, "*"), sandwich(3, "*"):
+    print(f"{repr(f)}, {str(f)}: {f.eval()}")   # *3*
+    f = F(sandwich, 3, toast='*')   # F(sandwich, 3, toast="*"), sandwich(
     print(f"{repr(f)}, {str(f)}: {f.eval()}")   # 3, toast="*"): *3*
 
     # Define a method
     class A:
-        def sandwich(self, anything="", toast:str="|"):
+        def sandwich(self, anything="", toast: str = "|"):
             return f"{toast}{anything}{toast}"
 
     # Case 2: Function argument is a method name
-    f = F("sandwich")         # F("sandwich"), sandwich(): ||
-    print(f"{repr(f)}, {str(f)}: {f.eval(obj=A())}")
-    f = F("sandwich", 3)      # F("sandwich", 3), sandwich(3): |3|
+    f = F("sandwich")               # F("sandwich"), sandwich(): ||
     print(f"{repr(f)}, {str(f)}: {f.eval(obj=A())}")
-    f = F("sandwich", 'A')    # F("sandwich", "A"), sandwich("A"): |A|
+    f = F("sandwich", 3)            # F("sandwich", 3), sandwich(3): |3|
     print(f"{repr(f)}, {str(f)}: {f.eval(obj=A())}")
-    f = F("sandwich", 3, '*') # F("sandwich", 3, "*"), sandwich(3, "*"): *3*
+    f = F("sandwich", 'A')          # F("sandwich", "A"), sandwich("A"): |A|
     print(f"{repr(f)}, {str(f)}: {f.eval(obj=A())}")
+    f = F("sandwich", 3, '*')       # F("sandwich", 3, "*"), sandwich(3, "*"):
+    print(f"{repr(f)}, {str(f)}: {f.eval(obj=A())}")    # *3*
     f = F("sandwich", 3, toast='*') # F("sandwich", 3, toast="*"), sandwich(
-    print(f"{repr(f)}, {str(f)}: {f.eval(obj=A())}")   # 3, toast="*"): *3*
+    print(f"{repr(f)}, {str(f)}: {f.eval(obj=A())}")    # 3, toast="*"): *3*
     """
     __slots__ = ('__callee', 'callee_args', 'callee_kwargs')
 
     @staticmethod
     def __quote(qs: str = "", qq: str = '"') -> str:
         """Special str quotes"""
         return f"{qq}{qs}{qq}" if isinstance(qs, str) else str(qs)
@@ -187,15 +187,15 @@
     def __iter__(self):
         return iter([self.__callee, self.callee_args, self.callee_kwargs])
 
     def __next__(self):
         pass  # __iter__ delegates to list iterator
 
     def eval(self, obj=None):
-        """Evaluate the callee(callee_args, callee_kwargs)"""
+        """Evaluate the value of callee(callee_args, callee_kwargs)"""
         if callable(self.__callee):
             # Assume default function semantics
             return self.__callee(*self.callee_args, **self.callee_kwargs)
         elif isinstance(self.__callee, str):
             # Assume an instance method semantics
             if obj is None:
                 # Assume obj is in first positional argument args[0]
@@ -205,77 +205,77 @@
                         return getattr(obj, self.__callee)(
                             *self.callee_args[1:], **self.callee_kwargs)
             elif hasattr(obj, self.__callee):
                 # Assume this obj as the instance of __callee
                 return getattr(obj, self.__callee)(
                     *self.callee_args, **self.callee_kwargs)
 
-        # In any other case
+        # In all other cases
         raise TypeError(f"'{self.__callee}' cannot be evaluated.")
 
     # Getter, Setter, Properties
     def __get__callee(self):
         return self.__callee
 
     def __set__callee(self, value: Union[callable, str]):
-        self.__callee = value  # Read only object key, see init above
+        self.__callee = value  # Read-only object key, see init above
 
     callee = property(__get__callee)
 
 
 class X(F):
-    """A cross-wrapper for callee and *callee_args as well as **callee_kwargs.
+    """A cross-wrapper for callee vs. *callee_args and/or **callee_kwargs.
 
     Technically, X is equivalent to F. Both share the same code, the same
     syntax, but they follow different semantics:
        - F is a wrapper for a callee and its OWN arguments, whereas
        - X is a wrapper for a callee and arguments for another caller
 
     Although X can be substituted by F, it is recommended to use X to indicate
     that the callee and the specified arguments do not belong to each other,
     for reasons of code clarity.
     """
     pass
 
 
 class Parser:
-    """Function and Class Constructor Parser.
+    """Parser to resolve the function/class decoration argument language.
 
     A Parser to resolve the function/class decoration argument language where
     a callable is mandatory and the optional arguments have empty defaults
-    into a list of F structures.
+    into a list of F-structures.
 
     Syntax:
         Parser.eval(item) -> [F(callable|method_name, *args, **kwarg), ...]
 
     Production:
         item        :=  list | tuple | F | callable | str | None
         list        := [list | tuple | F | callable | str | None]
-            [..,list,..]                -> [..,*list,...]
+            [..,list,..]                -> [..,*list,..]
         tuple       := (..,) | (..,..) | (..,..,..)
             (callable|str,)             -> F(callable|str)
             (callable|str, (..))        -> F(callable|str, *(..))
             (callable|str, {..})        -> F(callable|str, **{..})
             (callable|str, (..), {..})  -> F(callable|str, *(..), **{..})
         F           := F(..) | F(..,..) | F(..,..,..)
             F(callable|str)             -> F(callable|str)
             F(callable|str, *a)         -> F(callable|str, *a)
-            F(callable|str, **kw)       -> F(callable|str, **kw)
-            F(callable|str, *a, **kw)   -> F(callable|str, *a, **kw)
+            F(callable|str, **kwa)      -> F(callable|str, **kwa)
+            F(callable|str, *a, **kwa)  -> F(callable|str, *a, **kwa)
         callable    := callable
             callable                    -> F(callable)
         str         := str
             str                         -> F(str)
         None        := None
             None                        -> []
     """
 
     @classmethod
     def eval(cls, item: Union[list, tuple, F, callable, str, None]) -> list:
-        """Format data, resolve and collect as F structures in a flat list
+        """Format data, resolve and collect as F-structures in a flat list
 
         list        -> cls.list         (see below)
         tuple       -> [cls.tuple]      (see below)
         F(..,..,..) -> [F(.,.,.)]
         callable    -> [F(callable)]
         string      -> [F(string)]
         None        -> []               (empty list)
@@ -295,15 +295,15 @@
             raise TypeError(f"Object '{item}' cannot be parsed.")
         return result
 
     @classmethod
     def list(cls, list_obj: list) -> list:
         """Resolve (nested) list recursively.
 
-        Loop over list (iterable) and resolve list items (item):
+        Loop over list (iterable) and resolve list items:
 
         list        -> [..., cls.list]       (extend recursively)
         tuple       -> [..., cls.tuple]      (see below)
         F(..,..,..) -> [..., F(..,..,..)]
         callable    -> [..., F(callable)]
         str         -> [..., F(str)]
         None        -> [...]
```

### Comparing `decoratory-0.1.0.1/Sources/decoratory/multiton.py` & `decoratory-0.1.0.2/Sources/decoratory/multiton.py`

 * *Files identical despite different names*

### Comparing `decoratory-0.1.0.1/Sources/decoratory/observer.py` & `decoratory-0.1.0.2/Sources/decoratory/observer.py`

 * *Files identical despite different names*

### Comparing `decoratory-0.1.0.1/Sources/decoratory/singleton.py` & `decoratory-0.1.0.2/Sources/decoratory/singleton.py`

 * *Files identical despite different names*

### Comparing `decoratory-0.1.0.1/Sources/decoratory/wrapper.py` & `decoratory-0.1.0.2/Sources/decoratory/wrapper.py`

 * *Files 7% similar despite different names*

```diff
@@ -89,31 +89,56 @@
     # Function call with decoration: before, after and replacement
     default_printer()               # ENTER         (before)
                                     # result = 1    (replacement_printer, 1)
                                     # result = 4    (replacement_printer, 3)
                                     # result = 9    (replacement_printer, 5)
                                     # LEAVE         (after)
                                     # 9             (output default_printer)
+
+    # Case 4: Decoration of a class always refers to __init__
+    @Wrapper(before=F(print, "BEFORE init"), after=F(print, "AFTER init"))
+    class Animal:
+        def __init__(self, name):
+            self.name = name
+            print("RUNNING init")
+
+    a = Animal(name='Bello')        # BEFORE init
+                                    # RUNNING init
+                                    # AFTER init
+
+    # Case 5: Define a private wrapper library
+    before_wrapper = Wrapper(before=F(print, "BEFORE"))
+    after_wrapper = Wrapper(after=F(print, "AFTER"))
+
+    # Multiple decorations for specialized functionality encapsulation
+    @before_wrapper
+    @after_wrapper
+    def some_function(value: str = "original"):
+        print(f"value = '{value}'")
+
+    some_function()                 # BEFORE
+                                    # value = 'original'
+                                    # AFTER
 """
 
 # -----------------------------------------------------------------------------
 # Module Level Dunders
 __title__ = "Wrapper"
 __module__ = "wrapper.py"
 __author__ = "Martin Abel"
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.0.1"
-__date__ = "2023-06-12"
-__time__ = "14:49:52"
+__version__ = "0.1.0.2"
+__date__ = "2023-06-13"
+__time__ = "18:23:53"
 __state__ = "Beta"
 __license__ = "PSF"
 
 __all__ = ["Wrapper"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
@@ -210,14 +235,39 @@
     # Function call with decoration: before, after and replacement
     default_printer()               # ENTER         (before)
                                     # result = 1    (replacement_printer, 1)
                                     # result = 4    (replacement_printer, 3)
                                     # result = 9    (replacement_printer, 5)
                                     # LEAVE         (after)
                                     # 9             (output default_printer)
+
+    # Case 4: Decoration of a class always refers to __init__
+    @Wrapper(before=F(print, "BEFORE init"), after=F(print, "AFTER init"))
+    class Animal:
+        def __init__(self, name):
+            self.name = name
+            print("RUNNING init")
+
+    a = Animal(name='Bello')        # BEFORE init
+                                    # RUNNING init
+                                    # AFTER init
+
+    # Case 5: Define a private wrapper library
+    before_wrapper = Wrapper(before=F(print, "BEFORE"))
+    after_wrapper = Wrapper(after=F(print, "AFTER"))
+
+    # Multiple decorations for specialized functionality encapsulation
+    @before_wrapper
+    @after_wrapper
+    def some_function(value: str = "original"):
+        print(f"value = '{value}'")
+
+    some_function()                 # BEFORE
+                                    # value = 'original'
+                                    # AFTER
     """
 
     def __init__(self,
                  substitute: callable or type = None,
                  *args: object,
                  before: callable or list = None,
                  replace: callable or list = None,
```

### Comparing `decoratory-0.1.0.1/Sources/decoratory.egg-info/PKG-INFO` & `decoratory-0.1.0.2/Sources/decoratory.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: decoratory
-Version: 0.1.0.1
+Version: 0.1.0.2
 Summary: Decorators: Singleton, Multiton, Observer, generic Wrapper.
 Home-page: http://evation.eu
 Download-URL: http://evation.eu
 Author: Martin Abel
 Author-email: Martin Abel <python@evation.eu>
 Maintainer: Martin Abel
 Maintainer-email: Martin Abel <python@evation.eu>
 License: PSF
 Project-URL: Projekt, http://evation.eu
 Project-URL: Release Notes, http://evation.eu
 Project-URL: Download, http://evation.eu
-Keywords: decorator singleton multiton observer wrapper
+Keywords: decorator singleton multiton observer observable wrapper
 Platform: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
 Classifier: Natural Language :: English
@@ -44,66 +44,66 @@
 Decoratory
 ==============================================================================
 
 
 **Introduction**
 
 The "decoratory" package is based on the `Decorator Arguments Pattern`_, an 
-integrated concept for Python decorators with and without parameters. Thus 
-all decorators created with it support complex arguments, e.g. lists of 
-values and functions, without unnecessarily complicating the decoration of 
-simple cases by these extensions. All implementation details are described 
-on the `project homepage`_.
+integrated concept for Python decorators with and without parameters. In
+addition, all decorators created with it support complex arguments, e.g. 
+lists of values and functions, without unnecessarily complicating the 
+decoration of simple cases by these extensions. All implementation details 
+are described on the `project homepage`_.
 
 
 **Installation** ::
 
-    pip install decoratory
+    pip install --upgrade decoratory
 
 After installation, basic information about the package, the individual 
 modules and their methods is also available from the command line. ::
 
     python -m decoratory --help
 
 
-**Content**
+**Package Content**
 
-The "decoratory" package available here includes some classic decorators
+The decoratory package available here includes some classic decorators
 implemented and functionally extended with this concept, e.g.
 
 * `Singleton`_
 * `Multiton`_
 * `Wrapper`_
 * `Observer`_   (coming soon...)
 
-This is an open list that will grow over time.
+This is an open list that possibly will grow over time.
 
 
 **Description**
 
 To illustrate the functionality of each module, a simple as well as a 
-possibly more complex example is presented. Even if only one particular module 
+more complex example is presented. Even if only one particular module 
 is needed, it is recommended to view the preceding examples as well. For even
-more examples of the full range of possibilities, again, please refer to the 
+more examples of the full range of possibilities, please refer to the 
 `project homepage`_.
 
 
 ******************************************************************************
 Singleton
 ******************************************************************************
 
 A `singleton pattern`_ is a design pattern that limits the instantiation of 
 a class to a single (unique) instance. This is useful when exactly one unique 
 object is needed i.e. to manage an expensive resource or coordinate actions 
 across modules.
 
-As a simple example serves the decoration of the class  ``Animal`` as singleton. 
-In the context of the `Decorator Arguments Pattern`_, this can be done both 
-without brackets (class) and with brackets (object, instance), because both 
-notations describe the same functionality.
+As a simple example serves the decoration of the class  ``Animal`` as 
+singleton. In the context of the `Decorator Arguments Pattern`_, this can be 
+done both without brackets (decorator class) and with brackets (decorator 
+instance), meaning both notations describe the same functional situation.
 
 .. code-block:: python
    
     # *** example_singleton.py - class Animal with Singleton decoration
 
     from decoratory.singleton import Singleton
 
@@ -111,42 +111,36 @@
     class Animal:
         def __init__(self, name):
             self.name = name
 
         def __repr__(self):
             return f"{self.__class__.__name__}('{self.name}')"
 
-If instances of the class ``Animal`` are now created, this is only done for the 
-very first instantiation, and for all further instantiations always this 
-"primary instance" is given back.
-            
-.. code-block:: python
-   
-    # *** example_singleton.py - creation of instances
-
     # Create Instances
     a = Animal(name='Bello')        # Creates Bello
     b = Animal(name='Tessa')        # Returns Bello
 
-This can be verified by the following comparisons.
-
+If instances of the class ``Animal`` are now created, this is only done for the 
+very first instantiation, and for all further instantiations always this 
+"primary instance" is given back.
+            
 .. code-block:: python
 
     # *** example_singleton.py - verfication of the unique instance
 
     # Case 1: Static decoration using @Singleton or @Singleton()
     print(f"a = {a}")               # a = Animal('Bello')
     print(f"b = {b}")               # b = Animal('Bello')
     print(f"a is b: {a is b}")      # a is b: True
     print(f"a == b: {a == b}")      # a == b: True
 
 If instead of the above "static decoration" using pie-notation, i.e. with 
-@-notation at the class declaration, the "dynamic decoration" in Python code 
-is used, additional parameters can be passed to the decorator for passing 
-to the class constructor.
+@-notation at the class declaration, the "dynamic decoration" within Python 
+code is used, additional parameters can be passed to the decorator for 
+passing to the class constructor.
 
 .. code-block:: python
 
     # *** example_singleton.py - dynamic decoration with extra parameters
 
     # Case 2: Dynamic decoration providing extra initial default values 
     Animal = Singleton(Animal, 'Bello')
@@ -154,18 +148,19 @@
     Animal(name='Tessa')            # Returns Bello
     print(Animal.instance)          # Animal('Bello')
 
 Quite generally, for all the following decorators based on this 
 `Decorator Arguments Pattern`_, these two properties are always fulfilled:
 
 .. note::
+
     * Decoration as a class (without parentheses) and Decoration as an instance 
       (with empty parentheses) are equivalent
-    * For dynamic decoration, extra parameters can be passed, e.g. for the class 
-      constructor
+    * For dynamic decoration, extra parameters can be passed, e.g. for the 
+      class constructor
 
 
 ******************************************************************************
 Multiton
 ******************************************************************************
 
 A `multiton pattern`_ is a design pattern that extends the singleton pattern.
@@ -175,18 +170,18 @@
 In this implementation the key parameter can be either any immutable type
 or a callable returning such an immutable type which can be used as a key
 of a dictionary. In case of an invalid key, key is set ``None`` and with only 
 one key value the multiton simply collapses to a singleton, therefore the 
 decoration ``@Multiton`` resp. ``@Multiton()`` or even ``@Multiton(key=17)`` 
 or  ``@Multiton(key='some fixed value')`` and so on always creates a singleton.
 
-Sometimes the key is independent of the classified object, but in many cases 
-it is part of the classified object itself, as in the following example where
-the key string matches the parameter ``name`` of the constructor of the 
-class ``Animal``.
+Usually the key is independent of the classified object. However, it is not 
+uncommon for it to be part of the classified object itself, as in the 
+following example, where the key string matches the parameter ``name`` of 
+the constructor of the class ``Animal``.
 
 .. code-block:: python
    
     # *** example_multitonton.py - class Animal with Multiton decoration
 
     from decoratory.multiton import Multiton
 
@@ -195,30 +190,24 @@
         def __init__(self, spec, name):
             self.spec = spec
             self.name = name
 
         def __repr__(self):
             return f"{self.__class__.__name__}('{self.spec}', '{self.name}')"
 
-When instances of the class ``Animal`` are now created, this only happens for 
-the *first instantiation per key value*, the initial name of the animal. For 
-all subsequent instantiations, this "primary instance per key value" is 
-returned. But for each new key value, a new ``Animal`` instance is created 
-and stored in the internal directory.
-
-.. code-block:: python
-   
-    # *** example_multitonton.py - creation of instances
-
     # Create Instances
     a = Animal('dog', name='Bello')
     b = Animal('cat', name='Mausi')
     c = Animal('dog', name='Tessa')
 
-This can be verified by the following comparisons.
+When instances of the class ``Animal`` are now created, this only happens for 
+the *first instantiation per key value*, the initial name of the animal. For 
+all subsequent instantiations, this "primary instance per key value" is 
+returned. But for each new key value, a new ``Animal`` instance is created 
+and stored in the internal directory.
 
 .. code-block:: python
 
     # *** example_multitonton.py - One unique instance per name
 
     # Case 1: key='name' references kwargs['name'] from __init__(..,name)
     print(a)                        # Animal('dog', 'Bello')
@@ -253,14 +242,24 @@
 generally is not recommended. 
 
 For this reason, each object knows its multiton: Setting ``Multiton``'s ``attrib`` 
 parameter while decoration to a valid attribute name string the multiton is 
 attributed in the new instantiated substitute object, is the chosen name 
 invalid or missing, the default attribute name ``multiton`` is chosen. 
 
+.. code-block:: python
+
+    # *** example_multitonton.py - One unique instance per equivalence class
+
+    # Case 3: with decoration @Multiton(key=lambda spec, name: 'a' in name)
+    print(a)                        # Animal('dog', 'Bello')
+    print(a.multiton)               # <decoratory.multiton.Multiton object..>
+    print(a.multiton.instances())   # {False: Animal('dog', 'Bello'), 
+                                    #   True: Animal('cat', 'Mausi')}
+
 Thus, in the above example, ``a.multiton`` would be the multiton of ``a`` 
 ('Bello') and ``a.multiton.instances()`` would be the directory of equivalence 
 classes to which it belongs.
 
 .. warning::
  
     Classifications into the multiton directory are done only once on
@@ -283,25 +282,25 @@
 
 * (optional) ``after`` call functionality.
 
 This implementation additionally supports an 
 
 * (optional) ``replace`` call functionality.
 
-The wrapper is all the more useful and broadly applicable the more flexible 
+This generic Wrapper is all the more broadly applicable, the more flexibly 
 these three activities can be formulated. All three decorator parameters, 
 ``before``, ``after`` and ``replace``, can be combined with each other and 
-support both single callables and (nested) lists of F-types 
+support both single callables and (nested) lists of ``F``-types 
 (imported from module decoratory.basic, see below for details). 
 In addition, ``replace`` supports passing results from successive 
 replacement calls through an optional keyword argument named ``result`` 
-(defaut value is None).
+(defaut value is ``None``).
 
-Even without any of these arguments, the wrapper can be used to "overwrite" 
-default values, for example.
+Even without any of these arguments, such a "do nothing wrapper" can be used 
+to "overwrite" default values, for example.
 
 .. code-block:: python
 
     # *** example_wrapper.py - overwrite default parameter values
 
     from decoratory.wrapper import Wrapper
 
@@ -314,14 +313,15 @@
     some_function = Wrapper(some_function, value="changed")
     some_function()                 # value = 'changed'
 
 The functionality of ``some_function()`` itself remains unchanged. A typical 
 scenario for a wrapper is, of course, the execution of additional functionality 
 before and/or after a given functionality, which itself remains unchanged, 
 such as ``enter/leave`` markers, call data caches, runtime measurements, etc.
+Here is a typical example:
 
 .. code-block:: python
 
     # *** example_wrapper.py - enclose original function
 
     from decoratory.wrapper import Wrapper
     from decoratory.basic import F
@@ -338,63 +338,132 @@
                                     # value = 'original'
                                     # LEAVE
 
 While ``before`` calls ``print_message`` with its default parameters the 
 ``after`` parameter uses the ``F``-function from ``decoratory.basic``. 
 It has a signature ``F(callable, *args, **kwargs)`` and encapsulates the 
 passing of any function with optional positional and keyword parameters. 
+Accordingly, the keyword variant ``after=F(print_message, message="LEAVE")`` 
+would also be possible.
 
-Finally, a more complex example illustrates the replacement of the original 
+A rather more complex example illustrates the replacement of the original 
 functionality with a sequence of replacement functionalities, passing a 
 ``result`` object of type ``int`` between successive calls.
 
 .. code-block:: python
 
     # *** example_wrapper.py - enclose and replacing original function
 
     from decoratory.wrapper import Wrapper
     from decoratory.basic import F
 
     # Case 3: Decoration with before, after and multiple replacements
-    def print_message(message: str = "BEFORE"):
+    def print_message(message: str = "UNDEFINED"):
         print(message)
 
     def replacement_printer(add: int = 1, *, result=None):
         result += add if isinstance(result, int) else 0
         print(f"result = {result}")
         return result
 
-    @Wrapper(before=F(print_message, "ENTER"),
+    @Wrapper(before=F(print, "ENTER"), # Python's print()
              replace=[F(replacement_printer, 1, result=0),
                       F(replacement_printer, 3),
                       F(replacement_printer, 5)],
              after=F(print_message, "LEAVE"))
-    def default_printer(message: str = "DEFAULT"):
+    def result_printer(message: str = "UNKNOWN"):
         print(message)
 
-    default_printer()               # ENTER         (before)
+    result_printer()                # ENTER         (before)
                                     # result = 1    (replacement_printer, 1)
                                     # result = 4    (replacement_printer, 3)
                                     # result = 9    (replacement_printer, 5)
                                     # LEAVE         (after)
                                     # 9             (output default_printer)
 
-The absence of the outputs of ``BEFORE`` and ``DEFAULT`` reflects the correct 
-replacements by the decoration, and the order of execution is exactly as 
-expected: ``before`` then ``replace`` then ``after`` and in each of these 
+The absence of the outputs of ``UNDEFINED`` and ``UNKNOWN`` reflects the 
+correct replacements by the decoration, and the order of execution is exactly 
+as expected: ``before`` then ``replace`` then ``after`` and in each of these 
 variables the lists are processed in ascending order.
 
+The *decoration of a class* always refers to the constructor of the class, e.g.
+
+.. code-block:: python
+
+    # *** example_wrapper.py - class decoration
+
+    from decoratory.wrapper import Wrapper
+    from decoratory.basic import F
+
+    @Wrapper(before=F(print, "BEFORE init"), after=F(print, "AFTER init"))
+    class Animal:
+        def __init__(self, name):
+            self.name = name
+            print("RUNNING init")
+    
+    # Case 4: Decoration of a class always refers to __init__
+    a = Animal(name='Bello')        # BEFORE init
+                                    # RUNNING init
+                                    # AFTER init
+
+
+For all other methods applies:
+
+.. note::
+
+    Decorations to ``@staticmethod`` or ``@classmethod`` can be done 
+    analogously to the function decorations above, since they already exist 
+    at compile time. Instance methods, on the other hand, do not exist until 
+    an object instance is created and must be handled differently.
+
+With ``Wrapper`` and custom service functions, a "private wrapper library" 
+can be built and reused.
+
+.. code-block:: python
+
+    # *** example_wrapper.py - private wrapper library
+
+    from decoratory.wrapper import Wrapper
+    from decoratory.basic import F
+
+    # Case 5: Define a private wrapper library
+    before_wrapper = Wrapper(before=F(print, "BEFORE"))
+    after_wrapper = Wrapper(after=F(print, "AFTER"))
+
+    # Multiple decorations for specialized functionality encapsulation
+    @before_wrapper
+    @after_wrapper
+    def some_function(value: str = "original"):
+        print(f"value = '{value}'")
+
+    some_function()                 # BEFORE
+                                    # value = 'original'
+                                    # AFTER
+
 
 ******************************************************************************
 Observer
 ******************************************************************************
 
 coming soon...
 
 
+******************************************************************************
+Version History
+******************************************************************************
+
+**Version: 0.1.0.2, Build: 2023-06-13**
+
+- Documentation enhancements
+
+**Version: 0.1.0.1, Build: 2023-06-12**
+
+- Initial version with Singleton, Multiton and Wrapper
+
+
 .. ===========================================================================
 .. _project homepage: http://evation.eu
 .. _singleton pattern: https://en.wikipedia.org/wiki/Singleton_pattern
 .. _multiton pattern: https://en.wikipedia.org/wiki/Multiton_pattern
 .. _Decorator Arguments Pattern: http://evation.eu
 
 `back to top <#top>`_
```

### Comparing `decoratory-0.1.0.1/setup.py` & `decoratory-0.1.0.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,29 +12,29 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.0.1"
-__date__ = "2023-06-12"
-__time__ = "14:49:52"
+__version__ = "0.1.0.2"
+__date__ = "2023-06-13"
+__time__ = "18:28:13"
 __state__ = "Beta"
 __license__ = "PSF"
 
 # -----------------------------------------------------------------------------
 # Libraries
 from os.path import join
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 
 # -----------------------------------------------------------------------------
 # Parameters
-root = "Sources"
+src = "Sources"
 
 with open("Readme.rst", "r") as f:
     description = f.read()
 
 with open("Requirements.txt", "r") as f:
     requirements = [str(req) for req in f.read().splitlines() if req]
 
@@ -63,15 +63,15 @@
     description='Decorators: Singleton, Multiton, Observer, generic Wrapper.',
     long_description=description,
     long_description_content_type='text/x-rst',
     project_urls={
         'Projekt': __url__,
         'Release Notes': __url__,
         'Download': __url__},
-    keywords='decorator singleton multiton observer wrapper',
+    keywords='decorator singleton multiton observer observable wrapper',
     # Technical
     license=__license__,
     platforms=['Operating System :: OS Independent'],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Intended Audience :: Education',
@@ -89,19 +89,19 @@
         'Operating System :: OS Independent',
         'Topic :: Education',
         'Topic :: Software Development',
         'Topic :: Software Development :: Libraries',
         'Topic :: Utilities'],
     # Modules, Files and Data
     # https://setuptools.pypa.io/en/latest/userguide/package_discovery.html#finding-simple-packages
-    packages=find_packages(where=root),
-    package_dir={"": root},
+    packages=find_packages(where=src),
+    package_dir={"": src},
     package_data={},
     py_modules=[],
-    data_files=[(f"lib/site-packages/{__title__}",
+    data_files=[(f"./lib/site-packages/{__title__}/data",
                  ["License.txt", "Readme.rst", "Requirements.txt"])],
     entry_points={},
     # Dependencies
     python_requires='>=3.7',
     setup_requires=[],
     install_requires=requirements,
     # Post install
```

