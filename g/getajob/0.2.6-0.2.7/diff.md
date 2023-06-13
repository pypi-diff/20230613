# Comparing `tmp/getajob-0.2.6.tar.gz` & `tmp/getajob-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getajob-0.2.6.tar", max compression
+gzip compressed data, was "getajob-0.2.7.tar", max compression
```

## Comparing `getajob-0.2.6.tar` & `getajob-0.2.7.tar`

### file list

```diff
@@ -1,77 +1,83 @@
--rw-r--r--   0        0        0    11357 2023-06-13 00:33:46.860116 getajob-0.2.6/LICENSE
--rw-r--r--   0        0        0       69 2023-06-13 00:33:46.860116 getajob-0.2.6/README.md
--rw-r--r--   0        0        0       22 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/__init__.py
--rw-r--r--   0        0        0     1811 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/abstractions/models.py
--rw-r--r--   0        0        0     8332 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/abstractions/repository.py
--rw-r--r--   0        0        0     1341 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/config/settings.py
--rw-r--r--   0        0        0        0 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/admin/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/admin/search/__init__.py
--rw-r--r--   0        0        0      141 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/admin/search/models.py
--rw-r--r--   0        0        0      394 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/admin/search/repository.py
--rw-r--r--   0        0        0        0 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/admin/users/__init__.py
--rw-r--r--   0        0        0      620 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/admin/users/models.py
--rw-r--r--   0        0        0      598 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/admin/users/repository.py
--rw-r--r--   0        0        0        0 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/ai/text/__init__.py
--rw-r--r--   0        0        0      823 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/ai/text/models.py
--rw-r--r--   0        0        0     2470 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/ai/text/repository.py
--rw-r--r--   0        0        0        0 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/companies/__init__.py
--rw-r--r--   0        0        0      102 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/companies/models.py
--rw-r--r--   0        0        0      395 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/companies/repository.py
--rw-r--r--   0        0        0        0 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/jobs/__init__.py
--rw-r--r--   0        0        0     3021 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/jobs/models.py
--rw-r--r--   0        0        0     1120 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/jobs/repository.py
--rw-r--r--   0        0        0      462 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/jobs/unit_of_work.py
--rw-r--r--   0        0        0        0 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/scheduled_events/__init__.py
--rw-r--r--   0        0        0     1155 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/scheduled_events/models.py
--rw-r--r--   0        0        0     1556 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/scheduled_events/repository.py
--rw-r--r--   0        0        0        0 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/static/__init__.py
--rw-r--r--   0        0        0     1327 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/static/repository.py
--rw-r--r--   0        0        0        0 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/users/cover_letters/__init__.py
--rw-r--r--   0        0        0      277 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/users/cover_letters/models.py
--rw-r--r--   0        0        0      516 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/users/cover_letters/repository.py
--rw-r--r--   0        0        0       89 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/users/models.py
--rw-r--r--   0        0        0      568 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/users/repository.py
--rw-r--r--   0        0        0        0 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/users/resumes/__init__.py
--rw-r--r--   0        0        0      196 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/users/resumes/models.py
--rw-r--r--   0        0        0      462 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/users/resumes/repository.py
--rw-r--r--   0        0        0        0 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/users/sessions/__init__.py
--rw-r--r--   0        0        0      306 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/users/sessions/models.py
--rw-r--r--   0        0        0        0 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/users/skills/__init__.py
--rw-r--r--   0        0        0      404 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/users/skills/models.py
--rw-r--r--   0        0        0      491 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/contexts/users/skills/repository.py
--rw-r--r--   0        0        0     2318 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/exceptions.py
--rw-r--r--   0        0        0      375 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/utils.py
--rw-r--r--   0        0        0        0 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/__init__.py
--rw-r--r--   0        0        0      165 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/aiocron.py
--rw-r--r--   0        0        0      466 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/algolia/models.py
--rw-r--r--   0        0        0     1385 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/algolia/repository.py
--rw-r--r--   0        0        0        0 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/clerk/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/clerk/companies/__init__.py
--rw-r--r--   0        0        0      894 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/clerk/companies/models.py
--rw-r--r--   0        0        0     1848 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/clerk/companies/repository.py
--rw-r--r--   0        0        0      103 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/clerk/exceptions.py
--rw-r--r--   0        0        0      413 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/clerk/models.py
--rw-r--r--   0        0        0        0 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/clerk/recruiter_invitation/__init__.py
--rw-r--r--   0        0        0      747 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/clerk/recruiter_invitation/models.py
--rw-r--r--   0        0        0     2120 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/clerk/recruiter_invitation/repository.py
--rw-r--r--   0        0        0        0 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/clerk/recruiters/__init__.py
--rw-r--r--   0        0        0     1748 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/clerk/recruiters/models.py
--rw-r--r--   0        0        0     2774 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/clerk/recruiters/repository.py
--rw-r--r--   0        0        0     3021 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/clerk/repository.py
--rw-r--r--   0        0        0        0 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/clerk/users/__init__.py
--rw-r--r--   0        0        0     1320 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/clerk/users/models.py
--rw-r--r--   0        0        0     1839 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/clerk/users/repository.py
--rw-r--r--   0        0        0     9580 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/firebase.py
--rw-r--r--   0        0        0        0 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/kafka/__init__.py
--rw-r--r--   0        0        0      724 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/kafka/authentication.py
--rw-r--r--   0        0        0      320 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/kafka/exceptions.py
--rw-r--r--   0        0        0     1254 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/kafka/kafka.py
--rw-r--r--   0        0        0      221 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/kafka/mock.py
--rw-r--r--   0        0        0     1480 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/kafka/models.py
--rw-r--r--   0        0        0      589 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/kafka/repository.py
--rw-r--r--   0        0        0     1862 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/openai.py
--rw-r--r--   0        0        0      599 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/sendgrid/sendgrid.py
--rw-r--r--   0        0        0      251 2023-06-13 00:33:46.860116 getajob-0.2.6/getajob/vendor/sentry.py
--rw-r--r--   0        0        0     1742 2023-06-13 00:33:46.864116 getajob-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     2805 1970-01-01 00:00:00.000000 getajob-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-13 02:01:30.836240 getajob-0.2.7/LICENSE
+-rw-r--r--   0        0        0       69 2023-06-13 02:01:30.840240 getajob-0.2.7/README.md
+-rw-r--r--   0        0        0       22 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/__init__.py
+-rw-r--r--   0        0        0     1811 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/abstractions/models.py
+-rw-r--r--   0        0        0     8332 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/abstractions/repository.py
+-rw-r--r--   0        0        0     1308 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/config/settings.py
+-rw-r--r--   0        0        0        0 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/admin/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/admin/search/__init__.py
+-rw-r--r--   0        0        0      141 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/admin/search/models.py
+-rw-r--r--   0        0        0      394 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/admin/search/repository.py
+-rw-r--r--   0        0        0        0 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/admin/users/__init__.py
+-rw-r--r--   0        0        0      620 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/admin/users/models.py
+-rw-r--r--   0        0        0      598 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/admin/users/repository.py
+-rw-r--r--   0        0        0        0 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/ai/text/__init__.py
+-rw-r--r--   0        0        0      823 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/ai/text/models.py
+-rw-r--r--   0        0        0     2470 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/ai/text/repository.py
+-rw-r--r--   0        0        0        0 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/companies/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/companies/invitations/__init__.py
+-rw-r--r--   0        0        0      145 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/companies/invitations/models.py
+-rw-r--r--   0        0        0      444 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/companies/invitations/repository.py
+-rw-r--r--   0        0        0      102 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/companies/models.py
+-rw-r--r--   0        0        0        0 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/companies/recruiters/__init__.py
+-rw-r--r--   0        0        0      117 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/companies/recruiters/models.py
+-rw-r--r--   0        0        0      402 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/companies/recruiters/repository.py
+-rw-r--r--   0        0        0      395 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/companies/repository.py
+-rw-r--r--   0        0        0        0 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/jobs/__init__.py
+-rw-r--r--   0        0        0     3021 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/jobs/models.py
+-rw-r--r--   0        0        0     1120 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/jobs/repository.py
+-rw-r--r--   0        0        0      462 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/jobs/unit_of_work.py
+-rw-r--r--   0        0        0        0 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/scheduled_events/__init__.py
+-rw-r--r--   0        0        0     1155 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/scheduled_events/models.py
+-rw-r--r--   0        0        0     1556 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/scheduled_events/repository.py
+-rw-r--r--   0        0        0        0 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/static/__init__.py
+-rw-r--r--   0        0        0     1327 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/static/repository.py
+-rw-r--r--   0        0        0        0 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/users/cover_letters/__init__.py
+-rw-r--r--   0        0        0      277 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/users/cover_letters/models.py
+-rw-r--r--   0        0        0      516 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/users/cover_letters/repository.py
+-rw-r--r--   0        0        0       89 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/users/models.py
+-rw-r--r--   0        0        0      568 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/users/repository.py
+-rw-r--r--   0        0        0        0 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/users/resumes/__init__.py
+-rw-r--r--   0        0        0      196 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/users/resumes/models.py
+-rw-r--r--   0        0        0      462 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/users/resumes/repository.py
+-rw-r--r--   0        0        0        0 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/users/sessions/__init__.py
+-rw-r--r--   0        0        0      306 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/users/sessions/models.py
+-rw-r--r--   0        0        0        0 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/users/skills/__init__.py
+-rw-r--r--   0        0        0      404 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/users/skills/models.py
+-rw-r--r--   0        0        0      491 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/users/skills/repository.py
+-rw-r--r--   0        0        0     2318 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/exceptions.py
+-rw-r--r--   0        0        0      375 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/utils.py
+-rw-r--r--   0        0        0        0 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/__init__.py
+-rw-r--r--   0        0        0      165 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/aiocron.py
+-rw-r--r--   0        0        0      702 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/algolia/models.py
+-rw-r--r--   0        0        0     1056 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/algolia/repository.py
+-rw-r--r--   0        0        0        0 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/clerk/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/clerk/companies/__init__.py
+-rw-r--r--   0        0        0      894 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/clerk/companies/models.py
+-rw-r--r--   0        0        0     1848 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/clerk/companies/repository.py
+-rw-r--r--   0        0        0      103 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/clerk/exceptions.py
+-rw-r--r--   0        0        0      413 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/clerk/models.py
+-rw-r--r--   0        0        0        0 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/clerk/recruiter_invitation/__init__.py
+-rw-r--r--   0        0        0      747 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/clerk/recruiter_invitation/models.py
+-rw-r--r--   0        0        0     2486 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/clerk/recruiter_invitation/repository.py
+-rw-r--r--   0        0        0        0 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/clerk/recruiters/__init__.py
+-rw-r--r--   0        0        0     1748 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/clerk/recruiters/models.py
+-rw-r--r--   0        0        0     2774 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/clerk/recruiters/repository.py
+-rw-r--r--   0        0        0     3101 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/clerk/repository.py
+-rw-r--r--   0        0        0        0 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/clerk/users/__init__.py
+-rw-r--r--   0        0        0     1320 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/clerk/users/models.py
+-rw-r--r--   0        0        0     1839 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/clerk/users/repository.py
+-rw-r--r--   0        0        0     9580 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/firebase.py
+-rw-r--r--   0        0        0        0 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/kafka/__init__.py
+-rw-r--r--   0        0        0      724 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/kafka/authentication.py
+-rw-r--r--   0        0        0      320 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/kafka/exceptions.py
+-rw-r--r--   0        0        0     1254 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/kafka/kafka.py
+-rw-r--r--   0        0        0      221 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/kafka/mock.py
+-rw-r--r--   0        0        0     1480 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/kafka/models.py
+-rw-r--r--   0        0        0      589 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/kafka/repository.py
+-rw-r--r--   0        0        0     1862 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/openai.py
+-rw-r--r--   0        0        0      599 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/sendgrid/sendgrid.py
+-rw-r--r--   0        0        0      251 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/sentry.py
+-rw-r--r--   0        0        0     1742 2023-06-13 02:01:30.844240 getajob-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     2805 1970-01-01 00:00:00.000000 getajob-0.2.7/PKG-INFO
```

### Comparing `getajob-0.2.6/LICENSE` & `getajob-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `getajob-0.2.6/getajob/abstractions/models.py` & `getajob-0.2.7/getajob/abstractions/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.6/getajob/abstractions/repository.py` & `getajob-0.2.7/getajob/abstractions/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.6/getajob/config/settings.py` & `getajob-0.2.7/getajob/config/settings.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,15 +20,14 @@
     OPENAI_MODEL_ABILITY: int = 1
 
     # Clerk config
     CLERK_JWT_PEM_KEY: str = os.getenv("CLERK_JWT_PEM_KEY", "").replace(r"\n", "\n")
     CLERK_TOKEN_LEEWAY: int = 300
     CLERK_USER_WEBHOOK_SECRET: str = ""
     CLERK_SECRET_KEY: str = ""
-    CLERK_API_BASE_URL: str = ""
 
     DEFAULT_PAGE_LIMIT: int = 20
 
     LOCAL_TESTING: bool = get_bool_from_string(os.getenv("LOCAL_TESTING", "false"))
     ENABLED_KAFKA_EVENTS: bool = get_bool_from_string(
         os.getenv("ENABLED_KAFKA_EVENTS", "false")
     )
```

