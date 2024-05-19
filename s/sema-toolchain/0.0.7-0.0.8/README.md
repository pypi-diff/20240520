# Comparing `tmp/sema_toolchain-0.0.7.tar.gz` & `tmp/sema_toolchain-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sema_toolchain-0.0.7.tar", last modified: Tue May  7 14:12:47 2024, max compression
+gzip compressed data, was "sema_toolchain-0.0.8.tar", last modified: Sun May 19 22:37:06 2024, max compression
```

## Comparing `sema_toolchain-0.0.7.tar` & `sema_toolchain-0.0.8.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxr-x   0 manon     (1000) manon     (1000)        0 2024-05-07 14:12:47.428660 sema_toolchain-0.0.7/
--rw-rw-r--   0 manon     (1000) manon     (1000)     1332 2024-04-16 10:03:35.000000 sema_toolchain-0.0.7/LICENSE
--rw-r--r--   0 manon     (1000) manon     (1000)    18083 2024-05-07 14:12:47.428660 sema_toolchain-0.0.7/PKG-INFO
--rw-rw-r--   0 manon     (1000) manon     (1000)    14818 2024-04-30 11:40:38.000000 sema_toolchain-0.0.7/README.md
--rw-rw-r--   0 manon     (1000) manon     (1000)     1561 2024-05-07 14:12:43.000000 sema_toolchain-0.0.7/pyproject.toml
-drwxrwxr-x   0 manon     (1000) manon     (1000)        0 2024-05-07 14:12:47.428660 sema_toolchain-0.0.7/sema_toolchain.egg-info/
--rw-r--r--   0 manon     (1000) manon     (1000)    18083 2024-05-07 14:12:47.000000 sema_toolchain-0.0.7/sema_toolchain.egg-info/PKG-INFO
--rw-rw-r--   0 manon     (1000) manon     (1000)      221 2024-05-07 14:12:47.000000 sema_toolchain-0.0.7/sema_toolchain.egg-info/SOURCES.txt
--rw-rw-r--   0 manon     (1000) manon     (1000)        1 2024-05-07 14:12:47.000000 sema_toolchain-0.0.7/sema_toolchain.egg-info/dependency_links.txt
--rw-rw-r--   0 manon     (1000) manon     (1000)      532 2024-05-07 14:12:47.000000 sema_toolchain-0.0.7/sema_toolchain.egg-info/requires.txt
--rw-rw-r--   0 manon     (1000) manon     (1000)       39 2024-05-07 14:12:47.000000 sema_toolchain-0.0.7/sema_toolchain.egg-info/top_level.txt
--rw-rw-r--   0 manon     (1000) manon     (1000)       38 2024-05-07 14:12:47.428660 sema_toolchain-0.0.7/setup.cfg
+drwxrwxr-x   0 manon     (1000) manon     (1000)        0 2024-05-19 22:37:06.810842 sema_toolchain-0.0.8/
+-rw-rw-r--   0 manon     (1000) manon     (1000)     1332 2024-04-16 10:03:35.000000 sema_toolchain-0.0.8/LICENSE
+-rw-r--r--   0 manon     (1000) manon     (1000)    19381 2024-05-19 22:37:06.810842 sema_toolchain-0.0.8/PKG-INFO
+drwxrwxr-x   0 manon     (1000) manon     (1000)        0 2024-05-19 22:37:06.806842 sema_toolchain-0.0.8/doc/
+-rw-rw-r--   0 manon     (1000) manon     (1000)    16116 2024-05-19 20:36:35.000000 sema_toolchain-0.0.8/doc/README.md
+-rw-rw-r--   0 manon     (1000) manon     (1000)     1491 2024-05-19 22:37:01.000000 sema_toolchain-0.0.8/pyproject.toml
+drwxrwxr-x   0 manon     (1000) manon     (1000)        0 2024-05-19 22:37:06.810842 sema_toolchain-0.0.8/sema_toolchain.egg-info/
+-rw-r--r--   0 manon     (1000) manon     (1000)    19381 2024-05-19 22:37:06.000000 sema_toolchain-0.0.8/sema_toolchain.egg-info/PKG-INFO
+-rw-rw-r--   0 manon     (1000) manon     (1000)      225 2024-05-19 22:37:06.000000 sema_toolchain-0.0.8/sema_toolchain.egg-info/SOURCES.txt
+-rw-rw-r--   0 manon     (1000) manon     (1000)        1 2024-05-19 22:37:06.000000 sema_toolchain-0.0.8/sema_toolchain.egg-info/dependency_links.txt
+-rw-rw-r--   0 manon     (1000) manon     (1000)      532 2024-05-19 22:37:06.000000 sema_toolchain-0.0.8/sema_toolchain.egg-info/requires.txt
+-rw-rw-r--   0 manon     (1000) manon     (1000)        1 2024-05-19 22:37:06.000000 sema_toolchain-0.0.8/sema_toolchain.egg-info/top_level.txt
+-rw-rw-r--   0 manon     (1000) manon     (1000)       38 2024-05-19 22:37:06.810842 sema_toolchain-0.0.8/setup.cfg
```

### Comparing `sema_toolchain-0.0.7/LICENSE` & `sema_toolchain-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sema_toolchain-0.0.7/PKG-INFO` & `sema_toolchain-0.0.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sema_toolchain
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python symbolic execution package
 Author-email: Manon-Oreins <manon.oreins@gmail.com>
 License: BSD 2-Clause License
         
         Copyright (c) 2022, UCL-Cybersecurity team
         All rights reserved.
         
