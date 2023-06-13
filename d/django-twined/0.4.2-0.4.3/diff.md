# Comparing `tmp/django_twined-0.4.2.tar.gz` & `tmp/django_twined-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_twined-0.4.2.tar", max compression
+gzip compressed data, was "django_twined-0.4.3.tar", max compression
```

## Comparing `django_twined-0.4.2.tar` & `django_twined-0.4.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0     1088 2023-05-05 16:50:04.055920 django_twined-0.4.2/LICENSE
--rw-r--r--   0        0        0     1463 2023-05-05 16:50:04.055920 django_twined-0.4.2/README.md
--rw-r--r--   0        0        0       64 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/__init__.py
--rw-r--r--   0        0        0      257 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/admin/__init__.py
--rw-r--r--   0        0        0     6781 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/admin/admin.py
--rw-r--r--   0        0        0      402 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/admin/fieldsets.py
--rw-r--r--   0        0        0      881 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/admin/mixins.py
--rw-r--r--   0        0        0      682 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/admin/proxy.py
--rw-r--r--   0        0        0      496 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/apps.py
--rw-r--r--   0        0        0      104 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/consumers/__init__.py
--rw-r--r--   0        0        0     3765 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/consumers/analysis.py
--rw-r--r--   0        0        0     1001 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/consumers/analysis_log.py
--rw-r--r--   0        0        0     5822 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/consumers/service.py
--rw-r--r--   0        0        0      130 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/exceptions.py
--rw-r--r--   0        0        0     2357 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/fields.py
--rw-r--r--   0        0        0        0 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/management/__init__.py
--rw-r--r--   0        0        0        0 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/management/commands/__init__.py
--rw-r--r--   0        0        0     2299 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/management/commands/sync_data_stores.py
--rw-r--r--   0        0        0     2990 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/messages.py
--rw-r--r--   0        0        0     2345 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/migrations/0001_initial.py
--rw-r--r--   0        0        0      595 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/migrations/0002_slug_unique_and_not_editable.py
--rw-r--r--   0        0        0      408 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/migrations/0003_rename_slug_to_name.py
--rw-r--r--   0        0        0      670 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/migrations/0004_add_timestamps.py
--rw-r--r--   0        0        0      731 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/migrations/0005_question_date_help_text.py
--rw-r--r--   0        0        0     4710 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/migrations/0006_service_revisions_and_events.py
--rw-r--r--   0        0        0     1476 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/migrations/0007_registered_to_revision.py
--rw-r--r--   0        0        0      669 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/migrations/0008_registered_relations_to_nullable.py
--rw-r--r--   0        0        0      683 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/migrations/0009_remove_registered_services.py
--rw-r--r--   0        0        0      681 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/migrations/0010_alter_servicerevision_project_name.py
--rw-r--r--   0        0        0      362 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/migrations/0011_remove_servicerevision_topic_id.py
--rw-r--r--   0        0        0      568 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/migrations/0012_servicerevision_is_default.py
--rw-r--r--   0        0        0      639 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/migrations/0013_alter_serviceusageevent_question.py
--rw-r--r--   0        0        0        0 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/migrations/__init__.py
--rw-r--r--   0        0        0      698 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/models/__init__.py
--rw-r--r--   0        0        0    11448 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/models/datastores.py
--rw-r--r--   0        0        0       85 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/models/querysets/__init__.py
--rw-r--r--   0        0        0     9794 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/models/querysets/datastore_queryset.py
--rw-r--r--   0        0        0     6623 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/models/questions.py
--rw-r--r--   0        0        0     7824 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/models/service_revisions.py
--rw-r--r--   0        0        0     2514 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/models/service_usage_events.py
--rw-r--r--   0        0        0      290 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/routing.py
--rw-r--r--   0        0        0      479 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/signals/__init__.py
--rw-r--r--   0        0        0     3079 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/signals/receivers.py
--rw-r--r--   0        0        0      262 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/signals/senders.py
--rw-r--r--   0        0        0        0 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/static/.gitignore
--rw-r--r--   0        0        0     2666 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/tasks.py
--rw-r--r--   0        0        0     1149 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/templates/admin/question_ask_row.html
--rw-r--r--   0        0        0        0 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/templates/django_twined/.gitignore
--rw-r--r--   0        0        0      343 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/templates/django_twined/question_changeform.html
--rw-r--r--   0        0        0        0 2023-05-05 16:50:04.059920 django_twined-0.4.2/django_twined/templatetags/__init__.py
--rw-r--r--   0        0        0      480 2023-05-05 16:50:04.059920 django_twined-0.4.2/django_twined/templatetags/question_ask_row.py
--rw-r--r--   0        0        0     1532 2023-05-05 16:50:04.059920 django_twined-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     2700 1970-01-01 00:00:00.000000 django_twined-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-06-13 08:00:29.727306 django_twined-0.4.3/LICENSE
+-rw-r--r--   0        0        0     1463 2023-06-13 08:00:29.727306 django_twined-0.4.3/README.md
+-rw-r--r--   0        0        0       64 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/__init__.py
+-rw-r--r--   0        0        0      257 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/admin/__init__.py
+-rw-r--r--   0        0        0     6781 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/admin/admin.py
+-rw-r--r--   0        0        0      402 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/admin/fieldsets.py
+-rw-r--r--   0        0        0      881 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/admin/mixins.py
+-rw-r--r--   0        0        0      682 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/admin/proxy.py
+-rw-r--r--   0        0        0      496 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/apps.py
+-rw-r--r--   0        0        0      104 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/consumers/__init__.py
+-rw-r--r--   0        0        0     3765 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/consumers/analysis.py
+-rw-r--r--   0        0        0     1001 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/consumers/analysis_log.py
+-rw-r--r--   0        0        0     5822 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/consumers/service.py
+-rw-r--r--   0        0        0      130 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/exceptions.py
+-rw-r--r--   0        0        0     2357 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/fields.py
+-rw-r--r--   0        0        0        0 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/management/commands/__init__.py
+-rw-r--r--   0        0        0     2299 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/management/commands/sync_data_stores.py
+-rw-r--r--   0        0        0     2990 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/messages.py
+-rw-r--r--   0        0        0     2345 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/migrations/0001_initial.py
+-rw-r--r--   0        0        0      595 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/migrations/0002_slug_unique_and_not_editable.py
+-rw-r--r--   0        0        0      408 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/migrations/0003_rename_slug_to_name.py
+-rw-r--r--   0        0        0      670 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/migrations/0004_add_timestamps.py
+-rw-r--r--   0        0        0      731 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/migrations/0005_question_date_help_text.py
+-rw-r--r--   0        0        0     4710 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/migrations/0006_service_revisions_and_events.py
+-rw-r--r--   0        0        0     1476 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/migrations/0007_registered_to_revision.py
+-rw-r--r--   0        0        0      669 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/migrations/0008_registered_relations_to_nullable.py
+-rw-r--r--   0        0        0      683 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/migrations/0009_remove_registered_services.py
+-rw-r--r--   0        0        0      681 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/migrations/0010_alter_servicerevision_project_name.py
+-rw-r--r--   0        0        0      362 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/migrations/0011_remove_servicerevision_topic_id.py
+-rw-r--r--   0        0        0      568 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/migrations/0012_servicerevision_is_default.py
+-rw-r--r--   0        0        0      639 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/migrations/0013_alter_serviceusageevent_question.py
+-rw-r--r--   0        0        0        0 2023-06-13 08:00:29.727306 django_twined-0.4.3/django_twined/migrations/__init__.py
+-rw-r--r--   0        0        0      698 2023-06-13 08:00:29.731306 django_twined-0.4.3/django_twined/models/__init__.py
+-rw-r--r--   0        0        0    11448 2023-06-13 08:00:29.731306 django_twined-0.4.3/django_twined/models/datastores.py
+-rw-r--r--   0        0        0       85 2023-06-13 08:00:29.731306 django_twined-0.4.3/django_twined/models/querysets/__init__.py
+-rw-r--r--   0        0        0     9794 2023-06-13 08:00:29.731306 django_twined-0.4.3/django_twined/models/querysets/datastore_queryset.py
+-rw-r--r--   0        0        0     6623 2023-06-13 08:00:29.731306 django_twined-0.4.3/django_twined/models/questions.py
+-rw-r--r--   0        0        0     7824 2023-06-13 08:00:29.731306 django_twined-0.4.3/django_twined/models/service_revisions.py
+-rw-r--r--   0        0        0     2514 2023-06-13 08:00:29.731306 django_twined-0.4.3/django_twined/models/service_usage_events.py
+-rw-r--r--   0        0        0      290 2023-06-13 08:00:29.731306 django_twined-0.4.3/django_twined/routing.py
+-rw-r--r--   0        0        0      479 2023-06-13 08:00:29.731306 django_twined-0.4.3/django_twined/signals/__init__.py
+-rw-r--r--   0        0        0     3079 2023-06-13 08:00:29.731306 django_twined-0.4.3/django_twined/signals/receivers.py
+-rw-r--r--   0        0        0      262 2023-06-13 08:00:29.731306 django_twined-0.4.3/django_twined/signals/senders.py
+-rw-r--r--   0        0        0        0 2023-06-13 08:00:29.731306 django_twined-0.4.3/django_twined/static/.gitignore
+-rw-r--r--   0        0        0     2666 2023-06-13 08:00:29.731306 django_twined-0.4.3/django_twined/tasks.py
+-rw-r--r--   0        0        0     1149 2023-06-13 08:00:29.731306 django_twined-0.4.3/django_twined/templates/admin/question_ask_row.html
+-rw-r--r--   0        0        0        0 2023-06-13 08:00:29.731306 django_twined-0.4.3/django_twined/templates/django_twined/.gitignore
+-rw-r--r--   0        0        0      343 2023-06-13 08:00:29.731306 django_twined-0.4.3/django_twined/templates/django_twined/question_changeform.html
+-rw-r--r--   0        0        0        0 2023-06-13 08:00:29.731306 django_twined-0.4.3/django_twined/templatetags/__init__.py
+-rw-r--r--   0        0        0      480 2023-06-13 08:00:29.731306 django_twined-0.4.3/django_twined/templatetags/question_ask_row.py
+-rw-r--r--   0        0        0     1532 2023-06-13 08:00:29.731306 django_twined-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     2599 1970-01-01 00:00:00.000000 django_twined-0.4.3/PKG-INFO
```

### Comparing `django_twined-0.4.2/LICENSE` & `django_twined-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.2/README.md` & `django_twined-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.2/django_twined/admin/admin.py` & `django_twined-0.4.3/django_twined/admin/admin.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.2/django_twined/admin/mixins.py` & `django_twined-0.4.3/django_twined/admin/mixins.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.2/django_twined/admin/proxy.py` & `django_twined-0.4.3/django_twined/admin/proxy.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.2/django_twined/consumers/analysis.py` & `django_twined-0.4.3/django_twined/consumers/analysis.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.2/django_twined/consumers/analysis_log.py` & `django_twined-0.4.3/django_twined/consumers/analysis_log.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.2/django_twined/consumers/service.py` & `django_twined-0.4.3/django_twined/consumers/service.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.2/django_twined/fields.py` & `django_twined-0.4.3/django_twined/fields.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.2/django_twined/management/commands/sync_data_stores.py` & `django_twined-0.4.3/django_twined/management/commands/sync_data_stores.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.2/django_twined/messages.py` & `django_twined-0.4.3/django_twined/messages.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.2/django_twined/migrations/0001_initial.py` & `django_twined-0.4.3/django_twined/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.2/django_twined/migrations/0002_slug_unique_and_not_editable.py` & `django_twined-0.4.3/django_twined/migrations/0002_slug_unique_and_not_editable.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.2/django_twined/migrations/0004_add_timestamps.py` & `django_twined-0.4.3/django_twined/migrations/0004_add_timestamps.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.2/django_twined/migrations/0005_question_date_help_text.py` & `django_twined-0.4.3/django_twined/migrations/0005_question_date_help_text.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.2/django_twined/migrations/0006_service_revisions_and_events.py` & `django_twined-0.4.3/django_twined/migrations/0006_service_revisions_and_events.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.2/django_twined/migrations/0007_registered_to_revision.py` & `django_twined-0.4.3/django_twined/migrations/0007_registered_to_revision.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.2/django_twined/migrations/0008_registered_relations_to_nullable.py` & `django_twined-0.4.3/django_twined/migrations/0008_registered_relations_to_nullable.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.2/django_twined/migrations/0009_remove_registered_services.py` & `django_twined-0.4.3/django_twined/migrations/0009_remove_registered_services.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.2/django_twined/migrations/0010_alter_servicerevision_project_name.py` & `django_twined-0.4.3/django_twined/migrations/0010_alter_servicerevision_project_name.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.2/django_twined/migrations/0012_servicerevision_is_default.py` & `django_twined-0.4.3/django_twined/migrations/0012_servicerevision_is_default.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.2/django_twined/migrations/0013_alter_serviceusageevent_question.py` & `django_twined-0.4.3/django_twined/migrations/0013_alter_serviceusageevent_question.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.2/django_twined/models/__init__.py` & `django_twined-0.4.3/django_twined/models/__init__.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.2/django_twined/models/datastores.py` & `django_twined-0.4.3/django_twined/models/datastores.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.2/django_twined/models/querysets/datastore_queryset.py` & `django_twined-0.4.3/django_twined/models/querysets/datastore_queryset.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.2/django_twined/models/questions.py` & `django_twined-0.4.3/django_twined/models/questions.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.2/django_twined/models/service_revisions.py` & `django_twined-0.4.3/django_twined/models/service_revisions.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.2/django_twined/models/service_usage_events.py` & `django_twined-0.4.3/django_twined/models/service_usage_events.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.2/django_twined/signals/receivers.py` & `django_twined-0.4.3/django_twined/signals/receivers.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.2/django_twined/tasks.py` & `django_twined-0.4.3/django_twined/tasks.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.2/django_twined/templates/admin/question_ask_row.html` & `django_twined-0.4.3/django_twined/templates/admin/question_ask_row.html`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.2/pyproject.toml` & `django_twined-0.4.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-twined"
-version = "0.4.2"
+version = "0.4.3"
 description = "A django app to manage octue services"
 authors = ["Tom Clark <tom@octue.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
@@ -21,15 +21,15 @@
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.11"
 django = ">=3.0,<4.0"
 channels = ">=3.0,<4.0"
 octue = "^0.39.0"
 pika = "^1.2.0"
-django-gcp = ">=0.7.3,<0.10"
+django-gcp = ">=0.7.3,<0.11"
 django-jsoneditor = "^0.2.2"
 django-model-utils = "^4.2.0"
 
 [tool.poetry.group.dev.dependencies]
 channels = ">=3.0,<=4.0"
 coverage = "^6.2"
 django-dramatiq = "^0.10.0"
```

### Comparing `django_twined-0.4.2/PKG-INFO` & `django_twined-0.4.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 Metadata-Version: 2.1
 Name: django-twined
-Version: 0.4.2
+Version: 0.4.3
 Summary: A django app to manage octue services
 Home-page: https://github.com/octue/django-twined
 License: MIT
 Keywords: django,services,octue,twined
 Author: Tom Clark
 Author-email: tom@octue.com
 Requires-Python: >=3.9,<3.11
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: channels (>=3.0,<4.0)
 Requires-Dist: django (>=3.0,<4.0)
-Requires-Dist: django-gcp (>=0.7.3,<0.10)
+Requires-Dist: django-gcp (>=0.7.3,<0.11)
 Requires-Dist: django-jsoneditor (>=0.2.2,<0.3.0)
 Requires-Dist: django-model-utils (>=4.2.0,<5.0.0)
 Requires-Dist: octue (>=0.39.0,<0.40.0)
 Requires-Dist: pika (>=1.2.0,<2.0.0)
 Project-URL: Repository, https://github.com/octue/django-twined
 Description-Content-Type: text/markdown
```