### Comparing `getajob-0.2.6/getajob/contexts/admin/users/models.py` & `getajob-0.2.7/getajob/contexts/admin/users/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.6/getajob/contexts/admin/users/repository.py` & `getajob-0.2.7/getajob/contexts/admin/users/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.6/getajob/contexts/ai/text/models.py` & `getajob-0.2.7/getajob/contexts/ai/text/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.6/getajob/contexts/ai/text/repository.py` & `getajob-0.2.7/getajob/contexts/ai/text/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.6/getajob/contexts/jobs/models.py` & `getajob-0.2.7/getajob/contexts/jobs/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.6/getajob/contexts/jobs/repository.py` & `getajob-0.2.7/getajob/contexts/jobs/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.6/getajob/contexts/scheduled_events/models.py` & `getajob-0.2.7/getajob/contexts/scheduled_events/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.6/getajob/contexts/scheduled_events/repository.py` & `getajob-0.2.7/getajob/contexts/scheduled_events/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.6/getajob/contexts/static/repository.py` & `getajob-0.2.7/getajob/contexts/static/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.6/getajob/contexts/users/cover_letters/repository.py` & `getajob-0.2.7/getajob/contexts/users/cover_letters/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.6/getajob/contexts/users/repository.py` & `getajob-0.2.7/getajob/contexts/users/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.6/getajob/exceptions.py` & `getajob-0.2.7/getajob/exceptions.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.6/getajob/vendor/clerk/companies/models.py` & `getajob-0.2.7/getajob/vendor/clerk/companies/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.6/getajob/vendor/clerk/companies/repository.py` & `getajob-0.2.7/getajob/vendor/clerk/companies/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.6/getajob/vendor/clerk/recruiter_invitation/models.py` & `getajob-0.2.7/getajob/vendor/clerk/recruiter_invitation/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.6/getajob/vendor/clerk/recruiter_invitation/repository.py` & `getajob-0.2.7/getajob/vendor/clerk/recruiter_invitation/repository.py`

 * *Files 14% similar despite different names*

