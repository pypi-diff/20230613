# Comparing `tmp/routingfilter-1.4.1.tar.gz` & `tmp/routingfilter-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "routingfilter-1.4.1.tar", last modified: Wed May 31 09:00:58 2023, max compression
+gzip compressed data, was "routingfilter-1.5.1.tar", last modified: Tue Jun 13 14:18:42 2023, max compression
```

## Comparing `routingfilter-1.4.1.tar` & `routingfilter-1.5.1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:58.764170 routingfilter-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-31 09:00:43.000000 routingfilter-1.4.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 09:00:43.000000 routingfilter-1.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-31 09:00:58.764170 routingfilter-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-31 09:00:43.000000 routingfilter-1.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-31 09:00:43.000000 routingfilter-1.4.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:58.764170 routingfilter-1.4.1/routingfilter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:43.000000 routingfilter-1.4.1/routingfilter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9749 2023-05-31 09:00:43.000000 routingfilter-1.4.1/routingfilter/configfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-05-31 09:00:43.000000 routingfilter-1.4.1/routingfilter/dictquery.py
--rw-r--r--   0 runner    (1001) docker     (123)     8710 2023-05-31 09:00:43.000000 routingfilter-1.4.1/routingfilter/routing.py
--rw-r--r--   0 runner    (1001) docker     (123)    14920 2023-05-31 09:00:43.000000 routingfilter-1.4.1/routingfilter/routing_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:58.764170 routingfilter-1.4.1/routingfilter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-31 09:00:58.000000 routingfilter-1.4.1/routingfilter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-31 09:00:58.000000 routingfilter-1.4.1/routingfilter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 09:00:58.000000 routingfilter-1.4.1/routingfilter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-31 09:00:58.000000 routingfilter-1.4.1/routingfilter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-31 09:00:58.000000 routingfilter-1.4.1/routingfilter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 09:00:58.764170 routingfilter-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-31 09:00:43.000000 routingfilter-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:18:42.868234 routingfilter-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-13 14:18:25.000000 routingfilter-1.5.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 14:18:25.000000 routingfilter-1.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-13 14:18:42.868234 routingfilter-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-13 14:18:25.000000 routingfilter-1.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-13 14:18:25.000000 routingfilter-1.5.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:18:42.864234 routingfilter-1.5.1/routingfilter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 14:18:25.000000 routingfilter-1.5.1/routingfilter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9749 2023-06-13 14:18:25.000000 routingfilter-1.5.1/routingfilter/configfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-06-13 14:18:25.000000 routingfilter-1.5.1/routingfilter/dictquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9642 2023-06-13 14:18:25.000000 routingfilter-1.5.1/routingfilter/routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40228 2023-06-13 14:18:25.000000 routingfilter-1.5.1/routingfilter/routing_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19251 2023-06-13 14:18:25.000000 routingfilter-1.5.1/routingfilter/routing_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:18:42.868234 routingfilter-1.5.1/routingfilter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-13 14:18:42.000000 routingfilter-1.5.1/routingfilter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-13 14:18:42.000000 routingfilter-1.5.1/routingfilter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 14:18:42.000000 routingfilter-1.5.1/routingfilter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-13 14:18:42.000000 routingfilter-1.5.1/routingfilter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 14:18:42.000000 routingfilter-1.5.1/routingfilter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 14:18:42.868234 routingfilter-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-13 14:18:25.000000 routingfilter-1.5.1/setup.py
```

### Comparing `routingfilter-1.4.1/LICENSE.txt` & `routingfilter-1.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `routingfilter-1.4.1/routingfilter/configfilter.py` & `routingfilter-1.5.1/routingfilter/configfilter.py`

 * *Files identical despite different names*

### Comparing `routingfilter-1.4.1/routingfilter/dictquery.py` & `routingfilter-1.5.1/routingfilter/dictquery.py`

 * *Files identical despite different names*

### Comparing `routingfilter-1.4.1/routingfilter/routing.py` & `routingfilter-1.5.1/routingfilter/routing.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import copy
+from datetime import datetime
 import json
 import logging
 
 from routingfilter.configfilter import ConfigFilter
 from typing import List, Optional
 
 
