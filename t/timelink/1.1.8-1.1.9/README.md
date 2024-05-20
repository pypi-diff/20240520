# Comparing `tmp/timelink-1.1.8.tar.gz` & `tmp/timelink-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timelink-1.1.8.tar", last modified: Thu May  2 03:12:30 2024, max compression
+gzip compressed data, was "timelink-1.1.9.tar", last modified: Fri May  3 00:07:08 2024, max compression
```

## Comparing `timelink-1.1.8.tar` & `timelink-1.1.9.tar`

### file list

```diff
@@ -1,278 +1,278 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-02 03:12:30.580325 timelink-1.1.8/
--rw-rw-r--   0 travis    (2000) travis    (2000)      209 2024-05-02 03:09:30.000000 timelink-1.1.8/AUTHORS.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     9422 2024-05-02 03:09:30.000000 timelink-1.1.8/CONTRIBUTING.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     3393 2024-05-02 03:09:30.000000 timelink-1.1.8/HISTORY.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1084 2024-05-02 03:09:30.000000 timelink-1.1.8/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      262 2024-05-02 03:09:30.000000 timelink-1.1.8/MANIFEST.in
--rw-r--r--   0 travis    (2000) travis    (2000)     4847 2024-05-02 03:12:30.580325 timelink-1.1.8/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      507 2024-05-02 03:09:30.000000 timelink-1.1.8/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-02 03:12:30.488318 timelink-1.1.8/docs/
--rw-rw-r--   0 travis    (2000) travis    (2000)      609 2024-05-02 03:09:30.000000 timelink-1.1.8/docs/Makefile
--rw-rw-r--   0 travis    (2000) travis    (2000)       28 2024-05-02 03:09:30.000000 timelink-1.1.8/docs/authors.rst
--rwxrwxr-x   0 travis    (2000) travis    (2000)     5433 2024-05-02 03:09:30.000000 timelink-1.1.8/docs/conf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       33 2024-05-02 03:09:30.000000 timelink-1.1.8/docs/contributing.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      303 2024-05-02 03:09:30.000000 timelink-1.1.8/docs/documentation.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       28 2024-05-02 03:09:30.000000 timelink-1.1.8/docs/history.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1158 2024-05-02 03:09:30.000000 timelink-1.1.8/docs/index.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1183 2024-05-02 03:09:30.000000 timelink-1.1.8/docs/installation.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      770 2024-05-02 03:09:30.000000 timelink-1.1.8/docs/make.bat
--rw-rw-r--   0 travis    (2000) travis    (2000)      103 2024-05-02 03:09:30.000000 timelink-1.1.8/docs/modules.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       27 2024-05-02 03:09:30.000000 timelink-1.1.8/docs/readme.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)    20745 2024-05-02 03:09:30.000000 timelink-1.1.8/docs/som_pom_mapping.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     2081 2024-05-02 03:09:30.000000 timelink-1.1.8/docs/timelink-introduction.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     2866 2024-05-02 03:09:30.000000 timelink-1.1.8/docs/timelink-python-usage.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     2148 2024-05-02 03:09:30.000000 timelink-1.1.8/docs/timelink.api.models.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      777 2024-05-02 03:09:30.000000 timelink-1.1.8/docs/timelink.api.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      527 2024-05-02 03:09:30.000000 timelink-1.1.8/docs/timelink.app.backend.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      500 2024-05-02 03:09:30.000000 timelink-1.1.8/docs/timelink.app.models.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      604 2024-05-02 03:09:30.000000 timelink-1.1.8/docs/timelink.app.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      489 2024-05-02 03:09:30.000000 timelink-1.1.8/docs/timelink.app.schemas.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      661 2024-05-02 03:09:30.000000 timelink-1.1.8/docs/timelink.app.services.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      823 2024-05-02 03:09:30.000000 timelink-1.1.8/docs/timelink.app.web.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     2194 2024-05-02 03:09:30.000000 timelink-1.1.8/docs/timelink.kleio.groups.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      847 2024-05-02 03:09:30.000000 timelink-1.1.8/docs/timelink.kleio.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     2296 2024-05-02 03:09:30.000000 timelink-1.1.8/docs/timelink.mhk.models.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      369 2024-05-02 03:09:30.000000 timelink-1.1.8/docs/timelink.mhk.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      523 2024-05-02 03:09:30.000000 timelink-1.1.8/docs/timelink.networks.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      352 2024-05-02 03:09:30.000000 timelink-1.1.8/docs/timelink.notebooks.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      495 2024-05-02 03:09:30.000000 timelink-1.1.8/docs/timelink.pandas.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      565 2024-05-02 03:09:30.000000 timelink-1.1.8/docs/timelink.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      150 2024-05-02 03:09:30.000000 timelink-1.1.8/docs/usage.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      364 2024-05-02 03:09:30.000000 timelink-1.1.8/pyproject.toml
--rw-rw-r--   0 travis    (2000) travis    (2000)      468 2024-05-02 03:12:30.584325 timelink-1.1.8/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     2092 2024-05-02 03:09:30.000000 timelink-1.1.8/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-02 03:12:30.492318 timelink-1.1.8/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2709 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-02 03:12:30.492318 timelink-1.1.8/tests/db/
--rw-r--r--   0 travis    (2000) travis    (2000)    32768 2024-05-02 03:11:41.000000 timelink-1.1.8/tests/db/test_users.sqlite
--rw-rw-r--   0 travis    (2000) travis    (2000)    12170 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/test_api_models_db.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      903 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/test_api_models_no_db.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27174 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/test_groups.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3379 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/test_import_MHK.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13671 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/test_import_TL.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10833 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/test_kleio_server.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8920 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/test_mhk_models_db.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      870 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/test_mhk_models_no_db.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3313 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/test_mhk_utilities.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4187 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/test_pandas.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      168 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/test_postgres_db.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1359 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/test_timelink.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8352 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/test_timelink_users.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-02 03:12:30.492318 timelink-1.1.8/tests/timelink-home/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-02 03:12:30.472317 timelink-1.1.8/tests/timelink-home/.kleio/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-02 03:12:30.492318 timelink-1.1.8/tests/timelink-home/.kleio/conf/
--rw-r--r--   0 travis    (2000) travis    (2000)      724 2024-05-02 03:10:49.000000 timelink-1.1.8/tests/timelink-home/.kleio/conf/token_db
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-02 03:12:30.496318 timelink-1.1.8/tests/timelink-home/.kleio/logs/
--rw-r--r--   0 travis    (2000) travis    (2000)      867 2024-05-02 03:11:07.000000 timelink-1.1.8/tests/timelink-home/.kleio/logs/kleio_service.log
--rw-r--r--   0 travis    (2000) travis    (2000)      561 2024-05-02 03:11:04.000000 timelink-1.1.8/tests/timelink-home/.kleio.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-02 03:12:30.496318 timelink-1.1.8/tests/timelink-home/projects/
--rw-rw-r--   0 travis    (2000) travis    (2000)       71 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/.gitignore
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-02 03:12:30.476317 timelink-1.1.8/tests/timelink-home/projects/test-project/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-02 03:12:30.496318 timelink-1.1.8/tests/timelink-home/projects/test-project/identifications/
--rw-rw-r--   0 travis    (2000) travis    (2000)    16686 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/test-project/identifications/mhk_identification_toliveira.cli
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-02 03:12:30.476317 timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-02 03:12:30.476317 timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-02 03:12:30.496318 timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/linked_data/
--rw-rw-r--   0 travis    (2000) travis    (2000)   119167 2024-05-02 03:11:01.000000 timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/linked_data/dehergne-a.cli
--rw-rw-r--   0 travis    (2000) travis    (2000)   119167 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/linked_data/dehergne-a.org
--rw-rw-r--   0 travis    (2000) travis    (2000)    48349 2024-05-02 03:10:57.000000 timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/linked_data/dehergne-locations-1644.cli
--rw-rw-r--   0 travis    (2000) travis    (2000)    48349 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/linked_data/dehergne-locations-1644.org
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-02 03:12:30.496318 timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/notariais/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2171 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/notariais/docsregiospontepisc.cli
--rwxrwxr-x   0 travis    (2000) travis    (2000)    38720 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/notariais/notarial80.cli
--rw-rw-r--   0 travis    (2000) travis    (2000)    60802 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/notariais/notlousa1.cli
--rw-rw-r--   0 travis    (2000) travis    (2000)    80615 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/notariais/perdoes.cli
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-02 03:12:30.476317 timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-02 03:12:30.500319 timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/baptismos/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2732 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/baptismos/bap-com-celebrantes.cli
--rw-rw-r--   0 travis    (2000) travis    (2000)    43942 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/baptismos/bapt1714.cli
--rw-rw-r--   0 travis    (2000) travis    (2000)    97925 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/baptismos/bapteirasproblem1.cli
--rw-rw-r--   0 travis    (2000) travis    (2000)   136532 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/baptismos/bapteirasproblem2.cli
--rw-rw-r--   0 travis    (2000) travis    (2000)      640 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/baptismos/rogeriodomingos_bap_problem.cli
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-02 03:12:30.500319 timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/casamentos/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2034 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/casamentos/cas1714-1722-com-celebrante.cli
--rw-rw-r--   0 travis    (2000) travis    (2000)    94359 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/casamentos/cas1714-1722.cli
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-02 03:12:30.500319 timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/crisma/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1590 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/crisma/crisma1753.cli
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-02 03:12:30.504319 timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/obitos/
--rw-rw-r--   0 travis    (2000) travis    (2000)    16671 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/obitos/ob1688.cli
--rw-rw-r--   0 travis    (2000) travis    (2000)    16672 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/obitos/ob1688b.cli
--rw-rw-r--   0 travis    (2000) travis    (2000)     7263 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/obitos/obit1714.cli
--rw-rw-r--   0 travis    (2000) travis    (2000)   268277 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/obitos/obiteirasproblem.cli
--rw-rw-r--   0 travis    (2000) travis    (2000)      842 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/obitos/obitoShort.cli
--rw-rw-r--   0 travis    (2000) travis    (2000)      793 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/obitos/obitoShort_id.cli
--rw-rw-r--   0 travis    (2000) travis    (2000)      666 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/obitos/obitoShort_id_id.cli
--rw-rw-r--   0 travis    (2000) travis    (2000)     1229 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/obitos/testeParentescos.cli
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-02 03:12:30.504319 timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/roisdeconfessados/
--rw-rw-r--   0 travis    (2000) travis    (2000)   213581 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/roisdeconfessados/coja-rol-1841.cli
--rw-rw-r--   0 travis    (2000) travis    (2000)    52584 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/roisdeconfessados/eiras-rol1.cli
--rw-rw-r--   0 travis    (2000) travis    (2000)    51851 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/roisdeconfessados/eiras-rol2.cli
--rw-rw-r--   0 travis    (2000) travis    (2000)    52776 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/roisdeconfessados/eiras-rol3.cli
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-02 03:12:30.512320 timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3249 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/Devedores.cli
--rw-rw-r--   0 travis    (2000) travis    (2000)    39369 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/EmpFAfonso.cli
--rw-rw-r--   0 travis    (2000) travis    (2000)  1381318 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/auc-alunos.cli
--rw-rw-r--   0 travis    (2000) travis    (2000)   101268 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/auc_cartulario18.cli
--rw-rw-r--   0 travis    (2000) travis    (2000)    50693 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/eleicoes1.cli
--rw-rw-r--   0 travis    (2000) travis    (2000)    71568 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/genealdiversas.cli
--rw-rw-r--   0 travis    (2000) travis    (2000)   103980 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/glopes-lap1561.cli
--rw-rw-r--   0 travis    (2000) travis    (2000)    48446 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/ivcc.cli
--rw-rw-r--   0 travis    (2000) travis    (2000)   165942 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/lrazao516pe.cli
--rw-rw-r--   0 travis    (2000) travis    (2000)    80126 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/misMesa.cli
--rw-rw-r--   0 travis    (2000) travis    (2000)     3309 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/mp758-santiago-beduido.cli
--rwxrwxr-x   0 travis    (2000) travis    (2000)   113694 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/nommiz.cli
--rw-rw-r--   0 travis    (2000) travis    (2000)      674 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/quotes.cli
--rw-rw-r--   0 travis    (2000) travis    (2000)     1438 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/sourecoimbrabispcoimbra_apontamentosd.cli
--rw-rw-r--   0 travis    (2000) travis    (2000)     4473 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/vereacao.cli
--rw-rw-r--   0 travis    (2000) travis    (2000)    49876 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/xpto_comuns_soure.kleio
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-02 03:12:30.512320 timelink-1.1.8/tests/timelink-home/projects/test-project/notebooks/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4628 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/test-project/notebooks/kleio_files.ipynb
--rw-rw-r--   0 travis    (2000) travis    (2000)     3938 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/test-project/notebooks/kleio_server_version.ipynb
--rw-rw-r--   0 travis    (2000) travis    (2000)     1270 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/test-project/notebooks/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    77283 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/test-project/notebooks/test_entity_with_attributes.ipynb
--rw-rw-r--   0 travis    (2000) travis    (2000)    89284 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/test-project/notebooks/test_group_attributes.ipynb
--rw-rw-r--   0 travis    (2000) travis    (2000)    24174 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/test-project/notebooks/test_issue13.ipynb
--rw-rw-r--   0 travis    (2000) travis    (2000)     3638 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/test-project/notebooks/test_issue26.ipynb
--rw-rw-r--   0 travis    (2000) travis    (2000)     5838 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/test-project/notebooks/test_pnames.ipynb
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-02 03:12:30.512320 timelink-1.1.8/tests/timelink-home/projects/test-project/structures/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-02 03:12:30.476317 timelink-1.1.8/tests/timelink-home/projects/test-project/structures/sources/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-02 03:12:30.476317 timelink-1.1.8/tests/timelink-home/projects/test-project/structures/sources/reference_sources/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-02 03:12:30.476317 timelink-1.1.8/tests/timelink-home/projects/test-project/structures/sources/reference_sources/paroquiais/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-02 03:12:30.512320 timelink-1.1.8/tests/timelink-home/projects/test-project/structures/sources/reference_sources/paroquiais/casamentos/
--rw-rw-r--   0 travis    (2000) travis    (2000)    99663 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/test-project/structures/sources/reference_sources/paroquiais/casamentos/cas1714-1722.str
--rw-rw-r--   0 travis    (2000) travis    (2000)   100155 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/test-project/structures/sources.str
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-02 03:12:30.476317 timelink-1.1.8/tests/timelink-home/projects/tutorial/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-02 03:12:30.516320 timelink-1.1.8/tests/timelink-home/projects/tutorial/kleio/
--rw-rw-r--   0 travis    (2000) travis    (2000)  1381318 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/tutorial/kleio/auc-alunos.cli
--rw-rw-r--   0 travis    (2000) travis    (2000)    17236 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/tutorial/kleio/b1685.cli
--rw-rw-r--   0 travis    (2000) travis    (2000)   119167 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/tutorial/kleio/dehergne-a.cli
--rw-rw-r--   0 travis    (2000) travis    (2000)    48311 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/tutorial/kleio/dehergne-locations-1644.cli
--rw-rw-r--   0 travis    (2000) travis    (2000)    27101 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/tutorial/kleio/dehergne-locations-1701.cli
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-02 03:12:30.520320 timelink-1.1.8/tests/timelink-home/projects/tutorial/notebooks/
--rw-rw-r--   0 travis    (2000) travis    (2000)    33926 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/tutorial/notebooks/0-kleio-files.ipynb
--rw-rw-r--   0 travis    (2000) travis    (2000)   138142 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/tutorial/notebooks/0-tutorial.ipynb
--rw-rw-r--   0 travis    (2000) travis    (2000)   230699 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/tutorial/notebooks/1-receipts.ipynb
--rw-rw-r--   0 travis    (2000) travis    (2000)     1041 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/tutorial/notebooks/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)     1270 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/timelink-home/projects/tutorial/notebooks/requirements.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-02 03:12:30.528321 timelink-1.1.8/tests/xml_data/
--rw-rw-r--   0 travis    (2000) travis    (2000)    17236 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/xml_data/b1685.cli
--rw-rw-r--   0 travis    (2000) travis    (2000)   756798 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/xml_data/b1685.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)  2037922 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/xml_data/dehergne-a.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)   930555 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/xml_data/dehergne-locations-1644.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)    66759 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/xml_data/dev1692.cli
--rw-rw-r--   0 travis    (2000) travis    (2000)  1485749 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/xml_data/dev1692.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)   116461 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/xml_data/mhk_identification_toliveira.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)    49771 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/xml_data/test-atr-date.xml
--rw-rw-r--   0 travis    (2000) travis    (2000) 17741146 2024-05-02 03:09:30.000000 timelink-1.1.8/tests/xml_data/test-auc-alunos-264605-A-140337-140771.xml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-02 03:12:30.552323 timelink-1.1.8/timelink/
--rw-rw-r--   0 travis    (2000) travis    (2000)      525 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-02 03:12:30.556323 timelink-1.1.8/timelink/api/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/api/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3158 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/api/crud.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    37696 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/api/database.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-02 03:12:30.560323 timelink-1.1.8/timelink/api/models/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1500 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/api/models/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2768 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/api/models/act.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1669 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/api/models/attribute.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      661 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/api/models/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      798 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/api/models/base_class.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22257 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/api/models/base_mappings.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8693 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/api/models/entity.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1195 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/api/models/object.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1733 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/api/models/person.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24849 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/api/models/pom_som_mapper.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3150 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/api/models/relation.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2499 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/api/models/source.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5806 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/api/models/system.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4146 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/api/schemas.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2209 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/api/views.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-02 03:12:30.560323 timelink-1.1.8/timelink/app/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1713 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/app/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-02 03:12:30.560323 timelink-1.1.8/timelink/app/backend/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/app/backend/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      469 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/app/backend/settings.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20394 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/app/backend/timelink_webapp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3084 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/app/dependencies.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13303 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/app/main.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-02 03:12:30.560323 timelink-1.1.8/timelink/app/models/
--rw-rw-r--   0 travis    (2000) travis    (2000)       92 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/app/models/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3360 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/app/models/project.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5164 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/app/models/user.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21284 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/app/models/user_database.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-02 03:12:30.564324 timelink-1.1.8/timelink/app/schemas/
--rw-rw-r--   0 travis    (2000) travis    (2000)      113 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/app/schemas/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      812 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/app/schemas/project.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1719 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/app/schemas/user.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-02 03:12:30.564324 timelink-1.1.8/timelink/app/services/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/app/services/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2419 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/app/services/auth.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/app/services/syslog.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/app/services/syspar.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-02 03:12:30.564324 timelink-1.1.8/timelink/app/web/
--rw-rw-r--   0 travis    (2000) travis    (2000)     9979 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/app/web/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4664 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/app/web/home_page.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6092 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/app/web/login_page.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2431 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/app/web/projects_page.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1200 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/app/web/webapp_info.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2750 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/cli.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-02 03:12:30.564324 timelink-1.1.8/timelink/kleio/
--rw-rw-r--   0 travis    (2000) travis    (2000)      864 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/kleio/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-02 03:12:30.568324 timelink-1.1.8/timelink/kleio/groups/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4304 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/kleio/groups/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      264 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/kleio/groups/kabstraction.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1183 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/kleio/groups/kact.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      134 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/kleio/groups/katr.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1801 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/kleio/groups/kattribute.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14940 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/kleio/groups/kelement.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    30977 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/kleio/groups/kgroup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      948 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/kleio/groups/kkleio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      132 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/kleio/groups/kls.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1103 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/kleio/groups/kobject.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1026 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/kleio/groups/kperson.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2208 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/kleio/groups/krelation.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1521 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/kleio/groups/ksource.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24544 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/kleio/importer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    37132 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/kleio/kleio_server.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6172 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/kleio/schemas.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1951 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/kleio/utilities.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-02 03:12:30.568324 timelink-1.1.8/timelink/mhk/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/mhk/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-02 03:12:30.572324 timelink-1.1.8/timelink/mhk/models/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1503 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/mhk/models/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1896 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/mhk/models/act.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1699 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/mhk/models/attribute.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      640 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/mhk/models/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      834 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/mhk/models/base_class.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22062 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/mhk/models/base_mappings.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5193 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/mhk/models/db.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6445 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/mhk/models/entity.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1127 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/mhk/models/object.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1093 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/mhk/models/person.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21175 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/mhk/models/pom_som_mapper.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2644 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/mhk/models/relation.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1560 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/mhk/models/source.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4233 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/mhk/models/system.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6119 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/mhk/utilities.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-02 03:12:30.572324 timelink-1.1.8/timelink/networks/
--rw-rw-r--   0 travis    (2000) travis    (2000)       56 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/networks/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2266 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/networks/network_draw.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5950 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/networks/network_generation.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-02 03:12:30.572324 timelink-1.1.8/timelink/notebooks/
--rw-rw-r--   0 travis    (2000) travis    (2000)      539 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/notebooks/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17991 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/notebooks/timelink_notebook.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-02 03:12:30.576325 timelink-1.1.8/timelink/pandas/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1126 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/pandas/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2920 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/pandas/attribute_values.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8167 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/pandas/entities_with_attribute.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6948 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/pandas/group_attributes.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2027 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/pandas/name_to_df.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2174 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/pandas/styles.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       50 2024-05-02 03:09:30.000000 timelink-1.1.8/timelink/timelink.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-02 03:12:30.576325 timelink-1.1.8/timelink.egg-info/
--rw-r--r--   0 travis    (2000) travis    (2000)     4847 2024-05-02 03:12:30.000000 timelink-1.1.8/timelink.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    10397 2024-05-02 03:12:30.000000 timelink-1.1.8/timelink.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-05-02 03:12:30.000000 timelink-1.1.8/timelink.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       46 2024-05-02 03:12:30.000000 timelink-1.1.8/timelink.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-05-02 03:12:30.000000 timelink-1.1.8/timelink.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      253 2024-05-02 03:12:30.000000 timelink-1.1.8/timelink.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        9 2024-05-02 03:12:30.000000 timelink-1.1.8/timelink.egg-info/top_level.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-03 00:07:08.407640 timelink-1.1.9/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      209 2024-05-03 00:03:44.000000 timelink-1.1.9/AUTHORS.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9422 2024-05-03 00:03:44.000000 timelink-1.1.9/CONTRIBUTING.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3488 2024-05-03 00:03:44.000000 timelink-1.1.9/HISTORY.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1084 2024-05-03 00:03:44.000000 timelink-1.1.9/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)      262 2024-05-03 00:03:44.000000 timelink-1.1.9/MANIFEST.in
+-rw-r--r--   0 travis    (2000) travis    (2000)     4942 2024-05-03 00:07:08.407640 timelink-1.1.9/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      507 2024-05-03 00:03:44.000000 timelink-1.1.9/README.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-03 00:07:08.243629 timelink-1.1.9/docs/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      609 2024-05-03 00:03:44.000000 timelink-1.1.9/docs/Makefile
+-rw-rw-r--   0 travis    (2000) travis    (2000)       28 2024-05-03 00:03:44.000000 timelink-1.1.9/docs/authors.rst
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     5433 2024-05-03 00:03:44.000000 timelink-1.1.9/docs/conf.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       33 2024-05-03 00:03:44.000000 timelink-1.1.9/docs/contributing.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      303 2024-05-03 00:03:44.000000 timelink-1.1.9/docs/documentation.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)       28 2024-05-03 00:03:44.000000 timelink-1.1.9/docs/history.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1158 2024-05-03 00:03:44.000000 timelink-1.1.9/docs/index.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1183 2024-05-03 00:03:44.000000 timelink-1.1.9/docs/installation.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      770 2024-05-03 00:03:44.000000 timelink-1.1.9/docs/make.bat
+-rw-rw-r--   0 travis    (2000) travis    (2000)      103 2024-05-03 00:03:44.000000 timelink-1.1.9/docs/modules.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)       27 2024-05-03 00:03:44.000000 timelink-1.1.9/docs/readme.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20745 2024-05-03 00:03:44.000000 timelink-1.1.9/docs/som_pom_mapping.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2081 2024-05-03 00:03:44.000000 timelink-1.1.9/docs/timelink-introduction.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2866 2024-05-03 00:03:44.000000 timelink-1.1.9/docs/timelink-python-usage.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2148 2024-05-03 00:03:44.000000 timelink-1.1.9/docs/timelink.api.models.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      777 2024-05-03 00:03:44.000000 timelink-1.1.9/docs/timelink.api.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      527 2024-05-03 00:03:44.000000 timelink-1.1.9/docs/timelink.app.backend.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      500 2024-05-03 00:03:44.000000 timelink-1.1.9/docs/timelink.app.models.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      604 2024-05-03 00:03:44.000000 timelink-1.1.9/docs/timelink.app.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      489 2024-05-03 00:03:44.000000 timelink-1.1.9/docs/timelink.app.schemas.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      661 2024-05-03 00:03:44.000000 timelink-1.1.9/docs/timelink.app.services.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      823 2024-05-03 00:03:44.000000 timelink-1.1.9/docs/timelink.app.web.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2194 2024-05-03 00:03:44.000000 timelink-1.1.9/docs/timelink.kleio.groups.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      847 2024-05-03 00:03:44.000000 timelink-1.1.9/docs/timelink.kleio.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2296 2024-05-03 00:03:44.000000 timelink-1.1.9/docs/timelink.mhk.models.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      369 2024-05-03 00:03:44.000000 timelink-1.1.9/docs/timelink.mhk.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      523 2024-05-03 00:03:44.000000 timelink-1.1.9/docs/timelink.networks.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      352 2024-05-03 00:03:44.000000 timelink-1.1.9/docs/timelink.notebooks.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      495 2024-05-03 00:03:44.000000 timelink-1.1.9/docs/timelink.pandas.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      565 2024-05-03 00:03:44.000000 timelink-1.1.9/docs/timelink.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      150 2024-05-03 00:03:44.000000 timelink-1.1.9/docs/usage.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      364 2024-05-03 00:03:44.000000 timelink-1.1.9/pyproject.toml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      468 2024-05-03 00:07:08.411641 timelink-1.1.9/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2092 2024-05-03 00:03:44.000000 timelink-1.1.9/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-03 00:07:08.251630 timelink-1.1.9/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2709 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-03 00:07:08.251630 timelink-1.1.9/tests/db/
+-rw-r--r--   0 travis    (2000) travis    (2000)    32768 2024-05-03 00:06:02.000000 timelink-1.1.9/tests/db/test_users.sqlite
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12302 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/test_api_models_db.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      903 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/test_api_models_no_db.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27174 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/test_groups.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3379 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/test_import_MHK.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13671 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/test_import_TL.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10833 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/test_kleio_server.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8920 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/test_mhk_models_db.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      870 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/test_mhk_models_no_db.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3313 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/test_mhk_utilities.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4187 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/test_pandas.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      168 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/test_postgres_db.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1359 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/test_timelink.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8352 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/test_timelink_users.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-03 00:07:08.251630 timelink-1.1.9/tests/timelink-home/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-03 00:07:08.223628 timelink-1.1.9/tests/timelink-home/.kleio/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-03 00:07:08.251630 timelink-1.1.9/tests/timelink-home/.kleio/conf/
+-rw-r--r--   0 travis    (2000) travis    (2000)      726 2024-05-03 00:05:11.000000 timelink-1.1.9/tests/timelink-home/.kleio/conf/token_db
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-03 00:07:08.251630 timelink-1.1.9/tests/timelink-home/.kleio/logs/
+-rw-r--r--   0 travis    (2000) travis    (2000)      867 2024-05-03 00:05:28.000000 timelink-1.1.9/tests/timelink-home/.kleio/logs/kleio_service.log
+-rw-r--r--   0 travis    (2000) travis    (2000)      561 2024-05-03 00:05:26.000000 timelink-1.1.9/tests/timelink-home/.kleio.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-03 00:07:08.251630 timelink-1.1.9/tests/timelink-home/projects/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       71 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/.gitignore
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-03 00:07:08.223628 timelink-1.1.9/tests/timelink-home/projects/test-project/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-03 00:07:08.251630 timelink-1.1.9/tests/timelink-home/projects/test-project/identifications/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16686 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/test-project/identifications/mhk_identification_toliveira.cli
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-03 00:07:08.223628 timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-03 00:07:08.223628 timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-03 00:07:08.255630 timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/linked_data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)   119167 2024-05-03 00:05:23.000000 timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/linked_data/dehergne-a.cli
+-rw-rw-r--   0 travis    (2000) travis    (2000)   119167 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/linked_data/dehergne-a.org
+-rw-rw-r--   0 travis    (2000) travis    (2000)    48349 2024-05-03 00:05:19.000000 timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/linked_data/dehergne-locations-1644.cli
+-rw-rw-r--   0 travis    (2000) travis    (2000)    48349 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/linked_data/dehergne-locations-1644.org
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-03 00:07:08.255630 timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/notariais/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2171 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/notariais/docsregiospontepisc.cli
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    38720 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/notariais/notarial80.cli
+-rw-rw-r--   0 travis    (2000) travis    (2000)    60802 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/notariais/notlousa1.cli
+-rw-rw-r--   0 travis    (2000) travis    (2000)    80615 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/notariais/perdoes.cli
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-03 00:07:08.223628 timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-03 00:07:08.259630 timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/baptismos/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2732 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/baptismos/bap-com-celebrantes.cli
+-rw-rw-r--   0 travis    (2000) travis    (2000)    43942 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/baptismos/bapt1714.cli
+-rw-rw-r--   0 travis    (2000) travis    (2000)    97925 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/baptismos/bapteirasproblem1.cli
+-rw-rw-r--   0 travis    (2000) travis    (2000)   136532 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/baptismos/bapteirasproblem2.cli
+-rw-rw-r--   0 travis    (2000) travis    (2000)      640 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/baptismos/rogeriodomingos_bap_problem.cli
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-03 00:07:08.259630 timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/casamentos/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2034 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/casamentos/cas1714-1722-com-celebrante.cli
+-rw-rw-r--   0 travis    (2000) travis    (2000)    94359 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/casamentos/cas1714-1722.cli
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-03 00:07:08.259630 timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/crisma/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1590 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/crisma/crisma1753.cli
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-03 00:07:08.263630 timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/obitos/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16671 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/obitos/ob1688.cli
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16672 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/obitos/ob1688b.cli
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7263 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/obitos/obit1714.cli
+-rw-rw-r--   0 travis    (2000) travis    (2000)   268277 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/obitos/obiteirasproblem.cli
+-rw-rw-r--   0 travis    (2000) travis    (2000)      842 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/obitos/obitoShort.cli
+-rw-rw-r--   0 travis    (2000) travis    (2000)      793 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/obitos/obitoShort_id.cli
+-rw-rw-r--   0 travis    (2000) travis    (2000)      666 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/obitos/obitoShort_id_id.cli
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1229 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/obitos/testeParentescos.cli
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-03 00:07:08.263630 timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/roisdeconfessados/
+-rw-rw-r--   0 travis    (2000) travis    (2000)   213581 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/roisdeconfessados/coja-rol-1841.cli
+-rw-rw-r--   0 travis    (2000) travis    (2000)    52584 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/roisdeconfessados/eiras-rol1.cli
+-rw-rw-r--   0 travis    (2000) travis    (2000)    51851 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/roisdeconfessados/eiras-rol2.cli
+-rw-rw-r--   0 travis    (2000) travis    (2000)    52776 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/roisdeconfessados/eiras-rol3.cli
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-03 00:07:08.275631 timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3249 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/Devedores.cli
+-rw-rw-r--   0 travis    (2000) travis    (2000)    39369 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/EmpFAfonso.cli
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1381318 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/auc-alunos.cli
+-rw-rw-r--   0 travis    (2000) travis    (2000)   101268 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/auc_cartulario18.cli
+-rw-rw-r--   0 travis    (2000) travis    (2000)    50693 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/eleicoes1.cli
+-rw-rw-r--   0 travis    (2000) travis    (2000)    71568 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/genealdiversas.cli
+-rw-rw-r--   0 travis    (2000) travis    (2000)   103980 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/glopes-lap1561.cli
+-rw-rw-r--   0 travis    (2000) travis    (2000)    48446 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/ivcc.cli
+-rw-rw-r--   0 travis    (2000) travis    (2000)   165942 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/lrazao516pe.cli
+-rw-rw-r--   0 travis    (2000) travis    (2000)    80126 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/misMesa.cli
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3309 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/mp758-santiago-beduido.cli
+-rwxrwxr-x   0 travis    (2000) travis    (2000)   113694 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/nommiz.cli
+-rw-rw-r--   0 travis    (2000) travis    (2000)      674 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/quotes.cli
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1438 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/sourecoimbrabispcoimbra_apontamentosd.cli
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4473 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/vereacao.cli
+-rw-rw-r--   0 travis    (2000) travis    (2000)    49876 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/xpto_comuns_soure.kleio
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-03 00:07:08.279632 timelink-1.1.9/tests/timelink-home/projects/test-project/notebooks/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4628 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/test-project/notebooks/kleio_files.ipynb
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3938 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/test-project/notebooks/kleio_server_version.ipynb
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1270 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/test-project/notebooks/requirements.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)    77283 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/test-project/notebooks/test_entity_with_attributes.ipynb
+-rw-rw-r--   0 travis    (2000) travis    (2000)    89284 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/test-project/notebooks/test_group_attributes.ipynb
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24174 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/test-project/notebooks/test_issue13.ipynb
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3638 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/test-project/notebooks/test_issue26.ipynb
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5838 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/test-project/notebooks/test_pnames.ipynb
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-03 00:07:08.279632 timelink-1.1.9/tests/timelink-home/projects/test-project/structures/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-03 00:07:08.227628 timelink-1.1.9/tests/timelink-home/projects/test-project/structures/sources/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-03 00:07:08.227628 timelink-1.1.9/tests/timelink-home/projects/test-project/structures/sources/reference_sources/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-03 00:07:08.227628 timelink-1.1.9/tests/timelink-home/projects/test-project/structures/sources/reference_sources/paroquiais/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-03 00:07:08.279632 timelink-1.1.9/tests/timelink-home/projects/test-project/structures/sources/reference_sources/paroquiais/casamentos/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    99663 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/test-project/structures/sources/reference_sources/paroquiais/casamentos/cas1714-1722.str
+-rw-rw-r--   0 travis    (2000) travis    (2000)   100155 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/test-project/structures/sources.str
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-03 00:07:08.227628 timelink-1.1.9/tests/timelink-home/projects/tutorial/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-03 00:07:08.283632 timelink-1.1.9/tests/timelink-home/projects/tutorial/kleio/
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1381319 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/tutorial/kleio/auc-alunos.cli
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17236 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/tutorial/kleio/b1685.cli
+-rw-rw-r--   0 travis    (2000) travis    (2000)   119167 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/tutorial/kleio/dehergne-a.cli
+-rw-rw-r--   0 travis    (2000) travis    (2000)    48311 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/tutorial/kleio/dehergne-locations-1644.cli
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27101 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/tutorial/kleio/dehergne-locations-1701.cli
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-03 00:07:08.287632 timelink-1.1.9/tests/timelink-home/projects/tutorial/notebooks/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    52594 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/tutorial/notebooks/0-kleio-files.ipynb
+-rw-rw-r--   0 travis    (2000) travis    (2000)   138142 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/tutorial/notebooks/0-tutorial.ipynb
+-rw-rw-r--   0 travis    (2000) travis    (2000)   230699 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/tutorial/notebooks/1-receipts.ipynb
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1041 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/tutorial/notebooks/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1270 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/timelink-home/projects/tutorial/notebooks/requirements.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-03 00:07:08.299633 timelink-1.1.9/tests/xml_data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17236 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/xml_data/b1685.cli
+-rw-rw-r--   0 travis    (2000) travis    (2000)   756798 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/xml_data/b1685.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)  2037922 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/xml_data/dehergne-a.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)   930555 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/xml_data/dehergne-locations-1644.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)    66759 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/xml_data/dev1692.cli
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1485749 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/xml_data/dev1692.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)   116461 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/xml_data/mhk_identification_toliveira.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)    49771 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/xml_data/test-atr-date.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000) 17741146 2024-05-03 00:03:44.000000 timelink-1.1.9/tests/xml_data/test-auc-alunos-264605-A-140337-140771.xml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-03 00:07:08.335636 timelink-1.1.9/timelink/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      525 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-03 00:07:08.343636 timelink-1.1.9/timelink/api/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/api/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3158 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/api/crud.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37696 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/api/database.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-03 00:07:08.343636 timelink-1.1.9/timelink/api/models/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1500 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/api/models/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3036 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/api/models/act.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1909 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/api/models/attribute.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      661 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/api/models/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      798 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/api/models/base_class.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22257 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/api/models/base_mappings.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8905 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/api/models/entity.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1332 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/api/models/object.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1981 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/api/models/person.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24849 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/api/models/pom_som_mapper.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3106 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/api/models/relation.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2739 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/api/models/source.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5806 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/api/models/system.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4146 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/api/schemas.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2209 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/api/views.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-03 00:07:08.347636 timelink-1.1.9/timelink/app/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1713 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/app/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-03 00:07:08.347636 timelink-1.1.9/timelink/app/backend/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/app/backend/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      469 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/app/backend/settings.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20394 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/app/backend/timelink_webapp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3084 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/app/dependencies.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13303 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/app/main.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-03 00:07:08.351637 timelink-1.1.9/timelink/app/models/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       92 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/app/models/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3360 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/app/models/project.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5164 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/app/models/user.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21284 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/app/models/user_database.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-03 00:07:08.355637 timelink-1.1.9/timelink/app/schemas/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      113 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/app/schemas/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      812 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/app/schemas/project.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1719 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/app/schemas/user.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-03 00:07:08.359637 timelink-1.1.9/timelink/app/services/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/app/services/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2419 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/app/services/auth.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/app/services/syslog.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/app/services/syspar.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-03 00:07:08.367638 timelink-1.1.9/timelink/app/web/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9979 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/app/web/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4664 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/app/web/home_page.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6092 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/app/web/login_page.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2431 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/app/web/projects_page.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1200 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/app/web/webapp_info.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2750 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/cli.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-03 00:07:08.371638 timelink-1.1.9/timelink/kleio/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      864 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/kleio/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-03 00:07:08.379639 timelink-1.1.9/timelink/kleio/groups/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4304 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/kleio/groups/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      264 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/kleio/groups/kabstraction.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1183 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/kleio/groups/kact.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      134 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/kleio/groups/katr.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1801 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/kleio/groups/kattribute.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14940 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/kleio/groups/kelement.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30977 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/kleio/groups/kgroup.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      948 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/kleio/groups/kkleio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      132 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/kleio/groups/kls.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1103 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/kleio/groups/kobject.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1026 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/kleio/groups/kperson.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2208 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/kleio/groups/krelation.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1521 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/kleio/groups/ksource.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24544 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/kleio/importer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37132 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/kleio/kleio_server.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6172 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/kleio/schemas.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1951 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/kleio/utilities.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-03 00:07:08.379639 timelink-1.1.9/timelink/mhk/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/mhk/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-03 00:07:08.395640 timelink-1.1.9/timelink/mhk/models/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1503 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/mhk/models/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1896 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/mhk/models/act.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1699 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/mhk/models/attribute.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      640 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/mhk/models/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      834 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/mhk/models/base_class.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22062 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/mhk/models/base_mappings.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5193 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/mhk/models/db.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6445 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/mhk/models/entity.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1127 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/mhk/models/object.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1093 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/mhk/models/person.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21175 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/mhk/models/pom_som_mapper.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2644 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/mhk/models/relation.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1560 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/mhk/models/source.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4233 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/mhk/models/system.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6119 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/mhk/utilities.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-03 00:07:08.395640 timelink-1.1.9/timelink/networks/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       56 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/networks/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2266 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/networks/network_draw.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5950 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/networks/network_generation.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-03 00:07:08.395640 timelink-1.1.9/timelink/notebooks/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      539 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/notebooks/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17991 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/notebooks/timelink_notebook.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-03 00:07:08.399640 timelink-1.1.9/timelink/pandas/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1126 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/pandas/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2920 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/pandas/attribute_values.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8167 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/pandas/entities_with_attribute.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6948 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/pandas/group_attributes.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2027 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/pandas/name_to_df.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2174 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/pandas/styles.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       50 2024-05-03 00:03:44.000000 timelink-1.1.9/timelink/timelink.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-03 00:07:08.403640 timelink-1.1.9/timelink.egg-info/
+-rw-r--r--   0 travis    (2000) travis    (2000)     4942 2024-05-03 00:07:08.000000 timelink-1.1.9/timelink.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10397 2024-05-03 00:07:08.000000 timelink-1.1.9/timelink.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-05-03 00:07:08.000000 timelink-1.1.9/timelink.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       46 2024-05-03 00:07:08.000000 timelink-1.1.9/timelink.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-05-03 00:07:08.000000 timelink-1.1.9/timelink.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)      253 2024-05-03 00:07:08.000000 timelink-1.1.9/timelink.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        9 2024-05-03 00:07:08.000000 timelink-1.1.9/timelink.egg-info/top_level.txt
```

### Comparing `timelink-1.1.8/CONTRIBUTING.rst` & `timelink-1.1.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/HISTORY.rst` & `timelink-1.1.9/HISTORY.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 =======
 History
 =======
