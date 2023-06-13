# Comparing `tmp/rasa_sdk-3.6.0.tar.gz` & `tmp/rasa_sdk-3.6.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rasa_sdk-3.6.0.tar", max compression
+gzip compressed data, was "rasa_sdk-3.6.0a1.tar", max compression
```

## Comparing `rasa_sdk-3.6.0.tar` & `rasa_sdk-3.6.0a1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    11553 2023-06-13 13:41:20.925541 rasa_sdk-3.6.0/LICENSE.txt
--rw-r--r--   0        0        0     5282 2023-06-13 13:41:20.925541 rasa_sdk-3.6.0/README.md
--rw-r--r--   0        0        0     3122 2023-06-13 13:41:20.925541 rasa_sdk-3.6.0/pyproject.toml
--rw-r--r--   0        0        0      420 2023-06-13 13:41:20.925541 rasa_sdk-3.6.0/rasa_sdk/__init__.py
--rw-r--r--   0        0        0      947 2023-06-13 13:41:20.925541 rasa_sdk-3.6.0/rasa_sdk/__main__.py
--rw-r--r--   0        0        0        0 2023-06-13 13:41:20.925541 rasa_sdk-3.6.0/rasa_sdk/cli/__init__.py
--rw-r--r--   0        0        0     1528 2023-06-13 13:41:20.925541 rasa_sdk-3.6.0/rasa_sdk/cli/arguments.py
--rw-r--r--   0        0        0      399 2023-06-13 13:41:20.925541 rasa_sdk-3.6.0/rasa_sdk/constants.py
--rw-r--r--   0        0        0     5727 2023-06-13 13:41:20.925541 rasa_sdk-3.6.0/rasa_sdk/endpoint.py
--rw-r--r--   0        0        0     6459 2023-06-13 13:41:20.925541 rasa_sdk-3.6.0/rasa_sdk/events.py
--rw-r--r--   0        0        0     1905 2023-06-13 13:41:20.925541 rasa_sdk-3.6.0/rasa_sdk/exceptions.py
--rw-r--r--   0        0        0    15183 2023-06-13 13:41:20.925541 rasa_sdk-3.6.0/rasa_sdk/executor.py
--rw-r--r--   0        0        0    11265 2023-06-13 13:41:20.925541 rasa_sdk-3.6.0/rasa_sdk/forms.py
--rw-r--r--   0        0        0    12929 2023-06-13 13:41:20.925541 rasa_sdk-3.6.0/rasa_sdk/interfaces.py
--rw-r--r--   0        0        0        0 2023-06-13 13:41:20.925541 rasa_sdk-3.6.0/rasa_sdk/knowledge_base/__init__.py
--rw-r--r--   0        0        0    10413 2023-06-13 13:41:20.925541 rasa_sdk-3.6.0/rasa_sdk/knowledge_base/actions.py
--rw-r--r--   0        0        0     8091 2023-06-13 13:41:20.925541 rasa_sdk-3.6.0/rasa_sdk/knowledge_base/storage.py
--rw-r--r--   0        0        0     7266 2023-06-13 13:41:20.929541 rasa_sdk-3.6.0/rasa_sdk/knowledge_base/utils.py
--rw-r--r--   0        0        0     1039 2023-06-13 13:41:20.929541 rasa_sdk-3.6.0/rasa_sdk/plugin.py
--rw-r--r--   0        0        0     7066 2023-06-13 13:41:20.929541 rasa_sdk-3.6.0/rasa_sdk/slots.py
--rw-r--r--   0        0        0     1683 2023-06-13 13:41:20.929541 rasa_sdk-3.6.0/rasa_sdk/types.py
--rw-r--r--   0        0        0    11308 2023-06-13 13:41:20.929541 rasa_sdk-3.6.0/rasa_sdk/utils.py
--rw-r--r--   0        0        0      116 2023-06-13 13:41:20.929541 rasa_sdk-3.6.0/rasa_sdk/version.py
--rw-r--r--   0        0        0     6794 1970-01-01 00:00:00.000000 rasa_sdk-3.6.0/PKG-INFO
+-rw-r--r--   0        0        0    11553 2023-05-17 17:52:30.724710 rasa_sdk-3.6.0a1/LICENSE.txt
+-rw-r--r--   0        0        0     5282 2023-05-17 17:52:30.724710 rasa_sdk-3.6.0a1/README.md
+-rw-r--r--   0        0        0     3114 2023-05-17 17:52:30.724710 rasa_sdk-3.6.0a1/pyproject.toml
+-rw-r--r--   0        0        0      420 2023-05-17 17:52:30.724710 rasa_sdk-3.6.0a1/rasa_sdk/__init__.py
+-rw-r--r--   0        0        0      947 2023-05-17 17:52:30.724710 rasa_sdk-3.6.0a1/rasa_sdk/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-17 17:52:30.724710 rasa_sdk-3.6.0a1/rasa_sdk/cli/__init__.py
+-rw-r--r--   0        0        0     1528 2023-05-17 17:52:30.724710 rasa_sdk-3.6.0a1/rasa_sdk/cli/arguments.py
+-rw-r--r--   0        0        0      399 2023-05-17 17:52:30.724710 rasa_sdk-3.6.0a1/rasa_sdk/constants.py
+-rw-r--r--   0        0        0     5727 2023-05-17 17:52:30.724710 rasa_sdk-3.6.0a1/rasa_sdk/endpoint.py
+-rw-r--r--   0        0        0     6459 2023-05-17 17:52:30.724710 rasa_sdk-3.6.0a1/rasa_sdk/events.py
+-rw-r--r--   0        0        0     1905 2023-05-17 17:52:30.724710 rasa_sdk-3.6.0a1/rasa_sdk/exceptions.py
+-rw-r--r--   0        0        0    15183 2023-05-17 17:52:30.724710 rasa_sdk-3.6.0a1/rasa_sdk/executor.py
+-rw-r--r--   0        0        0    11265 2023-05-17 17:52:30.724710 rasa_sdk-3.6.0a1/rasa_sdk/forms.py
+-rw-r--r--   0        0        0    12929 2023-05-17 17:52:30.724710 rasa_sdk-3.6.0a1/rasa_sdk/interfaces.py
+-rw-r--r--   0        0        0        0 2023-05-17 17:52:30.724710 rasa_sdk-3.6.0a1/rasa_sdk/knowledge_base/__init__.py
+-rw-r--r--   0        0        0     8970 2023-05-17 17:52:30.724710 rasa_sdk-3.6.0a1/rasa_sdk/knowledge_base/actions.py
+-rw-r--r--   0        0        0     7766 2023-05-17 17:52:30.724710 rasa_sdk-3.6.0a1/rasa_sdk/knowledge_base/storage.py
+-rw-r--r--   0        0        0     6287 2023-05-17 17:52:30.724710 rasa_sdk-3.6.0a1/rasa_sdk/knowledge_base/utils.py
+-rw-r--r--   0        0        0     1039 2023-05-17 17:52:30.724710 rasa_sdk-3.6.0a1/rasa_sdk/plugin.py
+-rw-r--r--   0        0        0     7066 2023-05-17 17:52:30.724710 rasa_sdk-3.6.0a1/rasa_sdk/slots.py
+-rw-r--r--   0        0        0     1683 2023-05-17 17:52:30.724710 rasa_sdk-3.6.0a1/rasa_sdk/types.py
+-rw-r--r--   0        0        0    11308 2023-05-17 17:52:30.728710 rasa_sdk-3.6.0a1/rasa_sdk/utils.py
+-rw-r--r--   0        0        0      118 2023-05-17 17:52:30.728710 rasa_sdk-3.6.0a1/rasa_sdk/version.py
+-rw-r--r--   0        0        0     6796 1970-01-01 00:00:00.000000 rasa_sdk-3.6.0a1/PKG-INFO
```

### Comparing `rasa_sdk-3.6.0/LICENSE.txt` & `rasa_sdk-3.6.0a1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.6.0/README.md` & `rasa_sdk-3.6.0a1/README.md`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.6.0/pyproject.toml` & `rasa_sdk-3.6.0a1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.black]
 line-length = 88
 target-version = [ "py37", "py38", "py39", "py310",]
 exclude = "((.eggs | .git | .mypy_cache | .pytest_cache | build | dist))"
 
 [tool.poetry]
 name = "rasa-sdk"
-version = "3.6.0"
+version = "3.6.0a1"
 description = "Open source machine learning framework to automate text- and voice-based conversations: NLU, dialogue management, connect to Slack, Facebook, and more - Create chatbots and voice assistants"
 authors = [ "Rasa Technologies GmbH <hi@rasa.com>",]
 maintainers = [ "Tom Bocklisch <tom@rasa.com>",]
 homepage = "https://rasa.com"
 repository = "https://github.com/rasahq/rasa-sdk"
 documentation = "https://rasa.com/docs"
 classifiers = [ "Development Status :: 5 - Production/Stable", "Intended Audience :: Developers", "License :: OSI Approved :: Apache Software License", "Topic :: Software Development :: Libraries",]
@@ -83,27 +83,27 @@
 "ruamel.yaml" = ">=0.16.5,<0.18.0"
 websockets = ">=10.0,<11.0"
 pluggy = "^1.0.0"
 
 [tool.poetry.dev-dependencies]
 pytest-cov = "^4.0.0"
 coveralls = "^3.0.1"
-pytest = "^7.3.1"
+pytest = "^7.2.1"
 black = "22.12.0"
 questionary = ">=1.5.1,<1.11.0"
 towncrier = "^22.8.0"
 toml = "^0.10.0"
 pep440-version-utils = "^0.3.0"
 semantic_version = "^2.8.5"
-mypy = "^1.3"
+mypy = "^1.1"
 sanic-testing = "^22.3.0, <22.9.0"
 
-[tool.ruff.pydocstyle]
-convention = "google"
-
 [tool.pytest.ini_options]
 python_functions = "test_"
 asyncio_mode = "auto"
 
+[tool.ruff.pydocstyle]
+convention = "google"
+
 [tool.poetry.group.dev.dependencies]
-ruff = ">=0.0.256,<0.0.268"
+ruff = "^0.0.256"
 pytest-asyncio = "^0.21.0"
```

