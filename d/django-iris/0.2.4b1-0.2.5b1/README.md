# Comparing `tmp/django-iris-0.2.4b1.tar.gz` & `tmp/django_iris-0.2.5b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-iris-0.2.4b1.tar", last modified: Tue Dec 19 15:33:56 2023, max compression
+gzip compressed data, was "django_iris-0.2.5b1.tar", last modified: Mon May 20 12:52:39 2024, max compression
```

## Comparing `django-iris-0.2.4b1.tar` & `django_iris-0.2.5b1.tar`

### file list

```diff
@@ -1,93 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 15:33:56.722005 django-iris-0.2.4b1/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2023-12-19 15:33:38.000000 django-iris-0.2.4b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2023-12-19 15:33:56.722005 django-iris-0.2.4b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      691 2023-12-19 15:33:38.000000 django-iris-0.2.4b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 15:33:56.706006 django-iris-0.2.4b1/django_iris/
--rw-r--r--   0 runner    (1001) docker     (127)     4245 2023-12-19 15:33:38.000000 django-iris-0.2.4b1/django_iris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7196 2023-12-19 15:33:38.000000 django-iris-0.2.4b1/django_iris/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7738 2023-12-19 15:33:38.000000 django-iris-0.2.4b1/django_iris/compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2023-12-19 15:33:38.000000 django-iris-0.2.4b1/django_iris/creation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2023-12-19 15:33:38.000000 django-iris-0.2.4b1/django_iris/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8066 2023-12-19 15:33:38.000000 django-iris-0.2.4b1/django_iris/features.py
--rw-r--r--   0 runner    (1001) docker     (127)    10444 2023-12-19 15:33:38.000000 django-iris-0.2.4b1/django_iris/introspection.py
--rw-r--r--   0 runner    (1001) docker     (127)    13300 2023-12-19 15:33:38.000000 django-iris-0.2.4b1/django_iris/operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4148 2023-12-19 15:33:38.000000 django-iris-0.2.4b1/django_iris/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2023-12-19 15:33:38.000000 django-iris-0.2.4b1/django_iris/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2023-12-19 15:33:38.000000 django-iris-0.2.4b1/django_iris/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 15:33:56.722005 django-iris-0.2.4b1/django_iris.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/django_iris.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/django_iris.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/django_iris.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/django_iris.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 15:33:56.714006 django-iris-0.2.4b1/intersystems_iris/
--rw-rw-rw-   0 runner    (1001) docker     (127)      299 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/_BufferReader.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     1337 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/_BufferWriter.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     1896 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/_ConnectionInformation.py
--rw-rw-rw-   0 runner    (1001) docker     (127)      578 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/_ConnectionParameters.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     1483 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/_Constant.py
--rw-rw-rw-   0 runner    (1001) docker     (127)    20104 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/_DBList.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     2311 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/_Device.py
--rw-rw-rw-   0 runner    (1001) docker     (127)      618 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/_GatewayContext.py
--rw-rw-rw-   0 runner    (1001) docker     (127)       96 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/_GatewayException.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     2735 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/_GatewayUtility.py
--rw-rw-rw-   0 runner    (1001) docker     (127)    49548 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/_IRIS.py
--rw-rw-rw-   0 runner    (1001) docker     (127)    21467 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/_IRISConnection.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     2614 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/_IRISEmbedded.py
--rw-rw-rw-   0 runner    (1001) docker     (127)    12049 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/_IRISGlobalNode.py
--rw-rw-rw-   0 runner    (1001) docker     (127)      797 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/_IRISGlobalNodeView.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     6906 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/_IRISIterator.py
--rw-rw-rw-   0 runner    (1001) docker     (127)    10247 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/_IRISList.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     6756 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/_IRISNative.py
--rw-rw-rw-   0 runner    (1001) docker     (127)      213 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/_IRISOREF.py
--rw-rw-rw-   0 runner    (1001) docker     (127)    14456 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/_IRISObject.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     4905 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/_IRISReference.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     6643 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/_InStream.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     4130 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/_LegacyIterator.py
--rw-rw-rw-   0 runner    (1001) docker     (127)      354 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/_ListItem.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     2966 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/_ListReader.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     5515 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/_ListWriter.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     3797 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/_LogFileStream.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     1662 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/_MessageHeader.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     1327 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/_OutStream.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     1963 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/_PrintStream.py
--rw-rw-rw-   0 runner    (1001) docker     (127)    41638 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/_PythonGateway.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     4330 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/_SharedMemorySocket.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     1773 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/__init__.py
--rw-rw-rw-   0 runner    (1001) docker     (127)      218 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 15:33:56.718006 django-iris-0.2.4b1/intersystems_iris/dbapi/
--rw-rw-rw-   0 runner    (1001) docker     (127)     2535 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/dbapi/_Column.py
--rw-rw-rw-   0 runner    (1001) docker     (127)   102320 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/dbapi/_DBAPI.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     1391 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/dbapi/_Descriptor.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     2115 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/dbapi/_IRISStream.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     4076 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/dbapi/_Message.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     5293 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/dbapi/_Parameter.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     5541 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/dbapi/_ParameterCollection.py
--rw-rw-rw-   0 runner    (1001) docker     (127)    12910 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/dbapi/_ResultSetRow.py
--rw-rw-rw-   0 runner    (1001) docker     (127)      557 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/dbapi/_SQLType.py
--rw-rw-rw-   0 runner    (1001) docker     (127)        0 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/dbapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 15:33:56.718006 django-iris-0.2.4b1/intersystems_iris/dbapi/preparser/
--rw-rw-rw-   0 runner    (1001) docker     (127)    78828 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/dbapi/preparser/_PreParser.py
--rw-rw-rw-   0 runner    (1001) docker     (127)    16163 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/dbapi/preparser/_Scanner.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     2304 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/dbapi/preparser/_Token.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     6770 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/dbapi/preparser/_TokenList.py
--rw-rw-rw-   0 runner    (1001) docker     (127)        0 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/dbapi/preparser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 15:33:56.722005 django-iris-0.2.4b1/intersystems_iris/pex/
--rw-rw-rw-   0 runner    (1001) docker     (127)     4370 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/pex/_BusinessHost.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     5241 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/pex/_BusinessOperation.py
--rw-rw-rw-   0 runner    (1001) docker     (127)    10774 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/pex/_BusinessProcess.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     5441 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/pex/_BusinessService.py
--rw-rw-rw-   0 runner    (1001) docker     (127)    10509 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/pex/_Common.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     1203 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/pex/_Director.py
--rw-rw-rw-   0 runner    (1001) docker     (127)      172 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/pex/_IRISBusinessOperation.py
--rw-rw-rw-   0 runner    (1001) docker     (127)      585 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/pex/_IRISBusinessService.py
--rw-rw-rw-   0 runner    (1001) docker     (127)      171 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/pex/_IRISInboundAdapter.py
--rw-rw-rw-   0 runner    (1001) docker     (127)      522 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/pex/_IRISOutboundAdapter.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     2296 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/pex/_InboundAdapter.py
--rw-rw-rw-   0 runner    (1001) docker     (127)      320 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/pex/_Message.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     1628 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/pex/_OutboundAdapter.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     1379 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/intersystems_iris/pex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 15:33:56.722005 django-iris-0.2.4b1/irisnative/
--rw-rw-rw-   0 runner    (1001) docker     (127)      665 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/irisnative/_IRISNative.py
--rw-rw-rw-   0 runner    (1001) docker     (127)      341 2023-12-19 15:33:56.000000 django-iris-0.2.4b1/irisnative/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2023-12-19 15:33:56.722005 django-iris-0.2.4b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      541 2023-12-19 15:33:38.000000 django-iris-0.2.4b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:52:39.892733 django_iris-0.2.5b1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-20 12:52:28.000000 django_iris-0.2.5b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-20 12:52:39.892733 django_iris-0.2.5b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-20 12:52:28.000000 django_iris-0.2.5b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:52:39.876733 django_iris-0.2.5b1/django_iris/
+-rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-05-20 12:52:28.000000 django_iris-0.2.5b1/django_iris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7164 2024-05-20 12:52:28.000000 django_iris-0.2.5b1/django_iris/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7738 2024-05-20 12:52:28.000000 django_iris-0.2.5b1/django_iris/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-20 12:52:28.000000 django_iris-0.2.5b1/django_iris/creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-20 12:52:28.000000 django_iris-0.2.5b1/django_iris/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8729 2024-05-20 12:52:28.000000 django_iris-0.2.5b1/django_iris/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10444 2024-05-20 12:52:28.000000 django_iris-0.2.5b1/django_iris/introspection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13484 2024-05-20 12:52:28.000000 django_iris-0.2.5b1/django_iris/operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-20 12:52:28.000000 django_iris-0.2.5b1/django_iris/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-05-20 12:52:28.000000 django_iris-0.2.5b1/django_iris/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-20 12:52:28.000000 django_iris-0.2.5b1/django_iris/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-20 12:52:28.000000 django_iris-0.2.5b1/django_iris/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:52:39.892733 django_iris-0.2.5b1/django_iris.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/django_iris.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/django_iris.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/django_iris.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/django_iris.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:52:39.884733 django_iris-0.2.5b1/intersystems_iris/
+-rw-rw-rw-   0 runner    (1001) docker     (127)      299 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_BufferReader.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     1337 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_BufferWriter.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     1896 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_ConnectionInformation.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)      578 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_ConnectionParameters.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     1483 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_Constant.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)    20104 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_DBList.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     2311 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_Device.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)      618 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_GatewayContext.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)       96 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_GatewayException.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     2735 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_GatewayUtility.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)    49548 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_IRIS.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)    21467 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_IRISConnection.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     2614 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_IRISEmbedded.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)    12049 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_IRISGlobalNode.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)      797 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_IRISGlobalNodeView.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     6906 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_IRISIterator.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)    10247 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_IRISList.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     6756 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_IRISNative.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)      213 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_IRISOREF.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)    14456 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_IRISObject.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     4905 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_IRISReference.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     6643 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_InStream.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     4130 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_LegacyIterator.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)      354 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_ListItem.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     2966 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_ListReader.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     5515 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_ListWriter.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     3797 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_LogFileStream.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     1662 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_MessageHeader.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     1327 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_OutStream.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     1963 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_PrintStream.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)    41638 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_PythonGateway.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     4330 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_SharedMemorySocket.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     1773 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/__init__.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)      218 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:52:39.888733 django_iris-0.2.5b1/intersystems_iris/dbapi/
+-rw-rw-rw-   0 runner    (1001) docker     (127)     2535 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/dbapi/_Column.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)   102320 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/dbapi/_DBAPI.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     1391 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/dbapi/_Descriptor.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     2115 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/dbapi/_IRISStream.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     4076 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/dbapi/_Message.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     5293 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/dbapi/_Parameter.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     5541 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/dbapi/_ParameterCollection.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)    12910 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/dbapi/_ResultSetRow.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)      557 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/dbapi/_SQLType.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)        0 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/dbapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:52:39.888733 django_iris-0.2.5b1/intersystems_iris/dbapi/preparser/
+-rw-rw-rw-   0 runner    (1001) docker     (127)    78828 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/dbapi/preparser/_PreParser.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)    16163 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/dbapi/preparser/_Scanner.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     2304 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/dbapi/preparser/_Token.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     6770 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/dbapi/preparser/_TokenList.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)        0 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/dbapi/preparser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:52:39.888733 django_iris-0.2.5b1/intersystems_iris/pex/
+-rw-rw-rw-   0 runner    (1001) docker     (127)     4370 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/pex/_BusinessHost.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     5241 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/pex/_BusinessOperation.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)    10774 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/pex/_BusinessProcess.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     5441 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/pex/_BusinessService.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)    10509 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/pex/_Common.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     1203 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/pex/_Director.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)      172 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/pex/_IRISBusinessOperation.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)      585 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/pex/_IRISBusinessService.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)      171 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/pex/_IRISInboundAdapter.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)      522 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/pex/_IRISOutboundAdapter.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     2296 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/pex/_InboundAdapter.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)      320 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/pex/_Message.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     1628 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/pex/_OutboundAdapter.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     1379 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/pex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:52:39.892733 django_iris-0.2.5b1/irisnative/
+-rw-rw-rw-   0 runner    (1001) docker     (127)      665 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/irisnative/_IRISNative.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)      341 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/irisnative/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-20 12:52:39.892733 django_iris-0.2.5b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-20 12:52:28.000000 django_iris-0.2.5b1/setup.py
```

### Comparing `django-iris-0.2.4b1/LICENSE` & `django_iris-0.2.5b1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/PKG-INFO` & `django_iris-0.2.5b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-iris
-Version: 0.2.4b1
+Version: 0.2.5b1
 Summary: Django backend for InterSystems IRIS
 Home-page: https://github.com/caretdev/django-iris
 Maintainer: CaretDev
 Maintainer-email: dmitry@caretdev.com
 License: MIT
 Project-URL: Source, https://github.com/caretdev/django-iris
 Project-URL: Tracker, https://github.com/caretdev/django-iris/issues
