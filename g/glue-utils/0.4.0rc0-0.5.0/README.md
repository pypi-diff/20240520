# Comparing `tmp/glue_utils-0.4.0rc0.tar.gz` & `tmp/glue_utils-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glue_utils-0.4.0rc0.tar", max compression
+gzip compressed data, was "glue_utils-0.5.0.tar", max compression
```

## Comparing `glue_utils-0.4.0rc0.tar` & `glue_utils-0.5.0.tar`

### file list

```diff
@@ -1,14 +1,21 @@
--rw-r--r--   0        0        0     1077 2024-03-06 15:16:48.910706 glue_utils-0.4.0rc0/LICENSE
--rw-r--r--   0        0        0     1138 2024-03-07 09:36:58.526889 glue_utils-0.4.0rc0/README.md
--rw-r--r--   0        0        0     3828 2024-05-12 10:27:19.294331 glue_utils-0.4.0rc0/pyproject.toml
--rw-r--r--   0        0        0       92 2024-05-12 10:27:19.294679 glue_utils-0.4.0rc0/src/glue_utils/__init__.py
--rw-r--r--   0        0        0     1050 2024-05-10 09:44:26.756369 glue_utils-0.4.0rc0/src/glue_utils/options.py
--rw-r--r--   0        0        0        0 2024-05-03 09:02:47.986990 glue_utils-0.4.0rc0/src/glue_utils/py.typed
--rw-r--r--   0        0        0      577 2024-05-12 10:26:39.523202 glue_utils-0.4.0rc0/src/glue_utils/pyspark/__init__.py
--rw-r--r--   0        0        0      674 2024-05-10 12:17:39.961510 glue_utils-0.4.0rc0/src/glue_utils/pyspark/context.py
--rw-r--r--   0        0        0     2652 2024-05-10 12:17:39.961783 glue_utils-0.4.0rc0/src/glue_utils/pyspark/job.py
--rw-r--r--   0        0        0      466 2024-05-12 10:26:39.523784 glue_utils-0.4.0rc0/src/glue_utils/pyspark/mixins/__init__.py
--rw-r--r--   0        0        0      849 2024-05-10 12:17:39.962157 glue_utils-0.4.0rc0/src/glue_utils/pyspark/mixins/connection_types.py
--rw-r--r--   0        0        0     8981 2024-05-12 10:26:39.524433 glue_utils-0.4.0rc0/src/glue_utils/pyspark/mixins/jdbc.py
--rw-r--r--   0        0        0    13057 2024-05-12 10:26:39.525070 glue_utils-0.4.0rc0/src/glue_utils/pyspark/mixins/s3.py
--rw-r--r--   0        0        0     2253 1970-01-01 00:00:00.000000 glue_utils-0.4.0rc0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-03-06 15:16:48.910706 glue_utils-0.5.0/LICENSE
+-rw-r--r--   0        0        0     2221 2024-05-19 23:47:08.494209 glue_utils-0.5.0/README.md
+-rw-r--r--   0        0        0     4142 2024-05-20 00:27:25.073298 glue_utils-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0       89 2024-05-20 00:27:25.074725 glue_utils-0.5.0/src/glue_utils/__init__.py
+-rw-r--r--   0        0        0     1050 2024-05-10 09:44:26.756369 glue_utils-0.5.0/src/glue_utils/options.py
+-rw-r--r--   0        0        0        0 2024-05-03 09:02:47.986990 glue_utils-0.5.0/src/glue_utils/py.typed
+-rw-r--r--   0        0        0      950 2024-05-19 23:47:08.495182 glue_utils-0.5.0/src/glue_utils/pyspark/__init__.py
+-rw-r--r--   0        0        0     8542 2024-05-19 23:47:08.495829 glue_utils-0.5.0/src/glue_utils/pyspark/connection_options.py
+-rw-r--r--   0        0        0      919 2024-05-19 23:47:08.496480 glue_utils-0.5.0/src/glue_utils/pyspark/connection_types.py
+-rw-r--r--   0        0        0      897 2024-05-19 23:47:08.496994 glue_utils-0.5.0/src/glue_utils/pyspark/context/__init__.py
+-rw-r--r--   0        0        0     2188 2024-05-19 23:47:08.497455 glue_utils-0.5.0/src/glue_utils/pyspark/context/documentdb.py
+-rw-r--r--   0        0        0     2154 2024-05-19 23:47:08.497854 glue_utils-0.5.0/src/glue_utils/pyspark/context/dynamodb.py
+-rw-r--r--   0        0        0    10415 2024-05-19 23:47:08.498336 glue_utils-0.5.0/src/glue_utils/pyspark/context/jdbc.py
+-rw-r--r--   0        0        0     2137 2024-05-19 23:47:08.498764 glue_utils-0.5.0/src/glue_utils/pyspark/context/kinesis.py
+-rw-r--r--   0        0        0     2137 2024-05-19 23:47:08.499372 glue_utils-0.5.0/src/glue_utils/pyspark/context/mongodb.py
+-rw-r--r--   0        0        0     2188 2024-05-19 23:47:08.499825 glue_utils-0.5.0/src/glue_utils/pyspark/context/opensearch.py
+-rw-r--r--   0        0        0    10403 2024-05-19 23:47:08.500298 glue_utils-0.5.0/src/glue_utils/pyspark/context/s3.py
+-rw-r--r--   0        0        0     2007 2024-05-19 23:47:08.500797 glue_utils-0.5.0/src/glue_utils/pyspark/format_options.py
+-rw-r--r--   0        0        0      259 2024-05-19 23:47:08.501108 glue_utils-0.5.0/src/glue_utils/pyspark/formats.py
+-rw-r--r--   0        0        0     6123 2024-05-20 00:26:10.700994 glue_utils-0.5.0/src/glue_utils/pyspark/job.py
+-rw-r--r--   0        0        0     3333 1970-01-01 00:00:00.000000 glue_utils-0.5.0/PKG-INFO
```

### Comparing `glue_utils-0.4.0rc0/LICENSE` & `glue_utils-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `glue_utils-0.4.0rc0/pyproject.toml` & `glue_utils-0.5.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "glue-utils"
-version = "0.4.0rc0"
+version = "0.5.0"
 package-mode = true
 description = "Reusable utilities for working with Glue PySpark jobs"
 authors = ["Noel Llevares <dashmug@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/dashmug/glue-utils"
 repository = "https://github.com/dashmug/glue-utils/issues"
@@ -31,17 +31,17 @@
 python = "^3.9"
 
 [tool.poetry.group.dev.dependencies]
 pytest-randomly = "^3.15.0"
 pytest-cov = "^5.0.0"
 mypy = "^1.10.0"
 bumpver = "^2023.1129"
-pytest = "^8.2.0"
 import-linter = "^2.0"
 ruff = "^0.4.4"
+pytest = "^8.2.1"
 
 [tool.poetry.group.local.dependencies]
 # The "local" dependency group refers to dependencies that already 
 # exist in AWS Glue's runtime. We don't need to install these in the
 # container. We only need them for local (non-container) development to 
 # aid the IDE in providing code completion and type checking.
 # 
@@ -72,15 +72,17 @@
     "COM812",
     "ISC001",
     # missing-type-self
     "ANN101",
     # missing-type-cls
     "ANN102",
     # line-too-long
-    "E501"
+    "E501",
+    # Ignore camelCase attributes since Glue uses a lot of them
+    "N815"
 ]
 # # Allow unused variables when underscore-prefixed.
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 
 [tool.ruff.lint.mccabe]
 max-complexity = 5
 
@@ -99,19 +101,22 @@
 
 [[tool.mypy.overrides]]
 module = "test.*"
 disallow_incomplete_defs = false
 disallow_untyped_defs = false
 
 [tool.pytest.ini_options]
+addopts = "--cov=glue_utils --cov-report=term --cov-report=html --cov-report=xml"
 filterwarnings = [
     "ignore::FutureWarning:pyspark.sql.context",
 ]
 
 [tool.coverage.run]
+relative_files = true
+branch = true
 omit = ["**/test_*.py"]
 
 [tool.coverage.paths]
 source = ["src/glue_utils", "*/site-packages/glue_utils"]
 
 [tool.coverage.report]
 skip_empty = true
@@ -125,28 +130,34 @@
     "if __name__ == .__main__.:",
     "if TYPE_CHECKING:",
     "class .*\\bProtocol\\):",
     "@(abc\\.)?abstractmethod",
     "@overload",
 ]
 
+[tool.coverage.xml]
+output = "coverage/results.xml"
+
 [tool.bumpver]
-current_version = "0.4.0rc0"
+current_version = "0.5.0"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "release: Bump version {old_version} -> {new_version}"
 commit = true
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
     'current_version = "{version}"',
     'version = "{version}"',
 ]
 "src/glue_utils/__init__.py" = [
     '^__version__ = "{version}"$',
 ]
+"sonar-project.properties" = [
+    '^sonar.projectVersion={version}$',
+]
 
 [tool.importlinter]
 root_package = "glue_utils"
 
 [[tool.importlinter.contracts]]
 name = "Generic code should not import specific code"
 type = "layers"
```