```diff
@@ -37,16 +37,28 @@
             ClerkCompanyInvitationsWebhookType.organization_invitation_revoked: self.revoke_invitation,
             ClerkCompanyInvitationsWebhookType.organization_invitation_accepted: self.accept_invitation,
         }
         return event_dict[event.type](event)
 
     def create_invitation(self, event: ClerkCompanyInvitationsWebhookEvent):
         create_event = ClerkCompanyInvitation(**event.data)
-        return self.create(data=create_event, provided_id=create_event.id)
+        return self.create(
+            data=create_event,
+            provided_id=create_event.id,
+            parent_collections={Entity.COMPANIES.value: create_event.organization_id},
+        )
 
     def revoke_invitation(self, event: ClerkCompanyInvitationsWebhookEvent):
         update_event = ClerkCompanyInvitation(**event.data)
-        return self.update(doc_id=update_event.id, data=update_event)
+        return self.update(
+            doc_id=update_event.id,
+            data=update_event,
+            parent_collections={Entity.COMPANIES.value: update_event.organization_id},
+        )
 
     def accept_invitation(self, event: ClerkCompanyInvitationsWebhookEvent):
         update_event = ClerkCompanyInvitation(**event.data)
-        return self.update(doc_id=update_event.id, data=update_event)
+        return self.update(
+            doc_id=update_event.id,
+            data=update_event,
+            parent_collections={Entity.COMPANIES.value: update_event.organization_id},
+        )
```

