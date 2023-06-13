# Comparing `tmp/django-ipghrms-contract-1.8.tar.gz` & `tmp/django-ipghrms-contract-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\django-ipghrms-contract-1.8.tar", last modified: Sat Jun  3 01:26:29 2023, max compression
+gzip compressed data, was "django-ipghrms-contract-1.9.tar", last modified: Sat Jun  3 02:43:43 2023, max compression
```

## Comparing `django-ipghrms-contract-1.8.tar` & `django-ipghrms-contract-1.9.tar`

### file list

```diff
@@ -1,185 +1,185 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 01:26:29.324357 django-ipghrms-contract-1.8/
--rw-rw-rw-   0        0        0     1068 2023-03-22 07:40:25.000000 django-ipghrms-contract-1.8/LICENSE
--rw-rw-rw-   0        0        0      222 2023-03-27 14:21:27.000000 django-ipghrms-contract-1.8/MANIFEST.in
--rw-rw-rw-   0        0        0     1158 2023-06-03 01:26:29.324357 django-ipghrms-contract-1.8/PKG-INFO
--rw-rw-rw-   0        0        0      503 2023-03-27 01:42:56.000000 django-ipghrms-contract-1.8/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-03 01:26:29.094057 django-ipghrms-contract-1.8/contract/
--rw-rw-rw-   0        0        0        0 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.8/contract/__init__.py
--rw-rw-rw-   0        0        0     2240 2023-06-02 20:59:28.000000 django-ipghrms-contract-1.8/contract/admin.py
-drwxrwxrwx   0        0        0        0 2023-06-03 01:26:29.098047 django-ipghrms-contract-1.8/contract/api/
-drwxrwxrwx   0        0        0        0 2023-06-03 01:26:29.104038 django-ipghrms-contract-1.8/contract/api/__pycache__/
--rw-rw-rw-   0        0        0      405 2023-01-22 14:24:18.000000 django-ipghrms-contract-1.8/contract/api/__pycache__/urls.cpython-310.pyc
--rw-rw-rw-   0        0        0      348 2022-11-05 14:50:10.000000 django-ipghrms-contract-1.8/contract/api/__pycache__/urls.cpython-37.pyc
--rw-rw-rw-   0        0        0     2913 2023-03-12 11:13:58.000000 django-ipghrms-contract-1.8/contract/api/__pycache__/views.cpython-310.pyc
--rw-rw-rw-   0        0        0     2464 2022-11-05 14:50:10.000000 django-ipghrms-contract-1.8/contract/api/__pycache__/views.cpython-37.pyc
--rw-rw-rw-   0        0        0      262 2023-01-22 14:24:15.000000 django-ipghrms-contract-1.8/contract/api/urls.py
--rw-rw-rw-   0        0        0     2564 2023-03-12 11:13:55.000000 django-ipghrms-contract-1.8/contract/api/views.py
--rw-rw-rw-   0        0        0      132 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.8/contract/apps.py
-drwxrwxrwx   0        0        0        0 2023-06-03 01:26:29.108021 django-ipghrms-contract-1.8/contract/forms/
--rw-rw-rw-   0        0        0       48 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.8/contract/forms/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-03 01:26:29.122317 django-ipghrms-contract-1.8/contract/forms/__pycache__/
--rw-rw-rw-   0        0        0      189 2022-11-07 13:19:37.000000 django-ipghrms-contract-1.8/contract/forms/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      187 2022-10-20 01:02:26.000000 django-ipghrms-contract-1.8/contract/forms/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0      195 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.8/contract/forms/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     5690 2023-03-10 10:56:31.000000 django-ipghrms-contract-1.8/contract/forms/__pycache__/cont_form.cpython-310.pyc
--rw-rw-rw-   0        0        0     6246 2022-10-20 01:02:26.000000 django-ipghrms-contract-1.8/contract/forms/__pycache__/cont_form.cpython-37.pyc
--rw-rw-rw-   0        0        0     5285 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.8/contract/forms/__pycache__/cont_form.cpython-39.pyc
--rw-rw-rw-   0        0        0     5623 2023-02-14 06:18:32.000000 django-ipghrms-contract-1.8/contract/forms/__pycache__/man_form.cpython-310.pyc
--rw-rw-rw-   0        0        0     7744 2022-10-20 01:02:26.000000 django-ipghrms-contract-1.8/contract/forms/__pycache__/man_form.cpython-37.pyc
--rw-rw-rw-   0        0        0     6116 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.8/contract/forms/__pycache__/man_form.cpython-39.pyc
--rw-rw-rw-   0        0        0     6033 2023-03-10 10:56:27.000000 django-ipghrms-contract-1.8/contract/forms/cont_form.py
--rw-rw-rw-   0        0        0     7111 2023-02-14 06:18:28.000000 django-ipghrms-contract-1.8/contract/forms/man_form.py
--rw-rw-rw-   0        0        0        0 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.8/contract/forms.py
-drwxrwxrwx   0        0        0        0 2023-06-03 01:26:29.146257 django-ipghrms-contract-1.8/contract/migrations/
--rw-rw-rw-   0        0        0     8714 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.8/contract/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      507 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.8/contract/migrations/0002_rename_section_contract_department_and_more.py
--rw-rw-rw-   0        0        0     3256 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.8/contract/migrations/0003_rename_end_reason_empplacement_reason_and_more.py
--rw-rw-rw-   0        0        0     1093 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.8/contract/migrations/0004_remove_contract_category_remove_contract_de_and_more.py
--rw-rw-rw-   0        0        0      906 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.8/contract/migrations/0005_empplacement_position_alter_empposition_department.py
--rw-rw-rw-   0        0        0      472 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.8/contract/migrations/0006_remove_empsalary_employee_remove_empsalary_position.py
--rw-rw-rw-   0        0        0     1843 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.8/contract/migrations/0007_rename_total_empsalary_amount_and_more.py
--rw-rw-rw-   0        0        0      593 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.8/contract/migrations/0008_empsalary_employee.py
--rw-rw-rw-   0        0        0     1070 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.8/contract/migrations/0009_alter_empsalary_datetime_alter_empsalary_hashed_and_more.py
--rw-rw-rw-   0        0        0     1173 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.8/contract/migrations/0010_category_is_dep_category_is_deputy_category_is_eng_and_more.py
--rw-rw-rw-   0        0        0      456 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.8/contract/migrations/0011_category_is_advisor.py
--rw-rw-rw-   0        0        0      867 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.8/contract/migrations/0012_remove_category_is_advisor_remove_category_is_dep_and_more.py
--rw-rw-rw-   0        0        0      453 2022-12-07 12:36:45.000000 django-ipghrms-contract-1.8/contract/migrations/0013_empposition_is_manager.py
--rw-rw-rw-   0        0        0      648 2022-12-08 01:00:20.000000 django-ipghrms-contract-1.8/contract/migrations/0014_alter_contract_file.py
--rw-rw-rw-   0        0        0     1225 2023-02-02 09:37:19.000000 django-ipghrms-contract-1.8/contract/migrations/0015_organograma.py
--rw-rw-rw-   0        0        0      618 2023-02-02 09:54:33.000000 django-ipghrms-contract-1.8/contract/migrations/0016_alter_organograma_user.py
--rw-rw-rw-   0        0        0      650 2023-02-14 04:12:54.000000 django-ipghrms-contract-1.8/contract/migrations/0017_contract_file_end.py
--rw-rw-rw-   0        0        0     1500 2023-03-10 10:15:51.000000 django-ipghrms-contract-1.8/contract/migrations/0018_empcontracttor.py
--rw-rw-rw-   0        0        0      544 2023-03-10 11:30:11.000000 django-ipghrms-contract-1.8/contract/migrations/0019_alter_empcontracttor_contract.py
--rw-rw-rw-   0        0        0        0 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.8/contract/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-03 01:26:29.222052 django-ipghrms-contract-1.8/contract/migrations/__pycache__/
--rw-rw-rw-   0        0        0     3679 2022-11-07 13:19:39.000000 django-ipghrms-contract-1.8/contract/migrations/__pycache__/0001_initial.cpython-310.pyc
--rw-rw-rw-   0        0        0     3629 2022-10-20 01:03:56.000000 django-ipghrms-contract-1.8/contract/migrations/__pycache__/0001_initial.cpython-37.pyc
--rw-rw-rw-   0        0        0     3683 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.8/contract/migrations/__pycache__/0001_initial.cpython-39.pyc
--rw-rw-rw-   0        0        0      600 2022-11-07 13:19:39.000000 django-ipghrms-contract-1.8/contract/migrations/__pycache__/0002_rename_section_contract_department_and_more.cpython-310.pyc
--rw-rw-rw-   0        0        0      584 2022-10-20 01:03:56.000000 django-ipghrms-contract-1.8/contract/migrations/__pycache__/0002_rename_section_contract_department_and_more.cpython-37.pyc
--rw-rw-rw-   0        0        0      604 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.8/contract/migrations/__pycache__/0002_rename_section_contract_department_and_more.cpython-39.pyc
--rw-rw-rw-   0        0        0     2316 2022-11-07 13:19:39.000000 django-ipghrms-contract-1.8/contract/migrations/__pycache__/0003_rename_end_reason_empplacement_reason_and_more.cpython-310.pyc
--rw-rw-rw-   0        0        0     2302 2022-10-20 01:03:56.000000 django-ipghrms-contract-1.8/contract/migrations/__pycache__/0003_rename_end_reason_empplacement_reason_and_more.cpython-37.pyc
--rw-rw-rw-   0        0        0     2320 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.8/contract/migrations/__pycache__/0003_rename_end_reason_empplacement_reason_and_more.cpython-39.pyc
--rw-rw-rw-   0        0        0      976 2022-11-07 13:19:39.000000 django-ipghrms-contract-1.8/contract/migrations/__pycache__/0004_remove_contract_category_remove_contract_de_and_more.cpython-310.pyc
--rw-rw-rw-   0        0        0      952 2022-10-20 01:03:56.000000 django-ipghrms-contract-1.8/contract/migrations/__pycache__/0004_remove_contract_category_remove_contract_de_and_more.cpython-37.pyc
--rw-rw-rw-   0        0        0      980 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.8/contract/migrations/__pycache__/0004_remove_contract_category_remove_contract_de_and_more.cpython-39.pyc
--rw-rw-rw-   0        0        0     1012 2022-11-07 13:19:39.000000 django-ipghrms-contract-1.8/contract/migrations/__pycache__/0005_empplacement_position_alter_empposition_department.cpython-310.pyc
--rw-rw-rw-   0        0        0      996 2022-10-20 01:03:56.000000 django-ipghrms-contract-1.8/contract/migrations/__pycache__/0005_empplacement_position_alter_empposition_department.cpython-37.pyc
--rw-rw-rw-   0        0        0     1016 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.8/contract/migrations/__pycache__/0005_empplacement_position_alter_empposition_department.cpython-39.pyc
--rw-rw-rw-   0        0        0      620 2022-11-07 13:19:39.000000 django-ipghrms-contract-1.8/contract/migrations/__pycache__/0006_remove_empsalary_employee_remove_empsalary_position.cpython-310.pyc
--rw-rw-rw-   0        0        0      604 2022-10-20 01:03:56.000000 django-ipghrms-contract-1.8/contract/migrations/__pycache__/0006_remove_empsalary_employee_remove_empsalary_position.cpython-37.pyc
--rw-rw-rw-   0        0        0      624 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.8/contract/migrations/__pycache__/0006_remove_empsalary_employee_remove_empsalary_position.cpython-39.pyc
--rw-rw-rw-   0        0        0     1262 2022-11-07 13:19:39.000000 django-ipghrms-contract-1.8/contract/migrations/__pycache__/0007_rename_total_empsalary_amount_and_more.cpython-310.pyc
--rw-rw-rw-   0        0        0     1234 2022-10-20 01:03:56.000000 django-ipghrms-contract-1.8/contract/migrations/__pycache__/0007_rename_total_empsalary_amount_and_more.cpython-37.pyc
--rw-rw-rw-   0        0        0     1266 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.8/contract/migrations/__pycache__/0007_rename_total_empsalary_amount_and_more.cpython-39.pyc
--rw-rw-rw-   0        0        0      786 2022-11-07 13:19:39.000000 django-ipghrms-contract-1.8/contract/migrations/__pycache__/0008_empsalary_employee.cpython-310.pyc
--rw-rw-rw-   0        0        0      772 2022-10-20 01:03:56.000000 django-ipghrms-contract-1.8/contract/migrations/__pycache__/0008_empsalary_employee.cpython-37.pyc
--rw-rw-rw-   0        0        0      790 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.8/contract/migrations/__pycache__/0008_empsalary_employee.cpython-39.pyc
--rw-rw-rw-   0        0        0     1021 2022-11-07 13:19:39.000000 django-ipghrms-contract-1.8/contract/migrations/__pycache__/0009_alter_empsalary_datetime_alter_empsalary_hashed_and_more.cpython-310.pyc
--rw-rw-rw-   0        0        0     1001 2022-10-20 01:03:56.000000 django-ipghrms-contract-1.8/contract/migrations/__pycache__/0009_alter_empsalary_datetime_alter_empsalary_hashed_and_more.cpython-37.pyc
--rw-rw-rw-   0        0        0     1025 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.8/contract/migrations/__pycache__/0009_alter_empsalary_datetime_alter_empsalary_hashed_and_more.cpython-39.pyc
--rw-rw-rw-   0        0        0      867 2022-11-07 13:19:39.000000 django-ipghrms-contract-1.8/contract/migrations/__pycache__/0010_category_is_dep_category_is_deputy_category_is_eng_and_more.cpython-310.pyc
--rw-rw-rw-   0        0        0      845 2022-10-20 01:03:56.000000 django-ipghrms-contract-1.8/contract/migrations/__pycache__/0010_category_is_dep_category_is_deputy_category_is_eng_and_more.cpython-37.pyc
--rw-rw-rw-   0        0        0      871 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.8/contract/migrations/__pycache__/0010_category_is_dep_category_is_deputy_category_is_eng_and_more.cpython-39.pyc
--rw-rw-rw-   0        0        0      650 2022-11-07 13:19:39.000000 django-ipghrms-contract-1.8/contract/migrations/__pycache__/0011_category_is_advisor.cpython-310.pyc
--rw-rw-rw-   0        0        0      636 2022-10-20 01:03:56.000000 django-ipghrms-contract-1.8/contract/migrations/__pycache__/0011_category_is_advisor.cpython-37.pyc
--rw-rw-rw-   0        0        0      654 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.8/contract/migrations/__pycache__/0011_category_is_advisor.cpython-39.pyc
--rw-rw-rw-   0        0        0      715 2022-11-07 13:19:39.000000 django-ipghrms-contract-1.8/contract/migrations/__pycache__/0012_remove_category_is_advisor_remove_category_is_dep_and_more.cpython-310.pyc
--rw-rw-rw-   0        0        0      691 2022-10-20 01:03:56.000000 django-ipghrms-contract-1.8/contract/migrations/__pycache__/0012_remove_category_is_advisor_remove_category_is_dep_and_more.cpython-37.pyc
--rw-rw-rw-   0        0        0      719 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.8/contract/migrations/__pycache__/0012_remove_category_is_advisor_remove_category_is_dep_and_more.cpython-39.pyc
--rw-rw-rw-   0        0        0      635 2022-12-07 12:36:50.000000 django-ipghrms-contract-1.8/contract/migrations/__pycache__/0013_empposition_is_manager.cpython-310.pyc
--rw-rw-rw-   0        0        0      858 2022-12-08 01:00:27.000000 django-ipghrms-contract-1.8/contract/migrations/__pycache__/0014_alter_contract_file.cpython-310.pyc
--rw-rw-rw-   0        0        0     1304 2023-02-02 09:37:42.000000 django-ipghrms-contract-1.8/contract/migrations/__pycache__/0015_organograma.cpython-310.pyc
--rw-rw-rw-   0        0        0      790 2023-02-02 09:54:52.000000 django-ipghrms-contract-1.8/contract/migrations/__pycache__/0016_alter_organograma_user.cpython-310.pyc
--rw-rw-rw-   0        0        0      858 2023-02-14 04:12:59.000000 django-ipghrms-contract-1.8/contract/migrations/__pycache__/0017_contract_file_end.cpython-310.pyc
--rw-rw-rw-   0        0        0     1370 2023-03-10 10:16:01.000000 django-ipghrms-contract-1.8/contract/migrations/__pycache__/0018_empcontracttor.cpython-310.pyc
--rw-rw-rw-   0        0        0      743 2023-03-10 11:30:16.000000 django-ipghrms-contract-1.8/contract/migrations/__pycache__/0019_alter_empcontracttor_contract.cpython-310.pyc
--rw-rw-rw-   0        0        0      148 2022-11-07 13:19:39.000000 django-ipghrms-contract-1.8/contract/migrations/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      146 2022-10-20 01:03:56.000000 django-ipghrms-contract-1.8/contract/migrations/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0      154 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.8/contract/migrations/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     8503 2023-03-10 11:29:59.000000 django-ipghrms-contract-1.8/contract/models.py
--rw-rw-rw-   0        0        0      347 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.8/contract/signals.py
-drwxrwxrwx   0        0        0        0 2023-06-03 01:26:29.077300 django-ipghrms-contract-1.8/contract/templates/
-drwxrwxrwx   0        0        0        0 2023-06-03 01:26:29.233021 django-ipghrms-contract-1.8/contract/templates/contract/
--rw-rw-rw-   0        0        0     2432 2023-02-07 05:32:28.000000 django-ipghrms-contract-1.8/contract/templates/contract/cont_hist.html
--rw-rw-rw-   0        0        0     3341 2023-02-21 06:26:34.000000 django-ipghrms-contract-1.8/contract/templates/contract/dash.html
--rw-rw-rw-   0        0        0     9466 2023-06-02 20:55:42.000000 django-ipghrms-contract-1.8/contract/templates/contract/detail.html
--rw-rw-rw-   0        0        0     1883 2023-02-09 05:55:30.000000 django-ipghrms-contract-1.8/contract/templates/contract/form.html
--rw-rw-rw-   0        0        0     1298 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.8/contract/templates/contract/form_upgrade.html
--rw-rw-rw-   0        0        0     2401 2023-03-10 12:13:13.000000 django-ipghrms-contract-1.8/contract/templates/contract/list.html
--rw-rw-rw-   0        0        0     1732 2023-02-07 06:16:20.000000 django-ipghrms-contract-1.8/contract/templates/contract/nocont_list.html
-drwxrwxrwx   0        0        0        0 2023-06-03 01:26:29.241998 django-ipghrms-contract-1.8/contract/templates/contract_chart/
--rw-rw-rw-   0        0        0     2094 2023-02-13 02:45:01.000000 django-ipghrms-contract-1.8/contract/templates/contract_chart/cont_cat.js
--rw-rw-rw-   0        0        0     1475 2023-02-13 02:45:06.000000 django-ipghrms-contract-1.8/contract/templates/contract_chart/cont_cat2.js
--rw-rw-rw-   0        0        0     3911 2023-02-13 02:26:25.000000 django-ipghrms-contract-1.8/contract/templates/contract_chart/cont_chart.html
--rw-rw-rw-   0        0        0      754 2022-11-16 12:19:49.000000 django-ipghrms-contract-1.8/contract/templates/contract_chart/cont_pos.js
--rw-rw-rw-   0        0        0     1895 2023-01-22 14:24:35.000000 django-ipghrms-contract-1.8/contract/templates/contract_chart/cont_pos2.js
--rw-rw-rw-   0        0        0     1575 2023-02-14 06:05:26.000000 django-ipghrms-contract-1.8/contract/templates/contract_chart/cont_type.js
-drwxrwxrwx   0        0        0        0 2023-06-03 01:26:29.251972 django-ipghrms-contract-1.8/contract/templates/manager/
--rw-rw-rw-   0        0        0     4147 2023-02-14 06:24:14.000000 django-ipghrms-contract-1.8/contract/templates/manager/dash.html
--rw-rw-rw-   0        0        0        0 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.8/contract/templates/manager/detail.html
--rw-rw-rw-   0        0        0     1323 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.8/contract/templates/manager/form.html
--rw-rw-rw-   0        0        0        0 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.8/contract/templates/manager/list.html
--rw-rw-rw-   0        0        0     6181 2023-02-20 12:51:08.000000 django-ipghrms-contract-1.8/contract/templates/manager/man_de.html
--rw-rw-rw-   0        0        0     6248 2023-02-20 12:51:52.000000 django-ipghrms-contract-1.8/contract/templates/manager/man_dep.html
--rw-rw-rw-   0        0        0     4711 2023-02-20 12:43:03.000000 django-ipghrms-contract-1.8/contract/templates/manager/man_hist.html
--rw-rw-rw-   0        0        0     6225 2023-02-20 12:51:02.000000 django-ipghrms-contract-1.8/contract/templates/manager/man_unit.html
-drwxrwxrwx   0        0        0        0 2023-06-03 01:26:29.255961 django-ipghrms-contract-1.8/contract/templates/placement/
--rw-rw-rw-   0        0        0     5315 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.8/contract/templates/placement/detail.html
--rw-rw-rw-   0        0        0     1367 2023-02-09 05:41:03.000000 django-ipghrms-contract-1.8/contract/templates/placement/form.html
--rw-rw-rw-   0        0        0     2794 2022-11-16 15:16:32.000000 django-ipghrms-contract-1.8/contract/templates/placement/list.html
-drwxrwxrwx   0        0        0        0 2023-06-03 01:26:29.261945 django-ipghrms-contract-1.8/contract/templates/salary/
--rw-rw-rw-   0        0        0     5745 2023-02-08 08:06:21.000000 django-ipghrms-contract-1.8/contract/templates/salary/detail.html
--rw-rw-rw-   0        0        0     1881 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.8/contract/templates/salary/form.html
--rw-rw-rw-   0        0        0     2663 2023-02-08 08:14:44.000000 django-ipghrms-contract-1.8/contract/templates/salary/list.html
--rw-rw-rw-   0        0        0     1955 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.8/contract/templates/salary/no_salary_list.html
-drwxrwxrwx   0        0        0        0 2023-06-03 01:26:29.263939 django-ipghrms-contract-1.8/contract/templates/tor/
--rw-rw-rw-   0        0        0     1697 2023-03-10 11:22:43.000000 django-ipghrms-contract-1.8/contract/templates/tor/form.html
--rw-rw-rw-   0        0        0     4393 2023-03-10 12:15:09.000000 django-ipghrms-contract-1.8/contract/templates/tor/list.html
--rw-rw-rw-   0        0        0       60 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.8/contract/tests.py
--rw-rw-rw-   0        0        0     3853 2023-06-02 20:58:57.000000 django-ipghrms-contract-1.8/contract/urls.py
--rw-rw-rw-   0        0        0     1257 2023-01-25 03:51:54.000000 django-ipghrms-contract-1.8/contract/urls_man.py
-drwxrwxrwx   0        0        0        0 2023-06-03 01:26:29.273914 django-ipghrms-contract-1.8/contract/views/
--rw-rw-rw-   0        0        0      168 2023-03-10 10:19:39.000000 django-ipghrms-contract-1.8/contract/views/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-03 01:26:29.311392 django-ipghrms-contract-1.8/contract/views/__pycache__/
--rw-rw-rw-   0        0        0      287 2023-03-10 10:19:44.000000 django-ipghrms-contract-1.8/contract/views/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      272 2022-10-20 01:02:26.000000 django-ipghrms-contract-1.8/contract/views/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0      280 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.8/contract/views/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     3405 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.8/contract/views/__pycache__/contract.cpython-39.pyc
--rw-rw-rw-   0        0        0     4717 2023-02-23 05:55:32.000000 django-ipghrms-contract-1.8/contract/views/__pycache__/contract_m.cpython-310.pyc
--rw-rw-rw-   0        0        0     4356 2022-10-20 01:02:26.000000 django-ipghrms-contract-1.8/contract/views/__pycache__/contract_m.cpython-37.pyc
--rw-rw-rw-   0        0        0     4237 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.8/contract/views/__pycache__/contract_m.cpython-39.pyc
--rw-rw-rw-   0        0        0     5053 2023-02-21 00:08:06.000000 django-ipghrms-contract-1.8/contract/views/__pycache__/contract_v.cpython-310.pyc
--rw-rw-rw-   0        0        0     3586 2022-11-05 14:50:10.000000 django-ipghrms-contract-1.8/contract/views/__pycache__/contract_v.cpython-37.pyc
--rw-rw-rw-   0        0        0     3615 2022-11-04 05:28:45.000000 django-ipghrms-contract-1.8/contract/views/__pycache__/contract_v.cpython-39.pyc
--rw-rw-rw-   0        0        0      137 2022-11-16 07:11:52.000000 django-ipghrms-contract-1.8/contract/views/__pycache__/history.cpython-310.pyc
--rw-rw-rw-   0        0        0    14124 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.8/contract/views/__pycache__/manager.cpython-39.pyc
--rw-rw-rw-   0        0        0     8332 2023-03-17 02:59:45.000000 django-ipghrms-contract-1.8/contract/views/__pycache__/manager_m.cpython-310.pyc
--rw-rw-rw-   0        0        0     9697 2022-10-20 01:02:26.000000 django-ipghrms-contract-1.8/contract/views/__pycache__/manager_m.cpython-37.pyc
--rw-rw-rw-   0        0        0     9001 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.8/contract/views/__pycache__/manager_m.cpython-39.pyc
--rw-rw-rw-   0        0        0     4564 2023-03-08 09:45:19.000000 django-ipghrms-contract-1.8/contract/views/__pycache__/manager_v.cpython-310.pyc
--rw-rw-rw-   0        0        0     3263 2022-10-20 01:02:26.000000 django-ipghrms-contract-1.8/contract/views/__pycache__/manager_v.cpython-37.pyc
--rw-rw-rw-   0        0        0     3136 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.8/contract/views/__pycache__/manager_v.cpython-39.pyc
--rw-rw-rw-   0        0        0     2915 2023-02-09 05:46:27.000000 django-ipghrms-contract-1.8/contract/views/__pycache__/placement.cpython-310.pyc
--rw-rw-rw-   0        0        0     2885 2022-10-20 01:02:26.000000 django-ipghrms-contract-1.8/contract/views/__pycache__/placement.cpython-37.pyc
--rw-rw-rw-   0        0        0     2913 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.8/contract/views/__pycache__/placement.cpython-39.pyc
--rw-rw-rw-   0        0        0     3406 2023-02-23 06:03:20.000000 django-ipghrms-contract-1.8/contract/views/__pycache__/sallary.cpython-310.pyc
--rw-rw-rw-   0        0        0     3265 2022-10-20 01:02:26.000000 django-ipghrms-contract-1.8/contract/views/__pycache__/sallary.cpython-37.pyc
--rw-rw-rw-   0        0        0     3220 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.8/contract/views/__pycache__/sallary.cpython-39.pyc
--rw-rw-rw-   0        0        0     3057 2023-03-10 12:12:04.000000 django-ipghrms-contract-1.8/contract/views/__pycache__/tor.cpython-310.pyc
--rw-rw-rw-   0        0        0     5887 2023-02-23 05:55:30.000000 django-ipghrms-contract-1.8/contract/views/contract_m.py
--rw-rw-rw-   0        0        0     5711 2023-06-02 20:57:25.000000 django-ipghrms-contract-1.8/contract/views/contract_v.py
--rw-rw-rw-   0        0        0    13856 2023-03-16 00:00:39.000000 django-ipghrms-contract-1.8/contract/views/manager_m.py
--rw-rw-rw-   0        0        0     5350 2023-03-08 09:45:16.000000 django-ipghrms-contract-1.8/contract/views/manager_v.py
--rw-rw-rw-   0        0        0     9309 2023-06-02 20:58:09.000000 django-ipghrms-contract-1.8/contract/views/placement.py
--rw-rw-rw-   0        0        0     4123 2023-02-23 06:03:18.000000 django-ipghrms-contract-1.8/contract/views/sallary.py
--rw-rw-rw-   0        0        0     4080 2023-03-10 12:12:04.000000 django-ipghrms-contract-1.8/contract/views/tor.py
--rw-rw-rw-   0        0        0       63 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.8/contract/views.py
-drwxrwxrwx   0        0        0        0 2023-06-03 01:26:29.323360 django-ipghrms-contract-1.8/django_ipghrms_contract.egg-info/
--rw-rw-rw-   0        0        0     1158 2023-06-03 01:26:28.000000 django-ipghrms-contract-1.8/django_ipghrms_contract.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     9239 2023-06-03 01:26:29.000000 django-ipghrms-contract-1.8/django_ipghrms_contract.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 01:26:28.000000 django-ipghrms-contract-1.8/django_ipghrms_contract.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 01:26:28.000000 django-ipghrms-contract-1.8/django_ipghrms_contract.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      511 2023-06-03 01:26:29.326467 django-ipghrms-contract-1.8/setup.cfg
--rw-rw-rw-   0        0        0       39 2023-03-22 07:44:49.000000 django-ipghrms-contract-1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 02:43:43.206915 django-ipghrms-contract-1.9/
+-rw-rw-rw-   0        0        0     1068 2023-03-22 07:40:25.000000 django-ipghrms-contract-1.9/LICENSE
+-rw-rw-rw-   0        0        0      222 2023-03-27 14:21:27.000000 django-ipghrms-contract-1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      972 2023-06-03 02:43:43.206915 django-ipghrms-contract-1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      503 2023-03-27 01:42:56.000000 django-ipghrms-contract-1.9/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-03 02:43:41.831451 django-ipghrms-contract-1.9/contract/
+-rw-rw-rw-   0        0        0        0 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.9/contract/__init__.py
+-rw-rw-rw-   0        0        0     2240 2023-06-02 20:59:28.000000 django-ipghrms-contract-1.9/contract/admin.py
+drwxrwxrwx   0        0        0        0 2023-06-03 02:43:41.872683 django-ipghrms-contract-1.9/contract/api/
+drwxrwxrwx   0        0        0        0 2023-06-03 02:43:41.879742 django-ipghrms-contract-1.9/contract/api/__pycache__/
+-rw-rw-rw-   0        0        0      405 2023-01-22 14:24:18.000000 django-ipghrms-contract-1.9/contract/api/__pycache__/urls.cpython-310.pyc
+-rw-rw-rw-   0        0        0      348 2022-11-05 14:50:10.000000 django-ipghrms-contract-1.9/contract/api/__pycache__/urls.cpython-37.pyc
+-rw-rw-rw-   0        0        0     2913 2023-03-12 11:13:58.000000 django-ipghrms-contract-1.9/contract/api/__pycache__/views.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2464 2022-11-05 14:50:10.000000 django-ipghrms-contract-1.9/contract/api/__pycache__/views.cpython-37.pyc
+-rw-rw-rw-   0        0        0      262 2023-01-22 14:24:15.000000 django-ipghrms-contract-1.9/contract/api/urls.py
+-rw-rw-rw-   0        0        0     2564 2023-03-12 11:13:55.000000 django-ipghrms-contract-1.9/contract/api/views.py
+-rw-rw-rw-   0        0        0      132 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.9/contract/apps.py
+drwxrwxrwx   0        0        0        0 2023-06-03 02:43:41.958081 django-ipghrms-contract-1.9/contract/forms/
+-rw-rw-rw-   0        0        0       48 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.9/contract/forms/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-03 02:43:41.985333 django-ipghrms-contract-1.9/contract/forms/__pycache__/
+-rw-rw-rw-   0        0        0      189 2022-11-07 13:19:37.000000 django-ipghrms-contract-1.9/contract/forms/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      187 2022-10-20 01:02:26.000000 django-ipghrms-contract-1.9/contract/forms/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0      195 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.9/contract/forms/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     5690 2023-03-10 10:56:31.000000 django-ipghrms-contract-1.9/contract/forms/__pycache__/cont_form.cpython-310.pyc
+-rw-rw-rw-   0        0        0     6246 2022-10-20 01:02:26.000000 django-ipghrms-contract-1.9/contract/forms/__pycache__/cont_form.cpython-37.pyc
+-rw-rw-rw-   0        0        0     5285 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.9/contract/forms/__pycache__/cont_form.cpython-39.pyc
+-rw-rw-rw-   0        0        0     5623 2023-02-14 06:18:32.000000 django-ipghrms-contract-1.9/contract/forms/__pycache__/man_form.cpython-310.pyc
+-rw-rw-rw-   0        0        0     7744 2022-10-20 01:02:26.000000 django-ipghrms-contract-1.9/contract/forms/__pycache__/man_form.cpython-37.pyc
+-rw-rw-rw-   0        0        0     6116 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.9/contract/forms/__pycache__/man_form.cpython-39.pyc
+-rw-rw-rw-   0        0        0     6033 2023-03-10 10:56:27.000000 django-ipghrms-contract-1.9/contract/forms/cont_form.py
+-rw-rw-rw-   0        0        0     7111 2023-02-14 06:18:28.000000 django-ipghrms-contract-1.9/contract/forms/man_form.py
+-rw-rw-rw-   0        0        0        0 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.9/contract/forms.py
+drwxrwxrwx   0        0        0        0 2023-06-03 02:43:42.106094 django-ipghrms-contract-1.9/contract/migrations/
+-rw-rw-rw-   0        0        0     8714 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.9/contract/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      507 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.9/contract/migrations/0002_rename_section_contract_department_and_more.py
+-rw-rw-rw-   0        0        0     3256 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.9/contract/migrations/0003_rename_end_reason_empplacement_reason_and_more.py
+-rw-rw-rw-   0        0        0     1093 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.9/contract/migrations/0004_remove_contract_category_remove_contract_de_and_more.py
+-rw-rw-rw-   0        0        0      906 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.9/contract/migrations/0005_empplacement_position_alter_empposition_department.py
+-rw-rw-rw-   0        0        0      472 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.9/contract/migrations/0006_remove_empsalary_employee_remove_empsalary_position.py
+-rw-rw-rw-   0        0        0     1843 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.9/contract/migrations/0007_rename_total_empsalary_amount_and_more.py
+-rw-rw-rw-   0        0        0      593 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.9/contract/migrations/0008_empsalary_employee.py
+-rw-rw-rw-   0        0        0     1070 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.9/contract/migrations/0009_alter_empsalary_datetime_alter_empsalary_hashed_and_more.py
+-rw-rw-rw-   0        0        0     1173 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.9/contract/migrations/0010_category_is_dep_category_is_deputy_category_is_eng_and_more.py
+-rw-rw-rw-   0        0        0      456 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.9/contract/migrations/0011_category_is_advisor.py
+-rw-rw-rw-   0        0        0      867 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.9/contract/migrations/0012_remove_category_is_advisor_remove_category_is_dep_and_more.py
+-rw-rw-rw-   0        0        0      453 2022-12-07 12:36:45.000000 django-ipghrms-contract-1.9/contract/migrations/0013_empposition_is_manager.py
+-rw-rw-rw-   0        0        0      648 2022-12-08 01:00:20.000000 django-ipghrms-contract-1.9/contract/migrations/0014_alter_contract_file.py
+-rw-rw-rw-   0        0        0     1225 2023-02-02 09:37:19.000000 django-ipghrms-contract-1.9/contract/migrations/0015_organograma.py
+-rw-rw-rw-   0        0        0      618 2023-02-02 09:54:33.000000 django-ipghrms-contract-1.9/contract/migrations/0016_alter_organograma_user.py
+-rw-rw-rw-   0        0        0      650 2023-02-14 04:12:54.000000 django-ipghrms-contract-1.9/contract/migrations/0017_contract_file_end.py
+-rw-rw-rw-   0        0        0     1500 2023-03-10 10:15:51.000000 django-ipghrms-contract-1.9/contract/migrations/0018_empcontracttor.py
+-rw-rw-rw-   0        0        0      544 2023-03-10 11:30:11.000000 django-ipghrms-contract-1.9/contract/migrations/0019_alter_empcontracttor_contract.py
+-rw-rw-rw-   0        0        0        0 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.9/contract/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-03 02:43:42.279810 django-ipghrms-contract-1.9/contract/migrations/__pycache__/
+-rw-rw-rw-   0        0        0     3679 2022-11-07 13:19:39.000000 django-ipghrms-contract-1.9/contract/migrations/__pycache__/0001_initial.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3629 2022-10-20 01:03:56.000000 django-ipghrms-contract-1.9/contract/migrations/__pycache__/0001_initial.cpython-37.pyc
+-rw-rw-rw-   0        0        0     3683 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.9/contract/migrations/__pycache__/0001_initial.cpython-39.pyc
+-rw-rw-rw-   0        0        0      600 2022-11-07 13:19:39.000000 django-ipghrms-contract-1.9/contract/migrations/__pycache__/0002_rename_section_contract_department_and_more.cpython-310.pyc
+-rw-rw-rw-   0        0        0      584 2022-10-20 01:03:56.000000 django-ipghrms-contract-1.9/contract/migrations/__pycache__/0002_rename_section_contract_department_and_more.cpython-37.pyc
+-rw-rw-rw-   0        0        0      604 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.9/contract/migrations/__pycache__/0002_rename_section_contract_department_and_more.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2316 2022-11-07 13:19:39.000000 django-ipghrms-contract-1.9/contract/migrations/__pycache__/0003_rename_end_reason_empplacement_reason_and_more.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2302 2022-10-20 01:03:56.000000 django-ipghrms-contract-1.9/contract/migrations/__pycache__/0003_rename_end_reason_empplacement_reason_and_more.cpython-37.pyc
+-rw-rw-rw-   0        0        0     2320 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.9/contract/migrations/__pycache__/0003_rename_end_reason_empplacement_reason_and_more.cpython-39.pyc
+-rw-rw-rw-   0        0        0      976 2022-11-07 13:19:39.000000 django-ipghrms-contract-1.9/contract/migrations/__pycache__/0004_remove_contract_category_remove_contract_de_and_more.cpython-310.pyc
+-rw-rw-rw-   0        0        0      952 2022-10-20 01:03:56.000000 django-ipghrms-contract-1.9/contract/migrations/__pycache__/0004_remove_contract_category_remove_contract_de_and_more.cpython-37.pyc
+-rw-rw-rw-   0        0        0      980 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.9/contract/migrations/__pycache__/0004_remove_contract_category_remove_contract_de_and_more.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1012 2022-11-07 13:19:39.000000 django-ipghrms-contract-1.9/contract/migrations/__pycache__/0005_empplacement_position_alter_empposition_department.cpython-310.pyc
+-rw-rw-rw-   0        0        0      996 2022-10-20 01:03:56.000000 django-ipghrms-contract-1.9/contract/migrations/__pycache__/0005_empplacement_position_alter_empposition_department.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1016 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.9/contract/migrations/__pycache__/0005_empplacement_position_alter_empposition_department.cpython-39.pyc
+-rw-rw-rw-   0        0        0      620 2022-11-07 13:19:39.000000 django-ipghrms-contract-1.9/contract/migrations/__pycache__/0006_remove_empsalary_employee_remove_empsalary_position.cpython-310.pyc
+-rw-rw-rw-   0        0        0      604 2022-10-20 01:03:56.000000 django-ipghrms-contract-1.9/contract/migrations/__pycache__/0006_remove_empsalary_employee_remove_empsalary_position.cpython-37.pyc
+-rw-rw-rw-   0        0        0      624 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.9/contract/migrations/__pycache__/0006_remove_empsalary_employee_remove_empsalary_position.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1262 2022-11-07 13:19:39.000000 django-ipghrms-contract-1.9/contract/migrations/__pycache__/0007_rename_total_empsalary_amount_and_more.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1234 2022-10-20 01:03:56.000000 django-ipghrms-contract-1.9/contract/migrations/__pycache__/0007_rename_total_empsalary_amount_and_more.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1266 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.9/contract/migrations/__pycache__/0007_rename_total_empsalary_amount_and_more.cpython-39.pyc
+-rw-rw-rw-   0        0        0      786 2022-11-07 13:19:39.000000 django-ipghrms-contract-1.9/contract/migrations/__pycache__/0008_empsalary_employee.cpython-310.pyc
+-rw-rw-rw-   0        0        0      772 2022-10-20 01:03:56.000000 django-ipghrms-contract-1.9/contract/migrations/__pycache__/0008_empsalary_employee.cpython-37.pyc
+-rw-rw-rw-   0        0        0      790 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.9/contract/migrations/__pycache__/0008_empsalary_employee.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1021 2022-11-07 13:19:39.000000 django-ipghrms-contract-1.9/contract/migrations/__pycache__/0009_alter_empsalary_datetime_alter_empsalary_hashed_and_more.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1001 2022-10-20 01:03:56.000000 django-ipghrms-contract-1.9/contract/migrations/__pycache__/0009_alter_empsalary_datetime_alter_empsalary_hashed_and_more.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1025 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.9/contract/migrations/__pycache__/0009_alter_empsalary_datetime_alter_empsalary_hashed_and_more.cpython-39.pyc
+-rw-rw-rw-   0        0        0      867 2022-11-07 13:19:39.000000 django-ipghrms-contract-1.9/contract/migrations/__pycache__/0010_category_is_dep_category_is_deputy_category_is_eng_and_more.cpython-310.pyc
+-rw-rw-rw-   0        0        0      845 2022-10-20 01:03:56.000000 django-ipghrms-contract-1.9/contract/migrations/__pycache__/0010_category_is_dep_category_is_deputy_category_is_eng_and_more.cpython-37.pyc
+-rw-rw-rw-   0        0        0      871 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.9/contract/migrations/__pycache__/0010_category_is_dep_category_is_deputy_category_is_eng_and_more.cpython-39.pyc
+-rw-rw-rw-   0        0        0      650 2022-11-07 13:19:39.000000 django-ipghrms-contract-1.9/contract/migrations/__pycache__/0011_category_is_advisor.cpython-310.pyc
+-rw-rw-rw-   0        0        0      636 2022-10-20 01:03:56.000000 django-ipghrms-contract-1.9/contract/migrations/__pycache__/0011_category_is_advisor.cpython-37.pyc
+-rw-rw-rw-   0        0        0      654 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.9/contract/migrations/__pycache__/0011_category_is_advisor.cpython-39.pyc
+-rw-rw-rw-   0        0        0      715 2022-11-07 13:19:39.000000 django-ipghrms-contract-1.9/contract/migrations/__pycache__/0012_remove_category_is_advisor_remove_category_is_dep_and_more.cpython-310.pyc
+-rw-rw-rw-   0        0        0      691 2022-10-20 01:03:56.000000 django-ipghrms-contract-1.9/contract/migrations/__pycache__/0012_remove_category_is_advisor_remove_category_is_dep_and_more.cpython-37.pyc
+-rw-rw-rw-   0        0        0      719 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.9/contract/migrations/__pycache__/0012_remove_category_is_advisor_remove_category_is_dep_and_more.cpython-39.pyc
+-rw-rw-rw-   0        0        0      635 2022-12-07 12:36:50.000000 django-ipghrms-contract-1.9/contract/migrations/__pycache__/0013_empposition_is_manager.cpython-310.pyc
+-rw-rw-rw-   0        0        0      858 2022-12-08 01:00:27.000000 django-ipghrms-contract-1.9/contract/migrations/__pycache__/0014_alter_contract_file.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1304 2023-02-02 09:37:42.000000 django-ipghrms-contract-1.9/contract/migrations/__pycache__/0015_organograma.cpython-310.pyc
+-rw-rw-rw-   0        0        0      790 2023-02-02 09:54:52.000000 django-ipghrms-contract-1.9/contract/migrations/__pycache__/0016_alter_organograma_user.cpython-310.pyc
+-rw-rw-rw-   0        0        0      858 2023-02-14 04:12:59.000000 django-ipghrms-contract-1.9/contract/migrations/__pycache__/0017_contract_file_end.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1370 2023-03-10 10:16:01.000000 django-ipghrms-contract-1.9/contract/migrations/__pycache__/0018_empcontracttor.cpython-310.pyc
+-rw-rw-rw-   0        0        0      743 2023-03-10 11:30:16.000000 django-ipghrms-contract-1.9/contract/migrations/__pycache__/0019_alter_empcontracttor_contract.cpython-310.pyc
+-rw-rw-rw-   0        0        0      148 2022-11-07 13:19:39.000000 django-ipghrms-contract-1.9/contract/migrations/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      146 2022-10-20 01:03:56.000000 django-ipghrms-contract-1.9/contract/migrations/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0      154 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.9/contract/migrations/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     8503 2023-03-10 11:29:59.000000 django-ipghrms-contract-1.9/contract/models.py
+-rw-rw-rw-   0        0        0      347 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.9/contract/signals.py
+drwxrwxrwx   0        0        0        0 2023-06-03 02:43:41.705126 django-ipghrms-contract-1.9/contract/templates/
+drwxrwxrwx   0        0        0        0 2023-06-03 02:43:42.352156 django-ipghrms-contract-1.9/contract/templates/contract/
+-rw-rw-rw-   0        0        0     2432 2023-02-07 05:32:28.000000 django-ipghrms-contract-1.9/contract/templates/contract/cont_hist.html
+-rw-rw-rw-   0        0        0     3341 2023-02-21 06:26:34.000000 django-ipghrms-contract-1.9/contract/templates/contract/dash.html
+-rw-rw-rw-   0        0        0     9466 2023-06-02 20:55:42.000000 django-ipghrms-contract-1.9/contract/templates/contract/detail.html
+-rw-rw-rw-   0        0        0     1883 2023-02-09 05:55:30.000000 django-ipghrms-contract-1.9/contract/templates/contract/form.html
+-rw-rw-rw-   0        0        0     1298 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.9/contract/templates/contract/form_upgrade.html
+-rw-rw-rw-   0        0        0     2401 2023-03-10 12:13:13.000000 django-ipghrms-contract-1.9/contract/templates/contract/list.html
+-rw-rw-rw-   0        0        0     1732 2023-02-07 06:16:20.000000 django-ipghrms-contract-1.9/contract/templates/contract/nocont_list.html
+drwxrwxrwx   0        0        0        0 2023-06-03 02:43:42.405266 django-ipghrms-contract-1.9/contract/templates/contract_chart/
+-rw-rw-rw-   0        0        0     2094 2023-02-13 02:45:01.000000 django-ipghrms-contract-1.9/contract/templates/contract_chart/cont_cat.js
+-rw-rw-rw-   0        0        0     1475 2023-02-13 02:45:06.000000 django-ipghrms-contract-1.9/contract/templates/contract_chart/cont_cat2.js
+-rw-rw-rw-   0        0        0     3911 2023-02-13 02:26:25.000000 django-ipghrms-contract-1.9/contract/templates/contract_chart/cont_chart.html
+-rw-rw-rw-   0        0        0      754 2022-11-16 12:19:49.000000 django-ipghrms-contract-1.9/contract/templates/contract_chart/cont_pos.js
+-rw-rw-rw-   0        0        0     1895 2023-01-22 14:24:35.000000 django-ipghrms-contract-1.9/contract/templates/contract_chart/cont_pos2.js
+-rw-rw-rw-   0        0        0     1575 2023-02-14 06:05:26.000000 django-ipghrms-contract-1.9/contract/templates/contract_chart/cont_type.js
+drwxrwxrwx   0        0        0        0 2023-06-03 02:43:42.880531 django-ipghrms-contract-1.9/contract/templates/manager/
+-rw-rw-rw-   0        0        0     4147 2023-02-14 06:24:14.000000 django-ipghrms-contract-1.9/contract/templates/manager/dash.html
+-rw-rw-rw-   0        0        0        0 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.9/contract/templates/manager/detail.html
+-rw-rw-rw-   0        0        0     1323 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.9/contract/templates/manager/form.html
+-rw-rw-rw-   0        0        0        0 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.9/contract/templates/manager/list.html
+-rw-rw-rw-   0        0        0     6181 2023-02-20 12:51:08.000000 django-ipghrms-contract-1.9/contract/templates/manager/man_de.html
+-rw-rw-rw-   0        0        0     6248 2023-02-20 12:51:52.000000 django-ipghrms-contract-1.9/contract/templates/manager/man_dep.html
+-rw-rw-rw-   0        0        0     4711 2023-02-20 12:43:03.000000 django-ipghrms-contract-1.9/contract/templates/manager/man_hist.html
+-rw-rw-rw-   0        0        0     6225 2023-02-20 12:51:02.000000 django-ipghrms-contract-1.9/contract/templates/manager/man_unit.html
+drwxrwxrwx   0        0        0        0 2023-06-03 02:43:42.903661 django-ipghrms-contract-1.9/contract/templates/placement/
+-rw-rw-rw-   0        0        0     5315 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.9/contract/templates/placement/detail.html
+-rw-rw-rw-   0        0        0     1367 2023-02-09 05:41:03.000000 django-ipghrms-contract-1.9/contract/templates/placement/form.html
+-rw-rw-rw-   0        0        0     2794 2022-11-16 15:16:32.000000 django-ipghrms-contract-1.9/contract/templates/placement/list.html
+drwxrwxrwx   0        0        0        0 2023-06-03 02:43:42.959306 django-ipghrms-contract-1.9/contract/templates/salary/
+-rw-rw-rw-   0        0        0     5745 2023-02-08 08:06:21.000000 django-ipghrms-contract-1.9/contract/templates/salary/detail.html
+-rw-rw-rw-   0        0        0     1881 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.9/contract/templates/salary/form.html
+-rw-rw-rw-   0        0        0     2663 2023-02-08 08:14:44.000000 django-ipghrms-contract-1.9/contract/templates/salary/list.html
+-rw-rw-rw-   0        0        0     1955 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.9/contract/templates/salary/no_salary_list.html
+drwxrwxrwx   0        0        0        0 2023-06-03 02:43:42.995242 django-ipghrms-contract-1.9/contract/templates/tor/
+-rw-rw-rw-   0        0        0     1697 2023-03-10 11:22:43.000000 django-ipghrms-contract-1.9/contract/templates/tor/form.html
+-rw-rw-rw-   0        0        0     4393 2023-03-10 12:15:09.000000 django-ipghrms-contract-1.9/contract/templates/tor/list.html
+-rw-rw-rw-   0        0        0       60 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.9/contract/tests.py
+-rw-rw-rw-   0        0        0     3853 2023-06-02 20:58:57.000000 django-ipghrms-contract-1.9/contract/urls.py
+-rw-rw-rw-   0        0        0     1257 2023-01-25 03:51:54.000000 django-ipghrms-contract-1.9/contract/urls_man.py
+drwxrwxrwx   0        0        0        0 2023-06-03 02:43:43.130659 django-ipghrms-contract-1.9/contract/views/
+-rw-rw-rw-   0        0        0      168 2023-03-10 10:19:39.000000 django-ipghrms-contract-1.9/contract/views/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-03 02:43:43.187934 django-ipghrms-contract-1.9/contract/views/__pycache__/
+-rw-rw-rw-   0        0        0      287 2023-03-10 10:19:44.000000 django-ipghrms-contract-1.9/contract/views/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      272 2022-10-20 01:02:26.000000 django-ipghrms-contract-1.9/contract/views/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0      280 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.9/contract/views/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3405 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.9/contract/views/__pycache__/contract.cpython-39.pyc
+-rw-rw-rw-   0        0        0     4717 2023-02-23 05:55:32.000000 django-ipghrms-contract-1.9/contract/views/__pycache__/contract_m.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4356 2022-10-20 01:02:26.000000 django-ipghrms-contract-1.9/contract/views/__pycache__/contract_m.cpython-37.pyc
+-rw-rw-rw-   0        0        0     4237 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.9/contract/views/__pycache__/contract_m.cpython-39.pyc
+-rw-rw-rw-   0        0        0     5053 2023-02-21 00:08:06.000000 django-ipghrms-contract-1.9/contract/views/__pycache__/contract_v.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3586 2022-11-05 14:50:10.000000 django-ipghrms-contract-1.9/contract/views/__pycache__/contract_v.cpython-37.pyc
+-rw-rw-rw-   0        0        0     3615 2022-11-04 05:28:45.000000 django-ipghrms-contract-1.9/contract/views/__pycache__/contract_v.cpython-39.pyc
+-rw-rw-rw-   0        0        0      137 2022-11-16 07:11:52.000000 django-ipghrms-contract-1.9/contract/views/__pycache__/history.cpython-310.pyc
+-rw-rw-rw-   0        0        0    14124 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.9/contract/views/__pycache__/manager.cpython-39.pyc
+-rw-rw-rw-   0        0        0     8332 2023-03-17 02:59:45.000000 django-ipghrms-contract-1.9/contract/views/__pycache__/manager_m.cpython-310.pyc
+-rw-rw-rw-   0        0        0     9697 2022-10-20 01:02:26.000000 django-ipghrms-contract-1.9/contract/views/__pycache__/manager_m.cpython-37.pyc
+-rw-rw-rw-   0        0        0     9001 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.9/contract/views/__pycache__/manager_m.cpython-39.pyc
+-rw-rw-rw-   0        0        0     4564 2023-03-08 09:45:19.000000 django-ipghrms-contract-1.9/contract/views/__pycache__/manager_v.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3263 2022-10-20 01:02:26.000000 django-ipghrms-contract-1.9/contract/views/__pycache__/manager_v.cpython-37.pyc
+-rw-rw-rw-   0        0        0     3136 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.9/contract/views/__pycache__/manager_v.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2915 2023-02-09 05:46:27.000000 django-ipghrms-contract-1.9/contract/views/__pycache__/placement.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2885 2022-10-20 01:02:26.000000 django-ipghrms-contract-1.9/contract/views/__pycache__/placement.cpython-37.pyc
+-rw-rw-rw-   0        0        0     2913 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.9/contract/views/__pycache__/placement.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3406 2023-02-23 06:03:20.000000 django-ipghrms-contract-1.9/contract/views/__pycache__/sallary.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3265 2022-10-20 01:02:26.000000 django-ipghrms-contract-1.9/contract/views/__pycache__/sallary.cpython-37.pyc
+-rw-rw-rw-   0        0        0     3220 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.9/contract/views/__pycache__/sallary.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3057 2023-03-10 12:12:04.000000 django-ipghrms-contract-1.9/contract/views/__pycache__/tor.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5887 2023-02-23 05:55:30.000000 django-ipghrms-contract-1.9/contract/views/contract_m.py
+-rw-rw-rw-   0        0        0     5711 2023-06-02 20:57:25.000000 django-ipghrms-contract-1.9/contract/views/contract_v.py
+-rw-rw-rw-   0        0        0    13856 2023-03-16 00:00:39.000000 django-ipghrms-contract-1.9/contract/views/manager_m.py
+-rw-rw-rw-   0        0        0     5350 2023-03-08 09:45:16.000000 django-ipghrms-contract-1.9/contract/views/manager_v.py
+-rw-rw-rw-   0        0        0     9309 2023-06-02 20:58:09.000000 django-ipghrms-contract-1.9/contract/views/placement.py
+-rw-rw-rw-   0        0        0     4123 2023-02-23 06:03:18.000000 django-ipghrms-contract-1.9/contract/views/sallary.py
+-rw-rw-rw-   0        0        0     4080 2023-03-10 12:12:04.000000 django-ipghrms-contract-1.9/contract/views/tor.py
+-rw-rw-rw-   0        0        0       63 2022-10-18 10:39:30.000000 django-ipghrms-contract-1.9/contract/views.py
+drwxrwxrwx   0        0        0        0 2023-06-03 02:43:43.205886 django-ipghrms-contract-1.9/django_ipghrms_contract.egg-info/
+-rw-rw-rw-   0        0        0      972 2023-06-03 02:43:41.000000 django-ipghrms-contract-1.9/django_ipghrms_contract.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     9239 2023-06-03 02:43:41.000000 django-ipghrms-contract-1.9/django_ipghrms_contract.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 02:43:41.000000 django-ipghrms-contract-1.9/django_ipghrms_contract.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 02:43:41.000000 django-ipghrms-contract-1.9/django_ipghrms_contract.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      511 2023-06-03 02:43:43.208878 django-ipghrms-contract-1.9/setup.cfg
+-rw-rw-rw-   0        0        0       39 2023-03-22 07:44:49.000000 django-ipghrms-contract-1.9/setup.py
```

### Comparing `django-ipghrms-contract-1.8/LICENSE` & `django-ipghrms-contract-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/PKG-INFO` & `django-ipghrms-contract-1.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,44 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: django-ipghrms-contract
-Version: 1.8
+Version: 1.9
 Summary: Django IPG HRMS APP CONTRACT
 Home-page: http://ipg.tl/
 Author: Kinos
 Author-email: info@kinos.tl
 Maintainer: kinos
 Maintainer-email: info@kinos.tl
 License: MIT