@@ -100,189 +100,166 @@
       ░     ░  ░       ░         ░  ░
 
 ```
 
 
 # :books:  Documentation
 
-1. [ Architecture ](#arch)
-    1. [ Toolchain architecture ](#arch_std)
+1. [ Architecture ](#page_with_curl-architecture)
+    1. [ Toolchain architecture ](#toolchain-architecture)
 
-2. [ Installation ](#install)
+2. [ Recommended installation and usage ](#page_with_curl-recommended-installation-and-usage)
 
-3. [ SEMA ](#tc)
-    1. [ `SemaSCDG` ](#tcscdg)
-    2. [ `SemaClassifier` ](#tcc)
+3. [ Dockerhub installation and usage ](#page_with_curl-dockerhub-installation-and-usage)
 
-4. [Quick Start Demos](#)
-    1. [ `Extract SCDGs from binaries` ](https://github.com/csvl/SEMA-ToolChain/blob/production/Tutorial/Notebook/SEMA-SCDG%20Demo.ipynb)
+4. [ Pypi installation and usage ](#page_with_curl-Pypi-installation-and-usage)
 
-5. [ Credentials ](#credit)
+5. [ Credentials ](#page_with_curl-credentials)
 
 :page_with_curl: Architecture
 ====
 <a name="arch"></a>
 
 ### Toolchain architecture
 <a name="arch_std"></a>
 
+Our toolchain is represented in the next figure  and works as follow. A collection of labelled binaries of different malwares families is collected and used as the input of the toolchain. **Angr**, a framework for symbolic execution, is used to execute symbolically binaries and extract execution traces. For this purpose, different heuristics have been developped to optimize symbolic execution. Several execution traces (i.e : API calls used and their arguments) corresponding to one binary are extracted with Angr and gather together thanks to several graph heuristics to construct a SCDG. These resulting SCDGs are then used as input to graph mining to extract common graph between SCDG of the same family and create a signature. Finally when a new sample has to be classified, its SCDG is build and compared with SCDG of known families (thanks to a simple similarity metric).
 
-#### Main depencies:
-
-    * Python 3.8 (angr)
-
-    * Docker, docker buildx, docker compose
+![GitHub Logo](./images/SEMA_illustration.png)
 
-    * radare2
+This repository contains a first version of a SCDG extractor.
+During symbolic analysis of a binary, all system calls and their arguments found are recorded. After some stop conditions for symbolic analysis, a graph is build as follow : Nodes are systems Calls recorded, edges show that some arguments are shared between calls.
 
-#### Using Pypi sema-toolchain package
+When a new sample has to be evaluated, its SCDG is first build as described previously. Then, `gspan` is applied to extract the biggest common subgraph and a similarity score is evaluated to decide if the graph is considered as part of the family or not. The similarity score `S` between graph `G'` and `G''` is computed as follow:
+Since `G''` is a subgraph of `G'`, this is calculating how much `G'` appears in `G''`.
+Another classifier we use is the Support Vector Machine (`SVM`) with INRIA graph kernel or the Weisfeiler-Lehman extension graph kernel.
 
-If you wish to install the toolchain python dependencies on your system, use :
+A web application is available and is called SemaWebApp. It allows to manage the launch of experiments on SemaSCDG and/or SemaClassifier.
 
-```bash
-pip install sema-toolchain
-```
+#### Main depencies:
 
-#### Pypy3 usage
+    * Python 3.8
 
-By default, pypy3 can be used to launch experiments inside the SCDG's docker container. If you wish to use it outside the container, make sure to install pypy3 :
+    * Docker >=26.1.3 , docker buildx, Docker Compose >=v2.27.0
 
-```bash
-sudo add-apt-repository ppa:pypy/ppa
-sudo apt update
-sudo apt install pypy3
-```
-
-Then install the dependecies on pypy3 :
+    * radare2
 
-```bash
-pypy3 -m pip install -r /sema_scdg/requirements_pypy.txt
-```
+    * libvirt-dev, libgraphviz-dev, wheel
 
 #### Interesting links
 
 * https://angr.io/
 
 * https://bazaar.abuse.ch/
 
 * https://docs.docker.com/engine/install/ubuntu/
 
-:page_with_curl: Installation
-====
-<a name="install"></a>
-
-Tested on Ubuntu 20.04
-
-**Recommanded installation:**
-
-```bash
-git clone https://github.com/Manon-Oreins/SEMA-ToolChain.git;
-
-# Full installation (ubuntu)
-make build-toolchain;
-```
-
-If you only need the SCDG part of the toolchain you can use :
-```bash
-make pull-scdg
-```
-To pull the docker image directly from dockerHub
-
-Or visit `https://hub.docker.com/repository/docker/manonoreins/sema-scdg/tags`
-
-## Installation details (optional)
 
 #### For extracting database
 
 ```bash
 cd databases/Binaries; bash extract_deploy_db.sh
 ```
 
 Password for archive is "infected". Warning : it contains real samples of malwares.
 
-#### For code cleaning
+#### For compressing database
 
 ```bash
 #To zip back the test database
 cd databases/Binaries; bash compress_db.sh
 ```
 
-:page_with_curl: `SEMA - ToolChain`
+:page_with_curl: **Recommended installation and usage**
 ====
-<a name="tc"></a>
+<a name="install"></a>
 
-Our toolchain is represented in the next figure  and works as follow. A collection of labelled binaries of different malwares families is collected and used as the input of the toolchain. **Angr**, a framework for symbolic execution, is used to execute symbolically binaries and extract execution traces. For this purpose, different heuristics have been developped to optimize symbolic execution. Several execution traces (i.e : API calls used and their arguments) corresponding to one binary are extracted with Angr and gather together thanks to several graph heuristics to construct a SCDG. These resulting SCDGs are then used as input to graph mining to extract common graph between SCDG of the same family and create a signature. Finally when a new sample has to be classified, its SCDG is build and compared with SCDG of known families (thanks to a simple similarity metric).
+Install the entire toolchain
+
+```bash
+# Full installation (ubuntu)
+make build-toolchain;
+```
 
+## How to use ?
 
-### How to use ?
+### Using the web application
 
 First launch the containers :
 ```bash
 make run-toolchain
 ```
 
 It will start the scdg, the classifier and the web app services. If you wish to use only the scdg or only the classifier, refer to the next sections.
 
 Wait for the containers to be up
 
 Then visit 127.0.0.1:5000 on your browser
 
 See next sections for details about the different parameters.
 
-:page_with_curl: System Call Dependency Graphs extractor (`SemaSCDG`)
-====
-<a name="tcscdg"></a>
+#### Shut down
 
-This repository contains a first version of a SCDG extractor.
-During symbolic analysis of a binary, all system calls and their arguments found are recorded. After some stop conditions for symbolic analysis, a graph is build as follow : Nodes are systems Calls recorded, edges show that some arguments are shared between calls.
+To leave the toolchain just press Ctrl+C then use
+```bash
+make stop-toolchain
+```
+To stop all docker containers.
+
+If you want to remove all images :
 
-### How to use ?
-First run the SCDG container:
 ```bash
-make run-scdg-service
+docker rmi sema-web-app
+docker rmi sema-scdg
+docker rmi sema-classifier
+```
+
+### Use only SemaSCDG
+
+First run the SCDG container with volumes like this :
+```bash
+docker run --rm --name="sema-scdg" -v ${PWD}/OutputFolder:/sema-scdg/application/database/SCDG -v ${PWD}/ConfigFolder:/sema-scdg/application/configs -v ${PWD}/InputFolder:/sema-scdg/application/database/Binaries  -it sema-scdg bash
 ```
+Where the first volume corresponds to the output folder where the results will be put. The second volume corresponds to the folder containing the configuration files that will be passed to the docker. And the third matches the folder containing the binaries that are going to be passed to the container.
 
 Inside the container just run  :
 ```bash
 python3 SemaSCDG.py configs/config.ini
 ```
 Or if you want to use pypy3:
 ```bash
 pypy3 SemaSCDG.py configs/config.ini
 ```
 
+#### Configuration files
+
 The parameters are put in a configuration file : `configs/config.ini`
 Feel free to modify it or create new configuration files to run different experiments.
+
 To restore the default values of `config.ini` do :
 ```bash
 python3 restore_defaults.py
 ```
 The default parameters are stored in the file `default_config.ini`
