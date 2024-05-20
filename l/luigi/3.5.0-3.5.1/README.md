# Comparing `tmp/luigi-3.5.0.tar.gz` & `tmp/luigi-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luigi-3.5.0.tar", last modified: Mon Jan 15 15:27:05 2024, max compression
+gzip compressed data, was "luigi-3.5.1.tar", last modified: Mon May 20 08:19:10 2024, max compression
```

## Comparing `luigi-3.5.0.tar` & `luigi-3.5.1.tar`

### file list

```diff
@@ -1,316 +1,316 @@
-drwxr-xr-x   0 pabloc     (501) staff       (20)        0 2024-01-15 15:27:05.444049 luigi-3.5.0/
--rw-r--r--   0 pabloc     (501) staff       (20)    11345 2024-01-04 16:31:55.000000 luigi-3.5.0/LICENSE
--rw-r--r--   0 pabloc     (501) staff       (20)      140 2024-01-04 16:31:55.000000 luigi-3.5.0/MANIFEST.in
--rw-r--r--   0 pabloc     (501) staff       (20)    14096 2024-01-15 15:27:05.443695 luigi-3.5.0/PKG-INFO
--rw-r--r--   0 pabloc     (501) staff       (20)    12959 2024-01-15 15:17:29.000000 luigi-3.5.0/README.rst
-drwxr-xr-x   0 pabloc     (501) staff       (20)        0 2024-01-15 15:27:05.326736 luigi-3.5.0/examples/
--rw-r--r--   0 pabloc     (501) staff       (20)      603 2024-01-04 16:31:55.000000 luigi-3.5.0/examples/__init__.py
--rw-r--r--   0 pabloc     (501) staff       (20)     3746 2024-01-04 16:31:55.000000 luigi-3.5.0/examples/dynamic_requirements.py
--rw-r--r--   0 pabloc     (501) staff       (20)     3410 2024-01-04 16:31:55.000000 luigi-3.5.0/examples/elasticsearch_index.py
--rw-r--r--   0 pabloc     (501) staff       (20)     3319 2024-01-04 16:31:55.000000 luigi-3.5.0/examples/execution_summary_example.py
--rw-r--r--   0 pabloc     (501) staff       (20)     1462 2024-01-04 16:31:55.000000 luigi-3.5.0/examples/foo.py
--rw-r--r--   0 pabloc     (501) staff       (20)     1876 2024-01-04 16:31:55.000000 luigi-3.5.0/examples/foo_complex.py
--rw-r--r--   0 pabloc     (501) staff       (20)     3239 2024-01-04 16:31:55.000000 luigi-3.5.0/examples/ftp_experiment_outputs.py
--rw-r--r--   0 pabloc     (501) staff       (20)      500 2024-01-04 16:31:55.000000 luigi-3.5.0/examples/hello_world.py
--rw-r--r--   0 pabloc     (501) staff       (20)     1986 2024-01-04 16:31:55.000000 luigi-3.5.0/examples/kubernetes.py
--rw-r--r--   0 pabloc     (501) staff       (20)     5264 2024-01-04 16:31:55.000000 luigi-3.5.0/examples/per_task_retry_policy.py
--rw-r--r--   0 pabloc     (501) staff       (20)     3388 2024-01-04 16:31:55.000000 luigi-3.5.0/examples/pyspark_wc.py
--rw-r--r--   0 pabloc     (501) staff       (20)     4363 2024-01-04 16:31:55.000000 luigi-3.5.0/examples/spark_als.py
--rw-r--r--   0 pabloc     (501) staff       (20)     2823 2024-01-04 16:31:55.000000 luigi-3.5.0/examples/ssh_remote_execution.py
--rw-r--r--   0 pabloc     (501) staff       (20)     3400 2024-01-04 16:31:55.000000 luigi-3.5.0/examples/terasort.py
--rwxr-xr-x   0 pabloc     (501) staff       (20)     9069 2024-01-04 16:31:55.000000 luigi-3.5.0/examples/top_artists.py
--rwxr-xr-x   0 pabloc     (501) staff       (20)      645 2024-01-04 16:31:55.000000 luigi-3.5.0/examples/top_artists_spark.py
--rw-r--r--   0 pabloc     (501) staff       (20)     2904 2024-01-04 16:31:55.000000 luigi-3.5.0/examples/wordcount.py
--rw-r--r--   0 pabloc     (501) staff       (20)     2729 2024-01-04 16:31:55.000000 luigi-3.5.0/examples/wordcount_hadoop.py
-drwxr-xr-x   0 pabloc     (501) staff       (20)        0 2024-01-15 15:27:05.336886 luigi-3.5.0/luigi/
--rw-r--r--   0 pabloc     (501) staff       (20)     3723 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/__init__.py
--rw-r--r--   0 pabloc     (501) staff       (20)      683 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/__main__.py
--rw-r--r--   0 pabloc     (501) staff       (20)      249 2024-01-15 15:26:51.000000 luigi-3.5.0/luigi/__meta__.py
--rw-r--r--   0 pabloc     (501) staff       (20)     8863 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/batch_notifier.py
--rw-r--r--   0 pabloc     (501) staff       (20)     1426 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/cmdline.py
--rw-r--r--   0 pabloc     (501) staff       (20)     5458 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/cmdline_parser.py
-drwxr-xr-x   0 pabloc     (501) staff       (20)        0 2024-01-15 15:27:05.339150 luigi-3.5.0/luigi/configuration/
--rw-r--r--   0 pabloc     (501) staff       (20)      837 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/configuration/__init__.py
--rw-r--r--   0 pabloc     (501) staff       (20)     1307 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/configuration/base_parser.py
--rw-r--r--   0 pabloc     (501) staff       (20)     8424 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/configuration/cfg_parser.py
--rw-r--r--   0 pabloc     (501) staff       (20)     2760 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/configuration/core.py
--rw-r--r--   0 pabloc     (501) staff       (20)     2831 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/configuration/toml_parser.py
-drwxr-xr-x   0 pabloc     (501) staff       (20)        0 2024-01-15 15:27:05.356877 luigi-3.5.0/luigi/contrib/
--rw-r--r--   0 pabloc     (501) staff       (20)      661 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/__init__.py
--rw-r--r--   0 pabloc     (501) staff       (20)    13302 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/azureblob.py
--rw-r--r--   0 pabloc     (501) staff       (20)     7990 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/batch.py
--rw-r--r--   0 pabloc     (501) staff       (20)    16573 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/beam_dataflow.py
--rw-r--r--   0 pabloc     (501) staff       (20)    30813 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/bigquery.py
--rw-r--r--   0 pabloc     (501) staff       (20)     4347 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/bigquery_avro.py
--rw-r--r--   0 pabloc     (501) staff       (20)     5730 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/datadog_metric.py
--rw-r--r--   0 pabloc     (501) staff       (20)    10231 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/dataproc.py
--rw-r--r--   0 pabloc     (501) staff       (20)     9524 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/docker_runner.py
--rw-r--r--   0 pabloc     (501) staff       (20)    11346 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/dropbox.py
--rw-r--r--   0 pabloc     (501) staff       (20)     9599 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/ecs.py
--rw-r--r--   0 pabloc     (501) staff       (20)    14188 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/esindex.py
--rw-r--r--   0 pabloc     (501) staff       (20)     2330 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/external_daily_snapshot.py
--rw-r--r--   0 pabloc     (501) staff       (20)    11285 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/external_program.py
--rw-r--r--   0 pabloc     (501) staff       (20)    13354 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/ftp.py
--rw-r--r--   0 pabloc     (501) staff       (20)     1498 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/gcp.py
--rw-r--r--   0 pabloc     (501) staff       (20)    18537 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/gcs.py
--rw-r--r--   0 pabloc     (501) staff       (20)    37546 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/hadoop.py
--rw-r--r--   0 pabloc     (501) staff       (20)     5524 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/hadoop_jar.py
-drwxr-xr-x   0 pabloc     (501) staff       (20)        0 2024-01-15 15:27:05.359660 luigi-3.5.0/luigi/contrib/hdfs/
--rw-r--r--   0 pabloc     (501) staff       (20)     2901 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/hdfs/__init__.py
--rw-r--r--   0 pabloc     (501) staff       (20)     2839 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/hdfs/abstract_client.py
--rw-r--r--   0 pabloc     (501) staff       (20)     1922 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/hdfs/clients.py
--rw-r--r--   0 pabloc     (501) staff       (20)     4138 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/hdfs/config.py
--rw-r--r--   0 pabloc     (501) staff       (20)     1120 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/hdfs/error.py
--rw-r--r--   0 pabloc     (501) staff       (20)     6019 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/hdfs/format.py
--rw-r--r--   0 pabloc     (501) staff       (20)     9572 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/hdfs/hadoopcli_clients.py
--rw-r--r--   0 pabloc     (501) staff       (20)     7327 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/hdfs/target.py
--rw-r--r--   0 pabloc     (501) staff       (20)     6721 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/hdfs/webhdfs_client.py
--rw-r--r--   0 pabloc     (501) staff       (20)    19543 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/hive.py
--rw-r--r--   0 pabloc     (501) staff       (20)    14284 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/kubernetes.py
--rwxr-xr-x   0 pabloc     (501) staff       (20)    12181 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/lsf.py
--rwxr-xr-x   0 pabloc     (501) staff       (20)     2297 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/lsf_runner.py
--rw-r--r--   0 pabloc     (501) staff       (20)     6678 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/mongodb.py
--rw-r--r--   0 pabloc     (501) staff       (20)     2806 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/mrrunner.py
--rw-r--r--   0 pabloc     (501) staff       (20)     5538 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/mssqldb.py
--rw-r--r--   0 pabloc     (501) staff       (20)     8663 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/mysqldb.py
--rw-r--r--   0 pabloc     (501) staff       (20)     7286 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/opener.py
--rw-r--r--   0 pabloc     (501) staff       (20)    11126 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/pai.py
--rw-r--r--   0 pabloc     (501) staff       (20)     6517 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/pig.py
--rw-r--r--   0 pabloc     (501) staff       (20)    16403 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/postgres.py
--rw-r--r--   0 pabloc     (501) staff       (20)     7825 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/presto.py
--rw-r--r--   0 pabloc     (501) staff       (20)     2430 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/prometheus_metric.py
--rw-r--r--   0 pabloc     (501) staff       (20)     3897 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/pyspark_runner.py
--rw-r--r--   0 pabloc     (501) staff       (20)    11181 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/rdbms.py
--rw-r--r--   0 pabloc     (501) staff       (20)     3085 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/redis_store.py
--rw-r--r--   0 pabloc     (501) staff       (20)    25778 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/redshift.py
--rw-r--r--   0 pabloc     (501) staff       (20)    27902 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/s3.py
--rw-r--r--   0 pabloc     (501) staff       (20)    27695 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/salesforce.py
--rw-r--r--   0 pabloc     (501) staff       (20)    10682 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/scalding.py
--rwxr-xr-x   0 pabloc     (501) staff       (20)    13563 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/sge.py
--rwxr-xr-x   0 pabloc     (501) staff       (20)     2830 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/sge_runner.py
--rw-r--r--   0 pabloc     (501) staff       (20)     3406 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/simulate.py
--rw-r--r--   0 pabloc     (501) staff       (20)    12313 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/spark.py
--rw-r--r--   0 pabloc     (501) staff       (20)     1970 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/sparkey.py
--rw-r--r--   0 pabloc     (501) staff       (20)    16432 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/sqla.py
--rw-r--r--   0 pabloc     (501) staff       (20)    12356 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/ssh.py
--rw-r--r--   0 pabloc     (501) staff       (20)     2811 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/target.py
--rw-r--r--   0 pabloc     (501) staff       (20)     2974 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/contrib/webhdfs.py
--rw-r--r--   0 pabloc     (501) staff       (20)     8620 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/date_interval.py
--rw-r--r--   0 pabloc     (501) staff       (20)    11268 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/db_task_history.py
--rw-r--r--   0 pabloc     (501) staff       (20)     1758 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/event.py
--rw-r--r--   0 pabloc     (501) staff       (20)    20264 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/execution_summary.py
--rw-r--r--   0 pabloc     (501) staff       (20)    14691 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/format.py
--rw-r--r--   0 pabloc     (501) staff       (20)     2122 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/freezing.py
--rw-r--r--   0 pabloc     (501) staff       (20)     8971 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/interface.py
--rw-r--r--   0 pabloc     (501) staff       (20)     6182 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/local_target.py
--rw-r--r--   0 pabloc     (501) staff       (20)     5410 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/lock.py
--rw-r--r--   0 pabloc     (501) staff       (20)     2516 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/metrics.py
--rw-r--r--   0 pabloc     (501) staff       (20)     5663 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/mock.py
--rw-r--r--   0 pabloc     (501) staff       (20)    14535 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/notifications.py
--rw-r--r--   0 pabloc     (501) staff       (20)    53828 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/parameter.py
--rw-r--r--   0 pabloc     (501) staff       (20)     3489 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/process.py
--rw-r--r--   0 pabloc     (501) staff       (20)     4658 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/retcodes.py
--rw-r--r--   0 pabloc     (501) staff       (20)     6907 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/rpc.py
--rw-r--r--   0 pabloc     (501) staff       (20)    65995 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/scheduler.py
--rw-r--r--   0 pabloc     (501) staff       (20)    14294 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/server.py
--rw-r--r--   0 pabloc     (501) staff       (20)     5889 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/setup_logging.py
-drwxr-xr-x   0 pabloc     (501) staff       (20)        0 2024-01-15 15:27:05.317592 luigi-3.5.0/luigi/static/
-drwxr-xr-x   0 pabloc     (501) staff       (20)        0 2024-01-15 15:27:05.360506 luigi-3.5.0/luigi/static/visualiser/
-drwxr-xr-x   0 pabloc     (501) staff       (20)        0 2024-01-15 15:27:05.361420 luigi-3.5.0/luigi/static/visualiser/css/
--rw-r--r--   0 pabloc     (501) staff       (20)    23739 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/css/font-awesome.min.css
--rw-r--r--   0 pabloc     (501) staff       (20)     3413 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/css/luigi.css
--rw-r--r--   0 pabloc     (501) staff       (20)     2162 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/css/tipsy.css
-drwxr-xr-x   0 pabloc     (501) staff       (20)        0 2024-01-15 15:27:05.367048 luigi-3.5.0/luigi/static/visualiser/fonts/
--rw-r--r--   0 pabloc     (501) staff       (20)    93888 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/fonts/FontAwesome.otf
--rwxr-xr-x   0 pabloc     (501) staff       (20)    60767 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/fonts/fontawesome-webfont.eot
--rw-r--r--   0 pabloc     (501) staff       (20)   313398 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/fonts/fontawesome-webfont.svg
--rwxr-xr-x   0 pabloc     (501) staff       (20)   122092 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/fonts/fontawesome-webfont.ttf
--rwxr-xr-x   0 pabloc     (501) staff       (20)    71508 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/fonts/fontawesome-webfont.woff
--rw-r--r--   0 pabloc     (501) staff       (20)    56780 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 pabloc     (501) staff       (20)    20335 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 pabloc     (501) staff       (20)    62927 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 pabloc     (501) staff       (20)    41280 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 pabloc     (501) staff       (20)    23320 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 pabloc     (501) staff       (20)    33256 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/index.html
-drwxr-xr-x   0 pabloc     (501) staff       (20)        0 2024-01-15 15:27:05.368550 luigi-3.5.0/luigi/static/visualiser/js/
--rw-r--r--   0 pabloc     (501) staff       (20)    12091 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/js/graph.js
--rw-r--r--   0 pabloc     (501) staff       (20)     8076 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/js/luigi.js
-drwxr-xr-x   0 pabloc     (501) staff       (20)        0 2024-01-15 15:27:05.369153 luigi-3.5.0/luigi/static/visualiser/js/test/
--rw-r--r--   0 pabloc     (501) staff       (20)     3619 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/js/test/graph_test.js
--rw-r--r--   0 pabloc     (501) staff       (20)    11097 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/js/tipsy.js
--rw-r--r--   0 pabloc     (501) staff       (20)      189 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/js/util.js
--rw-r--r--   0 pabloc     (501) staff       (20)    58572 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/js/visualiserApp.js
-drwxr-xr-x   0 pabloc     (501) staff       (20)        0 2024-01-15 15:27:05.370692 luigi-3.5.0/luigi/static/visualiser/lib/
-drwxr-xr-x   0 pabloc     (501) staff       (20)        0 2024-01-15 15:27:05.318246 luigi-3.5.0/luigi/static/visualiser/lib/AdminLTE/
-drwxr-xr-x   0 pabloc     (501) staff       (20)        0 2024-01-15 15:27:05.372054 luigi-3.5.0/luigi/static/visualiser/lib/AdminLTE/css/
--rw-r--r--   0 pabloc     (501) staff       (20)    75652 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/lib/AdminLTE/css/AdminLTE.min.css
--rw-r--r--   0 pabloc     (501) staff       (20)     3800 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/lib/AdminLTE/css/skin-green-light.min.css
--rw-r--r--   0 pabloc     (501) staff       (20)     3033 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/lib/AdminLTE/css/skin-green.min.css
-drwxr-xr-x   0 pabloc     (501) staff       (20)        0 2024-01-15 15:27:05.372381 luigi-3.5.0/luigi/static/visualiser/lib/AdminLTE/js/
--rw-r--r--   0 pabloc     (501) staff       (20)     9420 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/lib/AdminLTE/js/app.min.js
-drwxr-xr-x   0 pabloc     (501) staff       (20)        0 2024-01-15 15:27:05.318405 luigi-3.5.0/luigi/static/visualiser/lib/URI/
-drwxr-xr-x   0 pabloc     (501) staff       (20)        0 2024-01-15 15:27:05.372671 luigi-3.5.0/luigi/static/visualiser/lib/URI/1.18.2/
--rw-r--r--   0 pabloc     (501) staff       (20)    62788 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/lib/URI/1.18.2/URI.js
-drwxr-xr-x   0 pabloc     (501) staff       (20)        0 2024-01-15 15:27:05.318646 luigi-3.5.0/luigi/static/visualiser/lib/bootstrap-toggle/
-drwxr-xr-x   0 pabloc     (501) staff       (20)        0 2024-01-15 15:27:05.372999 luigi-3.5.0/luigi/static/visualiser/lib/bootstrap-toggle/css/
--rwxr-xr-x   0 pabloc     (501) staff       (20)     1590 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/lib/bootstrap-toggle/css/bootstrap-toggle.min.css
-drwxr-xr-x   0 pabloc     (501) staff       (20)        0 2024-01-15 15:27:05.373222 luigi-3.5.0/luigi/static/visualiser/lib/bootstrap-toggle/js/
--rwxr-xr-x   0 pabloc     (501) staff       (20)     4129 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/lib/bootstrap-toggle/js/bootstrap-toggle.min.js
-drwxr-xr-x   0 pabloc     (501) staff       (20)        0 2024-01-15 15:27:05.318861 luigi-3.5.0/luigi/static/visualiser/lib/bootstrap3/
-drwxr-xr-x   0 pabloc     (501) staff       (20)        0 2024-01-15 15:27:05.373821 luigi-3.5.0/luigi/static/visualiser/lib/bootstrap3/css/
--rw-r--r--   0 pabloc     (501) staff       (20)    19970 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/lib/bootstrap3/css/bootstrap-theme.min.css
--rw-r--r--   0 pabloc     (501) staff       (20)   117308 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/lib/bootstrap3/css/bootstrap.min.css
-drwxr-xr-x   0 pabloc     (501) staff       (20)        0 2024-01-15 15:27:05.374557 luigi-3.5.0/luigi/static/visualiser/lib/bootstrap3/js/
--rw-r--r--   0 pabloc     (501) staff       (20)    35951 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/lib/bootstrap3/js/bootstrap.min.js
-drwxr-xr-x   0 pabloc     (501) staff       (20)        0 2024-01-15 15:27:05.375128 luigi-3.5.0/luigi/static/visualiser/lib/d3/
--rw-r--r--   0 pabloc     (501) staff       (20)   151143 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/lib/d3/d3.min.js
--rw-r--r--   0 pabloc     (501) staff       (20)   113027 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/lib/d3/dagre-d3.min.js
-drwxr-xr-x   0 pabloc     (501) staff       (20)        0 2024-01-15 15:27:05.319228 luigi-3.5.0/luigi/static/visualiser/lib/datatables/
-drwxr-xr-x   0 pabloc     (501) staff       (20)        0 2024-01-15 15:27:05.375408 luigi-3.5.0/luigi/static/visualiser/lib/datatables/css/
--rw-r--r--   0 pabloc     (501) staff       (20)    15353 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/lib/datatables/css/jquery.dataTables.min.css
-drwxr-xr-x   0 pabloc     (501) staff       (20)        0 2024-01-15 15:27:05.376891 luigi-3.5.0/luigi/static/visualiser/lib/datatables/images/
--rw-r--r--   0 pabloc     (501) staff       (20)    27490 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/lib/datatables/images/Sorting icons.psd
--rw-r--r--   0 pabloc     (501) staff       (20)      894 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/lib/datatables/images/favicon.ico
--rw-r--r--   0 pabloc     (501) staff       (20)      160 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/lib/datatables/images/sort_asc.png
--rw-r--r--   0 pabloc     (501) staff       (20)      148 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/lib/datatables/images/sort_asc_disabled.png
--rw-r--r--   0 pabloc     (501) staff       (20)      201 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/lib/datatables/images/sort_both.png
--rw-r--r--   0 pabloc     (501) staff       (20)      158 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/lib/datatables/images/sort_desc.png
--rw-r--r--   0 pabloc     (501) staff       (20)      146 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/lib/datatables/images/sort_desc_disabled.png
-drwxr-xr-x   0 pabloc     (501) staff       (20)        0 2024-01-15 15:27:05.377062 luigi-3.5.0/luigi/static/visualiser/lib/datatables/js/
--rw-r--r--   0 pabloc     (501) staff       (20)    79457 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/lib/datatables/js/jquery.dataTables.min.js
--rw-r--r--   0 pabloc     (501) staff       (20)    93026 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/lib/jquery-1.10.0.min.js
-drwxr-xr-x   0 pabloc     (501) staff       (20)        0 2024-01-15 15:27:05.319521 luigi-3.5.0/luigi/static/visualiser/lib/jquery-ui/
-drwxr-xr-x   0 pabloc     (501) staff       (20)        0 2024-01-15 15:27:05.377738 luigi-3.5.0/luigi/static/visualiser/lib/jquery-ui/css/
-drwxr-xr-x   0 pabloc     (501) staff       (20)        0 2024-01-15 15:27:05.381590 luigi-3.5.0/luigi/static/visualiser/lib/jquery-ui/css/images/
--rwxr-xr-x   0 pabloc     (501) staff       (20)     1738 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/lib/jquery-ui/css/images/animated-overlay.gif
--rwxr-xr-x   0 pabloc     (501) staff       (20)      212 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/lib/jquery-ui/css/images/ui-bg_flat_0_aaaaaa_40x100.png
--rwxr-xr-x   0 pabloc     (501) staff       (20)      208 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/lib/jquery-ui/css/images/ui-bg_flat_75_ffffff_40x100.png
--rwxr-xr-x   0 pabloc     (501) staff       (20)      335 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/lib/jquery-ui/css/images/ui-bg_glass_55_fbf9ee_1x400.png
--rwxr-xr-x   0 pabloc     (501) staff       (20)      207 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/lib/jquery-ui/css/images/ui-bg_glass_65_ffffff_1x400.png
--rwxr-xr-x   0 pabloc     (501) staff       (20)      262 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/lib/jquery-ui/css/images/ui-bg_glass_75_dadada_1x400.png
--rwxr-xr-x   0 pabloc     (501) staff       (20)      262 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/lib/jquery-ui/css/images/ui-bg_glass_75_e6e6e6_1x400.png
--rwxr-xr-x   0 pabloc     (501) staff       (20)      332 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/lib/jquery-ui/css/images/ui-bg_glass_95_fef1ec_1x400.png
--rwxr-xr-x   0 pabloc     (501) staff       (20)      280 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/lib/jquery-ui/css/images/ui-bg_highlight-soft_75_cccccc_1x100.png
--rwxr-xr-x   0 pabloc     (501) staff       (20)     4970 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/lib/jquery-ui/css/images/ui-icons_222222_256x240.png
--rwxr-xr-x   0 pabloc     (501) staff       (20)     4510 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/lib/jquery-ui/css/images/ui-icons_2e83ff_256x240.png
--rwxr-xr-x   0 pabloc     (501) staff       (20)     4974 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/lib/jquery-ui/css/images/ui-icons_454545_256x240.png
--rwxr-xr-x   0 pabloc     (501) staff       (20)     4979 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/lib/jquery-ui/css/images/ui-icons_888888_256x240.png
--rwxr-xr-x   0 pabloc     (501) staff       (20)     4510 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/lib/jquery-ui/css/images/ui-icons_cd0a0a_256x240.png
--rwxr-xr-x   0 pabloc     (501) staff       (20)    17063 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/lib/jquery-ui/css/jquery-ui-1.10.3.custom.min.css
-drwxr-xr-x   0 pabloc     (501) staff       (20)        0 2024-01-15 15:27:05.381852 luigi-3.5.0/luigi/static/visualiser/lib/jquery-ui/js/
--rwxr-xr-x   0 pabloc     (501) staff       (20)    38439 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/lib/jquery-ui/js/jquery-ui-1.10.3.custom.min.js
--rw-r--r--   0 pabloc     (501) staff       (20)     4650 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/lib/jquery.slimscroll.min.js
--rw-r--r--   0 pabloc     (501) staff       (20)    14853 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/lib/mustache.js
-drwxr-xr-x   0 pabloc     (501) staff       (20)        0 2024-01-15 15:27:05.382770 luigi-3.5.0/luigi/static/visualiser/mockdata/
--rw-r--r--   0 pabloc     (501) staff       (20)     1097 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/mockdata/dep_graph
--rw-r--r--   0 pabloc     (501) staff       (20)      400 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/mockdata/fetch_error
--rw-r--r--   0 pabloc     (501) staff       (20)     1097 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/mockdata/task_list
--rw-r--r--   0 pabloc     (501) staff       (20)      510 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/static/visualiser/test.html
--rw-r--r--   0 pabloc     (501) staff       (20)    12256 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/target.py
--rw-r--r--   0 pabloc     (501) staff       (20)    36223 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/task.py
--rw-r--r--   0 pabloc     (501) staff       (20)     1991 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/task_history.py
--rw-r--r--   0 pabloc     (501) staff       (20)     7999 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/task_register.py
--rw-r--r--   0 pabloc     (501) staff       (20)      892 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/task_status.py
-drwxr-xr-x   0 pabloc     (501) staff       (20)        0 2024-01-15 15:27:05.385347 luigi-3.5.0/luigi/templates/
--rwxr-xr-x   0 pabloc     (501) staff       (20)     4270 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/templates/history.html
--rwxr-xr-x   0 pabloc     (501) staff       (20)     3033 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/templates/layout.html
--rwxr-xr-x   0 pabloc     (501) staff       (20)      553 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/templates/menu.html
--rw-r--r--   0 pabloc     (501) staff       (20)      730 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/templates/recent.html
--rw-r--r--   0 pabloc     (501) staff       (20)     1282 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/templates/show.html
-drwxr-xr-x   0 pabloc     (501) staff       (20)        0 2024-01-15 15:27:05.386479 luigi-3.5.0/luigi/tools/
--rw-r--r--   0 pabloc     (501) staff       (20)      751 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/tools/__init__.py
--rwxr-xr-x   0 pabloc     (501) staff       (20)     4753 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/tools/deps.py
--rwxr-xr-x   0 pabloc     (501) staff       (20)     2566 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/tools/deps_tree.py
--rwxr-xr-x   0 pabloc     (501) staff       (20)     2808 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/tools/luigi_grep.py
--rwxr-xr-x   0 pabloc     (501) staff       (20)    33931 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/tools/range.py
--rw-r--r--   0 pabloc     (501) staff       (20)    16503 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/util.py
--rw-r--r--   0 pabloc     (501) staff       (20)    53126 2024-01-04 16:31:55.000000 luigi-3.5.0/luigi/worker.py
-drwxr-xr-x   0 pabloc     (501) staff       (20)        0 2024-01-15 15:27:05.337921 luigi-3.5.0/luigi.egg-info/
--rw-r--r--   0 pabloc     (501) staff       (20)    14096 2024-01-15 15:27:05.000000 luigi-3.5.0/luigi.egg-info/PKG-INFO
--rw-r--r--   0 pabloc     (501) staff       (20)     9111 2024-01-15 15:27:05.000000 luigi-3.5.0/luigi.egg-info/SOURCES.txt
--rw-r--r--   0 pabloc     (501) staff       (20)        1 2024-01-15 15:27:05.000000 luigi-3.5.0/luigi.egg-info/dependency_links.txt
--rw-r--r--   0 pabloc     (501) staff       (20)      201 2024-01-15 15:27:05.000000 luigi-3.5.0/luigi.egg-info/entry_points.txt
--rw-r--r--   0 pabloc     (501) staff       (20)      158 2024-01-15 15:27:05.000000 luigi-3.5.0/luigi.egg-info/requires.txt
--rw-r--r--   0 pabloc     (501) staff       (20)        6 2024-01-15 15:27:05.000000 luigi-3.5.0/luigi.egg-info/top_level.txt
--rw-r--r--   0 pabloc     (501) staff       (20)       38 2024-01-15 15:27:05.444293 luigi-3.5.0/setup.cfg
--rw-r--r--   0 pabloc     (501) staff       (20)     4248 2024-01-15 15:17:29.000000 luigi-3.5.0/setup.py
-drwxr-xr-x   0 pabloc     (501) staff       (20)        0 2024-01-15 15:27:05.442798 luigi-3.5.0/test/
--rw-r--r--   0 pabloc     (501) staff       (20)     1732 2024-01-11 12:30:30.000000 luigi-3.5.0/test/_mysqldb_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)     7317 2024-01-11 12:30:30.000000 luigi-3.5.0/test/_test_ftp.py
--rw-r--r--   0 pabloc     (501) staff       (20)    21729 2024-01-11 12:30:30.000000 luigi-3.5.0/test/batch_notifier_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)     2250 2024-01-11 12:30:30.000000 luigi-3.5.0/test/choice_parameter_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)     2286 2024-01-11 12:30:30.000000 luigi-3.5.0/test/clone_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)    14333 2024-01-15 15:17:29.000000 luigi-3.5.0/test/cmdline_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)     3496 2024-01-11 12:30:30.000000 luigi-3.5.0/test/config_env_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)     3012 2024-01-11 12:30:30.000000 luigi-3.5.0/test/config_toml_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)        0 2024-01-11 12:30:30.000000 luigi-3.5.0/test/conftest.py
--rw-r--r--   0 pabloc     (501) staff       (20)     3996 2024-01-11 12:30:30.000000 luigi-3.5.0/test/customized_run_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)     5623 2024-01-11 12:30:30.000000 luigi-3.5.0/test/date_interval_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)     7052 2024-01-11 12:30:30.000000 luigi-3.5.0/test/date_parameter_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)     6002 2024-01-11 12:30:30.000000 luigi-3.5.0/test/db_task_history_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)    10659 2024-01-11 12:30:30.000000 luigi-3.5.0/test/decorator_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)     5510 2024-01-11 12:30:30.000000 luigi-3.5.0/test/dict_parameter_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)     1179 2024-01-11 12:30:30.000000 luigi-3.5.0/test/dynamic_import_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)     9651 2024-01-11 12:30:30.000000 luigi-3.5.0/test/event_callbacks_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)    38687 2024-01-11 12:30:30.000000 luigi-3.5.0/test/execution_summary_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)     1449 2024-01-11 12:30:30.000000 luigi-3.5.0/test/factorial_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)     2262 2024-01-11 12:30:30.000000 luigi-3.5.0/test/fib_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)      858 2024-01-11 12:30:30.000000 luigi-3.5.0/test/hdfs_client_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)     7619 2024-01-11 12:30:30.000000 luigi-3.5.0/test/helpers.py
--rw-r--r--   0 pabloc     (501) staff       (20)     1686 2024-01-11 12:30:30.000000 luigi-3.5.0/test/helpers_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)     2249 2024-01-11 12:30:30.000000 luigi-3.5.0/test/import_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)     2677 2024-01-11 12:30:30.000000 luigi-3.5.0/test/instance_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)     3012 2024-01-11 12:30:30.000000 luigi-3.5.0/test/instance_wrap_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)     8909 2024-01-15 15:17:29.000000 luigi-3.5.0/test/interface_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)     4547 2024-01-11 12:30:30.000000 luigi-3.5.0/test/list_parameter_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)    11446 2024-01-11 12:30:30.000000 luigi-3.5.0/test/local_target_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)     5704 2024-01-11 12:30:30.000000 luigi-3.5.0/test/lock_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)     1323 2024-01-11 12:30:30.000000 luigi-3.5.0/test/metrics_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)     3312 2024-01-11 12:30:30.000000 luigi-3.5.0/test/mock_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)     1082 2024-01-11 12:30:30.000000 luigi-3.5.0/test/most_common_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)    15673 2024-01-11 12:30:30.000000 luigi-3.5.0/test/notifications_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)     4528 2024-01-11 12:30:30.000000 luigi-3.5.0/test/numerical_parameter_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)     7194 2024-01-11 12:30:30.000000 luigi-3.5.0/test/optional_parameter_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)      836 2024-01-11 12:30:30.000000 luigi-3.5.0/test/other_module.py
--rw-r--r--   0 pabloc     (501) staff       (20)    50865 2024-01-11 12:30:30.000000 luigi-3.5.0/test/parameter_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)     1592 2024-01-11 12:30:30.000000 luigi-3.5.0/test/priority_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)    65249 2024-01-11 12:30:30.000000 luigi-3.5.0/test/range_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)     1547 2024-01-11 12:30:30.000000 luigi-3.5.0/test/recursion_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)     1430 2024-01-11 12:30:30.000000 luigi-3.5.0/test/remote_scheduler_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)     6722 2024-01-11 12:30:30.000000 luigi-3.5.0/test/retcodes_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)     7810 2024-01-11 12:30:30.000000 luigi-3.5.0/test/rpc_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)      946 2024-01-11 12:30:30.000000 luigi-3.5.0/test/runtests.py
--rw-r--r--   0 pabloc     (501) staff       (20)   108568 2024-01-11 12:30:30.000000 luigi-3.5.0/test/scheduler_api_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)     3833 2024-01-11 12:30:30.000000 luigi-3.5.0/test/scheduler_message_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)     5046 2024-01-11 12:30:30.000000 luigi-3.5.0/test/scheduler_parameter_visibilities_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)    15901 2024-01-11 12:30:30.000000 luigi-3.5.0/test/scheduler_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)    19929 2024-01-11 12:30:30.000000 luigi-3.5.0/test/scheduler_visualisation_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)    19988 2024-01-11 12:30:30.000000 luigi-3.5.0/test/server_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)     1218 2024-01-11 12:30:30.000000 luigi-3.5.0/test/set_task_name_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)     6226 2024-01-11 12:30:30.000000 luigi-3.5.0/test/setup_logging_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)     2971 2024-01-11 12:30:30.000000 luigi-3.5.0/test/simulate_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)     1450 2024-01-11 12:30:30.000000 luigi-3.5.0/test/subtask_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)    11128 2024-01-11 12:30:30.000000 luigi-3.5.0/test/target_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)     2361 2024-01-11 12:30:30.000000 luigi-3.5.0/test/task_bulk_complete_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)     3033 2024-01-11 12:30:30.000000 luigi-3.5.0/test/task_forwarded_attributes_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)     1687 2024-01-11 12:30:30.000000 luigi-3.5.0/test/task_history_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)     1166 2024-01-11 12:30:30.000000 luigi-3.5.0/test/task_progress_percentage_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)     1847 2024-01-11 12:30:30.000000 luigi-3.5.0/test/task_register_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)     4482 2024-01-11 12:30:30.000000 luigi-3.5.0/test/task_running_resources_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)     4092 2024-01-11 12:30:30.000000 luigi-3.5.0/test/task_serialize_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)     1223 2024-01-11 12:30:30.000000 luigi-3.5.0/test/task_status_message_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)    20149 2024-01-15 15:17:29.000000 luigi-3.5.0/test/task_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)     2848 2024-01-11 12:30:30.000000 luigi-3.5.0/test/test_sigpipe.py
--rw-r--r--   0 pabloc     (501) staff       (20)     1796 2024-01-11 12:30:30.000000 luigi-3.5.0/test/test_ssh.py
--rw-r--r--   0 pabloc     (501) staff       (20)     6500 2024-01-11 12:30:30.000000 luigi-3.5.0/test/util_previous_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)     7333 2024-01-11 12:30:30.000000 luigi-3.5.0/test/util_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)     3499 2024-01-11 12:30:30.000000 luigi-3.5.0/test/visible_parameters_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)     6664 2024-01-11 12:30:30.000000 luigi-3.5.0/test/worker_external_task_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)     4240 2024-01-11 12:30:30.000000 luigi-3.5.0/test/worker_keep_alive_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)     4005 2024-01-11 12:30:30.000000 luigi-3.5.0/test/worker_multiprocess_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)     6351 2024-01-11 12:30:30.000000 luigi-3.5.0/test/worker_parallel_scheduling_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)     6895 2024-01-11 12:30:30.000000 luigi-3.5.0/test/worker_scheduler_com_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)     2797 2024-01-11 12:30:30.000000 luigi-3.5.0/test/worker_task_process_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)     5127 2024-01-11 12:30:30.000000 luigi-3.5.0/test/worker_task_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)    76929 2024-01-11 12:30:30.000000 luigi-3.5.0/test/worker_test.py
--rw-r--r--   0 pabloc     (501) staff       (20)     2878 2024-01-11 12:30:30.000000 luigi-3.5.0/test/wrap_test.py
+drwxr-xr-x   0 andresg    (501) staff       (20)        0 2024-05-20 08:19:10.041085 luigi-3.5.1/
+-rw-r--r--   0 andresg    (501) staff       (20)    11345 2023-06-08 13:13:56.000000 luigi-3.5.1/LICENSE
+-rw-r--r--   0 andresg    (501) staff       (20)      140 2023-06-08 13:13:56.000000 luigi-3.5.1/MANIFEST.in
+-rw-r--r--   0 andresg    (501) staff       (20)    14443 2024-05-20 08:19:10.040407 luigi-3.5.1/PKG-INFO
+-rw-r--r--   0 andresg    (501) staff       (20)    12965 2024-05-20 08:11:13.000000 luigi-3.5.1/README.rst
+drwxr-xr-x   0 andresg    (501) staff       (20)        0 2024-05-20 08:19:09.934888 luigi-3.5.1/examples/
+-rw-r--r--   0 andresg    (501) staff       (20)      603 2023-06-08 13:13:56.000000 luigi-3.5.1/examples/__init__.py
+-rw-r--r--   0 andresg    (501) staff       (20)     3746 2023-06-08 13:13:56.000000 luigi-3.5.1/examples/dynamic_requirements.py
+-rw-r--r--   0 andresg    (501) staff       (20)     3410 2023-06-08 13:13:56.000000 luigi-3.5.1/examples/elasticsearch_index.py
+-rw-r--r--   0 andresg    (501) staff       (20)     3319 2023-06-08 13:13:56.000000 luigi-3.5.1/examples/execution_summary_example.py
+-rw-r--r--   0 andresg    (501) staff       (20)     1462 2023-06-08 13:13:56.000000 luigi-3.5.1/examples/foo.py
+-rw-r--r--   0 andresg    (501) staff       (20)     1876 2023-06-08 13:13:56.000000 luigi-3.5.1/examples/foo_complex.py
+-rw-r--r--   0 andresg    (501) staff       (20)     3239 2023-06-08 13:13:56.000000 luigi-3.5.1/examples/ftp_experiment_outputs.py
+-rw-r--r--   0 andresg    (501) staff       (20)      500 2023-06-08 13:13:56.000000 luigi-3.5.1/examples/hello_world.py
+-rw-r--r--   0 andresg    (501) staff       (20)     1986 2023-06-08 13:13:56.000000 luigi-3.5.1/examples/kubernetes.py
+-rw-r--r--   0 andresg    (501) staff       (20)     5264 2023-06-08 13:13:56.000000 luigi-3.5.1/examples/per_task_retry_policy.py
+-rw-r--r--   0 andresg    (501) staff       (20)     3388 2023-06-08 13:13:56.000000 luigi-3.5.1/examples/pyspark_wc.py
+-rw-r--r--   0 andresg    (501) staff       (20)     4363 2023-06-08 13:13:56.000000 luigi-3.5.1/examples/spark_als.py
+-rw-r--r--   0 andresg    (501) staff       (20)     2823 2023-06-08 13:13:56.000000 luigi-3.5.1/examples/ssh_remote_execution.py
+-rw-r--r--   0 andresg    (501) staff       (20)     3400 2023-06-08 13:13:56.000000 luigi-3.5.1/examples/terasort.py
+-rwxr-xr-x   0 andresg    (501) staff       (20)     9069 2023-06-08 13:13:56.000000 luigi-3.5.1/examples/top_artists.py
+-rwxr-xr-x   0 andresg    (501) staff       (20)      645 2023-06-08 13:13:56.000000 luigi-3.5.1/examples/top_artists_spark.py
+-rw-r--r--   0 andresg    (501) staff       (20)     2904 2023-06-08 13:13:56.000000 luigi-3.5.1/examples/wordcount.py
+-rw-r--r--   0 andresg    (501) staff       (20)     2729 2023-06-08 13:13:56.000000 luigi-3.5.1/examples/wordcount_hadoop.py
+drwxr-xr-x   0 andresg    (501) staff       (20)        0 2024-05-20 08:19:09.942819 luigi-3.5.1/luigi/
+-rw-r--r--   0 andresg    (501) staff       (20)     3723 2023-06-08 13:13:56.000000 luigi-3.5.1/luigi/__init__.py
+-rw-r--r--   0 andresg    (501) staff       (20)      683 2023-06-08 13:13:56.000000 luigi-3.5.1/luigi/__main__.py
+-rw-r--r--   0 andresg    (501) staff       (20)      249 2024-05-20 08:19:02.000000 luigi-3.5.1/luigi/__meta__.py
+-rw-r--r--   0 andresg    (501) staff       (20)     8863 2023-06-08 13:13:56.000000 luigi-3.5.1/luigi/batch_notifier.py
+-rw-r--r--   0 andresg    (501) staff       (20)     1426 2023-06-08 13:13:56.000000 luigi-3.5.1/luigi/cmdline.py
+-rw-r--r--   0 andresg    (501) staff       (20)     5458 2023-06-08 13:13:56.000000 luigi-3.5.1/luigi/cmdline_parser.py
+drwxr-xr-x   0 andresg    (501) staff       (20)        0 2024-05-20 08:19:09.945233 luigi-3.5.1/luigi/configuration/
+-rw-r--r--   0 andresg    (501) staff       (20)      837 2023-06-08 13:13:56.000000 luigi-3.5.1/luigi/configuration/__init__.py
+-rw-r--r--   0 andresg    (501) staff       (20)     1307 2023-06-08 13:13:56.000000 luigi-3.5.1/luigi/configuration/base_parser.py
+-rw-r--r--   0 andresg    (501) staff       (20)     8424 2023-10-05 08:51:28.000000 luigi-3.5.1/luigi/configuration/cfg_parser.py
+-rw-r--r--   0 andresg    (501) staff       (20)     2760 2023-06-08 13:13:56.000000 luigi-3.5.1/luigi/configuration/core.py
+-rw-r--r--   0 andresg    (501) staff       (20)     2831 2023-06-08 13:13:56.000000 luigi-3.5.1/luigi/configuration/toml_parser.py
+drwxr-xr-x   0 andresg    (501) staff       (20)        0 2024-05-20 08:19:09.958760 luigi-3.5.1/luigi/contrib/
+-rw-r--r--   0 andresg    (501) staff       (20)      661 2023-06-08 13:13:56.000000 luigi-3.5.1/luigi/contrib/__init__.py
+-rw-r--r--   0 andresg    (501) staff       (20)    13302 2023-06-08 13:13:56.000000 luigi-3.5.1/luigi/contrib/azureblob.py
+-rw-r--r--   0 andresg    (501) staff       (20)     7990 2023-06-08 13:13:56.000000 luigi-3.5.1/luigi/contrib/batch.py
+-rw-r--r--   0 andresg    (501) staff       (20)    16573 2023-06-08 13:13:56.000000 luigi-3.5.1/luigi/contrib/beam_dataflow.py
+-rw-r--r--   0 andresg    (501) staff       (20)    30813 2023-06-08 13:13:56.000000 luigi-3.5.1/luigi/contrib/bigquery.py
+-rw-r--r--   0 andresg    (501) staff       (20)     4347 2023-06-08 13:13:56.000000 luigi-3.5.1/luigi/contrib/bigquery_avro.py
+-rw-r--r--   0 andresg    (501) staff       (20)     5730 2023-06-08 13:13:56.000000 luigi-3.5.1/luigi/contrib/datadog_metric.py
+-rw-r--r--   0 andresg    (501) staff       (20)    10231 2023-06-08 13:13:56.000000 luigi-3.5.1/luigi/contrib/dataproc.py
+-rw-r--r--   0 andresg    (501) staff       (20)     9524 2023-06-08 13:13:56.000000 luigi-3.5.1/luigi/contrib/docker_runner.py
+-rw-r--r--   0 andresg    (501) staff       (20)    11346 2023-11-15 13:11:31.000000 luigi-3.5.1/luigi/contrib/dropbox.py
+-rw-r--r--   0 andresg    (501) staff       (20)     9599 2023-06-08 13:13:56.000000 luigi-3.5.1/luigi/contrib/ecs.py
+-rw-r--r--   0 andresg    (501) staff       (20)    14188 2023-06-08 13:13:56.000000 luigi-3.5.1/luigi/contrib/esindex.py
+-rw-r--r--   0 andresg    (501) staff       (20)     2330 2023-06-08 13:13:56.000000 luigi-3.5.1/luigi/contrib/external_daily_snapshot.py
+-rw-r--r--   0 andresg    (501) staff       (20)    11285 2023-06-08 13:13:56.000000 luigi-3.5.1/luigi/contrib/external_program.py
+-rw-r--r--   0 andresg    (501) staff       (20)    13354 2023-06-08 13:13:56.000000 luigi-3.5.1/luigi/contrib/ftp.py
+-rw-r--r--   0 andresg    (501) staff       (20)     1498 2023-06-08 13:13:56.000000 luigi-3.5.1/luigi/contrib/gcp.py
+-rw-r--r--   0 andresg    (501) staff       (20)    18537 2023-06-08 13:13:56.000000 luigi-3.5.1/luigi/contrib/gcs.py
+-rw-r--r--   0 andresg    (501) staff       (20)    37546 2023-06-08 13:13:56.000000 luigi-3.5.1/luigi/contrib/hadoop.py
+-rw-r--r--   0 andresg    (501) staff       (20)     5524 2023-06-08 13:13:56.000000 luigi-3.5.1/luigi/contrib/hadoop_jar.py
+drwxr-xr-x   0 andresg    (501) staff       (20)        0 2024-05-20 08:19:09.961133 luigi-3.5.1/luigi/contrib/hdfs/
+-rw-r--r--   0 andresg    (501) staff       (20)     2901 2023-06-08 13:13:56.000000 luigi-3.5.1/luigi/contrib/hdfs/__init__.py
+-rw-r--r--   0 andresg    (501) staff       (20)     2839 2023-06-08 13:13:56.000000 luigi-3.5.1/luigi/contrib/hdfs/abstract_client.py
+-rw-r--r--   0 andresg    (501) staff       (20)     1922 2023-06-08 13:13:56.000000 luigi-3.5.1/luigi/contrib/hdfs/clients.py
+-rw-r--r--   0 andresg    (501) staff       (20)     4138 2023-06-08 13:13:56.000000 luigi-3.5.1/luigi/contrib/hdfs/config.py
+-rw-r--r--   0 andresg    (501) staff       (20)     1120 2023-06-08 13:13:56.000000 luigi-3.5.1/luigi/contrib/hdfs/error.py
+-rw-r--r--   0 andresg    (501) staff       (20)     6019 2023-06-08 13:13:56.000000 luigi-3.5.1/luigi/contrib/hdfs/format.py
+-rw-r--r--   0 andresg    (501) staff       (20)     9572 2023-06-08 13:13:56.000000 luigi-3.5.1/luigi/contrib/hdfs/hadoopcli_clients.py
+-rw-r--r--   0 andresg    (501) staff       (20)     7327 2023-06-08 13:13:56.000000 luigi-3.5.1/luigi/contrib/hdfs/target.py
+-rw-r--r--   0 andresg    (501) staff       (20)     6721 2023-06-08 13:13:56.000000 luigi-3.5.1/luigi/contrib/hdfs/webhdfs_client.py
+-rw-r--r--   0 andresg    (501) staff       (20)    19543 2023-11-15 13:11:31.000000 luigi-3.5.1/luigi/contrib/hive.py
+-rw-r--r--   0 andresg    (501) staff       (20)    14284 2023-06-08 13:13:56.000000 luigi-3.5.1/luigi/contrib/kubernetes.py
+-rwxr-xr-x   0 andresg    (501) staff       (20)    12181 2023-06-08 13:13:56.000000 luigi-3.5.1/luigi/contrib/lsf.py
+-rwxr-xr-x   0 andresg    (501) staff       (20)     2297 2023-06-08 13:13:56.000000 luigi-3.5.1/luigi/contrib/lsf_runner.py
+-rw-r--r--   0 andresg    (501) staff       (20)     6678 2023-11-15 13:11:31.000000 luigi-3.5.1/luigi/contrib/mongodb.py
+-rw-r--r--   0 andresg    (501) staff       (20)     2806 2023-06-08 13:13:56.000000 luigi-3.5.1/luigi/contrib/mrrunner.py
+-rw-r--r--   0 andresg    (501) staff       (20)     5538 2023-11-15 13:11:31.000000 luigi-3.5.1/luigi/contrib/mssqldb.py
+-rw-r--r--   0 andresg    (501) staff       (20)     8663 2023-11-15 13:11:31.000000 luigi-3.5.1/luigi/contrib/mysqldb.py
+-rw-r--r--   0 andresg    (501) staff       (20)     7286 2023-06-08 13:13:56.000000 luigi-3.5.1/luigi/contrib/opener.py
+-rw-r--r--   0 andresg    (501) staff       (20)    11126 2023-06-08 13:13:56.000000 luigi-3.5.1/luigi/contrib/pai.py
+-rw-r--r--   0 andresg    (501) staff       (20)     6517 2023-06-08 13:13:56.000000 luigi-3.5.1/luigi/contrib/pig.py
+-rw-r--r--   0 andresg    (501) staff       (20)    16403 2023-11-15 13:11:31.000000 luigi-3.5.1/luigi/contrib/postgres.py
+-rw-r--r--   0 andresg    (501) staff       (20)     7825 2024-05-20 08:11:13.000000 luigi-3.5.1/luigi/contrib/presto.py
+-rw-r--r--   0 andresg    (501) staff       (20)     2430 2023-06-08 13:13:56.000000 luigi-3.5.1/luigi/contrib/prometheus_metric.py
+-rw-r--r--   0 andresg    (501) staff       (20)     3897 2023-06-08 13:13:56.000000 luigi-3.5.1/luigi/contrib/pyspark_runner.py
+-rw-r--r--   0 andresg    (501) staff       (20)    11181 2023-06-08 13:13:56.000000 luigi-3.5.1/luigi/contrib/rdbms.py
+-rw-r--r--   0 andresg    (501) staff       (20)     3085 2023-11-15 13:11:31.000000 luigi-3.5.1/luigi/contrib/redis_store.py
+-rw-r--r--   0 andresg    (501) staff       (20)    25778 2023-06-08 13:13:56.000000 luigi-3.5.1/luigi/contrib/redshift.py
+-rw-r--r--   0 andresg    (501) staff       (20)    27902 2023-06-08 13:13:56.000000 luigi-3.5.1/luigi/contrib/s3.py
+-rw-r--r--   0 andresg    (501) staff       (20)    27695 2023-06-08 13:13:56.000000 luigi-3.5.1/luigi/contrib/salesforce.py
+-rw-r--r--   0 andresg    (501) staff       (20)    10682 2023-06-08 13:13:56.000000 luigi-3.5.1/luigi/contrib/scalding.py
+-rwxr-xr-x   0 andresg    (501) staff       (20)    13563 2023-06-08 13:13:56.000000 luigi-3.5.1/luigi/contrib/sge.py
+-rwxr-xr-x   0 andresg    (501) staff       (20)     2830 2023-06-08 13:13:56.000000 luigi-3.5.1/luigi/contrib/sge_runner.py
+-rw-r--r--   0 andresg    (501) staff       (20)     3406 2023-11-15 13:11:31.000000 luigi-3.5.1/luigi/contrib/simulate.py
+-rw-r--r--   0 andresg    (501) staff       (20)    12313 2023-06-08 13:13:56.000000 luigi-3.5.1/luigi/contrib/spark.py
+-rw-r--r--   0 andresg    (501) staff       (20)     1970 2023-06-08 13:13:56.000000 luigi-3.5.1/luigi/contrib/sparkey.py
+-rw-r--r--   0 andresg    (501) staff       (20)    16432 2023-11-15 13:11:31.000000 luigi-3.5.1/luigi/contrib/sqla.py
+-rw-r--r--   0 andresg    (501) staff       (20)    12356 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/contrib/ssh.py
+-rw-r--r--   0 andresg    (501) staff       (20)     2811 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/contrib/target.py
+-rw-r--r--   0 andresg    (501) staff       (20)     2974 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/contrib/webhdfs.py
+-rw-r--r--   0 andresg    (501) staff       (20)     8620 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/date_interval.py
+-rw-r--r--   0 andresg    (501) staff       (20)    11268 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/db_task_history.py
+-rw-r--r--   0 andresg    (501) staff       (20)     1758 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/event.py
+-rw-r--r--   0 andresg    (501) staff       (20)    20264 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/execution_summary.py
+-rw-r--r--   0 andresg    (501) staff       (20)    14691 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/format.py
+-rw-r--r--   0 andresg    (501) staff       (20)     2122 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/freezing.py
+-rw-r--r--   0 andresg    (501) staff       (20)     8971 2023-10-05 08:51:28.000000 luigi-3.5.1/luigi/interface.py
+-rw-r--r--   0 andresg    (501) staff       (20)     6182 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/local_target.py
+-rw-r--r--   0 andresg    (501) staff       (20)     5410 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/lock.py
+-rw-r--r--   0 andresg    (501) staff       (20)     2516 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/metrics.py
+-rw-r--r--   0 andresg    (501) staff       (20)     5663 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/mock.py
+-rw-r--r--   0 andresg    (501) staff       (20)    14535 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/notifications.py
+-rw-r--r--   0 andresg    (501) staff       (20)    54038 2024-05-20 08:11:13.000000 luigi-3.5.1/luigi/parameter.py
+-rw-r--r--   0 andresg    (501) staff       (20)     3489 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/process.py
+-rw-r--r--   0 andresg    (501) staff       (20)     4658 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/retcodes.py
+-rw-r--r--   0 andresg    (501) staff       (20)     6907 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/rpc.py
+-rw-r--r--   0 andresg    (501) staff       (20)    65995 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/scheduler.py
+-rw-r--r--   0 andresg    (501) staff       (20)    14294 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/server.py
+-rw-r--r--   0 andresg    (501) staff       (20)     5889 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/setup_logging.py
+drwxr-xr-x   0 andresg    (501) staff       (20)        0 2024-05-20 08:19:09.927431 luigi-3.5.1/luigi/static/
+drwxr-xr-x   0 andresg    (501) staff       (20)        0 2024-05-20 08:19:09.961994 luigi-3.5.1/luigi/static/visualiser/
+drwxr-xr-x   0 andresg    (501) staff       (20)        0 2024-05-20 08:19:09.962937 luigi-3.5.1/luigi/static/visualiser/css/
+-rw-r--r--   0 andresg    (501) staff       (20)    23739 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/css/font-awesome.min.css
+-rw-r--r--   0 andresg    (501) staff       (20)     3413 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/css/luigi.css
+-rw-r--r--   0 andresg    (501) staff       (20)     2162 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/css/tipsy.css
+drwxr-xr-x   0 andresg    (501) staff       (20)        0 2024-05-20 08:19:09.966636 luigi-3.5.1/luigi/static/visualiser/fonts/
+-rw-r--r--   0 andresg    (501) staff       (20)    93888 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/fonts/FontAwesome.otf
+-rwxr-xr-x   0 andresg    (501) staff       (20)    60767 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 andresg    (501) staff       (20)   313398 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/fonts/fontawesome-webfont.svg
+-rwxr-xr-x   0 andresg    (501) staff       (20)   122092 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/fonts/fontawesome-webfont.ttf
+-rwxr-xr-x   0 andresg    (501) staff       (20)    71508 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 andresg    (501) staff       (20)    56780 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 andresg    (501) staff       (20)    20335 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 andresg    (501) staff       (20)    62927 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 andresg    (501) staff       (20)    41280 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 andresg    (501) staff       (20)    23320 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 andresg    (501) staff       (20)    33256 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/index.html
+drwxr-xr-x   0 andresg    (501) staff       (20)        0 2024-05-20 08:19:09.967993 luigi-3.5.1/luigi/static/visualiser/js/
+-rw-r--r--   0 andresg    (501) staff       (20)    12101 2024-05-20 08:11:13.000000 luigi-3.5.1/luigi/static/visualiser/js/graph.js
+-rw-r--r--   0 andresg    (501) staff       (20)     8076 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/js/luigi.js
+drwxr-xr-x   0 andresg    (501) staff       (20)        0 2024-05-20 08:19:09.968628 luigi-3.5.1/luigi/static/visualiser/js/test/
+-rw-r--r--   0 andresg    (501) staff       (20)     3969 2024-05-20 08:11:13.000000 luigi-3.5.1/luigi/static/visualiser/js/test/graph_test.js
+-rw-r--r--   0 andresg    (501) staff       (20)    11097 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/js/tipsy.js
+-rw-r--r--   0 andresg    (501) staff       (20)      189 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/js/util.js
+-rw-r--r--   0 andresg    (501) staff       (20)    58572 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/js/visualiserApp.js
+drwxr-xr-x   0 andresg    (501) staff       (20)        0 2024-05-20 08:19:09.969727 luigi-3.5.1/luigi/static/visualiser/lib/
+drwxr-xr-x   0 andresg    (501) staff       (20)        0 2024-05-20 08:19:09.928203 luigi-3.5.1/luigi/static/visualiser/lib/AdminLTE/
+drwxr-xr-x   0 andresg    (501) staff       (20)        0 2024-05-20 08:19:09.970636 luigi-3.5.1/luigi/static/visualiser/lib/AdminLTE/css/
+-rw-r--r--   0 andresg    (501) staff       (20)    75652 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/lib/AdminLTE/css/AdminLTE.min.css
+-rw-r--r--   0 andresg    (501) staff       (20)     3800 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/lib/AdminLTE/css/skin-green-light.min.css
+-rw-r--r--   0 andresg    (501) staff       (20)     3033 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/lib/AdminLTE/css/skin-green.min.css
+drwxr-xr-x   0 andresg    (501) staff       (20)        0 2024-05-20 08:19:09.970839 luigi-3.5.1/luigi/static/visualiser/lib/AdminLTE/js/
+-rw-r--r--   0 andresg    (501) staff       (20)     9420 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/lib/AdminLTE/js/app.min.js
+drwxr-xr-x   0 andresg    (501) staff       (20)        0 2024-05-20 08:19:09.928362 luigi-3.5.1/luigi/static/visualiser/lib/URI/
+drwxr-xr-x   0 andresg    (501) staff       (20)        0 2024-05-20 08:19:09.971071 luigi-3.5.1/luigi/static/visualiser/lib/URI/1.18.2/
+-rw-r--r--   0 andresg    (501) staff       (20)    62788 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/lib/URI/1.18.2/URI.js
+drwxr-xr-x   0 andresg    (501) staff       (20)        0 2024-05-20 08:19:09.928601 luigi-3.5.1/luigi/static/visualiser/lib/bootstrap-toggle/
+drwxr-xr-x   0 andresg    (501) staff       (20)        0 2024-05-20 08:19:09.971369 luigi-3.5.1/luigi/static/visualiser/lib/bootstrap-toggle/css/
+-rwxr-xr-x   0 andresg    (501) staff       (20)     1590 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/lib/bootstrap-toggle/css/bootstrap-toggle.min.css
+drwxr-xr-x   0 andresg    (501) staff       (20)        0 2024-05-20 08:19:09.971610 luigi-3.5.1/luigi/static/visualiser/lib/bootstrap-toggle/js/
+-rwxr-xr-x   0 andresg    (501) staff       (20)     4129 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/lib/bootstrap-toggle/js/bootstrap-toggle.min.js
+drwxr-xr-x   0 andresg    (501) staff       (20)        0 2024-05-20 08:19:09.928831 luigi-3.5.1/luigi/static/visualiser/lib/bootstrap3/
+drwxr-xr-x   0 andresg    (501) staff       (20)        0 2024-05-20 08:19:09.972222 luigi-3.5.1/luigi/static/visualiser/lib/bootstrap3/css/
+-rw-r--r--   0 andresg    (501) staff       (20)    19970 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/lib/bootstrap3/css/bootstrap-theme.min.css
+-rw-r--r--   0 andresg    (501) staff       (20)   117308 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/lib/bootstrap3/css/bootstrap.min.css
+drwxr-xr-x   0 andresg    (501) staff       (20)        0 2024-05-20 08:19:09.972657 luigi-3.5.1/luigi/static/visualiser/lib/bootstrap3/js/
+-rw-r--r--   0 andresg    (501) staff       (20)    35951 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/lib/bootstrap3/js/bootstrap.min.js
+drwxr-xr-x   0 andresg    (501) staff       (20)        0 2024-05-20 08:19:09.973630 luigi-3.5.1/luigi/static/visualiser/lib/d3/
+-rw-r--r--   0 andresg    (501) staff       (20)   151143 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/lib/d3/d3.min.js
+-rw-r--r--   0 andresg    (501) staff       (20)   113027 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/lib/d3/dagre-d3.min.js
+drwxr-xr-x   0 andresg    (501) staff       (20)        0 2024-05-20 08:19:09.929225 luigi-3.5.1/luigi/static/visualiser/lib/datatables/
+drwxr-xr-x   0 andresg    (501) staff       (20)        0 2024-05-20 08:19:09.974090 luigi-3.5.1/luigi/static/visualiser/lib/datatables/css/
+-rw-r--r--   0 andresg    (501) staff       (20)    15353 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/lib/datatables/css/jquery.dataTables.min.css
+drwxr-xr-x   0 andresg    (501) staff       (20)        0 2024-05-20 08:19:09.975538 luigi-3.5.1/luigi/static/visualiser/lib/datatables/images/
+-rw-r--r--   0 andresg    (501) staff       (20)    27490 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/lib/datatables/images/Sorting icons.psd
+-rw-r--r--   0 andresg    (501) staff       (20)      894 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/lib/datatables/images/favicon.ico
+-rw-r--r--   0 andresg    (501) staff       (20)      160 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/lib/datatables/images/sort_asc.png
+-rw-r--r--   0 andresg    (501) staff       (20)      148 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/lib/datatables/images/sort_asc_disabled.png
+-rw-r--r--   0 andresg    (501) staff       (20)      201 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/lib/datatables/images/sort_both.png
+-rw-r--r--   0 andresg    (501) staff       (20)      158 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/lib/datatables/images/sort_desc.png
+-rw-r--r--   0 andresg    (501) staff       (20)      146 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/lib/datatables/images/sort_desc_disabled.png
+drwxr-xr-x   0 andresg    (501) staff       (20)        0 2024-05-20 08:19:09.975709 luigi-3.5.1/luigi/static/visualiser/lib/datatables/js/
+-rw-r--r--   0 andresg    (501) staff       (20)    79457 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/lib/datatables/js/jquery.dataTables.min.js
+-rw-r--r--   0 andresg    (501) staff       (20)    93026 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/lib/jquery-1.10.0.min.js
+drwxr-xr-x   0 andresg    (501) staff       (20)        0 2024-05-20 08:19:09.929552 luigi-3.5.1/luigi/static/visualiser/lib/jquery-ui/
+drwxr-xr-x   0 andresg    (501) staff       (20)        0 2024-05-20 08:19:09.975999 luigi-3.5.1/luigi/static/visualiser/lib/jquery-ui/css/
+drwxr-xr-x   0 andresg    (501) staff       (20)        0 2024-05-20 08:19:09.979432 luigi-3.5.1/luigi/static/visualiser/lib/jquery-ui/css/images/
+-rwxr-xr-x   0 andresg    (501) staff       (20)     1738 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/lib/jquery-ui/css/images/animated-overlay.gif
+-rwxr-xr-x   0 andresg    (501) staff       (20)      212 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/lib/jquery-ui/css/images/ui-bg_flat_0_aaaaaa_40x100.png
+-rwxr-xr-x   0 andresg    (501) staff       (20)      208 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/lib/jquery-ui/css/images/ui-bg_flat_75_ffffff_40x100.png
+-rwxr-xr-x   0 andresg    (501) staff       (20)      335 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/lib/jquery-ui/css/images/ui-bg_glass_55_fbf9ee_1x400.png
+-rwxr-xr-x   0 andresg    (501) staff       (20)      207 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/lib/jquery-ui/css/images/ui-bg_glass_65_ffffff_1x400.png
+-rwxr-xr-x   0 andresg    (501) staff       (20)      262 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/lib/jquery-ui/css/images/ui-bg_glass_75_dadada_1x400.png
+-rwxr-xr-x   0 andresg    (501) staff       (20)      262 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/lib/jquery-ui/css/images/ui-bg_glass_75_e6e6e6_1x400.png
+-rwxr-xr-x   0 andresg    (501) staff       (20)      332 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/lib/jquery-ui/css/images/ui-bg_glass_95_fef1ec_1x400.png
+-rwxr-xr-x   0 andresg    (501) staff       (20)      280 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/lib/jquery-ui/css/images/ui-bg_highlight-soft_75_cccccc_1x100.png
+-rwxr-xr-x   0 andresg    (501) staff       (20)     4970 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/lib/jquery-ui/css/images/ui-icons_222222_256x240.png
+-rwxr-xr-x   0 andresg    (501) staff       (20)     4510 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/lib/jquery-ui/css/images/ui-icons_2e83ff_256x240.png
+-rwxr-xr-x   0 andresg    (501) staff       (20)     4974 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/lib/jquery-ui/css/images/ui-icons_454545_256x240.png
+-rwxr-xr-x   0 andresg    (501) staff       (20)     4979 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/lib/jquery-ui/css/images/ui-icons_888888_256x240.png
+-rwxr-xr-x   0 andresg    (501) staff       (20)     4510 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/lib/jquery-ui/css/images/ui-icons_cd0a0a_256x240.png
+-rwxr-xr-x   0 andresg    (501) staff       (20)    17063 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/lib/jquery-ui/css/jquery-ui-1.10.3.custom.min.css
+drwxr-xr-x   0 andresg    (501) staff       (20)        0 2024-05-20 08:19:09.979730 luigi-3.5.1/luigi/static/visualiser/lib/jquery-ui/js/
+-rwxr-xr-x   0 andresg    (501) staff       (20)    38439 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/lib/jquery-ui/js/jquery-ui-1.10.3.custom.min.js
+-rw-r--r--   0 andresg    (501) staff       (20)     4650 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/lib/jquery.slimscroll.min.js
+-rw-r--r--   0 andresg    (501) staff       (20)    14853 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/lib/mustache.js
+drwxr-xr-x   0 andresg    (501) staff       (20)        0 2024-05-20 08:19:09.980726 luigi-3.5.1/luigi/static/visualiser/mockdata/
+-rw-r--r--   0 andresg    (501) staff       (20)     1097 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/mockdata/dep_graph
+-rw-r--r--   0 andresg    (501) staff       (20)      400 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/mockdata/fetch_error
+-rw-r--r--   0 andresg    (501) staff       (20)     1097 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/mockdata/task_list
+-rw-r--r--   0 andresg    (501) staff       (20)      510 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/static/visualiser/test.html
+-rw-r--r--   0 andresg    (501) staff       (20)    12256 2023-11-15 13:11:31.000000 luigi-3.5.1/luigi/target.py
+-rw-r--r--   0 andresg    (501) staff       (20)    36478 2024-05-20 08:11:13.000000 luigi-3.5.1/luigi/task.py
+-rw-r--r--   0 andresg    (501) staff       (20)     1991 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/task_history.py
+-rw-r--r--   0 andresg    (501) staff       (20)     7999 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/task_register.py
+-rw-r--r--   0 andresg    (501) staff       (20)      892 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/task_status.py
+drwxr-xr-x   0 andresg    (501) staff       (20)        0 2024-05-20 08:19:09.981736 luigi-3.5.1/luigi/templates/
+-rwxr-xr-x   0 andresg    (501) staff       (20)     4270 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/templates/history.html
+-rwxr-xr-x   0 andresg    (501) staff       (20)     3033 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/templates/layout.html
+-rwxr-xr-x   0 andresg    (501) staff       (20)      553 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/templates/menu.html
+-rw-r--r--   0 andresg    (501) staff       (20)      730 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/templates/recent.html
+-rw-r--r--   0 andresg    (501) staff       (20)     1282 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/templates/show.html
+drwxr-xr-x   0 andresg    (501) staff       (20)        0 2024-05-20 08:19:09.982808 luigi-3.5.1/luigi/tools/
+-rw-r--r--   0 andresg    (501) staff       (20)      751 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/tools/__init__.py
+-rwxr-xr-x   0 andresg    (501) staff       (20)     4753 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/tools/deps.py
+-rwxr-xr-x   0 andresg    (501) staff       (20)     2566 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/tools/deps_tree.py
+-rwxr-xr-x   0 andresg    (501) staff       (20)     2808 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/tools/luigi_grep.py
+-rwxr-xr-x   0 andresg    (501) staff       (20)    33931 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/tools/range.py
+-rw-r--r--   0 andresg    (501) staff       (20)    16503 2023-06-08 13:13:57.000000 luigi-3.5.1/luigi/util.py
+-rw-r--r--   0 andresg    (501) staff       (20)    53144 2024-05-20 08:11:13.000000 luigi-3.5.1/luigi/worker.py
+drwxr-xr-x   0 andresg    (501) staff       (20)        0 2024-05-20 08:19:10.038571 luigi-3.5.1/luigi.egg-info/
+-rw-r--r--   0 andresg    (501) staff       (20)    14443 2024-05-20 08:19:09.000000 luigi-3.5.1/luigi.egg-info/PKG-INFO
+-rw-r--r--   0 andresg    (501) staff       (20)     9111 2024-05-20 08:19:09.000000 luigi-3.5.1/luigi.egg-info/SOURCES.txt
+-rw-r--r--   0 andresg    (501) staff       (20)        1 2024-05-20 08:19:09.000000 luigi-3.5.1/luigi.egg-info/dependency_links.txt
+-rw-r--r--   0 andresg    (501) staff       (20)      201 2024-05-20 08:19:09.000000 luigi-3.5.1/luigi.egg-info/entry_points.txt
+-rw-r--r--   0 andresg    (501) staff       (20)      158 2024-05-20 08:19:09.000000 luigi-3.5.1/luigi.egg-info/requires.txt
+-rw-r--r--   0 andresg    (501) staff       (20)        6 2024-05-20 08:19:09.000000 luigi-3.5.1/luigi.egg-info/top_level.txt
+-rw-r--r--   0 andresg    (501) staff       (20)       38 2024-05-20 08:19:10.041326 luigi-3.5.1/setup.cfg
+-rw-r--r--   0 andresg    (501) staff       (20)     4298 2024-05-20 08:11:13.000000 luigi-3.5.1/setup.py
+drwxr-xr-x   0 andresg    (501) staff       (20)        0 2024-05-20 08:19:10.037364 luigi-3.5.1/test/
+-rw-r--r--   0 andresg    (501) staff       (20)     1732 2023-06-08 13:13:57.000000 luigi-3.5.1/test/_mysqldb_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)     7317 2023-06-08 13:13:57.000000 luigi-3.5.1/test/_test_ftp.py
+-rw-r--r--   0 andresg    (501) staff       (20)    21729 2023-06-08 13:13:57.000000 luigi-3.5.1/test/batch_notifier_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)     2250 2023-06-08 13:13:57.000000 luigi-3.5.1/test/choice_parameter_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)     2286 2023-06-08 13:13:57.000000 luigi-3.5.1/test/clone_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)    14332 2024-05-20 08:11:13.000000 luigi-3.5.1/test/cmdline_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)     3496 2023-06-08 13:13:57.000000 luigi-3.5.1/test/config_env_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)     3012 2023-06-08 13:13:57.000000 luigi-3.5.1/test/config_toml_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)        0 2023-06-08 13:13:57.000000 luigi-3.5.1/test/conftest.py
+-rw-r--r--   0 andresg    (501) staff       (20)     3996 2023-06-08 13:13:57.000000 luigi-3.5.1/test/customized_run_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)     5623 2023-06-08 13:13:57.000000 luigi-3.5.1/test/date_interval_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)     7052 2023-06-08 13:13:57.000000 luigi-3.5.1/test/date_parameter_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)     6002 2023-06-08 13:13:57.000000 luigi-3.5.1/test/db_task_history_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)    10659 2023-06-08 13:13:57.000000 luigi-3.5.1/test/decorator_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)     5510 2023-06-08 13:13:57.000000 luigi-3.5.1/test/dict_parameter_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)     1179 2023-06-08 13:13:57.000000 luigi-3.5.1/test/dynamic_import_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)    10086 2024-05-20 08:11:13.000000 luigi-3.5.1/test/event_callbacks_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)    38687 2023-06-08 13:13:57.000000 luigi-3.5.1/test/execution_summary_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)     1449 2023-06-08 13:13:57.000000 luigi-3.5.1/test/factorial_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)     2262 2023-06-08 13:13:57.000000 luigi-3.5.1/test/fib_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)      858 2023-06-08 13:13:57.000000 luigi-3.5.1/test/hdfs_client_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)     7619 2023-06-08 13:13:57.000000 luigi-3.5.1/test/helpers.py
+-rw-r--r--   0 andresg    (501) staff       (20)     1686 2023-06-08 13:13:57.000000 luigi-3.5.1/test/helpers_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)     2249 2023-06-08 13:13:57.000000 luigi-3.5.1/test/import_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)     2677 2023-06-08 13:13:57.000000 luigi-3.5.1/test/instance_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)     3012 2023-06-08 13:13:57.000000 luigi-3.5.1/test/instance_wrap_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)     8907 2024-05-20 08:11:13.000000 luigi-3.5.1/test/interface_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)     4517 2024-05-20 08:11:13.000000 luigi-3.5.1/test/list_parameter_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)    11446 2023-06-08 13:13:57.000000 luigi-3.5.1/test/local_target_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)     5704 2023-06-08 13:13:57.000000 luigi-3.5.1/test/lock_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)     1323 2023-06-08 13:13:57.000000 luigi-3.5.1/test/metrics_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)     3312 2023-06-08 13:13:57.000000 luigi-3.5.1/test/mock_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)     1082 2023-06-08 13:13:57.000000 luigi-3.5.1/test/most_common_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)    15673 2023-06-08 13:13:57.000000 luigi-3.5.1/test/notifications_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)     4528 2023-06-08 13:13:57.000000 luigi-3.5.1/test/numerical_parameter_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)     7412 2024-05-20 08:11:13.000000 luigi-3.5.1/test/optional_parameter_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)      836 2023-06-08 13:13:57.000000 luigi-3.5.1/test/other_module.py
+-rw-r--r--   0 andresg    (501) staff       (20)    51171 2024-05-20 08:11:13.000000 luigi-3.5.1/test/parameter_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)     1592 2023-06-08 13:13:57.000000 luigi-3.5.1/test/priority_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)    65249 2023-06-08 13:13:57.000000 luigi-3.5.1/test/range_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)     1547 2023-06-08 13:13:57.000000 luigi-3.5.1/test/recursion_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)     1430 2023-06-08 13:13:57.000000 luigi-3.5.1/test/remote_scheduler_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)     6722 2023-06-08 13:13:57.000000 luigi-3.5.1/test/retcodes_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)     7810 2023-06-08 13:13:57.000000 luigi-3.5.1/test/rpc_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)      946 2023-06-08 13:13:57.000000 luigi-3.5.1/test/runtests.py
+-rw-r--r--   0 andresg    (501) staff       (20)   108568 2023-06-08 13:13:57.000000 luigi-3.5.1/test/scheduler_api_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)     3833 2023-06-08 13:13:57.000000 luigi-3.5.1/test/scheduler_message_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)     5046 2023-06-08 13:13:57.000000 luigi-3.5.1/test/scheduler_parameter_visibilities_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)    15901 2023-06-08 13:13:57.000000 luigi-3.5.1/test/scheduler_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)    19929 2023-06-08 13:13:57.000000 luigi-3.5.1/test/scheduler_visualisation_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)    19988 2023-06-08 13:13:57.000000 luigi-3.5.1/test/server_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)     1218 2023-06-08 13:13:57.000000 luigi-3.5.1/test/set_task_name_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)     6226 2023-06-08 13:13:57.000000 luigi-3.5.1/test/setup_logging_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)     2971 2023-06-08 13:13:57.000000 luigi-3.5.1/test/simulate_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)     1450 2023-06-08 13:13:57.000000 luigi-3.5.1/test/subtask_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)    11128 2023-06-08 13:13:57.000000 luigi-3.5.1/test/target_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)     2361 2023-06-08 13:13:57.000000 luigi-3.5.1/test/task_bulk_complete_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)     3033 2023-06-08 13:13:57.000000 luigi-3.5.1/test/task_forwarded_attributes_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)     1687 2023-06-08 13:13:57.000000 luigi-3.5.1/test/task_history_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)     1166 2023-06-08 13:13:57.000000 luigi-3.5.1/test/task_progress_percentage_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)     1847 2023-06-08 13:13:57.000000 luigi-3.5.1/test/task_register_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)     4482 2023-06-08 13:13:57.000000 luigi-3.5.1/test/task_running_resources_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)     4092 2023-06-08 13:13:57.000000 luigi-3.5.1/test/task_serialize_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)     1223 2023-06-08 13:13:57.000000 luigi-3.5.1/test/task_status_message_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)    20148 2024-05-20 08:11:13.000000 luigi-3.5.1/test/task_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)     2848 2023-06-08 13:13:57.000000 luigi-3.5.1/test/test_sigpipe.py
+-rw-r--r--   0 andresg    (501) staff       (20)     1796 2023-06-08 13:13:57.000000 luigi-3.5.1/test/test_ssh.py
+-rw-r--r--   0 andresg    (501) staff       (20)     6500 2023-06-08 13:13:57.000000 luigi-3.5.1/test/util_previous_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)     7333 2023-06-08 13:13:57.000000 luigi-3.5.1/test/util_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)     3499 2023-06-08 13:13:57.000000 luigi-3.5.1/test/visible_parameters_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)     6664 2023-06-08 13:13:57.000000 luigi-3.5.1/test/worker_external_task_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)     4240 2023-06-08 13:13:57.000000 luigi-3.5.1/test/worker_keep_alive_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)     4005 2023-06-08 13:13:57.000000 luigi-3.5.1/test/worker_multiprocess_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)     6351 2023-06-08 13:13:57.000000 luigi-3.5.1/test/worker_parallel_scheduling_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)     6895 2023-06-08 13:13:57.000000 luigi-3.5.1/test/worker_scheduler_com_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)     2797 2023-06-08 13:13:57.000000 luigi-3.5.1/test/worker_task_process_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)     6390 2024-05-20 08:11:13.000000 luigi-3.5.1/test/worker_task_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)    76929 2023-10-05 08:51:28.000000 luigi-3.5.1/test/worker_test.py
+-rw-r--r--   0 andresg    (501) staff       (20)     2878 2023-06-08 13:13:57.000000 luigi-3.5.1/test/wrap_test.py
```

### Comparing `luigi-3.5.0/LICENSE` & `luigi-3.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/PKG-INFO` & `luigi-3.5.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luigi
-Version: 3.5.0
+Version: 3.5.1
 Summary: Workflow mgmgt + task scheduling + dependency resolution.
 Home-page: https://github.com/spotify/luigi
 Author: The Luigi Authors
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
@@ -14,19 +14,27 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Monitoring
+License-File: LICENSE
+Requires-Dist: python-dateutil<3,>=2.7.5
+Requires-Dist: tenacity<9,>=8
+Requires-Dist: python-daemon
+Requires-Dist: tornado<7,>=5.0
 Provides-Extra: jsonschema
