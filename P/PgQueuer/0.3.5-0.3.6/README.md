# Comparing `tmp/pgqueuer-0.3.5.tar.gz` & `tmp/pgqueuer-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgqueuer-0.3.5.tar", last modified: Sat May 11 14:41:23 2024, max compression
+gzip compressed data, was "pgqueuer-0.3.6.tar", last modified: Mon May 20 20:52:45 2024, max compression
```

## Comparing `pgqueuer-0.3.5.tar` & `pgqueuer-0.3.6.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:41:23.566411 pgqueuer-0.3.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:41:23.558411 pgqueuer-0.3.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:41:23.558411 pgqueuer-0.3.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-11 14:41:14.000000 pgqueuer-0.3.5/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-11 14:41:14.000000 pgqueuer-0.3.5/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-11 14:41:14.000000 pgqueuer-0.3.5/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-11 14:41:14.000000 pgqueuer-0.3.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-11 14:41:14.000000 pgqueuer-0.3.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-11 14:41:14.000000 pgqueuer-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7449 2024-05-11 14:41:23.566411 pgqueuer-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5803 2024-05-11 14:41:14.000000 pgqueuer-0.3.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-11 14:41:14.000000 pgqueuer-0.3.5/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-11 14:41:14.000000 pgqueuer-0.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 14:41:23.566411 pgqueuer-0.3.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:41:23.558411 pgqueuer-0.3.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:41:23.562411 pgqueuer-0.3.5/src/PgQueuer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 14:41:14.000000 pgqueuer-0.3.5/src/PgQueuer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-11 14:41:14.000000 pgqueuer-0.3.5/src/PgQueuer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-11 14:41:14.000000 pgqueuer-0.3.5/src/PgQueuer/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6575 2024-05-11 14:41:14.000000 pgqueuer-0.3.5/src/PgQueuer/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-11 14:41:14.000000 pgqueuer-0.3.5/src/PgQueuer/listeners.py
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-11 14:41:14.000000 pgqueuer-0.3.5/src/PgQueuer/logconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-11 14:41:14.000000 pgqueuer-0.3.5/src/PgQueuer/models.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 14:41:14.000000 pgqueuer-0.3.5/src/PgQueuer/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5466 2024-05-11 14:41:14.000000 pgqueuer-0.3.5/src/PgQueuer/qm.py
--rw-r--r--   0 runner    (1001) docker     (127)    16242 2024-05-11 14:41:14.000000 pgqueuer-0.3.5/src/PgQueuer/queries.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-11 14:41:14.000000 pgqueuer-0.3.5/src/PgQueuer/tm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:41:23.566411 pgqueuer-0.3.5/src/PgQueuer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7449 2024-05-11 14:41:23.000000 pgqueuer-0.3.5/src/PgQueuer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-11 14:41:23.000000 pgqueuer-0.3.5/src/PgQueuer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 14:41:23.000000 pgqueuer-0.3.5/src/PgQueuer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-11 14:41:23.000000 pgqueuer-0.3.5/src/PgQueuer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-11 14:41:23.000000 pgqueuer-0.3.5/src/PgQueuer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-11 14:41:23.000000 pgqueuer-0.3.5/src/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:41:23.562411 pgqueuer-0.3.5/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-11 14:41:14.000000 pgqueuer-0.3.5/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:41:23.562411 pgqueuer-0.3.5/test/db/
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-11 14:41:14.000000 pgqueuer-0.3.5/test/db/Dockerfile
--rwxr-xr-x   0 runner    (1001) docker     (127)      266 2024-05-11 14:41:14.000000 pgqueuer-0.3.5/test/db/init_db.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-11 14:41:14.000000 pgqueuer-0.3.5/test/test_qm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-05-11 14:41:14.000000 pgqueuer-0.3.5/test/test_queries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-11 14:41:14.000000 pgqueuer-0.3.5/test/test_tm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:41:23.562411 pgqueuer-0.3.5/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-11 14:41:14.000000 pgqueuer-0.3.5/tools/benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:52:45.159635 pgqueuer-0.3.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:52:45.151635 pgqueuer-0.3.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:52:45.155635 pgqueuer-0.3.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-20 20:52:36.000000 pgqueuer-0.3.6/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-20 20:52:36.000000 pgqueuer-0.3.6/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-20 20:52:36.000000 pgqueuer-0.3.6/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-20 20:52:36.000000 pgqueuer-0.3.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-20 20:52:36.000000 pgqueuer-0.3.6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-20 20:52:36.000000 pgqueuer-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10199 2024-05-20 20:52:45.159635 pgqueuer-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8553 2024-05-20 20:52:36.000000 pgqueuer-0.3.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-20 20:52:36.000000 pgqueuer-0.3.6/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-20 20:52:36.000000 pgqueuer-0.3.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 20:52:45.159635 pgqueuer-0.3.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:52:45.155635 pgqueuer-0.3.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:52:45.155635 pgqueuer-0.3.6/src/PgQueuer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 20:52:36.000000 pgqueuer-0.3.6/src/PgQueuer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-20 20:52:36.000000 pgqueuer-0.3.6/src/PgQueuer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-20 20:52:36.000000 pgqueuer-0.3.6/src/PgQueuer/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7504 2024-05-20 20:52:36.000000 pgqueuer-0.3.6/src/PgQueuer/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-20 20:52:36.000000 pgqueuer-0.3.6/src/PgQueuer/listeners.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-20 20:52:36.000000 pgqueuer-0.3.6/src/PgQueuer/logconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-20 20:52:36.000000 pgqueuer-0.3.6/src/PgQueuer/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 20:52:36.000000 pgqueuer-0.3.6/src/PgQueuer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-05-20 20:52:36.000000 pgqueuer-0.3.6/src/PgQueuer/qm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16506 2024-05-20 20:52:36.000000 pgqueuer-0.3.6/src/PgQueuer/queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-20 20:52:36.000000 pgqueuer-0.3.6/src/PgQueuer/tm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:52:45.159635 pgqueuer-0.3.6/src/PgQueuer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10199 2024-05-20 20:52:45.000000 pgqueuer-0.3.6/src/PgQueuer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-20 20:52:45.000000 pgqueuer-0.3.6/src/PgQueuer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 20:52:45.000000 pgqueuer-0.3.6/src/PgQueuer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-20 20:52:45.000000 pgqueuer-0.3.6/src/PgQueuer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-20 20:52:45.000000 pgqueuer-0.3.6/src/PgQueuer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-20 20:52:45.000000 pgqueuer-0.3.6/src/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:52:45.159635 pgqueuer-0.3.6/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-20 20:52:36.000000 pgqueuer-0.3.6/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:52:45.159635 pgqueuer-0.3.6/test/db/
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-20 20:52:36.000000 pgqueuer-0.3.6/test/db/Dockerfile
+-rwxr-xr-x   0 runner    (1001) docker     (127)      266 2024-05-20 20:52:36.000000 pgqueuer-0.3.6/test/db/init_db.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-05-20 20:52:36.000000 pgqueuer-0.3.6/test/test_qm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-05-20 20:52:36.000000 pgqueuer-0.3.6/test/test_queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-20 20:52:36.000000 pgqueuer-0.3.6/test/test_tm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:52:45.159635 pgqueuer-0.3.6/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-05-20 20:52:36.000000 pgqueuer-0.3.6/tools/benchmark.py
```

### Comparing `pgqueuer-0.3.5/.github/workflows/ci.yml` & `pgqueuer-0.3.6/.github/workflows/ci.yml`

 * *Files 12% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         run: |
           pip install pip -U
           pip install .[dev]
 
       - name: Benchmark
         run: PGUSER=testuser PGPASSWORD=testpassword PGDATABASE=testdb python3 tools/benchmark.py
 
-  ci:
+  test-pgqueuer:
     strategy:
       fail-fast: false
       matrix:
         python-version: ["3.10", "3.11", "3.12"]
         os: [ubuntu-latest]
 
     name: PY ${{ matrix.python-version }} on ${{ matrix.os }} 
@@ -63,15 +63,7 @@
       - name: Install PgQueuer
         run: |
           pip install pip -U
           pip install .[dev]
 
       - name: Full test
         run: pytest -v
-
-  check-all-ci-passed:
-    name: Check test matrix passed.
-    needs: ci
-    runs-on: ubuntu-latest
-    steps:
-      - name: Check status
-        run: echo "All tests passed; ready to merge."
```