### Comparing `rasa_sdk-3.6.0/rasa_sdk/__main__.py` & `rasa_sdk-3.6.0a1/rasa_sdk/__main__.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.6.0/rasa_sdk/cli/arguments.py` & `rasa_sdk-3.6.0a1/rasa_sdk/cli/arguments.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.6.0/rasa_sdk/endpoint.py` & `rasa_sdk-3.6.0a1/rasa_sdk/endpoint.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.6.0/rasa_sdk/events.py` & `rasa_sdk-3.6.0a1/rasa_sdk/events.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.6.0/rasa_sdk/exceptions.py` & `rasa_sdk-3.6.0a1/rasa_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.6.0/rasa_sdk/executor.py` & `rasa_sdk-3.6.0a1/rasa_sdk/executor.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.6.0/rasa_sdk/forms.py` & `rasa_sdk-3.6.0a1/rasa_sdk/forms.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.6.0/rasa_sdk/interfaces.py` & `rasa_sdk-3.6.0a1/rasa_sdk/interfaces.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.6.0/rasa_sdk/knowledge_base/actions.py` & `rasa_sdk-3.6.0a1/rasa_sdk/knowledge_base/actions.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,14 @@
     SLOT_ATTRIBUTE,
     reset_attribute_slots,
     SLOT_MENTION,
     SLOT_LAST_OBJECT,
     SLOT_LISTED_OBJECTS,
     get_object_name,
     get_attribute_slots,
