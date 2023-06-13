# Comparing `tmp/pydantic_xmlmodel-0.1.1.tar.gz` & `tmp/pydantic_xmlmodel-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_xmlmodel-0.1.1.tar", max compression
+gzip compressed data, was "pydantic_xmlmodel-0.2.tar", max compression
```

## Comparing `pydantic_xmlmodel-0.1.1.tar` & `pydantic_xmlmodel-0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1069 2023-05-17 13:32:22.273043 pydantic_xmlmodel-0.1.1/LICENSE
--rw-r--r--   0        0        0     2327 2023-05-17 14:55:31.763327 pydantic_xmlmodel-0.1.1/README.md
--rw-r--r--   0        0        0       55 2023-05-17 13:44:08.514440 pydantic_xmlmodel-0.1.1/pydantic_xmlmodel/__init__.py
--rw-r--r--   0        0        0        0 2023-05-24 08:52:39.775359 pydantic_xmlmodel-0.1.1/pydantic_xmlmodel/py.typed
--rw-r--r--   0        0        0     9357 2023-05-20 18:36:21.749673 pydantic_xmlmodel-0.1.1/pydantic_xmlmodel/xmlmodel.py
--rw-r--r--   0        0        0      613 2023-05-24 08:52:59.623623 pydantic_xmlmodel-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3071 1970-01-01 00:00:00.000000 pydantic_xmlmodel-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-17 13:32:22.273043 pydantic_xmlmodel-0.2/LICENSE
+-rw-r--r--   0        0        0     2323 2023-06-07 13:50:14.138462 pydantic_xmlmodel-0.2/README.md
+-rw-r--r--   0        0        0       55 2023-05-17 13:44:08.514440 pydantic_xmlmodel-0.2/pydantic_xmlmodel/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 08:52:39.775359 pydantic_xmlmodel-0.2/pydantic_xmlmodel/py.typed
+-rw-r--r--   0        0        0     9806 2023-06-13 10:18:19.983642 pydantic_xmlmodel-0.2/pydantic_xmlmodel/xmlmodel.py
+-rw-r--r--   0        0        0      611 2023-06-13 10:19:00.609226 pydantic_xmlmodel-0.2/pyproject.toml
+-rw-r--r--   0        0        0     3065 1970-01-01 00:00:00.000000 pydantic_xmlmodel-0.2/PKG-INFO
```

### Comparing `pydantic_xmlmodel-0.1.1/LICENSE` & `pydantic_xmlmodel-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_xmlmodel-0.1.1/README.md` & `pydantic_xmlmodel-0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -33,45 +33,45 @@
     color: str = "black"
     weight: int = 10
     is_friendly: bool = True
 ```
 
 ### Converting a Model to XML
 
-You can convert a model to XML by calling the `dicttoxml()` method:
+You can convert a model to XML by calling the `to_xml()` method:
 
 ```python
 class Cat(XMLModel):
     animal_characteristics: AnimalCharacteristics
     name: str = "Kitty"
 
 cat = Cat(animal_characteristics=AnimalCharacteristics())
-print(cat.dicttoxml(indent=4))
+print(cat.to_xml(indent=4))
 ```
 
 This will output:
 
 ```xml
 <?xml version="1.0" ?>
 <cat name="Kitty">
     <animalcharacteristics color="black" weight="10" is_friendly="True"/>
 </cat>
 ```
 
 ### Converting XML to a Model
 
-You can convert XML to a model by calling the `fromxml()` method:
+You can convert XML to a model by calling the `from_xml()` method:
 
 ```python
 xml = """<?xml version="1.0" ?>
 <cat name="Kitty">
     <animalcharacteristics color="black" is_friendly="true" weight="10"/>
 </cat>
 """
-cat = Cat.fromxml(xml)
+cat = Cat.from_xml(xml)
 print(cat)
 ```
 
 This will output:
 
 ```python
 animal_characteristics=AnimalCharacteristics(color='black', weight=10, is_friendly=True, __xml_content__=None) name='Kitty' __xml_content__='\n    '