+Requires-Dist: jsonschema; extra == "jsonschema"
 Provides-Extra: prometheus
+Requires-Dist: prometheus-client<0.15,>=0.5; extra == "prometheus"
 Provides-Extra: toml
-License-File: LICENSE
+Requires-Dist: toml<2.0.0; extra == "toml"
 
 
 
 
 .. note::
 
    For the latest source, discussion, etc, please visit the
@@ -49,15 +57,15 @@
 .. image:: https://img.shields.io/pypi/l/luigi.svg?style=flat
    :target: https://pypi.python.org/pypi/luigi
 
 .. image:: https://readthedocs.org/projects/luigi/badge/?version=stable
     :target: https://luigi.readthedocs.io/en/stable/?badge=stable
     :alt: Documentation Status
 
-Luigi is a Python (3.6, 3.7, 3.8, 3.9, 3.10, 3.11 tested) package that helps you build complex
+Luigi is a Python (3.6, 3.7, 3.8, 3.9, 3.10, 3.11, 3.12 tested) package that helps you build complex
 pipelines of batch jobs. It handles dependency resolution, workflow management,
 visualization, handling failures, command line integration, and much more.
 
 Getting Started
 ---------------
 
 Run ``pip install luigi`` to install the latest stable version from `PyPI
```

### Comparing `luigi-3.5.0/README.rst` & `luigi-3.5.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 .. image:: https://img.shields.io/pypi/l/luigi.svg?style=flat
    :target: https://pypi.python.org/pypi/luigi
 
 .. image:: https://readthedocs.org/projects/luigi/badge/?version=stable
     :target: https://luigi.readthedocs.io/en/stable/?badge=stable
     :alt: Documentation Status
 
