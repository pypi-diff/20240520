# Comparing `tmp/drapi_lemur-1.0.40.tar.gz` & `tmp/drapi-lemur-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drapi_lemur-1.0.40.tar", last modified: Mon May 20 21:20:37 2024, max compression
+gzip compressed data, was "drapi-lemur-1.0.5.tar", last modified: Mon Feb 12 02:49:40 2024, max compression
```

## Comparing `drapi_lemur-1.0.40.tar` & `drapi-lemur-1.0.5.tar`

### file list

```diff
@@ -1,229 +1,205 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:37.963600 drapi_lemur-1.0.40/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-20 21:20:37.963600 drapi_lemur-1.0.40/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-20 21:20:37.967600 drapi_lemur-1.0.40/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:37.943601 drapi_lemur-1.0.40/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:37.943601 drapi_lemur-1.0.40/src/drapi/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:37.943601 drapi_lemur-1.0.40/src/drapi/code/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/code/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:37.947600 drapi_lemur-1.0.40/src/drapi/code/drapi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/code/drapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:37.947600 drapi_lemur-1.0.40/src/drapi/code/drapi/c2s/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/code/drapi/c2s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/code/drapi/c2s/c2s.py
--rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/code/drapi/compareGroups.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:37.947600 drapi_lemur-1.0.40/src/drapi/code/drapi/constants/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/code/drapi/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6424 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/code/drapi/constants/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     9415 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/code/drapi/constants/phiValues.py
--rw-r--r--   0 runner    (1001) docker     (127)    19474 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/code/drapi/constants/phiVariables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/code/drapi/constants/variableAliases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:37.947600 drapi_lemur-1.0.40/src/drapi/code/drapi/convertColumns/
--rw-r--r--   0 runner    (1001) docker     (127)    18142 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/code/drapi/convertColumns/hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/code/drapi/deIdentificationFunctions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:37.947600 drapi_lemur-1.0.40/src/drapi/code/drapi/deIdentificationSuiteFuncs0/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/code/drapi/deIdentificationSuiteFuncs0/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4520 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/code/drapi/deIdentificationSuiteFuncs0/common.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4075 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/code/drapi/deIdentificationSuiteFuncs0/concatenateMaps.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3955 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/code/drapi/deIdentificationSuiteFuncs0/convertColumns.py
--rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/code/drapi/deIdentificationSuiteFuncs0/dataQualityTest.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6385 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/code/drapi/deIdentificationSuiteFuncs0/deIdentify.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4373 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/code/drapi/deIdentificationSuiteFuncs0/deleteColumns.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1376 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/code/drapi/deIdentificationSuiteFuncs0/gatherFiles.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4594 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/code/drapi/deIdentificationSuiteFuncs0/getIDValues.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2279 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/code/drapi/deIdentificationSuiteFuncs0/getProjectColumns.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8834 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/code/drapi/deIdentificationSuiteFuncs0/makeMapsFromOthers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2996 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/code/drapi/deIdentificationSuiteFuncs0/makeMapsFromScratch.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5686 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/code/drapi/deIdentificationSuiteFuncs0/makePersonIDMap.py
--rw-r--r--   0 runner    (1001) docker     (127)    27459 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/code/drapi/drapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/code/drapi/expandColumn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:37.951600 drapi_lemur-1.0.40/src/drapi/code/drapi/getData/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4000 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/code/drapi/getData/getData.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3711 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/code/drapi/getData/getData_inner.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8184 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/code/drapi/getData/getData_outer.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/code/drapi/getPersonIDs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:37.951600 drapi_lemur-1.0.40/src/drapi/code/drapi/idealist/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/code/drapi/idealist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/code/drapi/idealist/getEncountersMap.py
--rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/code/drapi/idealist/getPatientsMap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/code/drapi/idealist/idealist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:37.951600 drapi_lemur-1.0.40/src/drapi/code/drapi/images/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/code/drapi/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/code/drapi/images/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/code/drapi/makeListOfDates.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/code/drapi/makeSymLinks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/code/drapi/modifyTSV.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:37.951600 drapi_lemur-1.0.40/src/drapi/code/drapi/notes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/code/drapi/notes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29050 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/code/drapi/notes/freeText.py
--rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/code/drapi/notes/pullNotes.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/code/drapi/notes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:37.951600 drapi_lemur-1.0.40/src/drapi/code/drapi/omop/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/code/drapi/omop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/code/drapi/omop/configProcessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5545 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/code/drapi/omop/deidentify.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:37.951600 drapi_lemur-1.0.40/src/drapi/code/drapi/oneFlorida/
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/code/drapi/oneFlorida/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/code/drapi/oneFlorida/oneFlorida.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/code/drapi/parseAliasArguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     5590 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/code/drapi/prepTSVforSDOH.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:37.951600 drapi_lemur-1.0.40/src/drapi/code/drapi/qa/
--rw-r--r--   0 runner    (1001) docker     (127)     8413 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/code/drapi/qa/columnConversion.py
--rw-r--r--   0 runner    (1001) docker     (127)    13481 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/code/drapi/qa/deidentification.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/code/drapi/searchFolders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/code/drapi/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/code/drapi/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:37.951600 drapi_lemur-1.0.40/src/drapi/code/makeDirTemplate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/code/makeDirTemplate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:37.951600 drapi_lemur-1.0.40/src/drapi/sql/
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/sql/9-Digit Zip Code.SQL
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/sql/Consent2Share.sql
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/sql/ConvertBetweenMrnAndOneFloridaPatID.SQL
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/sql/LADMF.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/sql/MRNfromPatientKey.sql
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/sql/OneFlorida to UF Health Patient ID Map.SQL
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/sql/encounterNumber2patientKey.SQL
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:37.951600 drapi_lemur-1.0.40/src/drapi/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:37.943601 drapi_lemur-1.0.40/src/drapi/templates/Anaconda Environment Variables/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:37.951600 drapi_lemur-1.0.40/src/drapi/templates/Anaconda Environment Variables/RenameMe environment-name/
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Anaconda Environment Variables/RenameMe environment-name/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:37.951600 drapi_lemur-1.0.40/src/drapi/templates/Data Disclosure README/
--rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Data Disclosure README/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:37.951600 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:37.951600 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/
--rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:37.955601 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/
--rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (127)     4059 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:37.955601 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/
--rw-r--r--   0 runner    (1001) docker     (127)     8389 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/aliasVariables.py
--rw-r--r--   0 runner    (1001) docker     (127)     7506 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/common.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8540 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/concatenateMaps.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5445 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/concatenateTables.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7518 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/convertColumns.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18101 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/convertColumnsGeneral.py
--rw-r--r--   0 runner    (1001) docker     (127)     6695 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/dataQualityTest.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13989 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/deIdentify.py
--rw-r--r--   0 runner    (1001) docker     (127)    10807 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/deIdentifyByAge.py
--rw-r--r--   0 runner    (1001) docker     (127)    14614 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/deIdentifyDates.py
--rw-r--r--   0 runner    (1001) docker     (127)     7951 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/deleteByColumnValues.py
--rw-r--r--   0 runner    (1001) docker     (127)    14613 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/deleteColumns.py
--rw-r--r--   0 runner    (1001) docker     (127)    10657 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/gatherFiles.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13908 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/getIDValues.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9782 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/getProjectColumns.py
--rw-r--r--   0 runner    (1001) docker     (127)     8117 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/i2b2ConvertIDs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7133 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/i2b2GetIDs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/i2b2MakeMap.py
--rw-r--r--   0 runner    (1001) docker     (127)     8696 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/makeAgeMap.py
--rw-r--r--   0 runner    (1001) docker     (127)     4762 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/makeDateShiftMap.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16369 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/makeMapsFromOthers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6943 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/makeMapsFromScratch.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8852 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/makePersonIDMap.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11138 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/mapToSqlite.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      651 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/launchIPython.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:37.943601 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:37.955601 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/BO Portion Template/
--rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/BO Portion Template/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (127)      433 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/BO Portion Template/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:37.955601 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/BO Portion Template/code/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/BO Portion Template/code/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:37.943601 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/BO Portion Template/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:37.955601 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/BO Portion Template/data/input/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/BO Portion Template/data/input/.deleteme
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:37.955601 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/BO Portion Template/data/output/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/BO Portion Template/data/output/.deleteme
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/BO Portion Template/launchIPython.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:37.959601 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/Clinical Text Portion Template/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3122 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/Clinical Text Portion Template/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (127)      714 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/Clinical Text Portion Template/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:37.959601 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/Clinical Text Portion Template/code/
--rw-r--r--   0 runner    (1001) docker     (127)    12742 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/Clinical Text Portion Template/code/filterNotes.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    45323 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/Clinical Text Portion Template/code/freeText.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/Clinical Text Portion Template/code/script.bash
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:37.943601 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/Clinical Text Portion Template/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:37.959601 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/Clinical Text Portion Template/data/input/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/Clinical Text Portion Template/data/input/.deleteme
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:37.959601 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/Clinical Text Portion Template/data/output/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/Clinical Text Portion Template/data/output/.deleteme
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/Clinical Text Portion Template/launchIPython.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:37.959601 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/Clinical Text Portion Template/sql/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3248 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/Clinical Text Portion Template/sql/note_metadata.sql
--rwxr-xr-x   0 runner    (1001) docker     (127)      408 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/Clinical Text Portion Template/sql/note_text.sql
--rwxr-xr-x   0 runner    (1001) docker     (127)     2604 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/Clinical Text Portion Template/sql/order_impression_metadata.sql
--rwxr-xr-x   0 runner    (1001) docker     (127)      179 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/Clinical Text Portion Template/sql/order_impression_text.sql
--rwxr-xr-x   0 runner    (1001) docker     (127)     2603 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/Clinical Text Portion Template/sql/order_narrative_metadata.sql
--rwxr-xr-x   0 runner    (1001) docker     (127)      177 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/Clinical Text Portion Template/sql/order_narrative_text.sql
--rwxr-xr-x   0 runner    (1001) docker     (127)     2638 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/Clinical Text Portion Template/sql/order_result_comment_metadata.sql
--rwxr-xr-x   0 runner    (1001) docker     (127)      202 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/Clinical Text Portion Template/sql/order_result_comment_text.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:37.959601 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/General Script Template/
--rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/General Script Template/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (127)      185 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/General Script Template/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:37.959601 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/General Script Template/code/
--rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/General Script Template/code/RenameMe.py
--rw-r--r--   0 runner    (1001) docker     (127)     6800 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/General Script Template/code/compareGroupsTemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/General Script Template/code/loopTemplate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:37.943601 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/General Script Template/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:37.959601 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/General Script Template/data/input/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/General Script Template/data/input/.deleteme
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:37.959601 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/General Script Template/data/output/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/General Script Template/data/output/.deleteme
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/General Script Template/launchIPython.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:37.959601 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/OMOP Portion Template/
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/OMOP Portion Template/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/OMOP Portion Template/Config1.YAML
--rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/OMOP Portion Template/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:37.959601 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/OMOP Portion Template/code/
--rw-r--r--   0 runner    (1001) docker     (127)    15495 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/OMOP Portion Template/code/Project1.py
--rw-r--r--   0 runner    (1001) docker     (127)     5545 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/OMOP Portion Template/code/deidentify.py
--rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/OMOP Portion Template/code/getPersonIDs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:37.943601 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/OMOP Portion Template/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:37.959601 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/OMOP Portion Template/data/input/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/OMOP Portion Template/data/input/.deleteme
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:37.959601 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/OMOP Portion Template/data/output/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/OMOP Portion Template/data/output/.deleteme
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/OMOP Portion Template/launchIPython.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:37.963600 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/OMOP Portion Template/sql/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/OMOP Portion Template/sql/grabPersonIDs.SQL
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:37.963600 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/i2b2 Portion Template/
--rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/i2b2 Portion Template/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/i2b2 Portion Template/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:37.963600 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/i2b2 Portion Template/code/
--rw-r--r--   0 runner    (1001) docker     (127)    23578 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/i2b2 Portion Template/code/i2b2_dump.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:37.943601 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/i2b2 Portion Template/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:37.963600 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/i2b2 Portion Template/data/input/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/i2b2 Portion Template/data/input/.deleteme
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:37.963600 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/i2b2 Portion Template/data/output/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/i2b2 Portion Template/data/output/.deleteme
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/i2b2 Portion Template/launchIPython.bat
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:37.963600 drapi_lemur-1.0.40/src/drapi/templates/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     6323 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/scripts/Argparse Template - with SQL.py
--rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/scripts/hippaDisclosure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/drapi/templates/scripts/sqlQuery.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:37.963600 drapi_lemur-1.0.40/src/drapi_lemur.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-20 21:20:37.000000 drapi_lemur-1.0.40/src/drapi_lemur.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12823 2024-05-20 21:20:37.000000 drapi_lemur-1.0.40/src/drapi_lemur.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 21:20:37.000000 drapi_lemur-1.0.40/src/drapi_lemur.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-20 21:20:37.000000 drapi_lemur-1.0.40/src/drapi_lemur.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:20:37.963600 drapi_lemur-1.0.40/src/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/scripts/checkC2S.py
--rw-r--r--   0 runner    (1001) docker     (127)    18667 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/scripts/convertColumnsHash.py
--rw-r--r--   0 runner    (1001) docker     (127)     5306 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/scripts/expandColumns.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14578 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/scripts/getData.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8633 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/scripts/getIDSets.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4353 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/scripts/makeDirTemplate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3172 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/scripts/makeSymlink
--rwxr-xr-x   0 runner    (1001) docker     (127)    17391 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/scripts/mapOF2IDR_deid2deid.py
--rw-r--r--   0 runner    (1001) docker     (127)    13183 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/scripts/mapOF2IDR_id2id.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14458 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/scripts/map_deid2deid.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7571 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/scripts/prepTSVforSDOH.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6135 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/scripts/prepTSVforSDOH2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12142 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/scripts/qaColumnConversion.py
--rw-r--r--   0 runner    (1001) docker     (127)    11685 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/scripts/qaDeidentification.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4369 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/scripts/replaceText.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-20 21:20:32.000000 drapi_lemur-1.0.40/src/scripts/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.040113 drapi-lemur-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-02-12 02:49:40.040113 drapi-lemur-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-12 02:49:40.040113 drapi-lemur-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.020113 drapi-lemur-1.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.020113 drapi-lemur-1.0.5/src/drapi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.020113 drapi-lemur-1.0.5/src/drapi/code/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.024113 drapi-lemur-1.0.5/src/drapi/code/drapi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.024113 drapi-lemur-1.0.5/src/drapi/code/drapi/c2s/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/c2s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/c2s/c2s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/c2s/checkC2S.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/compareGroups.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.024113 drapi-lemur-1.0.5/src/drapi/code/drapi/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6248 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/constants/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9415 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/constants/phiValues.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18623 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/constants/phiVariables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.024113 drapi-lemur-1.0.5/src/drapi/code/drapi/deIdentificationSuiteFuncs0/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/deIdentificationSuiteFuncs0/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4520 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/deIdentificationSuiteFuncs0/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4075 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/deIdentificationSuiteFuncs0/concatenateMaps.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3955 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/deIdentificationSuiteFuncs0/convertColumns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/deIdentificationSuiteFuncs0/dataQualityTest.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6385 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/deIdentificationSuiteFuncs0/deIdentify.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4373 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/deIdentificationSuiteFuncs0/deleteColumns.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1376 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/deIdentificationSuiteFuncs0/gatherFiles.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4594 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/deIdentificationSuiteFuncs0/getIDValues.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2279 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/deIdentificationSuiteFuncs0/getProjectColumns.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8834 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/deIdentificationSuiteFuncs0/makeMapsFromOthers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2996 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/deIdentificationSuiteFuncs0/makeMapsFromScratch.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5686 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/deIdentificationSuiteFuncs0/makePersonIDMap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25947 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/drapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/getPersonIDs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.024113 drapi-lemur-1.0.5/src/drapi/code/drapi/idealist/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/idealist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6466 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/idealist/getEncountersMap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/idealist/getPatientsMap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/idealist/idealist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.024113 drapi-lemur-1.0.5/src/drapi/code/drapi/images/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/images/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/makeSymLinks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.028113 drapi-lemur-1.0.5/src/drapi/code/drapi/notes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/notes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29050 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/notes/freeText.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/notes/pullNotes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/notes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.028113 drapi-lemur-1.0.5/src/drapi/code/drapi/omop/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/omop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/omop/configProcessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5545 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/omop/deidentify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/oneFlorida.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5590 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/prepTSVforSDOH.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/searchFolders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/drapi/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.028113 drapi-lemur-1.0.5/src/drapi/code/makeDirTemplate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/makeDirTemplate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/code/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.028113 drapi-lemur-1.0.5/src/drapi/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/sql/9-Digit Zip Code.SQL
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/sql/Consent2Share.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/sql/ConvertBetweenMrnAndOneFloridaPatID.SQL
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/sql/LADMF.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/sql/MRNfromPatientKey.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/sql/MapOneFloridaIDs.SQL
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/sql/encounterNumber2patientKey.SQL
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.020113 drapi-lemur-1.0.5/src/drapi/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.028113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.020113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/Anaconda Environment Variables/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.028113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/Anaconda Environment Variables/RenameMe environment-name/
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/Anaconda Environment Variables/RenameMe environment-name/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.028113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/
+-rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.028113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/.env
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3987 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.032113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/
+-rw-r--r--   0 runner    (1001) docker     (127)     8382 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/aliasVariables.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9361 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8610 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/concatenateMaps.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7588 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/convertColumns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6695 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/dataQualityTest.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14059 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/deIdentify.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10796 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/deIdentifyByAge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14603 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/deIdentifyDates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7940 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/deleteByColumnValues.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14419 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/deleteColumns.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8538 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/gatherFiles.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14496 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/getIDValues.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9747 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/getProjectColumns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8117 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/i2b2ConvertIDs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7133 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/i2b2GetIDs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/i2b2MakeMap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8696 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/makeAgeMap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4762 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/makeDateShiftMap.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16439 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/makeMapsFromOthers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7024 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/makeMapsFromScratch.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8933 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/makePersonIDMap.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      651 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/launchIPython.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.020113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.032113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/.env
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)      395 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.032113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/code/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8100 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/code/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5560 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/code/getData.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.020113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.032113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/data/input/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/data/input/.deleteme
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.032113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/data/output/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/data/output/.deleteme
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/launchIPython.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.032113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/.env
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)      395 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.032113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/code/
+-rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/code/RenameMe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6800 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/code/compareGroupsTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/code/loopTemplate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.020113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.032113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/data/input/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/data/input/.deleteme
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.032113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/data/output/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/data/output/.deleteme
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/launchIPython.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.032113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/.env
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3114 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.032113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/code/
+-rw-r--r--   0 runner    (1001) docker     (127)    12742 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/code/filterNotes.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    35999 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/code/freeText.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.020113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.036113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/data/input/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/data/input/.deleteme
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.036113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/data/output/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/data/output/.deleteme
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/launchIPython.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.036113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/sql/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3248 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/sql/note_metadata.sql
+-rwxr-xr-x   0 runner    (1001) docker     (127)      408 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/sql/note_text.sql
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2604 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/sql/order_impression_metadata.sql
+-rwxr-xr-x   0 runner    (1001) docker     (127)      179 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/sql/order_impression_text.sql
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2603 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/sql/order_narrative_metadata.sql
+-rwxr-xr-x   0 runner    (1001) docker     (127)      177 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/sql/order_narrative_text.sql
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2638 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/sql/order_result_comment_metadata.sql
+-rwxr-xr-x   0 runner    (1001) docker     (127)      202 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/sql/order_result_comment_text.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.036113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/.env
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     7852 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/Config1.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.036113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/README Images/
+-rw-r--r--   0 runner    (1001) docker     (127)     5279 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/README Images/glDownloadButton.png
+-rw-r--r--   0 runner    (1001) docker     (127)   275966 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/README Images/glDownloadDirectory.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/README-INSTALLATION.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.036113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/code/
+-rw-r--r--   0 runner    (1001) docker     (127)    15463 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/code/Project1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5545 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/code/deidentify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7603 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/code/getPersonIDs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.020113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.036113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/data/input/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/data/input/.deleteme
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.036113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/data/output/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/data/output/.deleteme
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/launchIPython.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.036113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/sql/grabPersonIDs.SQL
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.036113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Portion 1/
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Portion 1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.036113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Portion 2/
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Portion 2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.036113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/.env
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.040113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/code/
+-rw-r--r--   0 runner    (1001) docker     (127)    23578 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/code/i2b2_dump.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.020113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.040113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/data/input/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/data/input/.deleteme
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.040113 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/data/output/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/data/output/.deleteme
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/launchIPython.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.040113 drapi-lemur-1.0.5/src/drapi/templates/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/scripts/hippaDisclosure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/drapi/templates/scripts/sqlQuery.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 02:49:40.040113 drapi-lemur-1.0.5/src/drapi_lemur.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-02-12 02:49:39.000000 drapi-lemur-1.0.5/src/drapi_lemur.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12185 2024-02-12 02:49:40.000000 drapi-lemur-1.0.5/src/drapi_lemur.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-12 02:49:39.000000 drapi-lemur-1.0.5/src/drapi_lemur.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-12 02:49:39.000000 drapi-lemur-1.0.5/src/drapi_lemur.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-02-12 02:49:29.000000 drapi-lemur-1.0.5/src/makeDirTemplate.py
```

### Comparing `drapi_lemur-1.0.40/PKG-INFO` & `drapi-lemur-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drapi-lemur
-Version: 1.0.40
+Version: 1.0.5
 Summary: Data Request API for the Integrated Data Repository Research Services of University of Florida.
 Home-page: https://github.com/ChemGuy88/hermanCode/archive/refs/tags/v1.0.0.tar.gz
 Author: Herman Autore
 Author-email: hf.autore+drapi@gmail.com
 Keywords: CTSI,Clinical and Translational Science Institute,IDR,Integrated Data Repository,Integrated Data Repository Research Services,ODSRI,Office of Data Science and Research Implementation,Shands,Sloth 🦥,UF,UF Health,UFHealth,University of Florida
 
 Data Request API for the Integrated Data Repository Research Services of University of Florida.
```

### Comparing `drapi_lemur-1.0.40/src/drapi/code/drapi/c2s/c2s.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/c2s/c2s.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 import os
 from pathlib import Path
 from typing import List
 from typing_extensions import Literal
 # Third-party libraries
 import pandas as pd
 # Local libraries
-from drapi.code.drapi.drapi import (replace_sql_query,
-                                    successiveParents)
+from drapi.drapi import replace_sql_query
+from drapi.drapi import successiveParents
 
 # Arguments
-MODULE_ROOT_DIRECTORY_PATH, _ = successiveParents(Path(__file__), 4)
+MODULE_ROOT_DIRECTORY_PATH = successiveParents(Path(__file__), 4)
 
 # Arguments: SQL connection settings
 SERVER = "EDW.shands.ufl.edu"
 DATABASE = "DWS_PROD"
 USERDOMAIN = "UFAD"
 USERNAME = os.environ["USER"]
 UID = None
```

### Comparing `drapi_lemur-1.0.40/src/drapi/code/drapi/compareGroups.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/compareGroups.py`

 * *Files identical despite different names*

### Comparing `drapi_lemur-1.0.40/src/drapi/code/drapi/constants/constants.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/constants/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Useful definitions used throughout IDR
 
-See the Clinical Text Portion for current IDR mapping standards: /Volumes/FILES/SHARE/DSS/IDR Data Requests/ACTIVE RDRs/Bian/IRB202202436/Intermediate Results/Clinical Text Portion/Data/Output/mapping
+See the Notes portion for current IDR mapping standards: /Volumes/FILES/SHARE/DSS/IDR Data Requests/ACTIVE RDRs/Bian/IRB202202436/Intermediate Results/Notes Portion/Data/Output/mapping
 See Noah's data request for my attempt at using these standards: /Volumes/FILES/SHARE/DSS/IDR Data Requests/ACTIVE RDRs/Bian/IRB202202436/Concatenated Results/Code/makeMap.py
 """
-from drapi.code.drapi.constants.phiVariables import LIST_OF_PHI_VARIABLES
+from drapi.constants.phiVariables import LIST_OF_PHI_VARIABLES
 
 __all__ = ["DeIdIDName2DeIdIDSuffix",
            "IDName2DeIdIDName",
            "mapDtypes",
            "DATA_TYPES_DICT"]
 
 IDName2DeIdIDNameRoot = {"ENCNTR_CSN_ID": "enc",
@@ -22,18 +22,14 @@
                            "link_note": "LINK_NOTE",
                            "order": "ORDER",
                            "provider": "PROV"}
 mapDtypes = {0: int,
              1: int,
              2: str}
 
-# De-identification prefixes
-DE_IDENTIFICATION_PREFIXES = {"classic": "deid",
-                              "DRAPI-Lemur": "De-identified"}
-
 # Define data types. NOTE that all the `String` variables contain numbers with leading zeros that get converted to integers in the current process. Either we convert these variables to `string` or we change the process.
 DATA_TYPES_BO = {"Acct Number - Enter DateTime Comb": "String",
                  "Acct Number - Exit DateTime Comb": "String",
                  "At Station": "String",
                  "Authoring Provider Key": "Numeric",
                  "Authorizing Provider Key": "Numeric",
                  "Chemotherapy Rx Hosp Code Desc": "String",
@@ -111,15 +107,15 @@
 
 DATA_TYPES_DICT = DATA_TYPES_BO.copy()
 DATA_TYPES_DICT.update(DATA_TYPES_I2B2)
 DATA_TYPES_DICT.update(DATA_TYPES_NOTES)
 DATA_TYPES_DICT.update(DATA_TYPES_OMOP)
 
 DATA_TYPES_BY_PORTION = {"BO": DATA_TYPES_BO,
-                         "Clinical Text": DATA_TYPES_NOTES,
+                         "Notes": DATA_TYPES_NOTES,
                          "OMOP": DATA_TYPES_OMOP}
 
 # Convert DRAPI data types to SQL data types
 DRAPI_TO_SQL_DATA_TYPES_MAP = {"Datetime": "TEXT",
                                "Numeric": "INTEGER",
                                "String": "TEXT"}
 DATA_TYPES_DICT_SQL = {name: DRAPI_TO_SQL_DATA_TYPES_MAP[drapiDataType] for name, drapiDataType in DATA_TYPES_DICT.items()}
```

### Comparing `drapi_lemur-1.0.40/src/drapi/code/drapi/constants/phiValues.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/constants/phiValues.py`

 * *Files identical despite different names*

### Comparing `drapi_lemur-1.0.40/src/drapi/code/drapi/constants/phiVariables.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/constants/phiVariables.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Useful definitions used throughout the IDR.
 """
 
-from drapi.code.drapi.drapi import flatExtend
+from drapi.drapi import flatExtend
 
 __all__ = ["LIST_OF_PHI_VARIABLES_BO",
-           "LIST_OF_PHI_VARIABLES_CLINICAL_TEXT",
+           "LIST_OF_PHI_VARIABLES_NOTES",
            "LIST_OF_PHI_VARIABLES_OMOP",
            "VARIABLE_NAME_TO_FILE_NAME_DICT",
            "FILE_NAME_TO_VARIABLE_NAME_DICT"]
 
 DICT_OF_PHI_VARIABLES_BIRTHDATES = {"BO": ["Date Of Birth"],
                                     "OMOP": ["birth_datetime"]}
 DICT_OF_PHI_VARIABLES_AGE = {"BO": ["Current Age",
@@ -36,20 +36,20 @@
                         "Non Cancer Directed Surgery Date",
                         "Other Rx Start Date",
                         "Radiation End Date",
                         "Radiation Start Date",
                         "Surgery Date Summary",
                         "Surgery Discharge Date Summary"]
 
-LIST_OF_PHI_DATES_CLINICAL_TEXT = ["ContactDate",
-                                   "CreatedDatetime",
-                                   "EncounterDate",
-                                   "OrderPlacedDatetime",
-                                   "OrderResultDatetime",
-                                   "ServiceDatetime"]
+LIST_OF_PHI_DATES_NOTES = ["ContactDate",
+                           "CreatedDatetime",
+                           "EncounterDate",
+                           "OrderPlacedDatetime",
+                           "OrderResultDatetime",
+                           "ServiceDatetime"]
 
 LIST_OF_PHI_DATES_OMOP = ["birth_datetime",
                           "condition_end_date",
                           "condition_end_datetime",
                           "condition_start_date",
                           "condition_start_datetime",
                           "death_date",
@@ -115,30 +115,30 @@
                             "Radiation Hosp Code Desc",
                             "Source Sys",
                             "Surgery Rx Hosp Code Desc",
                             "To Station"]
 
 LIST_OF_PHI_VARIABLES_I2B2 = ["LOCATION_CD"]
 
-LIST_OF_PHI_VARIABLES_CLINICAL_TEXT = ["AuthoringProviderKey",
-                                       "AuthorizingProviderKey",
-                                       "CosignProviderKey",
-                                       "EncounterCSN",
-                                       "EncounterKey",
-                                       "LinkageNoteID",
-                                       "MRN_GNV",
-                                       "MRN_JAX",
-                                       "NoteID",
-                                       "NoteKey",
-                                       "OrderID",
-                                       "OrderKey",
-                                       "OrderingProviderKey",
-                                       "PatientKey",
-                                       "Patient Key",
-                                       "ProviderKey"]
+LIST_OF_PHI_VARIABLES_NOTES = ["AuthoringProviderKey",
+                               "AuthorizingProviderKey",
+                               "CosignProviderKey",
+                               "EncounterCSN",
+                               "EncounterKey",
+                               "LinkageNoteID",
+                               "MRN_GNV",
+                               "MRN_JAX",
+                               "NoteID",
+                               "NoteKey",
+                               "OrderID",
+                               "OrderKey",
+                               "OrderingProviderKey",
+                               "PatientKey",
+                               "Patient Key",
+                               "ProviderKey"]
 
 # The list defined `LIST_OF_PHI_VARIABLES_OMOP_BIRTHDATE` is provided for reference. Each variable on its own is not PHI, but in combination with others they are PHI.
 LIST_OF_PHI_VARIABLES_OMOP_BIRTHDATE_CONDITIONAL = ["year_of_birth",
                                                     "month_of_birth",
                                                     "day_of_birth"]
 
 # The list `LIST_OF_PHI_VARIABLES_OMOP_UNINFORMATIVE` contains variables that are not analytically valuable because they only uniquely identify the row in a table.
@@ -160,18 +160,18 @@
                               "patient_key",
                               "preceding_visit_occurrence_id",
                               "provider_id",
                               "visit_occurrence_id"]
 
 LIST_OF_PHI_VARIABLES = flatExtend([LIST_OF_PHI_VARIABLES_BO,
                                     LIST_OF_PHI_VARIABLES_I2B2,
-                                    LIST_OF_PHI_VARIABLES_CLINICAL_TEXT,
+                                    LIST_OF_PHI_VARIABLES_NOTES,
                                     LIST_OF_PHI_VARIABLES_OMOP])
 