@@ -31,14 +32,16 @@
         :param type_: The event type (can be 'streams', 'customer' or everything else, as defined in the routing config). If the type does not exists, an empty list is returned
         :type type_: str
         :param tag_field_name: The event field to search into (default='tags')
         :type tag_field_name: str
         :return: A list of dicts containing the matched rules and the outputs in the following format: {"rules": [...], "output": {...}}; an empty list if no rule matched
         :rtype: List[dict]
         """
+        if not event.get("certego", {}).get("routing_history", {}):
+            event["certego"] = {"routing_history": {}}
         if not self.rules:
             self.logger.error("'rules_list' must be set before evaluating a match!")
             raise ValueError("'rules_list' must be set before evaluating a match!")
         if type_ not in self.rules:
             return []
 
         # iterate through the common set of tags
@@ -57,32 +60,34 @@
         if "all" in streams_tags:
             # the first matching rule wins
             rules = self.rules[type_]["rules"]["all"]
             rules = rules if rules else []
             for rule in rules:
                 # check if ALL the filters are matching
                 filters = [ConfigFilter(f) for f in rule.get("filters", [])]
-                if all(f.is_matching(event) for f in filters):
+                if all(f.is_matching(event) for f in filters) and not self.rule_in_routing_history(event, rule):
                     matching_rules.append(rule)
                     break
         if not matching_rules:
             for tag_field_name in msg_tags:
                 for rule in self.rules[type_]["rules"].get(tag_field_name, []):
                     # check if ALL the filters are matching
                     config_filters = [ConfigFilter(f) for f in rule.get("filters", [])]
-                    if config_filters and all(f.is_matching(event) for f in config_filters):
+                    if config_filters and all(f.is_matching(event) for f in config_filters) and not self.rule_in_routing_history(event, rule):
                         matching_rules.append(rule)
-                        break  # the first matching rule wins
+                        break  # the first matching rule wins if it doesn't exist in the output field
         # Rename "filters" to "rules" and "type" to "output" to be more generic
         matching_rules = copy.deepcopy(matching_rules)
         for mr in matching_rules:
             if "filters" in mr:
                 mr["rules"] = mr.pop("filters")
             if type_ in mr:
                 mr["output"] = mr.pop(type_)
+                if len(mr["output"]) > 0:
+                    event["certego"]["routing_history"][list(mr["output"].keys())[0]] = datetime.now().isoformat()
         return matching_rules
 
     def load_from_dicts(self, rules_list: List[dict], validate_rules: bool = True, variables: Optional[dict] = None) -> None:
         """Load routing configuration from a dictionary. It merges the different rules in list into a single routing rule.
         It optionally performs some rules validation before accepting them (an exception is raised in case of errors).
 
         :param rules_list: The configuration
@@ -168,7 +173,22 @@
         self.logger.info("Validating the loaded rules_list")
         for type_ in rules.keys():
             for tag_ in rules[type_]["rules"].keys():
                 for filter_output in rules[type_]["rules"][tag_]:
                     for filter_ in filter_output["filters"]:
                         config_filter_obj = ConfigFilter(filter_)
                         config_filter_obj.is_matching({})
+
+    def rule_in_routing_history(self, event, rule):
+        """Checking if the given rule has already been processed
+
+        :param event: The entire event to process
+        :type event: dict
+        :param rule: The rule to check
+        :type rule: dict
+        """
+        if rule["streams"] is None:
+            return False
+        for key in rule["streams"].keys():
+            if key in event["certego"]["routing_history"]:
+                return True
+        return False
```

### Comparing `routingfilter-1.4.1/routingfilter/routing_test.py` & `routingfilter-1.5.1/routingfilter/routing_test.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,37 +13,36 @@
     return data
 
 
 class RoutingTestCase(unittest.TestCase):
     """Class to tests routing.py file. These tests loads sample events from JSON files in 'test_data' folder
     and test if the routing rules are working correctly."""
 
-    # Load frequently accessed test data from JSON files
-    test_event_1 = load_test_data("test_event_1")
-    test_event_2 = load_test_data("test_event_2")
-    test_event_3 = load_test_data("test_event_3")
-    test_event_4 = load_test_data("test_event_4")
-    test_event_5 = load_test_data("test_event_5")
-    test_event_6 = load_test_data("test_event_6")
-    test_event_7 = load_test_data("test_event_7")
-    test_event_8 = load_test_data("test_event_8")
-    test_event_9 = load_test_data("test_event_9")
-    test_event_10 = load_test_data("test_event_10")
-    test_event_11 = load_test_data("test_event_11")
-    test_event_12 = load_test_data("test_event_12")
-    test_event_13 = load_test_data("test_event_13")
-    test_event_14 = load_test_data("test_event_14")
-    test_event_15 = load_test_data("test_event_15")
-    test_event_16 = load_test_data("test_event_16")
-    test_event_17 = load_test_data("test_event_17")
-    test_event_with_list_1 = load_test_data("test_event_with_list_1")
-    test_event_with_list_2 = load_test_data("test_event_with_list_2")
-
     def setUp(self):
         self.routing = Routing()