-Luigi is a Python (3.6, 3.7, 3.8, 3.9, 3.10, 3.11 tested) package that helps you build complex
+Luigi is a Python (3.6, 3.7, 3.8, 3.9, 3.10, 3.11, 3.12 tested) package that helps you build complex
 pipelines of batch jobs. It handles dependency resolution, workflow management,
 visualization, handling failures, command line integration, and much more.
 
 Getting Started
 ---------------
 
 Run ``pip install luigi`` to install the latest stable version from `PyPI
```

### Comparing `luigi-3.5.0/examples/__init__.py` & `luigi-3.5.1/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/examples/dynamic_requirements.py` & `luigi-3.5.1/examples/dynamic_requirements.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/examples/elasticsearch_index.py` & `luigi-3.5.1/examples/elasticsearch_index.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/examples/execution_summary_example.py` & `luigi-3.5.1/examples/execution_summary_example.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/examples/foo.py` & `luigi-3.5.1/examples/foo.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/examples/foo_complex.py` & `luigi-3.5.1/examples/foo_complex.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/examples/ftp_experiment_outputs.py` & `luigi-3.5.1/examples/ftp_experiment_outputs.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/examples/kubernetes.py` & `luigi-3.5.1/examples/kubernetes.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/examples/per_task_retry_policy.py` & `luigi-3.5.1/examples/per_task_retry_policy.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/examples/pyspark_wc.py` & `luigi-3.5.1/examples/pyspark_wc.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/examples/spark_als.py` & `luigi-3.5.1/examples/spark_als.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/examples/ssh_remote_execution.py` & `luigi-3.5.1/examples/ssh_remote_execution.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/examples/terasort.py` & `luigi-3.5.1/examples/terasort.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/examples/top_artists.py` & `luigi-3.5.1/examples/top_artists.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/examples/top_artists_spark.py` & `luigi-3.5.1/examples/top_artists_spark.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/examples/wordcount.py` & `luigi-3.5.1/examples/wordcount.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/examples/wordcount_hadoop.py` & `luigi-3.5.1/examples/wordcount_hadoop.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/__init__.py` & `luigi-3.5.1/luigi/__init__.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/__main__.py` & `luigi-3.5.1/luigi/__main__.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/batch_notifier.py` & `luigi-3.5.1/luigi/batch_notifier.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/cmdline.py` & `luigi-3.5.1/luigi/cmdline.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/cmdline_parser.py` & `luigi-3.5.1/luigi/cmdline_parser.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/configuration/__init__.py` & `luigi-3.5.1/luigi/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/configuration/base_parser.py` & `luigi-3.5.1/luigi/configuration/base_parser.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/configuration/cfg_parser.py` & `luigi-3.5.1/luigi/configuration/cfg_parser.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/configuration/core.py` & `luigi-3.5.1/luigi/configuration/core.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/configuration/toml_parser.py` & `luigi-3.5.1/luigi/configuration/toml_parser.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/__init__.py` & `luigi-3.5.1/luigi/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/azureblob.py` & `luigi-3.5.1/luigi/contrib/azureblob.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/batch.py` & `luigi-3.5.1/luigi/contrib/batch.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/beam_dataflow.py` & `luigi-3.5.1/luigi/contrib/beam_dataflow.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/bigquery.py` & `luigi-3.5.1/luigi/contrib/bigquery.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/bigquery_avro.py` & `luigi-3.5.1/luigi/contrib/bigquery_avro.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/datadog_metric.py` & `luigi-3.5.1/luigi/contrib/datadog_metric.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/dataproc.py` & `luigi-3.5.1/luigi/contrib/dataproc.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/docker_runner.py` & `luigi-3.5.1/luigi/contrib/docker_runner.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/dropbox.py` & `luigi-3.5.1/luigi/contrib/dropbox.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/ecs.py` & `luigi-3.5.1/luigi/contrib/ecs.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/esindex.py` & `luigi-3.5.1/luigi/contrib/esindex.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/external_daily_snapshot.py` & `luigi-3.5.1/luigi/contrib/external_daily_snapshot.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/external_program.py` & `luigi-3.5.1/luigi/contrib/external_program.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/ftp.py` & `luigi-3.5.1/luigi/contrib/ftp.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/gcp.py` & `luigi-3.5.1/luigi/contrib/gcp.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/gcs.py` & `luigi-3.5.1/luigi/contrib/gcs.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/hadoop.py` & `luigi-3.5.1/luigi/contrib/hadoop.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/hadoop_jar.py` & `luigi-3.5.1/luigi/contrib/hadoop_jar.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/hdfs/__init__.py` & `luigi-3.5.1/luigi/contrib/hdfs/__init__.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/hdfs/abstract_client.py` & `luigi-3.5.1/luigi/contrib/hdfs/abstract_client.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/hdfs/clients.py` & `luigi-3.5.1/luigi/contrib/hdfs/clients.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/hdfs/config.py` & `luigi-3.5.1/luigi/contrib/hdfs/config.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/hdfs/error.py` & `luigi-3.5.1/luigi/contrib/hdfs/error.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/hdfs/format.py` & `luigi-3.5.1/luigi/contrib/hdfs/format.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/hdfs/hadoopcli_clients.py` & `luigi-3.5.1/luigi/contrib/hdfs/hadoopcli_clients.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/hdfs/target.py` & `luigi-3.5.1/luigi/contrib/hdfs/target.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/hdfs/webhdfs_client.py` & `luigi-3.5.1/luigi/contrib/hdfs/webhdfs_client.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/hive.py` & `luigi-3.5.1/luigi/contrib/hive.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/kubernetes.py` & `luigi-3.5.1/luigi/contrib/kubernetes.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/lsf.py` & `luigi-3.5.1/luigi/contrib/lsf.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/lsf_runner.py` & `luigi-3.5.1/luigi/contrib/lsf_runner.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/mongodb.py` & `luigi-3.5.1/luigi/contrib/mongodb.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/mrrunner.py` & `luigi-3.5.1/luigi/contrib/mrrunner.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/mssqldb.py` & `luigi-3.5.1/luigi/contrib/mssqldb.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/mysqldb.py` & `luigi-3.5.1/luigi/contrib/mysqldb.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/opener.py` & `luigi-3.5.1/luigi/contrib/opener.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/pai.py` & `luigi-3.5.1/luigi/contrib/pai.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/pig.py` & `luigi-3.5.1/luigi/contrib/pig.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/postgres.py` & `luigi-3.5.1/luigi/contrib/postgres.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/presto.py` & `luigi-3.5.1/luigi/contrib/presto.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/prometheus_metric.py` & `luigi-3.5.1/luigi/contrib/prometheus_metric.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/pyspark_runner.py` & `luigi-3.5.1/luigi/contrib/pyspark_runner.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/rdbms.py` & `luigi-3.5.1/luigi/contrib/rdbms.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/redis_store.py` & `luigi-3.5.1/luigi/contrib/redis_store.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/redshift.py` & `luigi-3.5.1/luigi/contrib/redshift.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/s3.py` & `luigi-3.5.1/luigi/contrib/s3.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/salesforce.py` & `luigi-3.5.1/luigi/contrib/salesforce.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/scalding.py` & `luigi-3.5.1/luigi/contrib/scalding.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/sge.py` & `luigi-3.5.1/luigi/contrib/sge.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/sge_runner.py` & `luigi-3.5.1/luigi/contrib/sge_runner.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/simulate.py` & `luigi-3.5.1/luigi/contrib/simulate.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/spark.py` & `luigi-3.5.1/luigi/contrib/spark.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/sparkey.py` & `luigi-3.5.1/luigi/contrib/sparkey.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/sqla.py` & `luigi-3.5.1/luigi/contrib/sqla.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/ssh.py` & `luigi-3.5.1/luigi/contrib/ssh.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/target.py` & `luigi-3.5.1/luigi/contrib/target.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/contrib/webhdfs.py` & `luigi-3.5.1/luigi/contrib/webhdfs.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/date_interval.py` & `luigi-3.5.1/luigi/date_interval.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/db_task_history.py` & `luigi-3.5.1/luigi/db_task_history.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/event.py` & `luigi-3.5.1/luigi/event.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/execution_summary.py` & `luigi-3.5.1/luigi/execution_summary.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/format.py` & `luigi-3.5.1/luigi/format.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/freezing.py` & `luigi-3.5.1/luigi/freezing.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/interface.py` & `luigi-3.5.1/luigi/interface.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/local_target.py` & `luigi-3.5.1/luigi/local_target.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/lock.py` & `luigi-3.5.1/luigi/lock.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/metrics.py` & `luigi-3.5.1/luigi/metrics.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/mock.py` & `luigi-3.5.1/luigi/mock.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/notifications.py` & `luigi-3.5.1/luigi/notifications.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/parameter.py` & `luigi-3.5.1/luigi/parameter.py`

 * *Files 1% similar despite different names*

