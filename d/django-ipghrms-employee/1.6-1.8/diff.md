# Comparing `tmp/django-ipghrms-employee-1.6.tar.gz` & `tmp/django-ipghrms-employee-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-ipghrms-employee-1.6.tar", last modified: Mon Jun  5 04:27:45 2023, max compression
+gzip compressed data, was "django-ipghrms-employee-1.8.tar", last modified: Tue Jun 13 13:20:36 2023, max compression
```

## Comparing `django-ipghrms-employee-1.6.tar` & `django-ipghrms-employee-1.8.tar`

### file list

```diff
@@ -1,284 +1,284 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 04:27:45.589572 django-ipghrms-employee-1.6/
--rw-rw-rw-   0        0        0     1068 2023-03-27 14:44:23.000000 django-ipghrms-employee-1.6/LICENSE
--rw-rw-rw-   0        0        0      224 2023-03-27 14:44:31.000000 django-ipghrms-employee-1.6/MANIFEST.in
--rw-rw-rw-   0        0        0      951 2023-06-05 04:27:45.589572 django-ipghrms-employee-1.6/PKG-INFO
--rw-rw-rw-   0        0        0      503 2023-03-27 14:20:21.000000 django-ipghrms-employee-1.6/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-05 04:27:40.650743 django-ipghrms-employee-1.6/django_ipghrms_employee.egg-info/
--rw-rw-rw-   0        0        0      951 2023-06-05 04:27:40.000000 django-ipghrms-employee-1.6/django_ipghrms_employee.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    13169 2023-06-05 04:27:40.000000 django-ipghrms-employee-1.6/django_ipghrms_employee.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 04:27:40.000000 django-ipghrms-employee-1.6/django_ipghrms_employee.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-05 04:27:40.000000 django-ipghrms-employee-1.6/django_ipghrms_employee.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-05 04:27:40.750326 django-ipghrms-employee-1.6/employee/
--rw-rw-rw-   0        0        0        0 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/__init__.py
--rw-rw-rw-   0        0        0     1348 2023-06-05 04:17:59.000000 django-ipghrms-employee-1.6/employee/admin.py
-drwxrwxrwx   0        0        0        0 2023-06-05 04:27:40.763969 django-ipghrms-employee-1.6/employee/api/
--rw-rw-rw-   0        0        0        0 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 04:27:40.882200 django-ipghrms-employee-1.6/employee/api/__pycache__/
--rw-rw-rw-   0        0        0      141 2022-11-07 13:19:37.000000 django-ipghrms-employee-1.6/employee/api/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      139 2022-10-20 01:02:26.000000 django-ipghrms-employee-1.6/employee/api/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0      147 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/api/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0      718 2023-01-17 15:06:20.000000 django-ipghrms-employee-1.6/employee/api/__pycache__/urls.cpython-310.pyc
--rw-rw-rw-   0        0        0      664 2022-10-20 01:02:26.000000 django-ipghrms-employee-1.6/employee/api/__pycache__/urls.cpython-37.pyc
--rw-rw-rw-   0        0        0      674 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/api/__pycache__/urls.cpython-39.pyc
--rw-rw-rw-   0        0        0     8468 2023-02-13 01:12:07.000000 django-ipghrms-employee-1.6/employee/api/__pycache__/views.cpython-310.pyc
--rw-rw-rw-   0        0        0     7493 2022-10-20 01:02:26.000000 django-ipghrms-employee-1.6/employee/api/__pycache__/views.cpython-37.pyc
--rw-rw-rw-   0        0        0     7168 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/api/__pycache__/views.cpython-39.pyc
--rw-rw-rw-   0        0        0      647 2023-01-17 15:06:18.000000 django-ipghrms-employee-1.6/employee/api/urls.py
--rw-rw-rw-   0        0        0    10312 2023-02-13 01:12:04.000000 django-ipghrms-employee-1.6/employee/api/views.py
--rw-rw-rw-   0        0        0      132 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/apps.py
--rw-rw-rw-   0        0        0      152 2023-03-13 01:01:19.000000 django-ipghrms-employee-1.6/employee/contact_urls.py
--rw-rw-rw-   0        0        0      155 2023-03-08 09:34:17.000000 django-ipghrms-employee-1.6/employee/context_processors.py
--rw-rw-rw-   0        0        0    19649 2023-03-15 10:22:24.000000 django-ipghrms-employee-1.6/employee/forms.py
-drwxrwxrwx   0        0        0        0 2023-06-05 04:27:41.091381 django-ipghrms-employee-1.6/employee/migrations/
--rw-rw-rw-   0        0        0    20094 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/migrations/0001_initial.py
--rw-rw-rw-   0        0        0     1798 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/migrations/0002_curempposition_curempdivision.py
--rw-rw-rw-   0        0        0      422 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/migrations/0003_employee_is_new.py
--rw-rw-rw-   0        0        0      425 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/migrations/0004_employee_emp_id.py
--rw-rw-rw-   0        0        0      824 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/migrations/0005_alter_employee_blood_alter_employee_father_and_more.py
--rw-rw-rw-   0        0        0     1310 2022-11-04 05:28:45.000000 django-ipghrms-employee-1.6/employee/migrations/0006_fidnumber_bank_address_fidnumber_customer_name_and_more.py
--rw-rw-rw-   0        0        0      488 2022-11-04 05:28:45.000000 django-ipghrms-employee-1.6/employee/migrations/0007_alter_fidnumber_customer_name.py
--rw-rw-rw-   0        0        0      737 2022-11-04 05:28:45.000000 django-ipghrms-employee-1.6/employee/migrations/0008_empspecialize.py
--rw-rw-rw-   0        0        0      438 2022-11-04 05:28:45.000000 django-ipghrms-employee-1.6/employee/migrations/0009_alter_empspecialize_name.py
--rw-rw-rw-   0        0        0      557 2022-11-22 01:39:19.000000 django-ipghrms-employee-1.6/employee/migrations/0010_formaleducation_year.py
--rw-rw-rw-   0        0        0      556 2022-11-22 01:56:32.000000 django-ipghrms-employee-1.6/employee/migrations/0011_nonformaleducation_year.py
--rw-rw-rw-   0        0        0      851 2022-11-22 02:04:54.000000 django-ipghrms-employee-1.6/employee/migrations/0012_auto_20221122_1104.py
--rw-rw-rw-   0        0        0     1680 2022-11-22 02:27:59.000000 django-ipghrms-employee-1.6/employee/migrations/0013_auto_20221122_1127.py
--rw-rw-rw-   0        0        0     2814 2022-11-30 14:03:29.000000 django-ipghrms-employee-1.6/employee/migrations/0014_auto_20221130_2303.py
--rw-rw-rw-   0        0        0     1093 2022-11-30 14:04:07.000000 django-ipghrms-employee-1.6/employee/migrations/0015_auto_20221130_2304.py
--rw-rw-rw-   0        0        0     1177 2022-11-30 14:26:44.000000 django-ipghrms-employee-1.6/employee/migrations/0016_auto_20221130_2326.py
--rw-rw-rw-   0        0        0      916 2022-11-30 14:35:38.000000 django-ipghrms-employee-1.6/employee/migrations/0017_auto_20221130_2335.py
--rw-rw-rw-   0        0        0      411 2022-12-08 01:21:23.000000 django-ipghrms-employee-1.6/employee/migrations/0018_employee_pin.py
--rw-rw-rw-   0        0        0      405 2022-12-14 12:14:22.000000 django-ipghrms-employee-1.6/employee/migrations/0019_employee_ext.py
--rw-rw-rw-   0        0        0      801 2023-01-17 09:29:03.000000 django-ipghrms-employee-1.6/employee/migrations/0020_auto_20230117_1829.py
--rw-rw-rw-   0        0        0      663 2023-01-19 10:28:44.000000 django-ipghrms-employee-1.6/employee/migrations/0021_emplanguage_file_language.py
--rw-rw-rw-   0        0        0      710 2023-02-14 13:39:17.000000 django-ipghrms-employee-1.6/employee/migrations/0022_alter_photo_image.py
--rw-rw-rw-   0        0        0      650 2023-02-14 14:31:40.000000 django-ipghrms-employee-1.6/employee/migrations/0023_alter_photo_image.py
--rw-rw-rw-   0        0        0      407 2023-02-23 05:09:35.000000 django-ipghrms-employee-1.6/employee/migrations/0024_alter_fidnumber_options.py
--rw-rw-rw-   0        0        0      982 2023-03-15 09:56:18.000000 django-ipghrms-employee-1.6/employee/migrations/0025_empsignature.py
--rw-rw-rw-   0        0        0        0 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 04:27:41.718539 django-ipghrms-employee-1.6/employee/migrations/__pycache__/
--rw-rw-rw-   0        0        0     7287 2022-11-07 13:19:39.000000 django-ipghrms-employee-1.6/employee/migrations/__pycache__/0001_initial.cpython-310.pyc
--rw-rw-rw-   0        0        0     7215 2022-10-20 01:03:56.000000 django-ipghrms-employee-1.6/employee/migrations/__pycache__/0001_initial.cpython-37.pyc
--rw-rw-rw-   0        0        0     7291 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/migrations/__pycache__/0001_initial.cpython-39.pyc
--rw-rw-rw-   0        0        0     1280 2022-11-07 13:19:39.000000 django-ipghrms-employee-1.6/employee/migrations/__pycache__/0002_curempposition_curempdivision.cpython-310.pyc
--rw-rw-rw-   0        0        0     1260 2022-10-20 01:03:56.000000 django-ipghrms-employee-1.6/employee/migrations/__pycache__/0002_curempposition_curempdivision.cpython-37.pyc
--rw-rw-rw-   0        0        0     1284 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/migrations/__pycache__/0002_curempposition_curempdivision.cpython-39.pyc
--rw-rw-rw-   0        0        0      607 2022-11-07 13:19:39.000000 django-ipghrms-employee-1.6/employee/migrations/__pycache__/0003_employee_is_new.cpython-310.pyc
--rw-rw-rw-   0        0        0      593 2022-10-20 01:03:56.000000 django-ipghrms-employee-1.6/employee/migrations/__pycache__/0003_employee_is_new.cpython-37.pyc
--rw-rw-rw-   0        0        0      611 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/migrations/__pycache__/0003_employee_is_new.cpython-39.pyc
--rw-rw-rw-   0        0        0      618 2022-11-07 13:19:39.000000 django-ipghrms-employee-1.6/employee/migrations/__pycache__/0004_employee_emp_id.cpython-310.pyc
--rw-rw-rw-   0        0        0      604 2022-10-20 01:03:56.000000 django-ipghrms-employee-1.6/employee/migrations/__pycache__/0004_employee_emp_id.cpython-37.pyc
--rw-rw-rw-   0        0        0      622 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/migrations/__pycache__/0004_employee_emp_id.cpython-39.pyc
--rw-rw-rw-   0        0        0      802 2022-11-07 13:19:39.000000 django-ipghrms-employee-1.6/employee/migrations/__pycache__/0005_alter_employee_blood_alter_employee_father_and_more.cpython-310.pyc
--rw-rw-rw-   0        0        0      786 2022-10-20 01:03:56.000000 django-ipghrms-employee-1.6/employee/migrations/__pycache__/0005_alter_employee_blood_alter_employee_father_and_more.cpython-37.pyc
--rw-rw-rw-   0        0        0      806 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/migrations/__pycache__/0005_alter_employee_blood_alter_employee_father_and_more.cpython-39.pyc
--rw-rw-rw-   0        0        0      973 2022-11-07 13:19:39.000000 django-ipghrms-employee-1.6/employee/migrations/__pycache__/0006_fidnumber_bank_address_fidnumber_customer_name_and_more.cpython-310.pyc
--rw-rw-rw-   0        0        0      951 2022-11-05 14:52:09.000000 django-ipghrms-employee-1.6/employee/migrations/__pycache__/0006_fidnumber_bank_address_fidnumber_customer_name_and_more.cpython-37.pyc
--rw-rw-rw-   0        0        0      699 2022-11-07 13:19:39.000000 django-ipghrms-employee-1.6/employee/migrations/__pycache__/0007_alter_fidnumber_customer_name.cpython-310.pyc
--rw-rw-rw-   0        0        0      685 2022-11-05 14:52:09.000000 django-ipghrms-employee-1.6/employee/migrations/__pycache__/0007_alter_fidnumber_customer_name.cpython-37.pyc
--rw-rw-rw-   0        0        0      894 2022-11-07 13:19:39.000000 django-ipghrms-employee-1.6/employee/migrations/__pycache__/0008_empspecialize.cpython-310.pyc
--rw-rw-rw-   0        0        0      878 2022-11-05 14:52:09.000000 django-ipghrms-employee-1.6/employee/migrations/__pycache__/0008_empspecialize.cpython-37.pyc
--rw-rw-rw-   0        0        0      643 2022-11-07 13:19:39.000000 django-ipghrms-employee-1.6/employee/migrations/__pycache__/0009_alter_empspecialize_name.cpython-310.pyc
--rw-rw-rw-   0        0        0      629 2022-11-05 14:52:09.000000 django-ipghrms-employee-1.6/employee/migrations/__pycache__/0009_alter_empspecialize_name.cpython-37.pyc
--rw-rw-rw-   0        0        0      739 2022-11-22 01:39:26.000000 django-ipghrms-employee-1.6/employee/migrations/__pycache__/0010_formaleducation_year.cpython-310.pyc
--rw-rw-rw-   0        0        0      741 2022-11-22 01:56:39.000000 django-ipghrms-employee-1.6/employee/migrations/__pycache__/0011_nonformaleducation_year.cpython-310.pyc
--rw-rw-rw-   0        0        0      815 2022-11-22 02:04:58.000000 django-ipghrms-employee-1.6/employee/migrations/__pycache__/0012_auto_20221122_1104.cpython-310.pyc
--rw-rw-rw-   0        0        0     1198 2022-11-22 02:28:05.000000 django-ipghrms-employee-1.6/employee/migrations/__pycache__/0013_auto_20221122_1127.cpython-310.pyc
--rw-rw-rw-   0        0        0     1353 2022-11-30 14:04:06.000000 django-ipghrms-employee-1.6/employee/migrations/__pycache__/0014_auto_20221130_2303.cpython-310.pyc
--rw-rw-rw-   0        0        0      835 2022-11-30 14:04:17.000000 django-ipghrms-employee-1.6/employee/migrations/__pycache__/0015_auto_20221130_2304.cpython-310.pyc
--rw-rw-rw-   0        0        0      903 2022-11-30 14:26:49.000000 django-ipghrms-employee-1.6/employee/migrations/__pycache__/0016_auto_20221130_2326.cpython-310.pyc
--rw-rw-rw-   0        0        0      876 2022-11-30 14:35:49.000000 django-ipghrms-employee-1.6/employee/migrations/__pycache__/0017_auto_20221130_2335.cpython-310.pyc
--rw-rw-rw-   0        0        0      576 2022-12-08 01:21:27.000000 django-ipghrms-employee-1.6/employee/migrations/__pycache__/0018_employee_pin.cpython-310.pyc
--rw-rw-rw-   0        0        0      570 2022-12-14 12:14:28.000000 django-ipghrms-employee-1.6/employee/migrations/__pycache__/0019_employee_ext.cpython-310.pyc
--rw-rw-rw-   0        0        0      908 2023-01-17 09:25:30.000000 django-ipghrms-employee-1.6/employee/migrations/__pycache__/0020_auto_20230117_1825.cpython-310.pyc
--rw-rw-rw-   0        0        0      908 2023-01-17 09:27:40.000000 django-ipghrms-employee-1.6/employee/migrations/__pycache__/0020_auto_20230117_1827.cpython-310.pyc
--rw-rw-rw-   0        0        0      908 2023-01-17 09:29:07.000000 django-ipghrms-employee-1.6/employee/migrations/__pycache__/0020_auto_20230117_1829.cpython-310.pyc
--rw-rw-rw-   0        0        0      884 2023-01-19 10:28:51.000000 django-ipghrms-employee-1.6/employee/migrations/__pycache__/0021_emplanguage_file_language.cpython-310.pyc
--rw-rw-rw-   0        0        0      911 2023-02-14 13:39:22.000000 django-ipghrms-employee-1.6/employee/migrations/__pycache__/0022_alter_photo_image.cpython-310.pyc
--rw-rw-rw-   0        0        0      863 2023-02-14 14:31:44.000000 django-ipghrms-employee-1.6/employee/migrations/__pycache__/0023_alter_photo_image.cpython-310.pyc
--rw-rw-rw-   0        0        0      586 2023-02-23 05:09:41.000000 django-ipghrms-employee-1.6/employee/migrations/__pycache__/0024_alter_fidnumber_options.cpython-310.pyc
--rw-rw-rw-   0        0        0     1136 2023-03-15 09:56:33.000000 django-ipghrms-employee-1.6/employee/migrations/__pycache__/0025_empsignature.cpython-310.pyc
--rw-rw-rw-   0        0        0      148 2022-11-07 13:19:39.000000 django-ipghrms-employee-1.6/employee/migrations/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      146 2022-10-20 01:03:56.000000 django-ipghrms-employee-1.6/employee/migrations/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0      154 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/migrations/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0    18708 2023-06-05 04:18:47.000000 django-ipghrms-employee-1.6/employee/models.py
-drwxrwxrwx   0        0        0        0 2023-06-05 04:27:41.751879 django-ipghrms-employee-1.6/employee/reports/
--rw-rw-rw-   0        0        0        0 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/reports/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 04:27:41.860353 django-ipghrms-employee-1.6/employee/reports/__pycache__/
--rw-rw-rw-   0        0        0      145 2022-11-07 13:19:37.000000 django-ipghrms-employee-1.6/employee/reports/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      143 2022-10-20 01:02:26.000000 django-ipghrms-employee-1.6/employee/reports/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0      151 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/reports/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0      317 2022-11-07 13:19:37.000000 django-ipghrms-employee-1.6/employee/reports/__pycache__/urls.cpython-310.pyc
--rw-rw-rw-   0        0        0      313 2022-10-20 01:02:26.000000 django-ipghrms-employee-1.6/employee/reports/__pycache__/urls.cpython-37.pyc
--rw-rw-rw-   0        0        0      323 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/reports/__pycache__/urls.cpython-39.pyc
--rw-rw-rw-   0        0        0     1726 2022-11-07 13:19:37.000000 django-ipghrms-employee-1.6/employee/reports/__pycache__/views.cpython-310.pyc
--rw-rw-rw-   0        0        0     1722 2022-11-05 14:50:10.000000 django-ipghrms-employee-1.6/employee/reports/__pycache__/views.cpython-37.pyc
--rw-rw-rw-   0        0        0     1728 2022-11-04 05:28:45.000000 django-ipghrms-employee-1.6/employee/reports/__pycache__/views.cpython-39.pyc
--rw-rw-rw-   0        0        0      147 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/reports/urls.py
--rw-rw-rw-   0        0        0     1583 2022-11-04 05:28:45.000000 django-ipghrms-employee-1.6/employee/reports/views.py
--rw-rw-rw-   0        0        0     1110 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/signals.py
-drwxrwxrwx   0        0        0        0 2023-06-05 04:27:40.496060 django-ipghrms-employee-1.6/employee/templates/
-drwxrwxrwx   0        0        0        0 2023-06-05 04:27:41.910687 django-ipghrms-employee-1.6/employee/templates/components/
--rw-rw-rw-   0        0        0      877 2023-01-19 15:00:22.000000 django-ipghrms-employee-1.6/employee/templates/components/password_modal.html
--rw-rw-rw-   0        0        0      878 2023-01-19 13:55:13.000000 django-ipghrms-employee-1.6/employee/templates/components/password_modal_list.html
--rw-rw-rw-   0        0        0     1275 2023-01-19 15:06:29.000000 django-ipghrms-employee-1.6/employee/templates/components/password_validation.html
-drwxrwxrwx   0        0        0        0 2023-06-05 04:27:42.799616 django-ipghrms-employee-1.6/employee/templates/employee/
--rw-rw-rw-   0        0        0     8744 2023-03-16 00:18:59.000000 django-ipghrms-employee-1.6/employee/templates/employee/emp_attach.html
--rw-rw-rw-   0        0        0     5904 2023-03-13 01:47:47.000000 django-ipghrms-employee-1.6/employee/templates/employee/emp_contact_list.html
--rw-rw-rw-   0        0        0     4326 2023-03-13 01:46:45.000000 django-ipghrms-employee-1.6/employee/templates/employee/emp_dash.html
--rw-rw-rw-   0        0        0     2618 2023-03-31 05:55:07.000000 django-ipghrms-employee-1.6/employee/templates/employee/emp_detail.html
--rw-rw-rw-   0        0        0     2559 2022-12-12 12:14:17.000000 django-ipghrms-employee-1.6/employee/templates/employee/emp_detail_bottom.html
--rw-rw-rw-   0        0        0     6238 2023-03-15 13:54:44.000000 django-ipghrms-employee-1.6/employee/templates/employee/emp_detail_left.html
--rw-rw-rw-   0        0        0     2842 2023-02-20 12:31:39.000000 django-ipghrms-employee-1.6/employee/templates/employee/emp_detail_right.html
--rw-rw-rw-   0        0        0     8449 2023-03-08 09:58:00.000000 django-ipghrms-employee-1.6/employee/templates/employee/emp_list.html
--rw-rw-rw-   0        0        0     4874 2023-02-14 04:22:54.000000 django-ipghrms-employee-1.6/employee/templates/employee/emp_list_deact.html
--rw-rw-rw-   0        0        0     1944 2023-02-14 13:46:41.000000 django-ipghrms-employee-1.6/employee/templates/employee/emp_photo.html
--rw-rw-rw-   0        0        0     8438 2022-12-17 09:54:55.000000 django-ipghrms-employee-1.6/employee/templates/employee/emp_raw_data.html
--rw-rw-rw-   0        0        0     1126 2023-02-23 14:25:48.000000 django-ipghrms-employee-1.6/employee/templates/employee/form.html
--rw-rw-rw-   0        0        0     1186 2023-02-23 05:16:14.000000 django-ipghrms-employee-1.6/employee/templates/employee/form2.html
--rw-rw-rw-   0        0        0     6313 2022-11-30 15:30:41.000000 django-ipghrms-employee-1.6/employee/templates/employee/form3.html
--rw-rw-rw-   0        0        0     2983 2022-11-04 05:28:45.000000 django-ipghrms-employee-1.6/employee/templates/employee/form_address.html
--rw-rw-rw-   0        0        0     3024 2022-11-04 05:28:45.000000 django-ipghrms-employee-1.6/employee/templates/employee/form_location.html
--rw-rw-rw-   0        0        0     2911 2023-02-13 02:29:46.000000 django-ipghrms-employee-1.6/employee/templates/employee/maps.html
--rw-rw-rw-   0        0        0    10305 2023-03-16 00:20:50.000000 django-ipghrms-employee-1.6/employee/templates/employee/s_emp_attach.html
-drwxrwxrwx   0        0        0        0 2023-06-05 04:27:43.321594 django-ipghrms-employee-1.6/employee/templates/employee2/
--rw-rw-rw-   0        0        0     2490 2023-03-15 14:45:20.000000 django-ipghrms-employee-1.6/employee/templates/employee2/depend_list.html
--rw-rw-rw-   0        0        0     2062 2022-11-22 02:44:08.000000 django-ipghrms-employee-1.6/employee/templates/employee2/form.html
--rw-rw-rw-   0        0        0     2425 2022-11-22 01:53:05.000000 django-ipghrms-employee-1.6/employee/templates/employee2/formal_detail.html
--rw-rw-rw-   0        0        0     2965 2023-03-15 14:46:35.000000 django-ipghrms-employee-1.6/employee/templates/employee2/formal_list.html
--rw-rw-rw-   0        0        0     2286 2022-11-22 01:58:29.000000 django-ipghrms-employee-1.6/employee/templates/employee2/nonformal_detail.html
--rw-rw-rw-   0        0        0     2743 2023-03-15 14:47:54.000000 django-ipghrms-employee-1.6/employee/templates/employee2/nonformal_list.html
--rw-rw-rw-   0        0        0     4270 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/templates/employee2/photo.html
--rw-rw-rw-   0        0        0     1416 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/templates/employee2/photo_modal.html
--rw-rw-rw-   0        0        0     1997 2022-11-22 02:51:58.000000 django-ipghrms-employee-1.6/employee/templates/employee2/workexp_detail.html
--rw-rw-rw-   0        0        0     2821 2023-03-15 14:49:32.000000 django-ipghrms-employee-1.6/employee/templates/employee2/workexp_list.html
-drwxrwxrwx   0        0        0        0 2023-06-05 04:27:43.911625 django-ipghrms-employee-1.6/employee/templates/employee3/
--rw-rw-rw-   0        0        0     2066 2022-11-04 05:28:45.000000 django-ipghrms-employee-1.6/employee/templates/employee3/adv_list.html
--rw-rw-rw-   0        0        0     3633 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/templates/employee3/de_list.html
--rw-rw-rw-   0        0        0     2992 2022-12-13 00:56:08.000000 django-ipghrms-employee-1.6/employee/templates/employee3/dep_list.html
--rw-rw-rw-   0        0        0     1822 2023-02-07 02:52:12.000000 django-ipghrms-employee-1.6/employee/templates/employee3/no_div_list.html
--rw-rw-rw-   0        0        0     8458 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/templates/employee3/raw_data.html
--rw-rw-rw-   0        0        0     9718 2022-12-17 09:56:21.000000 django-ipghrms-employee-1.6/employee/templates/employee3/raw_data_adv.html
--rw-rw-rw-   0        0        0     9055 2022-12-17 09:56:20.000000 django-ipghrms-employee-1.6/employee/templates/employee3/raw_data_all.html
--rw-rw-rw-   0        0        0    11344 2023-02-07 02:42:52.000000 django-ipghrms-employee-1.6/employee/templates/employee3/raw_data_emp.html
--rw-rw-rw-   0        0        0     9039 2022-12-17 09:56:15.000000 django-ipghrms-employee-1.6/employee/templates/employee3/raw_data_habi.html
--rw-rw-rw-   0        0        0     4357 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/templates/employee3/staff_list.html
--rw-rw-rw-   0        0        0     3216 2023-01-25 02:36:21.000000 django-ipghrms-employee-1.6/employee/templates/employee3/unit_list.html
-drwxrwxrwx   0        0        0        0 2023-06-05 04:27:44.186425 django-ipghrms-employee-1.6/employee/templates/employee_chart/
--rw-rw-rw-   0        0        0     4736 2023-02-13 02:29:20.000000 django-ipghrms-employee-1.6/employee/templates/employee_chart/chart_emp.html
--rw-rw-rw-   0        0        0     4711 2023-02-13 01:08:00.000000 django-ipghrms-employee-1.6/employee/templates/employee_chart/chart_emp_dep.html
--rw-rw-rw-   0        0        0     4761 2023-02-13 01:24:23.000000 django-ipghrms-employee-1.6/employee/templates/employee_chart/chart_emp_unit.html
--rw-rw-rw-   0        0        0     1635 2023-02-13 02:43:14.000000 django-ipghrms-employee-1.6/employee/templates/employee_chart/emp_age.js
--rw-rw-rw-   0        0        0     1488 2023-02-13 02:43:19.000000 django-ipghrms-employee-1.6/employee/templates/employee_chart/emp_age2.js
--rw-rw-rw-   0        0        0     3931 2023-01-17 10:24:10.000000 django-ipghrms-employee-1.6/employee/templates/employee_chart/emp_all.js
--rw-rw-rw-   0        0        0     1281 2023-01-22 14:11:15.000000 django-ipghrms-employee-1.6/employee/templates/employee_chart/emp_country.js
--rw-rw-rw-   0        0        0     1884 2023-02-13 01:16:36.000000 django-ipghrms-employee-1.6/employee/templates/employee_chart/emp_dep.js
--rw-rw-rw-   0        0        0     2176 2023-02-13 01:21:07.000000 django-ipghrms-employee-1.6/employee/templates/employee_chart/emp_dep2.js
--rw-rw-rw-   0        0        0     1346 2023-01-22 09:44:27.000000 django-ipghrms-employee-1.6/employee/templates/employee_chart/emp_gender.js
--rw-rw-rw-   0        0        0      902 2023-02-10 02:06:54.000000 django-ipghrms-employee-1.6/employee/templates/employee_chart/emp_mun.js
--rw-rw-rw-   0        0        0     1275 2023-01-23 16:30:20.000000 django-ipghrms-employee-1.6/employee/templates/employee_chart/emp_nivelaca.js
--rw-rw-rw-   0        0        0     2110 2023-01-22 13:26:54.000000 django-ipghrms-employee-1.6/employee/templates/employee_chart/emp_nivelaca2.js
--rw-rw-rw-   0        0        0     1286 2023-01-17 14:41:16.000000 django-ipghrms-employee-1.6/employee/templates/employee_chart/emp_unit.js
--rw-rw-rw-   0        0        0     1217 2022-11-16 12:01:31.000000 django-ipghrms-employee-1.6/employee/templates/employee_chart/myoption.js
--rw-rw-rw-   0        0        0     2149 2022-11-16 12:18:31.000000 django-ipghrms-employee-1.6/employee/templates/employee_chart/udep_emp_gender.js
-drwxrwxrwx   0        0        0        0 2023-06-05 04:27:44.340870 django-ipghrms-employee-1.6/employee/templates/employee_detail/
--rw-rw-rw-   0        0        0     8896 2023-02-07 02:14:30.000000 django-ipghrms-employee-1.6/employee/templates/employee_detail/attendance.html
--rw-rw-rw-   0        0        0     4467 2023-03-17 07:17:38.000000 django-ipghrms-employee-1.6/employee/templates/employee_detail/basic.html
--rw-rw-rw-   0        0        0      226 2023-02-07 02:16:49.000000 django-ipghrms-employee-1.6/employee/templates/employee_detail/error.html
--rw-rw-rw-   0        0        0    17177 2023-02-07 02:20:55.000000 django-ipghrms-employee-1.6/employee/templates/employee_detail/evaluation.html
--rw-rw-rw-   0        0        0     1699 2023-02-14 09:34:06.000000 django-ipghrms-employee-1.6/employee/templates/employee_detail/header.html
--rw-rw-rw-   0        0        0    16526 2023-02-07 02:17:47.000000 django-ipghrms-employee-1.6/employee/templates/employee_detail/leave.html
--rw-rw-rw-   0        0        0     4840 2023-01-09 15:47:35.000000 django-ipghrms-employee-1.6/employee/templates/employee_detail/onboarding.html
--rw-rw-rw-   0        0        0     4920 2023-02-14 04:06:56.000000 django-ipghrms-employee-1.6/employee/templates/employee_detail/training.html
--rw-rw-rw-   0        0        0     4613 2023-02-07 02:15:08.000000 django-ipghrms-employee-1.6/employee/templates/employee_detail/trip.html
-drwxrwxrwx   0        0        0        0 2023-06-05 04:27:44.452995 django-ipghrms-employee-1.6/employee/templates/employee_print/
--rw-rw-rw-   0        0        0     3337 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/templates/employee_print/cv_1_iden.html
--rw-rw-rw-   0        0        0     1525 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/templates/employee_print/cv_2_nat_fam.html
--rw-rw-rw-   0        0        0     1536 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/templates/employee_print/cv_3_hab_acc.html
--rw-rw-rw-   0        0        0     3097 2022-11-16 15:17:31.000000 django-ipghrms-employee-1.6/employee/templates/employee_print/cv_4_col_fun.html
--rw-rw-rw-   0        0        0     2943 2022-11-16 15:17:22.000000 django-ipghrms-employee-1.6/employee/templates/employee_print/cv_4_col_fun_back.html
--rw-rw-rw-   0        0        0     1035 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/templates/employee_print/cv_5_per_fal.html
--rw-rw-rw-   0        0        0      930 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/templates/employee_print/cv_6_pen_lov.html
--rw-rw-rw-   0        0        0     1864 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/templates/employee_print/layout.html
--rw-rw-rw-   0        0        0     1163 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/templates/employee_print/print_cv.html
-drwxrwxrwx   0        0        0        0 2023-06-05 04:27:44.532234 django-ipghrms-employee-1.6/employee/templates/employee_reports/
--rw-rw-rw-   0        0        0     5669 2023-02-10 02:05:16.000000 django-ipghrms-employee-1.6/employee/templates/employee_reports/aca_level_list.html
--rw-rw-rw-   0        0        0      622 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/templates/employee_reports/r_dash.html
-drwxrwxrwx   0        0        0        0 2023-06-05 04:27:44.828364 django-ipghrms-employee-1.6/employee/templates/employee_users/
--rw-rw-rw-   0        0        0     3738 2023-02-13 00:54:29.000000 django-ipghrms-employee-1.6/employee/templates/employee_users/emp_dep_list.html
--rw-rw-rw-   0        0        0     2942 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/templates/employee_users/emp_detail.html
--rw-rw-rw-   0        0        0     2439 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/templates/employee_users/emp_detail_bottom.html
--rw-rw-rw-   0        0        0     2940 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/templates/employee_users/emp_detail_left.html
--rw-rw-rw-   0        0        0     2567 2022-11-16 15:17:34.000000 django-ipghrms-employee-1.6/employee/templates/employee_users/emp_detail_right.html
--rw-rw-rw-   0        0        0     4364 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/templates/employee_users/emp_staff_list.html
--rw-rw-rw-   0        0        0     3121 2023-02-21 06:02:09.000000 django-ipghrms-employee-1.6/employee/templates/employee_users/emp_unit_dash.html
--rw-rw-rw-   0        0        0       60 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/tests.py
--rw-rw-rw-   0        0        0     5809 2023-03-17 07:17:29.000000 django-ipghrms-employee-1.6/employee/urls.py
--rw-rw-rw-   0        0        0      139 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/urls_reports.py
--rw-rw-rw-   0        0        0     2568 2023-03-08 09:45:30.000000 django-ipghrms-employee-1.6/employee/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-05 04:27:44.971974 django-ipghrms-employee-1.6/employee/views/
--rw-rw-rw-   0        0        0      310 2022-11-16 06:23:14.000000 django-ipghrms-employee-1.6/employee/views/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 04:27:45.581388 django-ipghrms-employee-1.6/employee/views/__pycache__/
--rw-rw-rw-   0        0        0      379 2022-11-16 06:23:16.000000 django-ipghrms-employee-1.6/employee/views/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      329 2022-11-04 11:20:35.000000 django-ipghrms-employee-1.6/employee/views/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0      388 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/views/__pycache__/__init__.cpython-38.pyc
--rw-rw-rw-   0        0        0      363 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/views/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     2560 2022-12-14 12:34:34.000000 django-ipghrms-employee-1.6/employee/views/__pycache__/emp_rawdata.cpython-310.pyc
--rw-rw-rw-   0        0        0     2600 2022-11-06 05:43:59.000000 django-ipghrms-employee-1.6/employee/views/__pycache__/emp_rawdata.cpython-37.pyc
--rw-rw-rw-   0        0        0     2561 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/views/__pycache__/emp_rawdata.cpython-39.pyc
--rw-rw-rw-   0        0        0    11219 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/views/__pycache__/employee.cpython-37.pyc
--rw-rw-rw-   0        0        0    10162 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/views/__pycache__/employee.cpython-38.pyc
--rw-rw-rw-   0        0        0     9594 2023-03-17 07:44:47.000000 django-ipghrms-employee-1.6/employee/views/__pycache__/employee2.cpython-310.pyc
--rw-rw-rw-   0        0        0    11547 2022-11-05 14:50:10.000000 django-ipghrms-employee-1.6/employee/views/__pycache__/employee2.cpython-37.pyc
--rw-rw-rw-   0        0        0     9642 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/views/__pycache__/employee2.cpython-38.pyc
--rw-rw-rw-   0        0        0    10485 2022-11-04 05:28:45.000000 django-ipghrms-employee-1.6/employee/views/__pycache__/employee2.cpython-39.pyc
--rw-rw-rw-   0        0        0     3723 2023-01-25 02:35:37.000000 django-ipghrms-employee-1.6/employee/views/__pycache__/employee3.cpython-310.pyc
--rw-rw-rw-   0        0        0     3680 2022-11-07 09:09:48.000000 django-ipghrms-employee-1.6/employee/views/__pycache__/employee3.cpython-37.pyc
--rw-rw-rw-   0        0        0     8130 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/views/__pycache__/employee3.cpython-38.pyc
--rw-rw-rw-   0        0        0     3694 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/views/__pycache__/employee3.cpython-39.pyc
--rw-rw-rw-   0        0        0     3680 2023-02-14 14:08:28.000000 django-ipghrms-employee-1.6/employee/views/__pycache__/employee_attach.cpython-310.pyc
--rw-rw-rw-   0        0        0     2693 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/views/__pycache__/employee_attach.cpython-38.pyc
--rw-rw-rw-   0        0        0     5499 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/views/__pycache__/employee_carrier.cpython-38.pyc
--rw-rw-rw-   0        0        0     1115 2023-02-10 01:57:59.000000 django-ipghrms-employee-1.6/employee/views/__pycache__/employee_chart.cpython-310.pyc
--rw-rw-rw-   0        0        0      868 2022-10-20 01:02:26.000000 django-ipghrms-employee-1.6/employee/views/__pycache__/employee_chart.cpython-37.pyc
--rw-rw-rw-   0        0        0      755 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/views/__pycache__/employee_chart.cpython-38.pyc
--rw-rw-rw-   0        0        0      884 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/views/__pycache__/employee_chart.cpython-39.pyc
--rw-rw-rw-   0        0        0     1043 2023-03-08 09:34:10.000000 django-ipghrms-employee-1.6/employee/views/__pycache__/employee_dash.cpython-310.pyc
--rw-rw-rw-   0        0        0     1953 2022-10-20 01:02:07.000000 django-ipghrms-employee-1.6/employee/views/__pycache__/employee_dash.cpython-37.pyc
--rw-rw-rw-   0        0        0     2891 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/views/__pycache__/employee_dash.cpython-38.pyc
--rw-rw-rw-   0        0        0     1955 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/views/__pycache__/employee_dash.cpython-39.pyc
--rw-rw-rw-   0        0        0     4512 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/views/__pycache__/employee_de.cpython-39.pyc
--rw-rw-rw-   0        0        0     1362 2023-02-10 01:57:31.000000 django-ipghrms-employee-1.6/employee/views/__pycache__/employee_dep.cpython-310.pyc
--rw-rw-rw-   0        0        0     1354 2022-10-20 01:02:26.000000 django-ipghrms-employee-1.6/employee/views/__pycache__/employee_dep.cpython-37.pyc
--rw-rw-rw-   0        0        0     1370 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/views/__pycache__/employee_dep.cpython-39.pyc
--rw-rw-rw-   0        0        0     4567 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/views/__pycache__/employee_dg.cpython-38.pyc
--rw-rw-rw-   0        0        0     2763 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/views/__pycache__/employee_div.cpython-38.pyc
--rw-rw-rw-   0        0        0     9214 2023-03-17 07:39:53.000000 django-ipghrms-employee-1.6/employee/views/__pycache__/employee_m.cpython-310.pyc
--rw-rw-rw-   0        0        0     8446 2022-10-20 01:02:26.000000 django-ipghrms-employee-1.6/employee/views/__pycache__/employee_m.cpython-37.pyc
--rw-rw-rw-   0        0        0     7814 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/views/__pycache__/employee_m.cpython-39.pyc
--rw-rw-rw-   0        0        0     2783 2023-02-13 00:45:04.000000 django-ipghrms-employee-1.6/employee/views/__pycache__/employee_unit.cpython-310.pyc
--rw-rw-rw-   0        0        0     2771 2022-11-06 05:56:24.000000 django-ipghrms-employee-1.6/employee/views/__pycache__/employee_unit.cpython-37.pyc
--rw-rw-rw-   0        0        0     2823 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/views/__pycache__/employee_unit.cpython-39.pyc
--rw-rw-rw-   0        0        0     2307 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/views/__pycache__/employee_user.cpython-38.pyc
--rw-rw-rw-   0        0        0    15410 2023-03-15 13:47:43.000000 django-ipghrms-employee-1.6/employee/views/__pycache__/employee_v.cpython-310.pyc
--rw-rw-rw-   0        0        0     3007 2022-11-04 05:54:18.000000 django-ipghrms-employee-1.6/employee/views/__pycache__/employee_v.cpython-37.pyc
--rw-rw-rw-   0        0        0     3036 2022-11-04 05:28:45.000000 django-ipghrms-employee-1.6/employee/views/__pycache__/employee_v.cpython-39.pyc
--rw-rw-rw-   0        0        0     6379 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/views/__pycache__/id_card_print.cpython-38.pyc
--rw-rw-rw-   0        0        0     6219 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/views/__pycache__/print.cpython-38.pyc
--rw-rw-rw-   0        0        0     2708 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/views/__pycache__/print_cv.cpython-38.pyc
--rw-rw-rw-   0        0        0     1395 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/views/__pycache__/users.cpython-37.pyc
--rw-rw-rw-   0        0        0     1429 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/views/__pycache__/users.cpython-38.pyc
--rw-rw-rw-   0        0        0     2907 2022-12-14 12:34:30.000000 django-ipghrms-employee-1.6/employee/views/emp_rawdata.py
--rw-rw-rw-   0        0        0    14951 2023-03-17 07:43:05.000000 django-ipghrms-employee-1.6/employee/views/employee2.py
--rw-rw-rw-   0        0        0     4024 2023-01-25 02:35:35.000000 django-ipghrms-employee-1.6/employee/views/employee3.py
--rw-rw-rw-   0        0        0     4288 2023-02-14 14:08:26.000000 django-ipghrms-employee-1.6/employee/views/employee_attach.py
--rw-rw-rw-   0        0        0     1135 2023-02-10 01:57:57.000000 django-ipghrms-employee-1.6/employee/views/employee_chart.py
--rw-rw-rw-   0        0        0     2809 2023-03-08 09:34:07.000000 django-ipghrms-employee-1.6/employee/views/employee_dash.py
--rw-rw-rw-   0        0        0     1109 2023-02-10 01:57:18.000000 django-ipghrms-employee-1.6/employee/views/employee_dep.py
--rw-rw-rw-   0        0        0    12343 2023-03-24 07:01:56.000000 django-ipghrms-employee-1.6/employee/views/employee_m.py
--rw-rw-rw-   0        0        0     2840 2023-02-13 00:45:01.000000 django-ipghrms-employee-1.6/employee/views/employee_unit.py
--rw-rw-rw-   0        0        0     2696 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/views/employee_user.py
--rw-rw-rw-   0        0        0    21922 2023-04-11 09:19:16.000000 django-ipghrms-employee-1.6/employee/views/employee_v.py
--rw-rw-rw-   0        0        0       63 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.6/employee/views.py
--rw-rw-rw-   0        0        0      511 2023-06-05 04:27:45.623360 django-ipghrms-employee-1.6/setup.cfg
--rw-rw-rw-   0        0        0       39 2023-03-22 07:44:49.000000 django-ipghrms-employee-1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 13:20:36.250566 django-ipghrms-employee-1.8/
+-rw-rw-rw-   0        0        0     1068 2023-03-27 14:44:23.000000 django-ipghrms-employee-1.8/LICENSE
+-rw-rw-rw-   0        0        0      224 2023-03-27 14:44:31.000000 django-ipghrms-employee-1.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      951 2023-06-13 13:20:36.251565 django-ipghrms-employee-1.8/PKG-INFO
+-rw-rw-rw-   0        0        0      503 2023-03-27 14:20:21.000000 django-ipghrms-employee-1.8/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-13 13:20:32.669389 django-ipghrms-employee-1.8/django_ipghrms_employee.egg-info/
+-rw-rw-rw-   0        0        0      951 2023-06-13 13:20:32.000000 django-ipghrms-employee-1.8/django_ipghrms_employee.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    13169 2023-06-13 13:20:32.000000 django-ipghrms-employee-1.8/django_ipghrms_employee.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 13:20:32.000000 django-ipghrms-employee-1.8/django_ipghrms_employee.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-13 13:20:32.000000 django-ipghrms-employee-1.8/django_ipghrms_employee.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 13:20:32.760730 django-ipghrms-employee-1.8/employee/
+-rw-rw-rw-   0        0        0        0 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/__init__.py
+-rw-rw-rw-   0        0        0     1348 2023-06-05 04:17:59.000000 django-ipghrms-employee-1.8/employee/admin.py
+drwxrwxrwx   0        0        0        0 2023-06-13 13:20:32.776524 django-ipghrms-employee-1.8/employee/api/
+-rw-rw-rw-   0        0        0        0 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 13:20:32.857479 django-ipghrms-employee-1.8/employee/api/__pycache__/
+-rw-rw-rw-   0        0        0      141 2022-11-07 13:19:37.000000 django-ipghrms-employee-1.8/employee/api/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      139 2022-10-20 01:02:26.000000 django-ipghrms-employee-1.8/employee/api/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0      147 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/api/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0      718 2023-01-17 15:06:20.000000 django-ipghrms-employee-1.8/employee/api/__pycache__/urls.cpython-310.pyc
+-rw-rw-rw-   0        0        0      664 2022-10-20 01:02:26.000000 django-ipghrms-employee-1.8/employee/api/__pycache__/urls.cpython-37.pyc
+-rw-rw-rw-   0        0        0      674 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/api/__pycache__/urls.cpython-39.pyc
+-rw-rw-rw-   0        0        0     8468 2023-02-13 01:12:07.000000 django-ipghrms-employee-1.8/employee/api/__pycache__/views.cpython-310.pyc
+-rw-rw-rw-   0        0        0     7493 2022-10-20 01:02:26.000000 django-ipghrms-employee-1.8/employee/api/__pycache__/views.cpython-37.pyc
+-rw-rw-rw-   0        0        0     7168 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/api/__pycache__/views.cpython-39.pyc
+-rw-rw-rw-   0        0        0      647 2023-01-17 15:06:18.000000 django-ipghrms-employee-1.8/employee/api/urls.py
+-rw-rw-rw-   0        0        0    10312 2023-02-13 01:12:04.000000 django-ipghrms-employee-1.8/employee/api/views.py
+-rw-rw-rw-   0        0        0      132 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/apps.py
+-rw-rw-rw-   0        0        0      152 2023-03-13 01:01:19.000000 django-ipghrms-employee-1.8/employee/contact_urls.py
+-rw-rw-rw-   0        0        0      155 2023-03-08 09:34:17.000000 django-ipghrms-employee-1.8/employee/context_processors.py
+-rw-rw-rw-   0        0        0    19649 2023-03-15 10:22:24.000000 django-ipghrms-employee-1.8/employee/forms.py
+drwxrwxrwx   0        0        0        0 2023-06-13 13:20:33.042567 django-ipghrms-employee-1.8/employee/migrations/
+-rw-rw-rw-   0        0        0    20094 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0     1798 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/migrations/0002_curempposition_curempdivision.py
+-rw-rw-rw-   0        0        0      422 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/migrations/0003_employee_is_new.py
+-rw-rw-rw-   0        0        0      425 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/migrations/0004_employee_emp_id.py
+-rw-rw-rw-   0        0        0      824 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/migrations/0005_alter_employee_blood_alter_employee_father_and_more.py
+-rw-rw-rw-   0        0        0     1310 2022-11-04 05:28:45.000000 django-ipghrms-employee-1.8/employee/migrations/0006_fidnumber_bank_address_fidnumber_customer_name_and_more.py
+-rw-rw-rw-   0        0        0      488 2022-11-04 05:28:45.000000 django-ipghrms-employee-1.8/employee/migrations/0007_alter_fidnumber_customer_name.py
+-rw-rw-rw-   0        0        0      737 2022-11-04 05:28:45.000000 django-ipghrms-employee-1.8/employee/migrations/0008_empspecialize.py
+-rw-rw-rw-   0        0        0      438 2022-11-04 05:28:45.000000 django-ipghrms-employee-1.8/employee/migrations/0009_alter_empspecialize_name.py
+-rw-rw-rw-   0        0        0      557 2022-11-22 01:39:19.000000 django-ipghrms-employee-1.8/employee/migrations/0010_formaleducation_year.py
+-rw-rw-rw-   0        0        0      556 2022-11-22 01:56:32.000000 django-ipghrms-employee-1.8/employee/migrations/0011_nonformaleducation_year.py
+-rw-rw-rw-   0        0        0      851 2022-11-22 02:04:54.000000 django-ipghrms-employee-1.8/employee/migrations/0012_auto_20221122_1104.py
+-rw-rw-rw-   0        0        0     1680 2022-11-22 02:27:59.000000 django-ipghrms-employee-1.8/employee/migrations/0013_auto_20221122_1127.py
+-rw-rw-rw-   0        0        0     2814 2022-11-30 14:03:29.000000 django-ipghrms-employee-1.8/employee/migrations/0014_auto_20221130_2303.py
+-rw-rw-rw-   0        0        0     1093 2022-11-30 14:04:07.000000 django-ipghrms-employee-1.8/employee/migrations/0015_auto_20221130_2304.py
+-rw-rw-rw-   0        0        0     1177 2022-11-30 14:26:44.000000 django-ipghrms-employee-1.8/employee/migrations/0016_auto_20221130_2326.py
+-rw-rw-rw-   0        0        0      916 2022-11-30 14:35:38.000000 django-ipghrms-employee-1.8/employee/migrations/0017_auto_20221130_2335.py
+-rw-rw-rw-   0        0        0      411 2022-12-08 01:21:23.000000 django-ipghrms-employee-1.8/employee/migrations/0018_employee_pin.py
+-rw-rw-rw-   0        0        0      405 2022-12-14 12:14:22.000000 django-ipghrms-employee-1.8/employee/migrations/0019_employee_ext.py
+-rw-rw-rw-   0        0        0      801 2023-01-17 09:29:03.000000 django-ipghrms-employee-1.8/employee/migrations/0020_auto_20230117_1829.py
+-rw-rw-rw-   0        0        0      663 2023-01-19 10:28:44.000000 django-ipghrms-employee-1.8/employee/migrations/0021_emplanguage_file_language.py
+-rw-rw-rw-   0        0        0      710 2023-02-14 13:39:17.000000 django-ipghrms-employee-1.8/employee/migrations/0022_alter_photo_image.py
+-rw-rw-rw-   0        0        0      650 2023-02-14 14:31:40.000000 django-ipghrms-employee-1.8/employee/migrations/0023_alter_photo_image.py
+-rw-rw-rw-   0        0        0      407 2023-02-23 05:09:35.000000 django-ipghrms-employee-1.8/employee/migrations/0024_alter_fidnumber_options.py
+-rw-rw-rw-   0        0        0      982 2023-03-15 09:56:18.000000 django-ipghrms-employee-1.8/employee/migrations/0025_empsignature.py
+-rw-rw-rw-   0        0        0        0 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 13:20:33.441125 django-ipghrms-employee-1.8/employee/migrations/__pycache__/
+-rw-rw-rw-   0        0        0     7287 2022-11-07 13:19:39.000000 django-ipghrms-employee-1.8/employee/migrations/__pycache__/0001_initial.cpython-310.pyc
+-rw-rw-rw-   0        0        0     7215 2022-10-20 01:03:56.000000 django-ipghrms-employee-1.8/employee/migrations/__pycache__/0001_initial.cpython-37.pyc
+-rw-rw-rw-   0        0        0     7291 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/migrations/__pycache__/0001_initial.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1280 2022-11-07 13:19:39.000000 django-ipghrms-employee-1.8/employee/migrations/__pycache__/0002_curempposition_curempdivision.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1260 2022-10-20 01:03:56.000000 django-ipghrms-employee-1.8/employee/migrations/__pycache__/0002_curempposition_curempdivision.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1284 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/migrations/__pycache__/0002_curempposition_curempdivision.cpython-39.pyc
+-rw-rw-rw-   0        0        0      607 2022-11-07 13:19:39.000000 django-ipghrms-employee-1.8/employee/migrations/__pycache__/0003_employee_is_new.cpython-310.pyc
+-rw-rw-rw-   0        0        0      593 2022-10-20 01:03:56.000000 django-ipghrms-employee-1.8/employee/migrations/__pycache__/0003_employee_is_new.cpython-37.pyc
+-rw-rw-rw-   0        0        0      611 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/migrations/__pycache__/0003_employee_is_new.cpython-39.pyc
+-rw-rw-rw-   0        0        0      618 2022-11-07 13:19:39.000000 django-ipghrms-employee-1.8/employee/migrations/__pycache__/0004_employee_emp_id.cpython-310.pyc
+-rw-rw-rw-   0        0        0      604 2022-10-20 01:03:56.000000 django-ipghrms-employee-1.8/employee/migrations/__pycache__/0004_employee_emp_id.cpython-37.pyc
+-rw-rw-rw-   0        0        0      622 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/migrations/__pycache__/0004_employee_emp_id.cpython-39.pyc
+-rw-rw-rw-   0        0        0      802 2022-11-07 13:19:39.000000 django-ipghrms-employee-1.8/employee/migrations/__pycache__/0005_alter_employee_blood_alter_employee_father_and_more.cpython-310.pyc
+-rw-rw-rw-   0        0        0      786 2022-10-20 01:03:56.000000 django-ipghrms-employee-1.8/employee/migrations/__pycache__/0005_alter_employee_blood_alter_employee_father_and_more.cpython-37.pyc
+-rw-rw-rw-   0        0        0      806 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/migrations/__pycache__/0005_alter_employee_blood_alter_employee_father_and_more.cpython-39.pyc
+-rw-rw-rw-   0        0        0      973 2022-11-07 13:19:39.000000 django-ipghrms-employee-1.8/employee/migrations/__pycache__/0006_fidnumber_bank_address_fidnumber_customer_name_and_more.cpython-310.pyc
+-rw-rw-rw-   0        0        0      951 2022-11-05 14:52:09.000000 django-ipghrms-employee-1.8/employee/migrations/__pycache__/0006_fidnumber_bank_address_fidnumber_customer_name_and_more.cpython-37.pyc
+-rw-rw-rw-   0        0        0      699 2022-11-07 13:19:39.000000 django-ipghrms-employee-1.8/employee/migrations/__pycache__/0007_alter_fidnumber_customer_name.cpython-310.pyc
+-rw-rw-rw-   0        0        0      685 2022-11-05 14:52:09.000000 django-ipghrms-employee-1.8/employee/migrations/__pycache__/0007_alter_fidnumber_customer_name.cpython-37.pyc
+-rw-rw-rw-   0        0        0      894 2022-11-07 13:19:39.000000 django-ipghrms-employee-1.8/employee/migrations/__pycache__/0008_empspecialize.cpython-310.pyc
+-rw-rw-rw-   0        0        0      878 2022-11-05 14:52:09.000000 django-ipghrms-employee-1.8/employee/migrations/__pycache__/0008_empspecialize.cpython-37.pyc
+-rw-rw-rw-   0        0        0      643 2022-11-07 13:19:39.000000 django-ipghrms-employee-1.8/employee/migrations/__pycache__/0009_alter_empspecialize_name.cpython-310.pyc
+-rw-rw-rw-   0        0        0      629 2022-11-05 14:52:09.000000 django-ipghrms-employee-1.8/employee/migrations/__pycache__/0009_alter_empspecialize_name.cpython-37.pyc
+-rw-rw-rw-   0        0        0      739 2022-11-22 01:39:26.000000 django-ipghrms-employee-1.8/employee/migrations/__pycache__/0010_formaleducation_year.cpython-310.pyc
+-rw-rw-rw-   0        0        0      741 2022-11-22 01:56:39.000000 django-ipghrms-employee-1.8/employee/migrations/__pycache__/0011_nonformaleducation_year.cpython-310.pyc
+-rw-rw-rw-   0        0        0      815 2022-11-22 02:04:58.000000 django-ipghrms-employee-1.8/employee/migrations/__pycache__/0012_auto_20221122_1104.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1198 2022-11-22 02:28:05.000000 django-ipghrms-employee-1.8/employee/migrations/__pycache__/0013_auto_20221122_1127.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1353 2022-11-30 14:04:06.000000 django-ipghrms-employee-1.8/employee/migrations/__pycache__/0014_auto_20221130_2303.cpython-310.pyc
+-rw-rw-rw-   0        0        0      835 2022-11-30 14:04:17.000000 django-ipghrms-employee-1.8/employee/migrations/__pycache__/0015_auto_20221130_2304.cpython-310.pyc
+-rw-rw-rw-   0        0        0      903 2022-11-30 14:26:49.000000 django-ipghrms-employee-1.8/employee/migrations/__pycache__/0016_auto_20221130_2326.cpython-310.pyc
+-rw-rw-rw-   0        0        0      876 2022-11-30 14:35:49.000000 django-ipghrms-employee-1.8/employee/migrations/__pycache__/0017_auto_20221130_2335.cpython-310.pyc
+-rw-rw-rw-   0        0        0      576 2022-12-08 01:21:27.000000 django-ipghrms-employee-1.8/employee/migrations/__pycache__/0018_employee_pin.cpython-310.pyc
+-rw-rw-rw-   0        0        0      570 2022-12-14 12:14:28.000000 django-ipghrms-employee-1.8/employee/migrations/__pycache__/0019_employee_ext.cpython-310.pyc
+-rw-rw-rw-   0        0        0      908 2023-01-17 09:25:30.000000 django-ipghrms-employee-1.8/employee/migrations/__pycache__/0020_auto_20230117_1825.cpython-310.pyc
+-rw-rw-rw-   0        0        0      908 2023-01-17 09:27:40.000000 django-ipghrms-employee-1.8/employee/migrations/__pycache__/0020_auto_20230117_1827.cpython-310.pyc
+-rw-rw-rw-   0        0        0      908 2023-01-17 09:29:07.000000 django-ipghrms-employee-1.8/employee/migrations/__pycache__/0020_auto_20230117_1829.cpython-310.pyc
+-rw-rw-rw-   0        0        0      884 2023-01-19 10:28:51.000000 django-ipghrms-employee-1.8/employee/migrations/__pycache__/0021_emplanguage_file_language.cpython-310.pyc
+-rw-rw-rw-   0        0        0      911 2023-02-14 13:39:22.000000 django-ipghrms-employee-1.8/employee/migrations/__pycache__/0022_alter_photo_image.cpython-310.pyc
+-rw-rw-rw-   0        0        0      863 2023-02-14 14:31:44.000000 django-ipghrms-employee-1.8/employee/migrations/__pycache__/0023_alter_photo_image.cpython-310.pyc
+-rw-rw-rw-   0        0        0      586 2023-02-23 05:09:41.000000 django-ipghrms-employee-1.8/employee/migrations/__pycache__/0024_alter_fidnumber_options.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1136 2023-03-15 09:56:33.000000 django-ipghrms-employee-1.8/employee/migrations/__pycache__/0025_empsignature.cpython-310.pyc
+-rw-rw-rw-   0        0        0      148 2022-11-07 13:19:39.000000 django-ipghrms-employee-1.8/employee/migrations/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      146 2022-10-20 01:03:56.000000 django-ipghrms-employee-1.8/employee/migrations/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0      154 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/migrations/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0    18708 2023-06-05 04:18:47.000000 django-ipghrms-employee-1.8/employee/models.py
+drwxrwxrwx   0        0        0        0 2023-06-13 13:20:33.451854 django-ipghrms-employee-1.8/employee/reports/
+-rw-rw-rw-   0        0        0        0 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/reports/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 13:20:33.530392 django-ipghrms-employee-1.8/employee/reports/__pycache__/
+-rw-rw-rw-   0        0        0      145 2022-11-07 13:19:37.000000 django-ipghrms-employee-1.8/employee/reports/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      143 2022-10-20 01:02:26.000000 django-ipghrms-employee-1.8/employee/reports/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0      151 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/reports/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0      317 2022-11-07 13:19:37.000000 django-ipghrms-employee-1.8/employee/reports/__pycache__/urls.cpython-310.pyc
+-rw-rw-rw-   0        0        0      313 2022-10-20 01:02:26.000000 django-ipghrms-employee-1.8/employee/reports/__pycache__/urls.cpython-37.pyc
+-rw-rw-rw-   0        0        0      323 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/reports/__pycache__/urls.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1726 2022-11-07 13:19:37.000000 django-ipghrms-employee-1.8/employee/reports/__pycache__/views.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1722 2022-11-05 14:50:10.000000 django-ipghrms-employee-1.8/employee/reports/__pycache__/views.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1728 2022-11-04 05:28:45.000000 django-ipghrms-employee-1.8/employee/reports/__pycache__/views.cpython-39.pyc
+-rw-rw-rw-   0        0        0      147 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/reports/urls.py
+-rw-rw-rw-   0        0        0     1583 2022-11-04 05:28:45.000000 django-ipghrms-employee-1.8/employee/reports/views.py
+-rw-rw-rw-   0        0        0     1110 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/signals.py
+drwxrwxrwx   0        0        0        0 2023-06-13 13:20:32.581577 django-ipghrms-employee-1.8/employee/templates/
+drwxrwxrwx   0        0        0        0 2023-06-13 13:20:33.567542 django-ipghrms-employee-1.8/employee/templates/components/
+-rw-rw-rw-   0        0        0      877 2023-01-19 15:00:22.000000 django-ipghrms-employee-1.8/employee/templates/components/password_modal.html
+-rw-rw-rw-   0        0        0      878 2023-01-19 13:55:13.000000 django-ipghrms-employee-1.8/employee/templates/components/password_modal_list.html
+-rw-rw-rw-   0        0        0     1275 2023-01-19 15:06:29.000000 django-ipghrms-employee-1.8/employee/templates/components/password_validation.html
+drwxrwxrwx   0        0        0        0 2023-06-13 13:20:34.117328 django-ipghrms-employee-1.8/employee/templates/employee/
+-rw-rw-rw-   0        0        0     8744 2023-03-16 00:18:59.000000 django-ipghrms-employee-1.8/employee/templates/employee/emp_attach.html
+-rw-rw-rw-   0        0        0     5904 2023-03-13 01:47:47.000000 django-ipghrms-employee-1.8/employee/templates/employee/emp_contact_list.html
+-rw-rw-rw-   0        0        0     4326 2023-03-13 01:46:45.000000 django-ipghrms-employee-1.8/employee/templates/employee/emp_dash.html
+-rw-rw-rw-   0        0        0     2618 2023-03-31 05:55:07.000000 django-ipghrms-employee-1.8/employee/templates/employee/emp_detail.html
+-rw-rw-rw-   0        0        0     2559 2022-12-12 12:14:17.000000 django-ipghrms-employee-1.8/employee/templates/employee/emp_detail_bottom.html
+-rw-rw-rw-   0        0        0     6238 2023-03-15 13:54:44.000000 django-ipghrms-employee-1.8/employee/templates/employee/emp_detail_left.html
+-rw-rw-rw-   0        0        0     2842 2023-02-20 12:31:39.000000 django-ipghrms-employee-1.8/employee/templates/employee/emp_detail_right.html
+-rw-rw-rw-   0        0        0     8449 2023-03-08 09:58:00.000000 django-ipghrms-employee-1.8/employee/templates/employee/emp_list.html
+-rw-rw-rw-   0        0        0     4874 2023-02-14 04:22:54.000000 django-ipghrms-employee-1.8/employee/templates/employee/emp_list_deact.html
+-rw-rw-rw-   0        0        0     1944 2023-02-14 13:46:41.000000 django-ipghrms-employee-1.8/employee/templates/employee/emp_photo.html
+-rw-rw-rw-   0        0        0     8438 2022-12-17 09:54:55.000000 django-ipghrms-employee-1.8/employee/templates/employee/emp_raw_data.html
+-rw-rw-rw-   0        0        0     1126 2023-02-23 14:25:48.000000 django-ipghrms-employee-1.8/employee/templates/employee/form.html
+-rw-rw-rw-   0        0        0     1186 2023-02-23 05:16:14.000000 django-ipghrms-employee-1.8/employee/templates/employee/form2.html
+-rw-rw-rw-   0        0        0     6313 2022-11-30 15:30:41.000000 django-ipghrms-employee-1.8/employee/templates/employee/form3.html
+-rw-rw-rw-   0        0        0     2983 2022-11-04 05:28:45.000000 django-ipghrms-employee-1.8/employee/templates/employee/form_address.html
+-rw-rw-rw-   0        0        0     3024 2022-11-04 05:28:45.000000 django-ipghrms-employee-1.8/employee/templates/employee/form_location.html
+-rw-rw-rw-   0        0        0     2911 2023-02-13 02:29:46.000000 django-ipghrms-employee-1.8/employee/templates/employee/maps.html
+-rw-rw-rw-   0        0        0    10305 2023-03-16 00:20:50.000000 django-ipghrms-employee-1.8/employee/templates/employee/s_emp_attach.html
+drwxrwxrwx   0        0        0        0 2023-06-13 13:20:34.515082 django-ipghrms-employee-1.8/employee/templates/employee2/
+-rw-rw-rw-   0        0        0     2490 2023-03-15 14:45:20.000000 django-ipghrms-employee-1.8/employee/templates/employee2/depend_list.html
+-rw-rw-rw-   0        0        0     2062 2022-11-22 02:44:08.000000 django-ipghrms-employee-1.8/employee/templates/employee2/form.html
+-rw-rw-rw-   0        0        0     2425 2022-11-22 01:53:05.000000 django-ipghrms-employee-1.8/employee/templates/employee2/formal_detail.html
+-rw-rw-rw-   0        0        0     2965 2023-03-15 14:46:35.000000 django-ipghrms-employee-1.8/employee/templates/employee2/formal_list.html
+-rw-rw-rw-   0        0        0     2286 2022-11-22 01:58:29.000000 django-ipghrms-employee-1.8/employee/templates/employee2/nonformal_detail.html
+-rw-rw-rw-   0        0        0     2743 2023-03-15 14:47:54.000000 django-ipghrms-employee-1.8/employee/templates/employee2/nonformal_list.html
+-rw-rw-rw-   0        0        0     4270 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/templates/employee2/photo.html
+-rw-rw-rw-   0        0        0     1416 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/templates/employee2/photo_modal.html
+-rw-rw-rw-   0        0        0     1997 2022-11-22 02:51:58.000000 django-ipghrms-employee-1.8/employee/templates/employee2/workexp_detail.html
+-rw-rw-rw-   0        0        0     2821 2023-03-15 14:49:32.000000 django-ipghrms-employee-1.8/employee/templates/employee2/workexp_list.html
+drwxrwxrwx   0        0        0        0 2023-06-13 13:20:34.991850 django-ipghrms-employee-1.8/employee/templates/employee3/
+-rw-rw-rw-   0        0        0     2066 2022-11-04 05:28:45.000000 django-ipghrms-employee-1.8/employee/templates/employee3/adv_list.html
+-rw-rw-rw-   0        0        0     3633 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/templates/employee3/de_list.html
+-rw-rw-rw-   0        0        0     2992 2022-12-13 00:56:08.000000 django-ipghrms-employee-1.8/employee/templates/employee3/dep_list.html
+-rw-rw-rw-   0        0        0     1822 2023-02-07 02:52:12.000000 django-ipghrms-employee-1.8/employee/templates/employee3/no_div_list.html
+-rw-rw-rw-   0        0        0     8458 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/templates/employee3/raw_data.html
+-rw-rw-rw-   0        0        0     9718 2022-12-17 09:56:21.000000 django-ipghrms-employee-1.8/employee/templates/employee3/raw_data_adv.html
+-rw-rw-rw-   0        0        0     9055 2022-12-17 09:56:20.000000 django-ipghrms-employee-1.8/employee/templates/employee3/raw_data_all.html
+-rw-rw-rw-   0        0        0    11344 2023-02-07 02:42:52.000000 django-ipghrms-employee-1.8/employee/templates/employee3/raw_data_emp.html
+-rw-rw-rw-   0        0        0     9039 2022-12-17 09:56:15.000000 django-ipghrms-employee-1.8/employee/templates/employee3/raw_data_habi.html
+-rw-rw-rw-   0        0        0     4357 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/templates/employee3/staff_list.html
+-rw-rw-rw-   0        0        0     3216 2023-01-25 02:36:21.000000 django-ipghrms-employee-1.8/employee/templates/employee3/unit_list.html
+drwxrwxrwx   0        0        0        0 2023-06-13 13:20:35.222519 django-ipghrms-employee-1.8/employee/templates/employee_chart/
+-rw-rw-rw-   0        0        0     4736 2023-02-13 02:29:20.000000 django-ipghrms-employee-1.8/employee/templates/employee_chart/chart_emp.html
+-rw-rw-rw-   0        0        0     4711 2023-02-13 01:08:00.000000 django-ipghrms-employee-1.8/employee/templates/employee_chart/chart_emp_dep.html
+-rw-rw-rw-   0        0        0     4761 2023-02-13 01:24:23.000000 django-ipghrms-employee-1.8/employee/templates/employee_chart/chart_emp_unit.html
+-rw-rw-rw-   0        0        0     1635 2023-02-13 02:43:14.000000 django-ipghrms-employee-1.8/employee/templates/employee_chart/emp_age.js
+-rw-rw-rw-   0        0        0     1488 2023-02-13 02:43:19.000000 django-ipghrms-employee-1.8/employee/templates/employee_chart/emp_age2.js
+-rw-rw-rw-   0        0        0     3931 2023-01-17 10:24:10.000000 django-ipghrms-employee-1.8/employee/templates/employee_chart/emp_all.js
+-rw-rw-rw-   0        0        0     1281 2023-01-22 14:11:15.000000 django-ipghrms-employee-1.8/employee/templates/employee_chart/emp_country.js
+-rw-rw-rw-   0        0        0     1315 2023-06-11 13:25:00.000000 django-ipghrms-employee-1.8/employee/templates/employee_chart/emp_dep.js
+-rw-rw-rw-   0        0        0     2176 2023-02-13 01:21:07.000000 django-ipghrms-employee-1.8/employee/templates/employee_chart/emp_dep2.js
+-rw-rw-rw-   0        0        0     1346 2023-01-22 09:44:27.000000 django-ipghrms-employee-1.8/employee/templates/employee_chart/emp_gender.js
+-rw-rw-rw-   0        0        0      902 2023-02-10 02:06:54.000000 django-ipghrms-employee-1.8/employee/templates/employee_chart/emp_mun.js
+-rw-rw-rw-   0        0        0     1275 2023-01-23 16:30:20.000000 django-ipghrms-employee-1.8/employee/templates/employee_chart/emp_nivelaca.js
+-rw-rw-rw-   0        0        0     2110 2023-01-22 13:26:54.000000 django-ipghrms-employee-1.8/employee/templates/employee_chart/emp_nivelaca2.js
+-rw-rw-rw-   0        0        0     1286 2023-01-17 14:41:16.000000 django-ipghrms-employee-1.8/employee/templates/employee_chart/emp_unit.js
+-rw-rw-rw-   0        0        0     1217 2022-11-16 12:01:31.000000 django-ipghrms-employee-1.8/employee/templates/employee_chart/myoption.js
+-rw-rw-rw-   0        0        0     2149 2022-11-16 12:18:31.000000 django-ipghrms-employee-1.8/employee/templates/employee_chart/udep_emp_gender.js
+drwxrwxrwx   0        0        0        0 2023-06-13 13:20:35.346922 django-ipghrms-employee-1.8/employee/templates/employee_detail/
+-rw-rw-rw-   0        0        0     8896 2023-02-07 02:14:30.000000 django-ipghrms-employee-1.8/employee/templates/employee_detail/attendance.html
+-rw-rw-rw-   0        0        0     4467 2023-03-17 07:17:38.000000 django-ipghrms-employee-1.8/employee/templates/employee_detail/basic.html
+-rw-rw-rw-   0        0        0      226 2023-02-07 02:16:49.000000 django-ipghrms-employee-1.8/employee/templates/employee_detail/error.html
+-rw-rw-rw-   0        0        0    17177 2023-02-07 02:20:55.000000 django-ipghrms-employee-1.8/employee/templates/employee_detail/evaluation.html
+-rw-rw-rw-   0        0        0     1699 2023-02-14 09:34:06.000000 django-ipghrms-employee-1.8/employee/templates/employee_detail/header.html
+-rw-rw-rw-   0        0        0    16526 2023-02-07 02:17:47.000000 django-ipghrms-employee-1.8/employee/templates/employee_detail/leave.html
+-rw-rw-rw-   0        0        0     4840 2023-01-09 15:47:35.000000 django-ipghrms-employee-1.8/employee/templates/employee_detail/onboarding.html
+-rw-rw-rw-   0        0        0     4920 2023-02-14 04:06:56.000000 django-ipghrms-employee-1.8/employee/templates/employee_detail/training.html
+-rw-rw-rw-   0        0        0     4613 2023-02-07 02:15:08.000000 django-ipghrms-employee-1.8/employee/templates/employee_detail/trip.html
+drwxrwxrwx   0        0        0        0 2023-06-13 13:20:35.453986 django-ipghrms-employee-1.8/employee/templates/employee_print/
+-rw-rw-rw-   0        0        0     3337 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/templates/employee_print/cv_1_iden.html
+-rw-rw-rw-   0        0        0     1525 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/templates/employee_print/cv_2_nat_fam.html
+-rw-rw-rw-   0        0        0     1536 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/templates/employee_print/cv_3_hab_acc.html
+-rw-rw-rw-   0        0        0     3097 2022-11-16 15:17:31.000000 django-ipghrms-employee-1.8/employee/templates/employee_print/cv_4_col_fun.html
+-rw-rw-rw-   0        0        0     2943 2022-11-16 15:17:22.000000 django-ipghrms-employee-1.8/employee/templates/employee_print/cv_4_col_fun_back.html
+-rw-rw-rw-   0        0        0     1035 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/templates/employee_print/cv_5_per_fal.html
+-rw-rw-rw-   0        0        0      930 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/templates/employee_print/cv_6_pen_lov.html
+-rw-rw-rw-   0        0        0     1864 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/templates/employee_print/layout.html
+-rw-rw-rw-   0        0        0     1163 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/templates/employee_print/print_cv.html
+drwxrwxrwx   0        0        0        0 2023-06-13 13:20:35.511125 django-ipghrms-employee-1.8/employee/templates/employee_reports/
+-rw-rw-rw-   0        0        0     5669 2023-02-10 02:05:16.000000 django-ipghrms-employee-1.8/employee/templates/employee_reports/aca_level_list.html
+-rw-rw-rw-   0        0        0      622 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/templates/employee_reports/r_dash.html
+drwxrwxrwx   0        0        0        0 2023-06-13 13:20:35.658033 django-ipghrms-employee-1.8/employee/templates/employee_users/
+-rw-rw-rw-   0        0        0     3738 2023-02-13 00:54:29.000000 django-ipghrms-employee-1.8/employee/templates/employee_users/emp_dep_list.html
+-rw-rw-rw-   0        0        0     2942 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/templates/employee_users/emp_detail.html
+-rw-rw-rw-   0        0        0     2439 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/templates/employee_users/emp_detail_bottom.html
+-rw-rw-rw-   0        0        0     2940 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/templates/employee_users/emp_detail_left.html
+-rw-rw-rw-   0        0        0     2567 2022-11-16 15:17:34.000000 django-ipghrms-employee-1.8/employee/templates/employee_users/emp_detail_right.html
+-rw-rw-rw-   0        0        0     4364 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/templates/employee_users/emp_staff_list.html
+-rw-rw-rw-   0        0        0     3121 2023-02-21 06:02:09.000000 django-ipghrms-employee-1.8/employee/templates/employee_users/emp_unit_dash.html
+-rw-rw-rw-   0        0        0       60 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/tests.py
+-rw-rw-rw-   0        0        0     5809 2023-03-17 07:17:29.000000 django-ipghrms-employee-1.8/employee/urls.py
+-rw-rw-rw-   0        0        0      139 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/urls_reports.py
+-rw-rw-rw-   0        0        0     2568 2023-03-08 09:45:30.000000 django-ipghrms-employee-1.8/employee/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-13 13:20:35.754908 django-ipghrms-employee-1.8/employee/views/
+-rw-rw-rw-   0        0        0      310 2022-11-16 06:23:14.000000 django-ipghrms-employee-1.8/employee/views/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 13:20:36.244897 django-ipghrms-employee-1.8/employee/views/__pycache__/
+-rw-rw-rw-   0        0        0      379 2022-11-16 06:23:16.000000 django-ipghrms-employee-1.8/employee/views/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      329 2022-11-04 11:20:35.000000 django-ipghrms-employee-1.8/employee/views/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0      388 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/views/__pycache__/__init__.cpython-38.pyc
+-rw-rw-rw-   0        0        0      363 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/views/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2560 2022-12-14 12:34:34.000000 django-ipghrms-employee-1.8/employee/views/__pycache__/emp_rawdata.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2600 2022-11-06 05:43:59.000000 django-ipghrms-employee-1.8/employee/views/__pycache__/emp_rawdata.cpython-37.pyc
+-rw-rw-rw-   0        0        0     2561 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/views/__pycache__/emp_rawdata.cpython-39.pyc
+-rw-rw-rw-   0        0        0    11219 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/views/__pycache__/employee.cpython-37.pyc
+-rw-rw-rw-   0        0        0    10162 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/views/__pycache__/employee.cpython-38.pyc
+-rw-rw-rw-   0        0        0     9594 2023-03-17 07:44:47.000000 django-ipghrms-employee-1.8/employee/views/__pycache__/employee2.cpython-310.pyc
+-rw-rw-rw-   0        0        0    11547 2022-11-05 14:50:10.000000 django-ipghrms-employee-1.8/employee/views/__pycache__/employee2.cpython-37.pyc
+-rw-rw-rw-   0        0        0     9642 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/views/__pycache__/employee2.cpython-38.pyc
+-rw-rw-rw-   0        0        0    10485 2022-11-04 05:28:45.000000 django-ipghrms-employee-1.8/employee/views/__pycache__/employee2.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3723 2023-01-25 02:35:37.000000 django-ipghrms-employee-1.8/employee/views/__pycache__/employee3.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3680 2022-11-07 09:09:48.000000 django-ipghrms-employee-1.8/employee/views/__pycache__/employee3.cpython-37.pyc
+-rw-rw-rw-   0        0        0     8130 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/views/__pycache__/employee3.cpython-38.pyc
+-rw-rw-rw-   0        0        0     3694 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/views/__pycache__/employee3.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3680 2023-02-14 14:08:28.000000 django-ipghrms-employee-1.8/employee/views/__pycache__/employee_attach.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2693 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/views/__pycache__/employee_attach.cpython-38.pyc
+-rw-rw-rw-   0        0        0     5499 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/views/__pycache__/employee_carrier.cpython-38.pyc
+-rw-rw-rw-   0        0        0     1115 2023-02-10 01:57:59.000000 django-ipghrms-employee-1.8/employee/views/__pycache__/employee_chart.cpython-310.pyc
+-rw-rw-rw-   0        0        0      868 2022-10-20 01:02:26.000000 django-ipghrms-employee-1.8/employee/views/__pycache__/employee_chart.cpython-37.pyc
+-rw-rw-rw-   0        0        0      755 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/views/__pycache__/employee_chart.cpython-38.pyc
+-rw-rw-rw-   0        0        0      884 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/views/__pycache__/employee_chart.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1043 2023-03-08 09:34:10.000000 django-ipghrms-employee-1.8/employee/views/__pycache__/employee_dash.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1953 2022-10-20 01:02:07.000000 django-ipghrms-employee-1.8/employee/views/__pycache__/employee_dash.cpython-37.pyc
+-rw-rw-rw-   0        0        0     2891 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/views/__pycache__/employee_dash.cpython-38.pyc
+-rw-rw-rw-   0        0        0     1955 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/views/__pycache__/employee_dash.cpython-39.pyc
+-rw-rw-rw-   0        0        0     4512 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/views/__pycache__/employee_de.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1362 2023-02-10 01:57:31.000000 django-ipghrms-employee-1.8/employee/views/__pycache__/employee_dep.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1354 2022-10-20 01:02:26.000000 django-ipghrms-employee-1.8/employee/views/__pycache__/employee_dep.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1370 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/views/__pycache__/employee_dep.cpython-39.pyc
+-rw-rw-rw-   0        0        0     4567 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/views/__pycache__/employee_dg.cpython-38.pyc
+-rw-rw-rw-   0        0        0     2763 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/views/__pycache__/employee_div.cpython-38.pyc
+-rw-rw-rw-   0        0        0     9214 2023-03-17 07:39:53.000000 django-ipghrms-employee-1.8/employee/views/__pycache__/employee_m.cpython-310.pyc
+-rw-rw-rw-   0        0        0     8446 2022-10-20 01:02:26.000000 django-ipghrms-employee-1.8/employee/views/__pycache__/employee_m.cpython-37.pyc
+-rw-rw-rw-   0        0        0     7814 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/views/__pycache__/employee_m.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2783 2023-02-13 00:45:04.000000 django-ipghrms-employee-1.8/employee/views/__pycache__/employee_unit.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2771 2022-11-06 05:56:24.000000 django-ipghrms-employee-1.8/employee/views/__pycache__/employee_unit.cpython-37.pyc
+-rw-rw-rw-   0        0        0     2823 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/views/__pycache__/employee_unit.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2307 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/views/__pycache__/employee_user.cpython-38.pyc
+-rw-rw-rw-   0        0        0    15410 2023-03-15 13:47:43.000000 django-ipghrms-employee-1.8/employee/views/__pycache__/employee_v.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3007 2022-11-04 05:54:18.000000 django-ipghrms-employee-1.8/employee/views/__pycache__/employee_v.cpython-37.pyc
+-rw-rw-rw-   0        0        0     3036 2022-11-04 05:28:45.000000 django-ipghrms-employee-1.8/employee/views/__pycache__/employee_v.cpython-39.pyc
+-rw-rw-rw-   0        0        0     6379 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/views/__pycache__/id_card_print.cpython-38.pyc
+-rw-rw-rw-   0        0        0     6219 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/views/__pycache__/print.cpython-38.pyc
+-rw-rw-rw-   0        0        0     2708 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/views/__pycache__/print_cv.cpython-38.pyc
+-rw-rw-rw-   0        0        0     1395 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/views/__pycache__/users.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1429 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/views/__pycache__/users.cpython-38.pyc
+-rw-rw-rw-   0        0        0     2907 2022-12-14 12:34:30.000000 django-ipghrms-employee-1.8/employee/views/emp_rawdata.py
+-rw-rw-rw-   0        0        0    14951 2023-03-17 07:43:05.000000 django-ipghrms-employee-1.8/employee/views/employee2.py
+-rw-rw-rw-   0        0        0     4024 2023-01-25 02:35:35.000000 django-ipghrms-employee-1.8/employee/views/employee3.py
+-rw-rw-rw-   0        0        0     4288 2023-02-14 14:08:26.000000 django-ipghrms-employee-1.8/employee/views/employee_attach.py
+-rw-rw-rw-   0        0        0     1135 2023-02-10 01:57:57.000000 django-ipghrms-employee-1.8/employee/views/employee_chart.py
+-rw-rw-rw-   0        0        0     2809 2023-03-08 09:34:07.000000 django-ipghrms-employee-1.8/employee/views/employee_dash.py
+-rw-rw-rw-   0        0        0     1109 2023-02-10 01:57:18.000000 django-ipghrms-employee-1.8/employee/views/employee_dep.py
+-rw-rw-rw-   0        0        0    12343 2023-03-24 07:01:56.000000 django-ipghrms-employee-1.8/employee/views/employee_m.py
+-rw-rw-rw-   0        0        0     2840 2023-02-13 00:45:01.000000 django-ipghrms-employee-1.8/employee/views/employee_unit.py
+-rw-rw-rw-   0        0        0     2696 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/views/employee_user.py
+-rw-rw-rw-   0        0        0    21922 2023-04-11 09:19:16.000000 django-ipghrms-employee-1.8/employee/views/employee_v.py
+-rw-rw-rw-   0        0        0       63 2022-10-18 10:39:30.000000 django-ipghrms-employee-1.8/employee/views.py
+-rw-rw-rw-   0        0        0      511 2023-06-13 13:20:36.265791 django-ipghrms-employee-1.8/setup.cfg
+-rw-rw-rw-   0        0        0       39 2023-03-22 07:44:49.000000 django-ipghrms-employee-1.8/setup.py
```

### Comparing `django-ipghrms-employee-1.6/LICENSE` & `django-ipghrms-employee-1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/PKG-INFO` & `django-ipghrms-employee-1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ipghrms-employee
-Version: 1.6
+Version: 1.8
 Summary: Django IPG HRMS APP EMPLOYEE
 Home-page: http://ipg.tl/
 Author: Kinos
 Author-email: info@kinos.tl
 Maintainer: kinos
 Maintainer-email: info@kinos.tl
 License: MIT