+Do not modify `config_tutorial.ini` and `config_test.ini` as they are designed to fit the Tutorial and the tests needs respectively.
 
-If you wish to run multiple experiments with different configuration files, the script `multiple_experiments.sh` is available and can be used inside the scdg container:
+The output of the SCDG are put into `database/SCDG/runs/` by default. If you are not using volumes and want to save some runs from the container to your host machine :
 ```bash
-# To show usage
-./multiple_experiments.sh -h
-
-# Run example
-./multiple_experiments.sh -m python3 -c configs/config configs/default_configs
+make save-scdg-runs ARGS=PATH
 ```
 
-### Parameters description
+#### Parameters description
 SCDG module arguments
 
 ```
 expl_method:
   DFS                 Depth First Search
   BFS                 Breadth First Search
-  CDFS                Custom Depth First Search (Default)
-  CBFS                Custom Breadth First Search
-  DBFS                TODO
-  SDFS                TODO
-  SCDFS               TODO
+  CDFS                Coverage Depth-First Search Strategy (Default)
+  CBFS                Coverage Breadth First Search
 
 graph_output:
   gs                  .GS format
   json                .JSON format
   EMPTY               if left empty then build on all available format
 
 packing_type:
@@ -340,66 +317,53 @@
   plugin_hooks            Enable the hooks plugin
 ```
 
 **The binary path has to be a relative path to a binary beeing into the `database` directory**
 
 To know the details of the angr options see [Angr documentation](https://docs.angr.io/en/latest/appendix/options.html)
 
-Program will output a graph in `.gs` format that could be exploited by `gspan`.
-
 You also have a script `MergeGspan.py` in `sema_scdg/application/helper` which could merge all `.gs` from a directory into only one file.
 
+#### Run multiple experiments automatically
 
-## Managing your runs
-
-The output of the SCDG are put into `database/SCDG/runs/`
-
-If you want to save some runs from the container to your host machine :
+If you wish to run multiple experiments with different configuration files, the script `multiple_experiments.sh` is available and can be used inside the scdg container:
 ```bash
-make save-scdg-runs ARGS=PATH
+# To show usage
+./multiple_experiments.sh -h
+
+# Run example
+./multiple_experiments.sh -m python3 -c configs/config configs/default_configs
 ```
 
-## Tests
+#### Tests
 
 To run the test, inside the docker container :
 ```bash
 python3 scdg_tests.py configs/config_test.ini
 ```
 
-## Tutorial
+#### Tutorial
 
-There is a jupyter notebook providing a tutorial on how to use the scdg. To launch it, run the container by using :
-```bash
-make run-scdg
-```
-
-Then, inside the docker, run
+There is a jupyter notebook providing a tutorial on how to use the scdg. To launch it, inside the docker, run
 ```bash
 jupyter notebook --ip=0.0.0.0 --port=5001 --no-browser --allow-root --NotebookApp.token=''
 ```
-
 and visit `http://127.0.0.1:5001/tree` on your browser. Go to `/Tutorial` and open the jupyter notebook.
 
+### Use only SemaClassifier
 
-:page_with_curl: Model & Classification extractor (`SemaClassifier`)
-====
-<a name="tcc"></a>
-
-When a new sample has to be evaluated, its SCDG is first build as described previously. Then, `gspan` is applied to extract the biggest common subgraph and a similarity score is evaluated to decide if the graph is considered as part of the family or not.
-
-The similarity score `S` between graph `G'` and `G''` is computed as follow:
-
-Since `G''` is a subgraph of `G'`, this is calculating how much `G'` appears in `G''`.
-
-Another classifier we use is the Support Vector Machine (`SVM`) with INRIA graph kernel or the Weisfeiler-Lehman extension graph kernel.
+Launch the container:
+```bash
+docker run --rm --name="sema-scdg" -v ${PWD}/InputFolder:/sema-classifier/application/database -it sema-classifier ../docker_startup.sh 1
+```
 
-### How to use ?
+Where the volume correspond to the folder containings the inputs that will be accessible by the container.
 
-Just run the script :
-```bash
+Then just run the script :
+```
 python3 SemaClassifier.py FOLDER/FILE
 
 usage: update_readme_usage.py [-h] [--threshold THRESHOLD] [--biggest_subgraph BIGGEST_SUBGRAPH] [--support SUPPORT] [--ctimeout CTIMEOUT] [--epoch EPOCH] [--sepoch SEPOCH]
                               [--data_scale DATA_SCALE] [--vector_size VECTOR_SIZE] [--batch_size BATCH_SIZE] (--classification | --detection) (--wl | --inria | --dl | --gspan)
                               [--bancteian] [--delf] [--FeakerStealer] [--gandcrab] [--ircbot] [--lamer] [--nitol] [--RedLineStealer] [--sfone] [--sillyp2p] [--simbot]
                               [--Sodinokibi] [--sytro] [--upatre] [--wabot] [--RemcosRAT] [--verbose_classifier] [--train] [--nthread NTHREAD]
                               binaries
@@ -454,55 +418,85 @@
   --RemcosRAT
 
 Global parameter:
   --verbose_classifier  Verbose output during train/classification (default : False)
   --train               Launch training process, else classify/detect new sample with previously computed model
   --nthread NTHREAD     Number of thread used (default: max)
   binaries              Name of the folder containing binary'signatures to analyze (Default: output/save-SCDG/, only that for ToolChain)
-
 ```
 
 #### Example
 
 This will train models for input dataset
 
 ```bash
-python3 SemaClassifier/SemaClassifier.py --train output/save-SCDG/
+python3 SemaClassifier.py --train output/save-SCDG/
 ```
 
 This will classify input dataset based on previously computed models
 
 ```bash
-python3 SemaClassifier/SemaClassifier.py output/test-set/
+python3 SemaClassifier.py output/test-set/
 ```
 
-### Tests
+#### Tests
 
 To run the classifier tests, run inside the docker container:
 ```bash
 python3 classifier_tests.py configs/config_test.ini
 ```
 
+:page_with_curl: **Dockerhub installation**
+====
+<a name="dockerhub"></a>
 
-## Shut down
+## SemaSCDG
 
-To leave the toolchain just press Ctrl+C then use
+If you only need the SCDG part of the toolchain you can use :
+```bash
+make pull-scdg
+```
+To pull the docker image directly from dockerHub. Or visit `https://hub.docker.com/repository/docker/manonoreins/sema-scdg/tags`
+
+Then use the same commands than in the recommended usage section
 
+## SemaClassifier
+
+If you only need the Classifier part of the toolchain you can use :
 ```bash
-make stop-toolchain
+make pull-classifier
 ```
+To pull the docker image directly from dockerHub. Or visit `https://hub.docker.com/repository/docker/manonoreins/sema-classifier/tags`
 
-To stop all docker containers.
+Then use the same commands than in the recommended usage section
 
-If you want to remove all images :
+:page_with_curl: **Pypi installation and usage**
+====
+<a name="pypi"></a>
+
+If you wish to install the toolchain python dependencies on your system, use :
 
 ```bash
-docker rmi sema-web-app
-docker rmi sema-scdg
-docker rmi sema-classifier
+pip install sema-toolchain
+```
+
+#### Pypy3 usage
+
+By default, pypy3 can be used to launch experiments inside the SCDG's docker container. If you wish to use it outside the container, make sure to install pypy3 :
+
+```bash
+sudo add-apt-repository ppa:pypy/ppa
+sudo apt update
+sudo apt install pypy3
+```
+
+Then install the dependecies on pypy3 :
+
+```bash
+pypy3 -m pip install -r /sema_scdg/requirements_pypy.txt
 ```
 
 :page_with_curl: Credentials
 ====
 <a name="credit"></a>
 
 Main authors of the projects:
```

### Comparing `sema_toolchain-0.0.7/README.md` & `sema_toolchain-0.0.8/doc/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -12,189 +12,166 @@
       ░     ░  ░       ░         ░  ░
 
 ```
 
 
 # :books:  Documentation
 
-1. [ Architecture ](#arch)
-    1. [ Toolchain architecture ](#arch_std)
+1. [ Architecture ](#page_with_curl-architecture)
+    1. [ Toolchain architecture ](#toolchain-architecture)
 
-2. [ Installation ](#install)
+2. [ Recommended installation and usage ](#page_with_curl-recommended-installation-and-usage)
 
-3. [ SEMA ](#tc)
-    1. [ `SemaSCDG` ](#tcscdg)
-    2. [ `SemaClassifier` ](#tcc)
+3. [ Dockerhub installation and usage ](#page_with_curl-dockerhub-installation-and-usage)
 
-4. [Quick Start Demos](#)
-    1. [ `Extract SCDGs from binaries` ](https://github.com/csvl/SEMA-ToolChain/blob/production/Tutorial/Notebook/SEMA-SCDG%20Demo.ipynb)
+4. [ Pypi installation and usage ](#page_with_curl-Pypi-installation-and-usage)
 
-5. [ Credentials ](#credit)
+5. [ Credentials ](#page_with_curl-credentials)
 
 :page_with_curl: Architecture
 ====
 <a name="arch"></a>
 
 ### Toolchain architecture
 <a name="arch_std"></a>
 
+Our toolchain is represented in the next figure  and works as follow. A collection of labelled binaries of different malwares families is collected and used as the input of the toolchain. **Angr**, a framework for symbolic execution, is used to execute symbolically binaries and extract execution traces. For this purpose, different heuristics have been developped to optimize symbolic execution. Several execution traces (i.e : API calls used and their arguments) corresponding to one binary are extracted with Angr and gather together thanks to several graph heuristics to construct a SCDG. These resulting SCDGs are then used as input to graph mining to extract common graph between SCDG of the same family and create a signature. Finally when a new sample has to be classified, its SCDG is build and compared with SCDG of known families (thanks to a simple similarity metric).
 
-#### Main depencies:
-
-    * Python 3.8 (angr)
-
-    * Docker, docker buildx, docker compose
+![GitHub Logo](./images/SEMA_illustration.png)
 
-    * radare2
+This repository contains a first version of a SCDG extractor.
+During symbolic analysis of a binary, all system calls and their arguments found are recorded. After some stop conditions for symbolic analysis, a graph is build as follow : Nodes are systems Calls recorded, edges show that some arguments are shared between calls.
 
-#### Using Pypi sema-toolchain package
+When a new sample has to be evaluated, its SCDG is first build as described previously. Then, `gspan` is applied to extract the biggest common subgraph and a similarity score is evaluated to decide if the graph is considered as part of the family or not. The similarity score `S` between graph `G'` and `G''` is computed as follow:
+Since `G''` is a subgraph of `G'`, this is calculating how much `G'` appears in `G''`.
+Another classifier we use is the Support Vector Machine (`SVM`) with INRIA graph kernel or the Weisfeiler-Lehman extension graph kernel.
 
-If you wish to install the toolchain python dependencies on your system, use :
+A web application is available and is called SemaWebApp. It allows to manage the launch of experiments on SemaSCDG and/or SemaClassifier.
 
-```bash
-pip install sema-toolchain
-```
+#### Main depencies:
 
-#### Pypy3 usage
+    * Python 3.8
 
-By default, pypy3 can be used to launch experiments inside the SCDG's docker container. If you wish to use it outside the container, make sure to install pypy3 :
+    * Docker >=26.1.3 , docker buildx, Docker Compose >=v2.27.0
 
-```bash
-sudo add-apt-repository ppa:pypy/ppa
-sudo apt update
-sudo apt install pypy3
-```
-
-Then install the dependecies on pypy3 :
+    * radare2
 
-```bash
-pypy3 -m pip install -r /sema_scdg/requirements_pypy.txt
-```
+    * libvirt-dev, libgraphviz-dev, wheel
 
 #### Interesting links
 
 * https://angr.io/
 
 * https://bazaar.abuse.ch/
 
 * https://docs.docker.com/engine/install/ubuntu/
 
-:page_with_curl: Installation
-====
-<a name="install"></a>
-
-Tested on Ubuntu 20.04
-
-**Recommanded installation:**
-
-```bash
-git clone https://github.com/Manon-Oreins/SEMA-ToolChain.git;
-
-# Full installation (ubuntu)
-make build-toolchain;
-```
-
-If you only need the SCDG part of the toolchain you can use :
-```bash
-make pull-scdg
-```
-To pull the docker image directly from dockerHub
-
-Or visit `https://hub.docker.com/repository/docker/manonoreins/sema-scdg/tags`
-
-## Installation details (optional)
 
 #### For extracting database
 
 ```bash
 cd databases/Binaries; bash extract_deploy_db.sh
 ```
 
 Password for archive is "infected". Warning : it contains real samples of malwares.
 
-#### For code cleaning
+#### For compressing database
 
 ```bash
 #To zip back the test database
 cd databases/Binaries; bash compress_db.sh
 ```
 
-:page_with_curl: `SEMA - ToolChain`
+:page_with_curl: **Recommended installation and usage**
 ====
-<a name="tc"></a>
+<a name="install"></a>
 
-Our toolchain is represented in the next figure  and works as follow. A collection of labelled binaries of different malwares families is collected and used as the input of the toolchain. **Angr**, a framework for symbolic execution, is used to execute symbolically binaries and extract execution traces. For this purpose, different heuristics have been developped to optimize symbolic execution. Several execution traces (i.e : API calls used and their arguments) corresponding to one binary are extracted with Angr and gather together thanks to several graph heuristics to construct a SCDG. These resulting SCDGs are then used as input to graph mining to extract common graph between SCDG of the same family and create a signature. Finally when a new sample has to be classified, its SCDG is build and compared with SCDG of known families (thanks to a simple similarity metric).
+Install the entire toolchain
+
+```bash
+# Full installation (ubuntu)
+make build-toolchain;
+```
 
+## How to use ?
 
-### How to use ?
+### Using the web application
 
 First launch the containers :
 ```bash
 make run-toolchain
 ```
 
 It will start the scdg, the classifier and the web app services. If you wish to use only the scdg or only the classifier, refer to the next sections.
 
 Wait for the containers to be up
 
 Then visit 127.0.0.1:5000 on your browser
 
 See next sections for details about the different parameters.
 
-:page_with_curl: System Call Dependency Graphs extractor (`SemaSCDG`)
-====
-<a name="tcscdg"></a>
+#### Shut down
 
-This repository contains a first version of a SCDG extractor.
-During symbolic analysis of a binary, all system calls and their arguments found are recorded. After some stop conditions for symbolic analysis, a graph is build as follow : Nodes are systems Calls recorded, edges show that some arguments are shared between calls.
+To leave the toolchain just press Ctrl+C then use
+```bash
+make stop-toolchain
+```
+To stop all docker containers.
+
+If you want to remove all images :
 
-### How to use ?
-First run the SCDG container:
 ```bash
-make run-scdg-service
+docker rmi sema-web-app
+docker rmi sema-scdg
+docker rmi sema-classifier
+```
+
+### Use only SemaSCDG
+
+First run the SCDG container with volumes like this :
+```bash
+docker run --rm --name="sema-scdg" -v ${PWD}/OutputFolder:/sema-scdg/application/database/SCDG -v ${PWD}/ConfigFolder:/sema-scdg/application/configs -v ${PWD}/InputFolder:/sema-scdg/application/database/Binaries  -it sema-scdg bash
 ```
+Where the first volume corresponds to the output folder where the results will be put. The second volume corresponds to the folder containing the configuration files that will be passed to the docker. And the third matches the folder containing the binaries that are going to be passed to the container.
 
 Inside the container just run  :
 ```bash
 python3 SemaSCDG.py configs/config.ini
 ```
 Or if you want to use pypy3:
 ```bash
 pypy3 SemaSCDG.py configs/config.ini
 ```
 
+#### Configuration files
+
 The parameters are put in a configuration file : `configs/config.ini`
 Feel free to modify it or create new configuration files to run different experiments.
+
 To restore the default values of `config.ini` do :
 ```bash
 python3 restore_defaults.py
 ```
 The default parameters are stored in the file `default_config.ini`
+Do not modify `config_tutorial.ini` and `config_test.ini` as they are designed to fit the Tutorial and the tests needs respectively.
 
-If you wish to run multiple experiments with different configuration files, the script `multiple_experiments.sh` is available and can be used inside the scdg container:
+The output of the SCDG are put into `database/SCDG/runs/` by default. If you are not using volumes and want to save some runs from the container to your host machine :
 ```bash
-# To show usage
-./multiple_experiments.sh -h
-
-# Run example
-./multiple_experiments.sh -m python3 -c configs/config configs/default_configs
+make save-scdg-runs ARGS=PATH
 ```
 
-### Parameters description
+#### Parameters description
 SCDG module arguments
 
 ```
 expl_method:
   DFS                 Depth First Search
   BFS                 Breadth First Search
-  CDFS                Custom Depth First Search (Default)
-  CBFS                Custom Breadth First Search
-  DBFS                TODO
-  SDFS                TODO
-  SCDFS               TODO
+  CDFS                Coverage Depth-First Search Strategy (Default)
+  CBFS                Coverage Breadth First Search
 
 graph_output:
   gs                  .GS format
   json                .JSON format
   EMPTY               if left empty then build on all available format
 
 packing_type:
@@ -252,66 +229,53 @@
   plugin_hooks            Enable the hooks plugin
 ```
 
 **The binary path has to be a relative path to a binary beeing into the `database` directory**
 
 To know the details of the angr options see [Angr documentation](https://docs.angr.io/en/latest/appendix/options.html)
 
-Program will output a graph in `.gs` format that could be exploited by `gspan`.
-
 You also have a script `MergeGspan.py` in `sema_scdg/application/helper` which could merge all `.gs` from a directory into only one file.
 
+#### Run multiple experiments automatically
 
-## Managing your runs
-
-The output of the SCDG are put into `database/SCDG/runs/`
-
-If you want to save some runs from the container to your host machine :
+If you wish to run multiple experiments with different configuration files, the script `multiple_experiments.sh` is available and can be used inside the scdg container:
 ```bash
-make save-scdg-runs ARGS=PATH
+# To show usage
+./multiple_experiments.sh -h
+
+# Run example
+./multiple_experiments.sh -m python3 -c configs/config configs/default_configs
 ```
 
-## Tests
+#### Tests
 
 To run the test, inside the docker container :
 ```bash
 python3 scdg_tests.py configs/config_test.ini
 ```
 
-## Tutorial
+#### Tutorial
 
-There is a jupyter notebook providing a tutorial on how to use the scdg. To launch it, run the container by using :
-```bash
-make run-scdg
-```
-
-Then, inside the docker, run
+There is a jupyter notebook providing a tutorial on how to use the scdg. To launch it, inside the docker, run
 ```bash
 jupyter notebook --ip=0.0.0.0 --port=5001 --no-browser --allow-root --NotebookApp.token=''
 ```
-
 and visit `http://127.0.0.1:5001/tree` on your browser. Go to `/Tutorial` and open the jupyter notebook.
 
+### Use only SemaClassifier
 
-:page_with_curl: Model & Classification extractor (`SemaClassifier`)
-====
-<a name="tcc"></a>
-
-When a new sample has to be evaluated, its SCDG is first build as described previously. Then, `gspan` is applied to extract the biggest common subgraph and a similarity score is evaluated to decide if the graph is considered as part of the family or not.
-
-The similarity score `S` between graph `G'` and `G''` is computed as follow:
-
-Since `G''` is a subgraph of `G'`, this is calculating how much `G'` appears in `G''`.
-
-Another classifier we use is the Support Vector Machine (`SVM`) with INRIA graph kernel or the Weisfeiler-Lehman extension graph kernel.
+Launch the container:
+```bash
+docker run --rm --name="sema-scdg" -v ${PWD}/InputFolder:/sema-classifier/application/database -it sema-classifier ../docker_startup.sh 1
+```
 
-### How to use ?
+Where the volume correspond to the folder containings the inputs that will be accessible by the container.
 
-Just run the script :
-```bash
+Then just run the script :
+```
 python3 SemaClassifier.py FOLDER/FILE
 
 usage: update_readme_usage.py [-h] [--threshold THRESHOLD] [--biggest_subgraph BIGGEST_SUBGRAPH] [--support SUPPORT] [--ctimeout CTIMEOUT] [--epoch EPOCH] [--sepoch SEPOCH]
                               [--data_scale DATA_SCALE] [--vector_size VECTOR_SIZE] [--batch_size BATCH_SIZE] (--classification | --detection) (--wl | --inria | --dl | --gspan)
                               [--bancteian] [--delf] [--FeakerStealer] [--gandcrab] [--ircbot] [--lamer] [--nitol] [--RedLineStealer] [--sfone] [--sillyp2p] [--simbot]
                               [--Sodinokibi] [--sytro] [--upatre] [--wabot] [--RemcosRAT] [--verbose_classifier] [--train] [--nthread NTHREAD]
                               binaries
@@ -366,55 +330,85 @@
   --RemcosRAT
 
 Global parameter:
   --verbose_classifier  Verbose output during train/classification (default : False)
   --train               Launch training process, else classify/detect new sample with previously computed model
   --nthread NTHREAD     Number of thread used (default: max)
   binaries              Name of the folder containing binary'signatures to analyze (Default: output/save-SCDG/, only that for ToolChain)
-
 ```
 
 #### Example
 
 This will train models for input dataset
 
 ```bash
-python3 SemaClassifier/SemaClassifier.py --train output/save-SCDG/
+python3 SemaClassifier.py --train output/save-SCDG/
 ```
 
 This will classify input dataset based on previously computed models
 
 ```bash
-python3 SemaClassifier/SemaClassifier.py output/test-set/
+python3 SemaClassifier.py output/test-set/
 ```
 
-### Tests
+#### Tests
 
 To run the classifier tests, run inside the docker container:
 ```bash
 python3 classifier_tests.py configs/config_test.ini
 ```
 
+:page_with_curl: **Dockerhub installation**
+====
+<a name="dockerhub"></a>
 
-## Shut down
+## SemaSCDG
 
-To leave the toolchain just press Ctrl+C then use
+If you only need the SCDG part of the toolchain you can use :
+```bash
+make pull-scdg
+```
+To pull the docker image directly from dockerHub. Or visit `https://hub.docker.com/repository/docker/manonoreins/sema-scdg/tags`
+
+Then use the same commands than in the recommended usage section
 
+## SemaClassifier
+
+If you only need the Classifier part of the toolchain you can use :
 ```bash
-make stop-toolchain
+make pull-classifier
 ```
+To pull the docker image directly from dockerHub. Or visit `https://hub.docker.com/repository/docker/manonoreins/sema-classifier/tags`
 
-To stop all docker containers.
+Then use the same commands than in the recommended usage section
 
-If you want to remove all images :
+:page_with_curl: **Pypi installation and usage**
+====
+<a name="pypi"></a>
+
+If you wish to install the toolchain python dependencies on your system, use :
 
 ```bash
-docker rmi sema-web-app
-docker rmi sema-scdg
-docker rmi sema-classifier
+pip install sema-toolchain
+```
+
+#### Pypy3 usage
+
+By default, pypy3 can be used to launch experiments inside the SCDG's docker container. If you wish to use it outside the container, make sure to install pypy3 :
+
+```bash
+sudo add-apt-repository ppa:pypy/ppa
+sudo apt update
+sudo apt install pypy3
+```
+
+Then install the dependecies on pypy3 :
+
+```bash
+pypy3 -m pip install -r /sema_scdg/requirements_pypy.txt
 ```
 
 :page_with_curl: Credentials
 ====
 <a name="credit"></a>
 
 Main authors of the projects:
```

### Comparing `sema_toolchain-0.0.7/pyproject.toml` & `sema_toolchain-0.0.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 [build-system]
-requires = ["setuptools>=62.4"]
+requires = ["setuptools>=62.4", "wheel"]
 build-backend = "setuptools.build_meta"
 
-[tool.setuptools]
-py-modules = ["sema_scdg", "sema_web_app", "sema_classifier"]
-
 [project]
 name = "sema_toolchain"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Manon-Oreins", email="manon.oreins@gmail.com" },
 ]
 description = "Python symbolic execution package"
-readme = "README.md"
+readme = "doc/README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: Unix",
 ]
 keywords = ["scdg", "binary", "symbolic", "analysis"]