+        # Load frequently accessed test data from JSON files
+        self.test_event_1 = load_test_data("test_event_1")
+        self.test_event_2 = load_test_data("test_event_2")
+        self.test_event_3 = load_test_data("test_event_3")
+        self.test_event_4 = load_test_data("test_event_4")
+        self.test_event_5 = load_test_data("test_event_5")
+        self.test_event_6 = load_test_data("test_event_6")
+        self.test_event_7 = load_test_data("test_event_7")
+        self.test_event_8 = load_test_data("test_event_8")
+        self.test_event_9 = load_test_data("test_event_9")
+        self.test_event_10 = load_test_data("test_event_10")
+        self.test_event_11 = load_test_data("test_event_11")
+        self.test_event_12 = load_test_data("test_event_12")
+        self.test_event_13 = load_test_data("test_event_13")
+        self.test_event_14 = load_test_data("test_event_14")
+        self.test_event_15 = load_test_data("test_event_15")
+        self.test_event_16 = load_test_data("test_event_16")
+        self.test_event_17 = load_test_data("test_event_17")
+        self.test_event_with_list_1 = load_test_data("test_event_with_list_1")
+        self.test_event_with_list_2 = load_test_data("test_event_with_list_2")
 
     def test_wrong_inputs(self):
         self.assertIsNone(self.routing.get_rules())
         with self.assertRaises(ValueError):
             self.routing.match({})
         self.routing.load_from_dicts([load_test_data("test_rule_1_equals")])
         self.assertEqual(self.routing.match(self.test_event_1, "wrong_type"), [])
@@ -69,14 +68,46 @@
         rule_all = load_test_data("test_rule_2_all_equals")
         filter_2 = copy.deepcopy(rule_all["streams"]["rules"]["all"][0])
         filter_2["streams"] = {"Other": None}
         rule_all["streams"]["rules"]["all"].append(filter_2)
         self.routing.load_from_dicts([rule_all])
         self.assertDictEqual(self.routing.match(self.test_event_1)[0]["output"], {'Workshop': {'workers_needed': 1}})
 
+    def test_routing_history(self):
+        self.routing.load_from_dicts([load_test_data("test_rule_24_routing_history")])
+        self.routing.match(self.test_event_1)
+        self.assertTrue(self.test_event_1["certego"]["routing_history"]["Workshop"])
+        # Check if the rule is processed twice
+        self.assertTrue("Workshop" in self.test_event_1["certego"]["routing_history"])
+        self.assertFalse("TyreFit" in self.test_event_1["certego"]["routing_history"])
+        # Just the second rule has to be parsed
+        self.routing.match(self.test_event_1)
+        self.assertTrue("Workshop" in self.test_event_1["certego"]["routing_history"])
+        self.assertTrue("TyreFit" in self.test_event_1["certego"]["routing_history"])
+        
+    def test_routing_history_stream_none(self):
+        self.routing.load_from_dicts([load_test_data("test_rule_1_equals")])
+        self.routing.match(self.test_event_1)
+        self.assertTrue(self.test_event_1["certego"]["routing_history"]["Workshop"])
+        self.routing.load_from_dicts([load_test_data("test_rule_25_routing_history_streams_none")])
+        self.routing.match(self.test_event_1)
+        self.assertEqual(len(self.test_event_1["certego"]["routing_history"].keys()), 1)
+
+    def test_routing_history_same_rule_twice(self):
+            workshop_count = 0
+            self.routing.load_from_dicts([load_test_data("test_rule_1_equals")])
+            self.routing.match(self.test_event_1)
+            self.assertTrue(self.test_event_1["certego"]["routing_history"]["Workshop"])
+            self.routing.load_from_dicts([load_test_data("test_rule_1_equals")])
+            self.routing.match(self.test_event_1)
+            for key in self.test_event_1["certego"]["routing_history"].keys():
+                if key == "Workshop":
+                    workshop_count = workshop_count + 1
+            self.assertEqual(workshop_count, 1)
+
     def test_rule_1(self):
         # Test rule loading and applying with full output
         self.routing.load_from_dicts([load_test_data("test_rule_1_equals")])
         self.assertDictEqual(self.routing.match(self.test_event_1)[0], load_test_data("test_event_1_rule_1_response"))
         self.assertEqual(self.routing.match(self.test_event_2), [])
         self.assertEqual(self.routing.match(self.test_event_3), [])
 
