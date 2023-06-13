# Comparing `tmp/molecule-qemu-0.4.7.tar.gz` & `tmp/molecule-qemu-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molecule-qemu-0.4.7.tar", last modified: Tue Jun 13 07:37:52 2023, max compression
+gzip compressed data, was "molecule-qemu-0.4.8.tar", last modified: Tue Jun 13 07:38:05 2023, max compression
```

## Comparing `molecule-qemu-0.4.7.tar` & `molecule-qemu-0.4.8.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:52.329084 molecule-qemu-0.4.7/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-13 07:37:41.000000 molecule-qemu-0.4.7/.ansible-lint
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:52.321084 molecule-qemu-0.4.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:52.325084 molecule-qemu-0.4.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-13 07:37:41.000000 molecule-qemu-0.4.7/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-13 07:37:41.000000 molecule-qemu-0.4.7/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-13 07:37:41.000000 molecule-qemu-0.4.7/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-13 07:37:41.000000 molecule-qemu-0.4.7/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:52.325084 molecule-qemu-0.4.7/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-13 07:37:41.000000 molecule-qemu-0.4.7/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-13 07:37:41.000000 molecule-qemu-0.4.7/.yamllint
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-13 07:37:41.000000 molecule-qemu-0.4.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-13 07:37:41.000000 molecule-qemu-0.4.7/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-06-13 07:37:52.329084 molecule-qemu-0.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-06-13 07:37:41.000000 molecule-qemu-0.4.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:52.325084 molecule-qemu-0.4.7/molecule_qemu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:41.000000 molecule-qemu-0.4.7/molecule_qemu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:52.325084 molecule-qemu-0.4.7/molecule_qemu/cookiecutter/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-13 07:37:41.000000 molecule-qemu-0.4.7/molecule_qemu/cookiecutter/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:52.321084 molecule-qemu-0.4.7/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:52.325084 molecule-qemu-0.4.7/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-13 07:37:41.000000 molecule-qemu-0.4.7/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-13 07:37:41.000000 molecule-qemu-0.4.7/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/prepare.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-13 07:37:41.000000 molecule-qemu-0.4.7/molecule_qemu/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:52.329084 molecule-qemu-0.4.7/molecule_qemu/playbooks/
--rw-r--r--   0 runner    (1001) docker     (123)  2097152 2023-06-13 07:37:41.000000 molecule-qemu-0.4.7/molecule_qemu/playbooks/QEMU_EFI.fd
--rw-r--r--   0 runner    (1001) docker     (123)    13299 2023-06-13 07:37:41.000000 molecule-qemu-0.4.7/molecule_qemu/playbooks/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-06-13 07:37:41.000000 molecule-qemu-0.4.7/molecule_qemu/playbooks/destroy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:52.329084 molecule-qemu-0.4.7/molecule_qemu/playbooks/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-13 07:37:41.000000 molecule-qemu-0.4.7/molecule_qemu/playbooks/templates/meta-data.j2
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-13 07:37:41.000000 molecule-qemu-0.4.7/molecule_qemu/playbooks/templates/user-data.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:52.325084 molecule-qemu-0.4.7/molecule_qemu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-06-13 07:37:52.000000 molecule-qemu-0.4.7/molecule_qemu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-13 07:37:52.000000 molecule-qemu-0.4.7/molecule_qemu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 07:37:52.000000 molecule-qemu-0.4.7/molecule_qemu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-13 07:37:52.000000 molecule-qemu-0.4.7/molecule_qemu.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 07:37:52.000000 molecule-qemu-0.4.7/molecule_qemu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 07:37:52.000000 molecule-qemu-0.4.7/molecule_qemu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-13 07:37:41.000000 molecule-qemu-0.4.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-13 07:37:41.000000 molecule-qemu-0.4.7/requirements.yml
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-13 07:37:52.329084 molecule-qemu-0.4.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:38:05.525043 molecule-qemu-0.4.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-13 07:37:55.000000 molecule-qemu-0.4.8/.ansible-lint
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:38:05.517043 molecule-qemu-0.4.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:38:05.521043 molecule-qemu-0.4.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-13 07:37:55.000000 molecule-qemu-0.4.8/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-13 07:37:55.000000 molecule-qemu-0.4.8/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-13 07:37:55.000000 molecule-qemu-0.4.8/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-13 07:37:55.000000 molecule-qemu-0.4.8/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:38:05.521043 molecule-qemu-0.4.8/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-13 07:37:55.000000 molecule-qemu-0.4.8/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-13 07:37:55.000000 molecule-qemu-0.4.8/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-13 07:37:55.000000 molecule-qemu-0.4.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-13 07:37:55.000000 molecule-qemu-0.4.8/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-06-13 07:38:05.525043 molecule-qemu-0.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-06-13 07:37:55.000000 molecule-qemu-0.4.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:38:05.521043 molecule-qemu-0.4.8/molecule_qemu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:55.000000 molecule-qemu-0.4.8/molecule_qemu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:38:05.525043 molecule-qemu-0.4.8/molecule_qemu/cookiecutter/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-13 07:37:55.000000 molecule-qemu-0.4.8/molecule_qemu/cookiecutter/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:38:05.521043 molecule-qemu-0.4.8/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:38:05.525043 molecule-qemu-0.4.8/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-13 07:37:55.000000 molecule-qemu-0.4.8/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-13 07:37:55.000000 molecule-qemu-0.4.8/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/prepare.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-13 07:37:55.000000 molecule-qemu-0.4.8/molecule_qemu/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:38:05.525043 molecule-qemu-0.4.8/molecule_qemu/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (123)  2097152 2023-06-13 07:37:55.000000 molecule-qemu-0.4.8/molecule_qemu/playbooks/QEMU_EFI.fd
+-rw-r--r--   0 runner    (1001) docker     (123)    13317 2023-06-13 07:37:55.000000 molecule-qemu-0.4.8/molecule_qemu/playbooks/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-06-13 07:37:55.000000 molecule-qemu-0.4.8/molecule_qemu/playbooks/destroy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:38:05.525043 molecule-qemu-0.4.8/molecule_qemu/playbooks/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-13 07:37:55.000000 molecule-qemu-0.4.8/molecule_qemu/playbooks/templates/meta-data.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-13 07:37:55.000000 molecule-qemu-0.4.8/molecule_qemu/playbooks/templates/user-data.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:38:05.525043 molecule-qemu-0.4.8/molecule_qemu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-06-13 07:38:05.000000 molecule-qemu-0.4.8/molecule_qemu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-13 07:38:05.000000 molecule-qemu-0.4.8/molecule_qemu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 07:38:05.000000 molecule-qemu-0.4.8/molecule_qemu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-13 07:38:05.000000 molecule-qemu-0.4.8/molecule_qemu.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 07:38:05.000000 molecule-qemu-0.4.8/molecule_qemu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 07:38:05.000000 molecule-qemu-0.4.8/molecule_qemu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-13 07:37:55.000000 molecule-qemu-0.4.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-13 07:37:55.000000 molecule-qemu-0.4.8/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-13 07:38:05.525043 molecule-qemu-0.4.8/setup.cfg
```

### Comparing `molecule-qemu-0.4.7/.github/workflows/lint.yml` & `molecule-qemu-0.4.8/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.7/.github/workflows/publish.yml` & `molecule-qemu-0.4.8/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.7/.github/workflows/release.yml` & `molecule-qemu-0.4.8/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.7/.gitignore` & `molecule-qemu-0.4.8/.gitignore`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.7/.yamllint` & `molecule-qemu-0.4.8/.yamllint`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.7/LICENSE` & `molecule-qemu-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.7/Makefile` & `molecule-qemu-0.4.8/Makefile`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.7/PKG-INFO` & `molecule-qemu-0.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecule-qemu
-Version: 0.4.7
+Version: 0.4.8
 Summary: Molecule QEMU
 Author-email: Andrey Gubarev <andrey@andreygubarev.com>
 License: MIT
 Project-URL: Homepage, https://github.com/andreygubarev/molecule-qemu/
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `molecule-qemu-0.4.7/README.md` & `molecule-qemu-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.7/molecule_qemu/driver.py` & `molecule-qemu-0.4.8/molecule_qemu/driver.py`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.7/molecule_qemu/playbooks/QEMU_EFI.fd` & `molecule-qemu-0.4.8/molecule_qemu/playbooks/QEMU_EFI.fd`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.7/molecule_qemu/playbooks/create.yml` & `molecule-qemu-0.4.8/molecule_qemu/playbooks/create.yml`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
           "image": "{{ item.image }}",
           "image_checksum": "{{ item.image_checksum | default(omit) }}",
           "image_arch": "{{ item.image_arch | default(qemu_vm_image_arch) }}",
           "image_format": "{{ item.image_format | default(qemu_vm_image_format) }}",
 
           "ssh_port": "{{ item.ssh_port | default(22) }}",
-          "ssh_user": "{{ item.ssh_user }}",
+          "ssh_user": "{{ item.ssh_user | default('root') }}",
 
           "vm_cpus": "{{ item.vm_cpus | default(qemu_vm_cpus) }}",
           "vm_memory": "{{ item.vm_memory | default(qemu_vm_memory) }}",
           "vm_disk": "{{ item.vm_disk | default(qemu_vm_disk) }}",
           "vm_network": "{{ item.vm_network | default(qemu_vm_network) }}",
           "vm_network_mac": "{{ '52:54:00' | community.general.random_mac(seed=item.name | to_json | hash('md5')) | regex_replace('(^|:)0([0-9A-Fa-f])', '\\1\\2') }}",
```

### Comparing `molecule-qemu-0.4.7/molecule_qemu/playbooks/destroy.yml` & `molecule-qemu-0.4.8/molecule_qemu/playbooks/destroy.yml`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.7/molecule_qemu.egg-info/PKG-INFO` & `molecule-qemu-0.4.8/molecule_qemu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecule-qemu
-Version: 0.4.7
+Version: 0.4.8
 Summary: Molecule QEMU
 Author-email: Andrey Gubarev <andrey@andreygubarev.com>
 License: MIT
 Project-URL: Homepage, https://github.com/andreygubarev/molecule-qemu/
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `molecule-qemu-0.4.7/molecule_qemu.egg-info/SOURCES.txt` & `molecule-qemu-0.4.8/molecule_qemu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.4.7/pyproject.toml` & `molecule-qemu-0.4.8/pyproject.toml`

 * *Files identical despite different names*

