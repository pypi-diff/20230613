# Comparing `tmp/django-ipghrms-attendance-1.1.tar.gz` & `tmp/django-ipghrms-attendance-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-ipghrms-attendance-1.1.tar", last modified: Mon Mar 27 00:59:15 2023, max compression
+gzip compressed data, was "django-ipghrms-attendance-1.5.tar", last modified: Tue Jun 13 12:54:21 2023, max compression
```

## Comparing `django-ipghrms-attendance-1.1.tar` & `django-ipghrms-attendance-1.5.tar`

### file list

```diff
@@ -1,179 +1,179 @@
-drwxrwxrwx   0        0        0        0 2023-03-27 00:59:14.995800 django-ipghrms-attendance-1.1/
--rw-rw-rw-   0        0        0     1068 2023-03-22 07:40:25.000000 django-ipghrms-attendance-1.1/LICENSE
--rw-rw-rw-   0        0        0      158 2023-03-27 00:52:22.000000 django-ipghrms-attendance-1.1/MANIFEST.in
--rw-rw-rw-   0        0        0      953 2023-03-27 00:59:14.995800 django-ipghrms-attendance-1.1/PKG-INFO
--rw-rw-rw-   0        0        0      512 2023-03-22 08:09:49.000000 django-ipghrms-attendance-1.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-03-27 00:59:14.080848 django-ipghrms-attendance-1.1/attendance/
--rw-rw-rw-   0        0        0        0 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.1/attendance/__init__.py
--rw-rw-rw-   0        0        0      251 2022-12-09 18:30:25.000000 django-ipghrms-attendance-1.1/attendance/admin.py
--rw-rw-rw-   0        0        0      152 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.1/attendance/apps.py
--rw-rw-rw-   0        0        0     5432 2023-02-15 10:39:25.000000 django-ipghrms-attendance-1.1/attendance/forms.py
-drwxrwxrwx   0        0        0        0 2023-03-27 00:59:14.194837 django-ipghrms-attendance-1.1/attendance/migrations/
--rw-rw-rw-   0        0        0     4663 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.1/attendance/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      580 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.1/attendance/migrations/0002_alter_attendance_time_am_alter_attendance_time_pm.py
--rw-rw-rw-   0        0        0      668 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.1/attendance/migrations/0003_alter_attendance_time_am_alter_attendance_time_pm.py
--rw-rw-rw-   0        0        0     1139 2022-11-04 05:28:45.000000 django-ipghrms-attendance-1.1/attendance/migrations/0004_alter_attendance_is_present_attendancetotal.py
--rw-rw-rw-   0        0        0      782 2022-11-04 05:28:45.000000 django-ipghrms-attendance-1.1/attendance/migrations/0005_attendance_month_attendance_year.py
--rw-rw-rw-   0        0        0      731 2022-11-04 05:28:45.000000 django-ipghrms-attendance-1.1/attendance/migrations/0006_alter_attendancetotal_month_and_more.py
--rw-rw-rw-   0        0        0      451 2022-11-04 05:28:45.000000 django-ipghrms-attendance-1.1/attendance/migrations/0007_alter_attendance_is_present.py
--rw-rw-rw-   0        0        0      724 2022-11-04 05:28:45.000000 django-ipghrms-attendance-1.1/attendance/migrations/0008_alter_attendanceunit_month_alter_attendanceunit_year.py
--rw-rw-rw-   0        0        0      611 2022-11-04 05:28:45.000000 django-ipghrms-attendance-1.1/attendance/migrations/0009_attendancetotal_unit.py
--rw-rw-rw-   0        0        0      655 2022-11-22 01:39:19.000000 django-ipghrms-attendance-1.1/attendance/migrations/0010_alter_attendanceunit_file.py
--rw-rw-rw-   0        0        0      669 2022-12-08 01:56:49.000000 django-ipghrms-attendance-1.1/attendance/migrations/0011_auto_20221208_1056.py
--rw-rw-rw-   0        0        0      737 2022-12-08 03:51:53.000000 django-ipghrms-attendance-1.1/attendance/migrations/0012_auto_20221208_1251.py
--rw-rw-rw-   0        0        0      460 2022-12-08 04:13:59.000000 django-ipghrms-attendance-1.1/attendance/migrations/0013_auto_20221208_1313.py
--rw-rw-rw-   0        0        0      622 2022-12-08 17:13:59.000000 django-ipghrms-attendance-1.1/attendance/migrations/0014_attendance_leader.py
--rw-rw-rw-   0        0        0     3002 2022-12-09 06:36:09.000000 django-ipghrms-attendance-1.1/attendance/migrations/0015_auto_20221209_1536.py
--rw-rw-rw-   0        0        0      959 2022-12-10 13:58:18.000000 django-ipghrms-attendance-1.1/attendance/migrations/0016_auto_20221210_2258.py
--rw-rw-rw-   0        0        0      659 2022-12-12 06:02:42.000000 django-ipghrms-attendance-1.1/attendance/migrations/0017_auto_20221212_1502.py
--rw-rw-rw-   0        0        0      448 2022-12-12 07:36:13.000000 django-ipghrms-attendance-1.1/attendance/migrations/0018_alter_attendance_totat_hour.py
--rw-rw-rw-   0        0        0      447 2023-02-15 10:11:30.000000 django-ipghrms-attendance-1.1/attendance/migrations/0019_attendance_is_hr_update.py
--rw-rw-rw-   0        0        0      446 2023-02-15 10:15:09.000000 django-ipghrms-attendance-1.1/attendance/migrations/0020_alter_attendance_is_hr_update.py
--rw-rw-rw-   0        0        0     1054 2023-02-15 10:23:09.000000 django-ipghrms-attendance-1.1/attendance/migrations/0021_auto_20230215_1923.py
--rw-rw-rw-   0        0        0        0 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.1/attendance/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-27 00:59:14.499980 django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/
--rw-rw-rw-   0        0        0     2628 2022-11-07 13:19:40.000000 django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0001_initial.cpython-310.pyc
--rw-rw-rw-   0        0        0     2598 2022-10-20 01:03:56.000000 django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0001_initial.cpython-37.pyc
--rw-rw-rw-   0        0        0     2632 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0001_initial.cpython-39.pyc
--rw-rw-rw-   0        0        0      691 2022-11-07 13:19:40.000000 django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0002_alter_attendance_time_am_alter_attendance_time_pm.cpython-310.pyc
--rw-rw-rw-   0        0        0      675 2022-10-20 01:03:56.000000 django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0002_alter_attendance_time_am_alter_attendance_time_pm.cpython-37.pyc
--rw-rw-rw-   0        0        0      695 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0002_alter_attendance_time_am_alter_attendance_time_pm.cpython-39.pyc
--rw-rw-rw-   0        0        0      755 2022-11-07 13:19:40.000000 django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0003_alter_attendance_time_am_alter_attendance_time_pm.cpython-310.pyc
--rw-rw-rw-   0        0        0      739 2022-10-20 01:03:56.000000 django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0003_alter_attendance_time_am_alter_attendance_time_pm.cpython-37.pyc
--rw-rw-rw-   0        0        0      759 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0003_alter_attendance_time_am_alter_attendance_time_pm.cpython-39.pyc
--rw-rw-rw-   0        0        0     1180 2022-11-07 13:19:40.000000 django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0004_alter_attendance_is_present_attendancetotal.cpython-310.pyc
--rw-rw-rw-   0        0        0     1162 2022-11-05 14:52:09.000000 django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0004_alter_attendance_is_present_attendancetotal.cpython-37.pyc
--rw-rw-rw-   0        0        0      821 2022-11-07 13:19:40.000000 django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0005_attendance_month_attendance_year.cpython-310.pyc
--rw-rw-rw-   0        0        0      805 2022-11-05 14:52:09.000000 django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0005_attendance_month_attendance_year.cpython-37.pyc
--rw-rw-rw-   0        0        0      810 2022-11-07 13:19:40.000000 django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0006_alter_attendancetotal_month_and_more.cpython-310.pyc
--rw-rw-rw-   0        0        0      794 2022-11-05 14:52:09.000000 django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0006_alter_attendancetotal_month_and_more.cpython-37.pyc
--rw-rw-rw-   0        0        0      652 2022-11-07 13:19:40.000000 django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0007_alter_attendance_is_present.cpython-310.pyc
--rw-rw-rw-   0        0        0      638 2022-11-05 14:52:09.000000 django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0007_alter_attendance_is_present.cpython-37.pyc
--rw-rw-rw-   0        0        0      820 2022-11-07 13:19:40.000000 django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0008_alter_attendanceunit_month_alter_attendanceunit_year.cpython-310.pyc
--rw-rw-rw-   0        0        0      804 2022-11-05 14:52:09.000000 django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0008_alter_attendanceunit_month_alter_attendanceunit_year.cpython-37.pyc
--rw-rw-rw-   0        0        0      808 2022-11-07 13:19:40.000000 django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0009_attendancetotal_unit.cpython-310.pyc
--rw-rw-rw-   0        0        0      794 2022-11-05 14:52:09.000000 django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0009_attendancetotal_unit.cpython-37.pyc
--rw-rw-rw-   0        0        0      875 2022-11-22 01:39:26.000000 django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0010_alter_attendanceunit_file.cpython-310.pyc
--rw-rw-rw-   0        0        0      702 2022-12-08 01:56:57.000000 django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0011_auto_20221208_1056.cpython-310.pyc
--rw-rw-rw-   0        0        0      666 2022-12-08 03:51:59.000000 django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0012_auto_20221208_1251.cpython-310.pyc
--rw-rw-rw-   0        0        0      546 2022-12-08 04:14:06.000000 django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0013_auto_20221208_1313.cpython-310.pyc
--rw-rw-rw-   0        0        0      792 2022-12-08 17:14:03.000000 django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0014_attendance_leader.cpython-310.pyc
--rw-rw-rw-   0        0        0     1636 2022-12-09 06:36:18.000000 django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0015_auto_20221209_1536.cpython-310.pyc
--rw-rw-rw-   0        0        0      801 2022-12-10 13:58:24.000000 django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0016_auto_20221210_2258.cpython-310.pyc
--rw-rw-rw-   0        0        0      690 2022-12-12 06:02:48.000000 django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0017_auto_20221212_1502.cpython-310.pyc
--rw-rw-rw-   0        0        0      629 2022-12-12 07:36:17.000000 django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0018_alter_attendance_totat_hour.cpython-310.pyc
--rw-rw-rw-   0        0        0      620 2023-02-15 10:11:39.000000 django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0019_attendance_is_hr_update.cpython-310.pyc
--rw-rw-rw-   0        0        0      625 2023-02-15 10:15:13.000000 django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0020_alter_attendance_is_hr_update.cpython-310.pyc
--rw-rw-rw-   0        0        0      796 2023-02-15 10:23:13.000000 django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0021_auto_20230215_1923.cpython-310.pyc
--rw-rw-rw-   0        0        0      150 2022-11-07 13:19:40.000000 django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      148 2022-10-20 01:03:56.000000 django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0      156 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     6910 2023-03-22 07:29:58.000000 django-ipghrms-attendance-1.1/attendance/models.py
-drwxrwxrwx   0        0        0        0 2023-03-27 00:59:13.995480 django-ipghrms-attendance-1.1/attendance/templates/
-drwxrwxrwx   0        0        0        0 2023-03-27 00:59:14.574931 django-ipghrms-attendance-1.1/attendance/templates/attendance/
--rw-rw-rw-   0        0        0     1811 2023-03-27 00:57:38.000000 django-ipghrms-attendance-1.1/attendance/templates/attendance/dash.html
--rw-rw-rw-   0        0        0     2757 2022-12-13 05:01:14.000000 django-ipghrms-attendance-1.1/attendance/templates/attendance/day_list.html
--rw-rw-rw-   0        0        0     1256 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.1/attendance/templates/attendance/form_am-pm.html
--rw-rw-rw-   0        0        0     1297 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.1/attendance/templates/attendance/form_emp.html
--rw-rw-rw-   0        0        0     1103 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.1/attendance/templates/attendance/form_upload.html
--rw-rw-rw-   0        0        0     2263 2023-02-15 09:23:11.000000 django-ipghrms-attendance-1.1/attendance/templates/attendance/import.html
--rw-rw-rw-   0        0        0     2412 2023-02-08 06:02:53.000000 django-ipghrms-attendance-1.1/attendance/templates/attendance/list.html
--rw-rw-rw-   0        0        0     4124 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.1/attendance/templates/attendance/unit_date_emp.html
--rw-rw-rw-   0        0        0     3645 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.1/attendance/templates/attendance/unit_day_emp.html
--rw-rw-rw-   0        0        0     4807 2022-12-12 12:51:19.000000 django-ipghrms-attendance-1.1/attendance/templates/attendance/unit_emp_date.html
--rw-rw-rw-   0        0        0    17366 2023-03-13 01:04:46.000000 django-ipghrms-attendance-1.1/attendance/templates/attendance/unit_list.html
-drwxrwxrwx   0        0        0        0 2023-03-27 00:59:14.671593 django-ipghrms-attendance-1.1/attendance/templates/attendance_back/
--rw-rw-rw-   0        0        0     3650 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.1/attendance/templates/attendance_back/adv_day_emp.html
--rw-rw-rw-   0        0        0     4678 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.1/attendance/templates/attendance_back/adv_list.html
--rw-rw-rw-   0        0        0     1539 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.1/attendance/templates/attendance_back/dash.html
--rw-rw-rw-   0        0        0     2015 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.1/attendance/templates/attendance_back/dash_back.html
--rw-rw-rw-   0        0        0     3650 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.1/attendance/templates/attendance_back/dg_day_emp.html
--rw-rw-rw-   0        0        0     3125 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.1/attendance/templates/attendance_back/dg_emp_date.html
--rw-rw-rw-   0        0        0     4688 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.1/attendance/templates/attendance_back/dg_list.html
--rw-rw-rw-   0        0        0     3740 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.1/attendance/templates/attendance_back/div_date_emp.html
--rw-rw-rw-   0        0        0     3654 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.1/attendance/templates/attendance_back/div_day_emp.html
--rw-rw-rw-   0        0        0     3133 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.1/attendance/templates/attendance_back/div_emp_date.html
--rw-rw-rw-   0        0        0     4731 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.1/attendance/templates/attendance_back/div_list.html
--rw-rw-rw-   0        0        0     1266 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.1/attendance/templates/attendance_back/form_am-pm.html
--rw-rw-rw-   0        0        0     1306 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.1/attendance/templates/attendance_back/form_emp.html
--rw-rw-rw-   0        0        0     1112 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.1/attendance/templates/attendance_back/form_upload.html
-drwxrwxrwx   0        0        0        0 2023-03-27 00:59:14.693421 django-ipghrms-attendance-1.1/attendance/templates/attendance_custom/
--rw-rw-rw-   0        0        0     3859 2023-02-08 05:57:14.000000 django-ipghrms-attendance-1.1/attendance/templates/attendance_custom/dash.html
--rw-rw-rw-   0        0        0     1275 2023-02-08 05:55:54.000000 django-ipghrms-attendance-1.1/attendance/templates/attendance_custom/form.html
--rw-rw-rw-   0        0        0     2001 2023-02-08 05:53:02.000000 django-ipghrms-attendance-1.1/attendance/templates/attendance_custom/list.html
--rw-rw-rw-   0        0        0      794 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.1/attendance/templates/attendance_custom/year.html
-drwxrwxrwx   0        0        0        0 2023-03-27 00:59:14.715777 django-ipghrms-attendance-1.1/attendance/templates/attendance_print/
--rw-rw-rw-   0        0        0     2294 2022-11-30 08:00:13.000000 django-ipghrms-attendance-1.1/attendance/templates/attendance_print/layout.html
--rw-rw-rw-   0        0        0     5520 2023-02-08 05:04:16.000000 django-ipghrms-attendance-1.1/attendance/templates/attendance_print/print_attend.html
--rw-rw-rw-   0        0        0     2199 2023-01-07 14:02:48.000000 django-ipghrms-attendance-1.1/attendance/templates/attendance_print/print_r_emp.html
--rw-rw-rw-   0        0        0     4250 2023-02-08 05:30:25.000000 django-ipghrms-attendance-1.1/attendance/templates/attendance_print/print_r_lic_fal.html
-drwxrwxrwx   0        0        0        0 2023-03-27 00:59:14.749723 django-ipghrms-attendance-1.1/attendance/templates/attendance_report/
--rw-rw-rw-   0        0        0     2574 2023-02-08 05:12:58.000000 django-ipghrms-attendance-1.1/attendance/templates/attendance_report/r_dash.html
--rw-rw-rw-   0        0        0     9471 2023-01-31 03:48:50.000000 django-ipghrms-attendance-1.1/attendance/templates/attendance_report/r_emp_dash.html
--rw-rw-rw-   0        0        0     2870 2023-02-08 05:17:39.000000 django-ipghrms-attendance-1.1/attendance/templates/attendance_report/r_emp_search.html
--rw-rw-rw-   0        0        0     1410 2023-02-08 05:28:53.000000 django-ipghrms-attendance-1.1/attendance/templates/attendance_report/r_licfal_year.html
--rw-rw-rw-   0        0        0    18080 2023-03-13 20:46:15.000000 django-ipghrms-attendance-1.1/attendance/templates/attendance_report/r_unit_dash.html
--rw-rw-rw-   0        0        0    17991 2023-03-13 20:49:02.000000 django-ipghrms-attendance-1.1/attendance/templates/attendance_report/r_unit_list.html
--rw-rw-rw-   0        0        0       60 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.1/attendance/tests.py
--rw-rw-rw-   0        0        0     3707 2023-02-08 05:58:11.000000 django-ipghrms-attendance-1.1/attendance/urls.py
--rw-rw-rw-   0        0        0     1462 2023-01-31 03:45:05.000000 django-ipghrms-attendance-1.1/attendance/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-27 00:59:14.786846 django-ipghrms-attendance-1.1/attendance/views/
--rw-rw-rw-   0        0        0      148 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.1/attendance/views/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-27 00:59:14.977191 django-ipghrms-attendance-1.1/attendance/views/__pycache__/
--rw-rw-rw-   0        0        0      275 2022-11-07 13:19:38.000000 django-ipghrms-attendance-1.1/attendance/views/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      273 2022-10-20 01:03:04.000000 django-ipghrms-attendance-1.1/attendance/views/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0      355 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.1/attendance/views/__pycache__/__init__.cpython-38.pyc
--rw-rw-rw-   0        0        0      281 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.1/attendance/views/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     3891 2023-02-08 05:31:42.000000 django-ipghrms-attendance-1.1/attendance/views/__pycache__/attend_custom.cpython-310.pyc
--rw-rw-rw-   0        0        0     4526 2022-11-05 14:50:11.000000 django-ipghrms-attendance-1.1/attendance/views/__pycache__/attend_custom.cpython-37.pyc
--rw-rw-rw-   0        0        0     4300 2022-11-04 05:28:45.000000 django-ipghrms-attendance-1.1/attendance/views/__pycache__/attend_custom.cpython-39.pyc
--rw-rw-rw-   0        0        0    12374 2023-02-15 10:14:59.000000 django-ipghrms-attendance-1.1/attendance/views/__pycache__/attend_m.cpython-310.pyc
--rw-rw-rw-   0        0        0     9821 2022-11-07 06:12:38.000000 django-ipghrms-attendance-1.1/attendance/views/__pycache__/attend_m.cpython-37.pyc
--rw-rw-rw-   0        0        0     9286 2022-11-04 05:28:45.000000 django-ipghrms-attendance-1.1/attendance/views/__pycache__/attend_m.cpython-39.pyc
--rw-rw-rw-   0        0        0     4938 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.1/attendance/views/__pycache__/attend_unit.cpython-39.pyc
--rw-rw-rw-   0        0        0     5849 2023-03-13 20:41:29.000000 django-ipghrms-attendance-1.1/attendance/views/__pycache__/attend_v.cpython-310.pyc
--rw-rw-rw-   0        0        0     3586 2022-11-05 14:50:11.000000 django-ipghrms-attendance-1.1/attendance/views/__pycache__/attend_v.cpython-37.pyc
--rw-rw-rw-   0        0        0     3582 2022-11-04 05:28:45.000000 django-ipghrms-attendance-1.1/attendance/views/__pycache__/attend_v.cpython-39.pyc
--rw-rw-rw-   0        0        0     9896 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.1/attendance/views/__pycache__/attendance.cpython-38.pyc
--rw-rw-rw-   0        0        0     9728 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.1/attendance/views/__pycache__/attendance.cpython-39.pyc
--rw-rw-rw-   0        0        0     4818 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.1/attendance/views/__pycache__/attendance_adv.cpython-38.pyc
--rw-rw-rw-   0        0        0     5286 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.1/attendance/views/__pycache__/attendance_custom.cpython-38.pyc
--rw-rw-rw-   0        0        0     3890 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.1/attendance/views/__pycache__/attendance_custom.cpython-39.pyc
--rw-rw-rw-   0        0        0     4979 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.1/attendance/views/__pycache__/attendance_dg.cpython-38.pyc
--rw-rw-rw-   0        0        0     4940 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.1/attendance/views/__pycache__/attendance_dg.cpython-39.pyc
--rw-rw-rw-   0        0        0     2321 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.1/attendance/views/__pycache__/attendance_report.cpython-38.pyc
--rw-rw-rw-   0        0        0     5287 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.1/attendance/views/__pycache__/attendance_set.cpython-38.pyc
--rw-rw-rw-   0        0        0     1726 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.1/attendance/views/__pycache__/export.cpython-38.pyc
--rw-rw-rw-   0        0        0     1487 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.1/attendance/views/__pycache__/general.cpython-38.pyc
--rw-rw-rw-   0        0        0      147 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.1/attendance/views/__pycache__/holiday.cpython-38.pyc
--rw-rw-rw-   0        0        0     5313 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.1/attendance/views/__pycache__/leave.cpython-38.pyc
--rw-rw-rw-   0        0        0     5963 2022-11-16 14:38:57.000000 django-ipghrms-attendance-1.1/attendance/views/__pycache__/print.cpython-310.pyc
--rw-rw-rw-   0        0        0     6127 2022-11-07 09:08:07.000000 django-ipghrms-attendance-1.1/attendance/views/__pycache__/print.cpython-37.pyc
--rw-rw-rw-   0        0        0     6276 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.1/attendance/views/__pycache__/print.cpython-38.pyc
--rw-rw-rw-   0        0        0     5929 2022-11-04 05:28:45.000000 django-ipghrms-attendance-1.1/attendance/views/__pycache__/print.cpython-39.pyc
--rw-rw-rw-   0        0        0     2310 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.1/attendance/views/__pycache__/qrscanner.cpython-38.pyc
--rw-rw-rw-   0        0        0     8596 2023-03-13 20:48:11.000000 django-ipghrms-attendance-1.1/attendance/views/__pycache__/reports.cpython-310.pyc
--rw-rw-rw-   0        0        0     6021 2022-11-05 14:50:11.000000 django-ipghrms-attendance-1.1/attendance/views/__pycache__/reports.cpython-37.pyc
--rw-rw-rw-   0        0        0     5836 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.1/attendance/views/__pycache__/reports.cpython-38.pyc
--rw-rw-rw-   0        0        0     5964 2022-11-04 05:28:45.000000 django-ipghrms-attendance-1.1/attendance/views/__pycache__/reports.cpython-39.pyc
--rw-rw-rw-   0        0        0     5220 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.1/attendance/views/__pycache__/reports_dg.cpython-38.pyc
--rw-rw-rw-   0        0        0     4721 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.1/attendance/views/__pycache__/reports_div.cpython-38.pyc
--rw-rw-rw-   0        0        0     5031 2023-03-13 20:43:37.000000 django-ipghrms-attendance-1.1/attendance/views/__pycache__/reports_unit.cpython-310.pyc
--rw-rw-rw-   0        0        0     4802 2022-10-20 01:03:04.000000 django-ipghrms-attendance-1.1/attendance/views/__pycache__/reports_unit.cpython-37.pyc
--rw-rw-rw-   0        0        0     4808 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.1/attendance/views/__pycache__/reports_unit.cpython-39.pyc
--rw-rw-rw-   0        0        0      148 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.1/attendance/views/__pycache__/timesheet.cpython-38.pyc
--rw-rw-rw-   0        0        0     2215 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.1/attendance/views/__pycache__/webcam.cpython-38.pyc
--rw-rw-rw-   0        0        0     4882 2023-02-08 05:31:36.000000 django-ipghrms-attendance-1.1/attendance/views/attend_custom.py
--rw-rw-rw-   0        0        0    16927 2023-02-15 10:14:55.000000 django-ipghrms-attendance-1.1/attendance/views/attend_m.py
--rw-rw-rw-   0        0        0     7058 2023-03-13 20:41:26.000000 django-ipghrms-attendance-1.1/attendance/views/attend_v.py
--rw-rw-rw-   0        0        0     8638 2022-11-16 14:38:53.000000 django-ipghrms-attendance-1.1/attendance/views/print.py
--rw-rw-rw-   0        0        0    11893 2023-03-13 20:48:08.000000 django-ipghrms-attendance-1.1/attendance/views/reports.py
--rw-rw-rw-   0        0        0     6146 2023-03-13 20:43:34.000000 django-ipghrms-attendance-1.1/attendance/views/reports_unit.py
--rw-rw-rw-   0        0        0       63 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.1/attendance/views.py
-drwxrwxrwx   0        0        0        0 2023-03-27 00:59:14.992875 django-ipghrms-attendance-1.1/django_ipghrms_attendance.egg-info/
--rw-rw-rw-   0        0        0      953 2023-03-27 00:59:13.000000 django-ipghrms-attendance-1.1/django_ipghrms_attendance.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     9225 2023-03-27 00:59:13.000000 django-ipghrms-attendance-1.1/django_ipghrms_attendance.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-27 00:59:13.000000 django-ipghrms-attendance-1.1/django_ipghrms_attendance.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-03-27 00:59:13.000000 django-ipghrms-attendance-1.1/django_ipghrms_attendance.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      504 2023-03-27 00:59:14.995800 django-ipghrms-attendance-1.1/setup.cfg
--rw-rw-rw-   0        0        0       39 2023-03-22 07:44:49.000000 django-ipghrms-attendance-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 12:54:21.343343 django-ipghrms-attendance-1.5/
+-rw-rw-rw-   0        0        0     1068 2023-03-22 07:40:25.000000 django-ipghrms-attendance-1.5/LICENSE
+-rw-rw-rw-   0        0        0      158 2023-03-27 00:52:22.000000 django-ipghrms-attendance-1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      953 2023-06-13 12:54:21.343343 django-ipghrms-attendance-1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      512 2023-03-22 08:09:49.000000 django-ipghrms-attendance-1.5/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-13 12:54:19.443945 django-ipghrms-attendance-1.5/attendance/
+-rw-rw-rw-   0        0        0        0 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.5/attendance/__init__.py
+-rw-rw-rw-   0        0        0      251 2022-12-09 18:30:25.000000 django-ipghrms-attendance-1.5/attendance/admin.py
+-rw-rw-rw-   0        0        0      152 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.5/attendance/apps.py
+-rw-rw-rw-   0        0        0     5432 2023-02-15 10:39:25.000000 django-ipghrms-attendance-1.5/attendance/forms.py
+drwxrwxrwx   0        0        0        0 2023-06-13 12:54:19.578986 django-ipghrms-attendance-1.5/attendance/migrations/
+-rw-rw-rw-   0        0        0     4663 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.5/attendance/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      580 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.5/attendance/migrations/0002_alter_attendance_time_am_alter_attendance_time_pm.py
+-rw-rw-rw-   0        0        0      668 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.5/attendance/migrations/0003_alter_attendance_time_am_alter_attendance_time_pm.py
+-rw-rw-rw-   0        0        0     1139 2022-11-04 05:28:45.000000 django-ipghrms-attendance-1.5/attendance/migrations/0004_alter_attendance_is_present_attendancetotal.py
+-rw-rw-rw-   0        0        0      782 2022-11-04 05:28:45.000000 django-ipghrms-attendance-1.5/attendance/migrations/0005_attendance_month_attendance_year.py
+-rw-rw-rw-   0        0        0      731 2022-11-04 05:28:45.000000 django-ipghrms-attendance-1.5/attendance/migrations/0006_alter_attendancetotal_month_and_more.py
+-rw-rw-rw-   0        0        0      451 2022-11-04 05:28:45.000000 django-ipghrms-attendance-1.5/attendance/migrations/0007_alter_attendance_is_present.py
+-rw-rw-rw-   0        0        0      724 2022-11-04 05:28:45.000000 django-ipghrms-attendance-1.5/attendance/migrations/0008_alter_attendanceunit_month_alter_attendanceunit_year.py
+-rw-rw-rw-   0        0        0      611 2022-11-04 05:28:45.000000 django-ipghrms-attendance-1.5/attendance/migrations/0009_attendancetotal_unit.py
+-rw-rw-rw-   0        0        0      655 2022-11-22 01:39:19.000000 django-ipghrms-attendance-1.5/attendance/migrations/0010_alter_attendanceunit_file.py
+-rw-rw-rw-   0        0        0      669 2022-12-08 01:56:49.000000 django-ipghrms-attendance-1.5/attendance/migrations/0011_auto_20221208_1056.py
+-rw-rw-rw-   0        0        0      737 2022-12-08 03:51:53.000000 django-ipghrms-attendance-1.5/attendance/migrations/0012_auto_20221208_1251.py
+-rw-rw-rw-   0        0        0      460 2022-12-08 04:13:59.000000 django-ipghrms-attendance-1.5/attendance/migrations/0013_auto_20221208_1313.py
+-rw-rw-rw-   0        0        0      622 2022-12-08 17:13:59.000000 django-ipghrms-attendance-1.5/attendance/migrations/0014_attendance_leader.py
+-rw-rw-rw-   0        0        0     3002 2022-12-09 06:36:09.000000 django-ipghrms-attendance-1.5/attendance/migrations/0015_auto_20221209_1536.py
+-rw-rw-rw-   0        0        0      959 2022-12-10 13:58:18.000000 django-ipghrms-attendance-1.5/attendance/migrations/0016_auto_20221210_2258.py
+-rw-rw-rw-   0        0        0      659 2022-12-12 06:02:42.000000 django-ipghrms-attendance-1.5/attendance/migrations/0017_auto_20221212_1502.py
+-rw-rw-rw-   0        0        0      448 2022-12-12 07:36:13.000000 django-ipghrms-attendance-1.5/attendance/migrations/0018_alter_attendance_totat_hour.py
+-rw-rw-rw-   0        0        0      447 2023-02-15 10:11:30.000000 django-ipghrms-attendance-1.5/attendance/migrations/0019_attendance_is_hr_update.py
+-rw-rw-rw-   0        0        0      446 2023-02-15 10:15:09.000000 django-ipghrms-attendance-1.5/attendance/migrations/0020_alter_attendance_is_hr_update.py
+-rw-rw-rw-   0        0        0     1054 2023-02-15 10:23:09.000000 django-ipghrms-attendance-1.5/attendance/migrations/0021_auto_20230215_1923.py
+-rw-rw-rw-   0        0        0        0 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.5/attendance/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 12:54:19.993650 django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/
+-rw-rw-rw-   0        0        0     2628 2022-11-07 13:19:40.000000 django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0001_initial.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2598 2022-10-20 01:03:56.000000 django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0001_initial.cpython-37.pyc
+-rw-rw-rw-   0        0        0     2632 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0001_initial.cpython-39.pyc
+-rw-rw-rw-   0        0        0      691 2022-11-07 13:19:40.000000 django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0002_alter_attendance_time_am_alter_attendance_time_pm.cpython-310.pyc
+-rw-rw-rw-   0        0        0      675 2022-10-20 01:03:56.000000 django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0002_alter_attendance_time_am_alter_attendance_time_pm.cpython-37.pyc
+-rw-rw-rw-   0        0        0      695 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0002_alter_attendance_time_am_alter_attendance_time_pm.cpython-39.pyc
+-rw-rw-rw-   0        0        0      755 2022-11-07 13:19:40.000000 django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0003_alter_attendance_time_am_alter_attendance_time_pm.cpython-310.pyc
+-rw-rw-rw-   0        0        0      739 2022-10-20 01:03:56.000000 django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0003_alter_attendance_time_am_alter_attendance_time_pm.cpython-37.pyc
+-rw-rw-rw-   0        0        0      759 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0003_alter_attendance_time_am_alter_attendance_time_pm.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1180 2022-11-07 13:19:40.000000 django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0004_alter_attendance_is_present_attendancetotal.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1162 2022-11-05 14:52:09.000000 django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0004_alter_attendance_is_present_attendancetotal.cpython-37.pyc
+-rw-rw-rw-   0        0        0      821 2022-11-07 13:19:40.000000 django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0005_attendance_month_attendance_year.cpython-310.pyc
+-rw-rw-rw-   0        0        0      805 2022-11-05 14:52:09.000000 django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0005_attendance_month_attendance_year.cpython-37.pyc
+-rw-rw-rw-   0        0        0      810 2022-11-07 13:19:40.000000 django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0006_alter_attendancetotal_month_and_more.cpython-310.pyc
+-rw-rw-rw-   0        0        0      794 2022-11-05 14:52:09.000000 django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0006_alter_attendancetotal_month_and_more.cpython-37.pyc
+-rw-rw-rw-   0        0        0      652 2022-11-07 13:19:40.000000 django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0007_alter_attendance_is_present.cpython-310.pyc
+-rw-rw-rw-   0        0        0      638 2022-11-05 14:52:09.000000 django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0007_alter_attendance_is_present.cpython-37.pyc
+-rw-rw-rw-   0        0        0      820 2022-11-07 13:19:40.000000 django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0008_alter_attendanceunit_month_alter_attendanceunit_year.cpython-310.pyc
+-rw-rw-rw-   0        0        0      804 2022-11-05 14:52:09.000000 django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0008_alter_attendanceunit_month_alter_attendanceunit_year.cpython-37.pyc
+-rw-rw-rw-   0        0        0      808 2022-11-07 13:19:40.000000 django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0009_attendancetotal_unit.cpython-310.pyc
+-rw-rw-rw-   0        0        0      794 2022-11-05 14:52:09.000000 django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0009_attendancetotal_unit.cpython-37.pyc
+-rw-rw-rw-   0        0        0      875 2022-11-22 01:39:26.000000 django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0010_alter_attendanceunit_file.cpython-310.pyc
+-rw-rw-rw-   0        0        0      702 2022-12-08 01:56:57.000000 django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0011_auto_20221208_1056.cpython-310.pyc
+-rw-rw-rw-   0        0        0      666 2022-12-08 03:51:59.000000 django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0012_auto_20221208_1251.cpython-310.pyc
+-rw-rw-rw-   0        0        0      546 2022-12-08 04:14:06.000000 django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0013_auto_20221208_1313.cpython-310.pyc
+-rw-rw-rw-   0        0        0      792 2022-12-08 17:14:03.000000 django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0014_attendance_leader.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1636 2022-12-09 06:36:18.000000 django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0015_auto_20221209_1536.cpython-310.pyc
+-rw-rw-rw-   0        0        0      801 2022-12-10 13:58:24.000000 django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0016_auto_20221210_2258.cpython-310.pyc
+-rw-rw-rw-   0        0        0      690 2022-12-12 06:02:48.000000 django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0017_auto_20221212_1502.cpython-310.pyc
+-rw-rw-rw-   0        0        0      629 2022-12-12 07:36:17.000000 django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0018_alter_attendance_totat_hour.cpython-310.pyc
+-rw-rw-rw-   0        0        0      620 2023-02-15 10:11:39.000000 django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0019_attendance_is_hr_update.cpython-310.pyc
+-rw-rw-rw-   0        0        0      625 2023-02-15 10:15:13.000000 django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0020_alter_attendance_is_hr_update.cpython-310.pyc
+-rw-rw-rw-   0        0        0      796 2023-02-15 10:23:13.000000 django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0021_auto_20230215_1923.cpython-310.pyc
+-rw-rw-rw-   0        0        0      150 2022-11-07 13:19:40.000000 django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      148 2022-10-20 01:03:56.000000 django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0      156 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     6910 2023-03-22 07:29:58.000000 django-ipghrms-attendance-1.5/attendance/models.py
+drwxrwxrwx   0        0        0        0 2023-06-13 12:54:19.351902 django-ipghrms-attendance-1.5/attendance/templates/
+drwxrwxrwx   0        0        0        0 2023-06-13 12:54:20.203139 django-ipghrms-attendance-1.5/attendance/templates/attendance/
+-rw-rw-rw-   0        0        0     1811 2023-03-27 00:57:38.000000 django-ipghrms-attendance-1.5/attendance/templates/attendance/dash.html
+-rw-rw-rw-   0        0        0     2757 2022-12-13 05:01:14.000000 django-ipghrms-attendance-1.5/attendance/templates/attendance/day_list.html
+-rw-rw-rw-   0        0        0     1256 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.5/attendance/templates/attendance/form_am-pm.html
+-rw-rw-rw-   0        0        0     1297 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.5/attendance/templates/attendance/form_emp.html
+-rw-rw-rw-   0        0        0     1103 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.5/attendance/templates/attendance/form_upload.html
+-rw-rw-rw-   0        0        0     2263 2023-02-15 09:23:11.000000 django-ipghrms-attendance-1.5/attendance/templates/attendance/import.html
+-rw-rw-rw-   0        0        0     2412 2023-02-08 06:02:53.000000 django-ipghrms-attendance-1.5/attendance/templates/attendance/list.html
+-rw-rw-rw-   0        0        0     4124 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.5/attendance/templates/attendance/unit_date_emp.html
+-rw-rw-rw-   0        0        0     3645 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.5/attendance/templates/attendance/unit_day_emp.html
+-rw-rw-rw-   0        0        0     4807 2022-12-12 12:51:19.000000 django-ipghrms-attendance-1.5/attendance/templates/attendance/unit_emp_date.html
+-rw-rw-rw-   0        0        0    17366 2023-03-13 01:04:46.000000 django-ipghrms-attendance-1.5/attendance/templates/attendance/unit_list.html
+drwxrwxrwx   0        0        0        0 2023-06-13 12:54:20.552776 django-ipghrms-attendance-1.5/attendance/templates/attendance_back/
+-rw-rw-rw-   0        0        0     3650 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.5/attendance/templates/attendance_back/adv_day_emp.html
+-rw-rw-rw-   0        0        0     4678 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.5/attendance/templates/attendance_back/adv_list.html
+-rw-rw-rw-   0        0        0     1539 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.5/attendance/templates/attendance_back/dash.html
+-rw-rw-rw-   0        0        0     2015 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.5/attendance/templates/attendance_back/dash_back.html
+-rw-rw-rw-   0        0        0     3650 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.5/attendance/templates/attendance_back/dg_day_emp.html
+-rw-rw-rw-   0        0        0     3125 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.5/attendance/templates/attendance_back/dg_emp_date.html
+-rw-rw-rw-   0        0        0     4688 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.5/attendance/templates/attendance_back/dg_list.html
+-rw-rw-rw-   0        0        0     3740 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.5/attendance/templates/attendance_back/div_date_emp.html
+-rw-rw-rw-   0        0        0     3654 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.5/attendance/templates/attendance_back/div_day_emp.html
+-rw-rw-rw-   0        0        0     3133 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.5/attendance/templates/attendance_back/div_emp_date.html
+-rw-rw-rw-   0        0        0     4731 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.5/attendance/templates/attendance_back/div_list.html
+-rw-rw-rw-   0        0        0     1266 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.5/attendance/templates/attendance_back/form_am-pm.html
+-rw-rw-rw-   0        0        0     1306 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.5/attendance/templates/attendance_back/form_emp.html
+-rw-rw-rw-   0        0        0     1112 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.5/attendance/templates/attendance_back/form_upload.html
+drwxrwxrwx   0        0        0        0 2023-06-13 12:54:20.630330 django-ipghrms-attendance-1.5/attendance/templates/attendance_custom/
+-rw-rw-rw-   0        0        0     3859 2023-02-08 05:57:14.000000 django-ipghrms-attendance-1.5/attendance/templates/attendance_custom/dash.html
+-rw-rw-rw-   0        0        0     1275 2023-02-08 05:55:54.000000 django-ipghrms-attendance-1.5/attendance/templates/attendance_custom/form.html
+-rw-rw-rw-   0        0        0     2001 2023-02-08 05:53:02.000000 django-ipghrms-attendance-1.5/attendance/templates/attendance_custom/list.html
+-rw-rw-rw-   0        0        0      794 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.5/attendance/templates/attendance_custom/year.html
+drwxrwxrwx   0        0        0        0 2023-06-13 12:54:20.713599 django-ipghrms-attendance-1.5/attendance/templates/attendance_print/
+-rw-rw-rw-   0        0        0     2294 2022-11-30 08:00:13.000000 django-ipghrms-attendance-1.5/attendance/templates/attendance_print/layout.html
+-rw-rw-rw-   0        0        0     5520 2023-02-08 05:04:16.000000 django-ipghrms-attendance-1.5/attendance/templates/attendance_print/print_attend.html
+-rw-rw-rw-   0        0        0     2199 2023-01-07 14:02:48.000000 django-ipghrms-attendance-1.5/attendance/templates/attendance_print/print_r_emp.html
+-rw-rw-rw-   0        0        0     4250 2023-02-08 05:30:25.000000 django-ipghrms-attendance-1.5/attendance/templates/attendance_print/print_r_lic_fal.html
+drwxrwxrwx   0        0        0        0 2023-06-13 12:54:20.833020 django-ipghrms-attendance-1.5/attendance/templates/attendance_report/
+-rw-rw-rw-   0        0        0     2574 2023-02-08 05:12:58.000000 django-ipghrms-attendance-1.5/attendance/templates/attendance_report/r_dash.html
+-rw-rw-rw-   0        0        0     9471 2023-01-31 03:48:50.000000 django-ipghrms-attendance-1.5/attendance/templates/attendance_report/r_emp_dash.html
+-rw-rw-rw-   0        0        0     2870 2023-02-08 05:17:39.000000 django-ipghrms-attendance-1.5/attendance/templates/attendance_report/r_emp_search.html
+-rw-rw-rw-   0        0        0     1410 2023-02-08 05:28:53.000000 django-ipghrms-attendance-1.5/attendance/templates/attendance_report/r_licfal_year.html
+-rw-rw-rw-   0        0        0    18080 2023-03-13 20:46:15.000000 django-ipghrms-attendance-1.5/attendance/templates/attendance_report/r_unit_dash.html
+-rw-rw-rw-   0        0        0    17991 2023-03-13 20:49:02.000000 django-ipghrms-attendance-1.5/attendance/templates/attendance_report/r_unit_list.html
+-rw-rw-rw-   0        0        0       60 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.5/attendance/tests.py
+-rw-rw-rw-   0        0        0     3707 2023-02-08 05:58:11.000000 django-ipghrms-attendance-1.5/attendance/urls.py
+-rw-rw-rw-   0        0        0     1462 2023-01-31 03:45:05.000000 django-ipghrms-attendance-1.5/attendance/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-13 12:54:20.883612 django-ipghrms-attendance-1.5/attendance/views/
+-rw-rw-rw-   0        0        0      148 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.5/attendance/views/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 12:54:21.312511 django-ipghrms-attendance-1.5/attendance/views/__pycache__/
+-rw-rw-rw-   0        0        0      275 2022-11-07 13:19:38.000000 django-ipghrms-attendance-1.5/attendance/views/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      273 2022-10-20 01:03:04.000000 django-ipghrms-attendance-1.5/attendance/views/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0      355 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.5/attendance/views/__pycache__/__init__.cpython-38.pyc
+-rw-rw-rw-   0        0        0      281 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.5/attendance/views/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3891 2023-02-08 05:31:42.000000 django-ipghrms-attendance-1.5/attendance/views/__pycache__/attend_custom.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4526 2022-11-05 14:50:11.000000 django-ipghrms-attendance-1.5/attendance/views/__pycache__/attend_custom.cpython-37.pyc
+-rw-rw-rw-   0        0        0     4300 2022-11-04 05:28:45.000000 django-ipghrms-attendance-1.5/attendance/views/__pycache__/attend_custom.cpython-39.pyc
+-rw-rw-rw-   0        0        0    12374 2023-02-15 10:14:59.000000 django-ipghrms-attendance-1.5/attendance/views/__pycache__/attend_m.cpython-310.pyc
+-rw-rw-rw-   0        0        0     9821 2022-11-07 06:12:38.000000 django-ipghrms-attendance-1.5/attendance/views/__pycache__/attend_m.cpython-37.pyc
+-rw-rw-rw-   0        0        0     9286 2022-11-04 05:28:45.000000 django-ipghrms-attendance-1.5/attendance/views/__pycache__/attend_m.cpython-39.pyc
+-rw-rw-rw-   0        0        0     4938 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.5/attendance/views/__pycache__/attend_unit.cpython-39.pyc
+-rw-rw-rw-   0        0        0     5849 2023-03-13 20:41:29.000000 django-ipghrms-attendance-1.5/attendance/views/__pycache__/attend_v.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3586 2022-11-05 14:50:11.000000 django-ipghrms-attendance-1.5/attendance/views/__pycache__/attend_v.cpython-37.pyc
+-rw-rw-rw-   0        0        0     3582 2022-11-04 05:28:45.000000 django-ipghrms-attendance-1.5/attendance/views/__pycache__/attend_v.cpython-39.pyc
+-rw-rw-rw-   0        0        0     9896 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.5/attendance/views/__pycache__/attendance.cpython-38.pyc
+-rw-rw-rw-   0        0        0     9728 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.5/attendance/views/__pycache__/attendance.cpython-39.pyc
+-rw-rw-rw-   0        0        0     4818 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.5/attendance/views/__pycache__/attendance_adv.cpython-38.pyc
+-rw-rw-rw-   0        0        0     5286 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.5/attendance/views/__pycache__/attendance_custom.cpython-38.pyc
+-rw-rw-rw-   0        0        0     3890 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.5/attendance/views/__pycache__/attendance_custom.cpython-39.pyc
+-rw-rw-rw-   0        0        0     4979 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.5/attendance/views/__pycache__/attendance_dg.cpython-38.pyc
+-rw-rw-rw-   0        0        0     4940 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.5/attendance/views/__pycache__/attendance_dg.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2321 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.5/attendance/views/__pycache__/attendance_report.cpython-38.pyc
+-rw-rw-rw-   0        0        0     5287 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.5/attendance/views/__pycache__/attendance_set.cpython-38.pyc
+-rw-rw-rw-   0        0        0     1726 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.5/attendance/views/__pycache__/export.cpython-38.pyc
+-rw-rw-rw-   0        0        0     1487 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.5/attendance/views/__pycache__/general.cpython-38.pyc
+-rw-rw-rw-   0        0        0      147 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.5/attendance/views/__pycache__/holiday.cpython-38.pyc
+-rw-rw-rw-   0        0        0     5313 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.5/attendance/views/__pycache__/leave.cpython-38.pyc
+-rw-rw-rw-   0        0        0     5963 2022-11-16 14:38:57.000000 django-ipghrms-attendance-1.5/attendance/views/__pycache__/print.cpython-310.pyc
+-rw-rw-rw-   0        0        0     6127 2022-11-07 09:08:07.000000 django-ipghrms-attendance-1.5/attendance/views/__pycache__/print.cpython-37.pyc
+-rw-rw-rw-   0        0        0     6276 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.5/attendance/views/__pycache__/print.cpython-38.pyc
+-rw-rw-rw-   0        0        0     5929 2022-11-04 05:28:45.000000 django-ipghrms-attendance-1.5/attendance/views/__pycache__/print.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2310 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.5/attendance/views/__pycache__/qrscanner.cpython-38.pyc
+-rw-rw-rw-   0        0        0     8596 2023-03-13 20:48:11.000000 django-ipghrms-attendance-1.5/attendance/views/__pycache__/reports.cpython-310.pyc
+-rw-rw-rw-   0        0        0     6021 2022-11-05 14:50:11.000000 django-ipghrms-attendance-1.5/attendance/views/__pycache__/reports.cpython-37.pyc
+-rw-rw-rw-   0        0        0     5836 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.5/attendance/views/__pycache__/reports.cpython-38.pyc
+-rw-rw-rw-   0        0        0     5964 2022-11-04 05:28:45.000000 django-ipghrms-attendance-1.5/attendance/views/__pycache__/reports.cpython-39.pyc
+-rw-rw-rw-   0        0        0     5220 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.5/attendance/views/__pycache__/reports_dg.cpython-38.pyc
+-rw-rw-rw-   0        0        0     4721 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.5/attendance/views/__pycache__/reports_div.cpython-38.pyc
+-rw-rw-rw-   0        0        0     5031 2023-03-13 20:43:37.000000 django-ipghrms-attendance-1.5/attendance/views/__pycache__/reports_unit.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4802 2022-10-20 01:03:04.000000 django-ipghrms-attendance-1.5/attendance/views/__pycache__/reports_unit.cpython-37.pyc
+-rw-rw-rw-   0        0        0     4808 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.5/attendance/views/__pycache__/reports_unit.cpython-39.pyc
+-rw-rw-rw-   0        0        0      148 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.5/attendance/views/__pycache__/timesheet.cpython-38.pyc
+-rw-rw-rw-   0        0        0     2215 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.5/attendance/views/__pycache__/webcam.cpython-38.pyc
+-rw-rw-rw-   0        0        0     4882 2023-02-08 05:31:36.000000 django-ipghrms-attendance-1.5/attendance/views/attend_custom.py
+-rw-rw-rw-   0        0        0    17127 2023-06-13 12:51:26.000000 django-ipghrms-attendance-1.5/attendance/views/attend_m.py
+-rw-rw-rw-   0        0        0     7058 2023-03-13 20:41:26.000000 django-ipghrms-attendance-1.5/attendance/views/attend_v.py
+-rw-rw-rw-   0        0        0     8638 2022-11-16 14:38:53.000000 django-ipghrms-attendance-1.5/attendance/views/print.py
+-rw-rw-rw-   0        0        0    11893 2023-03-13 20:48:08.000000 django-ipghrms-attendance-1.5/attendance/views/reports.py
+-rw-rw-rw-   0        0        0     6146 2023-03-13 20:43:34.000000 django-ipghrms-attendance-1.5/attendance/views/reports_unit.py
+-rw-rw-rw-   0        0        0       63 2022-10-18 10:39:30.000000 django-ipghrms-attendance-1.5/attendance/views.py
+drwxrwxrwx   0        0        0        0 2023-06-13 12:54:21.338760 django-ipghrms-attendance-1.5/django_ipghrms_attendance.egg-info/
+-rw-rw-rw-   0        0        0      953 2023-06-13 12:54:19.000000 django-ipghrms-attendance-1.5/django_ipghrms_attendance.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     9225 2023-06-13 12:54:19.000000 django-ipghrms-attendance-1.5/django_ipghrms_attendance.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 12:54:19.000000 django-ipghrms-attendance-1.5/django_ipghrms_attendance.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-13 12:54:19.000000 django-ipghrms-attendance-1.5/django_ipghrms_attendance.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      504 2023-06-13 12:54:21.357361 django-ipghrms-attendance-1.5/setup.cfg
+-rw-rw-rw-   0        0        0       39 2023-03-22 07:44:49.000000 django-ipghrms-attendance-1.5/setup.py
```

### Comparing `django-ipghrms-attendance-1.1/LICENSE` & `django-ipghrms-attendance-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/PKG-INFO` & `django-ipghrms-attendance-1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ipghrms-attendance
-Version: 1.1
+Version: 1.5
 Summary: Django IPG HRMS APP
 Home-page: http://ipg.tl/
 Author: Kinos
 Author-email: info@kinos.tl
 Maintainer: kinos
 Maintainer-email: info@kinos.tl
 License: MIT