-    match_extracted_entities_to_object_type,
 )
 from rasa_sdk import utils
 from rasa_sdk.executor import CollectingDispatcher
 from rasa_sdk.interfaces import Tracker
 from rasa_sdk.knowledge_base.storage import KnowledgeBase
 
 if typing.TYPE_CHECKING:  # pragma: no cover
@@ -109,63 +108,49 @@
 
     async def run(
         self,
         dispatcher: CollectingDispatcher,
         tracker: Tracker,
         domain: "DomainDict",
     ) -> List[Dict[Text, Any]]:
-        """
-        Executes this action. If the user ask a question about an attribute,
+        """Executes this action.
+
+        If the user ask a question about an attribute,
         the knowledge base is queried for that attribute. Otherwise, if no
-        attribute was detected in the latest request it assumes user is talking
-        about a new object type and, multiple objects of the requested type are
-        returned from the knowledge base.
+        attribute was detected in the request or the user is talking about a new
+        object type, multiple objects of the requested type are returned from the
+        knowledge base.
 
         Args:
             dispatcher: the dispatcher
             tracker: the tracker
             domain: the domain
 
         Returns: list of slots
 
         """
         object_type = tracker.get_slot(SLOT_OBJECT_TYPE)
         last_object_type = tracker.get_slot(SLOT_LAST_OBJECT_TYPE)
         attribute = tracker.get_slot(SLOT_ATTRIBUTE)
-        has_mention = tracker.get_slot(SLOT_MENTION) is not None
 
-        # check if attribute entity is found in latest user message. This is used
-        # to track whether the request is to query objects or query attributes
-        has_attribute_in_latest_message = any(
-            entity.get("entity") == "attribute"
-            for entity in tracker.latest_message["entities"]
-        )
+        new_request = object_type != last_object_type
 
         if not object_type:
-            # sets the object type dynamically from entities if object_type is not
-            # found in user query
-            object_types = self.knowledge_base.get_object_types()
-            object_type = match_extracted_entities_to_object_type(tracker, object_types)
-            set_object_type_slot_event = [SlotSet(SLOT_OBJECT_TYPE, object_type)]
-            tracker.add_slots(
-                set_object_type_slot_event
-            )  # temporarily set the `object_type_slot` to extracted value
+            # object type always needs to be set as this is needed to query the
+            # knowledge base
+            dispatcher.utter_message(response="utter_ask_rephrase")
+            return []
 
-        if object_type and not has_attribute_in_latest_message:
+        if not attribute or new_request:
             return await self._query_objects(dispatcher, object_type, tracker)
-        elif object_type and attribute:
+        elif attribute:
             return await self._query_attribute(
                 dispatcher, object_type, attribute, tracker
             )
 
-        if last_object_type and has_mention and attribute:
-            return await self._query_attribute(
-                dispatcher, last_object_type, attribute, tracker
-            )
-
         dispatcher.utter_message(response="utter_ask_rephrase")
         return []
 
     async def _query_objects(
         self, dispatcher: CollectingDispatcher, object_type: Text, tracker: Tracker
     ) -> List[Dict]:
         """
