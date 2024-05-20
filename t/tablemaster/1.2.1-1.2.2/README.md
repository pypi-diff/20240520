# Comparing `tmp/tablemaster-1.2.1.tar.gz` & `tmp/tablemaster-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tablemaster-1.2.1.tar", last modified: Mon Apr 15 07:00:28 2024, max compression
+gzip compressed data, was "tablemaster-1.2.2.tar", last modified: Mon May 20 11:46:29 2024, max compression
```

## Comparing `tablemaster-1.2.1.tar` & `tablemaster-1.2.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 07:00:28.285554 tablemaster-1.2.1/
--rw-rw-rw-   0        0        0    11558 2024-04-10 02:51:24.000000 tablemaster-1.2.1/LICENSE
--rw-rw-rw-   0        0        0      247 2024-04-15 07:00:28.284528 tablemaster-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     2692 2024-04-10 05:57:40.000000 tablemaster-1.2.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-15 07:00:28.285554 tablemaster-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0      538 2024-04-15 06:58:17.000000 tablemaster-1.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-15 07:00:28.280933 tablemaster-1.2.1/tablemaster/
--rw-rw-rw-   0        0        0      671 2024-04-10 05:38:21.000000 tablemaster-1.2.1/tablemaster/__init__.py
--rw-rw-rw-   0        0        0     1749 2024-04-10 02:51:24.000000 tablemaster-1.2.1/tablemaster/feishu.py
--rw-rw-rw-   0        0        0     1170 2024-04-10 02:51:24.000000 tablemaster-1.2.1/tablemaster/gspread.py
--rw-rw-rw-   0        0        0     3427 2024-04-10 02:51:24.000000 tablemaster-1.2.1/tablemaster/local.py
--rw-rw-rw-   0        0        0     5913 2024-04-15 06:58:08.000000 tablemaster-1.2.1/tablemaster/mysql.py
--rw-rw-rw-   0        0        0      828 2024-04-10 02:51:24.000000 tablemaster-1.2.1/tablemaster/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-15 07:00:28.284528 tablemaster-1.2.1/tablemaster.egg-info/
--rw-rw-rw-   0        0        0      247 2024-04-15 07:00:28.000000 tablemaster-1.2.1/tablemaster.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      332 2024-04-15 07:00:28.000000 tablemaster-1.2.1/tablemaster.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 07:00:28.000000 tablemaster-1.2.1/tablemaster.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2024-04-15 07:00:28.000000 tablemaster-1.2.1/tablemaster.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-15 07:00:28.000000 tablemaster-1.2.1/tablemaster.egg-info/top_level.txt
+drwxr-xr-x   0 livid      (501) staff       (20)        0 2024-05-20 11:46:29.965291 tablemaster-1.2.2/
+-rw-r--r--   0 livid      (501) staff       (20)    11357 2024-05-20 11:04:14.000000 tablemaster-1.2.2/LICENSE
+-rw-r--r--   0 livid      (501) staff       (20)      451 2024-05-20 11:46:29.965106 tablemaster-1.2.2/PKG-INFO
+-rw-r--r--   0 livid      (501) staff       (20)     2560 2024-05-20 11:04:14.000000 tablemaster-1.2.2/README.md
+-rw-r--r--   0 livid      (501) staff       (20)       38 2024-05-20 11:46:29.965331 tablemaster-1.2.2/setup.cfg
+-rw-r--r--   0 livid      (501) staff       (20)      517 2024-05-20 11:45:52.000000 tablemaster-1.2.2/setup.py
+drwxr-xr-x   0 livid      (501) staff       (20)        0 2024-05-20 11:46:29.964252 tablemaster-1.2.2/tablemaster/
+-rw-r--r--   0 livid      (501) staff       (20)      632 2024-05-20 11:04:14.000000 tablemaster-1.2.2/tablemaster/__init__.py
+-rw-r--r--   0 livid      (501) staff       (20)     1716 2024-05-20 11:04:14.000000 tablemaster-1.2.2/tablemaster/feishu.py
+-rw-r--r--   0 livid      (501) staff       (20)     1138 2024-05-20 11:04:14.000000 tablemaster-1.2.2/tablemaster/gspread.py
+-rw-r--r--   0 livid      (501) staff       (20)     3334 2024-05-20 11:04:14.000000 tablemaster-1.2.2/tablemaster/local.py
+-rw-r--r--   0 livid      (501) staff       (20)     5829 2024-05-20 11:45:13.000000 tablemaster-1.2.2/tablemaster/mysql.py
+-rw-r--r--   0 livid      (501) staff       (20)      810 2024-05-20 11:04:14.000000 tablemaster-1.2.2/tablemaster/utils.py
+drwxr-xr-x   0 livid      (501) staff       (20)        0 2024-05-20 11:46:29.964911 tablemaster-1.2.2/tablemaster.egg-info/
+-rw-r--r--   0 livid      (501) staff       (20)      451 2024-05-20 11:46:29.000000 tablemaster-1.2.2/tablemaster.egg-info/PKG-INFO
+-rw-r--r--   0 livid      (501) staff       (20)      332 2024-05-20 11:46:29.000000 tablemaster-1.2.2/tablemaster.egg-info/SOURCES.txt
+-rw-r--r--   0 livid      (501) staff       (20)        1 2024-05-20 11:46:29.000000 tablemaster-1.2.2/tablemaster.egg-info/dependency_links.txt
+-rw-r--r--   0 livid      (501) staff       (20)       77 2024-05-20 11:46:29.000000 tablemaster-1.2.2/tablemaster.egg-info/requires.txt
+-rw-r--r--   0 livid      (501) staff       (20)       12 2024-05-20 11:46:29.000000 tablemaster-1.2.2/tablemaster.egg-info/top_level.txt
```

### Comparing `tablemaster-1.2.1/LICENSE` & `tablemaster-1.2.2/LICENSE`

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

### Comparing `tablemaster-1.2.1/tablemaster/__init__.py` & `tablemaster-1.2.2/tablemaster/__init__.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-
-from yaml import load, dump
-try:
-    from yaml import CLoader as Loader, CDumper as Dumper
-except ImportError:
-    from yaml import Loader, Dumper
-import json
-from types import SimpleNamespace
-import pandas as pd
-
-
-with open('cfg.yaml') as cfg:
-    cfg = json.loads(json.dumps(load(cfg, Loader=Loader)), object_hook=lambda d: SimpleNamespace(**d))
-
-from . import utils
-
-from .mysql import (
-    query,
-    opt,
-    ManageTable,
-    Manage_table,
-)
-
-from .gspread import (
-    gs_read_df,
-    gs_write_df,
-)
-
-from .local import (
-    read,
-    batch_read,
-    read_dfs,
-)
-
-from .feishu import (
-    fs_read_df,
-    fs_read_base,
-)
-
+
+from yaml import load, dump
+try:
+    from yaml import CLoader as Loader, CDumper as Dumper
+except ImportError:
+    from yaml import Loader, Dumper
+import json
+from types import SimpleNamespace
+import pandas as pd
+
+
+with open('cfg.yaml') as cfg:
+    cfg = json.loads(json.dumps(load(cfg, Loader=Loader)), object_hook=lambda d: SimpleNamespace(**d))
+
+from . import utils
+
+from .mysql import (
+    query,
+    opt,
+    ManageTable,
+    Manage_table,
+)
+
+from .gspread import (
+    gs_read_df,
+    gs_write_df,
+)
+
+from .local import (
+    read,
+    batch_read,
+    read_dfs,
+)
+
+from .feishu import (
+    fs_read_df,
+    fs_read_base,
+)
+
```

### Comparing `tablemaster-1.2.1/tablemaster/feishu.py` & `tablemaster-1.2.2/tablemaster/feishu.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-import json
-import requests
-import pandas as pd
-
-def fs_read_df(sheet_address, feishu_cfg):
-    # 获取tenant_access_token
-    feishu_url = "https://open.feishu.cn/open-apis/auth/v3/tenant_access_token/internal/"
-    post_data = {"app_id":feishu_cfg.feishu_app_id,
-                "app_secret":feishu_cfg.feishu_app_secret}
-    r = requests.post(feishu_url, data=post_data)
-    tat = r.json()["tenant_access_token"]
-    header = {"content-type":"application/json",
-    "Authorization":"Bearer " + str(tat)}
-    url = "https://open.feishu.cn/open-apis/sheets/v2/spreadsheets/" + sheet_address[0] + "/values/" + sheet_address[1] \
-        + "?valueRenderOption=ToString&dateTimeRenderOption=FormattedString"
-    r = requests.get(url, headers = header)
-    pull_data = r.json()['data']['valueRange']['values']
-    return pd.DataFrame(pull_data[1:], columns=pull_data[0])
-
-def fs_read_base(sheet_address, feishu_cfg):
-    # 获取tenant_access_token
-    feishu_url = "https://open.feishu.cn/open-apis/auth/v3/tenant_access_token/internal/"
-    post_data = {"app_id":feishu_cfg.feishu_app_id,
-                "app_secret":feishu_cfg.feishu_app_secret}
-    r = requests.post(feishu_url, data=post_data)
-    tat = r.json()["tenant_access_token"]
-    header = {"content-type":"application/json",
-    "Authorization":"Bearer " + str(tat)}
-    url = "https://open.feishu.cn/open-apis/bitable/v1/apps/" + sheet_address[0] + "/tables/" + sheet_address[1] + '/records'\
-        + "?valueRenderOption=ToString&dateTimeRenderOption=FormattedString"
-    r = requests.get(url, headers = header)
-    pull_data = r.json()['data']['items']
-    pull_data_parse = [x['fields'] for x in pull_data]
+import json
+import requests
+import pandas as pd
+
+def fs_read_df(sheet_address, feishu_cfg):
+    # 获取tenant_access_token
+    feishu_url = "https://open.feishu.cn/open-apis/auth/v3/tenant_access_token/internal/"
+    post_data = {"app_id":feishu_cfg.feishu_app_id,
+                "app_secret":feishu_cfg.feishu_app_secret}
+    r = requests.post(feishu_url, data=post_data)
+    tat = r.json()["tenant_access_token"]
+    header = {"content-type":"application/json",
+    "Authorization":"Bearer " + str(tat)}
+    url = "https://open.feishu.cn/open-apis/sheets/v2/spreadsheets/" + sheet_address[0] + "/values/" + sheet_address[1] \
+        + "?valueRenderOption=ToString&dateTimeRenderOption=FormattedString"
+    r = requests.get(url, headers = header)
+    pull_data = r.json()['data']['valueRange']['values']
+    return pd.DataFrame(pull_data[1:], columns=pull_data[0])
+
+def fs_read_base(sheet_address, feishu_cfg):
+    # 获取tenant_access_token
+    feishu_url = "https://open.feishu.cn/open-apis/auth/v3/tenant_access_token/internal/"
+    post_data = {"app_id":feishu_cfg.feishu_app_id,
+                "app_secret":feishu_cfg.feishu_app_secret}
+    r = requests.post(feishu_url, data=post_data)
+    tat = r.json()["tenant_access_token"]
+    header = {"content-type":"application/json",
+    "Authorization":"Bearer " + str(tat)}
+    url = "https://open.feishu.cn/open-apis/bitable/v1/apps/" + sheet_address[0] + "/tables/" + sheet_address[1] + '/records'\
+        + "?valueRenderOption=ToString&dateTimeRenderOption=FormattedString"
+    r = requests.get(url, headers = header)
+    pull_data = r.json()['data']['items']
+    pull_data_parse = [x['fields'] for x in pull_data]
     return pd.DataFrame(pull_data_parse)