### Comparing `glue_utils-0.4.0rc0/src/glue_utils/options.py` & `glue_utils-0.5.0/src/glue_utils/options.py`

 * *Files identical despite different names*

### Comparing `glue_utils-0.4.0rc0/src/glue_utils/pyspark/mixins/connection_types.py` & `glue_utils-0.5.0/src/glue_utils/pyspark/connection_types.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from enum import Enum  # noqa: D100
+"""Module containing classes and types for handling different connection types."""
+
+from enum import Enum
 
 
 class ConnectionType(Enum):
     """Enum class representing different types of connections."""
 
     DYNAMODB = "dynamodb"
     KINESIS = "kinesis"
```

### Comparing `glue_utils-0.4.0rc0/src/glue_utils/pyspark/mixins/jdbc.py` & `glue_utils-0.5.0/src/glue_utils/pyspark/context/jdbc.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,21 @@
 from __future__ import annotations  # noqa: D100
 
-from typing import TYPE_CHECKING, Literal, TypedDict
+from typing import TYPE_CHECKING
 
-from .connection_types import ConnectionType
+from glue_utils.pyspark.connection_types import ConnectionType
 
 if TYPE_CHECKING:
     from awsglue.context import GlueContext
     from awsglue.dynamicframe import DynamicFrame
 
