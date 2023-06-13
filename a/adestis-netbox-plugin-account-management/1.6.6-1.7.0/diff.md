# Comparing `tmp/adestis-netbox-plugin-account-management-1.6.6.tar.gz` & `tmp/adestis-netbox-plugin-account-management-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adestis-netbox-plugin-account-management-1.6.6.tar", last modified: Tue May 30 15:03:40 2023, max compression
+gzip compressed data, was "adestis-netbox-plugin-account-management-1.7.0.tar", last modified: Tue Jun 13 09:32:12 2023, max compression
```

## Comparing `adestis-netbox-plugin-account-management-1.6.6.tar` & `adestis-netbox-plugin-account-management-1.7.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 15:03:40.007635 adestis-netbox-plugin-account-management-1.6.6/
--rw-rw-rw-   0        0        0     1088 2023-02-09 23:32:58.000000 adestis-netbox-plugin-account-management-1.6.6/LICENSE
--rw-rw-rw-   0        0        0      175 2023-05-30 11:37:32.000000 adestis-netbox-plugin-account-management-1.6.6/MANIFEST.in
--rw-rw-rw-   0        0        0      326 2023-05-30 15:03:39.988637 adestis-netbox-plugin-account-management-1.6.6/PKG-INFO
--rw-rw-rw-   0        0        0     1374 2023-05-30 11:37:32.000000 adestis-netbox-plugin-account-management-1.6.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 15:03:38.854226 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/
--rw-rw-rw-   0        0        0      494 2023-05-30 12:56:32.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-30 15:03:38.999538 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/api/
--rw-rw-rw-   0        0        0        0 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/api/__init__.py
--rw-rw-rw-   0        0        0      516 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/api/nested_serializer.py
--rw-rw-rw-   0        0        0     2693 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/api/serializers.py
--rw-rw-rw-   0        0        0      301 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/api/urls.py
--rw-rw-rw-   0        0        0      659 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/api/views.py
-drwxrwxrwx   0        0        0        0 2023-05-30 15:03:39.076328 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/filtersets/
--rw-rw-rw-   0        0        0       57 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/filtersets/__init__.py
--rw-rw-rw-   0        0        0     1899 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/filtersets/login_credentials.py
--rw-rw-rw-   0        0        0     2610 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/filtersets/system.py
-drwxrwxrwx   0        0        0        0 2023-05-30 15:03:39.148741 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/forms/
--rw-rw-rw-   0        0        0       57 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/forms/__init__.py
--rw-rw-rw-   0        0        0     4733 2023-05-30 12:18:13.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/forms/login_credentials.py
--rw-rw-rw-   0        0        0     8074 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/forms/system.py
--rw-rw-rw-   0        0        0      878 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/graphql.py
-drwxrwxrwx   0        0        0        0 2023-05-30 15:03:39.400424 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/migrations/
--rw-rw-rw-   0        0        0     4725 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      444 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/migrations/0002_alter_system_system_url.py
--rw-rw-rw-   0        0        0      756 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/migrations/0003_remove_logincredentials_adestis_netbox_plugin_account_management_logincredentials_unique_login_crede.py
--rw-rw-rw-   0        0        0     4163 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/migrations/0004_alter_logincredentials_options_alter_person_options_and_more.py
--rw-rw-rw-   0        0        0     1470 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/migrations/0005_person_mitigation.py
--rw-rw-rw-   0        0        0      761 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/migrations/0006_fix_constraint_logincredentials.py
--rw-rw-rw-   0        0        0      286 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/migrations/0007_remove_logincredentials_person.py
--rw-rw-rw-   0        0        0      662 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/migrations/0008_alter_logincredentials_contact.py
--rw-rw-rw-   0        0        0        0 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-30 15:03:39.512797 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/models/
--rw-rw-rw-   0        0        0       80 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/models/__init__.py
--rw-rw-rw-   0        0        0     3303 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/models/login_credentials.py
--rw-rw-rw-   0        0        0     2805 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/models/person.py
--rw-rw-rw-   0        0        0     3347 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/models/system.py
--rw-rw-rw-   0        0        0     1331 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/navigation.py
-drwxrwxrwx   0        0        0        0 2023-05-30 15:03:39.593633 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/tables/
--rw-rw-rw-   0        0        0       57 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/tables/__init__.py
--rw-rw-rw-   0        0        0      947 2023-05-30 14:24:33.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/tables/login_credentials.py
--rw-rw-rw-   0        0        0     1180 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/tables/system.py
-drwxrwxrwx   0        0        0        0 2023-05-30 15:03:38.721206 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/templates/
-drwxrwxrwx   0        0        0        0 2023-05-30 15:03:39.820637 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/templates/adestis_netbox_plugin_account_management/
--rw-rw-rw-   0        0        0      371 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/templates/adestis_netbox_plugin_account_management/device_login_credentials_table.html
--rw-rw-rw-   0        0        0     1685 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/templates/adestis_netbox_plugin_account_management/logincredentials.html
--rw-rw-rw-   0        0        0     2865 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/templates/adestis_netbox_plugin_account_management/system.html
--rw-rw-rw-   0        0        0     2110 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/urls.py
-drwxrwxrwx   0        0        0        0 2023-05-30 15:03:39.964632 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/views/
--rw-rw-rw-   0        0        0       57 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/views/__init__.py
--rw-rw-rw-   0        0        0     2544 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/views/login_credentials.py
--rw-rw-rw-   0        0        0     1734 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/views/system.py
-drwxrwxrwx   0        0        0        0 2023-05-30 15:03:38.911543 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management.egg-info/
--rw-rw-rw-   0        0        0      326 2023-05-30 15:03:37.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2988 2023-05-30 15:03:38.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 15:03:37.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-05-30 15:03:37.000000 adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-30 15:03:40.010641 adestis-netbox-plugin-account-management-1.6.6/setup.cfg
--rw-rw-rw-   0        0        0      602 2023-05-30 12:56:38.000000 adestis-netbox-plugin-account-management-1.6.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:32:12.248045 adestis-netbox-plugin-account-management-1.7.0/
+-rw-rw-rw-   0        0        0     1088 2023-02-09 23:32:58.000000 adestis-netbox-plugin-account-management-1.7.0/LICENSE
+-rw-rw-rw-   0        0        0      175 2023-05-30 11:37:32.000000 adestis-netbox-plugin-account-management-1.7.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      326 2023-06-13 09:32:12.236042 adestis-netbox-plugin-account-management-1.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1378 2023-06-13 09:11:18.000000 adestis-netbox-plugin-account-management-1.7.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 09:32:11.565044 adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/
+-rw-rw-rw-   0        0        0      494 2023-06-13 09:28:59.000000 adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:32:11.679076 adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/api/
+-rw-rw-rw-   0        0        0        0 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/api/__init__.py
+-rw-rw-rw-   0        0        0      516 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/api/nested_serializer.py
+-rw-rw-rw-   0        0        0     2693 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/api/serializers.py
+-rw-rw-rw-   0        0        0      301 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/api/urls.py
+-rw-rw-rw-   0        0        0      659 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/api/views.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:32:11.736043 adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/filtersets/
+-rw-rw-rw-   0        0        0       57 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/filtersets/__init__.py
+-rw-rw-rw-   0        0        0     1863 2023-06-13 09:24:28.000000 adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/filtersets/login_credentials.py
+-rw-rw-rw-   0        0        0     2537 2023-06-13 09:21:49.000000 adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/filtersets/system.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:32:11.792044 adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/forms/
+-rw-rw-rw-   0        0        0       57 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/forms/__init__.py
+-rw-rw-rw-   0        0        0     4762 2023-06-13 09:25:46.000000 adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/forms/login_credentials.py
+-rw-rw-rw-   0        0        0     7992 2023-06-13 09:26:12.000000 adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/forms/system.py
+-rw-rw-rw-   0        0        0      878 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/graphql.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:32:11.956042 adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/migrations/
+-rw-rw-rw-   0        0        0     4725 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      444 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/migrations/0002_alter_system_system_url.py
+-rw-rw-rw-   0        0        0      756 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/migrations/0003_remove_logincredentials_adestis_netbox_plugin_account_management_logincredentials_unique_login_crede.py
+-rw-rw-rw-   0        0        0     4163 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/migrations/0004_alter_logincredentials_options_alter_person_options_and_more.py
+-rw-rw-rw-   0        0        0     1470 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/migrations/0005_person_mitigation.py
+-rw-rw-rw-   0        0        0      761 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/migrations/0006_fix_constraint_logincredentials.py
+-rw-rw-rw-   0        0        0      286 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/migrations/0007_remove_logincredentials_person.py
+-rw-rw-rw-   0        0        0      662 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/migrations/0008_alter_logincredentials_contact.py
+-rw-rw-rw-   0        0        0        0 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:32:12.019056 adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/models/
+-rw-rw-rw-   0        0        0       80 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/models/__init__.py
+-rw-rw-rw-   0        0        0     3303 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/models/login_credentials.py
+-rw-rw-rw-   0        0        0     2805 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/models/person.py
+-rw-rw-rw-   0        0        0     3347 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/models/system.py
+-rw-rw-rw-   0        0        0     1331 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/navigation.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:32:12.122055 adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/tables/
+-rw-rw-rw-   0        0        0       57 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/tables/__init__.py
+-rw-rw-rw-   0        0        0      947 2023-06-13 08:57:21.000000 adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/tables/login_credentials.py
+-rw-rw-rw-   0        0        0     1180 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/tables/system.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:32:11.366901 adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/templates/
+drwxrwxrwx   0        0        0        0 2023-06-13 09:32:12.172045 adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/templates/adestis_netbox_plugin_account_management/
+-rw-rw-rw-   0        0        0      371 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/templates/adestis_netbox_plugin_account_management/device_login_credentials_table.html
+-rw-rw-rw-   0        0        0     1685 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/templates/adestis_netbox_plugin_account_management/logincredentials.html
+-rw-rw-rw-   0        0        0     2865 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/templates/adestis_netbox_plugin_account_management/system.html
+-rw-rw-rw-   0        0        0     2110 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/urls.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:32:12.224043 adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/views/
+-rw-rw-rw-   0        0        0       57 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/views/__init__.py
+-rw-rw-rw-   0        0        0     2544 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/views/login_credentials.py
+-rw-rw-rw-   0        0        0     1734 2023-05-30 11:40:21.000000 adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/views/system.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:32:11.620041 adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management.egg-info/
+-rw-rw-rw-   0        0        0      326 2023-06-13 09:32:10.000000 adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2988 2023-06-13 09:32:11.000000 adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 09:32:10.000000 adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-06-13 09:32:10.000000 adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 09:32:12.248045 adestis-netbox-plugin-account-management-1.7.0/setup.cfg
+-rw-rw-rw-   0        0        0      602 2023-06-13 09:28:59.000000 adestis-netbox-plugin-account-management-1.7.0/setup.py
```

### Comparing `adestis-netbox-plugin-account-management-1.6.6/LICENSE` & `adestis-netbox-plugin-account-management-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.6/README.md` & `adestis-netbox-plugin-account-management-1.7.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # NetBox Account Management
 
 A NetBox plugin for managing the ownership of accounts.