-# Variable suffixes: By portion
+# Variable suffixes
 VARIABLE_SUFFIXES_BO = {"Authoring Provider Key": {"columnSuffix": "provider",
                                                    "deIdIDSuffix": "PROV"},
                         "Authorizing Provider Key": {"columnSuffix": "provider",
                                                      "deIdIDSuffix": "PROV"},
                         "Accct Number - Enter DateTime Comb": {"columnSuffix": "account",
                                                                "deIdIDSuffix": "ACCT"},
                         "Acct Number - Exit DateTime Comb": {"columnSuffix": "account",
@@ -245,48 +245,48 @@
                         "Source Sys": {"columnSuffix": "location",
                                        "deIdIDSuffix": "LOC"},
                         "Surgery Rx Hosp Code Desc": {"columnSuffix": "location",
                                                       "deIdIDSuffix": "LOC"},
                         "To Station": {"columnSuffix": "station",
                                        "deIdIDSuffix": "STN"}}
 
-VARIABLE_SUFFIXES_CLINICAL_TEXT = {"AuthoringProviderKey": {"columnSuffix": "provider",
-                                                            "deIdIDSuffix": "PROV"},
-                                   "AuthorizingProviderKey": {"columnSuffix": "provider",
-                                                              "deIdIDSuffix": "PROV"},
-                                   "CosignProviderKey": {"columnSuffix": "provider",
-                                                         "deIdIDSuffix": "PROV"},
-                                   "EncounterCSN": {"columnSuffix": "encounter",
-                                                    "deIdIDSuffix": "ENC"},
-                                   "EncounterKey": {"columnSuffix": "encounter",
-                                                    "deIdIDSuffix": "ENC"},
-                                   "LinkageNoteID": {"columnSuffix": "link_note",
-                                                     "deIdIDSuffix": "LINK_NOTE"},
-                                   "MRN_GNV": {"columnSuffix": "patient",
-                                               "deIdIDSuffix": "PAT"},
-                                   "MRN_JAX": {"columnSuffix": "patient",
-                                               "deIdIDSuffix": "PAT"},
-                                   "NoteID": {"columnSuffix": "note",
-                                              "deIdIDSuffix": "NOTE"},
-                                   "NoteKey": {"columnSuffix": "note",
-                                               "deIdIDSuffix": "NOTE"},
-                                   "OrderID": {"columnSuffix": "order",
-                                               "deIdIDSuffix": "ORD"},
-                                   "OrderKey": {"columnSuffix": "order",
-                                                "deIdIDSuffix": "ORD"},
-                                   "OrderingProviderKey": {"columnSuffix": "order",
-                                                           "deIdIDSuffix": "ORD"},
-                                   "PatientKey": {"columnSuffix": "patient",
-                                                  "deIdIDSuffix": "PAT"},
-                                   "ProviderKey": {"columnSuffix": "provider",
-                                                   "deIdIDSuffix": "PROV"}}
-
 VARIABLE_SUFFIXES_I2B2 = {"LOCATION_CD": {"columnSuffix": "location",
                                           "deIdIDSuffix": "LOC"}}
 
+VARIABLE_SUFFIXES_NOTES = {"AuthoringProviderKey": {"columnSuffix": "provider",
+                                                    "deIdIDSuffix": "PROV"},
+                           "AuthorizingProviderKey": {"columnSuffix": "provider",
+                                                      "deIdIDSuffix": "PROV"},
+                           "CosignProviderKey": {"columnSuffix": "provider",
+                                                 "deIdIDSuffix": "PROV"},
+                           "EncounterCSN": {"columnSuffix": "encounter",
+                                            "deIdIDSuffix": "ENC"},
+                           "EncounterKey": {"columnSuffix": "encounter",
+                                            "deIdIDSuffix": "ENC"},
+                           "LinkageNoteID": {"columnSuffix": "link_note",
+                                             "deIdIDSuffix": "LINK_NOTE"},
+                           "MRN_GNV": {"columnSuffix": "patient",
+                                       "deIdIDSuffix": "PAT"},
+                           "MRN_JAX": {"columnSuffix": "patient",
+                                       "deIdIDSuffix": "PAT"},
+                           "NoteID": {"columnSuffix": "note",
+                                      "deIdIDSuffix": "NOTE"},
+                           "NoteKey": {"columnSuffix": "note",
+                                       "deIdIDSuffix": "NOTE"},
+                           "OrderID": {"columnSuffix": "order",
+                                       "deIdIDSuffix": "ORD"},
+                           "OrderKey": {"columnSuffix": "order",
+                                        "deIdIDSuffix": "ORD"},
+                           "OrderingProviderKey": {"columnSuffix": "order",
+                                                   "deIdIDSuffix": "ORD"},
+                           "PatientKey": {"columnSuffix": "patient",
+                                          "deIdIDSuffix": "PAT"},
+                           "ProviderKey": {"columnSuffix": "provider",
+                                           "deIdIDSuffix": "PROV"}}
+
 VARIABLE_SUFFIXES_OMOP = {"care_site_id": {"columnSuffix": "location",
                                            "deIdIDSuffix": "LOC"},
                           "city": {"columnSuffix": "location",
                                    "deIdIDSuffix": "LOC"},
                           "county": {"columnSuffix": "location",
                                      "deIdIDSuffix": "LOC"},
                           "csn": {"columnSuffix": "encounter",
@@ -301,33 +301,25 @@
                                         "deIdIDSuffix": "PAT"},
                           "preceding_visit_occurrence_id": {"columnSuffix": "encounter",
                                                             "deIdIDSuffix": "ENC"},
                           "provider_id": {"columnSuffix": "provider",
                                           "deIdIDSuffix": "PROV"},
                           "visit_occurrence_id": {"columnSuffix": "encounter",
                                                   "deIdIDSuffix": "ENC"}}
-# Variable suffixes: All
-VARIABLE_SUFFIXES_LIST = [VARIABLE_SUFFIXES_BO,
-                          VARIABLE_SUFFIXES_CLINICAL_TEXT,
-                          VARIABLE_SUFFIXES_I2B2,
-                          VARIABLE_SUFFIXES_OMOP]
-VARIABLE_SUFFIXES = dict()
-for variableSuffixDict in VARIABLE_SUFFIXES_LIST:
-    VARIABLE_SUFFIXES.update(variableSuffixDict)
 
 # Variable name to file name map. This is necessary because some variable names have characters which are not allowed in file names, e.g., "/".
 VARIABLE_NAME_TO_FILE_NAME_DICT = {varName: varName for varName in LIST_OF_PHI_VARIABLES}
 
 # Over-write the necessary values
 VARIABLES_TO_OVER_WRITE = {"F/u Physicians": "F-u Physicians"}
 VARIABLE_NAME_TO_FILE_NAME_DICT.update(VARIABLES_TO_OVER_WRITE)
 FILE_NAME_TO_VARIABLE_NAME_DICT = {fileName: varName for varName, fileName in VARIABLE_NAME_TO_FILE_NAME_DICT.items()}
 
 # QA
 for key in VARIABLE_SUFFIXES_BO.keys():
-    checkBO = key not in list(VARIABLE_SUFFIXES_CLINICAL_TEXT.keys()) + list(VARIABLE_SUFFIXES_OMOP.keys())
-for key in VARIABLE_SUFFIXES_CLINICAL_TEXT.keys():
-    checkClinicalText = key not in list(VARIABLE_SUFFIXES_BO.keys()) + list(VARIABLE_SUFFIXES_OMOP.keys())
+    checkBO = key not in list(VARIABLE_SUFFIXES_NOTES.keys()) + list(VARIABLE_SUFFIXES_OMOP.keys())
+for key in VARIABLE_SUFFIXES_NOTES.keys():
+    checkNotes = key not in list(VARIABLE_SUFFIXES_BO.keys()) + list(VARIABLE_SUFFIXES_OMOP.keys())
 for key in VARIABLE_SUFFIXES_OMOP.keys():
-    checkOMOP = key not in list(VARIABLE_SUFFIXES_BO.keys()) + list(VARIABLE_SUFFIXES_CLINICAL_TEXT.keys())
+    checkOMOP = key not in list(VARIABLE_SUFFIXES_BO.keys()) + list(VARIABLE_SUFFIXES_NOTES.keys())
 
-assert all([checkBO, checkClinicalText, checkOMOP]), "Some variables are present in more than one variable suffix dictionary. This may lead to unintended consequences."
+assert all([checkBO, checkNotes, checkOMOP]), "Some variables are present in more than one variable suffix dictionary. This may lead to unintended consequences."
```

### Comparing `drapi_lemur-1.0.40/src/drapi/code/drapi/deIdentificationSuiteFuncs0/common.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/deIdentificationSuiteFuncs0/common.py`

 * *Files identical despite different names*

### Comparing `drapi_lemur-1.0.40/src/drapi/code/drapi/deIdentificationSuiteFuncs0/concatenateMaps.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/deIdentificationSuiteFuncs0/concatenateMaps.py`

 * *Files identical despite different names*

### Comparing `drapi_lemur-1.0.40/src/drapi/code/drapi/deIdentificationSuiteFuncs0/convertColumns.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/deIdentificationSuiteFuncs0/convertColumns.py`

 * *Files identical despite different names*

### Comparing `drapi_lemur-1.0.40/src/drapi/code/drapi/deIdentificationSuiteFuncs0/dataQualityTest.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/deIdentificationSuiteFuncs0/dataQualityTest.py`

 * *Files identical despite different names*

### Comparing `drapi_lemur-1.0.40/src/drapi/code/drapi/deIdentificationSuiteFuncs0/deIdentify.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/deIdentificationSuiteFuncs0/deIdentify.py`

 * *Files identical despite different names*

### Comparing `drapi_lemur-1.0.40/src/drapi/code/drapi/deIdentificationSuiteFuncs0/deleteColumns.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/deIdentificationSuiteFuncs0/deleteColumns.py`

 * *Files identical despite different names*

### Comparing `drapi_lemur-1.0.40/src/drapi/code/drapi/deIdentificationSuiteFuncs0/gatherFiles.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/deIdentificationSuiteFuncs0/gatherFiles.py`

 * *Files identical despite different names*

### Comparing `drapi_lemur-1.0.40/src/drapi/code/drapi/deIdentificationSuiteFuncs0/getIDValues.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/deIdentificationSuiteFuncs0/getIDValues.py`

 * *Files identical despite different names*

### Comparing `drapi_lemur-1.0.40/src/drapi/code/drapi/deIdentificationSuiteFuncs0/getProjectColumns.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/deIdentificationSuiteFuncs0/getProjectColumns.py`

 * *Files identical despite different names*

### Comparing `drapi_lemur-1.0.40/src/drapi/code/drapi/deIdentificationSuiteFuncs0/makeMapsFromOthers.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/deIdentificationSuiteFuncs0/makeMapsFromOthers.py`

 * *Files identical despite different names*

### Comparing `drapi_lemur-1.0.40/src/drapi/code/drapi/deIdentificationSuiteFuncs0/makeMapsFromScratch.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/deIdentificationSuiteFuncs0/makeMapsFromScratch.py`

 * *Files identical despite different names*

### Comparing `drapi_lemur-1.0.40/src/drapi/code/drapi/deIdentificationSuiteFuncs0/makePersonIDMap.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/deIdentificationSuiteFuncs0/makePersonIDMap.py`

 * *Files identical despite different names*

### Comparing `drapi_lemur-1.0.40/src/drapi/code/drapi/drapi.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/drapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,27 +2,26 @@
 Utility functions commonly used in IDR data request projects.
 """
 
 import datetime as dt
 import logging
 import os
 import re
-import sys
 from array import array
 from collections.abc import Collection
 from datetime import datetime
 from datetime import date
 from datetime import time
 from dateutil.parser import parse
 from itertools import islice
 from logging import Logger
 from pathlib import Path
-from time import sleep
 from typing import Callable, List, Tuple, Union
 from typing_extensions import Literal
+import sys
 # Third-party packages
 import numpy as np
 import pandas as pd
 import sqlalchemy as sa
 import sqlite3
 from pandas.io.parsers.readers import TextFileReader
 # Local packages
@@ -184,55 +183,14 @@
         if commonPrefix == "":
             pathResult = primaryPath
         else:
             pathResult = primaryPath.absolute().relative_to(secondaryPath)
     return pathResult
 
 
-def choosePathToLog(path: Path, rootPath: Path) -> Path:
-    """
-    Decides if a path is a subpath of `rootPath`. If it is, display it reltaive to `rootPath`. If it is not, display it as an absolute path.
-    """
-    commonPath = os.path.commonpath([path.absolute(), rootPath.absolute()])
-
-    lenCommonPath = len(commonPath)
-    lenRootPath = len(str(rootPath.absolute()))
-    if lenCommonPath < lenRootPath:
-        pathToDisplay = path
-    elif lenCommonPath >= lenRootPath:
-        pathToDisplay = path.absolute().relative_to(rootPath)
-    else:
-        raise Exception("An unexpected error occurred.")
-
-    return pathToDisplay
-
-
-def getMapType(df: pd.DataFrame) -> Literal["1:1", "1:m", "m:1", "m:m"]:
-    """
-    h/t to https://stackoverflow.com/questions/59091196
-    """
-    df = df.drop_duplicates()
-    dfShape0 = df.shape
-    assert dfShape0[1] == 2, "Maps are supposed to have only two columns."
-    col1Name, col2Name = df.columns
-
-    first_max = df.groupby(col2Name).count().max().loc[col1Name]
-    second_max = df.groupby(col1Name).count().max().loc[col2Name]
-    if first_max == 1:
-        if second_max == 1:
-            return "1:1"
-        else:
-            return "1:m"
-    else:
-        if second_max == 1:
-            return "m:1"
-        else:
-            return "m:m"
-
-
 def getFilesToRelease(filesToRelease: List[Path], fileCriteria: List[Callable]):
     """
     Applies the functions in the iterable `fileCriteria` to each Path object in `filesToRelease`.
     """
     filesToRelease = []
     for file in filesToRelease:
         criteria = []
@@ -241,15 +199,15 @@
         criteriaMet = all(criteria)
         if criteriaMet:
             filesToRelease.append(file)
         else:
             pass
 
 
-def getLastIDNum(df: pd.DataFrame, columnName="deid_num"):
+def getLastIDNum(df, columnName="deid_num"):
     """
     Gets the last ID number in a de-identification map.
     """
     numbers = df[columnName].astype(int)
     return max(numbers)
 
 
@@ -268,26 +226,14 @@
             return False
         elif "could not convert string to float:" in msg:  # I think this is the new exception message
             return False
         else:
             raise Exception(error)
 
 
-def getSerialNumber(string: str):
-    """
-    Extracts the serial number of a file name using regular expressions.
-    """
-    reObj = re.search("[0-9]+", string)
-    if reObj:
-        result = reObj.group()
-    else:
-        result = "0"
-    return int(result)
-
-
 def fileName2variableName(pathObj):
     """
     """
     pattern = r"^(?P<variableName>.+) map"
     string = pathObj.stem
     obj = re.match(pattern, string)
     if obj:
@@ -438,19 +384,22 @@
     An agnostic converter that takes int or str and returns int. If input is int, output is the same as input"""
     dummy = logging.getLogger("dummy")
     dummy.setLevel(loglevel)
     loglevel = dummy.level
     return loglevel
 
 
-def replace_sql_query(query: str, old: str, new: str, logger: logging.Logger) -> str:
+def replace_sql_query(query: str, old: str, new: str, loglevel: Union[int, str] = "INFO") -> str:
     """
     Replaces text in a SQL query only if it's not commented out. I.e., this function applies string.replace() only if the string doesn't begin with "--".
     TODO Don't replace text after "--".
     """
+    loglevel_asnumber = loglevel2int(loglevel)
+    logger.setLevel(loglevel_asnumber + 10)
+
     pattern = r"^\w*--"
     li = query.split("\n")
     result = []
     logger.debug("Starting")
     for line in li:
         logger.debug(f"""  Working on "{line}".""")
         obj = re.search(pattern, line)
@@ -756,17 +705,15 @@
 
 # >>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
 # >>> tree function >>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
 # >>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
 # h/t https://stackoverflow.com/a/59109706/5478086
 
 
-def tree(dir_path: Path,
-         level: int = -1,
-         limit_to_directories: bool = False,
+def tree(dir_path: Path, level: int = -1, limit_to_directories: bool = False,
          length_limit: int = 1000):
     """Given a directory Path object print a visual tree structure"""
     # prefix components:
     space = '    '
     branch = '│   '
     # pointers:
     tee = '├── '
```

### Comparing `drapi_lemur-1.0.40/src/drapi/code/drapi/idealist/getEncountersMap.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/idealist/getEncountersMap.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 Outline
 
     - Initilalize an empty pandas dataframe as the master de-identification map.
     - Iterate over the encounter SQLite database files.
     - For each file, append the encounter de-identification maps to the master map.
 """
 
-# NOTE See DNR folder for latest version
+""" NOTE See DNR folder for latest version
 # Private variables ("dunders")
 __all__ = ["encounterMapDf"]
 
 # Imports
 from pathlib import Path
 import logging
 import os
 import re
 import sys
 # Third-party packages
 import numpy as np
 import pandas as pd
 import sqlite3
 # Local imports
-from drapi.code.drapi.drapi import sqlite2df, getTimestamp, replace_sql_query, makeChunks
+from drapi.drapi import sqlite2df, getTimestamp, replace_sql_query, makeChunks
 
 # Arguments
 QUERY_PATH = Path("sql/encounterNumber2patientKey.SQL")
 DATABSE_DIR_MAC = os.path.join("/",
                                "Volumes",
                                "FILES",
                                "FTP",
@@ -167,7 +167,8 @@
     # Create final de-identification map.
     if False:
         COLUMN_NAME = None
         encounterMapDf[COLUMN_NAME] = encounterMapDf["deiden_id"].apply(lambda integer: f"{integer}")
 
     # Script end
     logging.info(f"""Finished running "{thisFilePath}".""")
+"""
```

### Comparing `drapi_lemur-1.0.40/src/drapi/code/drapi/idealist/getPatientsMap.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/idealist/getPatientsMap.py`

 * *Files identical despite different names*

### Comparing `drapi_lemur-1.0.40/src/drapi/code/drapi/idealist/idealist.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/idealist/idealist.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Herman's utility functions commonly used in his IDEALIST projects
 """
 
 __all__ = ["idealistMap2dict",
            "patientKey2MRNs"]
 
 from pathlib import Path
-from drapi.code.drapi.drapi import replace_sql_query
+from drapi.drapi import replace_sql_query
 import os
 import pandas as pd
 import sqlalchemy as sa
 
 # Variables
 this_file_path = Path(__file__)
 this_file_stem = this_file_path.stem
```

### Comparing `drapi_lemur-1.0.40/src/drapi/code/drapi/images/utilities.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/images/utilities.py`

 * *Files identical despite different names*

### Comparing `drapi_lemur-1.0.40/src/drapi/code/drapi/makeSymLinks.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/makeSymLinks.py`

 * *Files identical despite different names*

### Comparing `drapi_lemur-1.0.40/src/drapi/code/drapi/notes/freeText.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/notes/freeText.py`

 * *Files identical despite different names*

### Comparing `drapi_lemur-1.0.40/src/drapi/code/drapi/notes/pullNotes.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/notes/pullNotes.py`

 * *Files identical despite different names*

### Comparing `drapi_lemur-1.0.40/src/drapi/code/drapi/notes/utils.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/notes/utils.py`

 * *Files identical despite different names*

### Comparing `drapi_lemur-1.0.40/src/drapi/code/drapi/omop/configProcessing.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/omop/configProcessing.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,26 +4,24 @@
 
 import os
 import sys
 from pathlib import Path
 # Third-party packages
 import yaml
 # Custom packages
-from drapi.code.drapi.drapi import successiveParents
+from drapi.drapi import successiveParents
 
 
 def interpretPath(pathAsString: str) -> str:
     """
     Makes sure path separators are appropriate for the current operating system.
     """
     operatingSystem = sys.platform
     if operatingSystem == "darwin":
         newPathAsString = pathAsString.replace("\\", "/")
-    elif operatingSystem == "linux":
-        newPathAsString = pathAsString.replace("\\", "/")
     elif operatingSystem == "win32":
         newPathAsString = pathAsString.replace("/", "\\")
     else:
         raise Exception("Unsupported operating system")
     return newPathAsString
```

### Comparing `drapi_lemur-1.0.40/src/drapi/code/drapi/omop/deidentify.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/omop/deidentify.py`

 * *Files identical despite different names*

### Comparing `drapi_lemur-1.0.40/src/drapi/code/drapi/oneFlorida/oneFlorida.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/oneFlorida.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import os
 from pathlib import Path
 from typing_extensions import Literal
 # Third-party packages
 import pandas as pd
 # Local packages
 from drapi.code.drapi.drapi import replace_sql_query, successiveParents
-from drapi.code.drapi.oneFlorida import ID_TYPE_DICT
 
 
 # Arguments: SQL connection settings
 SERVER = "DWSRSRCH01.shands.ufl.edu"
 DATABASE = "DWS_PROD"
 USERDOMAIN = "UFAD"
 USERNAME = os.environ["USER"]
@@ -47,21 +46,15 @@
                               new=listAsString)
 
     MRNseries = pd.read_sql(query, con=conStr)
 
     return MRNseries
 
 
-def mapOneFloridaIDs(IDTypeValues: pd.Series,
-                     IDType: Literal["PATID",
-                                     "Patient Key",
-                                     "MRN (UF)",
-                                     "MRN (Jax)",
-                                     "MRN (Pathology)"],
-                     returnQueryOnly: bool) -> pd.Series:
+def mapOneFloridaIDs(IDTypeValues: pd.Series, IDType: Literal["PATID", "Patient Key", "MRN (UF)", "MRN (Jax)", "MRN (Pathology)"]) -> pd.Series:
     """
     Queries the ID map containing all of the following variables, any of which can be used as a query filter using the `IDType` parameter. The values to query by are used in the `IDTypeValues` parameter.
         | Variable Definition           | Standard or Common Column Name    |
         |-------------------------------|-----------------------------------|
         | OneFlorida patient ID         | OneFlorida Patient ID             |
         | IDR patient key               | Patient Key                       |
         | UF Health Gainesvile MRN      | MRN (UF)                          |
@@ -74,21 +67,20 @@
     with open(sqlFilePath2, "r") as file:
         query0 = file.read()
 
     query = replace_sql_query(query=query0,
                               old="{PYTHON_VARIABLE: IDTypeValues}",
                               new=listAsString)
     IDTypeInput = IDType.lower()
-    IDTypeDict = ID_TYPE_DICT.copy()
+    IDTypeDict = {"oneflorida patient id": "a.PATID",
+                  "patient key": "a.PATNT_KEY",
+                  "mrn (uf)": "b.IDENT_ID",
+                  "mrn (jax)": "c.IDENT_ID",
+                  "mrn (pathology)": "d.IDENT_ID"}
     IDTypeSQL = IDTypeDict[IDTypeInput]
     query = replace_sql_query(query=query,
                               old="{PYTHON_VARIABLE: IDTypeSQL}",
                               new=IDTypeSQL)
 
-    if returnQueryOnly:
-        return query
-    else:
-        pass
-
-    dfResults = pd.read_sql(query, con=conStr)
+    MRNseries = pd.read_sql(query, con=conStr)
 
-    return dfResults
+    return MRNseries
```

### Comparing `drapi_lemur-1.0.40/src/drapi/code/drapi/prepTSVforSDOH.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/prepTSVforSDOH.py`

 * *Files identical despite different names*

### Comparing `drapi_lemur-1.0.40/src/drapi/code/drapi/qa/columnConversion.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/deleteByColumnValues.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,137 +1,208 @@
 """
-Quality Assurance functions to make sure columns were properly converted or de-identified.
+Deletes rows based on column values.
 """
 
 import logging
+import os
+import sys
+from pathlib import Path
 # Third-party packages
 import pandas as pd
-# First-party packages
+# Local packages
+from drapi.code.drapi.drapi import (getTimestamp,
+                                    makeDirPath,
+                                    successiveParents)
+# Local packages: Script parameters: General
+from drapi.constants.phiValues import PHI_VALUES_DICT_ALL
+# Local packages: Script parameters: General
+# Local packages: Script parameters: Paths
+# Local packages: Script parameters: File criteria
+from common import BO_PORTION_FILE_CRITERIA
+
+# Arguments
+COLUMN_VALUES_TO_DROP = PHI_VALUES_DICT_ALL
+
+# Arguments: OMOP data set selection
+USE_MODIFIED_OMOP_DATA_SET = True
+
+# Arguments: Portion Paths and conditions
+MAC_PATHS = [Path(r"..\Concatenated Results\data\output\deIdentifyByAge\...")]
+WIN_PATHS = [Path(r"..\Concatenated Results\data\output\deIdentifyByAge\...")]
+
+LIST_OF_PORTION_CONDITIONS = [BO_PORTION_FILE_CRITERIA]
+
+# Arguments; General
+CHUNK_SIZE = 50000
+
+# Arguments: Meta-variables
+PROJECT_DIR_DEPTH = 2
+DATA_REQUEST_DIR_DEPTH = PROJECT_DIR_DEPTH + 2
+IRB_DIR_DEPTH = DATA_REQUEST_DIR_DEPTH + 0
+IDR_DATA_REQUEST_DIR_DEPTH = IRB_DIR_DEPTH + 3
+
+ROOT_DIRECTORY = "IRB_DIRECTORY"  # TODO One of the following:
+                                                 # ["IDR_DATA_REQUEST_DIRECTORY",    # noqa
+                                                 #  "IRB_DIRECTORY",                 # noqa
+                                                 #  "DATA_REQUEST_DIRECTORY",        # noqa
+                                                 #  "PROJECT_OR_PORTION_DIRECTORY"]  # noqa
+
+LOG_LEVEL = "INFO"
+
+# Arguments: SQL connection settings
+SERVER = "DWSRSRCH01.shands.ufl.edu"
+DATABASE = "DWS_PROD"
+USERDOMAIN = "UFAD"
+USERNAME = os.environ["USER"]
+UID = None
+PWD = os.environ["HFA_UFADPWD"]
+
+# Variables: Path construction: General
+runTimestamp = getTimestamp()
+thisFilePath = Path(__file__)
+thisFileStem = thisFilePath.stem
+projectDir, _ = successiveParents(thisFilePath.absolute(), PROJECT_DIR_DEPTH)
+dataRequestDir, _ = successiveParents(thisFilePath.absolute(), DATA_REQUEST_DIR_DEPTH)
+IRBDir, _ = successiveParents(thisFilePath, IRB_DIR_DEPTH)
+IDRDataRequestDir, _ = successiveParents(thisFilePath.absolute(), IDR_DATA_REQUEST_DIR_DEPTH)
+dataDir = projectDir.joinpath("data")
+if dataDir:
+    inputDataDir = dataDir.joinpath("input")
+    outputDataDir = dataDir.joinpath("output")
+    if outputDataDir:
+        runOutputDir = outputDataDir.joinpath(thisFileStem, runTimestamp)
+logsDir = projectDir.joinpath("logs")
+if logsDir:
+    runLogsDir = logsDir.joinpath(thisFileStem)
+sqlDir = projectDir.joinpath("sql")
+
+if ROOT_DIRECTORY == "PROJECT_OR_PORTION_DIRECTORY":
+    rootDirectory = projectDir
+elif ROOT_DIRECTORY == "DATA_REQUEST_DIRECTORY":
+    rootDirectory = dataRequestDir
+elif ROOT_DIRECTORY == "IRB_DIRECTORY":
+    rootDirectory = IRBDir
+elif ROOT_DIRECTORY == "IDR_DATA_REQUEST_DIRECTORY":
+    rootDirectory = IDRDataRequestDir
+else:
+    raise Exception("An unexpected error occurred.")
+
+# Variables: Path construction: OS-specific
+isAccessible = all([path.exists() for path in MAC_PATHS]) or all([path.exists() for path in WIN_PATHS])
+if isAccessible:
+    # If you have access to either of the below directories, use this block.
+    operatingSystem = sys.platform
+    if operatingSystem == "darwin":
+        listOfPortionDirs = MAC_PATHS[:]
+    elif operatingSystem == "win32":
+        listOfPortionDirs = WIN_PATHS[:]
+    else:
+        raise Exception("Unsupported operating system")
+else:
+    # If the above option doesn't work, manually copy the database to the `input` directory.
+    print("Not implemented. Check settings in your script.")
+    sys.exit()
+
+# Variables: Path construction: Project-specific
 pass
 
-# Functions
+# Variables: SQL Parameters
+if UID:
+    uid = UID[:]
+else:
+    uid = fr"{USERDOMAIN}\{USERNAME}"
+conStr = f"mssql+pymssql://{uid}:{PWD}@{SERVER}/{DATABASE}"
 
-def spotCheckColumns(listOfFiles1: list,
-                     listofFiles2: list,
-                     connectionString: str,
-                     logger: logging.Logger,
-                     moduloChunks: int,
-                     chunkSize: int = 50_000,
-                     messageModuloChunks: int = 50,
-                     messageModuloFiles: int = 100,
-                     columnsToCheck1: dict[int: str] = {0: "visit_occurrence_id",
-                                                        1: "person_id",
-                                                        2: "provider_id"},
-                     columnsToCheck2: dict[int: str] = {0: "Encounter # (CSN)",
-                                                        1: "Patient Key",
-                                                        2: "Provider Key"}) -> None:
-    """
-    This function "spot checks" pairs of files to see if the passed variables have been properly converted from the OMOP data model to the UF Health data model.
-
-    In `columnsToCheck1` and `columnsToCheck2` the keys of the dictionary have the following meaning:
-    - 0: Encounter ID Variable Name
-    - 1: Patient ID Variable Name
-    - 2: Provider ID Variable Name
-
-    The code is only meant to check these three ID types, because under the hood these integer values are mapped to SQL queries. So, for example, you could not pass `{0: "Note Key"}` to the function, because it would use the SQL query that maps encounter IDs.
-
-    NOTE This has only been tested and verified on 3-on-3 checks. That is, checking if all three informative OMOP ID variables have been mapped to their three UF Health equivalents. The code should be able to also do spot checks for less number of variables, like just `person_id` to `Patient Key`, but it has not been tested.
-    """
-    with open("../Concatenated Results/sql/BO Variable Spot Check - Encounter # (CSN).sql", "r") as file:
-        query0_0 = file.read()
-    with open("../Concatenated Results/sql/BO Variable Spot Check - Patient Key.sql", "r") as file:
-        query1_0 = file.read()
-    with open("../Concatenated Results/sql/BO Variable Spot Check - Provider Key.sql", "r") as file:
-        query2_0 = file.read()
-
-    for file1, file2 in zip(listOfFiles1, listofFiles2):
-        try:
-            logger.info(f"""  Working on file pair:
-        `file1`: "{file1}"
-        `file2`: "{file2}".""")
-            df2_0 = pd.read_csv(file2, nrows=2)
-            df2_0columns = df2_0.columns
-            columnChecks2 = df2_0columns.isin(columnsToCheck2.values())
-            logger.debug(f"""  Group 2 table:\n{df2_0.to_string()}""")
-            logger.debug(f"""  Group 2 columns:\n{df2_0.columns}""")
-            logger.debug(f"""  Group 2 columns check:\n{columnChecks2}""")
-            spot2df = df2_0.loc[0, columnChecks2]
-            spot2df = pd.DataFrame(spot2df)  # For type hinting
-            logger.info(f"  A row has been selected for a spot check:\n{spot2df.T.to_string()}")
-            # Convert group 2 spot to group 1 values
-            spot2dict = spot2df.to_dict()[0]
-            logger.info(spot2dict)
-            query0_1 = query0_0[:]
-            query1_1 = query1_0[:]
-            query2_1 = query2_0[:]
-            spot1dict = {}
-            if 0 in columnsToCheck2.keys():
-                encounterIDVariableName = columnsToCheck2[0]
-                if df2_0columns.isin([encounterIDVariableName]).sum() > 0:
-                    queryEncounterIDValue = spot2dict[encounterIDVariableName]
-                    query0_1 = query0_1.replace("{PYTHON_VARIABLE: Encounter # (CSN)}", str(queryEncounterIDValue))
-                    result0 = pd.read_sql(sql=query0_1, con=connectionString)
-                    if result0.shape != (1,2):
-                        logger.warning(f"""  ..  The encounter ID mapping is not one-to-one:\n{result0.to_string()}.""")
-                        spot1EncounterID = None  # NOTE This is a dummy value assigned to the variable to allow the code to continue running, but at the same time to indicate that an unexpected or undesired result has occurred.
-                    else:
-                        spot1EncounterID = result0["visit_occurrence_id"][0]
-                    spot1dict["visit_occurrence_id"] = [spot1EncounterID]
-            if 1 in columnsToCheck2.keys():
-                patientIDVariableName = columnsToCheck2[1]
-                if df2_0columns.isin([patientIDVariableName]).sum() > 0:
-                    queryPatientIDValue = spot2dict[patientIDVariableName]
-                    query1_1 = query1_1.replace("{PYTHON_VARIABLE: Patient Key}", str(queryPatientIDValue))
-                    result1 = pd.read_sql(sql=query1_1, con=connectionString)
-                    if result1.shape != (1,2):
-                        logger.warning(f"""  ..  The patient ID mapping is not one-to-one:\n{result1.to_string()}.""")
-                        spot1PatientID = None  # NOTE This is a dummy value assigned to the variable to allow the code to continue running, but at the same time to indicate that an unexpected or undesired result has occurred.
-                    else:
-                        spot1PatientID = result1["person_id"][0]
-                    spot1dict["person_id"] = [spot1PatientID]
-            if 1 in columnsToCheck2.keys():
-                providerIDVariableName = columnsToCheck2[2]
-                if df2_0columns.isin([providerIDVariableName]).sum() > 0:
-                    queryProviderIDValue = spot2dict[providerIDVariableName]
-                    query2_1 = query2_1.replace("{PYTHON_VARIABLE: Provider Key}", str(queryProviderIDValue))
-                    result2 = pd.read_sql(sql=query2_1, con=connectionString)
-                    if result2.shape != (1,2):
-                        logger.warning(f"""  ..  The provider ID mapping is not one-to-one:\n{result2.to_string()}.""")
-                        spot1ProviderID = None  # NOTE This is a dummy value assigned to the variable to allow the code to continue running, but at the same time to indicate that an unexpected or undesired result has occurred.
-                    else:
-                        spot1ProviderID = result2["provider_id"][0]
-                    spot1dict["provider_id"] = [spot1ProviderID]
-            spot1Targetdf = pd.DataFrame.from_dict(data=spot1dict, orient="columns")
-            logger.info(f"""The values that we are looking for in the group 1 set of files is below:\n{spot1Targetdf}""" )
-            # Chunk
-            chunkGenerator1 = pd.read_csv(file1, chunksize=chunkSize, low_memory=False)
-            chunkGenerator2 = pd.read_csv(file1, chunksize=chunkSize, low_memory=False)
-            logger.info("    Counting the number of chunks in the file.")
-            it1Total = sum([1 for _ in chunkGenerator1])
-            logger.info(f"    Counting the number of chunks in the file - done. There are {it1Total:,} chunks.")
-            if it1Total < messageModuloChunks:
-                moduloChunks = it1Total
-            else:
-                moduloChunks = round(it1Total / messageModuloChunks)
-            if it1Total / moduloChunks < 100:
-                moduloChunks = 1
+# Variables: Other
+pass
+
+# Directory creation: General
+makeDirPath(runOutputDir)
+makeDirPath(runLogsDir)
+
+# Logging block
+logpath = runLogsDir.joinpath(f"log {runTimestamp}.log")
+logFormat = logging.Formatter("""[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s""")
+
+logger = logging.getLogger(__name__)
+
+fileHandler = logging.FileHandler(logpath)
+fileHandler.setLevel(9)
+fileHandler.setFormatter(logFormat)
+
+streamHandler = logging.StreamHandler()
+streamHandler.setLevel(LOG_LEVEL)
+streamHandler.setFormatter(logFormat)
+
+logger.addHandler(fileHandler)
+logger.addHandler(streamHandler)
+
+logger.setLevel(9)
+
+if __name__ == "__main__":
+    logger.info(f"""Begin running "{thisFilePath}".""")
+    logger.info(f"""All other paths will be reported in debugging relative to `{ROOT_DIRECTORY}`: "{rootDirectory}".""")
+    logger.info(f"""Script arguments:
+
+
+    # Arguments
+    `COLUMN_VALUES_TO_DROP`: "{COLUMN_VALUES_TO_DROP}"
+    `USE_MODIFIED_OMOP_DATA_SET`: "{USE_MODIFIED_OMOP_DATA_SET}"
+    `MAC_PATHS`: "{MAC_PATHS}"
+    `WIN_PATHS`: "{WIN_PATHS}"
+
+    # Arguments: General
+    `PROJECT_DIR_DEPTH`: "{PROJECT_DIR_DEPTH}" ----------> "{projectDir}"
+    `IRB_DIR_DEPTH`: "{IRB_DIR_DEPTH}" --------------> "{IRBDir}"
+    `IDR_DATA_REQUEST_DIR_DEPTH`: "{IDR_DATA_REQUEST_DIR_DEPTH}" -> "{IDRDataRequestDir}"
+
+    `LOG_LEVEL` = "{LOG_LEVEL}"
+
+    # Arguments: SQL connection settings
+    `SERVER` = "{SERVER}"
+    `DATABASE` = "{DATABASE}"
+    `USERDOMAIN` = "{USERDOMAIN}"
+    `USERNAME` = "{USERNAME}"
+    `UID` = "{UID}"
+    `PWD` = censored
+    """)
+
+    logger.info("""De-identifying files.""")
+    for directory, fileConditions in zip(listOfPortionDirs, LIST_OF_PORTION_CONDITIONS):
+        # Act on directory
+        logger.info(f"""Working on directory "{directory.absolute().relative_to(rootDirectory)}".""")
+        for file in directory.iterdir():
+            logger.info(f"""  Working on file "{file.absolute().relative_to(rootDirectory)}".""")
+            conditions = [condition(file) for condition in fileConditions]
+            if all(conditions):
+                # Set file options
+                exportPath = runOutputDir.joinpath(file.name)
+                fileMode = "w"
+                fileHeaders = True
+                # Read file
+                logger.info("""    File has met all conditions for processing.""")
+                logger.info("""  ..  Reading file to count the number of chunks.""")
+                numChunks = sum([1 for _ in pd.read_csv(file, chunksize=CHUNK_SIZE)])
+                logger.info(f"""  ..  This file has {numChunks} chunks.""")
+                dfChunks = pd.read_csv(file, chunksize=CHUNK_SIZE)
+                for it, dfChunk in enumerate(dfChunks, start=1):
+                    dfChunk = pd.DataFrame(dfChunk)
+                    # Work on chunk
+                    logger.info(f"""  ..  Working on chunk {it} of {numChunks}.""")
+                    for columnName in dfChunk.columns:
+                        # Work on column
+                        logger.info(f"""  ..    Working on column "{columnName}".""")
+                        if columnName in COLUMN_VALUES_TO_DROP.keys():
+                            mask = ~dfChunk[columnName].isin(COLUMN_VALUES_TO_DROP[columnName])
+                            if mask.sum() > 0:
+                                logger.info("""  ..  ..  Column has values that need to be dropped. Dropping values.""")
+                            dfChunk = dfChunk[mask]
+                    # Save chunk
+                    dfChunk.to_csv(exportPath, mode=fileMode, header=fileHeaders, index=False)
+                    fileMode = "a"
+                    fileHeaders = False
+                    logger.info(f"""  ..  Chunk saved to "{exportPath.absolute().relative_to(rootDirectory)}".""")
             else:
-                pass
-            for it1, df1Chunk in enumerate(chunkGenerator2, start=1):
-                if it1 % moduloChunks == 0:
-                    allowLogging = True
-                else:
-                    allowLogging = False
-                if allowLogging:
-                    logger.info(f"""  ..  Working on chunk {it1:,} of {it1Total:,}.""")
-                df1Chunk = pd.DataFrame(df1Chunk)  # For type hinting
-                columnChecks1 = df1Chunk.columns.isin(columnsToCheck1.values())
-                df1 = df1Chunk.loc[:, columnChecks1]
-                df1 = pd.DataFrame(df1)  # For type hinting
-                mask = df1.isin(spot1Targetdf.values.flatten()).all(axis=1)
-                rowLocation = mask.index[mask][0]
-                if mask.sum() > 0:
-                    spot1Hitdf = df1[mask]
-                    logger.info(f"""    Found spot located at index value (row number) "{rowLocation}":\n{spot1Hitdf.to_string()}.""")
-                    break
-        except Exception as error:
-            logger.fatal(error)
+                logger.info("""    This file does not need to be processed.""")
+
+    # End script
+    logger.info(f"""Finished running "{thisFilePath.relative_to(projectDir)}".""")
```

### Comparing `drapi_lemur-1.0.40/src/drapi/code/drapi/sql.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/sql.py`

 * *Files identical despite different names*

### Comparing `drapi_lemur-1.0.40/src/drapi/code/drapi/stats.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/stats.py`

 * *Files identical despite different names*

### Comparing `drapi_lemur-1.0.40/src/drapi/sql/9-Digit Zip Code.SQL` & `drapi-lemur-1.0.5/src/drapi/sql/9-Digit Zip Code.SQL`

 * *Files identical despite different names*

### Comparing `drapi_lemur-1.0.40/src/drapi/sql/Consent2Share.sql` & `drapi-lemur-1.0.5/src/drapi/sql/Consent2Share.sql`

 * *Files identical despite different names*

### Comparing `drapi_lemur-1.0.40/src/drapi/sql/ConvertBetweenMrnAndOneFloridaPatID.SQL` & `drapi-lemur-1.0.5/src/drapi/sql/ConvertBetweenMrnAndOneFloridaPatID.SQL`

 * *Files identical despite different names*

### Comparing `drapi_lemur-1.0.40/src/drapi/sql/LADMF.sql` & `drapi-lemur-1.0.5/src/drapi/sql/LADMF.sql`

 * *Files identical despite different names*

### Comparing `drapi_lemur-1.0.40/src/drapi/sql/MRNfromPatientKey.sql` & `drapi-lemur-1.0.5/src/drapi/sql/MRNfromPatientKey.sql`

 * *Files identical despite different names*

### Comparing `drapi_lemur-1.0.40/src/drapi/sql/encounterNumber2patientKey.SQL` & `drapi-lemur-1.0.5/src/drapi/sql/encounterNumber2patientKey.SQL`

 * *Files identical despite different names*

### Comparing `drapi_lemur-1.0.40/src/drapi/templates/Anaconda Environment Variables/RenameMe environment-name/README.md` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/Anaconda Environment Variables/RenameMe environment-name/README.md`

 * *Files identical despite different names*

### Comparing `drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/.gitignore` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # >>> [start] Things added by Herman >>>
 **/logs/*
 **/*.7z
 **/.DS_Store
 **/*.bat
 !**/launchIPython.bat
 **/*.csv
-**/*.out
 **/*.pdf
 **/*.tsv
 **/*.xlsx
 **/*.zip
 # <<< [end] Things added by Herman <<<
 
 # >>> [start] Default IDR files >>>
@@ -132,15 +131,15 @@
 celerybeat-schedule
 celerybeat.pid
 
 # SageMath parsed files
 *.sage.py
 
 # Environments
-.env
+!.env
 .venv
 env/
 venv/
 ENV/
 env.bak/
 venv.bak/
```

### Comparing `drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/.gitignore` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # >>> [start] Things added by Herman >>>
 **/logs/*
 **/*.7z
 **/.DS_Store
 **/*.bat
 !**/launchIPython.bat
 **/*.csv
-**/*.out
 **/*.pdf
 **/*.tsv
 **/*.xlsx
 **/*.zip
 # <<< [end] Things added by Herman <<<
 
 # >>> [start] Default IDR files >>>
```

### Comparing `drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/README.md` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -45,21 +45,21 @@
 
 | File(s) Description                  | File(s) path or directory                                                             | Process that uses the file(s) |
 | ------------------------------------ | ------------------------------------------------------------------------------------- | ----------------------------- |
 | Original OMOP data set               | "IRB000000000/Intermediate Results/OMOP Portion/data/output/..."                      | makePersonIDMaps.py           |
 | OMOP Person ID map                   | "IRB000000000/Concatenated Results/data/output/makePersonIDMap/.../person_id map.csv" | convertColumns.py             |
 | Original OMOP data set               | "IRB000000000/Intermediate Results/OMOP Portion/data/output/..."                      | convertColumns.py             |
 | Modified OMOP files                  | "IRB000000000/Concatenated Results/data/output/convertColumns/..."                    | getIDValues.py                |
-| Clinical text metadata data set              | "IRB000000000/Intermediate Results/Clinical Text Portion/data/output/free_text"               | getIDValues.py                |
-| Clinical Text Portion de-identification maps | "IRB000000000/Intermediate Results/Clinical Text Portion/data/output/mapping"                 | makeMapsFromOthers.py         |
+| Notes metadata data set              | "IRB000000000/Intermediate Results/Notes Portion/data/output/free_text"               | getIDValues.py                |
+| Notes portion de-identification maps | "IRB000000000/Intermediate Results/Notes Portion/data/output/mapping"                 | makeMapsFromOthers.py         |
 | ID Sets (map intermediate files)     | "IRB000000000/Concatenated Results/data/output/getIDValues/..."                       | makeMapsFromOthers.py         |
-| Clinical Text Portion de-identification maps | "IRB000000000/Intermediate Results/Clinical Text Portion/data/output/mapping"                 | concatenateMaps.py            |
+| Notes portion de-identification maps | "IRB000000000/Intermediate Results/Notes Portion/data/output/mapping"                 | concatenateMaps.py            |
 | De-identification maps               | "IRB000000000/Concatenated Results/data/output/makeMapsFromOthers/..."                | concatenateMaps.py            |
 | De-identification maps               | "IRB000000000/Concatenated Results/data/output/makeMapsFromOthers/..."                | deIdentify.py                 |
 | Modified OMOP files                  | "IRB000000000/Concatenated Results/data/output/convertColumns/..."                    | deIdentify.py                 |
-| Clinical text metadata data set              | "IRB000000000/Intermediate Results/Clinical Text Portion/data/output/free_text"               | deIdentify.py                 |
+| Notes metadata data set              | "IRB000000000/Intermediate Results/Notes Portion/data/output/free_text"               | deIdentify.py                 |
 | De-identified data set               | "IRB000000000/Concatenated Results/data/output/deIdentify/..."                        | deleteColumns.py              |
 | Reduced de-identified data set       | "IRB000000000/Concatenated Results/data/output/deleteColumns/..."                     | gatherFiles.py                |
-| De-identified notes data set         | "IRB000000000/Intermediate Results/De-identified Clinical Text/..."                           | gatherFiles.py                |
+| De-identified notes data set         | "IRB000000000/Intermediate Results/De-identified Notes/..."                           | gatherFiles.py                |
 | Final results                        |                                                                                       | Honest broker                 |
 
 ____________________________________________________________
```

### Comparing `drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/aliasVariables.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/aliasVariables.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import pandas as pd
 from pandas.errors import EmptyDataError
 from sqlalchemy import create_engine
 # Local packages
 from drapi.code.drapi.drapi import (getTimestamp,
                                     makeDirPath,
                                     successiveParents)
-from drapi.code.drapi.constants.phiVariables import VARIABLE_NAME_TO_FILE_NAME_DICT, FILE_NAME_TO_VARIABLE_NAME_DICT
+from drapi.constants.phiVariables import VARIABLE_NAME_TO_FILE_NAME_DICT, FILE_NAME_TO_VARIABLE_NAME_DICT
 # Super-local
 from common import VARIABLE_ALIASES, DATA_TYPES_DICT
 
 # Arguments
 SET_FILES_DIR = Path(r"..\Concatenated Results\data\output\getIDValues\...\Set Files")
 
 # Arguments: Meta-variables
@@ -98,15 +98,15 @@
 
 # Directory creation: General
 makeDirPath(runOutputDir)
 makeDirPath(runLogsDir)
 
 # Logging block
 logpath = runLogsDir.joinpath(f"log {runTimestamp}.log")
-logFormat = logging.Formatter("[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s")
+logFormat = logging.Formatter("""[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s""")
 
 logger = logging.getLogger(__name__)
 
 fileHandler = logging.FileHandler(logpath)
 fileHandler.setLevel(9)
 fileHandler.setFormatter(logFormat)
```

### Comparing `drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/common.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/common.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,47 +1,67 @@
 """
 Variable constants common to this project
 """
 
 __all__ = ["COLUMNS_TO_DE_IDENTIFY",
+           "BO_PORTION_DIR_MAC",
+           "BO_PORTION_DIR_WIN",
            "MODIFIED_OMOP_PORTION_DIR_MAC",
            "MODIFIED_OMOP_PORTION_DIR_WIN",
-           "CLINICAL_TEXT_PORTION_DIR_MAC",
-           "CLINICAL_TEXT_PORTION_DIR_WIN",
+           "MODIFIED_I2B2_PORTION_DIR_MAC",
+           "MODIFIED_I2B2_PORTION_DIR_WIN",
+           "NOTES_PORTION_DIR_MAC",
+           "NOTES_PORTION_DIR_WIN",
            "OLD_MAPS_DIR_PATH",
            "OMOP_PORTION_DIR_MAC",
-           "OMOP_PORTION_DIR_WIN"]
+           "OMOP_PORTION_DIR_WIN",
+           "SDOH_PORTION_DIR_MAC",
+           "SDOH_PORTION_DIR_WIN"]
 
-import re
 from pathlib import Path
 # Local packages
-from drapi.code.drapi.constants.constants import DATA_TYPES_DICT
-from drapi.code.drapi.constants.phiVariables import (LIST_OF_PHI_VARIABLES_BO,
-                                                     LIST_OF_PHI_VARIABLES_I2B2,
-                                                     LIST_OF_PHI_VARIABLES_CLINICAL_TEXT,
-                                                     LIST_OF_PHI_VARIABLES_OMOP,
-                                                     VARIABLE_NAME_TO_FILE_NAME_DICT,
-                                                     VARIABLE_SUFFIXES_BO,
-                                                     VARIABLE_SUFFIXES_I2B2,
-                                                     VARIABLE_SUFFIXES_CLINICAL_TEXT,
-                                                     VARIABLE_SUFFIXES_OMOP)
-from drapi.code.drapi.constants.variableAliases import VARIABLE_ALIASES
+from drapi.constants.constants import DATA_TYPES_DICT
+from drapi.constants.phiVariables import (LIST_OF_PHI_VARIABLES_BO,
+                                          LIST_OF_PHI_VARIABLES_I2B2,
+                                          LIST_OF_PHI_VARIABLES_NOTES,
+                                          LIST_OF_PHI_VARIABLES_OMOP,
+                                          VARIABLE_NAME_TO_FILE_NAME_DICT,
+                                          VARIABLE_SUFFIXES_BO,
+                                          VARIABLE_SUFFIXES_I2B2,
+                                          VARIABLE_SUFFIXES_NOTES,
+                                          VARIABLE_SUFFIXES_OMOP)
 from drapi.code.drapi.drapi import flatExtend
 
 # Project parameters: Meta-variables
 STUDY_TYPE = "Limited Data Set (LDS)"  # Pick from "Non-Human", "Limited Data Set (LDS)", "Identified"
 IRB_NUMBER = None  # TODO
 DATA_REQUEST_ROOT_DIRECTORY_DEPTH = 3  # TODO  # NOTE To prevent unexpected results, like moving, writing, or deleting the wrong files, set this to folder that is the immediate parent of concatenated result and the intermediate results folder.
 
 
 # Project parameters: Aliases: Definitions  # TODO
 # NOTE: Some variable names are not standardized. This section is used by the de-identification process when looking for the de-identification map. This way several variables can be de-identified with the same map. If you have variables with a custom, non-BO name, you should alias them, if necessary using the following format:
 # VAR_ALIASES_CUSTOM_VARS = {"Custom Variable 1": "BO Equivalent 1",
 #                            "Custom Variable 2": "BO Equivalent 2"}
-pass
+VAR_ALIASES_NOTES_ENCOUNTERS = {"EncounterCSN": "Encounter # (CSN)"}
+VAR_ALIASES_NOTES_PATIENTS = {"MRN_GNV": "MRN (UF)",
+                              "MRN_JAX": "MRN (Jax)",
+                              "PatientKey": "Patient Key"}
+VAR_ALIASES_NOTES_PROVIDERS = {"AuthoringProviderKey": "ProviderKey",
+                               "AuthorizingProviderKey": "ProviderKey",
+                               "CosignProviderKey": "ProviderKey",
+                               "OrderingProviderKey": "ProviderKey"}
+VAR_ALIASES_SDOH_ENCOUNTERS = {"NOTE_ENCNTR_KEY": "LinkageNoteID",
+                               "NOTE_KEY": "NoteKey"}
+LIST_OF_ALIAS_DICTS = [VAR_ALIASES_NOTES_ENCOUNTERS,
+                       VAR_ALIASES_NOTES_PATIENTS,
+                       VAR_ALIASES_NOTES_PROVIDERS,
+                       VAR_ALIASES_SDOH_ENCOUNTERS]
+VARIABLE_ALIASES = {}
+for di in LIST_OF_ALIAS_DICTS:
+    VARIABLE_ALIASES.update(di)
 
 # Project parameters: Aliases: Data types  # TODO
 # NOTE Add each variable in `VARIABLE_ALIASES` to `ALIAS_DATA_TYPES`.
 ALIAS_DATA_TYPES_MANUAL = {}  # TODO
 ALIAS_DATA_TYPES_AUTOMATIC = {}
 for alias, variableName in VARIABLE_ALIASES.items():
     if alias not in DATA_TYPES_DICT.keys():
@@ -82,62 +102,84 @@
 # Project parameters: Columns to de-identify
 if STUDY_TYPE.lower() == "Non-Human":
     LIST_OF_PHI_VARIABLES_TO_KEEP = []
 else:
     LIST_OF_PHI_VARIABLES_TO_KEEP = []
 COLUMNS_TO_DE_IDENTIFY = flatExtend([LIST_OF_PHI_VARIABLES_BO,
                                      LIST_OF_PHI_VARIABLES_I2B2,
-                                     LIST_OF_PHI_VARIABLES_CLINICAL_TEXT,
+                                     LIST_OF_PHI_VARIABLES_NOTES,
                                      LIST_OF_PHI_VARIABLES_OMOP,
                                      LIST_OF_PHI_VARIABLES_FROM_ALIASES])
 COLUMNS_TO_DE_IDENTIFY = [variableName for variableName in COLUMNS_TO_DE_IDENTIFY if variableName not in LIST_OF_PHI_VARIABLES_TO_KEEP]
 
 # Project parameters: Variable suffixes
 VARIABLE_SUFFIXES_LIST = [VARIABLE_SUFFIXES_BO,
                           VARIABLE_SUFFIXES_I2B2,
-                          VARIABLE_SUFFIXES_CLINICAL_TEXT,
+                          VARIABLE_SUFFIXES_NOTES,
                           VARIABLE_SUFFIXES_OMOP]
 VARIABLE_SUFFIXES = dict()
 for variableSuffixDict in VARIABLE_SUFFIXES_LIST:
     VARIABLE_SUFFIXES.update(variableSuffixDict)
 
 # Project parameters: Portion directories
+BO_PORTION_DIR_MAC = Path(r"../Intermediate Results/BO Portion/data/output/getData/...")  # TODO
+BO_PORTION_DIR_WIN = Path(r"..\Intermediate Results\BO Portion\data\output\getData\...")  # TODO
+
+
+I2B2_PORTION_DIR_MAC = Path(r"../Concatenated Results/data/output/i2b2ConvertIDs/...")  # TODO
+I2B2_PORTION_DIR_WIN = Path(r"..\Concatenated Results\data\output\i2b2ConvertIDs\...")  # TODO
+
 MODIFIED_OMOP_PORTION_DIR_MAC = Path("data/output/convertColumns/...")  # TODO
 MODIFIED_OMOP_PORTION_DIR_WIN = Path(r"data\output\convertColumns\...")  # TODO
 
-CLINICAL_TEXT_ROOT_DIRECTORY = Path("../../Intermediate Results/Clinical Text Portion/data/output/freeText/...")  # TODO
-CLINICAL_TEXT_PORTION_DIR_MAC = CLINICAL_TEXT_ROOT_DIRECTORY.joinpath("free_text")
-CLINICAL_TEXT_PORTION_DIR_WIN = CLINICAL_TEXT_ROOT_DIRECTORY.joinpath("free_text")
+MODIFIED_I2B2_PORTION_DIR_MAC = Path(r"../Concatenated Results/data/output/i2b2ConvertIDs/...")  # TODO
+MODIFIED_I2B2_PORTION_DIR_WIN = Path(r"..\Concatenated Results\data\output\i2b2ConvertIDs\...")  # TODO
+
+NOTES_ROOT_DIRECTORY = Path(r"..\Intermediate Results\Notes Data Portion\data\output\2023-11-20 16-37-27")  # TODO
+NOTES_PORTION_DIR_MAC = NOTES_ROOT_DIRECTORY.joinpath("free_text")
+NOTES_PORTION_DIR_WIN = NOTES_ROOT_DIRECTORY.joinpath("free_text")
+
+OMOP_PORTION_DIR_MAC = Path(r"Intermediate Results/OMOP Portion/data/output/...")  # TODO
+OMOP_PORTION_DIR_WIN = Path(r"Intermediate Results\OMOP Portion\data\output\...")  # TODO
 
-OMOP_PORTION_DIR_MAC = Path("../../Intermediate Results/OMOP Portion/data/output/.../identified")  # TODO
-OMOP_PORTION_DIR_WIN = Path("../../Intermediate Results/OMOP Portion/data/output/.../identified")  # TODO
+SDOH_PORTION_DIR_MAC = Path(r"..\Intermediate Results\SDoH Portion")  # TODO
+SDOH_PORTION_DIR_WIN = Path(r"..\Intermediate Results\SDoH Portion")  # TODO
 
 # Project parameters: File criteria
-CLINICAL_TEXT_PORTION_FILE_CRITERIA = [lambda pathObj: pathObj.suffix.lower() == ".csv",
-                                       lambda pathObj: True if re.search(pattern=r"metadata_\d+.csv",
-                                                                         string=pathObj.name) else False]
+BO_PORTION_FILE_CRITERIA = [lambda pathObj: pathObj.suffix.lower() == ".csv"]
+I2B2_PORTION_FILE_CRITERIA = [lambda pathObj: pathObj.suffix.lower() == ".csv"]
+NOTES_PORTION_FILE_CRITERIA = [lambda pathObj: pathObj.suffix.lower() == ".csv"]
 OMOP_PORTION_FILE_CRITERIA = [lambda pathObj: pathObj.suffix.lower() == ".csv"]
+SDOH_PORTION_FILE_CRITERIA = [lambda pathObj: pathObj.suffix.lower() == ".tsv"]
 
 
 # Project parameters: Maps
-OLD_MAPS_DIR_PATH = {"EncounterCSN": [CLINICAL_TEXT_ROOT_DIRECTORY.joinpath("mapping/map_encounter.csv")],
-                     "LinkageNoteID": [CLINICAL_TEXT_ROOT_DIRECTORY.joinpath("mapping/map_note_link.csv")],
-                     "NoteKey": [CLINICAL_TEXT_ROOT_DIRECTORY.joinpath("mapping/map_note.csv")],
-                     "OrderKey": [CLINICAL_TEXT_ROOT_DIRECTORY.joinpath("mapping/map_order.csv")],
-                     "PatientKey": [CLINICAL_TEXT_ROOT_DIRECTORY.joinpath("mapping/map_patient.csv")],
-                     "ProviderKey": [CLINICAL_TEXT_ROOT_DIRECTORY.joinpath("mapping/map_provider.csv")]}
+OLD_MAPS_DIR_PATH = {"EncounterCSN": [NOTES_ROOT_DIRECTORY.joinpath("mapping/map_encounter.csv")],
+                     "LinkageNoteID": [NOTES_ROOT_DIRECTORY.joinpath("mapping/map_note_link.csv")],
+                     "NoteKey": [NOTES_ROOT_DIRECTORY.joinpath("mapping/map_note.csv")],
+                     "OrderKey": [NOTES_ROOT_DIRECTORY.joinpath("mapping/map_order.csv")],
+                     "PatientKey": [NOTES_ROOT_DIRECTORY.joinpath("mapping/map_patient.csv")],
+                     "ProviderKey": [NOTES_ROOT_DIRECTORY.joinpath("mapping/map_provider.csv")]}
 
 # Quality assurance
 if __name__ == "__main__":
-    ALL_VARS = [MODIFIED_OMOP_PORTION_DIR_MAC,
+    ALL_VARS = [BO_PORTION_DIR_MAC,
+                BO_PORTION_DIR_WIN,
+                I2B2_PORTION_DIR_MAC,
+                I2B2_PORTION_DIR_WIN,
+                MODIFIED_OMOP_PORTION_DIR_MAC,
                 MODIFIED_OMOP_PORTION_DIR_WIN,
-                CLINICAL_TEXT_ROOT_DIRECTORY,
-                CLINICAL_TEXT_PORTION_DIR_MAC,
-                CLINICAL_TEXT_PORTION_DIR_WIN,
+                MODIFIED_I2B2_PORTION_DIR_MAC,
+                MODIFIED_I2B2_PORTION_DIR_WIN,
+                NOTES_ROOT_DIRECTORY,
+                NOTES_PORTION_DIR_MAC,
+                NOTES_PORTION_DIR_WIN,
                 OMOP_PORTION_DIR_MAC,
-                OMOP_PORTION_DIR_WIN]
+                OMOP_PORTION_DIR_WIN,
+                SDOH_PORTION_DIR_MAC,
+                SDOH_PORTION_DIR_WIN]
 
     for li in OLD_MAPS_DIR_PATH.values():
         ALL_VARS.extend(li)
 
     for path in ALL_VARS:
         print(path.exists())
```

### Comparing `drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/concatenateMaps.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/concatenateMaps.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Makes de-identification maps, building on existing maps.
 
 # NOTE Does not expect data in nested directories (e.g., subfolders of "free_text"). Therefore it uses "Path.iterdir" instead of "Path.glob('*/**')".
+# NOTE Expects all files to be CSV files. This is because it uses "pd.read_csv".
 """
 
 import logging
 import re
 from collections import OrderedDict
 from pathlib import Path
 # Third-party packages
@@ -13,15 +14,15 @@
 import pprint
 # Local packages
 from drapi.code.drapi.drapi import (getTimestamp,
                                     makeDirPath,
                                     getPercentDifference,
                                     successiveParents,
                                     makeMap)
-from drapi.code.drapi.constants.phiVariables import (VARIABLE_NAME_TO_FILE_NAME_DICT,
+from drapi.constants.phiVariables import (VARIABLE_NAME_TO_FILE_NAME_DICT,
                                           FILE_NAME_TO_VARIABLE_NAME_DICT)
 # Project parameters: General
 from common import (IRB_NUMBER,
                     DATA_REQUEST_ROOT_DIRECTORY_DEPTH,
                     OLD_MAPS_DIR_PATH,
                     VARIABLE_ALIASES,
                     VARIABLE_SUFFIXES)
```

### Comparing `drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/concatenateTables.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/code/getData.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 """
-Concatenates files by converting them to Pandas DataFrames and using `pd.concat`.
+Script template to pull BO data using a query filter.
 """
 
 import logging
 import os
 from pathlib import Path
 # Third-party packages
 import pandas as pd
+from sqlalchemy import create_engine
 # Local packages
 from drapi.code.drapi.drapi import (getTimestamp,
                                     makeDirPath,
-                                    readDataFile,
                                     successiveParents)
+# Super-local imports
+from functions import checkFileConditions, getData, getData2
 
 # Arguments
-LIST_OF_FILE_PATHS = Path(r"..\..").iterdir()
-TARGET_FILE_PATH = Path()
+LIST_OF_SQL_FILES = []  # TODO
+COHORT_FILE_PATH = ""  # TODO
+USE_QUERY_FILTER = False  # TODO
 
-CHUNKSIZE = 10000
+QUERY_CHUNK_SIZE = 10000
 
 # Arguments: Meta-variables
 PROJECT_DIR_DEPTH = 2
 DATA_REQUEST_DIR_DEPTH = PROJECT_DIR_DEPTH + 2
 IRB_DIR_DEPTH = DATA_REQUEST_DIR_DEPTH + 0
 IDR_DATA_REQUEST_DIR_DEPTH = IRB_DIR_DEPTH + 3
 
@@ -76,14 +79,21 @@
 
 # Variables: SQL Parameters
 if UID:
     uid = UID[:]
 else:
     uid = fr"{USERDOMAIN}\{USERNAME}"
 conStr = f"mssql+pymssql://{uid}:{PWD}@{SERVER}/{DATABASE}"
+connection = create_engine(conStr).connect().execution_options(stream_results=True)
+
+# Variables: Other
+if not USE_QUERY_FILTER:
+    getDataFunction = getData
+else:
+    getDataFunction = getData2
 
 # Directory creation: General
 makeDirPath(runOutputDir)
 makeDirPath(runLogsDir)
 
 # Logging block
 logpath = runLogsDir.joinpath(f"log {runTimestamp}.log")
@@ -105,19 +115,18 @@
 logger.setLevel(9)
 
 if __name__ == "__main__":
     logger.info(f"""Begin running "{thisFilePath}".""")
     logger.info(f"""All other paths will be reported in debugging relative to `{ROOT_DIRECTORY}`: "{rootDirectory}".""")
     logger.info(f"""Script arguments:
 
-
     # Arguments
-    `LIST_OF_FILE_PATHS`: "{LIST_OF_FILE_PATHS}"
-    `TARGET_FILE_PATH`: "{TARGET_FILE_PATH}"
-    `CHUNKSIZE`: "{CHUNKSIZE}"
+    `LIST_OF_SQL_FILES`: "{LIST_OF_SQL_FILES}"
+    `USE_QUERY_FILTER`: "{USE_QUERY_FILTER}"
+    `COHORT_FILE_PATH`: "{COHORT_FILE_PATH}"
 
     # Arguments: General
     `PROJECT_DIR_DEPTH`: "{PROJECT_DIR_DEPTH}" ----------> "{projectDir}"
     `IRB_DIR_DEPTH`: "{IRB_DIR_DEPTH}" --------------> "{IRBDir}"
     `IDR_DATA_REQUEST_DIR_DEPTH`: "{IDR_DATA_REQUEST_DIR_DEPTH}" -> "{IDRDataRequestDir}"
 
     `LOG_LEVEL` = "{LOG_LEVEL}"
@@ -127,30 +136,30 @@
     `DATABASE` = "{DATABASE}"
     `USERDOMAIN` = "{USERDOMAIN}"
     `USERNAME` = "{USERNAME}"
     `UID` = "{UID}"
     `PWD` = censored
     """)
 
-    # Concatenate files
-    mode = "w"
-    numFiles = len(LIST_OF_FILE_PATHS)
-    logger
-    for it1, fpath in enumerate(sorted(LIST_OF_FILE_PATHS), start=1):
-        logger.info(f"""  Working on file {it1:,} of {numFiles:,}: {fpath.absolute().relative_to(projectDir)}.""")
-        logger.info("""    Counting the number of chunks.""")
-        numChunks = sum([1 for _ in readDataFile(fname=fpath,
-                                                 chunksize=CHUNKSIZE)])
-        logger.info("""    Counting the number of chunks - done.""")
-        fileChunks = readDataFile(fname=fpath,
-                                  chunksize=CHUNKSIZE)
-        for it2, df in enumerate(fileChunks, start=1):
-            logger.info(f"""    Working on chunk {it2:,} of {numChunks:,}: {fpath.absolute().relative_to(projectDir)}.""")
-            df = pd.DataFrame(df)
-            topath = TARGET_FILE_PATH.joinpath(fpath.name)
-            df.to_csv(topath)
+    # Read cohort file
+    logger.info("""Reading cohort file.""")
+    cohortData = pd.read_csv(COHORT_FILE_PATH)
+    logger.info("""Reading cohort file - done.""")
+
+    # Iterate over SQL directory contents
+    logger.info("""Iterating over SQL directory contents.""")
+    sqlFiles = sorted(LIST_OF_SQL_FILES)
+    for sqlFilePath in sqlFiles:
+        checkFileConditions(sqlFilePath=sqlFilePath,
+                            cohortData=cohortData,
+                            stepNumberCondition="NA",
+                            logger=logger,
+                            conStr=conStr,
+                            runOutputDir=runOutputDir,
+                            getDataFunction=getDataFunction,
+                            queryChunkSize=QUERY_CHUNK_SIZE)
 
     # Output location summary
     logger.info(f"""Script output is located in the following directory: "{runOutputDir.absolute().relative_to(rootDirectory)}".""")
 
     # End script
-    logger.info(f"""Finished running "{thisFilePath.relative_to(projectDir)}".""")
+    logger.info(f"""Finished running "{thisFilePath.absolute().relative_to(rootDirectory)}".""")
```

### Comparing `drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/convertColumns.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/convertColumns.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """
 Convert person ID column to patient key
 
 # NOTE Does not expect data in nested directories (e.g., subfolders of "free_text"). Therefore it uses "Path.iterdir" instead of "Path.glob('*/**')".
+# NOTE Expects all files to be CSV files. This is because it uses "pd.read_csv".
 """
 
 import logging
 import sys
 from pathlib import Path
 # Third-party packages
 import pandas as pd
 # Local packages
 from drapi.code.drapi.drapi import (getTimestamp,
                                     makeDirPath,
                                     readDataFile,
                                     successiveParents)
-from drapi.code.drapi.idealist.idealist import idealistMap2dict
+from drapi.idealist.idealist import idealistMap2dict
 # Local packages: Script parameters: General
 from common import DATA_REQUEST_ROOT_DIRECTORY_DEPTH
 # Local packages: Script parameters: Paths
 from common import OMOP_PORTION_DIR_MAC, OMOP_PORTION_DIR_WIN
 # Local packages: Script parameters: File criteria
 from common import OMOP_PORTION_FILE_CRITERIA
 
@@ -131,16 +132,16 @@
             if all(conditions):
                 # Set file options
                 exportPath = runOutputDir.joinpath(file.name)
                 fileMode = "w"
                 fileHeaders = True
                 # Read file
                 logging.info("""    File has met all conditions for processing.""")
-                numChunks = sum([1 for _ in readDataFile(file, chunksize=CHUNK_SIZE)])
-                dfChunks = readDataFile(file, chunksize=CHUNK_SIZE)
+                numChunks = sum([1 for _ in readDataFile(file, chunkSize=CHUNK_SIZE)])
+                dfChunks = readDataFile(file, chunkSize=CHUNK_SIZE)
                 for it, dfChunk in enumerate(dfChunks, start=1):
                     dfChunk = pd.DataFrame(dfChunk)
                     logging.info(f"""  ..  Working on chunk {it} of {numChunks}.""")
                     for columnName in dfChunk.columns:
                         logging.info(f"""  ..    Working on column "{columnName}".""")
                         if columnName in COLUMNS_TO_CONVERT_DI.keys():
                             logging.info("""  ..  ..  Column must be converted. Converting values.""")
```

### Comparing `drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/convertColumnsGeneral.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/getIDValues.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,101 +1,89 @@
 """
-Convert columns.
+Get the set of ID values for all variables to de-identify.
 
-# NOTE This is a more general form of the OMOP-only version, "convertColumns.py"
 # NOTE Does not expect data in nested directories (e.g., subfolders of "free_text"). Therefore it uses "Path.iterdir" instead of "Path.glob('*/**')".
-# TODO Assign portion name to each path (per OS) so that portion files are stored in their respective folders, this prevents file from being overwritten in the unlikely, but possible, case files from different portions have the same name.
+# NOTE Expects all files to be CSV files. This is because it uses "pd.read_csv".
 """
 
+__all__ = ["runIntermediateDataDir"]
+
+import csv
+import json
 import logging
-import os
 import sys
 from pathlib import Path
 # Third-party packages
 import pandas as pd
-import sqlite3
+from pandas.errors import EmptyDataError
 # Local packages
-from drapi.code.drapi.drapi import (flatExtend,
-                                    getTimestamp,
+from drapi.code.drapi.drapi import (getTimestamp,
                                     makeDirPath,
-                                    makeMap,
                                     readDataFile,
+                                    sortIntegersAndStrings,
                                     successiveParents)
-# Local packages: Script parameters: General
-from common import (IRB_NUMBER,
-                    ALIAS_DATA_TYPES,
+from drapi.constants.phiVariables import VARIABLE_NAME_TO_FILE_NAME_DICT
+# Project parameters: General
+from common import (COLUMNS_TO_DE_IDENTIFY,
                     DATA_REQUEST_ROOT_DIRECTORY_DEPTH,
-                    DATA_TYPES_DICT,
-                    VARIABLE_ALIASES,
-                    VARIABLE_SUFFIXES)
-# Local packages: Script parameters: Paths
-from common import (MODIFIED_OMOP_PORTION_DIR_MAC, MODIFIED_OMOP_PORTION_DIR_WIN,
+                    DATA_TYPES_DICT)
+# Project parameters: Portion paths and criteria
+from common import (BO_PORTION_DIR_MAC, BO_PORTION_DIR_WIN,
+                    I2B2_PORTION_DIR_MAC, I2B2_PORTION_DIR_WIN,
+                    MODIFIED_OMOP_PORTION_DIR_MAC, MODIFIED_OMOP_PORTION_DIR_WIN,
                     NOTES_PORTION_DIR_MAC, NOTES_PORTION_DIR_WIN,
-                    OMOP_PORTION_DIR_MAC, OMOP_PORTION_DIR_WIN,
-                    OMOP_PORTION_2_DIR_MAC, OMOP_PORTION_2_DIR_WIN)
-# Local packages: Script parameters: File criteria
-from common import (NOTES_PORTION_FILE_CRITERIA,
+                    OMOP_PORTION_DIR_MAC, OMOP_PORTION_DIR_WIN)
+# Project parameters: Criteria
+from common import (BO_PORTION_FILE_CRITERIA,
+                    I2B2_PORTION_FILE_CRITERIA,
+                    NOTES_PORTION_FILE_CRITERIA,
                     OMOP_PORTION_FILE_CRITERIA)
 
+
 # Arguments
-if True:
-    MAPS = {"provider_id": {"to": "Provider Key",
-                            "mapPath": r"../Concatenated Results/data/output/mapToSqlite/2024-02-23 17-36-14/provider_id to Provider Key.db"}}
-    MAC_PATHS = [Path("/data/herman/mnt/ufhsd/SHANDS/SHARE/DSS/IDR Data Requests/ACTIVE RDRs/Liu/IRB202300703/Concatenated Results/data/output/convertColumnsGeneral/2024-01-24 17-48-25"),
-                 Path("/data/herman/mnt/ufhsd/SHANDS/SHARE/DSS/IDR Data Requests/ACTIVE RDRs/Liu/IRB202300703/Concatenated Results/data/output/convertColumnsGeneral/2024-01-26 20-17-44")]
-    WIN_PATHS = []
-    LIST_OF_PORTION_CONDITIONS = [OMOP_PORTION_FILE_CRITERIA,
-                                  OMOP_PORTION_FILE_CRITERIA]
-elif False:
-    MAPS = {"person_id": {"to": "PatientKey",
-                          "mapPath": r"..\Concatenated Results\data\output\mapToSqlite\2024-01-22 20-58-28\person_id to PatientKey.db"}}
-    MAC_PATHS = [OMOP_PORTION_DIR_MAC]
-    WIN_PATHS = [OMOP_PORTION_DIR_WIN]
-    LIST_OF_PORTION_CONDITIONS = [OMOP_PORTION_FILE_CRITERIA + [lambda pathObj: pathObj.stem != "condition_occurrence"]]
-elif True:
-    MAPS = {"person_id": {"to": "PatientKey",
-                          "mapPath": r"..\Concatenated Results\data\output\mapToSqlite\2024-01-22 20-58-28\person_id to PatientKey.db"},
-            "visit_occurrence_id": {"to": "Encounter # (CSN)",
-                                    "mapPath": r"..\Concatenated Results\data\output\mapToSqlite\2024-01-22 21-11-13\visit_occurrence_id to Encounter # (CSN).db"}}
-    MAC_PATHS = [OMOP_PORTION_DIR_MAC,
-                 OMOP_PORTION_2_DIR_MAC]
-    WIN_PATHS = [OMOP_PORTION_DIR_WIN,
-                 OMOP_PORTION_2_DIR_WIN]
-    previouslyDoneFiles = flatExtend([[fpath.stem for fpath in Path(r"..\Concatenated Results\data\output\convertColumnsGeneral\2024-01-24 17-48-25").iterdir()],
-                                      []])
-    newOMOPFileCriteria = OMOP_PORTION_FILE_CRITERIA + [lambda pathObj: pathObj.stem not in previouslyDoneFiles]
-    LIST_OF_PORTION_CONDITIONS = [newOMOPFileCriteria,
-                                  newOMOPFileCriteria]
-elif True:
-    MAPS = {"PatientKey": {"to": "De-identified PatientKey",
-                           "mapPath": r""},
-            "EncounterCSN": {"to": "De-identified EncounterCSN",
-                             "mapPath": r""}}
-    MAC_PATHS = [MODIFIED_OMOP_PORTION_DIR_MAC,
-                 NOTES_PORTION_DIR_MAC]
-    WIN_PATHS = [MODIFIED_OMOP_PORTION_DIR_WIN,
-                 NOTES_PORTION_DIR_WIN]
-    LIST_OF_PORTION_CONDITIONS = [OMOP_PORTION_FILE_CRITERIA,
-                                  NOTES_PORTION_FILE_CRITERIA]
+SETS_INTERMEDIATE_PATH = None
 
-# Arguments; General
 CHUNK_SIZE = 50000
-MESSAGE_MODULO_CHUNKS = 100  # How often to print a log message, i.e., print a message every x number of chunks, where x is `MESSAGE_MODULO_CHUNKS`
+
+# Arguments: OMOP data set selection
+USE_MODIFIED_OMOP_DATA_SET = True
+
+# Arguments: Portion Paths and conditions
+if USE_MODIFIED_OMOP_DATA_SET:
+    OMOPPortionDirMac = MODIFIED_OMOP_PORTION_DIR_MAC
+    OMOPPortionDirWin = MODIFIED_OMOP_PORTION_DIR_WIN
+else:
+    OMOPPortionDirMac = OMOP_PORTION_DIR_MAC
+    OMOPPortionDirWin = OMOP_PORTION_DIR_WIN
+
+PORTION_PATHS_MAC = {"BO": BO_PORTION_DIR_MAC,
+                     "i2b2": I2B2_PORTION_DIR_MAC,
+                     "Notes": NOTES_PORTION_DIR_MAC,
+                     "OMOP": OMOPPortionDirMac}
+PORTION_PATHS_WIN = {"BO": BO_PORTION_DIR_WIN,
+                     "i2b2": I2B2_PORTION_DIR_WIN,
+                     "Notes": NOTES_PORTION_DIR_WIN,
+                     "OMOP": OMOPPortionDirWin}
+
+DICT_OF_PORTION_CONDITIONS = {"BO": BO_PORTION_FILE_CRITERIA,
+                              "i2b2": I2B2_PORTION_FILE_CRITERIA,
+                              "Notes": NOTES_PORTION_FILE_CRITERIA,
+                              "OMOP": OMOP_PORTION_FILE_CRITERIA}
 
 # Arguments: Meta-variables
 CONCATENATED_RESULTS_DIRECTORY_DEPTH = DATA_REQUEST_ROOT_DIRECTORY_DEPTH - 1
 PROJECT_DIR_DEPTH = CONCATENATED_RESULTS_DIRECTORY_DEPTH  # The concatenation suite of scripts is considered to be the "project".
 IRB_DIR_DEPTH = CONCATENATED_RESULTS_DIRECTORY_DEPTH + 2
 IDR_DATA_REQUEST_DIR_DEPTH = IRB_DIR_DEPTH + 3
 
 ROOT_DIRECTORY = "DATA_REQUEST_DIRECTORY"  # TODO One of the following:
-# ["IDR_DATA_REQUEST_DIRECTORY",      # noqa
-#  "IRB_DIRECTORY",                   # noqa
-#  "DATA_REQUEST_DIRECTORY",          # noqa
-#  "CONCATENATED_RESULTS_DIRECTORY"]  # noqa
+                                           # ["IDR_DATA_REQUEST_DIRECTORY",      # noqa
+                                           #  "IRB_DIRECTORY",                   # noqa
+                                           #  "DATA_REQUEST_DIRECTORY",          # noqa
+                                           #  "CONCATENATED_RESULTS_DIRECTORY"]  # noqa
 
 LOG_LEVEL = "INFO"
 
 # Variables: Path construction: General
 runTimestamp = getTimestamp()
 thisFilePath = Path(__file__)
 thisFileStem = thisFilePath.stem
@@ -123,56 +111,34 @@
     rootDirectory = dataRequestDir
 elif ROOT_DIRECTORY == "IRB_DIRECTORY":
     rootDirectory = IRBDir
 elif ROOT_DIRECTORY == "IDR_DATA_REQUEST_DIRECTORY":
     rootDirectory = IDRDataRequestDir
 
 # Variables: Path construction: OS-specific
-isAccessible = all([path.exists() for path in MAC_PATHS]) or all([path.exists() for path in WIN_PATHS])
+isAccessible = all([path.exists() for path in PORTION_PATHS_MAC.values()]) or all([path.exists() for path in PORTION_PATHS_WIN.values()])
 if isAccessible:
     # If you have access to either of the below directories, use this block.
     operatingSystem = sys.platform
     if operatingSystem == "darwin":
-        listOfPortionDirs = MAC_PATHS[:]
-    elif operatingSystem == "linux":
-        listOfPortionDirs = MAC_PATHS[:]
+        dictOfPortionPaths = PORTION_PATHS_MAC.copy()
     elif operatingSystem == "win32":
-        listOfPortionDirs = WIN_PATHS[:]
+        dictOfPortionPaths = PORTION_PATHS_WIN.copy()
     else:
         raise Exception("Unsupported operating system")
 else:
     # If the above option doesn't work, manually copy the database to the `input` directory.
     print("Not implemented. Check settings in your script.")
     sys.exit()
 
 # Directory creation: General
 makeDirPath(runIntermediateDataDir)
 makeDirPath(runOutputDir)
 makeDirPath(runLogsDir)
 
-# Functions
-
-def choosePathToLog(path: Path, rootPath: Path) -> Path:
-    """
-    Decides if a path is a subpath of `rootPath`. If it is, display it reltaive to `rootPath`. If it is not, display it as an absolute path.
-    """
-    commonPath = os.path.commonpath([path.absolute(), rootPath.absolute()])
-
-    lenCommonPath = len(commonPath)
-    lenRootPath = len(str(rootPath.absolute()))
-    if lenCommonPath < lenRootPath:
-        pathToDisplay = path
-    elif lenCommonPath >= lenRootPath:
-        pathToDisplay = path.absolute().relative_to(rootPath)
-    else:
-        raise Exception("An unexpected error occurred.")
-                                    
-    return pathToDisplay
-
-
 if __name__ == "__main__":
     # Logging block
     logpath = runLogsDir.joinpath(f"log {runTimestamp}.log")
     fileHandler = logging.FileHandler(logpath)
     fileHandler.setLevel(LOG_LEVEL)
     streamHandler = logging.StreamHandler()
     streamHandler.setLevel(LOG_LEVEL)
@@ -180,162 +146,135 @@
     logging.basicConfig(format="[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s",
                         handlers=[fileHandler, streamHandler],
                         level=LOG_LEVEL)
 
     logging.info(f"""Begin running "{thisFilePath}".""")
     logging.info(f"""All other paths will be reported in debugging relative to `{ROOT_DIRECTORY}`: "{rootDirectory}".""")
 
-    # Assert all portions have file criteria accounted for
-    if len(listOfPortionDirs) == len(LIST_OF_PORTION_CONDITIONS):
-        pass
+    # Match portion paths and conditions
+    portionPathsAndConditions = {portionName: (dictOfPortionPaths[portionName], DICT_OF_PORTION_CONDITIONS[portionName]) for portionName in dictOfPortionPaths.keys()}
+    check1 = [pn1 in DICT_OF_PORTION_CONDITIONS.keys() for pn1 in dictOfPortionPaths.keys()]
+    check2 = [pn2 in dictOfPortionPaths.keys() for pn2 in DICT_OF_PORTION_CONDITIONS.keys()]
+    assert sum(check1) == len(check1), "Not all portion paths are associated with a portion condition"
+    assert sum(check2) == len(check2), "Not all portion conditions are associated with a portion path"
+
+    # Misc
+    columnSetsVarsDiFname = "Column Sets Dict.JSON"
+
+    # Get set of values
+    if SETS_INTERMEDIATE_PATH:
+        logging.info(f"""Using the set of values previously collected from "{SETS_INTERMEDIATE_PATH}".""")
+        with open(SETS_INTERMEDIATE_PATH.joinpath(columnSetsVarsDiFname)) as file:
+            columnSetsVarsDi = json.loads(file.read())
     else:
-        raise Exception("The number of portions does not equal the number of portion conditions.")
-
-    # Collect columns to convert
-    columnsToConvert = sorted(list(MAPS.keys()))
-
-    # Load de-identification maps for each variable that needs to be de-identified
-    logging.info("""Loading de-identification maps for each variable that needs to be de-identified.""")
-    mapsDi = {}
-    mapsColumnNames = {}
-    variablesCollected = [fname for fname in MAPS.keys()]
-    for varName in variablesCollected:
-        logging.info(f"""  Loading map for "{varName}".""")
-        toVariable = MAPS[varName]["to"]
-        varPath = MAPS[varName]["mapPath"]
-        tableName = f"{varName} to {toVariable}"
-        with sqlite3.connect(varPath) as connection:
-            map_ = pd.read_sql_query(sql=f"SELECT * FROM '{tableName}' LIMIT 1", con=connection)
-        mapsDi[varName] = map_
-        mapsColumnNames[varName] = map_.columns[-1]
-    # Add aliases to `mapsColumnNames`
-    for varName in VARIABLE_ALIASES.keys():
-        varAlias = VARIABLE_ALIASES[varName]
-        map_ = makeMap(IDset=set(),
-                       IDName=varName,
-                       startFrom=1,
-                       irbNumber=IRB_NUMBER,
-                       suffix=VARIABLE_SUFFIXES[varAlias]["deIdIDSuffix"],
-                       columnSuffix=varName,
-                       deIdentificationMapStyle="lemur",
-                       logger=logging.getLogger())
-        mapsColumnNames[varName] = map_.columns[-1]
-    # Add aliases to `DATA_TYPES_DICT`
-    DATA_TYPES_DICT.update(ALIAS_DATA_TYPES)
-
-    # De-identify columns
-    logging.info("""De-identifying files.""")
-    allowLogging = False
-    for directory, fileConditions in zip(listOfPortionDirs, LIST_OF_PORTION_CONDITIONS):
-        # Act on directory
-        logging.info(f"""Working on directory "{choosePathToLog(directory, rootDirectory)}".""")
-        for file in directory.iterdir():
-            logging.info(f"""  Working on file "{choosePathToLog(file, rootDirectory)}".""")
-            conditions = [condition(file) for condition in fileConditions]
-            if all(conditions):
-                # Set file options
-                exportPath = runOutputDir.joinpath(file.name)
-                fileMode = "w"
-                fileHeaders = True
-                # Read file
-                logging.info("""    File has met all conditions for processing.""")
-                logging.info("""  ..  Reading file to count the number of chunks.""")
-                numChunks = sum([1 for _ in readDataFile(file, chunksize=CHUNK_SIZE, low_memory=False)])
-                logging.info(f"""  ..  This file has {numChunks:,} chunks.""")
-                # Calculate logging requency
-                if numChunks < MESSAGE_MODULO_CHUNKS:
-                    moduloChunks = numChunks
-                else:
-                    moduloChunks = round(numChunks / MESSAGE_MODULO_CHUNKS)
-                if numChunks / moduloChunks < 100:
-                    moduloChunks = 1
-                else:
-                    pass
-                dfChunks = readDataFile(file, chunksize=CHUNK_SIZE, low_memory=False)
-                filePreview = readDataFile(file, nrows=2)
-                filePreview = pd.DataFrame(filePreview)
-                nasumDict = {columnName: {"nasumRows": 0,
-                                          "nasumValues": 0,
-                                          "nasumRowsTotal": 0,
-                                          "nasumValuesTotal": 0} for columnName in filePreview.columns}
-                for it, dfChunk0 in enumerate(dfChunks, start=1):
-                    dfChunk = pd.DataFrame(dfChunk0)
-                    # Work on chunk
-                    if it % moduloChunks == 0:
-                        allowLogging = True
-                    else:
-                        allowLogging = False
-                    if allowLogging:
-                        logging.info(f"""  ..  Working on chunk {it:,} of {numChunks:,}.""")
-                    for columnName in dfChunk.columns:
-                        # Work on column
-                        if allowLogging:
+        logging.info("""Getting the set of values for each variable to de-identify.""")
+        columnSetsVarsDi = {columnName: {"fpath": runIntermediateDataDir.joinpath(f"{VARIABLE_NAME_TO_FILE_NAME_DICT[columnName]}.txt"),
+                                         "fileMode": "w",
+                                         "portionName": None,
+                                         "collected": False} for columnName in COLUMNS_TO_DE_IDENTIFY}
+        for portionName, (directory, fileConditions) in portionPathsAndConditions.items():
+            # Act on directory
+            logging.info(f"""Working on directory "{directory.absolute().relative_to(rootDirectory)}".""")
+            for file in directory.iterdir():
+                logging.info(f"""  Working on file "{file.absolute().relative_to(rootDirectory)}".""")
+                conditions = [condition(file) for condition in fileConditions]
+                if all(conditions):
+                    # Read file
+                    logging.info("""    File has met all conditions for processing.""")
+                    numChunks = sum([1 for _ in readDataFile(file, chunkSize=CHUNK_SIZE)])
+                    dfChunks = readDataFile(file, chunkSize=CHUNK_SIZE)
+                    for it, dfChunk in enumerate(dfChunks, start=1):
+                        dfChunk = pd.DataFrame(dfChunk)
+                        logging.info(f"""  ..  Working on chunk {it} of {numChunks}.""")
+                        for columnName in dfChunk.columns:
                             logging.info(f"""  ..    Working on column "{columnName}".""")
-                        if columnName in columnsToConvert:
-                            if allowLogging:
-                                logging.info("""  ..  ..  Column must be converted. Converting column...""")
-                            # Get position of (old) column
-                            oldColumnPosition = dfChunk.columns.get_loc(columnName)
-                            # Build map for chunk
-                            databasePath = MAPS[columnName]["mapPath"]
-                            toVariable = MAPS[columnName]["to"]
-                            tableName = f"{columnName} to {toVariable}"
-                            with sqlite3.connect(database=databasePath) as connection:
-                                cursor = connection.cursor()
-                                uniqueValues = dfChunk[columnName].dropna().drop_duplicates()
-                                queryFilterArgument = ",".join(uniqueValues.astype(str).to_list())
-                                query = f"""SELECT
-                                                A.'{columnName}'
-                                                ,A.'{toVariable}'
-                                            FROM
-                                                '{tableName}' AS A
-                                            WHERE
-                                                A.'{columnName}' in ({queryFilterArgument})
-                                         """
-                                cursor.execute(query)
-                                sqliteResult = cursor.fetchall()
-                                chunkMapColumnNames = [columnName, toVariable]
-                                chunkMap = pd.DataFrame(sqliteResult, columns=chunkMapColumnNames)
-                            # Add new column
-                            dfChunk = dfChunk.join(other=chunkMap.set_index(columnName),
-                                                   on=columnName,
-                                                   how="outer",
-                                                   lsuffix="",
-                                                   rsuffix="_R")
-                            # Remove old column and extra column
-                            _ = dfChunk.pop(columnName)
-                            # Move new column to old column position
-                            newColumnName = mapsColumnNames[columnName]
-                            _ = dfChunk.insert(loc=oldColumnPosition,
-                                               column=newColumnName,
-                                               value=dfChunk.pop(newColumnName))
-                            # QA: Count un-mapped rows and values. Update total count for file
-                            columnSeries = pd.Series(dfChunk[newColumnName])
-                            nasumRows = columnSeries.isna().sum()
-                            nasumValues = len(uniqueValues) - uniqueValues.isin(chunkMap[columnName]).sum()
-                            nasumDict[columnName]["nasumRows"] = nasumRows
-                            nasumDict[columnName]["nasumValues"] = nasumValues
-                            nasumDict[columnName]["nasumRowsTotal"] += nasumRows
-                            nasumDict[columnName]["nasumValuesTotal"] += nasumValues
-                            if nasumValues > 0:
-                                logging.warning(f"""  ..  WARNING: there were {nasumRows:,} missing ID values (NaNs) for "{columnName}". This might be an indication of failure to map values. The number is not a count of unique values.""")
-                            if nasumValues > 0:
-                                logging.warning(f"""  ..  WARNING: There were {nasumValues:,} missing unique ID values (NaNs) for "{columnName}". This might be an indication of failure to map values.""")
-                    # Save chunk
-                    dfChunk.to_csv(exportPath, mode=fileMode, header=fileHeaders, index=False)
-                    fileMode = "a"
-                    fileHeaders = False
-                    if allowLogging:
-                        logging.info(f"""  ..  Chunk saved to "{choosePathToLog(exportPath, rootDirectory)}".""")
-                nasumRowsTotal = nasumDict[columnName]["nasumRowsTotal"]
-                nasumValuesTotal = nasumDict[columnName]["nasumValuesTotal"]
-                nasumdf = pd.DataFrame.from_dict(data=nasumDict)
-                warningText = f"""  ..  WARNING: Below are the missing value summaries. Missing values are NaNs. Missing values may be an indication of failure to map values (as in the case of IDs).\n{nasumdf.to_string()}"""
-                logging.warning(warningText)
-            else:
-                logging.info("""    This file does not need to be processed.""")
+                            if columnName in COLUMNS_TO_DE_IDENTIFY:
+                                logging.info("""  ..  ..  Column must be de-identified. Collecting values.""")
+                                dataType = DATA_TYPES_DICT[columnName]
+                                series = dfChunk[columnName]
+                                series = series.dropna()
+                                series = series.drop_duplicates()
+                                if dataType == "Datetime":
+                                    values = series.sort_values()
+                                    quoting = csv.QUOTE_NONE
+                                elif dataType == "Numeric":
+                                    series = series.astype(float).astype("Int64")
+                                    values = series.sort_values()
+                                    quoting = csv.QUOTE_NONE
+                                elif dataType == "String":
+                                    values = series.astype(str).sort_values()
+                                    quoting = csv.QUOTE_ALL
+                                elif dataType == "Numeric_Or_String":
+                                    mask = series.apply(lambda el: isinstance(el, float))
+                                    series.loc[mask[mask].index] = series[mask].astype(int)
+                                    values = sortIntegersAndStrings(series.to_list())
+                                    values = pd.Series(values)
+                                    quoting = csv.QUOTE_ALL
+                                else:
+                                    raise Exception(f"""Unexpected `dataType` value: "{dataType}".""")
+                                columnSetFpath = columnSetsVarsDi[columnName]["fpath"]
+                                columnSetFileMode = columnSetsVarsDi[columnName]["fileMode"]
+                                # logging.info(f"""  ..  ..  Values table preview:\n{values.head()}.""")
+                                values.to_csv(path_or_buf=columnSetFpath,
+                                              quoting=quoting,
+                                              index=False,
+                                              header=False,
+                                              mode=columnSetFileMode)
+                                # logging.info(f"""  ..  ..  Preview of table after saving:\n{pd.read_table(columnSetFpath)}.""")
+                                columnSetsVarsDi[columnName]["fileMode"] = "a"
+                                columnSetsVarsDi[columnName]["portionName"] = portionName
+                                columnSetsVarsDi[columnName]["collected"] = True
+                                logging.info(f"""  ..  ..  Values saved to "{columnSetFpath.absolute().relative_to(rootDirectory)}" in the project directory.""")
+                else:
+                    logging.info("""    This file does not need to be processed.""")
 
-    # Output location summary
-    logging.info(f"""Script output is located in the following directory: "{choosePathToLog(runOutputDir, rootDirectory)}".""")
+        columnSetsVarsDiPath = runIntermediateDataDir.joinpath("Metadata", columnSetsVarsDiFname)
+        makeDirPath(columnSetsVarsDiPath.parent)
+        columnSetsVarsDiSerializable = columnSetsVarsDi.copy()
+        for columnName, di in columnSetsVarsDiSerializable.items():
+            columnSetsVarsDiSerializable[columnName]["fpath"] = str(di["fpath"])
+        with open(columnSetsVarsDiPath, "w") as file:
+            file.write(json.dumps(columnSetsVarsDi))
+
+    # Drop variables that weren't found
+    for columnName in COLUMNS_TO_DE_IDENTIFY:
+        if columnName in columnSetsVarsDi.keys():
+            if columnSetsVarsDi[columnName]["collected"] is False:
+                columnSetsVarsDi.pop(columnName)
+
+    # Remove duplicates from set files and save according to data type
+    logging.info("Removing duplicates from set files and saving according to data type.")
+    columnSetsVarsLi = sorted(list(columnSetsVarsDi.items()), key=lambda tu: tu[0].lower())
+    for columnName, fileDi in columnSetsVarsLi:
+        logging.info(f"""  Working on variable "{columnName}".""")
+        fpath = fileDi["fpath"]
+        try:
+            series = pd.read_table(fpath, header=None)[0]
+        except EmptyDataError as err:
+            _ = err
+            series = pd.Series(dtype=str)
+        # Save according to data type
+        portionName = fileDi["portionName"]
+        dataType = DATA_TYPES_DICT[columnName]
+        if dataType == "Datetime":
+            quoting = csv.QUOTE_MINIMAL
+        elif dataType == "Numeric":
+            series = series.astype(float).astype("Int64")
+            quoting = csv.QUOTE_MINIMAL
+        elif dataType == "String":
+            quoting = csv.QUOTE_ALL
+        elif dataType == "Numeric_Or_String":
+            quoting = csv.QUOTE_ALL
+        else:
+            raise Exception(f"""Unexpected `dataType` value: "{dataType}".""")
+        series = series.drop_duplicates()
+        series = series.sort_values()
+        fpath2 = runOutputDir.joinpath("Set Files", f"{VARIABLE_NAME_TO_FILE_NAME_DICT[columnName]}.txt")
+        makeDirPath(fpath2.parent)
+        series.to_csv(fpath2, quoting=quoting, index=False, header=False)
+
+    # Return path to sets fo ID values
+    # TODO If this is implemented as a function, instead of a stand-alone script, return `runOutputDir` to define `setsPathDir` in the "makeMap" scripts.
+    logging.info(f"""Finished collecting the set of ID values to de-identify. The set files are located in "{runOutputDir.absolute().relative_to(rootDirectory)}".""")
 
     # End script
     logging.info(f"""Finished running "{thisFilePath.absolute().relative_to(rootDirectory)}".""")
```

### Comparing `drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/dataQualityTest.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/dataQualityTest.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,15 @@
             conditions = [condition(file) for condition in fileConditions]
             if all(conditions):
                 # Read file
                 logging.info("""    This file has met all conditions for testing.""")
                 # Test 1: Make sure all lines have the same number of delimiters
                 logging.info("""  ..  Test 1: Make sure all lines have the same number of delimiters.""")
                 try:
-                    numChunks = sum([1 for _ in readDataFile(file, chunksize=CHUNK_SIZE)])
+                    numChunks = sum([1 for _ in readDataFile(file, chunkSize=CHUNK_SIZE)])
                     logging.info("""  ..    There are no apparent problems reading this file.""")
                 except ParserError as err:
                     args = err
                     logging.info("""  ..    This file raised an error: "{err}".""")
                 # Test 2: ...
                 pass
             else:
```

### Comparing `drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/deIdentify.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/deIdentify.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 De-identify files
 
 # NOTE Does not expect data in nested directories (e.g., subfolders of "free_text"). Therefore it uses "Path.iterdir" instead of "Path.glob('*/**')".
+# NOTE Expects all files to be CSV files. This is because it uses "pd.read_csv".
 # TODO Assign portion name to each path (per OS) so that portion files are stored in their respective folders, this prevents file from being overwritten in the unlikely, but possible, case files from different portions have the same name.
 """
 
 import logging
 import sys
 from pathlib import Path
 # Third-party packages
@@ -15,15 +16,15 @@
                                     getTimestamp,
                                     makeDirPath,
                                     makeMap,
                                     map2di,
                                     numericOrString2integerOrString,
                                     readDataFile,
                                     successiveParents)
-from drapi.code.drapi.constants.phiVariables import (FILE_NAME_TO_VARIABLE_NAME_DICT,
+from drapi.constants.phiVariables import (FILE_NAME_TO_VARIABLE_NAME_DICT,
                                           VARIABLE_NAME_TO_FILE_NAME_DICT)
 # Local packages: Script parameters: General
 from common import (IRB_NUMBER,
                     ALIAS_DATA_TYPES,
                     COLUMNS_TO_DE_IDENTIFY,
                     DATA_REQUEST_ROOT_DIRECTORY_DEPTH,
                     DATA_TYPES_DICT,
@@ -200,17 +201,17 @@
                 # Set file options
                 exportPath = runOutputDir.joinpath(file.name)
                 fileMode = "w"
                 fileHeaders = True
                 # Read file
                 logging.info("""    File has met all conditions for processing.""")
                 logging.info("""  ..  Reading file to count the number of chunks.""")
-                numChunks = sum([1 for _ in readDataFile(file, chunksize=CHUNK_SIZE)])
+                numChunks = sum([1 for _ in readDataFile(file, chunkSize=CHUNK_SIZE)])
                 logging.info(f"""  ..  This file has {numChunks} chunks.""")
-                dfChunks = readDataFile(file, chunksize=CHUNK_SIZE)
+                dfChunks = readDataFile(file, chunkSize=CHUNK_SIZE)
                 for it, dfChunk in enumerate(dfChunks, start=1):
                     dfChunk = pd.DataFrame(dfChunk)
                     # Work on chunk
                     logging.info(f"""  ..  Working on chunk {it} of {numChunks}.""")
                     for columnName in dfChunk.columns:
                         # Work on column
                         logging.info(f"""  ..    Working on column "{columnName}".""")
```

### Comparing `drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/deIdentifyByAge.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/deIdentifyByAge.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Third-party packages
 import pandas as pd
 # Local packages
 from drapi.code.drapi.drapi import (getTimestamp,
                                     makeDirPath,
                                     successiveParents)
 # Local packages: Script parameters: General
-from drapi.code.drapi.constants.phiVariables import (DICT_OF_PHI_VARIABLES_AGE,
+from drapi.constants.phiVariables import (DICT_OF_PHI_VARIABLES_AGE,
                                           DICT_OF_PHI_VARIABLES_BIRTHDATES)
 # Local packages: Script parameters: Paths
 # Local packages: Script parameters: File criteria
 from common import BO_PORTION_FILE_CRITERIA
 
 # Arguments
 AGE_MAP = Path(r"..\Concatenated Results\data\output\makeAgeMap\2024-01-03 13-20-23\Age Map - De-identified Patient Key.CSV")
```

### Comparing `drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/deIdentifyDates.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/deIdentifyDates.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # Local packages
 from drapi.code.drapi.drapi import (getTimestamp,
                                     makeDirPath,
                                     makeMap,
                                     map2di,
                                     successiveParents)
 # Local packages: Script parameters: General
-from drapi.code.drapi.constants.phiVariables import (LIST_OF_PHI_DATES_BO,
+from drapi.constants.phiVariables import (LIST_OF_PHI_DATES_BO,
                                           LIST_OF_PHI_DATES_NOTES,
                                           LIST_OF_PHI_DATES_OMOP)
 # Local packages: Script parameters: General
 from common import IRB_NUMBER
 # Local packages: Script parameters: Paths
 # Local packages: Script parameters: File criteria
 from common import BO_PORTION_FILE_CRITERIA
```

### Comparing `drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/deleteByColumnValues.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/makePersonIDMap.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,94 +1,87 @@
 """
-Deletes rows based on column values.
+Convert OMOP person IDs to IDR patient keys.
+
+# NOTE Does not expect data in nested directories (e.g., subfolders of "free_text"). Therefore it uses "Path.iterdir" instead of "Path.glob('*/**')".
+# NOTE Expects all files to be CSV files. This is because it uses "pd.read_csv".
 """
 
 import logging
-import os
 import sys
 from pathlib import Path
 # Third-party packages
 import pandas as pd
+from pandas.errors import EmptyDataError
 # Local packages
 from drapi.code.drapi.drapi import (getTimestamp,
                                     makeDirPath,
+                                    personIDs2patientKeys,
+                                    readDataFile,
                                     successiveParents)
-# Local packages: Script parameters: General
-from drapi.code.drapi.constants.phiValues import PHI_VALUES_DICT_ALL
-# Local packages: Script parameters: General
-# Local packages: Script parameters: Paths
-# Local packages: Script parameters: File criteria
-from common import BO_PORTION_FILE_CRITERIA
+from common import (DATA_REQUEST_ROOT_DIRECTORY_DEPTH,
+                    OMOP_PORTION_DIR_MAC,
+                    OMOP_PORTION_DIR_WIN,
+                    OMOP_PORTION_FILE_CRITERIA)
 
 # Arguments
-COLUMN_VALUES_TO_DROP = PHI_VALUES_DICT_ALL
+COLUMNS_TO_CONVERT = ["person_id"]
 
-# Arguments: OMOP data set selection
-USE_MODIFIED_OMOP_DATA_SET = True
+MAC_PATHS = [OMOP_PORTION_DIR_MAC]
+WIN_PATHS = [OMOP_PORTION_DIR_WIN]
 
-# Arguments: Portion Paths and conditions
-MAC_PATHS = [Path(r"..\Concatenated Results\data\output\deIdentifyByAge\...")]
-WIN_PATHS = [Path(r"..\Concatenated Results\data\output\deIdentifyByAge\...")]
+LIST_OF_PORTION_CONDITIONS = [OMOP_PORTION_FILE_CRITERIA]
 
-LIST_OF_PORTION_CONDITIONS = [BO_PORTION_FILE_CRITERIA]
+SETS_PATH = None
 
-# Arguments; General
 CHUNK_SIZE = 50000
 
 # Arguments: Meta-variables
-PROJECT_DIR_DEPTH = 2
-DATA_REQUEST_DIR_DEPTH = PROJECT_DIR_DEPTH + 2
-IRB_DIR_DEPTH = DATA_REQUEST_DIR_DEPTH + 0
+CONCATENATED_RESULTS_DIRECTORY_DEPTH = DATA_REQUEST_ROOT_DIRECTORY_DEPTH - 1
+PROJECT_DIR_DEPTH = CONCATENATED_RESULTS_DIRECTORY_DEPTH  # The concatenation suite of scripts is considered to be the "project".
+IRB_DIR_DEPTH = CONCATENATED_RESULTS_DIRECTORY_DEPTH + 2
 IDR_DATA_REQUEST_DIR_DEPTH = IRB_DIR_DEPTH + 3
 
-ROOT_DIRECTORY = "IRB_DIRECTORY"  # TODO One of the following:
-                                                 # ["IDR_DATA_REQUEST_DIRECTORY",    # noqa
-                                                 #  "IRB_DIRECTORY",                 # noqa
-                                                 #  "DATA_REQUEST_DIRECTORY",        # noqa
-                                                 #  "PROJECT_OR_PORTION_DIRECTORY"]  # noqa
+ROOT_DIRECTORY = "DATA_REQUEST_DIRECTORY"  # TODO One of the following:
+                                           # ["IDR_DATA_REQUEST_DIRECTORY",      # noqa
+                                           #  "IRB_DIRECTORY",                   # noqa
+                                           #  "DATA_REQUEST_DIRECTORY",          # noqa
+                                           #  "CONCATENATED_RESULTS_DIRECTORY"]  # noqa
 
 LOG_LEVEL = "INFO"
 
-# Arguments: SQL connection settings
-SERVER = "DWSRSRCH01.shands.ufl.edu"
-DATABASE = "DWS_PROD"
-USERDOMAIN = "UFAD"
-USERNAME = os.environ["USER"]
-UID = None
-PWD = os.environ["HFA_UFADPWD"]
-
 # Variables: Path construction: General
 runTimestamp = getTimestamp()
 thisFilePath = Path(__file__)
 thisFileStem = thisFilePath.stem
 projectDir, _ = successiveParents(thisFilePath.absolute(), PROJECT_DIR_DEPTH)
-dataRequestDir, _ = successiveParents(thisFilePath.absolute(), DATA_REQUEST_DIR_DEPTH)
-IRBDir, _ = successiveParents(thisFilePath, IRB_DIR_DEPTH)
+dataRequestDir, _ = successiveParents(thisFilePath.absolute(), DATA_REQUEST_ROOT_DIRECTORY_DEPTH)
+IRBDir, _ = successiveParents(thisFilePath.absolute(), IRB_DIR_DEPTH)
 IDRDataRequestDir, _ = successiveParents(thisFilePath.absolute(), IDR_DATA_REQUEST_DIR_DEPTH)
 dataDir = projectDir.joinpath("data")
 if dataDir:
     inputDataDir = dataDir.joinpath("input")
+    intermediateDataDir = dataDir.joinpath("intermediate")
     outputDataDir = dataDir.joinpath("output")
+    if intermediateDataDir:
+        runIntermediateDataDir = intermediateDataDir.joinpath(thisFileStem, runTimestamp)
     if outputDataDir:
         runOutputDir = outputDataDir.joinpath(thisFileStem, runTimestamp)
 logsDir = projectDir.joinpath("logs")
 if logsDir:
     runLogsDir = logsDir.joinpath(thisFileStem)
 sqlDir = projectDir.joinpath("sql")
 
-if ROOT_DIRECTORY == "PROJECT_OR_PORTION_DIRECTORY":
+if ROOT_DIRECTORY == "CONCATENATED_RESULTS_DIRECTORY":
     rootDirectory = projectDir
 elif ROOT_DIRECTORY == "DATA_REQUEST_DIRECTORY":
     rootDirectory = dataRequestDir
 elif ROOT_DIRECTORY == "IRB_DIRECTORY":
     rootDirectory = IRBDir
 elif ROOT_DIRECTORY == "IDR_DATA_REQUEST_DIRECTORY":
     rootDirectory = IDRDataRequestDir
-else:
-    raise Exception("An unexpected error occurred.")
 
 # Variables: Path construction: OS-specific
 isAccessible = all([path.exists() for path in MAC_PATHS]) or all([path.exists() for path in WIN_PATHS])
 if isAccessible:
     # If you have access to either of the below directories, use this block.
     operatingSystem = sys.platform
     if operatingSystem == "darwin":
@@ -98,111 +91,107 @@
     else:
         raise Exception("Unsupported operating system")
 else:
     # If the above option doesn't work, manually copy the database to the `input` directory.
     print("Not implemented. Check settings in your script.")
     sys.exit()
 
-# Variables: Path construction: Project-specific
-pass
-
-# Variables: SQL Parameters
-if UID:
-    uid = UID[:]
-else:
-    uid = fr"{USERDOMAIN}\{USERNAME}"
-conStr = f"mssql+pymssql://{uid}:{PWD}@{SERVER}/{DATABASE}"
-
-# Variables: Other
-pass
-
 # Directory creation: General
+makeDirPath(runIntermediateDataDir)
 makeDirPath(runOutputDir)
 makeDirPath(runLogsDir)
 
-# Logging block
-logpath = runLogsDir.joinpath(f"log {runTimestamp}.log")
-logFormat = logging.Formatter("""[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s""")
-
-logger = logging.getLogger(__name__)
-
-fileHandler = logging.FileHandler(logpath)
-fileHandler.setLevel(9)
-fileHandler.setFormatter(logFormat)
-
-streamHandler = logging.StreamHandler()
-streamHandler.setLevel(LOG_LEVEL)
-streamHandler.setFormatter(logFormat)
-
-logger.addHandler(fileHandler)
-logger.addHandler(streamHandler)
-
-logger.setLevel(9)
-
 if __name__ == "__main__":
-    logger.info(f"""Begin running "{thisFilePath}".""")
-    logger.info(f"""All other paths will be reported in debugging relative to `{ROOT_DIRECTORY}`: "{rootDirectory}".""")
-    logger.info(f"""Script arguments:
-
-
-    # Arguments
-    `COLUMN_VALUES_TO_DROP`: "{COLUMN_VALUES_TO_DROP}"
-    `USE_MODIFIED_OMOP_DATA_SET`: "{USE_MODIFIED_OMOP_DATA_SET}"
-    `MAC_PATHS`: "{MAC_PATHS}"
-    `WIN_PATHS`: "{WIN_PATHS}"
-
-    # Arguments: General
-    `PROJECT_DIR_DEPTH`: "{PROJECT_DIR_DEPTH}" ----------> "{projectDir}"
-    `IRB_DIR_DEPTH`: "{IRB_DIR_DEPTH}" --------------> "{IRBDir}"
-    `IDR_DATA_REQUEST_DIR_DEPTH`: "{IDR_DATA_REQUEST_DIR_DEPTH}" -> "{IDRDataRequestDir}"
-
-    `LOG_LEVEL` = "{LOG_LEVEL}"
-
-    # Arguments: SQL connection settings
-    `SERVER` = "{SERVER}"
-    `DATABASE` = "{DATABASE}"
-    `USERDOMAIN` = "{USERDOMAIN}"
-    `USERNAME` = "{USERNAME}"
-    `UID` = "{UID}"
-    `PWD` = censored
-    """)
-
-    logger.info("""De-identifying files.""")
-    for directory, fileConditions in zip(listOfPortionDirs, LIST_OF_PORTION_CONDITIONS):
-        # Act on directory
-        logger.info(f"""Working on directory "{directory.absolute().relative_to(rootDirectory)}".""")
-        for file in directory.iterdir():
-            logger.info(f"""  Working on file "{file.absolute().relative_to(rootDirectory)}".""")
-            conditions = [condition(file) for condition in fileConditions]
-            if all(conditions):
-                # Set file options
-                exportPath = runOutputDir.joinpath(file.name)
-                fileMode = "w"
-                fileHeaders = True
-                # Read file
-                logger.info("""    File has met all conditions for processing.""")
-                logger.info("""  ..  Reading file to count the number of chunks.""")
-                numChunks = sum([1 for _ in pd.read_csv(file, chunksize=CHUNK_SIZE)])
-                logger.info(f"""  ..  This file has {numChunks} chunks.""")
-                dfChunks = pd.read_csv(file, chunksize=CHUNK_SIZE)
-                for it, dfChunk in enumerate(dfChunks, start=1):
-                    dfChunk = pd.DataFrame(dfChunk)
-                    # Work on chunk
-                    logger.info(f"""  ..  Working on chunk {it} of {numChunks}.""")
-                    for columnName in dfChunk.columns:
-                        # Work on column
-                        logger.info(f"""  ..    Working on column "{columnName}".""")
-                        if columnName in COLUMN_VALUES_TO_DROP.keys():
-                            mask = ~dfChunk[columnName].isin(COLUMN_VALUES_TO_DROP[columnName])
-                            if mask.sum() > 0:
-                                logger.info("""  ..  ..  Column has values that need to be dropped. Dropping values.""")
-                            dfChunk = dfChunk[mask]
-                    # Save chunk
-                    dfChunk.to_csv(exportPath, mode=fileMode, header=fileHeaders, index=False)
-                    fileMode = "a"
-                    fileHeaders = False
-                    logger.info(f"""  ..  Chunk saved to "{exportPath.absolute().relative_to(rootDirectory)}".""")
-            else:
-                logger.info("""    This file does not need to be processed.""")
+    # Logging block
+    logpath = runLogsDir.joinpath(f"log {runTimestamp}.log")
+    fileHandler = logging.FileHandler(logpath)
+    fileHandler.setLevel(LOG_LEVEL)
+    streamHandler = logging.StreamHandler()
+    streamHandler.setLevel(LOG_LEVEL)
+
+    logging.basicConfig(format="[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s",
+                        handlers=[fileHandler, streamHandler],
+                        level=LOG_LEVEL)
+
+    logging.info(f"""Begin running "{thisFilePath}".""")
+    logging.info(f"""All other paths will be reported in debugging relative to `IRBDir`: "{IRBDir}".""")
+
+    # Get set of values
+    if SETS_PATH:
+        logging.info(f"""Using the set of values previously collected from "{SETS_PATH}".""")
+    else:
+        logging.info("""Getting the set of values for each variable to convert.""")
+        columnSetsVarsDi = {columnName: {"fpath": runIntermediateDataDir.joinpath(f"{columnName}.txt"),
+                                         "fileMode": "w"} for columnName in COLUMNS_TO_CONVERT}
+        for directory, fileConditions in zip(listOfPortionDirs, LIST_OF_PORTION_CONDITIONS):
+            # Act on directory
+            logging.info(f"""Working on directory "{directory.relative_to(IRBDir)}".""")
+            for file in directory.iterdir():
+                logging.info(f"""  Working on file "{file.absolute().relative_to(IRBDir)}".""")
+                conditions = [condition(file) for condition in fileConditions]
+                if all(conditions):
+                    # Read file
+                    logging.info("""    File has met all conditions for processing.""")
+                    numChunks = sum([1 for _ in readDataFile(file, chunkSize=CHUNK_SIZE)])
+                    dfChunks = readDataFile(file, chunkSize=CHUNK_SIZE)
+                    for it, dfChunk in enumerate(dfChunks, start=1):
+                        logging.info(f"""  ..  Working on chunk {it} of {numChunks}.""")
+                        for columnName in dfChunk.columns:
+                            logging.info(f"""  ..    Working on column "{columnName}".""")
+                            if columnName in COLUMNS_TO_CONVERT:
+                                logging.info("""  ..  ..  Column must be converted. Collecting values.""")
+                                valuesSet = sorted(list(set(dfChunk[columnName].dropna().values)))
+                                columnSetFpath = columnSetsVarsDi[columnName]["fpath"]
+                                columnSetFileMode = columnSetsVarsDi[columnName]["fileMode"]
+                                with open(columnSetFpath, columnSetFileMode) as file:
+                                    for value in valuesSet:
+                                        file.write(str(value))
+                                        file.write("\n")
+                                columnSetsVarsDi[columnName]["fileMode"] = "a"
+                                logging.info(f"""  ..  ..  Values saved to "{columnSetFpath.absolute().relative_to(IRBDir)}" in the project directory.""")
+                else:
+                    logging.info("""    This file does not need to be processed.""")
+
+    # Map values
+    if SETS_PATH:
+        setsPathDir = SETS_PATH
+    else:
+        setsPathDir = runIntermediateDataDir
+    for file in setsPathDir.iterdir():
+        columnName = file.stem
+        logging.info(f"""  Working on variable "{columnName}" located at "{file.absolute().relative_to(IRBDir)}".""")
+        # Read file
+        try:
+            df = pd.read_table(file, header=None)
+        except EmptyDataError as err:
+            _ = err
+            df = pd.DataFrame()
+        # Assert
+        if df.shape[1] == 1:
+            # Try to convert to integer-type
+            try:
+                df.iloc[:, 0] = df.iloc[:, 0].astype(int)
+            except ValueError as err:
+                _ = err
+            # Check length differences
+            len0 = len(df)
+            values = set(df.iloc[:, 0].values)
+            len1 = len(values)
+            logging.info(f"""    The length of the ID array was reduced from {len0:,} to {len1:,} when removing duplicates.""")
+        elif df.shape[1] == 0:
+            pass
+        # Map contents
+        map_ = personIDs2patientKeys(list(values))
+        # Save map
+        mapPath = runOutputDir.joinpath(f"{columnName} map.csv")
+        map_.to_csv(mapPath, index=False)
+        logging.info(f"""    PersonID-to-PatientKey map saved to "{mapPath.absolute().relative_to(IRBDir)}".""")
+
+    # Clean up
+    # TODO If input directory is empty, delete
+    # TODO Delete intermediate run directory
+
+    # Output location summary
+    logging.info(f"""Script output is located in the following directory: "{runOutputDir.absolute().relative_to(IRBDir)}".""")
 
     # End script
-    logger.info(f"""Finished running "{thisFilePath.relative_to(projectDir)}".""")
+    logging.info(f"""Finished running "{thisFilePath.absolute().relative_to(IRBDir)}".""")
```

### Comparing `drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/deleteColumns.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/deleteColumns.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 De-identify files
 
 # NOTE Does not expect data in nested directories (e.g., subfolders of "free_text"). Therefore it uses "Path.iterdir" instead of "Path.glob('*/**')".
+# NOTE Expects all files to be CSV files. This is because it uses "pd.read_csv".
 # TODO Assign portion name to each path (per OS) so that portion files are stored in their respective folders, this prevents file from being overwritten in the unlikely, but possible, case files from different portions have the same name.
 # TODO Investigate if a symlink can be made for files that are copied without alteration, to save space and time on larger projects.
 """
 
 import logging
 import sys
 from pathlib import Path
@@ -13,33 +14,35 @@
 import pandas as pd
 # Local packages
 from drapi.code.drapi.drapi import (flatExtend,
                                     getTimestamp,
                                     makeDirPath,
                                     readDataFile,
                                     successiveParents)
-from drapi.code.drapi.constants.phiVariables import (LIST_OF_PHI_VARIABLES_OMOP_UNINFORMATIVE,
+from drapi.constants.phiVariables import (LIST_OF_PHI_VARIABLES_OMOP_UNINFORMATIVE,
                                           LIST_OF_PHI_VARIABLES_OMOP_BIRTHDATE_CONDITIONAL)
 # Project parameters: General
-from .common import (STUDY_TYPE,
-                     DATA_REQUEST_ROOT_DIRECTORY_DEPTH)
+from common import (STUDY_TYPE,
+                    DATA_REQUEST_ROOT_DIRECTORY_DEPTH)
 # Project parameters: Portion paths and criteria
-from .common import (MODIFIED_OMOP_PORTION_DIR_MAC, MODIFIED_OMOP_PORTION_DIR_WIN,
-                     CLINICAL_TEXT_PORTION_DIR_MAC, CLINICAL_TEXT_PORTION_DIR_WIN,
-                     OMOP_PORTION_DIR_MAC, OMOP_PORTION_DIR_WIN)
+from common import (BO_PORTION_DIR_MAC, BO_PORTION_DIR_WIN,
+                    I2B2_PORTION_DIR_MAC, I2B2_PORTION_DIR_WIN,
+                    MODIFIED_OMOP_PORTION_DIR_MAC, MODIFIED_OMOP_PORTION_DIR_WIN,
+                    NOTES_PORTION_DIR_MAC, NOTES_PORTION_DIR_WIN,
+                    OMOP_PORTION_DIR_MAC, OMOP_PORTION_DIR_WIN)
 
 # Arguments: Use concatenated files
 USE_CONCATENATED_FILES = True  # TODO
 
 # Arguments: OMOP data set selection
 USE_MODIFIED_OMOP_DATA_SET = True
 
 # Arguments: File location definition: By concatenation
-CONCATENATED_PORTIONS_DIR_MAC = Path("../../Concatenated Results/data/output/convertColumnsHash/.../Portions/OMOP")  # TODO
-CONCATENATED_PORTIONS_DIR_WIN = Path("../../Concatenated Results/data/output/convertColumnsHash/.../Portions/OMOP")  # TODO
+CONCATENATED_PORTIONS_DIR_MAC = Path(r"..\Concatenated Results\data\output\deleteByColumnValues\...")  # TODO
+CONCATENATED_PORTIONS_DIR_WIN = Path(r"..\Concatenated Results\data\output\deleteByColumnValues\...")  # TODO
 
 # Arguments: Portion Paths and conditions
 if USE_MODIFIED_OMOP_DATA_SET:
     OMOPPortionDirMac = MODIFIED_OMOP_PORTION_DIR_MAC
     OMOPPortionDirWin = MODIFIED_OMOP_PORTION_DIR_WIN
 else:
     OMOPPortionDirMac = OMOP_PORTION_DIR_MAC
@@ -48,18 +51,22 @@
 # Arguments: File location definition: OS-specific
 # There are two typical workflows. Deleting columns in the beginning of the workflow, or towards the end, after it's been de-identified (i.e., "concatenated")
 
 if USE_CONCATENATED_FILES:
     MAC_PATHS = [CONCATENATED_PORTIONS_DIR_MAC]
     WIN_PATHS = [CONCATENATED_PORTIONS_DIR_WIN]
 else:
-    MAC_PATHS = [CLINICAL_TEXT_PORTION_DIR_MAC,
+    MAC_PATHS = [BO_PORTION_DIR_MAC,
+                 I2B2_PORTION_DIR_MAC,
+                 NOTES_PORTION_DIR_MAC,
                  OMOPPortionDirMac]
-    WIN_PATHS = [OMOPPortionDirWin,
-                 CLINICAL_TEXT_PORTION_DIR_WIN]
+    WIN_PATHS = [BO_PORTION_DIR_WIN,
+                 I2B2_PORTION_DIR_WIN,
+                 OMOPPortionDirWin,
+                 NOTES_PORTION_DIR_WIN]
 
 # Arguments: Definition of criteria for file release
 # NOTE (Developer's Note) The files to release and the file criteiria both act as criteria to release. The argument structure here is not very clear and it will take some time to create a generalizeable template. However, it seems that `LIST_OF_PORTION_CONDITIONS` is the only output of this arguments section, i.e., the only require input for the script. Also note that each portion has its own criteria, but they are not used in the template.
 BO_FILES_TO_RELEASE = []  # TODO
 
 NOTES_COHORT_NAME = ""  # TODO
 NOTES_METADATA_FILES_TO_RELEASE = ["provider_metadata.csv",
@@ -77,15 +84,14 @@
                          f"{I2B2_COHORT_NAME}_visit_dimension_GNV.csv",
                          f"{I2B2_COHORT_NAME}_visit_dimension_JAX.csv"]
 
 OMOP_FILES_TO_RELEASE = ["condition_occurrence.csv",
                          "death.csv",
                          "device_exposure.csv",
                          "drug_exposure.csv",
-                         "episode.CSV",
                          "location.csv",
                          "measurement_laboratories.csv",
                          "measurement.csv",
                          "observation_period.csv",
                          "observation.csv",
                          "person.csv",
                          "procedure_occurrence.csv",
@@ -207,16 +213,14 @@
 # Variables: Path construction: OS-specific
 isAccessible = all([path.exists() for path in MAC_PATHS]) or all([path.exists() for path in WIN_PATHS])
 if isAccessible:
     # If you have access to either of the below directories, use this block.
     operatingSystem = sys.platform
     if operatingSystem == "darwin":
         listOfPortionDirs = MAC_PATHS[:]
-    elif operatingSystem == "linux":
-        listOfPortionDirs = MAC_PATHS[:]
     elif operatingSystem == "win32":
         listOfPortionDirs = WIN_PATHS[:]
     else:
         raise Exception("Unsupported operating system")
 else:
     # If the above option doesn't work, manually copy the database to the `input` directory.
     print("Not implemented. Check settings in your script.")
@@ -243,35 +247,31 @@
     logging.info(f"""All other paths will be reported in debugging relative to `{ROOT_DIRECTORY}`: "{rootDirectory}".""")
 
     # De-identify columns
     logging.info("""Deleting columns not authorized for release.""")
     for directory, fileConditions in zip(listOfPortionDirs, LIST_OF_PORTION_CONDITIONS):
         # Act on directory
         logging.info(f"""Working on directory "{directory.absolute().relative_to(rootDirectory)}".""")
-        listOfFiles = sorted(list(directory.iterdir()))
-        for file in listOfFiles:
+        for file in directory.iterdir():
             logging.info(f"""  Working on file "{file.absolute().relative_to(rootDirectory)}".""")
             conditions = [condition(file) for condition in fileConditions]
             logging.info(f"""  Conditions: "{conditions}".""")
             if all(conditions):
                 # Set file options
                 exportPath = runOutputDir.joinpath(file.name)
                 fileMode = "w"
                 fileHeaders = True
                 # Read file
                 logging.info("""    File has met all conditions for processing.""")
-                chunkGenerator1 = readDataFile(file, chunksize=CHUNK_SIZE, low_memory=False)
-                chunkGenerator2 = readDataFile(file, chunksize=CHUNK_SIZE, low_memory=False)
-                logging.info(f"""  ..  Reading file to count the number of chunks.""")
-                it1Total = sum([1 for _ in chunkGenerator1])
-                logging.info(f"""  ..  Reading file to count the number of chunks. There are {it1Total:,} chunks.""")
-                for it1, dfChunk in enumerate(chunkGenerator2, start=1):
+                numChunks = sum([1 for _ in readDataFile(file, chunkSize=CHUNK_SIZE)])
+                dfChunks = readDataFile(file, chunkSize=CHUNK_SIZE)
+                for it, dfChunk in enumerate(dfChunks, start=1):
                     dfChunk = pd.DataFrame(dfChunk)
                     # Work on chunk
-                    logging.info(f"""  ..  Working on chunk {it1:,} of {it1Total:,}.""")
+                    logging.info(f"""  ..  Working on chunk {it} of {numChunks}.""")
                     for columnName in dfChunk.columns:
                         # Work on column
                         logging.info(f"""  ..    Working on column "{columnName}".""")
                         if file.stem in COLUMNS_TO_DELETE_DICT.keys():
                             listOfColumns = COLUMNS_TO_DELETE + COLUMNS_TO_DELETE_DICT[file.stem]
                         else:
                             listOfColumns = COLUMNS_TO_DELETE
```

### Comparing `drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/gatherFiles.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/gatherFiles.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,31 @@
 """
 Copy files to a single destination directory. Optionally this directory can be added to a compressed archive.
 """
 
 import logging
 import os
-import pprint
 import shutil
 import zipfile
 from pathlib import Path
-# First-party packages
+# Local packages
 from drapi.code.drapi.drapi import (getTimestamp,
                                     makeDirPath,
                                     successiveParents)
 
 # Arguments
-LIST_OF_DIRECTORIES = ["../../Concatenated Results/disclosure/Portion Symlinks/Clinical Text",  # Clinical Text
-                       "../../Concatenated Results/disclosure/Portion Symlinks/Clinical Text Metadata",  # Clinical Text Metadata
-                       "../../Concatenated Results/disclosure/Portion Symlinks/OMOP"]  # OMOP
-LIST_OF_DIRECTORIES_NEW_NAMES = ["Clinical Text",
-                                 "Clinical Text Metadata",
-                                 "OMOP"]
+LIST_OF_DIRECTORIES = []
 LIST_OF_FILES = []
-TIMESTAMP = getTimestamp()
-DESTINATION_FOLDER = fr"disclosure/{TIMESTAMP}"
+DESTINATION_FOLDER = fr"..\Concatenated Results\disclosure\{getTimestamp()}"
 
 OVERWRITE_IF_EXISTS_FOLDER = False
 OVERWRITE_IF_EXISTS_FILE = False
 
-CREATE_MERGED_FOLDER = False
 CREATE_COMPRESSED_ARCHIVE = True
-DELETE_FOLDER_AFTER_ARCHIVING = False
+DELETE_FOLDER_AFTER_ARCHIVING = True
 
 # Arguments: Meta-variables
 PROJECT_DIR_DEPTH = 2
 DATA_REQUEST_DIR_DEPTH = PROJECT_DIR_DEPTH + 2
 IRB_DIR_DEPTH = PROJECT_DIR_DEPTH + 1
 IDR_DATA_REQUEST_DIR_DEPTH = PROJECT_DIR_DEPTH + 4
 
@@ -93,14 +85,15 @@
     uid = fr"{USERDOMAIN}\{USERNAME}"
 conStr = f"mssql+pymssql://{uid}:{PWD}@{SERVER}/{DATABASE}"
 
 # Variables: Other
 pass
 
 # Directory creation: General
+makeDirPath(runOutputDir)
 makeDirPath(runLogsDir)
 
 # Logging block
 logpath = runLogsDir.joinpath(f"log {runTimestamp}.log")
 logFormat = logging.Formatter("""[%(asctime)s][%(levelname)s](%(funcName)s): %(message)s""")
 
 logger = logging.getLogger(__name__)
@@ -122,24 +115,19 @@
     logger.info(f"""Begin running "{thisFilePath}".""")
     logger.info(f"""All other paths will be reported in debugging relative to `{ROOT_DIRECTORY}`: "{rootDirectory}".""")
     logger.info(f"""Script arguments:
 
 
     # Arguments
     `LIST_OF_DIRECTORIES`: "{LIST_OF_DIRECTORIES}"
-    `LIST_OF_DIRECTORIES_NEW_NAMES`: "{LIST_OF_DIRECTORIES_NEW_NAMES}"
     `LIST_OF_FILES`: "{LIST_OF_FILES}"
     `DESTINATION_FOLDER`: "{DESTINATION_FOLDER}"
-
     `OVERWRITE_IF_EXISTS_FOLDER`: "{OVERWRITE_IF_EXISTS_FOLDER}"
     `OVERWRITE_IF_EXISTS_FILE`: "{OVERWRITE_IF_EXISTS_FILE}"
 
-    `CREATE_COMPRESSED_ARCHIVE`: "{CREATE_COMPRESSED_ARCHIVE}"
-    `DELETE_FOLDER_AFTER_ARCHIVING`: "{DELETE_FOLDER_AFTER_ARCHIVING}"
-
     # Arguments: General
     `PROJECT_DIR_DEPTH`: "{PROJECT_DIR_DEPTH}" ----------> "{projectDir}"
     `IRB_DIR_DEPTH`: "{IRB_DIR_DEPTH}" --------------> "{IRBDir}"
     `IDR_DATA_REQUEST_DIR_DEPTH`: "{IDR_DATA_REQUEST_DIR_DEPTH}" -> "{IDRDataRequestDir}"
 
     `LOG_LEVEL` = "{LOG_LEVEL}"
 
@@ -149,113 +137,87 @@
     `USERDOMAIN` = "{USERDOMAIN}"
     `USERNAME` = "{USERNAME}"
     `UID` = "{UID}"
     `PWD` = censored
     """)
 
     # Define the destination path
-    destinationRootFolder = Path(DESTINATION_FOLDER)
+    destinationFolder = Path(DESTINATION_FOLDER)
 
     # Copy files and directories
-    if CREATE_MERGED_FOLDER:
-        if destinationRootFolder.exists():
-            logger.warning(f"""WARNING: The destination folder already exists: "{destinationRootFolder.absolute()}".""")
-            if OVERWRITE_IF_EXISTS_FOLDER:
-                logger.info("""  Removing folder contents to make room for new files.""")
-                for fpath in destinationRootFolder.iterdir():
-                    logger.info(f"""    Removing "{fpath.absolute()}".""")
-                    os.remove(fpath)
-                    logger.info(f"""    Removing "{fpath.absolute()}" - done.""")
-            else:
-                msg = "  The destination folder exists and no option was passed to over-write it."
-                logger.fatal(msg)
-                raise Exception(msg)
+    if destinationFolder.exists():
+        logger.warning(f"""WARNING: The destination folder already exists: "{destinationFolder.absolute().relative_to(rootDirectory)}".""")
+        if OVERWRITE_IF_EXISTS_FOLDER:
+            logger.info("""  Removing folder contents to make room for new files.""")
+            for fpath in destinationFolder.iterdir():
+                logger.info(f"""    Removing "{fpath.absolute().relative_to(rootDirectory)}".""")
+                os.remove(fpath)
+                logger.info(f"""    Removing "{fpath.absolute().relative_to(rootDirectory)}" - done.""")
         else:
-            logger.info(f"""Making destination folder: "{destinationRootFolder.absolute()}".""")
-            makeDirPath(destinationRootFolder)
-
-        logger.info("""Working on list of files.""")
-        for fpathString in LIST_OF_FILES:
-            fpath = Path(fpathString)
-            logger.info(f"""  Working on file "{fpath.absolute()}".""")
-            dest = destinationRootFolder.joinpath(fpath.name)
-            logger.info(f"""    Saving to "{dest.absolute()}".""")
-            shutil.copyfile(fpath, dest)
-        logger.info("""Working on list of files - done.""")
-
-        logger.info("""Working on list of directories.""")
-        if LIST_OF_DIRECTORIES_NEW_NAMES:
-            listOfDirectoriesNewNames = LIST_OF_DIRECTORIES_NEW_NAMES[:]
-        else:
-            listOfDirectoriesNewNames = ["" for _ in LIST_OF_DIRECTORIES]
-        directoryPathsAndNames = zip(LIST_OF_DIRECTORIES, listOfDirectoriesNewNames)
-        for directoryString, newDirectoryName in directoryPathsAndNames:
-            directory = Path(directoryString)
-            destinationFolder = destinationRootFolder.joinpath(newDirectoryName)
-            destinationFolder.mkdir()
-            listOfFiles1 = sorted(list(directory.iterdir()))
-            for fpath in listOfFiles1:
-                logger.info(f"""  Working on file "{fpath.absolute()}".""")
-                dest = destinationFolder.joinpath(fpath.name)
-                logger.info(f"""    The destination path is "{dest.absolute()}".""")
-                if dest.exists():
-                    msg = f"""    WARNING: This file already exists: "{dest}"."""
-                    logger.warning(msg)
-                    if OVERWRITE_IF_EXISTS_FILE:
-                        continueOperation = True
-                    else:
-                        continueOperation = False
-                else:
+            msg = "  The destination folder exists and no option was passed to over-write it."
+            logger.fatal(msg)
+            raise Exception(msg)
+    else:
+        logger.info(f"""Making destination folder: "{destinationFolder.absolute().relative_to(rootDirectory)}".""")
+        makeDirPath(destinationFolder)
+
+    logger.info("""Working on list of files.""")
+    for fpathString in LIST_OF_FILES:
+        fpath = Path(fpathString)
+        logger.info(f"""  Working on file "{fpath.absolute().relative_to(rootDirectory)}".""")
+        dest = destinationFolder.joinpath(fpath.name)
+        logger.info(f"""    Saving to "{dest.absolute().relative_to(rootDirectory)}".""")
+        shutil.copyfile(fpath, dest)
+    logger.info("""Working on list of files - done.""")
+
+    logger.info("""Working on list of directories.""")
+    for directoryString in LIST_OF_DIRECTORIES:
+        directory = Path(directoryString)
+        for fpath in directory.iterdir():
+            logger.info(f"""  Working on file "{fpath.absolute().relative_to(rootDirectory)}".""")
+            dest = destinationFolder.joinpath(fpath.name)
+            logger.info(f"""    The destination path is "{dest.absolute().relative_to(rootDirectory)}".""")
+            if dest.exists():
+                msg = f"""    WARNING: This file already exists: "{dest}"."""
+                logger.warning(msg)
+                if OVERWRITE_IF_EXISTS_FILE:
                     continueOperation = True
-                if continueOperation:
-                    logger.info("""    Saving to destination path.""")
-                    shutil.copyfile(fpath, dest)
                 else:
-                    logger.info("""    The file was not saved to the destination path. File over-write is set to `False`.""")
-        logger.info("""Working on list of directories - done.""")
+                    continueOperation = False
+            else:
+                continueOperation = True
+            if continueOperation:
+                logger.info("""    Saving to destination path.""")
+                shutil.copyfile(fpath, dest)
+            else:
+                logger.info("""    The file was not saved to the destination path. File over-write is set to `False`.""")
+    logger.info("""Working on list of directories - done.""")
 
     # Create compressed archive
     if CREATE_COMPRESSED_ARCHIVE:
-        archivePath = destinationRootFolder.with_suffix(".ZIP")
-        logger.info(f"""Creating compressed archive: "{archivePath.absolute()}"".""")
+        archivePath = destinationFolder.with_suffix(".ZIP")
+        logger.info(f"""Creating compressed archive: "{archivePath.absolute().relative_to(rootDirectory)}"".""")
         if archivePath.exists():
             logger.info("""The archive folder already exists and will be removed before writing.""")
             os.remove(archivePath)
         else:
-            destinationRootFolder.mkdir(parents=True)
-
-        # Define list of files to archive, and their paths
-        if LIST_OF_DIRECTORIES_NEW_NAMES:
-            listOfDirectoriesNewNames = LIST_OF_DIRECTORIES_NEW_NAMES[:]
-        else:
-            listOfDirectoriesNewNames = ["" for _ in LIST_OF_DIRECTORIES]
-        directoryPathsAndNames = zip(LIST_OF_DIRECTORIES, listOfDirectoriesNewNames)
-        listOfFiles2All = []
-        for directoryString, newDirectoryName in directoryPathsAndNames:
-            directory = Path(directoryString)
-            listOfFiles2 = sorted(list(directory.iterdir()))
-            for fpath2 in listOfFiles2:
-                dest2 = Path(TIMESTAMP).joinpath(newDirectoryName, fpath2.name)
-                listOfFiles2All.append((fpath2, dest2))
-        
-        logger.info(f"""These are the files paths for the archived items:\n{pprint.pformat(listOfFiles2All)}.""")
+            pass
 
         with zipfile.ZipFile(file=archivePath,
                              mode="a",
                              compression=zipfile.ZIP_DEFLATED) as zipObj:
             logger.info("Adding files to archive.")
-            for fpath2, dest2 in sorted(listOfFiles2All):
-                logger.info(f"""  Working on file "{fpath2.absolute()}".""")
-                logger.info(f"""    This has a destination path of "{dest2}".""")
-                zipObj.write(filename=fpath2, arcname=dest2)
+            for fpath in destinationFolder.iterdir():
+                logger.info(f"""  Working on file "{fpath.absolute().relative_to(rootDirectory)}".""")
+                newPath = fpath.name
+                zipObj.write(filename=fpath, arcname=newPath)
         logger.info("Creating compressed archive - done.")
 
-        if CREATE_MERGED_FOLDER:
-            if DELETE_FOLDER_AFTER_ARCHIVING:
-                logger.info("""Removing intermediate folder.""")
-                shutil.rmtree(destinationRootFolder)
-                logger.info("""Removing intermediate folder - done.""")
-            else:
-                pass
+        if DELETE_FOLDER_AFTER_ARCHIVING:
+            logger.info("""Removing intermediate folder.""")
+            shutil.rmtree(destinationFolder)
+            logger.info("""Removing intermediate folder - done.""")
+        else:
+            pass
 
     # End script
-    logger.info(f"""Finished running "{thisFilePath.absolute()}".""")
+    logger.info(f"""Finished running "{thisFilePath.absolute().relative_to(rootDirectory)}".""")
```

### Comparing `drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/getProjectColumns.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/getProjectColumns.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
                     NOTES_PORTION_DIR_MAC, NOTES_PORTION_DIR_WIN,
                     OMOP_PORTION_DIR_MAC, OMOP_PORTION_DIR_WIN)
 # Project parameters: Criteria
 from common import (BO_PORTION_FILE_CRITERIA,
                     I2B2_PORTION_FILE_CRITERIA,
                     NOTES_PORTION_FILE_CRITERIA,
                     OMOP_PORTION_FILE_CRITERIA)
-from drapi.code.drapi.constants.phiVariables import (LIST_OF_PHI_DATES_BO,
+from drapi.constants.phiVariables import (LIST_OF_PHI_DATES_BO,
                                           LIST_OF_PHI_DATES_NOTES,
                                           LIST_OF_PHI_DATES_OMOP)
 
 # Arguments: OMOP data set selection
 USE_MODIFIED_OMOP_DATA_SET = True
 
 # Arguments: Portion Paths and conditions
@@ -43,23 +43,23 @@
     OMOPPortionDirWin = MODIFIED_OMOP_PORTION_DIR_WIN
 else:
     OMOPPortionDirMac = OMOP_PORTION_DIR_MAC
     OMOPPortionDirWin = OMOP_PORTION_DIR_WIN
 
 PORTIONS_OUTPUT_DIR_PATH_MAC = {"BO": BO_PORTION_DIR_MAC,  # TODO
                                 "i2b2": I2B2_PORTION_DIR_MAC,
-                                "Clinical Text": NOTES_PORTION_DIR_MAC,
+                                "Notes": NOTES_PORTION_DIR_MAC,
                                 "OMOP": OMOP_PORTION_DIR_MAC}
 PORTIONS_OUTPUT_DIR_PATH_WIN = {"BO": BO_PORTION_DIR_WIN,  # TODO
                                 "i2b2": I2B2_PORTION_DIR_WIN,
-                                "Clinical Text": NOTES_PORTION_DIR_WIN,
+                                "Notes": NOTES_PORTION_DIR_WIN,
                                 "OMOP": OMOP_PORTION_DIR_WIN}
 PORTION_FILE_CRITERIA_DICT = {"BO": BO_PORTION_FILE_CRITERIA,
                               "i2b2": I2B2_PORTION_FILE_CRITERIA,
-                              "Clinical Text": NOTES_PORTION_FILE_CRITERIA,
+                              "Notes": NOTES_PORTION_FILE_CRITERIA,
                               "OMOP": OMOP_PORTION_FILE_CRITERIA}
 
 COMPARISON_SET = LIST_OF_PHI_DATES_BO + LIST_OF_PHI_DATES_NOTES + LIST_OF_PHI_DATES_OMOP
 
 # Arguments: Meta-variables
 LOG_LEVEL = "DEBUG"
```

### Comparing `drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/i2b2ConvertIDs.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/i2b2ConvertIDs.py`

 * *Files identical despite different names*

### Comparing `drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/i2b2GetIDs.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/i2b2GetIDs.py`

 * *Files identical despite different names*

### Comparing `drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/i2b2MakeMap.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/i2b2MakeMap.py`

 * *Files identical despite different names*

### Comparing `drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/makeAgeMap.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/makeAgeMap.py`

 * *Files identical despite different names*

### Comparing `drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/makeDateShiftMap.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/makeDateShiftMap.py`

 * *Files identical despite different names*

### Comparing `drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/makeMapsFromOthers.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/makeMapsFromOthers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Makes de-identification maps, building on existing maps.
 
 # NOTE Does not expect data in nested directories (e.g., subfolders of "free_text"). Therefore it uses "Path.iterdir" instead of "Path.glob('*/**')".
+# NOTE Expects all files to be CSV files. This is because it uses "pd.read_csv".
 # NOTE Expects integer IDs, so no string IDs like Epic Patient IDs.
 """
 
 import json
 import logging
 import sys
 from pathlib import Path
@@ -16,15 +17,15 @@
 from drapi.code.drapi.drapi import (ditchFloat,
                                     getTimestamp,
                                     handleDatetimeForJson,
                                     makeDirPath,
                                     makeMap,
                                     makeSetComplement,
                                     successiveParents)
-from drapi.code.drapi.constants.phiVariables import (FILE_NAME_TO_VARIABLE_NAME_DICT,
+from drapi.constants.phiVariables import (FILE_NAME_TO_VARIABLE_NAME_DICT,
                                           VARIABLE_NAME_TO_FILE_NAME_DICT)
 # Local packages: Script parameters: General
 from common import (IRB_NUMBER,
                     DATA_REQUEST_ROOT_DIRECTORY_DEPTH,
                     DATA_TYPES_DICT,
                     OLD_MAPS_DIR_PATH,
                     VARIABLE_ALIASES,
```

### Comparing `drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/makeMapsFromScratch.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/makeMapsFromScratch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Makes de-identification maps from scratch.
 
 # NOTE Does not expect data in nested directories (e.g., subfolders of "free_text"). Therefore it uses "Path.iterdir" instead of "Path.glob('*/**')".
+# NOTE Expects all files to be CSV files. This is because it uses "pd.read_csv".
 # TODO Needs to combine similar IDs, like different providers IDs.
 """
 
 import logging
 import sys
 from pathlib import Path
 # Third-party packages
```

### Comparing `drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/launchIPython.bat` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/launchIPython.bat`

 * *Files identical despite different names*

### Comparing `drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/BO Portion Template/.gitignore` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # >>> [start] Things added by Herman >>>
 **/logs/*
 **/*.7z
 **/.DS_Store
 **/*.bat
 !**/launchIPython.bat
 **/*.csv
-**/*.out
 **/*.pdf
 **/*.tsv
 **/*.xlsx
 **/*.zip
 # <<< [end] Things added by Herman <<<
 
 # >>> [start] Default IDR files >>>
```

### Comparing `drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/BO Portion Template/launchIPython.bat` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/launchIPython.bat`

 * *Files identical despite different names*

### Comparing `drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/Clinical Text Portion Template/.gitignore` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # >>> [start] Things added by Herman >>>
 **/logs/*
 **/*.7z
 **/.DS_Store
 **/*.bat
 !**/launchIPython.bat
 **/*.csv
-**/*.out
 **/*.pdf
 **/*.tsv
 **/*.xlsx
 **/*.zip
 # <<< [end] Things added by Herman <<<
 
 # >>> [start] Default IDR files >>>
@@ -132,15 +131,15 @@
 celerybeat-schedule
 celerybeat.pid
 
 # SageMath parsed files
 *.sage.py
 
 # Environments
-.env
+!.env
 .venv
 env/
 venv/
 ENV/
 env.bak/
 venv.bak/
```

### Comparing `drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/Clinical Text Portion Template/code/filterNotes.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/code/filterNotes.py`

 * *Files identical despite different names*

### Comparing `drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/Clinical Text Portion Template/code/freeText.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/code/freeText.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import concurrent.futures
 import logging
 import os
 import random
 import re
 import shutil
-import sys
 from datetime import timedelta
 from logging import Logger
 from pathlib import Path
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     from _typeshed.dbapi import DBAPIConnection
 # Third-party packages
@@ -19,27 +18,27 @@
 import sqlalchemy as sa
 # Local packages
 from drapi.code.drapi.drapi import (getTimestamp,
                                     makeDirPath,
                                     replace_sql_query,
                                     successiveParents)
 
-# Arguments: Script arguments
-COHORT_NAME = ""                                    # An arbitrary name used in file names
-COHORT_FILE = ""                                    # A file name that is located directory specified by the variable `data_dir`
-IRB_NUMBER = ""                                     # Used for creating the de-identification map IDs.
-ID_TYPE = ""                                        # Pick from "EncounterCSN", "EncounterKey", or "PatientKey". Choose the ID type you used in `COHORT_FILE`
-NOTE_VERSION = ""                                   # Pick from "all", or "last"
-DE_IDENTIFICATION_MODE = ""                         # Pick from "deid", "lds", or "phi"
-LOG_LEVEL = ""                                      # See the "logging" module for valid values for the `loglevel` parameter.
-SQL_ENCOUNTER_EFFECTIVE_DATE_START = ""   # The beginning of date range of encounters to collect. Format: YYYY-MM-DD
-SQL_ENCOUNTER_EFFECTIVE_DATE_END = ""     # The end of date range of encounters to collect. Format: YYYY-MM-DD
+# Arguments: Script settings
+COHORT_NAME = "SGMCPLGB"                                    # An arbitrary name used in file names
+COHORT_FILE = "cohort.csv"                                    # A file name that is located directory specified by the variable `data_dir`
+IRB_NUMBER = "IRB201902162"                                     # Used for creating the de-identification map IDs.
+ID_TYPE = "PatientKey"                                        # Pick from "EncounterCSN", "EncounterKey", or "PatientKey". Choose the ID type you used in `COHORT_FILE`
+NOTE_VERSION = "all"                                   # Pick from "all", or "last"
+DE_IDENTIFICATION_MODE = "phi"                         # Pick from "deid", "lds", or "phi"
+LOG_LEVEL = "DEBUG"                                      # See the "logging" module for valid values for the `loglevel` parameter.
+SQL_ENCOUNTER_EFFECTIVE_DATE_START = '2011-06-01'   # The beginning of date range of encounters to collect. Format: YYYY-MM-DD
+SQL_ENCOUNTER_EFFECTIVE_DATE_END = '2023-12-31'     # The end of date range of encounters to collect. Format: YYYY-MM-DD
 
 # Arguments: SQL connection settings
-USE_WINDOWS_AUTHENTICATION = None                   # Boolean or `None`. By default this is determined based on the operating system, but can be forced by the user.
+USE_WINDOWS_AUTHENTICATION = True
 SERVER = "DWSRSRCH01.shands.ufl.edu"
 DATABASE_PROD = "DWS_PROD"
 DATABASE_NOTES = "DWS_NOTES"
 USERDOMAIN = "UFAD"
 USERNAME = os.environ["USER"]
 UID = None
 PWD = os.environ["HFA_UFADPWD"]
@@ -109,24 +108,14 @@
 database_notes = DATABASE_NOTES
 
 # Variables: SQL connection settings
 if UID:
     uid = UID[:]
 else:
     uid = fr"{USERDOMAIN}\{USERNAME}"
-if isinstance(USE_WINDOWS_AUTHENTICATION, type(None)):
-    operatingSystem = sys.platform
-    if operatingSystem in ["win32"]:
-        useWindowsAuthentication = True
-    elif operatingSystem in ["darwin", "linux"]:
-        useWindowsAuthentication = False
-    else:
-        raise Exception(f"""Unsupported operating system: "{operatingSystem}".""")
-else:
-    useWindowsAuthentication = USE_WINDOWS_AUTHENTICATION
 
 # Directory creation: General
 makeDirPath(runOutputDir)
 makeDirPath(runLogsDir)
 
 # Directory creation: Project-specific
 for dir in [data_dir, sql_dir, notes_dir, disclosure_dir]:
@@ -136,31 +125,14 @@
 elif DE_IDENTIFICATION_MODE.lower() in ["deid", "lds"]:
     makeDirPath(map_dir)
 else:
     raise Exception(f"Unexpected value for `DE_IDENTIFICATION_MODE`: {DE_IDENTIFICATION_MODE}.")
 
 # Functions
 
-def choosePathToLog(path: Path, rootPath: Path) -> Path:
-    """
-    Decides if a path is a subpath of `rootPath`. If it is, display it reltaive to `rootPath`. If it is not, display it as an absolute path.
-    """
-    commonPath = os.path.commonpath([path.absolute(), rootPath.absolute()])
-
-    lenCommonPath = len(commonPath)
-    lenRootPath = len(str(rootPath.absolute()))
-    if lenCommonPath < lenRootPath:
-        pathToDisplay = path
-    elif lenCommonPath >= lenRootPath:
-        pathToDisplay = path.absolute().relative_to(rootPath)
-    else:
-        raise Exception("An unexpected error occurred.")
-                                    
-    return pathToDisplay
-
 
 def connectToDatabase(host: str,
                       database: str,
                       useWindowsAuthentication=True) -> DBAPIConnection:
     """
     Connects to a SQL database given a `host` (server) and `database` value.
     """
@@ -169,26 +141,25 @@
                                      database=database)
     else:
         conStr = f"mssql+pymssql://{uid}:{PWD}@{host}/{database}"
         connection = sa.create_engine(conStr).connect()
     return connection
 
 
-def executeQuery(query: str, host: str, database: str, useWindowsAuthentication: bool) -> pd.DataFrame:
+def executeQuery(query: str, host: str, database: str) -> pd.DataFrame:
     """
     Executes a SQL query.
     INPUT:
         `query`: a string
         `host`: a string
         `databse`: a string
-        `useWindowsAuthentication`: a boolean
     OUTPUT:
         A pandas dataframe object.
     """
-    databaseConnection = connectToDatabase(host, database, useWindowsAuthentication=useWindowsAuthentication)
+    databaseConnection = connectToDatabase(host, database)
     queryResult = pd.read_sql(query, databaseConnection)
     databaseConnection.close()
     return queryResult
 
 
 # notes methods
 
@@ -224,16 +195,15 @@
         query = replace_sql_query(query, "XXXXX", id_str)
         query = replace_sql_query(query, "{PYTHON_VARIABLE: SQL_ENCOUNTER_EFFECTIVE_DATE_START}", SQL_ENCOUNTER_EFFECTIVE_DATE_START)
         query = replace_sql_query(query, "{PYTHON_VARIABLE: SQL_ENCOUNTER_EFFECTIVE_DATE_END}", SQL_ENCOUNTER_EFFECTIVE_DATE_END)
 
         logger.log(9, f"Using the following query:\n>>> Begin query >>>\n{query}\n<<< End query <<<")
         result = executeQuery(query=query,
                               host=host,
-                              database=database_prod,
-                              useWindowsAuthentication=useWindowsAuthentication)
+                              database=database_prod)
 
         logger.info(f"The chunk query has {len(result):,} rows.")
         result = result.drop_duplicates()
 
         logger.info(f"After dropping duplicates, the chunk query has {len(result):,} rows.")
         if (note_type == 'note' and note_version == 'last'):  # keep only the last version of the note
             result = result.sort_values(by=['NoteKey', 'ContactNumber'], ascending=[True, False])
@@ -279,16 +249,15 @@
         query_file = os.path.join(sql_dir, query_file)
         fpath = os.path.join(sql_dir, query_file)
         with open(fpath, "r") as file:
             query = file.read()
         query = replace_sql_query(query, "XXXXX", note_list)
         result = executeQuery(query=query,
                               host=host,
-                              database=database_notes,
-                              useWindowsAuthentication=useWindowsAuthentication)
+                              database=database_notes)
         # ensure that all ID columns are integers
         columns = result.columns
         for c in ['LinkageNoteID', 'OrderKey']:
             if (c in columns):
                 # fill missing values with 0 since 0 is never used for these IDs in reality
                 result[c] = result[c].fillna(0)
                 # use string instead of int type since some fields, such as EncounterCSN, are bigger than what python considers an integer
@@ -336,174 +305,71 @@
                 _ = future.result()
                 logger.info(f"""Completed item "{item}".""")
             except Exception as e:
                 logger.info(f"""An exception was generated by item "{item}": "{e}".""")
     return
 
 
-def combine_order_metadata(notes_dir, cohort, logger: logging.Logger):
-    ORDER_TYPE_LIST = ['order_impression',
-                       'order_narrative',
-                       'order_result_comment']
-    LIST_OF_COLUMNS_TO_INCLUDE = ['OrderKey',
-                                  'Line',
-                                  'OrderID',
-                                  'OrderPlacedDatetime',
-                                  'OrderResultDatetime',
-                                  'PatientKey',
-                                  'MRN_GNV',
-                                  'MRN_JAX',
-                                  'NoteType',
-                                  'EncounterDate',
-                                  'EncounterKey',
-                                  'EncounterCSN',
-                                  'OrderingProviderKey',
-                                  'OrderingProviderType',
-                                  'OrderingProviderSpecialty',
-                                  'AuthorizingProviderKey',
-                                  'AuthorizingProviderType',
-                                  'AuthorizingProviderSpecialty']
-    HEADER = True
-    MODE = 'w'
-    CHUNKSIZE = 100000
-    for orderType in ORDER_TYPE_LIST:
-        file = cohort + '_' + orderType + '_metadata.csv'
-        fpath = os.path.join(notes_dir, file)
-        logger.info(f"""  Checking if file exists: "{fpath}".""")
-        fileExists = os.path.exists(fpath)
-        if fileExists:
-            logger.info(f"""    File exists.""")
-            chunkGenerator1 = pd.read_csv(fpath, chunksize=CHUNKSIZE)
-            chunkGenerator2 = pd.read_csv(fpath, chunksize=CHUNKSIZE)
-            logger.info("    Counting the number of chunks in the file.")
-            it1Total = sum([1 for _ in chunkGenerator1])
-            logger.info("    Counting the number of chunks in the file - done.")
-            for it1, dfChunk in enumerate(chunkGenerator2, start=1):
-                dfChunk = pd.DataFrame(dfChunk)  # For type hinting
-                logger.info(f"""  ..  Working on chunk {it1:,} of {it1Total}.""")
-                if (orderType in ['order_narrative', 'order_impression']):
-                    dfChunk['Line'] = ''
-                dfChunk = dfChunk[LIST_OF_COLUMNS_TO_INCLUDE]
-                savePath = os.path.join(notes_dir, '{}_order_metadata.csv'.format(cohort))
-                logger.info(f"""  ..  Saving chunk to "{savePath}".""")
-                dfChunk.to_csv(path_or_buf=savePath,
-                               index=False,
-                               header=HEADER,
-                               mode=MODE)
-                HEADER = False
-                MODE = "a"
-        else:
-            logger.info(f"""    Warning: File does not exist.""")  # Not sure if this merits a warning.
-
-    # Final removal of duplicates
-    logger.info("Performing final removal of duplicates.")
-    df = pd.read_csv(savePath).drop_duplicates()
-    df.to_csv(savePath, index=False)
-    logger.info("Performing final removal of duplicates - done.")
+def combine_order_metadata(notes_dir, cohort):
+    m = 'w'
+    h = True
+    for file1 in ['order_narrative', 'order_impression', 'order_result_comment']:
+        file = cohort + '_' + file1 + '_metadata.csv'
+        if os.path.exists(os.path.join(notes_dir, file)):
+            df = pd.read_csv(os.path.join(notes_dir, file))
+            if (file1 in ['order_narrative', 'order_impression']):
+                df['Line'] = ''
+            df = df[['OrderKey', 'Line', 'OrderID', 'OrderPlacedDatetime', 'OrderResultDatetime', 'PatientKey', 'MRN_GNV', 'MRN_JAX', 'NoteType', 'EncounterDate', 'EncounterKey', 'EncounterCSN', 'OrderingProviderKey', 'OrderingProviderType', 'OrderingProviderSpecialty', 'AuthorizingProviderKey', 'AuthorizingProviderType', 'AuthorizingProviderSpecialty']]
+            df.to_csv(os.path.join(notes_dir, '{}_order_metadata.csv'.format(cohort)), index=False, mode=m, header=h)
+            m = 'a'
+            h = False
     return
 
 
-def create_encounters(notes_dir, logger: logging.Logger):
-    CHUNKSIZE = 100000
-    HEADER = True
-    MODE = "w"
-    fileList = ['{}_order_narrative_metadata.csv'.format(cohort),
-                '{}_order_impression_metadata.csv'.format(cohort),
-                '{}_order_result_comment_metadata.csv'.format(cohort),
-                '{}_note_metadata.csv'.format(cohort)]
-    it1Total = sum([1 for _ in fileList])
-    for it1, file in enumerate(fileList, start=1):
-        logger.info(f"""  Working on file {it1:,} of {it1Total:,}: "{file}".""")
-        chunkGenerator1 = pd.read_csv(os.path.join(notes_dir, file), chunksize=CHUNKSIZE)
-        chunkGenerator2 = pd.read_csv(os.path.join(notes_dir, file), chunksize=CHUNKSIZE)
-        logger.info("    Counting the number of chunks in the file.")
-        it2Total = sum([1 for _ in chunkGenerator1])
-        logger.info(f"    Counting the number of chunks in the file - done. There are {it2Total:,} chunks.")
-        for it2, dfChunk in enumerate(chunkGenerator2,  start=1):
-            dfChunk = pd.DataFrame(dfChunk)  # For type hinting
-            logger.info(f"""    Working on chunk {it2:,} of {it2Total:,}.""")
-            df = dfChunk[['EncounterCSN']].drop_duplicates()
-            savePath = os.path.join(notes_dir, 'encounters.csv')
-            logger.info(f"""    Saving chunk to "{choosePathToLog(Path(savePath), rootDirectory)}".""")
-            df.to_csv(path_or_buf=savePath,
-                      index=False,
-                      header=HEADER,
-                      mode=MODE)  # TODO This is an intermediate file that might be eligible for removal.
-            logger.info(f"""    Saving chunk to "{choosePathToLog(Path(savePath), rootDirectory)}" - done.""")
-            HEADER = False
-            MODE = "a"
-        logger.info(f"""  Working on file {it1:,} of {it1Total:,}: "{file}" - done.""")
-
-    # Final removal of duplicates
-    logger.info("Performing final removal of duplicates.")
-    df = pd.read_csv(savePath).drop_duplicates()
-    df.to_csv(savePath, index=False)
-    logger.info("Performing final removal of duplicates - done.")
+def create_encounters(notes_dir):
+    df = pd.DataFrame()
+    for file in ['{}_order_narrative_metadata.csv'.format(cohort), '{}_order_impression_metadata.csv'.format(cohort), '{}_order_result_comment_metadata.csv'.format(cohort), '{}_note_metadata.csv'.format(cohort)]:
+        for dfx in pd.read_csv(os.path.join(notes_dir, file), chunksize=100000):
+            df1 = dfx[['EncounterCSN']].drop_duplicates()
+            df = pd.concat([df, df1])
+            df.drop_duplicates(inplace=True)
+    df.to_csv(os.path.join(notes_dir, 'encounters.csv'), index=False)
     return
 
 
-def create_provider_metadata(notes_dir, cohort, logger: logging.Logger):
-    """
-    Creates the provider metadata table. It does so by reading through all the metadata files in chunks and keeping the unique rows.
-    """
-    savePath = os.path.join(notes_dir, 'provider_metadata.csv')
-    CHUNKSIZE = 100000
-    HEADER = True
-    MODE = "w"
-    listOfClinicalTextTypes = ['note',
-                               'order_impression',
-                               'order_narrative',
-                               'order_result_comment']
-    it1Total = len(listOfClinicalTextTypes)
-    for it1, file1 in enumerate(listOfClinicalTextTypes, start=1):
-        logger.info(f"""  Work on file {it1:,} of {it1Total:,}: "{file1}".""")
+def create_provider_metadata(notes_dir, cohort):
+    m = 'w'
+    h = True
+    df = pd.DataFrame()
+    for file1 in ['order_narrative', 'order_impression', 'order_result_comment', 'note']:
+        # for file in ['note']:
         file = cohort + '_' + file1 + '_metadata.csv'
-        fpath = os.path.join(notes_dir, file)
-        logger.info(f"""  Checking if file exists: "{fpath}".""")
-        fileExists = os.path.exists(fpath)
-        if fileExists:
-            logger.info(f"""    File exists.""")
-            chunkGenerator1 = pd.read_csv(fpath, chunksize=CHUNKSIZE)
-            chunkGenerator2 = pd.read_csv(fpath, chunksize=CHUNKSIZE)
-            logger.info("    Counting the number of chunks in the file.")
-            it2Total = sum([1 for _ in chunkGenerator1])
-            logger.info(f"    Counting the number of chunks in the file - done. There are {it2Total:,} chunks.")
-            for it2, dfChunk in enumerate(chunkGenerator2, start=1):
-                logger.info(f"""    Working on chunk {it2:,} of {it2Total:,}.""")
-                dfChunk = pd.DataFrame(dfChunk)  # For type hinting
+        if os.path.exists(os.path.join(notes_dir, file)):
+            for dfx in pd.read_csv(os.path.join(notes_dir, file), chunksize=100000):
                 if (file1 in ['order_narrative', 'order_impression', 'order_result_comment']):
-                    df1 = dfChunk[['OrderingProviderKey', 'OrderingProviderType', 'OrderingProviderSpecialty']]
+                    df1 = dfx[['OrderingProviderKey', 'OrderingProviderType', 'OrderingProviderSpecialty']]
                     df1 = df1.rename(columns={"OrderingProviderKey": "ProviderKey", "OrderingProviderType": "ProviderType", "OrderingProviderSpecialty": "ProviderSpecialty"})
-                    df2 = dfChunk[['AuthorizingProviderKey', 'AuthorizingProviderType', 'AuthorizingProviderSpecialty']]
+                    df2 = dfx[['AuthorizingProviderKey', 'AuthorizingProviderType', 'AuthorizingProviderSpecialty']]
                     df2 = df2.rename(columns={"AuthorizingProviderKey": "ProviderKey", "AuthorizingProviderType": "ProviderType", "AuthorizingProviderSpecialty": "ProviderSpecialty"})
                 elif (file1 in ['note']):
-                    df1 = dfChunk[['AuthoringProviderKey', 'AuthoringProviderType', 'AuthoringProviderSpecialty']]
+                    df1 = dfx[['AuthoringProviderKey', 'AuthoringProviderType', 'AuthoringProviderSpecialty']]
                     df1 = df1.rename(columns={"AuthoringProviderKey": "ProviderKey", "AuthoringProviderType": "ProviderType", "AuthoringProviderSpecialty": "ProviderSpecialty"})
-                    df2 = dfChunk[['CosignProviderKey', 'CosignProviderType', 'CosignProviderSpecialty']]
+                    df2 = dfx[['CosignProviderKey', 'CosignProviderType', 'CosignProviderSpecialty']]
                     df2 = df2.rename(columns={"CosignProviderKey": "ProviderKey", "CosignProviderType": "ProviderType", "CosignProviderSpecialty": "ProviderSpecialty"})
-                    df = pd.concat([df1, df2])
-                    df = df.drop_duplicates()
-                    df.to_csv(path_or_buf=savePath,
-                              index=False,
-                              header=HEADER,
-                              mode=MODE)
-                    HEADER = False
-                    MODE = "a"
-        else:
-            logger.info(f"""    Warning: File does not exist.""")  # Not sure if this merits a warning.
-
-    # Final removal of duplicates
-    logger.info("Performing final removal of duplicates.")
-    df = pd.read_csv(savePath).drop_duplicates()
-    df.to_csv(savePath, index=False)
-    logger.info("Performing final removal of duplicates - done.")
+                df1 = pd.concat([df1, df2])
+                df1.drop_duplicates(inplace=True)
+                df = pd.concat([df, df1])
+                df.drop_duplicates(inplace=True)
+            df.to_csv(os.path.join(notes_dir, 'provider_metadata.csv'), index=False, mode=m, header=h)
+            m = 'a'
+            h = False
     return
 
 
-def generate_map(deid_mode, in_dir, map_dir, concept, cohort, logger: logging.Logger):
+def generate_map(deid_mode, in_dir, map_dir, concept, cohort):
     """
     `concept` can be any of the following values:
         - patient
         - encounter
         - note
         - note_link
         - order
@@ -514,15 +380,15 @@
         concept_cd = 'PAT'
         concept_id = 'deid_pat_id'
         file = os.path.join(in_dir, COHORT_FILE)  # NOTE
         concept_column = 'PatientKey'
     elif (concept == 'encounter'):
         concept_cd = 'ENC'
         concept_id = 'deid_enc_id'
-        create_encounters(in_dir, logger=logger)
+        create_encounters(in_dir)
         file = os.path.join(in_dir, 'encounters.csv')
         concept_column = 'EncounterCSN'
     elif (concept == 'note'):
         concept_cd = 'NOTE'
         concept_id = 'deid_note_id'
         file = os.path.join(in_dir, '{}_note_metadata.csv'.format(cohort))
         concept_column = 'NoteKey'
@@ -530,58 +396,40 @@
         concept_cd = 'LINK_NOTE'
         concept_id = 'deid_link_note_id'
         file = os.path.join(in_dir, '{}_note_metadata.csv'.format(cohort))
         concept_column = 'LinkageNoteID'
     elif (concept == 'order'):
         concept_cd = 'ORDER'
         concept_id = 'deid_order_id'
-        combine_order_metadata(in_dir, cohort, logger=logger)
+        combine_order_metadata(in_dir, cohort)
         file = os.path.join(in_dir, '{}_order_metadata.csv'.format(cohort))
         concept_column = 'OrderKey'
     elif (concept == 'provider'):
         concept_cd = 'PROV'
         concept_id = 'deid_provider_id'
-        create_provider_metadata(in_dir, cohort, logger=logger)
+        create_provider_metadata(in_dir, cohort)
         file = os.path.join(in_dir, 'provider_metadata.csv')
         concept_column = 'ProviderKey'
     else:
-        logger.error(f"""Nonexisting concept in `generate_map` method: "{concept}".""")
+        logging.error(f"""Nonexisting concept in `generate_map` method: "{concept}".""")
 
-    # Count the number of chunks in the file
-    CHUNKSIZE = 10000
-    chunkGenerator1 = pd.read_csv(file, chunksize=CHUNKSIZE)
-    chunkGenerator2 = pd.read_csv(file, chunksize=CHUNKSIZE)
-    logger.info("Counting the number of chunks in the file.")
-    it1Total = sum([1 for _ in chunkGenerator1])
-    logger.info(f"""Counting the number of chunks in the file - done. The are {it1Total:,} chunks.""")
-    INDEX_START = 1
-    HEADER = True
-    MODE = "w"
-    for it1, ids in enumerate(chunkGenerator2, start=1):
-        logger.info(f"""  Working on chunk {it1:,} of {it1Total:,}.""")
-        ids = pd.DataFrame(ids)  # For type hinting
+    ids_final = pd.DataFrame()
+    for ids in pd.read_csv(file, chunksize=10000):
         ids = ids[[concept_column]].drop_duplicates()
-        ids.drop_duplicates(inplace=True)
-        index_end = len(ids) + INDEX_START
-        ids.index = range(INDEX_START, index_end)
-        ids_map = ids.reset_index()
-        ids_map['deid_num'] = ids_map.index
-        # Assign de-identification value of "0" for unknown input (e.g., provider key < 0)
-        ids_map[concept_id] = ids_map.apply(lambda row: (str(irb) + '_' + concept_cd + '_0') if (int(row[concept_column]) < 0) else (str(irb) + '_' + concept_cd + '_' + str(int(row['deid_num']))), axis=1)
-        if (deid_mode == 'deid' and concept == 'patient'):
-            ids_map['date_shift'] = ids_map.apply(lambda row: random.randint(-30, 30), axis=1)
-        out_file = 'map_{}.csv'.format(concept)
-        INDEX_START = max(ids_map["index"]) + 1
-        ids_map = ids_map.drop(['index'], axis=1)
-        savePath = Path(os.path.join(map_dir, out_file))
-        logger.info(f"""  Saving chunk to "{choosePathToLog(savePath, rootDirectory)}".""")
-        ids_map.to_csv(savePath, index=False, header=HEADER, mode=MODE)
-        logger.info(f"""  Saving chunk to "{choosePathToLog(savePath, rootDirectory)}" - done.""")
-        HEADER = False
-        MODE = "a"
+        ids_final = pd.concat([ids_final, ids])
+        ids_final.drop_duplicates(inplace=True)
+    ids_map = ids_final.reset_index()
+    ids_map['deid_num'] = ids_map.index + 1
+    # assign deid value 0 for unknown input (e.g., provider key < 0)
+    ids_map[concept_id] = ids_map.apply(lambda row: (str(irb) + '_' + concept_cd + '_0') if (int(row[concept_column]) < 0) else (str(irb) + '_' + concept_cd + '_' + str(int(row['deid_num']))), axis=1)
+    if (deid_mode == 'deid' and concept == 'patient'):
+        ids_map['date_shift'] = ids_map.apply(lambda row: random.randint(-30, 30), axis=1)
+    out_file = 'map_{}.csv'.format(concept)
+    ids_map = ids_map.drop(['index'], axis=1)
+    ids_map.to_csv(os.path.join(map_dir, out_file), index=False)
     return
 
 
 def deid_metadata(deid_mode, note_type, map_dir, notes_dir, disclosure_dir):
     # define variables
     text_file = '{}_{}_metadata.csv'.format(cohort, note_type)
     if (note_type == 'note'):
@@ -764,15 +612,15 @@
 logger.setLevel(9)
 
 if __name__ == "__main__":
     logger.info(f"""Begin running "{thisFilePath}".""")
     logger.info(f"""All other paths will be reported in debugging relative to `{ROOT_DIRECTORY}`: "{rootDirectory}".""")
     logger.info(f"""Script arguments:
 
-    # Arguments: Script arguments
+    # Arguments
     `COHORT_NAME`: "{COHORT_NAME}"
     `COHORT_FILE`: "{COHORT_FILE}"
     `IRB_NUMBER`: "{IRB_NUMBER}"
     `ID_TYPE`: "{ID_TYPE}"
     `NOTE_VERSION`: "{NOTE_VERSION}"
     `DE_IDENTIFICATION_MODE`: "{DE_IDENTIFICATION_MODE}"
     `SQL_ENCOUNTER_EFFECTIVE_DATE_START`: "{SQL_ENCOUNTER_EFFECTIVE_DATE_START}"
@@ -822,50 +670,28 @@
         # combine all order metadata files and copy to discosure folder
         combine_order_metadata(notes_dir, cohort)
         format_metadata_files('order', notes_dir, disclosure_dir)
 
         # copy .tsv files with free text
         copy_tsv(cohort, notes_dir, disclosure_dir)
     else:
-        # Generate mappings
-        logger.info("Generating de-identification maps for PHI variables.")
-        logger.info("  Generating map for encounter IDs.")
-        generate_map(deid_mode, notes_dir, map_dir, 'encounter', cohort, logger=logger)
-        logger.info("  Generating map for encounter IDs - done.")
-        logger.info("  Generating map for note IDs.")
-        generate_map(deid_mode, notes_dir, map_dir, 'note', cohort, logger=logger)
-        logger.info("  Generating map for note IDs - done.")
-        logger.info("""  Generating map for note linkage IDs.""")
-        generate_map(deid_mode, notes_dir, map_dir, 'note_link', cohort, logger=logger)
-        logger.info("  Generating map for note linkage IDs.")
-        logger.info("  Generating map for order IDs.")
-        generate_map(deid_mode, notes_dir, map_dir, 'order', cohort, logger=logger)
-        logger.info("  Generating map for order IDs - done.")
-        logger.info("  Generating map for patient IDs.")
-        generate_map(deid_mode, data_dir, map_dir, 'patient', cohort, logger=logger)
-        logger.info("  Generating map for patient IDs - done.")
-        logger.info("  Generating map for provider IDs.")
-        generate_map(deid_mode, notes_dir, map_dir, 'provider', cohort, logger=logger)
-        logger.info("  Generating map for provider IDs - done.")
-        logger.info("Generating de-identification maps for PHI variables - done.")
-
-        # De-identify metadata.
-        logger.info("De-identifying metadata.")
-        for clinicalTextCategory in ["note", "order"]:
-            logger.info(f"""  De-identifying metadata for clinical text of category "{clinicalTextCategory}".""")
-            deid_metadata(deid_mode, clinicalTextCategory, map_dir, notes_dir, disclosure_dir)
-            logger.info(f"""  De-identifying metadata for clinical text of category "{clinicalTextCategory}" - done.""")
-        logger.info("De-identifying metadata - done.")
+        # generate mappings
+        generate_map(deid_mode, data_dir, map_dir, 'patient', cohort)
+        generate_map(deid_mode, notes_dir, map_dir, 'encounter', cohort)
+        generate_map(deid_mode, notes_dir, map_dir, 'note', cohort)
+        generate_map(deid_mode, notes_dir, map_dir, 'note_link', cohort)
+        generate_map(deid_mode, notes_dir, map_dir, 'order', cohort)
+        generate_map(deid_mode, notes_dir, map_dir, 'provider', cohort)
+
+        # deidentify metadata. We can create deidentified dataset or limited dataset.
+        deid_metadata(deid_mode, 'note', map_dir, notes_dir, disclosure_dir)
+        deid_metadata(deid_mode, 'order', map_dir, notes_dir, disclosure_dir)
 
-        # De-identify clinical text, i.e., de-identify ID in .tsv file(s)
-        logger.info("""De-identifying clinical text of category "note".""")
+        # prepare for text deidentification, i.e., deidentify ID in .tsv file(s)
         deid_tsv_note(map_dir, notes_dir, logger)
-        logger.info("""De-identifying clinical text of category "note" - done.""")
-        logger.info("""De-identifying clinical text of category "order".""")
         deid_tsv_order(map_dir, notes_dir, logger)
-        logger.info("""De-identifying clinical text of category "order" - done.""")
 
     # Output location summary
     logger.info(f"""Script output is located in the following directory: "{runOutputDir.absolute().relative_to(rootDirectory)}".""")
 
     # End script
     logger.info(f"""Finished running "{thisFilePath.absolute().relative_to(rootDirectory)}".""")
```

### Comparing `drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/Clinical Text Portion Template/launchIPython.bat` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/launchIPython.bat`

 * *Files identical despite different names*

### Comparing `drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/Clinical Text Portion Template/sql/note_metadata.sql` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/sql/note_metadata.sql`

 * *Files identical despite different names*

### Comparing `drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/Clinical Text Portion Template/sql/order_impression_metadata.sql` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/sql/order_impression_metadata.sql`

 * *Files identical despite different names*

### Comparing `drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/Clinical Text Portion Template/sql/order_narrative_metadata.sql` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/sql/order_narrative_metadata.sql`

 * *Files identical despite different names*

### Comparing `drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/Clinical Text Portion Template/sql/order_result_comment_metadata.sql` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/sql/order_result_comment_metadata.sql`

 * *Files identical despite different names*

### Comparing `drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/General Script Template/.gitignore` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # >>> [start] Things added by Herman >>>
 **/logs/*
 **/*.7z
 **/.DS_Store
 **/*.bat
 !**/launchIPython.bat
 **/*.csv
-**/*.out
 **/*.pdf
 **/*.tsv
 **/*.xlsx
 **/*.zip
 # <<< [end] Things added by Herman <<<
 
 # >>> [start] Default IDR files >>>
```

### Comparing `drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/General Script Template/code/RenameMe.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/code/RenameMe.py`

 * *Files identical despite different names*

### Comparing `drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/General Script Template/code/compareGroupsTemplate.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/code/compareGroupsTemplate.py`

 * *Files identical despite different names*

### Comparing `drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/General Script Template/code/loopTemplate.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/code/loopTemplate.py`

 * *Files identical despite different names*

### Comparing `drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/General Script Template/launchIPython.bat` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/launchIPython.bat`

 * *Files identical despite different names*

### Comparing `drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/OMOP Portion Template/.gitignore` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,22 @@
 # >>> [start] Things added by Herman >>>
-**/logs/*
 **/*.7z
 **/.DS_Store
-**/*.bat
-!**/launchIPython.bat
 **/*.csv
-**/*.out
-**/*.pdf
-**/*.tsv
-**/*.xlsx
-**/*.zip
-**/data/output/**/*.yml
+**/logs/*
 # <<< [end] Things added by Herman <<<
 
 # >>> [start] Default IDR files >>>
+settings.yaml
+types.yaml
 data/*
 !data/input/
 !data/output/
 documents/*
 HIPPA_disclosure/*
-settings.yaml
-types.yaml
 # <<< [end] Default IDR files <<<
 
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
@@ -133,15 +125,16 @@
 celerybeat-schedule
 celerybeat.pid
 
 # SageMath parsed files
 *.sage.py
 
 # Environments
-!.env
+.env
+!drapiPackage/templates/makeDirTemplate/**/.env
 .venv
 env/
 venv/
 ENV/
 env.bak/
 venv.bak/
```

### Comparing `drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/OMOP Portion Template/Config1.YAML` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/Config1.yml`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 date_range: 
   start_date: YYYY-MM-DD
   end_date: YYYY-MM-DD
 db_connections: 
   data_pull:
     server: DWSRSRCH01.shands.ufl.edu
     database: DWS_OMOP_PROD
-    schema: dbo # options: `dbo` or `hipaa`. For fully identified data, enter `dbo`, for de-identified data (date-shifted and no PHI) enter `hipaa`.
+    schema: dbo
 data_output:  # Assumes Windows path separator (i.e., "\"), and must end with path separator
-  identified_file_location: 'data\output\identified'
-  deidentified_file_location: 'data\output\de-identified'
+  identified_file_location: 'data\output\'
+  deidentified_file_location: 'data\output\'
   mapping_location: 'data\output\'
 
 # Path of the list of OMOP person IDs to use to pull the day, i.e. the cohort. The path
 # is expected to be relative to the project directory, i.e. the command line working directory.
-person_id: 'data/output/getPersonIDs/.../personIDs.csv'
+person_id: 'data/output/getPersonIDs/2023-03-08 16-09-44/personIDs.csv'
 
 #####   DATA RELEASE SELECTION   #####
 data_release:
   - identified
   # - deidentified
   # - limited
```

### Comparing `drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/OMOP Portion Template/README.md` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/README.md`

 * *Files identical despite different names*

### Comparing `drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/OMOP Portion Template/code/Project1.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/code/Project1.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,36 +12,36 @@
 import sys
 from pathlib import Path
 # Third-party libraries
 import pandas as pd
 import sqlalchemy as sa
 import yaml
 # Super-local libraries
-import deidentify
+import drapi.code.drapi.omop.deidentify as deidentify
 from drapi.code.drapi.drapi import (makeDirPath,
                                     getTimestamp)
 from drapi.code.drapi.omop.configProcessing import (editConfig,
                                                     interpretPath)
 
 # Arguments
-LOG_LEVEL = "INFO"  # Lowest level available is "9"
+LOG_LEVEL = "DEBUG"  # Lowest level available is "9"
 
 # Arguments: SQL server settings
 if False:
     # TODO Not implemented. See `db_connect`
     USERNAME_ENVIRONMENT_VARIABLE = "USER"
     PASSWORD_ENVIRONMENT_VARIABLE = "HFA_UFADPWD"
     SERVER = "DWSRSRCH01.shands.ufl.edu"  # AKA `HOST`
     DATABASE = "DWS_OMOP_PROD"
     USERDOMAIN = "UFAD"
 
 # Variables
 timestamp = getTimestamp()
-config_file0 = os.path.join("Config1.YAML")
-config_file = os.path.join("Data", "Output", "Config2.YAML")
+config_file0 = os.path.join("Config1.yml")
+config_file = os.path.join("Data", "Output", "Config2.yml")
 editConfig(config_file0, config_file, timestamp)
 base_dir = Path(__file__).parent.parent
 
 # Variables: SQL server settings
 if False:
     # TODO Not implemented. See `db_connect`
     username = os.environ[USERNAME_ENVIRONMENT_VARIABLE]
@@ -75,15 +75,15 @@
     return config_setting
 
 
 def db_query(query, db_connection):
     dfs = pd.DataFrame()
     for chunk in pd.read_sql(query, db_connection, chunksize=50000):
         df = pd.DataFrame(chunk)
-        dfs = pd.concat([dfs, df], ignore_index=False)
+        dfs = dfs.append(df, ignore_index=False)
     return dfs
 
 
 def db_execute_read_query(host, database, query):
     db_conn = db_connect(host, database)
     data = db_query(query, db_conn)
     db_close(db_conn)
@@ -179,15 +179,15 @@
         message = f"""  Working on table "{current_table}", table {i+1} of {numTables}."""
         logging.info(message)
         columns = search_config.get(current_table)
         columns_string = ', '.join(map(str, columns))
         # Get number of chunks of table
         numChunks = sum([1 for _ in pd.read_csv(person_id_file_path, chunksize=500)])
         for it, person_id in enumerate(pd.read_csv(person_id_file_path, chunksize=500), start=1):
-            logging.info(f"""    Working on table chunk {it} of {numChunks}""")
+            logging.debug(f"""    Working on table chunk {it} of {numChunks}""")
             person_id_list = person_id.iloc[:, 0]
             person_id_list_string = ', '.join(map(str, person_id_list))
             date_sorted_by = dict_of_dates.get(current_table)
             query_string = "(SELECT " + columns_string + " FROM " + current_table + " WHERE person_id IN (" + person_id_list_string + ") AND " + date_sorted_by + " BETWEEN " + start_date + " AND " + end_date + ")"
             if ((dict_of_search.get(current_table) is not None)):
                 row_query_string = ''
                 rows = dict_of_search.get(current_table)
@@ -235,15 +235,15 @@
             logging.log(9, f"  ..  >>> This is the query >>>\n{query_string}\n<<< End of query <<<")
             data = db_execute_read_query(host, database, query_string)
             if not data.empty:
                 identified_file_location_asString = interpretPath(search_config['data_output']['identified_file_location'])
                 file_location = identified_file_location_asString + current_table + '.csv'
                 csv_output_file = (file_location)
                 try:
-                    logging.info(f"""  ..  Saving query chunk results to "{csv_output_file}".""")
+                    logging.debug(f"""  ..  Saving query chunk results to "{csv_output_file}".""")
                     data.to_csv(csv_output_file, index=False, header=h, mode=m)
                     h = False
                     m = 'a'
                 except Exception as err:
                     errorMessage = f"{err.__class__.__name__}: {err.__str__()}"
                     message = f"An exception has occurred. This may be caused by an output directory error; please double check the directory in the config file. The actual exception message is below:\n{errorMessage}"
                     logging.error(message)
@@ -280,19 +280,18 @@
 
     logging.info("Starting program.")
     # import search configuration
     search_config = import_config()
     # import connection information for DB connection
     host, database, schema, list_of_tables, dict_of_dates, person_id_file_path, start_date, end_date, search_config, dict_of_search = db_info(search_config)
 
-    logging.info(f"""Reading cohort from `person_id_file_path`: "{person_id_file_path}".""")
+    logging.debug(f"""Reading cohort from `person_id_file_path`: "{person_id_file_path}".""")
 
     for dataType, path in search_config["data_output"].items():
         path = Path(interpretPath(path))
         makeDirPath(path)
 
     if (list_of_tables):
         query_attempt(search_config, list_of_tables, dict_of_dates, person_id_file_path, start_date, end_date, dict_of_search)
-    if "person_information_tables" in search_config.keys():
-        person_info_query(search_config)
+    person_info_query(search_config)
     # deidentify_(mapping_file_location)
     logging.info("Finished program.")
```

### Comparing `drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/OMOP Portion Template/code/deidentify.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/code/deidentify.py`

 * *Files identical despite different names*

### Comparing `drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/OMOP Portion Template/code/getPersonIDs.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/code/getPersonIDs.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 """
-Get "Person ID" from "Patient Key" using `getData`.
+Get "Person ID" from "Patient Key"
 """
 
 import logging
 import os
-import shutil
 from pathlib import Path
 # Third-party packages
 import pandas as pd
 # Local packages
 from drapi.code.drapi.drapi import (getTimestamp,
                                     makeDirPath,
                                     successiveParents)
-from drapi.code.drapi.getData.getData import getData
 
 # Arguments
-PATIENT_KEYS_CSV_FILE_PATH = ""  # TODO
-PATIENT_KEYS_CSV_FILE_HEADER = ""  # TODO
+PATIENT_KEYS_CSV_FILE_PATH = Path("data/input/Cohort - Patient Key.CSV")  # TODO
+PATIENT_KEYS_CSV_FILE_HEADER = "Patient Key"  # TODO
 
 # Arguments: Meta-variables
 PROJECT_DIR_DEPTH = 2
 DATA_REQUEST_DIR_DEPTH = PROJECT_DIR_DEPTH + 2
 IRB_DIR_DEPTH = PROJECT_DIR_DEPTH + 2
 IDR_DATA_REQUEST_DIR_DEPTH = IRB_DIR_DEPTH + 3
 
@@ -47,18 +45,15 @@
 projectDir, _ = successiveParents(thisFilePath.absolute(), PROJECT_DIR_DEPTH)
 dataRequestDir, _ = successiveParents(thisFilePath.absolute(), DATA_REQUEST_DIR_DEPTH)
 IRBDir, _ = successiveParents(thisFilePath, IRB_DIR_DEPTH)
 IDRDataRequestDir, _ = successiveParents(thisFilePath.absolute(), IDR_DATA_REQUEST_DIR_DEPTH)
 dataDir = projectDir.joinpath("data")
 if dataDir:
     inputDataDir = dataDir.joinpath("input")
-    intermediateDataDir = dataDir.joinpath("intermediate")
     outputDataDir = dataDir.joinpath("output")
-    if intermediateDataDir:
-        runIntermediateDataDir = intermediateDataDir.joinpath(thisFileStem, runTimestamp)
     if outputDataDir:
         runOutputDir = outputDataDir.joinpath(thisFileStem, runTimestamp)
 logsDir = projectDir.joinpath("logs")
 if logsDir:
     runLogsDir = logsDir.joinpath(thisFileStem)
 sqlDir = projectDir.joinpath("sql")
 
@@ -83,15 +78,14 @@
     uid = fr"{USERDOMAIN}\{USERNAME}"
 conStr = f"mssql+pymssql://{uid}:{PWD}@{SERVER}/{DATABASE}"
 
 # Variables: Other
 pass
 
 # Directory creation: General
-makeDirPath(runIntermediateDataDir)
 makeDirPath(runOutputDir)
 makeDirPath(runLogsDir)
 
 # Directory creation: Project-specific
 pass
 
 # Logging block
@@ -136,56 +130,33 @@
     `USERNAME` = "{USERNAME}"
     `UID` = "{UID}"
     `PWD` = censored
     """)
 
     # Script
     # Get patient keys
-    data = pd.read_csv(PATIENT_KEYS_CSV_FILE_PATH)
+    patientKeysInput = pd.read_csv(PATIENT_KEYS_CSV_FILE_PATH, dtype={0: int}).drop_duplicates()
+    listAsString = ",".join([str(x) for x in patientKeysInput.values.flatten()])
 
     # Get input file header
-    nColumns = data.shape[1]
+    assert patientKeysInput.shape[1] == 1, "Expected file input should be just one column containing patient keys."
     if PATIENT_KEYS_CSV_FILE_HEADER:
         inputFileHeader = PATIENT_KEYS_CSV_FILE_HEADER
     else:
-        if nColumns == 1:
-            inputFileHeader = data.columns[0]
-        else:
-            message = f"""The input data has more than one column and you did not specify the column to use. Please set a value for `PATIENT_KEYS_CSV_FILE_HEADER`."""
-            logger.critical(message)
-            raise Exception(message)
-
-    patientKeysInput = data[inputFileHeader].astype(int).drop_duplicates().sort_values()
+        inputFileHeader = patientKeysInput.columns[0]
 
     # Query person IDs
     logger.info("""Querying database for person IDs.""")
-    queryResultsDir = runIntermediateDataDir.joinpath("Query Results")
-    queryResultsDir.mkdir()
-    getData(sqlFilePath=personID_SQLQueryFilePath,
-            connectionString=conStr,
-            filterVariablePythonDataType="int",
-            filterVariableSqlQueryTemplatePlaceholder="{PYTHON_VARIABLE: Patient Key}",
-            logger=logger,
-            outputFileName="Person ID",
-            runOutputDir=queryResultsDir,
-            filterVariableColumnName=PATIENT_KEYS_CSV_FILE_HEADER,
-            filterVariableFilePath=PATIENT_KEYS_CSV_FILE_PATH)
+    with open(personID_SQLQueryFilePath, "r") as file:
+        text = file.read()
+    query = text.replace("XXXXX", listAsString)
+    queryResults = pd.read_sql(query, con=conStr)
     logger.info("""Querying database for person IDs - done.""")
 
-    # Load query results
-    queryResults = pd.DataFrame()
-    resultsList = sorted(queryResultsDir.iterdir())
-    it1Total = len(resultsList)
-    for it1, fpath in enumerate(resultsList, start=1):
-        logger.info(f"""  Loading query result {it1:,} of {it1Total:,}.""")
-        df = pd.read_csv(fpath)
-        queryResults = pd.concat([queryResults, df])
-
     # Compare number of Person IDs returned with Patient Keys queried
-    patientKeysInput = pd.DataFrame(patientKeysInput)
     patientKeysInput = patientKeysInput.rename(columns={inputFileHeader: "Patient Key"})
     patientKeysInput["Patient Key"] = patientKeysInput["Patient Key"].astype(int)
     queryResults["Patient Key"] = queryResults["Patient Key"].astype(int)
     patientKeysInput["Found"] = patientKeysInput["Patient Key"].isin(queryResults["Patient Key"])
     personIDsFound = patientKeysInput.set_index("Patient Key").join(queryResults.set_index("Patient Key"), "Patient Key", "left")
     personIDsFound = personIDsFound.sort_values("person_id")
 
@@ -205,22 +176,19 @@
                 if pd.isna(value):
                     li.append("")
                 else:
                     li.append(str(int(value)))
             personIDsFound2[column] = li
 
     # Save results: Person IDs found
-    personIDsFoundExportPath = runOutputDir.joinpath("Person IDs - QA.csv")
+    personIDsFoundExportPath = runOutputDir.joinpath("personIDsFound.csv")
     personIDsFound2.to_csv(personIDsFoundExportPath)
-    logger.info(f"""The map of patient keys to person IDs, and those missing or found, was saved to "{personIDsFoundExportPath.absolute().relative_to(rootDirectory)}".""")
+    logger.info(f"""The map of patient keys to person IDs, and those missing or found, was saved to "{personIDsFoundExportPath}".""")
 
     # Save results: person IDs
     personIDs = personIDsFound["person_id"].drop_duplicates().dropna().sort_values().astype(int)
-    personIDsExportPath = runOutputDir.joinpath("Person IDs.csv")
+    personIDsExportPath = runOutputDir.joinpath("personIDs.csv")
     personIDs.to_csv(personIDsExportPath, index=False)
     logger.info(f"""Person IDs were saved to "{personIDsExportPath.relative_to(projectDir)}".""")
 
-    # Remove intermediate files
-    shutil.rmtree(runIntermediateDataDir)
-
     # End script
     logger.info(f"""Finished running "{thisFilePath.relative_to(projectDir)}".""")
```

### Comparing `drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/OMOP Portion Template/launchIPython.bat` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/launchIPython.bat`

 * *Files identical despite different names*

### Comparing `drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/i2b2 Portion Template/.gitignore` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/.gitignore`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 # >>> [start] Things added by Herman >>>
-**/logs/*
 **/*.7z
 **/.DS_Store
-**/*.bat
-!**/launchIPython.bat
 **/*.csv
-**/*.out
-**/*.pdf
-**/*.tsv
-**/*.xlsx
-**/*.zip
+**/logs/*
 # <<< [end] Things added by Herman <<<
 
 # >>> [start] Default IDR files >>>
+# Do not add IDR files to the top-level .gitignore or it will ignore the directories and files in the template directory.
+# settings.yaml
+# types.yaml
 data/*
 !data/input/
 !data/output/
 documents/*
 HIPPA_disclosure/*
-settings.yaml
-types.yaml
 # <<< [end] Default IDR files <<<
 
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
```

### Comparing `drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/i2b2 Portion Template/code/i2b2_dump.py` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/code/i2b2_dump.py`

 * *Files identical despite different names*

### Comparing `drapi_lemur-1.0.40/src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/i2b2 Portion Template/launchIPython.bat` & `drapi-lemur-1.0.5/src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/launchIPython.bat`

 * *Files identical despite different names*

### Comparing `drapi_lemur-1.0.40/src/drapi/templates/scripts/hippaDisclosure.py` & `drapi-lemur-1.0.5/src/drapi/templates/scripts/hippaDisclosure.py`

 * *Files identical despite different names*

### Comparing `drapi_lemur-1.0.40/src/drapi/templates/scripts/sqlQuery.py` & `drapi-lemur-1.0.5/src/drapi/templates/scripts/sqlQuery.py`

 * *Files identical despite different names*

### Comparing `drapi_lemur-1.0.40/src/drapi_lemur.egg-info/PKG-INFO` & `drapi-lemur-1.0.5/src/drapi_lemur.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drapi-lemur
-Version: 1.0.40
+Version: 1.0.5
 Summary: Data Request API for the Integrated Data Repository Research Services of University of Florida.
 Home-page: https://github.com/ChemGuy88/hermanCode/archive/refs/tags/v1.0.0.tar.gz
 Author: Herman Autore
 Author-email: hf.autore+drapi@gmail.com
 Keywords: CTSI,Clinical and Translational Science Institute,IDR,Integrated Data Repository,Integrated Data Repository Research Services,ODSRI,Office of Data Science and Research Implementation,Shands,Sloth 🦥,UF,UF Health,UFHealth,University of Florida
 
 Data Request API for the Integrated Data Repository Research Services of University of Florida.
```

### Comparing `drapi_lemur-1.0.40/src/drapi_lemur.egg-info/SOURCES.txt` & `drapi-lemur-1.0.5/src/drapi_lemur.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,171 +1,150 @@
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
+src/makeDirTemplate.py
 src/drapi/__init__.py
 src/drapi/code/__init__.py
+src/drapi/code/tree.py
 src/drapi/code/drapi/__init__.py
 src/drapi/code/drapi/compareGroups.py
-src/drapi/code/drapi/deIdentificationFunctions.py
 src/drapi/code/drapi/drapi.py
-src/drapi/code/drapi/expandColumn.py
 src/drapi/code/drapi/getPersonIDs.py
-src/drapi/code/drapi/makeListOfDates.py
 src/drapi/code/drapi/makeSymLinks.py
-src/drapi/code/drapi/modifyTSV.py
-src/drapi/code/drapi/parseAliasArguments.py
+src/drapi/code/drapi/oneFlorida.py
 src/drapi/code/drapi/prepTSVforSDOH.py
 src/drapi/code/drapi/searchFolders.py
 src/drapi/code/drapi/sql.py
 src/drapi/code/drapi/stats.py
 src/drapi/code/drapi/c2s/__init__.py
 src/drapi/code/drapi/c2s/c2s.py
+src/drapi/code/drapi/c2s/checkC2S.py
 src/drapi/code/drapi/constants/__init__.py
 src/drapi/code/drapi/constants/constants.py
 src/drapi/code/drapi/constants/phiValues.py
 src/drapi/code/drapi/constants/phiVariables.py
-src/drapi/code/drapi/constants/variableAliases.py
-src/drapi/code/drapi/convertColumns/hash.py
 src/drapi/code/drapi/deIdentificationSuiteFuncs0/__init__.py
 src/drapi/code/drapi/deIdentificationSuiteFuncs0/common.py
 src/drapi/code/drapi/deIdentificationSuiteFuncs0/concatenateMaps.py
 src/drapi/code/drapi/deIdentificationSuiteFuncs0/convertColumns.py
 src/drapi/code/drapi/deIdentificationSuiteFuncs0/dataQualityTest.py
 src/drapi/code/drapi/deIdentificationSuiteFuncs0/deIdentify.py
 src/drapi/code/drapi/deIdentificationSuiteFuncs0/deleteColumns.py
 src/drapi/code/drapi/deIdentificationSuiteFuncs0/gatherFiles.py
 src/drapi/code/drapi/deIdentificationSuiteFuncs0/getIDValues.py
 src/drapi/code/drapi/deIdentificationSuiteFuncs0/getProjectColumns.py
 src/drapi/code/drapi/deIdentificationSuiteFuncs0/makeMapsFromOthers.py
 src/drapi/code/drapi/deIdentificationSuiteFuncs0/makeMapsFromScratch.py
 src/drapi/code/drapi/deIdentificationSuiteFuncs0/makePersonIDMap.py
-src/drapi/code/drapi/getData/getData.py
-src/drapi/code/drapi/getData/getData_inner.py
-src/drapi/code/drapi/getData/getData_outer.py
 src/drapi/code/drapi/idealist/__init__.py
 src/drapi/code/drapi/idealist/getEncountersMap.py
 src/drapi/code/drapi/idealist/getPatientsMap.py
 src/drapi/code/drapi/idealist/idealist.py
 src/drapi/code/drapi/images/__init__.py
 src/drapi/code/drapi/images/utilities.py
 src/drapi/code/drapi/notes/__init__.py
 src/drapi/code/drapi/notes/freeText.py
 src/drapi/code/drapi/notes/pullNotes.py
 src/drapi/code/drapi/notes/utils.py
 src/drapi/code/drapi/omop/__init__.py
 src/drapi/code/drapi/omop/configProcessing.py
 src/drapi/code/drapi/omop/deidentify.py
-src/drapi/code/drapi/oneFlorida/__init__.py
-src/drapi/code/drapi/oneFlorida/oneFlorida.py
-src/drapi/code/drapi/qa/columnConversion.py
-src/drapi/code/drapi/qa/deidentification.py
 src/drapi/code/makeDirTemplate/__init__.py
 src/drapi/sql/9-Digit Zip Code.SQL
 src/drapi/sql/Consent2Share.sql
 src/drapi/sql/ConvertBetweenMrnAndOneFloridaPatID.SQL
 src/drapi/sql/LADMF.sql
 src/drapi/sql/MRNfromPatientKey.sql
-src/drapi/sql/OneFlorida to UF Health Patient ID Map.SQL
+src/drapi/sql/MapOneFloridaIDs.SQL
 src/drapi/sql/encounterNumber2patientKey.SQL
-src/drapi/templates/__init__.py
-src/drapi/templates/Anaconda Environment Variables/RenameMe environment-name/README.md
-src/drapi/templates/Data Disclosure README/README.md
-src/drapi/templates/Portions Templates/__init__.py
-src/drapi/templates/Portions Templates/Multi-Portion Template/.gitignore
-src/drapi/templates/Portions Templates/Multi-Portion Template/README.md
-src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/.gitignore
-src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/README.md
-src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/launchIPython.bat
-src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/aliasVariables.py
-src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/common.py
-src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/concatenateMaps.py
-src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/concatenateTables.py
-src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/convertColumns.py
-src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/convertColumnsGeneral.py
-src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/dataQualityTest.py
-src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/deIdentify.py
-src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/deIdentifyByAge.py
-src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/deIdentifyDates.py
-src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/deleteByColumnValues.py
-src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/deleteColumns.py
-src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/gatherFiles.py
-src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/getIDValues.py
-src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/getProjectColumns.py
-src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/i2b2ConvertIDs.py
-src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/i2b2GetIDs.py
-src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/i2b2MakeMap.py
-src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/makeAgeMap.py
-src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/makeDateShiftMap.py
-src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/makeMapsFromOthers.py
-src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/makeMapsFromScratch.py
-src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/makePersonIDMap.py
-src/drapi/templates/Portions Templates/Multi-Portion Template/Concatenated Results/code/mapToSqlite.py
-src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/BO Portion Template/.gitignore
-src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/BO Portion Template/README.md
-src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/BO Portion Template/launchIPython.bat
-src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/BO Portion Template/code/example.py
-src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/BO Portion Template/data/input/.deleteme
-src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/BO Portion Template/data/output/.deleteme
-src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/Clinical Text Portion Template/.gitignore
-src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/Clinical Text Portion Template/README.md
-src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/Clinical Text Portion Template/launchIPython.bat
-src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/Clinical Text Portion Template/code/filterNotes.py
-src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/Clinical Text Portion Template/code/freeText.py
-src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/Clinical Text Portion Template/code/script.bash
-src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/Clinical Text Portion Template/data/input/.deleteme
-src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/Clinical Text Portion Template/data/output/.deleteme
-src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/Clinical Text Portion Template/sql/note_metadata.sql
-src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/Clinical Text Portion Template/sql/note_text.sql
-src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/Clinical Text Portion Template/sql/order_impression_metadata.sql
-src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/Clinical Text Portion Template/sql/order_impression_text.sql
-src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/Clinical Text Portion Template/sql/order_narrative_metadata.sql
-src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/Clinical Text Portion Template/sql/order_narrative_text.sql
-src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/Clinical Text Portion Template/sql/order_result_comment_metadata.sql
-src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/Clinical Text Portion Template/sql/order_result_comment_text.sql
-src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/General Script Template/.gitignore
-src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/General Script Template/README.md
-src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/General Script Template/launchIPython.bat
-src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/General Script Template/code/RenameMe.py
-src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/General Script Template/code/compareGroupsTemplate.py
-src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/General Script Template/code/loopTemplate.py
-src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/General Script Template/data/input/.deleteme
-src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/General Script Template/data/output/.deleteme
-src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/OMOP Portion Template/.gitignore
-src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/OMOP Portion Template/Config1.YAML
-src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/OMOP Portion Template/README.md
-src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/OMOP Portion Template/launchIPython.bat
-src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/OMOP Portion Template/code/Project1.py
-src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/OMOP Portion Template/code/deidentify.py
-src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/OMOP Portion Template/code/getPersonIDs.py
-src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/OMOP Portion Template/data/input/.deleteme
-src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/OMOP Portion Template/data/output/.deleteme
-src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/OMOP Portion Template/sql/grabPersonIDs.SQL
-src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/i2b2 Portion Template/.gitignore
-src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/i2b2 Portion Template/README.md
-src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/i2b2 Portion Template/launchIPython.bat
-src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/i2b2 Portion Template/code/i2b2_dump.py
-src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/i2b2 Portion Template/data/input/.deleteme
-src/drapi/templates/Portions Templates/Multi-Portion Template/Intermediate Results/i2b2 Portion Template/data/output/.deleteme
-src/drapi/templates/scripts/Argparse Template - with SQL.py
+src/drapi/templates/makeDirTemplate/__init__.py
+src/drapi/templates/makeDirTemplate/Anaconda Environment Variables/RenameMe environment-name/README.md
+src/drapi/templates/makeDirTemplate/MultiPortion Template/.gitignore
+src/drapi/templates/makeDirTemplate/MultiPortion Template/README.md
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/.env
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/.gitignore
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/README.md
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/launchIPython.bat
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/aliasVariables.py
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/common.py
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/concatenateMaps.py
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/convertColumns.py
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/dataQualityTest.py
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/deIdentify.py
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/deIdentifyByAge.py
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/deIdentifyDates.py
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/deleteByColumnValues.py
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/deleteColumns.py
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/gatherFiles.py
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/getIDValues.py
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/getProjectColumns.py
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/i2b2ConvertIDs.py
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/i2b2GetIDs.py
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/i2b2MakeMap.py
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/makeAgeMap.py
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/makeDateShiftMap.py
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/makeMapsFromOthers.py
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/makeMapsFromScratch.py
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Concatenated Results/code/makePersonIDMap.py
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/.env
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/.gitignore
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/README.md
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/launchIPython.bat
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/code/functions.py
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/code/getData.py
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/data/input/.deleteme
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/BO Portion Template/data/output/.deleteme
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/.env
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/.gitignore
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/README.md
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/launchIPython.bat
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/code/RenameMe.py
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/code/compareGroupsTemplate.py
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/code/loopTemplate.py
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/data/input/.deleteme
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/General Script Template/data/output/.deleteme
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/.env
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/.gitignore
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/README.md
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/launchIPython.bat
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/code/filterNotes.py
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/code/freeText.py
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/data/input/.deleteme
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/data/output/.deleteme
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/sql/note_metadata.sql
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/sql/note_text.sql
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/sql/order_impression_metadata.sql
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/sql/order_impression_text.sql
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/sql/order_narrative_metadata.sql
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/sql/order_narrative_text.sql
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/sql/order_result_comment_metadata.sql
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Notes Portion Template/sql/order_result_comment_text.sql
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/.env
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/.gitignore
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/Config1.yml
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/README-INSTALLATION.md
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/README.md
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/launchIPython.bat
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/README Images/glDownloadButton.png
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/README Images/glDownloadDirectory.png
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/code/Project1.py
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/code/deidentify.py
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/code/getPersonIDs.py
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/data/input/.deleteme
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/data/output/.deleteme
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/OMOP Portion Template/sql/grabPersonIDs.SQL
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Portion 1/README.md
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/Portion 2/README.md
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/.env
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/.gitignore
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/README.md
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/launchIPython.bat
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/code/i2b2_dump.py
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/data/input/.deleteme
+src/drapi/templates/makeDirTemplate/MultiPortion Template/Intermediate Results/i2b2 Portion Template/data/output/.deleteme
 src/drapi/templates/scripts/hippaDisclosure.py
 src/drapi/templates/scripts/sqlQuery.py
 src/drapi_lemur.egg-info/PKG-INFO
 src/drapi_lemur.egg-info/SOURCES.txt
 src/drapi_lemur.egg-info/dependency_links.txt
-src/drapi_lemur.egg-info/top_level.txt
-src/scripts/checkC2S.py
-src/scripts/convertColumnsHash.py
-src/scripts/expandColumns.py
-src/scripts/getData.py
-src/scripts/getIDSets.py
-src/scripts/makeDirTemplate.py
-src/scripts/makeSymlink
-src/scripts/mapOF2IDR_deid2deid.py
-src/scripts/mapOF2IDR_id2id.py
-src/scripts/map_deid2deid.py
-src/scripts/prepTSVforSDOH.py
-src/scripts/prepTSVforSDOH2.py
-src/scripts/qaColumnConversion.py
-src/scripts/qaDeidentification.py
-src/scripts/replaceText.py
-src/scripts/tree.py
+src/drapi_lemur.egg-info/top_level.txt
```

### Comparing `drapi_lemur-1.0.40/src/scripts/checkC2S.py` & `drapi-lemur-1.0.5/src/drapi/code/drapi/c2s/checkC2S.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import argparse
 import sys
 # Third-party packages
 import pandas as pd
 from pathlib import Path
 # Local packages
-from drapi.code.drapi.c2s.c2s import checkStatus, doCheck
+from c2s import checkStatus, doCheck
 
 
 def checkStatusWrapper(fpath: str, columnName: str, statusType: str, location: str, verbosity):
     """
     """
     fpath
     data = pd.read_csv(fpath)
```

### Comparing `drapi_lemur-1.0.40/src/scripts/makeDirTemplate.py` & `drapi-lemur-1.0.5/src/makeDirTemplate.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,63 +4,62 @@
 New Directory
 ├── code
 ├── data
 │   ├── input
 │   └── output
 ├── logs
 ├── sql
+├── .env
 ├── .gitignore
 └── README.md
 
 where "New Directory" is the name of the directory to be created
 """
 
 import argparse
 import json
 import os
 import sys
 import shutil
 from pathlib import Path
-# First-party imports
-from drapi.templates import PATH as templatesPath
+# Local imports
+from drapi.templates.makeDirTemplate import PATH as makeDirTemplatePath
 
 
 def win2nixPath(string: str) -> str:
     """
     Converts a Windows-like path to a Linux-like path by changing the path separators.
     """
     platform = sys.platform
     platformSeparator = os.sep
     if platform == "darwin":
         newString = platformSeparator.join(string.split("\\"))
-    elif platform == "linux":
-        newString = platformSeparator.join(string.split("\\"))
     elif platform == "win32":
         newString = string
     else:
         raise Exception(f"""Unsupported operating system: "{platform}".""")
     return newString
 
 
-ROOT_PATH = templatesPath.joinpath("Portions Templates").__str__()
+ROOT_PATH = makeDirTemplatePath.__str__()
 # NOTE `optionsDict` expects `"path"` values to be in Windows format because it's later used by `win2nixPath`
 optionsDict = {"BO": {"number": 2,
-                      "path": r"\Multi-Portion Template\Intermediate Results\BO Portion Template"},
+                      "path": r"\MultiPortion Template\Intermediate Results\BO Portion Template"},
                "De-identification Suite": {"number": 1,
-                                           "path": r"\Multi-Portion Template\Concatenated Results"},
+                                           "path": r"\MultiPortion Template\Concatenated Results"},
                "General Script": {"number": 3,
-                                  "path": r"\Multi-Portion Template\Intermediate Results\General Script Template"},
+                                  "path": r"\Intermediate Results\General Script Template"},
                "i2b2": {"number": 4,
-                        "path": r"\Multi-Portion Template\Intermediate Results\i2b2 Portion Template"},
+                        "path": r"\MultiPortion Template\Intermediate Results\i2b2 Portion Template"},
                "Multi-Portion Template": {"number": 0,
-                                          "path": r"\Multi-Portion Template"},
-               "Clinical Text": {"number": 5,
-                         "path": r"\Multi-Portion Template\Intermediate Results\Clinical Text Portion Template"},
+                                          "path": r"\MultiPortion Template"},
+               "Notes": {"number": 5,
+                         "path": r"\MultiPortion Template\Intermediate Results\Notes Portion Template"},
                "OMOP": {"number": 6,
-                        "path": r"\Multi-Portion Template\Intermediate Results\OMOP Portion Template"}}
+                        "path": r"\MultiPortion Template\Intermediate Results\OMOP Portion Template"}}
 
 optionsDict2 = {values["number"]: {"name": name,
                                    "path": ROOT_PATH + win2nixPath(values["path"])} for name, values in optionsDict.items()}
 
 optionsNumbers = {name: value for name, values in optionsDict.items() for key, value in values.items() if key == "number"}
 
 
@@ -78,14 +77,15 @@
     # Prepare template for use
     for fpath in Path(destinationPath).glob("./**/*.*"):
         # Remove placeholder files
         if fpath.name.lower() == ".deleteme":
             os.remove(fpath)
         # Modify ".gitignore"
         if fpath.name.lower() == ".gitignore":
+            print(fpath)
             with open(fpath, "r") as file:
                 text = file.read()
                 text = text.replace("!**/launchIPython.bat\n", "")
                 text = text.replace("!.env", ".env")
                 text = text.replace("!data/input/\n", "")
                 text = text.replace("!data/output/\n", "")
             with open(fpath, "w") as file:
@@ -93,20 +93,16 @@
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
 
     parser.add_argument("templateChoice", help=f"""The template you wish to copy. Each template has a numerical option: {json.dumps(optionsNumbers)}""", choices=sorted(list(optionsDict2.keys())), type=int)
 
-    parser.add_argument("destinationPath", help="The directory path for `templateChoice`.", type=str)
+    parser.add_argument("destinationPath", help="", type=str)
 
     args = parser.parse_args()
 
     templateChoice = args.templateChoice
     destinationPath = args.destinationPath
 
-    try:
-        copyTemplateDirectory(templateChoice=templateChoice,
-                              destinationPath=destinationPath)
-    except Exception as err:
-        shutil.rmtree(destinationPath)
-        raise err
+    copyTemplateDirectory(templateChoice=templateChoice,
+                          destinationPath=destinationPath)
```