```

### Comparing `django-iris-0.2.4b1/README.md` & `django_iris-0.2.5b1/README.md`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/django_iris/__init__.py` & `django_iris-0.2.5b1/django_iris/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from django.db.models.functions.math import Random, Ln, Log
 from django.db.models.functions.datetime import Now
 from django.db.models.expressions import Exists, Func, Value, Col, OrderBy
 from django.db.models.functions.text import Chr, ConcatPair, StrIndex
 from django.db.models.fields import TextField, CharField
 
+from django_iris.compiler import SQLCompiler
+
 fn_template = "{fn %(function)s(%(expressions)s)}"
 
 as_fn = [
     "ACOS",
     "ASIN",
     "ATAN",
     "ATAN2",
@@ -18,116 +20,134 @@
     "LOG",
     "LOG10",
     "PI",
     "SIN",
     "TAN",
 ]
 
+
 def as_intersystems(cls):
     def inner(func):
         cls.as_intersystems = func
+
     return inner
 
+
 class Log10(Func):
     function = "LOG10"
     arity = 1
     lookup_name = "log10"
 
+
 class Convert(Func):
     function = "CONVERT"
     lookup_name = "convert"
 
     template = "%(function)s(%(db_type)s, %(expressions)s)"
 
     def __init__(self, expression, output_field):
         super().__init__(expression, output_field=output_field)
 
     def as_sql(self, compiler, connection, **extra_context):
         extra_context["db_type"] = self.output_field.cast_db_type(connection)
         return super().as_sql(compiler, connection, **extra_context)
 
+
 def convert_streams(expressions):
     return [
-        Convert(expression, CharField()) if isinstance(expression, Col) and isinstance(expression.target, TextField) else expression
+        (
+            Convert(expression, CharField())
+            if isinstance(expression, Col) and isinstance(expression.target, TextField)
+            else expression
+        )
         for expression in expressions
     ]
 
+
 @as_intersystems(Exists)
 def exists_as_intersystems(self, compiler, connection, template=None, **extra_context):
     template = "(SELECT COUNT(*) FROM (%(subquery)s))"
     return self.as_sql(compiler, connection, template, **extra_context)
 
+
 @as_intersystems(Chr)
 def chr_as_intersystems(self, compiler, connection, **extra_context):
     return self.as_sql(compiler, connection, function="CHAR", **extra_context)
 
+
 @as_intersystems(ConcatPair)
 def concat_as_intersystems(self, compiler, connection, **extra_context):
     copy = self.copy()
     expressions = convert_streams(copy.get_source_expressions())
     """
     STRING in IRIS retuns NULL if all NULL arguments, so, just add empty string, to make it always non NULL
     """
-    copy.set_source_expressions([Value("")]+ expressions)
+    copy.set_source_expressions([Value("")] + expressions)
     return super(ConcatPair, copy).as_sql(
         compiler,
         connection,
         function="STRING",
         **extra_context,
     )
 
+
 @as_intersystems(StrIndex)
 def instr_as_intersystems(self, compiler, connection, **extra_context):
     copy = self.copy()
     expressions = convert_streams(copy.get_source_expressions())
     copy.set_source_expressions(expressions)
     return super(StrIndex, copy).as_sql(
         compiler,
         connection,
         **extra_context,
     )
 
+
 @as_intersystems(Random)
 def random_as_intersystems(self, compiler, connection, **extra_context):
-    return self.as_sql(compiler, connection, template="%%TSQL.ZRAND(1e10)", **extra_context)
+    return self.as_sql(
+        compiler, connection, template="%%TSQL.ZRAND(1e10)", **extra_context
+    )
+
 
 @as_intersystems(Ln)
 def ln_as_intersystems(self, compiler, connection, **extra_context):
-    return self.as_sql(compiler, connection, function="LOG", template=fn_template, **extra_context)
+    return self.as_sql(
+        compiler, connection, function="LOG", template=fn_template, **extra_context
+    )
 
 
 @as_intersystems(Log)
 def log_as_intersystems(self, compiler, connection, **extra_context):
     copy = self.copy()
     copy.set_source_expressions(
-        [
-            Log10(expression)
-            for expression in copy.get_source_expressions()[::-1]
-        ]
+        [Log10(expression) for expression in copy.get_source_expressions()[::-1]]
     )
     return super(Log, copy).as_sql(
         compiler,
         connection,
         arg_joiner=" / ",
         template="%(expressions)s",
         **extra_context,
     )
 
+
 @as_intersystems(Func)
-def func_as_intersystems(self, compiler, connection, **extra_context):
-    if self.function in as_fn:        
+def func_as_intersystems(self, compiler: SQLCompiler, connection, **extra_context):
+    if self.function in as_fn:
         return self.as_sql(compiler, connection, template=fn_template, **extra_context)
     return self.as_sql(compiler, connection, **extra_context)
 
+
 @as_intersystems(Now)
 def now_as_intersystems(self, compiler, connection, **extra_context):
     return self.as_sql(
         compiler, connection, template="CURRENT_TIMESTAMP(6)", **extra_context
     )
 
+
 @as_intersystems(OrderBy)
 def orderby_as_intersystems(self, compiler, connection, **extra_context):
     copy = self.copy()
     # IRIS does not support order NULL
-    copy.nulls_first =  copy.nulls_last = False
+    copy.nulls_first = copy.nulls_last = False
     return copy.as_sql(compiler, connection, **extra_context)
-
```