-Netbox `v3.4.4` is required.
+Netbox `v3.5-2.6.1` is required.
 
 # PIP Package
 
 [Click here](https://pypi.org/project/adestis-netbox-plugin-account-management/)
 
 ## Installation with Docker
```

### Comparing `adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/api/nested_serializer.py` & `adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/api/nested_serializer.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/api/serializers.py` & `adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/api/serializers.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/api/views.py` & `adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/api/views.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/filtersets/login_credentials.py` & `adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/filtersets/login_credentials.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from adestis_netbox_plugin_account_management.models import *
 from netbox.filtersets import NetBoxModelFilterSet
 from django.db.models import Q
 from django import forms
 import django_filters
 from django.utils.translation import gettext as _
-from utilities.forms import (
-    DynamicModelMultipleChoiceField, DatePicker,MultipleChoiceField, StaticSelect, TagFilterField, BOOLEAN_WITH_BLANK_CHOICES,
+from utilities.forms.fields import (
+    DynamicModelMultipleChoiceField
 )
+from utilities.forms.widgets import DatePicker
 from tenancy.models import *
 
 __all__ = (
     'LoginCredentialsFilterSet',
 )
```

### Comparing `adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/filtersets/system.py` & `adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/filtersets/system.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from netbox.filtersets import NetBoxModelFilterSet
 from django.db.models import Q
 
 from dcim.models import *
 from utilities.filters import TreeNodeMultipleChoiceFilter
 from django.utils.translation import gettext as _
 import django_filters
-from utilities.forms import (
-    DynamicModelMultipleChoiceField, MultipleChoiceField, StaticSelect, TagFilterField, BOOLEAN_WITH_BLANK_CHOICES,
+from utilities.forms.fields import (
+    DynamicModelMultipleChoiceField
 )
 from virtualization.models import VirtualMachine, ClusterGroup, Cluster
 from tenancy.models import *
 
 __all__ = (
     'SystemFilterSet',
 )
```

### Comparing `adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/forms/login_credentials.py` & `adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/forms/login_credentials.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from django import forms
 from django.core.exceptions import ValidationError
 from netbox.forms import NetBoxModelForm, NetBoxModelFilterSetForm, NetBoxModelBulkEditForm, NetBoxModelImportForm
-from utilities.forms.fields import CommentField, DynamicModelChoiceField
-from utilities.forms import DatePicker, DynamicModelMultipleChoiceField, CSVModelForm, CSVModelChoiceField, CSVChoiceField
+from utilities.forms.fields import CommentField, DynamicModelChoiceField, DynamicModelMultipleChoiceField
+from utilities.forms.widgets import DatePicker
+from utilities.forms.fields import CSVChoiceField, CSVModelChoiceField
 from adestis_netbox_plugin_account_management.models import *
 from tenancy.models import *
 from django.utils.translation import gettext as _
 
 __all__ = (
     'LoginCredentialsForm',
     'LoginCredentialsFilterForm',
```

### Comparing `adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/forms/system.py` & `adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/forms/system.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from django import forms
 from netbox.forms import NetBoxModelForm, NetBoxModelFilterSetForm, NetBoxModelBulkEditForm, NetBoxModelImportForm
-from utilities.forms.fields import CommentField
 from adestis_netbox_plugin_account_management.models import *
 from django.utils.translation import gettext as _
 from tenancy.models import *
 from dcim.models import *
-from utilities.forms import DynamicModelChoiceField, DynamicModelMultipleChoiceField, CommentField, DatePicker, CSVModelForm, CSVModelChoiceField, CSVChoiceField
+from utilities.forms.fields import DynamicModelChoiceField, DynamicModelMultipleChoiceField, CSVModelChoiceField, CSVChoiceField
 from virtualization.models import VirtualMachine, ClusterGroup, Cluster
 
 __all__ = (
     'SystemForm',
     'SystemFilterForm',
     'SystemBulkEditForm',
     'SystemCSVForm'
```

### Comparing `adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/graphql.py` & `adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/graphql.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/migrations/0001_initial.py` & `adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/migrations/0003_remove_logincredentials_adestis_netbox_plugin_account_management_logincredentials_unique_login_crede.py` & `adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/migrations/0003_remove_logincredentials_adestis_netbox_plugin_account_management_logincredentials_unique_login_crede.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/migrations/0004_alter_logincredentials_options_alter_person_options_and_more.py` & `adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/migrations/0004_alter_logincredentials_options_alter_person_options_and_more.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/migrations/0005_person_mitigation.py` & `adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/migrations/0005_person_mitigation.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/migrations/0006_fix_constraint_logincredentials.py` & `adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/migrations/0006_fix_constraint_logincredentials.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/migrations/0008_alter_logincredentials_contact.py` & `adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/migrations/0008_alter_logincredentials_contact.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/models/login_credentials.py` & `adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/models/login_credentials.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/models/person.py` & `adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/models/person.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/models/system.py` & `adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/models/system.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/navigation.py` & `adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/navigation.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/tables/login_credentials.py` & `adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/tables/login_credentials.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/tables/system.py` & `adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/tables/system.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/templates/adestis_netbox_plugin_account_management/logincredentials.html` & `adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/templates/adestis_netbox_plugin_account_management/logincredentials.html`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/templates/adestis_netbox_plugin_account_management/system.html` & `adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/templates/adestis_netbox_plugin_account_management/system.html`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/urls.py` & `adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/urls.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/views/login_credentials.py` & `adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/views/login_credentials.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management/views/system.py` & `adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management/views/system.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.6/adestis_netbox_plugin_account_management.egg-info/SOURCES.txt` & `adestis-netbox-plugin-account-management-1.7.0/adestis_netbox_plugin_account_management.egg-info/SOURCES.txt`

 * *Files identical despite different names*