### Comparing `pgqueuer-0.3.5/.github/workflows/linting.yml` & `pgqueuer-0.3.6/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.5/.github/workflows/release.yml` & `pgqueuer-0.3.6/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.5/.gitignore` & `pgqueuer-0.3.6/.gitignore`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.5/CONTRIBUTING.md` & `pgqueuer-0.3.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.5/LICENSE` & `pgqueuer-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.5/pyproject.toml` & `pgqueuer-0.3.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.5/src/PgQueuer/cli.py` & `pgqueuer-0.3.6/src/PgQueuer/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 import asyncio
 import os
 from datetime import timedelta
 
 import asyncpg
 from tabulate import tabulate, tabulate_formats
 
-from PgQueuer.models import LogStatistics
-from PgQueuer.queries import Queries, QueryBuilder
+from PgQueuer.listeners import initialize_event_listener
+from PgQueuer.models import LogStatistics, PGChannel
+from PgQueuer.queries import DBSettings, Queries, QueryBuilder
 
 
 async def display_stats(
     log_stats: list[LogStatistics],
     tablefmt: str,
 ) -> None:
     print(
@@ -38,14 +39,27 @@
                 "Priority",
             ],
             tablefmt=tablefmt,
         )
     )
 
 
+async def display_pg_channel(
+    pool: asyncpg.Pool,
+    channel: PGChannel,
+) -> None:
+    async with pool.acquire() as connection:
+        listener = await initialize_event_listener(
+            connection,  # type: ignore[arg-type]
+            channel,
+        )
+        while True:
+            print(repr(await listener.get()))
+
+
 async def fetch_and_display(
     queries: Queries,
     interval: timedelta | None,
     tail: int,
     tablefmt: str,
 ) -> None:
     clear_and_home = "\033[2J\033[H"
