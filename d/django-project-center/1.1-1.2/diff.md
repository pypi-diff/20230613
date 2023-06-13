# Comparing `tmp/django-project-center-1.1.tar.gz` & `tmp/django-project-center-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-project-center-1.1.tar", last modified: Mon Jun 12 21:50:59 2023, max compression
+gzip compressed data, was "django-project-center-1.2.tar", last modified: Tue Jun 13 20:42:00 2023, max compression
```

## Comparing `django-project-center-1.1.tar` & `django-project-center-1.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 21:50:59.211738 django-project-center-1.1/
--rw-rw-rw-   0        0        0        0 2023-01-28 18:46:35.000000 django-project-center-1.1/LICENCE.txt
--rw-rw-rw-   0        0        0      365 2023-06-12 21:50:59.210736 django-project-center-1.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-01-28 18:46:11.000000 django-project-center-1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 21:50:59.058735 django-project-center-1.1/django_project_center.egg-info/
--rw-rw-rw-   0        0        0      365 2023-06-12 21:50:58.000000 django-project-center-1.1/django_project_center.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1626 2023-06-12 21:50:58.000000 django-project-center-1.1/django_project_center.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 21:50:58.000000 django-project-center-1.1/django_project_center.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-01-29 17:53:35.000000 django-project-center-1.1/django_project_center.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       15 2023-06-12 21:50:58.000000 django-project-center-1.1/django_project_center.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-12 21:50:59.096738 django-project-center-1.1/project_center/
--rw-rw-rw-   0        0        0        0 2023-01-28 18:09:02.000000 django-project-center-1.1/project_center/__init__.py
--rw-rw-rw-   0        0        0    13635 2023-06-04 13:58:55.000000 django-project-center-1.1/project_center/admin.py
--rw-rw-rw-   0        0        0      202 2023-03-06 13:02:17.000000 django-project-center-1.1/project_center/apps.py
-drwxrwxrwx   0        0        0        0 2023-06-12 21:50:59.098736 django-project-center-1.1/project_center/management/
--rw-rw-rw-   0        0        0        0 2022-12-23 17:39:29.000000 django-project-center-1.1/project_center/management/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 21:50:59.113736 django-project-center-1.1/project_center/management/commands/
--rw-rw-rw-   0        0        0        0 2022-12-23 17:39:49.000000 django-project-center-1.1/project_center/management/commands/__init__.py
--rw-rw-rw-   0        0        0     1507 2023-04-09 00:02:35.000000 django-project-center-1.1/project_center/management/commands/check_aws_access.py
--rw-rw-rw-   0        0        0     3694 2023-05-30 16:51:15.000000 django-project-center-1.1/project_center/management/commands/send_project_alert_email.py
-drwxrwxrwx   0        0        0        0 2023-06-12 21:50:59.199739 django-project-center-1.1/project_center/migrations/
--rw-rw-rw-   0        0        0    12997 2023-01-28 19:12:29.000000 django-project-center-1.1/project_center/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      405 2023-02-05 19:27:59.000000 django-project-center-1.1/project_center/migrations/0002_user_email_notify.py
--rw-rw-rw-   0        0        0      424 2023-02-15 11:57:39.000000 django-project-center-1.1/project_center/migrations/0003_projectactivity_notes.py
--rw-rw-rw-   0        0        0      424 2023-02-16 02:02:07.000000 django-project-center-1.1/project_center/migrations/0004_projectcategory_display.py
--rw-rw-rw-   0        0        0      424 2023-02-16 02:06:16.000000 django-project-center-1.1/project_center/migrations/0005_projectstatus_display.py
--rw-rw-rw-   0        0        0      421 2023-02-16 02:06:34.000000 django-project-center-1.1/project_center/migrations/0006_projectstage_display.py
--rw-rw-rw-   0        0        0      827 2023-03-03 02:55:14.000000 django-project-center-1.1/project_center/migrations/0007_alter_company_options_alter_user_options_and_more.py
--rw-rw-rw-   0        0        0     1744 2023-03-05 20:22:08.000000 django-project-center-1.1/project_center/migrations/0008_activity_projectactivity_reply_alter_project_users_and_more.py
--rw-rw-rw-   0        0        0      861 2023-03-05 20:29:12.000000 django-project-center-1.1/project_center/migrations/0009_projectactivity_reply_file_and_more.py
--rw-rw-rw-   0        0        0     1292 2023-06-04 12:06:52.000000 django-project-center-1.1/project_center/migrations/0010_delete_activity_project_last_activity_date_and_more.py
--rw-rw-rw-   0        0        0      560 2023-06-04 12:40:06.000000 django-project-center-1.1/project_center/migrations/0011_project_last_activity_name.py
--rw-rw-rw-   0        0        0      542 2023-06-05 17:25:02.000000 django-project-center-1.1/project_center/migrations/0012_alter_projectactivity_file.py
--rw-rw-rw-   0        0        0        0 2023-01-28 18:09:02.000000 django-project-center-1.1/project_center/migrations/__init__.py
--rw-rw-rw-   0        0        0    13276 2023-06-12 11:15:25.000000 django-project-center-1.1/project_center/models.py
-drwxrwxrwx   0        0        0        0 2023-06-12 21:50:59.207737 django-project-center-1.1/project_center/signals/
--rw-rw-rw-   0        0        0        0 2023-03-06 12:44:24.000000 django-project-center-1.1/project_center/signals/__init__.py
--rw-rw-rw-   0        0        0      367 2023-03-06 12:58:21.000000 django-project-center-1.1/project_center/signals/handlers.py
--rw-rw-rw-   0        0        0      188 2023-02-01 19:52:44.000000 django-project-center-1.1/project_center/storage_backends.py
-drwxrwxrwx   0        0        0        0 2023-06-12 21:50:59.208738 django-project-center-1.1/project_center/templates/
--rw-rw-rw-   0        0        0        0 2023-02-05 20:00:02.000000 django-project-center-1.1/project_center/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 21:50:59.209737 django-project-center-1.1/project_center/templates/email/
--rw-rw-rw-   0        0        0        0 2023-02-05 20:03:52.000000 django-project-center-1.1/project_center/templates/email/__init__.py
--rw-rw-rw-   0        0        0       63 2023-01-28 18:09:02.000000 django-project-center-1.1/project_center/tests.py
--rw-rw-rw-   0        0        0      193 2023-02-05 20:17:46.000000 django-project-center-1.1/project_center/utils.py
--rw-rw-rw-   0        0        0     1071 2023-03-05 17:48:01.000000 django-project-center-1.1/project_center/views.py
--rw-rw-rw-   0        0        0       42 2023-06-12 21:50:59.211738 django-project-center-1.1/setup.cfg
--rw-rw-rw-   0        0        0      784 2023-06-12 21:50:43.000000 django-project-center-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 20:42:00.726460 django-project-center-1.2/
+-rw-rw-rw-   0        0        0        0 2023-01-28 18:46:35.000000 django-project-center-1.2/LICENCE.txt
+-rw-rw-rw-   0        0        0      365 2023-06-13 20:42:00.725460 django-project-center-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-01-28 18:46:11.000000 django-project-center-1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 20:42:00.586459 django-project-center-1.2/django_project_center.egg-info/
+-rw-rw-rw-   0        0        0      365 2023-06-13 20:42:00.000000 django-project-center-1.2/django_project_center.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1626 2023-06-13 20:42:00.000000 django-project-center-1.2/django_project_center.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 20:42:00.000000 django-project-center-1.2/django_project_center.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-01-29 17:53:35.000000 django-project-center-1.2/django_project_center.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       15 2023-06-13 20:42:00.000000 django-project-center-1.2/django_project_center.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 20:42:00.617460 django-project-center-1.2/project_center/
+-rw-rw-rw-   0        0        0        0 2023-01-28 18:09:02.000000 django-project-center-1.2/project_center/__init__.py
+-rw-rw-rw-   0        0        0    14112 2023-06-13 20:37:14.000000 django-project-center-1.2/project_center/admin.py
+-rw-rw-rw-   0        0        0      202 2023-03-06 13:02:17.000000 django-project-center-1.2/project_center/apps.py
+drwxrwxrwx   0        0        0        0 2023-06-13 20:42:00.619460 django-project-center-1.2/project_center/management/
+-rw-rw-rw-   0        0        0        0 2022-12-23 17:39:29.000000 django-project-center-1.2/project_center/management/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 20:42:00.634460 django-project-center-1.2/project_center/management/commands/
+-rw-rw-rw-   0        0        0        0 2022-12-23 17:39:49.000000 django-project-center-1.2/project_center/management/commands/__init__.py
+-rw-rw-rw-   0        0        0     1507 2023-04-09 00:02:35.000000 django-project-center-1.2/project_center/management/commands/check_aws_access.py
+-rw-rw-rw-   0        0        0     3694 2023-05-30 16:51:15.000000 django-project-center-1.2/project_center/management/commands/send_project_alert_email.py
+drwxrwxrwx   0        0        0        0 2023-06-13 20:42:00.715461 django-project-center-1.2/project_center/migrations/
+-rw-rw-rw-   0        0        0    12997 2023-01-28 19:12:29.000000 django-project-center-1.2/project_center/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      405 2023-02-05 19:27:59.000000 django-project-center-1.2/project_center/migrations/0002_user_email_notify.py
+-rw-rw-rw-   0        0        0      424 2023-02-15 11:57:39.000000 django-project-center-1.2/project_center/migrations/0003_projectactivity_notes.py
+-rw-rw-rw-   0        0        0      424 2023-02-16 02:02:07.000000 django-project-center-1.2/project_center/migrations/0004_projectcategory_display.py
+-rw-rw-rw-   0        0        0      424 2023-02-16 02:06:16.000000 django-project-center-1.2/project_center/migrations/0005_projectstatus_display.py
+-rw-rw-rw-   0        0        0      421 2023-02-16 02:06:34.000000 django-project-center-1.2/project_center/migrations/0006_projectstage_display.py
+-rw-rw-rw-   0        0        0      827 2023-03-03 02:55:14.000000 django-project-center-1.2/project_center/migrations/0007_alter_company_options_alter_user_options_and_more.py
+-rw-rw-rw-   0        0        0     1744 2023-03-05 20:22:08.000000 django-project-center-1.2/project_center/migrations/0008_activity_projectactivity_reply_alter_project_users_and_more.py
+-rw-rw-rw-   0        0        0      861 2023-03-05 20:29:12.000000 django-project-center-1.2/project_center/migrations/0009_projectactivity_reply_file_and_more.py
+-rw-rw-rw-   0        0        0     1292 2023-06-04 12:06:52.000000 django-project-center-1.2/project_center/migrations/0010_delete_activity_project_last_activity_date_and_more.py
+-rw-rw-rw-   0        0        0      560 2023-06-04 12:40:06.000000 django-project-center-1.2/project_center/migrations/0011_project_last_activity_name.py
+-rw-rw-rw-   0        0        0      542 2023-06-05 17:25:02.000000 django-project-center-1.2/project_center/migrations/0012_alter_projectactivity_file.py
+-rw-rw-rw-   0        0        0        0 2023-01-28 18:09:02.000000 django-project-center-1.2/project_center/migrations/__init__.py
+-rw-rw-rw-   0        0        0    13606 2023-06-13 20:26:52.000000 django-project-center-1.2/project_center/models.py
+drwxrwxrwx   0        0        0        0 2023-06-13 20:42:00.722459 django-project-center-1.2/project_center/signals/
+-rw-rw-rw-   0        0        0        0 2023-03-06 12:44:24.000000 django-project-center-1.2/project_center/signals/__init__.py
+-rw-rw-rw-   0        0        0      367 2023-03-06 12:58:21.000000 django-project-center-1.2/project_center/signals/handlers.py
+-rw-rw-rw-   0        0        0      188 2023-02-01 19:52:44.000000 django-project-center-1.2/project_center/storage_backends.py
+drwxrwxrwx   0        0        0        0 2023-06-13 20:42:00.723459 django-project-center-1.2/project_center/templates/
+-rw-rw-rw-   0        0        0        0 2023-02-05 20:00:02.000000 django-project-center-1.2/project_center/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 20:42:00.724459 django-project-center-1.2/project_center/templates/email/
+-rw-rw-rw-   0        0        0        0 2023-02-05 20:03:52.000000 django-project-center-1.2/project_center/templates/email/__init__.py
+-rw-rw-rw-   0        0        0       63 2023-01-28 18:09:02.000000 django-project-center-1.2/project_center/tests.py
+-rw-rw-rw-   0        0        0      193 2023-02-05 20:17:46.000000 django-project-center-1.2/project_center/utils.py
+-rw-rw-rw-   0        0        0     1071 2023-03-05 17:48:01.000000 django-project-center-1.2/project_center/views.py
+-rw-rw-rw-   0        0        0       42 2023-06-13 20:42:00.726460 django-project-center-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      784 2023-06-13 20:41:50.000000 django-project-center-1.2/setup.py
```

### Comparing `django-project-center-1.1/django_project_center.egg-info/SOURCES.txt` & `django-project-center-1.2/django_project_center.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-project-center-1.1/project_center/admin.py` & `django-project-center-1.2/project_center/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,14 +135,29 @@
     def last_activity(self, obj):
         return obj.projectactivity_set.order_by('-date').first()
 
     def get_form(self, request, obj=None, **kwargs):
         self.instance = obj
         return super(ProjectAdmin, self).get_form(request, obj=obj, **kwargs)
 