@@ -68,11 +65,9 @@
     "torchvision",
     "flask_session",
     "django",
     "Flask-Cors",
     "npf-web-extension"
 ]
 
-
-
 [project.urls]
 Homepage = "https://github.com/Manon-Oreins/SEMA-ToolChain/tree/refactor_simproc"
```

### Comparing `sema_toolchain-0.0.7/sema_toolchain.egg-info/PKG-INFO` & `sema_toolchain-0.0.8/sema_toolchain.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sema_toolchain
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python symbolic execution package
 Author-email: Manon-Oreins <manon.oreins@gmail.com>
 License: BSD 2-Clause License
         
         Copyright (c) 2022, UCL-Cybersecurity team
         All rights reserved.
         
@@ -100,189 +100,166 @@
       ░     ░  ░       ░         ░  ░
 
 ```
 
 
 # :books:  Documentation
 
-1. [ Architecture ](#arch)
-    1. [ Toolchain architecture ](#arch_std)
+1. [ Architecture ](#page_with_curl-architecture)
+    1. [ Toolchain architecture ](#toolchain-architecture)
 
-2. [ Installation ](#install)
+2. [ Recommended installation and usage ](#page_with_curl-recommended-installation-and-usage)
 
-3. [ SEMA ](#tc)
-    1. [ `SemaSCDG` ](#tcscdg)
-    2. [ `SemaClassifier` ](#tcc)
+3. [ Dockerhub installation and usage ](#page_with_curl-dockerhub-installation-and-usage)
 
-4. [Quick Start Demos](#)
-    1. [ `Extract SCDGs from binaries` ](https://github.com/csvl/SEMA-ToolChain/blob/production/Tutorial/Notebook/SEMA-SCDG%20Demo.ipynb)
+4. [ Pypi installation and usage ](#page_with_curl-Pypi-installation-and-usage)
 
-5. [ Credentials ](#credit)
+5. [ Credentials ](#page_with_curl-credentials)
 
 :page_with_curl: Architecture
 ====
 <a name="arch"></a>
 
 ### Toolchain architecture
 <a name="arch_std"></a>
 
+Our toolchain is represented in the next figure  and works as follow. A collection of labelled binaries of different malwares families is collected and used as the input of the toolchain. **Angr**, a framework for symbolic execution, is used to execute symbolically binaries and extract execution traces. For this purpose, different heuristics have been developped to optimize symbolic execution. Several execution traces (i.e : API calls used and their arguments) corresponding to one binary are extracted with Angr and gather together thanks to several graph heuristics to construct a SCDG. These resulting SCDGs are then used as input to graph mining to extract common graph between SCDG of the same family and create a signature. Finally when a new sample has to be classified, its SCDG is build and compared with SCDG of known families (thanks to a simple similarity metric).
 
-#### Main depencies:
-
-    * Python 3.8 (angr)
-
-    * Docker, docker buildx, docker compose
+![GitHub Logo](./images/SEMA_illustration.png)
 
-    * radare2
+This repository contains a first version of a SCDG extractor.
+During symbolic analysis of a binary, all system calls and their arguments found are recorded. After some stop conditions for symbolic analysis, a graph is build as follow : Nodes are systems Calls recorded, edges show that some arguments are shared between calls.
 
-#### Using Pypi sema-toolchain package
+When a new sample has to be evaluated, its SCDG is first build as described previously. Then, `gspan` is applied to extract the biggest common subgraph and a similarity score is evaluated to decide if the graph is considered as part of the family or not. The similarity score `S` between graph `G'` and `G''` is computed as follow:
+Since `G''` is a subgraph of `G'`, this is calculating how much `G'` appears in `G''`.
+Another classifier we use is the Support Vector Machine (`SVM`) with INRIA graph kernel or the Weisfeiler-Lehman extension graph kernel.
 