```

### Comparing `django-ipghrms-attendance-1.1/README.rst` & `django-ipghrms-attendance-1.5/README.rst`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/forms.py` & `django-ipghrms-attendance-1.5/attendance/forms.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/migrations/0001_initial.py` & `django-ipghrms-attendance-1.5/attendance/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/migrations/0002_alter_attendance_time_am_alter_attendance_time_pm.py` & `django-ipghrms-attendance-1.5/attendance/migrations/0002_alter_attendance_time_am_alter_attendance_time_pm.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/migrations/0003_alter_attendance_time_am_alter_attendance_time_pm.py` & `django-ipghrms-attendance-1.5/attendance/migrations/0003_alter_attendance_time_am_alter_attendance_time_pm.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/migrations/0004_alter_attendance_is_present_attendancetotal.py` & `django-ipghrms-attendance-1.5/attendance/migrations/0004_alter_attendance_is_present_attendancetotal.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/migrations/0005_attendance_month_attendance_year.py` & `django-ipghrms-attendance-1.5/attendance/migrations/0005_attendance_month_attendance_year.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/migrations/0006_alter_attendancetotal_month_and_more.py` & `django-ipghrms-attendance-1.5/attendance/migrations/0006_alter_attendancetotal_month_and_more.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/migrations/0008_alter_attendanceunit_month_alter_attendanceunit_year.py` & `django-ipghrms-attendance-1.5/attendance/migrations/0008_alter_attendanceunit_month_alter_attendanceunit_year.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/migrations/0009_attendancetotal_unit.py` & `django-ipghrms-attendance-1.5/attendance/migrations/0009_attendancetotal_unit.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/migrations/0010_alter_attendanceunit_file.py` & `django-ipghrms-attendance-1.5/attendance/migrations/0010_alter_attendanceunit_file.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/migrations/0011_auto_20221208_1056.py` & `django-ipghrms-attendance-1.5/attendance/migrations/0011_auto_20221208_1056.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/migrations/0012_auto_20221208_1251.py` & `django-ipghrms-attendance-1.5/attendance/migrations/0012_auto_20221208_1251.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/migrations/0014_attendance_leader.py` & `django-ipghrms-attendance-1.5/attendance/migrations/0014_attendance_leader.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/migrations/0015_auto_20221209_1536.py` & `django-ipghrms-attendance-1.5/attendance/migrations/0015_auto_20221209_1536.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/migrations/0016_auto_20221210_2258.py` & `django-ipghrms-attendance-1.5/attendance/migrations/0016_auto_20221210_2258.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/migrations/0017_auto_20221212_1502.py` & `django-ipghrms-attendance-1.5/attendance/migrations/0017_auto_20221212_1502.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/migrations/0021_auto_20230215_1923.py` & `django-ipghrms-attendance-1.5/attendance/migrations/0021_auto_20230215_1923.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0001_initial.cpython-310.pyc` & `django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0001_initial.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0001_initial.cpython-37.pyc` & `django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0001_initial.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0001_initial.cpython-39.pyc` & `django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0001_initial.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0002_alter_attendance_time_am_alter_attendance_time_pm.cpython-310.pyc` & `django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0002_alter_attendance_time_am_alter_attendance_time_pm.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0002_alter_attendance_time_am_alter_attendance_time_pm.cpython-37.pyc` & `django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0002_alter_attendance_time_am_alter_attendance_time_pm.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0002_alter_attendance_time_am_alter_attendance_time_pm.cpython-39.pyc` & `django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0002_alter_attendance_time_am_alter_attendance_time_pm.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0003_alter_attendance_time_am_alter_attendance_time_pm.cpython-310.pyc` & `django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0003_alter_attendance_time_am_alter_attendance_time_pm.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0003_alter_attendance_time_am_alter_attendance_time_pm.cpython-37.pyc` & `django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0003_alter_attendance_time_am_alter_attendance_time_pm.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0003_alter_attendance_time_am_alter_attendance_time_pm.cpython-39.pyc` & `django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0003_alter_attendance_time_am_alter_attendance_time_pm.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0004_alter_attendance_is_present_attendancetotal.cpython-310.pyc` & `django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0004_alter_attendance_is_present_attendancetotal.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0004_alter_attendance_is_present_attendancetotal.cpython-37.pyc` & `django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0004_alter_attendance_is_present_attendancetotal.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0005_attendance_month_attendance_year.cpython-310.pyc` & `django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0005_attendance_month_attendance_year.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0005_attendance_month_attendance_year.cpython-37.pyc` & `django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0005_attendance_month_attendance_year.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0006_alter_attendancetotal_month_and_more.cpython-310.pyc` & `django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0006_alter_attendancetotal_month_and_more.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0006_alter_attendancetotal_month_and_more.cpython-37.pyc` & `django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0006_alter_attendancetotal_month_and_more.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0007_alter_attendance_is_present.cpython-310.pyc` & `django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0007_alter_attendance_is_present.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0007_alter_attendance_is_present.cpython-37.pyc` & `django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0007_alter_attendance_is_present.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0008_alter_attendanceunit_month_alter_attendanceunit_year.cpython-310.pyc` & `django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0008_alter_attendanceunit_month_alter_attendanceunit_year.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0008_alter_attendanceunit_month_alter_attendanceunit_year.cpython-37.pyc` & `django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0008_alter_attendanceunit_month_alter_attendanceunit_year.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0009_attendancetotal_unit.cpython-310.pyc` & `django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0009_attendancetotal_unit.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0009_attendancetotal_unit.cpython-37.pyc` & `django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0009_attendancetotal_unit.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0010_alter_attendanceunit_file.cpython-310.pyc` & `django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0010_alter_attendanceunit_file.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0011_auto_20221208_1056.cpython-310.pyc` & `django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0011_auto_20221208_1056.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0012_auto_20221208_1251.cpython-310.pyc` & `django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0012_auto_20221208_1251.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0013_auto_20221208_1313.cpython-310.pyc` & `django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0013_auto_20221208_1313.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0014_attendance_leader.cpython-310.pyc` & `django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0014_attendance_leader.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0015_auto_20221209_1536.cpython-310.pyc` & `django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0015_auto_20221209_1536.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0016_auto_20221210_2258.cpython-310.pyc` & `django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0016_auto_20221210_2258.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0017_auto_20221212_1502.cpython-310.pyc` & `django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0017_auto_20221212_1502.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0018_alter_attendance_totat_hour.cpython-310.pyc` & `django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0018_alter_attendance_totat_hour.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0019_attendance_is_hr_update.cpython-310.pyc` & `django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0019_attendance_is_hr_update.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0020_alter_attendance_is_hr_update.cpython-310.pyc` & `django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0020_alter_attendance_is_hr_update.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/migrations/__pycache__/0021_auto_20230215_1923.cpython-310.pyc` & `django-ipghrms-attendance-1.5/attendance/migrations/__pycache__/0021_auto_20230215_1923.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/models.py` & `django-ipghrms-attendance-1.5/attendance/models.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/templates/attendance/dash.html` & `django-ipghrms-attendance-1.5/attendance/templates/attendance/dash.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/templates/attendance/day_list.html` & `django-ipghrms-attendance-1.5/attendance/templates/attendance/day_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/templates/attendance/form_am-pm.html` & `django-ipghrms-attendance-1.5/attendance/templates/attendance/form_am-pm.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/templates/attendance/form_emp.html` & `django-ipghrms-attendance-1.5/attendance/templates/attendance/form_emp.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/templates/attendance/form_upload.html` & `django-ipghrms-attendance-1.5/attendance/templates/attendance/form_upload.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/templates/attendance/import.html` & `django-ipghrms-attendance-1.5/attendance/templates/attendance/import.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/templates/attendance/list.html` & `django-ipghrms-attendance-1.5/attendance/templates/attendance/list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/templates/attendance/unit_date_emp.html` & `django-ipghrms-attendance-1.5/attendance/templates/attendance/unit_date_emp.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/templates/attendance/unit_day_emp.html` & `django-ipghrms-attendance-1.5/attendance/templates/attendance/unit_day_emp.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/templates/attendance/unit_emp_date.html` & `django-ipghrms-attendance-1.5/attendance/templates/attendance/unit_emp_date.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/templates/attendance/unit_list.html` & `django-ipghrms-attendance-1.5/attendance/templates/attendance/unit_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/templates/attendance_back/adv_day_emp.html` & `django-ipghrms-attendance-1.5/attendance/templates/attendance_back/adv_day_emp.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/templates/attendance_back/adv_list.html` & `django-ipghrms-attendance-1.5/attendance/templates/attendance_back/adv_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/templates/attendance_back/dash.html` & `django-ipghrms-attendance-1.5/attendance/templates/attendance_back/dash.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/templates/attendance_back/dash_back.html` & `django-ipghrms-attendance-1.5/attendance/templates/attendance_back/dash_back.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/templates/attendance_back/dg_day_emp.html` & `django-ipghrms-attendance-1.5/attendance/templates/attendance_back/dg_day_emp.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/templates/attendance_back/dg_emp_date.html` & `django-ipghrms-attendance-1.5/attendance/templates/attendance_back/dg_emp_date.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/templates/attendance_back/dg_list.html` & `django-ipghrms-attendance-1.5/attendance/templates/attendance_back/dg_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/templates/attendance_back/div_date_emp.html` & `django-ipghrms-attendance-1.5/attendance/templates/attendance_back/div_date_emp.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/templates/attendance_back/div_day_emp.html` & `django-ipghrms-attendance-1.5/attendance/templates/attendance_back/div_day_emp.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/templates/attendance_back/div_emp_date.html` & `django-ipghrms-attendance-1.5/attendance/templates/attendance_back/div_emp_date.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/templates/attendance_back/div_list.html` & `django-ipghrms-attendance-1.5/attendance/templates/attendance_back/div_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/templates/attendance_back/form_am-pm.html` & `django-ipghrms-attendance-1.5/attendance/templates/attendance_back/form_am-pm.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/templates/attendance_back/form_emp.html` & `django-ipghrms-attendance-1.5/attendance/templates/attendance_back/form_emp.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/templates/attendance_back/form_upload.html` & `django-ipghrms-attendance-1.5/attendance/templates/attendance_back/form_upload.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/templates/attendance_custom/dash.html` & `django-ipghrms-attendance-1.5/attendance/templates/attendance_custom/dash.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/templates/attendance_custom/form.html` & `django-ipghrms-attendance-1.5/attendance/templates/attendance_custom/form.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/templates/attendance_custom/list.html` & `django-ipghrms-attendance-1.5/attendance/templates/attendance_custom/list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/templates/attendance_custom/year.html` & `django-ipghrms-attendance-1.5/attendance/templates/attendance_custom/year.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/templates/attendance_print/layout.html` & `django-ipghrms-attendance-1.5/attendance/templates/attendance_print/layout.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/templates/attendance_print/print_attend.html` & `django-ipghrms-attendance-1.5/attendance/templates/attendance_print/print_attend.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/templates/attendance_print/print_r_emp.html` & `django-ipghrms-attendance-1.5/attendance/templates/attendance_print/print_r_emp.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/templates/attendance_print/print_r_lic_fal.html` & `django-ipghrms-attendance-1.5/attendance/templates/attendance_print/print_r_lic_fal.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/templates/attendance_report/r_dash.html` & `django-ipghrms-attendance-1.5/attendance/templates/attendance_report/r_dash.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/templates/attendance_report/r_emp_dash.html` & `django-ipghrms-attendance-1.5/attendance/templates/attendance_report/r_emp_dash.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/templates/attendance_report/r_emp_search.html` & `django-ipghrms-attendance-1.5/attendance/templates/attendance_report/r_emp_search.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/templates/attendance_report/r_licfal_year.html` & `django-ipghrms-attendance-1.5/attendance/templates/attendance_report/r_licfal_year.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/templates/attendance_report/r_unit_dash.html` & `django-ipghrms-attendance-1.5/attendance/templates/attendance_report/r_unit_dash.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/templates/attendance_report/r_unit_list.html` & `django-ipghrms-attendance-1.5/attendance/templates/attendance_report/r_unit_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/urls.py` & `django-ipghrms-attendance-1.5/attendance/urls.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/utils.py` & `django-ipghrms-attendance-1.5/attendance/utils.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/views/__pycache__/attend_custom.cpython-310.pyc` & `django-ipghrms-attendance-1.5/attendance/views/__pycache__/attend_custom.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/views/__pycache__/attend_custom.cpython-37.pyc` & `django-ipghrms-attendance-1.5/attendance/views/__pycache__/attend_custom.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/views/__pycache__/attend_custom.cpython-39.pyc` & `django-ipghrms-attendance-1.5/attendance/views/__pycache__/attend_custom.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/views/__pycache__/attend_m.cpython-310.pyc` & `django-ipghrms-attendance-1.5/attendance/views/__pycache__/attend_m.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/views/__pycache__/attend_m.cpython-37.pyc` & `django-ipghrms-attendance-1.5/attendance/views/__pycache__/attend_m.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/views/__pycache__/attend_m.cpython-39.pyc` & `django-ipghrms-attendance-1.5/attendance/views/__pycache__/attend_m.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/views/__pycache__/attend_unit.cpython-39.pyc` & `django-ipghrms-attendance-1.5/attendance/views/__pycache__/attend_unit.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/views/__pycache__/attend_v.cpython-310.pyc` & `django-ipghrms-attendance-1.5/attendance/views/__pycache__/attend_v.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/views/__pycache__/attend_v.cpython-37.pyc` & `django-ipghrms-attendance-1.5/attendance/views/__pycache__/attend_v.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/views/__pycache__/attend_v.cpython-39.pyc` & `django-ipghrms-attendance-1.5/attendance/views/__pycache__/attend_v.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/views/__pycache__/attendance.cpython-38.pyc` & `django-ipghrms-attendance-1.5/attendance/views/__pycache__/attendance.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/views/__pycache__/attendance.cpython-39.pyc` & `django-ipghrms-attendance-1.5/attendance/views/__pycache__/attendance.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/views/__pycache__/attendance_adv.cpython-38.pyc` & `django-ipghrms-attendance-1.5/attendance/views/__pycache__/attendance_adv.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/views/__pycache__/attendance_custom.cpython-38.pyc` & `django-ipghrms-attendance-1.5/attendance/views/__pycache__/attendance_custom.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/views/__pycache__/attendance_custom.cpython-39.pyc` & `django-ipghrms-attendance-1.5/attendance/views/__pycache__/attendance_custom.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/views/__pycache__/attendance_dg.cpython-38.pyc` & `django-ipghrms-attendance-1.5/attendance/views/__pycache__/attendance_dg.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/views/__pycache__/attendance_dg.cpython-39.pyc` & `django-ipghrms-attendance-1.5/attendance/views/__pycache__/attendance_dg.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/views/__pycache__/attendance_report.cpython-38.pyc` & `django-ipghrms-attendance-1.5/attendance/views/__pycache__/attendance_report.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/views/__pycache__/attendance_set.cpython-38.pyc` & `django-ipghrms-attendance-1.5/attendance/views/__pycache__/attendance_set.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/views/__pycache__/export.cpython-38.pyc` & `django-ipghrms-attendance-1.5/attendance/views/__pycache__/export.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/views/__pycache__/general.cpython-38.pyc` & `django-ipghrms-attendance-1.5/attendance/views/__pycache__/general.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/views/__pycache__/leave.cpython-38.pyc` & `django-ipghrms-attendance-1.5/attendance/views/__pycache__/leave.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/views/__pycache__/print.cpython-310.pyc` & `django-ipghrms-attendance-1.5/attendance/views/__pycache__/print.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/views/__pycache__/print.cpython-37.pyc` & `django-ipghrms-attendance-1.5/attendance/views/__pycache__/print.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/views/__pycache__/print.cpython-38.pyc` & `django-ipghrms-attendance-1.5/attendance/views/__pycache__/print.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/views/__pycache__/print.cpython-39.pyc` & `django-ipghrms-attendance-1.5/attendance/views/__pycache__/print.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/views/__pycache__/qrscanner.cpython-38.pyc` & `django-ipghrms-attendance-1.5/attendance/views/__pycache__/qrscanner.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/views/__pycache__/reports.cpython-310.pyc` & `django-ipghrms-attendance-1.5/attendance/views/__pycache__/reports.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/views/__pycache__/reports.cpython-37.pyc` & `django-ipghrms-attendance-1.5/attendance/views/__pycache__/reports.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/views/__pycache__/reports.cpython-38.pyc` & `django-ipghrms-attendance-1.5/attendance/views/__pycache__/reports.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/views/__pycache__/reports.cpython-39.pyc` & `django-ipghrms-attendance-1.5/attendance/views/__pycache__/reports.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/views/__pycache__/reports_dg.cpython-38.pyc` & `django-ipghrms-attendance-1.5/attendance/views/__pycache__/reports_dg.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/views/__pycache__/reports_div.cpython-38.pyc` & `django-ipghrms-attendance-1.5/attendance/views/__pycache__/reports_div.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/views/__pycache__/reports_unit.cpython-310.pyc` & `django-ipghrms-attendance-1.5/attendance/views/__pycache__/reports_unit.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/views/__pycache__/reports_unit.cpython-37.pyc` & `django-ipghrms-attendance-1.5/attendance/views/__pycache__/reports_unit.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/views/__pycache__/reports_unit.cpython-39.pyc` & `django-ipghrms-attendance-1.5/attendance/views/__pycache__/reports_unit.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/views/__pycache__/webcam.cpython-38.pyc` & `django-ipghrms-attendance-1.5/attendance/views/__pycache__/webcam.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/views/attend_custom.py` & `django-ipghrms-attendance-1.5/attendance/views/attend_custom.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/views/attend_m.py` & `django-ipghrms-attendance-1.5/attendance/views/attend_m.py`

 * *Files 1% similar despite different names*