-
-class JDBCConnectionOptions(TypedDict, total=False):
-    """Connection options for JDBC connections.
-
-    Reference
-    ---------
-    - https://docs.aws.amazon.com/glue/latest/dg/aws-glue-programming-etl-connect-jdbc-home.html
-
-    """
-
-    useConnectionProperties: Literal["true"]
-    connectionName: str
-    databaseName: str
-    url: str
-    dbtable: str
-    user: str
-    password: str
-    customJdbcDriverS3Path: str
-    customJdbcDriverClassName: str
-    bulkSize: int
-    hashfield: str
-    hashexpression: str
-    hashpartitions: int
-    sampleQuery: str
-    enablePartitioningForSampleQuery: bool
-    sampleSize: int
-    jobBookmarkKeys: list[str]
-    jobBookmarkKeysSortOrder: Literal["asc", "desc"]
+    from glue_utils.pyspark.connection_options import (
+        JDBCConnectionOptions,
+        RedshiftJDBCConnectionOptions,
+    )
 
 
 class SQLServerMixin:
     """Mixin for working with SQL Server connections."""
 
     def create_dynamic_frame_from_sqlserver(
         self: GlueContext,
@@ -274,9 +250,75 @@
             frame=frame,
             connection_type=ConnectionType.POSTGRESQL.value,
             connection_options=connection_options,
             transformation_ctx=transformation_ctx,
         )
 
 
-class JDBCMixin(MySQLMixin, OracleMixin, PostgreSQLMixin, SQLServerMixin):
+class RedshiftSQLMixin:
+    """Mixin for working with Redshift connections."""
+
+    def create_dynamic_frame_from_redshift(
+        self: GlueContext,
+        connection_options: RedshiftJDBCConnectionOptions,
+        transformation_ctx: str = "",
+    ) -> DynamicFrame:
+        """Create a DynamicFrame from a Redshift database connection.
+
+        Parameters
+        ----------
+        connection_options : RedshiftJDBCConnectionOptions
+            The connection options for the Redshift database.
+        transformation_ctx : str, optional
+            The transformation context for the DynamicFrame. Defaults to "".
+
+        Returns
+        -------
+        DynamicFrame
+            The DynamicFrame created from the Redshift database.
+
+        """
+        return self.create_dynamic_frame_from_options(
+            connection_type=ConnectionType.REDSHIFT.value,
+            connection_options=connection_options,
+            transformation_ctx=transformation_ctx,
+        )
+
+    def write_dynamic_frame_to_redshift(
+        self: GlueContext,
+        frame: DynamicFrame,
+        connection_options: RedshiftJDBCConnectionOptions,
+        transformation_ctx: str = "",
+    ) -> DynamicFrame:
+        """Write a DynamicFrame to a Redshift database.
+
+        Parameters
+        ----------
+        frame : DynamicFrame
+            The DynamicFrame to write to the database.
+        connection_options : RedshiftJDBCConnectionOptions
+            The JDBC connection options for the database.
+        transformation_ctx : str, optional
+            The transformation context. Defaults to "".
+
+        Returns
+        -------
+        DynamicFrame
+            The DynamicFrame that was written to the database.
+
+        """
+        return self.write_dynamic_frame_from_options(
+            frame=frame,
+            connection_type=ConnectionType.REDSHIFT.value,
+            connection_options=connection_options,
+            transformation_ctx=transformation_ctx,
+        )
+
+
+class JDBCMixin(
+    MySQLMixin,
+    OracleMixin,
+    PostgreSQLMixin,
+    RedshiftSQLMixin,
+    SQLServerMixin,
+):
     """Mixin for working with JDBC connections."""
```