-If you wish to install the toolchain python dependencies on your system, use :
+A web application is available and is called SemaWebApp. It allows to manage the launch of experiments on SemaSCDG and/or SemaClassifier.
 
-```bash
-pip install sema-toolchain
-```
+#### Main depencies:
 
-#### Pypy3 usage
+    * Python 3.8
 
-By default, pypy3 can be used to launch experiments inside the SCDG's docker container. If you wish to use it outside the container, make sure to install pypy3 :
+    * Docker >=26.1.3 , docker buildx, Docker Compose >=v2.27.0
 
-```bash
-sudo add-apt-repository ppa:pypy/ppa
-sudo apt update
-sudo apt install pypy3
-```
-
-Then install the dependecies on pypy3 :
+    * radare2
 
-```bash
-pypy3 -m pip install -r /sema_scdg/requirements_pypy.txt
-```
+    * libvirt-dev, libgraphviz-dev, wheel
 
 #### Interesting links
 
 * https://angr.io/
 
 * https://bazaar.abuse.ch/
 
 * https://docs.docker.com/engine/install/ubuntu/
 
-:page_with_curl: Installation
-====
-<a name="install"></a>
-
-Tested on Ubuntu 20.04
-
-**Recommanded installation:**
-
-```bash
-git clone https://github.com/Manon-Oreins/SEMA-ToolChain.git;
-
-# Full installation (ubuntu)
-make build-toolchain;
-```
-
-If you only need the SCDG part of the toolchain you can use :
-```bash
-make pull-scdg
-```
-To pull the docker image directly from dockerHub
-
-Or visit `https://hub.docker.com/repository/docker/manonoreins/sema-scdg/tags`
-
-## Installation details (optional)
 
 #### For extracting database
 
 ```bash
 cd databases/Binaries; bash extract_deploy_db.sh
 ```
 
 Password for archive is "infected". Warning : it contains real samples of malwares.
 