### Comparing `django-iris-0.2.4b1/django_iris/base.py` & `django_iris-0.2.5b1/django_iris/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,74 +20,74 @@
 def ignore(*args, **kwargs):
     pass
 
 
 class DatabaseClient(BaseDatabaseClient):
     runshell = ignore
 
+
 class DatabaseWrapper(BaseDatabaseWrapper):
-    vendor = 'intersystems'
-    display_name = 'InterSystems IRIS'
+    vendor = "intersystems"
+    display_name = "InterSystems IRIS"
 
     data_types = {
-        'AutoField': 'IDENTITY',
-        'BigAutoField': 'IDENTITY',
-        'BinaryField': 'LONG BINARY',
-        'BooleanField': 'BIT',
-        'CharField': 'VARCHAR(%(max_length)s)',
-        'DateField': 'DATE',
-        'DateTimeField': 'TIMESTAMP',
-        'DecimalField': 'NUMERIC(%(max_digits)s, %(decimal_places)s)',
-        'DurationField': 'BIGINT',
-        'FileField': 'VARCHAR(%(max_length)s)',
-        'FilePathField': 'VARCHAR(%(max_length)s)',
-        'FloatField': 'DOUBLE PRECISION',
-        'IntegerField': 'INTEGER',
-        'BigIntegerField': 'BIGINT',
-        'IPAddressField': 'CHAR(15)',
-        'GenericIPAddressField': 'CHAR(39)',
-        'JSONField': 'VARCHAR(32768)',
-        'OneToOneField': 'INTEGER',
-        'PositiveBigIntegerField': 'BIGINT',
-        'PositiveIntegerField': 'INTEGER',
-        'PositiveSmallIntegerField': 'SMALLINT',
-        'SlugField': 'VARCHAR(%(max_length)s)',
-        'SmallAutoField': 'IDENTITY',
-        'SmallIntegerField': 'SMALLINT',
-        'TextField': 'TEXT',
-        'TimeField': 'TIME(6)',
-        'UUIDField': 'CHAR(32)',
+        "AutoField": "IDENTITY",
+        "BigAutoField": "IDENTITY",
+        "BinaryField": "LONG BINARY",
+        "BooleanField": "BIT",
+        "CharField": "VARCHAR(%(max_length)s)",
+        "DateField": "DATE",
+        "DateTimeField": "TIMESTAMP",
+        "DecimalField": "NUMERIC(%(max_digits)s, %(decimal_places)s)",
+        "DurationField": "BIGINT",
+        "FileField": "VARCHAR(%(max_length)s)",
+        "FilePathField": "VARCHAR(%(max_length)s)",
+        "FloatField": "DOUBLE PRECISION",
+        "IntegerField": "INTEGER",
+        "BigIntegerField": "BIGINT",
+        "IPAddressField": "CHAR(15)",
+        "GenericIPAddressField": "CHAR(39)",
+        "JSONField": "VARCHAR(32768)",
+        "OneToOneField": "INTEGER",
+        "PositiveBigIntegerField": "BIGINT",
+        "PositiveIntegerField": "INTEGER",
+        "PositiveSmallIntegerField": "SMALLINT",
+        "SlugField": "VARCHAR(%(max_length)s)",
+        "SmallAutoField": "IDENTITY",
+        "SmallIntegerField": "SMALLINT",
+        "TextField": "TEXT",
+        "TimeField": "TIME(6)",
+        "UUIDField": "UNIQUEIDENTIFIER",
     }
 
     operators = {
-        'exact': '= %s',
-        'iexact': "LIKE %s ESCAPE '\\'",
-        'contains': "LIKE %s ESCAPE '\\'",
-        'icontains': "LIKE %s ESCAPE '\\'",
+        "exact": "= %s",
+        "iexact": "LIKE %s ESCAPE '\\'",
+        "contains": "LIKE %s ESCAPE '\\'",
+        "icontains": "LIKE %s ESCAPE '\\'",
         # 'regex': "%%%%MATCHES %s ESCAPE '\\'",
         # 'iregex': "%%%%MATCHES %s ESCAPE '\\'",
-        'gt': '> %s',
-        'gte': '>= %s',
-        'lt': '< %s',
-        'lte': '<= %s',
-        'startswith': "LIKE %s ESCAPE '\\'",
-        'endswith': "LIKE %s ESCAPE '\\'",
-        'istartswith': "LIKE %s ESCAPE '\\'",
-        'iendswith': "LIKE %s ESCAPE '\\'",
+        "gt": "> %s",
+        "gte": ">= %s",
+        "lt": "< %s",
+        "lte": "<= %s",
+        "startswith": "LIKE %s ESCAPE '\\'",
+        "endswith": "LIKE %s ESCAPE '\\'",
+        "istartswith": "LIKE %s ESCAPE '\\'",
+        "iendswith": "LIKE %s ESCAPE '\\'",
     }
 
     pattern_esc = r"REPLACE(REPLACE(REPLACE({}, '\', '\\'), '%%', '\%%'), '_', '\_')"
     pattern_ops = {
         "contains": "LIKE '%%' || {} || '%%'",
         "icontains": "LIKE '%%' || UPPER({}) || '%%'",
         "startswith": "LIKE {} || '%%'",
         "istartswith": "LIKE UPPER({}) || '%%'",
         "endswith": "LIKE '%%' || {}",
         "iendswith": "LIKE '%%' || UPPER({})",
-
     }
 
     Database = Database
 
     # _commit = ignore
     # _rollback = ignore
     # _savepoint = ignore