@@ -108,14 +139,19 @@
         # Test merge with special tag 'all' (matches all tags)
         test_rule_1_equals = load_test_data("test_rule_1_equals")
         test_rule_2_all_equals = load_test_data("test_rule_2_all_equals")
         self.routing.load_from_dicts([test_rule_1_equals, test_rule_2_all_equals])
         self.assertDictEqual(self.routing.match(self.test_event_1)[0], load_test_data("test_event_1_rule_1_response"))
         self.assertDictEqual(self.routing.match(self.test_event_2)[0], load_test_data("test_event_1_rule_1_response"))
         self.assertEqual(self.routing.match(self.test_event_3), [])
+        
+
+    def test_special_tag_all2(self):
+        test_rule_1_equals = load_test_data("test_rule_1_equals")
+        test_rule_2_all_equals = load_test_data("test_rule_2_all_equals")
         test_rule_2_all_equals["streams"]["rules"]["all"][0]["filters"][0]["key"] = "wheel_model_wrong"
         self.routing.load_from_dicts([test_rule_1_equals, test_rule_2_all_equals])
         self.assertDictEqual(self.routing.match(self.test_event_1)[0], load_test_data("test_event_1_rule_1_response"))
         self.assertEqual(self.routing.match(load_test_data("test_event_2")), [])
 
     def test_event_with_multiple_tags(self):
         test_rule_1_equals = load_test_data("test_rule_1_equals")
@@ -131,117 +167,192 @@
         self.assertEqual(len(self.routing.match(test_event_4_mod)), 2)
 
     def test_event_wrong_field_name(self):
         test_rule_7 = load_test_data("test_rule_7_wrongfield")
         self.routing.load_from_dicts([test_rule_7])
         self.assertEqual(self.routing.match(self.test_event_7), [])
 
-    def test_single_filters(self):
-        # Test all filter types defined in ConfigFilter
+    def test_single_filters_ALL(self):
         self.routing.load_from_dicts([load_test_data("test_rule_0_all")])  # ALL
         self.assertTrue(self.routing.match(self.test_event_1))
         self.assertFalse(self.routing.match(self.test_event_2))
         self.assertTrue(self.routing.match(self.test_event_3))
         self.assertFalse(self.routing.match(self.test_event_4))
+
+    def test_single_filters_EQUALS(self):
         self.routing.load_from_dicts([load_test_data("test_rule_1_equals")])  # EQUALS
         self.assertTrue(self.routing.match(self.test_event_1))
         self.assertFalse(self.routing.match(self.test_event_3))
+    
+    def test_single_filters_NOT_EQUALS(self):
         self.routing.load_from_dicts([load_test_data("test_rule_1_not_equals")])  # NOT EQUALS
         self.assertFalse(self.routing.match(self.test_event_1))
         self.assertTrue(self.routing.match(self.test_event_3))
+
+    def test_single_filters_STARTSWITH(self):
         self.routing.load_from_dicts([load_test_data("test_rule_6_startswith")])  # STARTSWITH
         self.assertTrue(self.routing.match(self.test_event_1))
         self.assertFalse(self.routing.match(self.test_event_3))
+
+    def test_single_filters_KEYWORD(self):
         self.routing.load_from_dicts([load_test_data("test_rule_7_keyword")])  # KEYWORD
         self.assertTrue(self.routing.match(self.test_event_1))
         self.assertFalse(self.routing.match(self.test_event_3))
+
+    def test_single_filters_REGEXP(self):
         self.routing.load_from_dicts([load_test_data("test_rule_8_regexp")])  # REGEXP
         self.assertTrue(self.routing.match(self.test_event_1))
         self.assertFalse(self.routing.match(self.test_event_3))