-#### For code cleaning
+#### For compressing database
 
 ```bash
 #To zip back the test database
 cd databases/Binaries; bash compress_db.sh
 ```
 
-:page_with_curl: `SEMA - ToolChain`
+:page_with_curl: **Recommended installation and usage**
 ====
-<a name="tc"></a>
+<a name="install"></a>
 
-Our toolchain is represented in the next figure  and works as follow. A collection of labelled binaries of different malwares families is collected and used as the input of the toolchain. **Angr**, a framework for symbolic execution, is used to execute symbolically binaries and extract execution traces. For this purpose, different heuristics have been developped to optimize symbolic execution. Several execution traces (i.e : API calls used and their arguments) corresponding to one binary are extracted with Angr and gather together thanks to several graph heuristics to construct a SCDG. These resulting SCDGs are then used as input to graph mining to extract common graph between SCDG of the same family and create a signature. Finally when a new sample has to be classified, its SCDG is build and compared with SCDG of known families (thanks to a simple similarity metric).
+Install the entire toolchain
+
+```bash
+# Full installation (ubuntu)
+make build-toolchain;
+```
 
+## How to use ?
 
-### How to use ?
+### Using the web application
 
 First launch the containers :
 ```bash
 make run-toolchain
 ```
 
 It will start the scdg, the classifier and the web app services. If you wish to use only the scdg or only the classifier, refer to the next sections.
 
 Wait for the containers to be up
 
 Then visit 127.0.0.1:5000 on your browser
 
 See next sections for details about the different parameters.
 