@@ -106,70 +106,67 @@
 
     _disable_constraint_checking = False
 
     def get_connection_params(self):
         settings_dict = self.settings_dict
 
         conn_params = {
-            'username': None,
-            'password': None,
-            'timeout': 30,
+            "username": None,
+            "password": None,
+            "timeout": 30,
         }
-        if settings_dict['USER']:
-            conn_params['username'] = settings_dict['USER']
-        if settings_dict['PASSWORD']:
-            conn_params['password'] = settings_dict['PASSWORD']
-        if 'TIMEOUT' in settings_dict:
-            conn_params['timeout'] = settings_dict['TIMEOUT']
-        if 'EMBEDDED' in settings_dict:
-            conn_params['embedded'] = settings_dict['EMBEDDED']
-        if 'CONNECTION_STRING' in settings_dict:
-            conn_params['connectionstr'] = settings_dict['CONNECTION_STRING']
+        if settings_dict["USER"]:
+            conn_params["username"] = settings_dict["USER"]
+        if settings_dict["PASSWORD"]:
+            conn_params["password"] = settings_dict["PASSWORD"]
+        if "TIMEOUT" in settings_dict:
+            conn_params["timeout"] = settings_dict["TIMEOUT"]
+        if "EMBEDDED" in settings_dict:
+            conn_params["embedded"] = settings_dict["EMBEDDED"]
+        if "CONNECTION_STRING" in settings_dict:
+            conn_params["connectionstr"] = settings_dict["CONNECTION_STRING"]
         else:
             conn_params = {
-                'hostname': 'localhost',
-                'port': 1972,
-                'namespace': 'USER',
+                "hostname": "localhost",
+                "port": 1972,
+                "namespace": "USER",
                 **conn_params,
             }
-            if settings_dict['HOST']:
-                conn_params['hostname'] = settings_dict['HOST']
-            if settings_dict['PORT']:
-                conn_params['port'] = settings_dict['PORT']
-            if 'NAMESPACE' in settings_dict:
-                conn_params['namespace'] = settings_dict['NAMESPACE']
-            if settings_dict['NAME']:
-                conn_params['namespace'] = settings_dict['NAME']
+            if settings_dict["HOST"]:
+                conn_params["hostname"] = settings_dict["HOST"]
+            if settings_dict["PORT"]:
+                conn_params["port"] = settings_dict["PORT"]
+            if "NAMESPACE" in settings_dict:
+                conn_params["namespace"] = settings_dict["NAMESPACE"]
+            if settings_dict["NAME"]:
+                conn_params["namespace"] = settings_dict["NAME"]
 
             if (
-                not conn_params['hostname'] or
-                not conn_params['port'] or
-                not conn_params['namespace']
+                not conn_params["hostname"]
+                or not conn_params["port"]
+                or not conn_params["namespace"]
             ):
                 raise ImproperlyConfigured(
                     "settings.DATABASES is improperly configured. "
                     "Please supply the HOST, PORT and NAME"
                 )
 