+
+    def test_single_filters_DOMAIN(self):
         self.routing.load_from_dicts([load_test_data("test_rule_11_domain")])  # DOMAIN
         self.assertTrue(self.routing.match(self.test_event_4))
         self.assertFalse(self.routing.match(self.test_event_5))
+
+    def test_single_filters_GREATER(self):
         self.routing.load_from_dicts([load_test_data("test_rule_12_greater")])  # GREATER
         self.assertFalse(self.routing.match({}))
         self.assertTrue(self.routing.match(self.test_event_1))
         self.assertFalse(self.routing.match(self.test_event_3))
         with self.assertRaises(ValueError):
             event_2 = self.test_event_2
             event_2["tags"] = "mountain_bike"
             event_2["price"] = "600a"
             self.routing.match(event_2)
+        
+    def test_single_filters_LESS(self):
         self.routing.load_from_dicts([load_test_data("test_rule_13_less")])  # LESS
         self.assertFalse(self.routing.match(self.test_event_1))
         self.assertTrue(self.routing.match(self.test_event_3))
+
+    def test_single_filters_ENDSSWITH(self):
         self.routing.load_from_dicts([load_test_data("test_rule_14_endswith")])  # ENDSSWITH
         self.assertTrue(self.routing.match(self.test_event_1))
         self.assertFalse(self.routing.match(self.test_event_3))
         self.assertFalse(self.routing.match(self.test_event_8))
 
-    def test_single_filter_EXIST_NOT_EXISTS(self):
+    def test_single_filter_EXIST(self):
         self.routing.load_from_dicts([load_test_data("test_rule_5_exists")])  # EXISTS
         self.assertTrue(self.routing.match(self.test_event_1))
         self.assertFalse(self.routing.match(self.test_event_3))
         self.assertTrue(self.routing.match(self.test_event_10))
+    
+    def test_single_filter_NOT_EXISTS(self):
         self.routing.load_from_dicts([load_test_data("test_rule_6_not_exists")])  # NOT_EXISTS
         self.assertFalse(self.routing.match(self.test_event_1))
         self.assertTrue(self.routing.match(self.test_event_3))
         self.assertFalse(self.routing.match(self.test_event_10))
 
-    def test_single_filter_NETWORK_NOT_NETWORK(self):
+    def test_single_filter_NETWORK(self):
         self.routing.load_from_dicts([load_test_data("test_rule_9_network")])  # NETWORK
         self.assertTrue(self.routing.match(self.test_event_4))
         self.assertFalse(self.routing.match(self.test_event_9))
         self.assertFalse(self.routing.match(self.test_event_6))  # Unparsable
+
+    def test_single_filter_NOT_NETWORK(self):
         self.routing.load_from_dicts([load_test_data("test_rule_10_not_network")])  # NOT_NETWORK
         self.assertFalse(self.routing.match(self.test_event_4))
         self.assertTrue(self.routing.match(self.test_event_5))
         self.assertFalse(self.routing.match(self.test_event_3))
         self.assertTrue(self.routing.match(self.test_event_9))
         self.assertTrue(self.routing.match(self.test_event_6))  # Unparsable
 
     def test_event_with_lists_as_fields(self):
         self.routing.load_from_dicts([load_test_data("test_rule_9_network")])  # NETWORK
         self.assertTrue(self.routing.match(self.test_event_with_list_1))
 
         self.routing.load_from_dicts([load_test_data("test_rule_1_equals")])
         self.assertTrue(self.routing.match(self.test_event_with_list_2))
 
-    def test_single_filter_TYPEOF(self):
+    def test_single_filter_TYPEOF_exception(self):
         # if self.value is a list, it returns True if almost one type is correct
         self.routing.load_from_dicts([load_test_data("test_rule_15_typeof_exception")]) # "value": ["str", "int", "dict"]
         self.assertTrue(self.routing.match(self.test_event_8))      # value: "str"
         self.assertTrue(self.routing.match(self.test_event_11))     # value: "int"
         self.assertTrue(self.routing.match(self.test_event_13))     # value: "dict"
         self.assertFalse(self.routing.match(self.test_event_12))
+
+    def test_single_filter_TYPEOF_str(self):
         self.routing.load_from_dicts([load_test_data("test_rule_16_typeof_str")])   # is_str
         self.assertTrue(self.routing.match(self.test_event_8))
         self.assertFalse(self.routing.match(self.test_event_10))    # is_not_str