```diff
@@ -313,17 +313,23 @@
 	month = Month.objects.filter(is_active=True).first()
 	date1 = f'{year.year}-{month.pk}-{day}'
 	date1 = dt.strptime(date1, '%Y-%m-%d')
 	date1 = date1.strftime('%Y-%m-%d')
 	if request.method == 'POST':
 		csv_file = request.FILES['fupload']
 		if not csv_file.name.endswith('.csv'):
-			messages.error(request, f'The uploaded file should in CSV format.')
+			messages.error(request, 'The uploaded file should be in CSV format.')
 
-		data_set = pd.read_csv(csv_file)
+		# Convert bytes to string
+		csv_data = csv_file.read().decode('utf-8')
+
+		# Use StringIO to create a file-like object
+		csv_file_obj = io.StringIO(csv_data)
+
+		data_set = pd.read_csv(csv_file_obj, delimiter=',|;', engine='python')
 		df = pd.DataFrame(data_set, columns=['PIN', 'Nama Karyawan', 'Tanggal', 'Jam', 'Mode'])
 		df = df.assign(AbsenceIn=df['Mode'] == 'Scan Masuk')
 		df = df.assign(AbsenceOut=df['Mode'] == 'Scan Keluar')
 		df['time'] = pd.to_datetime(df['Jam']).dt.time
 		df['date'] = pd.to_datetime(df['Tanggal']).dt.date
 		date2 = df.iloc[-1]['date']
 		date2 = date2.strftime('%Y-%m-%d')
```

### Comparing `django-ipghrms-attendance-1.1/attendance/views/attend_v.py` & `django-ipghrms-attendance-1.5/attendance/views/attend_v.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/views/print.py` & `django-ipghrms-attendance-1.5/attendance/views/print.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/views/reports.py` & `django-ipghrms-attendance-1.5/attendance/views/reports.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/attendance/views/reports_unit.py` & `django-ipghrms-attendance-1.5/attendance/views/reports_unit.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-attendance-1.1/django_ipghrms_attendance.egg-info/PKG-INFO` & `django-ipghrms-attendance-1.5/django_ipghrms_attendance.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ipghrms-attendance
-Version: 1.1
+Version: 1.5
 Summary: Django IPG HRMS APP
 Home-page: http://ipg.tl/
 Author: Kinos
 Author-email: info@kinos.tl
 Maintainer: kinos
 Maintainer-email: info@kinos.tl
 License: MIT
```

### Comparing `django-ipghrms-attendance-1.1/django_ipghrms_attendance.egg-info/SOURCES.txt` & `django-ipghrms-attendance-1.5/django_ipghrms_attendance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