-:page_with_curl: System Call Dependency Graphs extractor (`SemaSCDG`)
-====
-<a name="tcscdg"></a>
+#### Shut down
 
-This repository contains a first version of a SCDG extractor.
-During symbolic analysis of a binary, all system calls and their arguments found are recorded. After some stop conditions for symbolic analysis, a graph is build as follow : Nodes are systems Calls recorded, edges show that some arguments are shared between calls.
+To leave the toolchain just press Ctrl+C then use
+```bash
+make stop-toolchain
+```
+To stop all docker containers.
+
+If you want to remove all images :
 
-### How to use ?
-First run the SCDG container:
 ```bash
-make run-scdg-service
+docker rmi sema-web-app
+docker rmi sema-scdg
+docker rmi sema-classifier
+```
+
+### Use only SemaSCDG
+
+First run the SCDG container with volumes like this :
+```bash
+docker run --rm --name="sema-scdg" -v ${PWD}/OutputFolder:/sema-scdg/application/database/SCDG -v ${PWD}/ConfigFolder:/sema-scdg/application/configs -v ${PWD}/InputFolder:/sema-scdg/application/database/Binaries  -it sema-scdg bash
 ```
+Where the first volume corresponds to the output folder where the results will be put. The second volume corresponds to the folder containing the configuration files that will be passed to the docker. And the third matches the folder containing the binaries that are going to be passed to the container.
 
 Inside the container just run  :
 ```bash
 python3 SemaSCDG.py configs/config.ini
 ```
 Or if you want to use pypy3:
 ```bash
 pypy3 SemaSCDG.py configs/config.ini
 ```
 
+#### Configuration files
+
 The parameters are put in a configuration file : `configs/config.ini`
 Feel free to modify it or create new configuration files to run different experiments.
+
 To restore the default values of `config.ini` do :
 ```bash
 python3 restore_defaults.py
 ```
 The default parameters are stored in the file `default_config.ini`
+Do not modify `config_tutorial.ini` and `config_test.ini` as they are designed to fit the Tutorial and the tests needs respectively.
 
-If you wish to run multiple experiments with different configuration files, the script `multiple_experiments.sh` is available and can be used inside the scdg container:
+The output of the SCDG are put into `database/SCDG/runs/` by default. If you are not using volumes and want to save some runs from the container to your host machine :
 ```bash
-# To show usage
-./multiple_experiments.sh -h
-
-# Run example
-./multiple_experiments.sh -m python3 -c configs/config configs/default_configs
+make save-scdg-runs ARGS=PATH
 ```
 
