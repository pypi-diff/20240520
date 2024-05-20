# Comparing `tmp/chemfusekit-1.1.0b1.tar.gz` & `tmp/chemfusekit-1.1.0b2.tar.gz`

## Comparing `chemfusekit-1.1.0b1.tar` & `chemfusekit-1.1.0b2.tar`

### file list

```diff
@@ -1,125 +1,133 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/.python-version
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/.releaserc.yml
--rw-r--r--   0        0        0     6689 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/CHANGELOG.md
--rw-r--r--   0        0        0     5231 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/cda_example_notebook.ipynb
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/requirements-dev.lock
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/requirements.lock
--rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/.github/workflows/gh_pages.yml
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/.github/workflows/pylint.yml
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/.github/workflows/release.yml
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/.github/workflows/unittest.yml
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/chemfusekit/__init__.py
--rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/chemfusekit/knn.py
--rw-r--r--   0        0        0     5048 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/chemfusekit/lda.py
--rw-r--r--   0        0        0     4817 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/chemfusekit/lldf.py
--rw-r--r--   0        0        0     7562 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/chemfusekit/lr.py
--rw-r--r--   0        0        0     8825 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/chemfusekit/pca.py
--rw-r--r--   0        0        0     6863 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/chemfusekit/plsda.py
--rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/chemfusekit/svm.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/docs/README.md
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/docs/babel.config.js
--rw-r--r--   0        0        0     4025 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/docs/docusaurus.config.js
--rw-r--r--   0        0        0  1020872 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/docs/package-lock.json
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/docs/package.json
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/docs/sidebars.js
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/docs/docs/complete-workflow.md
--rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/docs/docs/tutorial.md
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/docs/docs/knn/_category_.json
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/docs/docs/knn/knn.md
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/docs/docs/knn/knnsettings.md
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/docs/docs/lda/_category_.json
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/docs/docs/lda/lda.md
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/docs/docs/lda/ldasettings.md
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/docs/docs/lldf/_category_.json
--rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/docs/docs/lldf/lldf.md
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/docs/docs/lldf/lldfmodel.md
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/docs/docs/lldf/lldfsettings.md
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/docs/docs/lr/_category_.json
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/docs/docs/lr/lr.md
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/docs/docs/lr/lrsettings.md
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/docs/docs/pca/_category_.json
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/docs/docs/pca/pca.md
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/docs/docs/pca/pcasettings.md
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/docs/docs/plsda/_category_.json
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/docs/docs/plsda/plsda.md
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/docs/docs/plsda/plsdasettings.md
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/docs/docs/svm/_category_.json
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/docs/docs/svm/svm.md
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/docs/docs/svm/svmsettings.md
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/docs/src/components/HomepageFeatures/index.js
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/docs/src/components/HomepageFeatures/styles.module.css
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/docs/src/css/custom.css
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/docs/src/pages/index.js
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/docs/src/pages/index.module.css
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/docs/src/pages/project.md
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/docs/src/pages/project/continuous-integration.md
--rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/docs/src/pages/project/process-model.md
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/docs/src/pages/project/project-philosophy.md
--rw-r--r--   0        0        0    10945 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/docs/src/pages/project/project-plan.md
--rw-r--r--   0        0        0     4767 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/docs/src/pages/project/requirements-specification.md
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/docs/src/pages/project/use-cases.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/docs/static/.nojekyll
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/docs/static/img/colab-logo.svg
--rw-r--r--   0        0        0    55746 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/docs/static/img/docusaurus-social-card.jpg
--rw-r--r--   0        0        0    10723 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/docs/static/img/docusaurus.png
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/docs/static/img/favicon.ico
--rw-r--r--   0        0        0    23978 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/docs/static/img/happy-woman.svg
--rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/docs/static/img/logo.svg
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/docs/static/img/magnifying-glass.svg
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/notes/Beartype.md
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/notes/Constructors.md
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/notes/Conventional Commits.md
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/notes/Kanban.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/notes/Logistic Regression.md
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/notes/PCA-LR.md
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/notes/PCA.md
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/notes/PEP coding standards.md
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/notes/SVM.md
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/notes/To do.md
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/notes/Use Case Diagram.md
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/notes/kNN.md
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/notes/.obsidian/app.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/notes/.obsidian/appearance.json
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/notes/.obsidian/community-plugins.json
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/notes/.obsidian/core-plugins-migration.json
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/notes/.obsidian/core-plugins.json
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/notes/.obsidian/daily-notes.json
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/notes/.obsidian/templates.json
--rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/notes/.obsidian/workspace.json
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/notes/.obsidian/plugins/calendar/data.json
--rw-r--r--   0        0        0   141498 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/notes/.obsidian/plugins/calendar/main.js
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/notes/.obsidian/plugins/calendar/manifest.json
--rw-r--r--   0        0        0   723669 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/notes/.obsidian/plugins/obsidian-kanban/main.js
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/notes/.obsidian/plugins/obsidian-kanban/manifest.json
--rw-r--r--   0        0        0    53515 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/notes/.obsidian/plugins/obsidian-kanban/styles.css
--rw-r--r--   0        0        0   294758 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/notes/.obsidian/plugins/obsidian-plantuml/main.js
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/notes/.obsidian/plugins/obsidian-plantuml/manifest.json
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/notes/.obsidian/plugins/obsidian-plantuml/styles.css
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/notes/Devlog/2024-04-19.md
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/notes/Devlog/2024-04-20.md
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/notes/Devlog/2024-04-22.md
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/notes/Devlog/2024-04-23.md
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/notes/Devlog/2024-05-06.md
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/notes/Devlog/2024-05-07.md
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/notes/Devlog/2024-05-08.md
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/notes/Devlog/2024-05-09.md
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/notes/Devlog/2024-05-17.md
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/notes/Devlog/2024-05-18.md
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/notes/Templates/Daily devlog.md
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/notes/UML/Components.md
--rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/notes/UML/Process state machine.md
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/notes/UML/Sequence.md
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/notes/UML/Use cases.md
--rw-r--r--   0        0        0   590311 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/tests/qepas.xlsx
--rw-r--r--   0        0        0    18770 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/tests/rt.xlsx
--rw-r--r--   0        0        0     5070 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/tests/test_knn.py
--rw-r--r--   0        0        0     3315 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/tests/test_lda.py
--rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/tests/test_lldf.py
--rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/tests/test_lr.py
--rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/tests/test_pca.py
--rw-r--r--   0        0        0     3833 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/tests/test_plsda.py
--rw-r--r--   0        0        0     3685 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/tests/test_svm.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/.gitignore
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/pyproject.toml
--rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/readme.md
--rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b1/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/.python-version
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/.releaserc.yml
+-rw-r--r--   0        0        0     7404 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/CHANGELOG.md
+-rw-r--r--   0        0        0     5231 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/cda_example_notebook.ipynb
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/requirements-dev.lock
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/requirements.lock
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/.github/workflows/gh_pages.yml
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/.github/workflows/release.yml
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/.github/workflows/thesis.yml
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/.github/workflows/unittest.yml
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/chemfusekit/__init__.py
+-rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/chemfusekit/__utils.py
+-rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/chemfusekit/knn.py
+-rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/chemfusekit/lda.py
+-rw-r--r--   0        0        0     4958 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/chemfusekit/lldf.py
+-rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/chemfusekit/lr.py
+-rw-r--r--   0        0        0     8825 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/chemfusekit/pca.py
+-rw-r--r--   0        0        0     4842 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/chemfusekit/plsda.py
+-rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/chemfusekit/svm.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/docs/README.md
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/docs/babel.config.js
+-rw-r--r--   0        0        0     4025 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/docs/docusaurus.config.js
+-rw-r--r--   0        0        0  1020872 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/docs/package-lock.json
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/docs/package.json
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/docs/sidebars.js
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/docs/docs/complete-workflow.md
+-rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/docs/docs/tutorial.md
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/docs/docs/knn/_category_.json
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/docs/docs/knn/knn.md
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/docs/docs/knn/knnsettings.md
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/docs/docs/lda/_category_.json
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/docs/docs/lda/lda.md
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/docs/docs/lda/ldasettings.md
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/docs/docs/lldf/_category_.json
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/docs/docs/lldf/lldf.md
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/docs/docs/lldf/lldfmodel.md
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/docs/docs/lldf/lldfsettings.md
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/docs/docs/lr/_category_.json
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/docs/docs/lr/lr.md
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/docs/docs/lr/lrsettings.md
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/docs/docs/pca/_category_.json
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/docs/docs/pca/pca.md
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/docs/docs/pca/pcasettings.md
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/docs/docs/plsda/_category_.json
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/docs/docs/plsda/plsda.md
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/docs/docs/plsda/plsdasettings.md
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/docs/docs/svm/_category_.json
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/docs/docs/svm/svm.md
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/docs/docs/svm/svmsettings.md
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/docs/src/components/HomepageFeatures/index.js
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/docs/src/components/HomepageFeatures/styles.module.css
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/docs/src/css/custom.css
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/docs/src/pages/index.js
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/docs/src/pages/index.module.css
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/docs/src/pages/project.md
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/docs/src/pages/project/continuous-integration.md
+-rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/docs/src/pages/project/process-model.md
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/docs/src/pages/project/project-philosophy.md
+-rw-r--r--   0        0        0    10945 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/docs/src/pages/project/project-plan.md
+-rw-r--r--   0        0        0     4767 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/docs/src/pages/project/requirements-specification.md
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/docs/src/pages/project/use-cases.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/docs/static/.nojekyll
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/docs/static/img/colab-logo.svg
+-rw-r--r--   0        0        0    55746 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/docs/static/img/docusaurus-social-card.jpg
+-rw-r--r--   0        0        0    10723 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/docs/static/img/docusaurus.png
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/docs/static/img/favicon.ico
+-rw-r--r--   0        0        0    23978 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/docs/static/img/happy-woman.svg
+-rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/docs/static/img/logo.svg
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/docs/static/img/magnifying-glass.svg
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/notes/Beartype.md
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/notes/Constructors.md
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/notes/Conventional Commits.md
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/notes/Kanban.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/notes/Logistic Regression.md
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/notes/PCA-LR.md
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/notes/PCA.md
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/notes/PEP coding standards.md
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/notes/SVM.md
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/notes/To do.md
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/notes/Use Case Diagram.md
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/notes/kNN.md
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/notes/.obsidian/app.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/notes/.obsidian/appearance.json
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/notes/.obsidian/community-plugins.json
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/notes/.obsidian/core-plugins-migration.json
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/notes/.obsidian/core-plugins.json
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/notes/.obsidian/daily-notes.json
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/notes/.obsidian/templates.json
+-rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/notes/.obsidian/workspace.json
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/notes/.obsidian/plugins/calendar/data.json
+-rw-r--r--   0        0        0   141498 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/notes/.obsidian/plugins/calendar/main.js
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/notes/.obsidian/plugins/calendar/manifest.json
+-rw-r--r--   0        0        0   723669 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/notes/.obsidian/plugins/obsidian-kanban/main.js
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/notes/.obsidian/plugins/obsidian-kanban/manifest.json
+-rw-r--r--   0        0        0    53515 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/notes/.obsidian/plugins/obsidian-kanban/styles.css
+-rw-r--r--   0        0        0   294758 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/notes/.obsidian/plugins/obsidian-plantuml/main.js
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/notes/.obsidian/plugins/obsidian-plantuml/manifest.json
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/notes/.obsidian/plugins/obsidian-plantuml/styles.css
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/notes/Devlog/2024-04-19.md
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/notes/Devlog/2024-04-20.md
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/notes/Devlog/2024-04-22.md
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/notes/Devlog/2024-04-23.md
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/notes/Devlog/2024-05-06.md
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/notes/Devlog/2024-05-07.md
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/notes/Devlog/2024-05-08.md
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/notes/Devlog/2024-05-09.md
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/notes/Devlog/2024-05-17.md
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/notes/Devlog/2024-05-18.md
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/notes/Templates/Daily devlog.md
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/notes/UML/Components.md
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/notes/UML/Process state machine.md
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/notes/UML/Sequence.md
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/notes/UML/Use cases.md
+-rw-r--r--   0        0        0   590311 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/tests/qepas.xlsx
+-rw-r--r--   0        0        0    18770 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/tests/rt.xlsx
+-rw-r--r--   0        0        0     5220 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/tests/test_knn.py
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/tests/test_lda.py
+-rw-r--r--   0        0        0     2631 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/tests/test_lldf.py
+-rw-r--r--   0        0        0     3945 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/tests/test_lr.py
+-rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/tests/test_pca.py
+-rw-r--r--   0        0        0     4039 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/tests/test_plsda.py
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/tests/test_svm.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/thesis/0-header.md
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/thesis/1-abstract.md
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/thesis/2-index.md.md
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/thesis/3-intro.md
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/thesis/999-ringraziamenti.md
+-rw-r--r--   0        0        0    21285 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/thesis/logo-unibg.png
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/.gitignore
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/pyproject.toml
+-rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/readme.md
+-rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b2/PKG-INFO
```

