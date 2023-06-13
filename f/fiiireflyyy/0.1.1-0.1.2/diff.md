# Comparing `tmp/fiiireflyyy-0.1.1.tar.gz` & `tmp/fiiireflyyy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiiireflyyy-0.1.1.tar", last modified: Mon Mar 27 08:14:53 2023, max compression
+gzip compressed data, was "fiiireflyyy-0.1.2.tar", last modified: Tue Jun 13 12:17:05 2023, max compression
```

## Comparing `fiiireflyyy-0.1.1.tar` & `fiiireflyyy-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 wlutz     (1001) wlutz     (1001)        0 2023-03-27 08:14:53.634788 fiiireflyyy-0.1.1/
--rw-rw-r--   0 wlutz     (1001) wlutz     (1001)      656 2023-03-27 08:14:53.634788 fiiireflyyy-0.1.1/PKG-INFO
--rw-rw-r--   0 wlutz     (1001) wlutz     (1001)     6198 2023-01-20 12:02:35.000000 fiiireflyyy-0.1.1/README.txt
-drwxrwxr-x   0 wlutz     (1001) wlutz     (1001)        0 2023-03-27 08:14:53.634788 fiiireflyyy-0.1.1/fiiireflyyy/
--rw-rw-r--   0 wlutz     (1001) wlutz     (1001)       77 2023-01-20 12:02:35.000000 fiiireflyyy-0.1.1/fiiireflyyy/__init__.py
--rw-rw-r--   0 wlutz     (1001) wlutz     (1001)     4178 2023-02-08 16:04:10.000000 fiiireflyyy-0.1.1/fiiireflyyy/firefiles.py
--rw-rw-r--   0 wlutz     (1001) wlutz     (1001)    49937 2023-03-14 11:59:24.000000 fiiireflyyy-0.1.1/fiiireflyyy/firelearn.py
--rw-rw-r--   0 wlutz     (1001) wlutz     (1001)    14340 2023-03-14 11:30:31.000000 fiiireflyyy-0.1.1/fiiireflyyy/fireprocess.py
--rw-rw-r--   0 wlutz     (1001) wlutz     (1001)    15375 2023-03-27 08:11:34.000000 fiiireflyyy-0.1.1/fiiireflyyy/flimage.py
-drwxrwxr-x   0 wlutz     (1001) wlutz     (1001)        0 2023-03-27 08:14:53.634788 fiiireflyyy-0.1.1/fiiireflyyy.egg-info/
--rw-rw-r--   0 wlutz     (1001) wlutz     (1001)      656 2023-03-27 08:14:53.000000 fiiireflyyy-0.1.1/fiiireflyyy.egg-info/PKG-INFO
--rw-rw-r--   0 wlutz     (1001) wlutz     (1001)      327 2023-03-27 08:14:53.000000 fiiireflyyy-0.1.1/fiiireflyyy.egg-info/SOURCES.txt
--rw-rw-r--   0 wlutz     (1001) wlutz     (1001)        1 2023-03-27 08:14:53.000000 fiiireflyyy-0.1.1/fiiireflyyy.egg-info/dependency_links.txt
--rw-rw-r--   0 wlutz     (1001) wlutz     (1001)      116 2023-03-27 08:14:53.000000 fiiireflyyy-0.1.1/fiiireflyyy.egg-info/requires.txt
--rw-rw-r--   0 wlutz     (1001) wlutz     (1001)       12 2023-03-27 08:14:53.000000 fiiireflyyy-0.1.1/fiiireflyyy.egg-info/top_level.txt
--rw-rw-r--   0 wlutz     (1001) wlutz     (1001)       79 2023-03-27 08:14:53.634788 fiiireflyyy-0.1.1/setup.cfg
--rw-rw-r--   0 wlutz     (1001) wlutz     (1001)     1113 2023-03-27 08:12:49.000000 fiiireflyyy-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 12:17:05.458712 fiiireflyyy-0.1.2/
+-rw-rw-rw-   0        0        0      669 2023-06-13 12:17:05.459711 fiiireflyyy-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6290 2023-06-13 09:58:55.000000 fiiireflyyy-0.1.2/README.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 12:17:05.453710 fiiireflyyy-0.1.2/fiiireflyyy/
+-rw-rw-rw-   0        0        0      153 2023-06-13 12:11:31.000000 fiiireflyyy-0.1.2/fiiireflyyy/__init__.py
+-rw-rw-rw-   0        0        0     4312 2023-06-13 09:58:55.000000 fiiireflyyy-0.1.2/fiiireflyyy/firefiles.py
+-rw-rw-rw-   0        0        0    51273 2023-06-13 09:58:55.000000 fiiireflyyy-0.1.2/fiiireflyyy/firelearn.py
+-rw-rw-rw-   0        0        0    14713 2023-06-13 09:58:55.000000 fiiireflyyy-0.1.2/fiiireflyyy/fireprocess.py
+-rw-rw-rw-   0        0        0    15817 2023-06-13 09:58:55.000000 fiiireflyyy-0.1.2/fiiireflyyy/flimage.py
+-rw-rw-rw-   0        0        0      649 2023-06-13 12:15:44.000000 fiiireflyyy-0.1.2/fiiireflyyy/logic_gates.py
+drwxrwxrwx   0        0        0        0 2023-06-13 12:17:05.458712 fiiireflyyy-0.1.2/fiiireflyyy.egg-info/
+-rw-rw-rw-   0        0        0      669 2023-06-13 12:17:05.000000 fiiireflyyy-0.1.2/fiiireflyyy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2023-06-13 12:17:05.000000 fiiireflyyy-0.1.2/fiiireflyyy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 12:17:05.000000 fiiireflyyy-0.1.2/fiiireflyyy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      116 2023-06-13 12:17:05.000000 fiiireflyyy-0.1.2/fiiireflyyy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-13 12:17:05.000000 fiiireflyyy-0.1.2/fiiireflyyy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-13 12:17:05.462712 fiiireflyyy-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1113 2023-06-13 12:06:42.000000 fiiireflyyy-0.1.2/setup.py
```

### Comparing `fiiireflyyy-0.1.1/README.txt` & `fiiireflyyy-0.1.2/README.txt`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,92 +1,92 @@
-# FireLib
-
-
-
-## Getting started
-
-To make it easy for you to get started with GitLab, here's a list of recommended next steps.
-
-Already a pro? Just edit this README.md and make it your own. Want to make it easy? [Use the template at the bottom](#editing-this-readme)!
-
-## Add your files
-
-- [ ] [Create](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#create-a-file) or [upload](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#upload-a-file) files
-- [ ] [Add files using the command line](https://docs.gitlab.com/ee/gitlab-basics/add-file.html#add-a-file-using-the-command-line) or push an existing Git repository with the following command:
-
-```
-cd existing_repo
-git remote add origin https://gitlab.com/FiiireFlyyy/firelib.git
-git branch -M main
-git push -uf origin main
-```
-
-## Integrate with your tools
-
-- [ ] [Set up project integrations](https://gitlab.com/FiiireFlyyy/firelib/-/settings/integrations)
-
-## Collaborate with your team
-
-- [ ] [Invite team members and collaborators](https://docs.gitlab.com/ee/user/project/members/)
-- [ ] [Create a new merge request](https://docs.gitlab.com/ee/user/project/merge_requests/creating_merge_requests.html)
-- [ ] [Automatically close issues from merge requests](https://docs.gitlab.com/ee/user/project/issues/managing_issues.html#closing-issues-automatically)
-- [ ] [Enable merge request approvals](https://docs.gitlab.com/ee/user/project/merge_requests/approvals/)
-- [ ] [Automatically merge when pipeline succeeds](https://docs.gitlab.com/ee/user/project/merge_requests/merge_when_pipeline_succeeds.html)
-
-## Test and Deploy
-
-Use the built-in continuous integration in GitLab.
-
-- [ ] [Get started with GitLab CI/CD](https://docs.gitlab.com/ee/ci/quick_start/index.html)
-- [ ] [Analyze your code for known vulnerabilities with Static Application Security Testing(SAST)](https://docs.gitlab.com/ee/user/application_security/sast/)
-- [ ] [Deploy to Kubernetes, Amazon EC2, or Amazon ECS using Auto Deploy](https://docs.gitlab.com/ee/topics/autodevops/requirements.html)
-- [ ] [Use pull-based deployments for improved Kubernetes management](https://docs.gitlab.com/ee/user/clusters/agent/)
-- [ ] [Set up protected environments](https://docs.gitlab.com/ee/ci/environments/protected_environments.html)
-
-***
-
-# Editing this README
-
-When you're ready to make this README your own, just edit this file and use the handy template below (or feel free to structure it however you want - this is just a starting point!). Thank you to [makeareadme.com](https://www.makeareadme.com/) for this template.
-
-## Suggestions for a good README
-Every project is different, so consider which of these sections apply to yours. The sections used in the template are suggestions for most open source projects. Also keep in mind that while a README can be too long and detailed, too long is better than too short. If you think your README is too long, consider utilizing another form of documentation rather than cutting out information.
-
-## Name
-Choose a self-explaining name for your project.
-
-## Description
-Let people know what your project can do specifically. Provide context and add a link to any reference visitors might be unfamiliar with. A list of Features or a Background subsection can also be added here. If there are alternatives to your project, this is a good place to list differentiating factors.
-
-## Badges
-On some READMEs, you may see small images that convey metadata, such as whether or not all the tests are passing for the project. You can use Shields to add some to your README. Many services also have instructions for adding a badge.
-
-## Visuals
-Depending on what you are making, it can be a good idea to include screenshots or even a video (you'll frequently see GIFs rather than actual videos). Tools like ttygif can help, but check out Asciinema for a more sophisticated method.
-
-## Installation
-Within a particular ecosystem, there may be a common way of installing things, such as using Yarn, NuGet, or Homebrew. However, consider the possibility that whoever is reading your README is a novice and would like more guidance. Listing specific steps helps remove ambiguity and gets people to using your project as quickly as possible. If it only runs in a specific context like a particular programming language version or operating system or has dependencies that have to be installed manually, also add a Requirements subsection.
-
-## Usage
-Use examples liberally, and show the expected output if you can. It's helpful to have inline the smallest example of usage that you can demonstrate, while providing links to more sophisticated examples if they are too long to reasonably include in the README.
-
-## Support
-Tell people where they can go to for help. It can be any combination of an issue tracker, a chat room, an email address, etc.
-
-## Roadmap
-If you have ideas for releases in the future, it is a good idea to list them in the README.
-
-## Contributing
-State if you are open to contributions and what your requirements are for accepting them.
-
-For people who want to make changes to your project, it's helpful to have some documentation on how to get started. Perhaps there is a script that they should run or some environment variables that they need to set. Make these steps explicit. These instructions could also be useful to your future self.
-
-You can also document commands to lint the code or run tests. These steps help to ensure high code quality and reduce the likelihood that the changes inadvertently break something. Having instructions for running tests is especially helpful if it requires external setup, such as starting a Selenium server for testing in a browser.
-
-## Authors and acknowledgment
-Show your appreciation to those who have contributed to the project.
-
-## License
-For open source projects, say how it is licensed.
-
-## Project status
-If you have run out of energy or time for your project, put a note at the top of the README saying that development has slowed down or stopped completely. Someone may choose to fork your project or volunteer to step in as a maintainer or owner, allowing your project to keep going. You can also make an explicit request for maintainers.
+# FireLib
+
+
+
+## Getting started
+
+To make it easy for you to get started with GitLab, here's a list of recommended next steps.
+
+Already a pro? Just edit this README.md and make it your own. Want to make it easy? [Use the template at the bottom](#editing-this-readme)!
+
+## Add your files
+
+- [ ] [Create](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#create-a-file) or [upload](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#upload-a-file) files
+- [ ] [Add files using the command line](https://docs.gitlab.com/ee/gitlab-basics/add-file.html#add-a-file-using-the-command-line) or push an existing Git repository with the following command:
+
+```
+cd existing_repo
+git remote add origin https://gitlab.com/FiiireFlyyy/firelib.git
+git branch -M main
+git push -uf origin main
+```
+
+## Integrate with your tools
+
+- [ ] [Set up project integrations](https://gitlab.com/FiiireFlyyy/firelib/-/settings/integrations)
+
+## Collaborate with your team
+
+- [ ] [Invite team members and collaborators](https://docs.gitlab.com/ee/user/project/members/)
+- [ ] [Create a new merge request](https://docs.gitlab.com/ee/user/project/merge_requests/creating_merge_requests.html)
+- [ ] [Automatically close issues from merge requests](https://docs.gitlab.com/ee/user/project/issues/managing_issues.html#closing-issues-automatically)
+- [ ] [Enable merge request approvals](https://docs.gitlab.com/ee/user/project/merge_requests/approvals/)
+- [ ] [Automatically merge when pipeline succeeds](https://docs.gitlab.com/ee/user/project/merge_requests/merge_when_pipeline_succeeds.html)
+
+## Test and Deploy
+
+Use the built-in continuous integration in GitLab.
+
+- [ ] [Get started with GitLab CI/CD](https://docs.gitlab.com/ee/ci/quick_start/index.html)
+- [ ] [Analyze your code for known vulnerabilities with Static Application Security Testing(SAST)](https://docs.gitlab.com/ee/user/application_security/sast/)
+- [ ] [Deploy to Kubernetes, Amazon EC2, or Amazon ECS using Auto Deploy](https://docs.gitlab.com/ee/topics/autodevops/requirements.html)
+- [ ] [Use pull-based deployments for improved Kubernetes management](https://docs.gitlab.com/ee/user/clusters/agent/)
+- [ ] [Set up protected environments](https://docs.gitlab.com/ee/ci/environments/protected_environments.html)
+
+***
+
+# Editing this README
+
+When you're ready to make this README your own, just edit this file and use the handy template below (or feel free to structure it however you want - this is just a starting point!). Thank you to [makeareadme.com](https://www.makeareadme.com/) for this template.
+
+## Suggestions for a good README
+Every project is different, so consider which of these sections apply to yours. The sections used in the template are suggestions for most open source projects. Also keep in mind that while a README can be too long and detailed, too long is better than too short. If you think your README is too long, consider utilizing another form of documentation rather than cutting out information.
+
+## Name
+Choose a self-explaining name for your project.
+
+## Description
+Let people know what your project can do specifically. Provide context and add a link to any reference visitors might be unfamiliar with. A list of Features or a Background subsection can also be added here. If there are alternatives to your project, this is a good place to list differentiating factors.
+
+## Badges
+On some READMEs, you may see small images that convey metadata, such as whether or not all the tests are passing for the project. You can use Shields to add some to your README. Many services also have instructions for adding a badge.
+
+## Visuals
+Depending on what you are making, it can be a good idea to include screenshots or even a video (you'll frequently see GIFs rather than actual videos). Tools like ttygif can help, but check out Asciinema for a more sophisticated method.
+
+## Installation
+Within a particular ecosystem, there may be a common way of installing things, such as using Yarn, NuGet, or Homebrew. However, consider the possibility that whoever is reading your README is a novice and would like more guidance. Listing specific steps helps remove ambiguity and gets people to using your project as quickly as possible. If it only runs in a specific context like a particular programming language version or operating system or has dependencies that have to be installed manually, also add a Requirements subsection.
+
+## Usage
+Use examples liberally, and show the expected output if you can. It's helpful to have inline the smallest example of usage that you can demonstrate, while providing links to more sophisticated examples if they are too long to reasonably include in the README.
+
+## Support
+Tell people where they can go to for help. It can be any combination of an issue tracker, a chat room, an email address, etc.
+
+## Roadmap
+If you have ideas for releases in the future, it is a good idea to list them in the README.
+
+## Contributing
+State if you are open to contributions and what your requirements are for accepting them.
+
+For people who want to make changes to your project, it's helpful to have some documentation on how to get started. Perhaps there is a script that they should run or some environment variables that they need to set. Make these steps explicit. These instructions could also be useful to your future self.
+
+You can also document commands to lint the code or run tests. These steps help to ensure high code quality and reduce the likelihood that the changes inadvertently break something. Having instructions for running tests is especially helpful if it requires external setup, such as starting a Selenium server for testing in a browser.
+
+## Authors and acknowledgment
+Show your appreciation to those who have contributed to the project.
+
+## License
+For open source projects, say how it is licensed.
+
+## Project status
+If you have run out of energy or time for your project, put a note at the top of the README saying that development has slowed down or stopped completely. Someone may choose to fork your project or volunteer to step in as a maintainer or owner, allowing your project to keep going. You can also make an explicit request for maintainers.
```