-        if (
-            not conn_params['username'] or
-            not conn_params['password']
-        ):
+        if not conn_params["username"] or not conn_params["password"]:
             raise ImproperlyConfigured(
                 "settings.DATABASES is improperly configured. "
                 "Please supply the USER and PASSWORD"
             )
 
-        conn_params['application_name'] = 'django'
+        conn_params["application_name"] = "django"
         conn_params["autoCommit"] = self.autocommit
         return conn_params
 
     def init_connection_state(self):
         pass
-    
+
     @async_unsafe
     def get_new_connection(self, conn_params):
         return Database.connect(**conn_params)
 
     def _close(self):
         if self.connection is not None:
             # Automatically rollbacks anyway
@@ -182,15 +179,15 @@
     def create_cursor(self, name=None):
         cursor = self.connection.cursor()
         return CursorWrapper(cursor)
 
     def is_usable(self):
         try:
             with self.connection.cursor() as cursor:
-                cursor.execute('SELECT 1')
+                cursor.execute("SELECT 1")
         except:
             return False
         else:
             return True
 
     @cached_property
     def wrap_database_errors(self):
```

### Comparing `django-iris-0.2.4b1/django_iris/compiler.py` & `django_iris-0.2.5b1/django_iris/compiler.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/django_iris/creation.py` & `django_iris-0.2.5b1/django_iris/creation.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/django_iris/cursor.py` & `django_iris-0.2.5b1/django_iris/cursor.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/django_iris/features.py` & `django_iris-0.2.5b1/django_iris/features.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from django.db.backends.base.features import BaseDatabaseFeatures
 from django.db import InterfaceError
 from django.utils.functional import cached_property
 
+
 class DatabaseFeatures(BaseDatabaseFeatures):
     empty_fetchmany_value = []
 
     requires_literal_defaults = True
-    
+
     supports_paramstyle_pyformat = False
-    
+
     supports_transactions = True
     uses_savepoints = True
-    has_bulk_insert =  True
-    has_native_uuid_field =  False
+    has_bulk_insert = True
+    has_native_uuid_field = True
     supports_timezones = False
     has_zoneinfo_database = False
-    can_clone_databases =  True
+    can_clone_databases = True
     test_db_allows_multiple_connections = False
-    supports_unspecified_pk =  False
+    supports_unspecified_pk = False
     can_return_columns_from_insert = False
 
     # Does the backend support NULLS FIRST and NULLS LAST in ORDER BY?
     supports_order_by_nulls_modifier = False
 
     # Does the backend orders NULLS FIRST by default?
     order_by_nulls_first = False
@@ -56,17 +57,21 @@
     supports_column_check_constraints = False
     supports_table_check_constraints = False
     can_introspect_check_constraints = False
 
     interprets_empty_strings_as_nulls = False
 
     supports_ignore_conflicts = False
-    
+
     closed_cursor_error_class = InterfaceError
 
+    # Does the backend support functions in defaults?
+    # IRIS, requires ObjectScript there, no way
+    supports_expression_defaults = False
+
     # Does the backend support partial indexes (CREATE INDEX ... WHERE ...)?
     supports_partial_indexes = False
     supports_functions_in_partial_indexes = False
     # Does the backend support covering indexes (CREATE INDEX ... INCLUDE ...)?
     supports_covering_indexes = False
     # Does the backend support indexes on expressions?
     supports_expression_indexes = False
@@ -103,85 +108,91 @@
 
     # Collation names for use by the Django test suite.
     test_collations = {
         # "ci": None,  # Case-insensitive.
         "cs": "EXACT",  # Case-sensitive.
         # "non_default": None,  # Non-default.
         # "swedish_ci": None,  # Swedish case-insensitive.
+        "virtual": None
     }
 