### Comparing `chemfusekit-1.1.0b1/.releaserc.yml` & `chemfusekit-1.1.0b2/.releaserc.yml`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/CHANGELOG.md` & `chemfusekit-1.1.0b2/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+## [1.1.0-beta.2](https://github.com/f-aguzzi/tesi/compare/v1.1.0-beta.1...v1.1.0-beta.2) (2024-05-20)
+
+
+### Bug Fixes
+
+* add missing checks to LLDFSettings ([3d57752](https://github.com/f-aguzzi/tesi/commit/3d577527eefd0b183a66c378d53cb1f1ee506343)), closes [#20](https://github.com/f-aguzzi/tesi/issues/20)
+
+
+### chore
+
+* **thesis:** set up build system (merge from [#22](https://github.com/f-aguzzi/tesi/issues/22)) ([0b13ed3](https://github.com/f-aguzzi/tesi/commit/0b13ed346448f0eeefecbc6fd051eb7c98919650))
+
+
+### Refactor
+
+* extract split tests and graphs (merge [#23](https://github.com/f-aguzzi/tesi/issues/23)) ([6865c88](https://github.com/f-aguzzi/tesi/commit/6865c88d70b650de5e8440807b0194022a15dc0e))
+
 ## [1.1.0-beta.1](https://github.com/f-aguzzi/tesi/compare/v1.0.0...v1.1.0-beta.1) (2024-05-18)
 
 
 ### Features
 
 * beartype integration ([2f823ce](https://github.com/f-aguzzi/tesi/commit/2f823cebee0cb8006523d9e0d6aaa673484bd928)), closes [#7](https://github.com/f-aguzzi/tesi/issues/7)
```

### Comparing `chemfusekit-1.1.0b1/cda_example_notebook.ipynb` & `chemfusekit-1.1.0b2/cda_example_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/requirements-dev.lock` & `chemfusekit-1.1.0b2/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/requirements.lock` & `chemfusekit-1.1.0b2/requirements.lock`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/.github/workflows/gh_pages.yml` & `chemfusekit-1.1.0b2/.github/workflows/gh_pages.yml`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/.github/workflows/pylint.yml` & `chemfusekit-1.1.0b2/.github/workflows/pylint.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 name: Linting
 on:
   push:
       paths:
         - 'colab_datafusion_analysis/**'
-        - '.github/workflows/**'
+        - '.github/workflows/pylint.yml'
 
 jobs:
   build:
     runs-on: ubuntu-latest
     steps:
       - name: Checkout code
         uses: actions/checkout@v3
```

### Comparing `chemfusekit-1.1.0b1/.github/workflows/release.yml` & `chemfusekit-1.1.0b2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/.github/workflows/unittest.yml` & `chemfusekit-1.1.0b2/.github/workflows/unittest.yml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 name: Unit Tests
 on:
   push:
       paths:
         - 'colab_datafusion_analysis/**'
         - 'tests/**'
-        - '.github/workflows/**'
+        - '.github/workflows/unittest.yml'
 
 jobs:
   build:
     runs-on: ubuntu-latest
     steps:
       - name: Checkout code
         uses: actions/checkout@v3
```

### Comparing `chemfusekit-1.1.0b1/chemfusekit/lda.py` & `chemfusekit-1.1.0b2/chemfusekit/plsda.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,143 +1,123 @@
-'''Linear Discriminant Analysis module'''
+'''Partial Least Squares Discriminant Analysis module.'''
 from typing import Optional
 
-import numpy as np
 import pandas as pd
-
-from sklearn.discriminant_analysis import LinearDiscriminantAnalysis as LD
-from sklearn.model_selection import train_test_split
-
-from sklearn.metrics import confusion_matrix, classification_report
+import numpy as np
 
 import plotly.express as px
-import seaborn as sns
-import matplotlib.pyplot as plt
+
+from sklearn.cross_decomposition import PLSRegression as PLSR
 
 from chemfusekit.lldf import LLDFModel
+from chemfusekit.__utils import print_confusion_matrix, run_split_test
+
 
-class LDASettings:
-    '''Holds the settings for the LDA object.'''
-    def __init__(self, components: int = 3, output: bool = False):
-        if components <= 2:
-            raise ValueError("Invalid component number: must be a > 1 integer.")
-        self.components = components
+class PLSDASettings:
+    '''Holds the settings for the PLSDA object.'''
+    def __init__(self, n_components: int = 3, output: bool = False, test_split: bool = False):
+        if n_components < 1:
+            raise ValueError("Invalid n_components number: should be a positive integer.")
+        if test_split is True and output is False:
+            raise Warning(
+                "You selected test_split but it won't run because you disabled the output."
+            )
+        self.n_components = n_components
         self.output = output
+        self.test_split = test_split
 
-class LDA:
-    '''Class to store the data, methods and artifacts for Linear Discriminant Analysis'''
-    def __init__(self, lldf_model: LLDFModel, settings: LDASettings):
+class PLSDA:
+    '''
+    Class to store the data, methods and artifacts for Partial Least Squares
+    Discriminant Analysis
+    '''
+    def __init__(self, settings: PLSDASettings, fused_data: LLDFModel):
         self.settings = settings
-        self.x_data = lldf_model.x_data
-        self.x_train = lldf_model.x_train
-        self.y = lldf_model.y
-        self.model: Optional[LD] = None
-
-    def lda(self):
-        '''Performs Linear Discriminant Analysis'''
+        self.fused_data = fused_data
+        self.model: Optional[PLSR] = None
 
-        lda = LD(n_components=self.settings.components) # N-1 where N are the classes
-        scores_lda = lda.fit(self.x_data, self.y).transform(self.x_data)
+    def plsda(self):
+        '''Performs Partial Least Squares Discriminant Analysis'''
+        x = self.fused_data.x_data
+        y = self.fused_data.x_train.Substance.astype('category').cat.codes
 
-        if self.settings.output:
-            print(f"LDA scores:\n{scores_lda}")
-            print(lda.priors_)
-            print(lda.means_)
-            print(lda.coef_[0:self.settings.components,:])
-            pred=lda.predict(self.x_data)
-            print(np.unique(pred, return_counts=True))
-
-            print(confusion_matrix(pred, self.y))
-            print(classification_report(self.y, pred, digits=2))
-
-        lv_cols = [f'LV{i+1}' for i in range(self.settings.components)]
-        scores = pd.DataFrame(data = scores_lda, columns = lv_cols) # latent variables
-        scores.index = self.x_data.index
-        y_dataframe = pd.DataFrame(self.y, columns=['Substance'])
+        regr_pls = PLSR(n_components=self.settings.n_components)
+        regr_pls.fit_transform(x,y)
 
-        scores = pd.concat([scores, y_dataframe], axis = 1)
+        # Save the model
+        self.model = regr_pls
 
         if self.settings.output:
+            # Re-create the model
+            regr_pls_2 = PLSR(n_components=self.settings.n_components)
+            regr_pls_2.fit_transform(x,y)
+
+            # Scores
+            scores = regr_pls_2.x_scores_
+            lv_cols = [f"LV{i+1}" for i in range(self.settings.n_components)]
+            scores = pd.DataFrame(scores, columns = lv_cols)
+            scores.index = self.fused_data.x_train.index
+            y = self.fused_data.x_train.Substance
+            scores = pd.concat([scores, y], axis = 1)
             print(scores)
 
-            print(f"""
-                explained variance ratio (three components) with LDA:
-                {lda.explained_variance_ratio_}
-            """)
+            # Loadings
+            loadings = pd.DataFrame(regr_pls.x_loadings_,columns = lv_cols)
+            loadings["Attributes"] = self.fused_data.x_train.iloc[:,1:].columns
+            print(loadings)
 
-            # Display the explained variance ratio
-            print("Explained Variance Ratio:", lda.explained_variance_ratio_)
-
-            #Scores plot
+            # Scores plot
             fig = px.scatter(scores, x="LV1", y="LV2", color="Substance", hover_data=['Substance'])
             fig.update_xaxes(zeroline=True, zerolinewidth=1, zerolinecolor='Black')
             fig.update_yaxes(zeroline=True, zerolinewidth=1, zerolinecolor='Black')
             fig.update_layout(
                 height=600,
                 width=800,
                 title_text='Scores Plot')
             fig.show()
 
             # Plot 3D scores
             fig = px.scatter_3d(scores, x='LV1', y='LV2', z='LV3',
                                 color='Substance', hover_data=['Substance'],
-                                hover_name=scores.index
-            )
+                                hover_name=scores.index)
+            fig.update_xaxes(zeroline=True, zerolinewidth=1, zerolinecolor='Black')
+            fig.update_yaxes(zeroline=True, zerolinewidth=1, zerolinecolor='Black')
             fig.update_layout(
-            title_text='3D colored by Substance for Linear Discriminant Analysis')
+                title_text='Scores 3D Plot colored by Class using the raw data')
             fig.show()
 
-        lda2 = LD(n_components=self.settings.components)
-
-        self.x_train, x_test, y_train, y_test = train_test_split(
-            (scores.drop('Substance', axis=1).values),
-            self.y,
-            test_size=0.3,
-            random_state=42
-        )
-
-        lda2.fit(self.x_train, y_train)
-        lda2.predict(x_test)
-        y_pred = lda2.predict(x_test)
+            # Loadings plot
+            fig = px.scatter(loadings, x="LV1", y="LV2",text="Attributes")
+            fig.update_xaxes(zeroline=True, zerolinewidth=1, zerolinecolor='Black')
+            fig.update_yaxes(zeroline=True, zerolinewidth=1, zerolinecolor='Black')
+            fig.update_traces(textposition='top center')
+            fig.update_layout(
+                height=600,
+                width=800,
+                title_text='Loadings Plot')
+            fig.show()
 
-        if self.settings.output:
-            self.__print_prediction_graphs(y_test, y_pred)
 
-        self.model = lda
+            # Predictions
+            pred = regr_pls.predict(x)
+            pred = np.int8(np.abs(np.around(pred, decimals=0)))
+            print(f"Predicted data:\n\n{pred}")
+
+            # Print confusion matrix
+            y = self.fused_data.x_train.Substance.astype('category').cat.codes 
+            print_confusion_matrix(y, pred, "Confusion Matrix based on training set")
 
-    def __print_prediction_graphs(self, y_test, y_pred):
-        '''Helper function to print graphs and stats about LDA predictions.'''
-        # Assuming 'y_test' and 'y_pred' are your true and predicted labels
-        cm = confusion_matrix(y_test, y_pred)
-
-        # Get unique class labels from y_true
-        class_labels = sorted(set(y_test))
-
-        # Plot the confusion matrix using seaborn with custom colormap (Blues)
-        sns.heatmap(cm,
-            annot=True,
-            fmt='d',
-            cmap='Blues',
-            xticklabels=class_labels,
-            yticklabels=class_labels,
-            cbar=False,
-            vmin=0,
-            vmax=cm.max()
-        )
-
-        plt.xlabel('Predicted')
-        plt.ylabel('True')
-        plt.title('Confusion Matrix based on evaluation set')
-        plt.show()
 
-        # Print the classification report
-        print(classification_report(y_test, y_pred, digits=2))
+        if self.settings.output and self.settings.test_split:
+            x = self.fused_data.x_data
+            y = self.fused_data.x_train.Substance.astype('category').cat.codes
+            run_split_test(x, y, PLSR(self.settings.n_components))
 
     def predict(self, x_data: pd.DataFrame):
-        '''Performs LDA prediction once the model is trained.'''
+        '''Performs PLSDA prediction once the model is trained.'''
         if x_data is None:
-            raise TypeError("X data for LDA prediction must be non-empty.")
+            raise TypeError("X data for PLSDA prediction must be non-empty.")
         if self.model is None:
-            raise RuntimeError("The LDA model is not trained yet!")
+            raise RuntimeError("The PLSDA model is not trained yet!")
 
         y_pred = self.model.predict(x_data)
         return y_pred
```

### Comparing `chemfusekit-1.1.0b1/chemfusekit/lldf.py` & `chemfusekit-1.1.0b2/chemfusekit/lldf.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,16 @@
         self,
         qepas_path: str,
         qepas_sheet: str,
         rt_path: str,
         rt_sheet: str,
         preprocessing: str = 'snv'
     ):
+        if preprocessing not in ['snv', 'savgol', 'savgol+snv']:
+            raise SyntaxError("This type of preprocessing does not exist.")
         self.qepas_path = qepas_path
         self.qepas_sheet = qepas_sheet
         self.rt_path = rt_path
         self.rt_sheet = rt_sheet
         self.preprocessing = preprocessing
 
 class LLDF:
```

### Comparing `chemfusekit-1.1.0b1/chemfusekit/pca.py` & `chemfusekit-1.1.0b2/chemfusekit/pca.py`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/chemfusekit/svm.py` & `chemfusekit-1.1.0b2/chemfusekit/svm.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,19 +10,24 @@
 from sklearn.metrics import confusion_matrix, classification_report
 from sklearn.svm import SVC
 
 from chemfusekit.lldf import LLDFModel
 
 class SVMSettings:
     '''Holds the settings for the SVM object.'''
-    def __init__(self, kernel: str = 'linear', output: bool = False):
+    def __init__(self, kernel: str = 'linear', output: bool = False, test_split: bool = False):
         if kernel not in ['linear', 'poly', 'gaussian', 'sigmoid']:
             raise ValueError("Invalid type: must be linear, poly, gaussian or sigmoid")
+        if test_split is True and output is False:
+            raise Warning(
+                "You selected test_split but it won't run because you disabled the output."
+            )
         self.kernel = kernel
         self.output = output
+        self.test_split = test_split
 
 class SVM:
     '''Class for Support Vector Machine analysis of the data'''
     def __init__(self, fused_data: LLDFModel, settings: SVMSettings):
         self.fused_data = fused_data
         self.settings = settings
         self.model: Optional[SVC] = None
```

### Comparing `chemfusekit-1.1.0b1/docs/README.md` & `chemfusekit-1.1.0b2/docs/README.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/docs/docusaurus.config.js` & `chemfusekit-1.1.0b2/docs/docusaurus.config.js`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/docs/package-lock.json` & `chemfusekit-1.1.0b2/docs/package-lock.json`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/docs/package.json` & `chemfusekit-1.1.0b2/docs/package.json`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/docs/sidebars.js` & `chemfusekit-1.1.0b2/docs/sidebars.js`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/docs/docs/complete-workflow.md` & `chemfusekit-1.1.0b2/docs/docs/complete-workflow.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/docs/docs/tutorial.md` & `chemfusekit-1.1.0b2/docs/docs/tutorial.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/docs/docs/knn/knn.md` & `chemfusekit-1.1.0b2/docs/docs/knn/knn.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/docs/docs/knn/knnsettings.md` & `chemfusekit-1.1.0b2/docs/docs/knn/knnsettings.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/docs/docs/lda/lda.md` & `chemfusekit-1.1.0b2/docs/docs/lda/lda.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/docs/docs/lda/ldasettings.md` & `chemfusekit-1.1.0b2/docs/docs/lda/ldasettings.md`

 * *Files 22% similar despite different names*

```diff
@@ -5,29 +5,33 @@
 # LDASettings class
 
 Holds the settings for the [`LDA`](./lda.md) object.
 
 ## Syntax
 
 ```python
-LDASettings(components: int, output: bool)
+LDASettings(components: int, output: bool, split_test: bool)
 ```
 
 ## Fields and constructor parameters
 
 - `components`: the amount of components to be used in the LDA model. Defaults to 3.
 - `output`: toggles graph output. Defaults to `False`.
+- `test_split`: toggles split testing. Defaults to `False`.
+
 
 The constructor raises:
 - `ValueError("Invalid component number: must be a > 1 integer.")` if the number of
   components is not valid.
+- `Warning("You selected test_split but it won't run because you disabled the output.")` if split tests are run with `output` disabled
 
 ## Example
 
 ```python
 from chemfusekit.lda import LDASettings
 
 settings = LDASettings(
     components=(pca.components - 1),    # one less component than the number determined by PCA
-    output=True # graphs will be printed
+    output=True,  # graphs will be printed
+    test_split=True # split testing is enabled
 )
 ```
```

### Comparing `chemfusekit-1.1.0b1/docs/docs/lldf/lldf.md` & `chemfusekit-1.1.0b2/docs/docs/lldf/lldf.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/docs/docs/lldf/lldfsettings.md` & `chemfusekit-1.1.0b2/docs/docs/lldf/lldfsettings.md`

 * *Files 10% similar despite different names*

```diff
@@ -22,14 +22,17 @@
 - `qepas_path`: a `str` containing the path to the QEPAS spectrography Excel datasheet
 - `qepas_sheet`: a `str` containing the sheet name within the QEPAS Excel file
 - `rt_path`: a `str` containing the path to the GC chromatrography Excel datasheet
 - `rt_sheet`: a `str` containing the sheet name within the GC Excel file
 - `preprocessing`: a `str` with the name of the preprocessing to be applied to the QEPAS data.
    Available options: `snv` (normalization), `savgol` (Savitski-Golay smoothing), `savgol+snv` (both).
 
+The constructor throws:
+- `TypeError("This type of preprocessing does not exist.")` if the preprocessing parameter is not one of the three available.
+
 ## Example
 
 ```python
 from chemfusekit.lldf import LLDFSettings
 
 # Initialize the settings for low-level data fusion
 lldf_settings = LLDFSettings(
```

### Comparing `chemfusekit-1.1.0b1/docs/docs/lr/lr.md` & `chemfusekit-1.1.0b2/docs/docs/lr/lr.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/docs/docs/pca/pca.md` & `chemfusekit-1.1.0b2/docs/docs/pca/pca.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/docs/docs/pca/pcasettings.md` & `chemfusekit-1.1.0b2/docs/docs/pca/pcasettings.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/docs/docs/plsda/plsda.md` & `chemfusekit-1.1.0b2/docs/docs/plsda/plsda.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/docs/docs/plsda/plsdasettings.md` & `chemfusekit-1.1.0b2/docs/docs/plsda/plsdasettings.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/docs/docs/svm/svm.md` & `chemfusekit-1.1.0b2/docs/docs/svm/svm.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/docs/docs/svm/svmsettings.md` & `chemfusekit-1.1.0b2/docs/docs/svm/svmsettings.md`

 * *Files 20% similar despite different names*

```diff
@@ -17,22 +17,25 @@
 - `kernel`: the type of kernel to use in the SVM analysis. Available options:
   - `linear`
   - `poly`
   - `gaussian`
   - `sigmoid`
   Defaults to `linear`.
 - `output`: toggles graph output. Defaults to `False`.
+- `test_split`: toggles split testing. Defaults to `False`.
 
 The constructor raises:
 - `ValueError("Invalid type: must be linear, poly, gaussian or sigmoid")` if the selected kernel is not one of the available
+- `Warning("You selected test_split but it won't run because you disabled the output.")` if split tests are run with `output` disabled
 
 ## Example
 
 ```python
 from chemfusekit.svm import SVMSettings
 
 # Initialize the settings for Support Vector Machine
 svm_settings = SVMSettings(
     type='linear',
-    output=True # graphs will be printed
+    output=True,  # graphs will be printed
+    test_split=True # split testing is enabled
 )
 ```
```

### Comparing `chemfusekit-1.1.0b1/docs/src/components/HomepageFeatures/index.js` & `chemfusekit-1.1.0b2/docs/src/components/HomepageFeatures/index.js`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/docs/src/css/custom.css` & `chemfusekit-1.1.0b2/docs/src/css/custom.css`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/docs/src/pages/index.js` & `chemfusekit-1.1.0b2/docs/src/pages/index.js`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/docs/src/pages/project/continuous-integration.md` & `chemfusekit-1.1.0b2/docs/src/pages/project/continuous-integration.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 ---
 title: Continuous Integration
 description: Our continuous integration workflow.
 ---
 
 # Continuous Integration
 
-Our remote repository operates four continuous integration / continuous deployment workflows.
+Our remote repository operates five continuous integration / continuous deployment workflows.
 
 Two of the workflows are about code quality:
 - a [`pylint`](https://pylint.readthedocs.io/en/stable/)` workflow that rejects commits with a code quality lower than 8.00
 - a [`unittest`](https://docs.python.org/3/library/unittest.html) workflow that rejects commits that do not pass unit tests
 
 A third workflow is about documentation deployment:
 - a [`Docusaurus`](https://docusaurus.io) page builder that automatically deploys this documentation
   website to [`GitHub Pages`](https://pages.github.com)
 
-A fourth, final workflow automates semantic releases.
+A fourth workflow automates semantic releases.
+
+A fifth, final workflow automates the building of the thesis document.
```

### Comparing `chemfusekit-1.1.0b1/docs/src/pages/project/process-model.md` & `chemfusekit-1.1.0b2/docs/src/pages/project/process-model.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/docs/src/pages/project/project-philosophy.md` & `chemfusekit-1.1.0b2/docs/src/pages/project/project-philosophy.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/docs/src/pages/project/project-plan.md` & `chemfusekit-1.1.0b2/docs/src/pages/project/project-plan.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/docs/src/pages/project/requirements-specification.md` & `chemfusekit-1.1.0b2/docs/src/pages/project/requirements-specification.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/docs/src/pages/project/use-cases.md` & `chemfusekit-1.1.0b2/docs/src/pages/project/use-cases.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/docs/static/img/colab-logo.svg` & `chemfusekit-1.1.0b2/docs/static/img/colab-logo.svg`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/docs/static/img/docusaurus-social-card.jpg` & `chemfusekit-1.1.0b2/docs/static/img/docusaurus-social-card.jpg`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/docs/static/img/docusaurus.png` & `chemfusekit-1.1.0b2/docs/static/img/docusaurus.png`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/docs/static/img/favicon.ico` & `chemfusekit-1.1.0b2/docs/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/docs/static/img/happy-woman.svg` & `chemfusekit-1.1.0b2/docs/static/img/happy-woman.svg`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/docs/static/img/logo.svg` & `chemfusekit-1.1.0b2/docs/static/img/logo.svg`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/docs/static/img/magnifying-glass.svg` & `chemfusekit-1.1.0b2/docs/static/img/magnifying-glass.svg`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/notes/Beartype.md` & `chemfusekit-1.1.0b2/notes/Beartype.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/notes/Constructors.md` & `chemfusekit-1.1.0b2/notes/Constructors.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/notes/Conventional Commits.md` & `chemfusekit-1.1.0b2/notes/Conventional Commits.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/notes/Kanban.md` & `chemfusekit-1.1.0b2/notes/Kanban.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/notes/Use Case Diagram.md` & `chemfusekit-1.1.0b2/notes/Use Case Diagram.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/notes/.obsidian/core-plugins-migration.json` & `chemfusekit-1.1.0b2/notes/.obsidian/core-plugins-migration.json`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/notes/.obsidian/workspace.json` & `chemfusekit-1.1.0b2/notes/.obsidian/workspace.json`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/notes/.obsidian/plugins/calendar/main.js` & `chemfusekit-1.1.0b2/notes/.obsidian/plugins/calendar/main.js`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/notes/.obsidian/plugins/obsidian-kanban/main.js` & `chemfusekit-1.1.0b2/notes/.obsidian/plugins/obsidian-kanban/main.js`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/notes/.obsidian/plugins/obsidian-kanban/styles.css` & `chemfusekit-1.1.0b2/notes/.obsidian/plugins/obsidian-kanban/styles.css`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/notes/.obsidian/plugins/obsidian-plantuml/main.js` & `chemfusekit-1.1.0b2/notes/.obsidian/plugins/obsidian-plantuml/main.js`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/notes/.obsidian/plugins/obsidian-plantuml/styles.css` & `chemfusekit-1.1.0b2/notes/.obsidian/plugins/obsidian-plantuml/styles.css`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/notes/Devlog/2024-04-19.md` & `chemfusekit-1.1.0b2/notes/Devlog/2024-04-19.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/notes/Devlog/2024-04-20.md` & `chemfusekit-1.1.0b2/notes/Devlog/2024-04-20.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/notes/Devlog/2024-04-22.md` & `chemfusekit-1.1.0b2/notes/Devlog/2024-04-22.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/notes/Devlog/2024-04-23.md` & `chemfusekit-1.1.0b2/notes/Devlog/2024-04-23.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/notes/Devlog/2024-05-06.md` & `chemfusekit-1.1.0b2/notes/Devlog/2024-05-06.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/notes/Devlog/2024-05-07.md` & `chemfusekit-1.1.0b2/notes/Devlog/2024-05-07.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/notes/Devlog/2024-05-08.md` & `chemfusekit-1.1.0b2/notes/Devlog/2024-05-08.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/notes/Devlog/2024-05-09.md` & `chemfusekit-1.1.0b2/notes/Devlog/2024-05-09.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/notes/Devlog/2024-05-17.md` & `chemfusekit-1.1.0b2/notes/Devlog/2024-05-17.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/notes/Devlog/2024-05-18.md` & `chemfusekit-1.1.0b2/notes/Devlog/2024-05-18.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/notes/UML/Process state machine.md` & `chemfusekit-1.1.0b2/notes/UML/Process state machine.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/notes/UML/Sequence.md` & `chemfusekit-1.1.0b2/notes/UML/Sequence.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/notes/UML/Use cases.md` & `chemfusekit-1.1.0b2/notes/UML/Use cases.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/tests/qepas.xlsx` & `chemfusekit-1.1.0b2/tests/qepas.xlsx`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/tests/rt.xlsx` & `chemfusekit-1.1.0b2/tests/rt.xlsx`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/tests/test_knn.py` & `chemfusekit-1.1.0b2/tests/test_knn.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,19 +96,24 @@
             rt_path='tests/rt.xlsx',
             rt_sheet='Sheet1',
             preprocessing='snv'
         )
         lldf = LLDF(lldf_settings)
         lldf.lldf()
 
-        # Set up and run KNN
+        # Set up and run KNN (no output)
         knn_settings = KNNSettings()
         knn = KNN(knn_settings, lldf.fused_data)
         knn.knn()
 
+        # With output
+        knn_settings = KNNSettings(output=True)
+        knn = KNN(knn_settings, lldf.fused_data)
+        knn.knn()
+
     def test_prediction(self):
         '''Test case against prediction parameter issues.'''
         # Perform preliminary data fusion
         lldf_settings = LLDFSettings(
             qepas_path='tests/qepas.xlsx',
             qepas_sheet='Sheet1',
             rt_path='tests/rt.xlsx',
```

### Comparing `chemfusekit-1.1.0b1/tests/test_lda.py` & `chemfusekit-1.1.0b2/tests/test_lda.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,20 @@
 from chemfusekit.lldf import LLDFSettings, LLDF
 
 class TestLDA(unittest.TestCase):
     '''Test suite for the LDA module.'''
 
     def test_lda_settings(self):
         '''Test case against settings errors.'''
+        # Check for negative component rejection
         with self.assertRaises(ValueError):
             LDASettings(components=-3, output=True)
+        # Check if split tests with no output cause warnings:
+        with self.assertRaises(Warning):
+            LDASettings(output=False,test_split=True)
 
     def test_lda_constructor(self):
         '''Test case against constructor parameter issues.'''
 
         # Create an LLDF model and initialize it
         lldf_settings = LLDFSettings(
             qepas_path='tests/qepas.xlsx',
@@ -61,14 +65,19 @@
         lda.lda()
 
         # Create an LDA object and train it, with false output
         lda_settings = LDASettings(output=False)
         lda = LDA(lldf.fused_data, lda_settings)
         lda.lda()
 
+        # Create an LDA object and train it, with true output and split tests
+        lda_settings = LDASettings(output=True, test_split=True)
+        lda = LDA(lldf.fused_data, lda_settings)
+        lda.lda()
+
     def test_lda_predict(self):
         '''Test case against prediction parameter issues.'''        
 
         # Create an LLDF model and initialize it
         lldf_settings = LLDFSettings(
             qepas_path='tests/qepas.xlsx',
             qepas_sheet='Sheet1',
```

### Comparing `chemfusekit-1.1.0b1/tests/test_lldf.py` & `chemfusekit-1.1.0b2/tests/test_lldf.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,22 +16,34 @@
             preprocessing='savgol'
         )
         lldf = LLDF(settings)
         self.assertRaises(FileNotFoundError, lldf.lldf)
 
     def test_preprocessing_techniques(self):
         '''Test case against wrong preprocessing user input.'''
+        with self.assertRaises(SyntaxError):
+            settings = LLDFSettings(
+                qepas_path='tests/qepas.xlsx',
+                qepas_sheet='Sheet1',
+                rt_path='tests/rt.xlsx',
+                rt_sheet='Sheet1',
+                preprocessing='qpl' # test with non-existent preprocessing technique
+            )
+        # Now a correct value:
         settings = LLDFSettings(
-            qepas_path='tests/qepas.xlsx',
-            qepas_sheet='Sheet1',
-            rt_path='tests/rt.xlsx',
-            rt_sheet='Sheet1',
-            preprocessing='qpl' # test with non-existent preprocessing technique
-        )
+                qepas_path='tests/qepas.xlsx',
+                qepas_sheet='Sheet1',
+                rt_path='tests/rt.xlsx',
+                rt_sheet='Sheet1',
+                preprocessing='snv' # test with non-existent preprocessing technique
+            )
+
+        # Make the value wrong and test LLDF
         lldf = LLDF(settings)
+        lldf.settings.preprocessing='qpl' 
         self.assertRaises(SyntaxError, lldf.lldf)
 
         # now check if it works with the three real processing techniques:
         lldf.settings.preprocessing='snv'
         lldf.lldf()
         lldf.settings.preprocessing='savgol'
         lldf.lldf()
```

### Comparing `chemfusekit-1.1.0b1/tests/test_lr.py` & `chemfusekit-1.1.0b2/tests/test_lr.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,33 +13,41 @@
 
     def test_lr_settings(self):
         '''Test case against settings input errors.'''
         # Should raise an exception when the algorithm is not available
         with self.assertRaises(ValueError):
             LRSettings(
                 algorithm='unknown',
-                output=True
+                output=True,
+                test_split=True
             )
 
         # Should raise an exception when any of the inputs is a null value
         with self.assertRaises(TypeError):
             LRSettings(
                 algorithm=None,
-                output=True
+                output=True,
+                test_split=True
             )
         with self.assertRaises(TypeError):
             LRSettings(
                 algorithm='liblinear',
-                output=None
-            )
+                output=None,
+                test_split=True
+            ) 
         with self.assertRaises(TypeError):
             LRSettings(
-                algorithm=None,
-                output=None
+                algorithm='liblinear',
+                output=True,
+                test_split=None
             )
+        
+        # Check if split tests with no output cause warnings:
+        with self.assertRaises(Warning):
+            LRSettings(output=False,test_split=True)
 
         # Should not raise any exception when the input is correct
         LRSettings(
             algorithm='liblinear',
             output=False
         )
 
@@ -86,18 +94,24 @@
         lldf.lldf()
 
         pca_settings = PCASettings()
         pca = PCA(lldf.fused_data, pca_settings)
         pca.pca()
         pca.pca_stats()
 
+        # With no output
         lr_settings = LRSettings()
         lr = LR(lr_settings, pca.array_scores, lldf.fused_data.y)
         lr.lr()
 
+        # With output and split tests
+        lr_settings = LRSettings(output=True, test_split=True)
+        lr = LR(lr_settings, pca.array_scores, lldf.fused_data.y)
+        lr.lr()
+
 
     def test_lr_predict(self):
         '''Test case against prediction input errors.'''
         # Set up the model
         lr_settings = LRSettings()
         lr = LR(lr_settings, np.asarray([7.02, 8.11]), np.asarray([43.1, 0.06]))
```

### Comparing `chemfusekit-1.1.0b1/tests/test_pca.py` & `chemfusekit-1.1.0b2/tests/test_pca.py`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/tests/test_plsda.py` & `chemfusekit-1.1.0b2/tests/test_plsda.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,31 +52,36 @@
 
         # fused_data parameter
         knn_settings = PLSDASettings()
         wrong_fused_data = lldf_settings
         with self.assertRaises(TypeError):
             PLSDA(knn_settings, wrong_fused_data)  # pass an object of the wrong class as fused_data
     
-    def test_knn(self):
+    def test_plsda(self):
         '''Integration test case for the training function.'''
         # Perform preliminary data fusion
         lldf_settings = LLDFSettings(
             qepas_path='tests/qepas.xlsx',
             qepas_sheet='Sheet1',
             rt_path='tests/rt.xlsx',
             rt_sheet='Sheet1',
             preprocessing='snv'
         )
         lldf = LLDF(lldf_settings)
         lldf.lldf()
 
-        # Set up and run PLSDA
+        # Set up and run PLSDA (no output)
         plsda_settings = PLSDASettings()
         plsda = PLSDA(plsda_settings, lldf.fused_data)
         plsda.plsda()
+
+        # Run with output and split testing
+        plsda_settings = PLSDASettings(output=True, test_split=True)
+        plsda = PLSDA(plsda_settings, lldf.fused_data)
+        plsda.plsda() 
     
     def test_prediction(self):
         '''Test case against prediction parameter issues.'''
         # Perform preliminary data fusion
         lldf_settings = LLDFSettings(
             qepas_path='tests/qepas.xlsx',
             qepas_sheet='Sheet1',
```

### Comparing `chemfusekit-1.1.0b1/tests/test_svm.py` & `chemfusekit-1.1.0b2/tests/test_svm.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,32 @@
 class TestSVM(unittest.TestCase):
     '''Test suite for the LDA module.'''
 
     def test_svm_settings(self):
         '''Test case against settings errors.'''
         # Test against null type
         with self.assertRaises(TypeError):
-            SVMSettings(None, False)
+            SVMSettings(None, False, False)
         # Test against null output selector
         with self.assertRaises(TypeError):
-            SVMSettings('linear', None)
-        with self.assertRaises(ValueError):
+            SVMSettings('linear', None, False)
+        # Test against null test_split selector
+        with self.assertRaises(TypeError):
+            SVMSettings('linear', None, False)
         # Test against non-existent kernels
-            SVMSettings(kernel='made up name')
+        with self.assertRaises(TypeError):
+            SVMSettings('linear', False, None)
+
+        # Check if split tests with no output cause warnings:
+        with self.assertRaises(Warning):
+            SVMSettings(output=False,test_split=True)
+
         # Now call with proper values:
-        SVMSettings(kernel='gaussian', output=True)
+        SVMSettings(kernel='gaussian', output=True, test_split=False)
+
 
     def test_svm_constructor(self):
         '''Test case against constructor parameter issues.'''
 
         # Create an LLDF model and initialize it
         lldf_settings = LLDFSettings(
             qepas_path='tests/qepas.xlsx',
```

### Comparing `chemfusekit-1.1.0b1/pyproject.toml` & `chemfusekit-1.1.0b2/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "chemfusekit"
-version = "1.1.0b1"
+version = "1.1.0b2"
 description = "A minimal Python / Jupyter Notebook / Colab library for data fusion and chemometrical analysis."
 authors = [
     { name = "Federico Aguzzi", email = "62149513+f-aguzzi@users.noreply.github.com" }
 ]
 dependencies = [
     "numpy>=1.26.4",
     "scipy>=1.13.0",
@@ -29,16 +29,16 @@
 managed = true
 dev-dependencies = [
     "pylint>=3.1.1",
 ]
 
 [tool.rye.scripts]
 test = "python -m unittest discover tests"
-pylint-local = "pylint colab_datafusuion_analysis/**/*.py"
-pylint-ci = "pylint --disable=C0114,C0115,C0116 --exit-zero colab_datafusion_analysis/**/*.py"
-pylint-score-ci = "pylint --disable=all --enable=metrics --output-format=text colab_datafusuion_analysis/**/.py"
+pylint-local = "pylint chemfusekit/**/*.py"
+pylint-ci = "pylint --disable=C0114,C0115,C0116 --exit-zero chemfusekit/**/*.py"
+pylint-score-ci = "pylint --disable=all --enable=metrics --output-format=text chemfusekit/**/.py"
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [tool.hatch.build.targets.wheel]
 packages = ["chemfusekit"]
```

### Comparing `chemfusekit-1.1.0b1/readme.md` & `chemfusekit-1.1.0b2/readme.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b1/PKG-INFO` & `chemfusekit-1.1.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: chemfusekit
-Version: 1.1.0b1
+Version: 1.1.0b2
 Summary: A minimal Python / Jupyter Notebook / Colab library for data fusion and chemometrical analysis.
 Author-email: Federico Aguzzi <62149513+f-aguzzi@users.noreply.github.com>
 Requires-Python: >=3.8
 Requires-Dist: beartype>=0.18.5
 Requires-Dist: matplotlib>=3.8.4
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: openpyxl>=3.1.2
```