+    def save_model(self, request, obj, form, change):
+
+        super().save_model(request, obj, form, change)
+        if not obj.last_activity():
+            activity = ProjectActivity.objects.create(
+                name='Project Created',
+                user=request.user,
+            project=obj,
+            date=timezone.now())
+
+            obj.last_activity_name = activity.name
+            obj.last_activity_date = activity.date
+            obj.save()
+
+
     def formfield_for_manytomany(self, db_field, request, **kwargs):
         """
         Restrict the list of authors to Super Users and Staff only.
         """
         if db_field.name == 'users':
             try:
                 if self.instance.company and request.user.is_superuser or request.user.groups.filter(name=settings.PROJECT_CENTER_ADMINISTRATOR_GROUP_NAME).exists():
```

### Comparing `django-project-center-1.1/project_center/management/commands/check_aws_access.py` & `django-project-center-1.2/project_center/management/commands/check_aws_access.py`

 * *Files identical despite different names*

### Comparing `django-project-center-1.1/project_center/management/commands/send_project_alert_email.py` & `django-project-center-1.2/project_center/management/commands/send_project_alert_email.py`

 * *Files identical despite different names*

### Comparing `django-project-center-1.1/project_center/migrations/0001_initial.py` & `django-project-center-1.2/project_center/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-project-center-1.1/project_center/migrations/0007_alter_company_options_alter_user_options_and_more.py` & `django-project-center-1.2/project_center/migrations/0007_alter_company_options_alter_user_options_and_more.py`

 * *Files identical despite different names*

### Comparing `django-project-center-1.1/project_center/migrations/0008_activity_projectactivity_reply_alter_project_users_and_more.py` & `django-project-center-1.2/project_center/migrations/0008_activity_projectactivity_reply_alter_project_users_and_more.py`

 * *Files identical despite different names*

### Comparing `django-project-center-1.1/project_center/migrations/0009_projectactivity_reply_file_and_more.py` & `django-project-center-1.2/project_center/migrations/0009_projectactivity_reply_file_and_more.py`

 * *Files identical despite different names*

### Comparing `django-project-center-1.1/project_center/migrations/0010_delete_activity_project_last_activity_date_and_more.py` & `django-project-center-1.2/project_center/migrations/0010_delete_activity_project_last_activity_date_and_more.py`

 * *Files identical despite different names*

### Comparing `django-project-center-1.1/project_center/migrations/0011_project_last_activity_name.py` & `django-project-center-1.2/project_center/migrations/0011_project_last_activity_name.py`

 * *Files identical despite different names*

### Comparing `django-project-center-1.1/project_center/migrations/0012_alter_projectactivity_file.py` & `django-project-center-1.2/project_center/migrations/0012_alter_projectactivity_file.py`

 * *Files identical despite different names*

### Comparing `django-project-center-1.1/project_center/models.py` & `django-project-center-1.2/project_center/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 from django.template.loader import render_to_string
 from django.urls import reverse
 from django.utils.safestring import mark_safe
 from django.utils.translation import gettext_lazy as _
 from django.core.mail import EmailMultiAlternatives
 from django.conf import settings
 from django.utils.timezone import datetime, make_aware, make_naive