```diff
@@ -305,15 +305,15 @@
         This is very implementation defined, but can be used to validate/clamp
         valid values. For example, if you wanted to only accept even integers,
         and "correct" odd values to the nearest integer, you can implement
         normalize as ``x // 2 * 2``.
         """
         return x  # default impl
 
-    def next_in_enumeration(self, _value):
+    def next_in_enumeration(self, value):
         """
         If your Parameter type has an enumerable ordering of values. You can
         choose to override this method. This method is used by the
         :py:mod:`luigi.execution_summary` module for pretty printing
         purposes. Enabling it to pretty print tasks like ``MyTask(num=1),
         MyTask(num=2), MyTask(num=3)`` to ``MyTask(num=1..3)``.
 
@@ -385,14 +385,17 @@
                 (
                     f'{self.__class__.__name__} "{param_name}" with value '
                     f'"{param_value}" is not of {param_type} or None.'
                 ),
                 OptionalParameterTypeWarning,
             )
 
+    def next_in_enumeration(self, value):
+        return None
+
 
 class OptionalParameter(OptionalParameterMixin, Parameter):
     """Class to parse optional parameters."""
 
     expected_type = str
 
 
@@ -1375,18 +1378,23 @@
         # json.loads(t_json_str) == t
         # json.loads(t_str) == ValueError: No JSON object could be decoded
 
         # Therefore, if json.loads(x) returns a ValueError, try ast.literal_eval(x).
         # ast.literal_eval(t_str) == t
         try:
             # loop required to parse tuple of tuples
-            return tuple(tuple(x) for x in json.loads(x, object_pairs_hook=FrozenOrderedDict))
+            return tuple(self._convert_iterable_to_tuple(x) for x in json.loads(x, object_pairs_hook=FrozenOrderedDict))
         except (ValueError, TypeError):
             return tuple(literal_eval(x))  # if this causes an error, let that error be raised.
 
+    def _convert_iterable_to_tuple(self, x):
+        if isinstance(x, str):
+            return x
+        return tuple(x)
+
 
 class OptionalTupleParameter(OptionalParameterMixin, TupleParameter):
     """Class to parse optional tuple parameters."""
 
     expected_type = tuple
```