-Description: 
-        ============================
-        Django IPG HRMS contract
-        ============================
-        
-        
-        Quick start
-        ============
-        
-        
-        1. Add 'contract' to your INSTALLED_APPS settings like this::
-        
-            INSTALLED_APPS = [
-                'contract'
-            ]
-        
-        2. Include the contract to project URLS like this::
-        
-            path('contract/', include('contract.urls')),
-        
-        3. Run ``python manage.py migrate`` to create contract model
-        
-        4. Another Apps Need for this Apps::
-            4.1. custom::
-            4.2. employee::
-            4.3. user
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
+License-File: LICENSE
+
+
+============================
+Django IPG HRMS contract
+============================
+
+
+Quick start
+============
+
+
+1. Add 'contract' to your INSTALLED_APPS settings like this::
+
+    INSTALLED_APPS = [
+        'contract'
+    ]
+
+2. Include the contract to project URLS like this::
+
+    path('contract/', include('contract.urls')),
+
+3. Run ``python manage.py migrate`` to create contract model
+
+4. Another Apps Need for this Apps::
+    4.1. custom::
+    4.2. employee::
+    4.3. user
+
```

### Comparing `django-ipghrms-contract-1.8/contract/admin.py` & `django-ipghrms-contract-1.9/contract/admin.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/api/__pycache__/views.cpython-310.pyc` & `django-ipghrms-contract-1.9/contract/api/__pycache__/views.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/api/__pycache__/views.cpython-37.pyc` & `django-ipghrms-contract-1.9/contract/api/__pycache__/views.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/api/views.py` & `django-ipghrms-contract-1.9/contract/api/views.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/forms/__pycache__/cont_form.cpython-310.pyc` & `django-ipghrms-contract-1.9/contract/forms/__pycache__/cont_form.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/forms/__pycache__/cont_form.cpython-37.pyc` & `django-ipghrms-contract-1.9/contract/forms/__pycache__/cont_form.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/forms/__pycache__/cont_form.cpython-39.pyc` & `django-ipghrms-contract-1.9/contract/forms/__pycache__/cont_form.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/forms/__pycache__/man_form.cpython-310.pyc` & `django-ipghrms-contract-1.9/contract/forms/__pycache__/man_form.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/forms/__pycache__/man_form.cpython-37.pyc` & `django-ipghrms-contract-1.9/contract/forms/__pycache__/man_form.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/forms/__pycache__/man_form.cpython-39.pyc` & `django-ipghrms-contract-1.9/contract/forms/__pycache__/man_form.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/forms/cont_form.py` & `django-ipghrms-contract-1.9/contract/forms/cont_form.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/forms/man_form.py` & `django-ipghrms-contract-1.9/contract/forms/man_form.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/0001_initial.py` & `django-ipghrms-contract-1.9/contract/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/0003_rename_end_reason_empplacement_reason_and_more.py` & `django-ipghrms-contract-1.9/contract/migrations/0003_rename_end_reason_empplacement_reason_and_more.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/0004_remove_contract_category_remove_contract_de_and_more.py` & `django-ipghrms-contract-1.9/contract/migrations/0004_remove_contract_category_remove_contract_de_and_more.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/0005_empplacement_position_alter_empposition_department.py` & `django-ipghrms-contract-1.9/contract/migrations/0005_empplacement_position_alter_empposition_department.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/0007_rename_total_empsalary_amount_and_more.py` & `django-ipghrms-contract-1.9/contract/migrations/0007_rename_total_empsalary_amount_and_more.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/0008_empsalary_employee.py` & `django-ipghrms-contract-1.9/contract/migrations/0008_empsalary_employee.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/0009_alter_empsalary_datetime_alter_empsalary_hashed_and_more.py` & `django-ipghrms-contract-1.9/contract/migrations/0009_alter_empsalary_datetime_alter_empsalary_hashed_and_more.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/0010_category_is_dep_category_is_deputy_category_is_eng_and_more.py` & `django-ipghrms-contract-1.9/contract/migrations/0010_category_is_dep_category_is_deputy_category_is_eng_and_more.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/0012_remove_category_is_advisor_remove_category_is_dep_and_more.py` & `django-ipghrms-contract-1.9/contract/migrations/0012_remove_category_is_advisor_remove_category_is_dep_and_more.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/0014_alter_contract_file.py` & `django-ipghrms-contract-1.9/contract/migrations/0014_alter_contract_file.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/0015_organograma.py` & `django-ipghrms-contract-1.9/contract/migrations/0015_organograma.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/0016_alter_organograma_user.py` & `django-ipghrms-contract-1.9/contract/migrations/0016_alter_organograma_user.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/0017_contract_file_end.py` & `django-ipghrms-contract-1.9/contract/migrations/0017_contract_file_end.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/0018_empcontracttor.py` & `django-ipghrms-contract-1.9/contract/migrations/0018_empcontracttor.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/0019_alter_empcontracttor_contract.py` & `django-ipghrms-contract-1.9/contract/migrations/0019_alter_empcontracttor_contract.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/__pycache__/0001_initial.cpython-310.pyc` & `django-ipghrms-contract-1.9/contract/migrations/__pycache__/0001_initial.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/__pycache__/0001_initial.cpython-37.pyc` & `django-ipghrms-contract-1.9/contract/migrations/__pycache__/0001_initial.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/__pycache__/0001_initial.cpython-39.pyc` & `django-ipghrms-contract-1.9/contract/migrations/__pycache__/0001_initial.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/__pycache__/0002_rename_section_contract_department_and_more.cpython-310.pyc` & `django-ipghrms-contract-1.9/contract/migrations/__pycache__/0002_rename_section_contract_department_and_more.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/__pycache__/0002_rename_section_contract_department_and_more.cpython-37.pyc` & `django-ipghrms-contract-1.9/contract/migrations/__pycache__/0002_rename_section_contract_department_and_more.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/__pycache__/0002_rename_section_contract_department_and_more.cpython-39.pyc` & `django-ipghrms-contract-1.9/contract/migrations/__pycache__/0002_rename_section_contract_department_and_more.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/__pycache__/0003_rename_end_reason_empplacement_reason_and_more.cpython-310.pyc` & `django-ipghrms-contract-1.9/contract/migrations/__pycache__/0003_rename_end_reason_empplacement_reason_and_more.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/__pycache__/0003_rename_end_reason_empplacement_reason_and_more.cpython-37.pyc` & `django-ipghrms-contract-1.9/contract/migrations/__pycache__/0003_rename_end_reason_empplacement_reason_and_more.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/__pycache__/0003_rename_end_reason_empplacement_reason_and_more.cpython-39.pyc` & `django-ipghrms-contract-1.9/contract/migrations/__pycache__/0003_rename_end_reason_empplacement_reason_and_more.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/__pycache__/0004_remove_contract_category_remove_contract_de_and_more.cpython-310.pyc` & `django-ipghrms-contract-1.9/contract/migrations/__pycache__/0004_remove_contract_category_remove_contract_de_and_more.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/__pycache__/0004_remove_contract_category_remove_contract_de_and_more.cpython-37.pyc` & `django-ipghrms-contract-1.9/contract/migrations/__pycache__/0004_remove_contract_category_remove_contract_de_and_more.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/__pycache__/0004_remove_contract_category_remove_contract_de_and_more.cpython-39.pyc` & `django-ipghrms-contract-1.9/contract/migrations/__pycache__/0004_remove_contract_category_remove_contract_de_and_more.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/__pycache__/0005_empplacement_position_alter_empposition_department.cpython-310.pyc` & `django-ipghrms-contract-1.9/contract/migrations/__pycache__/0005_empplacement_position_alter_empposition_department.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/__pycache__/0005_empplacement_position_alter_empposition_department.cpython-37.pyc` & `django-ipghrms-contract-1.9/contract/migrations/__pycache__/0005_empplacement_position_alter_empposition_department.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/__pycache__/0005_empplacement_position_alter_empposition_department.cpython-39.pyc` & `django-ipghrms-contract-1.9/contract/migrations/__pycache__/0005_empplacement_position_alter_empposition_department.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/__pycache__/0006_remove_empsalary_employee_remove_empsalary_position.cpython-310.pyc` & `django-ipghrms-contract-1.9/contract/migrations/__pycache__/0006_remove_empsalary_employee_remove_empsalary_position.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/__pycache__/0006_remove_empsalary_employee_remove_empsalary_position.cpython-37.pyc` & `django-ipghrms-contract-1.9/contract/migrations/__pycache__/0006_remove_empsalary_employee_remove_empsalary_position.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/__pycache__/0006_remove_empsalary_employee_remove_empsalary_position.cpython-39.pyc` & `django-ipghrms-contract-1.9/contract/migrations/__pycache__/0006_remove_empsalary_employee_remove_empsalary_position.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/__pycache__/0007_rename_total_empsalary_amount_and_more.cpython-310.pyc` & `django-ipghrms-contract-1.9/contract/migrations/__pycache__/0007_rename_total_empsalary_amount_and_more.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/__pycache__/0007_rename_total_empsalary_amount_and_more.cpython-37.pyc` & `django-ipghrms-contract-1.9/contract/migrations/__pycache__/0007_rename_total_empsalary_amount_and_more.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/__pycache__/0007_rename_total_empsalary_amount_and_more.cpython-39.pyc` & `django-ipghrms-contract-1.9/contract/migrations/__pycache__/0007_rename_total_empsalary_amount_and_more.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/__pycache__/0008_empsalary_employee.cpython-310.pyc` & `django-ipghrms-contract-1.9/contract/migrations/__pycache__/0008_empsalary_employee.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/__pycache__/0008_empsalary_employee.cpython-37.pyc` & `django-ipghrms-contract-1.9/contract/migrations/__pycache__/0008_empsalary_employee.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/__pycache__/0008_empsalary_employee.cpython-39.pyc` & `django-ipghrms-contract-1.9/contract/migrations/__pycache__/0008_empsalary_employee.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/__pycache__/0009_alter_empsalary_datetime_alter_empsalary_hashed_and_more.cpython-310.pyc` & `django-ipghrms-contract-1.9/contract/migrations/__pycache__/0009_alter_empsalary_datetime_alter_empsalary_hashed_and_more.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/__pycache__/0009_alter_empsalary_datetime_alter_empsalary_hashed_and_more.cpython-37.pyc` & `django-ipghrms-contract-1.9/contract/migrations/__pycache__/0009_alter_empsalary_datetime_alter_empsalary_hashed_and_more.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/__pycache__/0009_alter_empsalary_datetime_alter_empsalary_hashed_and_more.cpython-39.pyc` & `django-ipghrms-contract-1.9/contract/migrations/__pycache__/0009_alter_empsalary_datetime_alter_empsalary_hashed_and_more.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/__pycache__/0010_category_is_dep_category_is_deputy_category_is_eng_and_more.cpython-310.pyc` & `django-ipghrms-contract-1.9/contract/migrations/__pycache__/0010_category_is_dep_category_is_deputy_category_is_eng_and_more.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/__pycache__/0010_category_is_dep_category_is_deputy_category_is_eng_and_more.cpython-37.pyc` & `django-ipghrms-contract-1.9/contract/migrations/__pycache__/0010_category_is_dep_category_is_deputy_category_is_eng_and_more.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/__pycache__/0010_category_is_dep_category_is_deputy_category_is_eng_and_more.cpython-39.pyc` & `django-ipghrms-contract-1.9/contract/migrations/__pycache__/0010_category_is_dep_category_is_deputy_category_is_eng_and_more.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/__pycache__/0011_category_is_advisor.cpython-310.pyc` & `django-ipghrms-contract-1.9/contract/migrations/__pycache__/0011_category_is_advisor.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/__pycache__/0011_category_is_advisor.cpython-37.pyc` & `django-ipghrms-contract-1.9/contract/migrations/__pycache__/0011_category_is_advisor.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/__pycache__/0011_category_is_advisor.cpython-39.pyc` & `django-ipghrms-contract-1.9/contract/migrations/__pycache__/0011_category_is_advisor.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/__pycache__/0012_remove_category_is_advisor_remove_category_is_dep_and_more.cpython-310.pyc` & `django-ipghrms-contract-1.9/contract/migrations/__pycache__/0012_remove_category_is_advisor_remove_category_is_dep_and_more.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/__pycache__/0012_remove_category_is_advisor_remove_category_is_dep_and_more.cpython-37.pyc` & `django-ipghrms-contract-1.9/contract/migrations/__pycache__/0012_remove_category_is_advisor_remove_category_is_dep_and_more.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/__pycache__/0012_remove_category_is_advisor_remove_category_is_dep_and_more.cpython-39.pyc` & `django-ipghrms-contract-1.9/contract/migrations/__pycache__/0012_remove_category_is_advisor_remove_category_is_dep_and_more.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/__pycache__/0013_empposition_is_manager.cpython-310.pyc` & `django-ipghrms-contract-1.9/contract/migrations/__pycache__/0013_empposition_is_manager.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/__pycache__/0014_alter_contract_file.cpython-310.pyc` & `django-ipghrms-contract-1.9/contract/migrations/__pycache__/0014_alter_contract_file.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/__pycache__/0015_organograma.cpython-310.pyc` & `django-ipghrms-contract-1.9/contract/migrations/__pycache__/0015_organograma.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/__pycache__/0016_alter_organograma_user.cpython-310.pyc` & `django-ipghrms-contract-1.9/contract/migrations/__pycache__/0016_alter_organograma_user.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/__pycache__/0017_contract_file_end.cpython-310.pyc` & `django-ipghrms-contract-1.9/contract/migrations/__pycache__/0017_contract_file_end.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/__pycache__/0018_empcontracttor.cpython-310.pyc` & `django-ipghrms-contract-1.9/contract/migrations/__pycache__/0018_empcontracttor.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/migrations/__pycache__/0019_alter_empcontracttor_contract.cpython-310.pyc` & `django-ipghrms-contract-1.9/contract/migrations/__pycache__/0019_alter_empcontracttor_contract.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/models.py` & `django-ipghrms-contract-1.9/contract/models.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/templates/contract/cont_hist.html` & `django-ipghrms-contract-1.9/contract/templates/contract/cont_hist.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/templates/contract/dash.html` & `django-ipghrms-contract-1.9/contract/templates/contract/dash.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/templates/contract/detail.html` & `django-ipghrms-contract-1.9/contract/templates/contract/detail.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/templates/contract/form.html` & `django-ipghrms-contract-1.9/contract/templates/contract/form.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/templates/contract/form_upgrade.html` & `django-ipghrms-contract-1.9/contract/templates/contract/form_upgrade.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/templates/contract/list.html` & `django-ipghrms-contract-1.9/contract/templates/contract/list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/templates/contract/nocont_list.html` & `django-ipghrms-contract-1.9/contract/templates/contract/nocont_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/templates/contract_chart/cont_cat.js` & `django-ipghrms-contract-1.9/contract/templates/contract_chart/cont_cat.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/templates/contract_chart/cont_cat2.js` & `django-ipghrms-contract-1.9/contract/templates/contract_chart/cont_cat2.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/templates/contract_chart/cont_chart.html` & `django-ipghrms-contract-1.9/contract/templates/contract_chart/cont_chart.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/templates/contract_chart/cont_pos.js` & `django-ipghrms-contract-1.9/contract/templates/contract_chart/cont_pos.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/templates/contract_chart/cont_pos2.js` & `django-ipghrms-contract-1.9/contract/templates/contract_chart/cont_pos2.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/templates/contract_chart/cont_type.js` & `django-ipghrms-contract-1.9/contract/templates/contract_chart/cont_type.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/templates/manager/dash.html` & `django-ipghrms-contract-1.9/contract/templates/manager/dash.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/templates/manager/form.html` & `django-ipghrms-contract-1.9/contract/templates/manager/form.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/templates/manager/man_de.html` & `django-ipghrms-contract-1.9/contract/templates/manager/man_de.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/templates/manager/man_dep.html` & `django-ipghrms-contract-1.9/contract/templates/manager/man_dep.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/templates/manager/man_hist.html` & `django-ipghrms-contract-1.9/contract/templates/manager/man_hist.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/templates/manager/man_unit.html` & `django-ipghrms-contract-1.9/contract/templates/manager/man_unit.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/templates/placement/detail.html` & `django-ipghrms-contract-1.9/contract/templates/placement/detail.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/templates/placement/form.html` & `django-ipghrms-contract-1.9/contract/templates/placement/form.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/templates/placement/list.html` & `django-ipghrms-contract-1.9/contract/templates/placement/list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/templates/salary/detail.html` & `django-ipghrms-contract-1.9/contract/templates/salary/detail.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/templates/salary/form.html` & `django-ipghrms-contract-1.9/contract/templates/salary/form.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/templates/salary/list.html` & `django-ipghrms-contract-1.9/contract/templates/salary/list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/templates/salary/no_salary_list.html` & `django-ipghrms-contract-1.9/contract/templates/salary/no_salary_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/templates/tor/form.html` & `django-ipghrms-contract-1.9/contract/templates/tor/form.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/templates/tor/list.html` & `django-ipghrms-contract-1.9/contract/templates/tor/list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/urls.py` & `django-ipghrms-contract-1.9/contract/urls.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/urls_man.py` & `django-ipghrms-contract-1.9/contract/urls_man.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/views/__pycache__/contract.cpython-39.pyc` & `django-ipghrms-contract-1.9/contract/views/__pycache__/contract.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/views/__pycache__/contract_m.cpython-310.pyc` & `django-ipghrms-contract-1.9/contract/views/__pycache__/contract_m.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/views/__pycache__/contract_m.cpython-37.pyc` & `django-ipghrms-contract-1.9/contract/views/__pycache__/contract_m.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/views/__pycache__/contract_m.cpython-39.pyc` & `django-ipghrms-contract-1.9/contract/views/__pycache__/contract_m.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/views/__pycache__/contract_v.cpython-310.pyc` & `django-ipghrms-contract-1.9/contract/views/__pycache__/contract_v.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/views/__pycache__/contract_v.cpython-37.pyc` & `django-ipghrms-contract-1.9/contract/views/__pycache__/contract_v.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/views/__pycache__/contract_v.cpython-39.pyc` & `django-ipghrms-contract-1.9/contract/views/__pycache__/contract_v.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/views/__pycache__/manager.cpython-39.pyc` & `django-ipghrms-contract-1.9/contract/views/__pycache__/manager.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/views/__pycache__/manager_m.cpython-310.pyc` & `django-ipghrms-contract-1.9/contract/views/__pycache__/manager_m.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/views/__pycache__/manager_m.cpython-37.pyc` & `django-ipghrms-contract-1.9/contract/views/__pycache__/manager_m.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/views/__pycache__/manager_m.cpython-39.pyc` & `django-ipghrms-contract-1.9/contract/views/__pycache__/manager_m.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/views/__pycache__/manager_v.cpython-310.pyc` & `django-ipghrms-contract-1.9/contract/views/__pycache__/manager_v.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/views/__pycache__/manager_v.cpython-37.pyc` & `django-ipghrms-contract-1.9/contract/views/__pycache__/manager_v.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/views/__pycache__/manager_v.cpython-39.pyc` & `django-ipghrms-contract-1.9/contract/views/__pycache__/manager_v.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/views/__pycache__/placement.cpython-310.pyc` & `django-ipghrms-contract-1.9/contract/views/__pycache__/placement.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/views/__pycache__/placement.cpython-37.pyc` & `django-ipghrms-contract-1.9/contract/views/__pycache__/placement.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/views/__pycache__/placement.cpython-39.pyc` & `django-ipghrms-contract-1.9/contract/views/__pycache__/placement.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/views/__pycache__/sallary.cpython-310.pyc` & `django-ipghrms-contract-1.9/contract/views/__pycache__/sallary.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/views/__pycache__/sallary.cpython-37.pyc` & `django-ipghrms-contract-1.9/contract/views/__pycache__/sallary.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/views/__pycache__/sallary.cpython-39.pyc` & `django-ipghrms-contract-1.9/contract/views/__pycache__/sallary.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/views/__pycache__/tor.cpython-310.pyc` & `django-ipghrms-contract-1.9/contract/views/__pycache__/tor.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/views/contract_m.py` & `django-ipghrms-contract-1.9/contract/views/contract_m.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/views/contract_v.py` & `django-ipghrms-contract-1.9/contract/views/contract_v.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/views/manager_m.py` & `django-ipghrms-contract-1.9/contract/views/manager_m.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/views/manager_v.py` & `django-ipghrms-contract-1.9/contract/views/manager_v.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/views/placement.py` & `django-ipghrms-contract-1.9/contract/views/placement.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/views/sallary.py` & `django-ipghrms-contract-1.9/contract/views/sallary.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/contract/views/tor.py` & `django-ipghrms-contract-1.9/contract/views/tor.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-contract-1.8/django_ipghrms_contract.egg-info/PKG-INFO` & `django-ipghrms-contract-1.9/django_ipghrms_contract.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,44 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: django-ipghrms-contract
-Version: 1.8
+Version: 1.9
 Summary: Django IPG HRMS APP CONTRACT
 Home-page: http://ipg.tl/
 Author: Kinos
 Author-email: info@kinos.tl
 Maintainer: kinos
 Maintainer-email: info@kinos.tl
 License: MIT