### Comparing `getajob-0.2.6/getajob/vendor/clerk/recruiters/models.py` & `getajob-0.2.7/getajob/vendor/clerk/recruiters/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.6/getajob/vendor/clerk/recruiters/repository.py` & `getajob-0.2.7/getajob/vendor/clerk/recruiters/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.6/getajob/vendor/clerk/repository.py` & `getajob-0.2.7/getajob/vendor/clerk/repository.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,35 +31,35 @@
         return response
 
     def _format_response_to_model(self, response: Response, model: BaseModel):
         response_json = response.json()
         if "data" in response_json:
             response_json = response_json["data"]
         if isinstance(response_json, list):
-            return [model(**item) for item in response_json]
-        return model(**response_json)
+            return [model(**item) for item in response_json]  # type: ignore
+        return model(**response_json)  # type: ignore
 
     def get_user(self, user_id: str):
         endpoint = f"/v1/users/{user_id}"
         res = self._make_request("GET", endpoint)
         if res.status_code == 404:
             raise UserNotFoundException()
-        return self._format_response_to_model(res, ClerkUser)
+        return self._format_response_to_model(res, ClerkUser)  # type: ignore
 
     def get_company(self, company_id: str):
         endpoint = f"/v1/organizations/{company_id}"
         res = self._make_request("GET", endpoint)
         if res.status_code == 404:
             raise CompanyNotFoundException()