### Comparing `luigi-3.5.0/luigi/process.py` & `luigi-3.5.1/luigi/process.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/retcodes.py` & `luigi-3.5.1/luigi/retcodes.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/rpc.py` & `luigi-3.5.1/luigi/rpc.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/scheduler.py` & `luigi-3.5.1/luigi/scheduler.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/server.py` & `luigi-3.5.1/luigi/server.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/setup_logging.py` & `luigi-3.5.1/luigi/setup_logging.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/static/visualiser/css/font-awesome.min.css` & `luigi-3.5.1/luigi/static/visualiser/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/static/visualiser/css/luigi.css` & `luigi-3.5.1/luigi/static/visualiser/css/luigi.css`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/static/visualiser/css/tipsy.css` & `luigi-3.5.1/luigi/static/visualiser/css/tipsy.css`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/static/visualiser/fonts/FontAwesome.otf` & `luigi-3.5.1/luigi/static/visualiser/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/static/visualiser/fonts/fontawesome-webfont.eot` & `luigi-3.5.1/luigi/static/visualiser/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/static/visualiser/fonts/fontawesome-webfont.svg` & `luigi-3.5.1/luigi/static/visualiser/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/static/visualiser/fonts/fontawesome-webfont.ttf` & `luigi-3.5.1/luigi/static/visualiser/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/static/visualiser/fonts/fontawesome-webfont.woff` & `luigi-3.5.1/luigi/static/visualiser/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/static/visualiser/fonts/fontawesome-webfont.woff2` & `luigi-3.5.1/luigi/static/visualiser/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/static/visualiser/fonts/glyphicons-halflings-regular.eot` & `luigi-3.5.1/luigi/static/visualiser/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/static/visualiser/fonts/glyphicons-halflings-regular.svg` & `luigi-3.5.1/luigi/static/visualiser/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/static/visualiser/fonts/glyphicons-halflings-regular.ttf` & `luigi-3.5.1/luigi/static/visualiser/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/static/visualiser/fonts/glyphicons-halflings-regular.woff` & `luigi-3.5.1/luigi/static/visualiser/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/static/visualiser/index.html` & `luigi-3.5.1/luigi/static/visualiser/index.html`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/static/visualiser/js/graph.js` & `luigi-3.5.1/luigi/static/visualiser/js/graph.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -144,16 +144,16 @@
             }
             if (n.xOrder === undefined && depth === n.depth) {
                 n.xOrder = rowSizes[depth];
                 rowSizes[depth]++;
                 $.each(n.deps, function(i, dep) {
                     if (nodeIndex[dep]) {
                         var next_node = nodes[nodeIndex[dep]]
-                        var depth = (selfDependencies ? depth + 1 : classDepths[next_node.name])
-                        placeNodes(next_node, depth);
+                        var next_depth = (selfDependencies ? depth + 1 : classDepths[next_node.name])
+                        placeNodes(next_node, next_depth);
                     }
                 });
             }
         }
         placeNodes(nodes[0], 0);
 
         return rowSizes;