+
+1.1.9 (2024-05-03)
+------------------
+
+* fix bug with to_kleio() in models (bad identation)
+
+
 1.1.8 (2024-05-02)
 ------------------
 
 * Fix bug with export_to_kleio()
 * Several minor bug fixes
 
 1.1.7 (2024-04-28)
```

### Comparing `timelink-1.1.8/LICENSE` & `timelink-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/PKG-INFO` & `timelink-1.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timelink
-Version: 1.1.8
+Version: 1.1.9
 Summary: Timelink is an information system for person related information collected from historical sources. 
 Home-page: https://github.com/time-link/timelink-py
 Author: Joaquim Ramos de Carvalho
 Author-email: joaquimcarvalho@ipm.edu.mo
 License: MIT license
 Project-URL: Documentation, https://timelink-py.readthedocs.io/
 Keywords: timelink
@@ -41,14 +41,21 @@
 Requires-Dist: uvicorn
 
 Timelink is an information system for person related information collected from historical sources. 
 
 =======
 History
 =======
+
+1.1.9 (2024-05-03)
+------------------
+
+* fix bug with to_kleio() in models (bad identation)
+
+
 1.1.8 (2024-05-02)
 ------------------
 
 * Fix bug with export_to_kleio()
 * Several minor bug fixes
 
 1.1.7 (2024-04-28)