```

### Comparing `django-ipghrms-employee-1.6/django_ipghrms_employee.egg-info/PKG-INFO` & `django-ipghrms-employee-1.8/django_ipghrms_employee.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ipghrms-employee
-Version: 1.6
+Version: 1.8
 Summary: Django IPG HRMS APP EMPLOYEE
 Home-page: http://ipg.tl/
 Author: Kinos
 Author-email: info@kinos.tl
 Maintainer: kinos
 Maintainer-email: info@kinos.tl
 License: MIT
```

### Comparing `django-ipghrms-employee-1.6/django_ipghrms_employee.egg-info/SOURCES.txt` & `django-ipghrms-employee-1.8/django_ipghrms_employee.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/admin.py` & `django-ipghrms-employee-1.8/employee/admin.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/api/__pycache__/urls.cpython-310.pyc` & `django-ipghrms-employee-1.8/employee/api/__pycache__/urls.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/api/__pycache__/urls.cpython-37.pyc` & `django-ipghrms-employee-1.8/employee/api/__pycache__/urls.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/api/__pycache__/urls.cpython-39.pyc` & `django-ipghrms-employee-1.8/employee/api/__pycache__/urls.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/api/__pycache__/views.cpython-310.pyc` & `django-ipghrms-employee-1.8/employee/api/__pycache__/views.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/api/__pycache__/views.cpython-37.pyc` & `django-ipghrms-employee-1.8/employee/api/__pycache__/views.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/api/__pycache__/views.cpython-39.pyc` & `django-ipghrms-employee-1.8/employee/api/__pycache__/views.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/api/urls.py` & `django-ipghrms-employee-1.8/employee/api/urls.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/api/views.py` & `django-ipghrms-employee-1.8/employee/api/views.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/forms.py` & `django-ipghrms-employee-1.8/employee/forms.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/0001_initial.py` & `django-ipghrms-employee-1.8/employee/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/0002_curempposition_curempdivision.py` & `django-ipghrms-employee-1.8/employee/migrations/0002_curempposition_curempdivision.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/0005_alter_employee_blood_alter_employee_father_and_more.py` & `django-ipghrms-employee-1.8/employee/migrations/0005_alter_employee_blood_alter_employee_father_and_more.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/0006_fidnumber_bank_address_fidnumber_customer_name_and_more.py` & `django-ipghrms-employee-1.8/employee/migrations/0006_fidnumber_bank_address_fidnumber_customer_name_and_more.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/0008_empspecialize.py` & `django-ipghrms-employee-1.8/employee/migrations/0008_empspecialize.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/0010_formaleducation_year.py` & `django-ipghrms-employee-1.8/employee/migrations/0010_formaleducation_year.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/0011_nonformaleducation_year.py` & `django-ipghrms-employee-1.8/employee/migrations/0011_nonformaleducation_year.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/0012_auto_20221122_1104.py` & `django-ipghrms-employee-1.8/employee/migrations/0012_auto_20221122_1104.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/0013_auto_20221122_1127.py` & `django-ipghrms-employee-1.8/employee/migrations/0013_auto_20221122_1127.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/0014_auto_20221130_2303.py` & `django-ipghrms-employee-1.8/employee/migrations/0014_auto_20221130_2303.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/0015_auto_20221130_2304.py` & `django-ipghrms-employee-1.8/employee/migrations/0015_auto_20221130_2304.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/0016_auto_20221130_2326.py` & `django-ipghrms-employee-1.8/employee/migrations/0016_auto_20221130_2326.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/0017_auto_20221130_2335.py` & `django-ipghrms-employee-1.8/employee/migrations/0017_auto_20221130_2335.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/0020_auto_20230117_1829.py` & `django-ipghrms-employee-1.8/employee/migrations/0020_auto_20230117_1829.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/0021_emplanguage_file_language.py` & `django-ipghrms-employee-1.8/employee/migrations/0021_emplanguage_file_language.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/0022_alter_photo_image.py` & `django-ipghrms-employee-1.8/employee/migrations/0022_alter_photo_image.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/0023_alter_photo_image.py` & `django-ipghrms-employee-1.8/employee/migrations/0023_alter_photo_image.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/0025_empsignature.py` & `django-ipghrms-employee-1.8/employee/migrations/0025_empsignature.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/__pycache__/0001_initial.cpython-310.pyc` & `django-ipghrms-employee-1.8/employee/migrations/__pycache__/0001_initial.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/__pycache__/0001_initial.cpython-37.pyc` & `django-ipghrms-employee-1.8/employee/migrations/__pycache__/0001_initial.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/__pycache__/0001_initial.cpython-39.pyc` & `django-ipghrms-employee-1.8/employee/migrations/__pycache__/0001_initial.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/__pycache__/0002_curempposition_curempdivision.cpython-310.pyc` & `django-ipghrms-employee-1.8/employee/migrations/__pycache__/0002_curempposition_curempdivision.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/__pycache__/0002_curempposition_curempdivision.cpython-37.pyc` & `django-ipghrms-employee-1.8/employee/migrations/__pycache__/0002_curempposition_curempdivision.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/__pycache__/0002_curempposition_curempdivision.cpython-39.pyc` & `django-ipghrms-employee-1.8/employee/migrations/__pycache__/0002_curempposition_curempdivision.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/__pycache__/0003_employee_is_new.cpython-310.pyc` & `django-ipghrms-employee-1.8/employee/migrations/__pycache__/0003_employee_is_new.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/__pycache__/0003_employee_is_new.cpython-37.pyc` & `django-ipghrms-employee-1.8/employee/migrations/__pycache__/0003_employee_is_new.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/__pycache__/0003_employee_is_new.cpython-39.pyc` & `django-ipghrms-employee-1.8/employee/migrations/__pycache__/0003_employee_is_new.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/__pycache__/0004_employee_emp_id.cpython-310.pyc` & `django-ipghrms-employee-1.8/employee/migrations/__pycache__/0004_employee_emp_id.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/__pycache__/0004_employee_emp_id.cpython-37.pyc` & `django-ipghrms-employee-1.8/employee/migrations/__pycache__/0004_employee_emp_id.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/__pycache__/0004_employee_emp_id.cpython-39.pyc` & `django-ipghrms-employee-1.8/employee/migrations/__pycache__/0004_employee_emp_id.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/__pycache__/0005_alter_employee_blood_alter_employee_father_and_more.cpython-310.pyc` & `django-ipghrms-employee-1.8/employee/migrations/__pycache__/0005_alter_employee_blood_alter_employee_father_and_more.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/__pycache__/0005_alter_employee_blood_alter_employee_father_and_more.cpython-37.pyc` & `django-ipghrms-employee-1.8/employee/migrations/__pycache__/0005_alter_employee_blood_alter_employee_father_and_more.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/__pycache__/0005_alter_employee_blood_alter_employee_father_and_more.cpython-39.pyc` & `django-ipghrms-employee-1.8/employee/migrations/__pycache__/0005_alter_employee_blood_alter_employee_father_and_more.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/__pycache__/0006_fidnumber_bank_address_fidnumber_customer_name_and_more.cpython-310.pyc` & `django-ipghrms-employee-1.8/employee/migrations/__pycache__/0006_fidnumber_bank_address_fidnumber_customer_name_and_more.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/__pycache__/0006_fidnumber_bank_address_fidnumber_customer_name_and_more.cpython-37.pyc` & `django-ipghrms-employee-1.8/employee/migrations/__pycache__/0006_fidnumber_bank_address_fidnumber_customer_name_and_more.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/__pycache__/0007_alter_fidnumber_customer_name.cpython-310.pyc` & `django-ipghrms-employee-1.8/employee/migrations/__pycache__/0007_alter_fidnumber_customer_name.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/__pycache__/0007_alter_fidnumber_customer_name.cpython-37.pyc` & `django-ipghrms-employee-1.8/employee/migrations/__pycache__/0007_alter_fidnumber_customer_name.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/__pycache__/0008_empspecialize.cpython-310.pyc` & `django-ipghrms-employee-1.8/employee/migrations/__pycache__/0008_empspecialize.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/__pycache__/0008_empspecialize.cpython-37.pyc` & `django-ipghrms-employee-1.8/employee/migrations/__pycache__/0008_empspecialize.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/__pycache__/0009_alter_empspecialize_name.cpython-310.pyc` & `django-ipghrms-employee-1.8/employee/migrations/__pycache__/0009_alter_empspecialize_name.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/__pycache__/0009_alter_empspecialize_name.cpython-37.pyc` & `django-ipghrms-employee-1.8/employee/migrations/__pycache__/0009_alter_empspecialize_name.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/__pycache__/0010_formaleducation_year.cpython-310.pyc` & `django-ipghrms-employee-1.8/employee/migrations/__pycache__/0010_formaleducation_year.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/__pycache__/0011_nonformaleducation_year.cpython-310.pyc` & `django-ipghrms-employee-1.8/employee/migrations/__pycache__/0011_nonformaleducation_year.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/__pycache__/0012_auto_20221122_1104.cpython-310.pyc` & `django-ipghrms-employee-1.8/employee/migrations/__pycache__/0012_auto_20221122_1104.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/__pycache__/0013_auto_20221122_1127.cpython-310.pyc` & `django-ipghrms-employee-1.8/employee/migrations/__pycache__/0013_auto_20221122_1127.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/__pycache__/0014_auto_20221130_2303.cpython-310.pyc` & `django-ipghrms-employee-1.8/employee/migrations/__pycache__/0014_auto_20221130_2303.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/__pycache__/0015_auto_20221130_2304.cpython-310.pyc` & `django-ipghrms-employee-1.8/employee/migrations/__pycache__/0015_auto_20221130_2304.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/__pycache__/0016_auto_20221130_2326.cpython-310.pyc` & `django-ipghrms-employee-1.8/employee/migrations/__pycache__/0016_auto_20221130_2326.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/__pycache__/0017_auto_20221130_2335.cpython-310.pyc` & `django-ipghrms-employee-1.8/employee/migrations/__pycache__/0017_auto_20221130_2335.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/__pycache__/0018_employee_pin.cpython-310.pyc` & `django-ipghrms-employee-1.8/employee/migrations/__pycache__/0018_employee_pin.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/__pycache__/0019_employee_ext.cpython-310.pyc` & `django-ipghrms-employee-1.8/employee/migrations/__pycache__/0019_employee_ext.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/__pycache__/0020_auto_20230117_1825.cpython-310.pyc` & `django-ipghrms-employee-1.8/employee/migrations/__pycache__/0020_auto_20230117_1825.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/__pycache__/0020_auto_20230117_1827.cpython-310.pyc` & `django-ipghrms-employee-1.8/employee/migrations/__pycache__/0020_auto_20230117_1827.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/__pycache__/0020_auto_20230117_1829.cpython-310.pyc` & `django-ipghrms-employee-1.8/employee/migrations/__pycache__/0020_auto_20230117_1829.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/__pycache__/0021_emplanguage_file_language.cpython-310.pyc` & `django-ipghrms-employee-1.8/employee/migrations/__pycache__/0021_emplanguage_file_language.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/__pycache__/0022_alter_photo_image.cpython-310.pyc` & `django-ipghrms-employee-1.8/employee/migrations/__pycache__/0022_alter_photo_image.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/__pycache__/0023_alter_photo_image.cpython-310.pyc` & `django-ipghrms-employee-1.8/employee/migrations/__pycache__/0023_alter_photo_image.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/__pycache__/0024_alter_fidnumber_options.cpython-310.pyc` & `django-ipghrms-employee-1.8/employee/migrations/__pycache__/0024_alter_fidnumber_options.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/migrations/__pycache__/0025_empsignature.cpython-310.pyc` & `django-ipghrms-employee-1.8/employee/migrations/__pycache__/0025_empsignature.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/models.py` & `django-ipghrms-employee-1.8/employee/models.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/reports/__pycache__/views.cpython-310.pyc` & `django-ipghrms-employee-1.8/employee/reports/__pycache__/views.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/reports/__pycache__/views.cpython-37.pyc` & `django-ipghrms-employee-1.8/employee/reports/__pycache__/views.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/reports/__pycache__/views.cpython-39.pyc` & `django-ipghrms-employee-1.8/employee/reports/__pycache__/views.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/reports/views.py` & `django-ipghrms-employee-1.8/employee/reports/views.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/signals.py` & `django-ipghrms-employee-1.8/employee/signals.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/components/password_modal.html` & `django-ipghrms-employee-1.8/employee/templates/components/password_modal.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/components/password_modal_list.html` & `django-ipghrms-employee-1.8/employee/templates/components/password_modal_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/components/password_validation.html` & `django-ipghrms-employee-1.8/employee/templates/components/password_validation.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee/emp_attach.html` & `django-ipghrms-employee-1.8/employee/templates/employee/emp_attach.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee/emp_contact_list.html` & `django-ipghrms-employee-1.8/employee/templates/employee/emp_contact_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee/emp_dash.html` & `django-ipghrms-employee-1.8/employee/templates/employee/emp_dash.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee/emp_detail.html` & `django-ipghrms-employee-1.8/employee/templates/employee/emp_detail.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee/emp_detail_bottom.html` & `django-ipghrms-employee-1.8/employee/templates/employee/emp_detail_bottom.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee/emp_detail_left.html` & `django-ipghrms-employee-1.8/employee/templates/employee/emp_detail_left.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee/emp_detail_right.html` & `django-ipghrms-employee-1.8/employee/templates/employee/emp_detail_right.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee/emp_list.html` & `django-ipghrms-employee-1.8/employee/templates/employee/emp_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee/emp_list_deact.html` & `django-ipghrms-employee-1.8/employee/templates/employee/emp_list_deact.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee/emp_photo.html` & `django-ipghrms-employee-1.8/employee/templates/employee/emp_photo.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee/emp_raw_data.html` & `django-ipghrms-employee-1.8/employee/templates/employee/emp_raw_data.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee/form.html` & `django-ipghrms-employee-1.8/employee/templates/employee/form.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee/form2.html` & `django-ipghrms-employee-1.8/employee/templates/employee/form2.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee/form3.html` & `django-ipghrms-employee-1.8/employee/templates/employee/form3.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee/form_address.html` & `django-ipghrms-employee-1.8/employee/templates/employee/form_address.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee/form_location.html` & `django-ipghrms-employee-1.8/employee/templates/employee/form_location.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee/maps.html` & `django-ipghrms-employee-1.8/employee/templates/employee/maps.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee/s_emp_attach.html` & `django-ipghrms-employee-1.8/employee/templates/employee/s_emp_attach.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee2/depend_list.html` & `django-ipghrms-employee-1.8/employee/templates/employee2/depend_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee2/form.html` & `django-ipghrms-employee-1.8/employee/templates/employee2/form.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee2/formal_detail.html` & `django-ipghrms-employee-1.8/employee/templates/employee2/formal_detail.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee2/formal_list.html` & `django-ipghrms-employee-1.8/employee/templates/employee2/formal_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee2/nonformal_detail.html` & `django-ipghrms-employee-1.8/employee/templates/employee2/nonformal_detail.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee2/nonformal_list.html` & `django-ipghrms-employee-1.8/employee/templates/employee2/nonformal_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee2/photo.html` & `django-ipghrms-employee-1.8/employee/templates/employee2/photo.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee2/photo_modal.html` & `django-ipghrms-employee-1.8/employee/templates/employee2/photo_modal.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee2/workexp_detail.html` & `django-ipghrms-employee-1.8/employee/templates/employee2/workexp_detail.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee2/workexp_list.html` & `django-ipghrms-employee-1.8/employee/templates/employee2/workexp_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee3/adv_list.html` & `django-ipghrms-employee-1.8/employee/templates/employee3/adv_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee3/de_list.html` & `django-ipghrms-employee-1.8/employee/templates/employee3/de_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee3/dep_list.html` & `django-ipghrms-employee-1.8/employee/templates/employee3/dep_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee3/no_div_list.html` & `django-ipghrms-employee-1.8/employee/templates/employee3/no_div_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee3/raw_data.html` & `django-ipghrms-employee-1.8/employee/templates/employee3/raw_data.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee3/raw_data_adv.html` & `django-ipghrms-employee-1.8/employee/templates/employee3/raw_data_adv.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee3/raw_data_all.html` & `django-ipghrms-employee-1.8/employee/templates/employee3/raw_data_all.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee3/raw_data_emp.html` & `django-ipghrms-employee-1.8/employee/templates/employee3/raw_data_emp.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee3/raw_data_habi.html` & `django-ipghrms-employee-1.8/employee/templates/employee3/raw_data_habi.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee3/staff_list.html` & `django-ipghrms-employee-1.8/employee/templates/employee3/staff_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee3/unit_list.html` & `django-ipghrms-employee-1.8/employee/templates/employee3/unit_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee_chart/chart_emp.html` & `django-ipghrms-employee-1.8/employee/templates/employee_chart/chart_emp.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee_chart/chart_emp_dep.html` & `django-ipghrms-employee-1.8/employee/templates/employee_chart/chart_emp_dep.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee_chart/chart_emp_unit.html` & `django-ipghrms-employee-1.8/employee/templates/employee_chart/chart_emp_unit.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee_chart/emp_age.js` & `django-ipghrms-employee-1.8/employee/templates/employee_chart/emp_age.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee_chart/emp_age2.js` & `django-ipghrms-employee-1.8/employee/templates/employee_chart/emp_age2.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee_chart/emp_all.js` & `django-ipghrms-employee-1.8/employee/templates/employee_chart/emp_all.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee_chart/emp_country.js` & `django-ipghrms-employee-1.8/employee/templates/employee_chart/emp_country.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee_chart/emp_dep.js` & `django-ipghrms-employee-1.8/employee/templates/employee_chart/emp_nivelaca.js`

 * *Files 21% similar despite different names*

#### js-beautify {}

```diff
@@ -1,87 +1,60 @@
-var endpoint = '/api/employee/dep/'
+var endpoint = '/api/employee/nivelaca/'
 $.ajax({
     method: "GET",
     url: endpoint,
     success: function(data) {
         obj = data.obj
-        legend = 'DISTRIBUISAUN FUNSIONARIO TUIR EKIPA'
-        categories = data.label
-        setEmpDep()
+        legend = data.label
+        setEmpNivelAca()
     },
     error: function(error_data) {
         console.log("error")
         console.log(error_data)
     }
 })
 