@@ -178,41 +163,38 @@
             tracker: the tracker
 
         Returns: list of slots
         """
         object_attributes = await utils.call_potential_coroutine(
             self.knowledge_base.get_attributes_of_object(object_type)
         )
+
         # get all set attribute slots of the object type to be able to filter the
         # list of objects
         attributes = get_attribute_slots(tracker, object_attributes)
         # query the knowledge base
         objects = await utils.call_potential_coroutine(
             self.knowledge_base.get_objects(object_type, attributes)
         )
+
         await utils.call_potential_coroutine(
             self.utter_objects(dispatcher, object_type, objects)
         )
 
         if not objects:
             return reset_attribute_slots(tracker, object_attributes)
 
         key_attribute = await utils.call_potential_coroutine(
             self.knowledge_base.get_key_attribute_of_object(object_type)
         )
 
         last_object = None if len(objects) > 1 else objects[0][key_attribute]
 
-        # To prevent the user to first ask to list the objects for an object type,
-        # the object type has to be extracted while the action is executed.
-        # Therefore we need to reset the SLOT_OBJECT_TYPE to
-        # None to enable this functionality.
-
         slots = [
-            SlotSet(SLOT_OBJECT_TYPE, None),
+            SlotSet(SLOT_OBJECT_TYPE, object_type),
             SlotSet(SLOT_MENTION, None),
             SlotSet(SLOT_ATTRIBUTE, None),
             SlotSet(SLOT_LAST_OBJECT, last_object),
             SlotSet(SLOT_LAST_OBJECT_TYPE, object_type),
             SlotSet(
                 SLOT_LISTED_OBJECTS, list(map(lambda e: e[key_attribute], objects))
             ),
@@ -233,14 +215,15 @@
 
         Args:
             dispatcher: the dispatcher
             tracker: the tracker
 
         Returns: list of slots
         """