```

### Comparing `tablemaster-1.2.1/tablemaster/local.py` & `tablemaster-1.2.2/tablemaster/local.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,94 +1,94 @@
-import pandas as pd
-import pathlib
-from pathlib import Path
-
-def detect_header_read_csv(path, det_rows=10):
-    df = pd.read_csv(path)
-    l_unname = len([x for x in df.columns if 'Unnamed' in x])
-    if l_unname>1:
-        for i in range(det_rows):
-            df = pd.read_csv(path, header=i+1)
-            if(len([x for x in df.columns if 'Unnamed' in x])==0):
-                break
-    return df
-    
-def detect_header_read_excel(path, det_rows=10):
-    df = pd.read_excel(path)
-    l_unname = len([x for x in df.columns if 'Unnamed' in x])
-    if l_unname>1:
-        for i in range(det_rows):
-            df = pd.read_excel(path, header=i+1)
-            if(len([x for x in df.columns if 'Unnamed' in x])==0):
-                break
-    return df
-
-def equal_table(df1, df2, det_col='nan'):
-    if(len(df1) != len(df2)):
-        return False
-    elif df1.equals(df2):
-        return True
-    else:
-        if det_col == 'nan':
-            return False
-        else:
-            return all(df1[det_col].fillna("").sort_values().reset_index(drop=True).fillna(0) == df2[det_col].fillna("").sort_values().reset_index(drop=True))
-
-def read(file, det_header=True):
-    if isinstance(file, pathlib.PosixPath):
-        file = str(file)
-    file_detect = list(Path().glob(file))
-    file_detect = [i for i in file_detect if (str(i)[0]!="." or str(i)[:3]=="../")]
-    if len(file_detect)>1:
-        print(f'There are more 1 file detected, please specify the file name! \n {file_detect}')
-        return "error"
-    else:
-        file_path = file_detect[0]
-        if file_path.suffix[:3] == '.xl':
-            try:
-                if det_header == True:
-                    df = detect_header_read_excel(file_path)
-                else:
-                    df = pd.read_excel(file_path)
-            except Exception as e:
-                print(e)
-        elif file_path.suffix[:4] == '.csv':
-            try:
-                if det_header == True:
-                    df = detect_header_read_csv(file_path)
-                else:
-                    df = pd.read_csv(file_path)
-            except Exception as e:
-                print(e)
-        else:
-            raise Exception(f'unsupported file type: {file_path.suffix}')
-        return df
-
-def batch_read(file, det_col='nan'):
-    path_list = list(Path().glob(file))
-    print(f'below {len(path_list)} file found: {path_list}')
-    dataframes = []
-    for i, file in enumerate(path_list):
-        df = read(file)
-        dataframes.append(df)
-
-    unique_dataframes = []
-    for df in dataframes:
-        if not any(equal_table(df, existing_df, det_col) for existing_df in unique_dataframes):
-            unique_dataframes.append(df)
-    print(f'{len(unique_dataframes)}  unique files found!')
-    return pd.concat(unique_dataframes).reset_index(drop=True)
-
-
-def read_dfs(file, det_col='nan'):
-    path_list = list(Path().glob(file))
-    print(f'below {len(path_list)} file found: {path_list}')
-    dataframes = []
-    for i, file in enumerate(path_list):
-        df = read(file)
-        dataframes.append(df)
-    unique_dataframes = []
-    for df in dataframes:
-        if not any(equal_table(df, existing_df, det_col) for existing_df in unique_dataframes):
-            unique_dataframes.append(df)
-    print(f'{len(unique_dataframes)}  unique files found!')
+import pandas as pd
+import pathlib
+from pathlib import Path
+
+def detect_header_read_csv(path, det_rows=10):
+    df = pd.read_csv(path)
+    l_unname = len([x for x in df.columns if 'Unnamed' in x])
+    if l_unname>1:
+        for i in range(det_rows):
+            df = pd.read_csv(path, header=i+1)
+            if(len([x for x in df.columns if 'Unnamed' in x])==0):
+                break
+    return df
+    
+def detect_header_read_excel(path, det_rows=10):
+    df = pd.read_excel(path)
+    l_unname = len([x for x in df.columns if 'Unnamed' in x])
+    if l_unname>1:
+        for i in range(det_rows):
+            df = pd.read_excel(path, header=i+1)
+            if(len([x for x in df.columns if 'Unnamed' in x])==0):
+                break
+    return df
+
+def equal_table(df1, df2, det_col='nan'):
+    if(len(df1) != len(df2)):
+        return False
+    elif df1.equals(df2):
+        return True
+    else:
+        if det_col == 'nan':
+            return False
+        else:
+            return all(df1[det_col].fillna("").sort_values().reset_index(drop=True).fillna(0) == df2[det_col].fillna("").sort_values().reset_index(drop=True))
+
+def read(file, det_header=True):
+    if isinstance(file, pathlib.PosixPath):
+        file = str(file)
+    file_detect = list(Path().glob(file))
+    file_detect = [i for i in file_detect if (str(i)[0]!="." or str(i)[:3]=="../")]
+    if len(file_detect)>1:
+        print(f'There are more 1 file detected, please specify the file name! \n {file_detect}')
+        return "error"
+    else:
+        file_path = file_detect[0]
+        if file_path.suffix[:3] == '.xl':
+            try:
+                if det_header == True:
+                    df = detect_header_read_excel(file_path)
+                else:
+                    df = pd.read_excel(file_path)
+            except Exception as e:
+                print(e)
+        elif file_path.suffix[:4] == '.csv':
+            try:
+                if det_header == True:
+                    df = detect_header_read_csv(file_path)
+                else:
+                    df = pd.read_csv(file_path)
+            except Exception as e:
+                print(e)
+        else:
+            raise Exception(f'unsupported file type: {file_path.suffix}')
+        return df
+
+def batch_read(file, det_col='nan'):
+    path_list = list(Path().glob(file))
+    print(f'below {len(path_list)} file found: {path_list}')
+    dataframes = []
+    for i, file in enumerate(path_list):
+        df = read(file)
+        dataframes.append(df)
+
+    unique_dataframes = []
+    for df in dataframes:
+        if not any(equal_table(df, existing_df, det_col) for existing_df in unique_dataframes):
+            unique_dataframes.append(df)
+    print(f'{len(unique_dataframes)}  unique files found!')
+    return pd.concat(unique_dataframes).reset_index(drop=True)
+
+
+def read_dfs(file, det_col='nan'):
+    path_list = list(Path().glob(file))
+    print(f'below {len(path_list)} file found: {path_list}')
+    dataframes = []
+    for i, file in enumerate(path_list):
+        df = read(file)
+        dataframes.append(df)
+    unique_dataframes = []
+    for df in dataframes:
+        if not any(equal_table(df, existing_df, det_col) for existing_df in unique_dataframes):
+            unique_dataframes.append(df)
+    print(f'{len(unique_dataframes)}  unique files found!')
     return unique_dataframes