-### Parameters description
+#### Parameters description
 SCDG module arguments
 
 ```
 expl_method:
   DFS                 Depth First Search
   BFS                 Breadth First Search
-  CDFS                Custom Depth First Search (Default)
-  CBFS                Custom Breadth First Search
-  DBFS                TODO
-  SDFS                TODO
-  SCDFS               TODO
+  CDFS                Coverage Depth-First Search Strategy (Default)
+  CBFS                Coverage Breadth First Search
 
 graph_output:
   gs                  .GS format
   json                .JSON format
   EMPTY               if left empty then build on all available format
 
 packing_type:
@@ -340,66 +317,53 @@
   plugin_hooks            Enable the hooks plugin
 ```
 
 **The binary path has to be a relative path to a binary beeing into the `database` directory**
 
 To know the details of the angr options see [Angr documentation](https://docs.angr.io/en/latest/appendix/options.html)
 
-Program will output a graph in `.gs` format that could be exploited by `gspan`.
-
 You also have a script `MergeGspan.py` in `sema_scdg/application/helper` which could merge all `.gs` from a directory into only one file.
 
+#### Run multiple experiments automatically
 
-## Managing your runs
-
-The output of the SCDG are put into `database/SCDG/runs/`
-
-If you want to save some runs from the container to your host machine :
+If you wish to run multiple experiments with different configuration files, the script `multiple_experiments.sh` is available and can be used inside the scdg container:
 ```bash
-make save-scdg-runs ARGS=PATH
+# To show usage
+./multiple_experiments.sh -h
+
+# Run example
+./multiple_experiments.sh -m python3 -c configs/config configs/default_configs
 ```
 
-## Tests
+#### Tests
 
 To run the test, inside the docker container :
 ```bash
 python3 scdg_tests.py configs/config_test.ini
 ```
 
-## Tutorial
+#### Tutorial
 
-There is a jupyter notebook providing a tutorial on how to use the scdg. To launch it, run the container by using :
-```bash
-make run-scdg
-```
-
-Then, inside the docker, run
+There is a jupyter notebook providing a tutorial on how to use the scdg. To launch it, inside the docker, run
 ```bash
 jupyter notebook --ip=0.0.0.0 --port=5001 --no-browser --allow-root --NotebookApp.token=''
 ```
-
 and visit `http://127.0.0.1:5001/tree` on your browser. Go to `/Tutorial` and open the jupyter notebook.
 
+### Use only SemaClassifier
 
-:page_with_curl: Model & Classification extractor (`SemaClassifier`)
-====
-<a name="tcc"></a>
-
-When a new sample has to be evaluated, its SCDG is first build as described previously. Then, `gspan` is applied to extract the biggest common subgraph and a similarity score is evaluated to decide if the graph is considered as part of the family or not.
-
-The similarity score `S` between graph `G'` and `G''` is computed as follow:
-
-Since `G''` is a subgraph of `G'`, this is calculating how much `G'` appears in `G''`.
-
-Another classifier we use is the Support Vector Machine (`SVM`) with INRIA graph kernel or the Weisfeiler-Lehman extension graph kernel.
+Launch the container:
+```bash
+docker run --rm --name="sema-scdg" -v ${PWD}/InputFolder:/sema-classifier/application/database -it sema-classifier ../docker_startup.sh 1
+```
 
-### How to use ?
+Where the volume correspond to the folder containings the inputs that will be accessible by the container.
 
-Just run the script :
-```bash
+Then just run the script :
+```
 python3 SemaClassifier.py FOLDER/FILE
 
 usage: update_readme_usage.py [-h] [--threshold THRESHOLD] [--biggest_subgraph BIGGEST_SUBGRAPH] [--support SUPPORT] [--ctimeout CTIMEOUT] [--epoch EPOCH] [--sepoch SEPOCH]
                               [--data_scale DATA_SCALE] [--vector_size VECTOR_SIZE] [--batch_size BATCH_SIZE] (--classification | --detection) (--wl | --inria | --dl | --gspan)
                               [--bancteian] [--delf] [--FeakerStealer] [--gandcrab] [--ircbot] [--lamer] [--nitol] [--RedLineStealer] [--sfone] [--sillyp2p] [--simbot]
                               [--Sodinokibi] [--sytro] [--upatre] [--wabot] [--RemcosRAT] [--verbose_classifier] [--train] [--nthread NTHREAD]
                               binaries
@@ -454,55 +418,85 @@
   --RemcosRAT
 
 Global parameter:
   --verbose_classifier  Verbose output during train/classification (default : False)
   --train               Launch training process, else classify/detect new sample with previously computed model
   --nthread NTHREAD     Number of thread used (default: max)
   binaries              Name of the folder containing binary'signatures to analyze (Default: output/save-SCDG/, only that for ToolChain)
-
 ```
 
 #### Example
 
 This will train models for input dataset
 
 ```bash
-python3 SemaClassifier/SemaClassifier.py --train output/save-SCDG/
+python3 SemaClassifier.py --train output/save-SCDG/
 ```
 
 This will classify input dataset based on previously computed models
 
 ```bash
-python3 SemaClassifier/SemaClassifier.py output/test-set/
+python3 SemaClassifier.py output/test-set/
 ```
 
-### Tests
+#### Tests
 
 To run the classifier tests, run inside the docker container:
 ```bash
 python3 classifier_tests.py configs/config_test.ini
 ```
 
+:page_with_curl: **Dockerhub installation**
+====
+<a name="dockerhub"></a>
 
-## Shut down
+## SemaSCDG
 
-To leave the toolchain just press Ctrl+C then use
+If you only need the SCDG part of the toolchain you can use :
+```bash
+make pull-scdg
+```
+To pull the docker image directly from dockerHub. Or visit `https://hub.docker.com/repository/docker/manonoreins/sema-scdg/tags`
+
+Then use the same commands than in the recommended usage section
 
+## SemaClassifier
+
+If you only need the Classifier part of the toolchain you can use :
 ```bash
-make stop-toolchain
+make pull-classifier
 ```
+To pull the docker image directly from dockerHub. Or visit `https://hub.docker.com/repository/docker/manonoreins/sema-classifier/tags`
 
-To stop all docker containers.
+Then use the same commands than in the recommended usage section
 
-If you want to remove all images :
+:page_with_curl: **Pypi installation and usage**
+====
+<a name="pypi"></a>
+
+If you wish to install the toolchain python dependencies on your system, use :
 
 ```bash
-docker rmi sema-web-app
-docker rmi sema-scdg
-docker rmi sema-classifier
+pip install sema-toolchain
+```
+
+#### Pypy3 usage
+
+By default, pypy3 can be used to launch experiments inside the SCDG's docker container. If you wish to use it outside the container, make sure to install pypy3 :
+
+```bash
+sudo add-apt-repository ppa:pypy/ppa
+sudo apt update
+sudo apt install pypy3
+```
+
+Then install the dependecies on pypy3 :
+
+```bash
+pypy3 -m pip install -r /sema_scdg/requirements_pypy.txt
 ```
 
 :page_with_curl: Credentials
 ====
 <a name="credit"></a>
 
 Main authors of the projects:
```

### Comparing `sema_toolchain-0.0.7/sema_toolchain.egg-info/requires.txt` & `sema_toolchain-0.0.8/sema_toolchain.egg-info/requires.txt`

 * *Files identical despite different names*