-    django_test_skips = {
-        "IRIS doesn't support Hash functions.": {
-            "db_functions.text.test_md5.MD5Tests.test_basic",
-            "db_functions.text.test_md5.MD5Tests.test_transform",
-            "db_functions.text.test_sha1.SHA1Tests.test_basic",
-            "db_functions.text.test_sha1.SHA1Tests.test_transform",
-            "db_functions.text.test_sha224.SHA224Tests.test_basic",
-            "db_functions.text.test_sha224.SHA224Tests.test_transform",
-            "db_functions.text.test_sha256.SHA256Tests.test_basic",
-            "db_functions.text.test_sha256.SHA256Tests.test_transform",
-            "db_functions.text.test_sha384.SHA384Tests.test_basic",
-            "db_functions.text.test_sha384.SHA384Tests.test_transform",
-            "db_functions.text.test_sha512.SHA512Tests.test_basic",
-            "db_functions.text.test_sha512.SHA512Tests.test_transform",
-        },
-        "Unexpected result for RPAD/LPAD with 0 as length": {
-            "db_functions.text.test_pad.PadTests.test_pad",
-        },
-        "IRIS has bugs with renaming": {
-            "schema.tests.SchemaTests.test_alter_pk_with_self_referential_field",
-            "schema.tests.SchemaTests.test_alter_to_fk",
-            "schema.tests.SchemaTests.test_char_field_with_db_index_to_fk",
-            "schema.tests.SchemaTests.test_db_table",
-            "schema.tests.SchemaTests.test_m2m_repoint_custom",
-            "schema.tests.SchemaTests.test_m2m_repoint_inherited",
-            "schema.tests.SchemaTests.test_m2m_repoint",
-            "schema.tests.SchemaTests.test_rename_referenced_field",
-            "schema.tests.SchemaTests.test_text_field_with_db_index_to_fk",
-            "schema.tests.SchemaTests.test_rename_table_renames_deferred_sql_references",
-            "schema.tests.SchemaTests.test_rename_keep_null_status",
-            "schema.tests.SchemaTests.test_rename_column_renames_deferred_sql_references",
-            "schema.tests.SchemaTests.test_rename",
-        },
-        "IRIS does not care about ASC/DESC in index": {
-            "schema.tests.SchemaTests.test_order_index",
-        },
-        "Bug on IRIS side, add DATE column with default value on existing data": {
-            "schema.tests.SchemaTests.test_add_datefield_and_datetimefield_use_effective_default",
-        },
-        "No idea what's to do here": {
-            "datetimes.tests.DateTimesTests.test_datetimes_ambiguous_and_invalid_times",
-        },
-        "IRIS does not have check contsraints": {
-            "constraints.tests.CheckConstraintTests.test_validate",
-            "constraints.tests.CheckConstraintTests.test_validate_boolean_expressions",
-            "constraints.tests.UniqueConstraintTests.test_validate_expression_condition",
-        }
-    }
-    
+    @cached_property
+    def django_test_skips(self):
+        skips = super().django_test_skips
+        skips.update(
+            {
+                "IRIS doesn't support Hash functions.": {
+                    "db_functions.text.test_md5.MD5Tests.test_basic",
+                    "db_functions.text.test_md5.MD5Tests.test_transform",
+                    "db_functions.text.test_sha1.SHA1Tests.test_basic",
+                    "db_functions.text.test_sha1.SHA1Tests.test_transform",
+                    "db_functions.text.test_sha224.SHA224Tests.test_basic",
+                    "db_functions.text.test_sha224.SHA224Tests.test_transform",
+                    "db_functions.text.test_sha256.SHA256Tests.test_basic",
+                    "db_functions.text.test_sha256.SHA256Tests.test_transform",
+                    "db_functions.text.test_sha384.SHA384Tests.test_basic",
+                    "db_functions.text.test_sha384.SHA384Tests.test_transform",
+                    "db_functions.text.test_sha512.SHA512Tests.test_basic",
+                    "db_functions.text.test_sha512.SHA512Tests.test_transform",
+                },
+                "Unexpected result for RPAD/LPAD with 0 as length": {
+                    "db_functions.text.test_pad.PadTests.test_pad",
+                },
+                "IRIS has bugs with renaming": {
+                    "schema.tests.SchemaTests.test_alter_pk_with_self_referential_field",
+                    "schema.tests.SchemaTests.test_alter_to_fk",
+                    "schema.tests.SchemaTests.test_char_field_with_db_index_to_fk",
+                    "schema.tests.SchemaTests.test_db_table",
+                    "schema.tests.SchemaTests.test_m2m_repoint_custom",
+                    "schema.tests.SchemaTests.test_m2m_repoint_inherited",
+                    "schema.tests.SchemaTests.test_m2m_repoint",
+                    "schema.tests.SchemaTests.test_rename_referenced_field",
+                    "schema.tests.SchemaTests.test_text_field_with_db_index_to_fk",
+                    "schema.tests.SchemaTests.test_rename_table_renames_deferred_sql_references",
+                    "schema.tests.SchemaTests.test_rename_keep_null_status",
+                    "schema.tests.SchemaTests.test_rename_column_renames_deferred_sql_references",
+                    "schema.tests.SchemaTests.test_rename",
+                },
+                "IRIS does not care about ASC/DESC in index": {
+                    "schema.tests.SchemaTests.test_order_index",
+                },
+                "Bug on IRIS side, add DATE column with default value on existing data": {
+                    "schema.tests.SchemaTests.test_add_datefield_and_datetimefield_use_effective_default",
+                },
+                # "No idea what's to do here": {
+                #     "datetimes.tests.DateTimesTests.test_datetimes_ambiguous_and_invalid_times",
+                # },
+                "IRIS does not have check contsraints": {
+                    "constraints.tests.CheckConstraintTests.test_validate",
+                    "constraints.tests.CheckConstraintTests.test_validate_boolean_expressions",
+                    "constraints.tests.UniqueConstraintTests.test_validate_expression_condition",
+                },
+            }
+
+        )
+        return skips
+
     django_test_expected_failures = {
         # IRIS does not support DROP IDENTITY, and changing IDENTITY on fly
         "schema.tests.SchemaTests.test_alter_auto_field_to_char_field",
         "schema.tests.SchemaTests.test_alter_auto_field_to_integer_field",
         "schema.tests.SchemaTests.test_autofield_to_o2o",
         "schema.tests.SchemaTests.test_alter_int_pk_to_autofield_pk",
         "schema.tests.SchemaTests.test_alter_int_pk_to_bigautofield_pk",
         "schema.tests.SchemaTests.test_alter_smallint_pk_to_smallautofield_pk",
         "schema.tests.SchemaTests.test_char_field_pk_to_auto_field",
-
         # ADD COLUMN does not create unique indexes
         "schema.tests.SchemaTests.test_indexes",
-
         # Change column datatype to/from TextField (IRIS Streams)
         "schema.tests.SchemaTests.test_alter_text_field_to_time_field",
         "schema.tests.SchemaTests.test_alter_text_field_to_datetime_field",
         "schema.tests.SchemaTests.test_alter_text_field_to_date_field",
     }
 