+
         object_name = get_object_name(
             tracker,
             self.knowledge_base.ordinal_mention_mapping,
             self.use_last_object_mention,
         )
 
         if object_name is None or not attribute:
@@ -271,21 +254,16 @@
 
         await utils.call_potential_coroutine(
             self.utter_attribute_value(
                 dispatcher, object_representation, attribute, value
             )
         )
 
-        # To prevent the user to first ask to list the objects for an object type,
-        # the object type has to be extracted while the action is executed.
-        # Therefore we need to reset the SLOT_OBJECT_TYPE to
-        # None to enable this functionality.
-
         slots = [
-            SlotSet(SLOT_OBJECT_TYPE, None),
+            SlotSet(SLOT_OBJECT_TYPE, object_type),
             SlotSet(SLOT_ATTRIBUTE, None),
             SlotSet(SLOT_MENTION, None),
             SlotSet(SLOT_LAST_OBJECT, object_identifier),
             SlotSet(SLOT_LAST_OBJECT_TYPE, object_type),
         ]
 
         return slots
```

### Comparing `rasa_sdk-3.6.0/rasa_sdk/knowledge_base/storage.py` & `rasa_sdk-3.6.0a1/rasa_sdk/knowledge_base/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from rasa_sdk import utils
 
 logger = logging.getLogger(__name__)
 
 
 class KnowledgeBase:
     def __init__(self) -> None:
+
         self.ordinal_mention_mapping = {
             "1": lambda lst: lst[0],
             "2": lambda lst: lst[1],
             "3": lambda lst: lst[2],
             "4": lambda lst: lst[3],
             "5": lambda lst: lst[4],
             "6": lambda lst: lst[5],
@@ -105,20 +106,14 @@
             object_identifier: value of the key attribute or the string
             representation of the object
 
         Returns: the object of interest
         """
         raise NotImplementedError("Method is not implemented.")
 
-    def get_object_types(self) -> List[Text]:
-        """
-        Returns a list of object types from knowledge base data.
-        """
-        raise NotImplementedError("Method is not implemented.")
-
 
 class InMemoryKnowledgeBase(KnowledgeBase):
     def __init__(self, data_file: Text) -> None:
         """
         Initialize the in-memory knowledge base.
         Loads the data from the given data file into memory.
 
@@ -207,14 +202,15 @@
     async def get_object(
         self, object_type: Text, object_identifier: Text
     ) -> Optional[Dict[Text, Any]]:
         if object_type not in self.data:
             return None
 
         objects = self.data[object_type]
+
         key_attribute = await utils.call_potential_coroutine(
             self.get_key_attribute_of_object(object_type)
         )
 
         # filter the objects by its key attribute, for example, 'id'
         objects_of_interest = list(
             filter(
@@ -242,11 +238,7 @@
         if not objects_of_interest or len(objects_of_interest) > 1:
             # TODO:
             #  if multiple objects are found, the objects could be shown
             #  to the user. the user then needs to clarify what object he meant.
             return None
 
         return objects_of_interest[0]
-
-    def get_object_types(self) -> List[Text]:
-        """See parent class docstring."""
-        return list(self.data.keys())
```

### Comparing `rasa_sdk-3.6.0/rasa_sdk/knowledge_base/utils.py` & `rasa_sdk-3.6.0a1/rasa_sdk/knowledge_base/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -78,29 +78,28 @@
     Returns: name of the actually object
     """
 
     mention = tracker.get_slot(SLOT_MENTION)
     listed_items = tracker.get_slot(SLOT_LISTED_OBJECTS)
     last_object = tracker.get_slot(SLOT_LAST_OBJECT)
     last_object_type = tracker.get_slot(SLOT_LAST_OBJECT_TYPE)
+    current_object_type = tracker.get_slot(SLOT_OBJECT_TYPE)
 
     if not mention:
         return None
 
     if listed_items and mention in ordinal_mention_mapping:
         idx_function = ordinal_mention_mapping[mention]
         return idx_function(listed_items)
 
     # NOTE:
     # for now we just assume that if the user refers to an object, for
     # example via "it" or "that restaurant", they are actually referring to the last
     # object that was detected.
-    # Since object type slot is reset to 'None' value, it is sufficient to only check
-    # whether the last_object_type is not None.
-    if last_object_type:
+    if current_object_type == last_object_type:
         return last_object
 
     return None
 
 
 def get_attribute_slots(
     tracker: "Tracker", object_attributes: List[Text]
@@ -161,33 +160,7 @@
 
     for attr in object_attributes:
         attr_val = tracker.get_slot(attr) if attr in tracker.slots else None
         if attr_val is not None:
             slots.append(SlotSet(attr, None))
 
     return slots
-
-
-def match_extracted_entities_to_object_type(
-    tracker: "Tracker",
-    object_types: List[Text],
-) -> Optional[Text]:
-    """
-    If the user ask a question about an attribute using an object name and
-    without specifying the object type, then this function searches the
-    corresponding object type. (e.g: when user asks'price range of B&B', this
-    function extracts the object type as 'hotel'). Here we assume that the user
-    message contains reference only to one object type in the knowledge base.
-
-    Args:
-        tracker: the tracker
-        object_types: list of object types in the knowledge base
-
-    Returns: the name of the object type if found, otherwise `None`.
-    """
-    entities = tracker.latest_message.get("entities", [])
-    entity_names = [entity.get("entity") for entity in entities]
-    for entity in entity_names:
-        if entity in object_types:
-            return entity
-
-    return None
```

### Comparing `rasa_sdk-3.6.0/rasa_sdk/plugin.py` & `rasa_sdk-3.6.0a1/rasa_sdk/plugin.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.6.0/rasa_sdk/slots.py` & `rasa_sdk-3.6.0a1/rasa_sdk/slots.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.6.0/rasa_sdk/types.py` & `rasa_sdk-3.6.0a1/rasa_sdk/types.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.6.0/rasa_sdk/utils.py` & `rasa_sdk-3.6.0a1/rasa_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.6.0/PKG-INFO` & `rasa_sdk-3.6.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rasa-sdk
-Version: 3.6.0
+Version: 3.6.0a1
 Summary: Open source machine learning framework to automate text- and voice-based conversations: NLU, dialogue management, connect to Slack, Facebook, and more - Create chatbots and voice assistants
 Home-page: https://rasa.com
 License: Apache-2.0
 Keywords: nlp,machine-learning,machine-learning-library,bot,bots,botkit,rasa conversational-agents,conversational-ai,chatbot,chatbot-framework,bot-framework
 Author: Rasa Technologies GmbH
 Author-email: hi@rasa.com
 Maintainer: Tom Bocklisch
```