```

### Comparing `pydantic_xmlmodel-0.1.1/pydantic_xmlmodel/xmlmodel.py` & `pydantic_xmlmodel-0.2/pydantic_xmlmodel/xmlmodel.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""A module that contains the XMLModel class."""
+
 from typing import Any, Callable, Optional, Type, TypeVar, no_type_check
 from xml.dom.minidom import parseString
 from xml.etree.ElementTree import Element, SubElement, fromstring, tostring
 
 from pydantic import BaseModel
 from pydantic.main import ModelMetaclass
 
@@ -15,29 +17,30 @@
 
     It adds the following class attributes to XMLModel:
         - `__xml_name__`: The name of the XML element. If not specified, the name of the class is used.
     """
 
     @no_type_check
     def __new__(cls, name, bases, attrs, **kwargs):
-        """Adds the following class attributes to XMLModel:
+        """Add the following class attributes to XMLModel.
+
         - xml_name: The name of the XML element. If not specified, the name of the class is used.
         """
         xml_name = kwargs.pop("xml_name", None)
         if xml_name is not None:
             attrs["__xml_name__"] = xml_name
 
         return super().__new__(cls, name, bases, attrs, **kwargs)
 
 
 class XMLModel(BaseModel, metaclass=XMLModelMeta):
     """A base class for XML models.
 
     It's useful for converting a model to XML string (e.g. for libvirt XML manifests). It allows you to specify the name of the XML element and its content
-    and supports nested XML elements. See `XMLModel.dicttoxml()` for examples.
+    and supports nested XML elements. See `XMLModel.to_xml()` for examples.
 
     It's a subclass of `pydantic.BaseModel` and can be used as a regular model (and can be nested in other models).
 
     It's currently missing support for lists and dictionaries (it will be added as json attribute to the XML element).
 
     It adds the following class attributes to XMLModel:
         - `__xml_name__`: The name of the XML element. If not specified, the name of the class is used.
@@ -65,28 +68,35 @@
         >>> ExampleSchema._get_xml_name()
         'EXAMPLESCHEMA'
     """
 
     __xml_content__: Optional[str] = None
     """The content of the XML element inside `<element>{{__xml_content__}}</element>`. If not specified, the element will not have any content."""
 
+    def __init__(self, **data: Any) -> None:
+        """Initialize the model."""
+        xml_content = data.pop("__xml_content__", None)
+        super().__init__(**data)
+        if xml_content is not None:
+            object.__setattr__(self, "__xml_content__", xml_content)
+
     @classmethod
     def _get_xml_name(cls) -> str:
-        """A method that returns the name of the XML element."""
+        """Return the name of the XML element."""
         if cls.__xml_name__ is not None:
             return cls.__xml_name__
         else:
             if cls.__xml_name_function__ is not None:
                 return cls.__xml_name_function__(cls.__name__)
             return cls.__name__
 
-    def dicttoxml(
+    def to_xml(
         self, indent: Optional[int] = None, include_xml_version: bool = True
     ) -> str:
-        """Converts the model to XML string.
+        """Convert the model to XML string.
 
         Args:
             indent: If specified, the XML will be indented with the specified number of spaces.
 
         Returns:
             The XML string.
 
@@ -99,25 +109,23 @@
             >>> class Cat(XMLModel):
             ...     animal_characteristics: AnimalCharacteristics
             ...     name: str = "Kitty"
             ...
             >>> Cat(
             ...     animal_characteristics=AnimalCharacteristics(),
             ...     name="Kitty"
-            ... ).dicttoxml(indent=4)
-            \"\"\"
+            ... ).to_xml(indent=4)
             <?xml version="1.0" ?>
             <cat name="Kitty">
                 <animal_characteristics color="black" is_friendly="true" weight="10"/>
             </cat>
-            \"\"\"
         """
 
         def to_xml(e: Element, obj: Any) -> None:
-            """Converts the model to XML recursively."""
+            """Convert the model to XML recursively."""
             # Iterate over the fields of the model and convert them to XML
             for field, _ in obj.dict().items():
                 # We skip the __xml_content__ field because we handle it separately
                 if field == "__xml_content__":
                     continue
                 # We get the value of the field using getattr() because the we need subclass of BaseModel, not just dict
                 value = getattr(obj, field)
@@ -152,24 +160,25 @@
         # Convert the XML element to string
         xml = parseString(tostring(root, encoding="unicode"))
 
         if not include_xml_version:
             # See https://stackoverflow.com/a/65516230
             xml = xml.childNodes[0]
 