### Comparing `fiiireflyyy-0.1.1/fiiireflyyy/firefiles.py` & `fiiireflyyy-0.1.2/fiiireflyyy/firefiles.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,134 +1,134 @@
-import os
-import shutil
-
-
-def get_all_parent_by_degree(directory, degree):
-    """
-    Return all the possible parents from a directory at a specific degree.
-
-        Parameters
-        ----------
-        directory : str.
-            the directory to find the specific parents from.
-        degree: int
-            The nth parents to look for.
-
-        Returns
-        -------
-        out: list of str
-            list of possible parents at degree n.
-    """
-    files = get_all_files(directory)
-
-    all_parents = []
-    for f in files:
-        all_parents.append(os.path.basename(nth_parent(f, degree)))
-
-    return all_parents
-
-
-def nth_parent(path, n):
-    return path if n <= 0 else os.path.dirname(nth_parent(path, n - 1))
-
-
-def get_all_files(directory):
-    """
-    Get all the files and subdirectories within a directory recursively
-
-        Parameters
-        ----------
-            directory: str.
-                the path of the directory to sparse
-
-        Returns
-        -------
-        out: list of str
-            list of all files under the directory.
-    """
-    all_paths = []
-    paths = []
-    subfolders = os.listdir(directory)
-    if len(subfolders) >= 1:
-        for subfolder in subfolders:
-            if os.path.isdir(os.path.join(directory, subfolder)):
-                paths = get_all_files(os.path.join(directory, subfolder))
-                for p in paths:
-                    all_paths.append(p)
-            else:
-                all_paths.append(os.path.join(directory, subfolder))
-
-    return all_paths
-
-
-def verify_dir(directory):
-    """
-    verify if the directory exists. If not, then create it.
-
-        Parameters
-        ----------
-        directory: str
-            the path of the directory to verify
-    """
-    isExist = os.path.exists(directory)
-    if not isExist:
-        os.makedirs(directory)
-
-
-def split_train_test():
-    base_path = "E:/HIV-AI Project/20220330 Trial Images/"
-    technique = base_path + "CNN"
-    train_ni_path = technique + "/Train/NI"
-    train_inf_path = technique + "/Train/INF"
-    test_ni_path = technique + "/Test/NI"
-    test_inf_path = technique + "/Test/INF"
-
-    basic_directories = (train_inf_path, train_ni_path, test_inf_path, test_ni_path)
-    for bd in basic_directories:
-        isExist = os.path.exists(bd)
-        if not isExist:
-            os.makedirs(bd)
-
-    all_images = get_all_files("E:/HIV-AI Project/20220330 Trial Images/PNG")
-    count_class_one = 0
-    count_class_two = 0
-    for image in all_images:
-        head, tail = os.path.split(image)
-        if "INF10^6" in image:
-            count_class_two += 1
-        elif "NI" in image:
-            count_class_one += 1
-
-    if count_class_two > count_class_one:  # getting the same number of entries for each class
-        count_class_two = count_class_one
-    else:
-        count_class_one = count_class_two
-
-    total_images = count_class_two + count_class_one
-    train_proportion = int(0.7 * total_images)
-    test_proportion = total_images - train_proportion
-
-    inf_train_index = 0
-    ni_train_index = 0
-    print(train_proportion)
-    for image in all_images:
-        head, tail = os.path.split(image)
-        if "INF10^6" in image and inf_train_index < train_proportion / 2:
-            print("train inf ", inf_train_index)
-            destination = train_inf_path + "/" + tail
-            shutil.copyfile(image, destination)
-            inf_train_index += 1
-        elif "NI" in image and ni_train_index < train_proportion / 2:
-            print("train ni ", ni_train_index)
-            destination = train_ni_path + "/" + tail
-            shutil.copyfile(image, destination)
-            ni_train_index += 1
-        elif "INF10^6" in image and inf_train_index >= train_proportion / 2:
-            print("test inf ", inf_train_index)
-            destination = test_inf_path + "/" + tail
-            shutil.copyfile(image, destination)
-            inf_train_index += 1
-        elif "NI" in image and ni_train_index >= train_proportion / 2:
-            print("test ni ", ni_train_index)
-            destination = test_ni_path + "/" + tail
-            shutil.copyfile(image, destination)
-            ni_train_index += 1
+import os
+import shutil
+
+
+def get_all_parent_by_degree(directory, degree):
+    """
+    Return all the possible parents from a directory at a specific degree.
+
+        Parameters
+        ----------
+        directory : str.
+            the directory to find the specific parents from.
+        degree: int
+            The nth parents to look for.
+
+        Returns
+        -------
+        out: list of str
+            list of possible parents at degree n.
+    """
+    files = get_all_files(directory)
+
+    all_parents = []
+    for f in files:
+        all_parents.append(os.path.basename(nth_parent(f, degree)))
+
+    return all_parents
+
+
+def nth_parent(path, n):
+    return path if n <= 0 else os.path.dirname(nth_parent(path, n - 1))
+
+
+def get_all_files(directory):
+    """
+    Get all the files and subdirectories within a directory recursively
+
+        Parameters
+        ----------
+            directory: str.
+                the path of the directory to sparse
+
+        Returns
+        -------
+        out: list of str
+            list of all files under the directory.
+    """
+    all_paths = []
+    paths = []
+    subfolders = os.listdir(directory)
+    if len(subfolders) >= 1:
+        for subfolder in subfolders:
+            if os.path.isdir(os.path.join(directory, subfolder)):
+                paths = get_all_files(os.path.join(directory, subfolder))
+                for p in paths:
+                    all_paths.append(p)
+            else:
+                all_paths.append(os.path.join(directory, subfolder))
+
+    return all_paths
+
+
+def verify_dir(directory):
+    """
+    verify if the directory exists. If not, then create it.
+
+        Parameters
+        ----------
+        directory: str
+            the path of the directory to verify
+    """
+    isExist = os.path.exists(directory)
+    if not isExist:
+        os.makedirs(directory)
+
+
+def split_train_test():
+    base_path = "E:/HIV-AI Project/20220330 Trial Images/"
+    technique = base_path + "CNN"
+    train_ni_path = technique + "/Train/NI"
+    train_inf_path = technique + "/Train/INF"
+    test_ni_path = technique + "/Test/NI"
+    test_inf_path = technique + "/Test/INF"
+
+    basic_directories = (train_inf_path, train_ni_path, test_inf_path, test_ni_path)
+    for bd in basic_directories:
+        isExist = os.path.exists(bd)
+        if not isExist:
+            os.makedirs(bd)
+
+    all_images = get_all_files("E:/HIV-AI Project/20220330 Trial Images/PNG")
+    count_class_one = 0
+    count_class_two = 0
+    for image in all_images:
+        head, tail = os.path.split(image)
+        if "INF10^6" in image:
+            count_class_two += 1
+        elif "NI" in image:
+            count_class_one += 1
+
+    if count_class_two > count_class_one:  # getting the same number of entries for each class
+        count_class_two = count_class_one
+    else:
+        count_class_one = count_class_two
+
+    total_images = count_class_two + count_class_one
+    train_proportion = int(0.7 * total_images)
+    test_proportion = total_images - train_proportion
+
+    inf_train_index = 0
+    ni_train_index = 0
+    print(train_proportion)
+    for image in all_images:
+        head, tail = os.path.split(image)
+        if "INF10^6" in image and inf_train_index < train_proportion / 2:
+            print("train inf ", inf_train_index)
+            destination = train_inf_path + "/" + tail
+            shutil.copyfile(image, destination)
+            inf_train_index += 1
+        elif "NI" in image and ni_train_index < train_proportion / 2:
+            print("train ni ", ni_train_index)
+            destination = train_ni_path + "/" + tail
+            shutil.copyfile(image, destination)
+            ni_train_index += 1
+        elif "INF10^6" in image and inf_train_index >= train_proportion / 2:
+            print("test inf ", inf_train_index)
+            destination = test_inf_path + "/" + tail
+            shutil.copyfile(image, destination)
+            inf_train_index += 1
+        elif "NI" in image and ni_train_index >= train_proportion / 2:
+            print("test ni ", ni_train_index)
+            destination = test_ni_path + "/" + tail
+            shutil.copyfile(image, destination)
+            ni_train_index += 1
```

### Comparing `fiiireflyyy-0.1.1/fiiireflyyy/firelearn.py` & `fiiireflyyy-0.1.2/fiiireflyyy/firelearn.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,1336 +1,1336 @@
-import os
-import pathlib
-import pickle
-import shutil
-import sys
-from random import randint
-
-import seaborn as sns
-from tensorflow import keras
-
-import matplotlib.pyplot as plt
-import numpy as np
-import pandas as pd
-import tensorflow as tf
-from keras import layers
-from keras.models import Sequential, Model, load_model
-from matplotlib import transforms
-from keras.preprocessing.image import ImageDataGenerator
-from keras.layers import Dense, Conv2D, MaxPool2D, Flatten, Dropout
-from keras.callbacks import CSVLogger
-from keras.utils.np_utils import to_categorical
-from tensorflow.keras.optimizers import Adam
-
-from matplotlib.collections import PathCollection
-from matplotlib.legend_handler import HandlerPathCollection, HandlerLine2D
-from matplotlib.patches import Ellipse
-from sklearn.decomposition import PCA
-from sklearn.ensemble import RandomForestClassifier
-from sklearn.model_selection import train_test_split
-from sklearn.preprocessing import StandardScaler
-from umap import UMAP
-
-from fiiireflyyy import firefiles as ff
-
-
-def k_fold_cross_validation_deprecated(k_fold, x, y, clf=None, loading=False, clf_path=''):
-    """
-    DEPRECATED - Compute a K-fold cross validation method.
-
-    :param k_fold: Number of folds to split the dataset
-    :param x: Features dataset
-    :param y: target dataset
-    :param clf: classifier object, if loading is False.
-    :param clf_path: path of a classifier object, if loading is True.
-    :param loading: Whether to load a classifier object from path or not.
-    :return: k-fold scores, accuracy
-    """
-    if len(x) != len(y):
-        raise ValueError("Features and Targets do not have the same length.")
-
-    data_len = len(y)
-
-    if loading:
-        if clf_path == '':
-            raise ValueError('No classifier path specified.')
-        else:
-            clf = pickle.load(open(clf_path, "rb"))
-    elif clf is None:
-        raise ValueError("no classifier object specified.")
-
-    ori_x_train, ori_x_test, ori_y_train, ori_y_test = train_test_split(x, y, test_size=0.3)
-    train_len = len(ori_y_train)
-    test_len = len(ori_y_test)
-    local_scores = []
-    step = int(train_len / k_fold)
-    clf.fit(ori_x_train, ori_y_train)
-    for k in range(0, train_len - step, step):
-        x_train_split = ori_x_train.iloc[k:k + step]
-        y_train_split = ori_y_train.iloc[k:k + step]
-        y_test_split = pd.concat([ori_y_test.iloc[0:k], ori_y_test.iloc[k + step:data_len]])
-        x_test_split = pd.concat([ori_x_test.iloc[0:k], ori_x_test.iloc[k + step:data_len]])
-        # clf.fit(x_train_split, y_train_split)
-        local_scores.append(clf.score(x_test_split, y_test_split))
-
-    return local_scores
-
-
-def generate_classes(data_dir, destination, targets):
-    """
-    Generate a specific folder structure for Keras models by isolating classes as different folders.
-
-    :param data_dir:
-    :type data_dir: str
-    :param destination: Where to generate the classes folders
-    :type destination: str
-    :param targets: the different classes to use
-    :type targets: str
-    :return:
-    """
-    ff.verify_dir(destination)
-    files = ff.get_all_files(data_dir)
-
-    # Creating directories architecture for keras model
-    for target in targets:
-        ff.verify_dir(os.path.join(destination, target))
-
-        for file in files:
-            if target in file:
-                shutil.copy2(file, os.path.join(destination, target))
-
-
-def basic_keras(model_spec, src, dst, img_size, epochs=10, visualize=False, saving=True):
-    """
-    Compute a basic Keras model for a images binary classification problem.
-
-    :param model_spec: the name of the model. Identical to the root folder that will contain the model.
-    :type model_spec: str
-    :param src: Where to find the data.
-    :type src: str
-    :param dst: Where to save the sorted data
-    :type dst: str
-    :param img_size: the size of the image.
-    :type img_size: tuple[int]
-    :param epochs: The number of epochs of the model. Default at 10.
-    :param visualize: To visualize the model's results
-    :type visualize: bool
-    :param saving: To save the model's results
-    :type saving: bool
-    :return:
-    """
-    # generate_classes(src, dst, targets=['INF', 'NI'])
-    # Getting the dataset
-
-    data_dir = pathlib.Path(dst)
-    image_count = len(list(data_dir.glob('*.png')))
-    print(image_count)
-
-    # loading data
-    batch_size = 8
-    img_height = img_size[0]
-    img_width = img_size[1]
-
-    train_ds = tf.keras.utils.image_dataset_from_directory(
-        data_dir,
-        validation_split=0.2,
-        subset='training',
-        seed=123,
-        image_size=(img_height, img_width),
-        batch_size=batch_size)
-
-    val_ds = tf.keras.utils.image_dataset_from_directory(
-        data_dir,
-        validation_split=0.2,
-        subset='validation',
-        seed=123,
-        image_size=(img_height, img_width),
-        batch_size=batch_size)
-
-    class_names = train_ds.class_names
-    print(class_names)
-
-    # Visualizing data
-    if visualize:
-        plt.figure(figsize=(10, 10))
-        for images, labels in train_ds.take(1):
-            for i in range(9):
-                ax = plt.subplot(3, 3, i + 1)
-                plt.imshow(images[i].numpy().astype("uint8"))
-                plt.title(class_names[labels[i]])
-                plt.axis("off")
-        plt.show()
-
-    for image_batch, labels_batch in train_ds:
-        print(image_batch.shape)
-        print(labels_batch.shape)
-        break
-
-    # Configure the dataset for performance
-
-    AUTOTUNE = tf.data.AUTOTUNE
-
-    train_ds = train_ds.cache().shuffle(
-        1000)  # .prefetch(buffer_size=AUTOTUNE)  # Once loaded, keep the pictures in memory
-    val_ds = val_ds.cache().prefetch(buffer_size=AUTOTUNE)  # Overlaps data preprocessing/model execution while training
-
-    # Data augmentation
-    data_augmentation = keras.Sequential(
-        [
-            layers.RandomFlip("horizontal_and_vertical",
-                              input_shape=(img_height,
-                                           img_width,
-                                           3)),
-            layers.RandomRotation(1.0),
-            layers.RandomZoom(0.5),
-        ]
-    )
-
-    # Basic Keras model
-    num_classes = len(class_names)
-    model = Sequential([
-        data_augmentation,
-        layers.Rescaling(1. / 255),
-        layers.Conv2D(16, 3, padding='same', activation='relu'),
-        layers.MaxPooling2D(),
-        layers.Conv2D(32, 3, padding='same', activation='relu'),
-        layers.MaxPooling2D(),
-        layers.Conv2D(64, 3, padding='same', activation='relu'),
-        layers.MaxPooling2D(),
-        layers.Dropout(0.2),
-        layers.Flatten(),
-        layers.Dense(128, activation='relu'),
-        layers.Dense(num_classes, name="outputs")
-    ])
-
-    model.compile(optimizer='adam',
-                  loss=tf.keras.losses.SparseCategoricalCrossentropy(from_logits=True),
-                  metrics=['accuracy'])
-
-    model.summary()
-
-    # Train the model
-
-    history = model.fit(
-        train_ds,
-        validation_data=val_ds,
-        epochs=epochs
-    )
-
-    # Visualize training
-    acc = history.history['accuracy']
-    val_acc = history.history['val_accuracy']
-
-    loss = history.history['loss']
-    val_loss = history.history['val_loss']
-
-    epochs_range = range(epochs)
-
-    plt.figure(figsize=(8, 8))
-    plt.subplot(1, 2, 1)
-    plt.plot(epochs_range, acc, label='Training Accuracy')
-    plt.plot(epochs_range, val_acc, label='Validation Accuracy')
-    plt.legend(loc='lower right')
-    plt.title('Training and Validation Accuracy')
-
-    plt.subplot(1, 2, 2)
-    plt.plot(epochs_range, loss, label='Training Loss')
-    plt.plot(epochs_range, val_loss, label='Validation Loss')
-    plt.legend(loc='upper right')
-    plt.title('Training and Validation Loss')
-
-    save_path = os.path.join(os.path.join(pathlib.Path(dst).parent.parent.absolute(), "RESULTS"), model_spec,
-                             "training validation acc loss.png")
-    ff.verify_dir(os.path.join(os.path.join(pathlib.Path(dst).parent.parent.absolute(), "RESULTS"), model_spec))
-    if saving:
-        plt.savefig(save_path)
-    if visualize:
-        plt.show()
-    plt.close()
-
-
-def keras_tutorial():
-    """
-    A tutorial use of keras model for image multiclass classification
-
-    :return:
-    """
-    # downloading the test dataset
-    dataset_url = "https://storage.googleapis.com/download.tensorflow.org/example_images/flower_photos.tgz"
-    data_dir = tf.keras.utils.get_file('flower_photos', origin=dataset_url, untar=True)
-    data_dir = pathlib.Path(data_dir)
-    image_count = len(list(data_dir.glob('*/*.jpg')))
-
-    # loading data using keras
-    batch_size = 32
-    img_height = 180
-    img_width = 180
-
-    train_ds = tf.keras.utils.image_dataset_from_directory(
-        data_dir,
-        validation_split=0.2,
-        subset="training",
-        seed=123,
-        image_size=(img_height, img_width),
-        batch_size=batch_size)
-
-    val_ds = tf.keras.utils.image_dataset_from_directory(
-        data_dir,
-        validation_split=0.2,
-        subset="validation",
-        seed=123,
-        image_size=(img_height, img_width),
-        batch_size=batch_size)
-
-    class_names = train_ds.class_names
-    print(class_names)
-
-    # Visualizing data
-    plt.figure(figsize=(10, 10))
-    for images, labels in train_ds.take(1):
-        for i in range(9):
-            ax = plt.subplot(3, 3, i + 1)
-            plt.imshow(images[i].numpy().astype("uint8"))
-            plt.title(class_names[labels[i]])
-            plt.axis("off")
-    plt.show()
-
-    for image_batch, labels_batch in train_ds:
-        print(image_batch.shape)
-        print(labels_batch.shape)
-        break
-
-    # Configure the dataset for performance
-
-    AUTOTUNE = tf.data.AUTOTUNE
-
-    train_ds = train_ds.cache().shuffle(1000).prefetch(buffer_size=AUTOTUNE)  # Once loaded, keep the pictures in memory
-    val_ds = val_ds.cache().prefetch(buffer_size=AUTOTUNE)  # Overlaps data preprocessing/model execution while training
-
-    # Data augmentation
-    data_augmentation = keras.Sequential(
-        [
-            layers.RandomFlip("horizontal",
-                              input_shape=(img_height,
-                                           img_width,
-                                           3)),
-            layers.RandomRotation(0.1),
-            layers.RandomZoom(0.1),
-        ]
-    )
-
-    # Basic Keras model
-    num_classes = len(class_names)
-    model = Sequential([
-        data_augmentation,
-        layers.Rescaling(1. / 255),
-        layers.Conv2D(16, 3, padding='same', activation='relu'),
-        layers.MaxPooling2D(),
-        layers.Conv2D(32, 3, padding='same', activation='relu'),
-        layers.MaxPooling2D(),
-        layers.Conv2D(64, 3, padding='same', activation='relu'),
-        layers.MaxPooling2D(),
-        layers.Dropout(0.2),
-        layers.Flatten(),
-        layers.Dense(128, activation='relu'),
-        layers.Dense(num_classes, name="outputs")
-    ])
-
-    model.compile(optimizer='adam',
-                  loss=tf.keras.losses.SparseCategoricalCrossentropy(from_logits=True),
-                  metrics=['accuracy'])
-
-    model.summary()
-
-    # Train the model
-    epochs = 15
-    history = model.fit(
-        train_ds,
-        validation_data=val_ds,
-        epochs=epochs
-    )
-
-    # Visualize training
-    acc = history.history['accuracy']
-    val_acc = history.history['val_accuracy']
-
-    loss = history.history['loss']
-    val_loss = history.history['val_loss']
-
-    epochs_range = range(epochs)
-
-    plt.figure(figsize=(8, 8))
-    plt.subplot(1, 2, 1)
-    plt.plot(epochs_range, acc, label='Training Accuracy')
-    plt.plot(epochs_range, val_acc, label='Validation Accuracy')
-    plt.legend(loc='lower right')
-    plt.title('Training and Validation Accuracy')
-
-    plt.subplot(1, 2, 2)
-    plt.plot(epochs_range, loss, label='Training Loss')
-    plt.plot(epochs_range, val_loss, label='Validation Loss')
-    plt.legend(loc='upper right')
-    plt.title('Training and Validation Loss')
-    plt.show()
-
-    # Predict on new data
-    sunflower_url = "https://storage.googleapis.com/download.tensorflow.org/example_images/592px-Red_sunflower.jpg"
-    sunflower_path = tf.keras.utils.get_file('Red_sunflower', origin=sunflower_url)
-
-    img = tf.keras.utils.load_img(
-        sunflower_path, target_size=(img_height, img_width)
-    )
-    img_array = tf.keras.utils.img_to_array(img)
-    img_array = tf.expand_dims(img_array, 0)  # Create a batch
-
-    predictions = model.predict(img_array)
-    score = tf.nn.softmax(predictions[0])
-
-    print(
-        "This image most likely belongs to {} with a {:.2f} percent confidence."
-        .format(class_names[np.argmax(score)], 100 * np.max(score))
-    )
-
-
-def train_RFC_from_dataset(dataset: pd.DataFrame, savepath=""):
-    """
-    Train a Random Forest Classifier model from an already formatted dataset.
-
-        Parameters
-        ----------
-        dataset : pandas Dataframe
-            a pandas Dataframe where each row is an entry for a machine
-            learning model. Has a last column as 'target' containing
-            the target value for each entry.
-
-        savepath: str, optional, default:''
-            name of the saved file. If empty, does not save the file.
-
-            .. versionadded:: 1.0.0
-
-        Returns
-        -------
-        out : tuple of size (1, 2).
-            The first element is a trained random forest classifier.
-            The second is its scores.
-    """
-
-    clf = RandomForestClassifier(n_estimators=1000)
-    X = dataset[dataset.columns[:-1]]
-    y = dataset["label"]
-    X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.5)
-    clf.fit(X_train, y_train)
-    if savepath:
-        pickle.dump(clf, open(savepath, "wb"))
-    return clf, clf.score(X_test, y_test)
-
-
-def get_top_features_from_trained_RFC(clf, **kwargs):
-    """
-    select to top n% feature sorted by highest importance, of a trained Random Forest Classtifier model.
-
-        Parameters
-        ----------
-        clf : RandomForestClassifier
-            a trained model
-
-        **kwargs: keyword arguments
-            percentage: float, optional, default: 0.05
-                proportion of the most important features to keep
-
-            show: bool, optional, default: True
-                Whether to show a plot of the model feature importance or not.
-
-            save: bool, optional, default: False
-                Whether to save a plot of the model feature importance or not.
-
-            title: str, optional, default: ''
-                the title to give the plot and name of the resulting file if save if True.
-
-            savepath: str, optional, default: ""
-                If not empty, path where le result will be saved.
-
-        Returns
-        -------
-        out : tuple of lists
-            first element: list of the indexes of the most important features
-            second element: importance (values) corresponding to the indexes.
-    """
-    options = {"percentage": 0.05,
-               "show": True,
-               "save": False,
-               "title": "",
-               "savepath": ""}
-    options.update(**kwargs)
-
-    importances_over_iterations = []
-    for i in range(10):
-        mean = np.mean([tree.feature_importances_ for tree in clf.estimators_], axis=0)
-
-        importances_over_iterations.append(mean)
-
-    arrays = [np.array(x) for x in importances_over_iterations]
-    mean_importances_over_iterations = [np.mean(k) for k in zip(*arrays)]
-    std_arrays = [np.array(x) for x in importances_over_iterations]
-    std_importances_over_iterations = [np.std(k) for k in zip(*std_arrays)]
-
-    low_std = []
-    for i in range(len(mean_importances_over_iterations)):
-        low_std.append(mean_importances_over_iterations[i] - std_importances_over_iterations[i])
-    high_std = []
-    for i in range(len(mean_importances_over_iterations)):
-        high_std.append(mean_importances_over_iterations[i] + std_importances_over_iterations[i])
-
-    hertz = []
-    factor = 5000 / 300
-    for i in range(300):
-        hertz.append(int(i * factor))
-    n = int(options["percentage"] * len(mean_importances_over_iterations))
-    idx_foi = sorted(range(len(mean_importances_over_iterations)),
-                     key=lambda i: mean_importances_over_iterations[i], reverse=True)[:n]
-
-    plt.bar([x for x in range(300)], mean_importances_over_iterations, color="blue", )
-
-    xticks = [x for x in range(0, 300, 50)]
-    new_ticks = [hertz[x] for x in xticks]
-    xticks.append(300)
-    new_ticks.append(5000)
-    plt.xticks(xticks, new_ticks)
-    plt.ylabel("Relative importance [AU]")
-    plt.xlabel("Frequency-like features [Hz]")
-    plt.title(options["title"])
-    if options["save"]:
-        plt.savefig(options["savepath"])
-    # plt.fill_between(hertz, low_std, high_std, facecolor="blue", alpha=0.5)
-    if options["save"]:
-        plt.show()
-    plt.close()
-    return idx_foi, mean_importances_over_iterations
-
-
-def fit_pca(dataframe: pd.DataFrame, n_components=3):
-    """
-    fit a Principal Component Analysis and return its instance and dataset.
-
-        Parameters
-        ----------
-        dataframe: DataFrame
-            The data on which the pca instance has to be fitted.
-        n_components: int, optional, default: 3
-            The number of components for the PCA instance.
-
-        Returns
-        -------
-        out: tuple of shape (1, 3)
-            The first element is the PCA instance. The second
-            element is the resulting dataframe. The third is the
-            explained variance ratios.
-    """
-    features = dataframe.columns[:-1]
-    x = dataframe.loc[:, features].values
-    x = StandardScaler().fit_transform(x)  # normalizing the features
-    pca = PCA(n_components=n_components)
-    principalComponent = pca.fit_transform(x)
-    principal_component_columns = [f"principal component {i + 1}" for i in range(n_components)]
-
-    principal_tahyna_Df = pd.DataFrame(data=principalComponent
-                                       , columns=principal_component_columns)
-
-    principal_tahyna_Df["label"] = dataframe["label"]
-
-    return pca, principal_tahyna_Df, pca.explained_variance_ratio_
-
-
-def apply_pca(pca, dataframe):
-    """
-    Transform data using an already fit PCA instance.
-
-        Parameters
-        ----------
-        pca: PCA instance
-            The fitted PCA instance from what the data will
-            be transformed.
-        dataframe: DataFrame
-            The data to transform using an already fitted PCA.
-            Must have a 'label' column.
-
-        Returns
-        -------
-        out: DataFrame
-            The transformed data.
-    """
-    features = dataframe.columns[:-1]
-    x = dataframe.loc[:, features].values
-    x = StandardScaler().fit_transform(x)  # normalizing the features
-    transformed_ds = pca.transform(x)
-    transformed_df = pd.DataFrame(data=transformed_ds,
-                                  columns=[f"principal component {i + 1}" for i in range(transformed_ds.shape[1])])
-    transformed_df['label'] = dataframe['label']
-    return transformed_df
-
-
-def confidence_ellipse(x, y, ax, n_std=3.0, color='none', **kwargs):
-    """
-    Create a plot of the covariance confidence ellipse of *x* and *y*.
-
-        Parameters
-        ----------
-        x, y : array-like, shape (n, )
-            Input data.
-
-        ax : matplotlib.axes.Axes
-            The axes object to draw the ellipse into.
-
-        n_std : float
-            The number of standard deviations to determine the ellipse's radiuses.
-
-        color : str
-            color of the ellipsis.
-
-        **kwargs
-            Forwarded to `~matplotlib.patches.Ellipse`
-
-        Returns
-        -------
-        matplotlib.patches.Ellipse
-    """
-    if x.size != y.size:
-        raise ValueError("x and y must be the same size")
-
-    cov = np.cov(x, y)
-    pearson = cov[0, 1] / np.sqrt(cov[0, 0] * cov[1, 1])
-    # Using a special case to obtain the eigenvalues of this
-    # two-dimensional dataset.
-    ell_radius_x = np.sqrt(1 + pearson)
-    ell_radius_y = np.sqrt(1 - pearson)
-    ellipse = Ellipse((0, 0), width=ell_radius_x * 2, height=ell_radius_y * 2,
-                      color=color, **kwargs)
-
-    # Calculating the standard deviation of x from
-    # the squareroot of the variance and multiplying
-    # with the given number of standard deviations.
-    scale_x = np.sqrt(cov[0, 0]) * n_std
-    mean_x = np.mean(x)
-
-    # calculating the standard deviation of y ...
-    scale_y = np.sqrt(cov[1, 1]) * n_std
-    mean_y = np.mean(y)
-
-    transf = transforms.Affine2D() \
-        .rotate_deg(45) \
-        .scale(scale_x, scale_y) \
-        .translate(mean_x, mean_y)
-
-    ellipse.set_transform(transf + ax.transData)
-    return ax.add_patch(ellipse)
-
-
-def plot_pca(dataframe: pd.DataFrame, **kwargs):
-    """
-    plot the result of PCA.
-
-        Parameters
-        ----------
-        dataframe: DataFrame
-            The data to plot. Must contain a 'label' column.
-
-        **kwargs: keyword arguments
-            n_components: int, optional, default: 2
-                Number of principal components. Also, teh dimension
-                of the graph. Must be equal to 2 or 3.
-            show: bool, optional, default: True
-                Whether to show the plot or not.
-            save: bool, optional, default: False
-                Whether to save the plot or not.
-            commentary: str, optional, default: "T=48H"
-                Any specification to include in the file name while saving.
-            points: bool, optional, default: True
-                whether to plot the points or not.
-            metrics: bool, optional, default: False
-                Whether to plot the metrics or not
-            savedir: str, optional, default: ""
-                Directory where to save the resulting plot, if not empty.
-            title: str, optional, defualt: ""
-                The filename of the resulting plot. If empty,
-                an automatic name will be generated.
-            ratios: tuple of float, optional, default: ()
-                the PCA explained variance ratio, to display on
-                the plot axis.
-    """
-
-    options = {
-        'n_components': 2,
-        'show': True,
-        'commentary': "",
-        'points': True,
-        'metrics': False,
-        'savedir': "",
-        'pc_ratios': [],
-        'title': "",
-        'ratios': ()
-
-    }
-
-    options.update(kwargs)
-    targets = dataframe["label"].unique()
-    colors = ['g', 'b', 'r', 'k', 'sandybrown', 'deeppink', 'gray']
-    if len(targets) > len(colors):
-        n = len(targets) - len(colors) + 1
-        for i in range(n):
-            colors.append('#%06X' % randint(0, 0xFFFFFF))
-
-    if options['n_components'] == 2:
-        label_params = {'fontsize': 30, "labelpad": 8}
-        ticks_params = {'fontsize': 30, }
-        fig, ax = plt.subplots(1, 1, figsize=(12, 10))
-
-        plt.xticks(**ticks_params)
-        plt.yticks(**ticks_params)
-        xlabel = f'Principal Component-1 ({options["ratios"][0]}%)'
-        ylabel = f'Principal Component-2 ({options["ratios"][1]}%)'
-        if len(options['pc_ratios']):
-            xlabel += f" ({round(options['pc_ratios'][0] * 100, 2)}%)"
-            ylabel += f" ({round(options['pc_ratios'][1] * 100, 2)}%)"
-
-        plt.xlabel(xlabel, **label_params)
-        plt.ylabel(ylabel, **label_params)
-
-        for target, color in zip(targets, colors):
-            indicesToKeep = dataframe['label'] == target
-            x = dataframe.loc[indicesToKeep, 'principal component 1']
-            y = dataframe.loc[indicesToKeep, 'principal component 2']
-            if options['points']:
-                alpha = 1
-                if options['metrics']:
-                    alpha = .2
-                plt.scatter(x, y, c=color, s=10, alpha=alpha, label=target)
-            if options['metrics']:
-                plt.scatter(np.mean(x), np.mean(y), marker="+", color=color, linewidth=2, s=160)
-                confidence_ellipse(x, y, ax, n_std=1.0, color=color, fill=False, linewidth=2)
-
-        def update(handle, orig):
-            handle.update_from(orig)
-            handle.set_alpha(1)
-
-        plt.legend(prop={'size': 25}, handler_map={PathCollection: HandlerPathCollection(update_func=update),
-                                                   plt.Line2D: HandlerLine2D(update_func=update)})
-    elif options['n_components'] == 3:
-        label_params = {'fontsize': 20, "labelpad": 8}
-        ticks_params = {'fontsize': 20, }
-        plt.figure(figsize=(10, 10))
-        ax = plt.axes(projection='3d')
-
-        xlabel = f'Principal Component-1 ({options["ratios"][0]}%)'
-        ylabel = f'Principal Component-2 ({options["ratios"][1]}%)'
-        zlabel = f'Principal Component-3 ({options["ratios"][2]}%)'
-        if len(options['pc_ratios']):
-            xlabel += f" ({round(options['pc_ratios'][0] * 100, 2)}%)"
-            ylabel += f" ({round(options['pc_ratios'][1] * 100, 2)}%)"
-            zlabel += f" ({round(options['pc_ratios'][2] * 100, 2)}%)"
-
-        ax.set_xlabel(xlabel, **label_params)
-        ax.set_ylabel(ylabel, **label_params)
-        ax.set_zlabel(zlabel, **label_params)
-        for target, color in zip(targets, colors):
-            indicesToKeep = dataframe['label'] == target
-            x = dataframe.loc[indicesToKeep, 'principal component 1']
-            y = dataframe.loc[indicesToKeep, 'principal component 2']
-            z = dataframe.loc[indicesToKeep, 'principal component 3']
-            ax.scatter3D(x, y, z, c=color, s=10)
-        plt.legend(targets, prop={'size': 18})
-
-    if options['savedir']:
-        if options["title"] == "":
-            if options['commentary']:
-                options["title"] += options["commentary"]
-
-        plt.savefig(os.path.join(options['savedir'], options["title"] + ".png"), dpi=1200)
-
-    if options['show']:
-        plt.show()
-    plt.close()
-
-
-def fit_umap(dataframe, n_components=3):
-    """
-    fit a Uniform Manifold Approximated Projection and return its instance and dataset.
-
-        Parameters
-        ----------
-        dataframe: DataFrame
-            The data on which the umap instance has to be fitted.
-            Contains a column 'label'.
-        n_components: int, optional, default: 3
-            The number of components for the UMAP instance.
-
-        Returns
-        -------
-        out: tuple of shape (1, 2)
-            The first element is the UMAP instance. The second
-            element is the resulting dataframe.
-    """
-    # Configure UMAP hyperparameters
-    features = dataframe.columns[:-1]
-    x = dataframe.loc[:, features].values
-    reducer = UMAP(n_neighbors=100,
-                   n_components=n_components,  # default 2, The dimension of the space to embed into.
-                   metric='euclidean',
-                   n_epochs=1000,
-                   learning_rate=1.0, )
-
-    # Fit and transform the data
-    X_trans = reducer.fit_transform(x)
-    X_dimension = [f"dimension {i + 1}" for i in range(n_components)]
-    transformed_df = pd.DataFrame(data=X_trans, columns=X_dimension)
-
-    transformed_df["label"] = dataframe["label"]
-
-    return reducer, transformed_df
-
-
-def apply_umap(umap, dataframe):
-    """
-    Transform data using an already fit UMAP instance.
-
-       Parameters
-       ----------
-       umap: UMAP instance
-           The fitted PCA instance from what the data will
-           be transformed.
-       dataframe: DataFrame
-           The data to transform using an already fitted PCA.
-           Must have a 'label' column.
-
-       Returns
-       -------
-       out: DataFrame
-           The transformed data.
-   """
-    features = dataframe.columns[:-1]
-    x = dataframe.loc[:, features].values
-    x = StandardScaler().fit_transform(x)  # normalizing the features
-    transformed_ds = umap.transform(x)
-    transformed_df = pd.DataFrame(data=transformed_ds,
-                                  columns=[f"dimension {i + 1}" for i in range(transformed_ds.shape[1])])
-    transformed_df['label'] = dataframe['label']
-    return transformed_df
-
-
-def plot_umap(dataframe, **kwargs):
-    """
-    plot the result of UMAP.
-
-        Parameters
-        ----------
-        dataframe: DataFrame
-            The data to plot. Must contain a 'label' column.
-
-        **kwargs: keyword arguments
-            n_components: int, optional, default: 3
-                Number of principal components. Also, teh dimension
-                of the graph. Must be equal to 2 or 3.
-            show: bool, optional, default: True
-                Whether to show the plot or not.
-            save: bool, optional, default: False
-                Whether to save the plot or not.
-            commentary: str, optional, default: ""
-                Any specification to include in the file name while saving.
-            points: bool, optional, default: True
-                whether to plot the points or not.
-            metrics: bool, optional, default: False
-                Whether to plot the metrics or not
-            savedir: str, optional, default: ""
-                Directory where to save the resulting plot, if not empty.
-    """
-    options = {"n_components": 3, "show": True, "save": False, "commentary": "", "points": True,
-               "metrics": False, "savedir": ""}
-    options.update(**kwargs)
-    targets = dataframe["label"].unique()
-    colors = ['r', 'g', 'b', 'k', 'sandybrown', 'deeppink', 'gray']
-    if len(targets) > len(colors):
-        n = len(targets) - len(colors) + 1
-        for i in range(n):
-            colors.append('#%06X' % randint(0, 0xFFFFFF))
-    if options["n_components"] == 2:
-        fig, ax = plt.subplots(1, 1, figsize=(10, 10))
-        plt.xticks(fontsize=12)
-        plt.yticks(fontsize=14)
-        plt.xlabel(f'PC-1', fontsize=20)
-        plt.ylabel(f'PC-2', fontsize=20)
-        plt.title(f"Uniform Manifold Approximated Projection", fontsize=20)
-        for target, color in zip(targets, colors):
-            indicesToKeep = dataframe['label'] == target
-            x = dataframe.loc[indicesToKeep, 'dimension 1']
-            y = dataframe.loc[indicesToKeep, 'dimension 2']
-            if options["points"]:
-                alpha = 1
-                if options["metrics"]:
-                    alpha = .2
-                plt.scatter(x, y, c=color, s=10, alpha=alpha, label=target)
-            if options["metrics"]:
-                plt.scatter(np.mean(x), np.mean(y), marker="+", color=color, linewidth=2, s=160)
-                confidence_ellipse(x, y, ax, n_std=1.0, color=color, fill=False, linewidth=2)
-
-        def update(handle, orig):
-            handle.update_from(orig)
-            handle.set_alpha(1)
-
-        plt.legend(prop={'size': 15}, handler_map={PathCollection: HandlerPathCollection(update_func=update),
-                                                   plt.Line2D: HandlerLine2D(update_func=update)})
-    if options["n_components"] == 3:
-        plt.figure(figsize=(10, 10))
-        ax = plt.axes(projection='3d')
-        ax.set_xlabel(f'dimension-1', fontsize=20)
-        ax.set_ylabel(f'dimension-2', fontsize=20)
-        ax.set_zlabel(f'dimension-3', fontsize=20)
-        for target, color in zip(targets, colors):
-            indicesToKeep = dataframe['label'] == target
-            x = dataframe.loc[indicesToKeep, dataframe.columns[0]]
-            y = dataframe.loc[indicesToKeep, dataframe.columns[1]]
-            z = dataframe.loc[indicesToKeep, dataframe.columns[2]]
-            ax.scatter3D(x, y, z, c=color, s=10, label='bla')
-        plt.legend(targets, prop={'size': 15})
-        plt.title(f"Uniform Manifold Approximated Projection", fontsize=20)
-
-    if options["savedir"]:
-        if options["commentary"]:
-            plt.savefig(os.path.join(options["savedir"],
-                                     f"UMAP n={options['n_components']} t={targets} {options['commentary']}.png"))
-        else:
-            plt.savefig(os.path.join(options["savedir"], f"UMAP n={options['n_']} t={targets}.png"))
-
-    if options["show"]:
-        plt.show()
-    plt.close()
-
-
-def test_rfc_by_confusion(clf, dataset: pd.DataFrame, training_targets: tuple, **kwargs):
-    """
-    Test an already trained Random forest classifier model,
-    resulting in a confusion matrix. The test can be done
-    on targets_labels different from the targets_labels used for training
-    the model.
-        Parameters
-        ----------
-        clf: RandomForestClassifier
-            the trained model.
-        dataset:  pandas Dataframe.
-            Dataframe containing the data used for testing the
-            model. The rows are the entries, and the columns are
-            the features on which the model has been trained.
-            The last column is 'status' containing the labels
-            of the targets_labels for each entry.
-        training_targets: tuple of str
-            the targets on which the model has been trained.
-        **kwargs: keyword arguments
-            savepath: str, optional, default: ""
-                If not empty, path where le result will be saved.
-            verbose: Bool, optional. Default: False
-                Whether to display more information when computing
-                or not.
-            show: Bool, optional. Default: True
-                Whether to show the resulting confusion matrix or not.
-            iterations: int, optional. Default: 10
-                Number of iterations the test will be computed.
-            commentary: str, optional. Default: ""
-                If any specification to add to the file name.
-            testing_targets: tuple of str
-                the targets on which the model will be tested.
-                Can be different from the training targets.
-    """
-    options = {"verbose": False, "show": True,
-               "testing_targets": (),
-               "iterations": 10,
-               "commentary": "", "savepath": "", "title": ""}
-    options.update(**kwargs)
-    if not options["testing_targets"]:
-        options["testing_targets"] = training_targets
-    CORRESPONDANCE = {}
-    target_id = 0
-    for t in training_targets:
-        if t not in CORRESPONDANCE:
-            CORRESPONDANCE[t] = target_id
-            target_id += 1
-    for t in options["testing_targets"]:
-        if t not in CORRESPONDANCE:
-            CORRESPONDANCE[t] = target_id
-            target_id += 1
-    X = dataset[dataset.columns[:-1]]
-    y = dataset["label"]
-
-    if options["verbose"]:
-        progress = 0
-        sys.stdout.write(f"\rTesting model: {progress}%")
-        sys.stdout.flush()
-
-    X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.3)
-
-    # get predictions and probabilities
-    all_matrixes = []
-    all_probability_matrixes = []
-    for iters in range(options["iterations"]):
-        matrix = np.zeros((len(training_targets), len(options['testing_targets'])))
-        probabilities_matrix = np.empty((len(training_targets), len(options['testing_targets'])), dtype=object)
-
-        # Initializing the matrix containing the probabilities
-        for i in range(len(probabilities_matrix)):
-            for j in range(len(probabilities_matrix[i])):
-                probabilities_matrix[i][j] = []
-
-        # Making predictions and storing the results in predictions[]
-        predictions = []
-        for i in X_test.index:
-            row = X_test.loc[i, :]
-            y_pred = clf.predict([row])[0]
-            proba_class = clf.predict_proba([row])[0]
-            predictions.append((y_pred, proba_class))
-
-        #
-        targets = []
-        for i in y_test.index:
-            targets.append(y_test.loc[i])
-        # Building the confusion matrix
-        for i in range(len(targets)):
-            y_true = targets[i]
-            y_pred = predictions[i][0]
-            y_proba = max(predictions[i][1])
-            matrix[CORRESPONDANCE[y_pred]][CORRESPONDANCE[y_true]] += 1
-
-            probabilities_matrix[CORRESPONDANCE[y_pred]][CORRESPONDANCE[y_true]].append(y_proba)
-        mean_probabilities = np.zeros((len(training_targets), len(options['testing_targets'])))
-        for i in range(len(probabilities_matrix)):
-            for j in range(len(probabilities_matrix[i])):
-                mean_probabilities[i][j] = np.mean(probabilities_matrix[i][j])
-        all_matrixes.append(matrix)
-        all_probability_matrixes.append(mean_probabilities)
-
-    mixed_labels_matrix = np.empty((len(training_targets), len(options['testing_targets']))).tolist()
-    mean_probabilities_matrix = np.empty((len(training_targets), len(options['testing_targets'])))
-    overall_matrix = np.mean(np.array([i for i in all_matrixes]), axis=0)
-    overall_probabilities = np.mean(np.array([i for i in all_probability_matrixes]), axis=0)
-
-    # averaging the probabilities
-    for i in range(len(overall_probabilities)):
-        for j in range(len(overall_probabilities[i])):
-            mean_probabilities_matrix[i][j] = np.mean(overall_probabilities[i][j])
-
-    # mixing count and probabilities for displaying
-    for i in range(len(overall_probabilities)):
-        for j in range(len(overall_probabilities[i])):
-            np.nan_to_num(overall_matrix[i][j])
-            np.nan_to_num(mean_probabilities_matrix[i][j])
-            mixed_labels_matrix[i][j] = str(int(overall_matrix[i][j])) + "\nCUP=" + str(
-                round(mean_probabilities_matrix[i][j], 3))
-
-    # plotting
-    fig, ax = plt.subplots(1, 1, figsize=(7 / 4 * len(options['testing_targets']), 6 / 4 * len(training_targets)))
-
-    fig.suptitle("")
-    sns.heatmap(ax=ax, data=overall_matrix, annot=mixed_labels_matrix, fmt='', cmap="Blues")
-    ax.xaxis.tick_top()
-    ax.xaxis.set_label_position('top')
-    ax.set_ylabel("The input is classified as")
-    ax.set_xlabel("The input is")
-    ax.set_xticks([CORRESPONDANCE[x] + 0.5 for x in options['testing_targets']], options['testing_targets'])
-    ax.set_yticks([CORRESPONDANCE[x] + 0.5 for x in training_targets], training_targets)
-    plt.tight_layout()
-
-    if options['savepath']:
-        plt.savefig(os.path.join(options['savepath'], options["title"] + ".png"))
-    if options['show']:
-        plt.show()
-    plt.close()
-
-
-def test_sequential_by_confusion(model_path, dataset, training_targets, **kwargs):
-    """
-    Test an already trained keras Sequential model,
-    resulting in a confusion matrix. The test can be done
-    on targets_labels different from the targets_labels used for training
-    the model.
-        Parameters
-        ----------
-        model_path: str
-            the absolute path to the trained model, with extension (to open).
-        dataset:  list of lists, shape (n, (2, (ndarray(m,m)))
-            list of n pictures of size m*m, coupled with its
-            int-like label.
-        training_targets: list of int
-            the targets on which the model has been trained.
-        **kwargs: keyword arguments
-            savepath: str, optional, default: ""
-                If not empty, path where le result will be saved.
-            verbose: Bool, optional. Default: False
-                Whether to display more information when computing
-                or not.
-            show: Bool, optional. Default: True
-                Whether to show the resulting confusion matrix or not.
-            iterations: int, optional. Default: 10
-                Number of iterations the test will be computed.
-            commentary: str, optional. Default: ""
-                If any specification to add to the file name.
-            testing_targets: list of int
-                the targets on which the model will be tested.
-                Can be different from the training targets.
-            target_rename: dict, optional, default: {}
-                the keys are the actual targets, the values are
-                how you want to rename them on the confusion matrix.
-    """
-    model = load_model(model_path)
-    options = {"verbose": False, "show": True,
-               "testing_targets": (),
-               "iterations": 10,
-               "commentary": "",
-               "savepath": "",
-               "title": "",
-               "target_rename": ""}
-    options.update(**kwargs)
-    if not options["testing_targets"]:
-        options["testing_targets"] = training_targets
-    CORRESPONDANCE = {}
-    target_id = 0
-    for t in training_targets:
-        if t not in CORRESPONDANCE:
-            CORRESPONDANCE[t] = target_id
-            target_id += 1
-    for t in options["testing_targets"]:
-        if t not in CORRESPONDANCE:
-            CORRESPONDANCE[t] = target_id
-            target_id += 1
-    x_train, x_val, y_train, y_val = split_train_test(dataset, train_size=0.1)
-
-    x_val = np.array(x_val)
-    y_val = np.array(y_val)
-
-    # get predictions and probabilities
-    all_matrixes = []
-    all_probability_matrixes = []
-    for iters in range(options["iterations"]):
-        matrix = np.zeros((len(training_targets), len(options['testing_targets'])))
-        probabilities_matrix = np.empty((len(training_targets), len(options['testing_targets'])), dtype=object)
-
-        # Initializing the matrix containing the probabilities
-        for i in range(len(probabilities_matrix)):
-            for j in range(len(probabilities_matrix[i])):
-                probabilities_matrix[i][j] = []
-
-        # Making predictions and storing the results in predictions[]
-        predictions = []
-        for x in x_val:
-            y_pred = model.predict(x[None, ...])[0]
-            predictions.append((np.where(y_pred == max(y_pred))[0][0], list(y_pred)))
-
-        targets = []
-        for i in y_val:
-            targets.append(np.where(i == max(i))[0][0])
-        # Building the confusion matrix
-
-        for i in range(len(targets)):
-            y_true = targets[i]
-            y_pred = predictions[i][0]
-            y_proba = max(predictions[i][1])
-
-            matrix[CORRESPONDANCE[y_pred]][CORRESPONDANCE[y_true]] += 1
-
-            probabilities_matrix[CORRESPONDANCE[y_pred]][CORRESPONDANCE[y_true]].append(y_proba)
-        mean_probabilities = np.zeros((len(training_targets), len(options['testing_targets'])))
-        for i in range(len(probabilities_matrix)):
-            for j in range(len(probabilities_matrix[i])):
-                mean_probabilities[i][j] = np.mean(probabilities_matrix[i][j])
-        all_matrixes.append(matrix)
-        all_probability_matrixes.append(mean_probabilities)
-
-    mixed_labels_matrix = np.empty((len(training_targets), len(options['testing_targets']))).tolist()
-    mean_probabilities_matrix = np.empty((len(training_targets), len(options['testing_targets'])))
-    overall_matrix = np.mean(np.array([i for i in all_matrixes]), axis=0)
-    overall_probabilities = np.mean(np.array([i for i in all_probability_matrixes]), axis=0)
-
-    # averaging the probabilities
-    for i in range(len(overall_probabilities)):
-        for j in range(len(overall_probabilities[i])):
-            mean_probabilities_matrix[i][j] = np.mean(overall_probabilities[i][j])
-
-    # mixing count and probabilities for displaying
-    for i in range(len(overall_probabilities)):
-        for j in range(len(overall_probabilities[i])):
-            np.nan_to_num(overall_matrix[i][j])
-            np.nan_to_num(mean_probabilities_matrix[i][j])
-            mixed_labels_matrix[i][j] = str(int(overall_matrix[i][j])) + "\nCUP=" + str(
-                round(mean_probabilities_matrix[i][j], 3))
-
-    # plotting
-    fig, ax = plt.subplots(1, 1, figsize=(7 / 4 * len(options['testing_targets']), 6 / 4 * len(training_targets)))
-
-    fig.suptitle("")
-    sns.heatmap(ax=ax, data=overall_matrix, annot=mixed_labels_matrix, fmt='', cmap="Blues")
-    ax.xaxis.tick_top()
-    ax.xaxis.set_label_position('top')
-    ax.set_ylabel("The input is classified as")
-    ax.set_xlabel("The input is")
-
-    ax.set_xticks([CORRESPONDANCE[x] + 0.5 for x in options['testing_targets']],
-                  [options["target_rename"][x] for x in options['testing_targets']])
-    ax.set_yticks([CORRESPONDANCE[x] + 0.5 for x in training_targets],
-                  [options["target_rename"][x] for x in training_targets])
-    plt.tight_layout()
-
-    if options['savepath']:
-        plt.savefig(os.path.join(options['savepath'], options["title"] + ".png"))
-    if options['show']:
-        plt.show()
-    plt.close()
-
-
-def model_history_plot(history_path, savepath=""):
-    """
-    Save in a fancy way the history logs of a
-    trained keras model, saved in the form of a
-    csv file.
-
-        Parameters
-        ----------
-        history_path: str
-            the absolute path to the .log file,
-            containing the history in csv format.
-        savepath: str, optional, default: ""
-            If not empty, the directory where the plot will be saved.
-            If empty, the plot is shown.
-    """
-    data = pd.read_csv(history_path, index_col=False)
-    plt.figure(figsize=(6, 5))
-    plt.plot(data["accuracy"], linestyle="dashed", color="blue", label="training accuracy")
-    plt.plot(data["val_accuracy"], linestyle="solid", color="blue", label="validation accuracy")
-    plt.plot(data["loss"], linestyle="dashed", color="red", label="training loss")
-    plt.plot(data["val_loss"], linestyle="solid", color="red", label="training loss")
-
-    plt.xlabel("epochs", fontsize=15)
-    plt.ylabel("score", fontsize=15)
-    plt.xticks(fontsize=13)
-    plt.yticks(fontsize=13)
-    plt.legend(fontsize=13)
-    title = "history " + os.path.basename(history_path).replace("history", "").split(".")[0] + ".png"
-    if savepath:
-        plt.savefig(os.path.join(savepath, title))
-    else:
-        plt.show()
-    plt.close()
-
-
-def basic_sequential(data, epochs, comment="", model_savepath="", history_savepath=""):
-    """
-    Use of a generic Convolutional network, use for basic image classification.
-    The inputs are of shape (224, 224).
-
-        Parameters
-        ----------
-        data: ndarray shape((n, 2), m)
-            The numpy array containing the data.
-            Each entry is coupled within a tuple with its
-            corresponding label
-        epochs: int
-            number of epochs to train the model on.
-        comment: str, optional, default: ""
-            Add to the name a comment, used when saving
-            the model and for the model name.
-        savepath: str, optional, default: ""
-            If not empty, directory where to save the model.
-        savepath: str, optional, default: ""
-            If not empty, directory where to save the history plot.
-
-    """
-    x_train, x_val, y_train, y_val = split_train_test(data)
-    datagen = ImageDataGenerator(
-        featurewise_center=False,  # set input mean to 0 over the dataset
-        samplewise_center=False,  # set each sample mean to 0
-        featurewise_std_normalization=False,  # divide inputs by std of the dataset
-        samplewise_std_normalization=False,  # divide each input by its std
-        zca_whitening=False,  # apply ZCA whitening
-        rotation_range=180,  # randomly rotate images in the range (degrees, 0 to 180)
-        zoom_range=0.2,  # Randomly zoom image
-        width_shift_range=0,  # randomly shift images horizontally (fraction of total width)
-        height_shift_range=0,  # randomly shift images vertically (fraction of total height)
-        horizontal_flip=False,  # randomly flip images
-        vertical_flip=False,  # randomly flip images
-    )
-
-    datagen.fit(x_train)
-    model = Sequential()
-
-    model.add(Conv2D(32, 7, padding="same", activation="relu", input_shape=(224, 224, 3)))
-    model.add(MaxPool2D())
-
-    model.add(Conv2D(32, 7, padding="same", activation="relu"))
-    model.add(MaxPool2D())
-
-    model.add(Conv2D(64, 7, padding="same", activation="relu"))
-    model.add(MaxPool2D())
-    model.add(Dropout(0.4))
-
-    model.add(Flatten())
-    model.add(Dense(128, activation="relu"))
-    model.add(Dense(2, activation="softmax"))
-
-    opt = Adam(learning_rate=0.000001)
-    model.compile(optimizer=opt, loss="categorical_crossentropy",
-                  metrics=['accuracy'])
-
-    name = f"e={epochs} basic model{comment}"
-
-    csv_logger = CSVLogger(os.path.join(model_savepath, f"{name} history.log"), separator=',', append=False)
-    history = model.fit(x_train, y_train, epochs=epochs, validation_data=(x_val, y_val), callbacks=[csv_logger])
-    if model_savepath:
-        model.save(os.path.join(model_savepath, f"{name}.h5"))
-    if history_savepath:
-        model_history_plot(os.path.join(model_savepath, f"{name} history.log"), savepath=history_savepath)
-
-
-def split_train_test(data, train_size: float = 0.7):
-    """
-    Split a dataset into train and validation sets for features and labels.
-
-        Parameters
-        ----------
-        data: ndarray, shape((n, 2), m)
-            The numpy array containing the data.
-            Each entry is coupled within a tuple with its
-            corresponding label
-        train_size: float, optional, default: 0.7
-            The proportion, between 0 and 1, that the train
-            set will take on the whole dataset.
-
-        Returns
-        -------
-        out: tuple of length 4
-            The first element is the train set for features.
-            The second is the validation set for features.
-            The third is the train set for the labels.
-            The fourth is the validation set for labels.
-    """
-    img_size = 224
-    train = data[:int(len(data) * train_size)]
-    val = data[int(len(data) * train_size):]
-
-    x_train = []
-    y_train = []
-    x_val = []
-    y_val = []
-
-    for feature, label in train:
-        x_train.append(feature)
-        y_train.append(label)
-
-    for feature, label in val:
-        x_val.append(feature)
-        y_val.append(label)
-
-    x_train = np.array(x_train) / 255
-    x_val = np.array(x_val) / 255
-
-    x_train.reshape(-1, img_size, img_size, 1)
-    y_train = np.array(y_train)
-
-    x_val.reshape(-1, img_size, img_size, 1)
-    y_val = np.array(y_val)
-
-    y_train = to_categorical(y_train, 2)
-    y_val = to_categorical(y_val, 2)
-    return x_train, x_val, y_train, y_val
+import os
+import pathlib
+import pickle
+import shutil
+import sys
+from random import randint
+
+import seaborn as sns
+from tensorflow import keras
+
+import matplotlib.pyplot as plt
+import numpy as np
+import pandas as pd
+import tensorflow as tf
+from keras import layers
+from keras.models import Sequential, Model, load_model
+from matplotlib import transforms
+from keras.preprocessing.image import ImageDataGenerator
+from keras.layers import Dense, Conv2D, MaxPool2D, Flatten, Dropout
+from keras.callbacks import CSVLogger
+from keras.utils.np_utils import to_categorical
+from tensorflow.keras.optimizers import Adam
+
+from matplotlib.collections import PathCollection
+from matplotlib.legend_handler import HandlerPathCollection, HandlerLine2D
+from matplotlib.patches import Ellipse
+from sklearn.decomposition import PCA
+from sklearn.ensemble import RandomForestClassifier
+from sklearn.model_selection import train_test_split
+from sklearn.preprocessing import StandardScaler
+from umap import UMAP
+
+from fiiireflyyy import firefiles as ff
+
+
+def k_fold_cross_validation_deprecated(k_fold, x, y, clf=None, loading=False, clf_path=''):
+    """
+    DEPRECATED - Compute a K-fold cross validation method.
+
+    :param k_fold: Number of folds to split the dataset
+    :param x: Features dataset
+    :param y: target dataset
+    :param clf: classifier object, if loading is False.
+    :param clf_path: path of a classifier object, if loading is True.
+    :param loading: Whether to load a classifier object from path or not.
+    :return: k-fold scores, accuracy
+    """
+    if len(x) != len(y):
+        raise ValueError("Features and Targets do not have the same length.")
+
+    data_len = len(y)
+
+    if loading:
+        if clf_path == '':
+            raise ValueError('No classifier path specified.')
+        else:
+            clf = pickle.load(open(clf_path, "rb"))
+    elif clf is None:
+        raise ValueError("no classifier object specified.")
+
+    ori_x_train, ori_x_test, ori_y_train, ori_y_test = train_test_split(x, y, test_size=0.3)
+    train_len = len(ori_y_train)
+    test_len = len(ori_y_test)
+    local_scores = []
+    step = int(train_len / k_fold)
+    clf.fit(ori_x_train, ori_y_train)
+    for k in range(0, train_len - step, step):
+        x_train_split = ori_x_train.iloc[k:k + step]
+        y_train_split = ori_y_train.iloc[k:k + step]
+        y_test_split = pd.concat([ori_y_test.iloc[0:k], ori_y_test.iloc[k + step:data_len]])
+        x_test_split = pd.concat([ori_x_test.iloc[0:k], ori_x_test.iloc[k + step:data_len]])
+        # clf.fit(x_train_split, y_train_split)
+        local_scores.append(clf.score(x_test_split, y_test_split))
+
+    return local_scores
+
+
+def generate_classes(data_dir, destination, targets):
+    """
+    Generate a specific folder structure for Keras models by isolating classes as different folders.
+
+    :param data_dir:
+    :type data_dir: str
+    :param destination: Where to generate the classes folders
+    :type destination: str
+    :param targets: the different classes to use
+    :type targets: str
+    :return:
+    """
+    ff.verify_dir(destination)
+    files = ff.get_all_files(data_dir)
+
+    # Creating directories architecture for keras model
+    for target in targets:
+        ff.verify_dir(os.path.join(destination, target))
+
+        for file in files:
+            if target in file:
+                shutil.copy2(file, os.path.join(destination, target))
+
+
+def basic_keras(model_spec, src, dst, img_size, epochs=10, visualize=False, saving=True):
+    """
+    Compute a basic Keras model for a images binary classification problem.
+
+    :param model_spec: the name of the model. Identical to the root folder that will contain the model.
+    :type model_spec: str
+    :param src: Where to find the data.
+    :type src: str
+    :param dst: Where to save the sorted data
+    :type dst: str
+    :param img_size: the size of the image.
+    :type img_size: tuple[int]
+    :param epochs: The number of epochs of the model. Default at 10.
+    :param visualize: To visualize the model's results
+    :type visualize: bool
+    :param saving: To save the model's results
+    :type saving: bool
+    :return:
+    """
+    # generate_classes(src, dst, targets=['INF', 'NI'])
+    # Getting the dataset
+
+    data_dir = pathlib.Path(dst)
+    image_count = len(list(data_dir.glob('*.png')))
+    print(image_count)
+
+    # loading data
+    batch_size = 8
+    img_height = img_size[0]
+    img_width = img_size[1]
+
+    train_ds = tf.keras.utils.image_dataset_from_directory(
+        data_dir,
+        validation_split=0.2,
+        subset='training',
+        seed=123,
+        image_size=(img_height, img_width),
+        batch_size=batch_size)
+
+    val_ds = tf.keras.utils.image_dataset_from_directory(
+        data_dir,
+        validation_split=0.2,
+        subset='validation',
+        seed=123,
+        image_size=(img_height, img_width),
+        batch_size=batch_size)
+
+    class_names = train_ds.class_names
+    print(class_names)
+
+    # Visualizing data
+    if visualize:
+        plt.figure(figsize=(10, 10))
+        for images, labels in train_ds.take(1):
+            for i in range(9):
+                ax = plt.subplot(3, 3, i + 1)
+                plt.imshow(images[i].numpy().astype("uint8"))
+                plt.title(class_names[labels[i]])
+                plt.axis("off")
+        plt.show()
+
+    for image_batch, labels_batch in train_ds:
+        print(image_batch.shape)
+        print(labels_batch.shape)
+        break
+
+    # Configure the dataset for performance
+
+    AUTOTUNE = tf.data.AUTOTUNE
+
+    train_ds = train_ds.cache().shuffle(
+        1000)  # .prefetch(buffer_size=AUTOTUNE)  # Once loaded, keep the pictures in memory
+    val_ds = val_ds.cache().prefetch(buffer_size=AUTOTUNE)  # Overlaps data preprocessing/model execution while training
+
+    # Data augmentation
+    data_augmentation = keras.Sequential(
+        [
+            layers.RandomFlip("horizontal_and_vertical",
+                              input_shape=(img_height,
+                                           img_width,
+                                           3)),
+            layers.RandomRotation(1.0),
+            layers.RandomZoom(0.5),
+        ]
+    )
+
+    # Basic Keras model
+    num_classes = len(class_names)
+    model = Sequential([
+        data_augmentation,
+        layers.Rescaling(1. / 255),
+        layers.Conv2D(16, 3, padding='same', activation='relu'),
+        layers.MaxPooling2D(),
+        layers.Conv2D(32, 3, padding='same', activation='relu'),
+        layers.MaxPooling2D(),
+        layers.Conv2D(64, 3, padding='same', activation='relu'),
+        layers.MaxPooling2D(),
+        layers.Dropout(0.2),
+        layers.Flatten(),
+        layers.Dense(128, activation='relu'),
+        layers.Dense(num_classes, name="outputs")
+    ])
+
+    model.compile(optimizer='adam',
+                  loss=tf.keras.losses.SparseCategoricalCrossentropy(from_logits=True),
+                  metrics=['accuracy'])
+
+    model.summary()
+
+    # Train the model
+
+    history = model.fit(
+        train_ds,
+        validation_data=val_ds,
+        epochs=epochs
+    )
+
+    # Visualize training
+    acc = history.history['accuracy']
+    val_acc = history.history['val_accuracy']
+
+    loss = history.history['loss']
+    val_loss = history.history['val_loss']
+
+    epochs_range = range(epochs)
+
+    plt.figure(figsize=(8, 8))
+    plt.subplot(1, 2, 1)
+    plt.plot(epochs_range, acc, label='Training Accuracy')
+    plt.plot(epochs_range, val_acc, label='Validation Accuracy')
+    plt.legend(loc='lower right')
+    plt.title('Training and Validation Accuracy')
+
+    plt.subplot(1, 2, 2)
+    plt.plot(epochs_range, loss, label='Training Loss')
+    plt.plot(epochs_range, val_loss, label='Validation Loss')
+    plt.legend(loc='upper right')
+    plt.title('Training and Validation Loss')
+
+    save_path = os.path.join(os.path.join(pathlib.Path(dst).parent.parent.absolute(), "RESULTS"), model_spec,
+                             "training validation acc loss.png")
+    ff.verify_dir(os.path.join(os.path.join(pathlib.Path(dst).parent.parent.absolute(), "RESULTS"), model_spec))
+    if saving:
+        plt.savefig(save_path)
+    if visualize:
+        plt.show()
+    plt.close()
+
+
+def keras_tutorial():
+    """
+    A tutorial use of keras model for image multiclass classification
+
+    :return:
+    """
+    # downloading the test dataset
+    dataset_url = "https://storage.googleapis.com/download.tensorflow.org/example_images/flower_photos.tgz"
+    data_dir = tf.keras.utils.get_file('flower_photos', origin=dataset_url, untar=True)
+    data_dir = pathlib.Path(data_dir)
+    image_count = len(list(data_dir.glob('*/*.jpg')))
+
+    # loading data using keras
+    batch_size = 32
+    img_height = 180
+    img_width = 180
+
+    train_ds = tf.keras.utils.image_dataset_from_directory(
+        data_dir,
+        validation_split=0.2,
+        subset="training",
+        seed=123,
+        image_size=(img_height, img_width),
+        batch_size=batch_size)
+
+    val_ds = tf.keras.utils.image_dataset_from_directory(
+        data_dir,
+        validation_split=0.2,
+        subset="validation",
+        seed=123,
+        image_size=(img_height, img_width),
+        batch_size=batch_size)
+
+    class_names = train_ds.class_names
+    print(class_names)
+
+    # Visualizing data
+    plt.figure(figsize=(10, 10))
+    for images, labels in train_ds.take(1):
+        for i in range(9):
+            ax = plt.subplot(3, 3, i + 1)
+            plt.imshow(images[i].numpy().astype("uint8"))
+            plt.title(class_names[labels[i]])
+            plt.axis("off")
+    plt.show()
+
+    for image_batch, labels_batch in train_ds:
+        print(image_batch.shape)
+        print(labels_batch.shape)
+        break
+
+    # Configure the dataset for performance
+
+    AUTOTUNE = tf.data.AUTOTUNE
+
+    train_ds = train_ds.cache().shuffle(1000).prefetch(buffer_size=AUTOTUNE)  # Once loaded, keep the pictures in memory
+    val_ds = val_ds.cache().prefetch(buffer_size=AUTOTUNE)  # Overlaps data preprocessing/model execution while training
+
+    # Data augmentation
+    data_augmentation = keras.Sequential(
+        [
+            layers.RandomFlip("horizontal",
+                              input_shape=(img_height,
+                                           img_width,
+                                           3)),
+            layers.RandomRotation(0.1),
+            layers.RandomZoom(0.1),
+        ]
+    )
+
+    # Basic Keras model
+    num_classes = len(class_names)
+    model = Sequential([
+        data_augmentation,
+        layers.Rescaling(1. / 255),
+        layers.Conv2D(16, 3, padding='same', activation='relu'),
+        layers.MaxPooling2D(),
+        layers.Conv2D(32, 3, padding='same', activation='relu'),
+        layers.MaxPooling2D(),
+        layers.Conv2D(64, 3, padding='same', activation='relu'),
+        layers.MaxPooling2D(),
+        layers.Dropout(0.2),
+        layers.Flatten(),
+        layers.Dense(128, activation='relu'),
+        layers.Dense(num_classes, name="outputs")
+    ])
+
+    model.compile(optimizer='adam',
+                  loss=tf.keras.losses.SparseCategoricalCrossentropy(from_logits=True),
+                  metrics=['accuracy'])
+
+    model.summary()
+
+    # Train the model
+    epochs = 15
+    history = model.fit(
+        train_ds,
+        validation_data=val_ds,
+        epochs=epochs
+    )
+
+    # Visualize training
+    acc = history.history['accuracy']
+    val_acc = history.history['val_accuracy']
+
+    loss = history.history['loss']
+    val_loss = history.history['val_loss']
+
+    epochs_range = range(epochs)
+
+    plt.figure(figsize=(8, 8))
+    plt.subplot(1, 2, 1)
+    plt.plot(epochs_range, acc, label='Training Accuracy')
+    plt.plot(epochs_range, val_acc, label='Validation Accuracy')
+    plt.legend(loc='lower right')
+    plt.title('Training and Validation Accuracy')
+
+    plt.subplot(1, 2, 2)
+    plt.plot(epochs_range, loss, label='Training Loss')
+    plt.plot(epochs_range, val_loss, label='Validation Loss')
+    plt.legend(loc='upper right')
+    plt.title('Training and Validation Loss')
+    plt.show()
+
+    # Predict on new data
+    sunflower_url = "https://storage.googleapis.com/download.tensorflow.org/example_images/592px-Red_sunflower.jpg"
+    sunflower_path = tf.keras.utils.get_file('Red_sunflower', origin=sunflower_url)
+
+    img = tf.keras.utils.load_img(
+        sunflower_path, target_size=(img_height, img_width)
+    )
+    img_array = tf.keras.utils.img_to_array(img)
+    img_array = tf.expand_dims(img_array, 0)  # Create a batch
+
+    predictions = model.predict(img_array)
+    score = tf.nn.softmax(predictions[0])
+
+    print(
+        "This image most likely belongs to {} with a {:.2f} percent confidence."
+        .format(class_names[np.argmax(score)], 100 * np.max(score))
+    )
+
+
+def train_RFC_from_dataset(dataset: pd.DataFrame, savepath=""):
+    """
+    Train a Random Forest Classifier model from an already formatted dataset.
+
+        Parameters
+        ----------
+        dataset : pandas Dataframe
+            a pandas Dataframe where each row is an entry for a machine
+            learning model. Has a last column as 'target' containing
+            the target value for each entry.
+
+        savepath: str, optional, default:''
+            name of the saved file. If empty, does not save the file.
+
+            .. versionadded:: 1.0.0
+
+        Returns
+        -------
+        out : tuple of size (1, 2).
+            The first element is a trained random forest classifier.
+            The second is its scores.
+    """
+
+    clf = RandomForestClassifier(n_estimators=1000)
+    X = dataset[dataset.columns[:-1]]
+    y = dataset["label"]
+    X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.5)
+    clf.fit(X_train, y_train)
+    if savepath:
+        pickle.dump(clf, open(savepath, "wb"))
+    return clf, clf.score(X_test, y_test)
+
+
+def get_top_features_from_trained_RFC(clf, **kwargs):
+    """
+    select to top n% feature sorted by highest importance, of a trained Random Forest Classtifier model.
+
+        Parameters
+        ----------
+        clf : RandomForestClassifier
+            a trained model
+
+        **kwargs: keyword arguments
+            percentage: float, optional, default: 0.05
+                proportion of the most important features to keep
+
+            show: bool, optional, default: True
+                Whether to show a plot of the model feature importance or not.
+
+            save: bool, optional, default: False
+                Whether to save a plot of the model feature importance or not.
+
+            title: str, optional, default: ''
+                the title to give the plot and name of the resulting file if save if True.
+
+            savepath: str, optional, default: ""
+                If not empty, path where le result will be saved.
+
+        Returns
+        -------
+        out : tuple of lists
+            first element: list of the indexes of the most important features
+            second element: importance (values) corresponding to the indexes.
+    """
+    options = {"percentage": 0.05,
+               "show": True,
+               "save": False,
+               "title": "",
+               "savepath": ""}
+    options.update(**kwargs)
+
+    importances_over_iterations = []
+    for i in range(10):
+        mean = np.mean([tree.feature_importances_ for tree in clf.estimators_], axis=0)
+
+        importances_over_iterations.append(mean)
+
+    arrays = [np.array(x) for x in importances_over_iterations]
+    mean_importances_over_iterations = [np.mean(k) for k in zip(*arrays)]
+    std_arrays = [np.array(x) for x in importances_over_iterations]
+    std_importances_over_iterations = [np.std(k) for k in zip(*std_arrays)]
+
+    low_std = []
+    for i in range(len(mean_importances_over_iterations)):
+        low_std.append(mean_importances_over_iterations[i] - std_importances_over_iterations[i])
+    high_std = []
+    for i in range(len(mean_importances_over_iterations)):
+        high_std.append(mean_importances_over_iterations[i] + std_importances_over_iterations[i])
+
+    hertz = []
+    factor = 5000 / 300
+    for i in range(300):
+        hertz.append(int(i * factor))
+    n = int(options["percentage"] * len(mean_importances_over_iterations))
+    idx_foi = sorted(range(len(mean_importances_over_iterations)),
+                     key=lambda i: mean_importances_over_iterations[i], reverse=True)[:n]
+
+    plt.bar([x for x in range(300)], mean_importances_over_iterations, color="blue", )
+
+    xticks = [x for x in range(0, 300, 50)]
+    new_ticks = [hertz[x] for x in xticks]
+    xticks.append(300)
+    new_ticks.append(5000)
+    plt.xticks(xticks, new_ticks)
+    plt.ylabel("Relative importance [AU]")
+    plt.xlabel("Frequency-like features [Hz]")
+    plt.title(options["title"])
+    if options["save"]:
+        plt.savefig(options["savepath"])
+    # plt.fill_between(hertz, low_std, high_std, facecolor="blue", alpha=0.5)
+    if options["save"]:
+        plt.show()
+    plt.close()
+    return idx_foi, mean_importances_over_iterations
+
+
+def fit_pca(dataframe: pd.DataFrame, n_components=3):
+    """
+    fit a Principal Component Analysis and return its instance and dataset.
+
+        Parameters
+        ----------
+        dataframe: DataFrame
+            The data on which the pca instance has to be fitted.
+        n_components: int, optional, default: 3
+            The number of components for the PCA instance.
+
+        Returns
+        -------
+        out: tuple of shape (1, 3)
+            The first element is the PCA instance. The second
+            element is the resulting dataframe. The third is the
+            explained variance ratios.
+    """
+    features = dataframe.columns[:-1]
+    x = dataframe.loc[:, features].values
+    x = StandardScaler().fit_transform(x)  # normalizing the features
+    pca = PCA(n_components=n_components)
+    principalComponent = pca.fit_transform(x)
+    principal_component_columns = [f"principal component {i + 1}" for i in range(n_components)]
+
+    principal_tahyna_Df = pd.DataFrame(data=principalComponent
+                                       , columns=principal_component_columns)
+
+    principal_tahyna_Df["label"] = dataframe["label"]
+
+    return pca, principal_tahyna_Df, pca.explained_variance_ratio_
+
+
+def apply_pca(pca, dataframe):
+    """
+    Transform data using an already fit PCA instance.
+
+        Parameters
+        ----------
+        pca: PCA instance
+            The fitted PCA instance from what the data will
+            be transformed.
+        dataframe: DataFrame
+            The data to transform using an already fitted PCA.
+            Must have a 'label' column.
+
+        Returns
+        -------
+        out: DataFrame
+            The transformed data.
+    """
+    features = dataframe.columns[:-1]
+    x = dataframe.loc[:, features].values
+    x = StandardScaler().fit_transform(x)  # normalizing the features
+    transformed_ds = pca.transform(x)
+    transformed_df = pd.DataFrame(data=transformed_ds,
+                                  columns=[f"principal component {i + 1}" for i in range(transformed_ds.shape[1])])
+    transformed_df['label'] = dataframe['label']
+    return transformed_df
+
+
+def confidence_ellipse(x, y, ax, n_std=3.0, color='none', **kwargs):
+    """
+    Create a plot of the covariance confidence ellipse of *x* and *y*.
+
+        Parameters
+        ----------
+        x, y : array-like, shape (n, )
+            Input data.
+
+        ax : matplotlib.axes.Axes
+            The axes object to draw the ellipse into.
+
+        n_std : float
+            The number of standard deviations to determine the ellipse's radiuses.
+
+        color : str
+            color of the ellipsis.
+
+        **kwargs
+            Forwarded to `~matplotlib.patches.Ellipse`
+
+        Returns
+        -------
+        matplotlib.patches.Ellipse
+    """
+    if x.size != y.size:
+        raise ValueError("x and y must be the same size")
+
+    cov = np.cov(x, y)
+    pearson = cov[0, 1] / np.sqrt(cov[0, 0] * cov[1, 1])
+    # Using a special case to obtain the eigenvalues of this
+    # two-dimensional dataset.
+    ell_radius_x = np.sqrt(1 + pearson)
+    ell_radius_y = np.sqrt(1 - pearson)
+    ellipse = Ellipse((0, 0), width=ell_radius_x * 2, height=ell_radius_y * 2,
+                      color=color, **kwargs)
+
+    # Calculating the standard deviation of x from
+    # the squareroot of the variance and multiplying
+    # with the given number of standard deviations.
+    scale_x = np.sqrt(cov[0, 0]) * n_std
+    mean_x = np.mean(x)
+
+    # calculating the standard deviation of y ...
+    scale_y = np.sqrt(cov[1, 1]) * n_std
+    mean_y = np.mean(y)
+
+    transf = transforms.Affine2D() \
+        .rotate_deg(45) \
+        .scale(scale_x, scale_y) \
+        .translate(mean_x, mean_y)
+
+    ellipse.set_transform(transf + ax.transData)
+    return ax.add_patch(ellipse)
+
+
+def plot_pca(dataframe: pd.DataFrame, **kwargs):
+    """
+    plot the result of PCA.
+
+        Parameters
+        ----------
+        dataframe: DataFrame
+            The data to plot. Must contain a 'label' column.
+
+        **kwargs: keyword arguments
+            n_components: int, optional, default: 2
+                Number of principal components. Also, teh dimension
+                of the graph. Must be equal to 2 or 3.
+            show: bool, optional, default: True
+                Whether to show the plot or not.
+            save: bool, optional, default: False
+                Whether to save the plot or not.
+            commentary: str, optional, default: "T=48H"
+                Any specification to include in the file name while saving.
+            points: bool, optional, default: True
+                whether to plot the points or not.
+            metrics: bool, optional, default: False
+                Whether to plot the metrics or not
+            savedir: str, optional, default: ""
+                Directory where to save the resulting plot, if not empty.
+            title: str, optional, defualt: ""
+                The filename of the resulting plot. If empty,
+                an automatic name will be generated.
+            ratios: tuple of float, optional, default: ()
+                the PCA explained variance ratio, to display on
+                the plot axis.
+    """
+
+    options = {
+        'n_components': 2,
+        'show': True,
+        'commentary': "",
+        'points': True,
+        'metrics': False,
+        'savedir': "",
+        'pc_ratios': [],
+        'title': "",
+        'ratios': ()
+
+    }
+
+    options.update(kwargs)
+    targets = dataframe["label"].unique()
+    colors = ['g', 'b', 'r', 'k', 'sandybrown', 'deeppink', 'gray']
+    if len(targets) > len(colors):
+        n = len(targets) - len(colors) + 1
+        for i in range(n):
+            colors.append('#%06X' % randint(0, 0xFFFFFF))
+
+    if options['n_components'] == 2:
+        label_params = {'fontsize': 30, "labelpad": 8}
+        ticks_params = {'fontsize': 30, }
+        fig, ax = plt.subplots(1, 1, figsize=(12, 10))
+
+        plt.xticks(**ticks_params)
+        plt.yticks(**ticks_params)
+        xlabel = f'Principal Component-1 ({options["ratios"][0]}%)'
+        ylabel = f'Principal Component-2 ({options["ratios"][1]}%)'
+        if len(options['pc_ratios']):
+            xlabel += f" ({round(options['pc_ratios'][0] * 100, 2)}%)"
+            ylabel += f" ({round(options['pc_ratios'][1] * 100, 2)}%)"
+
+        plt.xlabel(xlabel, **label_params)
+        plt.ylabel(ylabel, **label_params)
+
+        for target, color in zip(targets, colors):
+            indicesToKeep = dataframe['label'] == target
+            x = dataframe.loc[indicesToKeep, 'principal component 1']
+            y = dataframe.loc[indicesToKeep, 'principal component 2']
+            if options['points']:
+                alpha = 1
+                if options['metrics']:
+                    alpha = .2
+                plt.scatter(x, y, c=color, s=10, alpha=alpha, label=target)
+            if options['metrics']:
+                plt.scatter(np.mean(x), np.mean(y), marker="+", color=color, linewidth=2, s=160)
+                confidence_ellipse(x, y, ax, n_std=1.0, color=color, fill=False, linewidth=2)
+
+        def update(handle, orig):
+            handle.update_from(orig)
+            handle.set_alpha(1)
+
+        plt.legend(prop={'size': 25}, handler_map={PathCollection: HandlerPathCollection(update_func=update),
+                                                   plt.Line2D: HandlerLine2D(update_func=update)})
+    elif options['n_components'] == 3:
+        label_params = {'fontsize': 20, "labelpad": 8}
+        ticks_params = {'fontsize': 20, }
+        plt.figure(figsize=(10, 10))
+        ax = plt.axes(projection='3d')
+
+        xlabel = f'Principal Component-1 ({options["ratios"][0]}%)'
+        ylabel = f'Principal Component-2 ({options["ratios"][1]}%)'
+        zlabel = f'Principal Component-3 ({options["ratios"][2]}%)'
+        if len(options['pc_ratios']):
+            xlabel += f" ({round(options['pc_ratios'][0] * 100, 2)}%)"
+            ylabel += f" ({round(options['pc_ratios'][1] * 100, 2)}%)"
+            zlabel += f" ({round(options['pc_ratios'][2] * 100, 2)}%)"
+
+        ax.set_xlabel(xlabel, **label_params)
+        ax.set_ylabel(ylabel, **label_params)
+        ax.set_zlabel(zlabel, **label_params)
+        for target, color in zip(targets, colors):
+            indicesToKeep = dataframe['label'] == target
+            x = dataframe.loc[indicesToKeep, 'principal component 1']
+            y = dataframe.loc[indicesToKeep, 'principal component 2']
+            z = dataframe.loc[indicesToKeep, 'principal component 3']
+            ax.scatter3D(x, y, z, c=color, s=10)
+        plt.legend(targets, prop={'size': 18})
+
+    if options['savedir']:
+        if options["title"] == "":
+            if options['commentary']:
+                options["title"] += options["commentary"]
+
+        plt.savefig(os.path.join(options['savedir'], options["title"] + ".png"), dpi=1200)
+
+    if options['show']:
+        plt.show()
+    plt.close()
+
+
+def fit_umap(dataframe, n_components=3):
+    """
+    fit a Uniform Manifold Approximated Projection and return its instance and dataset.
+
+        Parameters
+        ----------
+        dataframe: DataFrame
+            The data on which the umap instance has to be fitted.
+            Contains a column 'label'.
+        n_components: int, optional, default: 3
+            The number of components for the UMAP instance.
+
+        Returns
+        -------
+        out: tuple of shape (1, 2)
+            The first element is the UMAP instance. The second
+            element is the resulting dataframe.
+    """
+    # Configure UMAP hyperparameters
+    features = dataframe.columns[:-1]
+    x = dataframe.loc[:, features].values
+    reducer = UMAP(n_neighbors=100,
+                   n_components=n_components,  # default 2, The dimension of the space to embed into.
+                   metric='euclidean',
+                   n_epochs=1000,
+                   learning_rate=1.0, )
+
+    # Fit and transform the data
+    X_trans = reducer.fit_transform(x)
+    X_dimension = [f"dimension {i + 1}" for i in range(n_components)]
+    transformed_df = pd.DataFrame(data=X_trans, columns=X_dimension)
+
+    transformed_df["label"] = dataframe["label"]
+
+    return reducer, transformed_df
+
+
+def apply_umap(umap, dataframe):
+    """
+    Transform data using an already fit UMAP instance.
+
+       Parameters
+       ----------
+       umap: UMAP instance
+           The fitted PCA instance from what the data will
+           be transformed.
+       dataframe: DataFrame
+           The data to transform using an already fitted PCA.
+           Must have a 'label' column.
+
+       Returns
+       -------
+       out: DataFrame
+           The transformed data.
+   """
+    features = dataframe.columns[:-1]
+    x = dataframe.loc[:, features].values
+    x = StandardScaler().fit_transform(x)  # normalizing the features
+    transformed_ds = umap.transform(x)
+    transformed_df = pd.DataFrame(data=transformed_ds,
+                                  columns=[f"dimension {i + 1}" for i in range(transformed_ds.shape[1])])
+    transformed_df['label'] = dataframe['label']
+    return transformed_df
+
+
+def plot_umap(dataframe, **kwargs):
+    """
+    plot the result of UMAP.
+
+        Parameters
+        ----------
+        dataframe: DataFrame
+            The data to plot. Must contain a 'label' column.
+
+        **kwargs: keyword arguments
+            n_components: int, optional, default: 3
+                Number of principal components. Also, teh dimension
+                of the graph. Must be equal to 2 or 3.
+            show: bool, optional, default: True
+                Whether to show the plot or not.
+            save: bool, optional, default: False
+                Whether to save the plot or not.
+            commentary: str, optional, default: ""
+                Any specification to include in the file name while saving.
+            points: bool, optional, default: True
+                whether to plot the points or not.
+            metrics: bool, optional, default: False
+                Whether to plot the metrics or not
+            savedir: str, optional, default: ""
+                Directory where to save the resulting plot, if not empty.
+    """
+    options = {"n_components": 3, "show": True, "save": False, "commentary": "", "points": True,
+               "metrics": False, "savedir": ""}
+    options.update(**kwargs)
+    targets = dataframe["label"].unique()
+    colors = ['r', 'g', 'b', 'k', 'sandybrown', 'deeppink', 'gray']
+    if len(targets) > len(colors):
+        n = len(targets) - len(colors) + 1
+        for i in range(n):
+            colors.append('#%06X' % randint(0, 0xFFFFFF))
+    if options["n_components"] == 2:
+        fig, ax = plt.subplots(1, 1, figsize=(10, 10))
+        plt.xticks(fontsize=12)
+        plt.yticks(fontsize=14)
+        plt.xlabel(f'PC-1', fontsize=20)
+        plt.ylabel(f'PC-2', fontsize=20)
+        plt.title(f"Uniform Manifold Approximated Projection", fontsize=20)
+        for target, color in zip(targets, colors):
+            indicesToKeep = dataframe['label'] == target
+            x = dataframe.loc[indicesToKeep, 'dimension 1']
+            y = dataframe.loc[indicesToKeep, 'dimension 2']
+            if options["points"]:
+                alpha = 1
+                if options["metrics"]:
+                    alpha = .2
+                plt.scatter(x, y, c=color, s=10, alpha=alpha, label=target)
+            if options["metrics"]:
+                plt.scatter(np.mean(x), np.mean(y), marker="+", color=color, linewidth=2, s=160)
+                confidence_ellipse(x, y, ax, n_std=1.0, color=color, fill=False, linewidth=2)
+
+        def update(handle, orig):
+            handle.update_from(orig)
+            handle.set_alpha(1)
+
+        plt.legend(prop={'size': 15}, handler_map={PathCollection: HandlerPathCollection(update_func=update),
+                                                   plt.Line2D: HandlerLine2D(update_func=update)})
+    if options["n_components"] == 3:
+        plt.figure(figsize=(10, 10))
+        ax = plt.axes(projection='3d')
+        ax.set_xlabel(f'dimension-1', fontsize=20)
+        ax.set_ylabel(f'dimension-2', fontsize=20)
+        ax.set_zlabel(f'dimension-3', fontsize=20)
+        for target, color in zip(targets, colors):
+            indicesToKeep = dataframe['label'] == target
+            x = dataframe.loc[indicesToKeep, dataframe.columns[0]]
+            y = dataframe.loc[indicesToKeep, dataframe.columns[1]]
+            z = dataframe.loc[indicesToKeep, dataframe.columns[2]]
+            ax.scatter3D(x, y, z, c=color, s=10, label='bla')
+        plt.legend(targets, prop={'size': 15})
+        plt.title(f"Uniform Manifold Approximated Projection", fontsize=20)
+
+    if options["savedir"]:
+        if options["commentary"]:
+            plt.savefig(os.path.join(options["savedir"],
+                                     f"UMAP n={options['n_components']} t={targets} {options['commentary']}.png"))
+        else:
+            plt.savefig(os.path.join(options["savedir"], f"UMAP n={options['n_']} t={targets}.png"))
+
+    if options["show"]:
+        plt.show()
+    plt.close()
+
+
+def test_rfc_by_confusion(clf, dataset: pd.DataFrame, training_targets: tuple, **kwargs):
+    """
+    Test an already trained Random forest classifier model,
+    resulting in a confusion matrix. The test can be done
+    on targets_labels different from the targets_labels used for training
+    the model.
+        Parameters
+        ----------
+        clf: RandomForestClassifier
+            the trained model.
+        dataset:  pandas Dataframe.
+            Dataframe containing the data used for testing the
+            model. The rows are the entries, and the columns are
+            the features on which the model has been trained.
+            The last column is 'status' containing the labels
+            of the targets_labels for each entry.
+        training_targets: tuple of str
+            the targets on which the model has been trained.
+        **kwargs: keyword arguments
+            savepath: str, optional, default: ""
+                If not empty, path where le result will be saved.
+            verbose: Bool, optional. Default: False
+                Whether to display more information when computing
+                or not.
+            show: Bool, optional. Default: True
+                Whether to show the resulting confusion matrix or not.
+            iterations: int, optional. Default: 10
+                Number of iterations the test will be computed.
+            commentary: str, optional. Default: ""
+                If any specification to add to the file name.
+            testing_targets: tuple of str
+                the targets on which the model will be tested.
+                Can be different from the training targets.
+    """
+    options = {"verbose": False, "show": True,
+               "testing_targets": (),
+               "iterations": 10,
+               "commentary": "", "savepath": "", "title": ""}
+    options.update(**kwargs)
+    if not options["testing_targets"]:
+        options["testing_targets"] = training_targets
+    CORRESPONDANCE = {}
+    target_id = 0
+    for t in training_targets:
+        if t not in CORRESPONDANCE:
+            CORRESPONDANCE[t] = target_id
+            target_id += 1
+    for t in options["testing_targets"]:
+        if t not in CORRESPONDANCE:
+            CORRESPONDANCE[t] = target_id
+            target_id += 1
+    X = dataset[dataset.columns[:-1]]
+    y = dataset["label"]
+
+    if options["verbose"]:
+        progress = 0
+        sys.stdout.write(f"\rTesting model: {progress}%")
+        sys.stdout.flush()
+
+    X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.3)
+
+    # get predictions and probabilities
+    all_matrixes = []
+    all_probability_matrixes = []
+    for iters in range(options["iterations"]):
+        matrix = np.zeros((len(training_targets), len(options['testing_targets'])))
+        probabilities_matrix = np.empty((len(training_targets), len(options['testing_targets'])), dtype=object)
+
+        # Initializing the matrix containing the probabilities
+        for i in range(len(probabilities_matrix)):
+            for j in range(len(probabilities_matrix[i])):
+                probabilities_matrix[i][j] = []
+
+        # Making predictions and storing the results in predictions[]
+        predictions = []
+        for i in X_test.index:
+            row = X_test.loc[i, :]
+            y_pred = clf.predict([row])[0]
+            proba_class = clf.predict_proba([row])[0]
+            predictions.append((y_pred, proba_class))
+
+        #
+        targets = []
+        for i in y_test.index:
+            targets.append(y_test.loc[i])
+        # Building the confusion matrix
+        for i in range(len(targets)):
+            y_true = targets[i]
+            y_pred = predictions[i][0]
+            y_proba = max(predictions[i][1])
+            matrix[CORRESPONDANCE[y_pred]][CORRESPONDANCE[y_true]] += 1
+
+            probabilities_matrix[CORRESPONDANCE[y_pred]][CORRESPONDANCE[y_true]].append(y_proba)
+        mean_probabilities = np.zeros((len(training_targets), len(options['testing_targets'])))
+        for i in range(len(probabilities_matrix)):
+            for j in range(len(probabilities_matrix[i])):
+                mean_probabilities[i][j] = np.mean(probabilities_matrix[i][j])
+        all_matrixes.append(matrix)
+        all_probability_matrixes.append(mean_probabilities)
+
+    mixed_labels_matrix = np.empty((len(training_targets), len(options['testing_targets']))).tolist()
+    mean_probabilities_matrix = np.empty((len(training_targets), len(options['testing_targets'])))
+    overall_matrix = np.mean(np.array([i for i in all_matrixes]), axis=0)
+    overall_probabilities = np.mean(np.array([i for i in all_probability_matrixes]), axis=0)
+
+    # averaging the probabilities
+    for i in range(len(overall_probabilities)):
+        for j in range(len(overall_probabilities[i])):
+            mean_probabilities_matrix[i][j] = np.mean(overall_probabilities[i][j])
+
+    # mixing count and probabilities for displaying
+    for i in range(len(overall_probabilities)):
+        for j in range(len(overall_probabilities[i])):
+            np.nan_to_num(overall_matrix[i][j])
+            np.nan_to_num(mean_probabilities_matrix[i][j])
+            mixed_labels_matrix[i][j] = str(int(overall_matrix[i][j])) + "\nCUP=" + str(
+                round(mean_probabilities_matrix[i][j], 3))
+
+    # plotting
+    fig, ax = plt.subplots(1, 1, figsize=(7 / 4 * len(options['testing_targets']), 6 / 4 * len(training_targets)))
+
+    fig.suptitle("")
+    sns.heatmap(ax=ax, data=overall_matrix, annot=mixed_labels_matrix, fmt='', cmap="Blues")
+    ax.xaxis.tick_top()
+    ax.xaxis.set_label_position('top')
+    ax.set_ylabel("The input is classified as")
+    ax.set_xlabel("The input is")
+    ax.set_xticks([CORRESPONDANCE[x] + 0.5 for x in options['testing_targets']], options['testing_targets'])
+    ax.set_yticks([CORRESPONDANCE[x] + 0.5 for x in training_targets], training_targets)
+    plt.tight_layout()
+
+    if options['savepath']:
+        plt.savefig(os.path.join(options['savepath'], options["title"] + ".png"))
+    if options['show']:
+        plt.show()
+    plt.close()
+
+
+def test_sequential_by_confusion(model_path, dataset, training_targets, **kwargs):
+    """
+    Test an already trained keras Sequential model,
+    resulting in a confusion matrix. The test can be done
+    on targets_labels different from the targets_labels used for training
+    the model.
+        Parameters
+        ----------
+        model_path: str
+            the absolute path to the trained model, with extension (to open).
+        dataset:  list of lists, shape (n, (2, (ndarray(m,m)))
+            list of n pictures of size m*m, coupled with its
+            int-like label.
+        training_targets: list of int
+            the targets on which the model has been trained.
+        **kwargs: keyword arguments
+            savepath: str, optional, default: ""
+                If not empty, path where le result will be saved.
+            verbose: Bool, optional. Default: False
+                Whether to display more information when computing
+                or not.
+            show: Bool, optional. Default: True
+                Whether to show the resulting confusion matrix or not.
+            iterations: int, optional. Default: 10
+                Number of iterations the test will be computed.
+            commentary: str, optional. Default: ""
+                If any specification to add to the file name.
+            testing_targets: list of int
+                the targets on which the model will be tested.
+                Can be different from the training targets.
+            target_rename: dict, optional, default: {}
+                the keys are the actual targets, the values are
+                how you want to rename them on the confusion matrix.
+    """
+    model = load_model(model_path)
+    options = {"verbose": False, "show": True,
+               "testing_targets": (),
+               "iterations": 10,
+               "commentary": "",
+               "savepath": "",
+               "title": "",
+               "target_rename": ""}
+    options.update(**kwargs)
+    if not options["testing_targets"]:
+        options["testing_targets"] = training_targets
+    CORRESPONDANCE = {}
+    target_id = 0
+    for t in training_targets:
+        if t not in CORRESPONDANCE:
+            CORRESPONDANCE[t] = target_id
+            target_id += 1
+    for t in options["testing_targets"]:
+        if t not in CORRESPONDANCE:
+            CORRESPONDANCE[t] = target_id
+            target_id += 1
+    x_train, x_val, y_train, y_val = split_train_test(dataset, train_size=0.1)
+
+    x_val = np.array(x_val)
+    y_val = np.array(y_val)
+
+    # get predictions and probabilities
+    all_matrixes = []
+    all_probability_matrixes = []
+    for iters in range(options["iterations"]):
+        matrix = np.zeros((len(training_targets), len(options['testing_targets'])))
+        probabilities_matrix = np.empty((len(training_targets), len(options['testing_targets'])), dtype=object)
+
+        # Initializing the matrix containing the probabilities
+        for i in range(len(probabilities_matrix)):
+            for j in range(len(probabilities_matrix[i])):
+                probabilities_matrix[i][j] = []
+
+        # Making predictions and storing the results in predictions[]
+        predictions = []
+        for x in x_val:
+            y_pred = model.predict(x[None, ...])[0]
+            predictions.append((np.where(y_pred == max(y_pred))[0][0], list(y_pred)))
+
+        targets = []
+        for i in y_val:
+            targets.append(np.where(i == max(i))[0][0])
+        # Building the confusion matrix
+
+        for i in range(len(targets)):
+            y_true = targets[i]
+            y_pred = predictions[i][0]
+            y_proba = max(predictions[i][1])
+
+            matrix[CORRESPONDANCE[y_pred]][CORRESPONDANCE[y_true]] += 1
+
+            probabilities_matrix[CORRESPONDANCE[y_pred]][CORRESPONDANCE[y_true]].append(y_proba)
+        mean_probabilities = np.zeros((len(training_targets), len(options['testing_targets'])))
+        for i in range(len(probabilities_matrix)):
+            for j in range(len(probabilities_matrix[i])):
+                mean_probabilities[i][j] = np.mean(probabilities_matrix[i][j])
+        all_matrixes.append(matrix)
+        all_probability_matrixes.append(mean_probabilities)
+
+    mixed_labels_matrix = np.empty((len(training_targets), len(options['testing_targets']))).tolist()
+    mean_probabilities_matrix = np.empty((len(training_targets), len(options['testing_targets'])))
+    overall_matrix = np.mean(np.array([i for i in all_matrixes]), axis=0)
+    overall_probabilities = np.mean(np.array([i for i in all_probability_matrixes]), axis=0)
+
+    # averaging the probabilities
+    for i in range(len(overall_probabilities)):
+        for j in range(len(overall_probabilities[i])):
+            mean_probabilities_matrix[i][j] = np.mean(overall_probabilities[i][j])
+
+    # mixing count and probabilities for displaying
+    for i in range(len(overall_probabilities)):
+        for j in range(len(overall_probabilities[i])):
+            np.nan_to_num(overall_matrix[i][j])
+            np.nan_to_num(mean_probabilities_matrix[i][j])
+            mixed_labels_matrix[i][j] = str(int(overall_matrix[i][j])) + "\nCUP=" + str(
+                round(mean_probabilities_matrix[i][j], 3))
+
+    # plotting
+    fig, ax = plt.subplots(1, 1, figsize=(7 / 4 * len(options['testing_targets']), 6 / 4 * len(training_targets)))
+
+    fig.suptitle("")
+    sns.heatmap(ax=ax, data=overall_matrix, annot=mixed_labels_matrix, fmt='', cmap="Blues")
+    ax.xaxis.tick_top()
+    ax.xaxis.set_label_position('top')
+    ax.set_ylabel("The input is classified as")
+    ax.set_xlabel("The input is")
+
+    ax.set_xticks([CORRESPONDANCE[x] + 0.5 for x in options['testing_targets']],
+                  [options["target_rename"][x] for x in options['testing_targets']])
+    ax.set_yticks([CORRESPONDANCE[x] + 0.5 for x in training_targets],
+                  [options["target_rename"][x] for x in training_targets])
+    plt.tight_layout()
+
+    if options['savepath']:
+        plt.savefig(os.path.join(options['savepath'], options["title"] + ".png"))
+    if options['show']:
+        plt.show()
+    plt.close()
+
+
+def model_history_plot(history_path, savepath=""):
+    """
+    Save in a fancy way the history logs of a
+    trained keras model, saved in the form of a
+    csv file.
+
+        Parameters
+        ----------
+        history_path: str
+            the absolute path to the .log file,
+            containing the history in csv format.
+        savepath: str, optional, default: ""
+            If not empty, the directory where the plot will be saved.
+            If empty, the plot is shown.
+    """
+    data = pd.read_csv(history_path, index_col=False)
+    plt.figure(figsize=(6, 5))
+    plt.plot(data["accuracy"], linestyle="dashed", color="blue", label="training accuracy")
+    plt.plot(data["val_accuracy"], linestyle="solid", color="blue", label="validation accuracy")
+    plt.plot(data["loss"], linestyle="dashed", color="red", label="training loss")
+    plt.plot(data["val_loss"], linestyle="solid", color="red", label="training loss")
+
+    plt.xlabel("epochs", fontsize=15)
+    plt.ylabel("score", fontsize=15)
+    plt.xticks(fontsize=13)
+    plt.yticks(fontsize=13)
+    plt.legend(fontsize=13)
+    title = "history " + os.path.basename(history_path).replace("history", "").split(".")[0] + ".png"
+    if savepath:
+        plt.savefig(os.path.join(savepath, title))
+    else:
+        plt.show()
+    plt.close()
+
+
+def basic_sequential(data, epochs, comment="", model_savepath="", history_savepath=""):
+    """
+    Use of a generic Convolutional network, use for basic image classification.
+    The inputs are of shape (224, 224).
+
+        Parameters
+        ----------
+        data: ndarray shape((n, 2), m)
+            The numpy array containing the data.
+            Each entry is coupled within a tuple with its
+            corresponding label
+        epochs: int
+            number of epochs to train the model on.
+        comment: str, optional, default: ""
+            Add to the name a comment, used when saving
+            the model and for the model name.
+        savepath: str, optional, default: ""
+            If not empty, directory where to save the model.
+        savepath: str, optional, default: ""
+            If not empty, directory where to save the history plot.
+
+    """
+    x_train, x_val, y_train, y_val = split_train_test(data)
+    datagen = ImageDataGenerator(
+        featurewise_center=False,  # set input mean to 0 over the dataset
+        samplewise_center=False,  # set each sample mean to 0
+        featurewise_std_normalization=False,  # divide inputs by std of the dataset
+        samplewise_std_normalization=False,  # divide each input by its std
+        zca_whitening=False,  # apply ZCA whitening
+        rotation_range=180,  # randomly rotate images in the range (degrees, 0 to 180)
+        zoom_range=0.2,  # Randomly zoom image
+        width_shift_range=0,  # randomly shift images horizontally (fraction of total width)
+        height_shift_range=0,  # randomly shift images vertically (fraction of total height)
+        horizontal_flip=False,  # randomly flip images
+        vertical_flip=False,  # randomly flip images
+    )
+
+    datagen.fit(x_train)
+    model = Sequential()
+
+    model.add(Conv2D(32, 7, padding="same", activation="relu", input_shape=(224, 224, 3)))
+    model.add(MaxPool2D())
+
+    model.add(Conv2D(32, 7, padding="same", activation="relu"))
+    model.add(MaxPool2D())
+
+    model.add(Conv2D(64, 7, padding="same", activation="relu"))
+    model.add(MaxPool2D())
+    model.add(Dropout(0.4))
+
+    model.add(Flatten())
+    model.add(Dense(128, activation="relu"))
+    model.add(Dense(2, activation="softmax"))
+
+    opt = Adam(learning_rate=0.000001)
+    model.compile(optimizer=opt, loss="categorical_crossentropy",
+                  metrics=['accuracy'])
+
+    name = f"e={epochs} basic model{comment}"
+
+    csv_logger = CSVLogger(os.path.join(model_savepath, f"{name} history.log"), separator=',', append=False)
+    history = model.fit(x_train, y_train, epochs=epochs, validation_data=(x_val, y_val), callbacks=[csv_logger])
+    if model_savepath:
+        model.save(os.path.join(model_savepath, f"{name}.h5"))
+    if history_savepath:
+        model_history_plot(os.path.join(model_savepath, f"{name} history.log"), savepath=history_savepath)
+
+
+def split_train_test(data, train_size: float = 0.7):
+    """
+    Split a dataset into train and validation sets for features and labels.
+
+        Parameters
+        ----------
+        data: ndarray, shape((n, 2), m)
+            The numpy array containing the data.
+            Each entry is coupled within a tuple with its
+            corresponding label
+        train_size: float, optional, default: 0.7
+            The proportion, between 0 and 1, that the train
+            set will take on the whole dataset.
+
+        Returns
+        -------
+        out: tuple of length 4
+            The first element is the train set for features.
+            The second is the validation set for features.
+            The third is the train set for the labels.
+            The fourth is the validation set for labels.
+    """
+    img_size = 224
+    train = data[:int(len(data) * train_size)]
+    val = data[int(len(data) * train_size):]
+
+    x_train = []
+    y_train = []
+    x_val = []
+    y_val = []
+
+    for feature, label in train:
+        x_train.append(feature)
+        y_train.append(label)
+
+    for feature, label in val:
+        x_val.append(feature)
+        y_val.append(label)
+
+    x_train = np.array(x_train) / 255
+    x_val = np.array(x_val) / 255
+
+    x_train.reshape(-1, img_size, img_size, 1)
+    y_train = np.array(y_train)
+
+    x_val.reshape(-1, img_size, img_size, 1)
+    y_val = np.array(y_val)
+
+    y_train = to_categorical(y_train, 2)
+    y_val = to_categorical(y_val, 2)
+    return x_train, x_val, y_train, y_val
```

### Comparing `fiiireflyyy-0.1.1/fiiireflyyy/fireprocess.py` & `fiiireflyyy-0.1.2/fiiireflyyy/fireprocess.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,373 +1,373 @@
-import os
-import re
-import sys
-
-import pandas as pd
-import numpy as np
-import fiiireflyyy.firefiles as ff
-from pathlib import Path
-import matplotlib.pyplot as plt
-
-
-def floor_ceil_in_range(value, low_thresh: float == 0.0, high_thresh: float == 255.0):
-    """
-    Thresholds a value considering a minimum and maximum value.
-
-        Parameters
-        ----------
-        value: int, float
-            the value to floor or ceil.
-        low_thresh: float, optional, default: 0.0
-            The minimum limit to thresholds the value
-        high_thresh: float, optional, default: 255.0
-            The maximum limit to thresholds the value.
-
-        Returns
-        -------
-        out: int, float
-            The thresholded value.
-    """
-    if value > high_thresh:
-        return high_thresh
-    elif value < low_thresh:
-        return low_thresh
-    else:
-        return value
-
-
-
-
-def merge_all_columns_to_mean(df: pd.DataFrame, except_column=""):
-    """
-    average all the columns, except an optional specified one,
-    in a dataframe into one. The average is done row-wise.
-
-        Parameters
-        ----------
-        df: DataFrame
-            the dataframe to average
-        except_column: str, optional, default: ""
-            the name of the column to exclude from the average.
-            Will be included in the resulting dataset.
-
-        Returns
-        --------
-        out: DataFrame
-            Dataframe containing on column labeled 'mean', and
-            an optional second column based on the
-            except_column parameter
-    """
-
-    excepted_column = pd.DataFrame()
-    if except_column:
-        for col in df.columns:
-            if except_column in col:
-                except_column = col
-        excepted_column = df[except_column]
-        df.drop(except_column, axis=1, inplace=True)
-
-    df_mean = pd.DataFrame(columns=["mean", ])
-    df_mean['mean'] = df.mean(axis=1)
-
-    if except_column != "":
-        for col in df.columns:
-            if except_column in col:
-                except_column = col
-        df_mean[except_column] = excepted_column
-
-    return df_mean
-
-def equal_samples(df, n):
-    """
-    cuts a DataFrame in n sub-DataFrame of same length.
-
-        Parameters
-        ----------
-        df: DataFrame
-            Object to cut, row-wise.
-        n: int
-            number of resulting samples.
-
-        Returns
-        -------
-        out: list of DataFrame
-            contains all the sub DataFrames.
-    """
-    step = int(len(df) / n)
-    lower_limit = 0
-    upper_limit = step
-    samples = []
-    while upper_limit <= len(df):
-        samples.append(df[lower_limit:upper_limit])
-        lower_limit = upper_limit
-        upper_limit += step
-    return samples
-
-def discard_outliers_by_iqr(df: pd.DataFrame, **kwargs):
-    """
-    remove outliers from a dataframe using the interquartile range method.
-
-        Parameters
-        ----------
-        df: pd.Dataframe
-            the dataframe containing the data.
-            Must contain a column 'label'.
-
-        **kwargs: keyword arguments
-            low_percentile : float, default: 0.25
-                the low percentile for IQR outliers removal.
-            high_percentile : float, default: 0.75
-                the high percentile for IQR outliers removal.
-            iqr_limit_factor : float, default: 1.5
-                the factor used to determine when the point is
-                an outlier compared to the percentiles.
-            save: str, default: ""
-                Where to save the resulting plot.
-                If empty, the plot will not be saved.
-                WARNING : may cause randomly 'Key error: 0'.
-            mode: {'capping', }, default: capping
-                The method used to discard the outliers.
-                More to come.
-
-        Returns
-        -------
-        out: pd.Dataframe
-            the dataframe without the outliers
-    """
-    options = {"low_percentile": 0.25,
-               "high_percentile": 0.75,
-               "iqr_limit_factor": 1.5,
-               "save": "",
-               "mode": "capping"}
-    options.update(kwargs)
-    labels = df["label"].unique()
-    labels_values = {}
-    for n in range(len(labels)):
-        labels_values[labels[n]] = n
-
-    features = list(df.columns.values)
-    features.remove('label')
-    metrics = np.empty(shape=(len(labels), len(features)), dtype=object)
-
-    # obtaining the metrics [lower_limit, upper_limit]
-    for i_label in range(len(labels)):
-        label = labels[i_label]
-        sub_df = df.loc[df['label'] == label]
-        for i_feat in range(len(features)):
-            feat = features[i_feat]
-            # finding the iqr
-            low_percentile = sub_df[feat].quantile(options["low_percentile"])
-            high_percentile = sub_df[feat].quantile(options["high_percentile"])
-            iqr = high_percentile - low_percentile
-            # finding upper and lower limit
-            lower_limit = low_percentile - options["iqr_limit_factor"] * iqr
-            upper_limit = high_percentile + options["iqr_limit_factor"] * iqr
-            metrics[i_label][i_feat] = [lower_limit, upper_limit]
-
-    discarded_df = pd.DataFrame(columns=features)
-    discarded_labels = pd.DataFrame(columns=["label", ])
-
-    for i in range(len(df.values)):
-        discarded_row = []
-        discarded_label = df['label'].iloc[i]
-        for j in range(len(df.values[i]) - 1):
-            lower_limit, upper_limit = metrics[labels_values[discarded_label], j]
-            if options["mode"] == "capping":
-                if df.iloc[i, j] > upper_limit:
-                    discarded_row.append(upper_limit)
-                elif df.iloc[i, j] < lower_limit:
-                    discarded_row.append(lower_limit)
-                else:
-                    discarded_row.append(df.iloc[i, j])
-
-        discarded_labels.loc[len(discarded_labels)] = discarded_label
-        discarded_df.loc[len(discarded_df)] = discarded_row
-
-    discarded_df["label"] = discarded_labels["label"]
-    return discarded_df
-
-
-def smoothing(data, n: int, mode='mean'):
-    """
-    Smoothen a signal down to n values, depending on the smoothing mode.
-
-        Parameters
-        ----------
-        data: list of int, list of float
-            contains the numerical data to smoothen.
-        n: int
-            number of points to down sample the data to.
-        mode: str, optional, default: 'mean'
-            the way to smoothen the data between the points.
-
-        Returns
-        -------
-        out: list of floats
-            the smoothened data.
-
-    """
-    if len(data.index) > n:
-        step = int(len(data.index) / n)
-        lower_limit = 0
-        upper_limit = step
-        ds_data = []
-        if mode == 'mean':
-            while upper_limit <= len(data):
-                ds_data.append(np.mean(data[lower_limit:upper_limit]).round(3))
-                lower_limit = upper_limit
-                upper_limit += step
-        excedent = len(ds_data) - n
-        ds_data = ds_data[:-excedent or None]
-        return ds_data
-    else:
-        raise Exception("smoothing: length of data " + str(len(data.index)) + "< n " + str(n))
-
-
-def make_dataset_from_freq_files(parent_dir, **kwargs):
-    """
-    Use frequency files of format two columns (one column 'Frequencies [Hz]' and one column 'mean') to generate a
-    dataset used for classification. Specialized for recording of electrical signal. The path tree has to be
-    organised as such :
-    base/condition (ej. drug addition)/recording time/target for classification (ej. infected/not
-    infected)/sample number/my_freq_files.csv .
-
-        Parameters
-        ----------
-        parent_dir: str.
-            the parent directory where to look for all the
-            frequency files.
-
-        **kwargs: keyword arguments
-            filename: str, optional. Default: ""
-                the name of the resulting csv file if
-                'savedir' is not empty.
-            savedir: str, optional. Default: ""
-                If empty, the resulting dataset will
-                not be saved under a csv file. Else,
-                is the path where to save the csv file.
-            to_include: tuple of str, optional. Default: ()
-                Allows to specify what sequences the file paths must
-                contain. All the elements of this tuple must be
-                present in the file path for it to be kept for the
-                final dataset.
-            to_exclude: tuple of str, optional. Default: ()
-                Allows to specify what sequences the file paths must
-                not contain. If the path contains any of the element
-                of this tuple, the file will not be kept for the final
-                dataset.
-            freq_range: tuple of floats of length 2, optional. Default: ()
-                If not empty, only the frequencies between the first
-                element (min frequency) and the second element
-                (max frequency) will be kept, looking at the column
-                "Frequency [Hz]" of the frequency file.
-            verbose: bool, optional. Default: False
-                Whether to display more information in the console
-                during the process or not.
-            separate_samples: bool, optional. Default: False.
-                Whether to give the different samples of a same
-                condition different labels.
-            select_sample: list of str, optional. Default: None
-                If not None, keep only the frequency files that come
-                from the specified samples.
-            sample_parent_degree: int, optional. Default: 1
-                In the path, the parenting degree that is referring
-                to the sample number.
-            target_parent_degree : int, optional. Default: 2
-                In the path, the parenting degree that is referring
-                to the target label.
-            target_keys : dict, optional. Default: {'NI': 'NI', 'INF': 'INF'}
-                The keys refer to how the target is labeled in the file path.
-                The value is how the target will be labeled in the dataset.
-            label_comment: str, optional. Default: ""
-                Any str to add to the labels in the dataset.
-
-        Returns
-        -------
-        out: pd.Dataframe
-            the resulting dataset.
-
-        Example
-        -------
-        >>> import fiiireflyyy.fireprocess as fp
-        >>> mydf = fp.make_dataset_from_freq_files(parent_dir="my/parent/path/here",
-                                             to_include=("freq_50hz_sample", "T=24H"),
-                                             to_exclude=("TTX", "mydrug",),
-                                             verbose=False,
-                                             savedir=False,
-                                             freq_range=(0, 400),
-                                             select_samples=None,
-                                             target_keys={"NI": "not infected", "INF": "infected"},
-                                             separate_samples=False,
-                                             label_comment="")
-
-        will result in a dataset based on all the files containing both "freq_50hz_sample" and "T=24H",
-        and that do contain neither "TTX" nor "mydrug". The dataset will be the result of the smoothing
-        of all frequencies between 0 and 400 Hz, taking account of all the samples. In the path,
-        the 'NI' condition will be labeled as 'not infected' in the dataset, same goes for 'INF' and
-        'infected'. The dataset will not be saved on the system.
-    """
-
-    options = {"filename": "",
-               "to_include": (),
-               "to_exclude": (),
-               "freq_range": (),
-               "savedir": "",
-               "verbose": False,
-               "separate_samples": False,
-               "select_samples": None,
-               "sample_parent_degree": 1,
-               "target_parent_degree": 2,
-               "target_keys": {'NI': 'NI', 'INF': 'INF'},
-               "label_comment": "", }
-    options.update(**kwargs)
-
-    if options["select_samples"] is None:
-        options["select_samples"] = list(
-            set(list(ff.get_all_parent_by_degree(parent_dir, options["sample_parent_degree"]))))
-
-    files = ff.get_all_files(os.path.join(parent_dir))
-    freq_files = []
-    for f in files:
-        if all(i in f for i in options["to_include"]) and (not any(e in f for e in options["to_exclude"])) and \
-                os.path.basename(ff.nth_parent(f, options["sample_parent_degree"])) in options["select_samples"]:
-            freq_files.append(f)
-    if options["verbose"]:
-        print("added: ", freq_files)
-    columns = list(range(0, 300))
-    dataset = pd.DataFrame(columns=columns)
-    target_df = pd.DataFrame(columns=["label", ])
-
-    n_processed_files = 0
-    for f in freq_files:
-        df = pd.read_csv(f)
-        if options["freq_range"]:
-            # selecting the frequencies range
-            df = df.loc[
-                (df["Frequency [Hz]"] >= options["freq_range"][0]) & (df["Frequency [Hz]"] <= options["freq_range"][1])]
-        # smoothing by n values
-        smooth_df = smoothing(df["mean"], 300, 'mean')
-
-        # construct the dataset with n features
-        dataset.loc[len(dataset)] = smooth_df
-
-        path = Path(f)
-
-        for target in options["target_keys"]:
-            if target in os.path.basename(ff.nth_parent(f, options["target_parent_degree"])):
-                if options["separate_samples"]:
-                    target_df.loc[len(target_df)] = options["target_keys"][target] + str(
-                        os.path.basename(path.parent)) + options["label_comment"]
-                else:
-                    target_df.loc[len(target_df)] = options["target_keys"][target] + options["label_comment"]
-
-        if options["verbose"]:
-            progress = int(np.ceil(n_processed_files / len(freq_files) * 100))
-            sys.stdout.write(f"\rProgression of processing files: {progress}%")
-            sys.stdout.flush()
-            n_processed_files += 1
-    dataset["label"] = target_df["label"]
-    if options["verbose"]:
-        print("\n")
-    if options["savedir"]:
-        dataset.to_csv(os.path.join(options["savedir"], options["filename"]), index=False)
-    return dataset
+import os
+import re
+import sys
+
+import pandas as pd
+import numpy as np
+import fiiireflyyy.firefiles as ff
+from pathlib import Path
+import matplotlib.pyplot as plt
+
+
+def floor_ceil_in_range(value, low_thresh: float == 0.0, high_thresh: float == 255.0):
+    """
+    Thresholds a value considering a minimum and maximum value.
+
+        Parameters
+        ----------
+        value: int, float
+            the value to floor or ceil.
+        low_thresh: float, optional, default: 0.0
+            The minimum limit to thresholds the value
+        high_thresh: float, optional, default: 255.0
+            The maximum limit to thresholds the value.
+
+        Returns
+        -------
+        out: int, float
+            The thresholded value.
+    """
+    if value > high_thresh:
+        return high_thresh
+    elif value < low_thresh:
+        return low_thresh
+    else:
+        return value
+
+
+
+
+def merge_all_columns_to_mean(df: pd.DataFrame, except_column=""):
+    """
+    average all the columns, except an optional specified one,
+    in a dataframe into one. The average is done row-wise.
+
+        Parameters
+        ----------
+        df: DataFrame
+            the dataframe to average
+        except_column: str, optional, default: ""
+            the name of the column to exclude from the average.
+            Will be included in the resulting dataset.
+
+        Returns
+        --------
+        out: DataFrame
+            Dataframe containing on column labeled 'mean', and
+            an optional second column based on the
+            except_column parameter
+    """
+
+    excepted_column = pd.DataFrame()
+    if except_column:
+        for col in df.columns:
+            if except_column in col:
+                except_column = col
+        excepted_column = df[except_column]
+        df.drop(except_column, axis=1, inplace=True)
+
+    df_mean = pd.DataFrame(columns=["mean", ])
+    df_mean['mean'] = df.mean(axis=1)
+
+    if except_column != "":
+        for col in df.columns:
+            if except_column in col:
+                except_column = col
+        df_mean[except_column] = excepted_column
+
+    return df_mean
+
+def equal_samples(df, n):
+    """
+    cuts a DataFrame in n sub-DataFrame of same length.
+
+        Parameters
+        ----------
+        df: DataFrame
+            Object to cut, row-wise.
+        n: int
+            number of resulting samples.
+
+        Returns
+        -------
+        out: list of DataFrame
+            contains all the sub DataFrames.
+    """
+    step = int(len(df) / n)
+    lower_limit = 0
+    upper_limit = step
+    samples = []
+    while upper_limit <= len(df):
+        samples.append(df[lower_limit:upper_limit])
+        lower_limit = upper_limit
+        upper_limit += step
+    return samples
+
+def discard_outliers_by_iqr(df: pd.DataFrame, **kwargs):
+    """
+    remove outliers from a dataframe using the interquartile range method.
+
+        Parameters
+        ----------
+        df: pd.Dataframe
+            the dataframe containing the data.
+            Must contain a column 'label'.
+
+        **kwargs: keyword arguments
+            low_percentile : float, default: 0.25
+                the low percentile for IQR outliers removal.
+            high_percentile : float, default: 0.75
+                the high percentile for IQR outliers removal.
+            iqr_limit_factor : float, default: 1.5
+                the factor used to determine when the point is
+                an outlier compared to the percentiles.
+            save: str, default: ""
+                Where to save the resulting plot.
+                If empty, the plot will not be saved.
+                WARNING : may cause randomly 'Key error: 0'.
+            mode: {'capping', }, default: capping
+                The method used to discard the outliers.
+                More to come.
+
+        Returns
+        -------
+        out: pd.Dataframe
+            the dataframe without the outliers
+    """
+    options = {"low_percentile": 0.25,
+               "high_percentile": 0.75,
+               "iqr_limit_factor": 1.5,
+               "save": "",
+               "mode": "capping"}
+    options.update(kwargs)
+    labels = df["label"].unique()
+    labels_values = {}
+    for n in range(len(labels)):
+        labels_values[labels[n]] = n
+
+    features = list(df.columns.values)
+    features.remove('label')
+    metrics = np.empty(shape=(len(labels), len(features)), dtype=object)
+
+    # obtaining the metrics [lower_limit, upper_limit]
+    for i_label in range(len(labels)):
+        label = labels[i_label]
+        sub_df = df.loc[df['label'] == label]
+        for i_feat in range(len(features)):
+            feat = features[i_feat]
+            # finding the iqr
+            low_percentile = sub_df[feat].quantile(options["low_percentile"])
+            high_percentile = sub_df[feat].quantile(options["high_percentile"])
+            iqr = high_percentile - low_percentile
+            # finding upper and lower limit
+            lower_limit = low_percentile - options["iqr_limit_factor"] * iqr
+            upper_limit = high_percentile + options["iqr_limit_factor"] * iqr
+            metrics[i_label][i_feat] = [lower_limit, upper_limit]
+
+    discarded_df = pd.DataFrame(columns=features)
+    discarded_labels = pd.DataFrame(columns=["label", ])
+
+    for i in range(len(df.values)):
+        discarded_row = []
+        discarded_label = df['label'].iloc[i]
+        for j in range(len(df.values[i]) - 1):
+            lower_limit, upper_limit = metrics[labels_values[discarded_label], j]
+            if options["mode"] == "capping":
+                if df.iloc[i, j] > upper_limit:
+                    discarded_row.append(upper_limit)
+                elif df.iloc[i, j] < lower_limit:
+                    discarded_row.append(lower_limit)
+                else:
+                    discarded_row.append(df.iloc[i, j])
+
+        discarded_labels.loc[len(discarded_labels)] = discarded_label
+        discarded_df.loc[len(discarded_df)] = discarded_row
+
+    discarded_df["label"] = discarded_labels["label"]
+    return discarded_df
+
+
+def smoothing(data, n: int, mode='mean'):
+    """
+    Smoothen a signal down to n values, depending on the smoothing mode.
+
+        Parameters
+        ----------
+        data: list of int, list of float
+            contains the numerical data to smoothen.
+        n: int
+            number of points to down sample the data to.
+        mode: str, optional, default: 'mean'
+            the way to smoothen the data between the points.
+
+        Returns
+        -------
+        out: list of floats
+            the smoothened data.
+
+    """
+    if len(data.index) > n:
+        step = int(len(data.index) / n)
+        lower_limit = 0
+        upper_limit = step
+        ds_data = []
+        if mode == 'mean':
+            while upper_limit <= len(data):
+                ds_data.append(np.mean(data[lower_limit:upper_limit]).round(3))
+                lower_limit = upper_limit
+                upper_limit += step
+        excedent = len(ds_data) - n
+        ds_data = ds_data[:-excedent or None]
+        return ds_data
+    else:
+        raise Exception("smoothing: length of data " + str(len(data.index)) + "< n " + str(n))
+
+
+def make_dataset_from_freq_files(parent_dir, **kwargs):
+    """
+    Use frequency files of format two columns (one column 'Frequencies [Hz]' and one column 'mean') to generate a
+    dataset used for classification. Specialized for recording of electrical signal. The path tree has to be
+    organised as such :
+    base/condition (ej. drug addition)/recording time/target for classification (ej. infected/not
+    infected)/sample number/my_freq_files.csv .
+
+        Parameters
+        ----------
+        parent_dir: str.
+            the parent directory where to look for all the
+            frequency files.
+
+        **kwargs: keyword arguments
+            filename: str, optional. Default: ""
+                the name of the resulting csv file if
+                'savedir' is not empty.
+            savedir: str, optional. Default: ""
+                If empty, the resulting dataset will
+                not be saved under a csv file. Else,
+                is the path where to save the csv file.
+            to_include: tuple of str, optional. Default: ()
+                Allows to specify what sequences the file paths must
+                contain. All the elements of this tuple must be
+                present in the file path for it to be kept for the
+                final dataset.
+            to_exclude: tuple of str, optional. Default: ()
+                Allows to specify what sequences the file paths must
+                not contain. If the path contains any of the element
+                of this tuple, the file will not be kept for the final
+                dataset.
+            freq_range: tuple of floats of length 2, optional. Default: ()
+                If not empty, only the frequencies between the first
+                element (min frequency) and the second element
+                (max frequency) will be kept, looking at the column
+                "Frequency [Hz]" of the frequency file.
+            verbose: bool, optional. Default: False
+                Whether to display more information in the console
+                during the process or not.
+            separate_samples: bool, optional. Default: False.
+                Whether to give the different samples of a same
+                condition different labels.
+            select_sample: list of str, optional. Default: None
+                If not None, keep only the frequency files that come
+                from the specified samples.
+            sample_parent_degree: int, optional. Default: 1
+                In the path, the parenting degree that is referring
+                to the sample number.
+            target_parent_degree : int, optional. Default: 2
+                In the path, the parenting degree that is referring
+                to the target label.
+            target_keys : dict, optional. Default: {'NI': 'NI', 'INF': 'INF'}
+                The keys refer to how the target is labeled in the file path.
+                The value is how the target will be labeled in the dataset.
+            label_comment: str, optional. Default: ""
+                Any str to add to the labels in the dataset.
+
+        Returns
+        -------
+        out: pd.Dataframe
+            the resulting dataset.
+
+        Example
+        -------
+        >>> import fiiireflyyy.fireprocess as fp
+        >>> mydf = fp.make_dataset_from_freq_files(parent_dir="my/parent/path/here",
+                                             to_include=("freq_50hz_sample", "T=24H"),
+                                             to_exclude=("TTX", "mydrug",),
+                                             verbose=False,
+                                             savedir=False,
+                                             freq_range=(0, 400),
+                                             select_samples=None,
+                                             target_keys={"NI": "not infected", "INF": "infected"},
+                                             separate_samples=False,
+                                             label_comment="")
+
+        will result in a dataset based on all the files containing both "freq_50hz_sample" and "T=24H",
+        and that do contain neither "TTX" nor "mydrug". The dataset will be the result of the smoothing
+        of all frequencies between 0 and 400 Hz, taking account of all the samples. In the path,
+        the 'NI' condition will be labeled as 'not infected' in the dataset, same goes for 'INF' and
+        'infected'. The dataset will not be saved on the system.
+    """
+
+    options = {"filename": "",
+               "to_include": (),
+               "to_exclude": (),
+               "freq_range": (),
+               "savedir": "",
+               "verbose": False,
+               "separate_samples": False,
+               "select_samples": None,
+               "sample_parent_degree": 1,
+               "target_parent_degree": 2,
+               "target_keys": {'NI': 'NI', 'INF': 'INF'},
+               "label_comment": "", }
+    options.update(**kwargs)
+
+    if options["select_samples"] is None:
+        options["select_samples"] = list(
+            set(list(ff.get_all_parent_by_degree(parent_dir, options["sample_parent_degree"]))))
+
+    files = ff.get_all_files(os.path.join(parent_dir))
+    freq_files = []
+    for f in files:
+        if all(i in f for i in options["to_include"]) and (not any(e in f for e in options["to_exclude"])) and \
+                os.path.basename(ff.nth_parent(f, options["sample_parent_degree"])) in options["select_samples"]:
+            freq_files.append(f)
+    if options["verbose"]:
+        print("added: ", freq_files)
+    columns = list(range(0, 300))
+    dataset = pd.DataFrame(columns=columns)
+    target_df = pd.DataFrame(columns=["label", ])
+
+    n_processed_files = 0
+    for f in freq_files:
+        df = pd.read_csv(f)
+        if options["freq_range"]:
+            # selecting the frequencies range
+            df = df.loc[
+                (df["Frequency [Hz]"] >= options["freq_range"][0]) & (df["Frequency [Hz]"] <= options["freq_range"][1])]
+        # smoothing by n values
+        smooth_df = smoothing(df["mean"], 300, 'mean')
+
+        # construct the dataset with n features
+        dataset.loc[len(dataset)] = smooth_df
+
+        path = Path(f)
+
+        for target in options["target_keys"]:
+            if target in os.path.basename(ff.nth_parent(f, options["target_parent_degree"])):
+                if options["separate_samples"]:
+                    target_df.loc[len(target_df)] = options["target_keys"][target] + str(
+                        os.path.basename(path.parent)) + options["label_comment"]
+                else:
+                    target_df.loc[len(target_df)] = options["target_keys"][target] + options["label_comment"]
+
+        if options["verbose"]:
+            progress = int(np.ceil(n_processed_files / len(freq_files) * 100))
+            sys.stdout.write(f"\rProgression of processing files: {progress}%")
+            sys.stdout.flush()
+            n_processed_files += 1
+    dataset["label"] = target_df["label"]
+    if options["verbose"]:
+        print("\n")
+    if options["savedir"]:
+        dataset.to_csv(os.path.join(options["savedir"], options["filename"]), index=False)
+    return dataset
```

### Comparing `fiiireflyyy-0.1.1/fiiireflyyy/flimage.py` & `fiiireflyyy-0.1.2/fiiireflyyy/flimage.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,442 +1,442 @@
-import cv2
-import numpy as np
-import os
-import fiiireflyyy.firefiles as ff
-import fiiireflyyy.fireprocess as fp
-
-from imaris_ims_file_reader.ims import ims
-import zarr
-from PIL import Image
-
-
-def get_value_region_proportion_per_picture(arr, value=0):
-    """
-    Return the percentage that represents a certain pixel value
-    in a gray scaled image. The image is processed beforehand
-    to reduce the background noise
-
-    Parameters
-    ----------
-        arr: ndarray, shape(n, n)
-            the image
-        value: int, default: 0
-            the value to look for in the picture.
-
-    Returns
-    -------
-        out: tuple of length 2.
-            The first element is the int representing the percentage
-            that the initial value represents in the image.
-            The second element is the resulting image after
-            processing.
-    """
-    edges = cv2.Canny(image=arr, threshold1=50, threshold2=100)
-    edges = convolution_edge_spreading(edges)
-    edges = cv2.GaussianBlur(edges, (3, 3), cv2.BORDER_DEFAULT)
-    edges = convolution_edge_spreading(edges)
-    value_percent = int(np.ceil((np.count_nonzero(edges == value) / (edges.shape[0] * edges.shape[1])) * 100))
-    return value_percent, edges
-
-
-
-
-def convolution_edge_spreading(arr, kernel=None):
-    """
-     Spread the pixels by using a convolution. Used preferentially
-     to spread the edges of an edge-detection resulting image.
-
-        Parameters
-        ----------
-        arr: ndarray, shape(n, n)
-            The picture to operate on.
-        kernel: list of list, shape(n, n), optional. Default : [[0, 1, 0], [1, 1, 1], [0, 1, 0]]
-            A cross-shaped filter used to spread the pixels.
-
-        Returns
-        -------
-        out: ndarray, shape(n, n)
-            the spread-edges image.
-    """
-    if kernel is None:
-        kernel = [[0, 1, 0],
-                  [1, 1, 1],
-                  [0, 1, 0]]
-    n = arr.shape[0]  # original image size
-    s = 1  # stride
-    f = len(kernel)
-    p = int((f - 1) / 2)  # valid padding
-    arr = np.pad(arr, pad_width=p)
-    conv_size = int(np.floor((n + 2 * p - f / s) + 1))
-    conv_arr = np.empty(shape=(conv_size, conv_size), )
-    for i in range(0, conv_size, s):
-        for j in range(0, conv_size, s):
-            convolution = 0
-            for fi in range(f):
-                for fj in range(f):
-                    convolution += arr[i + fi, j + fj] * kernel[fi][fj]
-            convolution = fp.floor_ceil_in_range(convolution, 0, 255)
-            conv_arr[i, j] = int(convolution)
-
-    return np.uint8(conv_arr)
-
-
-def grayscale(imarr, mode="high_thresh"):
-    """
-        transforms an array of an image into its
-        grayscale conversion.
-
-        Parameters
-        ----------
-        imarr : ndarray
-            the array of shape (n, n, 3)
-        mode : {'high_thresh', 'avg'}, default: 'avg'
-            conversion mode for grayscale conversion.
-            'high_thresh' is setting the maximum value in between
-            the channels of a pixel as the new value for
-            the 3 channels.
-            'avg' is using the mean of the 3 channels as
-            the new pixel value.
-
-        Returns
-        -------
-        out: ndarray, shape(n, n, 3)
-            The gray scaled array.
-    """
-    for i in range(len(imarr)):
-        for j in range(len(imarr[i])):
-            if mode == "avg":
-                imarr[i][j] = np.array([np.mean(imarr[i][j])] * 3)
-            if mode == "high_thresh":
-                imarr[i][j] = np.array([np.max(imarr[i][j])] * 3)
-    return imarr
-
-
-
-def scale_range(value, min_measurement, max_measurement, min_target=0,
-                max_target=255):
-    """
-    scale measurement value given an interval.
-
-        Parameters
-        ----------
-        value : int, float
-            The value to scale
-        min_measurement : int, float
-            The minimal measured value of the sample to scale.
-        max_measurement : int, float
-            The maximal measured value of the sample to scale.
-        min_target : int, float, optional, default : 0
-            The lower limit of the interval used for scaling.
-        max_target : int, float, optional, default : 255
-            The upper limit of the interval used for scaling.
-
-        Returns
-        -------
-        out : int, float
-            The scaled value
-    """
-    scaled_value = (value - min_measurement) / (max_measurement - min_measurement) * (
-            max_target - min_target) + min_target
-    return scaled_value
-
-
-def combine(images, z_mode='firstlayer'):
-    """
-    combine multiple images of the same size as one.
-
-        Parameters
-        ----------
-        images : list of PIL Image instances
-
-        z_mode : {'firstlayer', 'midlayer', 'endlayer', 'max', 'average'}, optional, default : 'firstlayer'
-            How to process the z dimension of the ims file.
-            'firstlayer', 'midlayer' and 'endlayer' will process only the first, middle or last z layer respectively.
-            'max' takes account of all z layers. Per channel and per pixel, select the highest value among all the z.
-            'average' takes account of all z layers. Per channel and per pixel, make the average among all the z.
-
-        Returns
-        -------
-        out : a Pillow Image instance
-
-    """
-    h, w = images[0].size
-    merged_array = np.zeros((h, w, 3), dtype=np.uint8)
-    converted_image = Image.fromarray(merged_array, 'RGB')
-
-    if z_mode == 'midlayer':
-        mid_idx = int(len(images) / 2)
-        converted_image = images[mid_idx]
-
-    elif z_mode == 'firstlayer':
-        converted_image = images[0]
-
-    elif z_mode == 'endlayer':
-        converted_image = images[len(images)]
-
-    elif z_mode == 'max':
-        for img_idx in range(len(images)):
-            img = images[img_idx]
-            # noinspection PyTypeChecker
-            img_matrix = np.asarray(img)
-            for y in range(h):
-                for x in range(w):
-                    r, g, b = img_matrix[x, y]
-                    new_r = max(merged_array[x, y][0], r)
-                    new_g = max(merged_array[x, y][1], g)
-                    new_b = max(merged_array[x, y][2], b)
-                    merged_array[x, y] = [new_r, new_g, new_b]
-        converted_image = Image.fromarray(merged_array, 'RGB')
-
-    elif z_mode == 'average':
-        for y in range(h):
-            for x in range(w):
-                r_values = []
-                g_values = []
-                b_values = []
-                for img_idx in range(len(images)):
-                    # noinspection PyTypeChecker
-                    img_matrix = np.asarray(images[img_idx])
-                    r, g, b = img_matrix[x, y]
-                    r_values.append(r)
-                    g_values.append(g)
-                    b_values.append(b)
-                merged_array[x, y] = [int(np.mean(r_values)), int(np.mean(g_values)), int(np.mean(b_values))]
-        converted_image = Image.fromarray(merged_array, 'RGB')
-
-    return converted_image
-
-
-def ims_to_2D_image(ims_path, **kwargs):
-    """
-    convert an .ims file picture (Imaris) into a .png file.
-
-        Parameters
-        ----------
-        ims_path : str
-            complete path where the file to convert is stored
-        
-        **kwargs: keywords arguments
-            mode : str, optional, default : 'RGB'
-                made of the combination of 'R' 'G' and 'B' corresponding to the red green and blue channels of the
-                image respectively. Any channel present will be processed in the resulting png file. The channels
-                not represented will have pixels values at 0.
-    
-            z_mode : {'firstlayer', 'midlayer', 'endlayer', 'max', 'average'}, optional, default : 'firstlayer'
-                How to process the z dimension of the ims file.
-                'firstlayer', 'midlayer' and 'endlayer' will process only the first, middle or last z layer respectively.
-                'max' takes account of all z layers. Per channel and per pixel, select the highest value among all the z.
-                'average' takes account of all z layers. Per channel and per pixel, make the average among all the z.
-    
-            minmax_scaling : {'auto', } or tuple of ints, optional, default : 'auto'
-                Used to scale the intensity values in the ims file between target values 0 and 255.
-                if 'auto' takes the minimum and maximum measurement values as the min and max intensity in each channel.
-                if (int, int), the first value is the min measurement value and the second is the max.
-    
-            save : str, optional, default : ''
-                path where the resulting image is saved as a png, or other format. You need to precise the extension.
-    
-            show : bool, optional, default : False
-                if True, display the resulting png image in a window.
-
-        Returns
-        -------
-        out : a Pillow Image
-    """
-    options = {"mode": 'RGB', "z_mode": "firstlayer", "minmax_scaling": 'auto', "show": False,
-               "save": ""}
-    options.update(**kwargs)
-    # Get the channels to process
-    channels_state = {'R': 0, 'G': 1, 'B': 2}
-
-    store = ims(ims_path, ResolutionLevelLock=2, aszarr=True)
-    zarray = zarr.open(store, mode='r')
-    w = zarray.shape[-2]
-    h = zarray.shape[-1]
-    max_depth = 1
-    if options["z_mode"] not in ("firstlayer", "midlayer", 'endlayer'):
-        max_depth = zarray.shape[-3]
-
-    # ------------- SELECTING THE CHANNELS TO PROCESS --------------------
-    channels_to_process = []
-    for channel in channels_state:
-        if channel in options["mode"]:
-            channels_to_process.append(channel)
-
-    all_depths_pictures = []
-    for z in range(max_depth):  # parsing all depths
-        fused_data = np.zeros((h, w, 3), dtype=np.uint8)
-        for channel in channels_to_process:  # processing all color channels
-
-            # --------------------------- SCALING PREPARATION ---------------------------------
-            min_intensity = 0
-            max_intensity = 0
-
-            single_channel_picture = zarray[0, channels_state[channel], z]
-
-            if isinstance(options["minmax_scaling"], str):
-                if options["minmax_scaling"] == 'auto':
-                    min_intensity = single_channel_picture[0][0]
-                    max_intensity = single_channel_picture[0][0]
-                    for x in range(w):
-                        for y in range(h):
-                            if single_channel_picture[x][y] > max_intensity:
-                                max_intensity = single_channel_picture[x][y]
-                            if single_channel_picture[x][y] < min_intensity:
-                                min_intensity = single_channel_picture[x][y]
-
-            elif isinstance(options["minmax_scaling"], type((0, 0))):
-                min_intensity = options["minmax_scaling"][0]
-                max_intensity = options["minmax_scaling"][1]
-
-            # ------------------------- RECONSTRUCTING THE IMAGE ------------------------
-            for y in range(h):
-                for x in range(w):
-                    value = single_channel_picture[x][y]
-                    scaled_value = scale_range(value, min_intensity, max_intensity)
-
-                    if channel == 'R':
-                        fused_data[x][y] = [scaled_value, fused_data[x][y][1], fused_data[x][y][2]]
-                    if channel == 'G':
-                        fused_data[x][y] = [fused_data[x][y][0], scaled_value, fused_data[x][y][2]]
-                    if channel == 'B':
-                        fused_data[x][y] = [fused_data[x][y][0], fused_data[x][y][1], scaled_value]
-        img = Image.fromarray(fused_data, 'RGB')
-        all_depths_pictures.append(img)
-
-    converted_image = combine(all_depths_pictures, z_mode=options["z_mode"])
-    if options["show"]:
-        converted_image.show()
-    if options["save"]:
-        converted_image.save(options["save"])
-    return converted_image
-
-
-def show_image(title, image):
-    """
-    Show an image and wait for interaction before closing
-
-        Parameters
-        ----------
-        title: str
-            Title of the picture's windows.
-        image: cv2 object
-            The picture to show.
-    """
-    cv2.imshow(title, image)
-    cv2.waitKey(0)
-
-
-def rotate_image(image, angle):
-    """
-    Rotate a picture
-
-        Parameters
-        ----------
-        image: cv2 Object
-            The picture to rotate
-        angle: float
-            Rotation angle
-
-        Returns
-        -------
-        out: cv2 Object
-            Rotated picture
-    """
-    image_center = tuple(np.array(image.shape[1::-1]) / 2)
-    rot_mat = cv2.getRotationMatrix2D(image_center, angle, 1.0)
-    result = cv2.warpAffine(image, rot_mat, image.shape[1::-1], flags=cv2.INTER_LINEAR)
-    return result
-
-
-def flip_image(image, orientation):
-    """
-    Flip a picture
-
-        Parameters
-        ----------
-        image: cv2 Object
-            The picture to flip
-        orientation: {'x', 'y', 'xy'}
-            The axis upon which to flip the picture. Take values "x", "y", "xy".
-
-        Returns
-        -------
-        out: cv2 object
-            the flipped image
-        """
-    if orientation.lower() == "x":
-        flip = cv2.flip(image, 0)
-        return flip
-    elif orientation.lower() == "y":
-        flip = cv2.flip(image, 1)
-        return flip
-    elif orientation.lower() == "xy":
-        flip = cv2.flip(image, -1)
-        return flip
-
-
-def save_image(path, image):
-    """
-    Save an image on the system.
-
-        Parameters
-        ----------
-        path: str
-            Where to save the picture
-        image: cv2 object
-            The picture to save.
-
-    """
-    head, tail = os.path.split(path)
-    isExist = os.path.exists(head)
-    if isExist:
-        cv2.imwrite(path, image)
-    else:
-        os.mkdir(head)
-        cv2.imwrite(path, image)
-
-
-def slice_images(source, destination, slice_size):
-    """
-    Slice all images in the source directory in multiple square sized images and save them in destination. The image
-    must be square sized.
-
-        Parameters
-        ----------
-        source: str
-            directory where all images to slice are.
-        destination: str
-            where the sliced images will be saved.
-        slice_size: int
-            the square size of the sliced image.
-    """
-
-    images_paths = ff.get_all_files(source)
-    img = cv2.imread(images_paths[0])
-    img_size = img.shape[1]
-
-    if img.shape[0] != img.shape[1]:
-        raise ValueError(f"The image is not square sized: width:{img.shape[1]} != height:{img.shape[0]}")
-    if img_size < slice_size:
-        raise ValueError(f"Slicing size superior to image size: {slice_size} > {img_size}")
-
-    for path in images_paths:
-        slice_number = 1
-        for x in range(0, img_size, slice_size):
-            x1 = x
-            x2 = x + slice_size
-
-            for y in range(0, img_size, slice_size):
-                y1 = y
-                y2 = y + slice_size
-
-                img = cv2.imread(path)
-                sliced_img = img[y1:y2, x1:x2]
-
-                title = destination + os.path.basename(path).split(".")[0] + "_sliced_" + str(slice_number) + ".png"
-
-                ff.verify_dir(destination)
-
-                cv2.imwrite(title, sliced_img)
-
-                slice_number += 1
+import cv2
+import numpy as np
+import os
+import fiiireflyyy.firefiles as ff
+import fiiireflyyy.fireprocess as fp
+
+from imaris_ims_file_reader.ims import ims
+import zarr
+from PIL import Image
+
+
+def get_value_region_proportion_per_picture(arr, value=0):
+    """
+    Return the percentage that represents a certain pixel value
+    in a gray scaled image. The image is processed beforehand
+    to reduce the background noise
+
+    Parameters
+    ----------
+        arr: ndarray, shape(n, n)
+            the image
+        value: int, default: 0
+            the value to look for in the picture.
+
+    Returns
+    -------
+        out: tuple of length 2.
+            The first element is the int representing the percentage
+            that the initial value represents in the image.
+            The second element is the resulting image after
+            processing.
+    """
+    edges = cv2.Canny(image=arr, threshold1=50, threshold2=100)
+    edges = convolution_edge_spreading(edges)
+    edges = cv2.GaussianBlur(edges, (3, 3), cv2.BORDER_DEFAULT)
+    edges = convolution_edge_spreading(edges)
+    value_percent = int(np.ceil((np.count_nonzero(edges == value) / (edges.shape[0] * edges.shape[1])) * 100))
+    return value_percent, edges
+
+
+
+
+def convolution_edge_spreading(arr, kernel=None):
+    """
+     Spread the pixels by using a convolution. Used preferentially
+     to spread the edges of an edge-detection resulting image.
+
+        Parameters
+        ----------
+        arr: ndarray, shape(n, n)
+            The picture to operate on.
+        kernel: list of list, shape(n, n), optional. Default : [[0, 1, 0], [1, 1, 1], [0, 1, 0]]
+            A cross-shaped filter used to spread the pixels.
+
+        Returns
+        -------
+        out: ndarray, shape(n, n)
+            the spread-edges image.
+    """
+    if kernel is None:
+        kernel = [[0, 1, 0],
+                  [1, 1, 1],
+                  [0, 1, 0]]
+    n = arr.shape[0]  # original image size
+    s = 1  # stride
+    f = len(kernel)
+    p = int((f - 1) / 2)  # valid padding
+    arr = np.pad(arr, pad_width=p)
+    conv_size = int(np.floor((n + 2 * p - f / s) + 1))
+    conv_arr = np.empty(shape=(conv_size, conv_size), )
+    for i in range(0, conv_size, s):
+        for j in range(0, conv_size, s):
+            convolution = 0
+            for fi in range(f):
+                for fj in range(f):
+                    convolution += arr[i + fi, j + fj] * kernel[fi][fj]
+            convolution = fp.floor_ceil_in_range(convolution, 0, 255)
+            conv_arr[i, j] = int(convolution)
+
+    return np.uint8(conv_arr)
+
+
+def grayscale(imarr, mode="high_thresh"):
+    """
+        transforms an array of an image into its
+        grayscale conversion.
+
+        Parameters
+        ----------
+        imarr : ndarray
+            the array of shape (n, n, 3)
+        mode : {'high_thresh', 'avg'}, default: 'avg'
+            conversion mode for grayscale conversion.
+            'high_thresh' is setting the maximum value in between
+            the channels of a pixel as the new value for
+            the 3 channels.
+            'avg' is using the mean of the 3 channels as
+            the new pixel value.
+
+        Returns
+        -------
+        out: ndarray, shape(n, n, 3)
+            The gray scaled array.
+    """
+    for i in range(len(imarr)):
+        for j in range(len(imarr[i])):
+            if mode == "avg":
+                imarr[i][j] = np.array([np.mean(imarr[i][j])] * 3)
+            if mode == "high_thresh":
+                imarr[i][j] = np.array([np.max(imarr[i][j])] * 3)
+    return imarr
+
+
+
+def scale_range(value, min_measurement, max_measurement, min_target=0,
+                max_target=255):
+    """
+    scale measurement value given an interval.
+
+        Parameters
+        ----------
+        value : int, float
+            The value to scale
+        min_measurement : int, float
+            The minimal measured value of the sample to scale.
+        max_measurement : int, float
+            The maximal measured value of the sample to scale.
+        min_target : int, float, optional, default : 0
+            The lower limit of the interval used for scaling.
+        max_target : int, float, optional, default : 255
+            The upper limit of the interval used for scaling.
+
+        Returns
+        -------
+        out : int, float
+            The scaled value
+    """
+    scaled_value = (value - min_measurement) / (max_measurement - min_measurement) * (
+            max_target - min_target) + min_target
+    return scaled_value
+
+
+def combine(images, z_mode='firstlayer'):
+    """
+    combine multiple images of the same size as one.
+
+        Parameters
+        ----------
+        images : list of PIL Image instances
+
+        z_mode : {'firstlayer', 'midlayer', 'endlayer', 'max', 'average'}, optional, default : 'firstlayer'
+            How to process the z dimension of the ims file.
+            'firstlayer', 'midlayer' and 'endlayer' will process only the first, middle or last z layer respectively.
+            'max' takes account of all z layers. Per channel and per pixel, select the highest value among all the z.
+            'average' takes account of all z layers. Per channel and per pixel, make the average among all the z.
+
+        Returns
+        -------
+        out : a Pillow Image instance
+
+    """
+    h, w = images[0].size
+    merged_array = np.zeros((h, w, 3), dtype=np.uint8)
+    converted_image = Image.fromarray(merged_array, 'RGB')
+
+    if z_mode == 'midlayer':
+        mid_idx = int(len(images) / 2)
+        converted_image = images[mid_idx]
+
+    elif z_mode == 'firstlayer':
+        converted_image = images[0]
+
+    elif z_mode == 'endlayer':
+        converted_image = images[len(images)]
+
+    elif z_mode == 'max':
+        for img_idx in range(len(images)):
+            img = images[img_idx]
+            # noinspection PyTypeChecker
+            img_matrix = np.asarray(img)
+            for y in range(h):
+                for x in range(w):
+                    r, g, b = img_matrix[x, y]
+                    new_r = max(merged_array[x, y][0], r)
+                    new_g = max(merged_array[x, y][1], g)
+                    new_b = max(merged_array[x, y][2], b)
+                    merged_array[x, y] = [new_r, new_g, new_b]
+        converted_image = Image.fromarray(merged_array, 'RGB')
+
+    elif z_mode == 'average':
+        for y in range(h):
+            for x in range(w):
+                r_values = []
+                g_values = []
+                b_values = []
+                for img_idx in range(len(images)):
+                    # noinspection PyTypeChecker
+                    img_matrix = np.asarray(images[img_idx])
+                    r, g, b = img_matrix[x, y]
+                    r_values.append(r)
+                    g_values.append(g)
+                    b_values.append(b)
+                merged_array[x, y] = [int(np.mean(r_values)), int(np.mean(g_values)), int(np.mean(b_values))]
+        converted_image = Image.fromarray(merged_array, 'RGB')
+
+    return converted_image
+
+
+def ims_to_2D_image(ims_path, **kwargs):
+    """
+    convert an .ims file picture (Imaris) into a .png file.
+
+        Parameters
+        ----------
+        ims_path : str
+            complete path where the file to convert is stored
+        
+        **kwargs: keywords arguments
+            mode : str, optional, default : 'RGB'
+                made of the combination of 'R' 'G' and 'B' corresponding to the red green and blue channels of the
+                image respectively. Any channel present will be processed in the resulting png file. The channels
+                not represented will have pixels values at 0.
+    
+            z_mode : {'firstlayer', 'midlayer', 'endlayer', 'max', 'average'}, optional, default : 'firstlayer'
+                How to process the z dimension of the ims file.
+                'firstlayer', 'midlayer' and 'endlayer' will process only the first, middle or last z layer respectively.
+                'max' takes account of all z layers. Per channel and per pixel, select the highest value among all the z.
+                'average' takes account of all z layers. Per channel and per pixel, make the average among all the z.
+    
+            minmax_scaling : {'auto', } or tuple of ints, optional, default : 'auto'
+                Used to scale the intensity values in the ims file between target values 0 and 255.
+                if 'auto' takes the minimum and maximum measurement values as the min and max intensity in each channel.
+                if (int, int), the first value is the min measurement value and the second is the max.
+    
+            save : str, optional, default : ''
+                path where the resulting image is saved as a png, or other format. You need to precise the extension.
+    
+            show : bool, optional, default : False
+                if True, display the resulting png image in a window.
+
+        Returns
+        -------
+        out : a Pillow Image
+    """
+    options = {"mode": 'RGB', "z_mode": "firstlayer", "minmax_scaling": 'auto', "show": False,
+               "save": ""}
+    options.update(**kwargs)
+    # Get the channels to process
+    channels_state = {'R': 0, 'G': 1, 'B': 2}
+
+    store = ims(ims_path, ResolutionLevelLock=2, aszarr=True)
+    zarray = zarr.open(store, mode='r')
+    w = zarray.shape[-2]
+    h = zarray.shape[-1]
+    max_depth = 1
+    if options["z_mode"] not in ("firstlayer", "midlayer", 'endlayer'):
+        max_depth = zarray.shape[-3]
+
+    # ------------- SELECTING THE CHANNELS TO PROCESS --------------------
+    channels_to_process = []
+    for channel in channels_state:
+        if channel in options["mode"]:
+            channels_to_process.append(channel)
+
+    all_depths_pictures = []
+    for z in range(max_depth):  # parsing all depths
+        fused_data = np.zeros((h, w, 3), dtype=np.uint8)
+        for channel in channels_to_process:  # processing all color channels
+
+            # --------------------------- SCALING PREPARATION ---------------------------------
+            min_intensity = 0
+            max_intensity = 0
+
+            single_channel_picture = zarray[0, channels_state[channel], z]
+
+            if isinstance(options["minmax_scaling"], str):
+                if options["minmax_scaling"] == 'auto':
+                    min_intensity = single_channel_picture[0][0]
+                    max_intensity = single_channel_picture[0][0]
+                    for x in range(w):
+                        for y in range(h):
+                            if single_channel_picture[x][y] > max_intensity:
+                                max_intensity = single_channel_picture[x][y]
+                            if single_channel_picture[x][y] < min_intensity:
+                                min_intensity = single_channel_picture[x][y]
+
+            elif isinstance(options["minmax_scaling"], type((0, 0))):
+                min_intensity = options["minmax_scaling"][0]
+                max_intensity = options["minmax_scaling"][1]
+
+            # ------------------------- RECONSTRUCTING THE IMAGE ------------------------
+            for y in range(h):
+                for x in range(w):
+                    value = single_channel_picture[x][y]
+                    scaled_value = scale_range(value, min_intensity, max_intensity)
+
+                    if channel == 'R':
+                        fused_data[x][y] = [scaled_value, fused_data[x][y][1], fused_data[x][y][2]]
+                    if channel == 'G':
+                        fused_data[x][y] = [fused_data[x][y][0], scaled_value, fused_data[x][y][2]]
+                    if channel == 'B':
+                        fused_data[x][y] = [fused_data[x][y][0], fused_data[x][y][1], scaled_value]
+        img = Image.fromarray(fused_data, 'RGB')
+        all_depths_pictures.append(img)
+
+    converted_image = combine(all_depths_pictures, z_mode=options["z_mode"])
+    if options["show"]:
+        converted_image.show()
+    if options["save"]:
+        converted_image.save(options["save"])
+    return converted_image
+
+
+def show_image(title, image):
+    """
+    Show an image and wait for interaction before closing
+
+        Parameters
+        ----------
+        title: str
+            Title of the picture's windows.
+        image: cv2 object
+            The picture to show.
+    """
+    cv2.imshow(title, image)
+    cv2.waitKey(0)
+
+
+def rotate_image(image, angle):
+    """
+    Rotate a picture
+
+        Parameters
+        ----------
+        image: cv2 Object
+            The picture to rotate
+        angle: float
+            Rotation angle
+
+        Returns
+        -------
+        out: cv2 Object
+            Rotated picture
+    """
+    image_center = tuple(np.array(image.shape[1::-1]) / 2)
+    rot_mat = cv2.getRotationMatrix2D(image_center, angle, 1.0)
+    result = cv2.warpAffine(image, rot_mat, image.shape[1::-1], flags=cv2.INTER_LINEAR)
+    return result
+
+
+def flip_image(image, orientation):
+    """
+    Flip a picture
+
+        Parameters
+        ----------
+        image: cv2 Object
+            The picture to flip
+        orientation: {'x', 'y', 'xy'}
+            The axis upon which to flip the picture. Take values "x", "y", "xy".
+
+        Returns
+        -------
+        out: cv2 object
+            the flipped image
+        """
+    if orientation.lower() == "x":
+        flip = cv2.flip(image, 0)
+        return flip
+    elif orientation.lower() == "y":
+        flip = cv2.flip(image, 1)
+        return flip
+    elif orientation.lower() == "xy":
+        flip = cv2.flip(image, -1)
+        return flip
+
+
+def save_image(path, image):
+    """
+    Save an image on the system.
+
+        Parameters
+        ----------
+        path: str
+            Where to save the picture
+        image: cv2 object
+            The picture to save.
+
+    """
+    head, tail = os.path.split(path)
+    isExist = os.path.exists(head)
+    if isExist:
+        cv2.imwrite(path, image)
+    else:
+        os.mkdir(head)
+        cv2.imwrite(path, image)
+
+
+def slice_images(source, destination, slice_size):
+    """
+    Slice all images in the source directory in multiple square sized images and save them in destination. The image
+    must be square sized.
+
+        Parameters
+        ----------
+        source: str
+            directory where all images to slice are.
+        destination: str
+            where the sliced images will be saved.
+        slice_size: int
+            the square size of the sliced image.
+    """
+
+    images_paths = ff.get_all_files(source)
+    img = cv2.imread(images_paths[0])
+    img_size = img.shape[1]
+
+    if img.shape[0] != img.shape[1]:
+        raise ValueError(f"The image is not square sized: width:{img.shape[1]} != height:{img.shape[0]}")
+    if img_size < slice_size:
+        raise ValueError(f"Slicing size superior to image size: {slice_size} > {img_size}")
+
+    for path in images_paths:
+        slice_number = 1
+        for x in range(0, img_size, slice_size):
+            x1 = x
+            x2 = x + slice_size
+
+            for y in range(0, img_size, slice_size):
+                y1 = y
+                y2 = y + slice_size
+
+                img = cv2.imread(path)
+                sliced_img = img[y1:y2, x1:x2]
+
+                title = destination + os.path.basename(path).split(".")[0] + "_sliced_" + str(slice_number) + ".png"
+
+                ff.verify_dir(destination)
+
+                cv2.imwrite(title, sliced_img)
+
+                slice_number += 1
```

### Comparing `fiiireflyyy-0.1.1/setup.py` & `fiiireflyyy-0.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.1.1'
+VERSION = '0.1.2'
 DESCRIPTION = 'A python package covering miscellaneous uses, from system management to machine learning and image or' \
               ' data processing. Developed for personal uses.'
 
 # Setting up
 setup(
     name="fiiireflyyy",
     version=VERSION,
```