+
+    def test_single_filter_TYPEOF_int(self):
         self.routing.load_from_dicts([load_test_data("test_rule_17_typeof_int")])   # is_int
         self.assertTrue(self.routing.match(self.test_event_11))
         self.assertFalse(self.routing.match(self.test_event_8))     # is_not_int
+
+    def test_single_filter_TYPEOF_bool(self):
         self.routing.load_from_dicts([load_test_data("test_rule_18_typeof_bool")])   # is_bool
         self.assertTrue(self.routing.match(self.test_event_12))
         self.assertFalse(self.routing.match(self.test_event_8))     # is_not_bool
+    
+    def test_single_filter_TYPEOF_list(self):
         self.routing.load_from_dicts([load_test_data("test_rule_19_typeof_list")])  # is_list
         self.assertTrue(self.routing.match(self.test_event_10))
         self.assertFalse(self.routing.match(self.test_event_8))    # is_not_list
+
+    def test_single_filter_TYPEOF_dict(self):
         self.routing.load_from_dicts([load_test_data("test_rule_20_typeof_dict")])  # is_dict
         self.assertTrue(self.routing.match(self.test_event_13))
         self.assertFalse(self.routing.match(self.test_event_11))    # is_not_dict
+
+    def test_single_filter_TYPEOF_ip_address(self):
         self.routing.load_from_dicts([load_test_data("test_rule_21_typeof_ip")])  # is_ipv4
         self.assertTrue(self.routing.match(self.test_event_15))
         self.assertTrue(self.routing.match(self.test_event_16))     # is_ipv6
         self.assertFalse(self.routing.match(self.test_event_11))    # insert an integer
         self.assertFalse(self.routing.match(self.test_event_14))    # insert a string with a number: ex. "8"
         self.assertFalse(self.routing.match(self.test_event_12))    # is_not_ip
+
+    def test_single_filter_TYPEOF_mac_address(self):
         self.routing.load_from_dicts([load_test_data("test_rule_22_typeof_mac")])    # is_mac
         self.assertTrue(self.routing.match(self.test_event_17))
         self.assertFalse(self.routing.match(self.test_event_16))    # is_not_mac
         # key doesn't exist
         self.assertFalse(self.routing.match(self.test_event_5))
 
     def test_variables(self):
         self.routing.load_from_dicts([load_test_data("test_rule_23_network_variables")])
         self.assertFalse(self.routing.match(self.test_event_4))
         self.routing.load_from_dicts([load_test_data("test_rule_23_network_variables")], variables={"$INTERNAL_IPS": "192.168.0.0/16"})
         self.assertTrue(self.routing.match(self.test_event_4))
+
+    def test_rule_in_routing_history(self):
+        event = {"certego": {"routing_history": {}}}
+        rule = {
+            "filters": [
+              {
+                "type": "EQUALS",
+                "key": "wheel_model",
+                "description": "Carbon fiber wheels needs manual truing",
+                "value": [
+                  "Superlight",
+                  "RacePro"
+                ]
+              }
+            ],
+            "streams": {
+            }
+          }
+        self.assertFalse(self.routing.rule_in_routing_history(event, rule))
+        event = {"certego": {"routing_history": {"Workshop": "2023-06-06T18:00:00.000Z"}}}
+        self.assertFalse(self.routing.rule_in_routing_history(event, rule))
+        rule = {
+            "filters": [
+              {
+                "type": "EQUALS",
+                "key": "wheel_model",
+                "description": "Carbon fiber wheels needs manual truing",
+                "value": [
+                  "Superlight",
+                  "RacePro"
+                ]
+              }
+            ],
+            "streams": {
+                "Workshop": {
+                    "workers_needed": 1
+                }
+            }
+          }
+        self.assertTrue(self.routing.rule_in_routing_history(event, rule))
```

### Comparing `routingfilter-1.4.1/setup.py` & `routingfilter-1.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as readme_file:
     long_description = readme_file.read()
 
 setup(
     name='routingfilter',
-    version='1.4.1',
+    version='1.5.1',
     packages=['routingfilter'],
     include_package_data=True,
     install_requires=["IPy~=1.1", "macaddress~=2.0.2"],
     url='https://github.com/certego/RoutingFilter',
     license='GNU LGPLv3',
     author='Certego S.r.l.',
     author_email='support@certego.net',
```