```

### Comparing `luigi-3.5.0/luigi/static/visualiser/js/luigi.js` & `luigi-3.5.1/luigi/static/visualiser/js/luigi.js`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/static/visualiser/js/test/graph_test.js` & `luigi-3.5.1/luigi/static/visualiser/js/test/graph_test.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,23 +1,32 @@
 module("graph.js");
 
 test("nodeFromTask", function() {
     var task = {
-        deps: ["B", "C"],
-        taskId: "A",
-        status: "DONE"
+        deps: ["B1", "C1"],
+        taskId: "A1",
+        status: "DONE",
+        name: "A",
+        params: {},
+        priority: 0,
     };
     var expected = {
-        taskId: "A",
+        taskId: "A1",
         status: "DONE",
-        trackingUrl: "#A",
-        deps: ["B", "C"],
-        depth: -1
+        trackingUrl: "#A1",
+        deps: ["B1", "C1"],
+        depth: -1,
+        name: "A",
+        params: {},
+        priority: 0,
     };
-    deepEqual(Graph.testableMethods.nodeFromTask(task), expected);
+    let graph = {
+        hashBase: "#"
+    }
+    deepEqual(Graph.testableMethods.nodeFromTask.bind(graph)(task), expected);
 });
 
 test("uniqueIndexByProperty", function() {
     var input = [{
         a: "x",
         b: 100
     }, {
@@ -131,15 +140,15 @@
     var nodeIndex = {
         "A1": 0,
         "A2": 1
     }
     var rowSizes = Graph.testableMethods.computeRows(nodes, nodeIndex)
     equal(A1.depth, 0)
     equal(A2.depth, 1)
-    equal(rowSizes, [1, 1])
+    deepEqual(rowSizes, [1, 1])
 });
 
 test("computeRowsGrouped", function() {
     var A0 = {
         name: "A",
         taskId: "A0",
         deps: ["D0", "B0"],
@@ -189,25 +198,37 @@
     }
     var E2 = {
         name: "E",
         taskId: "E2",
         deps: [],
         depth: -1
     }
+    var nodes = [A0, B0, C1, C2, D0, D1, D2, E1, E2]
+    var nodeIndex = {
+        "A0": 0,
+        "B0": 1,
+        "C1": 2,
+        "C2": 3,
+        "D0": 4,
+        "D1": 5,
+        "D2": 6,
+        "E1": 7,
+        "E2": 8
+    }
     var rowSizes = Graph.testableMethods.computeRows(nodes, nodeIndex)
     equal(A0.depth, 0)
     equal(B0.depth, 1)
     equal(C1.depth, 2)
     equal(C2.depth, 2)
     equal(D0.depth, 3)
     equal(D1.depth, 3)
     equal(D2.depth, 3)
     equal(E1.depth, 4)
     equal(E2.depth, 4)
-    equal(rowSizes, [1, 1, 2, 3, 2])
+    deepEqual(rowSizes, [1, 1, 2, 3, 2])
 });
 
 test("createGraph", function() {
     var tasks = [{
         taskId: "A",
         deps: ["B", "C"],
         status: "PENDING"
```