-Description: 
-        ============================
-        Django IPG HRMS contract
-        ============================
-        
-        
-        Quick start
-        ============
-        
-        
-        1. Add 'contract' to your INSTALLED_APPS settings like this::
-        
-            INSTALLED_APPS = [
-                'contract'
-            ]
-        
-        2. Include the contract to project URLS like this::
-        
-            path('contract/', include('contract.urls')),
-        
-        3. Run ``python manage.py migrate`` to create contract model
-        
-        4. Another Apps Need for this Apps::
-            4.1. custom::
-            4.2. employee::
-            4.3. user
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
+License-File: LICENSE
+
+
+============================
+Django IPG HRMS contract
+============================
+
+
+Quick start
+============
+
+
+1. Add 'contract' to your INSTALLED_APPS settings like this::
+
+    INSTALLED_APPS = [
+        'contract'
+    ]
+
+2. Include the contract to project URLS like this::
+
+    path('contract/', include('contract.urls')),
+
+3. Run ``python manage.py migrate`` to create contract model
+
+4. Another Apps Need for this Apps::
+    4.1. custom::
+    4.2. employee::
+    4.3. user
+
```

### Comparing `django-ipghrms-contract-1.8/django_ipghrms_contract.egg-info/SOURCES.txt` & `django-ipghrms-contract-1.9/django_ipghrms_contract.egg-info/SOURCES.txt`

 * *Files identical despite different names*