-    # django_test_skips["IRIS Bugs"] = django_test_expected_failures    
+    # django_test_skips["IRIS Bugs"] = django_test_expected_failures
 
     @cached_property
     def introspected_field_types(self):
         return {
             **super().introspected_field_types,
             "BigAutoField": "AutoField",
             "DurationField": "BigIntegerField",
```

### Comparing `django-iris-0.2.4b1/django_iris/introspection.py` & `django_iris-0.2.5b1/django_iris/introspection.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/django_iris/operations.py` & `django_iris-0.2.5b1/django_iris/operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,27 +172,32 @@
             return None
 
         if timezone.is_aware(value):
             raise ValueError("IRIS backend does not support timezone-aware times.")
 
         return str(value)
 
-    def field_cast_sql(self, db_type, internal_type):
-        """
-        Given a column type (e.g. 'BLOB', 'VARCHAR') and an internal type
-        (e.g. 'GenericIPAddressField'), return the SQL to cast it before using
-        it in a WHERE statement. The resulting string should contain a '%s'
-        placeholder for the column being searched against.
-        
-        IRIS cannot work with streams directly in WHERE, wrap it with CONVERT
-        """
-        if db_type in ('TEXT', 'LONG BINARY'):
+    # def field_cast_sql(self, db_type, internal_type):
+    #     """
+    #     Given a column type (e.g. 'BLOB', 'VARCHAR') and an internal type
+    #     (e.g. 'GenericIPAddressField'), return the SQL to cast it before using
+    #     it in a WHERE statement. The resulting string should contain a '%s'
+    #     placeholder for the column being searched against.
+
+    #     IRIS cannot work with streams directly in WHERE, wrap it with CONVERT
+    #     """
+    #     if db_type in ('TEXT', 'LONG BINARY'):
+    #         return "CONVERT(VARCHAR, %s)"
+    #     return "%s"
+
+    def lookup_cast(self, lookup_type, internal_type=None):
+        if lookup_type in ('TEXT', 'LONG BINARY'):
             return "CONVERT(VARCHAR, %s)"
         return "%s"
-    
+
     def max_name_length(self):
         """
         Return the maximum length of table and column names, or None if there
         is no limit.
         """
         return 60
```

### Comparing `django-iris-0.2.4b1/django_iris/schema.py` & `django_iris-0.2.5b1/django_iris/schema.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from django.db.backends.base.schema import BaseDatabaseSchemaEditor
 from django.db import NotSupportedError, models
 
 
 class DatabaseSchemaEditor(BaseDatabaseSchemaEditor):
 
     sql_create_table = (
-        "CREATE TABLE %(table)s (%(definition)s)" 
+        "CREATE TABLE %(table)s (%(definition)s)"
         "WITH %%%%CLASSPARAMETER ALLOWIDENTITYINSERT = 1"
     )
 
     sql_alter_column_type = "ALTER COLUMN %(column)s %(type)s"
     sql_alter_column_collation = "ALTER COLUMN %(column)s %(collation)s"
     sql_alter_column_null = "ALTER COLUMN %(column)s NULL"
     sql_alter_column_not_null = "ALTER COLUMN %(column)s NOT NULL"
@@ -35,19 +35,19 @@
 
     def quote_value(self, value):
         if isinstance(value, bool):
             return str(int(value))
         elif isinstance(value, (Decimal, float, int)):
             return str(value)
         elif isinstance(value, str):
-            return "'%s'" % value.replace("\'", "\'\'")
+            return "'%s'" % value.replace("'", "''")
         elif value is None:
             return "NULL"
         elif isinstance(value, bytes):
-            return "'%s'" % value.decode().replace("\'", "\'\'")
+            return "'%s'" % value.decode().replace("'", "''")
         return value
 
     def quote_name(self, name):
         # if '.' in name:
         #     return name
         return self.connection.ops.quote_name(name)
 
@@ -61,17 +61,17 @@
     #         )
     #     return super().table_sql(model)
 
     def _create_fk_sql(self, model, field, suffix):
         on_delete = getattr(field.remote_field, "on_delete", None)
         stmt = super()._create_fk_sql(model, field, suffix)
         if on_delete == models.CASCADE:
-            stmt = str(stmt) + ' ON DELETE CASCADE'
+            stmt = str(stmt) + " ON DELETE CASCADE"
         if on_delete == models.SET_NULL:
-            stmt = str(stmt) + ' ON DELETE SET NULL'
+            stmt = str(stmt) + " ON DELETE SET NULL"
         return stmt
 
     # def _rename_field_sql(self, table, old_field, new_field, new_type):
     #     return self.sql_rename_column % {
     #         "table": self.quote_name(table),
     #         "old_column": self.quote_name(old_field.column),
     #         "new_column": self.quote_name(new_field.column),
@@ -81,39 +81,41 @@
     def _collate_sql(self, collation, old_collation=None, table_name=None):
         return f"COLLATE {collation}"
 
     def _alter_column_type_sql(
         self, model, old_field, new_field, new_type, old_collation, new_collation
     ):
 
-        action, other_actions = super()._alter_column_type_sql(model, old_field, new_field, new_type, None, None)
+        action, other_actions = super()._alter_column_type_sql(
+            model, old_field, new_field, new_type, None, None
+        )
         if not new_collation:
             return action, other_actions
 
         if collate_sql := self._collate_sql(
             new_collation, old_collation, model._meta.db_table
         ):
             collate_sql = f" {collate_sql}"
         else:
             collate_sql = ""
 
         other_actions += [
             (
-            self.sql_alter_column
-            % {
-                "table": self.quote_name(model._meta.db_table),
-                "changes": (
-                    self.sql_alter_column_collation
-                    % {
-                        "column": self.quote_name(new_field.column),
-                        "collation": collate_sql
-                    }
-                ),
-            },
-            []
+                self.sql_alter_column
+                % {
+                    "table": self.quote_name(model._meta.db_table),
+                    "changes": (
+                        self.sql_alter_column_collation
+                        % {
+                            "column": self.quote_name(new_field.column),
+                            "collation": collate_sql,
+                        }
+                    ),
+                },
+                [],
             )
         ]
-        
+
         return action, other_actions
 
     def _index_condition_sql(self, condition):
         return ""
```

### Comparing `django-iris-0.2.4b1/django_iris/utils.py` & `django_iris-0.2.5b1/django_iris/utils.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/django_iris.egg-info/PKG-INFO` & `django_iris-0.2.5b1/django_iris.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-iris
-Version: 0.2.4b1
+Version: 0.2.5b1
 Summary: Django backend for InterSystems IRIS
 Home-page: https://github.com/caretdev/django-iris
 Maintainer: CaretDev
 Maintainer-email: dmitry@caretdev.com
 License: MIT
 Project-URL: Source, https://github.com/caretdev/django-iris
 Project-URL: Tracker, https://github.com/caretdev/django-iris/issues
```

### Comparing `django-iris-0.2.4b1/django_iris.egg-info/SOURCES.txt` & `django_iris-0.2.5b1/django_iris.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 django_iris/base.py
 django_iris/compiler.py
 django_iris/creation.py
 django_iris/cursor.py
 django_iris/features.py
 django_iris/introspection.py
 django_iris/operations.py
+django_iris/runner.py
 django_iris/schema.py
 django_iris/utils.py
 django_iris/validation.py
 django_iris.egg-info/PKG-INFO
 django_iris.egg-info/SOURCES.txt
 django_iris.egg-info/dependency_links.txt
 django_iris.egg-info/top_level.txt
```

### Comparing `django-iris-0.2.4b1/intersystems_iris/_BufferWriter.py` & `django_iris-0.2.5b1/intersystems_iris/_BufferWriter.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/intersystems_iris/_ConnectionInformation.py` & `django_iris-0.2.5b1/intersystems_iris/_ConnectionInformation.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/intersystems_iris/_ConnectionParameters.py` & `django_iris-0.2.5b1/intersystems_iris/_ConnectionParameters.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/intersystems_iris/_Constant.py` & `django_iris-0.2.5b1/intersystems_iris/_Constant.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/intersystems_iris/_DBList.py` & `django_iris-0.2.5b1/intersystems_iris/_DBList.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/intersystems_iris/_Device.py` & `django_iris-0.2.5b1/intersystems_iris/_Device.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/intersystems_iris/_GatewayContext.py` & `django_iris-0.2.5b1/intersystems_iris/_GatewayContext.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/intersystems_iris/_GatewayUtility.py` & `django_iris-0.2.5b1/intersystems_iris/_GatewayUtility.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/intersystems_iris/_IRIS.py` & `django_iris-0.2.5b1/intersystems_iris/_IRIS.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/intersystems_iris/_IRISConnection.py` & `django_iris-0.2.5b1/intersystems_iris/_IRISConnection.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/intersystems_iris/_IRISEmbedded.py` & `django_iris-0.2.5b1/intersystems_iris/_IRISEmbedded.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/intersystems_iris/_IRISGlobalNode.py` & `django_iris-0.2.5b1/intersystems_iris/_IRISGlobalNode.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/intersystems_iris/_IRISGlobalNodeView.py` & `django_iris-0.2.5b1/intersystems_iris/_IRISGlobalNodeView.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/intersystems_iris/_IRISIterator.py` & `django_iris-0.2.5b1/intersystems_iris/_IRISIterator.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/intersystems_iris/_IRISList.py` & `django_iris-0.2.5b1/intersystems_iris/_IRISList.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/intersystems_iris/_IRISNative.py` & `django_iris-0.2.5b1/intersystems_iris/_IRISNative.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/intersystems_iris/_IRISObject.py` & `django_iris-0.2.5b1/intersystems_iris/_IRISObject.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/intersystems_iris/_IRISReference.py` & `django_iris-0.2.5b1/intersystems_iris/_IRISReference.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/intersystems_iris/_InStream.py` & `django_iris-0.2.5b1/intersystems_iris/_InStream.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/intersystems_iris/_LegacyIterator.py` & `django_iris-0.2.5b1/intersystems_iris/_LegacyIterator.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/intersystems_iris/_ListReader.py` & `django_iris-0.2.5b1/intersystems_iris/_ListReader.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/intersystems_iris/_ListWriter.py` & `django_iris-0.2.5b1/intersystems_iris/_ListWriter.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/intersystems_iris/_LogFileStream.py` & `django_iris-0.2.5b1/intersystems_iris/_LogFileStream.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/intersystems_iris/_MessageHeader.py` & `django_iris-0.2.5b1/intersystems_iris/_MessageHeader.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/intersystems_iris/_OutStream.py` & `django_iris-0.2.5b1/intersystems_iris/_OutStream.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/intersystems_iris/_PrintStream.py` & `django_iris-0.2.5b1/intersystems_iris/_PrintStream.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/intersystems_iris/_PythonGateway.py` & `django_iris-0.2.5b1/intersystems_iris/_PythonGateway.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/intersystems_iris/_SharedMemorySocket.py` & `django_iris-0.2.5b1/intersystems_iris/_SharedMemorySocket.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/intersystems_iris/__init__.py` & `django_iris-0.2.5b1/intersystems_iris/__init__.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/intersystems_iris/dbapi/_Column.py` & `django_iris-0.2.5b1/intersystems_iris/dbapi/_Column.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/intersystems_iris/dbapi/_DBAPI.py` & `django_iris-0.2.5b1/intersystems_iris/dbapi/_DBAPI.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/intersystems_iris/dbapi/_Descriptor.py` & `django_iris-0.2.5b1/intersystems_iris/dbapi/_Descriptor.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/intersystems_iris/dbapi/_IRISStream.py` & `django_iris-0.2.5b1/intersystems_iris/dbapi/_IRISStream.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/intersystems_iris/dbapi/_Message.py` & `django_iris-0.2.5b1/intersystems_iris/dbapi/_Message.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/intersystems_iris/dbapi/_Parameter.py` & `django_iris-0.2.5b1/intersystems_iris/dbapi/_Parameter.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/intersystems_iris/dbapi/_ParameterCollection.py` & `django_iris-0.2.5b1/intersystems_iris/dbapi/_ParameterCollection.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/intersystems_iris/dbapi/_ResultSetRow.py` & `django_iris-0.2.5b1/intersystems_iris/dbapi/_ResultSetRow.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/intersystems_iris/dbapi/_SQLType.py` & `django_iris-0.2.5b1/intersystems_iris/dbapi/_SQLType.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/intersystems_iris/dbapi/preparser/_PreParser.py` & `django_iris-0.2.5b1/intersystems_iris/dbapi/preparser/_PreParser.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/intersystems_iris/dbapi/preparser/_Scanner.py` & `django_iris-0.2.5b1/intersystems_iris/dbapi/preparser/_Scanner.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/intersystems_iris/dbapi/preparser/_Token.py` & `django_iris-0.2.5b1/intersystems_iris/dbapi/preparser/_Token.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/intersystems_iris/dbapi/preparser/_TokenList.py` & `django_iris-0.2.5b1/intersystems_iris/dbapi/preparser/_TokenList.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/intersystems_iris/pex/_BusinessHost.py` & `django_iris-0.2.5b1/intersystems_iris/pex/_BusinessHost.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/intersystems_iris/pex/_BusinessOperation.py` & `django_iris-0.2.5b1/intersystems_iris/pex/_BusinessOperation.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/intersystems_iris/pex/_BusinessProcess.py` & `django_iris-0.2.5b1/intersystems_iris/pex/_BusinessProcess.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/intersystems_iris/pex/_BusinessService.py` & `django_iris-0.2.5b1/intersystems_iris/pex/_BusinessService.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/intersystems_iris/pex/_Common.py` & `django_iris-0.2.5b1/intersystems_iris/pex/_Common.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/intersystems_iris/pex/_Director.py` & `django_iris-0.2.5b1/intersystems_iris/pex/_Director.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/intersystems_iris/pex/_IRISBusinessService.py` & `django_iris-0.2.5b1/intersystems_iris/pex/_IRISBusinessService.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/intersystems_iris/pex/_IRISOutboundAdapter.py` & `django_iris-0.2.5b1/intersystems_iris/pex/_IRISOutboundAdapter.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/intersystems_iris/pex/_InboundAdapter.py` & `django_iris-0.2.5b1/intersystems_iris/pex/_InboundAdapter.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/intersystems_iris/pex/_OutboundAdapter.py` & `django_iris-0.2.5b1/intersystems_iris/pex/_OutboundAdapter.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/intersystems_iris/pex/__init__.py` & `django_iris-0.2.5b1/intersystems_iris/pex/__init__.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/irisnative/_IRISNative.py` & `django_iris-0.2.5b1/irisnative/_IRISNative.py`

 * *Files identical despite different names*

### Comparing `django-iris-0.2.4b1/setup.cfg` & `django_iris-0.2.5b1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-iris
-version = 0.2.4b1
+version = 0.2.5b1
 url = https://github.com/caretdev/django-iris
 maintainer = CaretDev
 maintainer_email = dmitry@caretdev.com
 license = MIT
 description = Django backend for InterSystems IRIS
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `django-iris-0.2.4b1/setup.py` & `django_iris-0.2.5b1/setup.py`

 * *Files identical despite different names*

