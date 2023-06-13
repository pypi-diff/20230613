# Comparing `tmp/custom_diffusion-0.1.3.tar.gz` & `tmp/custom_diffusion-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custom_diffusion-0.1.3.tar", last modified: Mon Jun 12 11:16:19 2023, max compression
+gzip compressed data, was "custom_diffusion-0.1.5.tar", last modified: Tue Jun 13 10:47:42 2023, max compression
```

## Comparing `custom_diffusion-0.1.3.tar` & `custom_diffusion-0.1.5.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 11:16:19.735103 custom_diffusion-0.1.3/
--rw-rw-rw-   0        0        0    11558 2023-06-07 17:52:13.000000 custom_diffusion-0.1.3/LICENSE
--rw-rw-rw-   0        0        0       24 2023-06-09 11:29:48.000000 custom_diffusion-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2595 2023-06-12 11:16:19.735103 custom_diffusion-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1451 2023-06-11 10:55:21.000000 custom_diffusion-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 11:16:19.676183 custom_diffusion-0.1.3/custom_diffusion/
--rw-rw-rw-   0        0        0      230 2023-06-12 11:15:32.000000 custom_diffusion-0.1.3/custom_diffusion/__init__.py
--rw-rw-rw-   0        0        0     2740 2023-06-12 11:16:06.000000 custom_diffusion-0.1.3/custom_diffusion/demo.py
-drwxrwxrwx   0        0        0        0 2023-06-12 11:16:19.721035 custom_diffusion-0.1.3/custom_diffusion/pipelines/
--rw-rw-rw-   0        0        0        0 2023-06-11 10:55:21.000000 custom_diffusion-0.1.3/custom_diffusion/pipelines/__init__.py
--rw-rw-rw-   0        0        0     6872 2023-06-10 12:22:15.000000 custom_diffusion-0.1.3/custom_diffusion/pipelines/controlnet_inpaint_pipeline.py
--rw-rw-rw-   0        0        0     7330 2023-06-11 11:53:22.000000 custom_diffusion-0.1.3/custom_diffusion/pipelines/controlnet_pipeline.py
--rw-rw-rw-   0        0        0     9308 2023-06-12 11:16:13.000000 custom_diffusion-0.1.3/custom_diffusion/preprocces.py
-drwxrwxrwx   0        0        0        0 2023-06-12 11:16:19.732082 custom_diffusion-0.1.3/custom_diffusion/utils/
--rw-rw-rw-   0        0        0        0 2023-06-09 11:02:04.000000 custom_diffusion-0.1.3/custom_diffusion/utils/__init__.py
--rw-rw-rw-   0        0        0     2330 2023-06-11 16:27:33.000000 custom_diffusion-0.1.3/custom_diffusion/utils/data_utils.py
--rw-rw-rw-   0        0        0     1813 2023-06-12 11:16:05.000000 custom_diffusion-0.1.3/custom_diffusion/utils/downloads.py
--rw-rw-rw-   0        0        0     1307 2023-06-10 12:22:15.000000 custom_diffusion-0.1.3/custom_diffusion/utils/scheduler_utils.py
--rw-rw-rw-   0        0        0     3637 2023-06-11 10:55:21.000000 custom_diffusion-0.1.3/custom_diffusion/utils/video_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-12 11:16:19.713017 custom_diffusion-0.1.3/custom_diffusion.egg-info/
--rw-rw-rw-   0        0        0     2595 2023-06-12 11:16:19.000000 custom_diffusion-0.1.3/custom_diffusion.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      699 2023-06-12 11:16:19.000000 custom_diffusion-0.1.3/custom_diffusion.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 11:16:19.000000 custom_diffusion-0.1.3/custom_diffusion.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      175 2023-06-12 11:16:19.000000 custom_diffusion-0.1.3/custom_diffusion.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-12 11:16:19.000000 custom_diffusion-0.1.3/custom_diffusion.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-06-09 11:02:04.000000 custom_diffusion-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0      123 2023-06-10 12:22:15.000000 custom_diffusion-0.1.3/requirements.txt
--rw-rw-rw-   0        0        0      375 2023-06-12 11:16:19.739065 custom_diffusion-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     2218 2023-06-09 11:29:48.000000 custom_diffusion-0.1.3/setup.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-06-13 10:47:42.100524 custom_diffusion-0.1.5/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    11357 2023-06-12 21:08:38.000000 custom_diffusion-0.1.5/LICENSE
+-rw-r--r--   0 kadir     (1000) kadir     (1001)       24 2023-06-12 21:08:38.000000 custom_diffusion-0.1.5/MANIFEST.in
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     3110 2023-06-13 10:47:42.100524 custom_diffusion-0.1.5/PKG-INFO
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2062 2023-06-12 22:10:36.000000 custom_diffusion-0.1.5/README.md
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-06-13 10:47:42.093857 custom_diffusion-0.1.5/custom_diffusion/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      326 2023-06-13 10:45:31.000000 custom_diffusion-0.1.5/custom_diffusion/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2112 2023-06-13 10:35:42.000000 custom_diffusion-0.1.5/custom_diffusion/demo.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-06-13 10:47:42.097191 custom_diffusion-0.1.5/custom_diffusion/pipelines/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-06-12 21:08:38.000000 custom_diffusion-0.1.5/custom_diffusion/pipelines/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     7258 2023-06-13 10:47:00.000000 custom_diffusion-0.1.5/custom_diffusion/pipelines/controlnet_img2img.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     6684 2023-06-12 21:08:38.000000 custom_diffusion-0.1.5/custom_diffusion/pipelines/controlnet_inpaint_pipeline.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     7401 2023-06-13 10:45:31.000000 custom_diffusion-0.1.5/custom_diffusion/pipelines/controlnet_pipeline.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     8950 2023-06-12 21:08:38.000000 custom_diffusion-0.1.5/custom_diffusion/preprocces.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-06-13 10:47:42.100524 custom_diffusion-0.1.5/custom_diffusion/utils/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-06-12 21:08:38.000000 custom_diffusion-0.1.5/custom_diffusion/utils/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2330 2023-06-12 21:08:38.000000 custom_diffusion-0.1.5/custom_diffusion/utils/data_utils.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1759 2023-06-12 21:08:38.000000 custom_diffusion-0.1.5/custom_diffusion/utils/downloads.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      811 2023-06-13 10:45:31.000000 custom_diffusion-0.1.5/custom_diffusion/utils/model_list.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1268 2023-06-13 10:06:55.000000 custom_diffusion-0.1.5/custom_diffusion/utils/scheduler_utils.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     3545 2023-06-13 10:45:31.000000 custom_diffusion-0.1.5/custom_diffusion/utils/video_utils.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-06-13 10:47:42.097191 custom_diffusion-0.1.5/custom_diffusion.egg-info/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     3110 2023-06-13 10:47:41.000000 custom_diffusion-0.1.5/custom_diffusion.egg-info/PKG-INFO
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      785 2023-06-13 10:47:42.000000 custom_diffusion-0.1.5/custom_diffusion.egg-info/SOURCES.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        1 2023-06-13 10:47:41.000000 custom_diffusion-0.1.5/custom_diffusion.egg-info/dependency_links.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      175 2023-06-13 10:47:41.000000 custom_diffusion-0.1.5/custom_diffusion.egg-info/requires.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)       17 2023-06-13 10:47:41.000000 custom_diffusion-0.1.5/custom_diffusion.egg-info/top_level.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)       80 2023-06-12 21:08:38.000000 custom_diffusion-0.1.5/pyproject.toml
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      113 2023-06-12 21:08:38.000000 custom_diffusion-0.1.5/requirements.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      359 2023-06-13 10:47:42.103857 custom_diffusion-0.1.5/setup.cfg
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2151 2023-06-12 21:08:38.000000 custom_diffusion-0.1.5/setup.py
```

### Comparing `custom_diffusion-0.1.3/LICENSE` & `custom_diffusion-0.1.5/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `custom_diffusion-0.1.3/PKG-INFO` & `custom_diffusion-0.1.5/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,7 @@
-Metadata-Version: 2.1
-Name: custom_diffusion
-Version: 0.1.3
-Summary: Custom Diffusion: Creating Video from Frame Using Multiple Diffusion
-Home-page: https://github.com/kadirnar/Custom-Diffusion
-Author: kadirnar
-License: Apache License 2.0
-Keywords: machine-learning,deep-learning,pytorch,diffusion,diffusion models,controlnet,stable diffusion
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Education
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 <div align="center">
 <h2>
      Custom Diffusion: Creating Video from Frame Using Multiple Diffusion
 </h2>
 <div>
     <a href="https://pepy.tech/project/custom_diffusion"><img src="https://pepy.tech/badge/custom_diffusion" alt="downloads"></a>
     <a href="https://badge.fury.io/py/custom_diffusion"><img src="https://badge.fury.io/py/custom_diffusion.svg" alt="pypi version"></a>
@@ -39,32 +13,58 @@
 ### Installation
 ```bash
 pip install custom_diffusion
 ```
 
 ### Usage
 ```python