```

### Comparing `timelink-1.1.8/docs/Makefile` & `timelink-1.1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/docs/conf.py` & `timelink-1.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/docs/index.rst` & `timelink-1.1.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/docs/installation.rst` & `timelink-1.1.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/docs/make.bat` & `timelink-1.1.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/docs/som_pom_mapping.rst` & `timelink-1.1.9/docs/som_pom_mapping.rst`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/docs/timelink-introduction.rst` & `timelink-1.1.9/docs/timelink-introduction.rst`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/docs/timelink-python-usage.rst` & `timelink-1.1.9/docs/timelink-python-usage.rst`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/docs/timelink.api.models.rst` & `timelink-1.1.9/docs/timelink.api.models.rst`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/docs/timelink.api.rst` & `timelink-1.1.9/docs/timelink.api.rst`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/docs/timelink.app.backend.rst` & `timelink-1.1.9/docs/timelink.app.backend.rst`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/docs/timelink.app.rst` & `timelink-1.1.9/docs/timelink.app.rst`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/docs/timelink.app.services.rst` & `timelink-1.1.9/docs/timelink.app.services.rst`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/docs/timelink.app.web.rst` & `timelink-1.1.9/docs/timelink.app.web.rst`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/docs/timelink.kleio.groups.rst` & `timelink-1.1.9/docs/timelink.kleio.groups.rst`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/docs/timelink.kleio.rst` & `timelink-1.1.9/docs/timelink.kleio.rst`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/docs/timelink.mhk.models.rst` & `timelink-1.1.9/docs/timelink.mhk.models.rst`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/docs/timelink.networks.rst` & `timelink-1.1.9/docs/timelink.networks.rst`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/docs/timelink.rst` & `timelink-1.1.9/docs/timelink.rst`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/setup.py` & `timelink-1.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,10 +66,10 @@
     include_package_data=True,
     keywords='timelink',
     name='timelink',
     packages=find_packages(include=['timelink', 'timelink.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/time-link/timelink-py',
-    version='1.1.8',
+    version='1.1.9',
     zip_safe=False,
 )
```

### Comparing `timelink-1.1.8/tests/__init__.py` & `timelink-1.1.9/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/db/test_users.sqlite` & `timelink-1.1.9/tests/db/test_users.sqlite`

 * *Files 19% similar despite different names*

#### sqlite3 {} .dump

```diff
@@ -8,43 +8,43 @@
 	hashed_password VARCHAR, 
 	disabled BOOLEAN, 
 	created DATETIME NOT NULL, 
 	updated DATETIME, 
 	PRIMARY KEY (id), 
 	UNIQUE (email)
 );