+        xml_str: str
         if indent is not None:
             xml_str = xml.toprettyxml(indent=" " * indent)
         else:
             xml_str = xml.toxml()
 
         return xml_str
 
     @classmethod
-    def fromxml(cls: Type[T], xml: str) -> T:
-        """Converts XML string to a model.
+    def from_xml(cls: Type[T], xml: str) -> T:
+        """Convert XML string to a model.
 
         Args:
             xml: The XML string.
 
         Returns:
             The model.
 
@@ -179,20 +188,20 @@
             ...     weight: int = 10
             ...     is_friendly: bool = True
             ...
             >>> class Cat(XMLModel):
             ...     animal_characteristics: AnimalCharacteristics
             ...     name: str = "Kitty"
             ...
-            >>> cat = Cat.fromxml(\"\"\"
+            >>> cat = Cat.from_xml('''
             ... <?xml version="1.0" ?>
             ... <cat name="Kitty">
             ...     <animal_characteristics color="black" is_friendly="true" weight="10"/>
             ... </cat>
-            ... \"\"\")
+            ... ''')
             >>> cat
             Cat(animal_characteristics=AnimalCharacteristics(color='black', weight=10, is_friendly=True), name='Kitty')
         """
 
         def from_element(element: Element, model: Type[BaseModel]) -> Any:
             data = {}
             for field in model.__fields__:
@@ -228,7 +237,11 @@
             if isinstance(out, XMLModel):
                 object.__setattr__(out, "__xml_content__", element.text)
 
             return out
 
         root = fromstring(xml)
         return from_element(root, cls)  # type: ignore
+
+    def set_xml_content(self, value: Optional[str]) -> None:
+        """Set the content of the XML element."""
+        object.__setattr__(self, "__xml_content__", value)
```

### Comparing `pydantic_xmlmodel-0.1.1/pyproject.toml` & `pydantic_xmlmodel-0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-xmlmodel"
-version = "0.1.1"
+version = "0.2"
 description = "PydanticXML is a Python library that provides a way to convert Pydantic models to XML and vice versa."
 authors = ["cofob <cofob@riseup.net>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/cofob/pydanticxml"
 homepage = "https://github.com/cofob/pydanticxml"
```

### Comparing `pydantic_xmlmodel-0.1.1/PKG-INFO` & `pydantic_xmlmodel-0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-xmlmodel
-Version: 0.1.1
+Version: 0.2
 Summary: PydanticXML is a Python library that provides a way to convert Pydantic models to XML and vice versa.
 Home-page: https://github.com/cofob/pydanticxml
 License: MIT
 Author: cofob
 Author-email: cofob@riseup.net
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -52,45 +52,45 @@
     color: str = "black"
     weight: int = 10
     is_friendly: bool = True
 ```
 
 ### Converting a Model to XML
 
-You can convert a model to XML by calling the `dicttoxml()` method:
+You can convert a model to XML by calling the `to_xml()` method:
 
 ```python
 class Cat(XMLModel):
     animal_characteristics: AnimalCharacteristics
     name: str = "Kitty"
 
 cat = Cat(animal_characteristics=AnimalCharacteristics())
-print(cat.dicttoxml(indent=4))
+print(cat.to_xml(indent=4))
 ```
 
 This will output:
 
 ```xml
 <?xml version="1.0" ?>
 <cat name="Kitty">
     <animalcharacteristics color="black" weight="10" is_friendly="True"/>
 </cat>
 ```
 
 ### Converting XML to a Model
 
-You can convert XML to a model by calling the `fromxml()` method:
+You can convert XML to a model by calling the `from_xml()` method:
 
 ```python
 xml = """<?xml version="1.0" ?>
 <cat name="Kitty">
     <animalcharacteristics color="black" is_friendly="true" weight="10"/>
 </cat>
 """
-cat = Cat.fromxml(xml)
+cat = Cat.from_xml(xml)
 print(cat)
 ```
 
 This will output:
 
 ```python
 animal_characteristics=AnimalCharacteristics(color='black', weight=10, is_friendly=True, __xml_content__=None) name='Kitty' __xml_content__='\n    '
```