-        return self._format_response_to_model(res, ClerkCompany)
+        return self._format_response_to_model(res, ClerkCompany)  # type: ignore
 
     def get_company_invitations(self, company_id: str):
         endpoint = f"/v1/organizations/{company_id}/invitations/pending"
         res = self._make_request("GET", endpoint)
-        return self._format_response_to_model(res, ClerkCompanyInvitation)
+        return self._format_response_to_model(res, ClerkCompanyInvitation)  # type: ignore
 
     def get_company_recruiters(self, company_id):
         endpoint = f"/v1/organizations/{company_id}/memberships"
         res = self._make_request("GET", endpoint)
         return self._format_response_to_model(res, ClerkCompanyMembership)
 
     def get_companies_by_user_id(self, user_id):
```

### Comparing `getajob-0.2.6/getajob/vendor/clerk/users/models.py` & `getajob-0.2.7/getajob/vendor/clerk/users/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.6/getajob/vendor/clerk/users/repository.py` & `getajob-0.2.7/getajob/vendor/clerk/users/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.6/getajob/vendor/firebase.py` & `getajob-0.2.7/getajob/vendor/firebase.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.6/getajob/vendor/kafka/authentication.py` & `getajob-0.2.7/getajob/vendor/kafka/authentication.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.6/getajob/vendor/kafka/kafka.py` & `getajob-0.2.7/getajob/vendor/kafka/kafka.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.6/getajob/vendor/kafka/models.py` & `getajob-0.2.7/getajob/vendor/kafka/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.6/getajob/vendor/kafka/repository.py` & `getajob-0.2.7/getajob/vendor/kafka/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.6/getajob/vendor/openai.py` & `getajob-0.2.7/getajob/vendor/openai.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.6/getajob/vendor/sendgrid/sendgrid.py` & `getajob-0.2.7/getajob/vendor/sendgrid/sendgrid.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.6/pyproject.toml` & `getajob-0.2.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "getajob"
-version = "0.2.6"
+version = "0.2.7"
 description = ""
 authors = ["Your Name <you@example.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 aiohttp = "3.8.4"
```

### Comparing `getajob-0.2.6/PKG-INFO` & `getajob-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getajob
-Version: 0.2.6
+Version: 0.2.7
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiocron (>=1.8,<2.0)
```