-function setEmpDep() {
-    Highcharts.chart('setEmpDep', {
+function setEmpNivelAca() {
+    Highcharts.chart('setEmpNivelAca', {
+        colors: ['#01BAF2', '#71BF45', '#FAA74B', '#B37CD2', '#d42c06', '#dbde23', '#68d9d7'],
         chart: {
-            type: 'bar'
+            type: 'pie'
         },
-        title: {
-            align: 'center',
-            text: legend
-        },
-        subtitle: {},
         accessibility: {
-            announceNewData: {
-                enabled: true
+            point: {
+                valueSuffix: '%'
             }
         },
-        xAxis: {
-            categories: categories,
-            title: {
-                text: null
-            }
+        title: {
+            text: legend
         },
-        yAxis: {
-            min: 0,
-            title: {
-                text: 'Total Staff',
-                align: 'high'
-            },
-            labels: {
-                overflow: 'justify'
+        tooltip: {
+            formatter: function() {
+                return this.point.name + ': ' + this.y;
             }
-
-        },
-        legend: {
-            enabled: false
         },
         plotOptions: {
-            series: {
-                borderWidth: 0,
+            pie: {
+                allowPointSelect: true,
+                cursor: 'pointer',
                 dataLabels: {
                     enabled: true,
-                    format: '{point.y}'
-                }
+                    formatter: function() {
+                        return this.point.name + ': ' + this.y;
+                    }
+                },
+                showInLegend: true
             }
         },
         credits: {
             enabled: false
         },
-
-        tooltip: {
-            formatter: function() {
-                return this.point.name + ': ' + this.y;
-            }
-        },
-
         series: [{
-            name: "Ekipa",
+            name: 'Registrations',
             colorByPoint: true,
+            innerSize: '75%',
             data: obj
-        }],
-        drilldown: {
-            breadcrumbs: {
-                position: {
-                    align: 'right'
-                }
-            },
-            series: []
-        }
+        }]
     });
 
 
 }
```

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee_chart/emp_dep2.js` & `django-ipghrms-employee-1.8/employee/templates/employee_chart/emp_dep2.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee_chart/emp_gender.js` & `django-ipghrms-employee-1.8/employee/templates/employee_chart/emp_gender.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee_chart/emp_mun.js` & `django-ipghrms-employee-1.8/employee/templates/employee_chart/emp_mun.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee_chart/emp_nivelaca.js` & `django-ipghrms-employee-1.8/employee/templates/employee_chart/emp_unit.js`

 * *Files 26% similar despite different names*

#### js-beautify {}

```diff
@@ -1,60 +1,56 @@
-var endpoint = '/api/employee/nivelaca/'
+var endpoint = '/api/employee/unit/'
 $.ajax({
     method: "GET",
     url: endpoint,
     success: function(data) {
-        obj = data.obj
+        d = data,
+            obj = data.obj
         legend = data.label
-        setEmpNivelAca()
+        dt = data.datas
+        setEmpDivision()
     },
     error: function(error_data) {
         console.log("error")
         console.log(error_data)
     }
 })
 
-function setEmpNivelAca() {
-    Highcharts.chart('setEmpNivelAca', {
-        colors: ['#01BAF2', '#71BF45', '#FAA74B', '#B37CD2', '#d42c06', '#dbde23', '#68d9d7'],
+function setEmpDivision() {
+    Highcharts.chart('setEmpDivision', {
         chart: {
+            plotBackgroundColor: null,
+            plotBorderWidth: null,
+            plotShadow: false,
             type: 'pie'
         },
-        accessibility: {
-            point: {
-                valueSuffix: '%'
-            }
-        },
         title: {
-            text: legend
+            text: 'DISTRIBUISAUN FUNSIONARIO TUIR DIVIZAUN',
+            align: 'center'
         },
         tooltip: {
             formatter: function() {
                 return this.point.name + ': ' + this.y;
             }
         },
         plotOptions: {
             pie: {
                 allowPointSelect: true,
                 cursor: 'pointer',
                 dataLabels: {
                     enabled: true,
-                    formatter: function() {
-                        return this.point.name + ': ' + this.y;
-                    }
-                },
-                showInLegend: true
+                    format: '{point.name}: {point.y}'
+                }
             }
         },
         credits: {
             enabled: false
         },
         series: [{
-            name: 'Registrations',
+            name: 'Brands',
             colorByPoint: true,
-            innerSize: '75%',
-            data: obj
+            data: dt
         }]
     });
 
 
 }
```

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee_chart/emp_nivelaca2.js` & `django-ipghrms-employee-1.8/employee/templates/employee_chart/emp_nivelaca2.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee_chart/emp_unit.js` & `django-ipghrms-employee-1.8/employee/templates/employee_chart/myoption.js`

 * *Files 24% similar despite different names*

#### js-beautify {}

```diff
@@ -1,56 +1,53 @@
-var endpoint = '/api/employee/unit/'
-$.ajax({
-    method: "GET",
-    url: endpoint,
-    success: function(data) {
-        d = data,
-            obj = data.obj
-        legend = data.label
-        dt = data.datas
-        setEmpDivision()
+var myoption = {
+    tooltips: {
+        enabled: true
     },
-    error: function(error_data) {
-        console.log("error")
-        console.log(error_data)
-    }
-})
-
-function setEmpDivision() {
-    Highcharts.chart('setEmpDivision', {
-        chart: {
-            plotBackgroundColor: null,
-            plotBorderWidth: null,
-            plotShadow: false,
-            type: 'pie'
-        },
-        title: {
-            text: 'DISTRIBUISAUN FUNSIONARIO TUIR DIVIZAUN',
-            align: 'center'
-        },
-        tooltip: {
-            formatter: function() {
-                return this.point.name + ': ' + this.y;
-            }
-        },
-        plotOptions: {
-            pie: {
-                allowPointSelect: true,
-                cursor: 'pointer',
-                dataLabels: {
-                    enabled: true,
-                    format: '{point.name}: {point.y}'
-                }
+    hover: {
+        animationDuration: 1
+    },
+    legend: {
+        display: false,
+        position: 'bottom',
+        labels: {
+            fontColor: 'rgb(255, 99, 132)'
+        }
+    },
+    responsive: true,
+    maintainAspectRatio: false,
+    scales: {
+        yAxes: [{
+            ticks: {
+                beginAtZero: true,
+                precision: 0
             }
-        },
-        credits: {
-            enabled: false
-        },
-        series: [{
-            name: 'Brands',
-            colorByPoint: true,
-            data: dt
         }]
-    });
+    },
+    animation: {
+        duration: 1,
+        onComplete: function() {
+            var chartInstance = this.chart,
+                ctx = chartInstance.ctx;
+            ctx.textAlign = 'center';
+            ctx.fillStyle = "rgba(0, 0, 0, 1)";
+            ctx.textBaseline = 'bottom';
+
+            this.data.datasets.forEach(function(dataset, i) {
+                var meta = chartInstance.controller.getDatasetMeta(i);
+                meta.data.forEach(function(bar, index) {
+                    var data = dataset.data[index];
+                    ctx.fillText(data, bar._model.x, bar._model.y - 0);
 
+                });
+            });
+        }
+    },
 
-}
+    layout: {
+        padding: {
+            left: 10,
+            right: 10,
+            top: 20,
+            bottom: 10
+        }
+    }
+};
```

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee_chart/myoption.js` & `django-ipghrms-employee-1.8/employee/templates/employee_chart/udep_emp_gender.js`

 * *Files 20% similar despite different names*

#### js-beautify {}

```diff
@@ -1,28 +1,27 @@
-var myoption = {
+var gender_myoption = {
     tooltips: {
         enabled: true
     },
     hover: {
         animationDuration: 1
     },
     legend: {
-        display: false,
+        display: true,
         position: 'bottom',
         labels: {
-            fontColor: 'rgb(255, 99, 132)'
+            fontColor: 'rgba(132, 138, 240, 0.75)'
         }
     },
     responsive: true,
     maintainAspectRatio: false,
     scales: {
         yAxes: [{
             ticks: {
-                beginAtZero: true,
-                precision: 0
+                beginAtZero: true
             }
         }]
     },
     animation: {
         duration: 1,
         onComplete: function() {
             var chartInstance = this.chart,
@@ -37,17 +36,52 @@
                     var data = dataset.data[index];
                     ctx.fillText(data, bar._model.x, bar._model.y - 0);
 
                 });
             });
         }
     },
-
     layout: {
         padding: {
             left: 10,
             right: 10,
             top: 20,
             bottom: 10
         }
     }
-};
+};
+
+var genderbgColors = [
+    'rgba(54, 162, 235, 1)', 'rgba(255, 99, 132, 1)', 'rgba(255, 206, 86, 1)',
+    'rgba(75, 192, 192, 1)', 'rgba(153, 102, 255, 1)', 'rgba(255, 159, 64, 1)'
+];
+
+var endpoint1 = '/api/employee/u/dep/gender/'
+$.ajax({
+    method: "GET",
+    url: endpoint1,
+    success: function(data) {
+        const data1 = {
+            labels: data.label,
+            datasets: [{
+                label: 'Generu',
+                data: data.obj,
+                backgroundColor: genderbgColors,
+                borderWidth: 1
+            }]
+        };
+
+        const config_gen = {
+            type: 'pie',
+            data: data1,
+            options: gender_myoption
+        };
+        const genderChart_data1 = new Chart(
+            document.getElementById('genderChart_data1'),
+            config_gen
+        );
+    },
+    error: function(error_data) {
+        console.log("error")
+        console.log(error_data)
+    }
+})
```

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee_detail/attendance.html` & `django-ipghrms-employee-1.8/employee/templates/employee_detail/attendance.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee_detail/basic.html` & `django-ipghrms-employee-1.8/employee/templates/employee_detail/basic.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee_detail/evaluation.html` & `django-ipghrms-employee-1.8/employee/templates/employee_detail/evaluation.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee_detail/header.html` & `django-ipghrms-employee-1.8/employee/templates/employee_detail/header.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee_detail/leave.html` & `django-ipghrms-employee-1.8/employee/templates/employee_detail/leave.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee_detail/onboarding.html` & `django-ipghrms-employee-1.8/employee/templates/employee_detail/onboarding.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee_detail/training.html` & `django-ipghrms-employee-1.8/employee/templates/employee_detail/training.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee_detail/trip.html` & `django-ipghrms-employee-1.8/employee/templates/employee_detail/trip.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee_print/cv_1_iden.html` & `django-ipghrms-employee-1.8/employee/templates/employee_print/cv_1_iden.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee_print/cv_2_nat_fam.html` & `django-ipghrms-employee-1.8/employee/templates/employee_print/cv_2_nat_fam.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee_print/cv_3_hab_acc.html` & `django-ipghrms-employee-1.8/employee/templates/employee_print/cv_3_hab_acc.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee_print/cv_4_col_fun.html` & `django-ipghrms-employee-1.8/employee/templates/employee_print/cv_4_col_fun.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee_print/cv_4_col_fun_back.html` & `django-ipghrms-employee-1.8/employee/templates/employee_print/cv_4_col_fun_back.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee_print/cv_5_per_fal.html` & `django-ipghrms-employee-1.8/employee/templates/employee_print/cv_5_per_fal.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee_print/cv_6_pen_lov.html` & `django-ipghrms-employee-1.8/employee/templates/employee_print/cv_6_pen_lov.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee_print/layout.html` & `django-ipghrms-employee-1.8/employee/templates/employee_print/layout.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee_print/print_cv.html` & `django-ipghrms-employee-1.8/employee/templates/employee_print/print_cv.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee_reports/aca_level_list.html` & `django-ipghrms-employee-1.8/employee/templates/employee_reports/aca_level_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee_reports/r_dash.html` & `django-ipghrms-employee-1.8/employee/templates/employee_reports/r_dash.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee_users/emp_dep_list.html` & `django-ipghrms-employee-1.8/employee/templates/employee_users/emp_dep_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee_users/emp_detail.html` & `django-ipghrms-employee-1.8/employee/templates/employee_users/emp_detail.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee_users/emp_detail_bottom.html` & `django-ipghrms-employee-1.8/employee/templates/employee_users/emp_detail_bottom.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee_users/emp_detail_left.html` & `django-ipghrms-employee-1.8/employee/templates/employee_users/emp_detail_left.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee_users/emp_detail_right.html` & `django-ipghrms-employee-1.8/employee/templates/employee_users/emp_detail_right.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee_users/emp_staff_list.html` & `django-ipghrms-employee-1.8/employee/templates/employee_users/emp_staff_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/templates/employee_users/emp_unit_dash.html` & `django-ipghrms-employee-1.8/employee/templates/employee_users/emp_unit_dash.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/urls.py` & `django-ipghrms-employee-1.8/employee/urls.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/utils.py` & `django-ipghrms-employee-1.8/employee/utils.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/views/__pycache__/emp_rawdata.cpython-310.pyc` & `django-ipghrms-employee-1.8/employee/views/__pycache__/emp_rawdata.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/views/__pycache__/emp_rawdata.cpython-37.pyc` & `django-ipghrms-employee-1.8/employee/views/__pycache__/emp_rawdata.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/views/__pycache__/emp_rawdata.cpython-39.pyc` & `django-ipghrms-employee-1.8/employee/views/__pycache__/emp_rawdata.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/views/__pycache__/employee.cpython-37.pyc` & `django-ipghrms-employee-1.8/employee/views/__pycache__/employee.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/views/__pycache__/employee.cpython-38.pyc` & `django-ipghrms-employee-1.8/employee/views/__pycache__/employee.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/views/__pycache__/employee2.cpython-310.pyc` & `django-ipghrms-employee-1.8/employee/views/__pycache__/employee2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/views/__pycache__/employee2.cpython-37.pyc` & `django-ipghrms-employee-1.8/employee/views/__pycache__/employee2.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/views/__pycache__/employee2.cpython-38.pyc` & `django-ipghrms-employee-1.8/employee/views/__pycache__/employee2.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/views/__pycache__/employee2.cpython-39.pyc` & `django-ipghrms-employee-1.8/employee/views/__pycache__/employee2.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/views/__pycache__/employee3.cpython-310.pyc` & `django-ipghrms-employee-1.8/employee/views/__pycache__/employee3.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/views/__pycache__/employee3.cpython-37.pyc` & `django-ipghrms-employee-1.8/employee/views/__pycache__/employee3.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/views/__pycache__/employee3.cpython-38.pyc` & `django-ipghrms-employee-1.8/employee/views/__pycache__/employee3.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/views/__pycache__/employee3.cpython-39.pyc` & `django-ipghrms-employee-1.8/employee/views/__pycache__/employee3.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/views/__pycache__/employee_attach.cpython-310.pyc` & `django-ipghrms-employee-1.8/employee/views/__pycache__/employee_attach.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/views/__pycache__/employee_attach.cpython-38.pyc` & `django-ipghrms-employee-1.8/employee/views/__pycache__/employee_attach.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/views/__pycache__/employee_carrier.cpython-38.pyc` & `django-ipghrms-employee-1.8/employee/views/__pycache__/employee_carrier.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/views/__pycache__/employee_chart.cpython-310.pyc` & `django-ipghrms-employee-1.8/employee/views/__pycache__/employee_chart.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/views/__pycache__/employee_chart.cpython-37.pyc` & `django-ipghrms-employee-1.8/employee/views/__pycache__/employee_chart.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/views/__pycache__/employee_chart.cpython-38.pyc` & `django-ipghrms-employee-1.8/employee/views/__pycache__/employee_chart.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/views/__pycache__/employee_chart.cpython-39.pyc` & `django-ipghrms-employee-1.8/employee/views/__pycache__/employee_chart.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/views/__pycache__/employee_dash.cpython-310.pyc` & `django-ipghrms-employee-1.8/employee/views/__pycache__/employee_dash.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/views/__pycache__/employee_dash.cpython-37.pyc` & `django-ipghrms-employee-1.8/employee/views/__pycache__/employee_dash.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/views/__pycache__/employee_dash.cpython-38.pyc` & `django-ipghrms-employee-1.8/employee/views/__pycache__/employee_dash.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/views/__pycache__/employee_dash.cpython-39.pyc` & `django-ipghrms-employee-1.8/employee/views/__pycache__/employee_dash.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/views/__pycache__/employee_de.cpython-39.pyc` & `django-ipghrms-employee-1.8/employee/views/__pycache__/employee_de.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/views/__pycache__/employee_dep.cpython-310.pyc` & `django-ipghrms-employee-1.8/employee/views/__pycache__/employee_dep.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/views/__pycache__/employee_dep.cpython-37.pyc` & `django-ipghrms-employee-1.8/employee/views/__pycache__/employee_dep.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/views/__pycache__/employee_dep.cpython-39.pyc` & `django-ipghrms-employee-1.8/employee/views/__pycache__/employee_dep.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/views/__pycache__/employee_dg.cpython-38.pyc` & `django-ipghrms-employee-1.8/employee/views/__pycache__/employee_dg.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/views/__pycache__/employee_div.cpython-38.pyc` & `django-ipghrms-employee-1.8/employee/views/__pycache__/employee_div.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/views/__pycache__/employee_m.cpython-310.pyc` & `django-ipghrms-employee-1.8/employee/views/__pycache__/employee_m.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/views/__pycache__/employee_m.cpython-37.pyc` & `django-ipghrms-employee-1.8/employee/views/__pycache__/employee_m.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/views/__pycache__/employee_m.cpython-39.pyc` & `django-ipghrms-employee-1.8/employee/views/__pycache__/employee_m.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/views/__pycache__/employee_unit.cpython-310.pyc` & `django-ipghrms-employee-1.8/employee/views/__pycache__/employee_unit.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/views/__pycache__/employee_unit.cpython-37.pyc` & `django-ipghrms-employee-1.8/employee/views/__pycache__/employee_unit.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/views/__pycache__/employee_unit.cpython-39.pyc` & `django-ipghrms-employee-1.8/employee/views/__pycache__/employee_unit.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/views/__pycache__/employee_user.cpython-38.pyc` & `django-ipghrms-employee-1.8/employee/views/__pycache__/employee_user.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/views/__pycache__/employee_v.cpython-310.pyc` & `django-ipghrms-employee-1.8/employee/views/__pycache__/employee_v.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/views/__pycache__/employee_v.cpython-37.pyc` & `django-ipghrms-employee-1.8/employee/views/__pycache__/employee_v.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/views/__pycache__/employee_v.cpython-39.pyc` & `django-ipghrms-employee-1.8/employee/views/__pycache__/employee_v.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/views/__pycache__/id_card_print.cpython-38.pyc` & `django-ipghrms-employee-1.8/employee/views/__pycache__/id_card_print.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/views/__pycache__/print.cpython-38.pyc` & `django-ipghrms-employee-1.8/employee/views/__pycache__/print.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/views/__pycache__/print_cv.cpython-38.pyc` & `django-ipghrms-employee-1.8/employee/views/__pycache__/print_cv.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/views/__pycache__/users.cpython-37.pyc` & `django-ipghrms-employee-1.8/employee/views/__pycache__/users.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/views/__pycache__/users.cpython-38.pyc` & `django-ipghrms-employee-1.8/employee/views/__pycache__/users.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/views/emp_rawdata.py` & `django-ipghrms-employee-1.8/employee/views/emp_rawdata.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/views/employee2.py` & `django-ipghrms-employee-1.8/employee/views/employee2.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/views/employee3.py` & `django-ipghrms-employee-1.8/employee/views/employee3.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/views/employee_attach.py` & `django-ipghrms-employee-1.8/employee/views/employee_attach.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/views/employee_chart.py` & `django-ipghrms-employee-1.8/employee/views/employee_chart.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/views/employee_dash.py` & `django-ipghrms-employee-1.8/employee/views/employee_dash.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/views/employee_dep.py` & `django-ipghrms-employee-1.8/employee/views/employee_dep.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/views/employee_m.py` & `django-ipghrms-employee-1.8/employee/views/employee_m.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/views/employee_unit.py` & `django-ipghrms-employee-1.8/employee/views/employee_unit.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/views/employee_user.py` & `django-ipghrms-employee-1.8/employee/views/employee_user.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-employee-1.6/employee/views/employee_v.py` & `django-ipghrms-employee-1.8/employee/views/employee_v.py`

 * *Files identical despite different names*

