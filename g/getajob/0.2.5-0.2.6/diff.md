# Comparing `tmp/getajob-0.2.5.tar.gz` & `tmp/getajob-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getajob-0.2.5.tar", max compression
+gzip compressed data, was "getajob-0.2.6.tar", max compression
```

## Comparing `getajob-0.2.5.tar` & `getajob-0.2.6.tar`

### file list

```diff
@@ -1,73 +1,77 @@
--rw-r--r--   0        0        0    11357 2023-06-12 21:15:39.354895 getajob-0.2.5/LICENSE
--rw-r--r--   0        0        0       69 2023-06-12 21:15:39.354895 getajob-0.2.5/README.md
--rw-r--r--   0        0        0       22 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/__init__.py
--rw-r--r--   0        0        0     1811 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/abstractions/models.py
--rw-r--r--   0        0        0     8332 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/abstractions/repository.py
--rw-r--r--   0        0        0     1341 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/config/settings.py
--rw-r--r--   0        0        0        0 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/__init__.py
--rw-r--r--   0        0        0        0 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/admin/__init__.py
--rw-r--r--   0        0        0        0 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/admin/search/__init__.py
--rw-r--r--   0        0        0      141 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/admin/search/models.py
--rw-r--r--   0        0        0      394 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/admin/search/repository.py
--rw-r--r--   0        0        0        0 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/admin/users/__init__.py
--rw-r--r--   0        0        0      620 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/admin/users/models.py
--rw-r--r--   0        0        0      598 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/admin/users/repository.py
--rw-r--r--   0        0        0        0 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/ai/text/__init__.py
--rw-r--r--   0        0        0      823 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/ai/text/models.py
--rw-r--r--   0        0        0     2470 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/ai/text/repository.py
--rw-r--r--   0        0        0        0 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/companies/__init__.py
--rw-r--r--   0        0        0      102 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/companies/models.py
--rw-r--r--   0        0        0      395 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/companies/repository.py
--rw-r--r--   0        0        0        0 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/jobs/__init__.py
--rw-r--r--   0        0        0     3021 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/jobs/models.py
--rw-r--r--   0        0        0     1120 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/jobs/repository.py
--rw-r--r--   0        0        0      462 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/jobs/unit_of_work.py
--rw-r--r--   0        0        0        0 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/scheduled_events/__init__.py
--rw-r--r--   0        0        0     1155 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/scheduled_events/models.py
--rw-r--r--   0        0        0     1556 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/scheduled_events/repository.py
--rw-r--r--   0        0        0        0 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/static/__init__.py
--rw-r--r--   0        0        0     1327 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/static/repository.py
--rw-r--r--   0        0        0        0 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/users/cover_letters/__init__.py
--rw-r--r--   0        0        0      277 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/users/cover_letters/models.py
--rw-r--r--   0        0        0      516 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/users/cover_letters/repository.py
--rw-r--r--   0        0        0       89 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/users/models.py
--rw-r--r--   0        0        0      568 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/users/repository.py
--rw-r--r--   0        0        0        0 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/users/resumes/__init__.py
--rw-r--r--   0        0        0      196 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/users/resumes/models.py
--rw-r--r--   0        0        0      462 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/users/resumes/repository.py
--rw-r--r--   0        0        0        0 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/users/sessions/__init__.py
--rw-r--r--   0        0        0      306 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/users/sessions/models.py
--rw-r--r--   0        0        0        0 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/users/skills/__init__.py
--rw-r--r--   0        0        0      404 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/users/skills/models.py
--rw-r--r--   0        0        0      491 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/contexts/users/skills/repository.py
--rw-r--r--   0        0        0     2318 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/exceptions.py
--rw-r--r--   0        0        0      375 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/utils.py
--rw-r--r--   0        0        0        0 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/vendor/__init__.py
--rw-r--r--   0        0        0      165 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/vendor/aiocron.py
--rw-r--r--   0        0        0        0 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/vendor/clerk/__init__.py
--rw-r--r--   0        0        0        0 2023-06-12 21:15:39.354895 getajob-0.2.5/getajob/vendor/clerk/companies/__init__.py
--rw-r--r--   0        0        0      894 2023-06-12 21:15:39.358895 getajob-0.2.5/getajob/vendor/clerk/companies/models.py
--rw-r--r--   0        0        0     1848 2023-06-12 21:15:39.358895 getajob-0.2.5/getajob/vendor/clerk/companies/repository.py
--rw-r--r--   0        0        0      413 2023-06-12 21:15:39.358895 getajob-0.2.5/getajob/vendor/clerk/models.py
--rw-r--r--   0        0        0        0 2023-06-12 21:15:39.358895 getajob-0.2.5/getajob/vendor/clerk/recruiter_invitation/__init__.py
--rw-r--r--   0        0        0      747 2023-06-12 21:15:39.358895 getajob-0.2.5/getajob/vendor/clerk/recruiter_invitation/models.py
--rw-r--r--   0        0        0     2120 2023-06-12 21:15:39.358895 getajob-0.2.5/getajob/vendor/clerk/recruiter_invitation/repository.py
--rw-r--r--   0        0        0        0 2023-06-12 21:15:39.358895 getajob-0.2.5/getajob/vendor/clerk/recruiters/__init__.py
--rw-r--r--   0        0        0     1748 2023-06-12 21:15:39.358895 getajob-0.2.5/getajob/vendor/clerk/recruiters/models.py
--rw-r--r--   0        0        0     2774 2023-06-12 21:15:39.358895 getajob-0.2.5/getajob/vendor/clerk/recruiters/repository.py
--rw-r--r--   0        0        0        0 2023-06-12 21:15:39.358895 getajob-0.2.5/getajob/vendor/clerk/users/__init__.py
--rw-r--r--   0        0        0     1320 2023-06-12 21:15:39.358895 getajob-0.2.5/getajob/vendor/clerk/users/models.py
--rw-r--r--   0        0        0     1839 2023-06-12 21:15:39.358895 getajob-0.2.5/getajob/vendor/clerk/users/repository.py
--rw-r--r--   0        0        0     9580 2023-06-12 21:15:39.358895 getajob-0.2.5/getajob/vendor/firebase.py
--rw-r--r--   0        0        0        0 2023-06-12 21:15:39.358895 getajob-0.2.5/getajob/vendor/kafka/__init__.py
--rw-r--r--   0        0        0      724 2023-06-12 21:15:39.358895 getajob-0.2.5/getajob/vendor/kafka/authentication.py
--rw-r--r--   0        0        0      320 2023-06-12 21:15:39.358895 getajob-0.2.5/getajob/vendor/kafka/exceptions.py
--rw-r--r--   0        0        0     1254 2023-06-12 21:15:39.358895 getajob-0.2.5/getajob/vendor/kafka/kafka.py
--rw-r--r--   0        0        0      221 2023-06-12 21:15:39.358895 getajob-0.2.5/getajob/vendor/kafka/mock.py
--rw-r--r--   0        0        0     1480 2023-06-12 21:15:39.358895 getajob-0.2.5/getajob/vendor/kafka/models.py
--rw-r--r--   0        0        0      589 2023-06-12 21:15:39.358895 getajob-0.2.5/getajob/vendor/kafka/repository.py
--rw-r--r--   0        0        0     1862 2023-06-12 21:15:39.358895 getajob-0.2.5/getajob/vendor/openai.py
--rw-r--r--   0        0        0      599 2023-06-12 21:15:39.358895 getajob-0.2.5/getajob/vendor/sendgrid/sendgrid.py
--rw-r--r--   0        0        0      251 2023-06-12 21:15:39.358895 getajob-0.2.5/getajob/vendor/sentry.py
--rw-r--r--   0        0        0     1742 2023-06-12 21:15:39.358895 getajob-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     2805 1970-01-01 00:00:00.000000 getajob-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-13 00:33:46.860116 getajob-0.2.6/LICENSE
+-rw-r--r--   0        0        0       69 2023-06-13 00:33:46.860116 getajob-0.2.6/README.md
+-rw-r--r--   0        0        0       22 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/__init__.py
+-rw-r--r--   0        0        0     1811 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/abstractions/models.py
+-rw-r--r--   0        0        0     8332 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/abstractions/repository.py
+-rw-r--r--   0        0        0     1341 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/config/settings.py
+-rw-r--r--   0        0        0        0 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/admin/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/admin/search/__init__.py
+-rw-r--r--   0        0        0      141 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/admin/search/models.py
+-rw-r--r--   0        0        0      394 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/admin/search/repository.py
+-rw-r--r--   0        0        0        0 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/admin/users/__init__.py
+-rw-r--r--   0        0        0      620 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/admin/users/models.py
+-rw-r--r--   0        0        0      598 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/admin/users/repository.py
+-rw-r--r--   0        0        0        0 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/ai/text/__init__.py
+-rw-r--r--   0        0        0      823 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/ai/text/models.py
+-rw-r--r--   0        0        0     2470 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/ai/text/repository.py
+-rw-r--r--   0        0        0        0 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/companies/__init__.py
+-rw-r--r--   0        0        0      102 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/companies/models.py
+-rw-r--r--   0        0        0      395 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/companies/repository.py
+-rw-r--r--   0        0        0        0 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/jobs/__init__.py
+-rw-r--r--   0        0        0     3021 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/jobs/models.py
+-rw-r--r--   0        0        0     1120 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/jobs/repository.py
+-rw-r--r--   0        0        0      462 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/jobs/unit_of_work.py
+-rw-r--r--   0        0        0        0 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/scheduled_events/__init__.py
+-rw-r--r--   0        0        0     1155 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/scheduled_events/models.py
+-rw-r--r--   0        0        0     1556 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/scheduled_events/repository.py
+-rw-r--r--   0        0        0        0 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/static/__init__.py
+-rw-r--r--   0        0        0     1327 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/static/repository.py
+-rw-r--r--   0        0        0        0 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/users/cover_letters/__init__.py
+-rw-r--r--   0        0        0      277 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/users/cover_letters/models.py
+-rw-r--r--   0        0        0      516 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/users/cover_letters/repository.py
+-rw-r--r--   0        0        0       89 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/users/models.py
+-rw-r--r--   0        0        0      568 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/users/repository.py
+-rw-r--r--   0        0        0        0 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/users/resumes/__init__.py
+-rw-r--r--   0        0        0      196 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/users/resumes/models.py
+-rw-r--r--   0        0        0      462 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/users/resumes/repository.py
+-rw-r--r--   0        0        0        0 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/users/sessions/__init__.py
+-rw-r--r--   0        0        0      306 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/users/sessions/models.py
+-rw-r--r--   0        0        0        0 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/users/skills/__init__.py
+-rw-r--r--   0        0        0      404 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/users/skills/models.py
+-rw-r--r--   0        0        0      491 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/users/skills/repository.py
+-rw-r--r--   0        0        0     2318 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/exceptions.py
+-rw-r--r--   0        0        0      375 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/utils.py
+-rw-r--r--   0        0        0        0 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/__init__.py
+-rw-r--r--   0        0        0      165 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/aiocron.py
+-rw-r--r--   0        0        0      466 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/algolia/models.py
+-rw-r--r--   0        0        0     1385 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/algolia/repository.py
+-rw-r--r--   0        0        0        0 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/clerk/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/clerk/companies/__init__.py
+-rw-r--r--   0        0        0      894 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/clerk/companies/models.py
+-rw-r--r--   0        0        0     1848 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/clerk/companies/repository.py
+-rw-r--r--   0        0        0      103 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/clerk/exceptions.py
+-rw-r--r--   0        0        0      413 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/clerk/models.py
+-rw-r--r--   0        0        0        0 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/clerk/recruiter_invitation/__init__.py
+-rw-r--r--   0        0        0      747 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/clerk/recruiter_invitation/models.py
+-rw-r--r--   0        0        0     2120 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/clerk/recruiter_invitation/repository.py
+-rw-r--r--   0        0        0        0 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/clerk/recruiters/__init__.py
+-rw-r--r--   0        0        0     1748 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/clerk/recruiters/models.py
+-rw-r--r--   0        0        0     2774 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/clerk/recruiters/repository.py
+-rw-r--r--   0        0        0     3021 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/clerk/repository.py
+-rw-r--r--   0        0        0        0 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/clerk/users/__init__.py
+-rw-r--r--   0        0        0     1320 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/clerk/users/models.py
+-rw-r--r--   0        0        0     1839 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/clerk/users/repository.py
+-rw-r--r--   0        0        0     9580 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/firebase.py
+-rw-r--r--   0        0        0        0 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/kafka/__init__.py
+-rw-r--r--   0        0        0      724 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/kafka/authentication.py
+-rw-r--r--   0        0        0      320 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/kafka/exceptions.py
+-rw-r--r--   0        0        0     1254 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/kafka/kafka.py
+-rw-r--r--   0        0        0      221 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/kafka/mock.py
+-rw-r--r--   0        0        0     1480 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/kafka/models.py
+-rw-r--r--   0        0        0      589 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/kafka/repository.py
+-rw-r--r--   0        0        0     1862 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/openai.py
+-rw-r--r--   0        0        0      599 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/sendgrid/sendgrid.py
+-rw-r--r--   0        0        0      251 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/sentry.py
+-rw-r--r--   0        0        0     1742 2023-06-13 00:33:46.864116 getajob-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     2805 1970-01-01 00:00:00.000000 getajob-0.2.6/PKG-INFO
```

### Comparing `getajob-0.2.5/LICENSE` & `getajob-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `getajob-0.2.5/getajob/abstractions/models.py` & `getajob-0.2.6/getajob/abstractions/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.5/getajob/abstractions/repository.py` & `getajob-0.2.6/getajob/abstractions/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.5/getajob/config/settings.py` & `getajob-0.2.6/getajob/config/settings.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.5/getajob/contexts/admin/users/models.py` & `getajob-0.2.6/getajob/contexts/admin/users/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.5/getajob/contexts/admin/users/repository.py` & `getajob-0.2.6/getajob/contexts/admin/users/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.5/getajob/contexts/ai/text/models.py` & `getajob-0.2.6/getajob/contexts/ai/text/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.5/getajob/contexts/ai/text/repository.py` & `getajob-0.2.6/getajob/contexts/ai/text/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.5/getajob/contexts/jobs/models.py` & `getajob-0.2.6/getajob/contexts/jobs/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.5/getajob/contexts/jobs/repository.py` & `getajob-0.2.6/getajob/contexts/jobs/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.5/getajob/contexts/scheduled_events/models.py` & `getajob-0.2.6/getajob/contexts/scheduled_events/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.5/getajob/contexts/scheduled_events/repository.py` & `getajob-0.2.6/getajob/contexts/scheduled_events/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.5/getajob/contexts/static/repository.py` & `getajob-0.2.6/getajob/contexts/static/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.5/getajob/contexts/users/cover_letters/repository.py` & `getajob-0.2.6/getajob/contexts/users/cover_letters/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.5/getajob/contexts/users/repository.py` & `getajob-0.2.6/getajob/contexts/users/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.5/getajob/exceptions.py` & `getajob-0.2.6/getajob/exceptions.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.5/getajob/vendor/clerk/companies/models.py` & `getajob-0.2.6/getajob/vendor/clerk/companies/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.5/getajob/vendor/clerk/companies/repository.py` & `getajob-0.2.6/getajob/vendor/clerk/companies/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.5/getajob/vendor/clerk/recruiter_invitation/models.py` & `getajob-0.2.6/getajob/vendor/clerk/recruiter_invitation/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.5/getajob/vendor/clerk/recruiter_invitation/repository.py` & `getajob-0.2.6/getajob/vendor/clerk/recruiter_invitation/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.5/getajob/vendor/clerk/recruiters/models.py` & `getajob-0.2.6/getajob/vendor/clerk/recruiters/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.5/getajob/vendor/clerk/recruiters/repository.py` & `getajob-0.2.6/getajob/vendor/clerk/recruiters/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.5/getajob/vendor/clerk/users/models.py` & `getajob-0.2.6/getajob/vendor/clerk/users/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.5/getajob/vendor/clerk/users/repository.py` & `getajob-0.2.6/getajob/vendor/clerk/users/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.5/getajob/vendor/firebase.py` & `getajob-0.2.6/getajob/vendor/firebase.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.5/getajob/vendor/kafka/authentication.py` & `getajob-0.2.6/getajob/vendor/kafka/authentication.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.5/getajob/vendor/kafka/kafka.py` & `getajob-0.2.6/getajob/vendor/kafka/kafka.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.5/getajob/vendor/kafka/models.py` & `getajob-0.2.6/getajob/vendor/kafka/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.5/getajob/vendor/kafka/repository.py` & `getajob-0.2.6/getajob/vendor/kafka/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.5/getajob/vendor/openai.py` & `getajob-0.2.6/getajob/vendor/openai.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.5/getajob/vendor/sendgrid/sendgrid.py` & `getajob-0.2.6/getajob/vendor/sendgrid/sendgrid.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.5/pyproject.toml` & `getajob-0.2.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "getajob"
-version = "0.2.5"
+version = "0.2.6"
 description = ""
 authors = ["Your Name <you@example.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 aiohttp = "3.8.4"
```

### Comparing `getajob-0.2.5/PKG-INFO` & `getajob-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getajob
-Version: 0.2.5
+Version: 0.2.6
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiocron (>=1.8,<2.0)
```