```

### Comparing `tablemaster-1.2.1/tablemaster/mysql.py` & `tablemaster-1.2.2/tablemaster/mysql.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,142 +1,143 @@
-
-from sqlalchemy import create_engine, text
-import pandas as pd
-from datetime import datetime
-from tqdm import tqdm
-
-
-#query function
-def query(sql, configs):
-    try:
-        cf_port = configs.port
-    except:
-        cf_port = 3306
-    print(f'try to connect to {configs.name}...')
-    engine = create_engine(f'mysql+pymysql://{configs.user}:{configs.password}@{configs.host}:{cf_port}/{configs.database}')
-    df = pd.read_sql(sql, engine)
-    print(df.head())
-    return df
-
-#opt function
-def opt(sql, configs):
-    try:
-        cf_port = configs.port
-    except:
-        cf_port = 3306
-    print(f'try to connect to {configs.name}...')
-    engine = create_engine(f'mysql+pymysql://{configs.user}:{configs.password}@{configs.host}:{cf_port}/{configs.database}')
-    # Connect to the database using the engine's connect method
-    with engine.connect() as conn:
-        # Execute the SQL statement directly, without using pandas
-        conn.execute(text(sql))
-    print('mysql execute success!')
-
-class ManageTable:
-    def __init__(self, table, configs):
-        try:
-            self.port = configs.port
-        except:
-            self.port = 3306
-        self.table = table
-        self.name = configs.name
-        self.user = configs.user
-        self.password = configs.password
-        self.host = configs.host
-        self.database = configs.database
-        try:
-            query(sql = f"SELECT * FROM {self.table} LIMIT 1", configs=configs)
-            print("table exist!")
-        except:
-            print("table not found!")
-
-    def delete_table(self):
-        opt(f'DROP TABLE {self.table}', self)
-        print(f'{self.table} deleted!')
-
-    def par_del(self, clause):
-        del_clause = f"DELETE FROM {self.table} WHERE {clause}"
-        opt(del_clause, self)
-        print(f'records of table that {clause} are deleted!')
-
-    def change_data_type(self, cols_name, data_type):
-        change_clause = f'ALTER TABLE {self.table} MODIFY COLUMN {cols_name} {data_type}'
-        opt(change_clause, self)
-        print(f'{cols_name} changed to {data_type} successfully!')
-
-
-    def upload_data(self, df, chunk_size=10000, add_date=False):
-        db_url = f'mysql+pymysql://{self.user}:{self.password}@{self.host}:{self.port}/{self.database}'
-        with create_engine(db_url).begin() as connection:
-            # Add a 'rundate' column with the current date formatted as 'YYYY-MM-DD' if required
-            if add_date:
-                df_copy = df.copy()
-                df_copy['rundate'] = datetime.now().strftime('%Y-%m-%d')
-            else:
-                df_copy = df
-            total_chunks = (len(df_copy) // chunk_size) + (0 if len(df_copy) % chunk_size == 0 else 1)
-            print(f'try to upload data now, chunk_size is {chunk_size}')
-            with tqdm(total=total_chunks, desc="Uploading Chunks", unit="chunk") as pbar:
-                try:
-                    for start in range(0, len(df_copy), chunk_size):
-                        end = min(start + chunk_size, len(df_copy))
-                        chunk = df_copy.iloc[start:end]
-                        chunk.to_sql(name=self.table, con=connection, if_exists='append', index=False)
-                        pbar.update(1)
-                except Exception as e:
-                    print(f"An error occurred: {e}")
-
-# Old ManageTable Way
-class Manage_table:
-    def __init__(self, table, configs):
-        print('We recommend using ManageTable for MySQL table management instead of Manage_table. e.g. tb=ManageTable(...)')
-        try:
-            self.port = configs.port
-        except:
-            self.port = 3306
-        self.table = table
-        self.name = configs.name
-        self.user = configs.user
-        self.password = configs.password
-        self.host = configs.host
-        self.database = configs.database
-        try:
-            query(sql = f"SELECT * FROM {self.table} LIMIT 1", configs=configs)
-            print("table exist!")
-        except:
-            print("table not found!")
-
-    def delete_table(self):
-        opt(f'DROP TABLE {self.table}', self)
-        print(f'{self.table} deleted!')
-
-    def par_del(self, clause):
-        del_clause = f"DELETE FROM {self.table} WHERE {clause}"
-        opt(del_clause, self)
-        print(f'records of table that {clause} are deleted!')
-
-    def change_data_type(self, cols_name, data_type):
-        change_clause = f'ALTER TABLE {self.table} MODIFY COLUMN {cols_name} {data_type}'
-        opt(change_clause, self)
-        print(f'{cols_name} changed to {data_type} successfully!')
-
-
-    def upload_data(self, df, chunk_size=10000, add_date=True):
-        db_url = f'mysql+pymysql://{self.user}:{self.password}@{self.host}:{self.port}/{self.database}'
-        with create_engine(db_url).begin() as connection:
-            # Add a 'rundate' column with the current date formatted as 'YYYY-MM-DD' if required
-            if add_date:
-                df_copy = df.copy()
-                df_copy['rundate'] = datetime.now().strftime('%Y-%m-%d')
-            else:
-                df_copy = df
-            total_chunks = (len(df_copy) // chunk_size) + (0 if len(df_copy) % chunk_size == 0 else 1)
-            print(f'try to upload data now, chunk_size is {chunk_size}')
-            with tqdm(total=total_chunks, desc="Uploading Chunks", unit="chunk") as pbar:
-                try:
-                    for start in range(0, len(df_copy), chunk_size):
-                        end = min(start + chunk_size, len(df_copy))
-                        chunk = df_copy.iloc[start:end]
-                        chunk.to_sql(name=self.table, con=connection, if_exists='append', index=False)
-                        pbar.update(1)
-                except Exception as e:
+
+from sqlalchemy import create_engine, text
+import pandas as pd
+from datetime import datetime
+from tqdm import tqdm
+
+
+#query function
+def query(sql, configs):
+    try:
+        cf_port = configs.port
+    except:
+        cf_port = 3306
+    print(f'try to connect to {configs.name}...')
+    engine = create_engine(f'mysql+pymysql://{configs.user}:{configs.password}@{configs.host}:{cf_port}/{configs.database}')
+    df = pd.read_sql(sql, engine)
+    print(df.head())
+    return df
+
+#opt function
+def opt(sql, configs):
+    try:
+        cf_port = configs.port
+    except:
+        cf_port = 3306
+    print(f'try to connect to {configs.name}...')
+    engine = create_engine(f'mysql+pymysql://{configs.user}:{configs.password}@{configs.host}:{cf_port}/{configs.database}',
+                           isolation_level="AUTOCOMMIT")
+    # Connect to the database using the engine's connect method
+    with engine.connect() as conn:
+        # Execute the SQL statement directly, without using pandas
+        conn.execute(text(sql))
+    print('mysql execute success!')
+
+class ManageTable:
+    def __init__(self, table, configs):
+        try:
+            self.port = configs.port
+        except:
+            self.port = 3306
+        self.table = table
+        self.name = configs.name
+        self.user = configs.user
+        self.password = configs.password
+        self.host = configs.host
+        self.database = configs.database
+        try:
+            query(sql = f"SELECT * FROM {self.table} LIMIT 1", configs=configs)
+            print("table exist!")
+        except:
+            print("table not found!")
+
+    def delete_table(self):
+        opt(f'DROP TABLE {self.table}', self)
+        print(f'{self.table} deleted!')
+
+    def par_del(self, clause):
+        del_clause = f"DELETE FROM {self.table} WHERE {clause}"
+        opt(del_clause, self)
+        print(f'records of table that {clause} are deleted!')
+
+    def change_data_type(self, cols_name, data_type):
+        change_clause = f'ALTER TABLE {self.table} MODIFY COLUMN {cols_name} {data_type}'
+        opt(change_clause, self)
+        print(f'{cols_name} changed to {data_type} successfully!')
+
+
+    def upload_data(self, df, chunk_size=10000, add_date=False):
+        db_url = f'mysql+pymysql://{self.user}:{self.password}@{self.host}:{self.port}/{self.database}'
+        with create_engine(db_url).begin() as connection:
+            # Add a 'rundate' column with the current date formatted as 'YYYY-MM-DD' if required
+            if add_date:
+                df_copy = df.copy()
+                df_copy['rundate'] = datetime.now().strftime('%Y-%m-%d')
+            else:
+                df_copy = df
+            total_chunks = (len(df_copy) // chunk_size) + (0 if len(df_copy) % chunk_size == 0 else 1)
+            print(f'try to upload data now, chunk_size is {chunk_size}')
+            with tqdm(total=total_chunks, desc="Uploading Chunks", unit="chunk") as pbar:
+                try:
+                    for start in range(0, len(df_copy), chunk_size):
+                        end = min(start + chunk_size, len(df_copy))
+                        chunk = df_copy.iloc[start:end]
+                        chunk.to_sql(name=self.table, con=connection, if_exists='append', index=False)
+                        pbar.update(1)
+                except Exception as e:
+                    print(f"An error occurred: {e}")
+
+# Old ManageTable Way
+class Manage_table:
+    def __init__(self, table, configs):
+        print('We recommend using ManageTable for MySQL table management instead of Manage_table. e.g. tb=ManageTable(...)')
+        try:
+            self.port = configs.port
+        except:
+            self.port = 3306
+        self.table = table
+        self.name = configs.name
+        self.user = configs.user
+        self.password = configs.password
+        self.host = configs.host
+        self.database = configs.database
+        try:
+            query(sql = f"SELECT * FROM {self.table} LIMIT 1", configs=configs)
+            print("table exist!")
+        except:
+            print("table not found!")
+
+    def delete_table(self):
+        opt(f'DROP TABLE {self.table}', self)
+        print(f'{self.table} deleted!')
+
+    def par_del(self, clause):
+        del_clause = f"DELETE FROM {self.table} WHERE {clause}"
+        opt(del_clause, self)
+        print(f'records of table that {clause} are deleted!')
+
+    def change_data_type(self, cols_name, data_type):
+        change_clause = f'ALTER TABLE {self.table} MODIFY COLUMN {cols_name} {data_type}'
+        opt(change_clause, self)
+        print(f'{cols_name} changed to {data_type} successfully!')
+
+
+    def upload_data(self, df, chunk_size=10000, add_date=True):
+        db_url = f'mysql+pymysql://{self.user}:{self.password}@{self.host}:{self.port}/{self.database}'
+        with create_engine(db_url).begin() as connection:
+            # Add a 'rundate' column with the current date formatted as 'YYYY-MM-DD' if required
+            if add_date:
+                df_copy = df.copy()
+                df_copy['rundate'] = datetime.now().strftime('%Y-%m-%d')
+            else:
+                df_copy = df
+            total_chunks = (len(df_copy) // chunk_size) + (0 if len(df_copy) % chunk_size == 0 else 1)
+            print(f'try to upload data now, chunk_size is {chunk_size}')
+            with tqdm(total=total_chunks, desc="Uploading Chunks", unit="chunk") as pbar:
+                try:
+                    for start in range(0, len(df_copy), chunk_size):
+                        end = min(start + chunk_size, len(df_copy))
+                        chunk = df_copy.iloc[start:end]
+                        chunk.to_sql(name=self.table, con=connection, if_exists='append', index=False)
+                        pbar.update(1)
+                except Exception as e:
                     print(f"An error occurred: {e}")
```

### Comparing `tablemaster-1.2.1/tablemaster/utils.py` & `tablemaster-1.2.2/tablemaster/utils.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from datetime import datetime
-from datetime import timedelta
-from dateutil.relativedelta import relativedelta
-
-def gen_month_list(month_start, month_end):
-    l = []
-    while datetime.strptime(month_start, '%Y-%m') <= datetime.strptime(month_end, '%Y-%m'):
-        l.append(month_start)
-        month_start = datetime.strftime(datetime.strptime(month_start, '%Y-%m')+ relativedelta(months=1), '%Y-%m')
-    return l
-
-def gen_day_list(day_start, day_end='now'):
-    if day_end == 'now':
-        day_end = datetime.strftime(datetime.now(), '%Y-%m-%d')
-    l = []
-    while datetime.strptime(day_start, '%Y-%m-%d') <= datetime.strptime(day_end, '%Y-%m-%d'):
-        l.append(day_start)
-        day_start = datetime.strftime(datetime.strptime(day_start, '%Y-%m-%d')+ relativedelta(days=1), '%Y-%m-%d')
+from datetime import datetime
+from datetime import timedelta
+from dateutil.relativedelta import relativedelta
+
+def gen_month_list(month_start, month_end):
+    l = []
+    while datetime.strptime(month_start, '%Y-%m') <= datetime.strptime(month_end, '%Y-%m'):
+        l.append(month_start)
+        month_start = datetime.strftime(datetime.strptime(month_start, '%Y-%m')+ relativedelta(months=1), '%Y-%m')
+    return l
+
+def gen_day_list(day_start, day_end='now'):
+    if day_end == 'now':
+        day_end = datetime.strftime(datetime.now(), '%Y-%m-%d')
+    l = []
+    while datetime.strptime(day_start, '%Y-%m-%d') <= datetime.strptime(day_end, '%Y-%m-%d'):
+        l.append(day_start)
+        day_start = datetime.strftime(datetime.strptime(day_start, '%Y-%m-%d')+ relativedelta(days=1), '%Y-%m-%d')
     return l
```