-INSERT INTO users VALUES(1,'User One','One(1)','one@xpto.com',NULL,0,'2024-05-02 03:11:40','2024-05-02 03:11:41');
-INSERT INTO users VALUES(2,'User 2','NumberTwo','two@xpto.com',NULL,0,'2024-05-02 03:11:41','2024-05-02 03:11:41');
-INSERT INTO users VALUES(3,'User 3','三','san@xpto.org',NULL,0,'2024-05-02 03:11:41','2024-05-02 03:11:41');
-INSERT INTO users VALUES(4,'Quarto Utilizador','Test Nickname','four@xpto.com',NULL,0,'2024-05-02 03:11:41','2024-05-02 03:11:41');
-INSERT INTO users VALUES(5,'User five','five','five@xpto.com',NULL,0,'2024-05-02 03:11:41','2024-05-02 03:11:41');
-INSERT INTO users VALUES(6,'Project User one','PU1','project_user_one@xpto.com',NULL,0,'2024-05-02 03:11:41','2024-05-02 03:11:41');
+INSERT INTO users VALUES(1,'User One','One(1)','one@xpto.com',NULL,0,'2024-05-03 00:06:01','2024-05-03 00:06:02');
+INSERT INTO users VALUES(2,'User 2','NumberTwo','two@xpto.com',NULL,0,'2024-05-03 00:06:02','2024-05-03 00:06:02');
+INSERT INTO users VALUES(3,'User 3','三','san@xpto.org',NULL,0,'2024-05-03 00:06:02','2024-05-03 00:06:02');
+INSERT INTO users VALUES(4,'Quarto Utilizador','Test Nickname','four@xpto.com',NULL,0,'2024-05-03 00:06:02','2024-05-03 00:06:02');
+INSERT INTO users VALUES(5,'User five','five','five@xpto.com',NULL,0,'2024-05-03 00:06:02','2024-05-03 00:06:02');
+INSERT INTO users VALUES(6,'Project User one','PU1','project_user_one@xpto.com',NULL,0,'2024-05-03 00:06:02','2024-05-03 00:06:02');
 CREATE TABLE projects (
 	id INTEGER NOT NULL, 
 	name VARCHAR(30) NOT NULL, 
 	description VARCHAR(4096), 
 	"databaseURL" VARCHAR(256), 
 	"kleioServerURL" VARCHAR(256), 
 	created DATETIME NOT NULL, 
 	updated DATETIME NOT NULL, 
 	PRIMARY KEY (id), 
 	UNIQUE (id), 
 	UNIQUE (name)
 );