-from custom_diffusion.pipelines.controlnet_pipeline import StableDiffusionControlNetGenerator
 
+frames_path = video_pipeline(
+    video_url="https://huggingface.co/spaces/kadirnar/torchyolo/resolve/main/testv2.mp4",
+    youtube=False,
+    output_path="output",
+    filename="test.mp4",
+    quality="720p",
+    start_time=0,
+    end_time=2,
+    frame_rate=1,
+)
+
+images_list = load_images_from_folder(frames_path)
+image_grid(images_list, rows=5, cols=5)
+
+prompt = "a anime boy"
+negative_prompt = "bad"
+
+list_prompt = [prompt] * len(images_list)
+list_negative_prompt = [negative_prompt] * len(images_list)
 
 generator = StableDiffusionControlNetGenerator()
 
-generated_image = generator.generate_image(
-     stable_model_path="runwayml/stable-diffusion-v1-5"
-     controlnet_model_path="lllyasviel/control_v11p_sd15_canny",
-     scheduler_name="DDIM",
-     image_path="test.png",
-     prompt="Anime boy",
-     negative_prompt="bad",
-     height=512,
-     width=512,
-     guess_mode=False,
-     num_images_per_prompt=1,
-     num_inference_steps=20,
-     guidance_scale=7.0,
-     controlnet_conditioning_scale=1.0,
-     generator_seed=0,
-     preprocess_type="Canny",
-     resize_type="center_crop_and_resize",
-     crop_size=512,
+generated_image_list = generator.generate_image(
+    stable_model_path="andite/anything-v4.0",
+    controlnet_model_path="lllyasviel/control_v11p_sd15_canny",
+    scheduler_name="EulerAncestralDiscrete",
+    images_list=images_list,
+    prompt=list_prompt,
+    negative_prompt=list_negative_prompt,
+    height=512,
+    width=512,
+    guess_mode=False,
+    num_images_per_prompt=1,
+    num_inference_steps=30,
+    guidance_scale=7.0,
+    controlnet_conditioning_scale=1.0,
+    generator_seed=0,
+    preprocess_type="Canny",
+    resize_type="center_crop_and_resize",
+    crop_size=512,
+)
+
+frame2video = frames_to_video(
+    folder_path=generated_image_list,
+    output_folder="output",
+    output_video_name="frame2video.mp4",
+    duration=5,
 )
+
 ```
```

#### html2text {}

```diff
@@ -1,29 +1,21 @@
-Metadata-Version: 2.1 Name: custom_diffusion Version: 0.1.3 Summary: Custom
-Diffusion: Creating Video from Frame Using Multiple Diffusion Home-page: https:
-//github.com/kadirnar/Custom-Diffusion Author: kadirnar License: Apache License
-2.0 Keywords: machine-learning,deep-learning,pytorch,diffusion,diffusion
-models,controlnet,stable diffusion Classifier: Development Status :: 5 -
-Production/Stable Classifier: Operating System :: OS Independent Classifier:
-Intended Audience :: Developers Classifier: Intended Audience :: Science/
-Research Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Topic :: Software Development :: Libraries Classifier: Topic :: Software
-Development :: Libraries :: Python Modules Classifier: Topic :: Education
-Classifier: Topic :: Scientific/Engineering Classifier: Topic :: Scientific/
-Engineering :: Artificial Intelligence Requires-Python: >=3.6 Description-
-Content-Type: text/markdown Provides-Extra: dev License-File: LICENSE
   ***** Custom Diffusion: Creating Video from Frame Using Multiple Diffusion
                                      *****
                 [downloads] [pypi_version] [HuggingFace_Spaces]
 ### Installation ```bash pip install custom_diffusion ``` ### Usage ```python
-from custom_diffusion.pipelines.controlnet_pipeline import
-StableDiffusionControlNetGenerator generator =
-StableDiffusionControlNetGenerator() generated_image = generator.generate_image
-( stable_model_path="runwayml/stable-diffusion-v1-5"
+frames_path = video_pipeline( video_url="https://huggingface.co/spaces/
+kadirnar/torchyolo/resolve/main/testv2.mp4", youtube=False,
+output_path="output", filename="test.mp4", quality="720p", start_time=0,
+end_time=2, frame_rate=1, ) images_list = load_images_from_folder(frames_path)
+image_grid(images_list, rows=5, cols=5) prompt = "a anime boy" negative_prompt
+= "bad" list_prompt = [prompt] * len(images_list) list_negative_prompt =
+[negative_prompt] * len(images_list) generator =
+StableDiffusionControlNetGenerator() generated_image_list =
+generator.generate_image( stable_model_path="andite/anything-v4.0",
 controlnet_model_path="lllyasviel/control_v11p_sd15_canny",
-scheduler_name="DDIM", image_path="test.png", prompt="Anime boy",
-negative_prompt="bad", height=512, width=512, guess_mode=False,
-num_images_per_prompt=1, num_inference_steps=20, guidance_scale=7.0,
-controlnet_conditioning_scale=1.0, generator_seed=0, preprocess_type="Canny",
-resize_type="center_crop_and_resize", crop_size=512, ) ```
+scheduler_name="EulerAncestralDiscrete", images_list=images_list,
+prompt=list_prompt, negative_prompt=list_negative_prompt, height=512,
+width=512, guess_mode=False, num_images_per_prompt=1, num_inference_steps=30,
+guidance_scale=7.0, controlnet_conditioning_scale=1.0, generator_seed=0,
+preprocess_type="Canny", resize_type="center_crop_and_resize", crop_size=512, )
+frame2video = frames_to_video( folder_path=generated_image_list,
+output_folder="output", output_video_name="frame2video.mp4", duration=5, ) ```
```

### Comparing `custom_diffusion-0.1.3/custom_diffusion/pipelines/controlnet_inpaint_pipeline.py` & `custom_diffusion-0.1.5/custom_diffusion/pipelines/controlnet_img2img.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,188 +1,196 @@
-from typing import Optional
-
-import numpy as np
-import torch
-from diffusers import ControlNetModel, StableDiffusionControlNetInpaintPipeline
-from PIL import Image
-
-from custom_diffusion.preprocces import preprocces_dicts
-from custom_diffusion.utils.data_utils import center_crop_and_resize
-from custom_diffusion.utils.scheduler_utils import get_scheduler
-
-
-class StableDiffusionControlNetInpaintGenerator:
-    """
-    A class to handle image generation using stable diffusion and control net models.
-    """
-
-    def __init__(self):
-        self.controlnet = None
-        self.pipe = None
-        self.model_cache = {}
-
-    def _load_controlnet_model(self, controlnet_model_path):
-        """
-        This function loads the controlnet model.
-
-        Args:
-        controlnet_model_path (str): Path to the controlnet model.
-
-        """
-        self.controlnet = ControlNetModel.from_pretrained(controlnet_model_path, torch_dtype=torch.float16)
-
-    def _load_stable_diffusion_pipeline(self, stable_model_path):
-        """
-        This function loads the stable diffusion pipeline.
-
-        Args:
-        stable_model_path (str): Path to the stable diffusion pipeline.
-
-        """
-        self.pipe = StableDiffusionControlNetInpaintPipeline.from_pretrained(
-            pretrained_model_name_or_path=stable_model_path,
-            controlnet=self.controlnet,
-            safety_checker=None,
-            torch_dtype=torch.float16,
-        )
-
-    def load_model(self, stable_model_path, controlnet_model_path, scheduler_name):
-        """
-        Load the models and setup the scheduler if not cached.
-
-        Args:
-        stable_model_path (str): Path to the stable model.
-        controlnet_model_path (str): Path to the controlnet model.
-        scheduler_name (str): Name of the scheduler.
-
-        Returns:
-        pipe: Configured model pipeline.
-        """
-        model_key = (stable_model_path, controlnet_model_path, scheduler_name)
-
-        # load and setup models only if they're not in the cache
-        if model_key not in self.model_cache:
-            self._load_controlnet_model(controlnet_model_path)
-            self._load_stable_diffusion_pipeline(stable_model_path)
-            self.pipe = get_scheduler(pipe=self.pipe, scheduler_name=scheduler_name)
-            self.pipe.to("cuda")
-            self.pipe.enable_xformers_memory_efficient_attention()
-
-            self.model_cache[model_key] = self.pipe
-
-        return self.model_cache[model_key]
-
-    def load_and_resize_image(
-        self, image: Image, resize_type: str, crop_size: Optional[int], height: Optional[int], width: Optional[int]
-    ):
-        """
-        This function loads and resizes an image to a specified size.
-
-        Args:
-        image (Image): The PIL Image object.
-
-        Returns:
-        Image: The resized and loaded PIL Image.
-        """
-        image = image.convert("RGB")
-
-        if resize_type == "center_crop_and_resize":
-            image = center_crop_and_resize(image, crop_size=crop_size, height=height, width=width)
-
-        elif resize_type == "resize":
-            image = image.resize((height, width))
-
-        else:
-            raise ValueError("Invalid resize type.")
-
-        image = np.array(image)
-
-        return Image.fromarray(image)
-
-    def _setup_generator(self, generator_seed):
-        if generator_seed == 0:
-            random_seed = torch.randint(0, 1000000, (1,))
-            generator = torch.manual_seed(random_seed)
-        else:
-            generator = torch.manual_seed(generator_seed)
-        return generator
-
-    def generate_image(
-        self,
-        stable_model_path: str,
-        controlnet_model_path: str,
-        scheduler_name: str,
-        image_paths: str,
-        prompt: str,
-        negative_prompt: str,
-        height: int,
-        width: int,
-        strength: int,
-        guess_mode: bool,
-        num_images_per_prompt: int,
-        num_inference_steps: int,
-        guidance_scale: int,
-        controlnet_conditioning_scale: int,
-        generator_seed: int,
-        preprocess_type: str,
-        resize_type: str,
-    ):
-        """
-        This function generates an image based on the given parameters.
-
-        Args:
-        stable_model_path (str): Path to the stable model.
-        controlnet_model_path (str): Path to the controlnet model.
-        scheduler_name (str): Name of the scheduler.
-        image_paths (str): Path to the image to generate.
-        prompt (str): The prompt for image generation.
-        negative_prompt (str): The negative prompt for image generation.
-        height (int): The height of the image to generate.
-        width (int): The width of the image to generate.
-        strength (int): The strength of the image generation process.
-        guess_mode (bool): Whether or not to use guess mode in image generation.
-        num_images_per_prompt (int): The number of images to generate per prompt.
-        num_inference_steps (int): The number of inference steps in image generation.
-        guidance_scale (int): The scale of guidance in image generation.
-        controlnet_conditioning_scale (int): The scale of controlnet conditioning in image generation.
-        generator_seed (int): The seed for the random generator.
-        preprocess_type (str): The type of preprocessing to apply.
-        resize_type (str): The type of resizing to apply.
-
-        Returns:
-        output: The generated image.
-        """
-        normal_image = self.load_and_resize_image(
-            image=image_paths["image"], resize_type=resize_type, height=height, width=width
-        )
-        mask_image = self.load_and_resize_image(
-            image=image_paths["mask"], resize_type=resize_type, height=height, width=width
-        )
-
-        control_image = preprocces_dicts[preprocess_type](normal_image)
-
-        pipe = self.load_model(
-            stable_model_path=stable_model_path,
-            controlnet_model_path=controlnet_model_path,
-            scheduler_name=scheduler_name,
-        )
-
-        generator = self._setup_generator(generator_seed)
-
-        output = pipe(
-            prompt=prompt,
-            image=normal_image,
-            height=height,
-            width=width,
-            mask_image=mask_image,
-            strength=strength,
-            guess_mode=guess_mode,
-            control_image=control_image,
-            negative_prompt=negative_prompt,
-            num_images_per_prompt=num_images_per_prompt,
-            num_inference_steps=num_inference_steps,
-            guidance_scale=guidance_scale,
-            controlnet_conditioning_scale=float(controlnet_conditioning_scale),
-            generator=generator,
-        ).images
-
-        return output
+from typing import List, Optional
+
+import torch
+from diffusers import ControlNetModel, StableDiffusionControlNetImg2ImgPipeline
+from PIL import Image
+
+from custom_diffusion.preprocces import preprocces_dicts
+from custom_diffusion.utils.data_utils import center_crop_and_resize
+from custom_diffusion.utils.scheduler_utils import get_scheduler
+
+
+class StableDiffusionControlNetImg2ImgGenerator:
+    """
+    A class to handle image generation using stable diffusion and control net models.
+    """
+
+    def __init__(self):
+        self.controlnet = None
+        self.pipe = None
+        self.model_cache = {}
+
+    def _load_controlnet_model(self, controlnet_model_path: str = "lllyasviel/control_v11p_sd15_canny"):
+        """
+        This function loads the controlnet model.
+
+        Args:
+        controlnet_model_path (str): Path to the controlnet model.
+
+        """
+        self.controlnet = ControlNetModel.from_pretrained(controlnet_model_path, torch_dtype=torch.float16)
+
+    def _load_stable_diffusion_pipeline(self, stable_model_path: str = "runwayml/stable-diffusion-v1-5"):
+        """
+        This function loads the stable diffusion pipeline.
+
+        Args:
+        stable_model_path (str): Path to the stable diffusion pipeline.
+
+        """
+        self.pipe = StableDiffusionControlNetImg2ImgPipeline.from_pretrained(
+            pretrained_model_name_or_path=stable_model_path,
+            controlnet=self.controlnet,
+            safety_checker=None,
+            torch_dtype=torch.float16,
+        )
+
+    def load_model(
+        self,
+        stable_model_path: str = "runwayml/stable-diffusion-v1-5",
+        controlnet_model_path: str = "lllyasviel/control_v11p_sd15_canny",
+        scheduler_name: str = "DDIM",
+    ):
+        """
+        Load the models and setup the scheduler if not cached.
+
+        Args:
+        stable_model_path (str): Path to the stable model.
+        controlnet_model_path (str): Path to the controlnet model.
+        scheduler_name (str): Name of the scheduler.
+
+        Returns:
+        pipe: Configured model pipeline.
+        """
+        model_key = (stable_model_path, controlnet_model_path, scheduler_name)
+
+        # load and setup models only if they're not in the cache
+        if model_key not in self.model_cache:
+            self._load_controlnet_model(controlnet_model_path)
+            self._load_stable_diffusion_pipeline(stable_model_path)
+            self.pipe = get_scheduler(pipe=self.pipe, scheduler_name=scheduler_name)
+            self.pipe.to("cuda")
+            self.pipe.enable_xformers_memory_efficient_attention()
+
+            self.model_cache[model_key] = self.pipe
+
+        return self.model_cache[model_key]
+
+    def load_and_resize_image(
+        self,
+        image_path: str = "test.png",
+        resize_type: str = "center_crop_and_resize",
+        crop_size: Optional[int] = 512,
+        height: Optional[int] = 512,
+        width: Optional[int] = 512,
+    ):
+        """
+        This function loads and resizes the image.
+
+        Args:
+        image_path (str): Path to the image.
+        resize_type (str): The type of resizing to apply.
+        crop_size (int): The size of the crop.
+        height (int): The height of the image to generate.
+        width (int): The width of the image to generate.
+
+        Returns:
+        Image: The resized and loaded PIL Image.
+        """
+        image = Image.open(image_path)
+
+        if resize_type == "center_crop_and_resize":
+            image = center_crop_and_resize(image, crop_size=crop_size, height=height, width=width)
+
+        elif resize_type == "resize":
+            image = image.resize((height, width))
+
+        else:
+            raise ValueError("Invalid resize type.")
+
+        return image
+
+    def _setup_generator(self, generator_seed: int = 0):
+        if generator_seed == 0:
+            random_seed = torch.randint(0, 1000000, (1,))
+            generator = torch.manual_seed(random_seed)
+        else:
+            generator = torch.manual_seed(generator_seed)
+        return generator
+
+    def generate_image(
+        self,
+        stable_model_path: str = "runwayml/stable-diffusion-v1-5",
+        controlnet_model_path: str = "lllyasviel/control_v11p_sd15_canny",
+        scheduler_name: str = "DDIM",
+        images_list: List[str] = ["test.png"],
+        prompt: List[str] = ["A photo of a cat."],
+        negative_prompt: List[str] = ["bad"],
+        height: int = 512,
+        width: int = 512,
+        guess_mode: bool = False,
+        num_images_per_prompt: int = 1,
+        num_inference_steps: int = 20,
+        guidance_scale: int = 7.0,
+        controlnet_conditioning_scale: int = 1.0,
+        strength: float = 0.5,
+        generator_seed: int = 0,
+        preprocess_type: str = "Canny",
+        resize_type: str = "center_crop_and_resize",
+        crop_size: int = 512,
+    ):
+        """
+        This function generates an image based on the given parameters.
+
+        Args:
+        stable_model_path (str): Path to the stable model.
+        controlnet_model_path (str): Path to the controlnet model.
+        scheduler_name (str): Name of the scheduler.
+        image_path (dict): Path of the images.
+        prompt (dict): The prompt for image generation.
+        negative_prompt (str): The negative prompt for image generation.
+        height (int): The height of the image to generate.
+        width (int): The width of the image to generate.
+        guess_mode (bool): Whether or not to use guess mode in image generation.
+        num_images_per_prompt (int): The number of images to generate per prompt.
+        num_inference_steps (int): The number of inference steps in image generation.
+        guidance_scale (int): The scale of guidance in image generation.
+        controlnet_conditioning_scale (int): The scale of controlnet conditioning in image generation.
+        generator_seed (int): The seed for the random generator.
+        preprocess_type (str): The type of preprocessing to apply.
+
+        Returns:
+        output: The generated image.
+        """
+        control_image_list = []
+        for image_path in images_list:
+            read_image = self.load_and_resize_image(
+                image_path=image_path, resize_type=resize_type, height=height, width=width, crop_size=crop_size
+            )
+            control_image = preprocces_dicts[preprocess_type](read_image)
+            control_image_list.append(control_image)
+
+        pipe = self.load_model(
+            stable_model_path=stable_model_path,
+            controlnet_model_path=controlnet_model_path,
+            scheduler_name=scheduler_name,
+        )
+
+        generator = self._setup_generator(generator_seed)
+
+        output = pipe(
+            prompt=prompt,
+            height=height,
+            width=width,
+            guess_mode=guess_mode,
+            control_image=control_image_list,
+            image=read_image,
+            strength=strength,
+            negative_prompt=negative_prompt,
+            num_images_per_prompt=num_images_per_prompt,
+            num_inference_steps=num_inference_steps,
+            guidance_scale=guidance_scale,
+            controlnet_conditioning_scale=float(controlnet_conditioning_scale),
+            generator=generator,
+        ).images
+
+        return output
```

### Comparing `custom_diffusion-0.1.3/custom_diffusion/utils/data_utils.py` & `custom_diffusion-0.1.5/custom_diffusion/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `custom_diffusion-0.1.3/custom_diffusion/utils/downloads.py` & `custom_diffusion-0.1.5/custom_diffusion/utils/downloads.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-def download_from_youtube_url(
-    youtube_video_url: str = "https://www.youtube.com/watch?v=8QRG4vzbdE0",
-    output_path: str = "output_videos",
-    quality: str = "720p",
-    filename: str = "downloaded_video.mp4",
-):
-    """
-    This function downloads a video and corresponding audio from YouTube and saves it in the designated output folder.
-
-    Args:
-    video_url (str): URL of the YouTube video to be downloaded.
-    output_path (str): Directory path where the downloaded video will be saved.
-    quality (str): Desired quality of the video to be downloaded. It can be '144p', '240p', '360p', '480p', '720p', '1080p', '1440p' (for 2K), or '2160p' (for 4K).
-    filename (str): Desired filename of the downloaded video.
-
-    Returns:
-    None
-    """
-    import os
-
-    from pytube import YouTube
-
-    # Create a YouTube object
-    yt = YouTube(youtube_video_url)
-
-    # Find the stream with the desired quality that also contains audio
-    video_stream = yt.streams.filter(progressive=True, file_extension="mp4", res=quality).first()
-
-    if video_stream is not None:
-        # Download the stream
-        video_stream.download(output_path, filename=filename)
-        print("Video downloaded successfully!")
-    else:
-        print(f"No video stream found for {quality} quality.")
-
-    save_path = os.path.join(output_path, filename)
-    return save_path
-
-
-def download_from_url(from_url: str, to_path: str):
-    # https://github.com/obss/sahi/blob/main/sahi/utils/file.py
-    import os
-    import urllib.request
-    from pathlib import Path
-
-    Path(to_path).parent.mkdir(parents=True, exist_ok=True)
-
-    if not os.path.exists(to_path):
-        urllib.request.urlretrieve(
-            from_url,
-            to_path,
-        )
-
-    return to_path
+def download_from_youtube_url(
+    youtube_video_url: str = "https://www.youtube.com/watch?v=8QRG4vzbdE0",
+    output_path: str = "output_videos",
+    quality: str = "720p",
+    filename: str = "downloaded_video.mp4",
+):
+    """
+    This function downloads a video and corresponding audio from YouTube and saves it in the designated output folder.
+
+    Args:
+    video_url (str): URL of the YouTube video to be downloaded.
+    output_path (str): Directory path where the downloaded video will be saved.
+    quality (str): Desired quality of the video to be downloaded. It can be '144p', '240p', '360p', '480p', '720p', '1080p', '1440p' (for 2K), or '2160p' (for 4K).
+    filename (str): Desired filename of the downloaded video.
+
+    Returns:
+    None
+    """
+    import os
+
+    from pytube import YouTube
+
+    # Create a YouTube object
+    yt = YouTube(youtube_video_url)
+
+    # Find the stream with the desired quality that also contains audio
+    video_stream = yt.streams.filter(progressive=True, file_extension="mp4", res=quality).first()
+
+    if video_stream is not None:
+        # Download the stream
+        video_stream.download(output_path, filename=filename)
+        print("Video downloaded successfully!")
+    else:
+        print(f"No video stream found for {quality} quality.")
+
+    save_path = os.path.join(output_path, filename)
+    return save_path
+
+
+def download_from_url(from_url: str, to_path: str):
+    # https://github.com/obss/sahi/blob/main/sahi/utils/file.py
+    import os
+    import urllib.request
+    from pathlib import Path
+
+    Path(to_path).parent.mkdir(parents=True, exist_ok=True)
+
+    if not os.path.exists(to_path):
+        urllib.request.urlretrieve(
+            from_url,
+            to_path,
+        )
+
+    return to_path
```

### Comparing `custom_diffusion-0.1.3/custom_diffusion/utils/scheduler_utils.py` & `custom_diffusion-0.1.5/custom_diffusion/utils/scheduler_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-from diffusers import (
-    DDIMScheduler,
-    DDPMScheduler,
-    DEISMultistepScheduler,
-    DPMSolverMultistepScheduler,
-    DPMSolverSinglestepScheduler,
-    EulerAncestralDiscreteScheduler,
-    EulerDiscreteScheduler,
-    HeunDiscreteScheduler,
-    KDPM2AncestralDiscreteScheduler,
-    KDPM2DiscreteScheduler,
-    PNDMScheduler,
-    UniPCMultistepScheduler,
-)
-
-SCHEDULER_MAPPING = {
-    "DDIM": DDIMScheduler,
-    "DDPMScheduler": DDPMScheduler,
-    "DEISMultistep": DEISMultistepScheduler,
-    "DPMSolverMultistep": DPMSolverMultistepScheduler,
-    "DPMSolverSinglestep": DPMSolverSinglestepScheduler,
-    "EulerAncestralDiscrete": EulerAncestralDiscreteScheduler,
-    "EulerDiscrete": EulerDiscreteScheduler,
-    "HeunDiscrete": HeunDiscreteScheduler,
-    "KDPM2AncestralDiscrete": KDPM2AncestralDiscreteScheduler,
-    "KDPM2Discrete": KDPM2DiscreteScheduler,
-    "PNDMScheduler": PNDMScheduler,
-    "UniPCMultistep": UniPCMultistepScheduler,
-}
-
-
-def get_scheduler(pipe, scheduler_name):
-    if scheduler_name in SCHEDULER_MAPPING:
-        SchedulerClass = SCHEDULER_MAPPING[scheduler_name]
-        pipe.scheduler = SchedulerClass.from_config(pipe.scheduler.config)
-    else:
-        raise ValueError(f"Invalid scheduler name {scheduler_name}")
-
-    return pipe
+from diffusers import (
+    DDIMScheduler,
+    DDPMScheduler,
+    DEISMultistepScheduler,
+    DPMSolverMultistepScheduler,
+    DPMSolverSinglestepScheduler,
+    EulerAncestralDiscreteScheduler,
+    EulerDiscreteScheduler,
+    HeunDiscreteScheduler,
+    KDPM2AncestralDiscreteScheduler,
+    KDPM2DiscreteScheduler,
+    PNDMScheduler,
+    UniPCMultistepScheduler,
+)
+
+scheduler_mapping = {
+    "DDIM": DDIMScheduler,
+    "DDPMScheduler": DDPMScheduler,
+    "DEISMultistep": DEISMultistepScheduler,
+    "DPMSolverMultistep": DPMSolverMultistepScheduler,
+    "DPMSolverSinglestep": DPMSolverSinglestepScheduler,
+    "EulerAncestralDiscrete": EulerAncestralDiscreteScheduler,
+    "EulerDiscrete": EulerDiscreteScheduler,
+    "HeunDiscrete": HeunDiscreteScheduler,
+    "KDPM2AncestralDiscrete": KDPM2AncestralDiscreteScheduler,
+    "KDPM2Discrete": KDPM2DiscreteScheduler,
+    "PNDMScheduler": PNDMScheduler,
+    "UniPCMultistep": UniPCMultistepScheduler,
+}
+
+
+def get_scheduler(pipe, scheduler_name):
+    if scheduler_name in scheduler_mapping:
+        SchedulerClass = scheduler_mapping[scheduler_name]
+        pipe.scheduler = SchedulerClass.from_config(pipe.scheduler.config)
+    else:
+        raise ValueError(f"Invalid scheduler name {scheduler_name}")
+
+    return pipe
```

### Comparing `custom_diffusion-0.1.3/custom_diffusion.egg-info/SOURCES.txt` & `custom_diffusion-0.1.5/custom_diffusion.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 custom_diffusion/preprocces.py
 custom_diffusion.egg-info/PKG-INFO
 custom_diffusion.egg-info/SOURCES.txt
 custom_diffusion.egg-info/dependency_links.txt
 custom_diffusion.egg-info/requires.txt
 custom_diffusion.egg-info/top_level.txt
 custom_diffusion/pipelines/__init__.py
+custom_diffusion/pipelines/controlnet_img2img.py
 custom_diffusion/pipelines/controlnet_inpaint_pipeline.py
 custom_diffusion/pipelines/controlnet_pipeline.py
 custom_diffusion/utils/__init__.py
 custom_diffusion/utils/data_utils.py
 custom_diffusion/utils/downloads.py
+custom_diffusion/utils/model_list.py
 custom_diffusion/utils/scheduler_utils.py
 custom_diffusion/utils/video_utils.py
```

### Comparing `custom_diffusion-0.1.3/setup.py` & `custom_diffusion-0.1.5/setup.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-import io
-import os
-import re
-
-import setuptools
-
-
-def get_long_description():
-    base_dir = os.path.abspath(os.path.dirname(__file__))
-    with io.open(os.path.join(base_dir, "README.md"), encoding="utf-8") as f:
-        return f.read()
-
-
-def get_requirements():
-    with open("requirements.txt") as f:
-        return f.read().splitlines()
-
-
-def get_version():
-    current_dir = os.path.abspath(os.path.dirname(__file__))
-    version_file = os.path.join(current_dir, "custom_diffusion", "__init__.py")
-    with io.open(version_file, encoding="utf-8") as f:
-        return re.search(r'^__version__ = [\'"]([^\'"]*)[\'"]', f.read(), re.M).group(1)
-
-
-_DEV_REQUIREMENTS = [
-    "black==21.7b0",
-    "flake8==3.9.2",
-    "isort==5.9.2",
-    "click==8.0.4",
-]
-
-
-extras = {"dev": _DEV_REQUIREMENTS}
-
-
-setuptools.setup(
-    name="custom_diffusion",
-    version=get_version(),
-    author="kadirnar",
-    license="Apache License 2.0",
-    description="Custom Diffusion: Creating Video from Frame Using Multiple Diffusion",
-    long_description=get_long_description(),
-    long_description_content_type="text/markdown",
-    url="https://github.com/kadirnar/Custom-Diffusion",
-    packages=setuptools.find_packages(exclude=["tests"]),
-    extras_require=extras,
-    include_package_data=True,
-    python_requires=">=3.6",
-    install_requires=get_requirements(),
-    classifiers=[
-        "Development Status :: 5 - Production/Stable",
-        "Operating System :: OS Independent",
-        "Intended Audience :: Developers",
-        "Intended Audience :: Science/Research",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Topic :: Software Development :: Libraries",
-        "Topic :: Software Development :: Libraries :: Python Modules",
-        "Topic :: Education",
-        "Topic :: Scientific/Engineering",
-        "Topic :: Scientific/Engineering :: Artificial Intelligence",
-    ],
-    keywords="machine-learning, deep-learning, pytorch, diffusion, diffusion models, controlnet,stable diffusion",
-)
+import io
+import os
+import re
+
+import setuptools
+
+
+def get_long_description():
+    base_dir = os.path.abspath(os.path.dirname(__file__))
+    with io.open(os.path.join(base_dir, "README.md"), encoding="utf-8") as f:
+        return f.read()
+
+
+def get_requirements():
+    with open("requirements.txt") as f:
+        return f.read().splitlines()
+
+
+def get_version():
+    current_dir = os.path.abspath(os.path.dirname(__file__))
+    version_file = os.path.join(current_dir, "custom_diffusion", "__init__.py")
+    with io.open(version_file, encoding="utf-8") as f:
+        return re.search(r'^__version__ = [\'"]([^\'"]*)[\'"]', f.read(), re.M).group(1)
+
+
+_DEV_REQUIREMENTS = [
+    "black==21.7b0",
+    "flake8==3.9.2",
+    "isort==5.9.2",
+    "click==8.0.4",
+]
+
+
+extras = {"dev": _DEV_REQUIREMENTS}
+
+
+setuptools.setup(
+    name="custom_diffusion",
+    version=get_version(),
+    author="kadirnar",
+    license="Apache License 2.0",
+    description="Custom Diffusion: Creating Video from Frame Using Multiple Diffusion",
+    long_description=get_long_description(),
+    long_description_content_type="text/markdown",
+    url="https://github.com/kadirnar/Custom-Diffusion",
+    packages=setuptools.find_packages(exclude=["tests"]),
+    extras_require=extras,
+    include_package_data=True,
+    python_requires=">=3.6",
+    install_requires=get_requirements(),
+    classifiers=[
+        "Development Status :: 5 - Production/Stable",
+        "Operating System :: OS Independent",
+        "Intended Audience :: Developers",
+        "Intended Audience :: Science/Research",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Topic :: Software Development :: Libraries",
+        "Topic :: Software Development :: Libraries :: Python Modules",
+        "Topic :: Education",
+        "Topic :: Scientific/Engineering",
+        "Topic :: Scientific/Engineering :: Artificial Intelligence",
+    ],
+    keywords="machine-learning, deep-learning, pytorch, diffusion, diffusion models, controlnet,stable diffusion",
+)
```