@@ -190,14 +204,25 @@
         help=(
             "Specify the format of the table used to display statistics. "
             "Options are provided by the tabulate library."
         ),
         choices=tabulate_formats,
     )
 
+    listen_parser = subparsers.add_parser(
+        "listen",
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
+        parents=[common_arguments],
+    )
+    listen_parser.add_argument(
+        "--channel",
+        help="Specifies the PostgreSQL NOTIFY channel to listen on for debug purposes.",
+        default=DBSettings().channel,
+    )
+
     return parser.parse_args()
 
 
 async def main() -> None:
     parsed = cliparser()
 
     if (
@@ -230,7 +255,12 @@
             case "dashboard":
                 await fetch_and_display(
                     queries,
                     parsed.interval,
                     parsed.tail,
                     parsed.table_format,
                 )
+            case "listen":
+                await display_pg_channel(
+                    pool,
+                    PGChannel(parsed.channel),
+                )
```

### Comparing `pgqueuer-0.3.5/src/PgQueuer/listeners.py` & `pgqueuer-0.3.6/src/PgQueuer/listeners.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.5/src/PgQueuer/models.py` & `pgqueuer-0.3.6/src/PgQueuer/models.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.5/src/PgQueuer/qm.py` & `pgqueuer-0.3.6/src/PgQueuer/qm.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,16 +65,17 @@
 class QueueManager:
     """
     Manages job queues and dispatches jobs to registered entry points,
     handling database connections and events.
     """
 
     pool: asyncpg.Pool
-    queries: Queries = dataclasses.field(init=False)
     channel: PGChannel = dataclasses.field(default=PGChannel(DBSettings().channel))
+
+    queries: Queries = dataclasses.field(init=False)
     alive: bool = dataclasses.field(init=False, default=True)
 
     # Should registry be a weakref?
     registry: dict[str, Entrypoint] = dataclasses.field(
         init=False, default_factory=dict
     )
 
@@ -104,39 +105,46 @@
             return func
 
         return register
 
     async def run(
         self,
         dequeue_timeout: timedelta = timedelta(seconds=30),
+        batch_size: int = 10,
     ) -> None:
         """
         Continuously listens for events and dispatches jobs. Manages connections and
         tasks, logs timeouts, and resets connections upon termination.
         """
         async with (
             self.pool.acquire() as connection,
             TaskManager() as tm,
         ):
             listener = await initialize_event_listener(connection, self.channel)  # type: ignore[arg-type]
 
             while self.alive:
-                while self.alive and (job := await self.queries.dequeue()):
-                    tm.add(asyncio.create_task(self._dispatch(job)))
-
-                try:
-                    await asyncio.wait_for(
-                        listener.get(),
-                        timeout=dequeue_timeout.total_seconds(),
-                    )
-                except asyncio.TimeoutError:
-                    logger.debug(
-                        "Timeout after %r without receiving an event.",
-                        dequeue_timeout,
+                while self.alive and (
+                    jobs := await self.queries.dequeue(
+                        batch_size=batch_size,
+                        entrypoints=set(self.registry.keys()),
                     )
+                ):
+                    for job in jobs:
+                        tm.add(asyncio.create_task(self._dispatch(job)))
+
+                    try:
+                        await asyncio.wait_for(
+                            listener.get(),
+                            timeout=dequeue_timeout.total_seconds(),
+                        )
+                    except asyncio.TimeoutError:
+                        logger.debug(
+                            "Timeout after %r without receiving an event.",
+                            dequeue_timeout,
+                        )
 
             connection.remove_termination_listener(_critical_termination_listener)
             await connection.reset()
 
     async def _dispatch(self, job: Job) -> None:
         """
         Handles asynchronous job dispatch. Logs exceptions, updates job status,
```

### Comparing `pgqueuer-0.3.5/src/PgQueuer/queries.py` & `pgqueuer-0.3.6/src/PgQueuer/queries.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,23 +195,26 @@
         This query sets the job status to 'queued' and includes parameters for priority,
         entrypoint, and payload.
         """
         return f"""
     WITH next_job AS (
         SELECT id
         FROM {self.settings.queue_table}
-        WHERE status = 'queued'
+        WHERE status = 'queued' AND entrypoint = ANY($2)
         ORDER BY priority DESC, id ASC
         FOR UPDATE SKIP LOCKED
-        LIMIT 1
+        LIMIT $1
+    ),
+    updated AS (
+        UPDATE {self.settings.queue_table}
+        SET status = 'picked'
+        WHERE id = ANY(SELECT id FROM next_job)
+        RETURNING *
     )
-    UPDATE {self.settings.queue_table}
-    SET status = 'picked'
-    WHERE id = ANY(SELECT id FROM next_job)
-    RETURNING *;
+    SELECT * FROM updated ORDER BY priority DESC, id ASC
     """
 
     def create_enqueue_query(self) -> str:
         """
         Generates the SQL query string to insert a new job into the queue.
         This query sets the job status to 'queued' and includes parameters for priority,
         entrypoint, and payload.
@@ -330,18 +333,15 @@
         count,
         created,
         time_in_queue,
         entrypoint,
         priority,
         status
     FROM {self.settings.statistics_table}
-    ORDER BY (
-        id, created, count, time_in_queue,
-        entrypoint, priority, status
-    ) DESC
+    ORDER BY id DESC
     LIMIT $1
     """
 
 
 @dataclasses.dataclass
 class Queries:
     """
@@ -363,24 +363,33 @@
     async def uninstall(self) -> None:
         """
         Drops all database structures related to job queuing
         and logging that were created by the install method.
         """
         await self.pool.execute(self.qb.create_uninstall_query())
 
-    async def dequeue(self) -> models.Job | None:
+    async def dequeue(
+        self,
+        batch_size: int,
+        entrypoints: set[str],
+    ) -> list[models.Job]:
         """
         Retrieves and updates the next 'queued' job to 'picked'
         status, ensuring no two jobs with the same entrypoint
         are picked simultaneously.
         """
+        if batch_size < 1:
+            raise ValueError("Batch size must be greter then one (1)")
 
-        if row := await self.pool.fetchrow(self.qb.create_dequeue_query()):
-            return models.Job.model_validate(dict(row))
-        return None
+        rows = await self.pool.fetch(
+            self.qb.create_dequeue_query(),
+            batch_size,
+            entrypoints,
+        )
+        return [models.Job.model_validate(dict(row)) for row in rows]
 
     async def enqueue(
         self,
         entrypoint: str | list[str],
         payload: bytes | None | list[bytes] | list[None] | list[bytes | None],
         priority: int | list[int] = 0,
     ) -> None:
```

### Comparing `pgqueuer-0.3.5/src/PgQueuer/tm.py` & `pgqueuer-0.3.6/src/PgQueuer/tm.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.5/src/PgQueuer.egg-info/SOURCES.txt` & `pgqueuer-0.3.6/src/PgQueuer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.5/test/conftest.py` & `pgqueuer-0.3.6/test/conftest.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.5/test/db/Dockerfile` & `pgqueuer-0.3.6/test/db/Dockerfile`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.5/test/test_qm.py` & `pgqueuer-0.3.6/test/test_qm.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import asyncio
 import time
+from contextlib import suppress
 
 import asyncpg
 import pytest
 from PgQueuer.models import Job
 from PgQueuer.qm import QueueManager
 from PgQueuer.queries import Queries
 
@@ -108,7 +109,43 @@
     await q.enqueue("fetch", None)
 
     await asyncio.wait_for(
         asyncio.gather(*[qm.run() for qm in qmpool]),
         timeout=10,
     )
     assert sorted(seen) == list(range(N))
+
+
+async def test_pick_local_entrypoints(
+    pgpool: asyncpg.Pool,
+) -> None:
+    q = Queries(pgpool)
+    qm = QueueManager(pgpool)
+
+    @qm.entrypoint("to_be_picked")
+    async def to_be_picked(job: Job) -> None:
+        if job.payload is None:
+            qm.alive = False
+
+    N = 100
+    await q.enqueue(
+        ["to_be_picked"] * N,
+        [f"{n}".encode() for n in range(N)],
+        [0] * N,
+    )
+
+    await q.enqueue(
+        ["not_picked"] * N,
+        [f"{n}".encode() for n in range(N)],
+        [0] * N,
+    )
+
+    with suppress(asyncio.TimeoutError):
+        await asyncio.wait_for(qm.run(), timeout=2)
+
+    assert (
+        sum(s.count for s in await q.queue_size() if s.entrypoint == "to_be_picked")
+        == 0
+    )
+    assert (
+        sum(s.count for s in await q.queue_size() if s.entrypoint == "not_picked") == N
+    )
```

### Comparing `pgqueuer-0.3.5/test/test_queries.py` & `pgqueuer-0.3.6/test/test_queries.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 @pytest.mark.parametrize("N", (1, 2, 64))
 async def test_queries_put(pgpool: asyncpg.Pool, N: int) -> None:
     q = queries.Queries(pgpool)
 
     assert sum(x.count for x in await q.queue_size()) == 0
 
     for _ in range(N):
-        await q.enqueue("placeholer", None)
+        await q.enqueue("placeholder", None)
 
     assert sum(x.count for x in await q.queue_size()) == N
 
 
 @pytest.mark.parametrize("N", (1, 2, 64))
 async def test_queries_next_jobs(
     pgpool: asyncpg.Pool,
@@ -27,19 +27,20 @@
     await q.enqueue(
         ["placeholder"] * N,
         [f"{n}".encode() for n in range(N)],
         [0] * N,
     )
 
     seen = list[int]()
-    while job := await q.dequeue():
-        payoad = job.payload
-        assert payoad is not None
-        seen.append(int(payoad))
-        await q.log_job(job, "successful")
+    while jobs := await q.dequeue(entrypoints={"placeholder"}, batch_size=10):
+        for job in jobs:
+            payoad = job.payload
+            assert payoad is not None
+            seen.append(int(payoad))
+            await q.log_job(job, "successful")
 
     assert seen == list(range(N))
 
 
 @pytest.mark.parametrize("N", (1, 2, 64))
 @pytest.mark.parametrize("concurrency", (1, 2, 4, 16))
 async def test_queries_next_jobs_concurrent(
@@ -55,100 +56,108 @@
         [f"{n}".encode() for n in range(N)],
         [0] * N,
     )
 
     seen = list[int]()
 
     async def consumer() -> None:
-        while job := await q.dequeue():
-            payload = job.payload
-            assert payload is not None
-            seen.append(int(payload))
-            await q.log_job(job, "successful")
+        while jobs := await q.dequeue(
+            entrypoints={"placeholder"},
+            batch_size=10,
+        ):
+            for job in jobs:
+                payload = job.payload
+                assert payload is not None
+                seen.append(int(payload))
+                await q.log_job(job, "successful")
 
     await asyncio.wait_for(
         asyncio.gather(*[consumer() for _ in range(concurrency)]),
         10,
     )
 
     assert sorted(seen) == list(range(N))
 
 
 async def test_queries_clear(pgpool: asyncpg.Pool) -> None:
     q = queries.Queries(pgpool)
     await q.clear_queue()
     assert sum(x.count for x in await q.queue_size()) == 0
 
-    await q.enqueue("placeholer", None)
+    await q.enqueue("placeholder", None)
     assert sum(x.count for x in await q.queue_size()) == 1
 
     await q.clear_queue()
     assert sum(x.count for x in await q.queue_size()) == 0
 
 
 @pytest.mark.parametrize("N", (1, 2, 64))
 async def test_move_job_log(
     pgpool: asyncpg.Pool,
     N: int,
 ) -> None:
     q = queries.Queries(pgpool)
 
     await q.enqueue(
-        ["placeholer"] * N,
+        ["placeholder"] * N,
         [f"{n}".encode() for n in range(N)],
         [0] * N,
     )
 
-    while job := await q.dequeue():
-        await q.log_job(job, status="successful")
+    while jobs := await q.dequeue(
+        entrypoints={"placeholder"},
+        batch_size=10,
+    ):
+        for job in jobs:
+            await q.log_job(job, status="successful")
 
     assert sum(x.count for x in await q.log_statistics(1_000_000_000)) == N
 
 
 @pytest.mark.parametrize("N", (1, 2, 5))
 async def test_clear_queue(
     pgpool: asyncpg.Pool,
     N: int,
 ) -> None:
     q = queries.Queries(pgpool)
 
     # Test delete all by listing all
     await q.enqueue(
-        [f"placeholer{n}" for n in range(N)],
+        [f"placeholder{n}" for n in range(N)],
         [None] * N,
         [0] * N,
     )
 
     assert all(x.count == 1 for x in await q.queue_size())
     assert sum(x.count for x in await q.queue_size()) == N
-    await q.clear_queue([f"placeholer{n}" for n in range(N)])
+    await q.clear_queue([f"placeholder{n}" for n in range(N)])
     assert sum(x.count for x in await q.queue_size()) == 0
 
     # Test delete all by None
     await q.enqueue(
-        [f"placeholer{n}" for n in range(N)],
+        [f"placeholder{n}" for n in range(N)],
         [None] * N,
         [0] * N,
     )
 
     assert all(x.count == 1 for x in await q.queue_size())
     assert sum(x.count for x in await q.queue_size()) == N
     await q.clear_queue(None)
     assert sum(x.count for x in await q.queue_size()) == 0
 
     # Test delete one(1).
     await q.enqueue(
-        [f"placeholer{n}" for n in range(N)],
+        [f"placeholder{n}" for n in range(N)],
         [None] * N,
         [0] * N,
     )
 
     assert all(x.count == 1 for x in await q.queue_size())
     assert sum(x.count for x in await q.queue_size()) == N
-    await q.clear_queue("placeholer0")
+    await q.clear_queue("placeholder0")
     assert sum(x.count for x in await q.queue_size()) == N - 1
 
 
 @pytest.mark.parametrize("N", (1, 2, 64))
 async def test_queue_priority(
     pgpool: asyncpg.Pool,
     N: int,
@@ -158,12 +167,16 @@
 
     await q.enqueue(
         ["placeholder"] * N,
         [f"{n}".encode() for n in range(N)],
         list(range(N)),
     )
 
-    while next_job := await q.dequeue():
-        jobs.append(next_job)
-        await q.log_job(next_job, status="successful")
+    while next_jobs := await q.dequeue(
+        entrypoints={"placeholder"},
+        batch_size=10,
+    ):
+        for job in next_jobs:
+            jobs.append(job)
+            await q.log_job(job, status="successful")
 
     assert jobs == sorted(jobs, key=lambda x: x.priority, reverse=True)
```

### Comparing `pgqueuer-0.3.5/test/test_tm.py` & `pgqueuer-0.3.6/test/test_tm.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import asyncio
 
 import pytest
-from PgQueuer import qm
+from PgQueuer.tm import TaskManager
 
 
 @pytest.mark.parametrize("N", (1, 2, 3, 5, 64))
 async def test_task_manager(N: int) -> None:
     future = asyncio.Future[None]()
 
-    tm = qm.TaskManager()
+    tm = TaskManager()
     assert len(tm.tasks) == 0
 
     async def waiter(future: asyncio.Future) -> None:
         return await future
 
     for _ in range(N):
         tm.add(asyncio.create_task(waiter(future)))
@@ -27,15 +27,15 @@
 @pytest.mark.parametrize("N", (1, 2, 3, 5, 64))
 async def test_task_manager_ctx_mngr(N: int) -> None:
     async def waiter(future: asyncio.Future) -> None:
         return await future
 
     future = asyncio.Future[None]()
 
-    async with qm.TaskManager() as tm:
+    async with TaskManager() as tm:
         assert len(tm.tasks) == 0
 
         for _ in range(N):
             tm.add(asyncio.create_task(waiter(future)))
 
         assert len(tm.tasks) == N
```

