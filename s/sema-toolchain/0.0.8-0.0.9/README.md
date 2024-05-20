# Comparing `tmp/sema_toolchain-0.0.8.tar.gz` & `tmp/sema_toolchain-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sema_toolchain-0.0.8.tar", last modified: Sun May 19 22:37:06 2024, max compression
+gzip compressed data, was "sema_toolchain-0.0.9.tar", last modified: Mon May 20 09:06:34 2024, max compression
```

## Comparing `sema_toolchain-0.0.8.tar` & `sema_toolchain-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 manon     (1000) manon     (1000)        0 2024-05-19 22:37:06.810842 sema_toolchain-0.0.8/
--rw-rw-r--   0 manon     (1000) manon     (1000)     1332 2024-04-16 10:03:35.000000 sema_toolchain-0.0.8/LICENSE
--rw-r--r--   0 manon     (1000) manon     (1000)    19381 2024-05-19 22:37:06.810842 sema_toolchain-0.0.8/PKG-INFO
-drwxrwxr-x   0 manon     (1000) manon     (1000)        0 2024-05-19 22:37:06.806842 sema_toolchain-0.0.8/doc/
--rw-rw-r--   0 manon     (1000) manon     (1000)    16116 2024-05-19 20:36:35.000000 sema_toolchain-0.0.8/doc/README.md
--rw-rw-r--   0 manon     (1000) manon     (1000)     1491 2024-05-19 22:37:01.000000 sema_toolchain-0.0.8/pyproject.toml
-drwxrwxr-x   0 manon     (1000) manon     (1000)        0 2024-05-19 22:37:06.810842 sema_toolchain-0.0.8/sema_toolchain.egg-info/
--rw-r--r--   0 manon     (1000) manon     (1000)    19381 2024-05-19 22:37:06.000000 sema_toolchain-0.0.8/sema_toolchain.egg-info/PKG-INFO
--rw-rw-r--   0 manon     (1000) manon     (1000)      225 2024-05-19 22:37:06.000000 sema_toolchain-0.0.8/sema_toolchain.egg-info/SOURCES.txt
--rw-rw-r--   0 manon     (1000) manon     (1000)        1 2024-05-19 22:37:06.000000 sema_toolchain-0.0.8/sema_toolchain.egg-info/dependency_links.txt
--rw-rw-r--   0 manon     (1000) manon     (1000)      532 2024-05-19 22:37:06.000000 sema_toolchain-0.0.8/sema_toolchain.egg-info/requires.txt
--rw-rw-r--   0 manon     (1000) manon     (1000)        1 2024-05-19 22:37:06.000000 sema_toolchain-0.0.8/sema_toolchain.egg-info/top_level.txt
--rw-rw-r--   0 manon     (1000) manon     (1000)       38 2024-05-19 22:37:06.810842 sema_toolchain-0.0.8/setup.cfg
+drwxrwxr-x   0 manon     (1000) manon     (1000)        0 2024-05-20 09:06:34.520099 sema_toolchain-0.0.9/
+-rw-rw-r--   0 manon     (1000) manon     (1000)     1332 2024-04-16 10:03:35.000000 sema_toolchain-0.0.9/LICENSE
+-rw-r--r--   0 manon     (1000) manon     (1000)    19777 2024-05-20 09:06:34.516100 sema_toolchain-0.0.9/PKG-INFO
+drwxrwxr-x   0 manon     (1000) manon     (1000)        0 2024-05-20 09:06:34.516100 sema_toolchain-0.0.9/doc/
+-rw-rw-r--   0 manon     (1000) manon     (1000)    16512 2024-05-20 08:52:38.000000 sema_toolchain-0.0.9/doc/README.md
+-rw-rw-r--   0 manon     (1000) manon     (1000)     1491 2024-05-20 09:06:29.000000 sema_toolchain-0.0.9/pyproject.toml
+drwxrwxr-x   0 manon     (1000) manon     (1000)        0 2024-05-20 09:06:34.516100 sema_toolchain-0.0.9/sema_toolchain.egg-info/
+-rw-r--r--   0 manon     (1000) manon     (1000)    19777 2024-05-20 09:06:34.000000 sema_toolchain-0.0.9/sema_toolchain.egg-info/PKG-INFO
+-rw-rw-r--   0 manon     (1000) manon     (1000)      225 2024-05-20 09:06:34.000000 sema_toolchain-0.0.9/sema_toolchain.egg-info/SOURCES.txt
+-rw-rw-r--   0 manon     (1000) manon     (1000)        1 2024-05-20 09:06:34.000000 sema_toolchain-0.0.9/sema_toolchain.egg-info/dependency_links.txt
+-rw-rw-r--   0 manon     (1000) manon     (1000)      532 2024-05-20 09:06:34.000000 sema_toolchain-0.0.9/sema_toolchain.egg-info/requires.txt
+-rw-rw-r--   0 manon     (1000) manon     (1000)        1 2024-05-20 09:06:34.000000 sema_toolchain-0.0.9/sema_toolchain.egg-info/top_level.txt
+-rw-rw-r--   0 manon     (1000) manon     (1000)       38 2024-05-20 09:06:34.520099 sema_toolchain-0.0.9/setup.cfg
```

### Comparing `sema_toolchain-0.0.8/LICENSE` & `sema_toolchain-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sema_toolchain-0.0.8/PKG-INFO` & `sema_toolchain-0.0.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sema_toolchain
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python symbolic execution package
 Author-email: Manon-Oreins <manon.oreins@gmail.com>
 License: BSD 2-Clause License
         
         Copyright (c) 2022, UCL-Cybersecurity team
         All rights reserved.
         