### Comparing `luigi-3.5.0/luigi/static/visualiser/js/tipsy.js` & `luigi-3.5.1/luigi/static/visualiser/js/tipsy.js`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/static/visualiser/js/visualiserApp.js` & `luigi-3.5.1/luigi/static/visualiser/js/visualiserApp.js`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/static/visualiser/lib/AdminLTE/css/AdminLTE.min.css` & `luigi-3.5.1/luigi/static/visualiser/lib/AdminLTE/css/AdminLTE.min.css`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/static/visualiser/lib/AdminLTE/css/skin-green-light.min.css` & `luigi-3.5.1/luigi/static/visualiser/lib/AdminLTE/css/skin-green-light.min.css`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/static/visualiser/lib/AdminLTE/css/skin-green.min.css` & `luigi-3.5.1/luigi/static/visualiser/lib/AdminLTE/css/skin-green.min.css`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/static/visualiser/lib/AdminLTE/js/app.min.js` & `luigi-3.5.1/luigi/static/visualiser/lib/AdminLTE/js/app.min.js`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/static/visualiser/lib/URI/1.18.2/URI.js` & `luigi-3.5.1/luigi/static/visualiser/lib/URI/1.18.2/URI.js`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/static/visualiser/lib/bootstrap-toggle/css/bootstrap-toggle.min.css` & `luigi-3.5.1/luigi/static/visualiser/lib/bootstrap-toggle/css/bootstrap-toggle.min.css`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/static/visualiser/lib/bootstrap-toggle/js/bootstrap-toggle.min.js` & `luigi-3.5.1/luigi/static/visualiser/lib/bootstrap-toggle/js/bootstrap-toggle.min.js`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/static/visualiser/lib/bootstrap3/css/bootstrap-theme.min.css` & `luigi-3.5.1/luigi/static/visualiser/lib/bootstrap3/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/static/visualiser/lib/bootstrap3/css/bootstrap.min.css` & `luigi-3.5.1/luigi/static/visualiser/lib/bootstrap3/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/static/visualiser/lib/bootstrap3/js/bootstrap.min.js` & `luigi-3.5.1/luigi/static/visualiser/lib/bootstrap3/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/static/visualiser/lib/d3/d3.min.js` & `luigi-3.5.1/luigi/static/visualiser/lib/d3/d3.min.js`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/static/visualiser/lib/d3/dagre-d3.min.js` & `luigi-3.5.1/luigi/static/visualiser/lib/d3/dagre-d3.min.js`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/static/visualiser/lib/datatables/css/jquery.dataTables.min.css` & `luigi-3.5.1/luigi/static/visualiser/lib/datatables/css/jquery.dataTables.min.css`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/static/visualiser/lib/datatables/images/Sorting icons.psd` & `luigi-3.5.1/luigi/static/visualiser/lib/datatables/images/Sorting icons.psd`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/static/visualiser/lib/datatables/images/favicon.ico` & `luigi-3.5.1/luigi/static/visualiser/lib/datatables/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/static/visualiser/lib/datatables/js/jquery.dataTables.min.js` & `luigi-3.5.1/luigi/static/visualiser/lib/datatables/js/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/static/visualiser/lib/jquery-1.10.0.min.js` & `luigi-3.5.1/luigi/static/visualiser/lib/jquery-1.10.0.min.js`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/static/visualiser/lib/jquery-ui/css/images/animated-overlay.gif` & `luigi-3.5.1/luigi/static/visualiser/lib/jquery-ui/css/images/animated-overlay.gif`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/static/visualiser/lib/jquery-ui/css/images/ui-icons_222222_256x240.png` & `luigi-3.5.1/luigi/static/visualiser/lib/jquery-ui/css/images/ui-icons_222222_256x240.png`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/static/visualiser/lib/jquery-ui/css/images/ui-icons_2e83ff_256x240.png` & `luigi-3.5.1/luigi/static/visualiser/lib/jquery-ui/css/images/ui-icons_2e83ff_256x240.png`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/static/visualiser/lib/jquery-ui/css/images/ui-icons_454545_256x240.png` & `luigi-3.5.1/luigi/static/visualiser/lib/jquery-ui/css/images/ui-icons_454545_256x240.png`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/static/visualiser/lib/jquery-ui/css/images/ui-icons_888888_256x240.png` & `luigi-3.5.1/luigi/static/visualiser/lib/jquery-ui/css/images/ui-icons_888888_256x240.png`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/static/visualiser/lib/jquery-ui/css/images/ui-icons_cd0a0a_256x240.png` & `luigi-3.5.1/luigi/static/visualiser/lib/jquery-ui/css/images/ui-icons_cd0a0a_256x240.png`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/static/visualiser/lib/jquery-ui/css/jquery-ui-1.10.3.custom.min.css` & `luigi-3.5.1/luigi/static/visualiser/lib/jquery-ui/css/jquery-ui-1.10.3.custom.min.css`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/static/visualiser/lib/jquery-ui/js/jquery-ui-1.10.3.custom.min.js` & `luigi-3.5.1/luigi/static/visualiser/lib/jquery-ui/js/jquery-ui-1.10.3.custom.min.js`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/static/visualiser/lib/jquery.slimscroll.min.js` & `luigi-3.5.1/luigi/static/visualiser/lib/jquery.slimscroll.min.js`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/static/visualiser/lib/mustache.js` & `luigi-3.5.1/luigi/static/visualiser/lib/mustache.js`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/static/visualiser/mockdata/dep_graph` & `luigi-3.5.1/luigi/static/visualiser/mockdata/dep_graph`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/static/visualiser/mockdata/task_list` & `luigi-3.5.1/luigi/static/visualiser/mockdata/task_list`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/target.py` & `luigi-3.5.1/luigi/target.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/task.py` & `luigi-3.5.1/luigi/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -260,14 +260,21 @@
         Decorator for adding event handlers.
         """
         def wrapped(callback):
             cls._event_callbacks.setdefault(cls, {}).setdefault(event, set()).add(callback)
             return callback
         return wrapped
 
+    @classmethod
+    def remove_event_handler(cls, event, callback):
+        """
+        Function to remove the event handler registered previously by the cls.event_handler decorator.
+        """
+        cls._event_callbacks[cls][event].remove(callback)
+
     def trigger_event(self, event, *args, **kwargs):
         """
         Trigger that calls all of the specified events associated with this class.
         """
         for event_class, event_callbacks in self._event_callbacks.items():
             if not isinstance(self, event_class):
                 continue
```

### Comparing `luigi-3.5.0/luigi/task_history.py` & `luigi-3.5.1/luigi/task_history.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/task_register.py` & `luigi-3.5.1/luigi/task_register.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/task_status.py` & `luigi-3.5.1/luigi/task_status.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/templates/history.html` & `luigi-3.5.1/luigi/templates/history.html`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/templates/layout.html` & `luigi-3.5.1/luigi/templates/layout.html`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/templates/menu.html` & `luigi-3.5.1/luigi/templates/menu.html`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/templates/recent.html` & `luigi-3.5.1/luigi/templates/recent.html`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/templates/show.html` & `luigi-3.5.1/luigi/templates/show.html`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/tools/__init__.py` & `luigi-3.5.1/luigi/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/tools/deps.py` & `luigi-3.5.1/luigi/tools/deps.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/tools/deps_tree.py` & `luigi-3.5.1/luigi/tools/deps_tree.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/tools/luigi_grep.py` & `luigi-3.5.1/luigi/tools/luigi_grep.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/tools/range.py` & `luigi-3.5.1/luigi/tools/range.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/util.py` & `luigi-3.5.1/luigi/util.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/luigi/worker.py` & `luigi-3.5.1/luigi/worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
 from luigi import notifications
 from luigi.event import Event
 from luigi.task_register import load_task
 from luigi.scheduler import DISABLED, DONE, FAILED, PENDING, UNKNOWN, Scheduler, RetryPolicy
 from luigi.scheduler import WORKER_STATE_ACTIVE, WORKER_STATE_DISABLED
 from luigi.target import Target
-from luigi.task import Task, Config, DynamicRequirements
+from luigi.task import Task, Config, DynamicRequirements, flatten
 from luigi.task_register import TaskClassException
 from luigi.task_status import RUNNING
 from luigi.parameter import BoolParameter, FloatParameter, IntParameter, OptionalParameter, Parameter, TimeDeltaParameter
 
 import json
 
 logger = logging.getLogger('luigi-interface')
@@ -181,15 +181,15 @@
             # don't care about unfulfilled dependencies, because we are just
             # checking completeness of self.task so outputs of dependencies are
             # irrelevant.
             if self.check_unfulfilled_deps and not _is_external(self.task):
                 missing = []
                 for dep in self.task.deps():
                     if not self.check_complete(dep):
-                        nonexistent_outputs = [output for output in dep.output() if not output.exists()]
+                        nonexistent_outputs = [output for output in flatten(dep.output()) if not output.exists()]
                         if nonexistent_outputs:
                             missing.append(f'{dep.task_id} ({", ".join(map(str, nonexistent_outputs))})')
                         else:
                             missing.append(dep.task_id)
                 if missing:
                     deps = 'dependency' if len(missing) == 1 else 'dependencies'
                     raise RuntimeError('Unfulfilled %s at run time: %s' % (deps, ', '.join(missing)))
```

### Comparing `luigi-3.5.0/luigi.egg-info/PKG-INFO` & `luigi-3.5.1/luigi.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luigi
-Version: 3.5.0
+Version: 3.5.1
 Summary: Workflow mgmgt + task scheduling + dependency resolution.
 Home-page: https://github.com/spotify/luigi
 Author: The Luigi Authors
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
@@ -14,19 +14,27 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Monitoring
+License-File: LICENSE
+Requires-Dist: python-dateutil<3,>=2.7.5
+Requires-Dist: tenacity<9,>=8
+Requires-Dist: python-daemon
+Requires-Dist: tornado<7,>=5.0
 Provides-Extra: jsonschema
+Requires-Dist: jsonschema; extra == "jsonschema"
 Provides-Extra: prometheus
+Requires-Dist: prometheus-client<0.15,>=0.5; extra == "prometheus"
 Provides-Extra: toml
-License-File: LICENSE
+Requires-Dist: toml<2.0.0; extra == "toml"
 
 
 
 
 .. note::
 
    For the latest source, discussion, etc, please visit the
@@ -49,15 +57,15 @@
 .. image:: https://img.shields.io/pypi/l/luigi.svg?style=flat
    :target: https://pypi.python.org/pypi/luigi
 
 .. image:: https://readthedocs.org/projects/luigi/badge/?version=stable
     :target: https://luigi.readthedocs.io/en/stable/?badge=stable
     :alt: Documentation Status
 
-Luigi is a Python (3.6, 3.7, 3.8, 3.9, 3.10, 3.11 tested) package that helps you build complex
+Luigi is a Python (3.6, 3.7, 3.8, 3.9, 3.10, 3.11, 3.12 tested) package that helps you build complex
 pipelines of batch jobs. It handles dependency resolution, workflow management,
 visualization, handling failures, command line integration, and much more.
 
 Getting Started
 ---------------
 
 Run ``pip install luigi`` to install the latest stable version from `PyPI
```

### Comparing `luigi-3.5.0/luigi.egg-info/SOURCES.txt` & `luigi-3.5.1/luigi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/setup.py` & `luigi-3.5.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,10 +114,11 @@
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'Topic :: System :: Monitoring',
     ],
 )
```

### Comparing `luigi-3.5.0/test/_mysqldb_test.py` & `luigi-3.5.1/test/_mysqldb_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/_test_ftp.py` & `luigi-3.5.1/test/_test_ftp.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/batch_notifier_test.py` & `luigi-3.5.1/test/batch_notifier_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/choice_parameter_test.py` & `luigi-3.5.1/test/choice_parameter_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/clone_test.py` & `luigi-3.5.1/test/clone_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/cmdline_test.py` & `luigi-3.5.1/test/cmdline_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -358,14 +358,14 @@
         returncode, stdout, stderr = self._run_cmdline([
             './bin/luigi', '--module', 'cmdline_test', 'TaskThatRequiresConfig', '--local-scheduler', '--no-lock'
             '--RequiredConfig-required-test-param', 'A',
         ])
         print(stdout)
         print(stderr)
 
-        self.assertNotEquals(returncode, 1)
+        self.assertNotEqual(returncode, 1)
         self.assertFalse(b'required_test_param' in stderr)
 
 
 if __name__ == '__main__':
     # Needed for one of the tests
     luigi.run()
```

### Comparing `luigi-3.5.0/test/config_env_test.py` & `luigi-3.5.1/test/config_env_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/config_toml_test.py` & `luigi-3.5.1/test/config_toml_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/customized_run_test.py` & `luigi-3.5.1/test/customized_run_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/date_interval_test.py` & `luigi-3.5.1/test/date_interval_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/date_parameter_test.py` & `luigi-3.5.1/test/date_parameter_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/db_task_history_test.py` & `luigi-3.5.1/test/db_task_history_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/decorator_test.py` & `luigi-3.5.1/test/decorator_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/dict_parameter_test.py` & `luigi-3.5.1/test/dict_parameter_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/dynamic_import_test.py` & `luigi-3.5.1/test/dynamic_import_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/event_callbacks_test.py` & `luigi-3.5.1/test/event_callbacks_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,14 +158,29 @@
         self.assertTrue(task is t)
         self.assertEqual(time, 42.0)
 
     def test_processing_time_handler_failure(self):
         t, result = self._run_processing_time_handler(True)
         self.assertEqual(result, [])
 
+    def test_remove_event_handler(self):
+        run_cnt = 0
+
+        @EmptyTask.event_handler(luigi.Event.START)
+        def handler(task):
+            nonlocal run_cnt
+            run_cnt += 1
+
+        task = EmptyTask()
+        build([task], local_scheduler=True)
+        assert run_cnt == 1
+        EmptyTask.remove_event_handler(luigi.Event.START, handler)
+        build([task], local_scheduler=True)
+        assert run_cnt == 1
+
 
 #        A
 #      /   \
 #    B(1)  B(2)
 #     |     |
 #    C(1)  C(2)
 #     |  \  |  \
```

### Comparing `luigi-3.5.0/test/execution_summary_test.py` & `luigi-3.5.1/test/execution_summary_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/factorial_test.py` & `luigi-3.5.1/test/factorial_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/fib_test.py` & `luigi-3.5.1/test/fib_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/hdfs_client_test.py` & `luigi-3.5.1/test/hdfs_client_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/helpers.py` & `luigi-3.5.1/test/helpers.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/helpers_test.py` & `luigi-3.5.1/test/helpers_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/import_test.py` & `luigi-3.5.1/test/import_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/instance_test.py` & `luigi-3.5.1/test/instance_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/instance_wrap_test.py` & `luigi-3.5.1/test/instance_wrap_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/interface_test.py` & `luigi-3.5.1/test/interface_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,13 +200,13 @@
                                     **env_params)
 
 
 class CoreConfigTest(LuigiTestCase):
 
     @with_config({})
     def test_parallel_scheduling_processes_default(self):
-        self.assertEquals(0, core().parallel_scheduling_processes)
+        self.assertEqual(0, core().parallel_scheduling_processes)
 
     @with_config({'core': {'parallel-scheduling-processes': '1234'}})
     def test_parallel_scheduling_processes(self):
         from luigi.interface import core
-        self.assertEquals(1234, core().parallel_scheduling_processes)
+        self.assertEqual(1234, core().parallel_scheduling_processes)
```

### Comparing `luigi-3.5.0/test/list_parameter_test.py` & `luigi-3.5.1/test/list_parameter_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,24 +77,24 @@
         )
 
         # Check that the default value is validated
         with pytest.raises(ValidationError, match=r"'INVALID_ATTRIBUTE' is not of type 'number'"):
             a.normalize(["INVALID_ATTRIBUTE"])
 
         # Check that empty list is not valid
-        with pytest.raises(ValidationError, match=r"\[\] is too short"):
+        with pytest.raises(ValidationError):
             a.normalize([])
 
         # Check that valid lists work
         valid_list = [1, 2, 3]
         a.normalize(valid_list)
 
         # Check that invalid lists raise correct errors
         invalid_list_type = ["NOT AN INT"]
-        invalid_list_value = [-999, 999]
+        invalid_list_value = [-999, 4]
 
         with pytest.raises(ValidationError, match="'NOT AN INT' is not of type 'number'"):
             a.normalize(invalid_list_type)
 
         with pytest.raises(ValidationError, match="-999 is less than the minimum of 0"):
             a.normalize(invalid_list_value)
```

### Comparing `luigi-3.5.0/test/local_target_test.py` & `luigi-3.5.1/test/local_target_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/lock_test.py` & `luigi-3.5.1/test/lock_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/metrics_test.py` & `luigi-3.5.1/test/metrics_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/mock_test.py` & `luigi-3.5.1/test/mock_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/most_common_test.py` & `luigi-3.5.1/test/most_common_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/notifications_test.py` & `luigi-3.5.1/test/notifications_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/numerical_parameter_test.py` & `luigi-3.5.1/test/numerical_parameter_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/optional_parameter_test.py` & `luigi-3.5.1/test/optional_parameter_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,18 @@
             def run(self):
                 assert self.param == expected_value
                 assert self.empty_param is None
 
         # Test parsing empty string (should be None)
         self.assertIsNone(cls(**kwargs).parse(''))
 
+        # Test next_in_enumeration always returns None for summary
+        self.assertIsNone(TestConfig.param.next_in_enumeration(expected_value))
+        self.assertIsNone(TestConfig.param.next_in_enumeration(None))
+
         # Test that warning is raised only with bad type
         with mock.patch('luigi.parameter.warnings') as warnings:
             TestConfig()
             warnings.warn.assert_not_called()
 
         if cls != luigi.OptionalChoiceParameter:
             with mock.patch('luigi.parameter.warnings') as warnings:
```

### Comparing `luigi-3.5.0/test/other_module.py` & `luigi-3.5.1/test/other_module.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/parameter_test.py` & `luigi-3.5.1/test/parameter_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -529,14 +529,22 @@
         class Foo(luigi.Task):
             args = luigi.parameter.TupleParameter()
 
         p = luigi.parameter.TupleParameter()
         self.assertEqual(hash(Foo(args=(('foo', 'bar'), ('doge', 'wow'))).args),
                          hash(p.normalize(p.parse('(("foo", "bar"), ("doge", "wow"))'))))
 
+    def test_tuple_string_with_json(self):
+        class Foo(luigi.Task):
+            args = luigi.parameter.TupleParameter()
+
+        p = luigi.parameter.TupleParameter()
+        self.assertEqual(hash(Foo(args=('foo', 'bar')).args),
+                         hash(p.normalize(p.parse('["foo", "bar"]'))))
+
     def test_task(self):
         class Bar(luigi.Task):
             pass
 
         class Foo(luigi.Task):
             args = luigi.parameter.TaskParameter()
```

### Comparing `luigi-3.5.0/test/priority_test.py` & `luigi-3.5.1/test/priority_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/range_test.py` & `luigi-3.5.1/test/range_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/recursion_test.py` & `luigi-3.5.1/test/recursion_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/remote_scheduler_test.py` & `luigi-3.5.1/test/remote_scheduler_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/retcodes_test.py` & `luigi-3.5.1/test/retcodes_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/rpc_test.py` & `luigi-3.5.1/test/rpc_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/runtests.py` & `luigi-3.5.1/test/runtests.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/scheduler_api_test.py` & `luigi-3.5.1/test/scheduler_api_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/scheduler_message_test.py` & `luigi-3.5.1/test/scheduler_message_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/scheduler_parameter_visibilities_test.py` & `luigi-3.5.1/test/scheduler_parameter_visibilities_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/scheduler_test.py` & `luigi-3.5.1/test/scheduler_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/scheduler_visualisation_test.py` & `luigi-3.5.1/test/scheduler_visualisation_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/server_test.py` & `luigi-3.5.1/test/server_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/set_task_name_test.py` & `luigi-3.5.1/test/set_task_name_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/setup_logging_test.py` & `luigi-3.5.1/test/setup_logging_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/simulate_test.py` & `luigi-3.5.1/test/simulate_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/subtask_test.py` & `luigi-3.5.1/test/subtask_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/target_test.py` & `luigi-3.5.1/test/target_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/task_bulk_complete_test.py` & `luigi-3.5.1/test/task_bulk_complete_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/task_forwarded_attributes_test.py` & `luigi-3.5.1/test/task_forwarded_attributes_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/task_history_test.py` & `luigi-3.5.1/test/task_history_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/task_progress_percentage_test.py` & `luigi-3.5.1/test/task_progress_percentage_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/task_register_test.py` & `luigi-3.5.1/test/task_register_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/task_running_resources_test.py` & `luigi-3.5.1/test/task_running_resources_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/task_serialize_test.py` & `luigi-3.5.1/test/task_serialize_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/task_status_message_test.py` & `luigi-3.5.1/test/task_status_message_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/task_test.py` & `luigi-3.5.1/test/task_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -573,8 +573,8 @@
         class ReceivesClassKwargs(luigi.Task):
             def __init_subclass__(cls, x, **kwargs):
                 super(ReceivesClassKwargs, cls).__init_subclass__()
                 cls.x = x
 
         class Receiver(ReceivesClassKwargs, x=1):
             pass
-        self.assertEquals(Receiver.x, 1)
+        self.assertEqual(Receiver.x, 1)
```

### Comparing `luigi-3.5.0/test/test_sigpipe.py` & `luigi-3.5.1/test/test_sigpipe.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/test_ssh.py` & `luigi-3.5.1/test/test_ssh.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/util_previous_test.py` & `luigi-3.5.1/test/util_previous_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/util_test.py` & `luigi-3.5.1/test/util_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/visible_parameters_test.py` & `luigi-3.5.1/test/visible_parameters_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/worker_external_task_test.py` & `luigi-3.5.1/test/worker_external_task_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/worker_keep_alive_test.py` & `luigi-3.5.1/test/worker_keep_alive_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/worker_multiprocess_test.py` & `luigi-3.5.1/test/worker_multiprocess_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/worker_parallel_scheduling_test.py` & `luigi-3.5.1/test/worker_parallel_scheduling_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/worker_scheduler_com_test.py` & `luigi-3.5.1/test/worker_scheduler_com_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/worker_task_process_test.py` & `luigi-3.5.1/test/worker_task_process_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/worker_task_test.py` & `luigi-3.5.1/test/worker_task_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 import mock
 from psutil import Process
 from time import sleep
 
 import luigi
 import luigi.date_interval
 import luigi.notifications
+from luigi.mock import MockTarget
 from luigi.worker import TaskException, TaskProcess
 from luigi.scheduler import DONE, FAILED
 
 luigi.notifications.DEBUG = True
 
 
 class WorkerTaskTest(LuigiTestCase):
@@ -102,14 +103,50 @@
                 task.task_id,
                 FAILED,
                 StringContaining("finished running, but complete() is still returning false"),
                 [],
                 None
             ))
 
+    def test_fail_on_unfulfilled_dependencies(self):
+        class NeverCompleteTask(luigi.Task):
+            def complete(self):
+                return False
+
+        class A(NeverCompleteTask):
+            def output(self):
+                return []
+
+        class B(NeverCompleteTask):
+            def output(self):
+                return MockTarget("foo-B")
+
+        class C(NeverCompleteTask):
+            def output(self):
+                return [MockTarget("foo-C1"), MockTarget("foo-C2")]
+
+        class Main(NeverCompleteTask):
+            def requires(self):
+                return [A(), B(), C()]
+
+        task = Main()
+        result_queue = multiprocessing.Queue()
+        task_process = TaskProcess(task, 1, result_queue, mock.Mock())
+
+        with mock.patch.object(result_queue, 'put') as mock_put:
+            task_process.run()
+            expected_missing = [A().task_id, f"{B().task_id} (foo-B)", f"{C().task_id} (foo-C1, foo-C2)"]
+            mock_put.assert_called_once_with((
+                task.task_id,
+                FAILED,
+                StringContaining(f"Unfulfilled dependencies at run time: {', '.join(expected_missing)}"),
+                expected_missing,
+                [],
+            ))
+
     def test_cleanup_children_on_terminate(self):
         """
         Subprocesses spawned by tasks should be terminated on terminate
         """
         class HangingSubprocessTask(luigi.Task):
             def run(self):
                 python = sys.executable
```

### Comparing `luigi-3.5.0/test/worker_test.py` & `luigi-3.5.1/test/worker_test.py`

 * *Files identical despite different names*

### Comparing `luigi-3.5.0/test/wrap_test.py` & `luigi-3.5.1/test/wrap_test.py`

 * *Files identical despite different names*

