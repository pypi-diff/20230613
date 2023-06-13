# Comparing `tmp/nobinobi-core-0.1.4.6.tar.gz` & `tmp/nobinobi-core-0.1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\nobinobi-core-0.1.4.6.tar", last modified: Thu Sep 16 13:45:58 2021, max compression
+gzip compressed data, was "nobinobi-core-0.1.4.7.tar", last modified: Tue Jun 13 10:54:12 2023, max compression
```

## Comparing `nobinobi-core-0.1.4.6.tar` & `nobinobi-core-0.1.4.7.tar`

### file list

```diff
@@ -1,81 +1,84 @@
-drwxrwxrwx   0        0        0        0 2021-09-16 13:45:58.000000 nobinobi-core-0.1.4.6/
--rw-rw-rw-   0        0        0      153 2020-10-06 09:14:17.000000 nobinobi-core-0.1.4.6/AUTHORS.rst
--rw-rw-rw-   0        0        0     3363 2020-10-06 13:39:46.000000 nobinobi-core-0.1.4.6/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     1268 2021-09-16 13:44:54.000000 nobinobi-core-0.1.4.6/HISTORY.rst
--rw-rw-rw-   0        0        0    31774 2020-10-06 09:20:38.000000 nobinobi-core-0.1.4.6/LICENSE
--rw-rw-rw-   0        0        0      247 2020-10-12 10:19:54.000000 nobinobi-core-0.1.4.6/MANIFEST.in
--rw-rw-rw-   0        0        0     5307 2021-09-16 13:45:58.000000 nobinobi-core-0.1.4.6/PKG-INFO
--rw-rw-rw-   0        0        0     2032 2020-10-06 13:39:46.000000 nobinobi-core-0.1.4.6/README.rst
-drwxrwxrwx   0        0        0        0 2021-09-16 13:45:58.000000 nobinobi-core-0.1.4.6/nobinobi_core/
--rw-rw-rw-   0        0        0      819 2021-09-16 13:44:54.000000 nobinobi-core-0.1.4.6/nobinobi_core/__init__.py
--rw-rw-rw-   0        0        0     4699 2020-10-12 09:49:15.000000 nobinobi-core-0.1.4.6/nobinobi_core/admin.py
--rw-rw-rw-   0        0        0     1100 2021-07-20 10:03:07.000000 nobinobi-core-0.1.4.6/nobinobi_core/apps.py
--rw-rw-rw-   0        0        0     1771 2021-09-16 12:50:17.000000 nobinobi-core-0.1.4.6/nobinobi_core/forms.py
--rw-rw-rw-   0        0        0    13512 2021-09-16 12:50:17.000000 nobinobi-core-0.1.4.6/nobinobi_core/functions.py
-drwxrwxrwx   0        0        0        0 2021-09-16 13:45:58.000000 nobinobi-core-0.1.4.6/nobinobi_core/locale/
-drwxrwxrwx   0        0        0        0 2021-09-16 13:45:58.000000 nobinobi-core-0.1.4.6/nobinobi_core/locale/en/
-drwxrwxrwx   0        0        0        0 2021-09-16 13:45:58.000000 nobinobi-core-0.1.4.6/nobinobi_core/locale/en/LC_MESSAGES/
--rw-rw-rw-   0        0        0      421 2020-09-01 10:42:31.000000 nobinobi-core-0.1.4.6/nobinobi_core/locale/en/LC_MESSAGES/django.mo
-drwxrwxrwx   0        0        0        0 2021-09-16 13:45:58.000000 nobinobi-core-0.1.4.6/nobinobi_core/locale/fr/
-drwxrwxrwx   0        0        0        0 2021-09-16 13:45:58.000000 nobinobi-core-0.1.4.6/nobinobi_core/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0        0        0     2138 2021-09-16 12:50:17.000000 nobinobi-core-0.1.4.6/nobinobi_core/locale/fr/LC_MESSAGES/django.mo
-drwxrwxrwx   0        0        0        0 2021-09-16 13:45:58.000000 nobinobi-core-0.1.4.6/nobinobi_core/migrations/
--rw-rw-rw-   0        0        0     2001 2020-10-06 13:39:46.000000 nobinobi-core-0.1.4.6/nobinobi_core/migrations/0001_initial.py
--rw-rw-rw-   0        0        0     2473 2020-10-08 13:04:26.000000 nobinobi-core-0.1.4.6/nobinobi_core/migrations/0002_organisation_organisationclosure.py
--rw-rw-rw-   0        0        0      442 2021-09-16 12:50:17.000000 nobinobi-core-0.1.4.6/nobinobi_core/migrations/0003_alter_holiday_date.py
--rw-rw-rw-   0        0        0     1231 2020-10-06 13:39:46.000000 nobinobi-core-0.1.4.6/nobinobi_core/migrations/__init__.py
--rw-rw-rw-   0        0        0     2719 2021-09-16 12:50:17.000000 nobinobi-core-0.1.4.6/nobinobi_core/models.py
-drwxrwxrwx   0        0        0        0 2021-09-16 13:45:58.000000 nobinobi-core-0.1.4.6/nobinobi_core/static/
-drwxrwxrwx   0        0        0        0 2021-09-16 13:45:58.000000 nobinobi-core-0.1.4.6/nobinobi_core/static/css/
--rw-rw-rw-   0        0        0     3108 2020-09-01 10:42:31.000000 nobinobi-core-0.1.4.6/nobinobi_core/static/css/bootstrap-datetimepicker-standalone.css
--rw-rw-rw-   0        0        0     9827 2020-09-01 10:42:31.000000 nobinobi-core-0.1.4.6/nobinobi_core/static/css/bootstrap-datetimepicker.css
--rw-rw-rw-   0        0        0     7785 2020-09-01 10:42:31.000000 nobinobi-core-0.1.4.6/nobinobi_core/static/css/bootstrap-datetimepicker.min.css
--rw-rw-rw-   0        0        0      805 2020-10-06 13:39:46.000000 nobinobi-core-0.1.4.6/nobinobi_core/static/css/nobinobi_core.css
-drwxrwxrwx   0        0        0        0 2021-09-16 13:45:58.000000 nobinobi-core-0.1.4.6/nobinobi_core/static/js/
--rw-rw-rw-   0        0        0    38510 2020-09-01 10:42:32.000000 nobinobi-core-0.1.4.6/nobinobi_core/static/js/bootstrap-datetimepicker.min.js
--rw-rw-rw-   0        0        0   336451 2020-09-01 10:42:32.000000 nobinobi-core-0.1.4.6/nobinobi_core/static/js/moment-with-locales.min.js
--rw-rw-rw-   0        0        0      805 2020-10-06 13:39:46.000000 nobinobi-core-0.1.4.6/nobinobi_core/static/js/nobinobi_core.js
-drwxrwxrwx   0        0        0        0 2021-09-16 13:45:58.000000 nobinobi-core-0.1.4.6/nobinobi_core/templates/
-drwxrwxrwx   0        0        0        0 2021-09-16 13:45:58.000000 nobinobi-core-0.1.4.6/nobinobi_core/templates/includes/
--rw-rw-rw-   0        0        0      504 2020-09-01 10:42:32.000000 nobinobi-core-0.1.4.6/nobinobi_core/templates/includes/messages.html
-drwxrwxrwx   0        0        0        0 2021-09-16 13:45:58.000000 nobinobi-core-0.1.4.6/nobinobi_core/templates/layout/
--rw-rw-rw-   0        0        0     2200 2020-09-01 10:42:32.000000 nobinobi-core-0.1.4.6/nobinobi_core/templates/layout/checkboxselectmultiple_act.html
--rw-rw-rw-   0        0        0     2204 2020-09-01 10:42:32.000000 nobinobi-core-0.1.4.6/nobinobi_core/templates/layout/checkboxselectmultiple_image.html
--rw-rw-rw-   0        0        0     1594 2020-09-01 10:42:32.000000 nobinobi-core-0.1.4.6/nobinobi_core/templates/layout/checkboxselectmultiple_inline.html
--rw-rw-rw-   0        0        0     1587 2020-09-01 10:42:32.000000 nobinobi-core-0.1.4.6/nobinobi_core/templates/layout/checkboxselectmultiple_inline_act.html
--rw-rw-rw-   0        0        0     1589 2020-09-01 10:42:32.000000 nobinobi-core-0.1.4.6/nobinobi_core/templates/layout/checkboxselectmultiple_inline_image.html
--rw-rw-rw-   0        0        0     1163 2020-09-01 10:42:32.000000 nobinobi-core-0.1.4.6/nobinobi_core/templates/layout/field_errors_block.html
--rw-rw-rw-   0        0        0     1225 2020-09-01 10:42:32.000000 nobinobi-core-0.1.4.6/nobinobi_core/templates/layout/help_text.html
--rw-rw-rw-   0        0        0     1782 2020-09-01 10:42:32.000000 nobinobi-core-0.1.4.6/nobinobi_core/templates/layout/radioselect.html
--rw-rw-rw-   0        0        0     2031 2020-09-01 10:42:32.000000 nobinobi-core-0.1.4.6/nobinobi_core/templates/layout/radioselect_image.html
--rw-rw-rw-   0        0        0     1625 2020-09-01 10:42:32.000000 nobinobi-core-0.1.4.6/nobinobi_core/templates/layout/radioselect_inline.html
--rw-rw-rw-   0        0        0     1631 2020-09-01 10:42:32.000000 nobinobi-core-0.1.4.6/nobinobi_core/templates/layout/radioselect_inline_image.html
-drwxrwxrwx   0        0        0        0 2021-09-16 13:45:58.000000 nobinobi-core-0.1.4.6/nobinobi_core/templates/layout/sj/
--rw-rw-rw-   0        0        0     1325 2020-09-01 10:42:32.000000 nobinobi-core-0.1.4.6/nobinobi_core/templates/layout/sj/collation_general.html
-drwxrwxrwx   0        0        0        0 2021-09-16 13:45:58.000000 nobinobi-core-0.1.4.6/nobinobi_core/templates/nobinobi_core/
--rw-rw-rw-   0        0        0      573 2021-09-16 12:50:17.000000 nobinobi-core-0.1.4.6/nobinobi_core/templates/nobinobi_core/add_official_holiday.html
--rw-rw-rw-   0        0        0      682 2020-10-06 13:39:46.000000 nobinobi-core-0.1.4.6/nobinobi_core/templates/nobinobi_core/base.html
-drwxrwxrwx   0        0        0        0 2021-09-16 13:45:58.000000 nobinobi-core-0.1.4.6/nobinobi_core/templatetags/
--rw-rw-rw-   0        0        0     1231 2020-10-06 13:39:46.000000 nobinobi-core-0.1.4.6/nobinobi_core/templatetags/__init__.py
--rw-rw-rw-   0        0        0     1779 2020-10-06 09:24:22.000000 nobinobi-core-0.1.4.6/nobinobi_core/templatetags/get_dict_value.py
--rw-rw-rw-   0        0        0      966 2020-10-06 09:24:24.000000 nobinobi-core-0.1.4.6/nobinobi_core/templatetags/get_user_method.py
--rw-rw-rw-   0        0        0     1634 2020-10-06 09:24:33.000000 nobinobi-core-0.1.4.6/nobinobi_core/templatetags/math.py
--rw-rw-rw-   0        0        0     3407 2020-10-06 09:24:36.000000 nobinobi-core-0.1.4.6/nobinobi_core/templatetags/notifications_tags_custom.py
--rw-rw-rw-   0        0        0      962 2020-10-06 09:24:38.000000 nobinobi-core-0.1.4.6/nobinobi_core/templatetags/remove_date_sem.py
--rw-rw-rw-   0        0        0     1056 2020-10-06 13:39:46.000000 nobinobi-core-0.1.4.6/nobinobi_core/templatetags/remove_tags_html.py
--rw-rw-rw-   0        0        0     1244 2020-10-06 09:24:44.000000 nobinobi-core-0.1.4.6/nobinobi_core/templatetags/startwith.py
--rw-rw-rw-   0        0        0     1127 2021-07-20 09:20:02.000000 nobinobi-core-0.1.4.6/nobinobi_core/urls.py
--rw-rw-rw-   0        0        0     3113 2021-09-16 13:44:54.000000 nobinobi-core-0.1.4.6/nobinobi_core/views.py
--rw-rw-rw-   0        0        0    23107 2020-10-06 13:39:46.000000 nobinobi-core-0.1.4.6/nobinobi_core/widgets.py
-drwxrwxrwx   0        0        0        0 2021-09-16 13:45:58.000000 nobinobi-core-0.1.4.6/nobinobi_core.egg-info/
--rw-rw-rw-   0        0        0     5307 2021-09-16 13:45:57.000000 nobinobi-core-0.1.4.6/nobinobi_core.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2466 2021-09-16 13:45:58.000000 nobinobi-core-0.1.4.6/nobinobi_core.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-09-16 13:45:57.000000 nobinobi-core-0.1.4.6/nobinobi_core.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-09-16 13:45:57.000000 nobinobi-core-0.1.4.6/nobinobi_core.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      146 2021-09-16 13:45:57.000000 nobinobi-core-0.1.4.6/nobinobi_core.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2021-09-16 13:45:57.000000 nobinobi-core-0.1.4.6/nobinobi_core.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      222 2021-09-14 13:49:38.000000 nobinobi-core-0.1.4.6/requirements.txt
--rw-rw-rw-   0        0        0       69 2021-09-14 13:49:38.000000 nobinobi-core-0.1.4.6/requirements_dev.txt
--rw-rw-rw-   0        0        0      117 2021-09-14 13:49:38.000000 nobinobi-core-0.1.4.6/requirements_test.txt
--rw-rw-rw-   0        0        0      427 2021-09-16 13:45:58.000000 nobinobi-core-0.1.4.6/setup.cfg
--rw-rw-rw-   0        0        0     2303 2020-10-06 13:39:46.000000 nobinobi-core-0.1.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 10:54:12.981832 nobinobi-core-0.1.4.7/
+-rw-rw-rw-   0        0        0      166 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3363 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     1389 2023-06-12 09:30:30.000000 nobinobi-core-0.1.4.7/HISTORY.rst
+-rw-rw-rw-   0        0        0    31960 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/LICENSE
+-rw-rw-rw-   0        0        0      247 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     4132 2023-06-13 10:54:12.982832 nobinobi-core-0.1.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2032 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-13 10:54:12.765581 nobinobi-core-0.1.4.7/nobinobi_core/
+-rw-rw-rw-   0        0        0      819 2023-06-12 09:30:30.000000 nobinobi-core-0.1.4.7/nobinobi_core/__init__.py
+-rw-rw-rw-   0        0        0     4699 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/admin.py
+-rw-rw-rw-   0        0        0     1100 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/apps.py
+-rw-rw-rw-   0        0        0     1775 2023-06-12 09:19:34.000000 nobinobi-core-0.1.4.7/nobinobi_core/forms.py
+-rw-rw-rw-   0        0        0    13512 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/functions.py
+drwxrwxrwx   0        0        0        0 2023-06-13 10:54:12.648265 nobinobi-core-0.1.4.7/nobinobi_core/locale/
+drwxrwxrwx   0        0        0        0 2023-06-13 10:54:12.647757 nobinobi-core-0.1.4.7/nobinobi_core/locale/en/
+drwxrwxrwx   0        0        0        0 2023-06-13 10:54:12.823835 nobinobi-core-0.1.4.7/nobinobi_core/locale/en/LC_MESSAGES/
+-rw-rw-rw-   0        0        0      421 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/locale/en/LC_MESSAGES/django.mo
+drwxrwxrwx   0        0        0        0 2023-06-13 10:54:12.648265 nobinobi-core-0.1.4.7/nobinobi_core/locale/fr/
+drwxrwxrwx   0        0        0        0 2023-06-13 10:54:12.824834 nobinobi-core-0.1.4.7/nobinobi_core/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     2138 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/locale/fr/LC_MESSAGES/django.mo
+drwxrwxrwx   0        0        0        0 2023-06-13 10:54:12.828214 nobinobi-core-0.1.4.7/nobinobi_core/migrations/
+-rw-rw-rw-   0        0        0     2001 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0     2473 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/migrations/0002_organisation_organisationclosure.py
+-rw-rw-rw-   0        0        0      442 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/migrations/0003_alter_holiday_date.py
+-rw-rw-rw-   0        0        0     1231 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/migrations/__init__.py
+-rw-rw-rw-   0        0        0     2719 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/models.py
+drwxrwxrwx   0        0        0        0 2023-06-13 10:54:12.661849 nobinobi-core-0.1.4.7/nobinobi_core/static/
+drwxrwxrwx   0        0        0        0 2023-06-13 10:54:12.855718 nobinobi-core-0.1.4.7/nobinobi_core/static/css/
+-rw-rw-rw-   0        0        0     3222 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/static/css/bootstrap-datetimepicker-standalone.css
+-rw-rw-rw-   0        0        0    10217 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/static/css/bootstrap-datetimepicker.css
+-rw-rw-rw-   0        0        0     7789 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/static/css/bootstrap-datetimepicker.min.css
+-rw-rw-rw-   0        0        0      805 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/static/css/nobinobi_core.css
+drwxrwxrwx   0        0        0        0 2023-06-13 10:54:12.952538 nobinobi-core-0.1.4.7/nobinobi_core/static/js/
+-rw-rw-rw-   0        0        0    38511 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/static/js/bootstrap-datetimepicker.min.js
+-rw-rw-rw-   0        0        0   336451 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/static/js/moment-with-locales.min.js
+-rw-rw-rw-   0        0        0      805 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/static/js/nobinobi_core.js
+drwxrwxrwx   0        0        0        0 2023-06-13 10:54:12.663863 nobinobi-core-0.1.4.7/nobinobi_core/templates/
+drwxrwxrwx   0        0        0        0 2023-06-13 10:54:12.956537 nobinobi-core-0.1.4.7/nobinobi_core/templates/includes/
+-rw-rw-rw-   0        0        0      521 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/templates/includes/messages.html
+drwxrwxrwx   0        0        0        0 2023-06-13 10:54:12.968024 nobinobi-core-0.1.4.7/nobinobi_core/templates/layout/
+-rw-rw-rw-   0        0        0     2248 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/templates/layout/checkboxselectmultiple_act.html
+-rw-rw-rw-   0        0        0     2251 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/templates/layout/checkboxselectmultiple_image.html
+-rw-rw-rw-   0        0        0     1627 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/templates/layout/checkboxselectmultiple_inline.html
+-rw-rw-rw-   0        0        0     1620 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/templates/layout/checkboxselectmultiple_inline_act.html
+-rw-rw-rw-   0        0        0     1622 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/templates/layout/checkboxselectmultiple_inline_image.html
+-rw-rw-rw-   0        0        0     1187 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/templates/layout/field_errors_block.html
+-rw-rw-rw-   0        0        0     1251 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/templates/layout/help_text.html
+-rw-rw-rw-   0        0        0     1817 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/templates/layout/radioselect.html
+-rw-rw-rw-   0        0        0     2076 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/templates/layout/radioselect_image.html
+-rw-rw-rw-   0        0        0     1658 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/templates/layout/radioselect_inline.html
+-rw-rw-rw-   0        0        0     1664 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/templates/layout/radioselect_inline_image.html
+drwxrwxrwx   0        0        0        0 2023-06-13 10:54:12.969054 nobinobi-core-0.1.4.7/nobinobi_core/templates/layout/sj/
+-rw-rw-rw-   0        0        0     1354 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/templates/layout/sj/collation_general.html
+drwxrwxrwx   0        0        0        0 2023-06-13 10:54:12.971003 nobinobi-core-0.1.4.7/nobinobi_core/templates/nobinobi_core/
+-rw-rw-rw-   0        0        0      520 2023-06-12 09:16:28.000000 nobinobi-core-0.1.4.7/nobinobi_core/templates/nobinobi_core/add_official_holiday.html
+-rw-rw-rw-   0        0        0      682 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/templates/nobinobi_core/base.html
+drwxrwxrwx   0        0        0        0 2023-06-13 10:54:12.979315 nobinobi-core-0.1.4.7/nobinobi_core/templatetags/
+-rw-rw-rw-   0        0        0     1231 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/templatetags/__init__.py
+-rw-rw-rw-   0        0        0     1837 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/templatetags/get_dict_value.py
+-rw-rw-rw-   0        0        0      989 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/templatetags/get_user_method.py
+-rw-rw-rw-   0        0        0     1685 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/templatetags/math.py
+-rw-rw-rw-   0        0        0     3512 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/templatetags/notifications_tags_custom.py
+-rw-rw-rw-   0        0        0      989 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/templatetags/remove_date_sem.py
+-rw-rw-rw-   0        0        0     1056 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/templatetags/remove_tags_html.py
+-rw-rw-rw-   0        0        0     1276 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/templatetags/startwith.py
+-rw-rw-rw-   0        0        0     1153 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/urls.py
+-rw-rw-rw-   0        0        0     3113 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/views.py
+-rw-rw-rw-   0        0        0    23107 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/nobinobi_core/widgets.py
+drwxrwxrwx   0        0        0        0 2023-06-13 10:54:12.822835 nobinobi-core-0.1.4.7/nobinobi_core.egg-info/
+-rw-rw-rw-   0        0        0     4132 2023-06-13 10:54:12.000000 nobinobi-core-0.1.4.7/nobinobi_core.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2507 2023-06-13 10:54:12.000000 nobinobi-core-0.1.4.7/nobinobi_core.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 10:54:12.000000 nobinobi-core-0.1.4.7/nobinobi_core.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-13 10:54:12.000000 nobinobi-core-0.1.4.7/nobinobi_core.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      102 2023-06-13 10:54:12.000000 nobinobi-core-0.1.4.7/nobinobi_core.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-13 10:54:12.000000 nobinobi-core-0.1.4.7/nobinobi_core.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      102 2023-06-13 10:53:58.000000 nobinobi-core-0.1.4.7/requirements.txt
+-rw-rw-rw-   0        0        0       63 2023-06-09 08:47:26.000000 nobinobi-core-0.1.4.7/requirements_dev.txt
+-rw-rw-rw-   0        0        0      119 2023-06-13 10:48:31.000000 nobinobi-core-0.1.4.7/requirements_test.txt
+-rw-rw-rw-   0        0        0      427 2023-06-13 10:54:12.983831 nobinobi-core-0.1.4.7/setup.cfg
+-rw-rw-rw-   0        0        0     2303 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 10:54:12.981832 nobinobi-core-0.1.4.7/tests/
+-rw-rw-rw-   0        0        0     2695 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/tests/test_admin.py
+-rw-rw-rw-   0        0        0     1399 2023-06-09 07:41:25.000000 nobinobi-core-0.1.4.7/tests/test_models.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `nobinobi-core-0.1.4.6/CONTRIBUTING.rst` & `nobinobi-core-0.1.4.7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.6/HISTORY.rst` & `nobinobi-core-0.1.4.7/HISTORY.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 .. :changelog:
 
 History
 -------
 
+0.1.4.7 (2023-06-12)
+++++++++++++++++++++++
+
+* 5c74e84 - Update for new cripsy form version
+* Update requirements
+
 0.1.4.6 (2021-09-16)
 ++++++++++++++++++++++
 
 * 5c6aace - Fix bug when add holiday but not same name but exist
 
 0.1.4.5 (2021-09-16)
 ++++++++++++++++++++++
```

### Comparing `nobinobi-core-0.1.4.6/LICENSE` & `nobinobi-core-0.1.4.7/LICENSE`

 * *Ordering differences only*

 * *Files 3% similar despite different names*

```diff
@@ -1,186 +1,186 @@
-GNU AFFERO GENERAL PUBLIC LICENSE
-
-Version 3, 19 November 2007
-
-Copyright © 2007 Free Software Foundation, Inc. <https://fsf.org/>
-Everyone is permitted to copy and distribute verbatim copies of this license document, but changing it is not allowed.
-Preamble
-
-The GNU Affero General Public License is a free, copyleft license for software and other kinds of works, specifically designed to ensure cooperation with the community in the case of network server software.
-
-The licenses for most software and other practical works are designed to take away your freedom to share and change the works. By contrast, our General Public Licenses are intended to guarantee your freedom to share and change all versions of a program--to make sure it remains free software for all its users.
-
-When we speak of free software, we are referring to freedom, not price. Our General Public Licenses are designed to make sure that you have the freedom to distribute copies of free software (and charge for them if you wish), that you receive source code or can get it if you want it, that you can change the software or use pieces of it in new free programs, and that you know you can do these things.
-
-Developers that use our General Public Licenses protect your rights with two steps: (1) assert copyright on the software, and (2) offer you this License which gives you legal permission to copy, distribute and/or modify the software.
-
-A secondary benefit of defending all users' freedom is that improvements made in alternate versions of the program, if they receive widespread use, become available for other developers to incorporate. Many developers of free software are heartened and encouraged by the resulting cooperation. However, in the case of software used on network servers, this result may fail to come about. The GNU General Public License permits making a modified version and letting the public access it on a server without ever releasing its source code to the public.
-
-The GNU Affero General Public License is designed specifically to ensure that, in such cases, the modified source code becomes available to the community. It requires the operator of a network server to provide the source code of the modified version running there to the users of that server. Therefore, public use of a modified version, on a publicly accessible server, gives the public access to the source code of the modified version.
-
-An older license, called the Affero General Public License and published by Affero, was designed to accomplish similar goals. This is a different license, not a version of the Affero GPL, but Affero has released a new version of the Affero GPL which permits relicensing under this license.
-
-The precise terms and conditions for copying, distribution and modification follow.
-TERMS AND CONDITIONS
-0. Definitions.
-
-"This License" refers to version 3 of the GNU Affero General Public License.
-
-"Copyright" also means copyright-like laws that apply to other kinds of works, such as semiconductor masks.
-
-"The Program" refers to any copyrightable work licensed under this License. Each licensee is addressed as "you". "Licensees" and "recipients" may be individuals or organizations.
-
-To "modify" a work means to copy from or adapt all or part of the work in a fashion requiring copyright permission, other than the making of an exact copy. The resulting work is called a "modified version" of the earlier work or a work "based on" the earlier work.
-
-A "covered work" means either the unmodified Program or a work based on the Program.
-
-To "propagate" a work means to do anything with it that, without permission, would make you directly or secondarily liable for infringement under applicable copyright law, except executing it on a computer or modifying a private copy. Propagation includes copying, distribution (with or without modification), making available to the public, and in some countries other activities as well.
-
-To "convey" a work means any kind of propagation that enables other parties to make or receive copies. Mere interaction with a user through a computer network, with no transfer of a copy, is not conveying.
-
-An interactive user interface displays "Appropriate Legal Notices" to the extent that it includes a convenient and prominently visible feature that (1) displays an appropriate copyright notice, and (2) tells the user that there is no warranty for the work (except to the extent that warranties are provided), that licensees may convey the work under this License, and how to view a copy of this License. If the interface presents a list of user commands or options, such as a menu, a prominent item in the list meets this criterion.
-1. Source Code.
-
-The "source code" for a work means the preferred form of the work for making modifications to it. "Object code" means any non-source form of a work.
-
-A "Standard Interface" means an interface that either is an official standard defined by a recognized standards body, or, in the case of interfaces specified for a particular programming language, one that is widely used among developers working in that language.
-
-The "System Libraries" of an executable work include anything, other than the work as a whole, that (a) is included in the normal form of packaging a Major Component, but which is not part of that Major Component, and (b) serves only to enable use of the work with that Major Component, or to implement a Standard Interface for which an implementation is available to the public in source code form. A "Major Component", in this context, means a major essential component (kernel, window system, and so on) of the specific operating system (if any) on which the executable work runs, or a compiler used to produce the work, or an object code interpreter used to run it.
-
-The "Corresponding Source" for a work in object code form means all the source code needed to generate, install, and (for an executable work) run the object code and to modify the work, including scripts to control those activities. However, it does not include the work's System Libraries, or general-purpose tools or generally available free programs which are used unmodified in performing those activities but which are not part of the work. For example, Corresponding Source includes interface definition files associated with source files for the work, and the source code for shared libraries and dynamically linked subprograms that the work is specifically designed to require, such as by intimate data communication or control flow between those subprograms and other parts of the work.
-
-The Corresponding Source need not include anything that users can regenerate automatically from other parts of the Corresponding Source.
-
-The Corresponding Source for a work in source code form is that same work.
-2. Basic Permissions.
-
-All rights granted under this License are granted for the term of copyright on the Program, and are irrevocable provided the stated conditions are met. This License explicitly affirms your unlimited permission to run the unmodified Program. The output from running a covered work is covered by this License only if the output, given its content, constitutes a covered work. This License acknowledges your rights of fair use or other equivalent, as provided by copyright law.
-
-You may make, run and propagate covered works that you do not convey, without conditions so long as your license otherwise remains in force. You may convey covered works to others for the sole purpose of having them make modifications exclusively for you, or provide you with facilities for running those works, provided that you comply with the terms of this License in conveying all material for which you do not control copyright. Those thus making or running the covered works for you must do so exclusively on your behalf, under your direction and control, on terms that prohibit them from making any copies of your copyrighted material outside their relationship with you.
-
-Conveying under any other circumstances is permitted solely under the conditions stated below. Sublicensing is not allowed; section 10 makes it unnecessary.
-3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-No covered work shall be deemed part of an effective technological measure under any applicable law fulfilling obligations under article 11 of the WIPO copyright treaty adopted on 20 December 1996, or similar laws prohibiting or restricting circumvention of such measures.
-
-When you convey a covered work, you waive any legal power to forbid circumvention of technological measures to the extent such circumvention is effected by exercising rights under this License with respect to the covered work, and you disclaim any intention to limit operation or modification of the work as a means of enforcing, against the work's users, your or third parties' legal rights to forbid circumvention of technological measures.
-4. Conveying Verbatim Copies.
-
-You may convey verbatim copies of the Program's source code as you receive it, in any medium, provided that you conspicuously and appropriately publish on each copy an appropriate copyright notice; keep intact all notices stating that this License and any non-permissive terms added in accord with section 7 apply to the code; keep intact all notices of the absence of any warranty; and give all recipients a copy of this License along with the Program.
-
-You may charge any price or no price for each copy that you convey, and you may offer support or warranty protection for a fee.
-5. Conveying Modified Source Versions.
-
-You may convey a work based on the Program, or the modifications to produce it from the Program, in the form of source code under the terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified it, and giving a relevant date.
-    b) The work must carry prominent notices stating that it is released under this License and any conditions added under section 7. This requirement modifies the requirement in section 4 to "keep intact all notices".
-    c) You must license the entire work, as a whole, under this License to anyone who comes into possession of a copy. This License will therefore apply, along with any applicable section 7 additional terms, to the whole of the work, and all its parts, regardless of how they are packaged. This License gives no permission to license the work in any other way, but it does not invalidate such permission if you have separately received it.
-    d) If the work has interactive user interfaces, each must display Appropriate Legal Notices; however, if the Program has interactive interfaces that do not display Appropriate Legal Notices, your work need not make them do so.
-
-A compilation of a covered work with other separate and independent works, which are not by their nature extensions of the covered work, and which are not combined with it such as to form a larger program, in or on a volume of a storage or distribution medium, is called an "aggregate" if the compilation and its resulting copyright are not used to limit the access or legal rights of the compilation's users beyond what the individual works permit. Inclusion of a covered work in an aggregate does not cause this License to apply to the other parts of the aggregate.
-6. Conveying Non-Source Forms.
-
-You may convey a covered work in object code form under the terms of sections 4 and 5, provided that you also convey the machine-readable Corresponding Source under the terms of this License, in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product (including a physical distribution medium), accompanied by the Corresponding Source fixed on a durable physical medium customarily used for software interchange.
-    b) Convey the object code in, or embodied in, a physical product (including a physical distribution medium), accompanied by a written offer, valid for at least three years and valid for as long as you offer spare parts or customer support for that product model, to give anyone who possesses the object code either (1) a copy of the Corresponding Source for all the software in the product that is covered by this License, on a durable physical medium customarily used for software interchange, for a price no more than your reasonable cost of physically performing this conveying of source, or (2) access to copy the Corresponding Source from a network server at no charge.
-    c) Convey individual copies of the object code with a copy of the written offer to provide the Corresponding Source. This alternative is allowed only occasionally and noncommercially, and only if you received the object code with such an offer, in accord with subsection 6b.
-    d) Convey the object code by offering access from a designated place (gratis or for a charge), and offer equivalent access to the Corresponding Source in the same way through the same place at no further charge. You need not require recipients to copy the Corresponding Source along with the object code. If the place to copy the object code is a network server, the Corresponding Source may be on a different server (operated by you or a third party) that supports equivalent copying facilities, provided you maintain clear directions next to the object code saying where to find the Corresponding Source. Regardless of what server hosts the Corresponding Source, you remain obligated to ensure that it is available for as long as needed to satisfy these requirements.
-    e) Convey the object code using peer-to-peer transmission, provided you inform other peers where the object code and Corresponding Source of the work are being offered to the general public at no charge under subsection 6d.
-
-A separable portion of the object code, whose source code is excluded from the Corresponding Source as a System Library, need not be included in conveying the object code work.
-
-A "User Product" is either (1) a "consumer product", which means any tangible personal property which is normally used for personal, family, or household purposes, or (2) anything designed or sold for incorporation into a dwelling. In determining whether a product is a consumer product, doubtful cases shall be resolved in favor of coverage. For a particular product received by a particular user, "normally used" refers to a typical or common use of that class of product, regardless of the status of the particular user or of the way in which the particular user actually uses, or expects or is expected to use, the product. A product is a consumer product regardless of whether the product has substantial commercial, industrial or non-consumer uses, unless such uses represent the only significant mode of use of the product.
-
-"Installation Information" for a User Product means any methods, procedures, authorization keys, or other information required to install and execute modified versions of a covered work in that User Product from a modified version of its Corresponding Source. The information must suffice to ensure that the continued functioning of the modified object code is in no case prevented or interfered with solely because modification has been made.
-
-If you convey an object code work under this section in, or with, or specifically for use in, a User Product, and the conveying occurs as part of a transaction in which the right of possession and use of the User Product is transferred to the recipient in perpetuity or for a fixed term (regardless of how the transaction is characterized), the Corresponding Source conveyed under this section must be accompanied by the Installation Information. But this requirement does not apply if neither you nor any third party retains the ability to install modified object code on the User Product (for example, the work has been installed in ROM).
-
-The requirement to provide Installation Information does not include a requirement to continue to provide support service, warranty, or updates for a work that has been modified or installed by the recipient, or for the User Product in which it has been modified or installed. Access to a network may be denied when the modification itself materially and adversely affects the operation of the network or violates the rules and protocols for communication across the network.
-
-Corresponding Source conveyed, and Installation Information provided, in accord with this section must be in a format that is publicly documented (and with an implementation available to the public in source code form), and must require no special password or key for unpacking, reading or copying.
-7. Additional Terms.
-
-"Additional permissions" are terms that supplement the terms of this License by making exceptions from one or more of its conditions. Additional permissions that are applicable to the entire Program shall be treated as though they were included in this License, to the extent that they are valid under applicable law. If additional permissions apply only to part of the Program, that part may be used separately under those permissions, but the entire Program remains governed by this License without regard to the additional permissions.
-
-When you convey a copy of a covered work, you may at your option remove any additional permissions from that copy, or from any part of it. (Additional permissions may be written to require their own removal in certain cases when you modify the work.) You may place additional permissions on material, added by you to a covered work, for which you have or can give appropriate copyright permission.
-
-Notwithstanding any other provision of this License, for material you add to a covered work, you may (if authorized by the copyright holders of that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the terms of sections 15 and 16 of this License; or
-    b) Requiring preservation of specified reasonable legal notices or author attributions in that material or in the Appropriate Legal Notices displayed by works containing it; or
-    c) Prohibiting misrepresentation of the origin of that material, or requiring that modified versions of such material be marked in reasonable ways as different from the original version; or
-    d) Limiting the use for publicity purposes of names of licensors or authors of the material; or
-    e) Declining to grant rights under trademark law for use of some trade names, trademarks, or service marks; or
-    f) Requiring indemnification of licensors and authors of that material by anyone who conveys the material (or modified versions of it) with contractual assumptions of liability to the recipient, for any liability that these contractual assumptions directly impose on those licensors and authors.
-
-All other non-permissive additional terms are considered "further restrictions" within the meaning of section 10. If the Program as you received it, or any part of it, contains a notice stating that it is governed by this License along with a term that is a further restriction, you may remove that term. If a license document contains a further restriction but permits relicensing or conveying under this License, you may add to a covered work material governed by the terms of that license document, provided that the further restriction does not survive such relicensing or conveying.
-
-If you add terms to a covered work in accord with this section, you must place, in the relevant source files, a statement of the additional terms that apply to those files, or a notice indicating where to find the applicable terms.
-
-Additional terms, permissive or non-permissive, may be stated in the form of a separately written license, or stated as exceptions; the above requirements apply either way.
-8. Termination.
-
-You may not propagate or modify a covered work except as expressly provided under this License. Any attempt otherwise to propagate or modify it is void, and will automatically terminate your rights under this License (including any patent licenses granted under the third paragraph of section 11).
-
-However, if you cease all violation of this License, then your license from a particular copyright holder is reinstated (a) provisionally, unless and until the copyright holder explicitly and finally terminates your license, and (b) permanently, if the copyright holder fails to notify you of the violation by some reasonable means prior to 60 days after the cessation.
-
-Moreover, your license from a particular copyright holder is reinstated permanently if the copyright holder notifies you of the violation by some reasonable means, this is the first time you have received notice of violation of this License (for any work) from that copyright holder, and you cure the violation prior to 30 days after your receipt of the notice.
-
-Termination of your rights under this section does not terminate the licenses of parties who have received copies or rights from you under this License. If your rights have been terminated and not permanently reinstated, you do not qualify to receive new licenses for the same material under section 10.
-9. Acceptance Not Required for Having Copies.
-
-You are not required to accept this License in order to receive or run a copy of the Program. Ancillary propagation of a covered work occurring solely as a consequence of using peer-to-peer transmission to receive a copy likewise does not require acceptance. However, nothing other than this License grants you permission to propagate or modify any covered work. These actions infringe copyright if you do not accept this License. Therefore, by modifying or propagating a covered work, you indicate your acceptance of this License to do so.
-10. Automatic Licensing of Downstream Recipients.
-
-Each time you convey a covered work, the recipient automatically receives a license from the original licensors, to run, modify and propagate that work, subject to this License. You are not responsible for enforcing compliance by third parties with this License.
-
-An "entity transaction" is a transaction transferring control of an organization, or substantially all assets of one, or subdividing an organization, or merging organizations. If propagation of a covered work results from an entity transaction, each party to that transaction who receives a copy of the work also receives whatever licenses to the work the party's predecessor in interest had or could give under the previous paragraph, plus a right to possession of the Corresponding Source of the work from the predecessor in interest, if the predecessor has it or can get it with reasonable efforts.
-
-You may not impose any further restrictions on the exercise of the rights granted or affirmed under this License. For example, you may not impose a license fee, royalty, or other charge for exercise of rights granted under this License, and you may not initiate litigation (including a cross-claim or counterclaim in a lawsuit) alleging that any patent claim is infringed by making, using, selling, offering for sale, or importing the Program or any portion of it.
-11. Patents.
-
-A "contributor" is a copyright holder who authorizes use under this License of the Program or a work on which the Program is based. The work thus licensed is called the contributor's "contributor version".
-
-A contributor's "essential patent claims" are all patent claims owned or controlled by the contributor, whether already acquired or hereafter acquired, that would be infringed by some manner, permitted by this License, of making, using, or selling its contributor version, but do not include claims that would be infringed only as a consequence of further modification of the contributor version. For purposes of this definition, "control" includes the right to grant patent sublicenses in a manner consistent with the requirements of this License.
-
-Each contributor grants you a non-exclusive, worldwide, royalty-free patent license under the contributor's essential patent claims, to make, use, sell, offer for sale, import and otherwise run, modify and propagate the contents of its contributor version.
-
-In the following three paragraphs, a "patent license" is any express agreement or commitment, however denominated, not to enforce a patent (such as an express permission to practice a patent or covenant not to sue for patent infringement). To "grant" such a patent license to a party means to make such an agreement or commitment not to enforce a patent against the party.
-
-If you convey a covered work, knowingly relying on a patent license, and the Corresponding Source of the work is not available for anyone to copy, free of charge and under the terms of this License, through a publicly available network server or other readily accessible means, then you must either (1) cause the Corresponding Source to be so available, or (2) arrange to deprive yourself of the benefit of the patent license for this particular work, or (3) arrange, in a manner consistent with the requirements of this License, to extend the patent license to downstream recipients. "Knowingly relying" means you have actual knowledge that, but for the patent license, your conveying the covered work in a country, or your recipient's use of the covered work in a country, would infringe one or more identifiable patents in that country that you have reason to believe are valid.
-
-If, pursuant to or in connection with a single transaction or arrangement, you convey, or propagate by procuring conveyance of, a covered work, and grant a patent license to some of the parties receiving the covered work authorizing them to use, propagate, modify or convey a specific copy of the covered work, then the patent license you grant is automatically extended to all recipients of the covered work and works based on it.
-
-A patent license is "discriminatory" if it does not include within the scope of its coverage, prohibits the exercise of, or is conditioned on the non-exercise of one or more of the rights that are specifically granted under this License. You may not convey a covered work if you are a party to an arrangement with a third party that is in the business of distributing software, under which you make payment to the third party based on the extent of your activity of conveying the work, and under which the third party grants, to any of the parties who would receive the covered work from you, a discriminatory patent license (a) in connection with copies of the covered work conveyed by you (or copies made from those copies), or (b) primarily for and in connection with specific products or compilations that contain the covered work, unless you entered into that arrangement, or that patent license was granted, prior to 28 March 2007.
-
-Nothing in this License shall be construed as excluding or limiting any implied license or other defenses to infringement that may otherwise be available to you under applicable patent law.
-12. No Surrender of Others' Freedom.
-
-If conditions are imposed on you (whether by court order, agreement or otherwise) that contradict the conditions of this License, they do not excuse you from the conditions of this License. If you cannot convey a covered work so as to satisfy simultaneously your obligations under this License and any other pertinent obligations, then as a consequence you may not convey it at all. For example, if you agree to terms that obligate you to collect a royalty for further conveying from those to whom you convey the Program, the only way you could satisfy both those terms and this License would be to refrain entirely from conveying the Program.
-13. Remote Network Interaction; Use with the GNU General Public License.
-
-Notwithstanding any other provision of this License, if you modify the Program, your modified version must prominently offer all users interacting with it remotely through a computer network (if your version supports such interaction) an opportunity to receive the Corresponding Source of your version by providing access to the Corresponding Source from a network server at no charge, through some standard or customary means of facilitating copying of software. This Corresponding Source shall include the Corresponding Source for any work covered by version 3 of the GNU General Public License that is incorporated pursuant to the following paragraph.
-
-Notwithstanding any other provision of this License, you have permission to link or combine any covered work with a work licensed under version 3 of the GNU General Public License into a single combined work, and to convey the resulting work. The terms of this License will continue to apply to the part which is the covered work, but the work with which it is combined will remain governed by version 3 of the GNU General Public License.
-14. Revised Versions of this License.
-
-The Free Software Foundation may publish revised and/or new versions of the GNU Affero General Public License from time to time. Such new versions will be similar in spirit to the present version, but may differ in detail to address new problems or concerns.
-
-Each version is given a distinguishing version number. If the Program specifies that a certain numbered version of the GNU Affero General Public License "or any later version" applies to it, you have the option of following the terms and conditions either of that numbered version or of any later version published by the Free Software Foundation. If the Program does not specify a version number of the GNU Affero General Public License, you may choose any version ever published by the Free Software Foundation.
-
-If the Program specifies that a proxy can decide which future versions of the GNU Affero General Public License can be used, that proxy's public statement of acceptance of a version permanently authorizes you to choose that version for the Program.
-
-Later license versions may give you additional or different permissions. However, no additional obligations are imposed on any author or copyright holder as a result of your choosing to follow a later version.
-15. Disclaimer of Warranty.
-
-THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY APPLICABLE LAW. EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE. THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM IS WITH YOU. SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-16. Limitation of Liability.
-
-IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS), EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES.
-17. Interpretation of Sections 15 and 16.
-
-If the disclaimer of warranty and limitation of liability provided above cannot be given local legal effect according to their terms, reviewing courts shall apply local law that most closely approximates an absolute waiver of all civil liability in connection with the Program, unless a warranty or assumption of liability accompanies a copy of the Program in return for a fee.
-
-END OF TERMS AND CONDITIONS
+GNU AFFERO GENERAL PUBLIC LICENSE
+
+Version 3, 19 November 2007
+
+Copyright © 2007 Free Software Foundation, Inc. <https://fsf.org/>
+Everyone is permitted to copy and distribute verbatim copies of this license document, but changing it is not allowed.
+Preamble
+
+The GNU Affero General Public License is a free, copyleft license for software and other kinds of works, specifically designed to ensure cooperation with the community in the case of network server software.
+
+The licenses for most software and other practical works are designed to take away your freedom to share and change the works. By contrast, our General Public Licenses are intended to guarantee your freedom to share and change all versions of a program--to make sure it remains free software for all its users.
+
+When we speak of free software, we are referring to freedom, not price. Our General Public Licenses are designed to make sure that you have the freedom to distribute copies of free software (and charge for them if you wish), that you receive source code or can get it if you want it, that you can change the software or use pieces of it in new free programs, and that you know you can do these things.
+
+Developers that use our General Public Licenses protect your rights with two steps: (1) assert copyright on the software, and (2) offer you this License which gives you legal permission to copy, distribute and/or modify the software.
+
+A secondary benefit of defending all users' freedom is that improvements made in alternate versions of the program, if they receive widespread use, become available for other developers to incorporate. Many developers of free software are heartened and encouraged by the resulting cooperation. However, in the case of software used on network servers, this result may fail to come about. The GNU General Public License permits making a modified version and letting the public access it on a server without ever releasing its source code to the public.
+
+The GNU Affero General Public License is designed specifically to ensure that, in such cases, the modified source code becomes available to the community. It requires the operator of a network server to provide the source code of the modified version running there to the users of that server. Therefore, public use of a modified version, on a publicly accessible server, gives the public access to the source code of the modified version.
+
+An older license, called the Affero General Public License and published by Affero, was designed to accomplish similar goals. This is a different license, not a version of the Affero GPL, but Affero has released a new version of the Affero GPL which permits relicensing under this license.
+
+The precise terms and conditions for copying, distribution and modification follow.
+TERMS AND CONDITIONS
+0. Definitions.
+
+"This License" refers to version 3 of the GNU Affero General Public License.
+
+"Copyright" also means copyright-like laws that apply to other kinds of works, such as semiconductor masks.
+
+"The Program" refers to any copyrightable work licensed under this License. Each licensee is addressed as "you". "Licensees" and "recipients" may be individuals or organizations.
+
+To "modify" a work means to copy from or adapt all or part of the work in a fashion requiring copyright permission, other than the making of an exact copy. The resulting work is called a "modified version" of the earlier work or a work "based on" the earlier work.
+
+A "covered work" means either the unmodified Program or a work based on the Program.
+
+To "propagate" a work means to do anything with it that, without permission, would make you directly or secondarily liable for infringement under applicable copyright law, except executing it on a computer or modifying a private copy. Propagation includes copying, distribution (with or without modification), making available to the public, and in some countries other activities as well.
+
+To "convey" a work means any kind of propagation that enables other parties to make or receive copies. Mere interaction with a user through a computer network, with no transfer of a copy, is not conveying.
+
+An interactive user interface displays "Appropriate Legal Notices" to the extent that it includes a convenient and prominently visible feature that (1) displays an appropriate copyright notice, and (2) tells the user that there is no warranty for the work (except to the extent that warranties are provided), that licensees may convey the work under this License, and how to view a copy of this License. If the interface presents a list of user commands or options, such as a menu, a prominent item in the list meets this criterion.
+1. Source Code.
+
+The "source code" for a work means the preferred form of the work for making modifications to it. "Object code" means any non-source form of a work.
+
+A "Standard Interface" means an interface that either is an official standard defined by a recognized standards body, or, in the case of interfaces specified for a particular programming language, one that is widely used among developers working in that language.
+
+The "System Libraries" of an executable work include anything, other than the work as a whole, that (a) is included in the normal form of packaging a Major Component, but which is not part of that Major Component, and (b) serves only to enable use of the work with that Major Component, or to implement a Standard Interface for which an implementation is available to the public in source code form. A "Major Component", in this context, means a major essential component (kernel, window system, and so on) of the specific operating system (if any) on which the executable work runs, or a compiler used to produce the work, or an object code interpreter used to run it.
+
+The "Corresponding Source" for a work in object code form means all the source code needed to generate, install, and (for an executable work) run the object code and to modify the work, including scripts to control those activities. However, it does not include the work's System Libraries, or general-purpose tools or generally available free programs which are used unmodified in performing those activities but which are not part of the work. For example, Corresponding Source includes interface definition files associated with source files for the work, and the source code for shared libraries and dynamically linked subprograms that the work is specifically designed to require, such as by intimate data communication or control flow between those subprograms and other parts of the work.
+
+The Corresponding Source need not include anything that users can regenerate automatically from other parts of the Corresponding Source.
+
+The Corresponding Source for a work in source code form is that same work.
+2. Basic Permissions.
+
+All rights granted under this License are granted for the term of copyright on the Program, and are irrevocable provided the stated conditions are met. This License explicitly affirms your unlimited permission to run the unmodified Program. The output from running a covered work is covered by this License only if the output, given its content, constitutes a covered work. This License acknowledges your rights of fair use or other equivalent, as provided by copyright law.
+
+You may make, run and propagate covered works that you do not convey, without conditions so long as your license otherwise remains in force. You may convey covered works to others for the sole purpose of having them make modifications exclusively for you, or provide you with facilities for running those works, provided that you comply with the terms of this License in conveying all material for which you do not control copyright. Those thus making or running the covered works for you must do so exclusively on your behalf, under your direction and control, on terms that prohibit them from making any copies of your copyrighted material outside their relationship with you.
+
+Conveying under any other circumstances is permitted solely under the conditions stated below. Sublicensing is not allowed; section 10 makes it unnecessary.
+3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+No covered work shall be deemed part of an effective technological measure under any applicable law fulfilling obligations under article 11 of the WIPO copyright treaty adopted on 20 December 1996, or similar laws prohibiting or restricting circumvention of such measures.
+
+When you convey a covered work, you waive any legal power to forbid circumvention of technological measures to the extent such circumvention is effected by exercising rights under this License with respect to the covered work, and you disclaim any intention to limit operation or modification of the work as a means of enforcing, against the work's users, your or third parties' legal rights to forbid circumvention of technological measures.
+4. Conveying Verbatim Copies.
+
+You may convey verbatim copies of the Program's source code as you receive it, in any medium, provided that you conspicuously and appropriately publish on each copy an appropriate copyright notice; keep intact all notices stating that this License and any non-permissive terms added in accord with section 7 apply to the code; keep intact all notices of the absence of any warranty; and give all recipients a copy of this License along with the Program.
+
+You may charge any price or no price for each copy that you convey, and you may offer support or warranty protection for a fee.
+5. Conveying Modified Source Versions.
+
+You may convey a work based on the Program, or the modifications to produce it from the Program, in the form of source code under the terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified it, and giving a relevant date.
+    b) The work must carry prominent notices stating that it is released under this License and any conditions added under section 7. This requirement modifies the requirement in section 4 to "keep intact all notices".
+    c) You must license the entire work, as a whole, under this License to anyone who comes into possession of a copy. This License will therefore apply, along with any applicable section 7 additional terms, to the whole of the work, and all its parts, regardless of how they are packaged. This License gives no permission to license the work in any other way, but it does not invalidate such permission if you have separately received it.
+    d) If the work has interactive user interfaces, each must display Appropriate Legal Notices; however, if the Program has interactive interfaces that do not display Appropriate Legal Notices, your work need not make them do so.
+
+A compilation of a covered work with other separate and independent works, which are not by their nature extensions of the covered work, and which are not combined with it such as to form a larger program, in or on a volume of a storage or distribution medium, is called an "aggregate" if the compilation and its resulting copyright are not used to limit the access or legal rights of the compilation's users beyond what the individual works permit. Inclusion of a covered work in an aggregate does not cause this License to apply to the other parts of the aggregate.
+6. Conveying Non-Source Forms.
+
+You may convey a covered work in object code form under the terms of sections 4 and 5, provided that you also convey the machine-readable Corresponding Source under the terms of this License, in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product (including a physical distribution medium), accompanied by the Corresponding Source fixed on a durable physical medium customarily used for software interchange.
+    b) Convey the object code in, or embodied in, a physical product (including a physical distribution medium), accompanied by a written offer, valid for at least three years and valid for as long as you offer spare parts or customer support for that product model, to give anyone who possesses the object code either (1) a copy of the Corresponding Source for all the software in the product that is covered by this License, on a durable physical medium customarily used for software interchange, for a price no more than your reasonable cost of physically performing this conveying of source, or (2) access to copy the Corresponding Source from a network server at no charge.
+    c) Convey individual copies of the object code with a copy of the written offer to provide the Corresponding Source. This alternative is allowed only occasionally and noncommercially, and only if you received the object code with such an offer, in accord with subsection 6b.
+    d) Convey the object code by offering access from a designated place (gratis or for a charge), and offer equivalent access to the Corresponding Source in the same way through the same place at no further charge. You need not require recipients to copy the Corresponding Source along with the object code. If the place to copy the object code is a network server, the Corresponding Source may be on a different server (operated by you or a third party) that supports equivalent copying facilities, provided you maintain clear directions next to the object code saying where to find the Corresponding Source. Regardless of what server hosts the Corresponding Source, you remain obligated to ensure that it is available for as long as needed to satisfy these requirements.
+    e) Convey the object code using peer-to-peer transmission, provided you inform other peers where the object code and Corresponding Source of the work are being offered to the general public at no charge under subsection 6d.
+
+A separable portion of the object code, whose source code is excluded from the Corresponding Source as a System Library, need not be included in conveying the object code work.
+
+A "User Product" is either (1) a "consumer product", which means any tangible personal property which is normally used for personal, family, or household purposes, or (2) anything designed or sold for incorporation into a dwelling. In determining whether a product is a consumer product, doubtful cases shall be resolved in favor of coverage. For a particular product received by a particular user, "normally used" refers to a typical or common use of that class of product, regardless of the status of the particular user or of the way in which the particular user actually uses, or expects or is expected to use, the product. A product is a consumer product regardless of whether the product has substantial commercial, industrial or non-consumer uses, unless such uses represent the only significant mode of use of the product.
+
+"Installation Information" for a User Product means any methods, procedures, authorization keys, or other information required to install and execute modified versions of a covered work in that User Product from a modified version of its Corresponding Source. The information must suffice to ensure that the continued functioning of the modified object code is in no case prevented or interfered with solely because modification has been made.
+
+If you convey an object code work under this section in, or with, or specifically for use in, a User Product, and the conveying occurs as part of a transaction in which the right of possession and use of the User Product is transferred to the recipient in perpetuity or for a fixed term (regardless of how the transaction is characterized), the Corresponding Source conveyed under this section must be accompanied by the Installation Information. But this requirement does not apply if neither you nor any third party retains the ability to install modified object code on the User Product (for example, the work has been installed in ROM).
+
+The requirement to provide Installation Information does not include a requirement to continue to provide support service, warranty, or updates for a work that has been modified or installed by the recipient, or for the User Product in which it has been modified or installed. Access to a network may be denied when the modification itself materially and adversely affects the operation of the network or violates the rules and protocols for communication across the network.
+
+Corresponding Source conveyed, and Installation Information provided, in accord with this section must be in a format that is publicly documented (and with an implementation available to the public in source code form), and must require no special password or key for unpacking, reading or copying.
+7. Additional Terms.
+
+"Additional permissions" are terms that supplement the terms of this License by making exceptions from one or more of its conditions. Additional permissions that are applicable to the entire Program shall be treated as though they were included in this License, to the extent that they are valid under applicable law. If additional permissions apply only to part of the Program, that part may be used separately under those permissions, but the entire Program remains governed by this License without regard to the additional permissions.
+
+When you convey a copy of a covered work, you may at your option remove any additional permissions from that copy, or from any part of it. (Additional permissions may be written to require their own removal in certain cases when you modify the work.) You may place additional permissions on material, added by you to a covered work, for which you have or can give appropriate copyright permission.
+
+Notwithstanding any other provision of this License, for material you add to a covered work, you may (if authorized by the copyright holders of that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the terms of sections 15 and 16 of this License; or
+    b) Requiring preservation of specified reasonable legal notices or author attributions in that material or in the Appropriate Legal Notices displayed by works containing it; or
+    c) Prohibiting misrepresentation of the origin of that material, or requiring that modified versions of such material be marked in reasonable ways as different from the original version; or
+    d) Limiting the use for publicity purposes of names of licensors or authors of the material; or
+    e) Declining to grant rights under trademark law for use of some trade names, trademarks, or service marks; or
+    f) Requiring indemnification of licensors and authors of that material by anyone who conveys the material (or modified versions of it) with contractual assumptions of liability to the recipient, for any liability that these contractual assumptions directly impose on those licensors and authors.
+
+All other non-permissive additional terms are considered "further restrictions" within the meaning of section 10. If the Program as you received it, or any part of it, contains a notice stating that it is governed by this License along with a term that is a further restriction, you may remove that term. If a license document contains a further restriction but permits relicensing or conveying under this License, you may add to a covered work material governed by the terms of that license document, provided that the further restriction does not survive such relicensing or conveying.
+
+If you add terms to a covered work in accord with this section, you must place, in the relevant source files, a statement of the additional terms that apply to those files, or a notice indicating where to find the applicable terms.
+
+Additional terms, permissive or non-permissive, may be stated in the form of a separately written license, or stated as exceptions; the above requirements apply either way.
+8. Termination.
+
+You may not propagate or modify a covered work except as expressly provided under this License. Any attempt otherwise to propagate or modify it is void, and will automatically terminate your rights under this License (including any patent licenses granted under the third paragraph of section 11).
+
+However, if you cease all violation of this License, then your license from a particular copyright holder is reinstated (a) provisionally, unless and until the copyright holder explicitly and finally terminates your license, and (b) permanently, if the copyright holder fails to notify you of the violation by some reasonable means prior to 60 days after the cessation.
+
+Moreover, your license from a particular copyright holder is reinstated permanently if the copyright holder notifies you of the violation by some reasonable means, this is the first time you have received notice of violation of this License (for any work) from that copyright holder, and you cure the violation prior to 30 days after your receipt of the notice.
+
+Termination of your rights under this section does not terminate the licenses of parties who have received copies or rights from you under this License. If your rights have been terminated and not permanently reinstated, you do not qualify to receive new licenses for the same material under section 10.
+9. Acceptance Not Required for Having Copies.
+
+You are not required to accept this License in order to receive or run a copy of the Program. Ancillary propagation of a covered work occurring solely as a consequence of using peer-to-peer transmission to receive a copy likewise does not require acceptance. However, nothing other than this License grants you permission to propagate or modify any covered work. These actions infringe copyright if you do not accept this License. Therefore, by modifying or propagating a covered work, you indicate your acceptance of this License to do so.
+10. Automatic Licensing of Downstream Recipients.
+
+Each time you convey a covered work, the recipient automatically receives a license from the original licensors, to run, modify and propagate that work, subject to this License. You are not responsible for enforcing compliance by third parties with this License.
+
+An "entity transaction" is a transaction transferring control of an organization, or substantially all assets of one, or subdividing an organization, or merging organizations. If propagation of a covered work results from an entity transaction, each party to that transaction who receives a copy of the work also receives whatever licenses to the work the party's predecessor in interest had or could give under the previous paragraph, plus a right to possession of the Corresponding Source of the work from the predecessor in interest, if the predecessor has it or can get it with reasonable efforts.
+
+You may not impose any further restrictions on the exercise of the rights granted or affirmed under this License. For example, you may not impose a license fee, royalty, or other charge for exercise of rights granted under this License, and you may not initiate litigation (including a cross-claim or counterclaim in a lawsuit) alleging that any patent claim is infringed by making, using, selling, offering for sale, or importing the Program or any portion of it.
+11. Patents.
+
+A "contributor" is a copyright holder who authorizes use under this License of the Program or a work on which the Program is based. The work thus licensed is called the contributor's "contributor version".
+
+A contributor's "essential patent claims" are all patent claims owned or controlled by the contributor, whether already acquired or hereafter acquired, that would be infringed by some manner, permitted by this License, of making, using, or selling its contributor version, but do not include claims that would be infringed only as a consequence of further modification of the contributor version. For purposes of this definition, "control" includes the right to grant patent sublicenses in a manner consistent with the requirements of this License.
+
+Each contributor grants you a non-exclusive, worldwide, royalty-free patent license under the contributor's essential patent claims, to make, use, sell, offer for sale, import and otherwise run, modify and propagate the contents of its contributor version.
+
+In the following three paragraphs, a "patent license" is any express agreement or commitment, however denominated, not to enforce a patent (such as an express permission to practice a patent or covenant not to sue for patent infringement). To "grant" such a patent license to a party means to make such an agreement or commitment not to enforce a patent against the party.
+
+If you convey a covered work, knowingly relying on a patent license, and the Corresponding Source of the work is not available for anyone to copy, free of charge and under the terms of this License, through a publicly available network server or other readily accessible means, then you must either (1) cause the Corresponding Source to be so available, or (2) arrange to deprive yourself of the benefit of the patent license for this particular work, or (3) arrange, in a manner consistent with the requirements of this License, to extend the patent license to downstream recipients. "Knowingly relying" means you have actual knowledge that, but for the patent license, your conveying the covered work in a country, or your recipient's use of the covered work in a country, would infringe one or more identifiable patents in that country that you have reason to believe are valid.
+
+If, pursuant to or in connection with a single transaction or arrangement, you convey, or propagate by procuring conveyance of, a covered work, and grant a patent license to some of the parties receiving the covered work authorizing them to use, propagate, modify or convey a specific copy of the covered work, then the patent license you grant is automatically extended to all recipients of the covered work and works based on it.
+
+A patent license is "discriminatory" if it does not include within the scope of its coverage, prohibits the exercise of, or is conditioned on the non-exercise of one or more of the rights that are specifically granted under this License. You may not convey a covered work if you are a party to an arrangement with a third party that is in the business of distributing software, under which you make payment to the third party based on the extent of your activity of conveying the work, and under which the third party grants, to any of the parties who would receive the covered work from you, a discriminatory patent license (a) in connection with copies of the covered work conveyed by you (or copies made from those copies), or (b) primarily for and in connection with specific products or compilations that contain the covered work, unless you entered into that arrangement, or that patent license was granted, prior to 28 March 2007.
+
+Nothing in this License shall be construed as excluding or limiting any implied license or other defenses to infringement that may otherwise be available to you under applicable patent law.
+12. No Surrender of Others' Freedom.
+
+If conditions are imposed on you (whether by court order, agreement or otherwise) that contradict the conditions of this License, they do not excuse you from the conditions of this License. If you cannot convey a covered work so as to satisfy simultaneously your obligations under this License and any other pertinent obligations, then as a consequence you may not convey it at all. For example, if you agree to terms that obligate you to collect a royalty for further conveying from those to whom you convey the Program, the only way you could satisfy both those terms and this License would be to refrain entirely from conveying the Program.
+13. Remote Network Interaction; Use with the GNU General Public License.
+
+Notwithstanding any other provision of this License, if you modify the Program, your modified version must prominently offer all users interacting with it remotely through a computer network (if your version supports such interaction) an opportunity to receive the Corresponding Source of your version by providing access to the Corresponding Source from a network server at no charge, through some standard or customary means of facilitating copying of software. This Corresponding Source shall include the Corresponding Source for any work covered by version 3 of the GNU General Public License that is incorporated pursuant to the following paragraph.
+
+Notwithstanding any other provision of this License, you have permission to link or combine any covered work with a work licensed under version 3 of the GNU General Public License into a single combined work, and to convey the resulting work. The terms of this License will continue to apply to the part which is the covered work, but the work with which it is combined will remain governed by version 3 of the GNU General Public License.
+14. Revised Versions of this License.
+
+The Free Software Foundation may publish revised and/or new versions of the GNU Affero General Public License from time to time. Such new versions will be similar in spirit to the present version, but may differ in detail to address new problems or concerns.
+
+Each version is given a distinguishing version number. If the Program specifies that a certain numbered version of the GNU Affero General Public License "or any later version" applies to it, you have the option of following the terms and conditions either of that numbered version or of any later version published by the Free Software Foundation. If the Program does not specify a version number of the GNU Affero General Public License, you may choose any version ever published by the Free Software Foundation.
+
+If the Program specifies that a proxy can decide which future versions of the GNU Affero General Public License can be used, that proxy's public statement of acceptance of a version permanently authorizes you to choose that version for the Program.
+
+Later license versions may give you additional or different permissions. However, no additional obligations are imposed on any author or copyright holder as a result of your choosing to follow a later version.
+15. Disclaimer of Warranty.
+
+THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY APPLICABLE LAW. EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE. THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM IS WITH YOU. SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+16. Limitation of Liability.
+
+IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS), EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES.
+17. Interpretation of Sections 15 and 16.
+
+If the disclaimer of warranty and limitation of liability provided above cannot be given local legal effect according to their terms, reviewing courts shall apply local law that most closely approximates an absolute waiver of all civil liability in connection with the Program, unless a warranty or assumption of liability accompanies a copy of the Program in return for a fee.
+
+END OF TERMS AND CONDITIONS
```

### Comparing `nobinobi-core-0.1.4.6/README.rst` & `nobinobi-core-0.1.4.7/README.rst`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.6/nobinobi_core/__init__.py` & `nobinobi-core-0.1.4.7/nobinobi_core/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #      but WITHOUT ANY WARRANTY; without even the implied warranty of
 #      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #      GNU Affero General Public License for more details.
 #
 #      You should have received a copy of the GNU Affero General Public License
 #      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-__version__ = '0.1.4.6'
+__version__ = '0.1.4.7'
```

### Comparing `nobinobi-core-0.1.4.6/nobinobi_core/admin.py` & `nobinobi-core-0.1.4.7/nobinobi_core/admin.py`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.6/nobinobi_core/apps.py` & `nobinobi-core-0.1.4.7/nobinobi_core/apps.py`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.6/nobinobi_core/forms.py` & `nobinobi-core-0.1.4.7/nobinobi_core/forms.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-#      Copyright (C) 2020 <Florian Alu - Prolibre - https://prolibre.com
-#      This program is free software: you can redistribute it and/or modify
-#      it under the terms of the GNU Affero General Public License as
-#      published by the Free Software Foundation, either version 3 of the
-#      License, or (at your option) any later version.
-#
-#      This program is distributed in the hope that it will be useful,
-#      but WITHOUT ANY WARRANTY; without even the implied warranty of
-#      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#      GNU Affero General Public License for more details.
-#
-#      You should have received a copy of the GNU Affero General Public License
-#      along with this program.  If not, see <https://www.gnu.org/licenses/>.
-#
-# -*- coding: utf-8 -*-
-
-from crispy_forms.helper import FormHelper
-from crispy_forms.layout import Submit
-from django import forms
-from django.utils import timezone
-from django.utils.translation import gettext as _
-
-
-def year_choices():
-    now = timezone.localdate()
-    min_date = now.year - 1
-    max_date = now.year + 2
-    return [(r, r) for r in range(min_date, max_date)], now
-
-
-class AddOfficialHolidayForm(forms.Form):
-    """form de validation pour l'ajout"""
-    year = forms.ChoiceField(label=_("Year"), choices=year_choices()[0], initial=year_choices()[1])
-
-    def __init__(self, *args, **kwargs):
-        super(AddOfficialHolidayForm, self).__init__(*args, **kwargs)
-
-        self.helper = FormHelper()
-        # self.helper.
-        self.helper.form_class = 'form-horizontal blueForms'
-        self.helper.label_class = ""
-        self.helper.field_class = "col-lg-12"
-        self.helper.add_input(Submit('submit', _("Submit")))
+#      Copyright (C) 2020 <Florian Alu - Prolibre - https://prolibre.com
+#      This program is free software: you can redistribute it and/or modify
+#      it under the terms of the GNU Affero General Public License as
+#      published by the Free Software Foundation, either version 3 of the
+#      License, or (at your option) any later version.
+#
+#      This program is distributed in the hope that it will be useful,
+#      but WITHOUT ANY WARRANTY; without even the implied warranty of
+#      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#      GNU Affero General Public License for more details.
+#
+#      You should have received a copy of the GNU Affero General Public License
+#      along with this program.  If not, see <https://www.gnu.org/licenses/>.
+#
+# -*- coding: utf-8 -*-
+from crispy_forms.helper import FormHelper
+from crispy_forms.layout import Submit
+from django import forms
+from django.utils import timezone
+from django.utils.translation import gettext as _
+
+
+def year_choices():
+    now = timezone.localdate()
+    min_date = now.year - 1
+    max_date = now.year + 2
+    return [(r, r) for r in range(min_date, max_date)], now
+
+
+class AddOfficialHolidayForm(forms.Form):
+    """Formulaire de validation pour l'ajout"""
+    year = forms.ChoiceField(label=_("Year"), choices=year_choices()[0], initial=year_choices()[1])
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.helper = FormHelper()
+        self.helper.form_id = 'id-add-holiday-Form'
+        self.helper.form_class = 'form-horizontal blueForms'
+        self.helper.form_method = 'post'
+        self.helper.label_class = ""
+        self.helper.field_class = "col-lg-12"
+
+        self.helper.add_input(Submit('submit', _("Submit")))
```

### Comparing `nobinobi-core-0.1.4.6/nobinobi_core/functions.py` & `nobinobi-core-0.1.4.7/nobinobi_core/functions.py`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.6/nobinobi_core/locale/fr/LC_MESSAGES/django.mo` & `nobinobi-core-0.1.4.7/nobinobi_core/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.6/nobinobi_core/migrations/0001_initial.py` & `nobinobi-core-0.1.4.7/nobinobi_core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.6/nobinobi_core/migrations/0002_organisation_organisationclosure.py` & `nobinobi-core-0.1.4.7/nobinobi_core/migrations/0002_organisation_organisationclosure.py`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.6/nobinobi_core/migrations/__init__.py` & `nobinobi-core-0.1.4.7/nobinobi_core/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.6/nobinobi_core/models.py` & `nobinobi-core-0.1.4.7/nobinobi_core/models.py`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.6/nobinobi_core/static/css/bootstrap-datetimepicker-standalone.css` & `nobinobi-core-0.1.4.7/nobinobi_core/static/css/bootstrap-datetimepicker-standalone.css`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,114 +1,114 @@
-/*
- *     Copyright (C) 2020 <Florian Alu - Prolibre - https://prolibre.com
- *     This program is free software: you can redistribute it and/or modify
- *     it under the terms of the GNU Affero General Public License as
- *     published by the Free Software Foundation, either version 3 of the
- *     License, or (at your option) any later version.
- *
- *     This program is distributed in the hope that it will be useful,
- *     but WITHOUT ANY WARRANTY; without even the implied warranty of
- *     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
- *     GNU Affero General Public License for more details.
- *
- *     You should have received a copy of the GNU Affero General Public License
- *     along with this program.  If not, see <https://www.gnu.org/licenses/>.
- */
-
-@font-face {
-    font-family: 'Glyphicons Halflings';
-    src: url('../fonts/glyphicons-halflings-regular.eot');
-    src: url('../fonts/glyphicons-halflings-regular.eot?#iefix') format('embedded-opentype'), url('../fonts/glyphicons-halflings-regular.woff2') format('woff2'), url('../fonts/glyphicons-halflings-regular.woff') format('woff'), url('../fonts/glyphicons-halflings-regular.ttf') format('truetype'), url('../fonts/glyphicons-halflings-regular.svg#glyphicons_halflingsregular') format('svg');
-}
-
-.glyphicon {
-    position: relative;
-    top: 1px;
-    display: inline-block;
-    font-family: 'Glyphicons Halflings';
-    font-style: normal;
-    font-weight: normal;
-    line-height: 1;
-    -webkit-font-smoothing: antialiased;
-    -moz-osx-font-smoothing: grayscale;
-}
-
-.glyphicon-time:before {
-    content: "\e023";
-}
-
-.glyphicon-chevron-left:before {
-    content: "\e079";
-}
-
-.glyphicon-chevron-right:before {
-    content: "\e080";
-}
-
-.glyphicon-chevron-up:before {
-    content: "\e113";
-}
-
-.glyphicon-chevron-down:before {
-    content: "\e114";
-}
-
-.glyphicon-calendar:before {
-    content: "\e109";
-}
-
-.btn {
-    display: inline-block;
-    padding: 6px 12px;
-    margin-bottom: 0;
-    font-size: 14px;
-    font-weight: normal;
-    line-height: 1.42857143;
-    text-align: center;
-    white-space: nowrap;
-    vertical-align: middle;
-    -ms-touch-action: manipulation;
-    touch-action: manipulation;
-    cursor: pointer;
-    -webkit-user-select: none;
-    -moz-user-select: none;
-    -ms-user-select: none;
-    user-select: none;
-    background-image: none;
-    border: 1px solid transparent;
-    border-radius: 4px;
-}
-
-.collapse {
-    display: none;
-}
-
-    .collapse.in {
-        display: block;
-    }
-
-.dropdown-menu {
-    position: absolute;
-    left: 0;
-    z-index: 1000;
-    display: none;
-    float: left;
-    min-width: 160px;
-    padding: 5px 0;
-    margin: 2px 0 0;
-    font-size: 14px;
-    text-align: left;
-    list-style: none;
-    background-color: #fff;
-    -webkit-background-clip: padding-box;
-    background-clip: padding-box;
-    border: 1px solid #ccc;
-    border: 1px solid rgba(0, 0, 0, .15);
-    border-radius: 4px;
-    -webkit-box-shadow: 0 6px 12px rgba(0, 0, 0, .175);
-    box-shadow: 0 6px 12px rgba(0, 0, 0, .175);
-}
-
-.list-unstyled {
-    padding-left: 0;
-    list-style: none;
-}
+/*
+ *     Copyright (C) 2020 <Florian Alu - Prolibre - https://prolibre.com
+ *     This program is free software: you can redistribute it and/or modify
+ *     it under the terms of the GNU Affero General Public License as
+ *     published by the Free Software Foundation, either version 3 of the
+ *     License, or (at your option) any later version.
+ *
+ *     This program is distributed in the hope that it will be useful,
+ *     but WITHOUT ANY WARRANTY; without even the implied warranty of
+ *     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+ *     GNU Affero General Public License for more details.
+ *
+ *     You should have received a copy of the GNU Affero General Public License
+ *     along with this program.  If not, see <https://www.gnu.org/licenses/>.
+ */
+
+@font-face {
+    font-family: 'Glyphicons Halflings';
+    src: url('../fonts/glyphicons-halflings-regular.eot');
+    src: url('../fonts/glyphicons-halflings-regular.eot?#iefix') format('embedded-opentype'), url('../fonts/glyphicons-halflings-regular.woff2') format('woff2'), url('../fonts/glyphicons-halflings-regular.woff') format('woff'), url('../fonts/glyphicons-halflings-regular.ttf') format('truetype'), url('../fonts/glyphicons-halflings-regular.svg#glyphicons_halflingsregular') format('svg');
+}
+
+.glyphicon {
+    position: relative;
+    top: 1px;
+    display: inline-block;
+    font-family: 'Glyphicons Halflings';
+    font-style: normal;
+    font-weight: normal;
+    line-height: 1;
+    -webkit-font-smoothing: antialiased;
+    -moz-osx-font-smoothing: grayscale;
+}
+
+.glyphicon-time:before {
+    content: "\e023";
+}
+
+.glyphicon-chevron-left:before {
+    content: "\e079";
+}
+
+.glyphicon-chevron-right:before {
+    content: "\e080";
+}
+
+.glyphicon-chevron-up:before {
+    content: "\e113";
+}
+
+.glyphicon-chevron-down:before {
+    content: "\e114";
+}
+
+.glyphicon-calendar:before {
+    content: "\e109";
+}
+
+.btn {
+    display: inline-block;
+    padding: 6px 12px;
+    margin-bottom: 0;
+    font-size: 14px;
+    font-weight: normal;
+    line-height: 1.42857143;
+    text-align: center;
+    white-space: nowrap;
+    vertical-align: middle;
+    -ms-touch-action: manipulation;
+    touch-action: manipulation;
+    cursor: pointer;
+    -webkit-user-select: none;
+    -moz-user-select: none;
+    -ms-user-select: none;
+    user-select: none;
+    background-image: none;
+    border: 1px solid transparent;
+    border-radius: 4px;
+}
+
+.collapse {
+    display: none;
+}
+
+    .collapse.in {
+        display: block;
+    }
+
+.dropdown-menu {
+    position: absolute;
+    left: 0;
+    z-index: 1000;
+    display: none;
+    float: left;
+    min-width: 160px;
+    padding: 5px 0;
+    margin: 2px 0 0;
+    font-size: 14px;
+    text-align: left;
+    list-style: none;
+    background-color: #fff;
+    -webkit-background-clip: padding-box;
+    background-clip: padding-box;
+    border: 1px solid #ccc;
+    border: 1px solid rgba(0, 0, 0, .15);
+    border-radius: 4px;
+    -webkit-box-shadow: 0 6px 12px rgba(0, 0, 0, .175);
+    box-shadow: 0 6px 12px rgba(0, 0, 0, .175);
+}
+
+.list-unstyled {
+    padding-left: 0;
+    list-style: none;
+}
```

### Comparing `nobinobi-core-0.1.4.6/nobinobi_core/static/css/bootstrap-datetimepicker.css` & `nobinobi-core-0.1.4.7/nobinobi_core/static/css/bootstrap-datetimepicker.css`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,390 +1,390 @@
-/*
- *     Copyright (C) 2020 <Florian Alu - Prolibre - https://prolibre.com
- *     This program is free software: you can redistribute it and/or modify
- *     it under the terms of the GNU Affero General Public License as
- *     published by the Free Software Foundation, either version 3 of the
- *     License, or (at your option) any later version.
- *
- *     This program is distributed in the hope that it will be useful,
- *     but WITHOUT ANY WARRANTY; without even the implied warranty of
- *     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
- *     GNU Affero General Public License for more details.
- *
- *     You should have received a copy of the GNU Affero General Public License
- *     along with this program.  If not, see <https://www.gnu.org/licenses/>.
- */
-
-/*!
- * Datetimepicker for Bootstrap 3
- * version : 4.17.47
- * https://github.com/Eonasdan/bootstrap-datetimepicker/
- */
-.bootstrap-datetimepicker-widget {
-  list-style: none;
-}
-.bootstrap-datetimepicker-widget.dropdown-menu {
-  display: block;
-  margin: 2px 0;
-  padding: 4px;
-  width: 19em;
-}
-@media (min-width: 768px) {
-  .bootstrap-datetimepicker-widget.dropdown-menu.timepicker-sbs {
-    width: 38em;
-  }
-}
-@media (min-width: 992px) {
-  .bootstrap-datetimepicker-widget.dropdown-menu.timepicker-sbs {
-    width: 38em;
-  }
-}
-@media (min-width: 1200px) {
-  .bootstrap-datetimepicker-widget.dropdown-menu.timepicker-sbs {
-    width: 38em;
-  }
-}
-.bootstrap-datetimepicker-widget.dropdown-menu:before,
-.bootstrap-datetimepicker-widget.dropdown-menu:after {
-  content: '';
-  display: inline-block;
-  position: absolute;
-}
-.bootstrap-datetimepicker-widget.dropdown-menu.bottom:before {
-  border-left: 7px solid transparent;
-  border-right: 7px solid transparent;
-  border-bottom: 7px solid #ccc;
-  border-bottom-color: rgba(0, 0, 0, 0.2);
-  top: -7px;
-  left: 7px;
-}
-.bootstrap-datetimepicker-widget.dropdown-menu.bottom:after {
-  border-left: 6px solid transparent;
-  border-right: 6px solid transparent;
-  border-bottom: 6px solid white;
-  top: -6px;
-  left: 8px;
-}
-.bootstrap-datetimepicker-widget.dropdown-menu.top:before {
-  border-left: 7px solid transparent;
-  border-right: 7px solid transparent;
-  border-top: 7px solid #ccc;
-  border-top-color: rgba(0, 0, 0, 0.2);
-  bottom: -7px;
-  left: 6px;
-}
-.bootstrap-datetimepicker-widget.dropdown-menu.top:after {
-  border-left: 6px solid transparent;
-  border-right: 6px solid transparent;
-  border-top: 6px solid white;
-  bottom: -6px;
-  left: 7px;
-}
-.bootstrap-datetimepicker-widget.dropdown-menu.pull-right:before {
-  left: auto;
-  right: 6px;
-}
-.bootstrap-datetimepicker-widget.dropdown-menu.pull-right:after {
-  left: auto;
-  right: 7px;
-}
-.bootstrap-datetimepicker-widget .list-unstyled {
-  margin: 0;
-}
-.bootstrap-datetimepicker-widget a[data-action] {
-  padding: 6px 0;
-}
-.bootstrap-datetimepicker-widget a[data-action]:active {
-  box-shadow: none;
-}
-.bootstrap-datetimepicker-widget .timepicker-hour,
-.bootstrap-datetimepicker-widget .timepicker-minute,
-.bootstrap-datetimepicker-widget .timepicker-second {
-  width: 54px;
-  font-weight: bold;
-  font-size: 1.2em;
-  margin: 0;
-}
-.bootstrap-datetimepicker-widget button[data-action] {
-  padding: 6px;
-}
-.bootstrap-datetimepicker-widget .btn[data-action="incrementHours"]::after {
-  position: absolute;
-  width: 1px;
-  height: 1px;
-  margin: -1px;
-  padding: 0;
-  overflow: hidden;
-  clip: rect(0, 0, 0, 0);
-  border: 0;
-  content: "Increment Hours";
-}
-.bootstrap-datetimepicker-widget .btn[data-action="incrementMinutes"]::after {
-  position: absolute;
-  width: 1px;
-  height: 1px;
-  margin: -1px;
-  padding: 0;
-  overflow: hidden;
-  clip: rect(0, 0, 0, 0);
-  border: 0;
-  content: "Increment Minutes";
-}
-.bootstrap-datetimepicker-widget .btn[data-action="decrementHours"]::after {
-  position: absolute;
-  width: 1px;
-  height: 1px;
-  margin: -1px;
-  padding: 0;
-  overflow: hidden;
-  clip: rect(0, 0, 0, 0);
-  border: 0;
-  content: "Decrement Hours";
-}
-.bootstrap-datetimepicker-widget .btn[data-action="decrementMinutes"]::after {
-  position: absolute;
-  width: 1px;
-  height: 1px;
-  margin: -1px;
-  padding: 0;
-  overflow: hidden;
-  clip: rect(0, 0, 0, 0);
-  border: 0;
-  content: "Decrement Minutes";
-}
-.bootstrap-datetimepicker-widget .btn[data-action="showHours"]::after {
-  position: absolute;
-  width: 1px;
-  height: 1px;
-  margin: -1px;
-  padding: 0;
-  overflow: hidden;
-  clip: rect(0, 0, 0, 0);
-  border: 0;
-  content: "Show Hours";
-}
-.bootstrap-datetimepicker-widget .btn[data-action="showMinutes"]::after {
-  position: absolute;
-  width: 1px;
-  height: 1px;
-  margin: -1px;
-  padding: 0;
-  overflow: hidden;
-  clip: rect(0, 0, 0, 0);
-  border: 0;
-  content: "Show Minutes";
-}
-.bootstrap-datetimepicker-widget .btn[data-action="togglePeriod"]::after {
-  position: absolute;
-  width: 1px;
-  height: 1px;
-  margin: -1px;
-  padding: 0;
-  overflow: hidden;
-  clip: rect(0, 0, 0, 0);
-  border: 0;
-  content: "Toggle AM/PM";
-}
-.bootstrap-datetimepicker-widget .btn[data-action="clear"]::after {
-  position: absolute;
-  width: 1px;
-  height: 1px;
-  margin: -1px;
-  padding: 0;
-  overflow: hidden;
-  clip: rect(0, 0, 0, 0);
-  border: 0;
-  content: "Clear the picker";
-}
-.bootstrap-datetimepicker-widget .btn[data-action="today"]::after {
-  position: absolute;
-  width: 1px;
-  height: 1px;
-  margin: -1px;
-  padding: 0;
-  overflow: hidden;
-  clip: rect(0, 0, 0, 0);
-  border: 0;
-  content: "Set the date to today";
-}
-.bootstrap-datetimepicker-widget .picker-switch {
-  text-align: center;
-}
-.bootstrap-datetimepicker-widget .picker-switch::after {
-  position: absolute;
-  width: 1px;
-  height: 1px;
-  margin: -1px;
-  padding: 0;
-  overflow: hidden;
-  clip: rect(0, 0, 0, 0);
-  border: 0;
-  content: "Toggle Date and Time Screens";
-}
-.bootstrap-datetimepicker-widget .picker-switch td {
-  padding: 0;
-  margin: 0;
-  height: auto;
-  width: auto;
-  line-height: inherit;
-}
-.bootstrap-datetimepicker-widget .picker-switch td span {
-  line-height: 2.5;
-  height: 2.5em;
-  width: 100%;
-}
-.bootstrap-datetimepicker-widget table {
-  width: 100%;
-  margin: 0;
-}
-.bootstrap-datetimepicker-widget table td,
-.bootstrap-datetimepicker-widget table th {
-  text-align: center;
-  border-radius: 4px;
-}
-.bootstrap-datetimepicker-widget table th {
-  height: 20px;
-  line-height: 20px;
-  width: 20px;
-}
-.bootstrap-datetimepicker-widget table th.picker-switch {
-  width: 145px;
-}
-.bootstrap-datetimepicker-widget table th.disabled,
-.bootstrap-datetimepicker-widget table th.disabled:hover {
-  background: none;
-  color: #777777;
-  cursor: not-allowed;
-}
-.bootstrap-datetimepicker-widget table th.prev::after {
-  position: absolute;
-  width: 1px;
-  height: 1px;
-  margin: -1px;
-  padding: 0;
-  overflow: hidden;
-  clip: rect(0, 0, 0, 0);
-  border: 0;
-  content: "Previous Month";
-}
-.bootstrap-datetimepicker-widget table th.next::after {
-  position: absolute;
-  width: 1px;
-  height: 1px;
-  margin: -1px;
-  padding: 0;
-  overflow: hidden;
-  clip: rect(0, 0, 0, 0);
-  border: 0;
-  content: "Next Month";
-}
-.bootstrap-datetimepicker-widget table thead tr:first-child th {
-  cursor: pointer;
-}
-.bootstrap-datetimepicker-widget table thead tr:first-child th:hover {
-  background: #eeeeee;
-}
-.bootstrap-datetimepicker-widget table td {
-  height: 54px;
-  line-height: 54px;
-  width: 54px;
-}
-.bootstrap-datetimepicker-widget table td.cw {
-  font-size: .8em;
-  height: 20px;
-  line-height: 20px;
-  color: #777777;
-}
-.bootstrap-datetimepicker-widget table td.day {
-  height: 20px;
-  line-height: 20px;
-  width: 20px;
-}
-.bootstrap-datetimepicker-widget table td.day:hover,
-.bootstrap-datetimepicker-widget table td.hour:hover,
-.bootstrap-datetimepicker-widget table td.minute:hover,
-.bootstrap-datetimepicker-widget table td.second:hover {
-  background: #eeeeee;
-  cursor: pointer;
-}
-.bootstrap-datetimepicker-widget table td.old,
-.bootstrap-datetimepicker-widget table td.new {
-  color: #777777;
-}
-.bootstrap-datetimepicker-widget table td.today {
-  position: relative;
-}
-.bootstrap-datetimepicker-widget table td.today:before {
-  content: '';
-  display: inline-block;
-  border: solid transparent;
-  border-width: 0 0 7px 7px;
-  border-bottom-color: #337ab7;
-  border-top-color: rgba(0, 0, 0, 0.2);
-  position: absolute;
-  bottom: 4px;
-  right: 4px;
-}
-.bootstrap-datetimepicker-widget table td.active,
-.bootstrap-datetimepicker-widget table td.active:hover {
-  background-color: #337ab7;
-  color: #fff;
-  text-shadow: 0 -1px 0 rgba(0, 0, 0, 0.25);
-}
-.bootstrap-datetimepicker-widget table td.active.today:before {
-  border-bottom-color: #fff;
-}
-.bootstrap-datetimepicker-widget table td.disabled,
-.bootstrap-datetimepicker-widget table td.disabled:hover {
-  background: none;
-  color: #777777;
-  cursor: not-allowed;
-}
-.bootstrap-datetimepicker-widget table td span {
-  display: inline-block;
-  width: 54px;
-  height: 54px;
-  line-height: 54px;
-  margin: 2px 1.5px;
-  cursor: pointer;
-  border-radius: 4px;
-}
-.bootstrap-datetimepicker-widget table td span:hover {
-  background: #eeeeee;
-}
-.bootstrap-datetimepicker-widget table td span.active {
-  background-color: #337ab7;
-  color: #fff;
-  text-shadow: 0 -1px 0 rgba(0, 0, 0, 0.25);
-}
-.bootstrap-datetimepicker-widget table td span.old {
-  color: #777777;
-}
-.bootstrap-datetimepicker-widget table td span.disabled,
-.bootstrap-datetimepicker-widget table td span.disabled:hover {
-  background: none;
-  color: #777777;
-  cursor: not-allowed;
-}
-.bootstrap-datetimepicker-widget.usetwentyfour td.hour {
-  height: 27px;
-  line-height: 27px;
-}
-.bootstrap-datetimepicker-widget.wider {
-  width: 21em;
-}
-.bootstrap-datetimepicker-widget .datepicker-decades .decade {
-  line-height: 1.8em !important;
-}
-.input-group.date .input-group-addon {
-  cursor: pointer;
-}
-.sr-only {
-  position: absolute;
-  width: 1px;
-  height: 1px;
-  margin: -1px;
-  padding: 0;
-  overflow: hidden;
-  clip: rect(0, 0, 0, 0);
-  border: 0;
-}
+/*
+ *     Copyright (C) 2020 <Florian Alu - Prolibre - https://prolibre.com
+ *     This program is free software: you can redistribute it and/or modify
+ *     it under the terms of the GNU Affero General Public License as
+ *     published by the Free Software Foundation, either version 3 of the
+ *     License, or (at your option) any later version.
+ *
+ *     This program is distributed in the hope that it will be useful,
+ *     but WITHOUT ANY WARRANTY; without even the implied warranty of
+ *     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+ *     GNU Affero General Public License for more details.
+ *
+ *     You should have received a copy of the GNU Affero General Public License
+ *     along with this program.  If not, see <https://www.gnu.org/licenses/>.
+ */
+
+/*!
+ * Datetimepicker for Bootstrap 3
+ * version : 4.17.47
+ * https://github.com/Eonasdan/bootstrap-datetimepicker/
+ */
+.bootstrap-datetimepicker-widget {
+  list-style: none;
+}
+.bootstrap-datetimepicker-widget.dropdown-menu {
+  display: block;
+  margin: 2px 0;
+  padding: 4px;
+  width: 19em;
+}
+@media (min-width: 768px) {
+  .bootstrap-datetimepicker-widget.dropdown-menu.timepicker-sbs {
+    width: 38em;
+  }
+}
+@media (min-width: 992px) {
+  .bootstrap-datetimepicker-widget.dropdown-menu.timepicker-sbs {
+    width: 38em;
+  }
+}
+@media (min-width: 1200px) {
+  .bootstrap-datetimepicker-widget.dropdown-menu.timepicker-sbs {
+    width: 38em;
+  }
+}
+.bootstrap-datetimepicker-widget.dropdown-menu:before,
+.bootstrap-datetimepicker-widget.dropdown-menu:after {
+  content: '';
+  display: inline-block;
+  position: absolute;
+}
+.bootstrap-datetimepicker-widget.dropdown-menu.bottom:before {
+  border-left: 7px solid transparent;
+  border-right: 7px solid transparent;
+  border-bottom: 7px solid #ccc;
+  border-bottom-color: rgba(0, 0, 0, 0.2);
+  top: -7px;
+  left: 7px;
+}
+.bootstrap-datetimepicker-widget.dropdown-menu.bottom:after {
+  border-left: 6px solid transparent;
+  border-right: 6px solid transparent;
+  border-bottom: 6px solid white;
+  top: -6px;
+  left: 8px;
+}
+.bootstrap-datetimepicker-widget.dropdown-menu.top:before {
+  border-left: 7px solid transparent;
+  border-right: 7px solid transparent;
+  border-top: 7px solid #ccc;
+  border-top-color: rgba(0, 0, 0, 0.2);
+  bottom: -7px;
+  left: 6px;
+}
+.bootstrap-datetimepicker-widget.dropdown-menu.top:after {
+  border-left: 6px solid transparent;
+  border-right: 6px solid transparent;
+  border-top: 6px solid white;
+  bottom: -6px;
+  left: 7px;
+}
+.bootstrap-datetimepicker-widget.dropdown-menu.pull-right:before {
+  left: auto;
+  right: 6px;
+}
+.bootstrap-datetimepicker-widget.dropdown-menu.pull-right:after {
+  left: auto;
+  right: 7px;
+}
+.bootstrap-datetimepicker-widget .list-unstyled {
+  margin: 0;
+}
+.bootstrap-datetimepicker-widget a[data-action] {
+  padding: 6px 0;
+}
+.bootstrap-datetimepicker-widget a[data-action]:active {
+  box-shadow: none;
+}
+.bootstrap-datetimepicker-widget .timepicker-hour,
+.bootstrap-datetimepicker-widget .timepicker-minute,
+.bootstrap-datetimepicker-widget .timepicker-second {
+  width: 54px;
+  font-weight: bold;
+  font-size: 1.2em;
+  margin: 0;
+}
+.bootstrap-datetimepicker-widget button[data-action] {
+  padding: 6px;
+}
+.bootstrap-datetimepicker-widget .btn[data-action="incrementHours"]::after {
+  position: absolute;
+  width: 1px;
+  height: 1px;
+  margin: -1px;
+  padding: 0;
+  overflow: hidden;
+  clip: rect(0, 0, 0, 0);
+  border: 0;
+  content: "Increment Hours";
+}
+.bootstrap-datetimepicker-widget .btn[data-action="incrementMinutes"]::after {
+  position: absolute;
+  width: 1px;
+  height: 1px;
+  margin: -1px;
+  padding: 0;
+  overflow: hidden;
+  clip: rect(0, 0, 0, 0);
+  border: 0;
+  content: "Increment Minutes";
+}
+.bootstrap-datetimepicker-widget .btn[data-action="decrementHours"]::after {
+  position: absolute;
+  width: 1px;
+  height: 1px;
+  margin: -1px;
+  padding: 0;
+  overflow: hidden;
+  clip: rect(0, 0, 0, 0);
+  border: 0;
+  content: "Decrement Hours";
+}
+.bootstrap-datetimepicker-widget .btn[data-action="decrementMinutes"]::after {
+  position: absolute;
+  width: 1px;
+  height: 1px;
+  margin: -1px;
+  padding: 0;
+  overflow: hidden;
+  clip: rect(0, 0, 0, 0);
+  border: 0;
+  content: "Decrement Minutes";
+}
+.bootstrap-datetimepicker-widget .btn[data-action="showHours"]::after {
+  position: absolute;
+  width: 1px;
+  height: 1px;
+  margin: -1px;
+  padding: 0;
+  overflow: hidden;
+  clip: rect(0, 0, 0, 0);
+  border: 0;
+  content: "Show Hours";
+}
+.bootstrap-datetimepicker-widget .btn[data-action="showMinutes"]::after {
+  position: absolute;
+  width: 1px;
+  height: 1px;
+  margin: -1px;
+  padding: 0;
+  overflow: hidden;
+  clip: rect(0, 0, 0, 0);
+  border: 0;
+  content: "Show Minutes";
+}
+.bootstrap-datetimepicker-widget .btn[data-action="togglePeriod"]::after {
+  position: absolute;
+  width: 1px;
+  height: 1px;
+  margin: -1px;
+  padding: 0;
+  overflow: hidden;
+  clip: rect(0, 0, 0, 0);
+  border: 0;
+  content: "Toggle AM/PM";
+}
+.bootstrap-datetimepicker-widget .btn[data-action="clear"]::after {
+  position: absolute;
+  width: 1px;
+  height: 1px;
+  margin: -1px;
+  padding: 0;
+  overflow: hidden;
+  clip: rect(0, 0, 0, 0);
+  border: 0;
+  content: "Clear the picker";
+}
+.bootstrap-datetimepicker-widget .btn[data-action="today"]::after {
+  position: absolute;
+  width: 1px;
+  height: 1px;
+  margin: -1px;
+  padding: 0;
+  overflow: hidden;
+  clip: rect(0, 0, 0, 0);
+  border: 0;
+  content: "Set the date to today";
+}
+.bootstrap-datetimepicker-widget .picker-switch {
+  text-align: center;
+}
+.bootstrap-datetimepicker-widget .picker-switch::after {
+  position: absolute;
+  width: 1px;
+  height: 1px;
+  margin: -1px;
+  padding: 0;
+  overflow: hidden;
+  clip: rect(0, 0, 0, 0);
+  border: 0;
+  content: "Toggle Date and Time Screens";
+}
+.bootstrap-datetimepicker-widget .picker-switch td {
+  padding: 0;
+  margin: 0;
+  height: auto;
+  width: auto;
+  line-height: inherit;
+}
+.bootstrap-datetimepicker-widget .picker-switch td span {
+  line-height: 2.5;
+  height: 2.5em;
+  width: 100%;
+}
+.bootstrap-datetimepicker-widget table {
+  width: 100%;
+  margin: 0;
+}
+.bootstrap-datetimepicker-widget table td,
+.bootstrap-datetimepicker-widget table th {
+  text-align: center;
+  border-radius: 4px;
+}
+.bootstrap-datetimepicker-widget table th {
+  height: 20px;
+  line-height: 20px;
+  width: 20px;
+}
+.bootstrap-datetimepicker-widget table th.picker-switch {
+  width: 145px;
+}
+.bootstrap-datetimepicker-widget table th.disabled,
+.bootstrap-datetimepicker-widget table th.disabled:hover {
+  background: none;
+  color: #777777;
+  cursor: not-allowed;
+}
+.bootstrap-datetimepicker-widget table th.prev::after {
+  position: absolute;
+  width: 1px;
+  height: 1px;
+  margin: -1px;
+  padding: 0;
+  overflow: hidden;
+  clip: rect(0, 0, 0, 0);
+  border: 0;
+  content: "Previous Month";
+}
+.bootstrap-datetimepicker-widget table th.next::after {
+  position: absolute;
+  width: 1px;
+  height: 1px;
+  margin: -1px;
+  padding: 0;
+  overflow: hidden;
+  clip: rect(0, 0, 0, 0);
+  border: 0;
+  content: "Next Month";
+}
+.bootstrap-datetimepicker-widget table thead tr:first-child th {
+  cursor: pointer;
+}
+.bootstrap-datetimepicker-widget table thead tr:first-child th:hover {
+  background: #eeeeee;
+}
+.bootstrap-datetimepicker-widget table td {
+  height: 54px;
+  line-height: 54px;
+  width: 54px;
+}
+.bootstrap-datetimepicker-widget table td.cw {
+  font-size: .8em;
+  height: 20px;
+  line-height: 20px;
+  color: #777777;
+}
+.bootstrap-datetimepicker-widget table td.day {
+  height: 20px;
+  line-height: 20px;
+  width: 20px;
+}
+.bootstrap-datetimepicker-widget table td.day:hover,
+.bootstrap-datetimepicker-widget table td.hour:hover,
+.bootstrap-datetimepicker-widget table td.minute:hover,
+.bootstrap-datetimepicker-widget table td.second:hover {
+  background: #eeeeee;
+  cursor: pointer;
+}
+.bootstrap-datetimepicker-widget table td.old,
+.bootstrap-datetimepicker-widget table td.new {
+  color: #777777;
+}
+.bootstrap-datetimepicker-widget table td.today {
+  position: relative;
+}
+.bootstrap-datetimepicker-widget table td.today:before {
+  content: '';
+  display: inline-block;
+  border: solid transparent;
+  border-width: 0 0 7px 7px;
+  border-bottom-color: #337ab7;
+  border-top-color: rgba(0, 0, 0, 0.2);
+  position: absolute;
+  bottom: 4px;
+  right: 4px;
+}
+.bootstrap-datetimepicker-widget table td.active,
+.bootstrap-datetimepicker-widget table td.active:hover {
+  background-color: #337ab7;
+  color: #fff;
+  text-shadow: 0 -1px 0 rgba(0, 0, 0, 0.25);
+}
+.bootstrap-datetimepicker-widget table td.active.today:before {
+  border-bottom-color: #fff;
+}
+.bootstrap-datetimepicker-widget table td.disabled,
+.bootstrap-datetimepicker-widget table td.disabled:hover {
+  background: none;
+  color: #777777;
+  cursor: not-allowed;
+}
+.bootstrap-datetimepicker-widget table td span {
+  display: inline-block;
+  width: 54px;
+  height: 54px;
+  line-height: 54px;
+  margin: 2px 1.5px;
+  cursor: pointer;
+  border-radius: 4px;
+}
+.bootstrap-datetimepicker-widget table td span:hover {
+  background: #eeeeee;
+}
+.bootstrap-datetimepicker-widget table td span.active {
+  background-color: #337ab7;
+  color: #fff;
+  text-shadow: 0 -1px 0 rgba(0, 0, 0, 0.25);
+}
+.bootstrap-datetimepicker-widget table td span.old {
+  color: #777777;
+}
+.bootstrap-datetimepicker-widget table td span.disabled,
+.bootstrap-datetimepicker-widget table td span.disabled:hover {
+  background: none;
+  color: #777777;
+  cursor: not-allowed;
+}
+.bootstrap-datetimepicker-widget.usetwentyfour td.hour {
+  height: 27px;
+  line-height: 27px;
+}
+.bootstrap-datetimepicker-widget.wider {
+  width: 21em;
+}
+.bootstrap-datetimepicker-widget .datepicker-decades .decade {
+  line-height: 1.8em !important;
+}
+.input-group.date .input-group-addon {
+  cursor: pointer;
+}
+.sr-only {
+  position: absolute;
+  width: 1px;
+  height: 1px;
+  margin: -1px;
+  padding: 0;
+  overflow: hidden;
+  clip: rect(0, 0, 0, 0);
+  border: 0;
+}
```

### Comparing `nobinobi-core-0.1.4.6/nobinobi_core/static/css/bootstrap-datetimepicker.min.css` & `nobinobi-core-0.1.4.7/nobinobi_core/static/css/bootstrap-datetimepicker.min.css`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,5 +1,5 @@
-/*!
- * Datetimepicker for Bootstrap 3
- * version : 4.17.47
- * https://github.com/Eonasdan/bootstrap-datetimepicker/
+/*!
+ * Datetimepicker for Bootstrap 3
+ * version : 4.17.47
+ * https://github.com/Eonasdan/bootstrap-datetimepicker/
  */.bootstrap-datetimepicker-widget{list-style:none}.bootstrap-datetimepicker-widget.dropdown-menu{display:block;margin:2px 0;padding:4px;width:19em}@media (min-width:768px){.bootstrap-datetimepicker-widget.dropdown-menu.timepicker-sbs{width:38em}}@media (min-width:992px){.bootstrap-datetimepicker-widget.dropdown-menu.timepicker-sbs{width:38em}}@media (min-width:1200px){.bootstrap-datetimepicker-widget.dropdown-menu.timepicker-sbs{width:38em}}.bootstrap-datetimepicker-widget.dropdown-menu:before,.bootstrap-datetimepicker-widget.dropdown-menu:after{content:'';display:inline-block;position:absolute}.bootstrap-datetimepicker-widget.dropdown-menu.bottom:before{border-left:7px solid transparent;border-right:7px solid transparent;border-bottom:7px solid #ccc;border-bottom-color:rgba(0,0,0,0.2);top:-7px;left:7px}.bootstrap-datetimepicker-widget.dropdown-menu.bottom:after{border-left:6px solid transparent;border-right:6px solid transparent;border-bottom:6px solid white;top:-6px;left:8px}.bootstrap-datetimepicker-widget.dropdown-menu.top:before{border-left:7px solid transparent;border-right:7px solid transparent;border-top:7px solid #ccc;border-top-color:rgba(0,0,0,0.2);bottom:-7px;left:6px}.bootstrap-datetimepicker-widget.dropdown-menu.top:after{border-left:6px solid transparent;border-right:6px solid transparent;border-top:6px solid white;bottom:-6px;left:7px}.bootstrap-datetimepicker-widget.dropdown-menu.pull-right:before{left:auto;right:6px}.bootstrap-datetimepicker-widget.dropdown-menu.pull-right:after{left:auto;right:7px}.bootstrap-datetimepicker-widget .list-unstyled{margin:0}.bootstrap-datetimepicker-widget a[data-action]{padding:6px 0}.bootstrap-datetimepicker-widget a[data-action]:active{box-shadow:none}.bootstrap-datetimepicker-widget .timepicker-hour,.bootstrap-datetimepicker-widget .timepicker-minute,.bootstrap-datetimepicker-widget .timepicker-second{width:54px;font-weight:bold;font-size:1.2em;margin:0}.bootstrap-datetimepicker-widget button[data-action]{padding:6px}.bootstrap-datetimepicker-widget .btn[data-action="incrementHours"]::after{position:absolute;width:1px;height:1px;margin:-1px;padding:0;overflow:hidden;clip:rect(0, 0, 0, 0);border:0;content:"Increment Hours"}.bootstrap-datetimepicker-widget .btn[data-action="incrementMinutes"]::after{position:absolute;width:1px;height:1px;margin:-1px;padding:0;overflow:hidden;clip:rect(0, 0, 0, 0);border:0;content:"Increment Minutes"}.bootstrap-datetimepicker-widget .btn[data-action="decrementHours"]::after{position:absolute;width:1px;height:1px;margin:-1px;padding:0;overflow:hidden;clip:rect(0, 0, 0, 0);border:0;content:"Decrement Hours"}.bootstrap-datetimepicker-widget .btn[data-action="decrementMinutes"]::after{position:absolute;width:1px;height:1px;margin:-1px;padding:0;overflow:hidden;clip:rect(0, 0, 0, 0);border:0;content:"Decrement Minutes"}.bootstrap-datetimepicker-widget .btn[data-action="showHours"]::after{position:absolute;width:1px;height:1px;margin:-1px;padding:0;overflow:hidden;clip:rect(0, 0, 0, 0);border:0;content:"Show Hours"}.bootstrap-datetimepicker-widget .btn[data-action="showMinutes"]::after{position:absolute;width:1px;height:1px;margin:-1px;padding:0;overflow:hidden;clip:rect(0, 0, 0, 0);border:0;content:"Show Minutes"}.bootstrap-datetimepicker-widget .btn[data-action="togglePeriod"]::after{position:absolute;width:1px;height:1px;margin:-1px;padding:0;overflow:hidden;clip:rect(0, 0, 0, 0);border:0;content:"Toggle AM/PM"}.bootstrap-datetimepicker-widget .btn[data-action="clear"]::after{position:absolute;width:1px;height:1px;margin:-1px;padding:0;overflow:hidden;clip:rect(0, 0, 0, 0);border:0;content:"Clear the picker"}.bootstrap-datetimepicker-widget .btn[data-action="today"]::after{position:absolute;width:1px;height:1px;margin:-1px;padding:0;overflow:hidden;clip:rect(0, 0, 0, 0);border:0;content:"Set the date to today"}.bootstrap-datetimepicker-widget .picker-switch{text-align:center}.bootstrap-datetimepicker-widget .picker-switch::after{position:absolute;width:1px;height:1px;margin:-1px;padding:0;overflow:hidden;clip:rect(0, 0, 0, 0);border:0;content:"Toggle Date and Time Screens"}.bootstrap-datetimepicker-widget .picker-switch td{padding:0;margin:0;height:auto;width:auto;line-height:inherit}.bootstrap-datetimepicker-widget .picker-switch td span{line-height:2.5;height:2.5em;width:100%}.bootstrap-datetimepicker-widget table{width:100%;margin:0}.bootstrap-datetimepicker-widget table td,.bootstrap-datetimepicker-widget table th{text-align:center;border-radius:4px}.bootstrap-datetimepicker-widget table th{height:20px;line-height:20px;width:20px}.bootstrap-datetimepicker-widget table th.picker-switch{width:145px}.bootstrap-datetimepicker-widget table th.disabled,.bootstrap-datetimepicker-widget table th.disabled:hover{background:none;color:#777;cursor:not-allowed}.bootstrap-datetimepicker-widget table th.prev::after{position:absolute;width:1px;height:1px;margin:-1px;padding:0;overflow:hidden;clip:rect(0, 0, 0, 0);border:0;content:"Previous Month"}.bootstrap-datetimepicker-widget table th.next::after{position:absolute;width:1px;height:1px;margin:-1px;padding:0;overflow:hidden;clip:rect(0, 0, 0, 0);border:0;content:"Next Month"}.bootstrap-datetimepicker-widget table thead tr:first-child th{cursor:pointer}.bootstrap-datetimepicker-widget table thead tr:first-child th:hover{background:#eee}.bootstrap-datetimepicker-widget table td{height:54px;line-height:54px;width:54px}.bootstrap-datetimepicker-widget table td.cw{font-size:.8em;height:20px;line-height:20px;color:#777}.bootstrap-datetimepicker-widget table td.day{height:20px;line-height:20px;width:20px}.bootstrap-datetimepicker-widget table td.day:hover,.bootstrap-datetimepicker-widget table td.hour:hover,.bootstrap-datetimepicker-widget table td.minute:hover,.bootstrap-datetimepicker-widget table td.second:hover{background:#eee;cursor:pointer}.bootstrap-datetimepicker-widget table td.old,.bootstrap-datetimepicker-widget table td.new{color:#777}.bootstrap-datetimepicker-widget table td.today{position:relative}.bootstrap-datetimepicker-widget table td.today:before{content:'';display:inline-block;border:solid transparent;border-width:0 0 7px 7px;border-bottom-color:#337ab7;border-top-color:rgba(0,0,0,0.2);position:absolute;bottom:4px;right:4px}.bootstrap-datetimepicker-widget table td.active,.bootstrap-datetimepicker-widget table td.active:hover{background-color:#337ab7;color:#fff;text-shadow:0 -1px 0 rgba(0,0,0,0.25)}.bootstrap-datetimepicker-widget table td.active.today:before{border-bottom-color:#fff}.bootstrap-datetimepicker-widget table td.disabled,.bootstrap-datetimepicker-widget table td.disabled:hover{background:none;color:#777;cursor:not-allowed}.bootstrap-datetimepicker-widget table td span{display:inline-block;width:54px;height:54px;line-height:54px;margin:2px 1.5px;cursor:pointer;border-radius:4px}.bootstrap-datetimepicker-widget table td span:hover{background:#eee}.bootstrap-datetimepicker-widget table td span.active{background-color:#337ab7;color:#fff;text-shadow:0 -1px 0 rgba(0,0,0,0.25)}.bootstrap-datetimepicker-widget table td span.old{color:#777}.bootstrap-datetimepicker-widget table td span.disabled,.bootstrap-datetimepicker-widget table td span.disabled:hover{background:none;color:#777;cursor:not-allowed}.bootstrap-datetimepicker-widget.usetwentyfour td.hour{height:27px;line-height:27px}.bootstrap-datetimepicker-widget.wider{width:21em}.bootstrap-datetimepicker-widget .datepicker-decades .decade{line-height:1.8em !important}.input-group.date .input-group-addon{cursor:pointer}.sr-only{position:absolute;width:1px;height:1px;margin:-1px;padding:0;overflow:hidden;clip:rect(0, 0, 0, 0);border:0}
```

### Comparing `nobinobi-core-0.1.4.6/nobinobi_core/static/css/nobinobi_core.css` & `nobinobi-core-0.1.4.7/nobinobi_core/static/css/nobinobi_core.css`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.6/nobinobi_core/static/js/bootstrap-datetimepicker.min.js` & `nobinobi-core-0.1.4.7/nobinobi_core/static/js/bootstrap-datetimepicker.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,965 +1,965 @@
-! function(a) {
-    "use strict";
-    if ("function" == typeof define && define.amd) define(["jquery", "moment"], a);
-    else if ("object" == typeof exports) module.exports = a(require("jquery"), require("moment"));
-    else {
-        if ("undefined" == typeof jQuery) throw "bootstrap-datetimepicker requires jQuery to be loaded first";
-        if ("undefined" == typeof moment) throw "bootstrap-datetimepicker requires Moment.js to be loaded first";
-        a(jQuery, moment)
-    }
-}(function(a, b) {
-    "use strict";
-    if (!b) throw new Error("bootstrap-datetimepicker requires Moment.js to be loaded first");
-    var c = function(c, d) {
-        var e, f, g, h, i, j, k, l = {},
-            m = !0,
-            n = !1,
-            o = !1,
-            p = 0,
-            q = [{
-                clsName: "days",
-                navFnc: "M",
-                navStep: 1
-            }, {
-                clsName: "months",
-                navFnc: "y",
-                navStep: 1
-            }, {
-                clsName: "years",
-                navFnc: "y",
-                navStep: 10
-            }, {
-                clsName: "decades",
-                navFnc: "y",
-                navStep: 100
-            }],
-            r = ["days", "months", "years", "decades"],
-            s = ["top", "bottom", "auto"],
-            t = ["left", "right", "auto"],
-            u = ["default", "top", "bottom"],
-            v = {
-                up: 38,
-                38: "up",
-                down: 40,
-                40: "down",
-                left: 37,
-                37: "left",
-                right: 39,
-                39: "right",
-                tab: 9,
-                9: "tab",
-                escape: 27,
-                27: "escape",
-                enter: 13,
-                13: "enter",
-                pageUp: 33,
-                33: "pageUp",
-                pageDown: 34,
-                34: "pageDown",
-                shift: 16,
-                16: "shift",
-                control: 17,
-                17: "control",
-                space: 32,
-                32: "space",
-                t: 84,
-                84: "t",
-                delete: 46,
-                46: "delete"
-            },
-            w = {},
-            x = function() {
-                return void 0 !== b.tz && void 0 !== d.timeZone && null !== d.timeZone && "" !== d.timeZone
-            },
-            y = function(a) {
-                var c;
-                return c = void 0 === a || null === a ? b() : b.isDate(a) || b.isMoment(a) ? b(a) : x() ? b.tz(a, j, d.useStrict, d.timeZone) : b(a, j, d.useStrict), x() && c.tz(d.timeZone), c
-            },
-            z = function(a) {
-                if ("string" != typeof a || a.length > 1) throw new TypeError("isEnabled expects a single character string parameter");
-                switch (a) {
-                    case "y":
-                        return i.indexOf("Y") !== -1;
-                    case "M":
-                        return i.indexOf("M") !== -1;
-                    case "d":
-                        return i.toLowerCase().indexOf("d") !== -1;
-                    case "h":
-                    case "H":
-                        return i.toLowerCase().indexOf("h") !== -1;
-                    case "m":
-                        return i.indexOf("m") !== -1;
-                    case "s":
-                        return i.indexOf("s") !== -1;
-                    default:
-                        return !1
-                }
-            },
-            A = function() {
-                return z("h") || z("m") || z("s")
-            },
-            B = function() {
-                return z("y") || z("M") || z("d")
-            },
-            C = function() {
-                var b = a("<thead>").append(a("<tr>").append(a("<th>").addClass("prev").attr("data-action", "previous").append(a("<span>").addClass(d.icons.previous))).append(a("<th>").addClass("picker-switch").attr("data-action", "pickerSwitch").attr("colspan", d.calendarWeeks ? "6" : "5")).append(a("<th>").addClass("next").attr("data-action", "next").append(a("<span>").addClass(d.icons.next)))),
-                    c = a("<tbody>").append(a("<tr>").append(a("<td>").attr("colspan", d.calendarWeeks ? "8" : "7")));
-                return [a("<div>").addClass("datepicker-days").append(a("<table>").addClass("table-condensed").append(b).append(a("<tbody>"))), a("<div>").addClass("datepicker-months").append(a("<table>").addClass("table-condensed").append(b.clone()).append(c.clone())), a("<div>").addClass("datepicker-years").append(a("<table>").addClass("table-condensed").append(b.clone()).append(c.clone())), a("<div>").addClass("datepicker-decades").append(a("<table>").addClass("table-condensed").append(b.clone()).append(c.clone()))]
-            },
-            D = function() {
-                var b = a("<tr>"),
-                    c = a("<tr>"),
-                    e = a("<tr>");
-                return z("h") && (b.append(a("<td>").append(a("<a>").attr({
-                    href: "#",
-                    tabindex: "-1",
-                    title: d.tooltips.incrementHour
-                }).addClass("btn").attr("data-action", "incrementHours").append(a("<span>").addClass(d.icons.up)))), c.append(a("<td>").append(a("<span>").addClass("timepicker-hour").attr({
-                    "data-time-component": "hours",
-                    title: d.tooltips.pickHour
-                }).attr("data-action", "showHours"))), e.append(a("<td>").append(a("<a>").attr({
-                    href: "#",
-                    tabindex: "-1",
-                    title: d.tooltips.decrementHour
-                }).addClass("btn").attr("data-action", "decrementHours").append(a("<span>").addClass(d.icons.down))))), z("m") && (z("h") && (b.append(a("<td>").addClass("separator")), c.append(a("<td>").addClass("separator").html(":")), e.append(a("<td>").addClass("separator"))), b.append(a("<td>").append(a("<a>").attr({
-                    href: "#",
-                    tabindex: "-1",
-                    title: d.tooltips.incrementMinute
-                }).addClass("btn").attr("data-action", "incrementMinutes").append(a("<span>").addClass(d.icons.up)))), c.append(a("<td>").append(a("<span>").addClass("timepicker-minute").attr({
-                    "data-time-component": "minutes",
-                    title: d.tooltips.pickMinute
-                }).attr("data-action", "showMinutes"))), e.append(a("<td>").append(a("<a>").attr({
-                    href: "#",
-                    tabindex: "-1",
-                    title: d.tooltips.decrementMinute
-                }).addClass("btn").attr("data-action", "decrementMinutes").append(a("<span>").addClass(d.icons.down))))), z("s") && (z("m") && (b.append(a("<td>").addClass("separator")), c.append(a("<td>").addClass("separator").html(":")), e.append(a("<td>").addClass("separator"))), b.append(a("<td>").append(a("<a>").attr({
-                    href: "#",
-                    tabindex: "-1",
-                    title: d.tooltips.incrementSecond
-                }).addClass("btn").attr("data-action", "incrementSeconds").append(a("<span>").addClass(d.icons.up)))), c.append(a("<td>").append(a("<span>").addClass("timepicker-second").attr({
-                    "data-time-component": "seconds",
-                    title: d.tooltips.pickSecond
-                }).attr("data-action", "showSeconds"))), e.append(a("<td>").append(a("<a>").attr({
-                    href: "#",
-                    tabindex: "-1",
-                    title: d.tooltips.decrementSecond
-                }).addClass("btn").attr("data-action", "decrementSeconds").append(a("<span>").addClass(d.icons.down))))), h || (b.append(a("<td>").addClass("separator")), c.append(a("<td>").append(a("<button>").addClass("btn btn-primary").attr({
-                    "data-action": "togglePeriod",
-                    tabindex: "-1",
-                    title: d.tooltips.togglePeriod
-                }))), e.append(a("<td>").addClass("separator"))), a("<div>").addClass("timepicker-picker").append(a("<table>").addClass("table-condensed").append([b, c, e]))
-            },
-            E = function() {
-                var b = a("<div>").addClass("timepicker-hours").append(a("<table>").addClass("table-condensed")),
-                    c = a("<div>").addClass("timepicker-minutes").append(a("<table>").addClass("table-condensed")),
-                    d = a("<div>").addClass("timepicker-seconds").append(a("<table>").addClass("table-condensed")),
-                    e = [D()];
-                return z("h") && e.push(b), z("m") && e.push(c), z("s") && e.push(d), e
-            },
-            F = function() {
-                var b = [];
-                return d.showTodayButton && b.push(a("<td>").append(a("<a>").attr({
-                    "data-action": "today",
-                    title: d.tooltips.today
-                }).append(a("<span>").addClass(d.icons.today)))), !d.sideBySide && B() && A() && b.push(a("<td>").append(a("<a>").attr({
-                    "data-action": "togglePicker",
-                    title: d.tooltips.selectTime
-                }).append(a("<span>").addClass(d.icons.time)))), d.showClear && b.push(a("<td>").append(a("<a>").attr({
-                    "data-action": "clear",
-                    title: d.tooltips.clear
-                }).append(a("<span>").addClass(d.icons.clear)))), d.showClose && b.push(a("<td>").append(a("<a>").attr({
-                    "data-action": "close",
-                    title: d.tooltips.close
-                }).append(a("<span>").addClass(d.icons.close)))), a("<table>").addClass("table-condensed").append(a("<tbody>").append(a("<tr>").append(b)))
-            },
-            G = function() {
-                var b = a("<div>").addClass("bootstrap-datetimepicker-widget dropdown-menu"),
-                    c = a("<div>").addClass("datepicker").append(C()),
-                    e = a("<div>").addClass("timepicker").append(E()),
-                    f = a("<ul>").addClass("list-unstyled"),
-                    g = a("<li>").addClass("picker-switch" + (d.collapse ? " accordion-toggle" : "")).append(F());
-                return d.inline && b.removeClass("dropdown-menu"), h && b.addClass("usetwentyfour"), z("s") && !h && b.addClass("wider"), d.sideBySide && B() && A() ? (b.addClass("timepicker-sbs"), "top" === d.toolbarPlacement && b.append(g), b.append(a("<div>").addClass("row").append(c.addClass("col-md-6")).append(e.addClass("col-md-6"))), "bottom" === d.toolbarPlacement && b.append(g), b) : ("top" === d.toolbarPlacement && f.append(g), B() && f.append(a("<li>").addClass(d.collapse && A() ? "collapse in" : "").append(c)), "default" === d.toolbarPlacement && f.append(g), A() && f.append(a("<li>").addClass(d.collapse && B() ? "collapse" : "").append(e)), "bottom" === d.toolbarPlacement && f.append(g), b.append(f))
-            },
-            H = function() {
-                var b, e = {};
-                return b = c.is("input") || d.inline ? c.data() : c.find("input").data(), b.dateOptions && b.dateOptions instanceof Object && (e = a.extend(!0, e, b.dateOptions)), a.each(d, function(a) {
-                    var c = "date" + a.charAt(0).toUpperCase() + a.slice(1);
-                    void 0 !== b[c] && (e[a] = b[c])
-                }), e
-            },
-            I = function() {
-                var b, e = (n || c).position(),
-                    f = (n || c).offset(),
-                    g = d.widgetPositioning.vertical,
-                    h = d.widgetPositioning.horizontal;
-                if (d.widgetParent) b = d.widgetParent.append(o);
-                else if (c.is("input")) b = c.after(o).parent();
-                else {
-                    if (d.inline) return void(b = c.append(o));
-                    b = c, c.children().first().after(o)
-                }
-                if ("auto" === g && (g = f.top + 1.5 * o.height() >= a(window).height() + a(window).scrollTop() && o.height() + c.outerHeight() < f.top ? "top" : "bottom"), "auto" === h && (h = b.width() < f.left + o.outerWidth() / 2 && f.left + o.outerWidth() > a(window).width() ? "right" : "left"), "top" === g ? o.addClass("top").removeClass("bottom") : o.addClass("bottom").removeClass("top"), "right" === h ? o.addClass("pull-right") : o.removeClass("pull-right"), "static" === b.css("position") && (b = b.parents().filter(function() {
-                        return "static" !== a(this).css("position")
-                    }).first()), 0 === b.length) throw new Error("datetimepicker component should be placed within a non-static positioned container");
-                o.css({
-                    top: "top" === g ? "auto" : e.top + c.outerHeight(),
-                    bottom: "top" === g ? b.outerHeight() - (b === c ? 0 : e.top) : "auto",
-                    left: "left" === h ? b === c ? 0 : e.left : "auto",
-                    right: "left" === h ? "auto" : b.outerWidth() - c.outerWidth() - (b === c ? 0 : e.left)
-                })
-            },
-            J = function(a) {
-                "dp.change" === a.type && (a.date && a.date.isSame(a.oldDate) || !a.date && !a.oldDate) || c.trigger(a)
-            },
-            K = function(a) {
-                "y" === a && (a = "YYYY"), J({
-                    type: "dp.update",
-                    change: a,
-                    viewDate: f.clone()
-                })
-            },
-            L = function(a) {
-                o && (a && (k = Math.max(p, Math.min(3, k + a))), o.find(".datepicker > div").hide().filter(".datepicker-" + q[k].clsName).show())
-            },
-            M = function() {
-                var b = a("<tr>"),
-                    c = f.clone().startOf("w").startOf("d");
-                for (d.calendarWeeks === !0 && b.append(a("<th>").addClass("cw").text("#")); c.isBefore(f.clone().endOf("w"));) b.append(a("<th>").addClass("dow").text(c.format("dd"))), c.add(1, "d");
-                o.find(".datepicker-days thead").append(b)
-            },
-            N = function(a) {
-                return d.disabledDates[a.format("YYYY-MM-DD")] === !0
-            },
-            O = function(a) {
-                return d.enabledDates[a.format("YYYY-MM-DD")] === !0
-            },
-            P = function(a) {
-                return d.disabledHours[a.format("H")] === !0
-            },
-            Q = function(a) {
-                return d.enabledHours[a.format("H")] === !0
-            },
-            R = function(b, c) {
-                if (!b.isValid()) return !1;
-                if (d.disabledDates && "d" === c && N(b)) return !1;
-                if (d.enabledDates && "d" === c && !O(b)) return !1;
-                if (d.minDate && b.isBefore(d.minDate, c)) return !1;
-                if (d.maxDate && b.isAfter(d.maxDate, c)) return !1;
-                if (d.daysOfWeekDisabled && "d" === c && d.daysOfWeekDisabled.indexOf(b.day()) !== -1) return !1;
-                if (d.disabledHours && ("h" === c || "m" === c || "s" === c) && P(b)) return !1;
-                if (d.enabledHours && ("h" === c || "m" === c || "s" === c) && !Q(b)) return !1;
-                if (d.disabledTimeIntervals && ("h" === c || "m" === c || "s" === c)) {
-                    var e = !1;
-                    if (a.each(d.disabledTimeIntervals, function() {
-                            if (b.isBetween(this[0], this[1])) return e = !0, !1
-                        }), e) return !1
-                }
-                return !0
-            },
-            S = function() {
-                for (var b = [], c = f.clone().startOf("y").startOf("d"); c.isSame(f, "y");) b.push(a("<span>").attr("data-action", "selectMonth").addClass("month").text(c.format("MMM"))), c.add(1, "M");
-                o.find(".datepicker-months td").empty().append(b)
-            },
-            T = function() {
-                var b = o.find(".datepicker-months"),
-                    c = b.find("th"),
-                    g = b.find("tbody").find("span");
-                c.eq(0).find("span").attr("title", d.tooltips.prevYear), c.eq(1).attr("title", d.tooltips.selectYear), c.eq(2).find("span").attr("title", d.tooltips.nextYear), b.find(".disabled").removeClass("disabled"), R(f.clone().subtract(1, "y"), "y") || c.eq(0).addClass("disabled"), c.eq(1).text(f.year()), R(f.clone().add(1, "y"), "y") || c.eq(2).addClass("disabled"), g.removeClass("active"), e.isSame(f, "y") && !m && g.eq(e.month()).addClass("active"), g.each(function(b) {
-                    R(f.clone().month(b), "M") || a(this).addClass("disabled")
-                })
-            },
-            U = function() {
-                var a = o.find(".datepicker-years"),
-                    b = a.find("th"),
-                    c = f.clone().subtract(5, "y"),
-                    g = f.clone().add(6, "y"),
-                    h = "";
-                for (b.eq(0).find("span").attr("title", d.tooltips.prevDecade), b.eq(1).attr("title", d.tooltips.selectDecade), b.eq(2).find("span").attr("title", d.tooltips.nextDecade), a.find(".disabled").removeClass("disabled"), d.minDate && d.minDate.isAfter(c, "y") && b.eq(0).addClass("disabled"), b.eq(1).text(c.year() + "-" + g.year()), d.maxDate && d.maxDate.isBefore(g, "y") && b.eq(2).addClass("disabled"); !c.isAfter(g, "y");) h += '<span data-action="selectYear" class="year' + (c.isSame(e, "y") && !m ? " active" : "") + (R(c, "y") ? "" : " disabled") + '">' + c.year() + "</span>", c.add(1, "y");
-                a.find("td").html(h)
-            },
-            V = function() {
-                var a, c = o.find(".datepicker-decades"),
-                    g = c.find("th"),
-                    h = b({
-                        y: f.year() - f.year() % 100 - 1
-                    }),
-                    i = h.clone().add(100, "y"),
-                    j = h.clone(),
-                    k = !1,
-                    l = !1,
-                    m = "";
-                for (g.eq(0).find("span").attr("title", d.tooltips.prevCentury), g.eq(2).find("span").attr("title", d.tooltips.nextCentury), c.find(".disabled").removeClass("disabled"), (h.isSame(b({
-                        y: 1900
-                    })) || d.minDate && d.minDate.isAfter(h, "y")) && g.eq(0).addClass("disabled"), g.eq(1).text(h.year() + "-" + i.year()), (h.isSame(b({
-                        y: 2e3
-                    })) || d.maxDate && d.maxDate.isBefore(i, "y")) && g.eq(2).addClass("disabled"); !h.isAfter(i, "y");) a = h.year() + 12, k = d.minDate && d.minDate.isAfter(h, "y") && d.minDate.year() <= a, l = d.maxDate && d.maxDate.isAfter(h, "y") && d.maxDate.year() <= a, m += '<span data-action="selectDecade" class="decade' + (e.isAfter(h) && e.year() <= a ? " active" : "") + (R(h, "y") || k || l ? "" : " disabled") + '" data-selection="' + (h.year() + 6) + '">' + (h.year() + 1) + " - " + (h.year() + 12) + "</span>", h.add(12, "y");
-                m += "<span></span><span></span><span></span>", c.find("td").html(m), g.eq(1).text(j.year() + 1 + "-" + h.year())
-            },
-            W = function() {
-                var b, c, g, h = o.find(".datepicker-days"),
-                    i = h.find("th"),
-                    j = [],
-                    k = [];
-                if (B()) {
-                    for (i.eq(0).find("span").attr("title", d.tooltips.prevMonth), i.eq(1).attr("title", d.tooltips.selectMonth), i.eq(2).find("span").attr("title", d.tooltips.nextMonth), h.find(".disabled").removeClass("disabled"), i.eq(1).text(f.format(d.dayViewHeaderFormat)), R(f.clone().subtract(1, "M"), "M") || i.eq(0).addClass("disabled"), R(f.clone().add(1, "M"), "M") || i.eq(2).addClass("disabled"), b = f.clone().startOf("M").startOf("w").startOf("d"), g = 0; g < 42; g++) 0 === b.weekday() && (c = a("<tr>"), d.calendarWeeks && c.append('<td class="cw">' + b.week() + "</td>"), j.push(c)), k = ["day"], b.isBefore(f, "M") && k.push("old"), b.isAfter(f, "M") && k.push("new"), b.isSame(e, "d") && !m && k.push("active"), R(b, "d") || k.push("disabled"), b.isSame(y(), "d") && k.push("today"), 0 !== b.day() && 6 !== b.day() || k.push("weekend"), J({
-                        type: "dp.classify",
-                        date: b,
-                        classNames: k
-                    }), c.append('<td data-action="selectDay" data-day="' + b.format("L") + '" class="' + k.join(" ") + '">' + b.date() + "</td>"), b.add(1, "d");
-                    h.find("tbody").empty().append(j), T(), U(), V()
-                }
-            },
-            X = function() {
-                var b = o.find(".timepicker-hours table"),
-                    c = f.clone().startOf("d"),
-                    d = [],
-                    e = a("<tr>");
-                for (f.hour() > 11 && !h && c.hour(12); c.isSame(f, "d") && (h || f.hour() < 12 && c.hour() < 12 || f.hour() > 11);) c.hour() % 4 === 0 && (e = a("<tr>"), d.push(e)), e.append('<td data-action="selectHour" class="hour' + (R(c, "h") ? "" : " disabled") + '">' + c.format(h ? "HH" : "hh") + "</td>"), c.add(1, "h");
-                b.empty().append(d)
-            },
-            Y = function() {
-                for (var b = o.find(".timepicker-minutes table"), c = f.clone().startOf("h"), e = [], g = a("<tr>"), h = 1 === d.stepping ? 5 : d.stepping; f.isSame(c, "h");) c.minute() % (4 * h) === 0 && (g = a("<tr>"), e.push(g)), g.append('<td data-action="selectMinute" class="minute' + (R(c, "m") ? "" : " disabled") + '">' + c.format("mm") + "</td>"), c.add(h, "m");
-                b.empty().append(e)
-            },
-            Z = function() {
-                for (var b = o.find(".timepicker-seconds table"), c = f.clone().startOf("m"), d = [], e = a("<tr>"); f.isSame(c, "m");) c.second() % 20 === 0 && (e = a("<tr>"), d.push(e)), e.append('<td data-action="selectSecond" class="second' + (R(c, "s") ? "" : " disabled") + '">' + c.format("ss") + "</td>"), c.add(5, "s");
-                b.empty().append(d)
-            },
-            $ = function() {
-                var a, b, c = o.find(".timepicker span[data-time-component]");
-                h || (a = o.find(".timepicker [data-action=togglePeriod]"), b = e.clone().add(e.hours() >= 12 ? -12 : 12, "h"), a.text(e.format("A")), R(b, "h") ? a.removeClass("disabled") : a.addClass("disabled")), c.filter("[data-time-component=hours]").text(e.format(h ? "HH" : "hh")), c.filter("[data-time-component=minutes]").text(e.format("mm")), c.filter("[data-time-component=seconds]").text(e.format("ss")), X(), Y(), Z()
-            },
-            _ = function() {
-                o && (W(), $())
-            },
-            aa = function(a) {
-                var b = m ? null : e;
-                if (!a) return m = !0, g.val(""), c.data("date", ""), J({
-                    type: "dp.change",
-                    date: !1,
-                    oldDate: b
-                }), void _();
-                if (a = a.clone().locale(d.locale), x() && a.tz(d.timeZone), 1 !== d.stepping)
-                    for (a.minutes(Math.round(a.minutes() / d.stepping) * d.stepping).seconds(0); d.minDate && a.isBefore(d.minDate);) a.add(d.stepping, "minutes");
-                R(a) ? (e = a, f = e.clone(), g.val(e.format(i)), c.data("date", e.format(i)), m = !1, _(), J({
-                    type: "dp.change",
-                    date: e.clone(),
-                    oldDate: b
-                })) : (d.keepInvalid ? J({
-                    type: "dp.change",
-                    date: a,
-                    oldDate: b
-                }) : g.val(m ? "" : e.format(i)), J({
-                    type: "dp.error",
-                    date: a,
-                    oldDate: b
-                }))
-            },
-            ba = function() {
-                var b = !1;
-                return o ? (o.find(".collapse").each(function() {
-                    var c = a(this).data("collapse");
-                    return !c || !c.transitioning || (b = !0, !1)
-                }), b ? l : (n && n.hasClass("btn") && n.toggleClass("active"), o.hide(), a(window).off("resize", I), o.off("click", "[data-action]"), o.off("mousedown", !1), o.remove(), o = !1, J({
-                    type: "dp.hide",
-                    date: e.clone()
-                }), g.blur(), f = e.clone(), l)) : l
-            },
-            ca = function() {
-                aa(null)
-            },
-            da = function(a) {
-                return void 0 === d.parseInputDate ? (!b.isMoment(a) || a instanceof Date) && (a = y(a)) : a = d.parseInputDate(a), a
-            },
-            ea = {
-                next: function() {
-                    var a = q[k].navFnc;
-                    f.add(q[k].navStep, a), W(), K(a)
-                },
-                previous: function() {
-                    var a = q[k].navFnc;
-                    f.subtract(q[k].navStep, a), W(), K(a)
-                },
-                pickerSwitch: function() {
-                    L(1)
-                },
-                selectMonth: function(b) {
-                    var c = a(b.target).closest("tbody").find("span").index(a(b.target));
-                    f.month(c), k === p ? (aa(e.clone().year(f.year()).month(f.month())), d.inline || ba()) : (L(-1), W()), K("M")
-                },
-                selectYear: function(b) {
-                    var c = parseInt(a(b.target).text(), 10) || 0;
-                    f.year(c), k === p ? (aa(e.clone().year(f.year())), d.inline || ba()) : (L(-1), W()), K("YYYY")
-                },
-                selectDecade: function(b) {
-                    var c = parseInt(a(b.target).data("selection"), 10) || 0;
-                    f.year(c), k === p ? (aa(e.clone().year(f.year())), d.inline || ba()) : (L(-1), W()), K("YYYY")
-                },
-                selectDay: function(b) {
-                    var c = f.clone();
-                    a(b.target).is(".old") && c.subtract(1, "M"), a(b.target).is(".new") && c.add(1, "M"), aa(c.date(parseInt(a(b.target).text(), 10))), A() || d.keepOpen || d.inline || ba()
-                },
-                incrementHours: function() {
-                    var a = e.clone().add(1, "h");
-                    R(a, "h") && aa(a)
-                },
-                incrementMinutes: function() {
-                    var a = e.clone().add(d.stepping, "m");
-                    R(a, "m") && aa(a)
-                },
-                incrementSeconds: function() {
-                    var a = e.clone().add(1, "s");
-                    R(a, "s") && aa(a)
-                },
-                decrementHours: function() {
-                    var a = e.clone().subtract(1, "h");
-                    R(a, "h") && aa(a)
-                },
-                decrementMinutes: function() {
-                    var a = e.clone().subtract(d.stepping, "m");
-                    R(a, "m") && aa(a)
-                },
-                decrementSeconds: function() {
-                    var a = e.clone().subtract(1, "s");
-                    R(a, "s") && aa(a)
-                },
-                togglePeriod: function() {
-                    aa(e.clone().add(e.hours() >= 12 ? -12 : 12, "h"))
-                },
-                togglePicker: function(b) {
-                    var c, e = a(b.target),
-                        f = e.closest("ul"),
-                        g = f.find(".in"),
-                        h = f.find(".collapse:not(.in)");
-                    if (g && g.length) {
-                        if (c = g.data("collapse"), c && c.transitioning) return;
-                        g.collapse ? (g.collapse("hide"), h.collapse("show")) : (g.removeClass("in"), h.addClass("in")), e.is("span") ? e.toggleClass(d.icons.time + " " + d.icons.date) : e.find("span").toggleClass(d.icons.time + " " + d.icons.date)
-                    }
-                },
-                showPicker: function() {
-                    o.find(".timepicker > div:not(.timepicker-picker)").hide(), o.find(".timepicker .timepicker-picker").show()
-                },
-                showHours: function() {
-                    o.find(".timepicker .timepicker-picker").hide(), o.find(".timepicker .timepicker-hours").show()
-                },
-                showMinutes: function() {
-                    o.find(".timepicker .timepicker-picker").hide(), o.find(".timepicker .timepicker-minutes").show()
-                },
-                showSeconds: function() {
-                    o.find(".timepicker .timepicker-picker").hide(), o.find(".timepicker .timepicker-seconds").show()
-                },
-                selectHour: function(b) {
-                    var c = parseInt(a(b.target).text(), 10);
-                    h || (e.hours() >= 12 ? 12 !== c && (c += 12) : 12 === c && (c = 0)), aa(e.clone().hours(c)), ea.showPicker.call(l)
-                },
-                selectMinute: function(b) {
-                    aa(e.clone().minutes(parseInt(a(b.target).text(), 10))), ea.showPicker.call(l)
-                },
-                selectSecond: function(b) {
-                    aa(e.clone().seconds(parseInt(a(b.target).text(), 10))), ea.showPicker.call(l)
-                },
-                clear: ca,
-                today: function() {
-                    var a = y();
-                    R(a, "d") && aa(a)
-                },
-                close: ba
-            },
-            fa = function(b) {
-                return !a(b.currentTarget).is(".disabled") && (ea[a(b.currentTarget).data("action")].apply(l, arguments), !1)
-            },
-            ga = function() {
-                var b, c = {
-                    year: function(a) {
-                        return a.month(0).date(1).hours(0).seconds(0).minutes(0)
-                    },
-                    month: function(a) {
-                        return a.date(1).hours(0).seconds(0).minutes(0)
-                    },
-                    day: function(a) {
-                        return a.hours(0).seconds(0).minutes(0)
-                    },
-                    hour: function(a) {
-                        return a.seconds(0).minutes(0)
-                    },
-                    minute: function(a) {
-                        return a.seconds(0)
-                    }
-                };
-                return g.prop("disabled") || !d.ignoreReadonly && g.prop("readonly") || o ? l : (void 0 !== g.val() && 0 !== g.val().trim().length ? aa(da(g.val().trim())) : m && d.useCurrent && (d.inline || g.is("input") && 0 === g.val().trim().length) && (b = y(), "string" == typeof d.useCurrent && (b = c[d.useCurrent](b)), aa(b)), o = G(), M(), S(), o.find(".timepicker-hours").hide(), o.find(".timepicker-minutes").hide(), o.find(".timepicker-seconds").hide(), _(), L(), a(window).on("resize", I), o.on("click", "[data-action]", fa), o.on("mousedown", !1), n && n.hasClass("btn") && n.toggleClass("active"), I(), o.show(), d.focusOnShow && !g.is(":focus") && g.focus(), J({
-                    type: "dp.show"
-                }), l)
-            },
-            ha = function() {
-                return o ? ba() : ga()
-            },
-            ia = function(a) {
-                var b, c, e, f, g = null,
-                    h = [],
-                    i = {},
-                    j = a.which,
-                    k = "p";
-                w[j] = k;
-                for (b in w) w.hasOwnProperty(b) && w[b] === k && (h.push(b), parseInt(b, 10) !== j && (i[b] = !0));
-                for (b in d.keyBinds)
-                    if (d.keyBinds.hasOwnProperty(b) && "function" == typeof d.keyBinds[b] && (e = b.split(" "), e.length === h.length && v[j] === e[e.length - 1])) {
-                        for (f = !0, c = e.length - 2; c >= 0; c--)
-                            if (!(v[e[c]] in i)) {
-                                f = !1;
-                                break
-                            } if (f) {
-                            g = d.keyBinds[b];
-                            break
-                        }
-                    } g && (g.call(l, o), a.stopPropagation(), a.preventDefault())
-            },
-            ja = function(a) {
-                w[a.which] = "r", a.stopPropagation(), a.preventDefault()
-            },
-            ka = function(b) {
-                var c = a(b.target).val().trim(),
-                    d = c ? da(c) : null;
-                return aa(d), b.stopImmediatePropagation(), !1
-            },
-            la = function() {
-                g.on({
-                    change: ka,
-                    blur: d.debug ? "" : ba,
-                    keydown: ia,
-                    keyup: ja,
-                    focus: d.allowInputToggle ? ga : ""
-                }), c.is("input") ? g.on({
-                    focus: ga
-                }) : n && (n.on("click", ha), n.on("mousedown", !1))
-            },
-            ma = function() {
-                g.off({
-                    change: ka,
-                    blur: blur,
-                    keydown: ia,
-                    keyup: ja,
-                    focus: d.allowInputToggle ? ba : ""
-                }), c.is("input") ? g.off({
-                    focus: ga
-                }) : n && (n.off("click", ha), n.off("mousedown", !1))
-            },
-            na = function(b) {
-                var c = {};
-                return a.each(b, function() {
-                    var a = da(this);
-                    a.isValid() && (c[a.format("YYYY-MM-DD")] = !0)
-                }), !!Object.keys(c).length && c
-            },
-            oa = function(b) {
-                var c = {};
-                return a.each(b, function() {
-                    c[this] = !0
-                }), !!Object.keys(c).length && c
-            },
-            pa = function() {
-                var a = d.format || "L LT";
-                i = a.replace(/(\[[^\[]*\])|(\\)?(LTS|LT|LL?L?L?|l{1,4})/g, function(a) {
-                    var b = e.localeData().longDateFormat(a) || a;
-                    return b.replace(/(\[[^\[]*\])|(\\)?(LTS|LT|LL?L?L?|l{1,4})/g, function(a) {
-                        return e.localeData().longDateFormat(a) || a
-                    })
-                }), j = d.extraFormats ? d.extraFormats.slice() : [], j.indexOf(a) < 0 && j.indexOf(i) < 0 && j.push(i), h = i.toLowerCase().indexOf("a") < 1 && i.replace(/\[.*?\]/g, "").indexOf("h") < 1, z("y") && (p = 2), z("M") && (p = 1), z("d") && (p = 0), k = Math.max(p, k), m || aa(e)
-            };
-        if (l.destroy = function() {
-                ba(), ma(), c.removeData("DateTimePicker"), c.removeData("date")
-            }, l.toggle = ha, l.show = ga, l.hide = ba, l.disable = function() {
-                return ba(), n && n.hasClass("btn") && n.addClass("disabled"), g.prop("disabled", !0), l
-            }, l.enable = function() {
-                return n && n.hasClass("btn") && n.removeClass("disabled"), g.prop("disabled", !1), l
-            }, l.ignoreReadonly = function(a) {
-                if (0 === arguments.length) return d.ignoreReadonly;
-                if ("boolean" != typeof a) throw new TypeError("ignoreReadonly () expects a boolean parameter");
-                return d.ignoreReadonly = a, l
-            }, l.options = function(b) {
-                if (0 === arguments.length) return a.extend(!0, {}, d);
-                if (!(b instanceof Object)) throw new TypeError("options() options parameter should be an object");
-                return a.extend(!0, d, b), a.each(d, function(a, b) {
-                    if (void 0 === l[a]) throw new TypeError("option " + a + " is not recognized!");
-                    l[a](b)
-                }), l
-            }, l.date = function(a) {
-                if (0 === arguments.length) return m ? null : e.clone();
-                if (!(null === a || "string" == typeof a || b.isMoment(a) || a instanceof Date)) throw new TypeError("date() parameter must be one of [null, string, moment or Date]");
-                return aa(null === a ? null : da(a)), l
-            }, l.format = function(a) {
-                if (0 === arguments.length) return d.format;
-                if ("string" != typeof a && ("boolean" != typeof a || a !== !1)) throw new TypeError("format() expects a string or boolean:false parameter " + a);
-                return d.format = a, i && pa(), l
-            }, l.timeZone = function(a) {
-                if (0 === arguments.length) return d.timeZone;
-                if ("string" != typeof a) throw new TypeError("newZone() expects a string parameter");
-                return d.timeZone = a, l
-            }, l.dayViewHeaderFormat = function(a) {
-                if (0 === arguments.length) return d.dayViewHeaderFormat;
-                if ("string" != typeof a) throw new TypeError("dayViewHeaderFormat() expects a string parameter");
-                return d.dayViewHeaderFormat = a, l
-            }, l.extraFormats = function(a) {
-                if (0 === arguments.length) return d.extraFormats;
-                if (a !== !1 && !(a instanceof Array)) throw new TypeError("extraFormats() expects an array or false parameter");
-                return d.extraFormats = a, j && pa(), l
-            }, l.disabledDates = function(b) {
-                if (0 === arguments.length) return d.disabledDates ? a.extend({}, d.disabledDates) : d.disabledDates;
-                if (!b) return d.disabledDates = !1, _(), l;
-                if (!(b instanceof Array)) throw new TypeError("disabledDates() expects an array parameter");
-                return d.disabledDates = na(b), d.enabledDates = !1, _(), l
-            }, l.enabledDates = function(b) {
-                if (0 === arguments.length) return d.enabledDates ? a.extend({}, d.enabledDates) : d.enabledDates;
-                if (!b) return d.enabledDates = !1, _(), l;
-                if (!(b instanceof Array)) throw new TypeError("enabledDates() expects an array parameter");
-                return d.enabledDates = na(b), d.disabledDates = !1, _(), l
-            }, l.daysOfWeekDisabled = function(a) {
-                if (0 === arguments.length) return d.daysOfWeekDisabled.splice(0);
-                if ("boolean" == typeof a && !a) return d.daysOfWeekDisabled = !1, _(), l;
-                if (!(a instanceof Array)) throw new TypeError("daysOfWeekDisabled() expects an array parameter");
-                if (d.daysOfWeekDisabled = a.reduce(function(a, b) {
-                        return b = parseInt(b, 10), b > 6 || b < 0 || isNaN(b) ? a : (a.indexOf(b) === -1 && a.push(b), a)
-                    }, []).sort(), d.useCurrent && !d.keepInvalid) {
-                    for (var b = 0; !R(e, "d");) {
-                        if (e.add(1, "d"), 31 === b) throw "Tried 31 times to find a valid date";
-                        b++
-                    }
-                    aa(e)
-                }
-                return _(), l
-            }, l.maxDate = function(a) {
-                if (0 === arguments.length) return d.maxDate ? d.maxDate.clone() : d.maxDate;
-                if ("boolean" == typeof a && a === !1) return d.maxDate = !1, _(), l;
-                "string" == typeof a && ("now" !== a && "moment" !== a || (a = y()));
-                var b = da(a);
-                if (!b.isValid()) throw new TypeError("maxDate() Could not parse date parameter: " + a);
-                if (d.minDate && b.isBefore(d.minDate)) throw new TypeError("maxDate() date parameter is before options.minDate: " + b.format(i));
-                return d.maxDate = b, d.useCurrent && !d.keepInvalid && e.isAfter(a) && aa(d.maxDate), f.isAfter(b) && (f = b.clone().subtract(d.stepping, "m")), _(), l
-            }, l.minDate = function(a) {
-                if (0 === arguments.length) return d.minDate ? d.minDate.clone() : d.minDate;
-                if ("boolean" == typeof a && a === !1) return d.minDate = !1, _(), l;
-                "string" == typeof a && ("now" !== a && "moment" !== a || (a = y()));
-                var b = da(a);
-                if (!b.isValid()) throw new TypeError("minDate() Could not parse date parameter: " + a);
-                if (d.maxDate && b.isAfter(d.maxDate)) throw new TypeError("minDate() date parameter is after options.maxDate: " + b.format(i));
-                return d.minDate = b, d.useCurrent && !d.keepInvalid && e.isBefore(a) && aa(d.minDate), f.isBefore(b) && (f = b.clone().add(d.stepping, "m")), _(), l
-            }, l.defaultDate = function(a) {
-                if (0 === arguments.length) return d.defaultDate ? d.defaultDate.clone() : d.defaultDate;
-                if (!a) return d.defaultDate = !1, l;
-                "string" == typeof a && (a = "now" === a || "moment" === a ? y() : y(a));
-                var b = da(a);
-                if (!b.isValid()) throw new TypeError("defaultDate() Could not parse date parameter: " + a);
-                if (!R(b)) throw new TypeError("defaultDate() date passed is invalid according to component setup validations");
-                return d.defaultDate = b, (d.defaultDate && d.inline || "" === g.val().trim()) && aa(d.defaultDate), l
-            }, l.locale = function(a) {
-                if (0 === arguments.length) return d.locale;
-                if (!b.localeData(a)) throw new TypeError("locale() locale " + a + " is not loaded from moment locales!");
-                return d.locale = a, e.locale(d.locale), f.locale(d.locale), i && pa(), o && (ba(), ga()), l
-            }, l.stepping = function(a) {
-                return 0 === arguments.length ? d.stepping : (a = parseInt(a, 10), (isNaN(a) || a < 1) && (a = 1), d.stepping = a, l)
-            }, l.useCurrent = function(a) {
-                var b = ["year", "month", "day", "hour", "minute"];
-                if (0 === arguments.length) return d.useCurrent;
-                if ("boolean" != typeof a && "string" != typeof a) throw new TypeError("useCurrent() expects a boolean or string parameter");
-                if ("string" == typeof a && b.indexOf(a.toLowerCase()) === -1) throw new TypeError("useCurrent() expects a string parameter of " + b.join(", "));
-                return d.useCurrent = a, l
-            }, l.collapse = function(a) {
-                if (0 === arguments.length) return d.collapse;
-                if ("boolean" != typeof a) throw new TypeError("collapse() expects a boolean parameter");
-                return d.collapse === a ? l : (d.collapse = a, o && (ba(), ga()), l)
-            }, l.icons = function(b) {
-                if (0 === arguments.length) return a.extend({}, d.icons);
-                if (!(b instanceof Object)) throw new TypeError("icons() expects parameter to be an Object");
-                return a.extend(d.icons, b), o && (ba(), ga()), l
-            }, l.tooltips = function(b) {
-                if (0 === arguments.length) return a.extend({}, d.tooltips);
-                if (!(b instanceof Object)) throw new TypeError("tooltips() expects parameter to be an Object");
-                return a.extend(d.tooltips, b), o && (ba(), ga()), l
-            }, l.useStrict = function(a) {
-                if (0 === arguments.length) return d.useStrict;
-                if ("boolean" != typeof a) throw new TypeError("useStrict() expects a boolean parameter");
-                return d.useStrict = a, l
-            }, l.sideBySide = function(a) {
-                if (0 === arguments.length) return d.sideBySide;
-                if ("boolean" != typeof a) throw new TypeError("sideBySide() expects a boolean parameter");
-                return d.sideBySide = a, o && (ba(), ga()), l
-            }, l.viewMode = function(a) {
-                if (0 === arguments.length) return d.viewMode;
-                if ("string" != typeof a) throw new TypeError("viewMode() expects a string parameter");
-                if (r.indexOf(a) === -1) throw new TypeError("viewMode() parameter must be one of (" + r.join(", ") + ") value");
-                return d.viewMode = a, k = Math.max(r.indexOf(a), p), L(), l
-            }, l.toolbarPlacement = function(a) {
-                if (0 === arguments.length) return d.toolbarPlacement;
-                if ("string" != typeof a) throw new TypeError("toolbarPlacement() expects a string parameter");
-                if (u.indexOf(a) === -1) throw new TypeError("toolbarPlacement() parameter must be one of (" + u.join(", ") + ") value");
-                return d.toolbarPlacement = a, o && (ba(), ga()), l
-            }, l.widgetPositioning = function(b) {
-                if (0 === arguments.length) return a.extend({}, d.widgetPositioning);
-                if ("[object Object]" !== {}.toString.call(b)) throw new TypeError("widgetPositioning() expects an object variable");
-                if (b.horizontal) {
-                    if ("string" != typeof b.horizontal) throw new TypeError("widgetPositioning() horizontal variable must be a string");
-                    if (b.horizontal = b.horizontal.toLowerCase(), t.indexOf(b.horizontal) === -1) throw new TypeError("widgetPositioning() expects horizontal parameter to be one of (" + t.join(", ") + ")");
-                    d.widgetPositioning.horizontal = b.horizontal
-                }
-                if (b.vertical) {
-                    if ("string" != typeof b.vertical) throw new TypeError("widgetPositioning() vertical variable must be a string");
-                    if (b.vertical = b.vertical.toLowerCase(), s.indexOf(b.vertical) === -1) throw new TypeError("widgetPositioning() expects vertical parameter to be one of (" + s.join(", ") + ")");
-                    d.widgetPositioning.vertical = b.vertical
-                }
-                return _(), l
-            }, l.calendarWeeks = function(a) {
-                if (0 === arguments.length) return d.calendarWeeks;
-                if ("boolean" != typeof a) throw new TypeError("calendarWeeks() expects parameter to be a boolean value");
-                return d.calendarWeeks = a, _(), l
-            }, l.showTodayButton = function(a) {
-                if (0 === arguments.length) return d.showTodayButton;
-                if ("boolean" != typeof a) throw new TypeError("showTodayButton() expects a boolean parameter");
-                return d.showTodayButton = a, o && (ba(), ga()), l
-            }, l.showClear = function(a) {
-                if (0 === arguments.length) return d.showClear;
-                if ("boolean" != typeof a) throw new TypeError("showClear() expects a boolean parameter");
-                return d.showClear = a, o && (ba(), ga()), l
-            }, l.widgetParent = function(b) {
-                if (0 === arguments.length) return d.widgetParent;
-                if ("string" == typeof b && (b = a(b)), null !== b && "string" != typeof b && !(b instanceof a)) throw new TypeError("widgetParent() expects a string or a jQuery object parameter");
-                return d.widgetParent = b, o && (ba(), ga()), l
-            }, l.keepOpen = function(a) {
-                if (0 === arguments.length) return d.keepOpen;
-                if ("boolean" != typeof a) throw new TypeError("keepOpen() expects a boolean parameter");
-                return d.keepOpen = a, l
-            }, l.focusOnShow = function(a) {
-                if (0 === arguments.length) return d.focusOnShow;
-                if ("boolean" != typeof a) throw new TypeError("focusOnShow() expects a boolean parameter");
-                return d.focusOnShow = a, l
-            }, l.inline = function(a) {
-                if (0 === arguments.length) return d.inline;
-                if ("boolean" != typeof a) throw new TypeError("inline() expects a boolean parameter");
-                return d.inline = a, l
-            }, l.clear = function() {
-                return ca(), l
-            }, l.keyBinds = function(a) {
-                return 0 === arguments.length ? d.keyBinds : (d.keyBinds = a, l)
-            }, l.getMoment = function(a) {
-                return y(a)
-            }, l.debug = function(a) {
-                if ("boolean" != typeof a) throw new TypeError("debug() expects a boolean parameter");
-                return d.debug = a, l
-            }, l.allowInputToggle = function(a) {
-                if (0 === arguments.length) return d.allowInputToggle;
-                if ("boolean" != typeof a) throw new TypeError("allowInputToggle() expects a boolean parameter");
-                return d.allowInputToggle = a, l
-            }, l.showClose = function(a) {
-                if (0 === arguments.length) return d.showClose;
-                if ("boolean" != typeof a) throw new TypeError("showClose() expects a boolean parameter");
-                return d.showClose = a, l
-            }, l.keepInvalid = function(a) {
-                if (0 === arguments.length) return d.keepInvalid;
-                if ("boolean" != typeof a) throw new TypeError("keepInvalid() expects a boolean parameter");
-                return d.keepInvalid = a, l
-            }, l.datepickerInput = function(a) {
-                if (0 === arguments.length) return d.datepickerInput;
-                if ("string" != typeof a) throw new TypeError("datepickerInput() expects a string parameter");
-                return d.datepickerInput = a, l
-            }, l.parseInputDate = function(a) {
-                if (0 === arguments.length) return d.parseInputDate;
-                if ("function" != typeof a) throw new TypeError("parseInputDate() sholud be as function");
-                return d.parseInputDate = a, l
-            }, l.disabledTimeIntervals = function(b) {
-                if (0 === arguments.length) return d.disabledTimeIntervals ? a.extend({}, d.disabledTimeIntervals) : d.disabledTimeIntervals;
-                if (!b) return d.disabledTimeIntervals = !1, _(), l;
-                if (!(b instanceof Array)) throw new TypeError("disabledTimeIntervals() expects an array parameter");
-                return d.disabledTimeIntervals = b, _(), l
-            }, l.disabledHours = function(b) {
-                if (0 === arguments.length) return d.disabledHours ? a.extend({}, d.disabledHours) : d.disabledHours;
-                if (!b) return d.disabledHours = !1, _(), l;
-                if (!(b instanceof Array)) throw new TypeError("disabledHours() expects an array parameter");
-                if (d.disabledHours = oa(b), d.enabledHours = !1, d.useCurrent && !d.keepInvalid) {
-                    for (var c = 0; !R(e, "h");) {
-                        if (e.add(1, "h"), 24 === c) throw "Tried 24 times to find a valid date";
-                        c++
-                    }
-                    aa(e)
-                }
-                return _(), l
-            }, l.enabledHours = function(b) {
-                if (0 === arguments.length) return d.enabledHours ? a.extend({}, d.enabledHours) : d.enabledHours;
-                if (!b) return d.enabledHours = !1, _(), l;
-                if (!(b instanceof Array)) throw new TypeError("enabledHours() expects an array parameter");
-                if (d.enabledHours = oa(b), d.disabledHours = !1, d.useCurrent && !d.keepInvalid) {
-                    for (var c = 0; !R(e, "h");) {
-                        if (e.add(1, "h"), 24 === c) throw "Tried 24 times to find a valid date";
-                        c++
-                    }
-                    aa(e)
-                }
-                return _(), l
-            }, l.viewDate = function(a) {
-                if (0 === arguments.length) return f.clone();
-                if (!a) return f = e.clone(), l;
-                if (!("string" == typeof a || b.isMoment(a) || a instanceof Date)) throw new TypeError("viewDate() parameter must be one of [string, moment or Date]");
-                return f = da(a), K(), l
-            }, c.is("input")) g = c;
-        else if (g = c.find(d.datepickerInput), 0 === g.length) g = c.find("input");
-        else if (!g.is("input")) throw new Error('CSS class "' + d.datepickerInput + '" cannot be applied to non input element');
-        if (c.hasClass("input-group") && (n = 0 === c.find(".datepickerbutton").length ? c.find(".input-group-addon") : c.find(".datepickerbutton")), !d.inline && !g.is("input")) throw new Error("Could not initialize DateTimePicker without an input element");
-        return e = y(), f = e.clone(), a.extend(!0, d, H()), l.options(d), pa(), la(), g.prop("disabled") && l.disable(), g.is("input") && 0 !== g.val().trim().length ? aa(da(g.val().trim())) : d.defaultDate && void 0 === g.attr("placeholder") && aa(d.defaultDate), d.inline && ga(), l
-    };
-    return a.fn.datetimepicker = function(b) {
-        b = b || {};
-        var d, e = Array.prototype.slice.call(arguments, 1),
-            f = !0,
-            g = ["destroy", "hide", "show", "toggle"];
-        if ("object" == typeof b) return this.each(function() {
-            var d, e = a(this);
-            e.data("DateTimePicker") || (d = a.extend(!0, {}, a.fn.datetimepicker.defaults, b), e.data("DateTimePicker", c(e, d)))
-        });
-        if ("string" == typeof b) return this.each(function() {
-            var c = a(this),
-                g = c.data("DateTimePicker");
-            if (!g) throw new Error('bootstrap-datetimepicker("' + b + '") method was called on an element that is not using DateTimePicker');
-            d = g[b].apply(g, e), f = d === g
-        }), f || a.inArray(b, g) > -1 ? this : d;
-        throw new TypeError("Invalid arguments for DateTimePicker: " + b)
-    }, a.fn.datetimepicker.defaults = {
-        timeZone: "",
-        format: !1,
-        dayViewHeaderFormat: "MMMM YYYY",
-        extraFormats: !1,
-        stepping: 1,
-        minDate: !1,
-        maxDate: !1,
-        useCurrent: !0,
-        collapse: !0,
-        locale: b.locale(),
-        defaultDate: !1,
-        disabledDates: !1,
-        enabledDates: !1,
-        icons: {
-            time: "glyphicon glyphicon-time",
-            date: "glyphicon glyphicon-calendar",
-            up: "glyphicon glyphicon-chevron-up",
-            down: "glyphicon glyphicon-chevron-down",
-            previous: "glyphicon glyphicon-chevron-left",
-            next: "glyphicon glyphicon-chevron-right",
-            today: "glyphicon glyphicon-screenshot",
-            clear: "glyphicon glyphicon-trash",
-            close: "glyphicon glyphicon-remove"
-        },
-        tooltips: {
-            today: "Go to today",
-            clear: "Clear selection",
-            close: "Close the picker",
-            selectMonth: "Select Month",
-            prevMonth: "Previous Month",
-            nextMonth: "Next Month",
-            selectYear: "Select Year",
-            prevYear: "Previous Year",
-            nextYear: "Next Year",
-            selectDecade: "Select Decade",
-            prevDecade: "Previous Decade",
-            nextDecade: "Next Decade",
-            prevCentury: "Previous Century",
-            nextCentury: "Next Century",
-            pickHour: "Pick Hour",
-            incrementHour: "Increment Hour",
-            decrementHour: "Decrement Hour",
-            pickMinute: "Pick Minute",
-            incrementMinute: "Increment Minute",
-            decrementMinute: "Decrement Minute",
-            pickSecond: "Pick Second",
-            incrementSecond: "Increment Second",
-            decrementSecond: "Decrement Second",
-            togglePeriod: "Toggle Period",
-            selectTime: "Select Time"
-        },
-        useStrict: !1,
-        sideBySide: !1,
-        daysOfWeekDisabled: !1,
-        calendarWeeks: !1,
-        viewMode: "days",
-        toolbarPlacement: "default",
-        showTodayButton: !1,
-        showClear: !1,
-        showClose: !1,
-        widgetPositioning: {
-            horizontal: "auto",
-            vertical: "auto"
-        },
-        widgetParent: null,
-        ignoreReadonly: !1,
-        keepOpen: !1,
-        focusOnShow: !0,
-        inline: !1,
-        keepInvalid: !1,
-        datepickerInput: ".datepickerinput",
-        keyBinds: {
-            up: function(a) {
-                if (a) {
-                    var b = this.date() || this.getMoment();
-                    a.find(".datepicker").is(":visible") ? this.date(b.clone().subtract(7, "d")) : this.date(b.clone().add(this.stepping(), "m"))
-                }
-            },
-            down: function(a) {
-                if (!a) return void this.show();
-                var b = this.date() || this.getMoment();
-                a.find(".datepicker").is(":visible") ? this.date(b.clone().add(7, "d")) : this.date(b.clone().subtract(this.stepping(), "m"))
-            },
-            "control up": function(a) {
-                if (a) {
-                    var b = this.date() || this.getMoment();
-                    a.find(".datepicker").is(":visible") ? this.date(b.clone().subtract(1, "y")) : this.date(b.clone().add(1, "h"))
-                }
-            },
-            "control down": function(a) {
-                if (a) {
-                    var b = this.date() || this.getMoment();
-                    a.find(".datepicker").is(":visible") ? this.date(b.clone().add(1, "y")) : this.date(b.clone().subtract(1, "h"))
-                }
-            },
-            left: function(a) {
-                if (a) {
-                    var b = this.date() || this.getMoment();
-                    a.find(".datepicker").is(":visible") && this.date(b.clone().subtract(1, "d"))
-                }
-            },
-            right: function(a) {
-                if (a) {
-                    var b = this.date() || this.getMoment();
-                    a.find(".datepicker").is(":visible") && this.date(b.clone().add(1, "d"))
-                }
-            },
-            pageUp: function(a) {
-                if (a) {
-                    var b = this.date() || this.getMoment();
-                    a.find(".datepicker").is(":visible") && this.date(b.clone().subtract(1, "M"))
-                }
-            },
-            pageDown: function(a) {
-                if (a) {
-                    var b = this.date() || this.getMoment();
-                    a.find(".datepicker").is(":visible") && this.date(b.clone().add(1, "M"))
-                }
-            },
-            enter: function() {
-                this.hide()
-            },
-            escape: function() {
-                this.hide()
-            },
-            "control space": function(a) {
-                a && a.find(".timepicker").is(":visible") && a.find('.btn[data-action="togglePeriod"]').click()
-            },
-            t: function() {
-                this.date(this.getMoment())
-            },
-            delete: function() {
-                this.clear()
-            }
-        },
-        debug: !1,
-        allowInputToggle: !1,
-        disabledTimeIntervals: !1,
-        disabledHours: !1,
-        enabledHours: !1,
-        viewDate: !1
-    }, a.fn.datetimepicker
+! function(a) {
+    "use strict";
+    if ("function" == typeof define && define.amd) define(["jquery", "moment"], a);
+    else if ("object" == typeof exports) module.exports = a(require("jquery"), require("moment"));
+    else {
+        if ("undefined" == typeof jQuery) throw "bootstrap-datetimepicker requires jQuery to be loaded first";
+        if ("undefined" == typeof moment) throw "bootstrap-datetimepicker requires Moment.js to be loaded first";
+        a(jQuery, moment)
+    }
+}(function(a, b) {
+    "use strict";
+    if (!b) throw new Error("bootstrap-datetimepicker requires Moment.js to be loaded first");
+    var c = function(c, d) {
+        var e, f, g, h, i, j, k, l = {},
+            m = !0,
+            n = !1,
+            o = !1,
+            p = 0,
+            q = [{
+                clsName: "days",
+                navFnc: "M",
+                navStep: 1
+            }, {
+                clsName: "months",
+                navFnc: "y",
+                navStep: 1
+            }, {
+                clsName: "years",
+                navFnc: "y",
+                navStep: 10
+            }, {
+                clsName: "decades",
+                navFnc: "y",
+                navStep: 100
+            }],
+            r = ["days", "months", "years", "decades"],
+            s = ["top", "bottom", "auto"],
+            t = ["left", "right", "auto"],
+            u = ["default", "top", "bottom"],
+            v = {
+                up: 38,
+                38: "up",
+                down: 40,
+                40: "down",
+                left: 37,
+                37: "left",
+                right: 39,
+                39: "right",
+                tab: 9,
+                9: "tab",
+                escape: 27,
+                27: "escape",
+                enter: 13,
+                13: "enter",
+                pageUp: 33,
+                33: "pageUp",
+                pageDown: 34,
+                34: "pageDown",
+                shift: 16,
+                16: "shift",
+                control: 17,
+                17: "control",
+                space: 32,
+                32: "space",
+                t: 84,
+                84: "t",
+                delete: 46,
+                46: "delete"
+            },
+            w = {},
+            x = function() {
+                return void 0 !== b.tz && void 0 !== d.timeZone && null !== d.timeZone && "" !== d.timeZone
+            },
+            y = function(a) {
+                var c;
+                return c = void 0 === a || null === a ? b() : b.isDate(a) || b.isMoment(a) ? b(a) : x() ? b.tz(a, j, d.useStrict, d.timeZone) : b(a, j, d.useStrict), x() && c.tz(d.timeZone), c
+            },
+            z = function(a) {
+                if ("string" != typeof a || a.length > 1) throw new TypeError("isEnabled expects a single character string parameter");
+                switch (a) {
+                    case "y":
+                        return i.indexOf("Y") !== -1;
+                    case "M":
+                        return i.indexOf("M") !== -1;
+                    case "d":
+                        return i.toLowerCase().indexOf("d") !== -1;
+                    case "h":
+                    case "H":
+                        return i.toLowerCase().indexOf("h") !== -1;
+                    case "m":
+                        return i.indexOf("m") !== -1;
+                    case "s":
+                        return i.indexOf("s") !== -1;
+                    default:
+                        return !1
+                }
+            },
+            A = function() {
+                return z("h") || z("m") || z("s")
+            },
+            B = function() {
+                return z("y") || z("M") || z("d")
+            },
+            C = function() {
+                var b = a("<thead>").append(a("<tr>").append(a("<th>").addClass("prev").attr("data-action", "previous").append(a("<span>").addClass(d.icons.previous))).append(a("<th>").addClass("picker-switch").attr("data-action", "pickerSwitch").attr("colspan", d.calendarWeeks ? "6" : "5")).append(a("<th>").addClass("next").attr("data-action", "next").append(a("<span>").addClass(d.icons.next)))),
+                    c = a("<tbody>").append(a("<tr>").append(a("<td>").attr("colspan", d.calendarWeeks ? "8" : "7")));
+                return [a("<div>").addClass("datepicker-days").append(a("<table>").addClass("table-condensed").append(b).append(a("<tbody>"))), a("<div>").addClass("datepicker-months").append(a("<table>").addClass("table-condensed").append(b.clone()).append(c.clone())), a("<div>").addClass("datepicker-years").append(a("<table>").addClass("table-condensed").append(b.clone()).append(c.clone())), a("<div>").addClass("datepicker-decades").append(a("<table>").addClass("table-condensed").append(b.clone()).append(c.clone()))]
+            },
+            D = function() {
+                var b = a("<tr>"),
+                    c = a("<tr>"),
+                    e = a("<tr>");
+                return z("h") && (b.append(a("<td>").append(a("<a>").attr({
+                    href: "#",
+                    tabindex: "-1",
+                    title: d.tooltips.incrementHour
+                }).addClass("btn").attr("data-action", "incrementHours").append(a("<span>").addClass(d.icons.up)))), c.append(a("<td>").append(a("<span>").addClass("timepicker-hour").attr({
+                    "data-time-component": "hours",
+                    title: d.tooltips.pickHour
+                }).attr("data-action", "showHours"))), e.append(a("<td>").append(a("<a>").attr({
+                    href: "#",
+                    tabindex: "-1",
+                    title: d.tooltips.decrementHour
+                }).addClass("btn").attr("data-action", "decrementHours").append(a("<span>").addClass(d.icons.down))))), z("m") && (z("h") && (b.append(a("<td>").addClass("separator")), c.append(a("<td>").addClass("separator").html(":")), e.append(a("<td>").addClass("separator"))), b.append(a("<td>").append(a("<a>").attr({
+                    href: "#",
+                    tabindex: "-1",
+                    title: d.tooltips.incrementMinute
+                }).addClass("btn").attr("data-action", "incrementMinutes").append(a("<span>").addClass(d.icons.up)))), c.append(a("<td>").append(a("<span>").addClass("timepicker-minute").attr({
+                    "data-time-component": "minutes",
+                    title: d.tooltips.pickMinute
+                }).attr("data-action", "showMinutes"))), e.append(a("<td>").append(a("<a>").attr({
+                    href: "#",
+                    tabindex: "-1",
+                    title: d.tooltips.decrementMinute
+                }).addClass("btn").attr("data-action", "decrementMinutes").append(a("<span>").addClass(d.icons.down))))), z("s") && (z("m") && (b.append(a("<td>").addClass("separator")), c.append(a("<td>").addClass("separator").html(":")), e.append(a("<td>").addClass("separator"))), b.append(a("<td>").append(a("<a>").attr({
+                    href: "#",
+                    tabindex: "-1",
+                    title: d.tooltips.incrementSecond
+                }).addClass("btn").attr("data-action", "incrementSeconds").append(a("<span>").addClass(d.icons.up)))), c.append(a("<td>").append(a("<span>").addClass("timepicker-second").attr({
+                    "data-time-component": "seconds",
+                    title: d.tooltips.pickSecond
+                }).attr("data-action", "showSeconds"))), e.append(a("<td>").append(a("<a>").attr({
+                    href: "#",
+                    tabindex: "-1",
+                    title: d.tooltips.decrementSecond
+                }).addClass("btn").attr("data-action", "decrementSeconds").append(a("<span>").addClass(d.icons.down))))), h || (b.append(a("<td>").addClass("separator")), c.append(a("<td>").append(a("<button>").addClass("btn btn-primary").attr({
+                    "data-action": "togglePeriod",
+                    tabindex: "-1",
+                    title: d.tooltips.togglePeriod
+                }))), e.append(a("<td>").addClass("separator"))), a("<div>").addClass("timepicker-picker").append(a("<table>").addClass("table-condensed").append([b, c, e]))
+            },
+            E = function() {
+                var b = a("<div>").addClass("timepicker-hours").append(a("<table>").addClass("table-condensed")),
+                    c = a("<div>").addClass("timepicker-minutes").append(a("<table>").addClass("table-condensed")),
+                    d = a("<div>").addClass("timepicker-seconds").append(a("<table>").addClass("table-condensed")),
+                    e = [D()];
+                return z("h") && e.push(b), z("m") && e.push(c), z("s") && e.push(d), e
+            },
+            F = function() {
+                var b = [];
+                return d.showTodayButton && b.push(a("<td>").append(a("<a>").attr({
+                    "data-action": "today",
+                    title: d.tooltips.today
+                }).append(a("<span>").addClass(d.icons.today)))), !d.sideBySide && B() && A() && b.push(a("<td>").append(a("<a>").attr({
+                    "data-action": "togglePicker",
+                    title: d.tooltips.selectTime
+                }).append(a("<span>").addClass(d.icons.time)))), d.showClear && b.push(a("<td>").append(a("<a>").attr({
+                    "data-action": "clear",
+                    title: d.tooltips.clear
+                }).append(a("<span>").addClass(d.icons.clear)))), d.showClose && b.push(a("<td>").append(a("<a>").attr({
+                    "data-action": "close",
+                    title: d.tooltips.close
+                }).append(a("<span>").addClass(d.icons.close)))), a("<table>").addClass("table-condensed").append(a("<tbody>").append(a("<tr>").append(b)))
+            },
+            G = function() {
+                var b = a("<div>").addClass("bootstrap-datetimepicker-widget dropdown-menu"),
+                    c = a("<div>").addClass("datepicker").append(C()),
+                    e = a("<div>").addClass("timepicker").append(E()),
+                    f = a("<ul>").addClass("list-unstyled"),
+                    g = a("<li>").addClass("picker-switch" + (d.collapse ? " accordion-toggle" : "")).append(F());
+                return d.inline && b.removeClass("dropdown-menu"), h && b.addClass("usetwentyfour"), z("s") && !h && b.addClass("wider"), d.sideBySide && B() && A() ? (b.addClass("timepicker-sbs"), "top" === d.toolbarPlacement && b.append(g), b.append(a("<div>").addClass("row").append(c.addClass("col-md-6")).append(e.addClass("col-md-6"))), "bottom" === d.toolbarPlacement && b.append(g), b) : ("top" === d.toolbarPlacement && f.append(g), B() && f.append(a("<li>").addClass(d.collapse && A() ? "collapse in" : "").append(c)), "default" === d.toolbarPlacement && f.append(g), A() && f.append(a("<li>").addClass(d.collapse && B() ? "collapse" : "").append(e)), "bottom" === d.toolbarPlacement && f.append(g), b.append(f))
+            },
+            H = function() {
+                var b, e = {};
+                return b = c.is("input") || d.inline ? c.data() : c.find("input").data(), b.dateOptions && b.dateOptions instanceof Object && (e = a.extend(!0, e, b.dateOptions)), a.each(d, function(a) {
+                    var c = "date" + a.charAt(0).toUpperCase() + a.slice(1);
+                    void 0 !== b[c] && (e[a] = b[c])
+                }), e
+            },
+            I = function() {
+                var b, e = (n || c).position(),
+                    f = (n || c).offset(),
+                    g = d.widgetPositioning.vertical,
+                    h = d.widgetPositioning.horizontal;
+                if (d.widgetParent) b = d.widgetParent.append(o);
+                else if (c.is("input")) b = c.after(o).parent();
+                else {
+                    if (d.inline) return void(b = c.append(o));
+                    b = c, c.children().first().after(o)
+                }
+                if ("auto" === g && (g = f.top + 1.5 * o.height() >= a(window).height() + a(window).scrollTop() && o.height() + c.outerHeight() < f.top ? "top" : "bottom"), "auto" === h && (h = b.width() < f.left + o.outerWidth() / 2 && f.left + o.outerWidth() > a(window).width() ? "right" : "left"), "top" === g ? o.addClass("top").removeClass("bottom") : o.addClass("bottom").removeClass("top"), "right" === h ? o.addClass("pull-right") : o.removeClass("pull-right"), "static" === b.css("position") && (b = b.parents().filter(function() {
+                        return "static" !== a(this).css("position")
+                    }).first()), 0 === b.length) throw new Error("datetimepicker component should be placed within a non-static positioned container");
+                o.css({
+                    top: "top" === g ? "auto" : e.top + c.outerHeight(),
+                    bottom: "top" === g ? b.outerHeight() - (b === c ? 0 : e.top) : "auto",
+                    left: "left" === h ? b === c ? 0 : e.left : "auto",
+                    right: "left" === h ? "auto" : b.outerWidth() - c.outerWidth() - (b === c ? 0 : e.left)
+                })
+            },
+            J = function(a) {
+                "dp.change" === a.type && (a.date && a.date.isSame(a.oldDate) || !a.date && !a.oldDate) || c.trigger(a)
+            },
+            K = function(a) {
+                "y" === a && (a = "YYYY"), J({
+                    type: "dp.update",
+                    change: a,
+                    viewDate: f.clone()
+                })
+            },
+            L = function(a) {
+                o && (a && (k = Math.max(p, Math.min(3, k + a))), o.find(".datepicker > div").hide().filter(".datepicker-" + q[k].clsName).show())
+            },
+            M = function() {
+                var b = a("<tr>"),
+                    c = f.clone().startOf("w").startOf("d");
+                for (d.calendarWeeks === !0 && b.append(a("<th>").addClass("cw").text("#")); c.isBefore(f.clone().endOf("w"));) b.append(a("<th>").addClass("dow").text(c.format("dd"))), c.add(1, "d");
+                o.find(".datepicker-days thead").append(b)
+            },
+            N = function(a) {
+                return d.disabledDates[a.format("YYYY-MM-DD")] === !0
+            },
+            O = function(a) {
+                return d.enabledDates[a.format("YYYY-MM-DD")] === !0
+            },
+            P = function(a) {
+                return d.disabledHours[a.format("H")] === !0
+            },
+            Q = function(a) {
+                return d.enabledHours[a.format("H")] === !0
+            },
+            R = function(b, c) {
+                if (!b.isValid()) return !1;
+                if (d.disabledDates && "d" === c && N(b)) return !1;
+                if (d.enabledDates && "d" === c && !O(b)) return !1;
+                if (d.minDate && b.isBefore(d.minDate, c)) return !1;
+                if (d.maxDate && b.isAfter(d.maxDate, c)) return !1;
+                if (d.daysOfWeekDisabled && "d" === c && d.daysOfWeekDisabled.indexOf(b.day()) !== -1) return !1;
+                if (d.disabledHours && ("h" === c || "m" === c || "s" === c) && P(b)) return !1;
+                if (d.enabledHours && ("h" === c || "m" === c || "s" === c) && !Q(b)) return !1;
+                if (d.disabledTimeIntervals && ("h" === c || "m" === c || "s" === c)) {
+                    var e = !1;
+                    if (a.each(d.disabledTimeIntervals, function() {
+                            if (b.isBetween(this[0], this[1])) return e = !0, !1
+                        }), e) return !1
+                }
+                return !0
+            },
+            S = function() {
+                for (var b = [], c = f.clone().startOf("y").startOf("d"); c.isSame(f, "y");) b.push(a("<span>").attr("data-action", "selectMonth").addClass("month").text(c.format("MMM"))), c.add(1, "M");
+                o.find(".datepicker-months td").empty().append(b)
+            },
+            T = function() {
+                var b = o.find(".datepicker-months"),
+                    c = b.find("th"),
+                    g = b.find("tbody").find("span");
+                c.eq(0).find("span").attr("title", d.tooltips.prevYear), c.eq(1).attr("title", d.tooltips.selectYear), c.eq(2).find("span").attr("title", d.tooltips.nextYear), b.find(".disabled").removeClass("disabled"), R(f.clone().subtract(1, "y"), "y") || c.eq(0).addClass("disabled"), c.eq(1).text(f.year()), R(f.clone().add(1, "y"), "y") || c.eq(2).addClass("disabled"), g.removeClass("active"), e.isSame(f, "y") && !m && g.eq(e.month()).addClass("active"), g.each(function(b) {
+                    R(f.clone().month(b), "M") || a(this).addClass("disabled")
+                })
+            },
+            U = function() {
+                var a = o.find(".datepicker-years"),
+                    b = a.find("th"),
+                    c = f.clone().subtract(5, "y"),
+                    g = f.clone().add(6, "y"),
+                    h = "";
+                for (b.eq(0).find("span").attr("title", d.tooltips.prevDecade), b.eq(1).attr("title", d.tooltips.selectDecade), b.eq(2).find("span").attr("title", d.tooltips.nextDecade), a.find(".disabled").removeClass("disabled"), d.minDate && d.minDate.isAfter(c, "y") && b.eq(0).addClass("disabled"), b.eq(1).text(c.year() + "-" + g.year()), d.maxDate && d.maxDate.isBefore(g, "y") && b.eq(2).addClass("disabled"); !c.isAfter(g, "y");) h += '<span data-action="selectYear" class="year' + (c.isSame(e, "y") && !m ? " active" : "") + (R(c, "y") ? "" : " disabled") + '">' + c.year() + "</span>", c.add(1, "y");
+                a.find("td").html(h)
+            },
+            V = function() {
+                var a, c = o.find(".datepicker-decades"),
+                    g = c.find("th"),
+                    h = b({
+                        y: f.year() - f.year() % 100 - 1
+                    }),
+                    i = h.clone().add(100, "y"),
+                    j = h.clone(),
+                    k = !1,
+                    l = !1,
+                    m = "";
+                for (g.eq(0).find("span").attr("title", d.tooltips.prevCentury), g.eq(2).find("span").attr("title", d.tooltips.nextCentury), c.find(".disabled").removeClass("disabled"), (h.isSame(b({
+                        y: 1900
+                    })) || d.minDate && d.minDate.isAfter(h, "y")) && g.eq(0).addClass("disabled"), g.eq(1).text(h.year() + "-" + i.year()), (h.isSame(b({
+                        y: 2e3
+                    })) || d.maxDate && d.maxDate.isBefore(i, "y")) && g.eq(2).addClass("disabled"); !h.isAfter(i, "y");) a = h.year() + 12, k = d.minDate && d.minDate.isAfter(h, "y") && d.minDate.year() <= a, l = d.maxDate && d.maxDate.isAfter(h, "y") && d.maxDate.year() <= a, m += '<span data-action="selectDecade" class="decade' + (e.isAfter(h) && e.year() <= a ? " active" : "") + (R(h, "y") || k || l ? "" : " disabled") + '" data-selection="' + (h.year() + 6) + '">' + (h.year() + 1) + " - " + (h.year() + 12) + "</span>", h.add(12, "y");
+                m += "<span></span><span></span><span></span>", c.find("td").html(m), g.eq(1).text(j.year() + 1 + "-" + h.year())
+            },
+            W = function() {
+                var b, c, g, h = o.find(".datepicker-days"),
+                    i = h.find("th"),
+                    j = [],
+                    k = [];
+                if (B()) {
+                    for (i.eq(0).find("span").attr("title", d.tooltips.prevMonth), i.eq(1).attr("title", d.tooltips.selectMonth), i.eq(2).find("span").attr("title", d.tooltips.nextMonth), h.find(".disabled").removeClass("disabled"), i.eq(1).text(f.format(d.dayViewHeaderFormat)), R(f.clone().subtract(1, "M"), "M") || i.eq(0).addClass("disabled"), R(f.clone().add(1, "M"), "M") || i.eq(2).addClass("disabled"), b = f.clone().startOf("M").startOf("w").startOf("d"), g = 0; g < 42; g++) 0 === b.weekday() && (c = a("<tr>"), d.calendarWeeks && c.append('<td class="cw">' + b.week() + "</td>"), j.push(c)), k = ["day"], b.isBefore(f, "M") && k.push("old"), b.isAfter(f, "M") && k.push("new"), b.isSame(e, "d") && !m && k.push("active"), R(b, "d") || k.push("disabled"), b.isSame(y(), "d") && k.push("today"), 0 !== b.day() && 6 !== b.day() || k.push("weekend"), J({
+                        type: "dp.classify",
+                        date: b,
+                        classNames: k
+                    }), c.append('<td data-action="selectDay" data-day="' + b.format("L") + '" class="' + k.join(" ") + '">' + b.date() + "</td>"), b.add(1, "d");
+                    h.find("tbody").empty().append(j), T(), U(), V()
+                }
+            },
+            X = function() {
+                var b = o.find(".timepicker-hours table"),
+                    c = f.clone().startOf("d"),
+                    d = [],
+                    e = a("<tr>");
+                for (f.hour() > 11 && !h && c.hour(12); c.isSame(f, "d") && (h || f.hour() < 12 && c.hour() < 12 || f.hour() > 11);) c.hour() % 4 === 0 && (e = a("<tr>"), d.push(e)), e.append('<td data-action="selectHour" class="hour' + (R(c, "h") ? "" : " disabled") + '">' + c.format(h ? "HH" : "hh") + "</td>"), c.add(1, "h");
+                b.empty().append(d)
+            },
+            Y = function() {
+                for (var b = o.find(".timepicker-minutes table"), c = f.clone().startOf("h"), e = [], g = a("<tr>"), h = 1 === d.stepping ? 5 : d.stepping; f.isSame(c, "h");) c.minute() % (4 * h) === 0 && (g = a("<tr>"), e.push(g)), g.append('<td data-action="selectMinute" class="minute' + (R(c, "m") ? "" : " disabled") + '">' + c.format("mm") + "</td>"), c.add(h, "m");
+                b.empty().append(e)
+            },
+            Z = function() {
+                for (var b = o.find(".timepicker-seconds table"), c = f.clone().startOf("m"), d = [], e = a("<tr>"); f.isSame(c, "m");) c.second() % 20 === 0 && (e = a("<tr>"), d.push(e)), e.append('<td data-action="selectSecond" class="second' + (R(c, "s") ? "" : " disabled") + '">' + c.format("ss") + "</td>"), c.add(5, "s");
+                b.empty().append(d)
+            },
+            $ = function() {
+                var a, b, c = o.find(".timepicker span[data-time-component]");
+                h || (a = o.find(".timepicker [data-action=togglePeriod]"), b = e.clone().add(e.hours() >= 12 ? -12 : 12, "h"), a.text(e.format("A")), R(b, "h") ? a.removeClass("disabled") : a.addClass("disabled")), c.filter("[data-time-component=hours]").text(e.format(h ? "HH" : "hh")), c.filter("[data-time-component=minutes]").text(e.format("mm")), c.filter("[data-time-component=seconds]").text(e.format("ss")), X(), Y(), Z()
+            },
+            _ = function() {
+                o && (W(), $())
+            },
+            aa = function(a) {
+                var b = m ? null : e;
+                if (!a) return m = !0, g.val(""), c.data("date", ""), J({
+                    type: "dp.change",
+                    date: !1,
+                    oldDate: b
+                }), void _();
+                if (a = a.clone().locale(d.locale), x() && a.tz(d.timeZone), 1 !== d.stepping)
+                    for (a.minutes(Math.round(a.minutes() / d.stepping) * d.stepping).seconds(0); d.minDate && a.isBefore(d.minDate);) a.add(d.stepping, "minutes");
+                R(a) ? (e = a, f = e.clone(), g.val(e.format(i)), c.data("date", e.format(i)), m = !1, _(), J({
+                    type: "dp.change",
+                    date: e.clone(),
+                    oldDate: b
+                })) : (d.keepInvalid ? J({
+                    type: "dp.change",
+                    date: a,
+                    oldDate: b
+                }) : g.val(m ? "" : e.format(i)), J({
+                    type: "dp.error",
+                    date: a,
+                    oldDate: b
+                }))
+            },
+            ba = function() {
+                var b = !1;
+                return o ? (o.find(".collapse").each(function() {
+                    var c = a(this).data("collapse");
+                    return !c || !c.transitioning || (b = !0, !1)
+                }), b ? l : (n && n.hasClass("btn") && n.toggleClass("active"), o.hide(), a(window).off("resize", I), o.off("click", "[data-action]"), o.off("mousedown", !1), o.remove(), o = !1, J({
+                    type: "dp.hide",
+                    date: e.clone()
+                }), g.blur(), f = e.clone(), l)) : l
+            },
+            ca = function() {
+                aa(null)
+            },
+            da = function(a) {
+                return void 0 === d.parseInputDate ? (!b.isMoment(a) || a instanceof Date) && (a = y(a)) : a = d.parseInputDate(a), a
+            },
+            ea = {
+                next: function() {
+                    var a = q[k].navFnc;
+                    f.add(q[k].navStep, a), W(), K(a)
+                },
+                previous: function() {
+                    var a = q[k].navFnc;
+                    f.subtract(q[k].navStep, a), W(), K(a)
+                },
+                pickerSwitch: function() {
+                    L(1)
+                },
+                selectMonth: function(b) {
+                    var c = a(b.target).closest("tbody").find("span").index(a(b.target));
+                    f.month(c), k === p ? (aa(e.clone().year(f.year()).month(f.month())), d.inline || ba()) : (L(-1), W()), K("M")
+                },
+                selectYear: function(b) {
+                    var c = parseInt(a(b.target).text(), 10) || 0;
+                    f.year(c), k === p ? (aa(e.clone().year(f.year())), d.inline || ba()) : (L(-1), W()), K("YYYY")
+                },
+                selectDecade: function(b) {
+                    var c = parseInt(a(b.target).data("selection"), 10) || 0;
+                    f.year(c), k === p ? (aa(e.clone().year(f.year())), d.inline || ba()) : (L(-1), W()), K("YYYY")
+                },
+                selectDay: function(b) {
+                    var c = f.clone();
+                    a(b.target).is(".old") && c.subtract(1, "M"), a(b.target).is(".new") && c.add(1, "M"), aa(c.date(parseInt(a(b.target).text(), 10))), A() || d.keepOpen || d.inline || ba()
+                },
+                incrementHours: function() {
+                    var a = e.clone().add(1, "h");
+                    R(a, "h") && aa(a)
+                },
+                incrementMinutes: function() {
+                    var a = e.clone().add(d.stepping, "m");
+                    R(a, "m") && aa(a)
+                },
+                incrementSeconds: function() {
+                    var a = e.clone().add(1, "s");
+                    R(a, "s") && aa(a)
+                },
+                decrementHours: function() {
+                    var a = e.clone().subtract(1, "h");
+                    R(a, "h") && aa(a)
+                },
+                decrementMinutes: function() {
+                    var a = e.clone().subtract(d.stepping, "m");
+                    R(a, "m") && aa(a)
+                },
+                decrementSeconds: function() {
+                    var a = e.clone().subtract(1, "s");
+                    R(a, "s") && aa(a)
+                },
+                togglePeriod: function() {
+                    aa(e.clone().add(e.hours() >= 12 ? -12 : 12, "h"))
+                },
+                togglePicker: function(b) {
+                    var c, e = a(b.target),
+                        f = e.closest("ul"),
+                        g = f.find(".in"),
+                        h = f.find(".collapse:not(.in)");
+                    if (g && g.length) {
+                        if (c = g.data("collapse"), c && c.transitioning) return;
+                        g.collapse ? (g.collapse("hide"), h.collapse("show")) : (g.removeClass("in"), h.addClass("in")), e.is("span") ? e.toggleClass(d.icons.time + " " + d.icons.date) : e.find("span").toggleClass(d.icons.time + " " + d.icons.date)
+                    }
+                },
+                showPicker: function() {
+                    o.find(".timepicker > div:not(.timepicker-picker)").hide(), o.find(".timepicker .timepicker-picker").show()
+                },
+                showHours: function() {
+                    o.find(".timepicker .timepicker-picker").hide(), o.find(".timepicker .timepicker-hours").show()
+                },
+                showMinutes: function() {
+                    o.find(".timepicker .timepicker-picker").hide(), o.find(".timepicker .timepicker-minutes").show()
+                },
+                showSeconds: function() {
+                    o.find(".timepicker .timepicker-picker").hide(), o.find(".timepicker .timepicker-seconds").show()
+                },
+                selectHour: function(b) {
+                    var c = parseInt(a(b.target).text(), 10);
+                    h || (e.hours() >= 12 ? 12 !== c && (c += 12) : 12 === c && (c = 0)), aa(e.clone().hours(c)), ea.showPicker.call(l)
+                },
+                selectMinute: function(b) {
+                    aa(e.clone().minutes(parseInt(a(b.target).text(), 10))), ea.showPicker.call(l)
+                },
+                selectSecond: function(b) {
+                    aa(e.clone().seconds(parseInt(a(b.target).text(), 10))), ea.showPicker.call(l)
+                },
+                clear: ca,
+                today: function() {
+                    var a = y();
+                    R(a, "d") && aa(a)
+                },
+                close: ba
+            },
+            fa = function(b) {
+                return !a(b.currentTarget).is(".disabled") && (ea[a(b.currentTarget).data("action")].apply(l, arguments), !1)
+            },
+            ga = function() {
+                var b, c = {
+                    year: function(a) {
+                        return a.month(0).date(1).hours(0).seconds(0).minutes(0)
+                    },
+                    month: function(a) {
+                        return a.date(1).hours(0).seconds(0).minutes(0)
+                    },
+                    day: function(a) {
+                        return a.hours(0).seconds(0).minutes(0)
+                    },
+                    hour: function(a) {
+                        return a.seconds(0).minutes(0)
+                    },
+                    minute: function(a) {
+                        return a.seconds(0)
+                    }
+                };
+                return g.prop("disabled") || !d.ignoreReadonly && g.prop("readonly") || o ? l : (void 0 !== g.val() && 0 !== g.val().trim().length ? aa(da(g.val().trim())) : m && d.useCurrent && (d.inline || g.is("input") && 0 === g.val().trim().length) && (b = y(), "string" == typeof d.useCurrent && (b = c[d.useCurrent](b)), aa(b)), o = G(), M(), S(), o.find(".timepicker-hours").hide(), o.find(".timepicker-minutes").hide(), o.find(".timepicker-seconds").hide(), _(), L(), a(window).on("resize", I), o.on("click", "[data-action]", fa), o.on("mousedown", !1), n && n.hasClass("btn") && n.toggleClass("active"), I(), o.show(), d.focusOnShow && !g.is(":focus") && g.focus(), J({
+                    type: "dp.show"
+                }), l)
+            },
+            ha = function() {
+                return o ? ba() : ga()
+            },
+            ia = function(a) {
+                var b, c, e, f, g = null,
+                    h = [],
+                    i = {},
+                    j = a.which,
+                    k = "p";
+                w[j] = k;
+                for (b in w) w.hasOwnProperty(b) && w[b] === k && (h.push(b), parseInt(b, 10) !== j && (i[b] = !0));
+                for (b in d.keyBinds)
+                    if (d.keyBinds.hasOwnProperty(b) && "function" == typeof d.keyBinds[b] && (e = b.split(" "), e.length === h.length && v[j] === e[e.length - 1])) {
+                        for (f = !0, c = e.length - 2; c >= 0; c--)
+                            if (!(v[e[c]] in i)) {
+                                f = !1;
+                                break
+                            } if (f) {
+                            g = d.keyBinds[b];
+                            break
+                        }
+                    } g && (g.call(l, o), a.stopPropagation(), a.preventDefault())
+            },
+            ja = function(a) {
+                w[a.which] = "r", a.stopPropagation(), a.preventDefault()
+            },
+            ka = function(b) {
+                var c = a(b.target).val().trim(),
+                    d = c ? da(c) : null;
+                return aa(d), b.stopImmediatePropagation(), !1
+            },
+            la = function() {
+                g.on({
+                    change: ka,
+                    blur: d.debug ? "" : ba,
+                    keydown: ia,
+                    keyup: ja,
+                    focus: d.allowInputToggle ? ga : ""
+                }), c.is("input") ? g.on({
+                    focus: ga
+                }) : n && (n.on("click", ha), n.on("mousedown", !1))
+            },
+            ma = function() {
+                g.off({
+                    change: ka,
+                    blur: blur,
+                    keydown: ia,
+                    keyup: ja,
+                    focus: d.allowInputToggle ? ba : ""
+                }), c.is("input") ? g.off({
+                    focus: ga
+                }) : n && (n.off("click", ha), n.off("mousedown", !1))
+            },
+            na = function(b) {
+                var c = {};
+                return a.each(b, function() {
+                    var a = da(this);
+                    a.isValid() && (c[a.format("YYYY-MM-DD")] = !0)
+                }), !!Object.keys(c).length && c
+            },
+            oa = function(b) {
+                var c = {};
+                return a.each(b, function() {
+                    c[this] = !0
+                }), !!Object.keys(c).length && c
+            },
+            pa = function() {
+                var a = d.format || "L LT";
+                i = a.replace(/(\[[^\[]*\])|(\\)?(LTS|LT|LL?L?L?|l{1,4})/g, function(a) {
+                    var b = e.localeData().longDateFormat(a) || a;
+                    return b.replace(/(\[[^\[]*\])|(\\)?(LTS|LT|LL?L?L?|l{1,4})/g, function(a) {
+                        return e.localeData().longDateFormat(a) || a
+                    })
+                }), j = d.extraFormats ? d.extraFormats.slice() : [], j.indexOf(a) < 0 && j.indexOf(i) < 0 && j.push(i), h = i.toLowerCase().indexOf("a") < 1 && i.replace(/\[.*?\]/g, "").indexOf("h") < 1, z("y") && (p = 2), z("M") && (p = 1), z("d") && (p = 0), k = Math.max(p, k), m || aa(e)
+            };
+        if (l.destroy = function() {
+                ba(), ma(), c.removeData("DateTimePicker"), c.removeData("date")
+            }, l.toggle = ha, l.show = ga, l.hide = ba, l.disable = function() {
+                return ba(), n && n.hasClass("btn") && n.addClass("disabled"), g.prop("disabled", !0), l
+            }, l.enable = function() {
+                return n && n.hasClass("btn") && n.removeClass("disabled"), g.prop("disabled", !1), l
+            }, l.ignoreReadonly = function(a) {
+                if (0 === arguments.length) return d.ignoreReadonly;
+                if ("boolean" != typeof a) throw new TypeError("ignoreReadonly () expects a boolean parameter");
+                return d.ignoreReadonly = a, l
+            }, l.options = function(b) {
+                if (0 === arguments.length) return a.extend(!0, {}, d);
+                if (!(b instanceof Object)) throw new TypeError("options() options parameter should be an object");
+                return a.extend(!0, d, b), a.each(d, function(a, b) {
+                    if (void 0 === l[a]) throw new TypeError("option " + a + " is not recognized!");
+                    l[a](b)
+                }), l
+            }, l.date = function(a) {
+                if (0 === arguments.length) return m ? null : e.clone();
+                if (!(null === a || "string" == typeof a || b.isMoment(a) || a instanceof Date)) throw new TypeError("date() parameter must be one of [null, string, moment or Date]");
+                return aa(null === a ? null : da(a)), l
+            }, l.format = function(a) {
+                if (0 === arguments.length) return d.format;
+                if ("string" != typeof a && ("boolean" != typeof a || a !== !1)) throw new TypeError("format() expects a string or boolean:false parameter " + a);
+                return d.format = a, i && pa(), l
+            }, l.timeZone = function(a) {
+                if (0 === arguments.length) return d.timeZone;
+                if ("string" != typeof a) throw new TypeError("newZone() expects a string parameter");
+                return d.timeZone = a, l
+            }, l.dayViewHeaderFormat = function(a) {
+                if (0 === arguments.length) return d.dayViewHeaderFormat;
+                if ("string" != typeof a) throw new TypeError("dayViewHeaderFormat() expects a string parameter");
+                return d.dayViewHeaderFormat = a, l
+            }, l.extraFormats = function(a) {
+                if (0 === arguments.length) return d.extraFormats;
+                if (a !== !1 && !(a instanceof Array)) throw new TypeError("extraFormats() expects an array or false parameter");
+                return d.extraFormats = a, j && pa(), l
+            }, l.disabledDates = function(b) {
+                if (0 === arguments.length) return d.disabledDates ? a.extend({}, d.disabledDates) : d.disabledDates;
+                if (!b) return d.disabledDates = !1, _(), l;
+                if (!(b instanceof Array)) throw new TypeError("disabledDates() expects an array parameter");
+                return d.disabledDates = na(b), d.enabledDates = !1, _(), l
+            }, l.enabledDates = function(b) {
+                if (0 === arguments.length) return d.enabledDates ? a.extend({}, d.enabledDates) : d.enabledDates;
+                if (!b) return d.enabledDates = !1, _(), l;
+                if (!(b instanceof Array)) throw new TypeError("enabledDates() expects an array parameter");
+                return d.enabledDates = na(b), d.disabledDates = !1, _(), l
+            }, l.daysOfWeekDisabled = function(a) {
+                if (0 === arguments.length) return d.daysOfWeekDisabled.splice(0);
+                if ("boolean" == typeof a && !a) return d.daysOfWeekDisabled = !1, _(), l;
+                if (!(a instanceof Array)) throw new TypeError("daysOfWeekDisabled() expects an array parameter");
+                if (d.daysOfWeekDisabled = a.reduce(function(a, b) {
+                        return b = parseInt(b, 10), b > 6 || b < 0 || isNaN(b) ? a : (a.indexOf(b) === -1 && a.push(b), a)
+                    }, []).sort(), d.useCurrent && !d.keepInvalid) {
+                    for (var b = 0; !R(e, "d");) {
+                        if (e.add(1, "d"), 31 === b) throw "Tried 31 times to find a valid date";
+                        b++
+                    }
+                    aa(e)
+                }
+                return _(), l
+            }, l.maxDate = function(a) {
+                if (0 === arguments.length) return d.maxDate ? d.maxDate.clone() : d.maxDate;
+                if ("boolean" == typeof a && a === !1) return d.maxDate = !1, _(), l;
+                "string" == typeof a && ("now" !== a && "moment" !== a || (a = y()));
+                var b = da(a);
+                if (!b.isValid()) throw new TypeError("maxDate() Could not parse date parameter: " + a);
+                if (d.minDate && b.isBefore(d.minDate)) throw new TypeError("maxDate() date parameter is before options.minDate: " + b.format(i));
+                return d.maxDate = b, d.useCurrent && !d.keepInvalid && e.isAfter(a) && aa(d.maxDate), f.isAfter(b) && (f = b.clone().subtract(d.stepping, "m")), _(), l
+            }, l.minDate = function(a) {
+                if (0 === arguments.length) return d.minDate ? d.minDate.clone() : d.minDate;
+                if ("boolean" == typeof a && a === !1) return d.minDate = !1, _(), l;
+                "string" == typeof a && ("now" !== a && "moment" !== a || (a = y()));
+                var b = da(a);
+                if (!b.isValid()) throw new TypeError("minDate() Could not parse date parameter: " + a);
+                if (d.maxDate && b.isAfter(d.maxDate)) throw new TypeError("minDate() date parameter is after options.maxDate: " + b.format(i));
+                return d.minDate = b, d.useCurrent && !d.keepInvalid && e.isBefore(a) && aa(d.minDate), f.isBefore(b) && (f = b.clone().add(d.stepping, "m")), _(), l
+            }, l.defaultDate = function(a) {
+                if (0 === arguments.length) return d.defaultDate ? d.defaultDate.clone() : d.defaultDate;
+                if (!a) return d.defaultDate = !1, l;
+                "string" == typeof a && (a = "now" === a || "moment" === a ? y() : y(a));
+                var b = da(a);
+                if (!b.isValid()) throw new TypeError("defaultDate() Could not parse date parameter: " + a);
+                if (!R(b)) throw new TypeError("defaultDate() date passed is invalid according to component setup validations");
+                return d.defaultDate = b, (d.defaultDate && d.inline || "" === g.val().trim()) && aa(d.defaultDate), l
+            }, l.locale = function(a) {
+                if (0 === arguments.length) return d.locale;
+                if (!b.localeData(a)) throw new TypeError("locale() locale " + a + " is not loaded from moment locales!");
+                return d.locale = a, e.locale(d.locale), f.locale(d.locale), i && pa(), o && (ba(), ga()), l
+            }, l.stepping = function(a) {
+                return 0 === arguments.length ? d.stepping : (a = parseInt(a, 10), (isNaN(a) || a < 1) && (a = 1), d.stepping = a, l)
+            }, l.useCurrent = function(a) {
+                var b = ["year", "month", "day", "hour", "minute"];
+                if (0 === arguments.length) return d.useCurrent;
+                if ("boolean" != typeof a && "string" != typeof a) throw new TypeError("useCurrent() expects a boolean or string parameter");
+                if ("string" == typeof a && b.indexOf(a.toLowerCase()) === -1) throw new TypeError("useCurrent() expects a string parameter of " + b.join(", "));
+                return d.useCurrent = a, l
+            }, l.collapse = function(a) {
+                if (0 === arguments.length) return d.collapse;
+                if ("boolean" != typeof a) throw new TypeError("collapse() expects a boolean parameter");
+                return d.collapse === a ? l : (d.collapse = a, o && (ba(), ga()), l)
+            }, l.icons = function(b) {
+                if (0 === arguments.length) return a.extend({}, d.icons);
+                if (!(b instanceof Object)) throw new TypeError("icons() expects parameter to be an Object");
+                return a.extend(d.icons, b), o && (ba(), ga()), l
+            }, l.tooltips = function(b) {
+                if (0 === arguments.length) return a.extend({}, d.tooltips);
+                if (!(b instanceof Object)) throw new TypeError("tooltips() expects parameter to be an Object");
+                return a.extend(d.tooltips, b), o && (ba(), ga()), l
+            }, l.useStrict = function(a) {
+                if (0 === arguments.length) return d.useStrict;
+                if ("boolean" != typeof a) throw new TypeError("useStrict() expects a boolean parameter");
+                return d.useStrict = a, l
+            }, l.sideBySide = function(a) {
+                if (0 === arguments.length) return d.sideBySide;
+                if ("boolean" != typeof a) throw new TypeError("sideBySide() expects a boolean parameter");
+                return d.sideBySide = a, o && (ba(), ga()), l
+            }, l.viewMode = function(a) {
+                if (0 === arguments.length) return d.viewMode;
+                if ("string" != typeof a) throw new TypeError("viewMode() expects a string parameter");
+                if (r.indexOf(a) === -1) throw new TypeError("viewMode() parameter must be one of (" + r.join(", ") + ") value");
+                return d.viewMode = a, k = Math.max(r.indexOf(a), p), L(), l
+            }, l.toolbarPlacement = function(a) {
+                if (0 === arguments.length) return d.toolbarPlacement;
+                if ("string" != typeof a) throw new TypeError("toolbarPlacement() expects a string parameter");
+                if (u.indexOf(a) === -1) throw new TypeError("toolbarPlacement() parameter must be one of (" + u.join(", ") + ") value");
+                return d.toolbarPlacement = a, o && (ba(), ga()), l
+            }, l.widgetPositioning = function(b) {
+                if (0 === arguments.length) return a.extend({}, d.widgetPositioning);
+                if ("[object Object]" !== {}.toString.call(b)) throw new TypeError("widgetPositioning() expects an object variable");
+                if (b.horizontal) {
+                    if ("string" != typeof b.horizontal) throw new TypeError("widgetPositioning() horizontal variable must be a string");
+                    if (b.horizontal = b.horizontal.toLowerCase(), t.indexOf(b.horizontal) === -1) throw new TypeError("widgetPositioning() expects horizontal parameter to be one of (" + t.join(", ") + ")");
+                    d.widgetPositioning.horizontal = b.horizontal
+                }
+                if (b.vertical) {
+                    if ("string" != typeof b.vertical) throw new TypeError("widgetPositioning() vertical variable must be a string");
+                    if (b.vertical = b.vertical.toLowerCase(), s.indexOf(b.vertical) === -1) throw new TypeError("widgetPositioning() expects vertical parameter to be one of (" + s.join(", ") + ")");
+                    d.widgetPositioning.vertical = b.vertical
+                }
+                return _(), l
+            }, l.calendarWeeks = function(a) {
+                if (0 === arguments.length) return d.calendarWeeks;
+                if ("boolean" != typeof a) throw new TypeError("calendarWeeks() expects parameter to be a boolean value");
+                return d.calendarWeeks = a, _(), l
+            }, l.showTodayButton = function(a) {
+                if (0 === arguments.length) return d.showTodayButton;
+                if ("boolean" != typeof a) throw new TypeError("showTodayButton() expects a boolean parameter");
+                return d.showTodayButton = a, o && (ba(), ga()), l
+            }, l.showClear = function(a) {
+                if (0 === arguments.length) return d.showClear;
+                if ("boolean" != typeof a) throw new TypeError("showClear() expects a boolean parameter");
+                return d.showClear = a, o && (ba(), ga()), l
+            }, l.widgetParent = function(b) {
+                if (0 === arguments.length) return d.widgetParent;
+                if ("string" == typeof b && (b = a(b)), null !== b && "string" != typeof b && !(b instanceof a)) throw new TypeError("widgetParent() expects a string or a jQuery object parameter");
+                return d.widgetParent = b, o && (ba(), ga()), l
+            }, l.keepOpen = function(a) {
+                if (0 === arguments.length) return d.keepOpen;
+                if ("boolean" != typeof a) throw new TypeError("keepOpen() expects a boolean parameter");
+                return d.keepOpen = a, l
+            }, l.focusOnShow = function(a) {
+                if (0 === arguments.length) return d.focusOnShow;
+                if ("boolean" != typeof a) throw new TypeError("focusOnShow() expects a boolean parameter");
+                return d.focusOnShow = a, l
+            }, l.inline = function(a) {
+                if (0 === arguments.length) return d.inline;
+                if ("boolean" != typeof a) throw new TypeError("inline() expects a boolean parameter");
+                return d.inline = a, l
+            }, l.clear = function() {
+                return ca(), l
+            }, l.keyBinds = function(a) {
+                return 0 === arguments.length ? d.keyBinds : (d.keyBinds = a, l)
+            }, l.getMoment = function(a) {
+                return y(a)
+            }, l.debug = function(a) {
+                if ("boolean" != typeof a) throw new TypeError("debug() expects a boolean parameter");
+                return d.debug = a, l
+            }, l.allowInputToggle = function(a) {
+                if (0 === arguments.length) return d.allowInputToggle;
+                if ("boolean" != typeof a) throw new TypeError("allowInputToggle() expects a boolean parameter");
+                return d.allowInputToggle = a, l
+            }, l.showClose = function(a) {
+                if (0 === arguments.length) return d.showClose;
+                if ("boolean" != typeof a) throw new TypeError("showClose() expects a boolean parameter");
+                return d.showClose = a, l
+            }, l.keepInvalid = function(a) {
+                if (0 === arguments.length) return d.keepInvalid;
+                if ("boolean" != typeof a) throw new TypeError("keepInvalid() expects a boolean parameter");
+                return d.keepInvalid = a, l
+            }, l.datepickerInput = function(a) {
+                if (0 === arguments.length) return d.datepickerInput;
+                if ("string" != typeof a) throw new TypeError("datepickerInput() expects a string parameter");
+                return d.datepickerInput = a, l
+            }, l.parseInputDate = function(a) {
+                if (0 === arguments.length) return d.parseInputDate;
+                if ("function" != typeof a) throw new TypeError("parseInputDate() sholud be as function");
+                return d.parseInputDate = a, l
+            }, l.disabledTimeIntervals = function(b) {
+                if (0 === arguments.length) return d.disabledTimeIntervals ? a.extend({}, d.disabledTimeIntervals) : d.disabledTimeIntervals;
+                if (!b) return d.disabledTimeIntervals = !1, _(), l;
+                if (!(b instanceof Array)) throw new TypeError("disabledTimeIntervals() expects an array parameter");
+                return d.disabledTimeIntervals = b, _(), l
+            }, l.disabledHours = function(b) {
+                if (0 === arguments.length) return d.disabledHours ? a.extend({}, d.disabledHours) : d.disabledHours;
+                if (!b) return d.disabledHours = !1, _(), l;
+                if (!(b instanceof Array)) throw new TypeError("disabledHours() expects an array parameter");
+                if (d.disabledHours = oa(b), d.enabledHours = !1, d.useCurrent && !d.keepInvalid) {
+                    for (var c = 0; !R(e, "h");) {
+                        if (e.add(1, "h"), 24 === c) throw "Tried 24 times to find a valid date";
+                        c++
+                    }
+                    aa(e)
+                }
+                return _(), l
+            }, l.enabledHours = function(b) {
+                if (0 === arguments.length) return d.enabledHours ? a.extend({}, d.enabledHours) : d.enabledHours;
+                if (!b) return d.enabledHours = !1, _(), l;
+                if (!(b instanceof Array)) throw new TypeError("enabledHours() expects an array parameter");
+                if (d.enabledHours = oa(b), d.disabledHours = !1, d.useCurrent && !d.keepInvalid) {
+                    for (var c = 0; !R(e, "h");) {
+                        if (e.add(1, "h"), 24 === c) throw "Tried 24 times to find a valid date";
+                        c++
+                    }
+                    aa(e)
+                }
+                return _(), l
+            }, l.viewDate = function(a) {
+                if (0 === arguments.length) return f.clone();
+                if (!a) return f = e.clone(), l;
+                if (!("string" == typeof a || b.isMoment(a) || a instanceof Date)) throw new TypeError("viewDate() parameter must be one of [string, moment or Date]");
+                return f = da(a), K(), l
+            }, c.is("input")) g = c;
+        else if (g = c.find(d.datepickerInput), 0 === g.length) g = c.find("input");
+        else if (!g.is("input")) throw new Error('CSS class "' + d.datepickerInput + '" cannot be applied to non input element');
+        if (c.hasClass("input-group") && (n = 0 === c.find(".datepickerbutton").length ? c.find(".input-group-addon") : c.find(".datepickerbutton")), !d.inline && !g.is("input")) throw new Error("Could not initialize DateTimePicker without an input element");
+        return e = y(), f = e.clone(), a.extend(!0, d, H()), l.options(d), pa(), la(), g.prop("disabled") && l.disable(), g.is("input") && 0 !== g.val().trim().length ? aa(da(g.val().trim())) : d.defaultDate && void 0 === g.attr("placeholder") && aa(d.defaultDate), d.inline && ga(), l
+    };
+    return a.fn.datetimepicker = function(b) {
+        b = b || {};
+        var d, e = Array.prototype.slice.call(arguments, 1),
+            f = !0,
+            g = ["destroy", "hide", "show", "toggle"];
+        if ("object" == typeof b) return this.each(function() {
+            var d, e = a(this);
+            e.data("DateTimePicker") || (d = a.extend(!0, {}, a.fn.datetimepicker.defaults, b), e.data("DateTimePicker", c(e, d)))
+        });
+        if ("string" == typeof b) return this.each(function() {
+            var c = a(this),
+                g = c.data("DateTimePicker");
+            if (!g) throw new Error('bootstrap-datetimepicker("' + b + '") method was called on an element that is not using DateTimePicker');
+            d = g[b].apply(g, e), f = d === g
+        }), f || a.inArray(b, g) > -1 ? this : d;
+        throw new TypeError("Invalid arguments for DateTimePicker: " + b)
+    }, a.fn.datetimepicker.defaults = {
+        timeZone: "",
+        format: !1,
+        dayViewHeaderFormat: "MMMM YYYY",
+        extraFormats: !1,
+        stepping: 1,
+        minDate: !1,
+        maxDate: !1,
+        useCurrent: !0,
+        collapse: !0,
+        locale: b.locale(),
+        defaultDate: !1,
+        disabledDates: !1,
+        enabledDates: !1,
+        icons: {
+            time: "glyphicon glyphicon-time",
+            date: "glyphicon glyphicon-calendar",
+            up: "glyphicon glyphicon-chevron-up",
+            down: "glyphicon glyphicon-chevron-down",
+            previous: "glyphicon glyphicon-chevron-left",
+            next: "glyphicon glyphicon-chevron-right",
+            today: "glyphicon glyphicon-screenshot",
+            clear: "glyphicon glyphicon-trash",
+            close: "glyphicon glyphicon-remove"
+        },
+        tooltips: {
+            today: "Go to today",
+            clear: "Clear selection",
+            close: "Close the picker",
+            selectMonth: "Select Month",
+            prevMonth: "Previous Month",
+            nextMonth: "Next Month",
+            selectYear: "Select Year",
+            prevYear: "Previous Year",
+            nextYear: "Next Year",
+            selectDecade: "Select Decade",
+            prevDecade: "Previous Decade",
+            nextDecade: "Next Decade",
+            prevCentury: "Previous Century",
+            nextCentury: "Next Century",
+            pickHour: "Pick Hour",
+            incrementHour: "Increment Hour",
+            decrementHour: "Decrement Hour",
+            pickMinute: "Pick Minute",
+            incrementMinute: "Increment Minute",
+            decrementMinute: "Decrement Minute",
+            pickSecond: "Pick Second",
+            incrementSecond: "Increment Second",
+            decrementSecond: "Decrement Second",
+            togglePeriod: "Toggle Period",
+            selectTime: "Select Time"
+        },
+        useStrict: !1,
+        sideBySide: !1,
+        daysOfWeekDisabled: !1,
+        calendarWeeks: !1,
+        viewMode: "days",
+        toolbarPlacement: "default",
+        showTodayButton: !1,
+        showClear: !1,
+        showClose: !1,
+        widgetPositioning: {
+            horizontal: "auto",
+            vertical: "auto"
+        },
+        widgetParent: null,
+        ignoreReadonly: !1,
+        keepOpen: !1,
+        focusOnShow: !0,
+        inline: !1,
+        keepInvalid: !1,
+        datepickerInput: ".datepickerinput",
+        keyBinds: {
+            up: function(a) {
+                if (a) {
+                    var b = this.date() || this.getMoment();
+                    a.find(".datepicker").is(":visible") ? this.date(b.clone().subtract(7, "d")) : this.date(b.clone().add(this.stepping(), "m"))
+                }
+            },
+            down: function(a) {
+                if (!a) return void this.show();
+                var b = this.date() || this.getMoment();
+                a.find(".datepicker").is(":visible") ? this.date(b.clone().add(7, "d")) : this.date(b.clone().subtract(this.stepping(), "m"))
+            },
+            "control up": function(a) {
+                if (a) {
+                    var b = this.date() || this.getMoment();
+                    a.find(".datepicker").is(":visible") ? this.date(b.clone().subtract(1, "y")) : this.date(b.clone().add(1, "h"))
+                }
+            },
+            "control down": function(a) {
+                if (a) {
+                    var b = this.date() || this.getMoment();
+                    a.find(".datepicker").is(":visible") ? this.date(b.clone().add(1, "y")) : this.date(b.clone().subtract(1, "h"))
+                }
+            },
+            left: function(a) {
+                if (a) {
+                    var b = this.date() || this.getMoment();
+                    a.find(".datepicker").is(":visible") && this.date(b.clone().subtract(1, "d"))
+                }
+            },
+            right: function(a) {
+                if (a) {
+                    var b = this.date() || this.getMoment();
+                    a.find(".datepicker").is(":visible") && this.date(b.clone().add(1, "d"))
+                }
+            },
+            pageUp: function(a) {
+                if (a) {
+                    var b = this.date() || this.getMoment();
+                    a.find(".datepicker").is(":visible") && this.date(b.clone().subtract(1, "M"))
+                }
+            },
+            pageDown: function(a) {
+                if (a) {
+                    var b = this.date() || this.getMoment();
+                    a.find(".datepicker").is(":visible") && this.date(b.clone().add(1, "M"))
+                }
+            },
+            enter: function() {
+                this.hide()
+            },
+            escape: function() {
+                this.hide()
+            },
+            "control space": function(a) {
+                a && a.find(".timepicker").is(":visible") && a.find('.btn[data-action="togglePeriod"]').click()
+            },
+            t: function() {
+                this.date(this.getMoment())
+            },
+            delete: function() {
+                this.clear()
+            }
+        },
+        debug: !1,
+        allowInputToggle: !1,
+        disabledTimeIntervals: !1,
+        disabledHours: !1,
+        enabledHours: !1,
+        viewDate: !1
+    }, a.fn.datetimepicker
 });
```

### Comparing `nobinobi-core-0.1.4.6/nobinobi_core/static/js/moment-with-locales.min.js` & `nobinobi-core-0.1.4.7/nobinobi_core/static/js/moment-with-locales.min.js`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.6/nobinobi_core/static/js/nobinobi_core.js` & `nobinobi-core-0.1.4.7/nobinobi_core/static/js/nobinobi_core.js`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.6/nobinobi_core/templates/layout/checkboxselectmultiple_act.html` & `nobinobi-core-0.1.4.7/nobinobi_core/templates/layout/checkboxselectmultiple_act.html`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-{###############################################################################}
-{##}
-{#   Copyright (C) <2016>  <Florian Alu - Prolibre - http://prolibre.com>#}
-{##}
-{#    This program is free software: you can redistribute it and/or modify#}
-{#    it under the terms of the GNU Affero General Public License as published#}
-{#    by the Free Software Foundation, either version 3 of the License.#}
-{#    #}
-{##}
-{#    This program is distributed in the hope that it will be useful,#}
-{#    but WITHOUT ANY WARRANTY; without even the implied warranty of#}
-{#    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the#}
-{#    GNU Affero General Public License for more details.#}
-{##}
-{#    You should have received a copy of the GNU Affero General Public License#}
-{#    along with this program.  If not, see <http://www.gnu.org/licenses/>.#}
-{##}
-{###############################################################################}
-
-{% load crispy_forms_filters %}
-{% load startwith %}
-{% load l10n %}
-
-<div class="controls {{ field_class }}"{% if flat_attrs %} {{ flat_attrs|safe }}{% endif %}>
-    {% include 'bootstrap3/layout/field_errors_block.html' %}
-    {% for a in list_group_act.items %}
-        <fieldset style="margin-bottom: 7px">
-            <legend style="margin-bottom: 1px">{{ a.0 }}</legend>
-            {% for choice in field.field.choices %}
-
-                {% if choice.0 in a.1 %}
-                <label class="{% if inline_class %}checkbox-{{ inline_class }}{% endif %}">
-
-                    <input type="checkbox"
-                            {% if choice.0 in field.value or choice.0|stringformat:"s" in field.value or choice.0|stringformat:"s" == field.value|stringformat:"s" %}
-                           checked="checked"{% endif %} name="{{ field.html_name }}"
-                           id="id_{{ field.html_name }}_{{ forloop.counter }}"
-                           value="{{ choice.0|unlocalize }}" {{ field.field.widget.attrs|flatatt }}>
-                    {{ choice.1|unlocalize }}
-                </label>
-
-                {% endif %}
-            {% endfor %}
-        </fieldset>
-    {% endfor %}
-
-    {% include 'bootstrap3/layout/help_text.html' %}
-</div>
+{###############################################################################}
+{##}
+{#   Copyright (C) <2016>  <Florian Alu - Prolibre - http://prolibre.com>#}
+{##}
+{#    This program is free software: you can redistribute it and/or modify#}
+{#    it under the terms of the GNU Affero General Public License as published#}
+{#    by the Free Software Foundation, either version 3 of the License.#}
+{#    #}
+{##}
+{#    This program is distributed in the hope that it will be useful,#}
+{#    but WITHOUT ANY WARRANTY; without even the implied warranty of#}
+{#    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the#}
+{#    GNU Affero General Public License for more details.#}
+{##}
+{#    You should have received a copy of the GNU Affero General Public License#}
+{#    along with this program.  If not, see <http://www.gnu.org/licenses/>.#}
+{##}
+{###############################################################################}
+
+{% load crispy_forms_filters %}
+{% load startwith %}
+{% load l10n %}
+
+<div class="controls {{ field_class }}"{% if flat_attrs %} {{ flat_attrs|safe }}{% endif %}>
+    {% include 'bootstrap3/layout/field_errors_block.html' %}
+    {% for a in list_group_act.items %}
+        <fieldset style="margin-bottom: 7px">
+            <legend style="margin-bottom: 1px">{{ a.0 }}</legend>
+            {% for choice in field.field.choices %}
+
+                {% if choice.0 in a.1 %}
+                <label class="{% if inline_class %}checkbox-{{ inline_class }}{% endif %}">
+
+                    <input type="checkbox"
+                            {% if choice.0 in field.value or choice.0|stringformat:"s" in field.value or choice.0|stringformat:"s" == field.value|stringformat:"s" %}
+                           checked="checked"{% endif %} name="{{ field.html_name }}"
+                           id="id_{{ field.html_name }}_{{ forloop.counter }}"
+                           value="{{ choice.0|unlocalize }}" {{ field.field.widget.attrs|flatatt }}>
+                    {{ choice.1|unlocalize }}
+                </label>
+
+                {% endif %}
+            {% endfor %}
+        </fieldset>
+    {% endfor %}
+
+    {% include 'bootstrap3/layout/help_text.html' %}
+</div>
```

### Comparing `nobinobi-core-0.1.4.6/nobinobi_core/templates/layout/checkboxselectmultiple_image.html` & `nobinobi-core-0.1.4.7/nobinobi_core/templates/layout/checkboxselectmultiple_image.html`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-{###############################################################################}
-{##}
-{#   Copyright (C) <2016>  <Florian Alu - Prolibre - http://prolibre.com>#}
-{##}
-{#    This program is free software: you can redistribute it and/or modify#}
-{#    it under the terms of the GNU Affero General Public License as published#}
-{#    by the Free Software Foundation, either version 3 of the License.#}
-{#    #}
-{##}
-{#    This program is distributed in the hope that it will be useful,#}
-{#    but WITHOUT ANY WARRANTY; without even the implied warranty of#}
-{#    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the#}
-{#    GNU Affero General Public License for more details.#}
-{##}
-{#    You should have received a copy of the GNU Affero General Public License#}
-{#    along with this program.  If not, see <http://www.gnu.org/licenses/>.#}
-{##}
-{###############################################################################}
-
-{% load crispy_forms_filters %}
-{% load l10n %}
-{% load static %}
-
-<div class="controls {{ field_class }}"{% if flat_attrs %} {{ flat_attrs|safe }}{% endif %}>
-    {% include 'layout/field_errors_block.html' %}
-
-    {% for choice in field.field.choices %}
-
-        {% if not inline_class %}
-            <div class="checkbox">{% endif %}
-    <label class="{% if inline_class %}checkbox-{{ inline_class }}{% endif %}">
-        <input type="checkbox"
-                {% if choice.0 in field.value or choice.0|stringformat:"s" in field.value or choice.0|stringformat:"s" == field.value|stringformat:"s" %}
-               checked="checked"{% endif %} name="{{ field.html_name }}"
-               id="id_{{ field.html_name }}_{{ forloop.counter }}"
-               value="{{ choice.0|unlocalize }}" {{ field.field.widget.attrs|flatatt }}>
-        {% if choice.0 == None or choice.0 == "" %}
-            <img class='img-responsive img-repas-list' src='{% static "img/smiley/question.png" %}'/>
-        {% else %}
-            <img class='img-responsive img-repas-list' src='{% static "img/repas/" %}{{ choice.1|unlocalize }}'/>
-        {% endif %}
-    </label>
-    {% if not inline_class %}</div>{% endif %}
-    {% endfor %}
-
-    {% include 'layout/help_text.html' %}
-</div>
+{###############################################################################}
+{##}
+{#   Copyright (C) <2016>  <Florian Alu - Prolibre - http://prolibre.com>#}
+{##}
+{#    This program is free software: you can redistribute it and/or modify#}
+{#    it under the terms of the GNU Affero General Public License as published#}
+{#    by the Free Software Foundation, either version 3 of the License.#}
+{#    #}
+{##}
+{#    This program is distributed in the hope that it will be useful,#}
+{#    but WITHOUT ANY WARRANTY; without even the implied warranty of#}
+{#    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the#}
+{#    GNU Affero General Public License for more details.#}
+{##}
+{#    You should have received a copy of the GNU Affero General Public License#}
+{#    along with this program.  If not, see <http://www.gnu.org/licenses/>.#}
+{##}
+{###############################################################################}
+
+{% load crispy_forms_filters %}
+{% load l10n %}
+{% load static %}
+
+<div class="controls {{ field_class }}"{% if flat_attrs %} {{ flat_attrs|safe }}{% endif %}>
+    {% include 'layout/field_errors_block.html' %}
+
+    {% for choice in field.field.choices %}
+
+        {% if not inline_class %}
+            <div class="checkbox">{% endif %}
+    <label class="{% if inline_class %}checkbox-{{ inline_class }}{% endif %}">
+        <input type="checkbox"
+                {% if choice.0 in field.value or choice.0|stringformat:"s" in field.value or choice.0|stringformat:"s" == field.value|stringformat:"s" %}
+               checked="checked"{% endif %} name="{{ field.html_name }}"
+               id="id_{{ field.html_name }}_{{ forloop.counter }}"
+               value="{{ choice.0|unlocalize }}" {{ field.field.widget.attrs|flatatt }}>
+        {% if choice.0 == None or choice.0 == "" %}
+            <img class='img-responsive img-repas-list' src='{% static "img/smiley/question.png" %}'/>
+        {% else %}
+            <img class='img-responsive img-repas-list' src='{% static "img/repas/" %}{{ choice.1|unlocalize }}'/>
+        {% endif %}
+    </label>
+    {% if not inline_class %}</div>{% endif %}
+    {% endfor %}
+
+    {% include 'layout/help_text.html' %}
+</div>
```

### Comparing `nobinobi-core-0.1.4.6/nobinobi_core/templates/layout/checkboxselectmultiple_inline.html` & `nobinobi-core-0.1.4.7/nobinobi_core/templates/layout/radioselect_inline_image.html`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-{###############################################################################}
-{##}
-{#   Copyright (C) <2016>  <Florian Alu - Prolibre - http://prolibre.com>#}
-{##}
-{#    This program is free software: you can redistribute it and/or modify#}
-{#    it under the terms of the GNU Affero General Public License as published#}
-{#    by the Free Software Foundation, either version 3 of the License.#}
-{#    #}
-{##}
-{#    This program is distributed in the hope that it will be useful,#}
-{#    but WITHOUT ANY WARRANTY; without even the implied warranty of#}
-{#    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the#}
-{#    GNU Affero General Public License for more details.#}
-{##}
-{#    You should have received a copy of the GNU Affero General Public License#}
-{#    along with this program.  If not, see <http://www.gnu.org/licenses/>.#}
-{##}
-{###############################################################################}
-
-{% if field.is_hidden %}
-    {{ field }}
-{% else %}
-    <div id="div_{{ field.auto_id }}" class="form-group{% if form_show_errors and field.errors %} has-error{% endif %}{% if field.css_classes %} {{ field.css_classes }}{% endif %}">
-
-        {% if field.label %}
-            <label for="{{ field.auto_id }}"  class="control-label {{ label_class }}{% if field.field.required %} requiredField{% endif %}">
-                {{ field.label|safe }}{% if field.field.required %}<span class="asteriskField">*</span>{% endif %}
-            </label>
-        {% endif %}
-
-        {% include 'bootstrap3/layout/checkboxselectmultiple.html' %}
-    </div>
-{% endif %}
+{###############################################################################}
+{##}
+{#   Copyright (C) <2016>  <Florian Alu - Prolibre - http://prolibre.com>#}
+{##}
+{#    This program is free software: you can redistribute it and/or modify#}
+{#    it under the terms of the GNU Affero General Public License as published#}
+{#    by the Free Software Foundation, either version 3 of the License.#}
+{#    #}
+{##}
+{#    This program is distributed in the hope that it will be useful,#}
+{#    but WITHOUT ANY WARRANTY; without even the implied warranty of#}
+{#    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the#}
+{#    GNU Affero General Public License for more details.#}
+{##}
+{#    You should have received a copy of the GNU Affero General Public License#}
+{#    along with this program.  If not, see <http://www.gnu.org/licenses/>.#}
+{##}
+{###############################################################################}
+
+{% if field.is_hidden %}
+    {{ field }}
+{% else %}
+    <div id="div_{{ field.auto_id }}" class="form-group{% if wrapper_class %} {{ wrapper_class }}{% endif %}{% if form_show_errors and field.errors %} has-error{% endif %}{% if field.css_classes %} {{ field.css_classes }}{% endif %}">
+
+        {% if field.label %}
+            <label for="{{ field.auto_id }}"  class="control-label {{ label_class }}{% if field.field.required %} requiredField{% endif %}">
+                {{ field.label|safe }}{% if field.field.required %}<span class="asteriskField">*</span>{% endif %}
+            </label>
+        {% endif %}
+
+        {% include 'layout/radioselect_image.html' %}
+    </div>
+{% endif %}
```

### Comparing `nobinobi-core-0.1.4.6/nobinobi_core/templates/layout/checkboxselectmultiple_inline_act.html` & `nobinobi-core-0.1.4.7/nobinobi_core/templates/layout/checkboxselectmultiple_inline.html`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-{###############################################################################}
-{##}
-{#   Copyright (C) <2016>  <Florian Alu - Prolibre - http://prolibre.com>#}
-{##}
-{#    This program is free software: you can redistribute it and/or modify#}
-{#    it under the terms of the GNU Affero General Public License as published#}
-{#    by the Free Software Foundation, either version 3 of the License.#}
-{#    #}
-{##}
-{#    This program is distributed in the hope that it will be useful,#}
-{#    but WITHOUT ANY WARRANTY; without even the implied warranty of#}
-{#    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the#}
-{#    GNU Affero General Public License for more details.#}
-{##}
-{#    You should have received a copy of the GNU Affero General Public License#}
-{#    along with this program.  If not, see <http://www.gnu.org/licenses/>.#}
-{##}
-{###############################################################################}
-
-{% if field.is_hidden %}
-    {{ field }}
-{% else %}
-    <div id="div_{{ field.auto_id }}" class="form-group{% if form_show_errors and field.errors %} has-error{% endif %}{% if field.css_classes %} {{ field.css_classes }}{% endif %}">
-
-        {% if field.label %}
-            <label for="{{ field.auto_id }}"  class="control-label {{ label_class }}{% if field.field.required %} requiredField{% endif %}">
-                {{ field.label|safe }}{% if field.field.required %}<span class="asteriskField">*</span>{% endif %}
-            </label>
-        {% endif %}
-
-        {% include 'layout/checkboxselectmultiple_act.html' %}
-    </div>
-{% endif %}
+{###############################################################################}
+{##}
+{#   Copyright (C) <2016>  <Florian Alu - Prolibre - http://prolibre.com>#}
+{##}
+{#    This program is free software: you can redistribute it and/or modify#}
+{#    it under the terms of the GNU Affero General Public License as published#}
+{#    by the Free Software Foundation, either version 3 of the License.#}
+{#    #}
+{##}
+{#    This program is distributed in the hope that it will be useful,#}
+{#    but WITHOUT ANY WARRANTY; without even the implied warranty of#}
+{#    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the#}
+{#    GNU Affero General Public License for more details.#}
+{##}
+{#    You should have received a copy of the GNU Affero General Public License#}
+{#    along with this program.  If not, see <http://www.gnu.org/licenses/>.#}
+{##}
+{###############################################################################}
+
+{% if field.is_hidden %}
+    {{ field }}
+{% else %}
+    <div id="div_{{ field.auto_id }}" class="form-group{% if form_show_errors and field.errors %} has-error{% endif %}{% if field.css_classes %} {{ field.css_classes }}{% endif %}">
+
+        {% if field.label %}
+            <label for="{{ field.auto_id }}"  class="control-label {{ label_class }}{% if field.field.required %} requiredField{% endif %}">
+                {{ field.label|safe }}{% if field.field.required %}<span class="asteriskField">*</span>{% endif %}
+            </label>
+        {% endif %}
+
+        {% include 'bootstrap3/layout/checkboxselectmultiple.html' %}
+    </div>
+{% endif %}
```

### Comparing `nobinobi-core-0.1.4.6/nobinobi_core/templates/layout/checkboxselectmultiple_inline_image.html` & `nobinobi-core-0.1.4.7/nobinobi_core/templates/layout/checkboxselectmultiple_inline_act.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-{###############################################################################}
-{##}
-{#   Copyright (C) <2016>  <Florian Alu - Prolibre - http://prolibre.com>#}
-{##}
-{#    This program is free software: you can redistribute it and/or modify#}
-{#    it under the terms of the GNU Affero General Public License as published#}
-{#    by the Free Software Foundation, either version 3 of the License.#}
-{#    #}
-{##}
-{#    This program is distributed in the hope that it will be useful,#}
-{#    but WITHOUT ANY WARRANTY; without even the implied warranty of#}
-{#    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the#}
-{#    GNU Affero General Public License for more details.#}
-{##}
-{#    You should have received a copy of the GNU Affero General Public License#}
-{#    along with this program.  If not, see <http://www.gnu.org/licenses/>.#}
-{##}
-{###############################################################################}
-
-{% if field.is_hidden %}
-    {{ field }}
-{% else %}
-    <div id="div_{{ field.auto_id }}" class="form-group{% if form_show_errors and field.errors %} has-error{% endif %}{% if field.css_classes %} {{ field.css_classes }}{% endif %}">
-
-        {% if field.label %}
-            <label for="{{ field.auto_id }}"  class="control-label {{ label_class }}{% if field.field.required %} requiredField{% endif %}">
-                {{ field.label|safe }}{% if field.field.required %}<span class="asteriskField">*</span>{% endif %}
-            </label>
-        {% endif %}
-
-        {% include 'layout/checkboxselectmultiple_image.html' %}
-    </div>
-{% endif %}
+{###############################################################################}
+{##}
+{#   Copyright (C) <2016>  <Florian Alu - Prolibre - http://prolibre.com>#}
+{##}
+{#    This program is free software: you can redistribute it and/or modify#}
+{#    it under the terms of the GNU Affero General Public License as published#}
+{#    by the Free Software Foundation, either version 3 of the License.#}
+{#    #}
+{##}
+{#    This program is distributed in the hope that it will be useful,#}
+{#    but WITHOUT ANY WARRANTY; without even the implied warranty of#}
+{#    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the#}
+{#    GNU Affero General Public License for more details.#}
+{##}
+{#    You should have received a copy of the GNU Affero General Public License#}
+{#    along with this program.  If not, see <http://www.gnu.org/licenses/>.#}
+{##}
+{###############################################################################}
+
+{% if field.is_hidden %}
+    {{ field }}
+{% else %}
+    <div id="div_{{ field.auto_id }}" class="form-group{% if form_show_errors and field.errors %} has-error{% endif %}{% if field.css_classes %} {{ field.css_classes }}{% endif %}">
+
+        {% if field.label %}
+            <label for="{{ field.auto_id }}"  class="control-label {{ label_class }}{% if field.field.required %} requiredField{% endif %}">
+                {{ field.label|safe }}{% if field.field.required %}<span class="asteriskField">*</span>{% endif %}
+            </label>
+        {% endif %}
+
+        {% include 'layout/checkboxselectmultiple_act.html' %}
+    </div>
+{% endif %}
```

### Comparing `nobinobi-core-0.1.4.6/nobinobi_core/templates/layout/field_errors_block.html` & `nobinobi-core-0.1.4.7/nobinobi_core/templates/layout/field_errors_block.html`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-{###############################################################################}
-{##}
-{#   Copyright (C) <2016>  <Florian Alu - Prolibre - http://prolibre.com>#}
-{##}
-{#    This program is free software: you can redistribute it and/or modify#}
-{#    it under the terms of the GNU Affero General Public License as published#}
-{#    by the Free Software Foundation, either version 3 of the License.#}
-{#    #}
-{##}
-{#    This program is distributed in the hope that it will be useful,#}
-{#    but WITHOUT ANY WARRANTY; without even the implied warranty of#}
-{#    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the#}
-{#    GNU Affero General Public License for more details.#}
-{##}
-{#    You should have received a copy of the GNU Affero General Public License#}
-{#    along with this program.  If not, see <http://www.gnu.org/licenses/>.#}
-{##}
-{###############################################################################}
-
-{% if form_show_errors and field.errors %}
-    {% for error in field.errors %}
-        <p id="error_{{ forloop.counter }}_{{ field.auto_id }}" class="help-block"><strong>{{ error }}</strong></p>
-    {% endfor %}
-{% endif %}
+{###############################################################################}
+{##}
+{#   Copyright (C) <2016>  <Florian Alu - Prolibre - http://prolibre.com>#}
+{##}
+{#    This program is free software: you can redistribute it and/or modify#}
+{#    it under the terms of the GNU Affero General Public License as published#}
+{#    by the Free Software Foundation, either version 3 of the License.#}
+{#    #}
+{##}
+{#    This program is distributed in the hope that it will be useful,#}
+{#    but WITHOUT ANY WARRANTY; without even the implied warranty of#}
+{#    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the#}
+{#    GNU Affero General Public License for more details.#}
+{##}
+{#    You should have received a copy of the GNU Affero General Public License#}
+{#    along with this program.  If not, see <http://www.gnu.org/licenses/>.#}
+{##}
+{###############################################################################}
+
+{% if form_show_errors and field.errors %}
+    {% for error in field.errors %}
+        <p id="error_{{ forloop.counter }}_{{ field.auto_id }}" class="help-block"><strong>{{ error }}</strong></p>
+    {% endfor %}
+{% endif %}
```

### Comparing `nobinobi-core-0.1.4.6/nobinobi_core/templates/layout/help_text.html` & `nobinobi-core-0.1.4.7/nobinobi_core/templates/layout/help_text.html`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-{###############################################################################}
-{##}
-{#   Copyright (C) <2016>  <Florian Alu - Prolibre - http://prolibre.com>#}
-{##}
-{#    This program is free software: you can redistribute it and/or modify#}
-{#    it under the terms of the GNU Affero General Public License as published#}
-{#    by the Free Software Foundation, either version 3 of the License.#}
-{#    #}
-{##}
-{#    This program is distributed in the hope that it will be useful,#}
-{#    but WITHOUT ANY WARRANTY; without even the implied warranty of#}
-{#    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the#}
-{#    GNU Affero General Public License for more details.#}
-{##}
-{#    You should have received a copy of the GNU Affero General Public License#}
-{#    along with this program.  If not, see <http://www.gnu.org/licenses/>.#}
-{##}
-{###############################################################################}
-
-{% if field.help_text %}
-    {% if help_text_inline %}
-        <span id="hint_{{ field.auto_id }}" class="help-block">{{ field.help_text|safe }}</span>
-    {% else %}
-        <p id="hint_{{ field.auto_id }}" class="help-block">{{ field.help_text|safe }}</p>
-    {% endif %}
-{% endif %}
+{###############################################################################}
+{##}
+{#   Copyright (C) <2016>  <Florian Alu - Prolibre - http://prolibre.com>#}
+{##}
+{#    This program is free software: you can redistribute it and/or modify#}
+{#    it under the terms of the GNU Affero General Public License as published#}
+{#    by the Free Software Foundation, either version 3 of the License.#}
+{#    #}
+{##}
+{#    This program is distributed in the hope that it will be useful,#}
+{#    but WITHOUT ANY WARRANTY; without even the implied warranty of#}
+{#    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the#}
+{#    GNU Affero General Public License for more details.#}
+{##}
+{#    You should have received a copy of the GNU Affero General Public License#}
+{#    along with this program.  If not, see <http://www.gnu.org/licenses/>.#}
+{##}
+{###############################################################################}
+
+{% if field.help_text %}
+    {% if help_text_inline %}
+        <span id="hint_{{ field.auto_id }}" class="help-block">{{ field.help_text|safe }}</span>
+    {% else %}
+        <p id="hint_{{ field.auto_id }}" class="help-block">{{ field.help_text|safe }}</p>
+    {% endif %}
+{% endif %}
```

### Comparing `nobinobi-core-0.1.4.6/nobinobi_core/templates/layout/radioselect.html` & `nobinobi-core-0.1.4.7/nobinobi_core/templates/layout/radioselect.html`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-{###############################################################################}
-{##}
-{#   Copyright (C) <2016>  <Florian Alu - Prolibre - http://prolibre.com>#}
-{##}
-{#    This program is free software: you can redistribute it and/or modify#}
-{#    it under the terms of the GNU Affero General Public License as published#}
-{#    by the Free Software Foundation, either version 3 of the License.#}
-{#    #}
-{##}
-{#    This program is distributed in the hope that it will be useful,#}
-{#    but WITHOUT ANY WARRANTY; without even the implied warranty of#}
-{#    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the#}
-{#    GNU Affero General Public License for more details.#}
-{##}
-{#    You should have received a copy of the GNU Affero General Public License#}
-{#    along with this program.  If not, see <http://www.gnu.org/licenses/>.#}
-{##}
-{###############################################################################}
-
-{% load crispy_forms_filters %}
-{% load l10n %}
-
-<div class="controls {{ field_class }}"{% if flat_attrs %} {{ flat_attrs|safe }}{% endif %}>
-    {% include 'bootstrap3/layout/field_errors_block.html' %}
-
-    {% for choice in field.field.choices %}
-      {% if not inline_class %}<div class="radio">{% endif %}
-        <label class="{% if inline_class %}radio-{{ inline_class }}{% endif %}">
-            <input type="radio"{% if choice.0|stringformat:"s" == field.value|stringformat:"s" %} checked="checked"{% endif %} name="{{ field.html_name }}" id="id_{{ field.html_name }}_{{ forloop.counter }}" value="{{ choice.0|unlocalize }}" {{ field.field.widget.attrs|flatatt }}>{{ choice.1|unlocalize }}
-        </label>
-      {% if not inline_class %}</div>{% endif %}
-    {% endfor %}
-
-    {% include 'bootstrap3/layout/help_text.html' %}
-</div>
+{###############################################################################}
+{##}
+{#   Copyright (C) <2016>  <Florian Alu - Prolibre - http://prolibre.com>#}
+{##}
+{#    This program is free software: you can redistribute it and/or modify#}
+{#    it under the terms of the GNU Affero General Public License as published#}
+{#    by the Free Software Foundation, either version 3 of the License.#}
+{#    #}
+{##}
+{#    This program is distributed in the hope that it will be useful,#}
+{#    but WITHOUT ANY WARRANTY; without even the implied warranty of#}
+{#    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the#}
+{#    GNU Affero General Public License for more details.#}
+{##}
+{#    You should have received a copy of the GNU Affero General Public License#}
+{#    along with this program.  If not, see <http://www.gnu.org/licenses/>.#}
+{##}
+{###############################################################################}
+
+{% load crispy_forms_filters %}
+{% load l10n %}
+
+<div class="controls {{ field_class }}"{% if flat_attrs %} {{ flat_attrs|safe }}{% endif %}>
+    {% include 'bootstrap3/layout/field_errors_block.html' %}
+
+    {% for choice in field.field.choices %}
+      {% if not inline_class %}<div class="radio">{% endif %}
+        <label class="{% if inline_class %}radio-{{ inline_class }}{% endif %}">
+            <input type="radio"{% if choice.0|stringformat:"s" == field.value|stringformat:"s" %} checked="checked"{% endif %} name="{{ field.html_name }}" id="id_{{ field.html_name }}_{{ forloop.counter }}" value="{{ choice.0|unlocalize }}" {{ field.field.widget.attrs|flatatt }}>{{ choice.1|unlocalize }}
+        </label>
+      {% if not inline_class %}</div>{% endif %}
+    {% endfor %}
+
+    {% include 'bootstrap3/layout/help_text.html' %}
+</div>
```

### Comparing `nobinobi-core-0.1.4.6/nobinobi_core/templates/layout/radioselect_image.html` & `nobinobi-core-0.1.4.7/nobinobi_core/templates/layout/radioselect_image.html`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-{###############################################################################}
-{##}
-{#   Copyright (C) <2016>  <Florian Alu - Prolibre - http://prolibre.com>#}
-{##}
-{#    This program is free software: you can redistribute it and/or modify#}
-{#    it under the terms of the GNU Affero General Public License as published#}
-{#    by the Free Software Foundation, either version 3 of the License.#}
-{#    #}
-{##}
-{#    This program is distributed in the hope that it will be useful,#}
-{#    but WITHOUT ANY WARRANTY; without even the implied warranty of#}
-{#    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the#}
-{#    GNU Affero General Public License for more details.#}
-{##}
-{#    You should have received a copy of the GNU Affero General Public License#}
-{#    along with this program.  If not, see <http://www.gnu.org/licenses/>.#}
-{##}
-{###############################################################################}
-
-{% load crispy_forms_filters %}
-{% load l10n %}
-{% load static %}
-
-<div class="controls {{ field_class }}"{% if flat_attrs %} {{ flat_attrs|safe }}{% endif %}>
-  {% include 'layout/field_errors_block.html' %}
-
-  {% for choice in field.field.choices %}
-    {% if not inline_class %}
-      <div class="radio">{% endif %}
-  <label class="{% if inline_class %}radio-{{ inline_class }}{% endif %}">
-    <input type="radio"{% if choice.0|stringformat:"s" == field.value|stringformat:"s" %}
-           checked="checked"{% endif %} name="{{ field.html_name }}"
-           id="id_{{ field.html_name }}_{{ forloop.counter }}"
-           value="{{ choice.0|unlocalize }}" {{ field.field.widget.attrs|flatatt }}>
-    {% if choice.0 == None or choice.0 == "" %}
-      <img class='img-fluid' width="100px" src='{% static "img/smiley/question.png" %}'/>
-    {% else %}
-      <img class='img-fluid' width="100px" src='{% static "img/smiley/" %}{{ choice.1|unlocalize }}'/>
-    {% endif %}
-  </label>
-  {% if not inline_class %}</div>{% endif %}
-  {% endfor %}
-
-  {% include 'layout/help_text.html' %}
-</div>
+{###############################################################################}
+{##}
+{#   Copyright (C) <2016>  <Florian Alu - Prolibre - http://prolibre.com>#}
+{##}
+{#    This program is free software: you can redistribute it and/or modify#}
+{#    it under the terms of the GNU Affero General Public License as published#}
+{#    by the Free Software Foundation, either version 3 of the License.#}
+{#    #}
+{##}
+{#    This program is distributed in the hope that it will be useful,#}
+{#    but WITHOUT ANY WARRANTY; without even the implied warranty of#}
+{#    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the#}
+{#    GNU Affero General Public License for more details.#}
+{##}
+{#    You should have received a copy of the GNU Affero General Public License#}
+{#    along with this program.  If not, see <http://www.gnu.org/licenses/>.#}
+{##}
+{###############################################################################}
+
+{% load crispy_forms_filters %}
+{% load l10n %}
+{% load static %}
+
+<div class="controls {{ field_class }}"{% if flat_attrs %} {{ flat_attrs|safe }}{% endif %}>
+  {% include 'layout/field_errors_block.html' %}
+
+  {% for choice in field.field.choices %}
+    {% if not inline_class %}
+      <div class="radio">{% endif %}
+  <label class="{% if inline_class %}radio-{{ inline_class }}{% endif %}">
+    <input type="radio"{% if choice.0|stringformat:"s" == field.value|stringformat:"s" %}
+           checked="checked"{% endif %} name="{{ field.html_name }}"
+           id="id_{{ field.html_name }}_{{ forloop.counter }}"
+           value="{{ choice.0|unlocalize }}" {{ field.field.widget.attrs|flatatt }}>
+    {% if choice.0 == None or choice.0 == "" %}
+      <img class='img-fluid' width="100px" src='{% static "img/smiley/question.png" %}'/>
+    {% else %}
+      <img class='img-fluid' width="100px" src='{% static "img/smiley/" %}{{ choice.1|unlocalize }}'/>
+    {% endif %}
+  </label>
+  {% if not inline_class %}</div>{% endif %}
+  {% endfor %}
+
+  {% include 'layout/help_text.html' %}
+</div>
```

### Comparing `nobinobi-core-0.1.4.6/nobinobi_core/templates/layout/radioselect_inline.html` & `nobinobi-core-0.1.4.7/nobinobi_core/templates/layout/radioselect_inline.html`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-{###############################################################################}
-{##}
-{#   Copyright (C) <2016>  <Florian Alu - Prolibre - http://prolibre.com>#}
-{##}
-{#    This program is free software: you can redistribute it and/or modify#}
-{#    it under the terms of the GNU Affero General Public License as published#}
-{#    by the Free Software Foundation, either version 3 of the License.#}
-{#    #}
-{##}
-{#    This program is distributed in the hope that it will be useful,#}
-{#    but WITHOUT ANY WARRANTY; without even the implied warranty of#}
-{#    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the#}
-{#    GNU Affero General Public License for more details.#}
-{##}
-{#    You should have received a copy of the GNU Affero General Public License#}
-{#    along with this program.  If not, see <http://www.gnu.org/licenses/>.#}
-{##}
-{###############################################################################}
-
-{% if field.is_hidden %}
-    {{ field }}
-{% else %}
-    <div id="div_{{ field.auto_id }}" class="form-group{% if wrapper_class %} {{ wrapper_class }}{% endif %}{% if form_show_errors and field.errors %} has-error{% endif %}{% if field.css_classes %} {{ field.css_classes }}{% endif %}">
-
-        {% if field.label %}
-            <label for="{{ field.auto_id }}"  class="control-label {{ label_class }}{% if field.field.required %} requiredField{% endif %}">
-                {{ field.label|safe }}{% if field.field.required %}<span class="asteriskField">*</span>{% endif %}
-            </label>
-        {% endif %}
-
-        {% include 'layout/radioselect.html' %}
-    </div>
-{% endif %}
+{###############################################################################}
+{##}
+{#   Copyright (C) <2016>  <Florian Alu - Prolibre - http://prolibre.com>#}
+{##}
+{#    This program is free software: you can redistribute it and/or modify#}
+{#    it under the terms of the GNU Affero General Public License as published#}
+{#    by the Free Software Foundation, either version 3 of the License.#}
+{#    #}
+{##}
+{#    This program is distributed in the hope that it will be useful,#}
+{#    but WITHOUT ANY WARRANTY; without even the implied warranty of#}
+{#    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the#}
+{#    GNU Affero General Public License for more details.#}
+{##}
+{#    You should have received a copy of the GNU Affero General Public License#}
+{#    along with this program.  If not, see <http://www.gnu.org/licenses/>.#}
+{##}
+{###############################################################################}
+
+{% if field.is_hidden %}
+    {{ field }}
+{% else %}
+    <div id="div_{{ field.auto_id }}" class="form-group{% if wrapper_class %} {{ wrapper_class }}{% endif %}{% if form_show_errors and field.errors %} has-error{% endif %}{% if field.css_classes %} {{ field.css_classes }}{% endif %}">
+
+        {% if field.label %}
+            <label for="{{ field.auto_id }}"  class="control-label {{ label_class }}{% if field.field.required %} requiredField{% endif %}">
+                {{ field.label|safe }}{% if field.field.required %}<span class="asteriskField">*</span>{% endif %}
+            </label>
+        {% endif %}
+
+        {% include 'layout/radioselect.html' %}
+    </div>
+{% endif %}
```

### Comparing `nobinobi-core-0.1.4.6/nobinobi_core/templates/layout/radioselect_inline_image.html` & `nobinobi-core-0.1.4.7/nobinobi_core/templates/layout/checkboxselectmultiple_inline_image.html`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-{###############################################################################}
-{##}
-{#   Copyright (C) <2016>  <Florian Alu - Prolibre - http://prolibre.com>#}
-{##}
-{#    This program is free software: you can redistribute it and/or modify#}
-{#    it under the terms of the GNU Affero General Public License as published#}
-{#    by the Free Software Foundation, either version 3 of the License.#}
-{#    #}
-{##}
-{#    This program is distributed in the hope that it will be useful,#}
-{#    but WITHOUT ANY WARRANTY; without even the implied warranty of#}
-{#    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the#}
-{#    GNU Affero General Public License for more details.#}
-{##}
-{#    You should have received a copy of the GNU Affero General Public License#}
-{#    along with this program.  If not, see <http://www.gnu.org/licenses/>.#}
-{##}
-{###############################################################################}
-
-{% if field.is_hidden %}
-    {{ field }}
-{% else %}
-    <div id="div_{{ field.auto_id }}" class="form-group{% if wrapper_class %} {{ wrapper_class }}{% endif %}{% if form_show_errors and field.errors %} has-error{% endif %}{% if field.css_classes %} {{ field.css_classes }}{% endif %}">
-
-        {% if field.label %}
-            <label for="{{ field.auto_id }}"  class="control-label {{ label_class }}{% if field.field.required %} requiredField{% endif %}">
-                {{ field.label|safe }}{% if field.field.required %}<span class="asteriskField">*</span>{% endif %}
-            </label>
-        {% endif %}
-
-        {% include 'layout/radioselect_image.html' %}
-    </div>
-{% endif %}
+{###############################################################################}
+{##}
+{#   Copyright (C) <2016>  <Florian Alu - Prolibre - http://prolibre.com>#}
+{##}
+{#    This program is free software: you can redistribute it and/or modify#}
+{#    it under the terms of the GNU Affero General Public License as published#}
+{#    by the Free Software Foundation, either version 3 of the License.#}
+{#    #}
+{##}
+{#    This program is distributed in the hope that it will be useful,#}
+{#    but WITHOUT ANY WARRANTY; without even the implied warranty of#}
+{#    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the#}
+{#    GNU Affero General Public License for more details.#}
+{##}
+{#    You should have received a copy of the GNU Affero General Public License#}
+{#    along with this program.  If not, see <http://www.gnu.org/licenses/>.#}
+{##}
+{###############################################################################}
+
+{% if field.is_hidden %}
+    {{ field }}
+{% else %}
+    <div id="div_{{ field.auto_id }}" class="form-group{% if form_show_errors and field.errors %} has-error{% endif %}{% if field.css_classes %} {{ field.css_classes }}{% endif %}">
+
+        {% if field.label %}
+            <label for="{{ field.auto_id }}"  class="control-label {{ label_class }}{% if field.field.required %} requiredField{% endif %}">
+                {{ field.label|safe }}{% if field.field.required %}<span class="asteriskField">*</span>{% endif %}
+            </label>
+        {% endif %}
+
+        {% include 'layout/checkboxselectmultiple_image.html' %}
+    </div>
+{% endif %}
```

### Comparing `nobinobi-core-0.1.4.6/nobinobi_core/templates/layout/sj/collation_general.html` & `nobinobi-core-0.1.4.7/nobinobi_core/templates/layout/sj/collation_general.html`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-{###############################################################################}
-{##}
-{#   Copyright (C) <2016>  <Florian Alu - Prolibre - http://prolibre.com>#}
-{##}
-{#    This program is free software: you can redistribute it and/or modify#}
-{#    it under the terms of the GNU Affero General Public License as published#}
-{#    by the Free Software Foundation, either version 3 of the License.#}
-{#    #}
-{##}
-{#    This program is distributed in the hope that it will be useful,#}
-{#    but WITHOUT ANY WARRANTY; without even the implied warranty of#}
-{#    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the#}
-{#    GNU Affero General Public License for more details.#}
-{##}
-{#    You should have received a copy of the GNU Affero General Public License#}
-{#    along with this program.  If not, see <http://www.gnu.org/licenses/>.#}
-{##}
-{###############################################################################}
-
-    <fieldset {% if fieldset.css_id %}id="{{ fieldset.css_id }}"{% endif %}
-              {% if fieldset.css_class or form_style %}class="{{ fieldset.css_class }} {{ form_style }}"{% endif %}
-            {{ fieldset.flat_attrs|safe }}>
-        {% if legend %}
-            <legend>{{ legend|safe }}</legend>
-        {% endif %}
-        {{ fields|safe }}
-
-    </fieldset>
-
+{###############################################################################}
+{##}
+{#   Copyright (C) <2016>  <Florian Alu - Prolibre - http://prolibre.com>#}
+{##}
+{#    This program is free software: you can redistribute it and/or modify#}
+{#    it under the terms of the GNU Affero General Public License as published#}
+{#    by the Free Software Foundation, either version 3 of the License.#}
+{#    #}
+{##}
+{#    This program is distributed in the hope that it will be useful,#}
+{#    but WITHOUT ANY WARRANTY; without even the implied warranty of#}
+{#    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the#}
+{#    GNU Affero General Public License for more details.#}
+{##}
+{#    You should have received a copy of the GNU Affero General Public License#}
+{#    along with this program.  If not, see <http://www.gnu.org/licenses/>.#}
+{##}
+{###############################################################################}
+
+    <fieldset {% if fieldset.css_id %}id="{{ fieldset.css_id }}"{% endif %}
+              {% if fieldset.css_class or form_style %}class="{{ fieldset.css_class }} {{ form_style }}"{% endif %}
+            {{ fieldset.flat_attrs|safe }}>
+        {% if legend %}
+            <legend>{{ legend|safe }}</legend>
+        {% endif %}
+        {{ fields|safe }}
+
+    </fieldset>
+
 {#{% endif %}#}
```

### Comparing `nobinobi-core-0.1.4.6/nobinobi_core/templates/nobinobi_core/base.html` & `nobinobi-core-0.1.4.7/nobinobi_core/templates/nobinobi_core/base.html`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.6/nobinobi_core/templatetags/__init__.py` & `nobinobi-core-0.1.4.7/nobinobi_core/templatetags/__init__.py`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.6/nobinobi_core/templatetags/get_dict_value.py` & `nobinobi-core-0.1.4.7/nobinobi_core/templatetags/get_dict_value.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-#      Copyright (C) 2020 <Florian Alu - Prolibre - https://prolibre.com
-#      This program is free software: you can redistribute it and/or modify
-#      it under the terms of the GNU Affero General Public License as
-#      published by the Free Software Foundation, either version 3 of the
-#      License, or (at your option) any later version.
-#
-#      This program is distributed in the hope that it will be useful,
-#      but WITHOUT ANY WARRANTY; without even the implied warranty of
-#      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#      GNU Affero General Public License for more details.
-#
-#      You should have received a copy of the GNU Affero General Public License
-#      along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-# -*- coding: utf-8 -*-
-
-from django.template.defaultfilters import register
-
-
-@register.filter
-def get(dict, key, default=''):
-    """
-    Usage:
-
-    view:
-    some_dict = {'keyA':'valueA','keyB':{'subKeyA':'subValueA','subKeyB':'subKeyB'},'keyC':'valueC'}
-    keys = ['keyA','keyC']
-    template:
-    {{ some_dict|get:"keyA" }}
-    {{ some_dict|get:"keyB"|get:"subKeyA" }}
-    {% for key in keys %}{{ some_dict|get:key }}{% endfor %}
-    """
-
-    try:
-        return dict.get(key, default)
-    except:
-        return default
-
-
-@register.filter
-def get_dict_items(dict, key, default=''):
-    """
-    Usage:
-
-    view:
-    some_dict = {'keyA':'valueA','keyB':{'subKeyA':'subValueA','subKeyB':'subKeyB'},'keyC':'valueC'}
-    keys = ['keyA','keyC']
-    template:
-    {{ some_dict|get:"keyA" }}
-    {{ some_dict|get:"keyB"|get:"subKeyA" }}
-    {% for key in keys %}{{ some_dict|get:key }}{% endfor %}
-    """
-    return dict[key].items()
-
-
-@register.filter
-def index(List, i):
-    return List[int(i)]
+#      Copyright (C) 2020 <Florian Alu - Prolibre - https://prolibre.com
+#      This program is free software: you can redistribute it and/or modify
+#      it under the terms of the GNU Affero General Public License as
+#      published by the Free Software Foundation, either version 3 of the
+#      License, or (at your option) any later version.
+#
+#      This program is distributed in the hope that it will be useful,
+#      but WITHOUT ANY WARRANTY; without even the implied warranty of
+#      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#      GNU Affero General Public License for more details.
+#
+#      You should have received a copy of the GNU Affero General Public License
+#      along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+# -*- coding: utf-8 -*-
+
+from django.template.defaultfilters import register
+
+
+@register.filter
+def get(dict, key, default=''):
+    """
+    Usage:
+
+    view:
+    some_dict = {'keyA':'valueA','keyB':{'subKeyA':'subValueA','subKeyB':'subKeyB'},'keyC':'valueC'}
+    keys = ['keyA','keyC']
+    template:
+    {{ some_dict|get:"keyA" }}
+    {{ some_dict|get:"keyB"|get:"subKeyA" }}
+    {% for key in keys %}{{ some_dict|get:key }}{% endfor %}
+    """
+
+    try:
+        return dict.get(key, default)
+    except:
+        return default
+
+
+@register.filter
+def get_dict_items(dict, key, default=''):
+    """
+    Usage:
+
+    view:
+    some_dict = {'keyA':'valueA','keyB':{'subKeyA':'subValueA','subKeyB':'subKeyB'},'keyC':'valueC'}
+    keys = ['keyA','keyC']
+    template:
+    {{ some_dict|get:"keyA" }}
+    {{ some_dict|get:"keyB"|get:"subKeyA" }}
+    {% for key in keys %}{{ some_dict|get:key }}{% endfor %}
+    """
+    return dict[key].items()
+
+
+@register.filter
+def index(List, i):
+    return List[int(i)]
```

### Comparing `nobinobi-core-0.1.4.6/nobinobi_core/templatetags/get_user_method.py` & `nobinobi-core-0.1.4.7/nobinobi_core/templatetags/remove_date_sem.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,27 @@
-#      Copyright (C) 2020 <Florian Alu - Prolibre - https://prolibre.com
-#      This program is free software: you can redistribute it and/or modify
-#      it under the terms of the GNU Affero General Public License as
-#      published by the Free Software Foundation, either version 3 of the
-#      License, or (at your option) any later version.
-#
-#      This program is distributed in the hope that it will be useful,
-#      but WITHOUT ANY WARRANTY; without even the implied warranty of
-#      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#      GNU Affero General Public License for more details.
-#
-#      You should have received a copy of the GNU Affero General Public License
-#      along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-
-from django import template
-
-register = template.Library()
-
-
-@register.filter(name='has_group')
-def has_group(user, group_name):
-    return user.groups.filter(name=group_name).exists()
+#      Copyright (C) 2020 <Florian Alu - Prolibre - https://prolibre.com
+#      This program is free software: you can redistribute it and/or modify
+#      it under the terms of the GNU Affero General Public License as
+#      published by the Free Software Foundation, either version 3 of the
+#      License, or (at your option) any later version.
+#
+#      This program is distributed in the hope that it will be useful,
+#      but WITHOUT ANY WARRANTY; without even the implied warranty of
+#      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#      GNU Affero General Public License for more details.
+#
+#      You should have received a copy of the GNU Affero General Public License
+#      along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+# -*- coding: utf-8 -*-
+
+from django.template.defaultfilters import register
+
+
+@register.filter
+def substract(val):
+    """
+    Usage:
+    """
+    val = int(val) - 1
+
+    return val
```

### Comparing `nobinobi-core-0.1.4.6/nobinobi_core/templatetags/math.py` & `nobinobi-core-0.1.4.7/nobinobi_core/templatetags/math.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-#      Copyright (C) 2020 <Florian Alu - Prolibre - https://prolibre.com
-#      This program is free software: you can redistribute it and/or modify
-#      it under the terms of the GNU Affero General Public License as
-#      published by the Free Software Foundation, either version 3 of the
-#      License, or (at your option) any later version.
-#
-#      This program is distributed in the hope that it will be useful,
-#      but WITHOUT ANY WARRANTY; without even the implied warranty of
-#      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#      GNU Affero General Public License for more details.
-#
-#      You should have received a copy of the GNU Affero General Public License
-#      along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-# -*- coding: utf-8 -*-
-import datetime
-
-from django import template
-
-register = template.Library()
-
-
-@register.filter
-def subtract(value, arg):
-    return value - arg
-
-
-@register.simple_tag(takes_context=True)
-def subtractify(context, obj, obj2):
-    newval = obj - obj2
-    return "%.1f" % newval
-
-
-@register.simple_tag()
-def multiply(qty, unit_price, *args, **kwargs):
-    # you would need to do any localization of the result here
-    return qty * unit_price
-
-
-@register.simple_tag()
-def get_pourcentage(value, pourcentage, ref, *args, **kwargs):
-    # 4 × 100 ÷ 8 = 50 =====0
-    if type(value) == datetime.timedelta:
-        value = value.total_seconds()
-    if type(ref) == datetime.timedelta:
-        ref = ref.total_seconds()
-
-    try:
-        return float(value) * int(pourcentage) / float(ref)
-    except ZeroDivisionError:
-        return 0
+#      Copyright (C) 2020 <Florian Alu - Prolibre - https://prolibre.com
+#      This program is free software: you can redistribute it and/or modify
+#      it under the terms of the GNU Affero General Public License as
+#      published by the Free Software Foundation, either version 3 of the
+#      License, or (at your option) any later version.
+#
+#      This program is distributed in the hope that it will be useful,
+#      but WITHOUT ANY WARRANTY; without even the implied warranty of
+#      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#      GNU Affero General Public License for more details.
+#
+#      You should have received a copy of the GNU Affero General Public License
+#      along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+# -*- coding: utf-8 -*-
+import datetime
+
+from django import template
+
+register = template.Library()
+
+
+@register.filter
+def subtract(value, arg):
+    return value - arg
+
+
+@register.simple_tag(takes_context=True)
+def subtractify(context, obj, obj2):
+    newval = obj - obj2
+    return "%.1f" % newval
+
+
+@register.simple_tag()
+def multiply(qty, unit_price, *args, **kwargs):
+    # you would need to do any localization of the result here
+    return qty * unit_price
+
+
+@register.simple_tag()
+def get_pourcentage(value, pourcentage, ref, *args, **kwargs):
+    # 4 × 100 ÷ 8 = 50 =====0
+    if type(value) == datetime.timedelta:
+        value = value.total_seconds()
+    if type(ref) == datetime.timedelta:
+        ref = ref.total_seconds()
+
+    try:
+        return float(value) * int(pourcentage) / float(ref)
+    except ZeroDivisionError:
+        return 0
```

### Comparing `nobinobi-core-0.1.4.6/nobinobi_core/templatetags/notifications_tags_custom.py` & `nobinobi-core-0.1.4.7/nobinobi_core/templatetags/notifications_tags_custom.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,213 +1,220 @@
 00000000: 2320 2020 2020 2043 6f70 7972 6967 6874  #      Copyright
 00000010: 2028 4329 2032 3032 3020 3c46 6c6f 7269   (C) 2020 <Flori
 00000020: 616e 2041 6c75 202d 2050 726f 6c69 6272  an Alu - Prolibr
 00000030: 6520 2d20 6874 7470 733a 2f2f 7072 6f6c  e - https://prol
-00000040: 6962 7265 2e63 6f6d 0a23 2020 2020 2020  ibre.com.#      
-00000050: 5468 6973 2070 726f 6772 616d 2069 7320  This program is 
-00000060: 6672 6565 2073 6f66 7477 6172 653a 2079  free software: y
-00000070: 6f75 2063 616e 2072 6564 6973 7472 6962  ou can redistrib
-00000080: 7574 6520 6974 2061 6e64 2f6f 7220 6d6f  ute it and/or mo
-00000090: 6469 6679 0a23 2020 2020 2020 6974 2075  dify.#      it u
-000000a0: 6e64 6572 2074 6865 2074 6572 6d73 206f  nder the terms o
-000000b0: 6620 7468 6520 474e 5520 4166 6665 726f  f the GNU Affero
-000000c0: 2047 656e 6572 616c 2050 7562 6c69 6320   General Public 
-000000d0: 4c69 6365 6e73 6520 6173 0a23 2020 2020  License as.#    
-000000e0: 2020 7075 626c 6973 6865 6420 6279 2074    published by t
-000000f0: 6865 2046 7265 6520 536f 6674 7761 7265  he Free Software
-00000100: 2046 6f75 6e64 6174 696f 6e2c 2065 6974   Foundation, eit
-00000110: 6865 7220 7665 7273 696f 6e20 3320 6f66  her version 3 of
-00000120: 2074 6865 0a23 2020 2020 2020 4c69 6365   the.#      Lice
-00000130: 6e73 652c 206f 7220 2861 7420 796f 7572  nse, or (at your
-00000140: 206f 7074 696f 6e29 2061 6e79 206c 6174   option) any lat
-00000150: 6572 2076 6572 7369 6f6e 2e0a 230a 2320  er version..#.# 
-00000160: 2020 2020 2054 6869 7320 7072 6f67 7261       This progra
-00000170: 6d20 6973 2064 6973 7472 6962 7574 6564  m is distributed
-00000180: 2069 6e20 7468 6520 686f 7065 2074 6861   in the hope tha
-00000190: 7420 6974 2077 696c 6c20 6265 2075 7365  t it will be use
-000001a0: 6675 6c2c 0a23 2020 2020 2020 6275 7420  ful,.#      but 
-000001b0: 5749 5448 4f55 5420 414e 5920 5741 5252  WITHOUT ANY WARR
-000001c0: 414e 5459 3b20 7769 7468 6f75 7420 6576  ANTY; without ev
-000001d0: 656e 2074 6865 2069 6d70 6c69 6564 2077  en the implied w
-000001e0: 6172 7261 6e74 7920 6f66 0a23 2020 2020  arranty of.#    
-000001f0: 2020 4d45 5243 4841 4e54 4142 494c 4954    MERCHANTABILIT
-00000200: 5920 6f72 2046 4954 4e45 5353 2046 4f52  Y or FITNESS FOR
-00000210: 2041 2050 4152 5449 4355 4c41 5220 5055   A PARTICULAR PU
-00000220: 5250 4f53 452e 2020 5365 6520 7468 650a  RPOSE.  See the.
-00000230: 2320 2020 2020 2047 4e55 2041 6666 6572  #      GNU Affer
-00000240: 6f20 4765 6e65 7261 6c20 5075 626c 6963  o General Public
-00000250: 204c 6963 656e 7365 2066 6f72 206d 6f72   License for mor
-00000260: 6520 6465 7461 696c 732e 0a23 0a23 2020  e details..#.#  
-00000270: 2020 2020 596f 7520 7368 6f75 6c64 2068      You should h
-00000280: 6176 6520 7265 6365 6976 6564 2061 2063  ave received a c
-00000290: 6f70 7920 6f66 2074 6865 2047 4e55 2041  opy of the GNU A
-000002a0: 6666 6572 6f20 4765 6e65 7261 6c20 5075  ffero General Pu
-000002b0: 626c 6963 204c 6963 656e 7365 0a23 2020  blic License.#  
-000002c0: 2020 2020 616c 6f6e 6720 7769 7468 2074      along with t
-000002d0: 6869 7320 7072 6f67 7261 6d2e 2020 4966  his program.  If
-000002e0: 206e 6f74 2c20 7365 6520 3c68 7474 7073   not, see <https
-000002f0: 3a2f 2f77 7777 2e67 6e75 2e6f 7267 2f6c  ://www.gnu.org/l
-00000300: 6963 656e 7365 732f 3e2e 0a0a 2320 2d2a  icenses/>...# -*
-00000310: 2d20 636f 6469 6e67 3a20 7574 662d 3820  - coding: utf-8 
-00000320: 2d2a 2d0a 696d 706f 7274 206a 736f 6e0a  -*-.import json.
-00000330: 0a66 726f 6d20 646a 616e 676f 2e63 6f72  .from django.cor
-00000340: 652e 6578 6365 7074 696f 6e73 2069 6d70  e.exceptions imp
-00000350: 6f72 7420 4f62 6a65 6374 446f 6573 4e6f  ort ObjectDoesNo
-00000360: 7445 7869 7374 0a66 726f 6d20 646a 616e  tExist.from djan
-00000370: 676f 2e63 6f72 652e 7365 7269 616c 697a  go.core.serializ
-00000380: 6572 732e 6a73 6f6e 2069 6d70 6f72 7420  ers.json import 
-00000390: 446a 616e 676f 4a53 4f4e 456e 636f 6465  DjangoJSONEncode
-000003a0: 720a 0a74 7279 3a0a 2020 2020 6672 6f6d  r..try:.    from
-000003b0: 2064 6a61 6e67 6f2e 7572 6c73 2069 6d70   django.urls imp
-000003c0: 6f72 7420 7265 7665 7273 650a 6578 6365  ort reverse.exce
-000003d0: 7074 3a0a 2020 2020 6672 6f6d 2064 6a61  pt:.    from dja
-000003e0: 6e67 6f2e 636f 7265 2e75 726c 7265 736f  ngo.core.urlreso
-000003f0: 6c76 6572 7320 696d 706f 7274 2072 6576  lvers import rev
-00000400: 6572 7365 0a66 726f 6d20 646a 616e 676f  erse.from django
-00000410: 2e74 656d 706c 6174 6520 696d 706f 7274  .template import
-00000420: 204c 6962 7261 7279 0a66 726f 6d20 646a   Library.from dj
-00000430: 616e 676f 2e75 7469 6c73 2e73 6166 6573  ango.utils.safes
-00000440: 7472 696e 6720 696d 706f 7274 206d 6172  tring import mar
-00000450: 6b5f 7361 6665 0a0a 7265 6769 7374 6572  k_safe..register
-00000460: 203d 204c 6962 7261 7279 2829 0a0a 0a40   = Library()...@
-00000470: 7265 6769 7374 6572 2e73 696d 706c 655f  register.simple_
-00000480: 7461 6728 7461 6b65 735f 636f 6e74 6578  tag(takes_contex
-00000490: 743d 5472 7565 290a 6465 6620 6e6f 7469  t=True).def noti
-000004a0: 6669 6361 7469 6f6e 735f 756e 7265 6164  fications_unread
-000004b0: 2863 6f6e 7465 7874 293a 0a20 2020 2075  (context):.    u
-000004c0: 7365 7220 3d20 7573 6572 5f63 6f6e 7465  ser = user_conte
-000004d0: 7874 2863 6f6e 7465 7874 290a 2020 2020  xt(context).    
-000004e0: 6966 206e 6f74 2075 7365 723a 0a20 2020  if not user:.   
-000004f0: 2020 2020 2072 6574 7572 6e20 2727 0a20       return ''. 
-00000500: 2020 2072 6574 7572 6e20 7573 6572 2e6e     return user.n
-00000510: 6f74 6966 6963 6174 696f 6e73 2e75 6e72  otifications.unr
-00000520: 6561 6428 292e 636f 756e 7428 290a 0a0a  ead().count()...
-00000530: 2320 5265 7175 6972 6573 2076 616e 696c  # Requires vanil
-00000540: 6c61 2d6a 7320 6672 616d 6577 6f72 6b20  la-js framework 
-00000550: 2d20 6874 7470 3a2f 2f76 616e 696c 6c61  - http://vanilla
-00000560: 2d6a 732e 636f 6d2f 0a40 7265 6769 7374  -js.com/.@regist
-00000570: 6572 2e73 696d 706c 655f 7461 670a 6465  er.simple_tag.de
-00000580: 6620 7265 6769 7374 6572 5f6e 6f74 6966  f register_notif
-00000590: 795f 6361 6c6c 6261 636b 7328 6261 6467  y_callbacks(badg
-000005a0: 655f 6964 3d27 6c69 7665 5f6e 6f74 6966  e_id='live_notif
-000005b0: 795f 6261 6467 6527 2c0a 2020 2020 2020  y_badge',.      
-000005c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000005d0: 2020 2020 2020 2020 6d65 6e75 5f69 643d          menu_id=
-000005e0: 276c 6976 655f 6e6f 7469 6679 5f6c 6973  'live_notify_lis
-000005f0: 7427 2c0a 2020 2020 2020 2020 2020 2020  t',.            
-00000600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000610: 2020 7265 6672 6573 685f 7065 7269 6f64    refresh_period
-00000620: 3d31 352c 0a20 2020 2020 2020 2020 2020  =15,.           
-00000630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000640: 2020 2063 616c 6c62 6163 6b73 3d27 272c     callbacks='',
-00000650: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000660: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00000670: 6574 6368 3d35 293a 0a20 2020 2072 6566  etch=5):.    ref
-00000680: 7265 7368 5f70 6572 696f 6420 3d20 696e  resh_period = in
-00000690: 7428 7265 6672 6573 685f 7065 7269 6f64  t(refresh_period
-000006a0: 2920 2a20 3130 3030 0a0a 2020 2020 6465  ) * 1000..    de
-000006b0: 6669 6e69 7469 6f6e 7320 3d20 2222 220a  finitions = """.
-000006c0: 2020 2020 2020 2020 6e6f 7469 6679 5f62          notify_b
-000006d0: 6164 6765 5f69 643d 277b 6261 6467 655f  adge_id='{badge_
-000006e0: 6964 7d27 3b0a 2020 2020 2020 2020 6e6f  id}';.        no
-000006f0: 7469 6679 5f6d 656e 755f 6964 3d27 7b6d  tify_menu_id='{m
-00000700: 656e 755f 6964 7d27 3b0a 2020 2020 2020  enu_id}';.      
-00000710: 2020 6e6f 7469 6679 5f61 7069 5f75 726c    notify_api_url
-00000720: 3d27 7b61 7069 5f75 726c 7d27 3b0a 2020  ='{api_url}';.  
-00000730: 2020 2020 2020 6e6f 7469 6679 5f66 6574        notify_fet
-00000740: 6368 5f63 6f75 6e74 3d27 7b66 6574 6368  ch_count='{fetch
-00000750: 5f63 6f75 6e74 7d27 3b0a 2020 2020 2020  _count}';.      
-00000760: 2020 6e6f 7469 6679 5f72 6566 7265 7368    notify_refresh
-00000770: 5f70 6572 696f 643d 7b72 6566 7265 7368  _period={refresh
-00000780: 7d3b 0a20 2020 2022 2222 2e66 6f72 6d61  };.    """.forma
-00000790: 7428 0a20 2020 2020 2020 2062 6164 6765  t(.        badge
-000007a0: 5f69 643d 6261 6467 655f 6964 2c0a 2020  _id=badge_id,.  
-000007b0: 2020 2020 2020 6d65 6e75 5f69 643d 6d65        menu_id=me
-000007c0: 6e75 5f69 642c 0a20 2020 2020 2020 2072  nu_id,.        r
-000007d0: 6566 7265 7368 3d72 6566 7265 7368 5f70  efresh=refresh_p
-000007e0: 6572 696f 642c 0a20 2020 2020 2020 2061  eriod,.        a
-000007f0: 7069 5f75 726c 3d22 7375 6976 696a 6f75  pi_url="suivijou
-00000800: 726e 616c 6965 722f 6e6f 7469 6669 6361  rnalier/notifica
-00000810: 7469 6f6e 2f6d 6564 6963 616d 656e 7473  tion/medicaments
-00000820: 2f22 2c0a 2020 2020 2020 2020 6665 7463  /",.        fetc
-00000830: 685f 636f 756e 743d 6665 7463 680a 2020  h_count=fetch.  
-00000840: 2020 290a 0a20 2020 2073 6372 6970 7420    )..    script 
-00000850: 3d20 223c 7363 7269 7074 3e22 202b 2064  = "<script>" + d
-00000860: 6566 696e 6974 696f 6e73 0a20 2020 2066  efinitions.    f
-00000870: 6f72 2063 616c 6c62 6163 6b20 696e 2063  or callback in c
-00000880: 616c 6c62 6163 6b73 2e73 706c 6974 2827  allbacks.split('
-00000890: 2c27 293a 0a20 2020 2020 2020 2073 6372  ,'):.        scr
-000008a0: 6970 7420 2b3d 2022 7265 6769 7374 6572  ipt += "register
-000008b0: 5f6e 6f74 6966 6965 7228 2220 2b20 6361  _notifier(" + ca
-000008c0: 6c6c 6261 636b 202b 2022 293b 220a 2020  llback + ");".  
-000008d0: 2020 7363 7269 7074 202b 3d20 223c 2f73    script += "</s
-000008e0: 6372 6970 743e 220a 2020 2020 7265 7475  cript>".    retu
-000008f0: 726e 206d 6172 6b5f 7361 6665 2873 6372  rn mark_safe(scr
-00000900: 6970 7429 0a0a 0a40 7265 6769 7374 6572  ipt)...@register
-00000910: 2e73 696d 706c 655f 7461 6728 7461 6b65  .simple_tag(take
-00000920: 735f 636f 6e74 6578 743d 5472 7565 290a  s_context=True).
-00000930: 6465 6620 6c69 7665 5f6e 6f74 6966 795f  def live_notify_
-00000940: 6261 6467 6528 636f 6e74 6578 742c 2062  badge(context, b
-00000950: 6164 6765 5f69 643d 276c 6976 655f 6e6f  adge_id='live_no
-00000960: 7469 6679 5f62 6164 6765 272c 2063 6c61  tify_badge', cla
-00000970: 7373 6573 3d22 2229 3a0a 2020 2020 7573  sses=""):.    us
-00000980: 6572 203d 2075 7365 725f 636f 6e74 6578  er = user_contex
-00000990: 7428 636f 6e74 6578 7429 0a20 2020 2069  t(context).    i
-000009a0: 6620 6e6f 7420 7573 6572 3a0a 2020 2020  f not user:.    
-000009b0: 2020 2020 7265 7475 726e 2027 270a 0a20      return ''.. 
-000009c0: 2020 2068 746d 6c20 3d20 223c 7370 616e     html = "<span
-000009d0: 2069 643d 277b 6261 6467 655f 6964 7d27   id='{badge_id}'
-000009e0: 2063 6c61 7373 3d27 7b63 6c61 7373 6573   class='{classes
-000009f0: 7d27 3e7b 756e 7265 6164 7d3c 2f73 7061  }'>{unread}</spa
-00000a00: 6e3e 222e 666f 726d 6174 280a 2020 2020  n>".format(.    
-00000a10: 2020 2020 6261 6467 655f 6964 3d62 6164      badge_id=bad
-00000a20: 6765 5f69 642c 2063 6c61 7373 6573 3d63  ge_id, classes=c
-00000a30: 6c61 7373 6573 2c20 756e 7265 6164 3d75  lasses, unread=u
-00000a40: 7365 722e 6e6f 7469 6669 6361 7469 6f6e  ser.notification
-00000a50: 732e 756e 7265 6164 2829 2e63 6f75 6e74  s.unread().count
-00000a60: 2829 0a20 2020 2029 0a20 2020 2072 6574  ().    ).    ret
-00000a70: 7572 6e20 6d61 726b 5f73 6166 6528 6874  urn mark_safe(ht
-00000a80: 6d6c 290a 0a0a 4072 6567 6973 7465 722e  ml)...@register.
-00000a90: 7369 6d70 6c65 5f74 6167 0a64 6566 206c  simple_tag.def l
-00000aa0: 6976 655f 6e6f 7469 6679 5f6c 6973 7428  ive_notify_list(
-00000ab0: 6c69 7374 5f69 643d 276c 6976 655f 6e6f  list_id='live_no
-00000ac0: 7469 6679 5f6c 6973 7427 2c20 636c 6173  tify_list', clas
-00000ad0: 7365 733d 2222 293a 0a20 2020 2068 746d  ses=""):.    htm
-00000ae0: 6c20 3d20 223c 756c 2069 643d 277b 6c69  l = "<ul id='{li
-00000af0: 7374 5f69 647d 2720 636c 6173 733d 277b  st_id}' class='{
-00000b00: 636c 6173 7365 737d 273e 3c2f 756c 3e22  classes}'></ul>"
-00000b10: 2e66 6f72 6d61 7428 6c69 7374 5f69 643d  .format(list_id=
-00000b20: 6c69 7374 5f69 642c 2063 6c61 7373 6573  list_id, classes
-00000b30: 3d63 6c61 7373 6573 290a 2020 2020 7265  =classes).    re
-00000b40: 7475 726e 206d 6172 6b5f 7361 6665 2868  turn mark_safe(h
-00000b50: 746d 6c29 0a0a 0a64 6566 2075 7365 725f  tml)...def user_
-00000b60: 636f 6e74 6578 7428 636f 6e74 6578 7429  context(context)
-00000b70: 3a0a 2020 2020 6966 2027 7573 6572 2720  :.    if 'user' 
-00000b80: 6e6f 7420 696e 2063 6f6e 7465 7874 3a0a  not in context:.
-00000b90: 2020 2020 2020 2020 7265 7475 726e 204e          return N
-00000ba0: 6f6e 650a 0a20 2020 2072 6571 7565 7374  one..    request
-00000bb0: 203d 2063 6f6e 7465 7874 5b27 7265 7175   = context['requ
-00000bc0: 6573 7427 5d0a 2020 2020 7573 6572 203d  est'].    user =
-00000bd0: 2072 6571 7565 7374 2e75 7365 720a 2020   request.user.  
-00000be0: 2020 6966 2075 7365 722e 6973 5f61 6e6f    if user.is_ano
-00000bf0: 6e79 6d6f 7573 3a0a 2020 2020 2020 2020  nymous:.        
-00000c00: 7265 7475 726e 204e 6f6e 650a 2020 2020  return None.    
-00000c10: 7265 7475 726e 2075 7365 720a 0a0a 4072  return user...@r
-00000c20: 6567 6973 7465 722e 7369 6d70 6c65 5f74  egister.simple_t
-00000c30: 6167 2874 616b 6573 5f63 6f6e 7465 7874  ag(takes_context
-00000c40: 3d54 7275 6529 0a64 6566 2069 7341 6c6c  =True).def isAll
-00000c50: 6f77 6564 436c 6173 7372 6f6f 6d28 636f  owedClassroom(co
-00000c60: 6e74 6578 7429 3a0a 2020 2020 7573 6572  ntext):.    user
-00000c70: 203d 2075 7365 725f 636f 6e74 6578 7428   = user_context(
-00000c80: 636f 6e74 6578 7429 0a20 2020 2074 7279  context).    try
-00000c90: 3a0a 2020 2020 2020 2020 636c 6173 7372  :.        classr
-00000ca0: 6f6f 6d5f 7661 6c69 6420 3d20 7573 6572  oom_valid = user
-00000cb0: 2e63 6c61 7373 726f 6f6d 5f73 6574 2e61  .classroom_set.a
-00000cc0: 6c6c 2829 2e76 616c 7565 735f 6c69 7374  ll().values_list
-00000cd0: 2822 6964 2229 0a20 2020 2065 7863 6570  ("id").    excep
-00000ce0: 7420 4f62 6a65 6374 446f 6573 4e6f 7445  t ObjectDoesNotE
-00000cf0: 7869 7374 3a0a 2020 2020 2020 2020 7265  xist:.        re
-00000d00: 7475 726e 2046 616c 7365 0a20 2020 2072  turn False.    r
-00000d10: 6574 7572 6e20 6a73 6f6e 2e64 756d 7073  eturn json.dumps
-00000d20: 286c 6973 7428 636c 6173 7372 6f6f 6d5f  (list(classroom_
-00000d30: 7661 6c69 6429 2c20 636c 733d 446a 616e  valid), cls=Djan
-00000d40: 676f 4a53 4f4e 456e 636f 6465 7229 0a    goJSONEncoder).
+00000040: 6962 7265 2e63 6f6d 0d0a 2320 2020 2020  ibre.com..#     
+00000050: 2054 6869 7320 7072 6f67 7261 6d20 6973   This program is
+00000060: 2066 7265 6520 736f 6674 7761 7265 3a20   free software: 
+00000070: 796f 7520 6361 6e20 7265 6469 7374 7269  you can redistri
+00000080: 6275 7465 2069 7420 616e 642f 6f72 206d  bute it and/or m
+00000090: 6f64 6966 790d 0a23 2020 2020 2020 6974  odify..#      it
+000000a0: 2075 6e64 6572 2074 6865 2074 6572 6d73   under the terms
+000000b0: 206f 6620 7468 6520 474e 5520 4166 6665   of the GNU Affe
+000000c0: 726f 2047 656e 6572 616c 2050 7562 6c69  ro General Publi
+000000d0: 6320 4c69 6365 6e73 6520 6173 0d0a 2320  c License as..# 
+000000e0: 2020 2020 2070 7562 6c69 7368 6564 2062       published b
+000000f0: 7920 7468 6520 4672 6565 2053 6f66 7477  y the Free Softw
+00000100: 6172 6520 466f 756e 6461 7469 6f6e 2c20  are Foundation, 
+00000110: 6569 7468 6572 2076 6572 7369 6f6e 2033  either version 3
+00000120: 206f 6620 7468 650d 0a23 2020 2020 2020   of the..#      
+00000130: 4c69 6365 6e73 652c 206f 7220 2861 7420  License, or (at 
+00000140: 796f 7572 206f 7074 696f 6e29 2061 6e79  your option) any
+00000150: 206c 6174 6572 2076 6572 7369 6f6e 2e0d   later version..
+00000160: 0a23 0d0a 2320 2020 2020 2054 6869 7320  .#..#      This 
+00000170: 7072 6f67 7261 6d20 6973 2064 6973 7472  program is distr
+00000180: 6962 7574 6564 2069 6e20 7468 6520 686f  ibuted in the ho
+00000190: 7065 2074 6861 7420 6974 2077 696c 6c20  pe that it will 
+000001a0: 6265 2075 7365 6675 6c2c 0d0a 2320 2020  be useful,..#   
+000001b0: 2020 2062 7574 2057 4954 484f 5554 2041     but WITHOUT A
+000001c0: 4e59 2057 4152 5241 4e54 593b 2077 6974  NY WARRANTY; wit
+000001d0: 686f 7574 2065 7665 6e20 7468 6520 696d  hout even the im
+000001e0: 706c 6965 6420 7761 7272 616e 7479 206f  plied warranty o
+000001f0: 660d 0a23 2020 2020 2020 4d45 5243 4841  f..#      MERCHA
+00000200: 4e54 4142 494c 4954 5920 6f72 2046 4954  NTABILITY or FIT
+00000210: 4e45 5353 2046 4f52 2041 2050 4152 5449  NESS FOR A PARTI
+00000220: 4355 4c41 5220 5055 5250 4f53 452e 2020  CULAR PURPOSE.  
+00000230: 5365 6520 7468 650d 0a23 2020 2020 2020  See the..#      
+00000240: 474e 5520 4166 6665 726f 2047 656e 6572  GNU Affero Gener
+00000250: 616c 2050 7562 6c69 6320 4c69 6365 6e73  al Public Licens
+00000260: 6520 666f 7220 6d6f 7265 2064 6574 6169  e for more detai
+00000270: 6c73 2e0d 0a23 0d0a 2320 2020 2020 2059  ls...#..#      Y
+00000280: 6f75 2073 686f 756c 6420 6861 7665 2072  ou should have r
+00000290: 6563 6569 7665 6420 6120 636f 7079 206f  eceived a copy o
+000002a0: 6620 7468 6520 474e 5520 4166 6665 726f  f the GNU Affero
+000002b0: 2047 656e 6572 616c 2050 7562 6c69 6320   General Public 
+000002c0: 4c69 6365 6e73 650d 0a23 2020 2020 2020  License..#      
+000002d0: 616c 6f6e 6720 7769 7468 2074 6869 7320  along with this 
+000002e0: 7072 6f67 7261 6d2e 2020 4966 206e 6f74  program.  If not
+000002f0: 2c20 7365 6520 3c68 7474 7073 3a2f 2f77  , see <https://w
+00000300: 7777 2e67 6e75 2e6f 7267 2f6c 6963 656e  ww.gnu.org/licen
+00000310: 7365 732f 3e2e 0d0a 0d0a 2320 2d2a 2d20  ses/>.....# -*- 
+00000320: 636f 6469 6e67 3a20 7574 662d 3820 2d2a  coding: utf-8 -*
+00000330: 2d0d 0a69 6d70 6f72 7420 6a73 6f6e 0d0a  -..import json..
+00000340: 0d0a 6672 6f6d 2064 6a61 6e67 6f2e 636f  ..from django.co
+00000350: 7265 2e65 7863 6570 7469 6f6e 7320 696d  re.exceptions im
+00000360: 706f 7274 204f 626a 6563 7444 6f65 734e  port ObjectDoesN
+00000370: 6f74 4578 6973 740d 0a66 726f 6d20 646a  otExist..from dj
+00000380: 616e 676f 2e63 6f72 652e 7365 7269 616c  ango.core.serial
+00000390: 697a 6572 732e 6a73 6f6e 2069 6d70 6f72  izers.json impor
+000003a0: 7420 446a 616e 676f 4a53 4f4e 456e 636f  t DjangoJSONEnco
+000003b0: 6465 720d 0a0d 0a74 7279 3a0d 0a20 2020  der....try:..   
+000003c0: 2066 726f 6d20 646a 616e 676f 2e75 726c   from django.url
+000003d0: 7320 696d 706f 7274 2072 6576 6572 7365  s import reverse
+000003e0: 0d0a 6578 6365 7074 3a0d 0a20 2020 2066  ..except:..    f
+000003f0: 726f 6d20 646a 616e 676f 2e63 6f72 652e  rom django.core.
+00000400: 7572 6c72 6573 6f6c 7665 7273 2069 6d70  urlresolvers imp
+00000410: 6f72 7420 7265 7665 7273 650d 0a66 726f  ort reverse..fro
+00000420: 6d20 646a 616e 676f 2e74 656d 706c 6174  m django.templat
+00000430: 6520 696d 706f 7274 204c 6962 7261 7279  e import Library
+00000440: 0d0a 6672 6f6d 2064 6a61 6e67 6f2e 7574  ..from django.ut
+00000450: 696c 732e 7361 6665 7374 7269 6e67 2069  ils.safestring i
+00000460: 6d70 6f72 7420 6d61 726b 5f73 6166 650d  mport mark_safe.
+00000470: 0a0d 0a72 6567 6973 7465 7220 3d20 4c69  ...register = Li
+00000480: 6272 6172 7928 290d 0a0d 0a0d 0a40 7265  brary()......@re
+00000490: 6769 7374 6572 2e73 696d 706c 655f 7461  gister.simple_ta
+000004a0: 6728 7461 6b65 735f 636f 6e74 6578 743d  g(takes_context=
+000004b0: 5472 7565 290d 0a64 6566 206e 6f74 6966  True)..def notif
+000004c0: 6963 6174 696f 6e73 5f75 6e72 6561 6428  ications_unread(
+000004d0: 636f 6e74 6578 7429 3a0d 0a20 2020 2075  context):..    u
+000004e0: 7365 7220 3d20 7573 6572 5f63 6f6e 7465  ser = user_conte
+000004f0: 7874 2863 6f6e 7465 7874 290d 0a20 2020  xt(context)..   
+00000500: 2069 6620 6e6f 7420 7573 6572 3a0d 0a20   if not user:.. 
+00000510: 2020 2020 2020 2072 6574 7572 6e20 2727         return ''
+00000520: 0d0a 2020 2020 7265 7475 726e 2075 7365  ..    return use
+00000530: 722e 6e6f 7469 6669 6361 7469 6f6e 732e  r.notifications.
+00000540: 756e 7265 6164 2829 2e63 6f75 6e74 2829  unread().count()
+00000550: 0d0a 0d0a 0d0a 2320 5265 7175 6972 6573  ......# Requires
+00000560: 2076 616e 696c 6c61 2d6a 7320 6672 616d   vanilla-js fram
+00000570: 6577 6f72 6b20 2d20 6874 7470 3a2f 2f76  ework - http://v
+00000580: 616e 696c 6c61 2d6a 732e 636f 6d2f 0d0a  anilla-js.com/..
+00000590: 4072 6567 6973 7465 722e 7369 6d70 6c65  @register.simple
+000005a0: 5f74 6167 0d0a 6465 6620 7265 6769 7374  _tag..def regist
+000005b0: 6572 5f6e 6f74 6966 795f 6361 6c6c 6261  er_notify_callba
+000005c0: 636b 7328 6261 6467 655f 6964 3d27 6c69  cks(badge_id='li
+000005d0: 7665 5f6e 6f74 6966 795f 6261 6467 6527  ve_notify_badge'
+000005e0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000005f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000600: 206d 656e 755f 6964 3d27 6c69 7665 5f6e   menu_id='live_n
+00000610: 6f74 6966 795f 6c69 7374 272c 0d0a 2020  otify_list',..  
+00000620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000630: 2020 2020 2020 2020 2020 2020 7265 6672              refr
+00000640: 6573 685f 7065 7269 6f64 3d31 352c 0d0a  esh_period=15,..
+00000650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000660: 2020 2020 2020 2020 2020 2020 2020 6361                ca
+00000670: 6c6c 6261 636b 733d 2727 2c0d 0a20 2020  llbacks='',..   
+00000680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000690: 2020 2020 2020 2020 2020 2066 6574 6368             fetch
+000006a0: 3d35 293a 0d0a 2020 2020 7265 6672 6573  =5):..    refres
+000006b0: 685f 7065 7269 6f64 203d 2069 6e74 2872  h_period = int(r
+000006c0: 6566 7265 7368 5f70 6572 696f 6429 202a  efresh_period) *
+000006d0: 2031 3030 300d 0a0d 0a20 2020 2064 6566   1000....    def
+000006e0: 696e 6974 696f 6e73 203d 2022 2222 0d0a  initions = """..
+000006f0: 2020 2020 2020 2020 6e6f 7469 6679 5f62          notify_b
+00000700: 6164 6765 5f69 643d 277b 6261 6467 655f  adge_id='{badge_
+00000710: 6964 7d27 3b0d 0a20 2020 2020 2020 206e  id}';..        n
+00000720: 6f74 6966 795f 6d65 6e75 5f69 643d 277b  otify_menu_id='{
+00000730: 6d65 6e75 5f69 647d 273b 0d0a 2020 2020  menu_id}';..    
+00000740: 2020 2020 6e6f 7469 6679 5f61 7069 5f75      notify_api_u
+00000750: 726c 3d27 7b61 7069 5f75 726c 7d27 3b0d  rl='{api_url}';.
+00000760: 0a20 2020 2020 2020 206e 6f74 6966 795f  .        notify_
+00000770: 6665 7463 685f 636f 756e 743d 277b 6665  fetch_count='{fe
+00000780: 7463 685f 636f 756e 747d 273b 0d0a 2020  tch_count}';..  
+00000790: 2020 2020 2020 6e6f 7469 6679 5f72 6566        notify_ref
+000007a0: 7265 7368 5f70 6572 696f 643d 7b72 6566  resh_period={ref
+000007b0: 7265 7368 7d3b 0d0a 2020 2020 2222 222e  resh};..    """.
+000007c0: 666f 726d 6174 280d 0a20 2020 2020 2020  format(..       
+000007d0: 2062 6164 6765 5f69 643d 6261 6467 655f   badge_id=badge_
+000007e0: 6964 2c0d 0a20 2020 2020 2020 206d 656e  id,..        men
+000007f0: 755f 6964 3d6d 656e 755f 6964 2c0d 0a20  u_id=menu_id,.. 
+00000800: 2020 2020 2020 2072 6566 7265 7368 3d72         refresh=r
+00000810: 6566 7265 7368 5f70 6572 696f 642c 0d0a  efresh_period,..
+00000820: 2020 2020 2020 2020 6170 695f 7572 6c3d          api_url=
+00000830: 2273 7569 7669 6a6f 7572 6e61 6c69 6572  "suivijournalier
+00000840: 2f6e 6f74 6966 6963 6174 696f 6e2f 6d65  /notification/me
+00000850: 6469 6361 6d65 6e74 732f 222c 0d0a 2020  dicaments/",..  
+00000860: 2020 2020 2020 6665 7463 685f 636f 756e        fetch_coun
+00000870: 743d 6665 7463 680d 0a20 2020 2029 0d0a  t=fetch..    )..
+00000880: 0d0a 2020 2020 7363 7269 7074 203d 2022  ..    script = "
+00000890: 3c73 6372 6970 743e 2220 2b20 6465 6669  <script>" + defi
+000008a0: 6e69 7469 6f6e 730d 0a20 2020 2066 6f72  nitions..    for
+000008b0: 2063 616c 6c62 6163 6b20 696e 2063 616c   callback in cal
+000008c0: 6c62 6163 6b73 2e73 706c 6974 2827 2c27  lbacks.split(','
+000008d0: 293a 0d0a 2020 2020 2020 2020 7363 7269  ):..        scri
+000008e0: 7074 202b 3d20 2272 6567 6973 7465 725f  pt += "register_
+000008f0: 6e6f 7469 6669 6572 2822 202b 2063 616c  notifier(" + cal
+00000900: 6c62 6163 6b20 2b20 2229 3b22 0d0a 2020  lback + ");"..  
+00000910: 2020 7363 7269 7074 202b 3d20 223c 2f73    script += "</s
+00000920: 6372 6970 743e 220d 0a20 2020 2072 6574  cript>"..    ret
+00000930: 7572 6e20 6d61 726b 5f73 6166 6528 7363  urn mark_safe(sc
+00000940: 7269 7074 290d 0a0d 0a0d 0a40 7265 6769  ript)......@regi
+00000950: 7374 6572 2e73 696d 706c 655f 7461 6728  ster.simple_tag(
+00000960: 7461 6b65 735f 636f 6e74 6578 743d 5472  takes_context=Tr
+00000970: 7565 290d 0a64 6566 206c 6976 655f 6e6f  ue)..def live_no
+00000980: 7469 6679 5f62 6164 6765 2863 6f6e 7465  tify_badge(conte
+00000990: 7874 2c20 6261 6467 655f 6964 3d27 6c69  xt, badge_id='li
+000009a0: 7665 5f6e 6f74 6966 795f 6261 6467 6527  ve_notify_badge'
+000009b0: 2c20 636c 6173 7365 733d 2222 293a 0d0a  , classes=""):..
+000009c0: 2020 2020 7573 6572 203d 2075 7365 725f      user = user_
+000009d0: 636f 6e74 6578 7428 636f 6e74 6578 7429  context(context)
+000009e0: 0d0a 2020 2020 6966 206e 6f74 2075 7365  ..    if not use
+000009f0: 723a 0d0a 2020 2020 2020 2020 7265 7475  r:..        retu
+00000a00: 726e 2027 270d 0a0d 0a20 2020 2068 746d  rn ''....    htm
+00000a10: 6c20 3d20 223c 7370 616e 2069 643d 277b  l = "<span id='{
+00000a20: 6261 6467 655f 6964 7d27 2063 6c61 7373  badge_id}' class
+00000a30: 3d27 7b63 6c61 7373 6573 7d27 3e7b 756e  ='{classes}'>{un
+00000a40: 7265 6164 7d3c 2f73 7061 6e3e 222e 666f  read}</span>".fo
+00000a50: 726d 6174 280d 0a20 2020 2020 2020 2062  rmat(..        b
+00000a60: 6164 6765 5f69 643d 6261 6467 655f 6964  adge_id=badge_id
+00000a70: 2c20 636c 6173 7365 733d 636c 6173 7365  , classes=classe
+00000a80: 732c 2075 6e72 6561 643d 7573 6572 2e6e  s, unread=user.n
+00000a90: 6f74 6966 6963 6174 696f 6e73 2e75 6e72  otifications.unr
+00000aa0: 6561 6428 292e 636f 756e 7428 290d 0a20  ead().count().. 
+00000ab0: 2020 2029 0d0a 2020 2020 7265 7475 726e     )..    return
+00000ac0: 206d 6172 6b5f 7361 6665 2868 746d 6c29   mark_safe(html)
+00000ad0: 0d0a 0d0a 0d0a 4072 6567 6973 7465 722e  ......@register.
+00000ae0: 7369 6d70 6c65 5f74 6167 0d0a 6465 6620  simple_tag..def 
+00000af0: 6c69 7665 5f6e 6f74 6966 795f 6c69 7374  live_notify_list
+00000b00: 286c 6973 745f 6964 3d27 6c69 7665 5f6e  (list_id='live_n
+00000b10: 6f74 6966 795f 6c69 7374 272c 2063 6c61  otify_list', cla
+00000b20: 7373 6573 3d22 2229 3a0d 0a20 2020 2068  sses=""):..    h
+00000b30: 746d 6c20 3d20 223c 756c 2069 643d 277b  tml = "<ul id='{
+00000b40: 6c69 7374 5f69 647d 2720 636c 6173 733d  list_id}' class=
+00000b50: 277b 636c 6173 7365 737d 273e 3c2f 756c  '{classes}'></ul
+00000b60: 3e22 2e66 6f72 6d61 7428 6c69 7374 5f69  >".format(list_i
+00000b70: 643d 6c69 7374 5f69 642c 2063 6c61 7373  d=list_id, class
+00000b80: 6573 3d63 6c61 7373 6573 290d 0a20 2020  es=classes)..   
+00000b90: 2072 6574 7572 6e20 6d61 726b 5f73 6166   return mark_saf
+00000ba0: 6528 6874 6d6c 290d 0a0d 0a0d 0a64 6566  e(html)......def
+00000bb0: 2075 7365 725f 636f 6e74 6578 7428 636f   user_context(co
+00000bc0: 6e74 6578 7429 3a0d 0a20 2020 2069 6620  ntext):..    if 
+00000bd0: 2775 7365 7227 206e 6f74 2069 6e20 636f  'user' not in co
+00000be0: 6e74 6578 743a 0d0a 2020 2020 2020 2020  ntext:..        
+00000bf0: 7265 7475 726e 204e 6f6e 650d 0a0d 0a20  return None.... 
+00000c00: 2020 2072 6571 7565 7374 203d 2063 6f6e     request = con
+00000c10: 7465 7874 5b27 7265 7175 6573 7427 5d0d  text['request'].
+00000c20: 0a20 2020 2075 7365 7220 3d20 7265 7175  .    user = requ
+00000c30: 6573 742e 7573 6572 0d0a 2020 2020 6966  est.user..    if
+00000c40: 2075 7365 722e 6973 5f61 6e6f 6e79 6d6f   user.is_anonymo
+00000c50: 7573 3a0d 0a20 2020 2020 2020 2072 6574  us:..        ret
+00000c60: 7572 6e20 4e6f 6e65 0d0a 2020 2020 7265  urn None..    re
+00000c70: 7475 726e 2075 7365 720d 0a0d 0a0d 0a40  turn user......@
+00000c80: 7265 6769 7374 6572 2e73 696d 706c 655f  register.simple_
+00000c90: 7461 6728 7461 6b65 735f 636f 6e74 6578  tag(takes_contex
+00000ca0: 743d 5472 7565 290d 0a64 6566 2069 7341  t=True)..def isA
+00000cb0: 6c6c 6f77 6564 436c 6173 7372 6f6f 6d28  llowedClassroom(
+00000cc0: 636f 6e74 6578 7429 3a0d 0a20 2020 2075  context):..    u
+00000cd0: 7365 7220 3d20 7573 6572 5f63 6f6e 7465  ser = user_conte
+00000ce0: 7874 2863 6f6e 7465 7874 290d 0a20 2020  xt(context)..   
+00000cf0: 2074 7279 3a0d 0a20 2020 2020 2020 2063   try:..        c
+00000d00: 6c61 7373 726f 6f6d 5f76 616c 6964 203d  lassroom_valid =
+00000d10: 2075 7365 722e 636c 6173 7372 6f6f 6d5f   user.classroom_
+00000d20: 7365 742e 616c 6c28 292e 7661 6c75 6573  set.all().values
+00000d30: 5f6c 6973 7428 2269 6422 290d 0a20 2020  _list("id")..   
+00000d40: 2065 7863 6570 7420 4f62 6a65 6374 446f   except ObjectDo
+00000d50: 6573 4e6f 7445 7869 7374 3a0d 0a20 2020  esNotExist:..   
+00000d60: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+00000d70: 650d 0a20 2020 2072 6574 7572 6e20 6a73  e..    return js
+00000d80: 6f6e 2e64 756d 7073 286c 6973 7428 636c  on.dumps(list(cl
+00000d90: 6173 7372 6f6f 6d5f 7661 6c69 6429 2c20  assroom_valid), 
+00000da0: 636c 733d 446a 616e 676f 4a53 4f4e 456e  cls=DjangoJSONEn
+00000db0: 636f 6465 7229 0d0a                      coder)..
```

### Comparing `nobinobi-core-0.1.4.6/nobinobi_core/templatetags/remove_date_sem.py` & `nobinobi-core-0.1.4.7/nobinobi_core/templatetags/remove_tags_html.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,30 @@
-#      Copyright (C) 2020 <Florian Alu - Prolibre - https://prolibre.com
-#      This program is free software: you can redistribute it and/or modify
-#      it under the terms of the GNU Affero General Public License as
-#      published by the Free Software Foundation, either version 3 of the
-#      License, or (at your option) any later version.
-#
-#      This program is distributed in the hope that it will be useful,
-#      but WITHOUT ANY WARRANTY; without even the implied warranty of
-#      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#      GNU Affero General Public License for more details.
-#
-#      You should have received a copy of the GNU Affero General Public License
-#      along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-# -*- coding: utf-8 -*-
-
-from django.template.defaultfilters import register
-
-
-@register.filter
-def substract(val):
-    """
-    Usage:
-    """
-    val = int(val) - 1
-
-    return val
+#      Copyright (C) 2020 <Florian Alu - Prolibre - https://prolibre.com
+#      This program is free software: you can redistribute it and/or modify
+#      it under the terms of the GNU Affero General Public License as
+#      published by the Free Software Foundation, either version 3 of the
+#      License, or (at your option) any later version.
+#
+#      This program is distributed in the hope that it will be useful,
+#      but WITHOUT ANY WARRANTY; without even the implied warranty of
+#      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#      GNU Affero General Public License for more details.
+#
+#      You should have received a copy of the GNU Affero General Public License
+#      along with this program.  If not, see <https://www.gnu.org/licenses/>.
+#
+
+# -*- coding: utf-8 -*-
+import re
+
+from django.template.defaultfilters import register
+
+TAG_RE = re.compile(r'<[^>]+>')
+
+
+@register.filter
+def removetagshtml(value):
+    """
+    Usage: value|removetags
+    """
+
+    return TAG_RE.sub('', value)
```

### Comparing `nobinobi-core-0.1.4.6/nobinobi_core/templatetags/remove_tags_html.py` & `nobinobi-core-0.1.4.7/nobinobi_core/templatetags/get_user_method.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,24 +7,17 @@
 #      This program is distributed in the hope that it will be useful,
 #      but WITHOUT ANY WARRANTY; without even the implied warranty of
 #      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #      GNU Affero General Public License for more details.
 #
 #      You should have received a copy of the GNU Affero General Public License
 #      along with this program.  If not, see <https://www.gnu.org/licenses/>.
-#
-
-# -*- coding: utf-8 -*-
-import re
 
-from django.template.defaultfilters import register
 
-TAG_RE = re.compile(r'<[^>]+>')
+from django import template
 
+register = template.Library()
 
-@register.filter
-def removetagshtml(value):
-    """
-    Usage: value|removetags
-    """
 
-    return TAG_RE.sub('', value)
+@register.filter(name='has_group')
+def has_group(user, group_name):
+    return user.groups.filter(name=group_name).exists()
```

### Comparing `nobinobi-core-0.1.4.6/nobinobi_core/templatetags/startwith.py` & `nobinobi-core-0.1.4.7/nobinobi_core/templatetags/startwith.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-#      Copyright (C) 2020 <Florian Alu - Prolibre - https://prolibre.com
-#      This program is free software: you can redistribute it and/or modify
-#      it under the terms of the GNU Affero General Public License as
-#      published by the Free Software Foundation, either version 3 of the
-#      License, or (at your option) any later version.
-#
-#      This program is distributed in the hope that it will be useful,
-#      but WITHOUT ANY WARRANTY; without even the implied warranty of
-#      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#      GNU Affero General Public License for more details.
-#
-#      You should have received a copy of the GNU Affero General Public License
-#      along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-# -*- coding: utf-8 -*-
-import arrow
-from django.template.defaultfilters import register
-
-
-@register.filter
-def starts_with(value, arg):
-    """Usage, {% if value|starts_with:"arg" %}"""
-    return value.startswith(arg)
-
-
-@register.filter
-def now(value, arg):
-    """Usage, {% if value|starts_with:"arg" %}"""
-    if arg == "heure":
-        return "%02d" % int(arrow.now().time().hour)
-    elif arg == "min":
-        return "%02d" % int(arrow.now().time().minute)
+#      Copyright (C) 2020 <Florian Alu - Prolibre - https://prolibre.com
+#      This program is free software: you can redistribute it and/or modify
+#      it under the terms of the GNU Affero General Public License as
+#      published by the Free Software Foundation, either version 3 of the
+#      License, or (at your option) any later version.
+#
+#      This program is distributed in the hope that it will be useful,
+#      but WITHOUT ANY WARRANTY; without even the implied warranty of
+#      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#      GNU Affero General Public License for more details.
+#
+#      You should have received a copy of the GNU Affero General Public License
+#      along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+# -*- coding: utf-8 -*-
+import arrow
+from django.template.defaultfilters import register
+
+
+@register.filter
+def starts_with(value, arg):
+    """Usage, {% if value|starts_with:"arg" %}"""
+    return value.startswith(arg)
+
+
+@register.filter
+def now(value, arg):
+    """Usage, {% if value|starts_with:"arg" %}"""
+    if arg == "heure":
+        return "%02d" % int(arrow.now().time().hour)
+    elif arg == "min":
+        return "%02d" % int(arrow.now().time().minute)
```

### Comparing `nobinobi-core-0.1.4.6/nobinobi_core/urls.py` & `nobinobi-core-0.1.4.7/nobinobi_core/urls.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-#      Copyright (C) 2020 <Florian Alu - Prolibre - https://prolibre.com
-#      This program is free software: you can redistribute it and/or modify
-#      it under the terms of the GNU Affero General Public License as
-#      published by the Free Software Foundation, either version 3 of the
-#      License, or (at your option) any later version.
-#
-#      This program is distributed in the hope that it will be useful,
-#      but WITHOUT ANY WARRANTY; without even the implied warranty of
-#      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#      GNU Affero General Public License for more details.
-#
-#      You should have received a copy of the GNU Affero General Public License
-#      along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-# -*- coding: utf-8 -*-
-
-from django.contrib.admin.views.decorators import staff_member_required
-from django.urls import path
-
-from .views import HolidayAddOffical
-
-app_name = 'nobinobi_core'
-
-urlpatterns = [
-    path('admin/nobinobi_core/add-official-holiday/', staff_member_required(HolidayAddOffical.as_view()), name='add_official_holiday'),
-]
+#      Copyright (C) 2020 <Florian Alu - Prolibre - https://prolibre.com
+#      This program is free software: you can redistribute it and/or modify
+#      it under the terms of the GNU Affero General Public License as
+#      published by the Free Software Foundation, either version 3 of the
+#      License, or (at your option) any later version.
+#
+#      This program is distributed in the hope that it will be useful,
+#      but WITHOUT ANY WARRANTY; without even the implied warranty of
+#      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#      GNU Affero General Public License for more details.
+#
+#      You should have received a copy of the GNU Affero General Public License
+#      along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+# -*- coding: utf-8 -*-
+
+from django.contrib.admin.views.decorators import staff_member_required
+from django.urls import path
+
+from .views import HolidayAddOffical
+
+app_name = 'nobinobi_core'
+
+urlpatterns = [
+    path('admin/nobinobi_core/add-official-holiday/', staff_member_required(HolidayAddOffical.as_view()), name='add_official_holiday'),
+]
```

### Comparing `nobinobi-core-0.1.4.6/nobinobi_core/views.py` & `nobinobi-core-0.1.4.7/nobinobi_core/views.py`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.6/nobinobi_core/widgets.py` & `nobinobi-core-0.1.4.7/nobinobi_core/widgets.py`

 * *Files identical despite different names*

### Comparing `nobinobi-core-0.1.4.6/nobinobi_core.egg-info/SOURCES.txt` & `nobinobi-core-0.1.4.7/nobinobi_core.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -55,8 +55,10 @@
 nobinobi_core/templatetags/__init__.py
 nobinobi_core/templatetags/get_dict_value.py
 nobinobi_core/templatetags/get_user_method.py
 nobinobi_core/templatetags/math.py
 nobinobi_core/templatetags/notifications_tags_custom.py
 nobinobi_core/templatetags/remove_date_sem.py
 nobinobi_core/templatetags/remove_tags_html.py
-nobinobi_core/templatetags/startwith.py
+nobinobi_core/templatetags/startwith.py
+tests/test_admin.py
+tests/test_models.py
```

### Comparing `nobinobi-core-0.1.4.6/setup.py` & `nobinobi-core-0.1.4.7/setup.py`

 * *Files identical despite different names*