@@ -98,42 +98,42 @@
 ░ ░▒  ░ ░ ░ ░  ░░  ░      ░  ▒   ▒▒ ░
 ░  ░  ░     ░   ░      ░     ░   ▒
       ░     ░  ░       ░         ░  ░
 
 ```
 
 
-# :books:  Documentation
-
-1. [ Architecture ](#page_with_curl-architecture)
-    1. [ Toolchain architecture ](#toolchain-architecture)
-
-2. [ Recommended installation and usage ](#page_with_curl-recommended-installation-and-usage)
-
-3. [ Dockerhub installation and usage ](#page_with_curl-dockerhub-installation-and-usage)
-
-4. [ Pypi installation and usage ](#page_with_curl-Pypi-installation-and-usage)
-
-5. [ Credentials ](#page_with_curl-credentials)
+# Table of Contents
+1. [Architecture](#architecture)
+    - [Toolchain Architecture](#toolchain-architecture)
+2. [Recommended Installation and Usage](#page_with_curl-recommended-installation-and-usage)
+3. [Dockerhub Installation and Usage](#page_with_curl-dockerhub-installation)
+4. [Pypi Installation and Usage](#page_with_curl-pypi-installation-and-usage)
+5. [Credentials](#page_with_curl-credentials)
 
 :page_with_curl: Architecture
 ====
-<a name="arch"></a>
+<a name="architecture"></a>
 
 ### Toolchain architecture
-<a name="arch_std"></a>
+<a name="toolchain-architecture"></a>
 
-Our toolchain is represented in the next figure  and works as follow. A collection of labelled binaries of different malwares families is collected and used as the input of the toolchain. **Angr**, a framework for symbolic execution, is used to execute symbolically binaries and extract execution traces. For this purpose, different heuristics have been developped to optimize symbolic execution. Several execution traces (i.e : API calls used and their arguments) corresponding to one binary are extracted with Angr and gather together thanks to several graph heuristics to construct a SCDG. These resulting SCDGs are then used as input to graph mining to extract common graph between SCDG of the same family and create a signature. Finally when a new sample has to be classified, its SCDG is build and compared with SCDG of known families (thanks to a simple similarity metric).
+Our toolchain is represented in the following figure and works as follows:
 
-![GitHub Logo](./images/SEMA_illustration.png)
+- A collection of labelled binaries from different malware families is collected and used as the input of the toolchain.
+- **Angr**, a framework for symbolic execution, is used to execute binaries symbolically and extract execution traces. For this purpose, different heuristics have been developed to optimize symbolic execution.
+- Several execution traces (i.e., API calls used and their arguments) corresponding to one binary are extracted with Angr and gathered together using several graph heuristics to construct a SCDG.
+- These resulting SCDGs are then used as input to graph mining to extract common graphs between SCDGs of the same family and create a signature.
+- Finally, when a new sample has to be classified, its SCDG is built and compared with SCDGs of known families using a simple similarity metric.
 
-This repository contains a first version of a SCDG extractor.
-During symbolic analysis of a binary, all system calls and their arguments found are recorded. After some stop conditions for symbolic analysis, a graph is build as follow : Nodes are systems Calls recorded, edges show that some arguments are shared between calls.
+![Toolchain Illustration](./images/SEMA_illustration.png)
 
-When a new sample has to be evaluated, its SCDG is first build as described previously. Then, `gspan` is applied to extract the biggest common subgraph and a similarity score is evaluated to decide if the graph is considered as part of the family or not. The similarity score `S` between graph `G'` and `G''` is computed as follow:
+This repository contains a first version of a SCDG extractor. During the symbolic analysis of a binary, all system calls and their arguments found are recorded. After some stop conditions for symbolic analysis, a graph is built as follows: Nodes are system calls recorded, edges show that some arguments are shared between calls.
+
+When a new sample has to be evaluated, its SCDG is first built as described previously. Then, `gspan` is applied to extract the biggest common subgraph and a similarity score is evaluated to decide if the graph is considered as part of the family or not. The similarity score `S` between graph `G'` and `G''` is computed as follows:
 Since `G''` is a subgraph of `G'`, this is calculating how much `G'` appears in `G''`.
 Another classifier we use is the Support Vector Machine (`SVM`) with INRIA graph kernel or the Weisfeiler-Lehman extension graph kernel.
 
 A web application is available and is called SemaWebApp. It allows to manage the launch of experiments on SemaSCDG and/or SemaClassifier.
 
 #### Main depencies:
 
@@ -143,41 +143,44 @@
 
     * radare2
 
     * libvirt-dev, libgraphviz-dev, wheel
 
 #### Interesting links
 
-* https://angr.io/
-
-* https://bazaar.abuse.ch/
 