-INSERT INTO projects VALUES(1,'Project One','Project One description',NULL,NULL,'2024-05-02 03:11:41','2024-05-02 03:11:41');
+INSERT INTO projects VALUES(1,'Project One','Project One description',NULL,NULL,'2024-05-03 00:06:02','2024-05-03 00:06:02');
 CREATE TABLE user_properties (
 	id INTEGER NOT NULL, 
 	name VARCHAR(30) NOT NULL, 
 	value VARCHAR(30) NOT NULL, 
 	user_id INTEGER NOT NULL, 
 	PRIMARY KEY (id), 
 	FOREIGN KEY(user_id) REFERENCES users (id)
 );
-INSERT INTO user_properties VALUES(1,'property1','OM38Y6PCSH',1);
-INSERT INTO user_properties VALUES(2,'property2','S7TTY98G5A',1);
+INSERT INTO user_properties VALUES(1,'property1','4Y3Y57QLBJ',1);
+INSERT INTO user_properties VALUES(2,'property2','2O2UXYPM0Z',1);
 INSERT INTO user_properties VALUES(3,'property1','value1',3);
 INSERT INTO user_properties VALUES(4,'property2','value2',3);
 CREATE TABLE user_project_access (
 	id INTEGER NOT NULL, 
 	user_id INTEGER NOT NULL, 
 	project_id INTEGER NOT NULL, 
 	access_level VARCHAR(11) NOT NULL,
```

### Comparing `timelink-1.1.8/tests/test_api_models_db.py` & `timelink-1.1.9/tests/test_api_models_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -297,15 +297,19 @@
     """Test exporting entities as Kleio"""
     ks = kgroup_person_attr_rel
     source_id = ks.get_id()
     with get_db.session() as session:
         PomSomMapper.store_KGroup(ks, session)
         session.commit()
         source_from_db = Entity.get_entity(source_id, session)
+        ksource = source_from_db.to_kleio(ident_inc="...")
+        assert ksource
         act = source_from_db.contains[0]
+        kact = act.to_kleio()
+        assert kact
         people = act.contains
         people_ids = [person.id for person in people]
         get_db.export_as_kleio(people_ids, 'tests/test_kleio_export.txt')
         assert os.path.exists('tests/test_kleio_export.txt')
         # read the file
         with open('tests/test_kleio_export.txt', 'r') as f:
             kleio = f.read()
```

### Comparing `timelink-1.1.8/tests/test_api_models_no_db.py` & `timelink-1.1.9/tests/test_api_models_no_db.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/test_groups.py` & `timelink-1.1.9/tests/test_groups.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/test_import_MHK.py` & `timelink-1.1.9/tests/test_import_MHK.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/test_import_TL.py` & `timelink-1.1.9/tests/test_import_TL.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/test_kleio_server.py` & `timelink-1.1.9/tests/test_kleio_server.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/test_mhk_models_db.py` & `timelink-1.1.9/tests/test_mhk_models_db.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/test_mhk_models_no_db.py` & `timelink-1.1.9/tests/test_mhk_models_no_db.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/test_mhk_utilities.py` & `timelink-1.1.9/tests/test_mhk_utilities.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/test_pandas.py` & `timelink-1.1.9/tests/test_pandas.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/test_timelink.py` & `timelink-1.1.9/tests/test_timelink.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/test_timelink_users.py` & `timelink-1.1.9/tests/test_timelink_users.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/timelink-home/.kleio/conf/token_db` & `timelink-1.1.9/tests/timelink-home/.kleio/conf/token_db`

 * *Files 13% similar despite different names*

```diff
@@ -1,3 +1,3 @@
-created(1714619449.4311173).
-assert(user_token(ba9e10acf7b4bda6594698a2e7ddfdbcee119ffa,limited_user,[created(1714619449.4253807),comment('An user that has no privileges, used to test authorization errors'),api([]),structures('projects/test-project/structures'),sources('projects/test-project/sources')])).
-assert(user_token(e576cbf80c613dfdcfb8342a9061250529e68878,normal_user,[created(1714619449.5104694),comment('An user able to translate, upload and delete files, and also create and remove directories, in specific sub-directories in kleio-home'),api([sources,kleioset,files,structures,translations,upload,delete,mkdir,rmdir]),structures('projects/test-project/structures'),sources('projects/test-project/sources')])).
+created(1714694711.0300004).
+assert(user_token(fba5ae00ba916fa588c812df0b24af3756eb1c00,limited_user,[created(1714694711.0241544),comment('An user that has no privileges, used to test authorization errors'),api([]),structures('projects/test-project/structures'),sources('projects/test-project/sources')])).
+assert(user_token('57856ea2f393dfaab705714e47dc6fb13bbdaf3d',normal_user,[created(1714694711.1174417),comment('An user able to translate, upload and delete files, and also create and remove directories, in specific sub-directories in kleio-home'),api([sources,kleioset,files,structures,translations,upload,delete,mkdir,rmdir]),structures('projects/test-project/structures'),sources('projects/test-project/sources')])).
```

### Comparing `timelink-1.1.8/tests/timelink-home/.kleio.json` & `timelink-1.1.9/tests/timelink-home/.kleio.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9583333333333334%*

 * *Differences: {"'kleio_setup_date'": "'2024-05-03T00:05:26+0000'"}*

```diff
@@ -2,13 +2,13 @@
     "keio_version_date": "2024-02-29 07:39:02",
     "kleio_admin_token": "0123456789",
     "kleio_admin_token_path": "/kleio-home/systems/conf/kleio/.admin_token",
     "kleio_conf_dir": "/kleio-home/systems/conf/kleio",
     "kleio_home": "/kleio-home",
     "kleio_home_local": null,
     "kleio_log": "/kleio-home/.kleio/logs//kleio_service.log",
-    "kleio_setup_date": "2024-05-02T03:11:04+0000",
+    "kleio_setup_date": "2024-05-03T00:05:26+0000",
     "kleio_token_db_status": "No tokens defined but KLEIO_ADMIN_TOKEN env has valid value",
     "kleio_url": "http://localhost:8089",
     "kleio_version": "12.5",
     "kleio_version_build": "570"
 }
```

### Comparing `timelink-1.1.8/tests/timelink-home/projects/test-project/identifications/mhk_identification_toliveira.cli` & `timelink-1.1.9/tests/timelink-home/projects/test-project/identifications/mhk_identification_toliveira.cli`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/linked_data/dehergne-a.cli` & `timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/linked_data/dehergne-a.cli`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-kleio$gacto2.str/translations=207
+kleio$gacto2.str/translations=210
    link$wikidata/"https://www.wikidata.org/wiki/$1"/id=root-lin2-171
    fonte$dehergne-a/1973/Dicionário Biográfico/loc=Online archive.org:details:bhsi37/obs=Dehergne, Joseph, Répertoire des Jésuites de Chine, de 1542 à 1800, 1973. Letra A - Entradas relacionadas com Coimbra.
 
       lista$dehergne-notices-a/0/0/0
 
          n$António de Abreu/id=deh-antonio-de-abreu
             ls$nacionalidade/Portugal
```

### Comparing `timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/linked_data/dehergne-a.org` & `timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/linked_data/dehergne-a.org`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-kleio$gacto2.str/translations=206
+kleio$gacto2.str/translations=209
    link$wikidata/"https://www.wikidata.org/wiki/$1"/id=root-lin2-171
    fonte$dehergne-a/1973/Dicionário Biográfico/loc=Online archive.org:details:bhsi37/obs=Dehergne, Joseph, Répertoire des Jésuites de Chine, de 1542 à 1800, 1973. Letra A - Entradas relacionadas com Coimbra.
 
       lista$dehergne-notices-a/0/0/0
 
          n$António de Abreu/id=deh-antonio-de-abreu
             ls$nacionalidade/Portugal
```

### Comparing `timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/linked_data/dehergne-locations-1644.cli` & `timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/linked_data/dehergne-locations-1644.cli`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-kleio$gacto2.str/translations=82
+kleio$gacto2.str/translations=85
    link$wikidata/"https://www.wikidata.org/wiki/$1"/id=root-lin2-44
    link$geonames/"https://www.geonames.org/$1"/id=root-lin2-45
    fonte$dehergne-locations-1644/1644/geoinformation/substitui=dehergne-map-1644/obs="""
       Planche: Carte des Chrétientés Chinoises de la fin des Ming (1644).p. 353
       
       _Diocèse_
       Depuis 1514, l'évêché de Funchal (île de Madère)
```

### Comparing `timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/linked_data/dehergne-locations-1644.org` & `timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/linked_data/dehergne-locations-1644.org`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-kleio$gacto2.str/translations=81
+kleio$gacto2.str/translations=84
    link$wikidata/"https://www.wikidata.org/wiki/$1"/id=root-lin2-44
    link$geonames/"https://www.geonames.org/$1"/id=root-lin2-45
    fonte$dehergne-locations-1644/1644/geoinformation/substitui=dehergne-map-1644/obs="""
       Planche: Carte des Chrétientés Chinoises de la fin des Ming (1644).p. 353
       
       _Diocèse_
       Depuis 1514, l'évêché de Funchal (île de Madère)
```

### Comparing `timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/notariais/docsregiospontepisc.cli` & `timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/notariais/docsregiospontepisc.cli`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/notariais/notarial80.cli` & `timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/notariais/notarial80.cli`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/notariais/notlousa1.cli` & `timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/notariais/notlousa1.cli`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/notariais/perdoes.cli` & `timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/notariais/perdoes.cli`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/baptismos/bap-com-celebrantes.cli` & `timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/baptismos/bap-com-celebrantes.cli`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/baptismos/bapt1714.cli` & `timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/baptismos/bapt1714.cli`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/baptismos/bapteirasproblem1.cli` & `timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/baptismos/bapteirasproblem1.cli`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/baptismos/bapteirasproblem2.cli` & `timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/baptismos/bapteirasproblem2.cli`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/baptismos/rogeriodomingos_bap_problem.cli` & `timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/baptismos/rogeriodomingos_bap_problem.cli`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/casamentos/cas1714-1722-com-celebrante.cli` & `timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/casamentos/cas1714-1722-com-celebrante.cli`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/casamentos/cas1714-1722.cli` & `timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/casamentos/cas1714-1722.cli`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/crisma/crisma1753.cli` & `timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/crisma/crisma1753.cli`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/obitos/ob1688.cli` & `timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/obitos/ob1688.cli`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/obitos/ob1688b.cli` & `timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/obitos/ob1688b.cli`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/obitos/obit1714.cli` & `timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/obitos/obit1714.cli`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/obitos/obiteirasproblem.cli` & `timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/obitos/obiteirasproblem.cli`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/obitos/obitoShort.cli` & `timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/obitos/obitoShort.cli`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/obitos/obitoShort_id.cli` & `timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/obitos/obitoShort_id.cli`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/obitos/obitoShort_id_id.cli` & `timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/obitos/obitoShort_id_id.cli`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/obitos/testeParentescos.cli` & `timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/paroquiais/obitos/testeParentescos.cli`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/roisdeconfessados/coja-rol-1841.cli` & `timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/roisdeconfessados/coja-rol-1841.cli`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/roisdeconfessados/eiras-rol1.cli` & `timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/roisdeconfessados/eiras-rol1.cli`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/roisdeconfessados/eiras-rol2.cli` & `timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/roisdeconfessados/eiras-rol2.cli`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/roisdeconfessados/eiras-rol3.cli` & `timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/roisdeconfessados/eiras-rol3.cli`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/Devedores.cli` & `timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/Devedores.cli`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/EmpFAfonso.cli` & `timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/EmpFAfonso.cli`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/auc-alunos.cli` & `timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/auc-alunos.cli`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/auc_cartulario18.cli` & `timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/auc_cartulario18.cli`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/eleicoes1.cli` & `timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/eleicoes1.cli`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/genealdiversas.cli` & `timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/genealdiversas.cli`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/glopes-lap1561.cli` & `timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/glopes-lap1561.cli`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/ivcc.cli` & `timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/ivcc.cli`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/lrazao516pe.cli` & `timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/lrazao516pe.cli`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/misMesa.cli` & `timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/misMesa.cli`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/mp758-santiago-beduido.cli` & `timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/mp758-santiago-beduido.cli`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/nommiz.cli` & `timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/nommiz.cli`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/quotes.cli` & `timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/quotes.cli`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/sourecoimbrabispcoimbra_apontamentosd.cli` & `timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/sourecoimbrabispcoimbra_apontamentosd.cli`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/vereacao.cli` & `timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/vereacao.cli`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/xpto_comuns_soure.kleio` & `timelink-1.1.9/tests/timelink-home/projects/test-project/kleio/reference_sources/varia/xpto_comuns_soure.kleio`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/timelink-home/projects/test-project/notebooks/kleio_files.ipynb` & `timelink-1.1.9/tests/timelink-home/projects/test-project/notebooks/kleio_files.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9976230158730159%*

 * *Differences: {"'cells'": "{1: {'outputs': {0: {'text': {insert: [(1, 'Token: kM1C\\n')], delete: [1]}}}}, 3: "*

 * *            "{'execution_count': 9}}",*

 * * "'metadata'": "{'language_info': {'version': '3.11.1'}}"}*

```diff
@@ -14,15 +14,15 @@
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Kleio Home Found: /Users/jrc/develop/timelink-py/tests/timelink-home/projects/test-project\n",
-                        "Token: l4cI\n",
+                        "Token: kM1C\n",
                         "URL: http://127.0.0.1:8088\n",
                         "Kleio Home: /Users/jrc/develop/timelink-py/tests/timelink-home/projects/test-project\n"
                     ]
                 }
             ],
             "source": [
                 "# NBVAL_IGNORE_OUTPUT\n",
@@ -49,15 +49,15 @@
             "metadata": {},
             "source": [
                 "# get the list of files in the directory"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 9,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from typing import List\n",
                 "from timelink.kleio.schemas import KleioFile\n",
                 "\n",
                 "kfiles: List[KleioFile] = kserver.translation_status(path='sources',recurse='yes',status=None)\n",
@@ -173,14 +173,14 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.9"
+            "version": "3.11.1"
         },
         "orig_nbformat": 4
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `timelink-1.1.8/tests/timelink-home/projects/test-project/notebooks/kleio_server_version.ipynb` & `timelink-1.1.9/tests/timelink-home/projects/test-project/notebooks/kleio_server_version.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9977678571428572%*

 * *Differences: {"'metadata'": "{'language_info': {'version': '3.11.1'}}"}*

```diff
@@ -106,13 +106,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.9"
+            "version": "3.11.1"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `timelink-1.1.8/tests/timelink-home/projects/test-project/notebooks/requirements.txt` & `timelink-1.1.9/tests/timelink-home/projects/test-project/notebooks/requirements.txt`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/timelink-home/projects/test-project/notebooks/test_entity_with_attributes.ipynb` & `timelink-1.1.9/tests/timelink-home/projects/test-project/notebooks/test_entity_with_attributes.ipynb`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/timelink-home/projects/test-project/notebooks/test_group_attributes.ipynb` & `timelink-1.1.9/tests/timelink-home/projects/test-project/notebooks/test_group_attributes.ipynb`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/timelink-home/projects/test-project/notebooks/test_issue13.ipynb` & `timelink-1.1.9/tests/timelink-home/projects/test-project/notebooks/test_issue13.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9977678571428572%*

 * *Differences: {"'metadata'": "{'language_info': {'version': '3.11.1'}}"}*

```diff
@@ -581,13 +581,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.9"
+            "version": "3.11.1"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `timelink-1.1.8/tests/timelink-home/projects/test-project/notebooks/test_issue26.ipynb` & `timelink-1.1.9/tests/timelink-home/projects/test-project/notebooks/test_issue26.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9977678571428572%*

 * *Differences: {"'metadata'": "{'language_info': {'version': '3.11.1'}}"}*

```diff
@@ -95,13 +95,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.9"
+            "version": "3.11.1"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `timelink-1.1.8/tests/timelink-home/projects/test-project/notebooks/test_pnames.ipynb` & `timelink-1.1.9/tests/timelink-home/projects/test-project/notebooks/test_pnames.ipynb`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/timelink-home/projects/test-project/structures/sources/reference_sources/paroquiais/casamentos/cas1714-1722.str` & `timelink-1.1.9/tests/timelink-home/projects/test-project/structures/sources/reference_sources/paroquiais/casamentos/cas1714-1722.str`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/timelink-home/projects/test-project/structures/sources.str` & `timelink-1.1.9/tests/timelink-home/projects/test-project/structures/sources.str`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/timelink-home/projects/tutorial/kleio/auc-alunos.cli` & `timelink-1.1.9/tests/timelink-home/projects/tutorial/kleio/auc-alunos.cli`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 kleio$gacto2.str/"""
       Generated from Archeevo export file:  database/other_exports/ficheiro-alunos-auc/PT-AUC-ELU-UC-AUC-B-001-001.CSV dated 2022-02-03 14:43
-  """/translations=9
+  """/translations=10
    fonte$auc-alunos/"PT/AUC/ELU/UC-AUC/B/001-001"/data=1537-00-00:1919-11-14/loc=Arquivo da Universidade de Coimbra/substitui=auc-alunos-264605-A-140337-140771/tipo=UC-AUC-ficheiro-alunos/obs="""
        Âmbito e conteúdo
 
        O índice de alunos da Universidade de Coimbra, também conhecido, apenas, como ficheiro de alunos, foi elaborado entre 1940 e 1950, pelos funcionários do Arquivo, por decisão do doutor Mário Brandão, então diretor do Arquivo da Universidade, como o atestam os relatórios de atividades enviados anualmente ao reitor da Universidade (v. Correspondência expedida do Arquivo (SR), cx.2 (1942-1947) e cx. 3 (1948-1951) – cota AUC-IV-2.ªE-10-2-18 e 19).
        Os citados relatórios revelam, por exemplo, que em 1941-1942 foram elaboradas fichas relativas aos livros de matrículas de 1720 a 1756, num total de 23.400 verbetes, em 1942-1943 foram elaboradas fichas dos livros de 1685 a 1719 num total de 25.000 verbetes, etc.
        Engloba dados relativos aos alunos que frequentaram a Universidade, com menção da sua naturalidade e filiação (apenas o nome do pai). No caso de alunos de ordens religiosas apenas apresentam a indicação da ordem religiosa a que pertenciam (por vezes, de forma generalizada, como, por exemplo “religioso de Santa cruz, religioso de S. Bento”) uma vez que os dados de naturalidade e de filiação destes alunos não ficaram registados nos livros originais de matrículas ou de livros de atos e graus e provas de curso.
        Inclui as datas de matrícula na Universidade, desde 1537, na cadeira de Instituta (a partir de 1772, deixa de existir esta cadeira) e nas diversas faculdades: Teologia, Cânones, Leis, Medicina; em 1772 foram criadas a Faculdade de Matemática e a Faculdade de Filosofia e a partir de 1834 a Faculdade de Cânones e a Faculdade de Leis fundiram-se, dando origem à Faculdade de Direito. Inclui também datas de provas de curso e datas de exames e graus.
```

### Comparing `timelink-1.1.8/tests/timelink-home/projects/tutorial/kleio/b1685.cli` & `timelink-1.1.9/tests/timelink-home/projects/tutorial/kleio/b1685.cli`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-kleio$gacto2.str/translations=40
+kleio$gacto2.str/translations=41
    fonte$baptismos 1685/tipo=reg paroquiais/localizacao=fol. 30-34/data=16850000/obs=existem baptismos anteriores mas em muito mau estado.#VERSAO ABREVIADA. USAR O TRADUTOR CORRECTO
 
       bap$b1685.1/8/7/1685/?/manuel cordeiro
 
          n$maria/f/id=b1685.1-per1
 
             pai$manuel madeira/m/id=b1685.1-per1-per2
```

### Comparing `timelink-1.1.8/tests/timelink-home/projects/tutorial/kleio/dehergne-a.cli` & `timelink-1.1.9/tests/timelink-home/projects/tutorial/kleio/dehergne-a.cli`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-kleio$gacto2.str/translations=184
+kleio$gacto2.str/translations=185
    link$wikidata/"https://www.wikidata.org/wiki/$1"/id=root-lin2-171
    fonte$dehergne-a/1973/Dicionário Biográfico/loc=Online archive.org:details:bhsi37/obs=Dehergne, Joseph, Répertoire des Jésuites de Chine, de 1542 à 1800, 1973. Letra A - Entradas relacionadas com Coimbra.
 
       lista$dehergne-notices-a/0/0/0
 
          n$António de Abreu/id=deh-antonio-de-abreu
             ls$nacionalidade/Portugal
```

### Comparing `timelink-1.1.8/tests/timelink-home/projects/tutorial/kleio/dehergne-locations-1644.cli` & `timelink-1.1.9/tests/timelink-home/projects/tutorial/kleio/dehergne-locations-1644.cli`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-kleio$gacto2.str/translations=56
+kleio$gacto2.str/translations=57
    link$wikidata/"https://www.wikidata.org/wiki/$1"/id=root-lin2-44
    link$geonames/"https://www.geonames.org/$1"/id=root-lin2-45
    fonte$dehergne-locations-1644/1644/geoinformation/substitui=dehergne-map-1644/obs="""
       Planche: Carte des Chrétientés Chinoises de la fin des Ming (1644).p. 353
 
       _Diocèse_
       Depuis 1514, l'évêché de Funchal (île de Madère)
```

### Comparing `timelink-1.1.8/tests/timelink-home/projects/tutorial/kleio/dehergne-locations-1701.cli` & `timelink-1.1.9/tests/timelink-home/projects/tutorial/kleio/dehergne-locations-1701.cli`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-kleio$gacto2.str/translations=10
+kleio$gacto2.str/translations=11
    link$wikidata/"https://www.wikidata.org/wiki/$1"/id=root-lin3-7
    fonte$dehergne-locations-1701/1701/geoinformation/obs="""p. 357        Depuis le 17 août 1658 est créé le vicariat apostolique de Nankin;         puis celui de Cochinchine, et celui du Tonkin; chacun d'eux a         l'administration de plusieurs provinces chinoises. L'ensemble         est remodelé en 1680. Le 10 avril 1690 sont créés les évêchés de         Nankin et de Pékin, qui forment, avec Macao, les trois évêchés du Padroado.         Le 15 oct. 1696, nouvelle redistribution des provinces de Chine,         avec, peu après, création de nouveaux vicariats apostoliques:         Shensi, Kiangsi, Fukien, Szechwan, Yunnan, en 1696;         Hukwang, et Chekiang en 1697; Kweichow, en 1701 (et Shansi en 1702).         Cf Moidrey, p. 253.        Depuis le 30 nov. 1700 la mission française des jésuites de Chine,         dont le supérieur a les pouvoirs de vice-provincial, se partage avec        la vice-province jésuite (dite portugaise) un certain nombre de résidences        éparpillées dans l'empire.        N..B La carte ci-jointe de 1701, hâtivement tracée, a oublié de marquer         le trait conduisant du Collège de Hangchow aux deux résidences jésuites         du Fou-kien, Yenping et Foochow (la résidence de Ningpo, achetée en         juillet-août 1701, est contestée, jugement favorable en septembre 1702,         AHSI 30 (1961), 321). On pourrait aussi prolonger les traits de Kiangchow         à Sian et de Chinkiang à Hwaian.        LÉGENDE        Les ronds désignent les résidences jésuites: résidence habitée en 1701, rond         noir; résidence non occupée, rond blanc sans point central; résidence de la         mission française.                 Les sigles sont les mêmes que ceux de la carte précédente (1644), sauf         qu'un triangle blanc désigne ici les Missions Etrangères de Paris, qui n'avaient         pas de résidence en Chine sous les Ming. — Nous groupons ensemble, par         province et par sigle, les résidences non-occupées en 1701.                 La Congrégation de la Propagande ne possède alors aucune résidence, celle        de Siaoshan du Shaohing au Chekiang n'ayant été achetée que le 9 nov. 1702;         mais il y avait plusieurs missionnaires de différents ordres et congrégations        envoyés par la Propagande.                 Le tableau ci-après, basé sur JS 134, et sur nos propres recherches (publiées        dans l'AHSI depuis 1953), demeure incomplet : € multa sunt templa et sacella         in pagis et oppidis, quae non recensui; imo et forte aliquae domus in urbibus         quas ignoro propter tantam locorum distantiam ». Le catalogue de 1703 multiplie        les « missio cum sede stabili », que nous traduisons par « résidence actuellement         inoccupée, ou maison sans prêtre à demeure » (R'). Nous avons préféré        nous en tenir à l'année 1701, car le nombre et la situation des résidences        (R) va grandement évoluer au cours des années suivantes avec l'afflux méthodique         des jésuites français (1701 sq), tout occupés à l'achat de nouvelles maisons         pour leur mission, et l'arrivée des franciscains de la Propagande (1705).         L'expulsion des missionnaires non munis du p'iao va contribuer à modifier        encore la situation, à partir de 1708. La liste de 1701 donne les noms de la résidence         et des missionnaires qui l'occupent. Il n'en est pas de même du catalogue          de 1703.                   R = Résidence SJ (sauf si marqué R OP; R MEP; R OFM; R OESA).          R' = Résidence inoccupée.                   Les noms des villes autres que les fou sont en italiques et les capitales        de province en majuscules. La carte de Chine de la Grande Encyclopédie,         t. V, p. 2770 Larousse, 1973, donne aussi en pinyin les noms des villes.        NOTA TRANSCRIÇÃO        "geo1$ = Provincia ou região"        "geo2$ = fou (perfeitura ou cidade de 1ª ordem) ou tcheou independente"        "geo3$ = tcheou-hien ou burgo"          Em cada entrada o formato é                    "geoN$Nome geográfico/Tipo (província, fou, tcheou-hien)/id=deh-r1701-nome"          Exº            "geo1$Chekiang#Zhejiang/província/deh-r1701-chekiang"           "geo2$Hangchou#Hangzhou/capital provincial/deh-r1701-hangzhou"           "geo3$Fuyang/tchou-hien/deh-r1701-fuyang"          Nos locais onde há presença de missionários:             "atr$residencia-missao/Jesuíta/16110000 (onde aparece R)"           "atr$residencia-missao/Dominicanos%OP/16560000" (quando passa a residência de outra ordem                                                   ver abreviaturas na legenda do mapa, exº p.354 em Kinhua)           "atr$activa/sim/16110000"         (onde só aparece uma data)            """
 
       geodesc$deh-chre-1701/0/0/1701
 
          geo1$Chekiang%CHEKIANG (actuel ZHEJIANG)#Zhejiang， @wikidata: Q16967/província/deh-r1701-chekiang
```

### Comparing `timelink-1.1.8/tests/timelink-home/projects/tutorial/notebooks/0-tutorial.ipynb` & `timelink-1.1.9/tests/timelink-home/projects/tutorial/notebooks/0-tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/timelink-home/projects/tutorial/notebooks/1-receipts.ipynb` & `timelink-1.1.9/tests/timelink-home/projects/tutorial/notebooks/1-receipts.ipynb`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/timelink-home/projects/tutorial/notebooks/README.md` & `timelink-1.1.9/tests/timelink-home/projects/tutorial/notebooks/README.md`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/timelink-home/projects/tutorial/notebooks/requirements.txt` & `timelink-1.1.9/tests/timelink-home/projects/tutorial/notebooks/requirements.txt`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/xml_data/b1685.cli` & `timelink-1.1.9/tests/xml_data/b1685.cli`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/xml_data/b1685.xml` & `timelink-1.1.9/tests/xml_data/b1685.xml`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/xml_data/dehergne-a.xml` & `timelink-1.1.9/tests/xml_data/dehergne-a.xml`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/xml_data/dehergne-locations-1644.xml` & `timelink-1.1.9/tests/xml_data/dehergne-locations-1644.xml`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/xml_data/dev1692.cli` & `timelink-1.1.9/tests/xml_data/dev1692.cli`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/xml_data/dev1692.xml` & `timelink-1.1.9/tests/xml_data/dev1692.xml`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/xml_data/mhk_identification_toliveira.xml` & `timelink-1.1.9/tests/xml_data/mhk_identification_toliveira.xml`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/xml_data/test-atr-date.xml` & `timelink-1.1.9/tests/xml_data/test-atr-date.xml`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/tests/xml_data/test-auc-alunos-264605-A-140337-140771.xml` & `timelink-1.1.9/tests/xml_data/test-auc-alunos-264605-A-140337-140771.xml`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/__init__.py` & `timelink-1.1.9/timelink/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,10 +14,10 @@
 from .api import models  # noqa: F401
 from .api import views  # noqa: F401
 from .api import schemas  # noqa: F401
 
 
 __author__ = """Joaquim Ramos de Carvalho"""
 __email__ = 'joaquim@uc.pt'
-__version__ = '1.1.8'
+__version__ = '1.1.9'
 
 version = __version__
```

### Comparing `timelink-1.1.8/timelink/api/crud.py` & `timelink-1.1.9/timelink/api/crud.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/api/database.py` & `timelink-1.1.9/timelink/api/database.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/api/models/__init__.py` & `timelink-1.1.9/timelink/api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/api/models/act.py` & `timelink-1.1.9/timelink/api/models/act.py`

 * *Files 17% similar despite different names*

```diff
@@ -62,20 +62,27 @@
             f'local="{kleio_escape(self.loc)}", '
             f'ref="{kleio_escape(self.ref)}", '
             f'obs="{quote_long_text(self.obs)}"'
             f")"
         )
 
     def __str__(self):
-        return self.to_kleio()
+        return self.to_kleio(show_contained=False)
 
-    def to_kleio(self, width=80) -> str:
+    def to_kleio(self, ident="", ident_inc="  ", show_contained=True, width=80) -> str:
         r = (
             f"{self.groupname}${self.id}"
             f"/{self.the_date}"
             f"/type={kleio_escape(self.the_type)}"
             f"/ref={quote_long_text(self.ref)}"
             f"/loc={quote_long_text(self.loc)}"
         )
         if self.obs is not None and len(self.obs.strip()) > 0:
             r = f"{r}/obs={quote_long_text(self.obs.strip(),width=width)}"
-        return r
+        kleio = super().to_kleio(
+            self_string=r,
+            ident=ident,
+            ident_inc=ident_inc,
+            show_contained=show_contained,
+            width=width,
+        )
+        return kleio
```

### Comparing `timelink-1.1.8/timelink/api/models/attribute.py` & `timelink-1.1.9/timelink/mhk/models/attribute.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # pylint: disable=import-error
 
 from sqlalchemy import Column, String, ForeignKey, Index
 from sqlalchemy.orm import relationship
-from .entity import Entity
+
 from timelink.kleio.utilities import quote_long_text
+from timelink.mhk.models.entity import Entity
 
 
 class Attribute(Entity):
+    __table_args__ = {"extend_existing": True}
     __tablename__ = "attributes"
 
-    id = Column(String, ForeignKey("entities.id", ondelete="CASCADE"), primary_key=True)
+    id = Column(String, ForeignKey("entities.id"), primary_key=True)
     entity = Column(String, ForeignKey("entities.id"), index=True)
     the_type = Column(String, index=True)
     the_value = Column(String, index=True)
     the_date = Column(String, index=True)
     obs = Column(String)
     the_entity = relationship(
         "Entity",
@@ -37,16 +39,15 @@
             f'the_value="{self.the_value}", '
             f'the_date="{self.the_date}"", '
             f"obs={self.obs}"
             f")"
         )
 
     def __str__(self):
-        r = f"{self.groupname}${quote_long_text(self.the_type)}"
-        r += f"/{quote_long_text(self.the_value)}/"
+        r = f"{self.groupname}${quote_long_text(self.the_type)}/{quote_long_text(self.the_value)}/"
         r += f"{self.the_date}"
         if self.obs is not None and len(self.obs.strip()) > 0:
             r = f"{r}/obs={quote_long_text(self.obs)}"
         return r
 
 
 Entity.attributes = relationship(
```

### Comparing `timelink-1.1.8/timelink/api/models/base.py` & `timelink-1.1.9/timelink/api/models/base.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/api/models/base_class.py` & `timelink-1.1.9/timelink/api/models/base_class.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/api/models/base_mappings.py` & `timelink-1.1.9/timelink/api/models/base_mappings.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/api/models/entity.py` & `timelink-1.1.9/timelink/api/models/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -224,17 +224,22 @@
             f"indexed={self.indexed},"
             f")"
         )
 
     def __str__(self):
         return f"{self.groupname}${kleio_escape(self.id)}/type={kleio_escape(self.pom_class)}"
 
-    def to_kleio(self, ident="", ident_inc="  ", **kwargs):
-        s = f"{ident}{str(self)}"
+    def to_kleio(self, self_string=None, show_contained=True, ident="", ident_inc="  ", **kwargs):
+        if self_string is None:
+            s = f"{ident}{str(self)}"
+        else:
+            s = f"{ident}{self_string}"
+
         contained_entities: List[Entity] = self.contains
         # sort by the_order
-        contained_entities.sort(key=lambda x: x.the_order)
-        for inner in contained_entities:
-            innerk = inner.to_kleio(ident=ident + ident_inc, ident_inc=ident_inc, **kwargs)
-            if innerk != "":
-                s = f"{s}\n{innerk}"
+        if show_contained and contained_entities is not None:
+            contained_entities.sort(key=lambda x: x.the_order)
+            for inner in contained_entities:
+                innerk = inner.to_kleio(ident=ident + ident_inc, ident_inc=ident_inc, **kwargs)
+                if innerk != "":
+                    s = f"{s}\n{innerk}"
         return s
```

### Comparing `timelink-1.1.8/timelink/api/models/object.py` & `timelink-1.1.9/timelink/api/models/object.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,18 +26,19 @@
             f'name="{self.name}", '
             f'the_type="{self.the_type}", '
             f"obs={self.obs}"
             f")"
         )
 
     def __str__(self):
-        self.to_kleio()
+        self.to_kleio(show_contained=False)
 
-    def to_kleio(self, width=80) -> str:
+    def to_kleio(self, ident="", ident_inc="  ", width=80) -> str:
         if self.name is None:
             name = ""
         else:
             name = self.name + "/"
         r = f"{self.groupname}${name}{quote_long_text(self.the_type, width=width)}/id={self.id}"
         if self.obs is not None and len(self.obs.strip()) > 0:
             r = f"{r}  /obs={quote_long_text(self.obs.strip(), width=width)}"
+        r = super().to_kleio(self_string=r, ident=ident, ident_inc=ident_inc, width=width)
         return r
```

### Comparing `timelink-1.1.8/timelink/api/models/person.py` & `timelink-1.1.9/timelink/api/models/person.py`

 * *Files 11% similar despite different names*

```diff
@@ -31,22 +31,29 @@
             f"obs={self.obs}"
             f")"
         )
 
     def __str__(self):
         return self.to_kleio()
 
-    def to_kleio(self, width=80) -> str:
+    def to_kleio(self, ident="", ident_inc="  ", show_contained=True, width=80) -> str:
         r = (
             f"{self.groupname}${quote_long_text(self.name)}/"
             f"{quote_long_text(self.sex)}/id={quote_long_text(self.id)}"
         )
         if self.obs is not None and len(self.obs.strip()) > 0:
             r = f"{r}/obs={quote_long_text(self.obs,width=width)}"
-        return r
+        kleio = super().to_kleio(
+            self_string=r,
+            show_contained=show_contained,
+            ident=ident,
+            ident_inc=ident_inc,
+            width=width,
+        )
+        return kleio
 
 
 def get_person(id: str = None, db=None, sql_echo: bool = False) -> Person:
     """
     Fetch a person from the database
     """
     if id is None:
```

### Comparing `timelink-1.1.8/timelink/api/models/pom_som_mapper.py` & `timelink-1.1.9/timelink/api/models/pom_som_mapper.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/api/models/relation.py` & `timelink-1.1.9/timelink/api/models/relation.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,20 +75,20 @@
                 f"rel${self.the_type}/{quote_long_text(self.the_value)}/"
                 f"{self.destination}/{self.the_date}"
             )
         if self.obs is not None and len(self.obs.strip()) > 0:
             r = f"{r}/obs={quote_long_text(self.obs)}"
         return r
 
-    def to_kleio(self, ident="", ident_inc="  ", **kwargs):
+    def to_kleio(self, **kwargs):
         if self.the_type == "function-in-act":
             return ""
         else:
             # call to_kleio from the parent class
-            return super().to_kleio(ident, ident_inc, **kwargs)
+            return super().to_kleio(**kwargs)
 
 
 Entity.rels_out = relationship(
     "Relation", foreign_keys=[Relation.origin], back_populates="dest"
 )
 
 Entity.rels_in = relationship(
```

### Comparing `timelink-1.1.8/timelink/api/models/source.py` & `timelink-1.1.9/timelink/api/models/source.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,19 +58,26 @@
             f'obs="{self.obs}"'
             f")"
         )
 
     def __str__(self):
         return self.to_kleio()
 
-    def to_kleio(self, width=80) -> str:
+    def to_kleio(self, ident="", ident_inc="  ", show_contained=True, width=80) -> str:
         r = (
             f"{self.groupname}${self.id}/{self.the_date}"
             f"/type={kleio_escape(self.the_type)}"
             f"/ref={kleio_escape(self.ref)}"
             f"/loc={kleio_escape(self.loc)}"
             f'/kleiofile={kleio_escape(self.kleiofile)}"'
             f"/replaces={self.replaces}"
         )
         if self.obs is not None and len(self.obs.strip()) > 0:
             r = f"{r}/obs={quote_long_text(self.obs.strip(), width=width)}"
+        r = super().to_kleio(
+            self_string=r,
+            ident=ident,
+            ident_inc=ident_inc,
+            show_contained=show_contained,
+            width=width,
+        )
         return r
```

### Comparing `timelink-1.1.8/timelink/api/models/system.py` & `timelink-1.1.9/timelink/api/models/system.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/api/schemas.py` & `timelink-1.1.9/timelink/api/schemas.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/api/views.py` & `timelink-1.1.9/timelink/api/views.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/app/__init__.py` & `timelink-1.1.9/timelink/app/__init__.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/app/backend/timelink_webapp.py` & `timelink-1.1.9/timelink/app/backend/timelink_webapp.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/app/dependencies.py` & `timelink-1.1.9/timelink/app/dependencies.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/app/main.py` & `timelink-1.1.9/timelink/app/main.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/app/models/project.py` & `timelink-1.1.9/timelink/app/models/project.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/app/models/user.py` & `timelink-1.1.9/timelink/app/models/user.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/app/models/user_database.py` & `timelink-1.1.9/timelink/app/models/user_database.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/app/schemas/project.py` & `timelink-1.1.9/timelink/app/schemas/project.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/app/schemas/user.py` & `timelink-1.1.9/timelink/app/schemas/user.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/app/services/auth.py` & `timelink-1.1.9/timelink/app/services/auth.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/app/web/__init__.py` & `timelink-1.1.9/timelink/app/web/__init__.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/app/web/home_page.py` & `timelink-1.1.9/timelink/app/web/home_page.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/app/web/login_page.py` & `timelink-1.1.9/timelink/app/web/login_page.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/app/web/projects_page.py` & `timelink-1.1.9/timelink/app/web/projects_page.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/app/web/webapp_info.py` & `timelink-1.1.9/timelink/app/web/webapp_info.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/cli.py` & `timelink-1.1.9/timelink/cli.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/kleio/__init__.py` & `timelink-1.1.9/timelink/kleio/__init__.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/kleio/groups/__init__.py` & `timelink-1.1.9/timelink/kleio/groups/__init__.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/kleio/groups/kact.py` & `timelink-1.1.9/timelink/kleio/groups/kact.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/kleio/groups/kattribute.py` & `timelink-1.1.9/timelink/kleio/groups/kattribute.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/kleio/groups/kelement.py` & `timelink-1.1.9/timelink/kleio/groups/kelement.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/kleio/groups/kgroup.py` & `timelink-1.1.9/timelink/kleio/groups/kgroup.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/kleio/groups/kkleio.py` & `timelink-1.1.9/timelink/kleio/groups/kkleio.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/kleio/groups/kobject.py` & `timelink-1.1.9/timelink/kleio/groups/kobject.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/kleio/groups/kperson.py` & `timelink-1.1.9/timelink/kleio/groups/kperson.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/kleio/groups/krelation.py` & `timelink-1.1.9/timelink/kleio/groups/krelation.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/kleio/groups/ksource.py` & `timelink-1.1.9/timelink/kleio/groups/ksource.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/kleio/importer.py` & `timelink-1.1.9/timelink/kleio/importer.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/kleio/kleio_server.py` & `timelink-1.1.9/timelink/kleio/kleio_server.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/kleio/schemas.py` & `timelink-1.1.9/timelink/kleio/schemas.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/kleio/utilities.py` & `timelink-1.1.9/timelink/kleio/utilities.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/mhk/models/__init__.py` & `timelink-1.1.9/timelink/mhk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/mhk/models/act.py` & `timelink-1.1.9/timelink/mhk/models/act.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/mhk/models/attribute.py` & `timelink-1.1.9/timelink/api/models/attribute.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 # pylint: disable=import-error
 
 from sqlalchemy import Column, String, ForeignKey, Index
 from sqlalchemy.orm import relationship
-
+from .entity import Entity
 from timelink.kleio.utilities import quote_long_text
-from timelink.mhk.models.entity import Entity
 
 
 class Attribute(Entity):
-    __table_args__ = {"extend_existing": True}
     __tablename__ = "attributes"
 
-    id = Column(String, ForeignKey("entities.id"), primary_key=True)
+    id = Column(String, ForeignKey("entities.id", ondelete="CASCADE"), primary_key=True)
     entity = Column(String, ForeignKey("entities.id"), index=True)
     the_type = Column(String, index=True)
     the_value = Column(String, index=True)
     the_date = Column(String, index=True)
     obs = Column(String)
     the_entity = relationship(
         "Entity",
@@ -39,17 +37,24 @@
             f'the_value="{self.the_value}", '
             f'the_date="{self.the_date}"", '
             f"obs={self.obs}"
             f")"
         )
 
     def __str__(self):
-        r = f"{self.groupname}${quote_long_text(self.the_type)}/{quote_long_text(self.the_value)}/"
+        return self.to_kleio(show_contained=False)
+
+    def to_kleio(self, ident="", ident_inc="  ", width=80) -> str:
+        r = f"{self.groupname}${quote_long_text(self.the_type)}"
+        r += f"/{quote_long_text(self.the_value)}/"
         r += f"{self.the_date}"
         if self.obs is not None and len(self.obs.strip()) > 0:
             r = f"{r}/obs={quote_long_text(self.obs)}"
-        return r
+        kleio = super().to_kleio(
+            self_string=r, ident=ident, ident_inc=ident_inc, width=width
+        )
+        return kleio
 
 
 Entity.attributes = relationship(
     "Attribute", foreign_keys=[Attribute.entity], back_populates="the_entity"
 )
```

### Comparing `timelink-1.1.8/timelink/mhk/models/base.py` & `timelink-1.1.9/timelink/mhk/models/base.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/mhk/models/base_class.py` & `timelink-1.1.9/timelink/mhk/models/base_class.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/mhk/models/base_mappings.py` & `timelink-1.1.9/timelink/mhk/models/base_mappings.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/mhk/models/db.py` & `timelink-1.1.9/timelink/mhk/models/db.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/mhk/models/entity.py` & `timelink-1.1.9/timelink/mhk/models/entity.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/mhk/models/object.py` & `timelink-1.1.9/timelink/mhk/models/object.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/mhk/models/person.py` & `timelink-1.1.9/timelink/mhk/models/person.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/mhk/models/pom_som_mapper.py` & `timelink-1.1.9/timelink/mhk/models/pom_som_mapper.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/mhk/models/relation.py` & `timelink-1.1.9/timelink/mhk/models/relation.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/mhk/models/source.py` & `timelink-1.1.9/timelink/mhk/models/source.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/mhk/models/system.py` & `timelink-1.1.9/timelink/mhk/models/system.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/mhk/utilities.py` & `timelink-1.1.9/timelink/mhk/utilities.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/networks/network_draw.py` & `timelink-1.1.9/timelink/networks/network_draw.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/networks/network_generation.py` & `timelink-1.1.9/timelink/networks/network_generation.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/notebooks/__init__.py` & `timelink-1.1.9/timelink/notebooks/__init__.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/notebooks/timelink_notebook.py` & `timelink-1.1.9/timelink/notebooks/timelink_notebook.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/pandas/__init__.py` & `timelink-1.1.9/timelink/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/pandas/attribute_values.py` & `timelink-1.1.9/timelink/pandas/attribute_values.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/pandas/entities_with_attribute.py` & `timelink-1.1.9/timelink/pandas/entities_with_attribute.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/pandas/group_attributes.py` & `timelink-1.1.9/timelink/pandas/group_attributes.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/pandas/name_to_df.py` & `timelink-1.1.9/timelink/pandas/name_to_df.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink/pandas/styles.py` & `timelink-1.1.9/timelink/pandas/styles.py`

 * *Files identical despite different names*

### Comparing `timelink-1.1.8/timelink.egg-info/PKG-INFO` & `timelink-1.1.9/timelink.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timelink
-Version: 1.1.8
+Version: 1.1.9
 Summary: Timelink is an information system for person related information collected from historical sources. 
 Home-page: https://github.com/time-link/timelink-py
 Author: Joaquim Ramos de Carvalho
 Author-email: joaquimcarvalho@ipm.edu.mo
 License: MIT license
 Project-URL: Documentation, https://timelink-py.readthedocs.io/
 Keywords: timelink
@@ -41,14 +41,21 @@
 Requires-Dist: uvicorn
 
 Timelink is an information system for person related information collected from historical sources. 
 
 =======
 History
 =======
+
+1.1.9 (2024-05-03)
+------------------
+
+* fix bug with to_kleio() in models (bad identation)
+
+
 1.1.8 (2024-05-02)
 ------------------
 
 * Fix bug with export_to_kleio()
 * Several minor bug fixes
 
 1.1.7 (2024-04-28)
```

### Comparing `timelink-1.1.8/timelink.egg-info/SOURCES.txt` & `timelink-1.1.9/timelink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