+from django.db.models.signals import post_save
+from django.dispatch import receiver
 
 from phonenumber_field.modelfields import PhoneNumberField
 
 
 class State(models.Model):
     name = models.CharField(_('name'), max_length=100, blank=False)
     abbrev = models.CharField(_('abbrev'), max_length=2, blank=True)
@@ -255,14 +257,21 @@
 def activity_file_directory_path(instance, filename):
     # file will be uploaded to MEDIA_ROOT/user_<id>/<filename>
     try:
         return 'project_activity_files/{0}/{1}'.format(instance.project.slug, os.path.basename(filename))
     except:
         return None
 
+# @receiver(post_save, sender=Project)
+# def create_project(sender, instance, created, **kwargs):
+#     if created:
+#         ProjectActivity.objects.create(
+#             name='Project Created',
+#             user=instance.
+#         )
 
 class ProjectActivity(models.Model):
     import_id = models.IntegerField(_('Import ID'), blank=True, null=True, default=None, help_text='Import ID')
     name = models.CharField(_('Activity Name'), max_length=255, blank=False, help_text='Activity Name')
     user = models.ForeignKey(User, blank=True, null=True, default=None, on_delete=models.SET_NULL)
     project = models.ForeignKey(Project, blank=True, null=True, default=None, on_delete=models.CASCADE)
     date = models.DateTimeField(_('Activity Date'), blank=True, null=True, help_text='Activity Date')
```

### Comparing `django-project-center-1.1/project_center/views.py` & `django-project-center-1.2/project_center/views.py`

 * *Files identical despite different names*

### Comparing `django-project-center-1.1/setup.py` & `django-project-center-1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ]
 
 # https://pypi.python.org/pypi?%3Aaction=list_classifiers
 CLASSIFIERS = []
 
 setup(
     name='django-project-center',
-    version='1.1',
+    version='1.2',
     description='Project Management Module for Django',
     author='siteshell.net',
     author_email='pdbethke@siteshell.net',
     url='https://github.com/pdbethke/django-project-center',
     packages=find_packages(),
     license='LICENSE.txt',
     platforms=['OS Independent'],
```