-* https://docs.docker.com/engine/install/ubuntu/
+- [Angr](https://angr.io/)
+- [Bazaar Abuse](https://bazaar.abuse.ch/)
+- [Docker Installation on Ubuntu](https://docs.docker.com/engine/install/ubuntu/)
 
 
-#### For extracting database
+#### Extracting database
 
+To extract the database, use the following commands:
 ```bash
-cd databases/Binaries; bash extract_deploy_db.sh
+cd databases/Binaries
+./extract_deploy_db.sh
 ```
 
 Password for archive is "infected". Warning : it contains real samples of malwares.
 
-#### For compressing database
+#### Compressing database
 
+To compress the database, use the following commands:
 ```bash
 #To zip back the test database
-cd databases/Binaries; bash compress_db.sh
+cd databases/Binaries
+./compress_db.sh
 ```
 
 :page_with_curl: **Recommended installation and usage**
 ====
-<a name="install"></a>
+<a name="recommended-installation-and-usage"></a>
 
-Install the entire toolchain
+To install the entire toolchain, use the following command:
 
 ```bash
 # Full installation (ubuntu)
 make build-toolchain;
 ```
 
 ## How to use ?
@@ -185,19 +188,17 @@
 ### Using the web application
 
 First launch the containers :
 ```bash
 make run-toolchain
 ```
 
-It will start the scdg, the classifier and the web app services. If you wish to use only the scdg or only the classifier, refer to the next sections.
-
-Wait for the containers to be up
+This will start the SCDG, the classifier, and the web app services. If you wish to use only the SCDG or only the classifier, refer to the specific sections below.
 
-Then visit 127.0.0.1:5000 on your browser
+Wait for the containers to be up, then visit 127.0.0.1:5000 on your browser
 
 See next sections for details about the different parameters.
 
 #### Shut down
 
 To leave the toolchain just press Ctrl+C then use
 ```bash
@@ -211,42 +212,38 @@
 docker rmi sema-web-app
 docker rmi sema-scdg
 docker rmi sema-classifier
 ```
 
 ### Use only SemaSCDG
 
-First run the SCDG container with volumes like this :
+To use only the SemaSCDG, first run the SCDG container with volumes like this:
 ```bash
 docker run --rm --name="sema-scdg" -v ${PWD}/OutputFolder:/sema-scdg/application/database/SCDG -v ${PWD}/ConfigFolder:/sema-scdg/application/configs -v ${PWD}/InputFolder:/sema-scdg/application/database/Binaries  -it sema-scdg bash
 ```
-Where the first volume corresponds to the output folder where the results will be put. The second volume corresponds to the folder containing the configuration files that will be passed to the docker. And the third matches the folder containing the binaries that are going to be passed to the container.
+In this command:
 
-Inside the container just run  :
+- The first volume corresponds to the output folder where the results will be put.
+- The second volume corresponds to the folder containing the configuration files that will be passed to the docker.
+- The third matches the folder containing the binaries that are going to be passed to the container.
+
+To run experiments, run inside the container :
 ```bash
 python3 SemaSCDG.py configs/config.ini
 ```
 Or if you want to use pypy3:
 ```bash
 pypy3 SemaSCDG.py configs/config.ini
 ```
 
 #### Configuration files
 
-The parameters are put in a configuration file : `configs/config.ini`
-Feel free to modify it or create new configuration files to run different experiments.
+The parameters are put in a configuration file : `configs/config.ini`. Feel free to modify it or create new configuration files to run different experiments.
 
-To restore the default values of `config.ini` do :
-```bash
-python3 restore_defaults.py
-```
-The default parameters are stored in the file `default_config.ini`
-Do not modify `config_tutorial.ini` and `config_test.ini` as they are designed to fit the Tutorial and the tests needs respectively.
-
-The output of the SCDG are put into `database/SCDG/runs/` by default. If you are not using volumes and want to save some runs from the container to your host machine :
+The output of the SCDG are put into `database/SCDG/runs/` by default. If you are not using volumes and want to save some runs from the container to your host machine, use :
 ```bash
 make save-scdg-runs ARGS=PATH
 ```
 
 #### Parameters description
 SCDG module arguments
 
@@ -327,22 +324,22 @@
 
 If you wish to run multiple experiments with different configuration files, the script `multiple_experiments.sh` is available and can be used inside the scdg container:
 ```bash
 # To show usage
 ./multiple_experiments.sh -h
 
 # Run example
-./multiple_experiments.sh -m python3 -c configs/config configs/default_configs
+./multiple_experiments.sh -m python3 -c configs/config1 configs/config2
 ```
 
 #### Tests
 
 To run the test, inside the docker container :
 ```bash
-python3 scdg_tests.py configs/config_test.ini
+python3 scdg_tests.py test_data/config_test.ini
 ```
 
 #### Tutorial
 
 There is a jupyter notebook providing a tutorial on how to use the scdg. To launch it, inside the docker, run
 ```bash
 jupyter notebook --ip=0.0.0.0 --port=5001 --no-browser --allow-root --NotebookApp.token=''
@@ -429,29 +426,28 @@
 This will train models for input dataset
 
 ```bash
 python3 SemaClassifier.py --train output/save-SCDG/
 ```
 
 This will classify input dataset based on previously computed models
-
 ```bash
 python3 SemaClassifier.py output/test-set/
 ```
 
 #### Tests
 
 To run the classifier tests, run inside the docker container:
 ```bash
 python3 classifier_tests.py configs/config_test.ini
 ```
 
 :page_with_curl: **Dockerhub installation**
 ====
-<a name="dockerhub"></a>
+<a name="dockerhub-installation-and-usage"></a>
 
 ## SemaSCDG
 
 If you only need the SCDG part of the toolchain you can use :
 ```bash
 make pull-scdg
 ```
@@ -467,22 +463,28 @@
 ```
 To pull the docker image directly from dockerHub. Or visit `https://hub.docker.com/repository/docker/manonoreins/sema-classifier/tags`
 
 Then use the same commands than in the recommended usage section
 
 :page_with_curl: **Pypi installation and usage**
 ====
-<a name="pypi"></a>
+<a name="pypi-installation-and-usage"></a>
 
-If you wish to install the toolchain python dependencies on your system, use :
+It is also possible to use the toolchain without docker container by using the Pypi package to install dependencies.
 
 ```bash
 pip install sema-toolchain
 ```
 
+After cloning the git you can then use the toolchain without docker
+Example :
+```bash
+python3 sema_scdg/application/SemaSCDG.py sema_scdg/application/configs/config.ini 
+```
+
 #### Pypy3 usage
 
 By default, pypy3 can be used to launch experiments inside the SCDG's docker container. If you wish to use it outside the container, make sure to install pypy3 :
 
 ```bash
 sudo add-apt-repository ppa:pypy/ppa
 sudo apt update
@@ -491,17 +493,22 @@
 
 Then install the dependecies on pypy3 :
 
 ```bash
 pypy3 -m pip install -r /sema_scdg/requirements_pypy.txt
 ```
 
+Then use pypy3 instead of python3 to launch experiments:
+```bash
+pypy3 sema_scdg/application/SemaSCDG.py sema_scdg/application/configs/config.ini 
+```
+
 :page_with_curl: Credentials
 ====
-<a name="credit"></a>
+<a name="credentials"></a>
 
 Main authors of the projects:
 
 * **Charles-Henry Bertrand Van Ouytsel** (UCLouvain)
 
 * **Christophe Crochet** (UCLouvain)
```

### Comparing `sema_toolchain-0.0.8/doc/README.md` & `sema_toolchain-0.0.9/doc/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -10,42 +10,42 @@
 ░ ░▒  ░ ░ ░ ░  ░░  ░      ░  ▒   ▒▒ ░
 ░  ░  ░     ░   ░      ░     ░   ▒
       ░     ░  ░       ░         ░  ░
 
 ```
 
 
-# :books:  Documentation
-
-1. [ Architecture ](#page_with_curl-architecture)
-    1. [ Toolchain architecture ](#toolchain-architecture)
-
-2. [ Recommended installation and usage ](#page_with_curl-recommended-installation-and-usage)
-
-3. [ Dockerhub installation and usage ](#page_with_curl-dockerhub-installation-and-usage)
-
-4. [ Pypi installation and usage ](#page_with_curl-Pypi-installation-and-usage)
-
-5. [ Credentials ](#page_with_curl-credentials)
+# Table of Contents
+1. [Architecture](#architecture)
+    - [Toolchain Architecture](#toolchain-architecture)
+2. [Recommended Installation and Usage](#page_with_curl-recommended-installation-and-usage)
+3. [Dockerhub Installation and Usage](#page_with_curl-dockerhub-installation)
+4. [Pypi Installation and Usage](#page_with_curl-pypi-installation-and-usage)
+5. [Credentials](#page_with_curl-credentials)
 
 :page_with_curl: Architecture
 ====
-<a name="arch"></a>
+<a name="architecture"></a>
 
 ### Toolchain architecture
-<a name="arch_std"></a>
+<a name="toolchain-architecture"></a>
 
-Our toolchain is represented in the next figure  and works as follow. A collection of labelled binaries of different malwares families is collected and used as the input of the toolchain. **Angr**, a framework for symbolic execution, is used to execute symbolically binaries and extract execution traces. For this purpose, different heuristics have been developped to optimize symbolic execution. Several execution traces (i.e : API calls used and their arguments) corresponding to one binary are extracted with Angr and gather together thanks to several graph heuristics to construct a SCDG. These resulting SCDGs are then used as input to graph mining to extract common graph between SCDG of the same family and create a signature. Finally when a new sample has to be classified, its SCDG is build and compared with SCDG of known families (thanks to a simple similarity metric).
+Our toolchain is represented in the following figure and works as follows:
 
-![GitHub Logo](./images/SEMA_illustration.png)
+- A collection of labelled binaries from different malware families is collected and used as the input of the toolchain.
+- **Angr**, a framework for symbolic execution, is used to execute binaries symbolically and extract execution traces. For this purpose, different heuristics have been developed to optimize symbolic execution.
+- Several execution traces (i.e., API calls used and their arguments) corresponding to one binary are extracted with Angr and gathered together using several graph heuristics to construct a SCDG.
+- These resulting SCDGs are then used as input to graph mining to extract common graphs between SCDGs of the same family and create a signature.
+- Finally, when a new sample has to be classified, its SCDG is built and compared with SCDGs of known families using a simple similarity metric.
 
-This repository contains a first version of a SCDG extractor.
-During symbolic analysis of a binary, all system calls and their arguments found are recorded. After some stop conditions for symbolic analysis, a graph is build as follow : Nodes are systems Calls recorded, edges show that some arguments are shared between calls.
+![Toolchain Illustration](./images/SEMA_illustration.png)
 
-When a new sample has to be evaluated, its SCDG is first build as described previously. Then, `gspan` is applied to extract the biggest common subgraph and a similarity score is evaluated to decide if the graph is considered as part of the family or not. The similarity score `S` between graph `G'` and `G''` is computed as follow:
+This repository contains a first version of a SCDG extractor. During the symbolic analysis of a binary, all system calls and their arguments found are recorded. After some stop conditions for symbolic analysis, a graph is built as follows: Nodes are system calls recorded, edges show that some arguments are shared between calls.
+
+When a new sample has to be evaluated, its SCDG is first built as described previously. Then, `gspan` is applied to extract the biggest common subgraph and a similarity score is evaluated to decide if the graph is considered as part of the family or not. The similarity score `S` between graph `G'` and `G''` is computed as follows:
 Since `G''` is a subgraph of `G'`, this is calculating how much `G'` appears in `G''`.
 Another classifier we use is the Support Vector Machine (`SVM`) with INRIA graph kernel or the Weisfeiler-Lehman extension graph kernel.
 
 A web application is available and is called SemaWebApp. It allows to manage the launch of experiments on SemaSCDG and/or SemaClassifier.
 
 #### Main depencies:
 
@@ -55,41 +55,44 @@
 
     * radare2
 
     * libvirt-dev, libgraphviz-dev, wheel
 
 #### Interesting links
 
-* https://angr.io/
-
-* https://bazaar.abuse.ch/
 
-* https://docs.docker.com/engine/install/ubuntu/
+- [Angr](https://angr.io/)
+- [Bazaar Abuse](https://bazaar.abuse.ch/)
+- [Docker Installation on Ubuntu](https://docs.docker.com/engine/install/ubuntu/)
 
 
-#### For extracting database
+#### Extracting database
 
+To extract the database, use the following commands:
 ```bash
-cd databases/Binaries; bash extract_deploy_db.sh
+cd databases/Binaries
+./extract_deploy_db.sh
 ```
 
 Password for archive is "infected". Warning : it contains real samples of malwares.
 
-#### For compressing database
+#### Compressing database
 
+To compress the database, use the following commands:
 ```bash
 #To zip back the test database
-cd databases/Binaries; bash compress_db.sh
+cd databases/Binaries
+./compress_db.sh
 ```
 
 :page_with_curl: **Recommended installation and usage**
 ====
-<a name="install"></a>
+<a name="recommended-installation-and-usage"></a>
 
-Install the entire toolchain
+To install the entire toolchain, use the following command:
 
 ```bash
 # Full installation (ubuntu)
 make build-toolchain;
 ```
 
 ## How to use ?
@@ -97,19 +100,17 @@
 ### Using the web application
 
 First launch the containers :
 ```bash
 make run-toolchain
 ```
 
-It will start the scdg, the classifier and the web app services. If you wish to use only the scdg or only the classifier, refer to the next sections.
-
-Wait for the containers to be up
+This will start the SCDG, the classifier, and the web app services. If you wish to use only the SCDG or only the classifier, refer to the specific sections below.
 
-Then visit 127.0.0.1:5000 on your browser
+Wait for the containers to be up, then visit 127.0.0.1:5000 on your browser
 
 See next sections for details about the different parameters.
 
 #### Shut down
 
 To leave the toolchain just press Ctrl+C then use
 ```bash
@@ -123,42 +124,38 @@
 docker rmi sema-web-app
 docker rmi sema-scdg
 docker rmi sema-classifier
 ```
 
 ### Use only SemaSCDG
 
-First run the SCDG container with volumes like this :
+To use only the SemaSCDG, first run the SCDG container with volumes like this:
 ```bash
 docker run --rm --name="sema-scdg" -v ${PWD}/OutputFolder:/sema-scdg/application/database/SCDG -v ${PWD}/ConfigFolder:/sema-scdg/application/configs -v ${PWD}/InputFolder:/sema-scdg/application/database/Binaries  -it sema-scdg bash
 ```
-Where the first volume corresponds to the output folder where the results will be put. The second volume corresponds to the folder containing the configuration files that will be passed to the docker. And the third matches the folder containing the binaries that are going to be passed to the container.
+In this command:
 
-Inside the container just run  :
+- The first volume corresponds to the output folder where the results will be put.
+- The second volume corresponds to the folder containing the configuration files that will be passed to the docker.
+- The third matches the folder containing the binaries that are going to be passed to the container.
+
+To run experiments, run inside the container :
 ```bash
 python3 SemaSCDG.py configs/config.ini
 ```
 Or if you want to use pypy3:
 ```bash
 pypy3 SemaSCDG.py configs/config.ini
 ```
 
 #### Configuration files
 
-The parameters are put in a configuration file : `configs/config.ini`
-Feel free to modify it or create new configuration files to run different experiments.
+The parameters are put in a configuration file : `configs/config.ini`. Feel free to modify it or create new configuration files to run different experiments.
 
-To restore the default values of `config.ini` do :
-```bash
-python3 restore_defaults.py
-```
-The default parameters are stored in the file `default_config.ini`
-Do not modify `config_tutorial.ini` and `config_test.ini` as they are designed to fit the Tutorial and the tests needs respectively.
-
-The output of the SCDG are put into `database/SCDG/runs/` by default. If you are not using volumes and want to save some runs from the container to your host machine :
+The output of the SCDG are put into `database/SCDG/runs/` by default. If you are not using volumes and want to save some runs from the container to your host machine, use :
 ```bash
 make save-scdg-runs ARGS=PATH
 ```
 
 #### Parameters description
 SCDG module arguments
 
@@ -239,22 +236,22 @@
 
 If you wish to run multiple experiments with different configuration files, the script `multiple_experiments.sh` is available and can be used inside the scdg container:
 ```bash
 # To show usage
 ./multiple_experiments.sh -h
 
 # Run example
-./multiple_experiments.sh -m python3 -c configs/config configs/default_configs
+./multiple_experiments.sh -m python3 -c configs/config1 configs/config2
 ```
 
 #### Tests
 
 To run the test, inside the docker container :
 ```bash
-python3 scdg_tests.py configs/config_test.ini
+python3 scdg_tests.py test_data/config_test.ini
 ```
 
 #### Tutorial
 
 There is a jupyter notebook providing a tutorial on how to use the scdg. To launch it, inside the docker, run
 ```bash
 jupyter notebook --ip=0.0.0.0 --port=5001 --no-browser --allow-root --NotebookApp.token=''
@@ -341,29 +338,28 @@
 This will train models for input dataset
 
 ```bash
 python3 SemaClassifier.py --train output/save-SCDG/
 ```
 
 This will classify input dataset based on previously computed models
-
 ```bash
 python3 SemaClassifier.py output/test-set/
 ```
 
 #### Tests
 
 To run the classifier tests, run inside the docker container:
 ```bash
 python3 classifier_tests.py configs/config_test.ini
 ```
 
 :page_with_curl: **Dockerhub installation**
 ====
-<a name="dockerhub"></a>
+<a name="dockerhub-installation-and-usage"></a>
 
 ## SemaSCDG
 
 If you only need the SCDG part of the toolchain you can use :
 ```bash
 make pull-scdg
 ```
@@ -379,22 +375,28 @@
 ```
 To pull the docker image directly from dockerHub. Or visit `https://hub.docker.com/repository/docker/manonoreins/sema-classifier/tags`
 
 Then use the same commands than in the recommended usage section
 
 :page_with_curl: **Pypi installation and usage**
 ====
-<a name="pypi"></a>
+<a name="pypi-installation-and-usage"></a>
 
-If you wish to install the toolchain python dependencies on your system, use :
+It is also possible to use the toolchain without docker container by using the Pypi package to install dependencies.
 
 ```bash
 pip install sema-toolchain
 ```
 
+After cloning the git you can then use the toolchain without docker
+Example :
+```bash
+python3 sema_scdg/application/SemaSCDG.py sema_scdg/application/configs/config.ini 
+```
+
 #### Pypy3 usage
 
 By default, pypy3 can be used to launch experiments inside the SCDG's docker container. If you wish to use it outside the container, make sure to install pypy3 :
 
 ```bash
 sudo add-apt-repository ppa:pypy/ppa
 sudo apt update
@@ -403,17 +405,22 @@
 
 Then install the dependecies on pypy3 :
 
 ```bash
 pypy3 -m pip install -r /sema_scdg/requirements_pypy.txt
 ```
 
+Then use pypy3 instead of python3 to launch experiments:
+```bash
+pypy3 sema_scdg/application/SemaSCDG.py sema_scdg/application/configs/config.ini 
+```
+
 :page_with_curl: Credentials
 ====
-<a name="credit"></a>
+<a name="credentials"></a>
 
 Main authors of the projects:
 
 * **Charles-Henry Bertrand Van Ouytsel** (UCLouvain)
 
 * **Christophe Crochet** (UCLouvain)
```

### Comparing `sema_toolchain-0.0.8/pyproject.toml` & `sema_toolchain-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=62.4", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sema_toolchain"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Manon-Oreins", email="manon.oreins@gmail.com" },
 ]
 description = "Python symbolic execution package"
 readme = "doc/README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `sema_toolchain-0.0.8/sema_toolchain.egg-info/PKG-INFO` & `sema_toolchain-0.0.9/sema_toolchain.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sema_toolchain
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python symbolic execution package
 Author-email: Manon-Oreins <manon.oreins@gmail.com>
 License: BSD 2-Clause License
         
         Copyright (c) 2022, UCL-Cybersecurity team
         All rights reserved.
         
@@ -98,42 +98,42 @@
 ░ ░▒  ░ ░ ░ ░  ░░  ░      ░  ▒   ▒▒ ░
 ░  ░  ░     ░   ░      ░     ░   ▒
       ░     ░  ░       ░         ░  ░
 
 ```
 
 
-# :books:  Documentation
-
-1. [ Architecture ](#page_with_curl-architecture)
-    1. [ Toolchain architecture ](#toolchain-architecture)
-
-2. [ Recommended installation and usage ](#page_with_curl-recommended-installation-and-usage)
-
-3. [ Dockerhub installation and usage ](#page_with_curl-dockerhub-installation-and-usage)
-
-4. [ Pypi installation and usage ](#page_with_curl-Pypi-installation-and-usage)
-
-5. [ Credentials ](#page_with_curl-credentials)
+# Table of Contents
+1. [Architecture](#architecture)
+    - [Toolchain Architecture](#toolchain-architecture)
+2. [Recommended Installation and Usage](#page_with_curl-recommended-installation-and-usage)
+3. [Dockerhub Installation and Usage](#page_with_curl-dockerhub-installation)
+4. [Pypi Installation and Usage](#page_with_curl-pypi-installation-and-usage)
+5. [Credentials](#page_with_curl-credentials)
 
 :page_with_curl: Architecture
 ====
-<a name="arch"></a>
+<a name="architecture"></a>
 
 ### Toolchain architecture
-<a name="arch_std"></a>
+<a name="toolchain-architecture"></a>
 
-Our toolchain is represented in the next figure  and works as follow. A collection of labelled binaries of different malwares families is collected and used as the input of the toolchain. **Angr**, a framework for symbolic execution, is used to execute symbolically binaries and extract execution traces. For this purpose, different heuristics have been developped to optimize symbolic execution. Several execution traces (i.e : API calls used and their arguments) corresponding to one binary are extracted with Angr and gather together thanks to several graph heuristics to construct a SCDG. These resulting SCDGs are then used as input to graph mining to extract common graph between SCDG of the same family and create a signature. Finally when a new sample has to be classified, its SCDG is build and compared with SCDG of known families (thanks to a simple similarity metric).
+Our toolchain is represented in the following figure and works as follows:
 
-![GitHub Logo](./images/SEMA_illustration.png)
+- A collection of labelled binaries from different malware families is collected and used as the input of the toolchain.
+- **Angr**, a framework for symbolic execution, is used to execute binaries symbolically and extract execution traces. For this purpose, different heuristics have been developed to optimize symbolic execution.
+- Several execution traces (i.e., API calls used and their arguments) corresponding to one binary are extracted with Angr and gathered together using several graph heuristics to construct a SCDG.
+- These resulting SCDGs are then used as input to graph mining to extract common graphs between SCDGs of the same family and create a signature.
+- Finally, when a new sample has to be classified, its SCDG is built and compared with SCDGs of known families using a simple similarity metric.
 
-This repository contains a first version of a SCDG extractor.
-During symbolic analysis of a binary, all system calls and their arguments found are recorded. After some stop conditions for symbolic analysis, a graph is build as follow : Nodes are systems Calls recorded, edges show that some arguments are shared between calls.
+![Toolchain Illustration](./images/SEMA_illustration.png)
 
-When a new sample has to be evaluated, its SCDG is first build as described previously. Then, `gspan` is applied to extract the biggest common subgraph and a similarity score is evaluated to decide if the graph is considered as part of the family or not. The similarity score `S` between graph `G'` and `G''` is computed as follow:
+This repository contains a first version of a SCDG extractor. During the symbolic analysis of a binary, all system calls and their arguments found are recorded. After some stop conditions for symbolic analysis, a graph is built as follows: Nodes are system calls recorded, edges show that some arguments are shared between calls.
+
+When a new sample has to be evaluated, its SCDG is first built as described previously. Then, `gspan` is applied to extract the biggest common subgraph and a similarity score is evaluated to decide if the graph is considered as part of the family or not. The similarity score `S` between graph `G'` and `G''` is computed as follows:
 Since `G''` is a subgraph of `G'`, this is calculating how much `G'` appears in `G''`.
 Another classifier we use is the Support Vector Machine (`SVM`) with INRIA graph kernel or the Weisfeiler-Lehman extension graph kernel.
 
 A web application is available and is called SemaWebApp. It allows to manage the launch of experiments on SemaSCDG and/or SemaClassifier.
 
 #### Main depencies:
 
@@ -143,41 +143,44 @@
 
     * radare2
 
     * libvirt-dev, libgraphviz-dev, wheel
 
 #### Interesting links
 
-* https://angr.io/
-
-* https://bazaar.abuse.ch/
 
-* https://docs.docker.com/engine/install/ubuntu/
+- [Angr](https://angr.io/)
+- [Bazaar Abuse](https://bazaar.abuse.ch/)
+- [Docker Installation on Ubuntu](https://docs.docker.com/engine/install/ubuntu/)
 
 
-#### For extracting database
+#### Extracting database
 
+To extract the database, use the following commands:
 ```bash
-cd databases/Binaries; bash extract_deploy_db.sh
+cd databases/Binaries
+./extract_deploy_db.sh
 ```
 
 Password for archive is "infected". Warning : it contains real samples of malwares.
 
-#### For compressing database
+#### Compressing database
 
+To compress the database, use the following commands:
 ```bash
 #To zip back the test database
-cd databases/Binaries; bash compress_db.sh
+cd databases/Binaries
+./compress_db.sh
 ```
 
 :page_with_curl: **Recommended installation and usage**
 ====
-<a name="install"></a>
+<a name="recommended-installation-and-usage"></a>
 
-Install the entire toolchain
+To install the entire toolchain, use the following command:
 
 ```bash
 # Full installation (ubuntu)
 make build-toolchain;
 ```
 
 ## How to use ?
@@ -185,19 +188,17 @@
 ### Using the web application
 
 First launch the containers :
 ```bash
 make run-toolchain
 ```
 
-It will start the scdg, the classifier and the web app services. If you wish to use only the scdg or only the classifier, refer to the next sections.
-
-Wait for the containers to be up
+This will start the SCDG, the classifier, and the web app services. If you wish to use only the SCDG or only the classifier, refer to the specific sections below.
 
-Then visit 127.0.0.1:5000 on your browser
+Wait for the containers to be up, then visit 127.0.0.1:5000 on your browser
 
 See next sections for details about the different parameters.
 
 #### Shut down
 
 To leave the toolchain just press Ctrl+C then use
 ```bash
@@ -211,42 +212,38 @@
 docker rmi sema-web-app
 docker rmi sema-scdg
 docker rmi sema-classifier
 ```
 
 ### Use only SemaSCDG
 
-First run the SCDG container with volumes like this :
+To use only the SemaSCDG, first run the SCDG container with volumes like this:
 ```bash
 docker run --rm --name="sema-scdg" -v ${PWD}/OutputFolder:/sema-scdg/application/database/SCDG -v ${PWD}/ConfigFolder:/sema-scdg/application/configs -v ${PWD}/InputFolder:/sema-scdg/application/database/Binaries  -it sema-scdg bash
 ```
-Where the first volume corresponds to the output folder where the results will be put. The second volume corresponds to the folder containing the configuration files that will be passed to the docker. And the third matches the folder containing the binaries that are going to be passed to the container.
+In this command:
 
-Inside the container just run  :
+- The first volume corresponds to the output folder where the results will be put.
+- The second volume corresponds to the folder containing the configuration files that will be passed to the docker.
+- The third matches the folder containing the binaries that are going to be passed to the container.
+
+To run experiments, run inside the container :
 ```bash
 python3 SemaSCDG.py configs/config.ini
 ```
 Or if you want to use pypy3:
 ```bash
 pypy3 SemaSCDG.py configs/config.ini
 ```
 
 #### Configuration files
 
-The parameters are put in a configuration file : `configs/config.ini`
-Feel free to modify it or create new configuration files to run different experiments.
+The parameters are put in a configuration file : `configs/config.ini`. Feel free to modify it or create new configuration files to run different experiments.
 
-To restore the default values of `config.ini` do :
-```bash
-python3 restore_defaults.py
-```
-The default parameters are stored in the file `default_config.ini`
-Do not modify `config_tutorial.ini` and `config_test.ini` as they are designed to fit the Tutorial and the tests needs respectively.
-
-The output of the SCDG are put into `database/SCDG/runs/` by default. If you are not using volumes and want to save some runs from the container to your host machine :
+The output of the SCDG are put into `database/SCDG/runs/` by default. If you are not using volumes and want to save some runs from the container to your host machine, use :
 ```bash
 make save-scdg-runs ARGS=PATH
 ```
 
 #### Parameters description
 SCDG module arguments
 
@@ -327,22 +324,22 @@
 
 If you wish to run multiple experiments with different configuration files, the script `multiple_experiments.sh` is available and can be used inside the scdg container:
 ```bash
 # To show usage
 ./multiple_experiments.sh -h
 
 # Run example
-./multiple_experiments.sh -m python3 -c configs/config configs/default_configs
+./multiple_experiments.sh -m python3 -c configs/config1 configs/config2
 ```
 
 #### Tests
 
 To run the test, inside the docker container :
 ```bash
-python3 scdg_tests.py configs/config_test.ini
+python3 scdg_tests.py test_data/config_test.ini
 ```
 
 #### Tutorial
 
 There is a jupyter notebook providing a tutorial on how to use the scdg. To launch it, inside the docker, run
 ```bash
 jupyter notebook --ip=0.0.0.0 --port=5001 --no-browser --allow-root --NotebookApp.token=''
@@ -429,29 +426,28 @@
 This will train models for input dataset
 
 ```bash
 python3 SemaClassifier.py --train output/save-SCDG/
 ```
 
 This will classify input dataset based on previously computed models
-
 ```bash
 python3 SemaClassifier.py output/test-set/
 ```
 
 #### Tests
 
 To run the classifier tests, run inside the docker container:
 ```bash
 python3 classifier_tests.py configs/config_test.ini
 ```
 
 :page_with_curl: **Dockerhub installation**
 ====
-<a name="dockerhub"></a>
+<a name="dockerhub-installation-and-usage"></a>
 
 ## SemaSCDG
 
 If you only need the SCDG part of the toolchain you can use :
 ```bash
 make pull-scdg
 ```
@@ -467,22 +463,28 @@
 ```
 To pull the docker image directly from dockerHub. Or visit `https://hub.docker.com/repository/docker/manonoreins/sema-classifier/tags`
 
 Then use the same commands than in the recommended usage section
 
 :page_with_curl: **Pypi installation and usage**
 ====
-<a name="pypi"></a>
+<a name="pypi-installation-and-usage"></a>
 
-If you wish to install the toolchain python dependencies on your system, use :
+It is also possible to use the toolchain without docker container by using the Pypi package to install dependencies.
 
 ```bash
 pip install sema-toolchain
 ```
 
+After cloning the git you can then use the toolchain without docker
+Example :
+```bash
+python3 sema_scdg/application/SemaSCDG.py sema_scdg/application/configs/config.ini 
+```
+
 #### Pypy3 usage
 
 By default, pypy3 can be used to launch experiments inside the SCDG's docker container. If you wish to use it outside the container, make sure to install pypy3 :
 
 ```bash
 sudo add-apt-repository ppa:pypy/ppa
 sudo apt update
@@ -491,17 +493,22 @@
 
 Then install the dependecies on pypy3 :
 
 ```bash
 pypy3 -m pip install -r /sema_scdg/requirements_pypy.txt
 ```
 
+Then use pypy3 instead of python3 to launch experiments:
+```bash
+pypy3 sema_scdg/application/SemaSCDG.py sema_scdg/application/configs/config.ini 
+```
+
 :page_with_curl: Credentials
 ====
-<a name="credit"></a>
+<a name="credentials"></a>
 
 Main authors of the projects:
 
 * **Charles-Henry Bertrand Van Ouytsel** (UCLouvain)
 
 * **Christophe Crochet** (UCLouvain)
```

### Comparing `sema_toolchain-0.0.8/sema_toolchain.egg-info/requires.txt` & `sema_toolchain-0.0.9/sema_toolchain.egg-info/requires.txt`

 * *Files identical despite different names*

