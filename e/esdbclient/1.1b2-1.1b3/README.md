# Comparing `tmp/esdbclient-1.1b2.tar.gz` & `tmp/esdbclient-1.1b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esdbclient-1.1b2.tar", max compression
+gzip compressed data, was "esdbclient-1.1b3.tar", max compression
```

## Comparing `esdbclient-1.1b2.tar` & `esdbclient-1.1b3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1520 2022-06-23 14:19:18.317032 esdbclient-1.1b2/LICENSE
--rw-r--r--   0        0        0   147009 2024-05-09 16:08:18.286706 esdbclient-1.1b2/README.md
--rw-r--r--   0        0        0      665 2024-05-09 12:30:42.655858 esdbclient-1.1b2/esdbclient/__init__.py
--rw-r--r--   0        0        0    60668 2024-05-09 15:19:09.242192 esdbclient-1.1b2/esdbclient/asyncio_client.py
--rw-r--r--   0        0        0    66978 2024-05-09 15:19:09.232635 esdbclient-1.1b2/esdbclient/client.py
--rw-r--r--   0        0        0    12402 2024-05-09 13:51:54.783176 esdbclient-1.1b2/esdbclient/common.py
--rw-r--r--   0        0        0     3819 2024-05-09 12:30:42.661945 esdbclient-1.1b2/esdbclient/connection.py
--rw-r--r--   0        0        0    10170 2024-05-09 12:30:42.663682 esdbclient-1.1b2/esdbclient/connection_spec.py
--rw-r--r--   0        0        0     3422 2024-05-09 12:30:42.664490 esdbclient-1.1b2/esdbclient/events.py
--rw-r--r--   0        0        0     6117 2024-05-09 13:25:45.934297 esdbclient-1.1b2/esdbclient/exceptions.py
--rw-r--r--   0        0        0     5532 2024-05-09 12:30:42.667329 esdbclient-1.1b2/esdbclient/gossip.py
--rw-r--r--   0        0        0    82861 2024-05-09 12:30:42.668861 esdbclient-1.1b2/esdbclient/persistent.py
--rw-r--r--   0        0        0    24972 2024-05-09 15:21:18.742508 esdbclient-1.1b2/esdbclient/projections.py
--rw-r--r--   0        0        0    14166 2024-05-09 12:30:42.671328 esdbclient-1.1b2/esdbclient/protos/Grpc/cluster_pb2.py
--rw-r--r--   0        0        0    37958 2024-05-02 13:49:41.275519 esdbclient-1.1b2/esdbclient/protos/Grpc/cluster_pb2.pyi
--rw-r--r--   0        0        0    19336 2024-05-02 13:49:40.865930 esdbclient-1.1b2/esdbclient/protos/Grpc/cluster_pb2_grpc.py
--rw-r--r--   0        0        0     1916 2024-05-09 12:30:42.672190 esdbclient-1.1b2/esdbclient/protos/Grpc/code_pb2.py
--rw-r--r--   0        0        0    13555 2024-05-02 13:49:40.538653 esdbclient-1.1b2/esdbclient/protos/Grpc/code_pb2.pyi
--rw-r--r--   0        0        0      158 2024-05-02 13:49:40.389375 esdbclient-1.1b2/esdbclient/protos/Grpc/code_pb2_grpc.py
--rw-r--r--   0        0        0     3030 2024-05-09 12:30:42.672780 esdbclient-1.1b2/esdbclient/protos/Grpc/gossip_pb2.py
--rw-r--r--   0        0        0     5524 2024-05-02 13:49:40.640362 esdbclient-1.1b2/esdbclient/protos/Grpc/gossip_pb2.pyi
--rw-r--r--   0        0        0     2752 2024-05-02 13:49:40.532290 esdbclient-1.1b2/esdbclient/protos/Grpc/gossip_pb2_grpc.py
--rw-r--r--   0        0        0    23846 2024-05-09 12:30:42.673979 esdbclient-1.1b2/esdbclient/protos/Grpc/persistent_pb2.py
--rw-r--r--   0        0        0    73220 2024-05-02 13:49:41.830902 esdbclient-1.1b2/esdbclient/protos/Grpc/persistent_pb2.pyi
--rw-r--r--   0        0        0    15771 2024-05-02 13:49:40.799320 esdbclient-1.1b2/esdbclient/protos/Grpc/persistent_pb2_grpc.py
--rw-r--r--   0        0        0    10621 2024-05-09 12:30:42.674904 esdbclient-1.1b2/esdbclient/protos/Grpc/projections_pb2.py
--rw-r--r--   0        0        0    25437 2024-05-09 12:30:42.675584 esdbclient-1.1b2/esdbclient/protos/Grpc/projections_pb2.pyi
--rw-r--r--   0        0        0    18841 2024-05-09 12:30:42.676247 esdbclient-1.1b2/esdbclient/protos/Grpc/projections_pb2_grpc.py
--rw-r--r--   0        0        0     4187 2024-05-09 12:30:42.677057 esdbclient-1.1b2/esdbclient/protos/Grpc/shared_pb2.py
--rw-r--r--   0        0        0     9874 2024-05-02 13:49:40.801616 esdbclient-1.1b2/esdbclient/protos/Grpc/shared_pb2.pyi
--rw-r--r--   0        0        0      158 2024-05-02 13:49:40.534944 esdbclient-1.1b2/esdbclient/protos/Grpc/shared_pb2_grpc.py
--rw-r--r--   0        0        0     1813 2024-05-09 12:30:42.677868 esdbclient-1.1b2/esdbclient/protos/Grpc/status_pb2.py
--rw-r--r--   0        0        0     2838 2024-05-02 13:49:40.608113 esdbclient-1.1b2/esdbclient/protos/Grpc/status_pb2.pyi
--rw-r--r--   0        0        0      158 2024-05-02 13:49:40.550725 esdbclient-1.1b2/esdbclient/protos/Grpc/status_pb2_grpc.py
--rw-r--r--   0        0        0    21622 2024-05-09 12:30:42.678599 esdbclient-1.1b2/esdbclient/protos/Grpc/streams_pb2.py
--rw-r--r--   0        0        0    72778 2024-05-09 12:30:42.679517 esdbclient-1.1b2/esdbclient/protos/Grpc/streams_pb2.pyi
--rw-r--r--   0        0        0     9787 2024-05-02 13:49:40.788920 esdbclient-1.1b2/esdbclient/protos/Grpc/streams_pb2_grpc.py
--rw-r--r--   0        0        0        0 2022-06-23 14:19:18.321130 esdbclient-1.1b2/esdbclient/py.typed
--rw-r--r--   0        0        0    52319 2024-05-09 12:30:42.680251 esdbclient-1.1b2/esdbclient/streams.py
--rw-r--r--   0        0        0     2778 2024-05-09 16:44:18.274739 esdbclient-1.1b2/pyproject.toml
--rw-r--r--   0        0        0   148047 1970-01-01 00:00:00.000000 esdbclient-1.1b2/PKG-INFO
+-rw-r--r--   0        0        0     1520 2022-06-23 14:19:18.317032 esdbclient-1.1b3/LICENSE
+-rw-r--r--   0        0        0   149456 2024-05-20 12:30:10.747941 esdbclient-1.1b3/README.md
+-rw-r--r--   0        0        0      665 2024-05-09 12:30:42.655858 esdbclient-1.1b3/esdbclient/__init__.py
+-rw-r--r--   0        0        0    60481 2024-05-20 12:30:10.773980 esdbclient-1.1b3/esdbclient/asyncio_client.py
+-rw-r--r--   0        0        0    66791 2024-05-20 13:00:04.101524 esdbclient-1.1b3/esdbclient/client.py
+-rw-r--r--   0        0        0    12634 2024-05-20 13:01:10.951193 esdbclient-1.1b3/esdbclient/common.py
+-rw-r--r--   0        0        0     3819 2024-05-09 12:30:42.661945 esdbclient-1.1b3/esdbclient/connection.py
+-rw-r--r--   0        0        0    10170 2024-05-09 12:30:42.663682 esdbclient-1.1b3/esdbclient/connection_spec.py
+-rw-r--r--   0        0        0     3422 2024-05-09 12:30:42.664490 esdbclient-1.1b3/esdbclient/events.py
+-rw-r--r--   0        0        0     6099 2024-05-20 13:44:45.701581 esdbclient-1.1b3/esdbclient/exceptions.py
+-rw-r--r--   0        0        0     5532 2024-05-09 12:30:42.667329 esdbclient-1.1b3/esdbclient/gossip.py
+-rw-r--r--   0        0        0    82861 2024-05-09 12:30:42.668861 esdbclient-1.1b3/esdbclient/persistent.py
+-rw-r--r--   0        0        0    24950 2024-05-20 12:30:10.781461 esdbclient-1.1b3/esdbclient/projections.py
+-rw-r--r--   0        0        0    14166 2024-05-09 12:30:42.671328 esdbclient-1.1b3/esdbclient/protos/Grpc/cluster_pb2.py
+-rw-r--r--   0        0        0    37958 2024-05-02 13:49:41.275519 esdbclient-1.1b3/esdbclient/protos/Grpc/cluster_pb2.pyi
+-rw-r--r--   0        0        0    19336 2024-05-02 13:49:40.865930 esdbclient-1.1b3/esdbclient/protos/Grpc/cluster_pb2_grpc.py
+-rw-r--r--   0        0        0     1916 2024-05-09 12:30:42.672190 esdbclient-1.1b3/esdbclient/protos/Grpc/code_pb2.py
+-rw-r--r--   0        0        0    13555 2024-05-02 13:49:40.538653 esdbclient-1.1b3/esdbclient/protos/Grpc/code_pb2.pyi
+-rw-r--r--   0        0        0      158 2024-05-02 13:49:40.389375 esdbclient-1.1b3/esdbclient/protos/Grpc/code_pb2_grpc.py
+-rw-r--r--   0        0        0     3030 2024-05-09 12:30:42.672780 esdbclient-1.1b3/esdbclient/protos/Grpc/gossip_pb2.py
+-rw-r--r--   0        0        0     5524 2024-05-02 13:49:40.640362 esdbclient-1.1b3/esdbclient/protos/Grpc/gossip_pb2.pyi
+-rw-r--r--   0        0        0     2752 2024-05-02 13:49:40.532290 esdbclient-1.1b3/esdbclient/protos/Grpc/gossip_pb2_grpc.py
+-rw-r--r--   0        0        0    23846 2024-05-09 12:30:42.673979 esdbclient-1.1b3/esdbclient/protos/Grpc/persistent_pb2.py
+-rw-r--r--   0        0        0    73220 2024-05-02 13:49:41.830902 esdbclient-1.1b3/esdbclient/protos/Grpc/persistent_pb2.pyi
+-rw-r--r--   0        0        0    15771 2024-05-02 13:49:40.799320 esdbclient-1.1b3/esdbclient/protos/Grpc/persistent_pb2_grpc.py
+-rw-r--r--   0        0        0    10621 2024-05-09 12:30:42.674904 esdbclient-1.1b3/esdbclient/protos/Grpc/projections_pb2.py
+-rw-r--r--   0        0        0    25437 2024-05-09 12:30:42.675584 esdbclient-1.1b3/esdbclient/protos/Grpc/projections_pb2.pyi
+-rw-r--r--   0        0        0    18841 2024-05-09 12:30:42.676247 esdbclient-1.1b3/esdbclient/protos/Grpc/projections_pb2_grpc.py
+-rw-r--r--   0        0        0     4187 2024-05-09 12:30:42.677057 esdbclient-1.1b3/esdbclient/protos/Grpc/shared_pb2.py
+-rw-r--r--   0        0        0     9874 2024-05-02 13:49:40.801616 esdbclient-1.1b3/esdbclient/protos/Grpc/shared_pb2.pyi
+-rw-r--r--   0        0        0      158 2024-05-02 13:49:40.534944 esdbclient-1.1b3/esdbclient/protos/Grpc/shared_pb2_grpc.py
+-rw-r--r--   0        0        0     1813 2024-05-09 12:30:42.677868 esdbclient-1.1b3/esdbclient/protos/Grpc/status_pb2.py
+-rw-r--r--   0        0        0     2838 2024-05-02 13:49:40.608113 esdbclient-1.1b3/esdbclient/protos/Grpc/status_pb2.pyi
+-rw-r--r--   0        0        0      158 2024-05-02 13:49:40.550725 esdbclient-1.1b3/esdbclient/protos/Grpc/status_pb2_grpc.py
+-rw-r--r--   0        0        0    21622 2024-05-09 12:30:42.678599 esdbclient-1.1b3/esdbclient/protos/Grpc/streams_pb2.py
+-rw-r--r--   0        0        0    72778 2024-05-09 12:30:42.679517 esdbclient-1.1b3/esdbclient/protos/Grpc/streams_pb2.pyi
+-rw-r--r--   0        0        0     9787 2024-05-02 13:49:40.788920 esdbclient-1.1b3/esdbclient/protos/Grpc/streams_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2022-06-23 14:19:18.321130 esdbclient-1.1b3/esdbclient/py.typed
+-rw-r--r--   0        0        0    52319 2024-05-14 18:22:42.464713 esdbclient-1.1b3/esdbclient/streams.py
+-rw-r--r--   0        0        0     2778 2024-05-20 17:38:51.647505 esdbclient-1.1b3/pyproject.toml
+-rw-r--r--   0        0        0   150494 1970-01-01 00:00:00.000000 esdbclient-1.1b3/PKG-INFO
```

### Comparing `esdbclient-1.1b2/LICENSE` & `esdbclient-1.1b3/LICENSE`

 * *Files identical despite different names*

### Comparing `esdbclient-1.1b2/README.md` & `esdbclient-1.1b3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,28 +4,108 @@
 clients for the [EventStoreDB](https://www.eventstore.com/) database.
 
 The multithreaded `EventStoreDBClient` is described in detail below. Please scroll
 down for <a href="#asyncio-client">information</a> about `AsyncioEventStoreDBClient`.
 
 These clients have been developed and are being maintained in a collaboration
 with the EventStoreDB team, and are officially support by Event Store Ltd.
-Although not all the features of EventStoreDB are supported, many of the most
-useful features are presented in an easy-to-use interface.
+Although not all aspects of the EventStoreDB gRPC API are implemented, many
+of the most useful features are presented in an easy-to-use interface.
 
-These clients have been tested to work with EventStoreDB LTS versions 21.10,
-22.10, 23.10, and version 24.2, without and without SSL/TLS, with single-server
+These clients have been tested to work with EventStoreDB LTS versions 22.10 and 23.10,
+and release candidates 24.2 and 24.6, without and without SSL/TLS, with both single-server
 and cluster modes, and with Python versions 3.7, 3.8, 3.9, 3.10, 3.11 and 3.12.
 
 The test suite has 100% line and branch coverage. The code has typing annotations
 checked strictly with mypy. The code is formatted with black and isort, and checked
 with flake8. Poetry is used for package management during development, and for
 building and publishing distributions to [PyPI](https://pypi.org/project/esdbclient/).
 
+For an example of usage, see the [eventsourcing-eventstoredb](
+https://github.com/pyeventsourcing/eventsourcing-eventstoredb) package.
+
+
+<!-- TOC -->
+* [Synopsis](#synopsis)
+* [Install package](#install-package)
+  * [From PyPI](#from-pypi)
+  * [With Poetry](#with-poetry)
+* [EventStoreDB server](#eventstoredb-server)
+  * [Run container](#run-container)
+  * [Stop container](#stop-container)
+* [EventStoreDB client](#eventstoredb-client)
+  * [Import class](#import-class)
+  * [Construct client](#construct-client)
+* [Connection strings](#connection-strings)
+  * [Two schemes](#two-schemes)
+  * [User info string](#user-info-string)
+  * [Query string](#query-string)
+  * [Examples](#examples)
+* [Event objects](#event-objects)
+  * [New events](#new-events)
+  * [Recorded events](#recorded-events)
+* [Streams](#streams)
+  * [Append events](#append-events)
+  * [Idempotent append operations](#idempotent-append-operations)
+  * [Read stream events](#read-stream-events)
+  * [Get current version](#get-current-version)
+  * [How to implement snapshotting with EventStoreDB](#how-to-implement-snapshotting-with-eventstoredb)
+  * [Read all events](#read-all-events)
+  * [Get commit position](#get-commit-position)
+  * [Get stream metadata](#get-stream-metadata)
+  * [Set stream metadata](#set-stream-metadata)
+  * [Delete stream](#delete-stream)
+  * [Tombstone stream](#tombstone-stream)
+* [Catch-up subscriptions](#catch-up-subscriptions)
+  * [Subscribe to all events](#subscribe-to-all-events)
+  * [Subscribe to stream events](#subscribe-to-stream-events)
+  * [How to implement exactly-once event processing](#how-to-implement-exactly-once-event-processing)
+* [Persistent subscriptions](#persistent-subscriptions)
+  * [Create subscription to all](#create-subscription-to-all)
+  * [Read subscription to all](#read-subscription-to-all)
+  * [How to write a persistent subscription consumer](#how-to-write-a-persistent-subscription-consumer)
+  * [Update subscription to all](#update-subscription-to-all)
+  * [Create subscription to stream](#create-subscription-to-stream)
+  * [Read subscription to stream](#read-subscription-to-stream)
+  * [Update subscription to stream](#update-subscription-to-stream)
+  * [Replay parked events](#replay-parked-events)
+  * [Get subscription info](#get-subscription-info)
+  * [List subscriptions](#list-subscriptions)
+  * [List subscriptions to stream](#list-subscriptions-to-stream)
+  * [Delete subscription](#delete-subscription)
+* [Projections](#projections)
+  * [Create projection](#create-projection)
+  * [Get projection state](#get-projection-state)
+  * [Get projection result](#get-projection-result)
+  * [Get projection statistics](#get-projection-statistics)
+  * [Update projection](#update-projection)
+  * [Enable projection](#enable-projection)
+  * [Disable projection](#disable-projection)
+  * [Reset projection](#reset-projection)
+  * [Delete projection](#delete-projection)
+  * [Restart projections subsystem](#restart-projections-subsystem)
+* [Call credentials](#call-credentials)
+  * [Construct call credentials](#construct-call-credentials)
+* [Connection](#connection)
+  * [Reconnect](#reconnect)
+  * [Close](#close)
+* [Asyncio client](#asyncio-client)
+  * [Synopsis](#synopsis-1)
+* [Notes](#notes)
+  * [Regular expression filters](#regular-expression-filters)
+  * [Reconnect and retry method decorators](#reconnect-and-retry-method-decorators)
+* [Communities](#communities)
+* [Contributors](#contributors)
+  * [Install Poetry](#install-poetry)
+  * [Setup for PyCharm users](#setup-for-pycharm-users)
+  * [Setup from command line](#setup-from-command-line)
+  * [Project Makefile commands](#project-makefile-commands)
+<!-- TOC -->
 
-## Synopsis
+## Synopsis<a id="synopsis"></a>
 
 The `EventStoreDBClient` class can be imported from the `esdbclient` package.
 
 Probably the three most useful methods of `EventStoreDBClient` are:
 
 * `append_to_stream()` This method can be used to record new events in a particular
 "stream". This is useful, for example, when executing a command in an application
@@ -183,95 +263,14 @@
 
 
 # Close the client's gRPC connection.
 
 client.close()
 ```
 
-See below for more details.
-
-For an example of usage, see the [eventsourcing-eventstoredb](
-https://github.com/pyeventsourcing/eventsourcing-eventstoredb) package.
-
-## Table of contents
-
-<!-- TOC -->
-* [Install package](#install-package)
-  * [From PyPI](#from-pypi)
-  * [With Poetry](#with-poetry)
-* [EventStoreDB server](#eventstoredb-server)
-  * [Run container](#run-container)
-  * [Stop container](#stop-container)
-* [EventStoreDB client](#eventstoredb-client)
-  * [Import class](#import-class)
-  * [Construct client](#construct-client)
-* [Connection strings](#connection-strings)
-  * [Two schemes](#two-schemes)
-  * [User info string](#user-info-string)
-  * [Query string](#query-string)
-  * [Examples](#examples)
-* [Event objects](#event-objects)
-  * [New events](#new-events)
-  * [Recorded events](#recorded-events)
-* [Streams](#streams)
-  * [Append events](#append-events)
-  * [Idempotent append operations](#idempotent-append-operations)
-  * [Read stream events](#read-stream-events)
-  * [Get current version](#get-current-version)
-  * [How to implement snapshotting with EventStoreDB](#how-to-implement-snapshotting-with-eventstoredb)
-  * [Read all events](#read-all-events)
-  * [Get commit position](#get-commit-position)
-  * [Get stream metadata](#get-stream-metadata)
-  * [Set stream metadata](#set-stream-metadata)
-  * [Delete stream](#delete-stream)
-  * [Tombstone stream](#tombstone-stream)
-* [Catch-up subscriptions](#catch-up-subscriptions)
-  * [Subscribe to all events](#subscribe-to-all-events)
-  * [Subscribe to stream events](#subscribe-to-stream-events)
-  * [How to implement exactly-once event processing](#how-to-implement-exactly-once-event-processing)
-* [Persistent subscriptions](#persistent-subscriptions)
-  * [Create subscription to all](#create-subscription-to-all)
-  * [Read subscription to all](#read-subscription-to-all)
-  * [How to write a persistent subscription consumer](#how-to-write-a-persistent-subscription-consumer)
-  * [Update subscription to all](#update-subscription-to-all)
-  * [Create subscription to stream](#create-subscription-to-stream)
-  * [Read subscription to stream](#read-subscription-to-stream)
-  * [Update subscription to stream](#update-subscription-to-stream)
-  * [Replay parked events](#replay-parked-events)
-  * [Get subscription info](#get-subscription-info)
-  * [List subscriptions](#list-subscriptions)
-  * [List subscriptions to stream](#list-subscriptions-to-stream)
-  * [Delete subscription](#delete-subscription)
-* [Projections](#projections)
-  * [Create projection](#create-projection)
-  * [Get projection state](#get-projection-state)
-  * [Get projection result](#get-projection-result)
-  * [Get projection statistics](#get-projection-statistics)
-  * [Update projection](#update-projection)
-  * [Enable projection](#enable-projection)
-  * [Disable projection](#disable-projection)
-  * [Reset projection](#reset-projection)
-  * [Delete projection](#delete-projection)
-  * [Restart projections subsystem](#restart-projections-subsystem)
-* [Call credentials](#call-credentials)
-  * [Construct call credentials](#construct-call-credentials)
-* [Connection](#connection)
-  * [Reconnect](#reconnect)
-  * [Close](#close)
-* [Asyncio client](#asyncio-client)
-  * [Synopsis](#synopsis-1)
-* [Notes](#notes)
-  * [Regular expression filters](#regular-expression-filters)
-  * [Reconnect and retry method decorators](#reconnect-and-retry-method-decorators)
-* [Contributors](#contributors)
-  * [Install Poetry](#install-poetry)
-  * [Setup for PyCharm users](#setup-for-pycharm-users)
-  * [Setup from command line](#setup-from-command-line)
-  * [Project Makefile commands](#project-makefile-commands)
-<!-- TOC -->
 
 ## Install package<a id="install-package"></a>
 
 It is recommended to install Python packages into a Python virtual environment.
 
 ### From PyPI<a id="from-pypi"></a>
 
@@ -290,15 +289,15 @@
 
 The EventStoreDB server can be run locally using the official Docker container image.
 
 ### Run container<a id="run-container"></a>
 
 For development, you can run a "secure" EventStoreDB server using the following command.
 
-    $ docker run -d --name eventstoredb-secure -it -p 2113:2113 --env "HOME=/tmp" eventstore/eventstore:21.10.9-buster-slim --dev
+    $ docker run -d --name eventstoredb-secure -it -p 2113:2113 --env "HOME=/tmp" docker.eventstore.com/eventstore-ce/eventstoredb-ce:23.10.0-jammy --dev
 
 As we will see, your client will need an EventStoreDB connection string URI as the value
 of its `uri` constructor argument. The connection string for this "secure" EventStoreDB
 server would be:
 
     esdb://admin:changeit@localhost:2113
 
@@ -320,15 +319,15 @@
 import ssl
 
 server_certificate = ssl.get_server_certificate(addr=('localhost', 2113))
 ```
 
 Alternatively, you can start an "insecure" server using the following command.
 
-    $ docker run -d --name eventstoredb-insecure -it -p 2113:2113 eventstore/eventstore:21.10.9-buster-slim --insecure
+    $ docker run -d --name eventstoredb-insecure -it -p 2113:2113 docker.eventstore.com/eventstore-ce/eventstoredb-ce:23.10.0-jammy --insecure
 
 The connection string URI for this "insecure" server would be:
 
     esdb://localhost:2113?Tls=false
 
 As we will see, when connecting to an "insecure" server, there is no need to include
 a "username" and a "password" in the connection string. If you do, these values will
@@ -367,45 +366,29 @@
 
 The `EventStoreDBClient` class has one required constructor argument, `uri`, and one
 optional constructor argument, `root_certificates`.
 
 The `uri` argument is expected to be an EventStoreDB connection string URI that
 conforms with the standard EventStoreDB "esdb" or "esdb+discover" URI schemes.
 
-For example, the following connection string specifies that the client should
-attempt to create a "secure" connection to port 2113 on "localhost", and use the
-client credentials "username" and "password" when making calls to the server.
-
-    esdb://username:password@localhost:2113?Tls=true
-
 The client must be configured to create a "secure" connection to a "secure" server,
 or alternatively an "insecure" connection to an "insecure" server. By default, the
 client will attempt to create a "secure" connection. And so, when connecting to an
 "insecure" server, the connection string must specify that the client should attempt
 to make an "insecure" connection.
 
-The following connection string specifies that the client should
-attempt to create an "insecure" connection to port 2113 on "localhost".
-When connecting to an "insecure" server, the client will ignore any
-username and password information included in the connection string,
-so that usernames and passwords are not sent over an "insecure" connection.
-
-    esdb://localhost:2113?Tls=false
-
-Please note, the "insecure" connection string uses a query string with the field-value
-`Tls=false`. The value of this field is by default `true`.
-
-When connecting to a "secure" server, the `root_certificates` argument can be
-a Python `str` containing PEM encoded SSL/TLS root certificates. This value is
-passed directly to `grpc.ssl_channel_credentials()`. It is used for authenticating the
-server to the client. It is commonly the certificate of the certificate authority that
-was responsible for generating the SSL/TLS certificate used by the EventStoreDB server.
-Often it is unnecessary to provide these certificates explicitly, if they are installed
-locally in a such a way that the Python grpc library can pick them up from a default
-location. Alternatively, for development, you can use the server's certificate itself.
+When connecting to a "secure" server, it may be necessary to set the optional `root_certificates`
+argument. The optional `root_certificates` argument is a Python `str` containing
+PEM encoded SSL/TLS root certificates. This value is passed directly to
+`grpc.ssl_channel_credentials()` and is used by the client to authenticate the server.
+It is commonly a public certificate of the certificate authority that was responsible
+for generating the certificate used by the EventStoreDB server. Often it is unnecessary
+to provide these certificates explicitly, as they are commonly installed locally in
+a default location such that the Python grpc library can pick them up. Alternatively,
+for development, you can use the server's certificate itself.
 
 In the example below, the constructor argument values are taken from the operating
 system environment.
 
 ```python
 import os
 
@@ -440,46 +423,52 @@
 
     grpc-target = ( hostname | ip-address ) , ":" , port-number ;
 
 If there is one gRPC target, the client will simply attempt to connect to this
 server, and it will use this connection when recording and retrieving events.
 
 If there are two or more gRPC targets, the client will attempt to connect to the
-Gossip API of each in turn, to obtain information about the whole cluster. A member
-of the cluster is then selected by the client according to the "node preference" option
-of the connection string. The client may then need to close its connection and reconnect
-to the selected node.
+Gossip API of each in turn, attempting to obtain information about the cluster from
+it, until information about the cluster is obtained. A member of the cluster is then
+selected by the client according to the "node preference" specified by the connection
+string URI. The client will then close its connection and connect to the selected node
+without the 'round robin' load balancing strategy. If the "node preference" is "leader",
+and after connecting to a leader, if the leader becomes a follower, the client will
+reconnect to the new leader.
+
 
 The "esdb+discover" URI scheme can be defined in the following way.
 
     esdb-discover-uri = "esdb+discover://" , [ user-info, "@" ] , cluster-domainname, [ ":" , port-number ] , [ "?" , query-string ] ;
 
 In the "esdb+discover" URI scheme, after the optional user info string, there should be
 a domain name which identifies a cluster of EventStoreDB servers. Individual nodes in
 the cluster should be declared with DNS 'A' records.
 
-The client will create a gRPC connection using the cluster's domain name, using the
-gRPC library's 'round robin' load balancing strategy to call the Gossip API of addresses
-to which this domain name resolves. Information about the EventStoreDB cluster is
-obtained from the Gossip API. A member of the cluster is then selected by the client
-according to the "node preference" option. The client may then need to close its
-connection and reconnect to the selected node.
+The client will use the cluster domain name with the gRPC library's 'round robin' load
+balancing strategy to call the Gossip APIs of addresses discovered from DNS 'A' records.
+Information about the EventStoreDB cluster is obtained from the Gossip API. A member of
+the cluster is then selected by the client according to the "node preference" option.
+The client will then close its connection and connect to the selected node without the
+'round robin' load balancing strategy. If the "node preference" is "leader",
+and after connecting to a leader, if the leader becomes a follower, the client will
+reconnect to the new leader.
 
 ### User info string<a id="user-info-string"></a>
 
 In both the "esdb" and "esdb+discover" schemes, the URI may include a user info string.
 If it exists in the URI, the user info string must be separated from the rest of the URI
 with the "@" character. The user info string must include a username and a password,
 separated with the ":" character.
 
     user-info = username , ":" , password ;
 
-The user info is sent by the client as "call credentials" in each call to a "secure"
-server, in a "basic auth" authorization header. This authorization header is used by
-the server to authenticate the client. The authorization header is not sent to
+The user info is sent by the client in a "basic auth" authorization header in each gRPC
+call to a "secure" server. This authorization header is used by the server to authenticate
+the client. The Python gRPC library does not allow call credentials to be transferred to
 "insecure" servers.
 
 ### Query string<a id="query-string"></a>
 
 In both the "esdb" and "esdb+discover" schemes, the optional query string must be one
 or many field-value arguments, separated from each other with the "&" character.
 
@@ -507,84 +496,94 @@
 | TlsVerifyCert       | "true", "false" (default: "true")                                     | This value is currently ignored.                                                                                                                                  |
 | ConnectionName      | string (default: auto-generated version-4 UUID)                       | Sent in call metadata for every call, to identify the client to the cluster.                                                                                      |
 | NodePreference      | "leader", "follower", "readonlyreplica", "random" (default: "leader") | The node state preferred by the client. The client will select a node from the cluster info received from the Gossip API according to this preference.            |
 | DefaultDeadline     | integer (default: `None`)                                             | The default value (in seconds) of the `timeout` argument of client "write" methods such as `append_to_stream()`.                                                  |
 | GossipTimeout       | integer (default: 5)                                                  | The default value (in seconds) of the `timeout` argument of gossip read methods, such as `read_gossip()`.                                                         |
 | MaxDiscoverAttempts | integer (default: 10)                                                 | The number of attempts to read gossip when connecting or reconnecting to a cluster member.                                                                        |
 | DiscoveryInterval   | integer (default: 100)                                                | How long to wait (in milliseconds) between gossip retries.                                                                                                        |
-| KeepAliveInterval   | integer (default: `None`)                                             | The value of the "grpc.keepalive_ms" gRPC channel option.                                                                                                         |
-| KeepAliveTimeout    | integer (default: `None`)                                             | The value of the "grpc.keepalive_timeout_ms" gRPC channel option.                                                                                                 |
+| KeepAliveInterval   | integer (default: `None`)                                             | The value (in milliseconds) of the "grpc.keepalive_ms" gRPC channel option.                                                                                       |
+| KeepAliveTimeout    | integer (default: `None`)                                             | The value (in milliseconds) of the "grpc.keepalive_timeout_ms" gRPC channel option.                                                                               |
+
+Please note, the client is insensitive to the case of fields and values. If fields are
+repeated in the query string, the query string will be parsed without error. However,
+the connection options used by the client will use the value of the first field. All
+the other field-values in the query string with the same field name will be ignored.
+Fields without values will also be ignored.
+
+If the client's node preference is "follower" and there are no follower
+nodes in the cluster, then the client will raise an exception. Similarly, if the
+client's node preference is "readonlyreplica" and there are no read-only replica
+nodes in the cluster, then the client will also raise an exception.
+
+The gRPC channel option "grpc.max_receive_message_length" is automatically
+configured to the value `17 * 1024 * 1024`. This value cannot be configured.
 
 
 ### Examples<a id="examples"></a>
 
 Here are some examples of EventStoreDB connection string URIs.
 
-The following URI will cause the client to connect to, and get
-cluster info, from "secure" server socket `localhost:2113`. And
-then to connect to a "leader" node. And also to use "admin" and
-"changeit" as the username and password when making calls to
-EventStoreDB API methods.
+The following URI will cause the client to make an "insecure" connection to
+gRPC target `'localhost:2113'`. Because the client's node preference is "follower",
+methods that can be called on a follower should complete successfully, methods that
+require a leader will raise a `NodeIsNotLeader` exception.
+
+    esdb://127.0.0.1:2113?Tls=false&NodePreference=follower
+
+The following URI will cause the client to make an "insecure" connection to
+gRPC target `'localhost:2113'`. Because the client's node preference is "leader",
+if this node is not a leader, then a `NodeIsNotLeader` exception will be raised by
+all methods.
+
+    esdb://127.0.0.1:2113?Tls=false&NodePreference=leader
+
+The following URI will cause the client to make a "secure" connection to
+gRPC target `'localhost:2113'` with username `'admin'` and password `'changeit'`
+as the default call credentials when making calls to the EventStoreDB gRPC API.
+Because the client's node preference is "leader", by default, if this node is not
+a leader, then a `NodeIsNotLeader` exception will be raised by all methods.
 
     esdb://admin:changeit@localhost:2113
 
+The following URI will cause the client to make "secure" connections, firstly to
+get cluster info from either `'localhost:2111'`, or `'localhost:2112'`, or `'localhost:2113'`.
+Because the client's node preference is "leader", the client will select the leader
+node from the cluster info and reconnect to the leader. If the "leader" node becomes
+a "follower" and another node becomes "leader", then the client will reconnect to the
+new leader.
+
+    esdb://admin:changeit@localhost:2111,localhost:2112,localhost:2113?NodePreference=leader
+
+
+The following URI will cause the client to make "secure" connections, firstly to
+get cluster info from either `'localhost:2111'`, or `'localhost:2112'`, or `'localhost:2113'`.
+Because the client's node preference is "follower", the client will select a follower
+node from the cluster info and reconnect to this follower. Please note, if the "follower"
+node becomes the "leader", the client will not reconnect to a follower -- such behavior
+may be implemented in a future version of the client and server.
 
-The following URI will cause the client to get cluster info from
-"insecure" server socket 127.0.0.1:2113.  And then to connect to
-a "leader" node.
-
-    esdb://127.0.0.1:2113?Tls=false
+    esdb://admin:changeit@localhost:2111,localhost:2112,localhost:2113?NodePreference=follower
 
 
-The following URI will cause the client to get cluster info from
-addresses in DNS 'A' records for cluster1.example.com. And then
-to connect to a "leader" node. And use a default deadline of 5
-seconds when making calls to EventStore API "write" methods.
+The following URI will cause the client to make "secure" connections, firstly to get
+cluster info from addresses in DNS 'A' records for `'cluster1.example.com'`, and then
+to connect to a "leader" node. The client will use a default timeout
+of 5 seconds when making calls to EventStore API "write" methods.
 
     esdb+discover://admin:changeit@cluster1.example.com?DefaultDeadline=5
 
 
-The following URI will cause the client to get cluster info from either
-localhost:2111, or localhost:2112, or localhost:2113. And then to connect
-to a "follower" node.
-
-    esdb://admin:changeit@localhost:2111,localhost:2112,localhost:2113?NodePreference=follower
-
-
-The following URI will cause the client to get cluster info from addresses in
-DNS 'A' records for cluster1.example.com. And to configure "keep alive" timeout
-and interval in the gRPC channel.
+The following URI will cause the client to make "secure" connections, firstly to get
+cluster info from addresses in DNS 'A' records for `'cluster1.example.com'`, and then
+to connect to a "leader" node. It will configure gRPC connections with a "keep alive
+interval" and a "keep alive timeout".
 
     esdb+discover://admin:changeit@cluster1.example.com?KeepAliveInterval=10000&KeepAliveTimeout=10000
 
 
-Please note, the client is insensitive to the case of fields and values. If fields are
-repeated in the query string, the query string will be parsed without error. However,
-the connection options used by the client will use the value of the first field. All
-the other field-values in the query string with the same field name will be ignored.
-Fields without values will also be ignored.
-
-If the client's node preference is "leader" and the node becomes a
-"follower", the client will attempt to reconnect to the current leader when a method
-is called that expects to call a leader. Methods which mutate the state of the database
-expect to call a leader. For such methods, the HTTP header "requires-leader" is set to
-"true", and this header is observed by the server, and so a node which is not a leader
-that receives such a request will return an error. This error is detected by the client,
-which will then close the current gRPC connection and create a new connection to the
-leader. The request will then be retried with the leader.
-
-If the client's node preference is "follower" and there are no follower
-nodes in the cluster, then the client will raise an exception. Similarly, if the
-client's node preference is "readonlyreplica" and there are no read-only replica
-nodes in the cluster, then the client will also raise an exception.
-
-The gRPC channel option "grpc.max_receive_message_length" is automatically
-configured to the value `17 * 1024 * 1024`. This value cannot be changed.
-
-
 ## Event objects<a id="event-objects"></a>
 
 This package defines a `NewEvent` class and a `RecordedEvent` class. The
 `NewEvent` class should be used when writing events to the database. The
 `RecordedEvent` class is used when reading events from the database.
 
 ### New events<a id="new-events"></a>
@@ -646,19 +645,20 @@
 The `RecordedEvent` class is used when reading events from an EventStoreDB
 database. The client will return event objects of this type from all methods
 that return recorded events, such as `get_stream()`, `subscribe_to_all()`,
 and `read_subscription_to_all()`. You do not need to construct recorded event objects.
 
 Like `NewEvent`, the `RecordedEvent` class is a frozen Python dataclass. It has
 all the attributes that `NewEvent` has (`type`, `data`, `metadata`, `content_type`, `id`)
-that follow from an event that was recorded, and some additional attributes that follow
+that follow from an event having been recorded, and some additional attributes that follow
 from the recording of an event (`stream_name`, `stream_position`, `commit_position`,
-`recorded_at`). It also has a `link` attribute, which is set only when "link events"
-are "resolved". And it has a `retry_count` which is set only when reading persistence
-subscriptions.
+`recorded_at`). It also has a `link` attribute, which is `None` unless the recorded
+event is a "link event" that has been "resolved" to the linked event. And it has a
+`retry_count` which has an integer value when receiving recorded events from persistence
+subscriptions, otherwise the value of `retry_count` is `None`.
 
 The `type` attribute is a Python `str`, used to indicate the type of an event
 that was recorded.
 
 The `data` attribute is a Python `bytes` object, used to indicate the data of an
 event that was recorded.
 
@@ -2835,15 +2835,15 @@
 ## Projections<a id="projections"></a>
 
 Please refer to the [EventStoreDB documentation](https://developers.eventstore.com/server/v23.10/projections.html)
 for more information on projections in EventStoreDB.
 
 ### Create projection<a id="create-projection"></a>
 
-The `create_projection()` method can be used to create a projection.
+The `create_projection()` method can be used to create a "continuous" projection.
 
 This method has two required arguments, `name` and `query`.
 
 This required `name` argument is a Python `str` that specifies the name of the projection.
 
 This required `query` argument is a Python `str` that defines what the projection will do.
 
@@ -2851,16 +2851,16 @@
 `track_emitted_streams`, `timeout`, and `credentials`.
 
 The optional `emit_enabled` argument is a Python `bool` which specifies whether a
 projection will be able to emit events. If a `True` value is specified, the projection
 will be able to emit events, otherwise the projection will not be able to emit events.
 The default value of `emit_enabled` is `False`.
 
-Please note, if your projection query includes a call to `emit()` then `emit_enabled`
-must be `True`, otherwise the projection will not run.
+Please note, `emit_enabled` must be `True` if your projection query includes a call to
+`emit()`, otherwise the projection will not run.
 
 The optional `track_emitted_streams` argument is a Python `bool` which specifies whether
 a projection will have its emitted streams tracked. If a `True` value is specified, the
 projection will have its emitted streams tracked, otherwise the projection will not
 have its emitted streams tracked. The default value of `track_emitted_streams` is `False`.
 
 The purpose of tracking emitted streams is that they can optionally be deleted when
@@ -2905,31 +2905,52 @@
 client.create_projection(
     name=projection_name,
     query=projection_query,
 )
 ```
 
 Please note, the `outputState()` call is optional, and causes the state of the
-projection to be persisted in a "result" stream. The default name of the result stream
-is `$projections-{projection_name}-result`, and this name can be used to read from and
-subscribe to the results stream with the `get_stream()`, `read_stream()`,
-`subscribe_stream()`, `create_subscription_to_stream()` and `read_subscription_to_stream()`
-methods.
-
+projection to be persisted in a "result" stream. If `outputState()` is called, an
+event representing the state of the projection will immediately be written to a
+"result" stream.
+
+The default name of the "result" stream for a projection with name `projection_name`
+is `$projections-{projection_name}-result`. This stream name can be used to read from
+and subscribe to the "result" stream, with the `get_stream()`, or `read_stream()`,
+or `subscribe_to_stream()`, or `create_subscription_to_stream()` and
+`read_subscription_to_stream()` methods.
+
+If your projections doesn't call `outputState()`, then you won't be able to read or
+subscribe to a "result" stream, but you will still be able to get the projection
+"result" using the `get_projection_result()` method.
+
+The "type" string of events recorded in "result" streams is `'Result'`. You may want to
+include this in a `filter_exclude` argument when filtering events by type whilst reading
+or subscribing to "all" events recorded in the database (with `read_all()`,
+`subscribe_to_all()`, etc).
+
+Additionally, and in any case, from time to time the state of the projection will be
+recorded in a "state" stream, and also the projection will write to a "checkpoint"
+stream. The "state" stream, the "checkpoint" stream, and all "emitted" streams that
+have been "tracked" (as a consequence of the `track_emitted_streams` argument having
+been `True`) can optionally be deleted when the projection is deleted. See
+`delete_projection()` for details.
+
+Unlike the "result" and "emitted" streams, the "state" and the "checkpoint" streams
+cannot be read or subscribed to by users, or viewed in the "stream browser" view of
+EventStoreDB's Web interface.
 
 ### Get projection state<a id="get-projection-state"></a>
 
-The `get_projection_state()` method can be used to get a projection's state.
+The `get_projection_state()` method can be used to get a projection's "state".
 
 This method has a required `name` argument, which is a Python `str` that
 specifies the name of a projection.
 
-This method also has three optional arguments, `partition`, `timeout`, and `credentials`.
-
-The optional `partition` argument is a Python `str` which specifies a partition...
+This method also has two optional arguments, `timeout` and `credentials`.
 
 The optional `timeout` argument is a Python `float` which sets a
 maximum duration, in seconds, for the completion of the gRPC operation.
 
 The optional `credentials` argument can be used to
 override call credentials derived from the connection string URI.
 
@@ -2943,22 +2964,22 @@
 projection_state = client.get_projection_state(name=projection_name)
 
 assert projection_state.value == {'count': 3}
 ```
 
 ### Get projection result<a id="get-projection-result"></a>
 
-The `get_projection_result()` method can be used to get a projection's result.
+The `get_projection_result()` method can be used to get a projection's "result".
+
+A projection's "result" holds the same data as the projections "state".
 
 This method has a required `name` argument, which is a Python `str` that
 specifies the name of a projection.
 
-This method also has three optional arguments, `partition`, `timeout`, and `credentials`.
-
-The optional `partition` argument is a Python `str` which specifies a partition.
+This method also has two optional arguments, `timeout` and `credentials`.
 
 The optional `timeout` argument is a Python `float` which sets a
 maximum duration, in seconds, for the completion of the gRPC operation.
 
 The optional `credentials` argument can be used to
 override call credentials derived from the connection string URI.
 
@@ -2969,22 +2990,20 @@
 projection_result = client.get_projection_result(name=projection_name)
 
 assert projection_result.value == {'count': 3}
 ```
 
 ### Get projection statistics<a id="get-projection-statistics"></a>
 
-The `get_projection_statistucs()` method can be used to get projection statistics.
+The `get_projection_statistics()` method can be used to get projection statistics.
 
 This method has a required `name` argument, which is a Python `str` that specifies the
 name of a projection.
 
-This method also has three optional arguments, `partition`, `timeout`, and `credentials`.
-
-The optional `partition` argument is a Python `str` which specifies a partition.
+This method also has two optional arguments, `timeout` and `credentials`.
 
 The optional `timeout` argument is a Python `float` which sets a
 maximum duration, in seconds, for the completion of the gRPC operation.
 
 The optional `credentials` argument can be used to
 override call credentials derived from the connection string URI.
 
@@ -3012,16 +3031,16 @@
 This method also has three optional arguments, `emit_enabled`, `timeout`, and `credentials`.
 
 The optional `emit_enabled` argument is a Python `bool` which specifies whether a
 projection will be able to emit events. If a `True` value is specified, the projection
 will be able to emit events. If a `False` value is specified, the projection will not
 be able to emit events. The default value of `emit_enabled` is `False`.
 
-Please note, if your projection query includes a call to `emit()` then `emit_enabled`
-must be `True`, otherwise the projection will not run.
+Please note, `emit_enabled` must be `True` if your projection query includes a call
+to `emit()`, otherwise the projection will not run.
 
 Please note, it is not possible to update `track_emitted_streams` via the gRPC API.
 
 The optional `timeout` argument is a Python `float` which sets a
 maximum duration, in seconds, for the completion of the gRPC operation.
 
 The optional `credentials` argument can be used to
@@ -3029,16 +3048,16 @@
 
 ```python
 client.update_projection(name=projection_name, query=projection_query)
 ```
 
 ### Enable projection<a id="enable-projection"></a>
 
-The `enable_projection()` method can be used to enable a projection that was previously
-disabled.
+The `enable_projection()` method can be used to enable (start running) a projection
+that was previously disabled (stopped).
 
 This method has a required `name` argument, which is a Python `str` that
 specifies the name of the projection to be enabled.
 
 This method also has two optional arguments, `timeout` and `credentials`.
 
 The optional `timeout` argument is a Python `float` which sets a
@@ -3049,25 +3068,20 @@
 
 ```python
 client.enable_projection(name=projection_name)
 ```
 
 ### Disable projection<a id="disable-projection"></a>
 
-The `disable_projection()` method can be used to disable a projection.
+The `disable_projection()` method can be used to disable (stop running) a projection.
 
 This method has a required `name` argument, which is a Python `str` that
 specifies the name of the projection to be disabled.
 
-This method also has three optional arguments, `write_checkpoint`, `timeout`, and `credentials`.
-
-The optional `write_checkpoint` argument is a Python `bool` which specifies whether
-a checkpoint will be written when the projection is disabled. If `write_checkpoint`
-is `True` a checkpoint will be written, otherwise a checkpoint will not be written.
-The default value of `write_checkpoint` is `False`.
+This method also has two optional arguments, `timeout`, and `credentials`.
 
 The optional `timeout` argument is a Python `float` which sets a
 maximum duration, in seconds, for the completion of the gRPC operation.
 
 The optional `credentials` argument can be used to
 override call credentials derived from the connection string URI.
 
@@ -3078,60 +3092,65 @@
 ### Reset projection<a id="reset-projection"></a>
 
 The `reset_projection()` method can be used to reset a projection.
 
 This method has a required `name` argument, which is a Python `str` that
 specifies the name of the projection to be reset.
 
-This method also has three optional arguments, `write_checkpoint`, `timeout`, and `credentials`.
-
-The optional `write_checkpoint` argument is a Python `bool` which specifies whether
-a checkpoint will be written when the projection is reset. If `write_checkpoint`
-is `True` a checkpoint will be written, otherwise a checkpoint will not be written.
-The default value of `write_checkpoint` is `False`.
+This method also has two optional arguments, `timeout`, and `credentials`.
 
 The optional `timeout` argument is a Python `float` which sets a
 maximum duration, in seconds, for the completion of the gRPC operation.
 
 The optional `credentials` argument can be used to
 override call credentials derived from the connection string URI.
 
 ```python
 client.reset_projection(name=projection_name)
 ```
 
+Please note, a projection must be disabled before it can be reset.
+
+
 ### Delete projection<a id="delete-projection"></a>
 
 The `delete_projection()` method can be used to delete a projection.
 
 This method has a required `name` argument, which is a Python `str` that
 specifies the name of the projection to be deleted.
 
 This method also has five optional arguments, `delete_emitted_streams`,
 `delete_state_stream`, `delete_checkpoint_stream`, `timeout`, and `credentials`.
 
 The optional `delete_emitted_streams` argument is a Python `bool` which specifies
-that the emitted streams will be deleted. For emitted streams to be deleted, they
-must have been tracked (see the `track_emitted_streams` argument of the `create_projection()`
-method.)
-
-The optional `delete_state_stream` argument is a Python `bool` which...
+that all "emitted" streams that have been tracked will be deleted. For emitted streams
+to be deleted, they must have been tracked (see the `track_emitted_streams` argument of
+the `create_projection()` method.)
+
+The optional `delete_state_stream` argument is a Python `bool` which specifies that
+the projection's "state" stream should also be deleted. The "state" stream is like
+the "result" stream, but events are written to the "state" stream occasionally, along
+with events written to the "checkpoint" stream, rather than being written immediately
+in the way a call `outputState()` immediately writes events to the "result" stream.
 
-The optional `delete_checkpoint_stream` argument is a Python `bool` which...
+The optional `delete_checkpoint_stream` argument is a Python `bool` which specifies
+that the projection's "checkpoint" stream should also be deleted.
 
 The optional `timeout` argument is a Python `float` which sets a
 maximum duration, in seconds, for the completion of the gRPC operation.
 
 The optional `credentials` argument can be used to
 override call credentials derived from the connection string URI.
 
 ```python
 client.delete_projection(name=projection_name)
 ```
 
+Please note, a projection must be disabled before it can be deleted.
+
 ### Restart projections subsystem<a id="restart-projections-subsystem"></a>
 
 The `restart_projections_subsystem()` method can be used to restart the projections subsystem.
 
 This method also has two optional arguments, `timeout` and `credentials`.
 
 The optional `timeout` argument is a Python `float` which sets a
@@ -3150,14 +3169,19 @@
 Default call credentials are derived by the client from the user info part of the
 connection string URI.
 
 Many of the client methods described above have an optional `credentials` argument,
 which can be used to set call credentials for an individual method call that override
 those derived from the connection string URI.
 
+Call credentials are sent to "secure" servers in a "basic auth" authorization header.
+This authorization header is used by the server to authenticate the client. The
+authorization header is not sent to "insecure" servers.
+
+
 ### Construct call credentials<a id="construct-call-credentials"></a>
 
 The client method `construct_call_credentials()` can be used to construct a call
 credentials object from a username and password.
 
 ```python
 call_credentials = client.construct_call_credentials(
@@ -3394,14 +3418,21 @@
 then the client will reconnect and retry. However, if an exception is raised when iterating over a
 successfully returned "catch-up subscription" object, the catch-up subscription will
 need to be restarted. Similarly, when reading persistent subscriptions, if there are
 connection issues whilst iterating over a successfully received response, the consumer
 will need to be restarted.
 
 
+## Communities<a id="communities"></a>
+
+- [Issues](https://github.com/pyeventsourcing/esdbclient/issues)
+- [Discuss](https://discuss.eventstore.com/)
+- [Discord (Event Store)](https://discord.gg/Phn9pmCw3t)
+
+
 ## Contributors<a id="contributors"></a>
 
 ### Install Poetry<a id="install-poetry"></a>
 
 The first thing is to check you have Poetry installed.
 
     $ poetry --version
```

#### html2text {}

```diff
@@ -1,54 +1,101 @@
 # Python gRPC Client for EventStoreDB This [Python package](https://pypi.org/
 project/esdbclient/) provides multithreaded and asyncio Python clients for the
 [EventStoreDB](https://www.eventstore.com/) database. The multithreaded
 `EventStoreDBClient` is described in detail below. Please scroll down for
 _i_n_f_o_r_m_a_t_i_o_n about `AsyncioEventStoreDBClient`. These clients have been
 developed and are being maintained in a collaboration with the EventStoreDB
-team, and are officially support by Event Store Ltd. Although not all the
-features of EventStoreDB are supported, many of the most useful features are
-presented in an easy-to-use interface. These clients have been tested to work
-with EventStoreDB LTS versions 21.10, 22.10, 23.10, and version 24.2, without
-and without SSL/TLS, with single-server and cluster modes, and with Python
-versions 3.7, 3.8, 3.9, 3.10, 3.11 and 3.12. The test suite has 100% line and
-branch coverage. The code has typing annotations checked strictly with mypy.
-The code is formatted with black and isort, and checked with flake8. Poetry is
-used for package management during development, and for building and publishing
-distributions to [PyPI](https://pypi.org/project/esdbclient/). ## Synopsis The
-`EventStoreDBClient` class can be imported from the `esdbclient` package.
-Probably the three most useful methods of `EventStoreDBClient` are: *
-`append_to_stream()` This method can be used to record new events in a
-particular "stream". This is useful, for example, when executing a command in
-an application that mutates an aggregate. This method is "atomic" in that
-either all or none of the events will be recorded. * `get_stream()` This method
-can be used to retrieve all the recorded events in a "stream". This is useful,
-for example, when reconstructing an aggregate from recorded events before
-executing a command in an application that creates new events. *
-`subscribe_to_all()` This method can be used to receive all recorded events in
-the database. This is useful, for example, in event-processing components
-because it supports processing events with "exactly-once" semantics. The
-example below uses an "insecure" EventStoreDB server running locally on port
-2113. ```python import uuid from esdbclient import EventStoreDBClient,
-NewEvent, StreamState # Construct EventStoreDBClient with an EventStoreDB URI.
-The # connection string URI specifies that the client should # connect to an
-"insecure" server running on port 2113. client = EventStoreDBClient( uri="esdb:
-//localhost:2113?Tls=false" ) # Generate new events. Typically, domain events
-of different # types are generated in a domain model, and then serialized #
-into NewEvent objects. An aggregate ID may be used as the # name of a stream in
-EventStoreDB. stream_name1 = str(uuid.uuid4()) event1 = NewEvent
-( type='OrderCreated', data=b'{"order_number": "123456"}' ) event2 = NewEvent
-( type='OrderSubmitted', data=b'{}' ) event3 = NewEvent( type='OrderCancelled',
-data=b'{}' ) # Append new events to a new stream. The value returned # from the
-append_to_stream() method is the overall # "commit position" in the database of
-the last new event # recorded by this operation. The returned "commit position"
-# may be used in a user interface to poll an eventually # consistent event-
-processing component until it can # present an up-to-date materialized view.
-New events are # each allocated a "stream position", which is the next #
-available position in the stream, starting from 0. commit_position1 =
-client.append_to_stream( stream_name=stream_name1,
+team, and are officially support by Event Store Ltd. Although not all aspects
+of the EventStoreDB gRPC API are implemented, many of the most useful features
+are presented in an easy-to-use interface. These clients have been tested to
+work with EventStoreDB LTS versions 22.10 and 23.10, and release candidates
+24.2 and 24.6, without and without SSL/TLS, with both single-server and cluster
+modes, and with Python versions 3.7, 3.8, 3.9, 3.10, 3.11 and 3.12. The test
+suite has 100% line and branch coverage. The code has typing annotations
+checked strictly with mypy. The code is formatted with black and isort, and
+checked with flake8. Poetry is used for package management during development,
+and for building and publishing distributions to [PyPI](https://pypi.org/
+project/esdbclient/). For an example of usage, see the [eventsourcing-
+eventstoredb]( https://github.com/pyeventsourcing/eventsourcing-eventstoredb)
+package. * [Synopsis](#synopsis) * [Install package](#install-package) * [From
+PyPI](#from-pypi) * [With Poetry](#with-poetry) * [EventStoreDB server]
+(#eventstoredb-server) * [Run container](#run-container) * [Stop container]
+(#stop-container) * [EventStoreDB client](#eventstoredb-client) * [Import
+class](#import-class) * [Construct client](#construct-client) * [Connection
+strings](#connection-strings) * [Two schemes](#two-schemes) * [User info
+string](#user-info-string) * [Query string](#query-string) * [Examples]
+(#examples) * [Event objects](#event-objects) * [New events](#new-events) *
+[Recorded events](#recorded-events) * [Streams](#streams) * [Append events]
+(#append-events) * [Idempotent append operations](#idempotent-append-
+operations) * [Read stream events](#read-stream-events) * [Get current version]
+(#get-current-version) * [How to implement snapshotting with EventStoreDB]
+(#how-to-implement-snapshotting-with-eventstoredb) * [Read all events](#read-
+all-events) * [Get commit position](#get-commit-position) * [Get stream
+metadata](#get-stream-metadata) * [Set stream metadata](#set-stream-metadata) *
+[Delete stream](#delete-stream) * [Tombstone stream](#tombstone-stream) *
+[Catch-up subscriptions](#catch-up-subscriptions) * [Subscribe to all events]
+(#subscribe-to-all-events) * [Subscribe to stream events](#subscribe-to-stream-
+events) * [How to implement exactly-once event processing](#how-to-implement-
+exactly-once-event-processing) * [Persistent subscriptions](#persistent-
+subscriptions) * [Create subscription to all](#create-subscription-to-all) *
+[Read subscription to all](#read-subscription-to-all) * [How to write a
+persistent subscription consumer](#how-to-write-a-persistent-subscription-
+consumer) * [Update subscription to all](#update-subscription-to-all) * [Create
+subscription to stream](#create-subscription-to-stream) * [Read subscription to
+stream](#read-subscription-to-stream) * [Update subscription to stream]
+(#update-subscription-to-stream) * [Replay parked events](#replay-parked-
+events) * [Get subscription info](#get-subscription-info) * [List
+subscriptions](#list-subscriptions) * [List subscriptions to stream](#list-
+subscriptions-to-stream) * [Delete subscription](#delete-subscription) *
+[Projections](#projections) * [Create projection](#create-projection) * [Get
+projection state](#get-projection-state) * [Get projection result](#get-
+projection-result) * [Get projection statistics](#get-projection-statistics) *
+[Update projection](#update-projection) * [Enable projection](#enable-
+projection) * [Disable projection](#disable-projection) * [Reset projection]
+(#reset-projection) * [Delete projection](#delete-projection) * [Restart
+projections subsystem](#restart-projections-subsystem) * [Call credentials]
+(#call-credentials) * [Construct call credentials](#construct-call-credentials)
+* [Connection](#connection) * [Reconnect](#reconnect) * [Close](#close) *
+[Asyncio client](#asyncio-client) * [Synopsis](#synopsis-1) * [Notes](#notes) *
+[Regular expression filters](#regular-expression-filters) * [Reconnect and
+retry method decorators](#reconnect-and-retry-method-decorators) *
+[Communities](#communities) * [Contributors](#contributors) * [Install Poetry]
+(#install-poetry) * [Setup for PyCharm users](#setup-for-pycharm-users) *
+[Setup from command line](#setup-from-command-line) * [Project Makefile
+commands](#project-makefile-commands) ## Synopsis The `EventStoreDBClient`
+class can be imported from the `esdbclient` package. Probably the three most
+useful methods of `EventStoreDBClient` are: * `append_to_stream()` This method
+can be used to record new events in a particular "stream". This is useful, for
+example, when executing a command in an application that mutates an aggregate.
+This method is "atomic" in that either all or none of the events will be
+recorded. * `get_stream()` This method can be used to retrieve all the recorded
+events in a "stream". This is useful, for example, when reconstructing an
+aggregate from recorded events before executing a command in an application
+that creates new events. * `subscribe_to_all()` This method can be used to
+receive all recorded events in the database. This is useful, for example, in
+event-processing components because it supports processing events with
+"exactly-once" semantics. The example below uses an "insecure" EventStoreDB
+server running locally on port 2113. ```python import uuid from esdbclient
+import EventStoreDBClient, NewEvent, StreamState # Construct EventStoreDBClient
+with an EventStoreDB URI. The # connection string URI specifies that the client
+should # connect to an "insecure" server running on port 2113. client =
+EventStoreDBClient( uri="esdb://localhost:2113?Tls=false" ) # Generate new
+events. Typically, domain events of different # types are generated in a domain
+model, and then serialized # into NewEvent objects. An aggregate ID may be used
+as the # name of a stream in EventStoreDB. stream_name1 = str(uuid.uuid4())
+event1 = NewEvent( type='OrderCreated', data=b'{"order_number": "123456"}' )
+event2 = NewEvent( type='OrderSubmitted', data=b'{}' ) event3 = NewEvent
+( type='OrderCancelled', data=b'{}' ) # Append new events to a new stream. The
+value returned # from the append_to_stream() method is the overall # "commit
+position" in the database of the last new event # recorded by this operation.
+The returned "commit position" # may be used in a user interface to poll an
+eventually # consistent event-processing component until it can # present an
+up-to-date materialized view. New events are # each allocated a "stream
+position", which is the next # available position in the stream, starting from
+0. commit_position1 = client.append_to_stream( stream_name=stream_name1,
 current_version=StreamState.NO_STREAM, events=[event1, event2], ) # Append
 events to an existing stream. The "current version" # is the "stream position"
 of the last recorded event in a # stream. We have recorded two new events, so
 the "current # version" is 1. The exception 'WrongCurrentVersion' will be #
 raised if an incorrect value is given. commit_position2 =
 client.append_to_stream( stream_name=stream_name1, current_version=1, events=
 [event3], ) # - allocated commit positions increase monotonically assert
@@ -83,90 +130,44 @@
 example. break # - events are received in the order they were recorded assert
 received_events[-3].type == "OrderCreated" assert received_events[-3].data ==
 b'{"order_number": "123456"}' assert received_events[-3].id == event1.id assert
 received_events[-2].type == "OrderSubmitted" assert received_events[-2].data ==
 b'{}' assert received_events[-2].id == event2.id assert received_events[-
 1].type == "OrderCancelled" assert received_events[-1].data == b'{}' assert
 received_events[-1].id == event3.id # Close the client's gRPC connection.
-client.close() ``` See below for more details. For an example of usage, see the
-[eventsourcing-eventstoredb]( https://github.com/pyeventsourcing/eventsourcing-
-eventstoredb) package. ## Table of contents * [Install package](#install-
-package) * [From PyPI](#from-pypi) * [With Poetry](#with-poetry) *
-[EventStoreDB server](#eventstoredb-server) * [Run container](#run-container) *
-[Stop container](#stop-container) * [EventStoreDB client](#eventstoredb-client)
-* [Import class](#import-class) * [Construct client](#construct-client) *
-[Connection strings](#connection-strings) * [Two schemes](#two-schemes) * [User
-info string](#user-info-string) * [Query string](#query-string) * [Examples]
-(#examples) * [Event objects](#event-objects) * [New events](#new-events) *
-[Recorded events](#recorded-events) * [Streams](#streams) * [Append events]
-(#append-events) * [Idempotent append operations](#idempotent-append-
-operations) * [Read stream events](#read-stream-events) * [Get current version]
-(#get-current-version) * [How to implement snapshotting with EventStoreDB]
-(#how-to-implement-snapshotting-with-eventstoredb) * [Read all events](#read-
-all-events) * [Get commit position](#get-commit-position) * [Get stream
-metadata](#get-stream-metadata) * [Set stream metadata](#set-stream-metadata) *
-[Delete stream](#delete-stream) * [Tombstone stream](#tombstone-stream) *
-[Catch-up subscriptions](#catch-up-subscriptions) * [Subscribe to all events]
-(#subscribe-to-all-events) * [Subscribe to stream events](#subscribe-to-stream-
-events) * [How to implement exactly-once event processing](#how-to-implement-
-exactly-once-event-processing) * [Persistent subscriptions](#persistent-
-subscriptions) * [Create subscription to all](#create-subscription-to-all) *
-[Read subscription to all](#read-subscription-to-all) * [How to write a
-persistent subscription consumer](#how-to-write-a-persistent-subscription-
-consumer) * [Update subscription to all](#update-subscription-to-all) * [Create
-subscription to stream](#create-subscription-to-stream) * [Read subscription to
-stream](#read-subscription-to-stream) * [Update subscription to stream]
-(#update-subscription-to-stream) * [Replay parked events](#replay-parked-
-events) * [Get subscription info](#get-subscription-info) * [List
-subscriptions](#list-subscriptions) * [List subscriptions to stream](#list-
-subscriptions-to-stream) * [Delete subscription](#delete-subscription) *
-[Projections](#projections) * [Create projection](#create-projection) * [Get
-projection state](#get-projection-state) * [Get projection result](#get-
-projection-result) * [Get projection statistics](#get-projection-statistics) *
-[Update projection](#update-projection) * [Enable projection](#enable-
-projection) * [Disable projection](#disable-projection) * [Reset projection]
-(#reset-projection) * [Delete projection](#delete-projection) * [Restart
-projections subsystem](#restart-projections-subsystem) * [Call credentials]
-(#call-credentials) * [Construct call credentials](#construct-call-credentials)
-* [Connection](#connection) * [Reconnect](#reconnect) * [Close](#close) *
-[Asyncio client](#asyncio-client) * [Synopsis](#synopsis-1) * [Notes](#notes) *
-[Regular expression filters](#regular-expression-filters) * [Reconnect and
-retry method decorators](#reconnect-and-retry-method-decorators) *
-[Contributors](#contributors) * [Install Poetry](#install-poetry) * [Setup for
-PyCharm users](#setup-for-pycharm-users) * [Setup from command line](#setup-
-from-command-line) * [Project Makefile commands](#project-makefile-commands) ##
-Install package It is recommended to install Python packages into a Python
-virtual environment. ### From PyPI You can use pip to install this package
-directly from [the Python Package Index](https://pypi.org/project/esdbclient/).
-$ pip install esdbclient ### With Poetry You can use Poetry to add this package
-to your pyproject.toml and install it. $ poetry add esdbclient ## EventStoreDB
-server The EventStoreDB server can be run locally using the official Docker
-container image. ### Run container For development, you can run a "secure"
-EventStoreDB server using the following command. $ docker run -d --name
-eventstoredb-secure -it -p 2113:2113 --env "HOME=/tmp" eventstore/eventstore:
-21.10.9-buster-slim --dev As we will see, your client will need an EventStoreDB
-connection string URI as the value of its `uri` constructor argument. The
-connection string for this "secure" EventStoreDB server would be: esdb://admin:
-changeit@localhost:2113 To connect to a "secure" server, you will usually need
-to include a "username" and a "password" in the connection string, so that the
-server can authenticate the client. With EventStoreDB, the default username is
-"admin" and the default password is "changeit". When connecting to a "secure"
-server, you may also need to provide an SSL/TLS certificate as the value of the
-`root_certificates` constructor argument. If the server certificate is publicly
-signed, the root certificates of the certificate authority may be installed
-locally and picked up by the grpc package from a default location. The client
-uses the root SSL/TLS certificate to authenticate the server. For development,
-you can either use the SSL/TLS certificate of a self-signing certificate
-authority used to create the server's certificate. Or, when using a single-node
-cluster, you can just use the server certificate itself, getting the server
-certificate with the following Python code. ```python import ssl
-server_certificate = ssl.get_server_certificate(addr=('localhost', 2113)) ```
-Alternatively, you can start an "insecure" server using the following command.
-$ docker run -d --name eventstoredb-insecure -it -p 2113:2113 eventstore/
-eventstore:21.10.9-buster-slim --insecure The connection string URI for this
+client.close() ``` ## Install package It is recommended to install Python
+packages into a Python virtual environment. ### From PyPI You can use pip to
+install this package directly from [the Python Package Index](https://pypi.org/
+project/esdbclient/). $ pip install esdbclient ### With Poetry You can use
+Poetry to add this package to your pyproject.toml and install it. $ poetry add
+esdbclient ## EventStoreDB server The EventStoreDB server can be run locally
+using the official Docker container image. ### Run container For development,
+you can run a "secure" EventStoreDB server using the following command. $
+docker run -d --name eventstoredb-secure -it -p 2113:2113 --env "HOME=/tmp"
+docker.eventstore.com/eventstore-ce/eventstoredb-ce:23.10.0-jammy --dev As we
+will see, your client will need an EventStoreDB connection string URI as the
+value of its `uri` constructor argument. The connection string for this
+"secure" EventStoreDB server would be: esdb://admin:changeit@localhost:2113 To
+connect to a "secure" server, you will usually need to include a "username" and
+a "password" in the connection string, so that the server can authenticate the
+client. With EventStoreDB, the default username is "admin" and the default
+password is "changeit". When connecting to a "secure" server, you may also need
+to provide an SSL/TLS certificate as the value of the `root_certificates`
+constructor argument. If the server certificate is publicly signed, the root
+certificates of the certificate authority may be installed locally and picked
+up by the grpc package from a default location. The client uses the root SSL/
+TLS certificate to authenticate the server. For development, you can either use
+the SSL/TLS certificate of a self-signing certificate authority used to create
+the server's certificate. Or, when using a single-node cluster, you can just
+use the server certificate itself, getting the server certificate with the
+following Python code. ```python import ssl server_certificate =
+ssl.get_server_certificate(addr=('localhost', 2113)) ``` Alternatively, you can
+start an "insecure" server using the following command. $ docker run -d --name
+eventstoredb-insecure -it -p 2113:2113 docker.eventstore.com/eventstore-ce/
+eventstoredb-ce:23.10.0-jammy --insecure The connection string URI for this
 "insecure" server would be: esdb://localhost:2113?Tls=false As we will see,
 when connecting to an "insecure" server, there is no need to include a
 "username" and a "password" in the connection string. If you do, these values
 will be ignored by the client, so that they are not sent over an insecure
 channel. Please note, the "insecure" connection string uses a query string with
 the field-value `Tls=false`. The value of this field is by default `true`. ###
 Stop container To stop and remove the "secure" container, use the following
@@ -176,42 +177,32 @@
 ## EventStoreDB client This EventStoreDB client is implemented in the
 `esdbclient` package with the `EventStoreDBClient` class. ### Import class The
 `EventStoreDBClient` class can be imported from the `esdbclient` package.
 ```python from esdbclient import EventStoreDBClient ``` ### Construct client
 The `EventStoreDBClient` class has one required constructor argument, `uri`,
 and one optional constructor argument, `root_certificates`. The `uri` argument
 is expected to be an EventStoreDB connection string URI that conforms with the
-standard EventStoreDB "esdb" or "esdb+discover" URI schemes. For example, the
-following connection string specifies that the client should attempt to create
-a "secure" connection to port 2113 on "localhost", and use the client
-credentials "username" and "password" when making calls to the server. esdb://
-username:password@localhost:2113?Tls=true The client must be configured to
-create a "secure" connection to a "secure" server, or alternatively an
-"insecure" connection to an "insecure" server. By default, the client will
-attempt to create a "secure" connection. And so, when connecting to an
-"insecure" server, the connection string must specify that the client should
-attempt to make an "insecure" connection. The following connection string
-specifies that the client should attempt to create an "insecure" connection to
-port 2113 on "localhost". When connecting to an "insecure" server, the client
-will ignore any username and password information included in the connection
-string, so that usernames and passwords are not sent over an "insecure"
-connection. esdb://localhost:2113?Tls=false Please note, the "insecure"
-connection string uses a query string with the field-value `Tls=false`. The
-value of this field is by default `true`. When connecting to a "secure" server,
-the `root_certificates` argument can be a Python `str` containing PEM encoded
+standard EventStoreDB "esdb" or "esdb+discover" URI schemes. The client must be
+configured to create a "secure" connection to a "secure" server, or
+alternatively an "insecure" connection to an "insecure" server. By default, the
+client will attempt to create a "secure" connection. And so, when connecting to
+an "insecure" server, the connection string must specify that the client should
+attempt to make an "insecure" connection. When connecting to a "secure" server,
+it may be necessary to set the optional `root_certificates` argument. The
+optional `root_certificates` argument is a Python `str` containing PEM encoded
 SSL/TLS root certificates. This value is passed directly to
-`grpc.ssl_channel_credentials()`. It is used for authenticating the server to
-the client. It is commonly the certificate of the certificate authority that
-was responsible for generating the SSL/TLS certificate used by the EventStoreDB
-server. Often it is unnecessary to provide these certificates explicitly, if
-they are installed locally in a such a way that the Python grpc library can
-pick them up from a default location. Alternatively, for development, you can
-use the server's certificate itself. In the example below, the constructor
-argument values are taken from the operating system environment. ```python
-import os client = EventStoreDBClient( uri=os.getenv("ESDB_URI"),
+`grpc.ssl_channel_credentials()` and is used by the client to authenticate the
+server. It is commonly a public certificate of the certificate authority that
+was responsible for generating the certificate used by the EventStoreDB server.
+Often it is unnecessary to provide these certificates explicitly, as they are
+commonly installed locally in a default location such that the Python grpc
+library can pick them up. Alternatively, for development, you can use the
+server's certificate itself. In the example below, the constructor argument
+values are taken from the operating system environment. ```python import os
+client = EventStoreDBClient( uri=os.getenv("ESDB_URI"),
 root_certificates=os.getenv("ESDB_ROOT_CERTIFICATES"), ) ``` ## Connection
 strings An EventStoreDB connection string is a URI that conforms with one of
 two possible schemes: either the "esdb" scheme, or the "esdb+discover" scheme.
 The syntax and semantics of the EventStoreDB URI schemes are described below.
 The syntax is defined using [EBNF](https://en.wikipedia.org/wiki/
 Extended_BackusâNaur_form). ### Two schemes The "esdb" URI scheme can be
 defined in the following way. esdb-uri = "esdb://" , [ user-info , "@" ] ,
@@ -222,129 +213,148 @@
 gRPC server socket, all in the same EventStoreDB cluster, by specifying a host
 and a port number separated with the ":" character. The host may be a hostname
 that can be resolved to an IP address, or an IP address. grpc-target =
 ( hostname | ip-address ) , ":" , port-number ; If there is one gRPC target,
 the client will simply attempt to connect to this server, and it will use this
 connection when recording and retrieving events. If there are two or more gRPC
 targets, the client will attempt to connect to the Gossip API of each in turn,
-to obtain information about the whole cluster. A member of the cluster is then
-selected by the client according to the "node preference" option of the
-connection string. The client may then need to close its connection and
-reconnect to the selected node. The "esdb+discover" URI scheme can be defined
-in the following way. esdb-discover-uri = "esdb+discover://" , [ user-info, "@"
-] , cluster-domainname, [ ":" , port-number ] , [ "?" , query-string ] ; In the
-"esdb+discover" URI scheme, after the optional user info string, there should
-be a domain name which identifies a cluster of EventStoreDB servers. Individual
-nodes in the cluster should be declared with DNS 'A' records. The client will
-create a gRPC connection using the cluster's domain name, using the gRPC
-library's 'round robin' load balancing strategy to call the Gossip API of
-addresses to which this domain name resolves. Information about the
-EventStoreDB cluster is obtained from the Gossip API. A member of the cluster
-is then selected by the client according to the "node preference" option. The
-client may then need to close its connection and reconnect to the selected
-node. ### User info string In both the "esdb" and "esdb+discover" schemes, the
-URI may include a user info string. If it exists in the URI, the user info
-string must be separated from the rest of the URI with the "@" character. The
-user info string must include a username and a password, separated with the ":
-" character. user-info = username , ":" , password ; The user info is sent by
-the client as "call credentials" in each call to a "secure" server, in a "basic
-auth" authorization header. This authorization header is used by the server to
-authenticate the client. The authorization header is not sent to "insecure"
-servers. ### Query string In both the "esdb" and "esdb+discover" schemes, the
-optional query string must be one or many field-value arguments, separated from
-each other with the "&" character. query-string = field-value, { "&", field-
-value } ; Each field-value argument must be one of the supported fields, and an
-appropriate value, separated with the "=" character. field-value = ( "Tls", "="
-, "true" | "false" ) | ( "TlsVerifyCert", "=" , "true" | "false" ) |
-( "ConnectionName", "=" , string ) | ( "NodePreference", "=" , "leader" |
-"follower" | "readonlyreplica" | "random" ) | ( "DefaultDeadline", "=" ,
-integer ) | ( "GossipTimeout", "=" , integer ) | ( "MaxDiscoverAttempts", "=" ,
-integer ) | ( "DiscoveryInterval", "=" , integer ) | ( "KeepAliveInterval", "="
-, integer ) | ( "KeepAliveTimeout", "=" , integer ) ; The table below describes
-the query field-values supported by this client. | Field | Value | Description
-| |---------------------|------------------------------------------------------
------------------|-------------------------------------------------------------
+attempting to obtain information about the cluster from it, until information
+about the cluster is obtained. A member of the cluster is then selected by the
+client according to the "node preference" specified by the connection string
+URI. The client will then close its connection and connect to the selected node
+without the 'round robin' load balancing strategy. If the "node preference" is
+"leader", and after connecting to a leader, if the leader becomes a follower,
+the client will reconnect to the new leader. The "esdb+discover" URI scheme can
+be defined in the following way. esdb-discover-uri = "esdb+discover://" ,
+[ user-info, "@" ] , cluster-domainname, [ ":" , port-number ] , [ "?" , query-
+string ] ; In the "esdb+discover" URI scheme, after the optional user info
+string, there should be a domain name which identifies a cluster of
+EventStoreDB servers. Individual nodes in the cluster should be declared with
+DNS 'A' records. The client will use the cluster domain name with the gRPC
+library's 'round robin' load balancing strategy to call the Gossip APIs of
+addresses discovered from DNS 'A' records. Information about the EventStoreDB
+cluster is obtained from the Gossip API. A member of the cluster is then
+selected by the client according to the "node preference" option. The client
+will then close its connection and connect to the selected node without the
+'round robin' load balancing strategy. If the "node preference" is "leader",
+and after connecting to a leader, if the leader becomes a follower, the client
+will reconnect to the new leader. ### User info string In both the "esdb" and
+"esdb+discover" schemes, the URI may include a user info string. If it exists
+in the URI, the user info string must be separated from the rest of the URI
+with the "@" character. The user info string must include a username and a
+password, separated with the ":" character. user-info = username , ":" ,
+password ; The user info is sent by the client in a "basic auth" authorization
+header in each gRPC call to a "secure" server. This authorization header is
+used by the server to authenticate the client. The Python gRPC library does not
+allow call credentials to be transferred to "insecure" servers. ### Query
+string In both the "esdb" and "esdb+discover" schemes, the optional query
+string must be one or many field-value arguments, separated from each other
+with the "&" character. query-string = field-value, { "&", field-value } ; Each
+field-value argument must be one of the supported fields, and an appropriate
+value, separated with the "=" character. field-value = ( "Tls", "=" , "true" |
+"false" ) | ( "TlsVerifyCert", "=" , "true" | "false" ) | ( "ConnectionName",
+"=" , string ) | ( "NodePreference", "=" , "leader" | "follower" |
+"readonlyreplica" | "random" ) | ( "DefaultDeadline", "=" , integer ) |
+( "GossipTimeout", "=" , integer ) | ( "MaxDiscoverAttempts", "=" , integer ) |
+( "DiscoveryInterval", "=" , integer ) | ( "KeepAliveInterval", "=" , integer )
+| ( "KeepAliveTimeout", "=" , integer ) ; The table below describes the query
+field-values supported by this client. | Field | Value | Description | |-------
+--------------|----------------------------------------------------------------
+-------|-----------------------------------------------------------------------
 -------------------------------------------------------------------------------
------------------------| | Tls | "true", "false" (default: "true") | If "true"
-the client will create a "secure" gRPC channel. If "false" the client will
-create an "insecure" gRPC channel. This must match the server configuration. |
-| TlsVerifyCert | "true", "false" (default: "true") | This value is currently
+-------------| | Tls | "true", "false" (default: "true") | If "true" the client
+will create a "secure" gRPC channel. If "false" the client will create an
+"insecure" gRPC channel. This must match the server configuration. | |
+TlsVerifyCert | "true", "false" (default: "true") | This value is currently
 ignored. | | ConnectionName | string (default: auto-generated version-4 UUID) |
 Sent in call metadata for every call, to identify the client to the cluster. |
 | NodePreference | "leader", "follower", "readonlyreplica", "random" (default:
 "leader") | The node state preferred by the client. The client will select a
 node from the cluster info received from the Gossip API according to this
 preference. | | DefaultDeadline | integer (default: `None`) | The default value
 (in seconds) of the `timeout` argument of client "write" methods such as
 `append_to_stream()`. | | GossipTimeout | integer (default: 5) | The default
 value (in seconds) of the `timeout` argument of gossip read methods, such as
 `read_gossip()`. | | MaxDiscoverAttempts | integer (default: 10) | The number
 of attempts to read gossip when connecting or reconnecting to a cluster member.
 | | DiscoveryInterval | integer (default: 100) | How long to wait (in
 milliseconds) between gossip retries. | | KeepAliveInterval | integer (default:
-`None`) | The value of the "grpc.keepalive_ms" gRPC channel option. | |
-KeepAliveTimeout | integer (default: `None`) | The value of the
-"grpc.keepalive_timeout_ms" gRPC channel option. | ### Examples Here are some
-examples of EventStoreDB connection string URIs. The following URI will cause
-the client to connect to, and get cluster info, from "secure" server socket
-`localhost:2113`. And then to connect to a "leader" node. And also to use
-"admin" and "changeit" as the username and password when making calls to
-EventStoreDB API methods. esdb://admin:changeit@localhost:2113 The following
-URI will cause the client to get cluster info from "insecure" server socket
-127.0.0.1:2113. And then to connect to a "leader" node. esdb://127.0.0.1:
-2113?Tls=false The following URI will cause the client to get cluster info from
-addresses in DNS 'A' records for cluster1.example.com. And then to connect to a
-"leader" node. And use a default deadline of 5 seconds when making calls to
-EventStore API "write" methods. esdb+discover://admin:
+`None`) | The value (in milliseconds) of the "grpc.keepalive_ms" gRPC channel
+option. | | KeepAliveTimeout | integer (default: `None`) | The value (in
+milliseconds) of the "grpc.keepalive_timeout_ms" gRPC channel option. | Please
+note, the client is insensitive to the case of fields and values. If fields are
+repeated in the query string, the query string will be parsed without error.
+However, the connection options used by the client will use the value of the
+first field. All the other field-values in the query string with the same field
+name will be ignored. Fields without values will also be ignored. If the
+client's node preference is "follower" and there are no follower nodes in the
+cluster, then the client will raise an exception. Similarly, if the client's
+node preference is "readonlyreplica" and there are no read-only replica nodes
+in the cluster, then the client will also raise an exception. The gRPC channel
+option "grpc.max_receive_message_length" is automatically configured to the
+value `17 * 1024 * 1024`. This value cannot be configured. ### Examples Here
+are some examples of EventStoreDB connection string URIs. The following URI
+will cause the client to make an "insecure" connection to gRPC target
+`'localhost:2113'`. Because the client's node preference is "follower", methods
+that can be called on a follower should complete successfully, methods that
+require a leader will raise a `NodeIsNotLeader` exception. esdb://127.0.0.1:
+2113?Tls=false&NodePreference=follower The following URI will cause the client
+to make an "insecure" connection to gRPC target `'localhost:2113'`. Because the
+client's node preference is "leader", if this node is not a leader, then a
+`NodeIsNotLeader` exception will be raised by all methods. esdb://127.0.0.1:
+2113?Tls=false&NodePreference=leader The following URI will cause the client to
+make a "secure" connection to gRPC target `'localhost:2113'` with username
+`'admin'` and password `'changeit'` as the default call credentials when making
+calls to the EventStoreDB gRPC API. Because the client's node preference is
+"leader", by default, if this node is not a leader, then a `NodeIsNotLeader`
+exception will be raised by all methods. esdb://admin:changeit@localhost:2113
+The following URI will cause the client to make "secure" connections, firstly
+to get cluster info from either `'localhost:2111'`, or `'localhost:2112'`, or
+`'localhost:2113'`. Because the client's node preference is "leader", the
+client will select the leader node from the cluster info and reconnect to the
+leader. If the "leader" node becomes a "follower" and another node becomes
+"leader", then the client will reconnect to the new leader. esdb://admin:
+changeit@localhost:2111,localhost:2112,localhost:2113?NodePreference=leader The
+following URI will cause the client to make "secure" connections, firstly to
+get cluster info from either `'localhost:2111'`, or `'localhost:2112'`, or
+`'localhost:2113'`. Because the client's node preference is "follower", the
+client will select a follower node from the cluster info and reconnect to this
+follower. Please note, if the "follower" node becomes the "leader", the client
+will not reconnect to a follower -- such behavior may be implemented in a
+future version of the client and server. esdb://admin:changeit@localhost:
+2111,localhost:2112,localhost:2113?NodePreference=follower The following URI
+will cause the client to make "secure" connections, firstly to get cluster info
+from addresses in DNS 'A' records for `'cluster1.example.com'`, and then to
+connect to a "leader" node. The client will use a default timeout of 5 seconds
+when making calls to EventStore API "write" methods. esdb+discover://admin:
 changeit@cluster1.example.com?DefaultDeadline=5 The following URI will cause
-the client to get cluster info from either localhost:2111, or localhost:2112,
-or localhost:2113. And then to connect to a "follower" node. esdb://admin:
-changeit@localhost:2111,localhost:2112,localhost:2113?NodePreference=follower
-The following URI will cause the client to get cluster info from addresses in
-DNS 'A' records for cluster1.example.com. And to configure "keep alive" timeout
-and interval in the gRPC channel. esdb+discover://admin:
-changeit@cluster1.example.com?KeepAliveInterval=10000&KeepAliveTimeout=10000
-Please note, the client is insensitive to the case of fields and values. If
-fields are repeated in the query string, the query string will be parsed
-without error. However, the connection options used by the client will use the
-value of the first field. All the other field-values in the query string with
-the same field name will be ignored. Fields without values will also be
-ignored. If the client's node preference is "leader" and the node becomes a
-"follower", the client will attempt to reconnect to the current leader when a
-method is called that expects to call a leader. Methods which mutate the state
-of the database expect to call a leader. For such methods, the HTTP header
-"requires-leader" is set to "true", and this header is observed by the server,
-and so a node which is not a leader that receives such a request will return an
-error. This error is detected by the client, which will then close the current
-gRPC connection and create a new connection to the leader. The request will
-then be retried with the leader. If the client's node preference is "follower"
-and there are no follower nodes in the cluster, then the client will raise an
-exception. Similarly, if the client's node preference is "readonlyreplica" and
-there are no read-only replica nodes in the cluster, then the client will also
-raise an exception. The gRPC channel option "grpc.max_receive_message_length"
-is automatically configured to the value `17 * 1024 * 1024`. This value cannot
-be changed. ## Event objects This package defines a `NewEvent` class and a
-`RecordedEvent` class. The `NewEvent` class should be used when writing events
-to the database. The `RecordedEvent` class is used when reading events from the
-database. ### New events The `NewEvent` class should be used when writing
-events to an EventStoreDB database. You will need to construct new event
-objects before calling `append_to_stream()`. The `NewEvent` class is a frozen
-Python dataclass. It has two required constructor arguments (`type` and `data`)
-and three optional constructor arguments (`metadata`, `content_type` and `id`).
-The required `type` argument is a Python `str`, used to describe the type of
-domain event that is being recorded. The required `data` argument is a Python
-`bytes` object, used to state the serialized data of the domain event that is
-being recorded. The optional `metadata` argument is a Python `bytes` object,
-used to indicate any metadata of the event that will be recorded. The default
-value is an empty `bytes` object. The optional `content_type` argument is a
-Python `str`, used to indicate the kind of data that is being recorded. The
-default value is `'application/json'`, which indicates that the `data` was
-serialised using JSON. An alternative value for this argument is the more
-general indication `'application/octet-stream'`. The optional `id` argument is
-a Python `UUID` object, used to specify the unique ID of the event that will be
+the client to make "secure" connections, firstly to get cluster info from
+addresses in DNS 'A' records for `'cluster1.example.com'`, and then to connect
+to a "leader" node. It will configure gRPC connections with a "keep alive
+interval" and a "keep alive timeout". esdb+discover://admin:
+changeit@cluster1.example.com?KeepAliveInterval=10000&KeepAliveTimeout=10000 ##
+Event objects This package defines a `NewEvent` class and a `RecordedEvent`
+class. The `NewEvent` class should be used when writing events to the database.
+The `RecordedEvent` class is used when reading events from the database. ###
+New events The `NewEvent` class should be used when writing events to an
+EventStoreDB database. You will need to construct new event objects before
+calling `append_to_stream()`. The `NewEvent` class is a frozen Python
+dataclass. It has two required constructor arguments (`type` and `data`) and
+three optional constructor arguments (`metadata`, `content_type` and `id`). The
+required `type` argument is a Python `str`, used to describe the type of domain
+event that is being recorded. The required `data` argument is a Python `bytes`
+object, used to state the serialized data of the domain event that is being
+recorded. The optional `metadata` argument is a Python `bytes` object, used to
+indicate any metadata of the event that will be recorded. The default value is
+an empty `bytes` object. The optional `content_type` argument is a Python
+`str`, used to indicate the kind of data that is being recorded. The default
+value is `'application/json'`, which indicates that the `data` was serialised
+using JSON. An alternative value for this argument is the more general
+indication `'application/octet-stream'`. The optional `id` argument is a Python
+`UUID` object, used to specify the unique ID of the event that will be
 recorded. If no value is provided, a new version-4 UUID will be generated.
 ```python new_event1 = NewEvent( type='OrderCreated', data=b'{"name": "Greg"}',
 ) assert new_event1.type == 'OrderCreated' assert new_event1.data == b'{"name":
 "Greg"}' assert new_event1.metadata == b'' assert new_event1.content_type ==
 'application/json' assert isinstance(new_event1.id, uuid.UUID) event_id =
 uuid.uuid4() new_event2 = NewEvent( type='ImageCreated',
 data=b'01010101010101', metadata=b'{"a": 1}', content_type='application/octet-
@@ -354,46 +364,48 @@
 new_event2.id == event_id ``` ### Recorded events The `RecordedEvent` class is
 used when reading events from an EventStoreDB database. The client will return
 event objects of this type from all methods that return recorded events, such
 as `get_stream()`, `subscribe_to_all()`, and `read_subscription_to_all()`. You
 do not need to construct recorded event objects. Like `NewEvent`, the
 `RecordedEvent` class is a frozen Python dataclass. It has all the attributes
 that `NewEvent` has (`type`, `data`, `metadata`, `content_type`, `id`) that
-follow from an event that was recorded, and some additional attributes that
+follow from an event having been recorded, and some additional attributes that
 follow from the recording of an event (`stream_name`, `stream_position`,
-`commit_position`, `recorded_at`). It also has a `link` attribute, which is set
-only when "link events" are "resolved". And it has a `retry_count` which is set
-only when reading persistence subscriptions. The `type` attribute is a Python
-`str`, used to indicate the type of an event that was recorded. The `data`
-attribute is a Python `bytes` object, used to indicate the data of an event
-that was recorded. The `metadata` attribute is a Python `bytes` object, used to
-indicate the metadata of an event that was recorded. The `content_type`
-attribute is a Python `str`, used to indicate the type of data that was
-recorded for an event. It is usually `'application/json'`, indicating that the
-data can be parsed as JSON. Alternatively, it is `'application/octet-stream'`.
-The `id` attribute is a Python `UUID` object, used to indicate the unique ID of
-an event that was recorded. The `stream_name` attribute is a Python `str`, used
-to indicate the name of a stream in which an event was recorded. The
-`stream_position` attribute is a Python `int`, used to indicate the position in
-a stream at which an event was recorded. In EventStoreDB, a "stream position"
-is an integer representing the position of a recorded event in a stream. Each
-recorded event is recorded at a position in a stream. Each stream position is
-occupied by only one recorded event. New events are recorded at the next
-unoccupied position. All sequences of stream positions are zero-based and
-gapless. The `commit_position` attribute is a Python `int`, used to indicate
-the position in the database at which an event was recorded. In EventStoreDB, a
-"commit position" is an integer representing the position of a recorded event
-in the database. Each recorded event is recorded at a position in the database.
-Each commit position is occupied by only one recorded event. Commit positions
-are zero-based and increase monotonically as new events are recorded. But,
-unlike stream positions, the sequence of successive commit positions is not
-gapless. Indeed, there are usually large differences between the commit
-positions of successively recorded events. Please note, in EventStoreDB 21.10,
-the `commit_position` of all `RecordedEvent` objects obtained from `read_stream
-()` is `None`, whereas those obtained from `read_all()` have the actual commit
+`commit_position`, `recorded_at`). It also has a `link` attribute, which is
+`None` unless the recorded event is a "link event" that has been "resolved" to
+the linked event. And it has a `retry_count` which has an integer value when
+receiving recorded events from persistence subscriptions, otherwise the value
+of `retry_count` is `None`. The `type` attribute is a Python `str`, used to
+indicate the type of an event that was recorded. The `data` attribute is a
+Python `bytes` object, used to indicate the data of an event that was recorded.
+The `metadata` attribute is a Python `bytes` object, used to indicate the
+metadata of an event that was recorded. The `content_type` attribute is a
+Python `str`, used to indicate the type of data that was recorded for an event.
+It is usually `'application/json'`, indicating that the data can be parsed as
+JSON. Alternatively, it is `'application/octet-stream'`. The `id` attribute is
+a Python `UUID` object, used to indicate the unique ID of an event that was
+recorded. The `stream_name` attribute is a Python `str`, used to indicate the
+name of a stream in which an event was recorded. The `stream_position`
+attribute is a Python `int`, used to indicate the position in a stream at which
+an event was recorded. In EventStoreDB, a "stream position" is an integer
+representing the position of a recorded event in a stream. Each recorded event
+is recorded at a position in a stream. Each stream position is occupied by only
+one recorded event. New events are recorded at the next unoccupied position.
+All sequences of stream positions are zero-based and gapless. The
+`commit_position` attribute is a Python `int`, used to indicate the position in
+the database at which an event was recorded. In EventStoreDB, a "commit
+position" is an integer representing the position of a recorded event in the
+database. Each recorded event is recorded at a position in the database. Each
+commit position is occupied by only one recorded event. Commit positions are
+zero-based and increase monotonically as new events are recorded. But, unlike
+stream positions, the sequence of successive commit positions is not gapless.
+Indeed, there are usually large differences between the commit positions of
+successively recorded events. Please note, in EventStoreDB 21.10, the
+`commit_position` of all `RecordedEvent` objects obtained from `read_stream()`
+is `None`, whereas those obtained from `read_all()` have the actual commit
 position of the recorded event. This was changed in version 22.10, so that
 event objects obtained from both `get_stream()` and `read_all()` have the
 actual commit position. The `commit_position` attribute of the `RecordedEvent`
 class is annotated with the type `Optional[int]` for this reason only. The
 `recorded_at` attribute is a Python `datetime`, used to indicate when an event
 was recorded by the database. The `link` attribute is an optional
 `RecordedEvent` that carries information about a "link event" that has been
@@ -1494,25 +1506,25 @@
 ( group_name=group_name1, ) ``` The example below deleted the persistent
 subscription `group_name2` on `stream_name2` which was created by calling
 `create_subscription_to_stream()`. ```python client.delete_subscription
 ( group_name=group_name2, stream_name=stream_name2, ) ``` ## Projections Please
 refer to the [EventStoreDB documentation](https://developers.eventstore.com/
 server/v23.10/projections.html) for more information on projections in
 EventStoreDB. ### Create projection The `create_projection()` method can be
-used to create a projection. This method has two required arguments, `name` and
-`query`. This required `name` argument is a Python `str` that specifies the
-name of the projection. This required `query` argument is a Python `str` that
-defines what the projection will do. This method also has four optional
-arguments, `emit_enabled`, `track_emitted_streams`, `timeout`, and
-`credentials`. The optional `emit_enabled` argument is a Python `bool` which
-specifies whether a projection will be able to emit events. If a `True` value
-is specified, the projection will be able to emit events, otherwise the
+used to create a "continuous" projection. This method has two required
+arguments, `name` and `query`. This required `name` argument is a Python `str`
+that specifies the name of the projection. This required `query` argument is a
+Python `str` that defines what the projection will do. This method also has
+four optional arguments, `emit_enabled`, `track_emitted_streams`, `timeout`,
+and `credentials`. The optional `emit_enabled` argument is a Python `bool`
+which specifies whether a projection will be able to emit events. If a `True`
+value is specified, the projection will be able to emit events, otherwise the
 projection will not be able to emit events. The default value of `emit_enabled`
-is `False`. Please note, if your projection query includes a call to `emit()`
-then `emit_enabled` must be `True`, otherwise the projection will not run. The
+is `False`. Please note, `emit_enabled` must be `True` if your projection query
+includes a call to `emit()`, otherwise the projection will not run. The
 optional `track_emitted_streams` argument is a Python `bool` which specifies
 whether a projection will have its emitted streams tracked. If a `True` value
 is specified, the projection will have its emitted streams tracked, otherwise
 the projection will not have its emitted streams tracked. The default value of
 `track_emitted_streams` is `False`. The purpose of tracking emitted streams is
 that they can optionally be deleted when a projection is deleted (see the
 `delete_projection()` method for more details). Please note, if you set
@@ -1526,50 +1538,64 @@
 have a "count" that is incremented once for each event. ```python
 projection_name = str(uuid.uuid4()) projection_query = """fromStream('%s')
 .when({ $init: function(){ return { count: 0 }; }, OrderCreated: function(s,e)
 { s.count += 1; }, OrderUpdated: function(s,e){ s.count += 1; }, OrderDeleted:
 function(s,e){ s.count += 1; } }) .outputState() """ % stream_name2
 client.create_projection( name=projection_name, query=projection_query, ) ```
 Please note, the `outputState()` call is optional, and causes the state of the
-projection to be persisted in a "result" stream. The default name of the result
-stream is `$projections-{projection_name}-result`, and this name can be used to
-read from and subscribe to the results stream with the `get_stream()`,
-`read_stream()`, `subscribe_stream()`, `create_subscription_to_stream()` and
-`read_subscription_to_stream()` methods. ### Get projection state The
-`get_projection_state()` method can be used to get a projection's state. This
-method has a required `name` argument, which is a Python `str` that specifies
-the name of a projection. This method also has three optional arguments,
-`partition`, `timeout`, and `credentials`. The optional `partition` argument is
-a Python `str` which specifies a partition... The optional `timeout` argument
-is a Python `float` which sets a maximum duration, in seconds, for the
+projection to be persisted in a "result" stream. If `outputState()` is called,
+an event representing the state of the projection will immediately be written
+to a "result" stream. The default name of the "result" stream for a projection
+with name `projection_name` is `$projections-{projection_name}-result`. This
+stream name can be used to read from and subscribe to the "result" stream, with
+the `get_stream()`, or `read_stream()`, or `subscribe_to_stream()`, or
+`create_subscription_to_stream()` and `read_subscription_to_stream()` methods.
+If your projections doesn't call `outputState()`, then you won't be able to
+read or subscribe to a "result" stream, but you will still be able to get the
+projection "result" using the `get_projection_result()` method. The "type"
+string of events recorded in "result" streams is `'Result'`. You may want to
+include this in a `filter_exclude` argument when filtering events by type
+whilst reading or subscribing to "all" events recorded in the database (with
+`read_all()`, `subscribe_to_all()`, etc). Additionally, and in any case, from
+time to time the state of the projection will be recorded in a "state" stream,
+and also the projection will write to a "checkpoint" stream. The "state"
+stream, the "checkpoint" stream, and all "emitted" streams that have been
+"tracked" (as a consequence of the `track_emitted_streams` argument having been
+`True`) can optionally be deleted when the projection is deleted. See
+`delete_projection()` for details. Unlike the "result" and "emitted" streams,
+the "state" and the "checkpoint" streams cannot be read or subscribed to by
+users, or viewed in the "stream browser" view of EventStoreDB's Web interface.
+### Get projection state The `get_projection_state()` method can be used to get
+a projection's "state". This method has a required `name` argument, which is a
+Python `str` that specifies the name of a projection. This method also has two
+optional arguments, `timeout` and `credentials`. The optional `timeout`
+argument is a Python `float` which sets a maximum duration, in seconds, for the
 completion of the gRPC operation. The optional `credentials` argument can be
 used to override call credentials derived from the connection string URI. In
 the example below, after sleeping for 1 second to allow the projection to
 process all the recorded events, the projection "state" is obtained. We can see
 that the projection has processed three events. ```python sleep(1) # allow time
 for projection to process recorded events projection_state =
 client.get_projection_state(name=projection_name) assert projection_state.value
 == {'count': 3} ``` ### Get projection result The `get_projection_result()`
-method can be used to get a projection's result. This method has a required
+method can be used to get a projection's "result". A projection's "result"
+holds the same data as the projections "state". This method has a required
 `name` argument, which is a Python `str` that specifies the name of a
-projection. This method also has three optional arguments, `partition`,
-`timeout`, and `credentials`. The optional `partition` argument is a Python
-`str` which specifies a partition. The optional `timeout` argument is a Python
-`float` which sets a maximum duration, in seconds, for the completion of the
-gRPC operation. The optional `credentials` argument can be used to override
-call credentials derived from the connection string URI. In the example below,
-the projection "result" is obtained. We can see that the projection has
-processed three events. ```python projection_result =
-client.get_projection_result(name=projection_name) assert
-projection_result.value == {'count': 3} ``` ### Get projection statistics The
-`get_projection_statistucs()` method can be used to get projection statistics.
-This method has a required `name` argument, which is a Python `str` that
-specifies the name of a projection. This method also has three optional
-arguments, `partition`, `timeout`, and `credentials`. The optional `partition`
-argument is a Python `str` which specifies a partition. The optional `timeout`
+projection. This method also has two optional arguments, `timeout` and
+`credentials`. The optional `timeout` argument is a Python `float` which sets a
+maximum duration, in seconds, for the completion of the gRPC operation. The
+optional `credentials` argument can be used to override call credentials
+derived from the connection string URI. In the example below, the projection
+"result" is obtained. We can see that the projection has processed three
+events. ```python projection_result = client.get_projection_result
+(name=projection_name) assert projection_result.value == {'count': 3} ``` ###
+Get projection statistics The `get_projection_statistics()` method can be used
+to get projection statistics. This method has a required `name` argument, which
+is a Python `str` that specifies the name of a projection. This method also has
+two optional arguments, `timeout` and `credentials`. The optional `timeout`
 argument is a Python `float` which sets a maximum duration, in seconds, for the
 completion of the gRPC operation. The optional `credentials` argument can be
 used to override call credentials derived from the connection string URI. This
 method returns a `ProjectionStatistics` object that represents the named
 projection. ```python statistics = client.get_projection_statistics
 (name=projection_name) ``` A `ProjectionStatistics` object is returned. The
 attributes of this object have values that represent the progress of the
@@ -1579,82 +1605,84 @@
 name of the projection to be updated. The required `query` argument is a Python
 `str` which defines what the projection will do. This method also has three
 optional arguments, `emit_enabled`, `timeout`, and `credentials`. The optional
 `emit_enabled` argument is a Python `bool` which specifies whether a projection
 will be able to emit events. If a `True` value is specified, the projection
 will be able to emit events. If a `False` value is specified, the projection
 will not be able to emit events. The default value of `emit_enabled` is
-`False`. Please note, if your projection query includes a call to `emit()` then
-`emit_enabled` must be `True`, otherwise the projection will not run. Please
+`False`. Please note, `emit_enabled` must be `True` if your projection query
+includes a call to `emit()`, otherwise the projection will not run. Please
 note, it is not possible to update `track_emitted_streams` via the gRPC API.
 The optional `timeout` argument is a Python `float` which sets a maximum
 duration, in seconds, for the completion of the gRPC operation. The optional
 `credentials` argument can be used to override call credentials derived from
 the connection string URI. ```python client.update_projection
 (name=projection_name, query=projection_query) ``` ### Enable projection The
-`enable_projection()` method can be used to enable a projection that was
-previously disabled. This method has a required `name` argument, which is a
-Python `str` that specifies the name of the projection to be enabled. This
-method also has two optional arguments, `timeout` and `credentials`. The
-optional `timeout` argument is a Python `float` which sets a maximum duration,
-in seconds, for the completion of the gRPC operation. The optional
-`credentials` argument can be used to override call credentials derived from
-the connection string URI. ```python client.enable_projection
-(name=projection_name) ``` ### Disable projection The `disable_projection()`
-method can be used to disable a projection. This method has a required `name`
+`enable_projection()` method can be used to enable (start running) a projection
+that was previously disabled (stopped). This method has a required `name`
 argument, which is a Python `str` that specifies the name of the projection to
-be disabled. This method also has three optional arguments, `write_checkpoint`,
-`timeout`, and `credentials`. The optional `write_checkpoint` argument is a
-Python `bool` which specifies whether a checkpoint will be written when the
-projection is disabled. If `write_checkpoint` is `True` a checkpoint will be
-written, otherwise a checkpoint will not be written. The default value of
-`write_checkpoint` is `False`. The optional `timeout` argument is a Python
+be enabled. This method also has two optional arguments, `timeout` and
+`credentials`. The optional `timeout` argument is a Python `float` which sets a
+maximum duration, in seconds, for the completion of the gRPC operation. The
+optional `credentials` argument can be used to override call credentials
+derived from the connection string URI. ```python client.enable_projection
+(name=projection_name) ``` ### Disable projection The `disable_projection()`
+method can be used to disable (stop running) a projection. This method has a
+required `name` argument, which is a Python `str` that specifies the name of
+the projection to be disabled. This method also has two optional arguments,
+`timeout`, and `credentials`. The optional `timeout` argument is a Python
 `float` which sets a maximum duration, in seconds, for the completion of the
 gRPC operation. The optional `credentials` argument can be used to override
 call credentials derived from the connection string URI. ```python
 client.disable_projection(name=projection_name) ``` ### Reset projection The
 `reset_projection()` method can be used to reset a projection. This method has
 a required `name` argument, which is a Python `str` that specifies the name of
-the projection to be reset. This method also has three optional arguments,
-`write_checkpoint`, `timeout`, and `credentials`. The optional
-`write_checkpoint` argument is a Python `bool` which specifies whether a
-checkpoint will be written when the projection is reset. If `write_checkpoint`
-is `True` a checkpoint will be written, otherwise a checkpoint will not be
-written. The default value of `write_checkpoint` is `False`. The optional
-`timeout` argument is a Python `float` which sets a maximum duration, in
-seconds, for the completion of the gRPC operation. The optional `credentials`
-argument can be used to override call credentials derived from the connection
-string URI. ```python client.reset_projection(name=projection_name) ``` ###
-Delete projection The `delete_projection()` method can be used to delete a
-projection. This method has a required `name` argument, which is a Python `str`
-that specifies the name of the projection to be deleted. This method also has
-five optional arguments, `delete_emitted_streams`, `delete_state_stream`,
-`delete_checkpoint_stream`, `timeout`, and `credentials`. The optional
-`delete_emitted_streams` argument is a Python `bool` which specifies that the
-emitted streams will be deleted. For emitted streams to be deleted, they must
-have been tracked (see the `track_emitted_streams` argument of the
-`create_projection()` method.) The optional `delete_state_stream` argument is a
-Python `bool` which... The optional `delete_checkpoint_stream` argument is a
-Python `bool` which... The optional `timeout` argument is a Python `float`
-which sets a maximum duration, in seconds, for the completion of the gRPC
-operation. The optional `credentials` argument can be used to override call
-credentials derived from the connection string URI. ```python
-client.delete_projection(name=projection_name) ``` ### Restart projections
+the projection to be reset. This method also has two optional arguments,
+`timeout`, and `credentials`. The optional `timeout` argument is a Python
+`float` which sets a maximum duration, in seconds, for the completion of the
+gRPC operation. The optional `credentials` argument can be used to override
+call credentials derived from the connection string URI. ```python
+client.reset_projection(name=projection_name) ``` Please note, a projection
+must be disabled before it can be reset. ### Delete projection The
+`delete_projection()` method can be used to delete a projection. This method
+has a required `name` argument, which is a Python `str` that specifies the name
+of the projection to be deleted. This method also has five optional arguments,
+`delete_emitted_streams`, `delete_state_stream`, `delete_checkpoint_stream`,
+`timeout`, and `credentials`. The optional `delete_emitted_streams` argument is
+a Python `bool` which specifies that all "emitted" streams that have been
+tracked will be deleted. For emitted streams to be deleted, they must have been
+tracked (see the `track_emitted_streams` argument of the `create_projection()`
+method.) The optional `delete_state_stream` argument is a Python `bool` which
+specifies that the projection's "state" stream should also be deleted. The
+"state" stream is like the "result" stream, but events are written to the
+"state" stream occasionally, along with events written to the "checkpoint"
+stream, rather than being written immediately in the way a call `outputState()`
+immediately writes events to the "result" stream. The optional
+`delete_checkpoint_stream` argument is a Python `bool` which specifies that the
+projection's "checkpoint" stream should also be deleted. The optional `timeout`
+argument is a Python `float` which sets a maximum duration, in seconds, for the
+completion of the gRPC operation. The optional `credentials` argument can be
+used to override call credentials derived from the connection string URI.
+```python client.delete_projection(name=projection_name) ``` Please note, a
+projection must be disabled before it can be deleted. ### Restart projections
 subsystem The `restart_projections_subsystem()` method can be used to restart
 the projections subsystem. This method also has two optional arguments,
 `timeout` and `credentials`. The optional `timeout` argument is a Python
 `float` which sets a maximum duration, in seconds, for the completion of the
 gRPC operation. The optional `credentials` argument can be used to override
 call credentials derived from the connection string URI. ```python
 client.restart_projections_subsystem() ``` ## Call credentials Default call
 credentials are derived by the client from the user info part of the connection
 string URI. Many of the client methods described above have an optional
 `credentials` argument, which can be used to set call credentials for an
 individual method call that override those derived from the connection string
-URI. ### Construct call credentials The client method
+URI. Call credentials are sent to "secure" servers in a "basic auth"
+authorization header. This authorization header is used by the server to
+authenticate the client. The authorization header is not sent to "insecure"
+servers. ### Construct call credentials The client method
 `construct_call_credentials()` can be used to construct a call credentials
 object from a username and password. ```python call_credentials =
 client.construct_call_credentials( username='admin', password='changeit' ) ```
 The call credentials object can be used as the value of the `credentials`
 argument in other client methods. ## Connection ### Reconnect The `reconnect()`
 method can be used to manually reconnect the client to a suitable EventStoreDB
 node. This method uses the same routine for reading the cluster node states and
@@ -1790,61 +1818,63 @@
 `subscribe_to_stream()`, if the server is unavailable, or if the channel has
 somehow been closed, or if the request fails for some other reason, then the
 client will reconnect and retry. However, if an exception is raised when
 iterating over a successfully returned "catch-up subscription" object, the
 catch-up subscription will need to be restarted. Similarly, when reading
 persistent subscriptions, if there are connection issues whilst iterating over
 a successfully received response, the consumer will need to be restarted. ##
-Contributors ### Install Poetry The first thing is to check you have Poetry
-installed. $ poetry --version If you don't, then please [install Poetry](https:
-//python-poetry.org/docs/#installing-with-the-official-installer). $ curl -sSL
-https://install.python-poetry.org | python3 - It will help to make sure
-Poetry's bin directory is in your `PATH` environment variable. But in any case,
-make sure you know the path to the `poetry` executable. The Poetry installer
-tells you where it has been installed, and how to configure your shell. Please
-refer to the [Poetry docs](https://python-poetry.org/docs/) for guidance on
-using Poetry. ### Setup for PyCharm users You can easily obtain the project
-files using PyCharm (menu "Git > Clone..."). PyCharm will then usually prompt
-you to open the project. Open the project in a new window. PyCharm will then
-usually prompt you to create a new virtual environment. Create a new Poetry
-virtual environment for the project. If PyCharm doesn't already know where your
-`poetry` executable is, then set the path to your `poetry` executable in the
-"New Poetry Environment" form input field labelled "Poetry executable". In the
-"New Poetry Environment" form, you will also have the opportunity to select
-which Python executable will be used by the virtual environment. PyCharm will
-then create a new Poetry virtual environment for your project, using a
-particular version of Python, and also install into this virtual environment
-the project's package dependencies according to the project's `poetry.lock`
-file. You can add different Poetry environments for different Python versions,
-and switch between them using the "Python Interpreter" settings of PyCharm. If
-you want to use a version of Python that isn't installed, either use your
-favourite package manager, or install Python by downloading an installer for
-recent versions of Python directly from the [Python website](https://
-www.python.org/downloads/). Once project dependencies have been installed, you
-should be able to run tests from within PyCharm (right-click on the `tests`
-folder and select the 'Run' option). Because of a conflict between pytest and
-PyCharm's debugger and the coverage tool, you may need to add ``--no-cov`` as
-an option to the test runner template. Alternatively, just use the Python
-Standard Library's ``unittest`` module. You should also be able to open a
-terminal window in PyCharm, and run the project's Makefile commands from the
-command line (see below). ### Setup from command line Obtain the project files,
-using Git or suitable alternative. In a terminal application, change your
-current working directory to the root folder of the project files. There should
-be a Makefile in this folder. Use the Makefile to create a new Poetry virtual
-environment for the project and install the project's package dependencies into
-it, using the following command. $ make install-packages It's also possible to
-also install the project in 'editable mode'. $ make install Please note, if you
-create the virtual environment in this way, and then try to open the project in
-PyCharm and configure the project to use this virtual environment as an
-"Existing Poetry Environment", PyCharm sometimes has some issues (don't know
-why) which might be problematic. If you encounter such issues, you can resolve
-these issues by deleting the virtual environment and creating the Poetry
-virtual environment using PyCharm (see above). ### Project Makefile commands
-You can start EventStoreDB using the following command. $ make start-
-eventstoredb You can run tests using the following command (needs EventStoreDB
-to be running). $ make test You can stop EventStoreDB using the following
-command. $ make stop-eventstoredb You can check the formatting of the code
-using the following command. $ make lint You can reformat the code using the
-following command. $ make fmt Tests belong in `./tests`. Code-under-test
-belongs in `./esdbclient`. Edit package dependencies in `pyproject.toml`.
-Update installed packages (and the `poetry.lock` file) using the following
-command. $ make update-packages
+Communities - [Issues](https://github.com/pyeventsourcing/esdbclient/issues) -
+[Discuss](https://discuss.eventstore.com/) - [Discord (Event Store)](https://
+discord.gg/Phn9pmCw3t) ## Contributors ### Install Poetry The first thing is to
+check you have Poetry installed. $ poetry --version If you don't, then please
+[install Poetry](https://python-poetry.org/docs/#installing-with-the-official-
+installer). $ curl -sSL https://install.python-poetry.org | python3 - It will
+help to make sure Poetry's bin directory is in your `PATH` environment
+variable. But in any case, make sure you know the path to the `poetry`
+executable. The Poetry installer tells you where it has been installed, and how
+to configure your shell. Please refer to the [Poetry docs](https://python-
+poetry.org/docs/) for guidance on using Poetry. ### Setup for PyCharm users You
+can easily obtain the project files using PyCharm (menu "Git > Clone...").
+PyCharm will then usually prompt you to open the project. Open the project in a
+new window. PyCharm will then usually prompt you to create a new virtual
+environment. Create a new Poetry virtual environment for the project. If
+PyCharm doesn't already know where your `poetry` executable is, then set the
+path to your `poetry` executable in the "New Poetry Environment" form input
+field labelled "Poetry executable". In the "New Poetry Environment" form, you
+will also have the opportunity to select which Python executable will be used
+by the virtual environment. PyCharm will then create a new Poetry virtual
+environment for your project, using a particular version of Python, and also
+install into this virtual environment the project's package dependencies
+according to the project's `poetry.lock` file. You can add different Poetry
+environments for different Python versions, and switch between them using the
+"Python Interpreter" settings of PyCharm. If you want to use a version of
+Python that isn't installed, either use your favourite package manager, or
+install Python by downloading an installer for recent versions of Python
+directly from the [Python website](https://www.python.org/downloads/). Once
+project dependencies have been installed, you should be able to run tests from
+within PyCharm (right-click on the `tests` folder and select the 'Run' option).
+Because of a conflict between pytest and PyCharm's debugger and the coverage
+tool, you may need to add ``--no-cov`` as an option to the test runner
+template. Alternatively, just use the Python Standard Library's ``unittest``
+module. You should also be able to open a terminal window in PyCharm, and run
+the project's Makefile commands from the command line (see below). ### Setup
+from command line Obtain the project files, using Git or suitable alternative.
+In a terminal application, change your current working directory to the root
+folder of the project files. There should be a Makefile in this folder. Use the
+Makefile to create a new Poetry virtual environment for the project and install
+the project's package dependencies into it, using the following command. $ make
+install-packages It's also possible to also install the project in 'editable
+mode'. $ make install Please note, if you create the virtual environment in
+this way, and then try to open the project in PyCharm and configure the project
+to use this virtual environment as an "Existing Poetry Environment", PyCharm
+sometimes has some issues (don't know why) which might be problematic. If you
+encounter such issues, you can resolve these issues by deleting the virtual
+environment and creating the Poetry virtual environment using PyCharm (see
+above). ### Project Makefile commands You can start EventStoreDB using the
+following command. $ make start-eventstoredb You can run tests using the
+following command (needs EventStoreDB to be running). $ make test You can stop
+EventStoreDB using the following command. $ make stop-eventstoredb You can
+check the formatting of the code using the following command. $ make lint You
+can reformat the code using the following command. $ make fmt Tests belong in
+`./tests`. Code-under-test belongs in `./esdbclient`. Edit package dependencies
+in `pyproject.toml`. Update installed packages (and the `poetry.lock` file)
+using the following command. $ make update-packages
```

### Comparing `esdbclient-1.1b2/esdbclient/__init__.py` & `esdbclient-1.1b3/esdbclient/__init__.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.1b2/esdbclient/asyncio_client.py` & `esdbclient-1.1b3/esdbclient/asyncio_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1477,39 +1477,38 @@
         credentials: Optional[grpc.CallCredentials] = None,
     ) -> ProjectionStatistics:
         """
         Gets projection statistics.
         """
         timeout = timeout if timeout is not None else self._default_deadline
 
-        return await self._connection.projections.get_projection_statistics(
+        return await self._connection.projections.get_statistics(
             name=name,
             timeout=timeout,
             metadata=self._call_metadata,
             credentials=credentials or self._call_credentials,
         )
 
     @retrygrpc
     @autoreconnect
     async def disable_projection(
         self,
         name: str,
         *,
-        write_checkpoint: bool = False,
         timeout: Optional[float] = None,
         credentials: Optional[grpc.CallCredentials] = None,
     ) -> None:
         """
         Disables a projection.
         """
         timeout = timeout if timeout is not None else self._default_deadline
 
         await self._connection.projections.disable(
             name=name,
-            write_checkpoint=write_checkpoint,
+            write_checkpoint=True,
             timeout=timeout,
             metadata=self._call_metadata,
             credentials=credentials or self._call_credentials,
         )
 
     @retrygrpc
     @autoreconnect
@@ -1534,72 +1533,69 @@
 
     @retrygrpc
     @autoreconnect
     async def reset_projection(
         self,
         name: str,
         *,
-        write_checkpoint: bool = False,
         timeout: Optional[float] = None,
         credentials: Optional[grpc.CallCredentials] = None,
     ) -> None:
         """
         Resets a projection.
         """
         timeout = timeout if timeout is not None else self._default_deadline
 
         await self._connection.projections.reset(
             name=name,
-            write_checkpoint=write_checkpoint,
+            write_checkpoint=True,
             timeout=timeout,
             metadata=self._call_metadata,
             credentials=credentials or self._call_credentials,
         )
 
     @retrygrpc
     @autoreconnect
     async def get_projection_state(
         self,
         name: str,
         *,
-        partition: str = "",
         timeout: Optional[float] = None,
         credentials: Optional[grpc.CallCredentials] = None,
     ) -> ProjectionState:
         """
         Gets projection state.
         """
         timeout = timeout if timeout is not None else self._default_deadline
 
         return await self._connection.projections.get_state(
             name=name,
-            partition=partition,
+            partition="",
             timeout=timeout,
             metadata=self._call_metadata,
             credentials=credentials or self._call_credentials,
         )
 
     @retrygrpc
     @autoreconnect
     async def get_projection_result(
         self,
         name: str,
         *,
-        partition: str = "",
         timeout: Optional[float] = None,
         credentials: Optional[grpc.CallCredentials] = None,
     ) -> ProjectionResult:
         """
         Gets projection result.
         """
         timeout = timeout if timeout is not None else self._default_deadline
 
         return await self._connection.projections.get_result(
             name=name,
-            partition=partition,
+            partition="",
             timeout=timeout,
             metadata=self._call_metadata,
             credentials=credentials or self._call_credentials,
         )
 
     @retrygrpc
     @autoreconnect
```

### Comparing `esdbclient-1.1b2/esdbclient/client.py` & `esdbclient-1.1b3/esdbclient/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1677,39 +1677,38 @@
         credentials: Optional[grpc.CallCredentials] = None,
     ) -> ProjectionStatistics:
         """
         Gets projection statistics.
         """
         timeout = timeout if timeout is not None else self._default_deadline
 
-        return self._esdb.projections.get_projection_statistics(
+        return self._esdb.projections.get_statistics(
             name=name,
             timeout=timeout,
             metadata=self._call_metadata,
             credentials=credentials or self._call_credentials,
         )
 
     @retrygrpc
     @autoreconnect
     def disable_projection(
         self,
         name: str,
         *,
-        write_checkpoint: bool = False,
         timeout: Optional[float] = None,
         credentials: Optional[grpc.CallCredentials] = None,
     ) -> None:
         """
         Disables a projection.
         """
         timeout = timeout if timeout is not None else self._default_deadline
 
         self._esdb.projections.disable(
             name=name,
-            write_checkpoint=write_checkpoint,
+            write_checkpoint=True,
             timeout=timeout,
             metadata=self._call_metadata,
             credentials=credentials or self._call_credentials,
         )
 
     @retrygrpc
     @autoreconnect
@@ -1734,72 +1733,69 @@
 
     @retrygrpc
     @autoreconnect
     def reset_projection(
         self,
         name: str,
         *,
-        write_checkpoint: bool = False,
         timeout: Optional[float] = None,
         credentials: Optional[grpc.CallCredentials] = None,
     ) -> None:
         """
         Resets a projection.
         """
         timeout = timeout if timeout is not None else self._default_deadline
 
         self._esdb.projections.reset(
             name=name,
-            write_checkpoint=write_checkpoint,
+            write_checkpoint=True,
             timeout=timeout,
             metadata=self._call_metadata,
             credentials=credentials or self._call_credentials,
         )
 
     @retrygrpc
     @autoreconnect
     def get_projection_state(
         self,
         name: str,
         *,
-        partition: str = "",
         timeout: Optional[float] = None,
         credentials: Optional[grpc.CallCredentials] = None,
     ) -> ProjectionState:
         """
         Gets projection state.
         """
         timeout = timeout if timeout is not None else self._default_deadline
 
         return self._esdb.projections.get_state(
             name=name,
-            partition=partition,
+            partition="",
             timeout=timeout,
             metadata=self._call_metadata,
             credentials=credentials or self._call_credentials,
         )
 
     @retrygrpc
     @autoreconnect
     def get_projection_result(
         self,
         name: str,
         *,
-        partition: str = "",
         timeout: Optional[float] = None,
         credentials: Optional[grpc.CallCredentials] = None,
     ) -> ProjectionResult:
         """
         Gets projection result.
         """
         timeout = timeout if timeout is not None else self._default_deadline
 
         return self._esdb.projections.get_result(
             name=name,
-            partition=partition,
+            partition="",
             timeout=timeout,
             metadata=self._call_metadata,
             credentials=credentials or self._call_credentials,
         )
 
     @retrygrpc
     @autoreconnect
```

### Comparing `esdbclient-1.1b2/esdbclient/common.py` & `esdbclient-1.1b3/esdbclient/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
 import datetime
+import os
 from abc import ABC, abstractmethod
 from base64 import b64encode
 from threading import Lock
 from typing import (
     TYPE_CHECKING,
     Any,
     Generic,
@@ -39,14 +40,19 @@
     OperationFailed,
     ServiceUnavailable,
     SSLError,
     UnknownError,
 )
 from esdbclient.protos.Grpc import persistent_pb2, streams_pb2
 
+# Avoid ares resolver.
+if "GRPC_DNS_RESOLVER" not in os.environ:
+    os.environ["GRPC_DNS_RESOLVER"] = "native"
+
+
 if TYPE_CHECKING:  # pragma: no cover
     from grpc import Metadata
 
 else:
     Metadata = Tuple[Tuple[str, str], ...]
 
 __all__ = ["handle_rpc_error", "BasicAuthCallCredentials", "ESDBService", "Metadata"]
@@ -162,34 +168,34 @@
             ):
                 # Projections.Create does this....
                 return AlreadyExists(e)
             elif (
                 "Envelope callback expected Updated, received NotFound instead"
                 in details
             ):
-                # Projections.Update and Projections.Delete does this....
-                return NotFound(e)
+                # Projections.Update and Projections.Delete does this in < v24.6
+                return NotFound(e)  # pragma: no cover
             elif (
                 "Envelope callback expected Statistics, received NotFound instead"
                 in details
             ):
-                # Projections.Statistics does this....
-                return NotFound(e)
+                # Projections.Statistics does this in < v24.6
+                return NotFound(e)  # pragma: no cover
             elif (
                 "Envelope callback expected ProjectionState, received NotFound instead"
                 in details
             ):
-                # Projections.State does this....
-                return NotFound(e)
+                # Projections.State does this in < v24.6
+                return NotFound(e)  # pragma: no cover
             elif (
                 "Envelope callback expected ProjectionResult, received NotFound instead"
                 in details
             ):
-                # Projections.Result does this....
-                return NotFound(e)
+                # Projections.Result does this in < v24.6
+                return NotFound(e)  # pragma: no cover
             elif (
                 "Envelope callback expected Updated, received OperationFailed instead"
                 in details
             ):
                 # Projections.Delete does this....
                 return OperationFailed(e)
             else:  # pragma: no cover
```

### Comparing `esdbclient-1.1b2/esdbclient/connection.py` & `esdbclient-1.1b3/esdbclient/connection.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.1b2/esdbclient/connection_spec.py` & `esdbclient-1.1b3/esdbclient/connection_spec.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.1b2/esdbclient/events.py` & `esdbclient-1.1b3/esdbclient/events.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.1b2/esdbclient/exceptions.py` & `esdbclient-1.1b3/esdbclient/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,15 @@
 
 class InvalidTransactionError(EventStoreDBClientException):
     """
     Raised when append operation fails with an "invalid transaction" error.
     """
 
 
-class OperationFailed(EventStoreDBClientException):
+class OperationFailed(GrpcError):
     """
     Raised when an operation fails (e.g. deleting a projection that isn't disabled).
     """
 
 
 class MaximumAppendSizeExceededError(EventStoreDBClientException):
     """
```

### Comparing `esdbclient-1.1b2/esdbclient/gossip.py` & `esdbclient-1.1b3/esdbclient/gossip.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.1b2/esdbclient/persistent.py` & `esdbclient-1.1b3/esdbclient/persistent.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.1b2/esdbclient/projections.py` & `esdbclient-1.1b3/esdbclient/projections.py`

 * *Files 0% similar despite different names*

```diff
@@ -311,15 +311,15 @@
                 metadata=self._metadata(metadata, requires_leader=True),
                 credentials=credentials,
             )
         except grpc.RpcError as e:
             raise handle_rpc_error(e) from None
         assert isinstance(delete_resp, projections_pb2.DeleteResp)
 
-    async def get_projection_statistics(
+    async def get_statistics(
         self,
         name: str,
         timeout: Optional[float] = None,
         metadata: Optional[Metadata] = None,
         credentials: Optional[grpc.CallCredentials] = None,
     ) -> ProjectionStatistics:
         statistics_req = self._construct_statistics_req(name=name)
@@ -560,15 +560,15 @@
                 metadata=self._metadata(metadata, requires_leader=True),
                 credentials=credentials,
             )
         except grpc.RpcError as e:
             raise handle_rpc_error(e) from None
         assert isinstance(delete_resp, projections_pb2.DeleteResp)
 
-    def get_projection_statistics(
+    def get_statistics(
         self,
         name: str,
         timeout: Optional[float] = None,
         metadata: Optional[Metadata] = None,
         credentials: Optional[grpc.CallCredentials] = None,
     ) -> ProjectionStatistics:
         statistics_req = self._construct_statistics_req(name=name)
```

### Comparing `esdbclient-1.1b2/esdbclient/protos/Grpc/cluster_pb2.py` & `esdbclient-1.1b3/esdbclient/protos/Grpc/cluster_pb2.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.1b2/esdbclient/protos/Grpc/cluster_pb2.pyi` & `esdbclient-1.1b3/esdbclient/protos/Grpc/cluster_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdbclient-1.1b2/esdbclient/protos/Grpc/cluster_pb2_grpc.py` & `esdbclient-1.1b3/esdbclient/protos/Grpc/cluster_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.1b2/esdbclient/protos/Grpc/code_pb2.py` & `esdbclient-1.1b3/esdbclient/protos/Grpc/code_pb2.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.1b2/esdbclient/protos/Grpc/code_pb2.pyi` & `esdbclient-1.1b3/esdbclient/protos/Grpc/code_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdbclient-1.1b2/esdbclient/protos/Grpc/gossip_pb2.py` & `esdbclient-1.1b3/esdbclient/protos/Grpc/gossip_pb2.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.1b2/esdbclient/protos/Grpc/gossip_pb2.pyi` & `esdbclient-1.1b3/esdbclient/protos/Grpc/gossip_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdbclient-1.1b2/esdbclient/protos/Grpc/gossip_pb2_grpc.py` & `esdbclient-1.1b3/esdbclient/protos/Grpc/gossip_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.1b2/esdbclient/protos/Grpc/persistent_pb2.py` & `esdbclient-1.1b3/esdbclient/protos/Grpc/persistent_pb2.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.1b2/esdbclient/protos/Grpc/persistent_pb2.pyi` & `esdbclient-1.1b3/esdbclient/protos/Grpc/persistent_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdbclient-1.1b2/esdbclient/protos/Grpc/persistent_pb2_grpc.py` & `esdbclient-1.1b3/esdbclient/protos/Grpc/persistent_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.1b2/esdbclient/protos/Grpc/projections_pb2.py` & `esdbclient-1.1b3/esdbclient/protos/Grpc/projections_pb2.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.1b2/esdbclient/protos/Grpc/projections_pb2.pyi` & `esdbclient-1.1b3/esdbclient/protos/Grpc/projections_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdbclient-1.1b2/esdbclient/protos/Grpc/projections_pb2_grpc.py` & `esdbclient-1.1b3/esdbclient/protos/Grpc/projections_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.1b2/esdbclient/protos/Grpc/shared_pb2.py` & `esdbclient-1.1b3/esdbclient/protos/Grpc/shared_pb2.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.1b2/esdbclient/protos/Grpc/shared_pb2.pyi` & `esdbclient-1.1b3/esdbclient/protos/Grpc/shared_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdbclient-1.1b2/esdbclient/protos/Grpc/status_pb2.py` & `esdbclient-1.1b3/esdbclient/protos/Grpc/status_pb2.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.1b2/esdbclient/protos/Grpc/status_pb2.pyi` & `esdbclient-1.1b3/esdbclient/protos/Grpc/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdbclient-1.1b2/esdbclient/protos/Grpc/streams_pb2.py` & `esdbclient-1.1b3/esdbclient/protos/Grpc/streams_pb2.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.1b2/esdbclient/protos/Grpc/streams_pb2.pyi` & `esdbclient-1.1b3/esdbclient/protos/Grpc/streams_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdbclient-1.1b2/esdbclient/protos/Grpc/streams_pb2_grpc.py` & `esdbclient-1.1b3/esdbclient/protos/Grpc/streams_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.1b2/esdbclient/streams.py` & `esdbclient-1.1b3/esdbclient/streams.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.1b2/pyproject.toml` & `esdbclient-1.1b3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "esdbclient"
-version = "1.1b2"
+version = "1.1b3"
 
 description = "Python gRPC Client for EventStoreDB"
 authors = [
     "John Bywater <john.bywater@appropriatesoftware.net>",
 ]
 license = "BSD 3-Clause"
 classifiers = [
```

### Comparing `esdbclient-1.1b2/PKG-INFO` & `esdbclient-1.1b3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esdbclient
-Version: 1.1b2
+Version: 1.1b3
 Summary: Python gRPC Client for EventStoreDB
 Home-page: https://github.com/pyeventsourcing/esdbclient
 License: BSD 3-Clause
 Author: John Bywater
 Author-email: john.bywater@appropriatesoftware.net
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -30,28 +30,108 @@
 clients for the [EventStoreDB](https://www.eventstore.com/) database.
 
 The multithreaded `EventStoreDBClient` is described in detail below. Please scroll
 down for <a href="#asyncio-client">information</a> about `AsyncioEventStoreDBClient`.
 
 These clients have been developed and are being maintained in a collaboration
 with the EventStoreDB team, and are officially support by Event Store Ltd.
-Although not all the features of EventStoreDB are supported, many of the most
-useful features are presented in an easy-to-use interface.
+Although not all aspects of the EventStoreDB gRPC API are implemented, many
+of the most useful features are presented in an easy-to-use interface.
 
-These clients have been tested to work with EventStoreDB LTS versions 21.10,
-22.10, 23.10, and version 24.2, without and without SSL/TLS, with single-server
+These clients have been tested to work with EventStoreDB LTS versions 22.10 and 23.10,
+and release candidates 24.2 and 24.6, without and without SSL/TLS, with both single-server
 and cluster modes, and with Python versions 3.7, 3.8, 3.9, 3.10, 3.11 and 3.12.
 
 The test suite has 100% line and branch coverage. The code has typing annotations
 checked strictly with mypy. The code is formatted with black and isort, and checked
 with flake8. Poetry is used for package management during development, and for
 building and publishing distributions to [PyPI](https://pypi.org/project/esdbclient/).
 
+For an example of usage, see the [eventsourcing-eventstoredb](
+https://github.com/pyeventsourcing/eventsourcing-eventstoredb) package.
+
+
+<!-- TOC -->
+* [Synopsis](#synopsis)
+* [Install package](#install-package)
+  * [From PyPI](#from-pypi)
+  * [With Poetry](#with-poetry)
+* [EventStoreDB server](#eventstoredb-server)
+  * [Run container](#run-container)
+  * [Stop container](#stop-container)
+* [EventStoreDB client](#eventstoredb-client)
+  * [Import class](#import-class)
+  * [Construct client](#construct-client)
+* [Connection strings](#connection-strings)
+  * [Two schemes](#two-schemes)
+  * [User info string](#user-info-string)
+  * [Query string](#query-string)
+  * [Examples](#examples)
+* [Event objects](#event-objects)
+  * [New events](#new-events)
+  * [Recorded events](#recorded-events)
+* [Streams](#streams)
+  * [Append events](#append-events)
+  * [Idempotent append operations](#idempotent-append-operations)
+  * [Read stream events](#read-stream-events)
+  * [Get current version](#get-current-version)
+  * [How to implement snapshotting with EventStoreDB](#how-to-implement-snapshotting-with-eventstoredb)
+  * [Read all events](#read-all-events)
+  * [Get commit position](#get-commit-position)
+  * [Get stream metadata](#get-stream-metadata)
+  * [Set stream metadata](#set-stream-metadata)
+  * [Delete stream](#delete-stream)
+  * [Tombstone stream](#tombstone-stream)
+* [Catch-up subscriptions](#catch-up-subscriptions)
+  * [Subscribe to all events](#subscribe-to-all-events)
+  * [Subscribe to stream events](#subscribe-to-stream-events)
+  * [How to implement exactly-once event processing](#how-to-implement-exactly-once-event-processing)
+* [Persistent subscriptions](#persistent-subscriptions)
+  * [Create subscription to all](#create-subscription-to-all)
+  * [Read subscription to all](#read-subscription-to-all)
+  * [How to write a persistent subscription consumer](#how-to-write-a-persistent-subscription-consumer)
+  * [Update subscription to all](#update-subscription-to-all)
+  * [Create subscription to stream](#create-subscription-to-stream)
+  * [Read subscription to stream](#read-subscription-to-stream)
+  * [Update subscription to stream](#update-subscription-to-stream)
+  * [Replay parked events](#replay-parked-events)
+  * [Get subscription info](#get-subscription-info)
+  * [List subscriptions](#list-subscriptions)
+  * [List subscriptions to stream](#list-subscriptions-to-stream)
+  * [Delete subscription](#delete-subscription)
+* [Projections](#projections)
+  * [Create projection](#create-projection)
+  * [Get projection state](#get-projection-state)
+  * [Get projection result](#get-projection-result)
+  * [Get projection statistics](#get-projection-statistics)
+  * [Update projection](#update-projection)
+  * [Enable projection](#enable-projection)
+  * [Disable projection](#disable-projection)
+  * [Reset projection](#reset-projection)
+  * [Delete projection](#delete-projection)
+  * [Restart projections subsystem](#restart-projections-subsystem)
+* [Call credentials](#call-credentials)
+  * [Construct call credentials](#construct-call-credentials)
+* [Connection](#connection)
+  * [Reconnect](#reconnect)
+  * [Close](#close)
+* [Asyncio client](#asyncio-client)
+  * [Synopsis](#synopsis-1)
+* [Notes](#notes)
+  * [Regular expression filters](#regular-expression-filters)
+  * [Reconnect and retry method decorators](#reconnect-and-retry-method-decorators)
+* [Communities](#communities)
+* [Contributors](#contributors)
+  * [Install Poetry](#install-poetry)
+  * [Setup for PyCharm users](#setup-for-pycharm-users)
+  * [Setup from command line](#setup-from-command-line)
+  * [Project Makefile commands](#project-makefile-commands)
+<!-- TOC -->
 
-## Synopsis
+## Synopsis<a id="synopsis"></a>
 
 The `EventStoreDBClient` class can be imported from the `esdbclient` package.
 
 Probably the three most useful methods of `EventStoreDBClient` are:
 
 * `append_to_stream()` This method can be used to record new events in a particular
 "stream". This is useful, for example, when executing a command in an application
@@ -209,95 +289,14 @@
 
 
 # Close the client's gRPC connection.
 
 client.close()
 ```
 
-See below for more details.
-
-For an example of usage, see the [eventsourcing-eventstoredb](
-https://github.com/pyeventsourcing/eventsourcing-eventstoredb) package.
-
-## Table of contents
-
-<!-- TOC -->
-* [Install package](#install-package)
-  * [From PyPI](#from-pypi)
-  * [With Poetry](#with-poetry)
-* [EventStoreDB server](#eventstoredb-server)
-  * [Run container](#run-container)
-  * [Stop container](#stop-container)
-* [EventStoreDB client](#eventstoredb-client)
-  * [Import class](#import-class)
-  * [Construct client](#construct-client)
-* [Connection strings](#connection-strings)
-  * [Two schemes](#two-schemes)
-  * [User info string](#user-info-string)
-  * [Query string](#query-string)
-  * [Examples](#examples)
-* [Event objects](#event-objects)
-  * [New events](#new-events)
-  * [Recorded events](#recorded-events)
-* [Streams](#streams)
-  * [Append events](#append-events)
-  * [Idempotent append operations](#idempotent-append-operations)
-  * [Read stream events](#read-stream-events)
-  * [Get current version](#get-current-version)
-  * [How to implement snapshotting with EventStoreDB](#how-to-implement-snapshotting-with-eventstoredb)
-  * [Read all events](#read-all-events)
-  * [Get commit position](#get-commit-position)
-  * [Get stream metadata](#get-stream-metadata)
-  * [Set stream metadata](#set-stream-metadata)
-  * [Delete stream](#delete-stream)
-  * [Tombstone stream](#tombstone-stream)
-* [Catch-up subscriptions](#catch-up-subscriptions)
-  * [Subscribe to all events](#subscribe-to-all-events)
-  * [Subscribe to stream events](#subscribe-to-stream-events)
-  * [How to implement exactly-once event processing](#how-to-implement-exactly-once-event-processing)
-* [Persistent subscriptions](#persistent-subscriptions)
-  * [Create subscription to all](#create-subscription-to-all)
-  * [Read subscription to all](#read-subscription-to-all)
-  * [How to write a persistent subscription consumer](#how-to-write-a-persistent-subscription-consumer)
-  * [Update subscription to all](#update-subscription-to-all)
-  * [Create subscription to stream](#create-subscription-to-stream)
-  * [Read subscription to stream](#read-subscription-to-stream)
-  * [Update subscription to stream](#update-subscription-to-stream)
-  * [Replay parked events](#replay-parked-events)
-  * [Get subscription info](#get-subscription-info)
-  * [List subscriptions](#list-subscriptions)
-  * [List subscriptions to stream](#list-subscriptions-to-stream)
-  * [Delete subscription](#delete-subscription)
-* [Projections](#projections)
-  * [Create projection](#create-projection)
-  * [Get projection state](#get-projection-state)
-  * [Get projection result](#get-projection-result)
-  * [Get projection statistics](#get-projection-statistics)
-  * [Update projection](#update-projection)
-  * [Enable projection](#enable-projection)
-  * [Disable projection](#disable-projection)
-  * [Reset projection](#reset-projection)
-  * [Delete projection](#delete-projection)
-  * [Restart projections subsystem](#restart-projections-subsystem)
-* [Call credentials](#call-credentials)
-  * [Construct call credentials](#construct-call-credentials)
-* [Connection](#connection)
-  * [Reconnect](#reconnect)
-  * [Close](#close)
-* [Asyncio client](#asyncio-client)
-  * [Synopsis](#synopsis-1)
-* [Notes](#notes)
-  * [Regular expression filters](#regular-expression-filters)
-  * [Reconnect and retry method decorators](#reconnect-and-retry-method-decorators)
-* [Contributors](#contributors)
-  * [Install Poetry](#install-poetry)
-  * [Setup for PyCharm users](#setup-for-pycharm-users)
-  * [Setup from command line](#setup-from-command-line)
-  * [Project Makefile commands](#project-makefile-commands)
-<!-- TOC -->
 
 ## Install package<a id="install-package"></a>
 
 It is recommended to install Python packages into a Python virtual environment.
 
 ### From PyPI<a id="from-pypi"></a>
 
@@ -316,15 +315,15 @@
 
 The EventStoreDB server can be run locally using the official Docker container image.
 
 ### Run container<a id="run-container"></a>
 
 For development, you can run a "secure" EventStoreDB server using the following command.
 
-    $ docker run -d --name eventstoredb-secure -it -p 2113:2113 --env "HOME=/tmp" eventstore/eventstore:21.10.9-buster-slim --dev
+    $ docker run -d --name eventstoredb-secure -it -p 2113:2113 --env "HOME=/tmp" docker.eventstore.com/eventstore-ce/eventstoredb-ce:23.10.0-jammy --dev
 
 As we will see, your client will need an EventStoreDB connection string URI as the value
 of its `uri` constructor argument. The connection string for this "secure" EventStoreDB
 server would be:
 
     esdb://admin:changeit@localhost:2113
 
@@ -346,15 +345,15 @@
 import ssl
 
 server_certificate = ssl.get_server_certificate(addr=('localhost', 2113))
 ```
 
 Alternatively, you can start an "insecure" server using the following command.
 
-    $ docker run -d --name eventstoredb-insecure -it -p 2113:2113 eventstore/eventstore:21.10.9-buster-slim --insecure
+    $ docker run -d --name eventstoredb-insecure -it -p 2113:2113 docker.eventstore.com/eventstore-ce/eventstoredb-ce:23.10.0-jammy --insecure
 
 The connection string URI for this "insecure" server would be:
 
     esdb://localhost:2113?Tls=false
 
 As we will see, when connecting to an "insecure" server, there is no need to include
 a "username" and a "password" in the connection string. If you do, these values will
@@ -393,45 +392,29 @@
 
 The `EventStoreDBClient` class has one required constructor argument, `uri`, and one
 optional constructor argument, `root_certificates`.
 
 The `uri` argument is expected to be an EventStoreDB connection string URI that
 conforms with the standard EventStoreDB "esdb" or "esdb+discover" URI schemes.
 
-For example, the following connection string specifies that the client should
-attempt to create a "secure" connection to port 2113 on "localhost", and use the
-client credentials "username" and "password" when making calls to the server.
-
-    esdb://username:password@localhost:2113?Tls=true
-
 The client must be configured to create a "secure" connection to a "secure" server,
 or alternatively an "insecure" connection to an "insecure" server. By default, the
 client will attempt to create a "secure" connection. And so, when connecting to an
 "insecure" server, the connection string must specify that the client should attempt
 to make an "insecure" connection.
 
-The following connection string specifies that the client should
-attempt to create an "insecure" connection to port 2113 on "localhost".
-When connecting to an "insecure" server, the client will ignore any
-username and password information included in the connection string,
-so that usernames and passwords are not sent over an "insecure" connection.
-
-    esdb://localhost:2113?Tls=false
-
-Please note, the "insecure" connection string uses a query string with the field-value
-`Tls=false`. The value of this field is by default `true`.
-
-When connecting to a "secure" server, the `root_certificates` argument can be
-a Python `str` containing PEM encoded SSL/TLS root certificates. This value is
-passed directly to `grpc.ssl_channel_credentials()`. It is used for authenticating the
-server to the client. It is commonly the certificate of the certificate authority that
-was responsible for generating the SSL/TLS certificate used by the EventStoreDB server.
-Often it is unnecessary to provide these certificates explicitly, if they are installed
-locally in a such a way that the Python grpc library can pick them up from a default
-location. Alternatively, for development, you can use the server's certificate itself.
+When connecting to a "secure" server, it may be necessary to set the optional `root_certificates`
+argument. The optional `root_certificates` argument is a Python `str` containing
+PEM encoded SSL/TLS root certificates. This value is passed directly to
+`grpc.ssl_channel_credentials()` and is used by the client to authenticate the server.
+It is commonly a public certificate of the certificate authority that was responsible
+for generating the certificate used by the EventStoreDB server. Often it is unnecessary
+to provide these certificates explicitly, as they are commonly installed locally in
+a default location such that the Python grpc library can pick them up. Alternatively,
+for development, you can use the server's certificate itself.
 
 In the example below, the constructor argument values are taken from the operating
 system environment.
 
 ```python
 import os
 
@@ -466,46 +449,52 @@
 
     grpc-target = ( hostname | ip-address ) , ":" , port-number ;
 
 If there is one gRPC target, the client will simply attempt to connect to this
 server, and it will use this connection when recording and retrieving events.
 
 If there are two or more gRPC targets, the client will attempt to connect to the
-Gossip API of each in turn, to obtain information about the whole cluster. A member
-of the cluster is then selected by the client according to the "node preference" option
-of the connection string. The client may then need to close its connection and reconnect
-to the selected node.
+Gossip API of each in turn, attempting to obtain information about the cluster from
+it, until information about the cluster is obtained. A member of the cluster is then
+selected by the client according to the "node preference" specified by the connection
+string URI. The client will then close its connection and connect to the selected node
+without the 'round robin' load balancing strategy. If the "node preference" is "leader",
+and after connecting to a leader, if the leader becomes a follower, the client will
+reconnect to the new leader.
+
 
 The "esdb+discover" URI scheme can be defined in the following way.
 
     esdb-discover-uri = "esdb+discover://" , [ user-info, "@" ] , cluster-domainname, [ ":" , port-number ] , [ "?" , query-string ] ;
 
 In the "esdb+discover" URI scheme, after the optional user info string, there should be
 a domain name which identifies a cluster of EventStoreDB servers. Individual nodes in
 the cluster should be declared with DNS 'A' records.
 
-The client will create a gRPC connection using the cluster's domain name, using the
-gRPC library's 'round robin' load balancing strategy to call the Gossip API of addresses
-to which this domain name resolves. Information about the EventStoreDB cluster is
-obtained from the Gossip API. A member of the cluster is then selected by the client
-according to the "node preference" option. The client may then need to close its
-connection and reconnect to the selected node.
+The client will use the cluster domain name with the gRPC library's 'round robin' load
+balancing strategy to call the Gossip APIs of addresses discovered from DNS 'A' records.
+Information about the EventStoreDB cluster is obtained from the Gossip API. A member of
+the cluster is then selected by the client according to the "node preference" option.
+The client will then close its connection and connect to the selected node without the
+'round robin' load balancing strategy. If the "node preference" is "leader",
+and after connecting to a leader, if the leader becomes a follower, the client will
+reconnect to the new leader.
 
 ### User info string<a id="user-info-string"></a>
 
 In both the "esdb" and "esdb+discover" schemes, the URI may include a user info string.
 If it exists in the URI, the user info string must be separated from the rest of the URI
 with the "@" character. The user info string must include a username and a password,
 separated with the ":" character.
 
     user-info = username , ":" , password ;
 
-The user info is sent by the client as "call credentials" in each call to a "secure"
-server, in a "basic auth" authorization header. This authorization header is used by
-the server to authenticate the client. The authorization header is not sent to
+The user info is sent by the client in a "basic auth" authorization header in each gRPC
+call to a "secure" server. This authorization header is used by the server to authenticate
+the client. The Python gRPC library does not allow call credentials to be transferred to
 "insecure" servers.
 
 ### Query string<a id="query-string"></a>
 
 In both the "esdb" and "esdb+discover" schemes, the optional query string must be one
 or many field-value arguments, separated from each other with the "&" character.
 
@@ -533,84 +522,94 @@
 | TlsVerifyCert       | "true", "false" (default: "true")                                     | This value is currently ignored.                                                                                                                                  |
 | ConnectionName      | string (default: auto-generated version-4 UUID)                       | Sent in call metadata for every call, to identify the client to the cluster.                                                                                      |
 | NodePreference      | "leader", "follower", "readonlyreplica", "random" (default: "leader") | The node state preferred by the client. The client will select a node from the cluster info received from the Gossip API according to this preference.            |
 | DefaultDeadline     | integer (default: `None`)                                             | The default value (in seconds) of the `timeout` argument of client "write" methods such as `append_to_stream()`.                                                  |
 | GossipTimeout       | integer (default: 5)                                                  | The default value (in seconds) of the `timeout` argument of gossip read methods, such as `read_gossip()`.                                                         |
 | MaxDiscoverAttempts | integer (default: 10)                                                 | The number of attempts to read gossip when connecting or reconnecting to a cluster member.                                                                        |
 | DiscoveryInterval   | integer (default: 100)                                                | How long to wait (in milliseconds) between gossip retries.                                                                                                        |
-| KeepAliveInterval   | integer (default: `None`)                                             | The value of the "grpc.keepalive_ms" gRPC channel option.                                                                                                         |
-| KeepAliveTimeout    | integer (default: `None`)                                             | The value of the "grpc.keepalive_timeout_ms" gRPC channel option.                                                                                                 |
+| KeepAliveInterval   | integer (default: `None`)                                             | The value (in milliseconds) of the "grpc.keepalive_ms" gRPC channel option.                                                                                       |
+| KeepAliveTimeout    | integer (default: `None`)                                             | The value (in milliseconds) of the "grpc.keepalive_timeout_ms" gRPC channel option.                                                                               |
+
+Please note, the client is insensitive to the case of fields and values. If fields are
+repeated in the query string, the query string will be parsed without error. However,
+the connection options used by the client will use the value of the first field. All
+the other field-values in the query string with the same field name will be ignored.
+Fields without values will also be ignored.
+
+If the client's node preference is "follower" and there are no follower
+nodes in the cluster, then the client will raise an exception. Similarly, if the
+client's node preference is "readonlyreplica" and there are no read-only replica
+nodes in the cluster, then the client will also raise an exception.
+
+The gRPC channel option "grpc.max_receive_message_length" is automatically
+configured to the value `17 * 1024 * 1024`. This value cannot be configured.
 
 
 ### Examples<a id="examples"></a>
 
 Here are some examples of EventStoreDB connection string URIs.
 
-The following URI will cause the client to connect to, and get
-cluster info, from "secure" server socket `localhost:2113`. And
-then to connect to a "leader" node. And also to use "admin" and
-"changeit" as the username and password when making calls to
-EventStoreDB API methods.
+The following URI will cause the client to make an "insecure" connection to
+gRPC target `'localhost:2113'`. Because the client's node preference is "follower",
+methods that can be called on a follower should complete successfully, methods that
+require a leader will raise a `NodeIsNotLeader` exception.
+
+    esdb://127.0.0.1:2113?Tls=false&NodePreference=follower
+
+The following URI will cause the client to make an "insecure" connection to
+gRPC target `'localhost:2113'`. Because the client's node preference is "leader",
+if this node is not a leader, then a `NodeIsNotLeader` exception will be raised by
+all methods.
+
+    esdb://127.0.0.1:2113?Tls=false&NodePreference=leader
+
+The following URI will cause the client to make a "secure" connection to
+gRPC target `'localhost:2113'` with username `'admin'` and password `'changeit'`
+as the default call credentials when making calls to the EventStoreDB gRPC API.
+Because the client's node preference is "leader", by default, if this node is not
+a leader, then a `NodeIsNotLeader` exception will be raised by all methods.
 
     esdb://admin:changeit@localhost:2113
 
+The following URI will cause the client to make "secure" connections, firstly to
+get cluster info from either `'localhost:2111'`, or `'localhost:2112'`, or `'localhost:2113'`.
+Because the client's node preference is "leader", the client will select the leader
+node from the cluster info and reconnect to the leader. If the "leader" node becomes
+a "follower" and another node becomes "leader", then the client will reconnect to the
+new leader.
+
+    esdb://admin:changeit@localhost:2111,localhost:2112,localhost:2113?NodePreference=leader
+
+
+The following URI will cause the client to make "secure" connections, firstly to
+get cluster info from either `'localhost:2111'`, or `'localhost:2112'`, or `'localhost:2113'`.
+Because the client's node preference is "follower", the client will select a follower
+node from the cluster info and reconnect to this follower. Please note, if the "follower"
+node becomes the "leader", the client will not reconnect to a follower -- such behavior
+may be implemented in a future version of the client and server.
 
-The following URI will cause the client to get cluster info from
-"insecure" server socket 127.0.0.1:2113.  And then to connect to
-a "leader" node.
-
-    esdb://127.0.0.1:2113?Tls=false
+    esdb://admin:changeit@localhost:2111,localhost:2112,localhost:2113?NodePreference=follower
 
 
-The following URI will cause the client to get cluster info from
-addresses in DNS 'A' records for cluster1.example.com. And then
-to connect to a "leader" node. And use a default deadline of 5
-seconds when making calls to EventStore API "write" methods.
+The following URI will cause the client to make "secure" connections, firstly to get
+cluster info from addresses in DNS 'A' records for `'cluster1.example.com'`, and then
+to connect to a "leader" node. The client will use a default timeout
+of 5 seconds when making calls to EventStore API "write" methods.
 
     esdb+discover://admin:changeit@cluster1.example.com?DefaultDeadline=5
 
 
-The following URI will cause the client to get cluster info from either
-localhost:2111, or localhost:2112, or localhost:2113. And then to connect
-to a "follower" node.
-
-    esdb://admin:changeit@localhost:2111,localhost:2112,localhost:2113?NodePreference=follower
-
-
-The following URI will cause the client to get cluster info from addresses in
-DNS 'A' records for cluster1.example.com. And to configure "keep alive" timeout
-and interval in the gRPC channel.
+The following URI will cause the client to make "secure" connections, firstly to get
+cluster info from addresses in DNS 'A' records for `'cluster1.example.com'`, and then
+to connect to a "leader" node. It will configure gRPC connections with a "keep alive
+interval" and a "keep alive timeout".
 
     esdb+discover://admin:changeit@cluster1.example.com?KeepAliveInterval=10000&KeepAliveTimeout=10000
 
 
-Please note, the client is insensitive to the case of fields and values. If fields are
-repeated in the query string, the query string will be parsed without error. However,
-the connection options used by the client will use the value of the first field. All
-the other field-values in the query string with the same field name will be ignored.
-Fields without values will also be ignored.
-
-If the client's node preference is "leader" and the node becomes a
-"follower", the client will attempt to reconnect to the current leader when a method
-is called that expects to call a leader. Methods which mutate the state of the database
-expect to call a leader. For such methods, the HTTP header "requires-leader" is set to
-"true", and this header is observed by the server, and so a node which is not a leader
-that receives such a request will return an error. This error is detected by the client,
-which will then close the current gRPC connection and create a new connection to the
-leader. The request will then be retried with the leader.
-
-If the client's node preference is "follower" and there are no follower
-nodes in the cluster, then the client will raise an exception. Similarly, if the
-client's node preference is "readonlyreplica" and there are no read-only replica
-nodes in the cluster, then the client will also raise an exception.
-
-The gRPC channel option "grpc.max_receive_message_length" is automatically
-configured to the value `17 * 1024 * 1024`. This value cannot be changed.
-
-
 ## Event objects<a id="event-objects"></a>
 
 This package defines a `NewEvent` class and a `RecordedEvent` class. The
 `NewEvent` class should be used when writing events to the database. The
 `RecordedEvent` class is used when reading events from the database.
 
 ### New events<a id="new-events"></a>
@@ -672,19 +671,20 @@
 The `RecordedEvent` class is used when reading events from an EventStoreDB
 database. The client will return event objects of this type from all methods
 that return recorded events, such as `get_stream()`, `subscribe_to_all()`,
 and `read_subscription_to_all()`. You do not need to construct recorded event objects.
 
 Like `NewEvent`, the `RecordedEvent` class is a frozen Python dataclass. It has
 all the attributes that `NewEvent` has (`type`, `data`, `metadata`, `content_type`, `id`)
-that follow from an event that was recorded, and some additional attributes that follow
+that follow from an event having been recorded, and some additional attributes that follow
 from the recording of an event (`stream_name`, `stream_position`, `commit_position`,
-`recorded_at`). It also has a `link` attribute, which is set only when "link events"
-are "resolved". And it has a `retry_count` which is set only when reading persistence
-subscriptions.
+`recorded_at`). It also has a `link` attribute, which is `None` unless the recorded
+event is a "link event" that has been "resolved" to the linked event. And it has a
+`retry_count` which has an integer value when receiving recorded events from persistence
+subscriptions, otherwise the value of `retry_count` is `None`.
 
 The `type` attribute is a Python `str`, used to indicate the type of an event
 that was recorded.
 
 The `data` attribute is a Python `bytes` object, used to indicate the data of an
 event that was recorded.
 
@@ -2861,15 +2861,15 @@
 ## Projections<a id="projections"></a>
 
 Please refer to the [EventStoreDB documentation](https://developers.eventstore.com/server/v23.10/projections.html)
 for more information on projections in EventStoreDB.
 
 ### Create projection<a id="create-projection"></a>
 
-The `create_projection()` method can be used to create a projection.
+The `create_projection()` method can be used to create a "continuous" projection.
 
 This method has two required arguments, `name` and `query`.
 
 This required `name` argument is a Python `str` that specifies the name of the projection.
 
 This required `query` argument is a Python `str` that defines what the projection will do.
 
@@ -2877,16 +2877,16 @@
 `track_emitted_streams`, `timeout`, and `credentials`.
 
 The optional `emit_enabled` argument is a Python `bool` which specifies whether a
 projection will be able to emit events. If a `True` value is specified, the projection
 will be able to emit events, otherwise the projection will not be able to emit events.
 The default value of `emit_enabled` is `False`.
 
-Please note, if your projection query includes a call to `emit()` then `emit_enabled`
-must be `True`, otherwise the projection will not run.
+Please note, `emit_enabled` must be `True` if your projection query includes a call to
+`emit()`, otherwise the projection will not run.
 
 The optional `track_emitted_streams` argument is a Python `bool` which specifies whether
 a projection will have its emitted streams tracked. If a `True` value is specified, the
 projection will have its emitted streams tracked, otherwise the projection will not
 have its emitted streams tracked. The default value of `track_emitted_streams` is `False`.
 
 The purpose of tracking emitted streams is that they can optionally be deleted when
@@ -2931,31 +2931,52 @@
 client.create_projection(
     name=projection_name,
     query=projection_query,
 )
 ```
 
 Please note, the `outputState()` call is optional, and causes the state of the
-projection to be persisted in a "result" stream. The default name of the result stream
-is `$projections-{projection_name}-result`, and this name can be used to read from and
-subscribe to the results stream with the `get_stream()`, `read_stream()`,
-`subscribe_stream()`, `create_subscription_to_stream()` and `read_subscription_to_stream()`
-methods.
-
+projection to be persisted in a "result" stream. If `outputState()` is called, an
+event representing the state of the projection will immediately be written to a
+"result" stream.
+
+The default name of the "result" stream for a projection with name `projection_name`
+is `$projections-{projection_name}-result`. This stream name can be used to read from
+and subscribe to the "result" stream, with the `get_stream()`, or `read_stream()`,
+or `subscribe_to_stream()`, or `create_subscription_to_stream()` and
+`read_subscription_to_stream()` methods.
+
+If your projections doesn't call `outputState()`, then you won't be able to read or
+subscribe to a "result" stream, but you will still be able to get the projection
+"result" using the `get_projection_result()` method.
+
+The "type" string of events recorded in "result" streams is `'Result'`. You may want to
+include this in a `filter_exclude` argument when filtering events by type whilst reading
+or subscribing to "all" events recorded in the database (with `read_all()`,
+`subscribe_to_all()`, etc).
+
+Additionally, and in any case, from time to time the state of the projection will be
+recorded in a "state" stream, and also the projection will write to a "checkpoint"
+stream. The "state" stream, the "checkpoint" stream, and all "emitted" streams that
+have been "tracked" (as a consequence of the `track_emitted_streams` argument having
+been `True`) can optionally be deleted when the projection is deleted. See
+`delete_projection()` for details.
+
+Unlike the "result" and "emitted" streams, the "state" and the "checkpoint" streams
+cannot be read or subscribed to by users, or viewed in the "stream browser" view of
+EventStoreDB's Web interface.
 
 ### Get projection state<a id="get-projection-state"></a>
 
-The `get_projection_state()` method can be used to get a projection's state.
+The `get_projection_state()` method can be used to get a projection's "state".
 
 This method has a required `name` argument, which is a Python `str` that
 specifies the name of a projection.
 
-This method also has three optional arguments, `partition`, `timeout`, and `credentials`.
-
-The optional `partition` argument is a Python `str` which specifies a partition...
+This method also has two optional arguments, `timeout` and `credentials`.
 
 The optional `timeout` argument is a Python `float` which sets a
 maximum duration, in seconds, for the completion of the gRPC operation.
 
 The optional `credentials` argument can be used to
 override call credentials derived from the connection string URI.
 
@@ -2969,22 +2990,22 @@
 projection_state = client.get_projection_state(name=projection_name)
 
 assert projection_state.value == {'count': 3}
 ```
 
 ### Get projection result<a id="get-projection-result"></a>
 
-The `get_projection_result()` method can be used to get a projection's result.
+The `get_projection_result()` method can be used to get a projection's "result".
+
+A projection's "result" holds the same data as the projections "state".
 
 This method has a required `name` argument, which is a Python `str` that
 specifies the name of a projection.
 
-This method also has three optional arguments, `partition`, `timeout`, and `credentials`.
-
-The optional `partition` argument is a Python `str` which specifies a partition.
+This method also has two optional arguments, `timeout` and `credentials`.
 
 The optional `timeout` argument is a Python `float` which sets a
 maximum duration, in seconds, for the completion of the gRPC operation.
 
 The optional `credentials` argument can be used to
 override call credentials derived from the connection string URI.
 
@@ -2995,22 +3016,20 @@
 projection_result = client.get_projection_result(name=projection_name)
 
 assert projection_result.value == {'count': 3}
 ```
 
 ### Get projection statistics<a id="get-projection-statistics"></a>
 
-The `get_projection_statistucs()` method can be used to get projection statistics.
+The `get_projection_statistics()` method can be used to get projection statistics.
 
 This method has a required `name` argument, which is a Python `str` that specifies the
 name of a projection.
 
-This method also has three optional arguments, `partition`, `timeout`, and `credentials`.
-
-The optional `partition` argument is a Python `str` which specifies a partition.
+This method also has two optional arguments, `timeout` and `credentials`.
 
 The optional `timeout` argument is a Python `float` which sets a
 maximum duration, in seconds, for the completion of the gRPC operation.
 
 The optional `credentials` argument can be used to
 override call credentials derived from the connection string URI.
 
@@ -3038,16 +3057,16 @@
 This method also has three optional arguments, `emit_enabled`, `timeout`, and `credentials`.
 
 The optional `emit_enabled` argument is a Python `bool` which specifies whether a
 projection will be able to emit events. If a `True` value is specified, the projection
 will be able to emit events. If a `False` value is specified, the projection will not
 be able to emit events. The default value of `emit_enabled` is `False`.
 
-Please note, if your projection query includes a call to `emit()` then `emit_enabled`
-must be `True`, otherwise the projection will not run.
+Please note, `emit_enabled` must be `True` if your projection query includes a call
+to `emit()`, otherwise the projection will not run.
 
 Please note, it is not possible to update `track_emitted_streams` via the gRPC API.
 
 The optional `timeout` argument is a Python `float` which sets a
 maximum duration, in seconds, for the completion of the gRPC operation.
 
 The optional `credentials` argument can be used to
@@ -3055,16 +3074,16 @@
 
 ```python
 client.update_projection(name=projection_name, query=projection_query)
 ```
 
 ### Enable projection<a id="enable-projection"></a>
 
-The `enable_projection()` method can be used to enable a projection that was previously
-disabled.
+The `enable_projection()` method can be used to enable (start running) a projection
+that was previously disabled (stopped).
 
 This method has a required `name` argument, which is a Python `str` that
 specifies the name of the projection to be enabled.
 
 This method also has two optional arguments, `timeout` and `credentials`.
 
 The optional `timeout` argument is a Python `float` which sets a
@@ -3075,25 +3094,20 @@
 
 ```python
 client.enable_projection(name=projection_name)
 ```
 
 ### Disable projection<a id="disable-projection"></a>
 
-The `disable_projection()` method can be used to disable a projection.
+The `disable_projection()` method can be used to disable (stop running) a projection.
 
 This method has a required `name` argument, which is a Python `str` that
 specifies the name of the projection to be disabled.
 
-This method also has three optional arguments, `write_checkpoint`, `timeout`, and `credentials`.
-
-The optional `write_checkpoint` argument is a Python `bool` which specifies whether
-a checkpoint will be written when the projection is disabled. If `write_checkpoint`
-is `True` a checkpoint will be written, otherwise a checkpoint will not be written.
-The default value of `write_checkpoint` is `False`.
+This method also has two optional arguments, `timeout`, and `credentials`.
 
 The optional `timeout` argument is a Python `float` which sets a
 maximum duration, in seconds, for the completion of the gRPC operation.
 
 The optional `credentials` argument can be used to
 override call credentials derived from the connection string URI.
 
@@ -3104,60 +3118,65 @@
 ### Reset projection<a id="reset-projection"></a>
 
 The `reset_projection()` method can be used to reset a projection.
 
 This method has a required `name` argument, which is a Python `str` that
 specifies the name of the projection to be reset.
 
-This method also has three optional arguments, `write_checkpoint`, `timeout`, and `credentials`.
-
-The optional `write_checkpoint` argument is a Python `bool` which specifies whether
-a checkpoint will be written when the projection is reset. If `write_checkpoint`
-is `True` a checkpoint will be written, otherwise a checkpoint will not be written.
-The default value of `write_checkpoint` is `False`.
+This method also has two optional arguments, `timeout`, and `credentials`.
 
 The optional `timeout` argument is a Python `float` which sets a
 maximum duration, in seconds, for the completion of the gRPC operation.
 
 The optional `credentials` argument can be used to
 override call credentials derived from the connection string URI.
 
 ```python
 client.reset_projection(name=projection_name)
 ```
 
+Please note, a projection must be disabled before it can be reset.
+
+
 ### Delete projection<a id="delete-projection"></a>
 
 The `delete_projection()` method can be used to delete a projection.
 
 This method has a required `name` argument, which is a Python `str` that
 specifies the name of the projection to be deleted.
 
 This method also has five optional arguments, `delete_emitted_streams`,
 `delete_state_stream`, `delete_checkpoint_stream`, `timeout`, and `credentials`.
 
 The optional `delete_emitted_streams` argument is a Python `bool` which specifies
-that the emitted streams will be deleted. For emitted streams to be deleted, they
-must have been tracked (see the `track_emitted_streams` argument of the `create_projection()`
-method.)
-
-The optional `delete_state_stream` argument is a Python `bool` which...
+that all "emitted" streams that have been tracked will be deleted. For emitted streams
+to be deleted, they must have been tracked (see the `track_emitted_streams` argument of
+the `create_projection()` method.)
+
+The optional `delete_state_stream` argument is a Python `bool` which specifies that
+the projection's "state" stream should also be deleted. The "state" stream is like
+the "result" stream, but events are written to the "state" stream occasionally, along
+with events written to the "checkpoint" stream, rather than being written immediately
+in the way a call `outputState()` immediately writes events to the "result" stream.
 
-The optional `delete_checkpoint_stream` argument is a Python `bool` which...
+The optional `delete_checkpoint_stream` argument is a Python `bool` which specifies
+that the projection's "checkpoint" stream should also be deleted.
 
 The optional `timeout` argument is a Python `float` which sets a
 maximum duration, in seconds, for the completion of the gRPC operation.
 
 The optional `credentials` argument can be used to
 override call credentials derived from the connection string URI.
 
 ```python
 client.delete_projection(name=projection_name)
 ```
 
+Please note, a projection must be disabled before it can be deleted.
+
 ### Restart projections subsystem<a id="restart-projections-subsystem"></a>
 
 The `restart_projections_subsystem()` method can be used to restart the projections subsystem.
 
 This method also has two optional arguments, `timeout` and `credentials`.
 
 The optional `timeout` argument is a Python `float` which sets a
@@ -3176,14 +3195,19 @@
 Default call credentials are derived by the client from the user info part of the
 connection string URI.
 
 Many of the client methods described above have an optional `credentials` argument,
 which can be used to set call credentials for an individual method call that override
 those derived from the connection string URI.
 
+Call credentials are sent to "secure" servers in a "basic auth" authorization header.
+This authorization header is used by the server to authenticate the client. The
+authorization header is not sent to "insecure" servers.
+
+
 ### Construct call credentials<a id="construct-call-credentials"></a>
 
 The client method `construct_call_credentials()` can be used to construct a call
 credentials object from a username and password.
 
 ```python
 call_credentials = client.construct_call_credentials(
@@ -3420,14 +3444,21 @@
 then the client will reconnect and retry. However, if an exception is raised when iterating over a
 successfully returned "catch-up subscription" object, the catch-up subscription will
 need to be restarted. Similarly, when reading persistent subscriptions, if there are
 connection issues whilst iterating over a successfully received response, the consumer
 will need to be restarted.
 
 
+## Communities<a id="communities"></a>
+
+- [Issues](https://github.com/pyeventsourcing/esdbclient/issues)
+- [Discuss](https://discuss.eventstore.com/)
+- [Discord (Event Store)](https://discord.gg/Phn9pmCw3t)
+
+
 ## Contributors<a id="contributors"></a>
 
 ### Install Poetry<a id="install-poetry"></a>
 
 The first thing is to check you have Poetry installed.
 
     $ poetry --version
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: esdbclient Version: 1.1b2 Summary: Python gRPC
+Metadata-Version: 2.1 Name: esdbclient Version: 1.1b3 Summary: Python gRPC
 Client for EventStoreDB Home-page: https://github.com/pyeventsourcing/
 esdbclient License: BSD 3-Clause Author: John Bywater Author-email:
 john.bywater@appropriatesoftware.net Requires-Python: >=3.7,<4.0 Classifier:
 Development Status :: 4 - Beta Classifier: License :: OSI Approved :: BSD
 License Classifier: License :: Other/Proprietary License Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
@@ -14,55 +14,102 @@
 pyeventsourcing/esdbclient Description-Content-Type: text/markdown # Python
 gRPC Client for EventStoreDB This [Python package](https://pypi.org/project/
 esdbclient/) provides multithreaded and asyncio Python clients for the
 [EventStoreDB](https://www.eventstore.com/) database. The multithreaded
 `EventStoreDBClient` is described in detail below. Please scroll down for
 _i_n_f_o_r_m_a_t_i_o_n about `AsyncioEventStoreDBClient`. These clients have been
 developed and are being maintained in a collaboration with the EventStoreDB
-team, and are officially support by Event Store Ltd. Although not all the
-features of EventStoreDB are supported, many of the most useful features are
-presented in an easy-to-use interface. These clients have been tested to work
-with EventStoreDB LTS versions 21.10, 22.10, 23.10, and version 24.2, without
-and without SSL/TLS, with single-server and cluster modes, and with Python
-versions 3.7, 3.8, 3.9, 3.10, 3.11 and 3.12. The test suite has 100% line and
-branch coverage. The code has typing annotations checked strictly with mypy.
-The code is formatted with black and isort, and checked with flake8. Poetry is
-used for package management during development, and for building and publishing
-distributions to [PyPI](https://pypi.org/project/esdbclient/). ## Synopsis The
-`EventStoreDBClient` class can be imported from the `esdbclient` package.
-Probably the three most useful methods of `EventStoreDBClient` are: *
-`append_to_stream()` This method can be used to record new events in a
-particular "stream". This is useful, for example, when executing a command in
-an application that mutates an aggregate. This method is "atomic" in that
-either all or none of the events will be recorded. * `get_stream()` This method
-can be used to retrieve all the recorded events in a "stream". This is useful,
-for example, when reconstructing an aggregate from recorded events before
-executing a command in an application that creates new events. *
-`subscribe_to_all()` This method can be used to receive all recorded events in
-the database. This is useful, for example, in event-processing components
-because it supports processing events with "exactly-once" semantics. The
-example below uses an "insecure" EventStoreDB server running locally on port
-2113. ```python import uuid from esdbclient import EventStoreDBClient,
-NewEvent, StreamState # Construct EventStoreDBClient with an EventStoreDB URI.
-The # connection string URI specifies that the client should # connect to an
-"insecure" server running on port 2113. client = EventStoreDBClient( uri="esdb:
-//localhost:2113?Tls=false" ) # Generate new events. Typically, domain events
-of different # types are generated in a domain model, and then serialized #
-into NewEvent objects. An aggregate ID may be used as the # name of a stream in
-EventStoreDB. stream_name1 = str(uuid.uuid4()) event1 = NewEvent
-( type='OrderCreated', data=b'{"order_number": "123456"}' ) event2 = NewEvent
-( type='OrderSubmitted', data=b'{}' ) event3 = NewEvent( type='OrderCancelled',
-data=b'{}' ) # Append new events to a new stream. The value returned # from the
-append_to_stream() method is the overall # "commit position" in the database of
-the last new event # recorded by this operation. The returned "commit position"
-# may be used in a user interface to poll an eventually # consistent event-
-processing component until it can # present an up-to-date materialized view.
-New events are # each allocated a "stream position", which is the next #
-available position in the stream, starting from 0. commit_position1 =
-client.append_to_stream( stream_name=stream_name1,
+team, and are officially support by Event Store Ltd. Although not all aspects
+of the EventStoreDB gRPC API are implemented, many of the most useful features
+are presented in an easy-to-use interface. These clients have been tested to
+work with EventStoreDB LTS versions 22.10 and 23.10, and release candidates
+24.2 and 24.6, without and without SSL/TLS, with both single-server and cluster
+modes, and with Python versions 3.7, 3.8, 3.9, 3.10, 3.11 and 3.12. The test
+suite has 100% line and branch coverage. The code has typing annotations
+checked strictly with mypy. The code is formatted with black and isort, and
+checked with flake8. Poetry is used for package management during development,
+and for building and publishing distributions to [PyPI](https://pypi.org/
+project/esdbclient/). For an example of usage, see the [eventsourcing-
+eventstoredb]( https://github.com/pyeventsourcing/eventsourcing-eventstoredb)
+package. * [Synopsis](#synopsis) * [Install package](#install-package) * [From
+PyPI](#from-pypi) * [With Poetry](#with-poetry) * [EventStoreDB server]
+(#eventstoredb-server) * [Run container](#run-container) * [Stop container]
+(#stop-container) * [EventStoreDB client](#eventstoredb-client) * [Import
+class](#import-class) * [Construct client](#construct-client) * [Connection
+strings](#connection-strings) * [Two schemes](#two-schemes) * [User info
+string](#user-info-string) * [Query string](#query-string) * [Examples]
+(#examples) * [Event objects](#event-objects) * [New events](#new-events) *
+[Recorded events](#recorded-events) * [Streams](#streams) * [Append events]
+(#append-events) * [Idempotent append operations](#idempotent-append-
+operations) * [Read stream events](#read-stream-events) * [Get current version]
+(#get-current-version) * [How to implement snapshotting with EventStoreDB]
+(#how-to-implement-snapshotting-with-eventstoredb) * [Read all events](#read-
+all-events) * [Get commit position](#get-commit-position) * [Get stream
+metadata](#get-stream-metadata) * [Set stream metadata](#set-stream-metadata) *
+[Delete stream](#delete-stream) * [Tombstone stream](#tombstone-stream) *
+[Catch-up subscriptions](#catch-up-subscriptions) * [Subscribe to all events]
+(#subscribe-to-all-events) * [Subscribe to stream events](#subscribe-to-stream-
+events) * [How to implement exactly-once event processing](#how-to-implement-
+exactly-once-event-processing) * [Persistent subscriptions](#persistent-
+subscriptions) * [Create subscription to all](#create-subscription-to-all) *
+[Read subscription to all](#read-subscription-to-all) * [How to write a
+persistent subscription consumer](#how-to-write-a-persistent-subscription-
+consumer) * [Update subscription to all](#update-subscription-to-all) * [Create
+subscription to stream](#create-subscription-to-stream) * [Read subscription to
+stream](#read-subscription-to-stream) * [Update subscription to stream]
+(#update-subscription-to-stream) * [Replay parked events](#replay-parked-
+events) * [Get subscription info](#get-subscription-info) * [List
+subscriptions](#list-subscriptions) * [List subscriptions to stream](#list-
+subscriptions-to-stream) * [Delete subscription](#delete-subscription) *
+[Projections](#projections) * [Create projection](#create-projection) * [Get
+projection state](#get-projection-state) * [Get projection result](#get-
+projection-result) * [Get projection statistics](#get-projection-statistics) *
+[Update projection](#update-projection) * [Enable projection](#enable-
+projection) * [Disable projection](#disable-projection) * [Reset projection]
+(#reset-projection) * [Delete projection](#delete-projection) * [Restart
+projections subsystem](#restart-projections-subsystem) * [Call credentials]
+(#call-credentials) * [Construct call credentials](#construct-call-credentials)
+* [Connection](#connection) * [Reconnect](#reconnect) * [Close](#close) *
+[Asyncio client](#asyncio-client) * [Synopsis](#synopsis-1) * [Notes](#notes) *
+[Regular expression filters](#regular-expression-filters) * [Reconnect and
+retry method decorators](#reconnect-and-retry-method-decorators) *
+[Communities](#communities) * [Contributors](#contributors) * [Install Poetry]
+(#install-poetry) * [Setup for PyCharm users](#setup-for-pycharm-users) *
+[Setup from command line](#setup-from-command-line) * [Project Makefile
+commands](#project-makefile-commands) ## Synopsis The `EventStoreDBClient`
+class can be imported from the `esdbclient` package. Probably the three most
+useful methods of `EventStoreDBClient` are: * `append_to_stream()` This method
+can be used to record new events in a particular "stream". This is useful, for
+example, when executing a command in an application that mutates an aggregate.
+This method is "atomic" in that either all or none of the events will be
+recorded. * `get_stream()` This method can be used to retrieve all the recorded
+events in a "stream". This is useful, for example, when reconstructing an
+aggregate from recorded events before executing a command in an application
+that creates new events. * `subscribe_to_all()` This method can be used to
+receive all recorded events in the database. This is useful, for example, in
+event-processing components because it supports processing events with
+"exactly-once" semantics. The example below uses an "insecure" EventStoreDB
+server running locally on port 2113. ```python import uuid from esdbclient
+import EventStoreDBClient, NewEvent, StreamState # Construct EventStoreDBClient
+with an EventStoreDB URI. The # connection string URI specifies that the client
+should # connect to an "insecure" server running on port 2113. client =
+EventStoreDBClient( uri="esdb://localhost:2113?Tls=false" ) # Generate new
+events. Typically, domain events of different # types are generated in a domain
+model, and then serialized # into NewEvent objects. An aggregate ID may be used
+as the # name of a stream in EventStoreDB. stream_name1 = str(uuid.uuid4())
+event1 = NewEvent( type='OrderCreated', data=b'{"order_number": "123456"}' )
+event2 = NewEvent( type='OrderSubmitted', data=b'{}' ) event3 = NewEvent
+( type='OrderCancelled', data=b'{}' ) # Append new events to a new stream. The
+value returned # from the append_to_stream() method is the overall # "commit
+position" in the database of the last new event # recorded by this operation.
+The returned "commit position" # may be used in a user interface to poll an
+eventually # consistent event-processing component until it can # present an
+up-to-date materialized view. New events are # each allocated a "stream
+position", which is the next # available position in the stream, starting from
+0. commit_position1 = client.append_to_stream( stream_name=stream_name1,
 current_version=StreamState.NO_STREAM, events=[event1, event2], ) # Append
 events to an existing stream. The "current version" # is the "stream position"
 of the last recorded event in a # stream. We have recorded two new events, so
 the "current # version" is 1. The exception 'WrongCurrentVersion' will be #
 raised if an incorrect value is given. commit_position2 =
 client.append_to_stream( stream_name=stream_name1, current_version=1, events=
 [event3], ) # - allocated commit positions increase monotonically assert
@@ -97,90 +144,44 @@
 example. break # - events are received in the order they were recorded assert
 received_events[-3].type == "OrderCreated" assert received_events[-3].data ==
 b'{"order_number": "123456"}' assert received_events[-3].id == event1.id assert
 received_events[-2].type == "OrderSubmitted" assert received_events[-2].data ==
 b'{}' assert received_events[-2].id == event2.id assert received_events[-
 1].type == "OrderCancelled" assert received_events[-1].data == b'{}' assert
 received_events[-1].id == event3.id # Close the client's gRPC connection.
-client.close() ``` See below for more details. For an example of usage, see the
-[eventsourcing-eventstoredb]( https://github.com/pyeventsourcing/eventsourcing-
-eventstoredb) package. ## Table of contents * [Install package](#install-
-package) * [From PyPI](#from-pypi) * [With Poetry](#with-poetry) *
-[EventStoreDB server](#eventstoredb-server) * [Run container](#run-container) *
-[Stop container](#stop-container) * [EventStoreDB client](#eventstoredb-client)
-* [Import class](#import-class) * [Construct client](#construct-client) *
-[Connection strings](#connection-strings) * [Two schemes](#two-schemes) * [User
-info string](#user-info-string) * [Query string](#query-string) * [Examples]
-(#examples) * [Event objects](#event-objects) * [New events](#new-events) *
-[Recorded events](#recorded-events) * [Streams](#streams) * [Append events]
-(#append-events) * [Idempotent append operations](#idempotent-append-
-operations) * [Read stream events](#read-stream-events) * [Get current version]
-(#get-current-version) * [How to implement snapshotting with EventStoreDB]
-(#how-to-implement-snapshotting-with-eventstoredb) * [Read all events](#read-
-all-events) * [Get commit position](#get-commit-position) * [Get stream
-metadata](#get-stream-metadata) * [Set stream metadata](#set-stream-metadata) *
-[Delete stream](#delete-stream) * [Tombstone stream](#tombstone-stream) *
-[Catch-up subscriptions](#catch-up-subscriptions) * [Subscribe to all events]
-(#subscribe-to-all-events) * [Subscribe to stream events](#subscribe-to-stream-
-events) * [How to implement exactly-once event processing](#how-to-implement-
-exactly-once-event-processing) * [Persistent subscriptions](#persistent-
-subscriptions) * [Create subscription to all](#create-subscription-to-all) *
-[Read subscription to all](#read-subscription-to-all) * [How to write a
-persistent subscription consumer](#how-to-write-a-persistent-subscription-
-consumer) * [Update subscription to all](#update-subscription-to-all) * [Create
-subscription to stream](#create-subscription-to-stream) * [Read subscription to
-stream](#read-subscription-to-stream) * [Update subscription to stream]
-(#update-subscription-to-stream) * [Replay parked events](#replay-parked-
-events) * [Get subscription info](#get-subscription-info) * [List
-subscriptions](#list-subscriptions) * [List subscriptions to stream](#list-
-subscriptions-to-stream) * [Delete subscription](#delete-subscription) *
-[Projections](#projections) * [Create projection](#create-projection) * [Get
-projection state](#get-projection-state) * [Get projection result](#get-
-projection-result) * [Get projection statistics](#get-projection-statistics) *
-[Update projection](#update-projection) * [Enable projection](#enable-
-projection) * [Disable projection](#disable-projection) * [Reset projection]
-(#reset-projection) * [Delete projection](#delete-projection) * [Restart
-projections subsystem](#restart-projections-subsystem) * [Call credentials]
-(#call-credentials) * [Construct call credentials](#construct-call-credentials)
-* [Connection](#connection) * [Reconnect](#reconnect) * [Close](#close) *
-[Asyncio client](#asyncio-client) * [Synopsis](#synopsis-1) * [Notes](#notes) *
-[Regular expression filters](#regular-expression-filters) * [Reconnect and
-retry method decorators](#reconnect-and-retry-method-decorators) *
-[Contributors](#contributors) * [Install Poetry](#install-poetry) * [Setup for
-PyCharm users](#setup-for-pycharm-users) * [Setup from command line](#setup-
-from-command-line) * [Project Makefile commands](#project-makefile-commands) ##
-Install package It is recommended to install Python packages into a Python
-virtual environment. ### From PyPI You can use pip to install this package
-directly from [the Python Package Index](https://pypi.org/project/esdbclient/).
-$ pip install esdbclient ### With Poetry You can use Poetry to add this package
-to your pyproject.toml and install it. $ poetry add esdbclient ## EventStoreDB
-server The EventStoreDB server can be run locally using the official Docker
-container image. ### Run container For development, you can run a "secure"
-EventStoreDB server using the following command. $ docker run -d --name
-eventstoredb-secure -it -p 2113:2113 --env "HOME=/tmp" eventstore/eventstore:
-21.10.9-buster-slim --dev As we will see, your client will need an EventStoreDB
-connection string URI as the value of its `uri` constructor argument. The
-connection string for this "secure" EventStoreDB server would be: esdb://admin:
-changeit@localhost:2113 To connect to a "secure" server, you will usually need
-to include a "username" and a "password" in the connection string, so that the
-server can authenticate the client. With EventStoreDB, the default username is
-"admin" and the default password is "changeit". When connecting to a "secure"
-server, you may also need to provide an SSL/TLS certificate as the value of the
-`root_certificates` constructor argument. If the server certificate is publicly
-signed, the root certificates of the certificate authority may be installed
-locally and picked up by the grpc package from a default location. The client
-uses the root SSL/TLS certificate to authenticate the server. For development,
-you can either use the SSL/TLS certificate of a self-signing certificate
-authority used to create the server's certificate. Or, when using a single-node
-cluster, you can just use the server certificate itself, getting the server
-certificate with the following Python code. ```python import ssl
-server_certificate = ssl.get_server_certificate(addr=('localhost', 2113)) ```
-Alternatively, you can start an "insecure" server using the following command.
-$ docker run -d --name eventstoredb-insecure -it -p 2113:2113 eventstore/
-eventstore:21.10.9-buster-slim --insecure The connection string URI for this
+client.close() ``` ## Install package It is recommended to install Python
+packages into a Python virtual environment. ### From PyPI You can use pip to
+install this package directly from [the Python Package Index](https://pypi.org/
+project/esdbclient/). $ pip install esdbclient ### With Poetry You can use
+Poetry to add this package to your pyproject.toml and install it. $ poetry add
+esdbclient ## EventStoreDB server The EventStoreDB server can be run locally
+using the official Docker container image. ### Run container For development,
+you can run a "secure" EventStoreDB server using the following command. $
+docker run -d --name eventstoredb-secure -it -p 2113:2113 --env "HOME=/tmp"
+docker.eventstore.com/eventstore-ce/eventstoredb-ce:23.10.0-jammy --dev As we
+will see, your client will need an EventStoreDB connection string URI as the
+value of its `uri` constructor argument. The connection string for this
+"secure" EventStoreDB server would be: esdb://admin:changeit@localhost:2113 To
+connect to a "secure" server, you will usually need to include a "username" and
+a "password" in the connection string, so that the server can authenticate the
+client. With EventStoreDB, the default username is "admin" and the default
+password is "changeit". When connecting to a "secure" server, you may also need
+to provide an SSL/TLS certificate as the value of the `root_certificates`
+constructor argument. If the server certificate is publicly signed, the root
+certificates of the certificate authority may be installed locally and picked
+up by the grpc package from a default location. The client uses the root SSL/
+TLS certificate to authenticate the server. For development, you can either use
+the SSL/TLS certificate of a self-signing certificate authority used to create
+the server's certificate. Or, when using a single-node cluster, you can just
+use the server certificate itself, getting the server certificate with the
+following Python code. ```python import ssl server_certificate =
+ssl.get_server_certificate(addr=('localhost', 2113)) ``` Alternatively, you can
+start an "insecure" server using the following command. $ docker run -d --name
+eventstoredb-insecure -it -p 2113:2113 docker.eventstore.com/eventstore-ce/
+eventstoredb-ce:23.10.0-jammy --insecure The connection string URI for this
 "insecure" server would be: esdb://localhost:2113?Tls=false As we will see,
 when connecting to an "insecure" server, there is no need to include a
 "username" and a "password" in the connection string. If you do, these values
 will be ignored by the client, so that they are not sent over an insecure
 channel. Please note, the "insecure" connection string uses a query string with
 the field-value `Tls=false`. The value of this field is by default `true`. ###
 Stop container To stop and remove the "secure" container, use the following
@@ -190,42 +191,32 @@
 ## EventStoreDB client This EventStoreDB client is implemented in the
 `esdbclient` package with the `EventStoreDBClient` class. ### Import class The
 `EventStoreDBClient` class can be imported from the `esdbclient` package.
 ```python from esdbclient import EventStoreDBClient ``` ### Construct client
 The `EventStoreDBClient` class has one required constructor argument, `uri`,
 and one optional constructor argument, `root_certificates`. The `uri` argument
 is expected to be an EventStoreDB connection string URI that conforms with the
-standard EventStoreDB "esdb" or "esdb+discover" URI schemes. For example, the
-following connection string specifies that the client should attempt to create
-a "secure" connection to port 2113 on "localhost", and use the client
-credentials "username" and "password" when making calls to the server. esdb://
-username:password@localhost:2113?Tls=true The client must be configured to
-create a "secure" connection to a "secure" server, or alternatively an
-"insecure" connection to an "insecure" server. By default, the client will
-attempt to create a "secure" connection. And so, when connecting to an
-"insecure" server, the connection string must specify that the client should
-attempt to make an "insecure" connection. The following connection string
-specifies that the client should attempt to create an "insecure" connection to
-port 2113 on "localhost". When connecting to an "insecure" server, the client
-will ignore any username and password information included in the connection
-string, so that usernames and passwords are not sent over an "insecure"
-connection. esdb://localhost:2113?Tls=false Please note, the "insecure"
-connection string uses a query string with the field-value `Tls=false`. The
-value of this field is by default `true`. When connecting to a "secure" server,
-the `root_certificates` argument can be a Python `str` containing PEM encoded
+standard EventStoreDB "esdb" or "esdb+discover" URI schemes. The client must be
+configured to create a "secure" connection to a "secure" server, or
+alternatively an "insecure" connection to an "insecure" server. By default, the
+client will attempt to create a "secure" connection. And so, when connecting to
+an "insecure" server, the connection string must specify that the client should
+attempt to make an "insecure" connection. When connecting to a "secure" server,
+it may be necessary to set the optional `root_certificates` argument. The
+optional `root_certificates` argument is a Python `str` containing PEM encoded
 SSL/TLS root certificates. This value is passed directly to
-`grpc.ssl_channel_credentials()`. It is used for authenticating the server to
-the client. It is commonly the certificate of the certificate authority that
-was responsible for generating the SSL/TLS certificate used by the EventStoreDB
-server. Often it is unnecessary to provide these certificates explicitly, if
-they are installed locally in a such a way that the Python grpc library can
-pick them up from a default location. Alternatively, for development, you can
-use the server's certificate itself. In the example below, the constructor
-argument values are taken from the operating system environment. ```python
-import os client = EventStoreDBClient( uri=os.getenv("ESDB_URI"),
+`grpc.ssl_channel_credentials()` and is used by the client to authenticate the
+server. It is commonly a public certificate of the certificate authority that
+was responsible for generating the certificate used by the EventStoreDB server.
+Often it is unnecessary to provide these certificates explicitly, as they are
+commonly installed locally in a default location such that the Python grpc
+library can pick them up. Alternatively, for development, you can use the
+server's certificate itself. In the example below, the constructor argument
+values are taken from the operating system environment. ```python import os
+client = EventStoreDBClient( uri=os.getenv("ESDB_URI"),
 root_certificates=os.getenv("ESDB_ROOT_CERTIFICATES"), ) ``` ## Connection
 strings An EventStoreDB connection string is a URI that conforms with one of
 two possible schemes: either the "esdb" scheme, or the "esdb+discover" scheme.
 The syntax and semantics of the EventStoreDB URI schemes are described below.
 The syntax is defined using [EBNF](https://en.wikipedia.org/wiki/
 Extended_BackusâNaur_form). ### Two schemes The "esdb" URI scheme can be
 defined in the following way. esdb-uri = "esdb://" , [ user-info , "@" ] ,
@@ -236,129 +227,148 @@
 gRPC server socket, all in the same EventStoreDB cluster, by specifying a host
 and a port number separated with the ":" character. The host may be a hostname
 that can be resolved to an IP address, or an IP address. grpc-target =
 ( hostname | ip-address ) , ":" , port-number ; If there is one gRPC target,
 the client will simply attempt to connect to this server, and it will use this
 connection when recording and retrieving events. If there are two or more gRPC
 targets, the client will attempt to connect to the Gossip API of each in turn,
-to obtain information about the whole cluster. A member of the cluster is then
-selected by the client according to the "node preference" option of the
-connection string. The client may then need to close its connection and
-reconnect to the selected node. The "esdb+discover" URI scheme can be defined
-in the following way. esdb-discover-uri = "esdb+discover://" , [ user-info, "@"
-] , cluster-domainname, [ ":" , port-number ] , [ "?" , query-string ] ; In the
-"esdb+discover" URI scheme, after the optional user info string, there should
-be a domain name which identifies a cluster of EventStoreDB servers. Individual
-nodes in the cluster should be declared with DNS 'A' records. The client will
-create a gRPC connection using the cluster's domain name, using the gRPC
-library's 'round robin' load balancing strategy to call the Gossip API of
-addresses to which this domain name resolves. Information about the
-EventStoreDB cluster is obtained from the Gossip API. A member of the cluster
-is then selected by the client according to the "node preference" option. The
-client may then need to close its connection and reconnect to the selected
-node. ### User info string In both the "esdb" and "esdb+discover" schemes, the
-URI may include a user info string. If it exists in the URI, the user info
-string must be separated from the rest of the URI with the "@" character. The
-user info string must include a username and a password, separated with the ":
-" character. user-info = username , ":" , password ; The user info is sent by
-the client as "call credentials" in each call to a "secure" server, in a "basic
-auth" authorization header. This authorization header is used by the server to
-authenticate the client. The authorization header is not sent to "insecure"
-servers. ### Query string In both the "esdb" and "esdb+discover" schemes, the
-optional query string must be one or many field-value arguments, separated from
-each other with the "&" character. query-string = field-value, { "&", field-
-value } ; Each field-value argument must be one of the supported fields, and an
-appropriate value, separated with the "=" character. field-value = ( "Tls", "="
-, "true" | "false" ) | ( "TlsVerifyCert", "=" , "true" | "false" ) |
-( "ConnectionName", "=" , string ) | ( "NodePreference", "=" , "leader" |
-"follower" | "readonlyreplica" | "random" ) | ( "DefaultDeadline", "=" ,
-integer ) | ( "GossipTimeout", "=" , integer ) | ( "MaxDiscoverAttempts", "=" ,
-integer ) | ( "DiscoveryInterval", "=" , integer ) | ( "KeepAliveInterval", "="
-, integer ) | ( "KeepAliveTimeout", "=" , integer ) ; The table below describes
-the query field-values supported by this client. | Field | Value | Description
-| |---------------------|------------------------------------------------------
------------------|-------------------------------------------------------------
+attempting to obtain information about the cluster from it, until information
+about the cluster is obtained. A member of the cluster is then selected by the
+client according to the "node preference" specified by the connection string
+URI. The client will then close its connection and connect to the selected node
+without the 'round robin' load balancing strategy. If the "node preference" is
+"leader", and after connecting to a leader, if the leader becomes a follower,
+the client will reconnect to the new leader. The "esdb+discover" URI scheme can
+be defined in the following way. esdb-discover-uri = "esdb+discover://" ,
+[ user-info, "@" ] , cluster-domainname, [ ":" , port-number ] , [ "?" , query-
+string ] ; In the "esdb+discover" URI scheme, after the optional user info
+string, there should be a domain name which identifies a cluster of
+EventStoreDB servers. Individual nodes in the cluster should be declared with
+DNS 'A' records. The client will use the cluster domain name with the gRPC
+library's 'round robin' load balancing strategy to call the Gossip APIs of
+addresses discovered from DNS 'A' records. Information about the EventStoreDB
+cluster is obtained from the Gossip API. A member of the cluster is then
+selected by the client according to the "node preference" option. The client
+will then close its connection and connect to the selected node without the
+'round robin' load balancing strategy. If the "node preference" is "leader",
+and after connecting to a leader, if the leader becomes a follower, the client
+will reconnect to the new leader. ### User info string In both the "esdb" and
+"esdb+discover" schemes, the URI may include a user info string. If it exists
+in the URI, the user info string must be separated from the rest of the URI
+with the "@" character. The user info string must include a username and a
+password, separated with the ":" character. user-info = username , ":" ,
+password ; The user info is sent by the client in a "basic auth" authorization
+header in each gRPC call to a "secure" server. This authorization header is
+used by the server to authenticate the client. The Python gRPC library does not
+allow call credentials to be transferred to "insecure" servers. ### Query
+string In both the "esdb" and "esdb+discover" schemes, the optional query
+string must be one or many field-value arguments, separated from each other
+with the "&" character. query-string = field-value, { "&", field-value } ; Each
+field-value argument must be one of the supported fields, and an appropriate
+value, separated with the "=" character. field-value = ( "Tls", "=" , "true" |
+"false" ) | ( "TlsVerifyCert", "=" , "true" | "false" ) | ( "ConnectionName",
+"=" , string ) | ( "NodePreference", "=" , "leader" | "follower" |
+"readonlyreplica" | "random" ) | ( "DefaultDeadline", "=" , integer ) |
+( "GossipTimeout", "=" , integer ) | ( "MaxDiscoverAttempts", "=" , integer ) |
+( "DiscoveryInterval", "=" , integer ) | ( "KeepAliveInterval", "=" , integer )
+| ( "KeepAliveTimeout", "=" , integer ) ; The table below describes the query
+field-values supported by this client. | Field | Value | Description | |-------
+--------------|----------------------------------------------------------------
+-------|-----------------------------------------------------------------------
 -------------------------------------------------------------------------------
------------------------| | Tls | "true", "false" (default: "true") | If "true"
-the client will create a "secure" gRPC channel. If "false" the client will
-create an "insecure" gRPC channel. This must match the server configuration. |
-| TlsVerifyCert | "true", "false" (default: "true") | This value is currently
+-------------| | Tls | "true", "false" (default: "true") | If "true" the client
+will create a "secure" gRPC channel. If "false" the client will create an
+"insecure" gRPC channel. This must match the server configuration. | |
+TlsVerifyCert | "true", "false" (default: "true") | This value is currently
 ignored. | | ConnectionName | string (default: auto-generated version-4 UUID) |
 Sent in call metadata for every call, to identify the client to the cluster. |
 | NodePreference | "leader", "follower", "readonlyreplica", "random" (default:
 "leader") | The node state preferred by the client. The client will select a
 node from the cluster info received from the Gossip API according to this
 preference. | | DefaultDeadline | integer (default: `None`) | The default value
 (in seconds) of the `timeout` argument of client "write" methods such as
 `append_to_stream()`. | | GossipTimeout | integer (default: 5) | The default
 value (in seconds) of the `timeout` argument of gossip read methods, such as
 `read_gossip()`. | | MaxDiscoverAttempts | integer (default: 10) | The number
 of attempts to read gossip when connecting or reconnecting to a cluster member.
 | | DiscoveryInterval | integer (default: 100) | How long to wait (in
 milliseconds) between gossip retries. | | KeepAliveInterval | integer (default:
-`None`) | The value of the "grpc.keepalive_ms" gRPC channel option. | |
-KeepAliveTimeout | integer (default: `None`) | The value of the
-"grpc.keepalive_timeout_ms" gRPC channel option. | ### Examples Here are some
-examples of EventStoreDB connection string URIs. The following URI will cause
-the client to connect to, and get cluster info, from "secure" server socket
-`localhost:2113`. And then to connect to a "leader" node. And also to use
-"admin" and "changeit" as the username and password when making calls to
-EventStoreDB API methods. esdb://admin:changeit@localhost:2113 The following
-URI will cause the client to get cluster info from "insecure" server socket
-127.0.0.1:2113. And then to connect to a "leader" node. esdb://127.0.0.1:
-2113?Tls=false The following URI will cause the client to get cluster info from
-addresses in DNS 'A' records for cluster1.example.com. And then to connect to a
-"leader" node. And use a default deadline of 5 seconds when making calls to
-EventStore API "write" methods. esdb+discover://admin:
+`None`) | The value (in milliseconds) of the "grpc.keepalive_ms" gRPC channel
+option. | | KeepAliveTimeout | integer (default: `None`) | The value (in
+milliseconds) of the "grpc.keepalive_timeout_ms" gRPC channel option. | Please
+note, the client is insensitive to the case of fields and values. If fields are
+repeated in the query string, the query string will be parsed without error.
+However, the connection options used by the client will use the value of the
+first field. All the other field-values in the query string with the same field
+name will be ignored. Fields without values will also be ignored. If the
+client's node preference is "follower" and there are no follower nodes in the
+cluster, then the client will raise an exception. Similarly, if the client's
+node preference is "readonlyreplica" and there are no read-only replica nodes
+in the cluster, then the client will also raise an exception. The gRPC channel
+option "grpc.max_receive_message_length" is automatically configured to the
+value `17 * 1024 * 1024`. This value cannot be configured. ### Examples Here
+are some examples of EventStoreDB connection string URIs. The following URI
+will cause the client to make an "insecure" connection to gRPC target
+`'localhost:2113'`. Because the client's node preference is "follower", methods
+that can be called on a follower should complete successfully, methods that
+require a leader will raise a `NodeIsNotLeader` exception. esdb://127.0.0.1:
+2113?Tls=false&NodePreference=follower The following URI will cause the client
+to make an "insecure" connection to gRPC target `'localhost:2113'`. Because the
+client's node preference is "leader", if this node is not a leader, then a
+`NodeIsNotLeader` exception will be raised by all methods. esdb://127.0.0.1:
+2113?Tls=false&NodePreference=leader The following URI will cause the client to
+make a "secure" connection to gRPC target `'localhost:2113'` with username
+`'admin'` and password `'changeit'` as the default call credentials when making
+calls to the EventStoreDB gRPC API. Because the client's node preference is
+"leader", by default, if this node is not a leader, then a `NodeIsNotLeader`
+exception will be raised by all methods. esdb://admin:changeit@localhost:2113
+The following URI will cause the client to make "secure" connections, firstly
+to get cluster info from either `'localhost:2111'`, or `'localhost:2112'`, or
+`'localhost:2113'`. Because the client's node preference is "leader", the
+client will select the leader node from the cluster info and reconnect to the
+leader. If the "leader" node becomes a "follower" and another node becomes
+"leader", then the client will reconnect to the new leader. esdb://admin:
+changeit@localhost:2111,localhost:2112,localhost:2113?NodePreference=leader The
+following URI will cause the client to make "secure" connections, firstly to
+get cluster info from either `'localhost:2111'`, or `'localhost:2112'`, or
+`'localhost:2113'`. Because the client's node preference is "follower", the
+client will select a follower node from the cluster info and reconnect to this
+follower. Please note, if the "follower" node becomes the "leader", the client
+will not reconnect to a follower -- such behavior may be implemented in a
+future version of the client and server. esdb://admin:changeit@localhost:
+2111,localhost:2112,localhost:2113?NodePreference=follower The following URI
+will cause the client to make "secure" connections, firstly to get cluster info
+from addresses in DNS 'A' records for `'cluster1.example.com'`, and then to
+connect to a "leader" node. The client will use a default timeout of 5 seconds
+when making calls to EventStore API "write" methods. esdb+discover://admin:
 changeit@cluster1.example.com?DefaultDeadline=5 The following URI will cause
-the client to get cluster info from either localhost:2111, or localhost:2112,
-or localhost:2113. And then to connect to a "follower" node. esdb://admin:
-changeit@localhost:2111,localhost:2112,localhost:2113?NodePreference=follower
-The following URI will cause the client to get cluster info from addresses in
-DNS 'A' records for cluster1.example.com. And to configure "keep alive" timeout
-and interval in the gRPC channel. esdb+discover://admin:
-changeit@cluster1.example.com?KeepAliveInterval=10000&KeepAliveTimeout=10000
-Please note, the client is insensitive to the case of fields and values. If
-fields are repeated in the query string, the query string will be parsed
-without error. However, the connection options used by the client will use the
-value of the first field. All the other field-values in the query string with
-the same field name will be ignored. Fields without values will also be
-ignored. If the client's node preference is "leader" and the node becomes a
-"follower", the client will attempt to reconnect to the current leader when a
-method is called that expects to call a leader. Methods which mutate the state
-of the database expect to call a leader. For such methods, the HTTP header
-"requires-leader" is set to "true", and this header is observed by the server,
-and so a node which is not a leader that receives such a request will return an
-error. This error is detected by the client, which will then close the current
-gRPC connection and create a new connection to the leader. The request will
-then be retried with the leader. If the client's node preference is "follower"
-and there are no follower nodes in the cluster, then the client will raise an
-exception. Similarly, if the client's node preference is "readonlyreplica" and
-there are no read-only replica nodes in the cluster, then the client will also
-raise an exception. The gRPC channel option "grpc.max_receive_message_length"
-is automatically configured to the value `17 * 1024 * 1024`. This value cannot
-be changed. ## Event objects This package defines a `NewEvent` class and a
-`RecordedEvent` class. The `NewEvent` class should be used when writing events
-to the database. The `RecordedEvent` class is used when reading events from the
-database. ### New events The `NewEvent` class should be used when writing
-events to an EventStoreDB database. You will need to construct new event
-objects before calling `append_to_stream()`. The `NewEvent` class is a frozen
-Python dataclass. It has two required constructor arguments (`type` and `data`)
-and three optional constructor arguments (`metadata`, `content_type` and `id`).
-The required `type` argument is a Python `str`, used to describe the type of
-domain event that is being recorded. The required `data` argument is a Python
-`bytes` object, used to state the serialized data of the domain event that is
-being recorded. The optional `metadata` argument is a Python `bytes` object,
-used to indicate any metadata of the event that will be recorded. The default
-value is an empty `bytes` object. The optional `content_type` argument is a
-Python `str`, used to indicate the kind of data that is being recorded. The
-default value is `'application/json'`, which indicates that the `data` was
-serialised using JSON. An alternative value for this argument is the more
-general indication `'application/octet-stream'`. The optional `id` argument is
-a Python `UUID` object, used to specify the unique ID of the event that will be
+the client to make "secure" connections, firstly to get cluster info from
+addresses in DNS 'A' records for `'cluster1.example.com'`, and then to connect
+to a "leader" node. It will configure gRPC connections with a "keep alive
+interval" and a "keep alive timeout". esdb+discover://admin:
+changeit@cluster1.example.com?KeepAliveInterval=10000&KeepAliveTimeout=10000 ##
+Event objects This package defines a `NewEvent` class and a `RecordedEvent`
+class. The `NewEvent` class should be used when writing events to the database.
+The `RecordedEvent` class is used when reading events from the database. ###
+New events The `NewEvent` class should be used when writing events to an
+EventStoreDB database. You will need to construct new event objects before
+calling `append_to_stream()`. The `NewEvent` class is a frozen Python
+dataclass. It has two required constructor arguments (`type` and `data`) and
+three optional constructor arguments (`metadata`, `content_type` and `id`). The
+required `type` argument is a Python `str`, used to describe the type of domain
+event that is being recorded. The required `data` argument is a Python `bytes`
+object, used to state the serialized data of the domain event that is being
+recorded. The optional `metadata` argument is a Python `bytes` object, used to
+indicate any metadata of the event that will be recorded. The default value is
+an empty `bytes` object. The optional `content_type` argument is a Python
+`str`, used to indicate the kind of data that is being recorded. The default
+value is `'application/json'`, which indicates that the `data` was serialised
+using JSON. An alternative value for this argument is the more general
+indication `'application/octet-stream'`. The optional `id` argument is a Python
+`UUID` object, used to specify the unique ID of the event that will be
 recorded. If no value is provided, a new version-4 UUID will be generated.
 ```python new_event1 = NewEvent( type='OrderCreated', data=b'{"name": "Greg"}',
 ) assert new_event1.type == 'OrderCreated' assert new_event1.data == b'{"name":
 "Greg"}' assert new_event1.metadata == b'' assert new_event1.content_type ==
 'application/json' assert isinstance(new_event1.id, uuid.UUID) event_id =
 uuid.uuid4() new_event2 = NewEvent( type='ImageCreated',
 data=b'01010101010101', metadata=b'{"a": 1}', content_type='application/octet-
@@ -368,46 +378,48 @@
 new_event2.id == event_id ``` ### Recorded events The `RecordedEvent` class is
 used when reading events from an EventStoreDB database. The client will return
 event objects of this type from all methods that return recorded events, such
 as `get_stream()`, `subscribe_to_all()`, and `read_subscription_to_all()`. You
 do not need to construct recorded event objects. Like `NewEvent`, the
 `RecordedEvent` class is a frozen Python dataclass. It has all the attributes
 that `NewEvent` has (`type`, `data`, `metadata`, `content_type`, `id`) that
-follow from an event that was recorded, and some additional attributes that
+follow from an event having been recorded, and some additional attributes that
 follow from the recording of an event (`stream_name`, `stream_position`,
-`commit_position`, `recorded_at`). It also has a `link` attribute, which is set
-only when "link events" are "resolved". And it has a `retry_count` which is set
-only when reading persistence subscriptions. The `type` attribute is a Python
-`str`, used to indicate the type of an event that was recorded. The `data`
-attribute is a Python `bytes` object, used to indicate the data of an event
-that was recorded. The `metadata` attribute is a Python `bytes` object, used to
-indicate the metadata of an event that was recorded. The `content_type`
-attribute is a Python `str`, used to indicate the type of data that was
-recorded for an event. It is usually `'application/json'`, indicating that the
-data can be parsed as JSON. Alternatively, it is `'application/octet-stream'`.
-The `id` attribute is a Python `UUID` object, used to indicate the unique ID of
-an event that was recorded. The `stream_name` attribute is a Python `str`, used
-to indicate the name of a stream in which an event was recorded. The
-`stream_position` attribute is a Python `int`, used to indicate the position in
-a stream at which an event was recorded. In EventStoreDB, a "stream position"
-is an integer representing the position of a recorded event in a stream. Each
-recorded event is recorded at a position in a stream. Each stream position is
-occupied by only one recorded event. New events are recorded at the next
-unoccupied position. All sequences of stream positions are zero-based and
-gapless. The `commit_position` attribute is a Python `int`, used to indicate
-the position in the database at which an event was recorded. In EventStoreDB, a
-"commit position" is an integer representing the position of a recorded event
-in the database. Each recorded event is recorded at a position in the database.
-Each commit position is occupied by only one recorded event. Commit positions
-are zero-based and increase monotonically as new events are recorded. But,
-unlike stream positions, the sequence of successive commit positions is not
-gapless. Indeed, there are usually large differences between the commit
-positions of successively recorded events. Please note, in EventStoreDB 21.10,
-the `commit_position` of all `RecordedEvent` objects obtained from `read_stream
-()` is `None`, whereas those obtained from `read_all()` have the actual commit
+`commit_position`, `recorded_at`). It also has a `link` attribute, which is
+`None` unless the recorded event is a "link event" that has been "resolved" to
+the linked event. And it has a `retry_count` which has an integer value when
+receiving recorded events from persistence subscriptions, otherwise the value
+of `retry_count` is `None`. The `type` attribute is a Python `str`, used to
+indicate the type of an event that was recorded. The `data` attribute is a
+Python `bytes` object, used to indicate the data of an event that was recorded.
+The `metadata` attribute is a Python `bytes` object, used to indicate the
+metadata of an event that was recorded. The `content_type` attribute is a
+Python `str`, used to indicate the type of data that was recorded for an event.
+It is usually `'application/json'`, indicating that the data can be parsed as
+JSON. Alternatively, it is `'application/octet-stream'`. The `id` attribute is
+a Python `UUID` object, used to indicate the unique ID of an event that was
+recorded. The `stream_name` attribute is a Python `str`, used to indicate the
+name of a stream in which an event was recorded. The `stream_position`
+attribute is a Python `int`, used to indicate the position in a stream at which
+an event was recorded. In EventStoreDB, a "stream position" is an integer
+representing the position of a recorded event in a stream. Each recorded event
+is recorded at a position in a stream. Each stream position is occupied by only
+one recorded event. New events are recorded at the next unoccupied position.
+All sequences of stream positions are zero-based and gapless. The
+`commit_position` attribute is a Python `int`, used to indicate the position in
+the database at which an event was recorded. In EventStoreDB, a "commit
+position" is an integer representing the position of a recorded event in the
+database. Each recorded event is recorded at a position in the database. Each
+commit position is occupied by only one recorded event. Commit positions are
+zero-based and increase monotonically as new events are recorded. But, unlike
+stream positions, the sequence of successive commit positions is not gapless.
+Indeed, there are usually large differences between the commit positions of
+successively recorded events. Please note, in EventStoreDB 21.10, the
+`commit_position` of all `RecordedEvent` objects obtained from `read_stream()`
+is `None`, whereas those obtained from `read_all()` have the actual commit
 position of the recorded event. This was changed in version 22.10, so that
 event objects obtained from both `get_stream()` and `read_all()` have the
 actual commit position. The `commit_position` attribute of the `RecordedEvent`
 class is annotated with the type `Optional[int]` for this reason only. The
 `recorded_at` attribute is a Python `datetime`, used to indicate when an event
 was recorded by the database. The `link` attribute is an optional
 `RecordedEvent` that carries information about a "link event" that has been
@@ -1508,25 +1520,25 @@
 ( group_name=group_name1, ) ``` The example below deleted the persistent
 subscription `group_name2` on `stream_name2` which was created by calling
 `create_subscription_to_stream()`. ```python client.delete_subscription
 ( group_name=group_name2, stream_name=stream_name2, ) ``` ## Projections Please
 refer to the [EventStoreDB documentation](https://developers.eventstore.com/
 server/v23.10/projections.html) for more information on projections in
 EventStoreDB. ### Create projection The `create_projection()` method can be
-used to create a projection. This method has two required arguments, `name` and
-`query`. This required `name` argument is a Python `str` that specifies the
-name of the projection. This required `query` argument is a Python `str` that
-defines what the projection will do. This method also has four optional
-arguments, `emit_enabled`, `track_emitted_streams`, `timeout`, and
-`credentials`. The optional `emit_enabled` argument is a Python `bool` which
-specifies whether a projection will be able to emit events. If a `True` value
-is specified, the projection will be able to emit events, otherwise the
+used to create a "continuous" projection. This method has two required
+arguments, `name` and `query`. This required `name` argument is a Python `str`
+that specifies the name of the projection. This required `query` argument is a
+Python `str` that defines what the projection will do. This method also has
+four optional arguments, `emit_enabled`, `track_emitted_streams`, `timeout`,
+and `credentials`. The optional `emit_enabled` argument is a Python `bool`
+which specifies whether a projection will be able to emit events. If a `True`
+value is specified, the projection will be able to emit events, otherwise the
 projection will not be able to emit events. The default value of `emit_enabled`
-is `False`. Please note, if your projection query includes a call to `emit()`
-then `emit_enabled` must be `True`, otherwise the projection will not run. The
+is `False`. Please note, `emit_enabled` must be `True` if your projection query
+includes a call to `emit()`, otherwise the projection will not run. The
 optional `track_emitted_streams` argument is a Python `bool` which specifies
 whether a projection will have its emitted streams tracked. If a `True` value
 is specified, the projection will have its emitted streams tracked, otherwise
 the projection will not have its emitted streams tracked. The default value of
 `track_emitted_streams` is `False`. The purpose of tracking emitted streams is
 that they can optionally be deleted when a projection is deleted (see the
 `delete_projection()` method for more details). Please note, if you set
@@ -1540,50 +1552,64 @@
 have a "count" that is incremented once for each event. ```python
 projection_name = str(uuid.uuid4()) projection_query = """fromStream('%s')
 .when({ $init: function(){ return { count: 0 }; }, OrderCreated: function(s,e)
 { s.count += 1; }, OrderUpdated: function(s,e){ s.count += 1; }, OrderDeleted:
 function(s,e){ s.count += 1; } }) .outputState() """ % stream_name2
 client.create_projection( name=projection_name, query=projection_query, ) ```
 Please note, the `outputState()` call is optional, and causes the state of the
-projection to be persisted in a "result" stream. The default name of the result
-stream is `$projections-{projection_name}-result`, and this name can be used to
-read from and subscribe to the results stream with the `get_stream()`,
-`read_stream()`, `subscribe_stream()`, `create_subscription_to_stream()` and
-`read_subscription_to_stream()` methods. ### Get projection state The
-`get_projection_state()` method can be used to get a projection's state. This
-method has a required `name` argument, which is a Python `str` that specifies
-the name of a projection. This method also has three optional arguments,
-`partition`, `timeout`, and `credentials`. The optional `partition` argument is
-a Python `str` which specifies a partition... The optional `timeout` argument
-is a Python `float` which sets a maximum duration, in seconds, for the
+projection to be persisted in a "result" stream. If `outputState()` is called,
+an event representing the state of the projection will immediately be written
+to a "result" stream. The default name of the "result" stream for a projection
+with name `projection_name` is `$projections-{projection_name}-result`. This
+stream name can be used to read from and subscribe to the "result" stream, with
+the `get_stream()`, or `read_stream()`, or `subscribe_to_stream()`, or
+`create_subscription_to_stream()` and `read_subscription_to_stream()` methods.
+If your projections doesn't call `outputState()`, then you won't be able to
+read or subscribe to a "result" stream, but you will still be able to get the
+projection "result" using the `get_projection_result()` method. The "type"
+string of events recorded in "result" streams is `'Result'`. You may want to
+include this in a `filter_exclude` argument when filtering events by type
+whilst reading or subscribing to "all" events recorded in the database (with
+`read_all()`, `subscribe_to_all()`, etc). Additionally, and in any case, from
+time to time the state of the projection will be recorded in a "state" stream,
+and also the projection will write to a "checkpoint" stream. The "state"
+stream, the "checkpoint" stream, and all "emitted" streams that have been
+"tracked" (as a consequence of the `track_emitted_streams` argument having been
+`True`) can optionally be deleted when the projection is deleted. See
+`delete_projection()` for details. Unlike the "result" and "emitted" streams,
+the "state" and the "checkpoint" streams cannot be read or subscribed to by
+users, or viewed in the "stream browser" view of EventStoreDB's Web interface.
+### Get projection state The `get_projection_state()` method can be used to get
+a projection's "state". This method has a required `name` argument, which is a
+Python `str` that specifies the name of a projection. This method also has two
+optional arguments, `timeout` and `credentials`. The optional `timeout`
+argument is a Python `float` which sets a maximum duration, in seconds, for the
 completion of the gRPC operation. The optional `credentials` argument can be
 used to override call credentials derived from the connection string URI. In
 the example below, after sleeping for 1 second to allow the projection to
 process all the recorded events, the projection "state" is obtained. We can see
 that the projection has processed three events. ```python sleep(1) # allow time
 for projection to process recorded events projection_state =
 client.get_projection_state(name=projection_name) assert projection_state.value
 == {'count': 3} ``` ### Get projection result The `get_projection_result()`
-method can be used to get a projection's result. This method has a required
+method can be used to get a projection's "result". A projection's "result"
+holds the same data as the projections "state". This method has a required
 `name` argument, which is a Python `str` that specifies the name of a
-projection. This method also has three optional arguments, `partition`,
-`timeout`, and `credentials`. The optional `partition` argument is a Python
-`str` which specifies a partition. The optional `timeout` argument is a Python
-`float` which sets a maximum duration, in seconds, for the completion of the
-gRPC operation. The optional `credentials` argument can be used to override
-call credentials derived from the connection string URI. In the example below,
-the projection "result" is obtained. We can see that the projection has
-processed three events. ```python projection_result =
-client.get_projection_result(name=projection_name) assert
-projection_result.value == {'count': 3} ``` ### Get projection statistics The
-`get_projection_statistucs()` method can be used to get projection statistics.
-This method has a required `name` argument, which is a Python `str` that
-specifies the name of a projection. This method also has three optional
-arguments, `partition`, `timeout`, and `credentials`. The optional `partition`
-argument is a Python `str` which specifies a partition. The optional `timeout`
+projection. This method also has two optional arguments, `timeout` and
+`credentials`. The optional `timeout` argument is a Python `float` which sets a
+maximum duration, in seconds, for the completion of the gRPC operation. The
+optional `credentials` argument can be used to override call credentials
+derived from the connection string URI. In the example below, the projection
+"result" is obtained. We can see that the projection has processed three
+events. ```python projection_result = client.get_projection_result
+(name=projection_name) assert projection_result.value == {'count': 3} ``` ###
+Get projection statistics The `get_projection_statistics()` method can be used
+to get projection statistics. This method has a required `name` argument, which
+is a Python `str` that specifies the name of a projection. This method also has
+two optional arguments, `timeout` and `credentials`. The optional `timeout`
 argument is a Python `float` which sets a maximum duration, in seconds, for the
 completion of the gRPC operation. The optional `credentials` argument can be
 used to override call credentials derived from the connection string URI. This
 method returns a `ProjectionStatistics` object that represents the named
 projection. ```python statistics = client.get_projection_statistics
 (name=projection_name) ``` A `ProjectionStatistics` object is returned. The
 attributes of this object have values that represent the progress of the
@@ -1593,82 +1619,84 @@
 name of the projection to be updated. The required `query` argument is a Python
 `str` which defines what the projection will do. This method also has three
 optional arguments, `emit_enabled`, `timeout`, and `credentials`. The optional
 `emit_enabled` argument is a Python `bool` which specifies whether a projection
 will be able to emit events. If a `True` value is specified, the projection
 will be able to emit events. If a `False` value is specified, the projection
 will not be able to emit events. The default value of `emit_enabled` is
-`False`. Please note, if your projection query includes a call to `emit()` then
-`emit_enabled` must be `True`, otherwise the projection will not run. Please
+`False`. Please note, `emit_enabled` must be `True` if your projection query
+includes a call to `emit()`, otherwise the projection will not run. Please
 note, it is not possible to update `track_emitted_streams` via the gRPC API.
 The optional `timeout` argument is a Python `float` which sets a maximum
 duration, in seconds, for the completion of the gRPC operation. The optional
 `credentials` argument can be used to override call credentials derived from
 the connection string URI. ```python client.update_projection
 (name=projection_name, query=projection_query) ``` ### Enable projection The
-`enable_projection()` method can be used to enable a projection that was
-previously disabled. This method has a required `name` argument, which is a
-Python `str` that specifies the name of the projection to be enabled. This
-method also has two optional arguments, `timeout` and `credentials`. The
-optional `timeout` argument is a Python `float` which sets a maximum duration,
-in seconds, for the completion of the gRPC operation. The optional
-`credentials` argument can be used to override call credentials derived from
-the connection string URI. ```python client.enable_projection
-(name=projection_name) ``` ### Disable projection The `disable_projection()`
-method can be used to disable a projection. This method has a required `name`
+`enable_projection()` method can be used to enable (start running) a projection
+that was previously disabled (stopped). This method has a required `name`
 argument, which is a Python `str` that specifies the name of the projection to
-be disabled. This method also has three optional arguments, `write_checkpoint`,
-`timeout`, and `credentials`. The optional `write_checkpoint` argument is a
-Python `bool` which specifies whether a checkpoint will be written when the
-projection is disabled. If `write_checkpoint` is `True` a checkpoint will be
-written, otherwise a checkpoint will not be written. The default value of
-`write_checkpoint` is `False`. The optional `timeout` argument is a Python
+be enabled. This method also has two optional arguments, `timeout` and
+`credentials`. The optional `timeout` argument is a Python `float` which sets a
+maximum duration, in seconds, for the completion of the gRPC operation. The
+optional `credentials` argument can be used to override call credentials
+derived from the connection string URI. ```python client.enable_projection
+(name=projection_name) ``` ### Disable projection The `disable_projection()`
+method can be used to disable (stop running) a projection. This method has a
+required `name` argument, which is a Python `str` that specifies the name of
+the projection to be disabled. This method also has two optional arguments,
+`timeout`, and `credentials`. The optional `timeout` argument is a Python
 `float` which sets a maximum duration, in seconds, for the completion of the
 gRPC operation. The optional `credentials` argument can be used to override
 call credentials derived from the connection string URI. ```python
 client.disable_projection(name=projection_name) ``` ### Reset projection The
 `reset_projection()` method can be used to reset a projection. This method has
 a required `name` argument, which is a Python `str` that specifies the name of
-the projection to be reset. This method also has three optional arguments,
-`write_checkpoint`, `timeout`, and `credentials`. The optional
-`write_checkpoint` argument is a Python `bool` which specifies whether a
-checkpoint will be written when the projection is reset. If `write_checkpoint`
-is `True` a checkpoint will be written, otherwise a checkpoint will not be
-written. The default value of `write_checkpoint` is `False`. The optional
-`timeout` argument is a Python `float` which sets a maximum duration, in
-seconds, for the completion of the gRPC operation. The optional `credentials`
-argument can be used to override call credentials derived from the connection
-string URI. ```python client.reset_projection(name=projection_name) ``` ###
-Delete projection The `delete_projection()` method can be used to delete a
-projection. This method has a required `name` argument, which is a Python `str`
-that specifies the name of the projection to be deleted. This method also has
-five optional arguments, `delete_emitted_streams`, `delete_state_stream`,
-`delete_checkpoint_stream`, `timeout`, and `credentials`. The optional
-`delete_emitted_streams` argument is a Python `bool` which specifies that the
-emitted streams will be deleted. For emitted streams to be deleted, they must
-have been tracked (see the `track_emitted_streams` argument of the
-`create_projection()` method.) The optional `delete_state_stream` argument is a
-Python `bool` which... The optional `delete_checkpoint_stream` argument is a
-Python `bool` which... The optional `timeout` argument is a Python `float`
-which sets a maximum duration, in seconds, for the completion of the gRPC
-operation. The optional `credentials` argument can be used to override call
-credentials derived from the connection string URI. ```python
-client.delete_projection(name=projection_name) ``` ### Restart projections
+the projection to be reset. This method also has two optional arguments,
+`timeout`, and `credentials`. The optional `timeout` argument is a Python
+`float` which sets a maximum duration, in seconds, for the completion of the
+gRPC operation. The optional `credentials` argument can be used to override
+call credentials derived from the connection string URI. ```python
+client.reset_projection(name=projection_name) ``` Please note, a projection
+must be disabled before it can be reset. ### Delete projection The
+`delete_projection()` method can be used to delete a projection. This method
+has a required `name` argument, which is a Python `str` that specifies the name
+of the projection to be deleted. This method also has five optional arguments,
+`delete_emitted_streams`, `delete_state_stream`, `delete_checkpoint_stream`,
+`timeout`, and `credentials`. The optional `delete_emitted_streams` argument is
+a Python `bool` which specifies that all "emitted" streams that have been
+tracked will be deleted. For emitted streams to be deleted, they must have been
+tracked (see the `track_emitted_streams` argument of the `create_projection()`
+method.) The optional `delete_state_stream` argument is a Python `bool` which
+specifies that the projection's "state" stream should also be deleted. The
+"state" stream is like the "result" stream, but events are written to the
+"state" stream occasionally, along with events written to the "checkpoint"
+stream, rather than being written immediately in the way a call `outputState()`
+immediately writes events to the "result" stream. The optional
+`delete_checkpoint_stream` argument is a Python `bool` which specifies that the
+projection's "checkpoint" stream should also be deleted. The optional `timeout`
+argument is a Python `float` which sets a maximum duration, in seconds, for the
+completion of the gRPC operation. The optional `credentials` argument can be
+used to override call credentials derived from the connection string URI.
+```python client.delete_projection(name=projection_name) ``` Please note, a
+projection must be disabled before it can be deleted. ### Restart projections
 subsystem The `restart_projections_subsystem()` method can be used to restart
 the projections subsystem. This method also has two optional arguments,
 `timeout` and `credentials`. The optional `timeout` argument is a Python
 `float` which sets a maximum duration, in seconds, for the completion of the
 gRPC operation. The optional `credentials` argument can be used to override
 call credentials derived from the connection string URI. ```python
 client.restart_projections_subsystem() ``` ## Call credentials Default call
 credentials are derived by the client from the user info part of the connection
 string URI. Many of the client methods described above have an optional
 `credentials` argument, which can be used to set call credentials for an
 individual method call that override those derived from the connection string
-URI. ### Construct call credentials The client method
+URI. Call credentials are sent to "secure" servers in a "basic auth"
+authorization header. This authorization header is used by the server to
+authenticate the client. The authorization header is not sent to "insecure"
+servers. ### Construct call credentials The client method
 `construct_call_credentials()` can be used to construct a call credentials
 object from a username and password. ```python call_credentials =
 client.construct_call_credentials( username='admin', password='changeit' ) ```
 The call credentials object can be used as the value of the `credentials`
 argument in other client methods. ## Connection ### Reconnect The `reconnect()`
 method can be used to manually reconnect the client to a suitable EventStoreDB
 node. This method uses the same routine for reading the cluster node states and
@@ -1804,61 +1832,63 @@
 `subscribe_to_stream()`, if the server is unavailable, or if the channel has
 somehow been closed, or if the request fails for some other reason, then the
 client will reconnect and retry. However, if an exception is raised when
 iterating over a successfully returned "catch-up subscription" object, the
 catch-up subscription will need to be restarted. Similarly, when reading
 persistent subscriptions, if there are connection issues whilst iterating over
 a successfully received response, the consumer will need to be restarted. ##
-Contributors ### Install Poetry The first thing is to check you have Poetry
-installed. $ poetry --version If you don't, then please [install Poetry](https:
-//python-poetry.org/docs/#installing-with-the-official-installer). $ curl -sSL
-https://install.python-poetry.org | python3 - It will help to make sure
-Poetry's bin directory is in your `PATH` environment variable. But in any case,
-make sure you know the path to the `poetry` executable. The Poetry installer
-tells you where it has been installed, and how to configure your shell. Please
-refer to the [Poetry docs](https://python-poetry.org/docs/) for guidance on
-using Poetry. ### Setup for PyCharm users You can easily obtain the project
-files using PyCharm (menu "Git > Clone..."). PyCharm will then usually prompt
-you to open the project. Open the project in a new window. PyCharm will then
-usually prompt you to create a new virtual environment. Create a new Poetry
-virtual environment for the project. If PyCharm doesn't already know where your
-`poetry` executable is, then set the path to your `poetry` executable in the
-"New Poetry Environment" form input field labelled "Poetry executable". In the
-"New Poetry Environment" form, you will also have the opportunity to select
-which Python executable will be used by the virtual environment. PyCharm will
-then create a new Poetry virtual environment for your project, using a
-particular version of Python, and also install into this virtual environment
-the project's package dependencies according to the project's `poetry.lock`
-file. You can add different Poetry environments for different Python versions,
-and switch between them using the "Python Interpreter" settings of PyCharm. If
-you want to use a version of Python that isn't installed, either use your
-favourite package manager, or install Python by downloading an installer for
-recent versions of Python directly from the [Python website](https://
-www.python.org/downloads/). Once project dependencies have been installed, you
-should be able to run tests from within PyCharm (right-click on the `tests`
-folder and select the 'Run' option). Because of a conflict between pytest and
-PyCharm's debugger and the coverage tool, you may need to add ``--no-cov`` as
-an option to the test runner template. Alternatively, just use the Python
-Standard Library's ``unittest`` module. You should also be able to open a
-terminal window in PyCharm, and run the project's Makefile commands from the
-command line (see below). ### Setup from command line Obtain the project files,
-using Git or suitable alternative. In a terminal application, change your
-current working directory to the root folder of the project files. There should
-be a Makefile in this folder. Use the Makefile to create a new Poetry virtual
-environment for the project and install the project's package dependencies into
-it, using the following command. $ make install-packages It's also possible to
-also install the project in 'editable mode'. $ make install Please note, if you
-create the virtual environment in this way, and then try to open the project in
-PyCharm and configure the project to use this virtual environment as an
-"Existing Poetry Environment", PyCharm sometimes has some issues (don't know
-why) which might be problematic. If you encounter such issues, you can resolve
-these issues by deleting the virtual environment and creating the Poetry
-virtual environment using PyCharm (see above). ### Project Makefile commands
-You can start EventStoreDB using the following command. $ make start-
-eventstoredb You can run tests using the following command (needs EventStoreDB
-to be running). $ make test You can stop EventStoreDB using the following
-command. $ make stop-eventstoredb You can check the formatting of the code
-using the following command. $ make lint You can reformat the code using the
-following command. $ make fmt Tests belong in `./tests`. Code-under-test
-belongs in `./esdbclient`. Edit package dependencies in `pyproject.toml`.
-Update installed packages (and the `poetry.lock` file) using the following
-command. $ make update-packages
+Communities - [Issues](https://github.com/pyeventsourcing/esdbclient/issues) -
+[Discuss](https://discuss.eventstore.com/) - [Discord (Event Store)](https://
+discord.gg/Phn9pmCw3t) ## Contributors ### Install Poetry The first thing is to
+check you have Poetry installed. $ poetry --version If you don't, then please
+[install Poetry](https://python-poetry.org/docs/#installing-with-the-official-
+installer). $ curl -sSL https://install.python-poetry.org | python3 - It will
+help to make sure Poetry's bin directory is in your `PATH` environment
+variable. But in any case, make sure you know the path to the `poetry`
+executable. The Poetry installer tells you where it has been installed, and how
+to configure your shell. Please refer to the [Poetry docs](https://python-
+poetry.org/docs/) for guidance on using Poetry. ### Setup for PyCharm users You
+can easily obtain the project files using PyCharm (menu "Git > Clone...").
+PyCharm will then usually prompt you to open the project. Open the project in a
+new window. PyCharm will then usually prompt you to create a new virtual
+environment. Create a new Poetry virtual environment for the project. If
+PyCharm doesn't already know where your `poetry` executable is, then set the
+path to your `poetry` executable in the "New Poetry Environment" form input
+field labelled "Poetry executable". In the "New Poetry Environment" form, you
+will also have the opportunity to select which Python executable will be used
+by the virtual environment. PyCharm will then create a new Poetry virtual
+environment for your project, using a particular version of Python, and also
+install into this virtual environment the project's package dependencies
+according to the project's `poetry.lock` file. You can add different Poetry
+environments for different Python versions, and switch between them using the
+"Python Interpreter" settings of PyCharm. If you want to use a version of
+Python that isn't installed, either use your favourite package manager, or
+install Python by downloading an installer for recent versions of Python
+directly from the [Python website](https://www.python.org/downloads/). Once
+project dependencies have been installed, you should be able to run tests from
+within PyCharm (right-click on the `tests` folder and select the 'Run' option).
+Because of a conflict between pytest and PyCharm's debugger and the coverage
+tool, you may need to add ``--no-cov`` as an option to the test runner
+template. Alternatively, just use the Python Standard Library's ``unittest``
+module. You should also be able to open a terminal window in PyCharm, and run
+the project's Makefile commands from the command line (see below). ### Setup
+from command line Obtain the project files, using Git or suitable alternative.
+In a terminal application, change your current working directory to the root
+folder of the project files. There should be a Makefile in this folder. Use the
+Makefile to create a new Poetry virtual environment for the project and install
+the project's package dependencies into it, using the following command. $ make
+install-packages It's also possible to also install the project in 'editable
+mode'. $ make install Please note, if you create the virtual environment in
+this way, and then try to open the project in PyCharm and configure the project
+to use this virtual environment as an "Existing Poetry Environment", PyCharm
+sometimes has some issues (don't know why) which might be problematic. If you
+encounter such issues, you can resolve these issues by deleting the virtual
+environment and creating the Poetry virtual environment using PyCharm (see
+above). ### Project Makefile commands You can start EventStoreDB using the
+following command. $ make start-eventstoredb You can run tests using the
+following command (needs EventStoreDB to be running). $ make test You can stop
+EventStoreDB using the following command. $ make stop-eventstoredb You can
+check the formatting of the code using the following command. $ make lint You
+can reformat the code using the following command. $ make fmt Tests belong in
+`./tests`. Code-under-test belongs in `./esdbclient`. Edit package dependencies
+in `pyproject.toml`. Update installed packages (and the `poetry.lock` file)
+using the following command. $ make update-packages
```

