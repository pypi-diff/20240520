# Comparing `tmp/nucliadb-4.0.0.post520-py3-none-any.whl.zip` & `tmp/nucliadb-4.0.0.post522-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,462 +1,463 @@
-Zip file size: 763442 bytes, number of entries: 460
--rw-r--r--  2.0 unx     1135 b- defN 24-May-20 10:15 migrations/0001_bootstrap.py
--rw-r--r--  2.0 unx     1177 b- defN 24-May-20 10:15 migrations/0002_rollover_shards.py
--rw-r--r--  2.0 unx     2436 b- defN 24-May-20 10:15 migrations/0003_allfields_key.py
--rw-r--r--  2.0 unx     1177 b- defN 24-May-20 10:15 migrations/0004_rollover_shards.py
--rw-r--r--  2.0 unx     1177 b- defN 24-May-20 10:15 migrations/0005_rollover_shards.py
--rw-r--r--  2.0 unx     1024 b- defN 24-May-20 10:15 migrations/0006_rollover_shards.py
--rw-r--r--  2.0 unx     1301 b- defN 24-May-20 10:15 migrations/0008_cleanup_leftover_rollover_metadata.py
--rw-r--r--  2.0 unx     1378 b- defN 24-May-20 10:15 migrations/0009_upgrade_relations_and_texts_to_v2.py
--rw-r--r--  2.0 unx     1610 b- defN 24-May-20 10:15 migrations/0010_fix_corrupt_indexes.py
--rw-r--r--  2.0 unx     1843 b- defN 24-May-20 10:15 migrations/0011_materialize_labelset_ids.py
--rw-r--r--  2.0 unx     1443 b- defN 24-May-20 10:15 migrations/0012_rollover_shards.py
--rw-r--r--  2.0 unx     1024 b- defN 24-May-20 10:15 migrations/0013_rollover_shards.py
--rw-r--r--  2.0 unx     1382 b- defN 24-May-20 10:15 migrations/0014_rollover_shards.py
--rw-r--r--  2.0 unx     1462 b- defN 24-May-20 10:15 migrations/0015_targeted_rollover.py
--rw-r--r--  2.0 unx     2506 b- defN 24-May-20 10:15 migrations/0016_upgrade_to_paragraphs_v2.py
--rw-r--r--  2.0 unx     2100 b- defN 24-May-20 10:15 migrations/0017_multiple_writable_shards.py
--rw-r--r--  2.0 unx     2264 b- defN 24-May-20 10:15 migrations/0018_purge_orphan_kbslugs.py
--rw-r--r--  2.0 unx     2506 b- defN 24-May-20 10:15 migrations/0019_upgrade_to_paragraphs_v3.py
--rw-r--r--  2.0 unx     3282 b- defN 24-May-20 10:15 migrations/0020_drain_nodes_from_cluster.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-20 10:15 migrations/__init__.py
--rw-r--r--  2.0 unx      891 b- defN 24-May-20 10:15 nucliadb/__init__.py
--rw-r--r--  2.0 unx     3733 b- defN 24-May-20 10:15 nucliadb/health.py
--rw-r--r--  2.0 unx    11639 b- defN 24-May-20 10:15 nucliadb/learning_proxy.py
--rw-r--r--  2.0 unx     4806 b- defN 24-May-20 10:15 nucliadb/metrics_exporter.py
--rw-r--r--  2.0 unx     2272 b- defN 24-May-20 10:15 nucliadb/openapi.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-20 10:15 nucliadb/py.typed
--rw-r--r--  2.0 unx      835 b- defN 24-May-20 10:15 nucliadb/common/__init__.py
--rw-r--r--  2.0 unx     5022 b- defN 24-May-20 10:15 nucliadb/common/locking.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-20 10:15 nucliadb/common/cluster/__init__.py
--rw-r--r--  2.0 unx     4971 b- defN 24-May-20 10:15 nucliadb/common/cluster/base.py
--rw-r--r--  2.0 unx     1495 b- defN 24-May-20 10:15 nucliadb/common/cluster/exceptions.py
--rw-r--r--  2.0 unx     3793 b- defN 24-May-20 10:15 nucliadb/common/cluster/grpc_node_dummy.py
--rw-r--r--  2.0 unx     3429 b- defN 24-May-20 10:15 nucliadb/common/cluster/index_node.py
--rw-r--r--  2.0 unx    22091 b- defN 24-May-20 10:15 nucliadb/common/cluster/manager.py
--rw-r--r--  2.0 unx     8590 b- defN 24-May-20 10:15 nucliadb/common/cluster/rebalance.py
--rw-r--r--  2.0 unx    20209 b- defN 24-May-20 10:15 nucliadb/common/cluster/rollover.py
--rw-r--r--  2.0 unx     3016 b- defN 24-May-20 10:15 nucliadb/common/cluster/settings.py
--rw-r--r--  2.0 unx     5713 b- defN 24-May-20 10:15 nucliadb/common/cluster/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-20 10:15 nucliadb/common/cluster/discovery/__init__.py
--rw-r--r--  2.0 unx     6553 b- defN 24-May-20 10:15 nucliadb/common/cluster/discovery/base.py
--rw-r--r--  2.0 unx    12515 b- defN 24-May-20 10:15 nucliadb/common/cluster/discovery/k8s.py
--rw-r--r--  2.0 unx     1957 b- defN 24-May-20 10:15 nucliadb/common/cluster/discovery/manual.py
--rw-r--r--  2.0 unx     1737 b- defN 24-May-20 10:15 nucliadb/common/cluster/discovery/single.py
--rw-r--r--  2.0 unx     1139 b- defN 24-May-20 10:15 nucliadb/common/cluster/discovery/types.py
--rw-r--r--  2.0 unx     2548 b- defN 24-May-20 10:15 nucliadb/common/cluster/discovery/utils.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-20 10:15 nucliadb/common/cluster/standalone/__init__.py
--rw-r--r--  2.0 unx    13707 b- defN 24-May-20 10:15 nucliadb/common/cluster/standalone/grpc_node_binding.py
--rw-r--r--  2.0 unx     4683 b- defN 24-May-20 10:15 nucliadb/common/cluster/standalone/index_node.py
--rw-r--r--  2.0 unx     3444 b- defN 24-May-20 10:15 nucliadb/common/cluster/standalone/service.py
--rw-r--r--  2.0 unx     3545 b- defN 24-May-20 10:15 nucliadb/common/cluster/standalone/utils.py
--rw-r--r--  2.0 unx     3440 b- defN 24-May-20 10:15 nucliadb/common/context/__init__.py
--rw-r--r--  2.0 unx     1628 b- defN 24-May-20 10:15 nucliadb/common/context/fastapi.py
--rw-r--r--  2.0 unx     1813 b- defN 24-May-20 10:15 nucliadb/common/datamanagers/__init__.py
--rw-r--r--  2.0 unx     1451 b- defN 24-May-20 10:15 nucliadb/common/datamanagers/cluster.py
--rw-r--r--  2.0 unx     5383 b- defN 24-May-20 10:15 nucliadb/common/datamanagers/entities.py
--rw-r--r--  2.0 unx      883 b- defN 24-May-20 10:15 nucliadb/common/datamanagers/exceptions.py
--rw-r--r--  2.0 unx     3994 b- defN 24-May-20 10:15 nucliadb/common/datamanagers/kb.py
--rw-r--r--  2.0 unx     5389 b- defN 24-May-20 10:15 nucliadb/common/datamanagers/labels.py
--rw-r--r--  2.0 unx     1599 b- defN 24-May-20 10:15 nucliadb/common/datamanagers/processing.py
--rw-r--r--  2.0 unx     8719 b- defN 24-May-20 10:15 nucliadb/common/datamanagers/resources.py
--rw-r--r--  2.0 unx     5634 b- defN 24-May-20 10:15 nucliadb/common/datamanagers/rollover.py
--rw-r--r--  2.0 unx     1631 b- defN 24-May-20 10:15 nucliadb/common/datamanagers/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-20 10:15 nucliadb/common/http_clients/__init__.py
--rw-r--r--  2.0 unx     2146 b- defN 24-May-20 10:15 nucliadb/common/http_clients/auth.py
--rw-r--r--  2.0 unx     1100 b- defN 24-May-20 10:15 nucliadb/common/http_clients/exceptions.py
--rw-r--r--  2.0 unx     7155 b- defN 24-May-20 10:15 nucliadb/common/http_clients/processing.py
--rw-r--r--  2.0 unx     1540 b- defN 24-May-20 10:15 nucliadb/common/http_clients/pypi.py
--rw-r--r--  2.0 unx     1551 b- defN 24-May-20 10:15 nucliadb/common/http_clients/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-20 10:15 nucliadb/common/maindb/__init__.py
--rw-r--r--  2.0 unx     3449 b- defN 24-May-20 10:15 nucliadb/common/maindb/driver.py
--rw-r--r--  2.0 unx      946 b- defN 24-May-20 10:15 nucliadb/common/maindb/exceptions.py
--rw-r--r--  2.0 unx     6769 b- defN 24-May-20 10:15 nucliadb/common/maindb/local.py
--rw-r--r--  2.0 unx     8391 b- defN 24-May-20 10:15 nucliadb/common/maindb/pg.py
--rw-r--r--  2.0 unx     6053 b- defN 24-May-20 10:15 nucliadb/common/maindb/redis.py
--rw-r--r--  2.0 unx    14502 b- defN 24-May-20 10:15 nucliadb/common/maindb/tikv.py
--rw-r--r--  2.0 unx     4167 b- defN 24-May-20 10:15 nucliadb/common/maindb/utils.py
--rw-r--r--  2.0 unx      932 b- defN 24-May-20 10:15 nucliadb/export_import/__init__.py
--rw-r--r--  2.0 unx     6171 b- defN 24-May-20 10:15 nucliadb/export_import/datamanager.py
--rw-r--r--  2.0 unx     1949 b- defN 24-May-20 10:15 nucliadb/export_import/exceptions.py
--rw-r--r--  2.0 unx     7116 b- defN 24-May-20 10:15 nucliadb/export_import/exporter.py
--rw-r--r--  2.0 unx     4258 b- defN 24-May-20 10:15 nucliadb/export_import/importer.py
--rw-r--r--  2.0 unx     2063 b- defN 24-May-20 10:15 nucliadb/export_import/models.py
--rw-r--r--  2.0 unx     2571 b- defN 24-May-20 10:15 nucliadb/export_import/tasks.py
--rw-r--r--  2.0 unx    19401 b- defN 24-May-20 10:15 nucliadb/export_import/utils.py
--rw-r--r--  2.0 unx     1011 b- defN 24-May-20 10:15 nucliadb/ingest/__init__.py
--rw-r--r--  2.0 unx     7277 b- defN 24-May-20 10:15 nucliadb/ingest/app.py
--rw-r--r--  2.0 unx     1005 b- defN 24-May-20 10:15 nucliadb/ingest/cache.py
--rw-r--r--  2.0 unx     2484 b- defN 24-May-20 10:15 nucliadb/ingest/partitions.py
--rw-r--r--  2.0 unx    19555 b- defN 24-May-20 10:15 nucliadb/ingest/processing.py
--rw-r--r--  2.0 unx    20277 b- defN 24-May-20 10:15 nucliadb/ingest/serialize.py
--rw-r--r--  2.0 unx     3207 b- defN 24-May-20 10:15 nucliadb/ingest/settings.py
--rw-r--r--  2.0 unx     2314 b- defN 24-May-20 10:15 nucliadb/ingest/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-20 10:15 nucliadb/ingest/consumer/__init__.py
--rw-r--r--  2.0 unx    11563 b- defN 24-May-20 10:15 nucliadb/ingest/consumer/auditing.py
--rw-r--r--  2.0 unx    12174 b- defN 24-May-20 10:15 nucliadb/ingest/consumer/consumer.py
--rw-r--r--  2.0 unx     3788 b- defN 24-May-20 10:15 nucliadb/ingest/consumer/materializer.py
--rw-r--r--  2.0 unx     1075 b- defN 24-May-20 10:15 nucliadb/ingest/consumer/metrics.py
--rw-r--r--  2.0 unx     9543 b- defN 24-May-20 10:15 nucliadb/ingest/consumer/pull.py
--rw-r--r--  2.0 unx     6935 b- defN 24-May-20 10:15 nucliadb/ingest/consumer/service.py
--rw-r--r--  2.0 unx     4331 b- defN 24-May-20 10:15 nucliadb/ingest/consumer/shard_creator.py
--rw-r--r--  2.0 unx     2656 b- defN 24-May-20 10:15 nucliadb/ingest/consumer/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-20 10:15 nucliadb/ingest/fields/__init__.py
--rw-r--r--  2.0 unx    18433 b- defN 24-May-20 10:15 nucliadb/ingest/fields/base.py
--rw-r--r--  2.0 unx     6516 b- defN 24-May-20 10:15 nucliadb/ingest/fields/conversation.py
--rw-r--r--  2.0 unx     1223 b- defN 24-May-20 10:15 nucliadb/ingest/fields/date.py
--rw-r--r--  2.0 unx     1205 b- defN 24-May-20 10:15 nucliadb/ingest/fields/exceptions.py
--rw-r--r--  2.0 unx     5159 b- defN 24-May-20 10:15 nucliadb/ingest/fields/file.py
--rw-r--r--  2.0 unx     1547 b- defN 24-May-20 10:15 nucliadb/ingest/fields/generic.py
--rw-r--r--  2.0 unx     1235 b- defN 24-May-20 10:15 nucliadb/ingest/fields/keywordset.py
--rw-r--r--  2.0 unx     2250 b- defN 24-May-20 10:15 nucliadb/ingest/fields/layout.py
--rw-r--r--  2.0 unx     4531 b- defN 24-May-20 10:15 nucliadb/ingest/fields/link.py
--rw-r--r--  2.0 unx     1319 b- defN 24-May-20 10:15 nucliadb/ingest/fields/text.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-20 10:15 nucliadb/ingest/orm/__init__.py
--rw-r--r--  2.0 unx    28448 b- defN 24-May-20 10:15 nucliadb/ingest/orm/brain.py
--rw-r--r--  2.0 unx    15758 b- defN 24-May-20 10:15 nucliadb/ingest/orm/entities.py
--rw-r--r--  2.0 unx     1279 b- defN 24-May-20 10:15 nucliadb/ingest/orm/exceptions.py
--rw-r--r--  2.0 unx    17167 b- defN 24-May-20 10:15 nucliadb/ingest/orm/knowledgebox.py
--rw-r--r--  2.0 unx     1096 b- defN 24-May-20 10:15 nucliadb/ingest/orm/metrics.py
--rw-r--r--  2.0 unx    60444 b- defN 24-May-20 10:15 nucliadb/ingest/orm/resource.py
--rw-r--r--  2.0 unx     1739 b- defN 24-May-20 10:15 nucliadb/ingest/orm/synonyms.py
--rw-r--r--  2.0 unx     3683 b- defN 24-May-20 10:15 nucliadb/ingest/orm/utils.py
--rw-r--r--  2.0 unx    26420 b- defN 24-May-20 10:15 nucliadb/ingest/orm/processor/__init__.py
--rw-r--r--  2.0 unx     1690 b- defN 24-May-20 10:15 nucliadb/ingest/orm/processor/sequence_manager.py
--rw-r--r--  2.0 unx     2057 b- defN 24-May-20 10:15 nucliadb/ingest/service/__init__.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-20 10:15 nucliadb/ingest/service/exceptions.py
--rw-r--r--  2.0 unx    33193 b- defN 24-May-20 10:15 nucliadb/ingest/service/writer.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-20 10:15 nucliadb/ingest/tests/__init__.py
--rw-r--r--  2.0 unx     1157 b- defN 24-May-20 10:15 nucliadb/ingest/tests/conftest.py
--rw-r--r--  2.0 unx    24060 b- defN 24-May-20 10:15 nucliadb/ingest/tests/fixtures.py
--rw-r--r--  2.0 unx    62843 b- defN 24-May-20 10:15 nucliadb/ingest/tests/vectors.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-20 10:15 nucliadb/ingest/tests/integration/__init__.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-20 10:15 nucliadb/ingest/tests/integration/consumer/__init__.py
--rw-r--r--  2.0 unx     2549 b- defN 24-May-20 10:15 nucliadb/ingest/tests/integration/consumer/test_auditing.py
--rw-r--r--  2.0 unx     2591 b- defN 24-May-20 10:15 nucliadb/ingest/tests/integration/consumer/test_materializer.py
--rw-r--r--  2.0 unx     4470 b- defN 24-May-20 10:15 nucliadb/ingest/tests/integration/consumer/test_pull.py
--rw-r--r--  2.0 unx     2763 b- defN 24-May-20 10:15 nucliadb/ingest/tests/integration/consumer/test_service.py
--rw-r--r--  2.0 unx     2019 b- defN 24-May-20 10:15 nucliadb/ingest/tests/integration/consumer/test_shard_creator.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-20 10:15 nucliadb/ingest/tests/integration/ingest/__init__.py
--rw-r--r--  2.0 unx    27336 b- defN 24-May-20 10:15 nucliadb/ingest/tests/integration/ingest/test_ingest.py
--rw-r--r--  2.0 unx     3040 b- defN 24-May-20 10:15 nucliadb/ingest/tests/integration/ingest/test_processing_engine.py
--rw-r--r--  2.0 unx     8586 b- defN 24-May-20 10:15 nucliadb/ingest/tests/integration/ingest/test_relations.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-20 10:15 nucliadb/ingest/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1189 b- defN 24-May-20 10:15 nucliadb/ingest/tests/unit/test_cache.py
--rw-r--r--  2.0 unx     1432 b- defN 24-May-20 10:15 nucliadb/ingest/tests/unit/test_partitions.py
--rw-r--r--  2.0 unx     5807 b- defN 24-May-20 10:15 nucliadb/ingest/tests/unit/test_processing.py
--rw-r--r--  2.0 unx      978 b- defN 24-May-20 10:15 nucliadb/ingest/tests/unit/test_settings.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-20 10:15 nucliadb/ingest/tests/unit/consumer/__init__.py
--rw-r--r--  2.0 unx     4004 b- defN 24-May-20 10:15 nucliadb/ingest/tests/unit/consumer/test_auditing.py
--rw-r--r--  2.0 unx     2472 b- defN 24-May-20 10:15 nucliadb/ingest/tests/unit/consumer/test_consumer.py
--rw-r--r--  2.0 unx     2063 b- defN 24-May-20 10:15 nucliadb/ingest/tests/unit/consumer/test_pull.py
--rw-r--r--  2.0 unx     4140 b- defN 24-May-20 10:15 nucliadb/ingest/tests/unit/consumer/test_shard_creator.py
--rw-r--r--  2.0 unx     1934 b- defN 24-May-20 10:15 nucliadb/ingest/tests/unit/consumer/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-20 10:15 nucliadb/ingest/tests/unit/orm/__init__.py
--rw-r--r--  2.0 unx     9876 b- defN 24-May-20 10:15 nucliadb/ingest/tests/unit/orm/test_brain.py
--rw-r--r--  2.0 unx     2435 b- defN 24-May-20 10:15 nucliadb/ingest/tests/unit/orm/test_brain_vectors.py
--rw-r--r--  2.0 unx     1174 b- defN 24-May-20 10:15 nucliadb/ingest/tests/unit/orm/test_orm_utils.py
--rw-r--r--  2.0 unx     4045 b- defN 24-May-20 10:15 nucliadb/ingest/tests/unit/orm/test_processor.py
--rw-r--r--  2.0 unx    11033 b- defN 24-May-20 10:15 nucliadb/ingest/tests/unit/orm/test_resource.py
--rw-r--r--  2.0 unx     2216 b- defN 24-May-20 10:15 nucliadb/middleware/__init__.py
--rw-r--r--  2.0 unx     3912 b- defN 24-May-20 10:15 nucliadb/middleware/transaction.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-20 10:15 nucliadb/migrator/__init__.py
--rw-r--r--  2.0 unx     2119 b- defN 24-May-20 10:15 nucliadb/migrator/command.py
--rw-r--r--  2.0 unx     1334 b- defN 24-May-20 10:15 nucliadb/migrator/context.py
--rw-r--r--  2.0 unx     5104 b- defN 24-May-20 10:15 nucliadb/migrator/datamanager.py
--rw-r--r--  2.0 unx      889 b- defN 24-May-20 10:15 nucliadb/migrator/exceptions.py
--rw-r--r--  2.0 unx     9370 b- defN 24-May-20 10:15 nucliadb/migrator/migrator.py
--rw-r--r--  2.0 unx     1145 b- defN 24-May-20 10:15 nucliadb/migrator/models.py
--rw-r--r--  2.0 unx     1144 b- defN 24-May-20 10:15 nucliadb/migrator/settings.py
--rw-r--r--  2.0 unx     2346 b- defN 24-May-20 10:15 nucliadb/migrator/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-20 10:15 nucliadb/models/__init__.py
--rw-r--r--  2.0 unx     1599 b- defN 24-May-20 10:15 nucliadb/models/responses.py
--rw-r--r--  2.0 unx     6041 b- defN 24-May-20 10:15 nucliadb/purge/__init__.py
--rw-r--r--  2.0 unx     9364 b- defN 24-May-20 10:15 nucliadb/purge/orphan_shards.py
--rw-r--r--  2.0 unx     1328 b- defN 24-May-20 10:15 nucliadb/reader/__init__.py
--rw-r--r--  2.0 unx     3709 b- defN 24-May-20 10:15 nucliadb/reader/app.py
--rw-r--r--  2.0 unx     1366 b- defN 24-May-20 10:15 nucliadb/reader/lifecycle.py
--rw-r--r--  2.0 unx     1031 b- defN 24-May-20 10:15 nucliadb/reader/openapi.py
--rw-r--r--  2.0 unx     1447 b- defN 24-May-20 10:15 nucliadb/reader/run.py
--rw-r--r--  2.0 unx      872 b- defN 24-May-20 10:15 nucliadb/reader/api/__init__.py
--rw-r--r--  2.0 unx     2458 b- defN 24-May-20 10:15 nucliadb/reader/api/models.py
--rw-r--r--  2.0 unx     1110 b- defN 24-May-20 10:15 nucliadb/reader/api/v1/__init__.py
--rw-r--r--  2.0 unx    12392 b- defN 24-May-20 10:15 nucliadb/reader/api/v1/download.py
--rw-r--r--  2.0 unx     6459 b- defN 24-May-20 10:15 nucliadb/reader/api/v1/export_import.py
--rw-r--r--  2.0 unx     3641 b- defN 24-May-20 10:15 nucliadb/reader/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     2099 b- defN 24-May-20 10:15 nucliadb/reader/api/v1/learning_collector.py
--rw-r--r--  2.0 unx     4472 b- defN 24-May-20 10:15 nucliadb/reader/api/v1/learning_config.py
--rw-r--r--  2.0 unx    13951 b- defN 24-May-20 10:15 nucliadb/reader/api/v1/resource.py
--rw-r--r--  2.0 unx     1011 b- defN 24-May-20 10:15 nucliadb/reader/api/v1/router.py
--rw-r--r--  2.0 unx    12399 b- defN 24-May-20 10:15 nucliadb/reader/api/v1/services.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-20 10:15 nucliadb/reader/reader/__init__.py
--rw-r--r--  2.0 unx     8155 b- defN 24-May-20 10:15 nucliadb/reader/reader/notifications.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-20 10:15 nucliadb/reader/tests/__init__.py
--rw-r--r--  2.0 unx     1224 b- defN 24-May-20 10:15 nucliadb/reader/tests/conftest.py
--rw-r--r--  2.0 unx     4345 b- defN 24-May-20 10:15 nucliadb/reader/tests/fixtures.py
--rw-r--r--  2.0 unx     2748 b- defN 24-May-20 10:15 nucliadb/reader/tests/test_list_resources.py
--rw-r--r--  2.0 unx    10199 b- defN 24-May-20 10:15 nucliadb/reader/tests/test_reader_file_download.py
--rw-r--r--  2.0 unx    10586 b- defN 24-May-20 10:15 nucliadb/reader/tests/test_reader_resource.py
--rw-r--r--  2.0 unx     6535 b- defN 24-May-20 10:15 nucliadb/reader/tests/test_reader_resource_field.py
--rw-r--r--  2.0 unx     1535 b- defN 24-May-20 10:15 nucliadb/search/__init__.py
--rw-r--r--  2.0 unx     4905 b- defN 24-May-20 10:15 nucliadb/search/app.py
--rw-r--r--  2.0 unx     1956 b- defN 24-May-20 10:15 nucliadb/search/lifecycle.py
--rw-r--r--  2.0 unx     1016 b- defN 24-May-20 10:15 nucliadb/search/openapi.py
--rw-r--r--  2.0 unx    20665 b- defN 24-May-20 10:15 nucliadb/search/predict.py
--rw-r--r--  2.0 unx     1402 b- defN 24-May-20 10:15 nucliadb/search/run.py
--rw-r--r--  2.0 unx     1193 b- defN 24-May-20 10:15 nucliadb/search/settings.py
--rw-r--r--  2.0 unx     1037 b- defN 24-May-20 10:15 nucliadb/search/utilities.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-20 10:15 nucliadb/search/api/__init__.py
--rw-r--r--  2.0 unx     1298 b- defN 24-May-20 10:15 nucliadb/search/api/v1/__init__.py
--rw-r--r--  2.0 unx     3534 b- defN 24-May-20 10:15 nucliadb/search/api/v1/ask.py
--rw-r--r--  2.0 unx     9493 b- defN 24-May-20 10:15 nucliadb/search/api/v1/chat.py
--rw-r--r--  2.0 unx     2668 b- defN 24-May-20 10:15 nucliadb/search/api/v1/feedback.py
--rw-r--r--  2.0 unx     8795 b- defN 24-May-20 10:15 nucliadb/search/api/v1/find.py
--rw-r--r--  2.0 unx     6938 b- defN 24-May-20 10:15 nucliadb/search/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     3047 b- defN 24-May-20 10:15 nucliadb/search/api/v1/predict_proxy.py
--rw-r--r--  2.0 unx      988 b- defN 24-May-20 10:15 nucliadb/search/api/v1/router.py
--rw-r--r--  2.0 unx    19262 b- defN 24-May-20 10:15 nucliadb/search/api/v1/search.py
--rw-r--r--  2.0 unx     5970 b- defN 24-May-20 10:15 nucliadb/search/api/v1/suggest.py
--rw-r--r--  2.0 unx     2499 b- defN 24-May-20 10:15 nucliadb/search/api/v1/summarize.py
--rw-r--r--  2.0 unx     1434 b- defN 24-May-20 10:15 nucliadb/search/api/v1/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-20 10:15 nucliadb/search/api/v1/resource/__init__.py
--rw-r--r--  2.0 unx     4064 b- defN 24-May-20 10:15 nucliadb/search/api/v1/resource/ask.py
--rw-r--r--  2.0 unx     5821 b- defN 24-May-20 10:15 nucliadb/search/api/v1/resource/chat.py
--rw-r--r--  2.0 unx     5303 b- defN 24-May-20 10:15 nucliadb/search/api/v1/resource/search.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-20 10:15 nucliadb/search/requesters/__init__.py
--rw-r--r--  2.0 unx     9111 b- defN 24-May-20 10:15 nucliadb/search/requesters/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-20 10:15 nucliadb/search/search/__init__.py
--rw-r--r--  2.0 unx     2746 b- defN 24-May-20 10:15 nucliadb/search/search/cache.py
--rw-r--r--  2.0 unx     1154 b- defN 24-May-20 10:15 nucliadb/search/search/exceptions.py
--rw-r--r--  2.0 unx     5465 b- defN 24-May-20 10:15 nucliadb/search/search/fetch.py
--rw-r--r--  2.0 unx     6513 b- defN 24-May-20 10:15 nucliadb/search/search/filters.py
--rw-r--r--  2.0 unx     4612 b- defN 24-May-20 10:15 nucliadb/search/search/find.py
--rw-r--r--  2.0 unx    17152 b- defN 24-May-20 10:15 nucliadb/search/search/find_merge.py
--rw-r--r--  2.0 unx    21282 b- defN 24-May-20 10:15 nucliadb/search/search/merge.py
--rw-r--r--  2.0 unx     1130 b- defN 24-May-20 10:15 nucliadb/search/search/metrics.py
--rw-r--r--  2.0 unx     8698 b- defN 24-May-20 10:15 nucliadb/search/search/paragraphs.py
--rw-r--r--  2.0 unx     3026 b- defN 24-May-20 10:15 nucliadb/search/search/predict_proxy.py
--rw-r--r--  2.0 unx    31127 b- defN 24-May-20 10:15 nucliadb/search/search/query.py
--rw-r--r--  2.0 unx     3018 b- defN 24-May-20 10:15 nucliadb/search/search/shards.py
--rw-r--r--  2.0 unx     5101 b- defN 24-May-20 10:15 nucliadb/search/search/summarize.py
--rw-r--r--  2.0 unx     2438 b- defN 24-May-20 10:15 nucliadb/search/search/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-20 10:15 nucliadb/search/search/chat/__init__.py
--rw-r--r--  2.0 unx    16676 b- defN 24-May-20 10:15 nucliadb/search/search/chat/ask.py
--rw-r--r--  2.0 unx     2058 b- defN 24-May-20 10:15 nucliadb/search/search/chat/images.py
--rw-r--r--  2.0 unx    20793 b- defN 24-May-20 10:15 nucliadb/search/search/chat/prompt.py
--rw-r--r--  2.0 unx    17543 b- defN 24-May-20 10:15 nucliadb/search/search/chat/query.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-20 10:15 nucliadb/search/tests/__init__.py
--rw-r--r--  2.0 unx     1295 b- defN 24-May-20 10:15 nucliadb/search/tests/conftest.py
--rw-r--r--  2.0 unx     6578 b- defN 24-May-20 10:15 nucliadb/search/tests/fixtures.py
--rw-r--r--  2.0 unx    15480 b- defN 24-May-20 10:15 nucliadb/search/tests/node.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-20 10:15 nucliadb/search/tests/unit/__init__.py
--rw-r--r--  2.0 unx     2649 b- defN 24-May-20 10:15 nucliadb/search/tests/unit/test_app.py
--rw-r--r--  2.0 unx     3374 b- defN 24-May-20 10:15 nucliadb/search/tests/unit/test_find_merge.py
--rw-r--r--  2.0 unx     1400 b- defN 24-May-20 10:15 nucliadb/search/tests/unit/test_merge.py
--rw-r--r--  2.0 unx    15721 b- defN 24-May-20 10:15 nucliadb/search/tests/unit/test_predict.py
--rw-r--r--  2.0 unx     1328 b- defN 24-May-20 10:15 nucliadb/search/tests/unit/test_run.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-20 10:15 nucliadb/search/tests/unit/api/__init__.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-20 10:15 nucliadb/search/tests/unit/api/v1/__init__.py
--rw-r--r--  2.0 unx     3759 b- defN 24-May-20 10:15 nucliadb/search/tests/unit/api/v1/test_ask.py
--rw-r--r--  2.0 unx     2966 b- defN 24-May-20 10:15 nucliadb/search/tests/unit/api/v1/test_chat.py
--rw-r--r--  2.0 unx     2865 b- defN 24-May-20 10:15 nucliadb/search/tests/unit/api/v1/test_predict_proxy.py
--rw-r--r--  2.0 unx     2901 b- defN 24-May-20 10:15 nucliadb/search/tests/unit/api/v1/test_summarize.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-20 10:15 nucliadb/search/tests/unit/api/v1/resource/__init__.py
--rw-r--r--  2.0 unx     3040 b- defN 24-May-20 10:15 nucliadb/search/tests/unit/api/v1/resource/test_chat.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-20 10:15 nucliadb/search/tests/unit/search/__init__.py
--rw-r--r--  2.0 unx     8586 b- defN 24-May-20 10:15 nucliadb/search/tests/unit/search/test_chat_prompt.py
--rw-r--r--  2.0 unx     3736 b- defN 24-May-20 10:15 nucliadb/search/tests/unit/search/test_fetch.py
--rw-r--r--  2.0 unx     4306 b- defN 24-May-20 10:15 nucliadb/search/tests/unit/search/test_filters.py
--rw-r--r--  2.0 unx     4492 b- defN 24-May-20 10:15 nucliadb/search/tests/unit/search/test_paragraphs.py
--rw-r--r--  2.0 unx     3496 b- defN 24-May-20 10:15 nucliadb/search/tests/unit/search/test_predict_proxy.py
--rw-r--r--  2.0 unx     5121 b- defN 24-May-20 10:15 nucliadb/search/tests/unit/search/test_query.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-20 10:15 nucliadb/search/tests/unit/search/requesters/__init__.py
--rw-r--r--  2.0 unx     6455 b- defN 24-May-20 10:15 nucliadb/search/tests/unit/search/requesters/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-20 10:15 nucliadb/search/tests/unit/search/search/__init__.py
--rw-r--r--  2.0 unx     1759 b- defN 24-May-20 10:15 nucliadb/search/tests/unit/search/search/test_shards.py
--rw-r--r--  2.0 unx     2511 b- defN 24-May-20 10:15 nucliadb/search/tests/unit/search/search/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-20 10:15 nucliadb/standalone/__init__.py
--rw-r--r--  2.0 unx     6746 b- defN 24-May-20 10:15 nucliadb/standalone/api_router.py
--rw-r--r--  2.0 unx     5763 b- defN 24-May-20 10:15 nucliadb/standalone/app.py
--rw-r--r--  2.0 unx     7800 b- defN 24-May-20 10:15 nucliadb/standalone/auth.py
--rw-r--r--  2.0 unx     5313 b- defN 24-May-20 10:15 nucliadb/standalone/config.py
--rw-r--r--  2.0 unx     6986 b- defN 24-May-20 10:15 nucliadb/standalone/introspect.py
--rw-r--r--  2.0 unx     2488 b- defN 24-May-20 10:15 nucliadb/standalone/lifecycle.py
--rw-r--r--  2.0 unx     1980 b- defN 24-May-20 10:15 nucliadb/standalone/migrations.py
--rw-r--r--  2.0 unx     1322 b- defN 24-May-20 10:15 nucliadb/standalone/purge.py
--rw-r--r--  2.0 unx     5429 b- defN 24-May-20 10:15 nucliadb/standalone/run.py
--rw-r--r--  2.0 unx     5822 b- defN 24-May-20 10:15 nucliadb/standalone/settings.py
--rw-r--r--  2.0 unx     3132 b- defN 24-May-20 10:15 nucliadb/standalone/versions.py
--rw-r--r--  2.0 unx     2285 b- defN 24-May-20 10:15 nucliadb/standalone/static/favicon.ico
--rw-r--r--  2.0 unx     3833 b- defN 24-May-20 10:15 nucliadb/standalone/static/index.html
--rw-r--r--  2.0 unx     2639 b- defN 24-May-20 10:15 nucliadb/standalone/static/logo.svg
--rw-r--r--  2.0 unx      835 b- defN 24-May-20 10:15 nucliadb/standalone/tests/__init__.py
--rw-r--r--  2.0 unx     1294 b- defN 24-May-20 10:15 nucliadb/standalone/tests/conftest.py
--rw-r--r--  2.0 unx     1319 b- defN 24-May-20 10:15 nucliadb/standalone/tests/fixtures.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-20 10:15 nucliadb/standalone/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1722 b- defN 24-May-20 10:15 nucliadb/standalone/tests/unit/test_api_router.py
--rw-r--r--  2.0 unx     5509 b- defN 24-May-20 10:15 nucliadb/standalone/tests/unit/test_auth.py
--rw-r--r--  2.0 unx     1334 b- defN 24-May-20 10:15 nucliadb/standalone/tests/unit/test_introspect.py
--rw-r--r--  2.0 unx     1845 b- defN 24-May-20 10:15 nucliadb/standalone/tests/unit/test_migrations.py
--rw-r--r--  2.0 unx     1546 b- defN 24-May-20 10:15 nucliadb/standalone/tests/unit/test_run.py
--rw-r--r--  2.0 unx     1972 b- defN 24-May-20 10:15 nucliadb/standalone/tests/unit/test_versions.py
--rw-r--r--  2.0 unx     1037 b- defN 24-May-20 10:15 nucliadb/tasks/__init__.py
--rw-r--r--  2.0 unx     7655 b- defN 24-May-20 10:15 nucliadb/tasks/consumer.py
--rw-r--r--  2.0 unx      924 b- defN 24-May-20 10:15 nucliadb/tasks/logger.py
--rw-r--r--  2.0 unx     1378 b- defN 24-May-20 10:15 nucliadb/tasks/models.py
--rw-r--r--  2.0 unx     3457 b- defN 24-May-20 10:15 nucliadb/tasks/producer.py
--rw-r--r--  2.0 unx     1753 b- defN 24-May-20 10:15 nucliadb/tasks/registry.py
--rw-r--r--  2.0 unx     1360 b- defN 24-May-20 10:15 nucliadb/tasks/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-20 10:15 nucliadb/tests/__init__.py
--rw-r--r--  2.0 unx     1229 b- defN 24-May-20 10:15 nucliadb/tests/conftest.py
--rw-r--r--  2.0 unx    22365 b- defN 24-May-20 10:15 nucliadb/tests/fixtures.py
--rw-r--r--  2.0 unx     7549 b- defN 24-May-20 10:15 nucliadb/tests/tikv.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-20 10:15 nucliadb/tests/benchmarks/__init__.py
--rw-r--r--  2.0 unx     3032 b- defN 24-May-20 10:15 nucliadb/tests/benchmarks/test_search.py
--rw-r--r--  2.0 unx      919 b- defN 24-May-20 10:15 nucliadb/tests/knowledgeboxes/__init__.py
--rw-r--r--  2.0 unx     7002 b- defN 24-May-20 10:15 nucliadb/tests/knowledgeboxes/philosophy_books.py
--rw-r--r--  2.0 unx     3037 b- defN 24-May-20 10:15 nucliadb/tests/knowledgeboxes/ten_dummy_resources.py
--rw-r--r--  2.0 unx     1148 b- defN 24-May-20 10:15 nucliadb/tests/migrations/__init__.py
--rw-r--r--  2.0 unx     2726 b- defN 24-May-20 10:15 nucliadb/tests/migrations/test_migration_0017.py
--rw-r--r--  2.0 unx     3662 b- defN 24-May-20 10:15 nucliadb/tests/migrations/test_migration_0018.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-20 10:15 nucliadb/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1487 b- defN 24-May-20 10:15 nucliadb/tests/unit/test_field_ids.py
--rw-r--r--  2.0 unx     2780 b- defN 24-May-20 10:15 nucliadb/tests/unit/test_health.py
--rw-r--r--  2.0 unx     1543 b- defN 24-May-20 10:15 nucliadb/tests/unit/test_kb_slugs.py
--rw-r--r--  2.0 unx     7892 b- defN 24-May-20 10:15 nucliadb/tests/unit/test_learning_proxy.py
--rw-r--r--  2.0 unx     2642 b- defN 24-May-20 10:15 nucliadb/tests/unit/test_metrics_exporter.py
--rw-r--r--  2.0 unx     1341 b- defN 24-May-20 10:15 nucliadb/tests/unit/test_openapi.py
--rw-r--r--  2.0 unx     3649 b- defN 24-May-20 10:15 nucliadb/tests/unit/test_purge.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-20 10:15 nucliadb/tests/unit/common/__init__.py
--rw-r--r--  2.0 unx     1268 b- defN 24-May-20 10:15 nucliadb/tests/unit/common/test_context.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-20 10:15 nucliadb/tests/unit/common/cluster/__init__.py
--rw-r--r--  2.0 unx    12240 b- defN 24-May-20 10:15 nucliadb/tests/unit/common/cluster/test_cluster.py
--rw-r--r--  2.0 unx     5387 b- defN 24-May-20 10:15 nucliadb/tests/unit/common/cluster/test_kb_shard_manager.py
--rw-r--r--  2.0 unx     9465 b- defN 24-May-20 10:15 nucliadb/tests/unit/common/cluster/test_rollover.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-20 10:15 nucliadb/tests/unit/common/cluster/discovery/__init__.py
--rw-r--r--  2.0 unx     5627 b- defN 24-May-20 10:15 nucliadb/tests/unit/common/cluster/discovery/test_k8s.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-20 10:15 nucliadb/tests/unit/common/cluster/standalone/__init__.py
--rw-r--r--  2.0 unx     3761 b- defN 24-May-20 10:15 nucliadb/tests/unit/common/cluster/standalone/test_service.py
--rw-r--r--  2.0 unx     2136 b- defN 24-May-20 10:15 nucliadb/tests/unit/common/cluster/standalone/test_utils.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-20 10:15 nucliadb/tests/unit/common/maindb/__init__.py
--rw-r--r--  2.0 unx     3579 b- defN 24-May-20 10:15 nucliadb/tests/unit/common/maindb/test_driver.py
--rw-r--r--  2.0 unx     1869 b- defN 24-May-20 10:15 nucliadb/tests/unit/common/maindb/test_tikv.py
--rw-r--r--  2.0 unx     3213 b- defN 24-May-20 10:15 nucliadb/tests/unit/common/maindb/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-20 10:15 nucliadb/tests/unit/export_import/__init__.py
--rw-r--r--  2.0 unx     1435 b- defN 24-May-20 10:15 nucliadb/tests/unit/export_import/test_datamanager.py
--rw-r--r--  2.0 unx     9706 b- defN 24-May-20 10:15 nucliadb/tests/unit/export_import/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-20 10:15 nucliadb/tests/unit/migrator/__init__.py
--rw-r--r--  2.0 unx     3233 b- defN 24-May-20 10:15 nucliadb/tests/unit/migrator/test_migrator.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-20 10:15 nucliadb/tests/unit/tasks/__init__.py
--rw-r--r--  2.0 unx     1375 b- defN 24-May-20 10:15 nucliadb/tests/unit/tasks/conftest.py
--rw-r--r--  2.0 unx     2714 b- defN 24-May-20 10:15 nucliadb/tests/unit/tasks/test_consumer.py
--rw-r--r--  2.0 unx     3189 b- defN 24-May-20 10:15 nucliadb/tests/unit/tasks/test_producer.py
--rw-r--r--  2.0 unx     1827 b- defN 24-May-20 10:15 nucliadb/tests/unit/tasks/test_tasks.py
--rw-r--r--  2.0 unx     2507 b- defN 24-May-20 10:15 nucliadb/tests/utils/__init__.py
--rw-r--r--  2.0 unx     1797 b- defN 24-May-20 10:15 nucliadb/tests/utils/aiohttp_session.py
--rw-r--r--  2.0 unx     2533 b- defN 24-May-20 10:15 nucliadb/tests/utils/entities.py
--rw-r--r--  2.0 unx     6327 b- defN 24-May-20 10:15 nucliadb/tests/utils/broker_messages/__init__.py
--rw-r--r--  2.0 unx     7557 b- defN 24-May-20 10:15 nucliadb/tests/utils/broker_messages/fields.py
--rw-r--r--  2.0 unx     1196 b- defN 24-May-20 10:15 nucliadb/tests/utils/broker_messages/helpers.py
--rw-r--r--  2.0 unx     1325 b- defN 24-May-20 10:15 nucliadb/train/__init__.py
--rw-r--r--  2.0 unx     3530 b- defN 24-May-20 10:15 nucliadb/train/app.py
--rw-r--r--  2.0 unx     3800 b- defN 24-May-20 10:15 nucliadb/train/generator.py
--rw-r--r--  2.0 unx     1698 b- defN 24-May-20 10:15 nucliadb/train/lifecycle.py
--rw-r--r--  2.0 unx     1198 b- defN 24-May-20 10:15 nucliadb/train/models.py
--rw-r--r--  2.0 unx     5706 b- defN 24-May-20 10:15 nucliadb/train/nodes.py
--rw-r--r--  2.0 unx     1400 b- defN 24-May-20 10:15 nucliadb/train/run.py
--rw-r--r--  2.0 unx     5926 b- defN 24-May-20 10:15 nucliadb/train/servicer.py
--rw-r--r--  2.0 unx     1415 b- defN 24-May-20 10:15 nucliadb/train/settings.py
--rw-r--r--  2.0 unx     1496 b- defN 24-May-20 10:15 nucliadb/train/types.py
--rw-r--r--  2.0 unx     3265 b- defN 24-May-20 10:15 nucliadb/train/upload.py
--rw-r--r--  2.0 unx     6420 b- defN 24-May-20 10:15 nucliadb/train/uploader.py
--rw-r--r--  2.0 unx     3179 b- defN 24-May-20 10:15 nucliadb/train/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-20 10:15 nucliadb/train/api/__init__.py
--rw-r--r--  2.0 unx     1479 b- defN 24-May-20 10:15 nucliadb/train/api/utils.py
--rw-r--r--  2.0 unx      928 b- defN 24-May-20 10:15 nucliadb/train/api/v1/__init__.py
--rw-r--r--  2.0 unx     2071 b- defN 24-May-20 10:15 nucliadb/train/api/v1/check.py
--rw-r--r--  2.0 unx      910 b- defN 24-May-20 10:15 nucliadb/train/api/v1/router.py
--rw-r--r--  2.0 unx     1908 b- defN 24-May-20 10:15 nucliadb/train/api/v1/shards.py
--rw-r--r--  2.0 unx     2135 b- defN 24-May-20 10:15 nucliadb/train/api/v1/trainset.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-20 10:15 nucliadb/train/generators/__init__.py
--rw-r--r--  2.0 unx     3723 b- defN 24-May-20 10:15 nucliadb/train/generators/field_classifier.py
--rw-r--r--  2.0 unx     6712 b- defN 24-May-20 10:15 nucliadb/train/generators/image_classifier.py
--rw-r--r--  2.0 unx     2789 b- defN 24-May-20 10:15 nucliadb/train/generators/paragraph_classifier.py
--rw-r--r--  2.0 unx     3590 b- defN 24-May-20 10:15 nucliadb/train/generators/paragraph_streaming.py
--rw-r--r--  2.0 unx     5372 b- defN 24-May-20 10:15 nucliadb/train/generators/question_answer_streaming.py
--rw-r--r--  2.0 unx     5160 b- defN 24-May-20 10:15 nucliadb/train/generators/sentence_classifier.py
--rw-r--r--  2.0 unx    10446 b- defN 24-May-20 10:15 nucliadb/train/generators/token_classifier.py
--rw-r--r--  2.0 unx     3877 b- defN 24-May-20 10:15 nucliadb/train/generators/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-20 10:15 nucliadb/train/tests/__init__.py
--rw-r--r--  2.0 unx     1125 b- defN 24-May-20 10:15 nucliadb/train/tests/conftest.py
--rw-r--r--  2.0 unx    11053 b- defN 24-May-20 10:15 nucliadb/train/tests/fixtures.py
--rw-r--r--  2.0 unx     4598 b- defN 24-May-20 10:15 nucliadb/train/tests/test_field_classification.py
--rw-r--r--  2.0 unx     2729 b- defN 24-May-20 10:15 nucliadb/train/tests/test_get_entities.py
--rw-r--r--  2.0 unx     1876 b- defN 24-May-20 10:15 nucliadb/train/tests/test_get_info.py
--rw-r--r--  2.0 unx     1382 b- defN 24-May-20 10:15 nucliadb/train/tests/test_get_ontology.py
--rw-r--r--  2.0 unx     2417 b- defN 24-May-20 10:15 nucliadb/train/tests/test_get_ontology_count.py
--rw-r--r--  2.0 unx     7669 b- defN 24-May-20 10:15 nucliadb/train/tests/test_image_classification.py
--rw-r--r--  2.0 unx     1416 b- defN 24-May-20 10:15 nucliadb/train/tests/test_list_fields.py
--rw-r--r--  2.0 unx     2944 b- defN 24-May-20 10:15 nucliadb/train/tests/test_list_paragraphs.py
--rw-r--r--  2.0 unx     1423 b- defN 24-May-20 10:15 nucliadb/train/tests/test_list_resources.py
--rw-r--r--  2.0 unx     2947 b- defN 24-May-20 10:15 nucliadb/train/tests/test_list_sentences.py
--rw-r--r--  2.0 unx     4645 b- defN 24-May-20 10:15 nucliadb/train/tests/test_paragraph_classification.py
--rw-r--r--  2.0 unx     4320 b- defN 24-May-20 10:15 nucliadb/train/tests/test_paragraph_streaming.py
--rw-r--r--  2.0 unx     8751 b- defN 24-May-20 10:15 nucliadb/train/tests/test_question_answer_streaming.py
--rw-r--r--  2.0 unx     5051 b- defN 24-May-20 10:15 nucliadb/train/tests/test_sentence_classification.py
--rw-r--r--  2.0 unx     5583 b- defN 24-May-20 10:15 nucliadb/train/tests/test_token_classification.py
--rw-r--r--  2.0 unx     3324 b- defN 24-May-20 10:15 nucliadb/train/tests/utils.py
--rw-r--r--  2.0 unx     1328 b- defN 24-May-20 10:15 nucliadb/writer/__init__.py
--rw-r--r--  2.0 unx     4268 b- defN 24-May-20 10:15 nucliadb/writer/app.py
--rw-r--r--  2.0 unx    19483 b- defN 24-May-20 10:15 nucliadb/writer/back_pressure.py
--rw-r--r--  2.0 unx      972 b- defN 24-May-20 10:15 nucliadb/writer/exceptions.py
--rw-r--r--  2.0 unx     1953 b- defN 24-May-20 10:15 nucliadb/writer/lifecycle.py
--rw-r--r--  2.0 unx     1032 b- defN 24-May-20 10:15 nucliadb/writer/openapi.py
--rw-r--r--  2.0 unx     1448 b- defN 24-May-20 10:15 nucliadb/writer/run.py
--rw-r--r--  2.0 unx     3103 b- defN 24-May-20 10:15 nucliadb/writer/settings.py
--rw-r--r--  2.0 unx     1036 b- defN 24-May-20 10:15 nucliadb/writer/utilities.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-20 10:15 nucliadb/writer/api/__init__.py
--rw-r--r--  2.0 unx     1429 b- defN 24-May-20 10:15 nucliadb/writer/api/constants.py
--rw-r--r--  2.0 unx     1095 b- defN 24-May-20 10:15 nucliadb/writer/api/v1/__init__.py
--rw-r--r--  2.0 unx     6571 b- defN 24-May-20 10:15 nucliadb/writer/api/v1/export_import.py
--rw-r--r--  2.0 unx    24482 b- defN 24-May-20 10:15 nucliadb/writer/api/v1/field.py
--rw-r--r--  2.0 unx     5248 b- defN 24-May-20 10:15 nucliadb/writer/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     2058 b- defN 24-May-20 10:15 nucliadb/writer/api/v1/learning_config.py
--rw-r--r--  2.0 unx    18893 b- defN 24-May-20 10:15 nucliadb/writer/api/v1/resource.py
--rw-r--r--  2.0 unx     1034 b- defN 24-May-20 10:15 nucliadb/writer/api/v1/router.py
--rw-r--r--  2.0 unx    10747 b- defN 24-May-20 10:15 nucliadb/writer/api/v1/services.py
--rw-r--r--  2.0 unx    30857 b- defN 24-May-20 10:15 nucliadb/writer/api/v1/upload.py
--rw-r--r--  2.0 unx     1612 b- defN 24-May-20 10:15 nucliadb/writer/layouts/__init__.py
--rw-r--r--  2.0 unx     2115 b- defN 24-May-20 10:15 nucliadb/writer/layouts/v1.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-20 10:15 nucliadb/writer/resource/__init__.py
--rw-r--r--  2.0 unx     1425 b- defN 24-May-20 10:15 nucliadb/writer/resource/audit.py
--rw-r--r--  2.0 unx    10968 b- defN 24-May-20 10:15 nucliadb/writer/resource/basic.py
--rw-r--r--  2.0 unx    16319 b- defN 24-May-20 10:15 nucliadb/writer/resource/field.py
--rw-r--r--  2.0 unx     2022 b- defN 24-May-20 10:15 nucliadb/writer/resource/origin.py
--rw-r--r--  2.0 unx     1152 b- defN 24-May-20 10:15 nucliadb/writer/resource/slug.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-20 10:15 nucliadb/writer/tests/__init__.py
--rw-r--r--  2.0 unx     1200 b- defN 24-May-20 10:15 nucliadb/writer/tests/conftest.py
--rw-r--r--  2.0 unx     5971 b- defN 24-May-20 10:15 nucliadb/writer/tests/fixtures.py
--rw-r--r--  2.0 unx    15472 b- defN 24-May-20 10:15 nucliadb/writer/tests/test_fields.py
--rw-r--r--  2.0 unx    25999 b- defN 24-May-20 10:15 nucliadb/writer/tests/test_files.py
--rw-r--r--  2.0 unx     1729 b- defN 24-May-20 10:15 nucliadb/writer/tests/test_knowledgebox.py
--rw-r--r--  2.0 unx     4358 b- defN 24-May-20 10:15 nucliadb/writer/tests/test_reprocess_file_field.py
--rw-r--r--  2.0 unx    16694 b- defN 24-May-20 10:15 nucliadb/writer/tests/test_resources.py
--rw-r--r--  2.0 unx     5120 b- defN 24-May-20 10:15 nucliadb/writer/tests/test_service.py
--rw-r--r--  2.0 unx     6054 b- defN 24-May-20 10:15 nucliadb/writer/tests/test_tus.py
--rw-r--r--  2.0 unx     1287 b- defN 24-May-20 10:15 nucliadb/writer/tests/utils.py
--rw-r--r--  2.0 unx     5226 b- defN 24-May-20 10:15 nucliadb/writer/tus/__init__.py
--rw-r--r--  2.0 unx     5082 b- defN 24-May-20 10:15 nucliadb/writer/tus/dm.py
--rw-r--r--  2.0 unx     2186 b- defN 24-May-20 10:15 nucliadb/writer/tus/exceptions.py
--rw-r--r--  2.0 unx    14527 b- defN 24-May-20 10:15 nucliadb/writer/tus/gcs.py
--rw-r--r--  2.0 unx     5849 b- defN 24-May-20 10:15 nucliadb/writer/tus/local.py
--rw-r--r--  2.0 unx     4367 b- defN 24-May-20 10:15 nucliadb/writer/tus/pg.py
--rw-r--r--  2.0 unx     9069 b- defN 24-May-20 10:15 nucliadb/writer/tus/s3.py
--rw-r--r--  2.0 unx     4734 b- defN 24-May-20 10:15 nucliadb/writer/tus/storage.py
--rw-r--r--  2.0 unx     2556 b- defN 24-May-20 10:15 nucliadb/writer/tus/utils.py
--rw-r--r--  2.0 unx     4423 b- defN 24-May-20 10:16 nucliadb-4.0.0.post520.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-20 10:16 nucliadb-4.0.0.post520.dist-info/WHEEL
--rw-r--r--  2.0 unx     1268 b- defN 24-May-20 10:16 nucliadb-4.0.0.post520.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       20 b- defN 24-May-20 10:16 nucliadb-4.0.0.post520.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 24-May-20 10:16 nucliadb-4.0.0.post520.dist-info/zip-safe
--rw-rw-r--  2.0 unx    43144 b- defN 24-May-20 10:16 nucliadb-4.0.0.post520.dist-info/RECORD
-460 files, 2260787 bytes uncompressed, 694452 bytes compressed:  69.3%
+Zip file size: 764195 bytes, number of entries: 461
+-rw-r--r--  2.0 unx     1135 b- defN 24-May-20 11:05 migrations/0001_bootstrap.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-May-20 11:05 migrations/0002_rollover_shards.py
+-rw-r--r--  2.0 unx     2436 b- defN 24-May-20 11:05 migrations/0003_allfields_key.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-May-20 11:05 migrations/0004_rollover_shards.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-May-20 11:05 migrations/0005_rollover_shards.py
+-rw-r--r--  2.0 unx     1024 b- defN 24-May-20 11:05 migrations/0006_rollover_shards.py
+-rw-r--r--  2.0 unx     1301 b- defN 24-May-20 11:05 migrations/0008_cleanup_leftover_rollover_metadata.py
+-rw-r--r--  2.0 unx     1378 b- defN 24-May-20 11:05 migrations/0009_upgrade_relations_and_texts_to_v2.py
+-rw-r--r--  2.0 unx     1610 b- defN 24-May-20 11:05 migrations/0010_fix_corrupt_indexes.py
+-rw-r--r--  2.0 unx     1843 b- defN 24-May-20 11:05 migrations/0011_materialize_labelset_ids.py
+-rw-r--r--  2.0 unx     1443 b- defN 24-May-20 11:05 migrations/0012_rollover_shards.py
+-rw-r--r--  2.0 unx     1024 b- defN 24-May-20 11:05 migrations/0013_rollover_shards.py
+-rw-r--r--  2.0 unx     1382 b- defN 24-May-20 11:05 migrations/0014_rollover_shards.py
+-rw-r--r--  2.0 unx     1462 b- defN 24-May-20 11:05 migrations/0015_targeted_rollover.py
+-rw-r--r--  2.0 unx     2506 b- defN 24-May-20 11:05 migrations/0016_upgrade_to_paragraphs_v2.py
+-rw-r--r--  2.0 unx     2100 b- defN 24-May-20 11:05 migrations/0017_multiple_writable_shards.py
+-rw-r--r--  2.0 unx     2264 b- defN 24-May-20 11:05 migrations/0018_purge_orphan_kbslugs.py
+-rw-r--r--  2.0 unx     2506 b- defN 24-May-20 11:05 migrations/0019_upgrade_to_paragraphs_v3.py
+-rw-r--r--  2.0 unx     3282 b- defN 24-May-20 11:05 migrations/0020_drain_nodes_from_cluster.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-20 11:05 migrations/__init__.py
+-rw-r--r--  2.0 unx      891 b- defN 24-May-20 11:05 nucliadb/__init__.py
+-rw-r--r--  2.0 unx     3733 b- defN 24-May-20 11:05 nucliadb/health.py
+-rw-r--r--  2.0 unx    11639 b- defN 24-May-20 11:05 nucliadb/learning_proxy.py
+-rw-r--r--  2.0 unx     4806 b- defN 24-May-20 11:05 nucliadb/metrics_exporter.py
+-rw-r--r--  2.0 unx     2272 b- defN 24-May-20 11:05 nucliadb/openapi.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 11:05 nucliadb/py.typed
+-rw-r--r--  2.0 unx      835 b- defN 24-May-20 11:05 nucliadb/common/__init__.py
+-rw-r--r--  2.0 unx     5022 b- defN 24-May-20 11:05 nucliadb/common/locking.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-20 11:05 nucliadb/common/cluster/__init__.py
+-rw-r--r--  2.0 unx     4971 b- defN 24-May-20 11:05 nucliadb/common/cluster/base.py
+-rw-r--r--  2.0 unx     1495 b- defN 24-May-20 11:05 nucliadb/common/cluster/exceptions.py
+-rw-r--r--  2.0 unx     3793 b- defN 24-May-20 11:05 nucliadb/common/cluster/grpc_node_dummy.py
+-rw-r--r--  2.0 unx     3429 b- defN 24-May-20 11:05 nucliadb/common/cluster/index_node.py
+-rw-r--r--  2.0 unx    22091 b- defN 24-May-20 11:05 nucliadb/common/cluster/manager.py
+-rw-r--r--  2.0 unx     8590 b- defN 24-May-20 11:05 nucliadb/common/cluster/rebalance.py
+-rw-r--r--  2.0 unx    20209 b- defN 24-May-20 11:05 nucliadb/common/cluster/rollover.py
+-rw-r--r--  2.0 unx     3016 b- defN 24-May-20 11:05 nucliadb/common/cluster/settings.py
+-rw-r--r--  2.0 unx     5713 b- defN 24-May-20 11:05 nucliadb/common/cluster/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-20 11:05 nucliadb/common/cluster/discovery/__init__.py
+-rw-r--r--  2.0 unx     6553 b- defN 24-May-20 11:05 nucliadb/common/cluster/discovery/base.py
+-rw-r--r--  2.0 unx    12515 b- defN 24-May-20 11:05 nucliadb/common/cluster/discovery/k8s.py
+-rw-r--r--  2.0 unx     1957 b- defN 24-May-20 11:05 nucliadb/common/cluster/discovery/manual.py
+-rw-r--r--  2.0 unx     1737 b- defN 24-May-20 11:05 nucliadb/common/cluster/discovery/single.py
+-rw-r--r--  2.0 unx     1139 b- defN 24-May-20 11:05 nucliadb/common/cluster/discovery/types.py
+-rw-r--r--  2.0 unx     2548 b- defN 24-May-20 11:05 nucliadb/common/cluster/discovery/utils.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-20 11:05 nucliadb/common/cluster/standalone/__init__.py
+-rw-r--r--  2.0 unx    13707 b- defN 24-May-20 11:05 nucliadb/common/cluster/standalone/grpc_node_binding.py
+-rw-r--r--  2.0 unx     4683 b- defN 24-May-20 11:05 nucliadb/common/cluster/standalone/index_node.py
+-rw-r--r--  2.0 unx     3444 b- defN 24-May-20 11:05 nucliadb/common/cluster/standalone/service.py
+-rw-r--r--  2.0 unx     3545 b- defN 24-May-20 11:05 nucliadb/common/cluster/standalone/utils.py
+-rw-r--r--  2.0 unx     3440 b- defN 24-May-20 11:05 nucliadb/common/context/__init__.py
+-rw-r--r--  2.0 unx     1628 b- defN 24-May-20 11:05 nucliadb/common/context/fastapi.py
+-rw-r--r--  2.0 unx     1813 b- defN 24-May-20 11:05 nucliadb/common/datamanagers/__init__.py
+-rw-r--r--  2.0 unx     1451 b- defN 24-May-20 11:05 nucliadb/common/datamanagers/cluster.py
+-rw-r--r--  2.0 unx     5383 b- defN 24-May-20 11:05 nucliadb/common/datamanagers/entities.py
+-rw-r--r--  2.0 unx      883 b- defN 24-May-20 11:05 nucliadb/common/datamanagers/exceptions.py
+-rw-r--r--  2.0 unx     3994 b- defN 24-May-20 11:05 nucliadb/common/datamanagers/kb.py
+-rw-r--r--  2.0 unx     5389 b- defN 24-May-20 11:05 nucliadb/common/datamanagers/labels.py
+-rw-r--r--  2.0 unx     1599 b- defN 24-May-20 11:05 nucliadb/common/datamanagers/processing.py
+-rw-r--r--  2.0 unx     8719 b- defN 24-May-20 11:05 nucliadb/common/datamanagers/resources.py
+-rw-r--r--  2.0 unx     5634 b- defN 24-May-20 11:05 nucliadb/common/datamanagers/rollover.py
+-rw-r--r--  2.0 unx     1631 b- defN 24-May-20 11:05 nucliadb/common/datamanagers/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-20 11:05 nucliadb/common/http_clients/__init__.py
+-rw-r--r--  2.0 unx     2146 b- defN 24-May-20 11:05 nucliadb/common/http_clients/auth.py
+-rw-r--r--  2.0 unx     1100 b- defN 24-May-20 11:05 nucliadb/common/http_clients/exceptions.py
+-rw-r--r--  2.0 unx     7155 b- defN 24-May-20 11:05 nucliadb/common/http_clients/processing.py
+-rw-r--r--  2.0 unx     1540 b- defN 24-May-20 11:05 nucliadb/common/http_clients/pypi.py
+-rw-r--r--  2.0 unx     1551 b- defN 24-May-20 11:05 nucliadb/common/http_clients/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-20 11:05 nucliadb/common/maindb/__init__.py
+-rw-r--r--  2.0 unx     3449 b- defN 24-May-20 11:05 nucliadb/common/maindb/driver.py
+-rw-r--r--  2.0 unx      946 b- defN 24-May-20 11:05 nucliadb/common/maindb/exceptions.py
+-rw-r--r--  2.0 unx     6769 b- defN 24-May-20 11:05 nucliadb/common/maindb/local.py
+-rw-r--r--  2.0 unx     8391 b- defN 24-May-20 11:05 nucliadb/common/maindb/pg.py
+-rw-r--r--  2.0 unx     6053 b- defN 24-May-20 11:05 nucliadb/common/maindb/redis.py
+-rw-r--r--  2.0 unx    14502 b- defN 24-May-20 11:05 nucliadb/common/maindb/tikv.py
+-rw-r--r--  2.0 unx     4167 b- defN 24-May-20 11:05 nucliadb/common/maindb/utils.py
+-rw-r--r--  2.0 unx      932 b- defN 24-May-20 11:05 nucliadb/export_import/__init__.py
+-rw-r--r--  2.0 unx     6171 b- defN 24-May-20 11:05 nucliadb/export_import/datamanager.py
+-rw-r--r--  2.0 unx     1949 b- defN 24-May-20 11:05 nucliadb/export_import/exceptions.py
+-rw-r--r--  2.0 unx     7116 b- defN 24-May-20 11:05 nucliadb/export_import/exporter.py
+-rw-r--r--  2.0 unx     4258 b- defN 24-May-20 11:05 nucliadb/export_import/importer.py
+-rw-r--r--  2.0 unx     2063 b- defN 24-May-20 11:05 nucliadb/export_import/models.py
+-rw-r--r--  2.0 unx     2571 b- defN 24-May-20 11:05 nucliadb/export_import/tasks.py
+-rw-r--r--  2.0 unx    19401 b- defN 24-May-20 11:05 nucliadb/export_import/utils.py
+-rw-r--r--  2.0 unx     1011 b- defN 24-May-20 11:05 nucliadb/ingest/__init__.py
+-rw-r--r--  2.0 unx     7277 b- defN 24-May-20 11:05 nucliadb/ingest/app.py
+-rw-r--r--  2.0 unx     1005 b- defN 24-May-20 11:05 nucliadb/ingest/cache.py
+-rw-r--r--  2.0 unx     2484 b- defN 24-May-20 11:05 nucliadb/ingest/partitions.py
+-rw-r--r--  2.0 unx    19555 b- defN 24-May-20 11:05 nucliadb/ingest/processing.py
+-rw-r--r--  2.0 unx    20277 b- defN 24-May-20 11:05 nucliadb/ingest/serialize.py
+-rw-r--r--  2.0 unx     3207 b- defN 24-May-20 11:05 nucliadb/ingest/settings.py
+-rw-r--r--  2.0 unx     2314 b- defN 24-May-20 11:05 nucliadb/ingest/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-20 11:05 nucliadb/ingest/consumer/__init__.py
+-rw-r--r--  2.0 unx     6918 b- defN 24-May-20 11:05 nucliadb/ingest/consumer/auditing.py
+-rw-r--r--  2.0 unx    12174 b- defN 24-May-20 11:05 nucliadb/ingest/consumer/consumer.py
+-rw-r--r--  2.0 unx     3788 b- defN 24-May-20 11:05 nucliadb/ingest/consumer/materializer.py
+-rw-r--r--  2.0 unx     1075 b- defN 24-May-20 11:05 nucliadb/ingest/consumer/metrics.py
+-rw-r--r--  2.0 unx     9543 b- defN 24-May-20 11:05 nucliadb/ingest/consumer/pull.py
+-rw-r--r--  2.0 unx     6871 b- defN 24-May-20 11:05 nucliadb/ingest/consumer/service.py
+-rw-r--r--  2.0 unx     4331 b- defN 24-May-20 11:05 nucliadb/ingest/consumer/shard_creator.py
+-rw-r--r--  2.0 unx     2656 b- defN 24-May-20 11:05 nucliadb/ingest/consumer/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-20 11:05 nucliadb/ingest/fields/__init__.py
+-rw-r--r--  2.0 unx    18433 b- defN 24-May-20 11:05 nucliadb/ingest/fields/base.py
+-rw-r--r--  2.0 unx     6516 b- defN 24-May-20 11:05 nucliadb/ingest/fields/conversation.py
+-rw-r--r--  2.0 unx     1223 b- defN 24-May-20 11:05 nucliadb/ingest/fields/date.py
+-rw-r--r--  2.0 unx     1205 b- defN 24-May-20 11:05 nucliadb/ingest/fields/exceptions.py
+-rw-r--r--  2.0 unx     5159 b- defN 24-May-20 11:05 nucliadb/ingest/fields/file.py
+-rw-r--r--  2.0 unx     1547 b- defN 24-May-20 11:05 nucliadb/ingest/fields/generic.py
+-rw-r--r--  2.0 unx     1235 b- defN 24-May-20 11:05 nucliadb/ingest/fields/keywordset.py
+-rw-r--r--  2.0 unx     2250 b- defN 24-May-20 11:05 nucliadb/ingest/fields/layout.py
+-rw-r--r--  2.0 unx     4531 b- defN 24-May-20 11:05 nucliadb/ingest/fields/link.py
+-rw-r--r--  2.0 unx     1319 b- defN 24-May-20 11:05 nucliadb/ingest/fields/text.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-20 11:05 nucliadb/ingest/orm/__init__.py
+-rw-r--r--  2.0 unx    28448 b- defN 24-May-20 11:05 nucliadb/ingest/orm/brain.py
+-rw-r--r--  2.0 unx    15758 b- defN 24-May-20 11:05 nucliadb/ingest/orm/entities.py
+-rw-r--r--  2.0 unx     1279 b- defN 24-May-20 11:05 nucliadb/ingest/orm/exceptions.py
+-rw-r--r--  2.0 unx    17167 b- defN 24-May-20 11:05 nucliadb/ingest/orm/knowledgebox.py
+-rw-r--r--  2.0 unx     1096 b- defN 24-May-20 11:05 nucliadb/ingest/orm/metrics.py
+-rw-r--r--  2.0 unx    60444 b- defN 24-May-20 11:05 nucliadb/ingest/orm/resource.py
+-rw-r--r--  2.0 unx     1739 b- defN 24-May-20 11:05 nucliadb/ingest/orm/synonyms.py
+-rw-r--r--  2.0 unx     3683 b- defN 24-May-20 11:05 nucliadb/ingest/orm/utils.py
+-rw-r--r--  2.0 unx    27042 b- defN 24-May-20 11:05 nucliadb/ingest/orm/processor/__init__.py
+-rw-r--r--  2.0 unx     5090 b- defN 24-May-20 11:05 nucliadb/ingest/orm/processor/auditing.py
+-rw-r--r--  2.0 unx     1690 b- defN 24-May-20 11:05 nucliadb/ingest/orm/processor/sequence_manager.py
+-rw-r--r--  2.0 unx     2057 b- defN 24-May-20 11:05 nucliadb/ingest/service/__init__.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-20 11:05 nucliadb/ingest/service/exceptions.py
+-rw-r--r--  2.0 unx    33193 b- defN 24-May-20 11:05 nucliadb/ingest/service/writer.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-20 11:05 nucliadb/ingest/tests/__init__.py
+-rw-r--r--  2.0 unx     1157 b- defN 24-May-20 11:05 nucliadb/ingest/tests/conftest.py
+-rw-r--r--  2.0 unx    24060 b- defN 24-May-20 11:05 nucliadb/ingest/tests/fixtures.py
+-rw-r--r--  2.0 unx    62843 b- defN 24-May-20 11:05 nucliadb/ingest/tests/vectors.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-20 11:05 nucliadb/ingest/tests/integration/__init__.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-20 11:05 nucliadb/ingest/tests/integration/consumer/__init__.py
+-rw-r--r--  2.0 unx     2500 b- defN 24-May-20 11:05 nucliadb/ingest/tests/integration/consumer/test_auditing.py
+-rw-r--r--  2.0 unx     2591 b- defN 24-May-20 11:05 nucliadb/ingest/tests/integration/consumer/test_materializer.py
+-rw-r--r--  2.0 unx     4470 b- defN 24-May-20 11:05 nucliadb/ingest/tests/integration/consumer/test_pull.py
+-rw-r--r--  2.0 unx     2763 b- defN 24-May-20 11:05 nucliadb/ingest/tests/integration/consumer/test_service.py
+-rw-r--r--  2.0 unx     2019 b- defN 24-May-20 11:05 nucliadb/ingest/tests/integration/consumer/test_shard_creator.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-20 11:05 nucliadb/ingest/tests/integration/ingest/__init__.py
+-rw-r--r--  2.0 unx    27247 b- defN 24-May-20 11:05 nucliadb/ingest/tests/integration/ingest/test_ingest.py
+-rw-r--r--  2.0 unx     3040 b- defN 24-May-20 11:05 nucliadb/ingest/tests/integration/ingest/test_processing_engine.py
+-rw-r--r--  2.0 unx     8586 b- defN 24-May-20 11:05 nucliadb/ingest/tests/integration/ingest/test_relations.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-20 11:05 nucliadb/ingest/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1189 b- defN 24-May-20 11:05 nucliadb/ingest/tests/unit/test_cache.py
+-rw-r--r--  2.0 unx     1432 b- defN 24-May-20 11:05 nucliadb/ingest/tests/unit/test_partitions.py
+-rw-r--r--  2.0 unx     5807 b- defN 24-May-20 11:05 nucliadb/ingest/tests/unit/test_processing.py
+-rw-r--r--  2.0 unx      978 b- defN 24-May-20 11:05 nucliadb/ingest/tests/unit/test_settings.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-20 11:05 nucliadb/ingest/tests/unit/consumer/__init__.py
+-rw-r--r--  2.0 unx     3885 b- defN 24-May-20 11:05 nucliadb/ingest/tests/unit/consumer/test_auditing.py
+-rw-r--r--  2.0 unx     2472 b- defN 24-May-20 11:05 nucliadb/ingest/tests/unit/consumer/test_consumer.py
+-rw-r--r--  2.0 unx     2063 b- defN 24-May-20 11:05 nucliadb/ingest/tests/unit/consumer/test_pull.py
+-rw-r--r--  2.0 unx     4140 b- defN 24-May-20 11:05 nucliadb/ingest/tests/unit/consumer/test_shard_creator.py
+-rw-r--r--  2.0 unx     1934 b- defN 24-May-20 11:05 nucliadb/ingest/tests/unit/consumer/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-20 11:05 nucliadb/ingest/tests/unit/orm/__init__.py
+-rw-r--r--  2.0 unx     9876 b- defN 24-May-20 11:05 nucliadb/ingest/tests/unit/orm/test_brain.py
+-rw-r--r--  2.0 unx     2435 b- defN 24-May-20 11:05 nucliadb/ingest/tests/unit/orm/test_brain_vectors.py
+-rw-r--r--  2.0 unx     1174 b- defN 24-May-20 11:05 nucliadb/ingest/tests/unit/orm/test_orm_utils.py
+-rw-r--r--  2.0 unx     4045 b- defN 24-May-20 11:05 nucliadb/ingest/tests/unit/orm/test_processor.py
+-rw-r--r--  2.0 unx    11033 b- defN 24-May-20 11:05 nucliadb/ingest/tests/unit/orm/test_resource.py
+-rw-r--r--  2.0 unx     2216 b- defN 24-May-20 11:05 nucliadb/middleware/__init__.py
+-rw-r--r--  2.0 unx     3912 b- defN 24-May-20 11:05 nucliadb/middleware/transaction.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-20 11:05 nucliadb/migrator/__init__.py
+-rw-r--r--  2.0 unx     2119 b- defN 24-May-20 11:05 nucliadb/migrator/command.py
+-rw-r--r--  2.0 unx     1334 b- defN 24-May-20 11:05 nucliadb/migrator/context.py
+-rw-r--r--  2.0 unx     5104 b- defN 24-May-20 11:05 nucliadb/migrator/datamanager.py
+-rw-r--r--  2.0 unx      889 b- defN 24-May-20 11:05 nucliadb/migrator/exceptions.py
+-rw-r--r--  2.0 unx     9370 b- defN 24-May-20 11:05 nucliadb/migrator/migrator.py
+-rw-r--r--  2.0 unx     1145 b- defN 24-May-20 11:05 nucliadb/migrator/models.py
+-rw-r--r--  2.0 unx     1144 b- defN 24-May-20 11:05 nucliadb/migrator/settings.py
+-rw-r--r--  2.0 unx     2346 b- defN 24-May-20 11:05 nucliadb/migrator/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-20 11:05 nucliadb/models/__init__.py
+-rw-r--r--  2.0 unx     1599 b- defN 24-May-20 11:05 nucliadb/models/responses.py
+-rw-r--r--  2.0 unx     6041 b- defN 24-May-20 11:05 nucliadb/purge/__init__.py
+-rw-r--r--  2.0 unx     9364 b- defN 24-May-20 11:05 nucliadb/purge/orphan_shards.py
+-rw-r--r--  2.0 unx     1328 b- defN 24-May-20 11:05 nucliadb/reader/__init__.py
+-rw-r--r--  2.0 unx     3709 b- defN 24-May-20 11:05 nucliadb/reader/app.py
+-rw-r--r--  2.0 unx     1366 b- defN 24-May-20 11:05 nucliadb/reader/lifecycle.py
+-rw-r--r--  2.0 unx     1031 b- defN 24-May-20 11:05 nucliadb/reader/openapi.py
+-rw-r--r--  2.0 unx     1447 b- defN 24-May-20 11:05 nucliadb/reader/run.py
+-rw-r--r--  2.0 unx      872 b- defN 24-May-20 11:05 nucliadb/reader/api/__init__.py
+-rw-r--r--  2.0 unx     2458 b- defN 24-May-20 11:05 nucliadb/reader/api/models.py
+-rw-r--r--  2.0 unx     1110 b- defN 24-May-20 11:05 nucliadb/reader/api/v1/__init__.py
+-rw-r--r--  2.0 unx    12392 b- defN 24-May-20 11:05 nucliadb/reader/api/v1/download.py
+-rw-r--r--  2.0 unx     6459 b- defN 24-May-20 11:05 nucliadb/reader/api/v1/export_import.py
+-rw-r--r--  2.0 unx     3641 b- defN 24-May-20 11:05 nucliadb/reader/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     2099 b- defN 24-May-20 11:05 nucliadb/reader/api/v1/learning_collector.py
+-rw-r--r--  2.0 unx     4472 b- defN 24-May-20 11:05 nucliadb/reader/api/v1/learning_config.py
+-rw-r--r--  2.0 unx    13951 b- defN 24-May-20 11:05 nucliadb/reader/api/v1/resource.py
+-rw-r--r--  2.0 unx     1011 b- defN 24-May-20 11:05 nucliadb/reader/api/v1/router.py
+-rw-r--r--  2.0 unx    12399 b- defN 24-May-20 11:05 nucliadb/reader/api/v1/services.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-20 11:05 nucliadb/reader/reader/__init__.py
+-rw-r--r--  2.0 unx     7988 b- defN 24-May-20 11:05 nucliadb/reader/reader/notifications.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-20 11:05 nucliadb/reader/tests/__init__.py
+-rw-r--r--  2.0 unx     1224 b- defN 24-May-20 11:05 nucliadb/reader/tests/conftest.py
+-rw-r--r--  2.0 unx     4345 b- defN 24-May-20 11:05 nucliadb/reader/tests/fixtures.py
+-rw-r--r--  2.0 unx     2748 b- defN 24-May-20 11:05 nucliadb/reader/tests/test_list_resources.py
+-rw-r--r--  2.0 unx    10199 b- defN 24-May-20 11:05 nucliadb/reader/tests/test_reader_file_download.py
+-rw-r--r--  2.0 unx    10586 b- defN 24-May-20 11:05 nucliadb/reader/tests/test_reader_resource.py
+-rw-r--r--  2.0 unx     6535 b- defN 24-May-20 11:05 nucliadb/reader/tests/test_reader_resource_field.py
+-rw-r--r--  2.0 unx     1535 b- defN 24-May-20 11:05 nucliadb/search/__init__.py
+-rw-r--r--  2.0 unx     4905 b- defN 24-May-20 11:05 nucliadb/search/app.py
+-rw-r--r--  2.0 unx     1956 b- defN 24-May-20 11:05 nucliadb/search/lifecycle.py
+-rw-r--r--  2.0 unx     1016 b- defN 24-May-20 11:05 nucliadb/search/openapi.py
+-rw-r--r--  2.0 unx    20665 b- defN 24-May-20 11:05 nucliadb/search/predict.py
+-rw-r--r--  2.0 unx     1402 b- defN 24-May-20 11:05 nucliadb/search/run.py
+-rw-r--r--  2.0 unx     1193 b- defN 24-May-20 11:05 nucliadb/search/settings.py
+-rw-r--r--  2.0 unx     1037 b- defN 24-May-20 11:05 nucliadb/search/utilities.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-20 11:05 nucliadb/search/api/__init__.py
+-rw-r--r--  2.0 unx     1298 b- defN 24-May-20 11:05 nucliadb/search/api/v1/__init__.py
+-rw-r--r--  2.0 unx     3534 b- defN 24-May-20 11:05 nucliadb/search/api/v1/ask.py
+-rw-r--r--  2.0 unx     9493 b- defN 24-May-20 11:05 nucliadb/search/api/v1/chat.py
+-rw-r--r--  2.0 unx     2668 b- defN 24-May-20 11:05 nucliadb/search/api/v1/feedback.py
+-rw-r--r--  2.0 unx     8795 b- defN 24-May-20 11:05 nucliadb/search/api/v1/find.py
+-rw-r--r--  2.0 unx     6938 b- defN 24-May-20 11:05 nucliadb/search/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     3047 b- defN 24-May-20 11:05 nucliadb/search/api/v1/predict_proxy.py
+-rw-r--r--  2.0 unx      988 b- defN 24-May-20 11:05 nucliadb/search/api/v1/router.py
+-rw-r--r--  2.0 unx    19262 b- defN 24-May-20 11:05 nucliadb/search/api/v1/search.py
+-rw-r--r--  2.0 unx     5970 b- defN 24-May-20 11:05 nucliadb/search/api/v1/suggest.py
+-rw-r--r--  2.0 unx     2499 b- defN 24-May-20 11:05 nucliadb/search/api/v1/summarize.py
+-rw-r--r--  2.0 unx     1434 b- defN 24-May-20 11:05 nucliadb/search/api/v1/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-20 11:05 nucliadb/search/api/v1/resource/__init__.py
+-rw-r--r--  2.0 unx     4064 b- defN 24-May-20 11:05 nucliadb/search/api/v1/resource/ask.py
+-rw-r--r--  2.0 unx     5821 b- defN 24-May-20 11:05 nucliadb/search/api/v1/resource/chat.py
+-rw-r--r--  2.0 unx     5303 b- defN 24-May-20 11:05 nucliadb/search/api/v1/resource/search.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-20 11:05 nucliadb/search/requesters/__init__.py
+-rw-r--r--  2.0 unx     9111 b- defN 24-May-20 11:05 nucliadb/search/requesters/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-20 11:05 nucliadb/search/search/__init__.py
+-rw-r--r--  2.0 unx     2746 b- defN 24-May-20 11:05 nucliadb/search/search/cache.py
+-rw-r--r--  2.0 unx     1154 b- defN 24-May-20 11:05 nucliadb/search/search/exceptions.py
+-rw-r--r--  2.0 unx     5465 b- defN 24-May-20 11:05 nucliadb/search/search/fetch.py
+-rw-r--r--  2.0 unx     6513 b- defN 24-May-20 11:05 nucliadb/search/search/filters.py
+-rw-r--r--  2.0 unx     4612 b- defN 24-May-20 11:05 nucliadb/search/search/find.py
+-rw-r--r--  2.0 unx    17152 b- defN 24-May-20 11:05 nucliadb/search/search/find_merge.py
+-rw-r--r--  2.0 unx    21282 b- defN 24-May-20 11:05 nucliadb/search/search/merge.py
+-rw-r--r--  2.0 unx     1130 b- defN 24-May-20 11:05 nucliadb/search/search/metrics.py
+-rw-r--r--  2.0 unx     8698 b- defN 24-May-20 11:05 nucliadb/search/search/paragraphs.py
+-rw-r--r--  2.0 unx     3026 b- defN 24-May-20 11:05 nucliadb/search/search/predict_proxy.py
+-rw-r--r--  2.0 unx    31127 b- defN 24-May-20 11:05 nucliadb/search/search/query.py
+-rw-r--r--  2.0 unx     3018 b- defN 24-May-20 11:05 nucliadb/search/search/shards.py
+-rw-r--r--  2.0 unx     5101 b- defN 24-May-20 11:05 nucliadb/search/search/summarize.py
+-rw-r--r--  2.0 unx     2438 b- defN 24-May-20 11:05 nucliadb/search/search/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-20 11:05 nucliadb/search/search/chat/__init__.py
+-rw-r--r--  2.0 unx    16676 b- defN 24-May-20 11:05 nucliadb/search/search/chat/ask.py
+-rw-r--r--  2.0 unx     2058 b- defN 24-May-20 11:05 nucliadb/search/search/chat/images.py
+-rw-r--r--  2.0 unx    20793 b- defN 24-May-20 11:05 nucliadb/search/search/chat/prompt.py
+-rw-r--r--  2.0 unx    17543 b- defN 24-May-20 11:05 nucliadb/search/search/chat/query.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-20 11:05 nucliadb/search/tests/__init__.py
+-rw-r--r--  2.0 unx     1295 b- defN 24-May-20 11:05 nucliadb/search/tests/conftest.py
+-rw-r--r--  2.0 unx     6578 b- defN 24-May-20 11:05 nucliadb/search/tests/fixtures.py
+-rw-r--r--  2.0 unx    15480 b- defN 24-May-20 11:05 nucliadb/search/tests/node.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-20 11:05 nucliadb/search/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     2649 b- defN 24-May-20 11:05 nucliadb/search/tests/unit/test_app.py
+-rw-r--r--  2.0 unx     3374 b- defN 24-May-20 11:05 nucliadb/search/tests/unit/test_find_merge.py
+-rw-r--r--  2.0 unx     1400 b- defN 24-May-20 11:05 nucliadb/search/tests/unit/test_merge.py
+-rw-r--r--  2.0 unx    15721 b- defN 24-May-20 11:05 nucliadb/search/tests/unit/test_predict.py
+-rw-r--r--  2.0 unx     1328 b- defN 24-May-20 11:05 nucliadb/search/tests/unit/test_run.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-20 11:05 nucliadb/search/tests/unit/api/__init__.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-20 11:05 nucliadb/search/tests/unit/api/v1/__init__.py
+-rw-r--r--  2.0 unx     3759 b- defN 24-May-20 11:05 nucliadb/search/tests/unit/api/v1/test_ask.py
+-rw-r--r--  2.0 unx     2966 b- defN 24-May-20 11:05 nucliadb/search/tests/unit/api/v1/test_chat.py
+-rw-r--r--  2.0 unx     2865 b- defN 24-May-20 11:05 nucliadb/search/tests/unit/api/v1/test_predict_proxy.py
+-rw-r--r--  2.0 unx     2901 b- defN 24-May-20 11:05 nucliadb/search/tests/unit/api/v1/test_summarize.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-20 11:05 nucliadb/search/tests/unit/api/v1/resource/__init__.py
+-rw-r--r--  2.0 unx     3040 b- defN 24-May-20 11:05 nucliadb/search/tests/unit/api/v1/resource/test_chat.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-20 11:05 nucliadb/search/tests/unit/search/__init__.py
+-rw-r--r--  2.0 unx     8586 b- defN 24-May-20 11:05 nucliadb/search/tests/unit/search/test_chat_prompt.py
+-rw-r--r--  2.0 unx     3736 b- defN 24-May-20 11:05 nucliadb/search/tests/unit/search/test_fetch.py
+-rw-r--r--  2.0 unx     4306 b- defN 24-May-20 11:05 nucliadb/search/tests/unit/search/test_filters.py
+-rw-r--r--  2.0 unx     4492 b- defN 24-May-20 11:05 nucliadb/search/tests/unit/search/test_paragraphs.py
+-rw-r--r--  2.0 unx     3496 b- defN 24-May-20 11:05 nucliadb/search/tests/unit/search/test_predict_proxy.py
+-rw-r--r--  2.0 unx     5121 b- defN 24-May-20 11:05 nucliadb/search/tests/unit/search/test_query.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-20 11:05 nucliadb/search/tests/unit/search/requesters/__init__.py
+-rw-r--r--  2.0 unx     6455 b- defN 24-May-20 11:05 nucliadb/search/tests/unit/search/requesters/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-20 11:05 nucliadb/search/tests/unit/search/search/__init__.py
+-rw-r--r--  2.0 unx     1759 b- defN 24-May-20 11:05 nucliadb/search/tests/unit/search/search/test_shards.py
+-rw-r--r--  2.0 unx     2511 b- defN 24-May-20 11:05 nucliadb/search/tests/unit/search/search/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-20 11:05 nucliadb/standalone/__init__.py
+-rw-r--r--  2.0 unx     6746 b- defN 24-May-20 11:05 nucliadb/standalone/api_router.py
+-rw-r--r--  2.0 unx     5763 b- defN 24-May-20 11:05 nucliadb/standalone/app.py
+-rw-r--r--  2.0 unx     7800 b- defN 24-May-20 11:05 nucliadb/standalone/auth.py
+-rw-r--r--  2.0 unx     5313 b- defN 24-May-20 11:05 nucliadb/standalone/config.py
+-rw-r--r--  2.0 unx     6986 b- defN 24-May-20 11:05 nucliadb/standalone/introspect.py
+-rw-r--r--  2.0 unx     2488 b- defN 24-May-20 11:05 nucliadb/standalone/lifecycle.py
+-rw-r--r--  2.0 unx     1980 b- defN 24-May-20 11:05 nucliadb/standalone/migrations.py
+-rw-r--r--  2.0 unx     1322 b- defN 24-May-20 11:05 nucliadb/standalone/purge.py
+-rw-r--r--  2.0 unx     5429 b- defN 24-May-20 11:05 nucliadb/standalone/run.py
+-rw-r--r--  2.0 unx     5822 b- defN 24-May-20 11:05 nucliadb/standalone/settings.py
+-rw-r--r--  2.0 unx     3132 b- defN 24-May-20 11:05 nucliadb/standalone/versions.py
+-rw-r--r--  2.0 unx     2285 b- defN 24-May-20 11:05 nucliadb/standalone/static/favicon.ico
+-rw-r--r--  2.0 unx     3833 b- defN 24-May-20 11:05 nucliadb/standalone/static/index.html
+-rw-r--r--  2.0 unx     2639 b- defN 24-May-20 11:05 nucliadb/standalone/static/logo.svg
+-rw-r--r--  2.0 unx      835 b- defN 24-May-20 11:05 nucliadb/standalone/tests/__init__.py
+-rw-r--r--  2.0 unx     1294 b- defN 24-May-20 11:05 nucliadb/standalone/tests/conftest.py
+-rw-r--r--  2.0 unx     1319 b- defN 24-May-20 11:05 nucliadb/standalone/tests/fixtures.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-20 11:05 nucliadb/standalone/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1722 b- defN 24-May-20 11:05 nucliadb/standalone/tests/unit/test_api_router.py
+-rw-r--r--  2.0 unx     5509 b- defN 24-May-20 11:05 nucliadb/standalone/tests/unit/test_auth.py
+-rw-r--r--  2.0 unx     1334 b- defN 24-May-20 11:05 nucliadb/standalone/tests/unit/test_introspect.py
+-rw-r--r--  2.0 unx     1845 b- defN 24-May-20 11:05 nucliadb/standalone/tests/unit/test_migrations.py
+-rw-r--r--  2.0 unx     1546 b- defN 24-May-20 11:05 nucliadb/standalone/tests/unit/test_run.py
+-rw-r--r--  2.0 unx     1972 b- defN 24-May-20 11:05 nucliadb/standalone/tests/unit/test_versions.py
+-rw-r--r--  2.0 unx     1037 b- defN 24-May-20 11:05 nucliadb/tasks/__init__.py
+-rw-r--r--  2.0 unx     7655 b- defN 24-May-20 11:05 nucliadb/tasks/consumer.py
+-rw-r--r--  2.0 unx      924 b- defN 24-May-20 11:05 nucliadb/tasks/logger.py
+-rw-r--r--  2.0 unx     1378 b- defN 24-May-20 11:05 nucliadb/tasks/models.py
+-rw-r--r--  2.0 unx     3457 b- defN 24-May-20 11:05 nucliadb/tasks/producer.py
+-rw-r--r--  2.0 unx     1753 b- defN 24-May-20 11:05 nucliadb/tasks/registry.py
+-rw-r--r--  2.0 unx     1360 b- defN 24-May-20 11:05 nucliadb/tasks/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-20 11:05 nucliadb/tests/__init__.py
+-rw-r--r--  2.0 unx     1229 b- defN 24-May-20 11:05 nucliadb/tests/conftest.py
+-rw-r--r--  2.0 unx    22365 b- defN 24-May-20 11:05 nucliadb/tests/fixtures.py
+-rw-r--r--  2.0 unx     7549 b- defN 24-May-20 11:05 nucliadb/tests/tikv.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-20 11:05 nucliadb/tests/benchmarks/__init__.py
+-rw-r--r--  2.0 unx     3032 b- defN 24-May-20 11:05 nucliadb/tests/benchmarks/test_search.py
+-rw-r--r--  2.0 unx      919 b- defN 24-May-20 11:05 nucliadb/tests/knowledgeboxes/__init__.py
+-rw-r--r--  2.0 unx     7002 b- defN 24-May-20 11:05 nucliadb/tests/knowledgeboxes/philosophy_books.py
+-rw-r--r--  2.0 unx     3037 b- defN 24-May-20 11:05 nucliadb/tests/knowledgeboxes/ten_dummy_resources.py
+-rw-r--r--  2.0 unx     1148 b- defN 24-May-20 11:05 nucliadb/tests/migrations/__init__.py
+-rw-r--r--  2.0 unx     2726 b- defN 24-May-20 11:05 nucliadb/tests/migrations/test_migration_0017.py
+-rw-r--r--  2.0 unx     3662 b- defN 24-May-20 11:05 nucliadb/tests/migrations/test_migration_0018.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-20 11:05 nucliadb/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1487 b- defN 24-May-20 11:05 nucliadb/tests/unit/test_field_ids.py
+-rw-r--r--  2.0 unx     2780 b- defN 24-May-20 11:05 nucliadb/tests/unit/test_health.py
+-rw-r--r--  2.0 unx     1543 b- defN 24-May-20 11:05 nucliadb/tests/unit/test_kb_slugs.py
+-rw-r--r--  2.0 unx     7892 b- defN 24-May-20 11:05 nucliadb/tests/unit/test_learning_proxy.py
+-rw-r--r--  2.0 unx     2642 b- defN 24-May-20 11:05 nucliadb/tests/unit/test_metrics_exporter.py
+-rw-r--r--  2.0 unx     1341 b- defN 24-May-20 11:05 nucliadb/tests/unit/test_openapi.py
+-rw-r--r--  2.0 unx     3649 b- defN 24-May-20 11:05 nucliadb/tests/unit/test_purge.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-20 11:05 nucliadb/tests/unit/common/__init__.py
+-rw-r--r--  2.0 unx     1268 b- defN 24-May-20 11:05 nucliadb/tests/unit/common/test_context.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-20 11:05 nucliadb/tests/unit/common/cluster/__init__.py
+-rw-r--r--  2.0 unx    12240 b- defN 24-May-20 11:05 nucliadb/tests/unit/common/cluster/test_cluster.py
+-rw-r--r--  2.0 unx     5387 b- defN 24-May-20 11:05 nucliadb/tests/unit/common/cluster/test_kb_shard_manager.py
+-rw-r--r--  2.0 unx     9465 b- defN 24-May-20 11:05 nucliadb/tests/unit/common/cluster/test_rollover.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-20 11:05 nucliadb/tests/unit/common/cluster/discovery/__init__.py
+-rw-r--r--  2.0 unx     5627 b- defN 24-May-20 11:05 nucliadb/tests/unit/common/cluster/discovery/test_k8s.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-20 11:05 nucliadb/tests/unit/common/cluster/standalone/__init__.py
+-rw-r--r--  2.0 unx     3761 b- defN 24-May-20 11:05 nucliadb/tests/unit/common/cluster/standalone/test_service.py
+-rw-r--r--  2.0 unx     2136 b- defN 24-May-20 11:05 nucliadb/tests/unit/common/cluster/standalone/test_utils.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-20 11:05 nucliadb/tests/unit/common/maindb/__init__.py
+-rw-r--r--  2.0 unx     3579 b- defN 24-May-20 11:05 nucliadb/tests/unit/common/maindb/test_driver.py
+-rw-r--r--  2.0 unx     1869 b- defN 24-May-20 11:05 nucliadb/tests/unit/common/maindb/test_tikv.py
+-rw-r--r--  2.0 unx     3213 b- defN 24-May-20 11:05 nucliadb/tests/unit/common/maindb/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-20 11:05 nucliadb/tests/unit/export_import/__init__.py
+-rw-r--r--  2.0 unx     1435 b- defN 24-May-20 11:05 nucliadb/tests/unit/export_import/test_datamanager.py
+-rw-r--r--  2.0 unx     9706 b- defN 24-May-20 11:05 nucliadb/tests/unit/export_import/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-20 11:05 nucliadb/tests/unit/migrator/__init__.py
+-rw-r--r--  2.0 unx     3233 b- defN 24-May-20 11:05 nucliadb/tests/unit/migrator/test_migrator.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-20 11:05 nucliadb/tests/unit/tasks/__init__.py
+-rw-r--r--  2.0 unx     1375 b- defN 24-May-20 11:05 nucliadb/tests/unit/tasks/conftest.py
+-rw-r--r--  2.0 unx     2714 b- defN 24-May-20 11:05 nucliadb/tests/unit/tasks/test_consumer.py
+-rw-r--r--  2.0 unx     3189 b- defN 24-May-20 11:05 nucliadb/tests/unit/tasks/test_producer.py
+-rw-r--r--  2.0 unx     1827 b- defN 24-May-20 11:05 nucliadb/tests/unit/tasks/test_tasks.py
+-rw-r--r--  2.0 unx     2507 b- defN 24-May-20 11:05 nucliadb/tests/utils/__init__.py
+-rw-r--r--  2.0 unx     1797 b- defN 24-May-20 11:05 nucliadb/tests/utils/aiohttp_session.py
+-rw-r--r--  2.0 unx     2533 b- defN 24-May-20 11:05 nucliadb/tests/utils/entities.py
+-rw-r--r--  2.0 unx     6327 b- defN 24-May-20 11:05 nucliadb/tests/utils/broker_messages/__init__.py
+-rw-r--r--  2.0 unx     7557 b- defN 24-May-20 11:05 nucliadb/tests/utils/broker_messages/fields.py
+-rw-r--r--  2.0 unx     1196 b- defN 24-May-20 11:05 nucliadb/tests/utils/broker_messages/helpers.py
+-rw-r--r--  2.0 unx     1325 b- defN 24-May-20 11:05 nucliadb/train/__init__.py
+-rw-r--r--  2.0 unx     3530 b- defN 24-May-20 11:05 nucliadb/train/app.py
+-rw-r--r--  2.0 unx     3800 b- defN 24-May-20 11:05 nucliadb/train/generator.py
+-rw-r--r--  2.0 unx     1698 b- defN 24-May-20 11:05 nucliadb/train/lifecycle.py
+-rw-r--r--  2.0 unx     1198 b- defN 24-May-20 11:05 nucliadb/train/models.py
+-rw-r--r--  2.0 unx     5706 b- defN 24-May-20 11:05 nucliadb/train/nodes.py
+-rw-r--r--  2.0 unx     1400 b- defN 24-May-20 11:05 nucliadb/train/run.py
+-rw-r--r--  2.0 unx     5926 b- defN 24-May-20 11:05 nucliadb/train/servicer.py
+-rw-r--r--  2.0 unx     1415 b- defN 24-May-20 11:05 nucliadb/train/settings.py
+-rw-r--r--  2.0 unx     1496 b- defN 24-May-20 11:05 nucliadb/train/types.py
+-rw-r--r--  2.0 unx     3265 b- defN 24-May-20 11:05 nucliadb/train/upload.py
+-rw-r--r--  2.0 unx     6420 b- defN 24-May-20 11:05 nucliadb/train/uploader.py
+-rw-r--r--  2.0 unx     3179 b- defN 24-May-20 11:05 nucliadb/train/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-20 11:05 nucliadb/train/api/__init__.py
+-rw-r--r--  2.0 unx     1479 b- defN 24-May-20 11:05 nucliadb/train/api/utils.py
+-rw-r--r--  2.0 unx      928 b- defN 24-May-20 11:05 nucliadb/train/api/v1/__init__.py
+-rw-r--r--  2.0 unx     2071 b- defN 24-May-20 11:05 nucliadb/train/api/v1/check.py
+-rw-r--r--  2.0 unx      910 b- defN 24-May-20 11:05 nucliadb/train/api/v1/router.py
+-rw-r--r--  2.0 unx     1908 b- defN 24-May-20 11:05 nucliadb/train/api/v1/shards.py
+-rw-r--r--  2.0 unx     2135 b- defN 24-May-20 11:05 nucliadb/train/api/v1/trainset.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-20 11:05 nucliadb/train/generators/__init__.py
+-rw-r--r--  2.0 unx     3723 b- defN 24-May-20 11:05 nucliadb/train/generators/field_classifier.py
+-rw-r--r--  2.0 unx     6712 b- defN 24-May-20 11:05 nucliadb/train/generators/image_classifier.py
+-rw-r--r--  2.0 unx     2789 b- defN 24-May-20 11:05 nucliadb/train/generators/paragraph_classifier.py
+-rw-r--r--  2.0 unx     3590 b- defN 24-May-20 11:05 nucliadb/train/generators/paragraph_streaming.py
+-rw-r--r--  2.0 unx     5372 b- defN 24-May-20 11:05 nucliadb/train/generators/question_answer_streaming.py
+-rw-r--r--  2.0 unx     5160 b- defN 24-May-20 11:05 nucliadb/train/generators/sentence_classifier.py
+-rw-r--r--  2.0 unx    10446 b- defN 24-May-20 11:05 nucliadb/train/generators/token_classifier.py
+-rw-r--r--  2.0 unx     3877 b- defN 24-May-20 11:05 nucliadb/train/generators/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-20 11:05 nucliadb/train/tests/__init__.py
+-rw-r--r--  2.0 unx     1125 b- defN 24-May-20 11:05 nucliadb/train/tests/conftest.py
+-rw-r--r--  2.0 unx    11053 b- defN 24-May-20 11:05 nucliadb/train/tests/fixtures.py
+-rw-r--r--  2.0 unx     4598 b- defN 24-May-20 11:05 nucliadb/train/tests/test_field_classification.py
+-rw-r--r--  2.0 unx     2729 b- defN 24-May-20 11:05 nucliadb/train/tests/test_get_entities.py
+-rw-r--r--  2.0 unx     1876 b- defN 24-May-20 11:05 nucliadb/train/tests/test_get_info.py
+-rw-r--r--  2.0 unx     1382 b- defN 24-May-20 11:05 nucliadb/train/tests/test_get_ontology.py
+-rw-r--r--  2.0 unx     2417 b- defN 24-May-20 11:05 nucliadb/train/tests/test_get_ontology_count.py
+-rw-r--r--  2.0 unx     7669 b- defN 24-May-20 11:05 nucliadb/train/tests/test_image_classification.py
+-rw-r--r--  2.0 unx     1416 b- defN 24-May-20 11:05 nucliadb/train/tests/test_list_fields.py
+-rw-r--r--  2.0 unx     2944 b- defN 24-May-20 11:05 nucliadb/train/tests/test_list_paragraphs.py
+-rw-r--r--  2.0 unx     1423 b- defN 24-May-20 11:05 nucliadb/train/tests/test_list_resources.py
+-rw-r--r--  2.0 unx     2947 b- defN 24-May-20 11:05 nucliadb/train/tests/test_list_sentences.py
+-rw-r--r--  2.0 unx     4645 b- defN 24-May-20 11:05 nucliadb/train/tests/test_paragraph_classification.py
+-rw-r--r--  2.0 unx     4320 b- defN 24-May-20 11:05 nucliadb/train/tests/test_paragraph_streaming.py
+-rw-r--r--  2.0 unx     8751 b- defN 24-May-20 11:05 nucliadb/train/tests/test_question_answer_streaming.py
+-rw-r--r--  2.0 unx     5051 b- defN 24-May-20 11:05 nucliadb/train/tests/test_sentence_classification.py
+-rw-r--r--  2.0 unx     5583 b- defN 24-May-20 11:05 nucliadb/train/tests/test_token_classification.py
+-rw-r--r--  2.0 unx     3324 b- defN 24-May-20 11:05 nucliadb/train/tests/utils.py
+-rw-r--r--  2.0 unx     1328 b- defN 24-May-20 11:05 nucliadb/writer/__init__.py
+-rw-r--r--  2.0 unx     4268 b- defN 24-May-20 11:05 nucliadb/writer/app.py
+-rw-r--r--  2.0 unx    19483 b- defN 24-May-20 11:05 nucliadb/writer/back_pressure.py
+-rw-r--r--  2.0 unx      972 b- defN 24-May-20 11:05 nucliadb/writer/exceptions.py
+-rw-r--r--  2.0 unx     1953 b- defN 24-May-20 11:05 nucliadb/writer/lifecycle.py
+-rw-r--r--  2.0 unx     1032 b- defN 24-May-20 11:05 nucliadb/writer/openapi.py
+-rw-r--r--  2.0 unx     1448 b- defN 24-May-20 11:05 nucliadb/writer/run.py
+-rw-r--r--  2.0 unx     3103 b- defN 24-May-20 11:05 nucliadb/writer/settings.py
+-rw-r--r--  2.0 unx     1036 b- defN 24-May-20 11:05 nucliadb/writer/utilities.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-20 11:05 nucliadb/writer/api/__init__.py
+-rw-r--r--  2.0 unx     1429 b- defN 24-May-20 11:05 nucliadb/writer/api/constants.py
+-rw-r--r--  2.0 unx     1095 b- defN 24-May-20 11:05 nucliadb/writer/api/v1/__init__.py
+-rw-r--r--  2.0 unx     6571 b- defN 24-May-20 11:05 nucliadb/writer/api/v1/export_import.py
+-rw-r--r--  2.0 unx    24482 b- defN 24-May-20 11:05 nucliadb/writer/api/v1/field.py
+-rw-r--r--  2.0 unx     5248 b- defN 24-May-20 11:05 nucliadb/writer/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     2058 b- defN 24-May-20 11:05 nucliadb/writer/api/v1/learning_config.py
+-rw-r--r--  2.0 unx    18893 b- defN 24-May-20 11:05 nucliadb/writer/api/v1/resource.py
+-rw-r--r--  2.0 unx     1034 b- defN 24-May-20 11:05 nucliadb/writer/api/v1/router.py
+-rw-r--r--  2.0 unx    10747 b- defN 24-May-20 11:05 nucliadb/writer/api/v1/services.py
+-rw-r--r--  2.0 unx    30857 b- defN 24-May-20 11:05 nucliadb/writer/api/v1/upload.py
+-rw-r--r--  2.0 unx     1612 b- defN 24-May-20 11:05 nucliadb/writer/layouts/__init__.py
+-rw-r--r--  2.0 unx     2115 b- defN 24-May-20 11:05 nucliadb/writer/layouts/v1.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-20 11:05 nucliadb/writer/resource/__init__.py
+-rw-r--r--  2.0 unx     1425 b- defN 24-May-20 11:05 nucliadb/writer/resource/audit.py
+-rw-r--r--  2.0 unx    10968 b- defN 24-May-20 11:05 nucliadb/writer/resource/basic.py
+-rw-r--r--  2.0 unx    16319 b- defN 24-May-20 11:05 nucliadb/writer/resource/field.py
+-rw-r--r--  2.0 unx     2022 b- defN 24-May-20 11:05 nucliadb/writer/resource/origin.py
+-rw-r--r--  2.0 unx     1152 b- defN 24-May-20 11:05 nucliadb/writer/resource/slug.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-20 11:05 nucliadb/writer/tests/__init__.py
+-rw-r--r--  2.0 unx     1200 b- defN 24-May-20 11:05 nucliadb/writer/tests/conftest.py
+-rw-r--r--  2.0 unx     5971 b- defN 24-May-20 11:05 nucliadb/writer/tests/fixtures.py
+-rw-r--r--  2.0 unx    15472 b- defN 24-May-20 11:05 nucliadb/writer/tests/test_fields.py
+-rw-r--r--  2.0 unx    25999 b- defN 24-May-20 11:05 nucliadb/writer/tests/test_files.py
+-rw-r--r--  2.0 unx     1729 b- defN 24-May-20 11:05 nucliadb/writer/tests/test_knowledgebox.py
+-rw-r--r--  2.0 unx     4358 b- defN 24-May-20 11:05 nucliadb/writer/tests/test_reprocess_file_field.py
+-rw-r--r--  2.0 unx    16694 b- defN 24-May-20 11:05 nucliadb/writer/tests/test_resources.py
+-rw-r--r--  2.0 unx     5120 b- defN 24-May-20 11:05 nucliadb/writer/tests/test_service.py
+-rw-r--r--  2.0 unx     6054 b- defN 24-May-20 11:05 nucliadb/writer/tests/test_tus.py
+-rw-r--r--  2.0 unx     1287 b- defN 24-May-20 11:05 nucliadb/writer/tests/utils.py
+-rw-r--r--  2.0 unx     5226 b- defN 24-May-20 11:05 nucliadb/writer/tus/__init__.py
+-rw-r--r--  2.0 unx     5082 b- defN 24-May-20 11:05 nucliadb/writer/tus/dm.py
+-rw-r--r--  2.0 unx     2186 b- defN 24-May-20 11:05 nucliadb/writer/tus/exceptions.py
+-rw-r--r--  2.0 unx    14527 b- defN 24-May-20 11:05 nucliadb/writer/tus/gcs.py
+-rw-r--r--  2.0 unx     5849 b- defN 24-May-20 11:05 nucliadb/writer/tus/local.py
+-rw-r--r--  2.0 unx     4367 b- defN 24-May-20 11:05 nucliadb/writer/tus/pg.py
+-rw-r--r--  2.0 unx     9069 b- defN 24-May-20 11:05 nucliadb/writer/tus/s3.py
+-rw-r--r--  2.0 unx     4734 b- defN 24-May-20 11:05 nucliadb/writer/tus/storage.py
+-rw-r--r--  2.0 unx     2556 b- defN 24-May-20 11:05 nucliadb/writer/tus/utils.py
+-rw-r--r--  2.0 unx     4423 b- defN 24-May-20 11:06 nucliadb-4.0.0.post522.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-20 11:06 nucliadb-4.0.0.post522.dist-info/WHEEL
+-rw-r--r--  2.0 unx     1268 b- defN 24-May-20 11:06 nucliadb-4.0.0.post522.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       20 b- defN 24-May-20 11:06 nucliadb-4.0.0.post522.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-May-20 11:06 nucliadb-4.0.0.post522.dist-info/zip-safe
+-rw-rw-r--  2.0 unx    43241 b- defN 24-May-20 11:06 nucliadb-4.0.0.post522.dist-info/RECORD
+461 files, 2261463 bytes uncompressed, 695047 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -360,14 +360,17 @@
 
 Filename: nucliadb/ingest/orm/utils.py
 Comment: 
 
 Filename: nucliadb/ingest/orm/processor/__init__.py
 Comment: 
 
+Filename: nucliadb/ingest/orm/processor/auditing.py
+Comment: 
+
 Filename: nucliadb/ingest/orm/processor/sequence_manager.py
 Comment: 
 
 Filename: nucliadb/ingest/service/__init__.py
 Comment: 
 
 Filename: nucliadb/ingest/service/exceptions.py
@@ -1356,26 +1359,26 @@
 
 Filename: nucliadb/writer/tus/storage.py
 Comment: 
 
 Filename: nucliadb/writer/tus/utils.py
 Comment: 
 
-Filename: nucliadb-4.0.0.post520.dist-info/METADATA
+Filename: nucliadb-4.0.0.post522.dist-info/METADATA
 Comment: 
 
-Filename: nucliadb-4.0.0.post520.dist-info/WHEEL
+Filename: nucliadb-4.0.0.post522.dist-info/WHEEL
 Comment: 
 
-Filename: nucliadb-4.0.0.post520.dist-info/entry_points.txt
+Filename: nucliadb-4.0.0.post522.dist-info/entry_points.txt
 Comment: 
 
-Filename: nucliadb-4.0.0.post520.dist-info/top_level.txt
+Filename: nucliadb-4.0.0.post522.dist-info/top_level.txt
 Comment: 
 
-Filename: nucliadb-4.0.0.post520.dist-info/zip-safe
+Filename: nucliadb-4.0.0.post522.dist-info/zip-safe
 Comment: 
 
-Filename: nucliadb-4.0.0.post520.dist-info/RECORD
+Filename: nucliadb-4.0.0.post522.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nucliadb/ingest/consumer/auditing.py

```diff
@@ -19,22 +19,17 @@
 #
 
 import asyncio
 import logging
 import uuid
 from functools import partial
 
-from nucliadb_protos.resources_pb2 import FieldType
-
 from nucliadb.common.cluster.exceptions import ShardsNotFound
 from nucliadb.common.cluster.manager import choose_node
 from nucliadb.common.cluster.utils import get_shard_manager
-from nucliadb.common.maindb.driver import Driver
-from nucliadb.ingest.orm.knowledgebox import KnowledgeBox
-from nucliadb.ingest.orm.resource import Resource
 from nucliadb_protos import audit_pb2, nodereader_pb2, noderesources_pb2, writer_pb2
 from nucliadb_utils import const
 from nucliadb_utils.audit.audit import AuditStorage
 from nucliadb_utils.cache.pubsub import PubSubDriver
 from nucliadb_utils.storages.storage import Storage
 
 from . import metrics
@@ -58,20 +53,18 @@
 
     subscription_id: str
     loop: asyncio.AbstractEventLoop
 
     def __init__(
         self,
         *,
-        driver: Driver,
         audit: AuditStorage,
         pubsub: PubSubDriver,
         check_delay: float = 5.0,
     ):
-        self.driver = driver
         self.audit = audit
         self.pubsub = pubsub
         self.shard_manager = get_shard_manager()
         self.task_handler = DelayedTaskHandler(check_delay)
 
     async def initialize(self) -> None:
         self.loop = asyncio.get_running_loop()
@@ -143,20 +136,18 @@
     """
 
     subscription_id: str
 
     def __init__(
         self,
         *,
-        driver: Driver,
         storage: Storage,
         audit: AuditStorage,
         pubsub: PubSubDriver,
     ):
-        self.driver = driver
         self.storage = storage
         self.audit = audit
         self.pubsub = pubsub
 
     async def initialize(self) -> None:
         self.subscription_id = str(uuid.uuid4())
         await self.pubsub.subscribe(
@@ -165,151 +156,41 @@
             group="audit-writes",
             subscription_id=self.subscription_id,
         )
 
     async def finalize(self) -> None:
         await self.pubsub.unsubscribe(self.subscription_id)
 
-    def iterate_auditable_fields(
-        self,
-        resource_keys: list[tuple[FieldType.ValueType, str]],
-        message: writer_pb2.BrokerMessage,
-    ):
-        """
-        Generator that emits the combined list of field ids from both
-        the existing resource and message that needs to be considered
-        in the audit of fields.
-        """
-        yielded = set()
-
-        # Include all fields present in the message we are processing
-        for field_id in message.files.keys():
-            key = (field_id, writer_pb2.FieldType.FILE)
-            yield key
-            yielded.add(key)
-
-        for field_id in message.conversations.keys():
-            key = (field_id, writer_pb2.FieldType.CONVERSATION)
-            yield key
-            yielded.add(key)
-
-        for field_id in message.layouts.keys():
-            key = (field_id, writer_pb2.FieldType.LAYOUT)
-            yield key
-            yielded.add(key)
-
-        for field_id in message.texts.keys():
-            key = (field_id, writer_pb2.FieldType.TEXT)
-            yield key
-            yielded.add(key)
-
-        for field_id in message.keywordsets.keys():
-            key = (field_id, writer_pb2.FieldType.KEYWORDSET)
-            yield key
-            yielded.add(key)
-
-        for field_id in message.datetimes.keys():
-            key = (field_id, writer_pb2.FieldType.DATETIME)
-            yield key
-            yielded.add(key)
-
-        for field_id in message.links.keys():
-            key = (field_id, writer_pb2.FieldType.LINK)
-            yield key
-            yielded.add(key)
-
-        for field_type, field_id in resource_keys:
-            if field_type is writer_pb2.FieldType.GENERIC:
-                continue
-
-            if not (
-                field_id in message.files
-                or message.type is writer_pb2.BrokerMessage.MessageType.DELETE
-            ):
-                continue
-
-            # Avoid duplicates
-            if (field_type, field_id) in yielded:
-                continue
-
-            yield (field_id, field_type)
-
-    async def collect_audit_fields(
-        self, message: writer_pb2.BrokerMessage
-    ) -> list[audit_pb2.AuditField]:
-        if message.type == writer_pb2.BrokerMessage.MessageType.DELETE:
-            # If we are fully deleting a resource we won't iterate the delete_fields (if any).
-            # Make no sense as we already collected all resource fields as deleted
-            return []
-
-        audit_storage_fields: list[audit_pb2.AuditField] = []
-        async with self.driver.transaction() as txn:
-            kb = KnowledgeBox(txn, self.storage, message.kbid)
-            resource = Resource(txn, self.storage, kb, message.uuid)
-            field_keys = await resource.get_fields_ids()
-
-            for field_id, field_type in self.iterate_auditable_fields(
-                field_keys, message
-            ):
-                auditfield = audit_pb2.AuditField()
-                auditfield.field_type = field_type
-                auditfield.field_id = field_id
-                if field_type is writer_pb2.FieldType.FILE:
-                    auditfield.filename = message.files[field_id].file.filename
-                # The field did exist, so we are overwriting it, with a modified file
-                # in case of a file
-                auditfield.action = audit_pb2.AuditField.FieldAction.MODIFIED
-                if field_type is writer_pb2.FieldType.FILE:
-                    auditfield.size = message.files[field_id].file.size
-
-                audit_storage_fields.append(auditfield)
-
-            for fieldid in message.delete_fields or []:
-                field = await resource.get_field(
-                    fieldid.field, writer_pb2.FieldType.FILE, load=True
-                )
-                audit_field = audit_pb2.AuditField()
-                audit_field.action = audit_pb2.AuditField.FieldAction.DELETED
-                audit_field.field_id = fieldid.field
-                audit_field.field_type = fieldid.field_type
-                if fieldid.field_type is writer_pb2.FieldType.FILE:
-                    val = await field.get_value()
-                    audit_field.size = 0
-                    if val is not None:
-                        audit_field.filename = val.file.filename
-                audit_storage_fields.append(audit_field)
-
-        return audit_storage_fields
-
     async def handle_message(self, raw_data) -> None:
         data = self.pubsub.parse(raw_data)
         notification = writer_pb2.Notification()
         notification.ParseFromString(data)
 
         if notification.write_type == notification.WriteType.UNSET:
             metrics.total_messages.inc({"action": "ignored", "type": "audit_fields"})
             return
 
-        message = notification.message
-        if message.source == message.MessageSource.PROCESSOR:
+        message_audit: writer_pb2.Audit = notification.message_audit
+        if (
+            message_audit.message_source
+            == writer_pb2.BrokerMessage.MessageSource.PROCESSOR
+        ):
             metrics.total_messages.inc({"action": "ignored", "type": "audit_fields"})
             return
 
         logger.info(
             {"message": "Processing field audit for kbid", "kbid": notification.kbid}
         )
 
         metrics.total_messages.inc({"action": "scheduled", "type": "audit_fields"})
         with metrics.handler_histo({"type": "audit_fields"}):
-            audit_fields = await self.collect_audit_fields(message)
-            field_metadata = [fi.field for fi in message.field_metadata]
-            when = message.audit.when if message.audit.HasField("when") else None
+            when = message_audit.when if message_audit.HasField("when") else None
             await self.audit.report(
-                kbid=message.kbid,
+                kbid=message_audit.kbid,
                 when=when,
-                user=message.audit.user,
-                rid=message.uuid,
-                origin=message.audit.origin,
-                field_metadata=field_metadata,
+                user=message_audit.user,
+                rid=message_audit.uuid,
+                origin=message_audit.origin,
+                field_metadata=list(message_audit.field_metadata),
                 audit_type=AUDIT_TYPES.get(notification.write_type),
-                audit_fields=audit_fields,
+                audit_fields=list(message_audit.audit_fields),
             )
```

## nucliadb/ingest/consumer/service.py

```diff
@@ -155,23 +155,22 @@
     )
     await consumer.initialize()
 
     return nats_connection_manager.finalize
 
 
 async def start_auditor() -> Callable[[], Awaitable[None]]:
-    driver = await setup_driver()
     audit = get_audit()
     assert audit is not None
     pubsub = await get_pubsub()
     assert pubsub is not None, "Pubsub is not configured"
     storage = await get_storage(service_name=SERVICE_NAME)
-    index_auditor = IndexAuditHandler(driver=driver, audit=audit, pubsub=pubsub)
+    index_auditor = IndexAuditHandler(audit=audit, pubsub=pubsub)
     resource_writes_auditor = ResourceWritesAuditHandler(
-        driver=driver, storage=storage, audit=audit, pubsub=pubsub
+        storage=storage, audit=audit, pubsub=pubsub
     )
 
     await index_auditor.initialize()
     await resource_writes_auditor.initialize()
 
     return partial(
         asyncio.gather, index_auditor.finalize(), resource_writes_auditor.finalize()  # type: ignore
```

## nucliadb/ingest/orm/processor/__init__.py

```diff
@@ -33,14 +33,15 @@
     KnowledgeBoxConflict,
     ResourceNotIndexable,
     SequenceOrderViolation,
 )
 from nucliadb.ingest.orm.knowledgebox import KnowledgeBox
 from nucliadb.ingest.orm.metrics import processor_observer
 from nucliadb.ingest.orm.processor import sequence_manager
+from nucliadb.ingest.orm.processor.auditing import collect_audit_fields
 from nucliadb.ingest.orm.resource import Resource
 from nucliadb_protos import (
     knowledgebox_pb2,
     noderesources_pb2,
     nodewriter_pb2,
     resources_pb2,
     utils_pb2,
@@ -511,36 +512,50 @@
             return
 
         await resource.set_basic(
             message.basic,
             deleted_fields=message.delete_fields,  # type: ignore
         )
 
+    async def get_extended_audit_data(
+        self, message: writer_pb2.BrokerMessage
+    ) -> writer_pb2.Audit:
+        message_audit = writer_pb2.Audit()
+        message_audit.CopyFrom(message.audit)
+        message_audit.kbid = message.kbid
+        message_audit.uuid = message.uuid
+        message_audit.message_source = message.source
+        message_audit.field_metadata.extend(
+            [fcmw.field for fcmw in message.field_metadata]
+        )
+        audit_fields = await collect_audit_fields(self.driver, self.storage, message)
+        message_audit.audit_fields.extend(audit_fields)
+        return message_audit
+
     async def notify_commit(
         self,
         *,
         partition: str,
         seqid: int,
         multi: str,
         message: writer_pb2.BrokerMessage,
         write_type: writer_pb2.Notification.WriteType.ValueType,
     ):
+        message_audit = await self.get_extended_audit_data(message)
         notification = writer_pb2.Notification(
             partition=int(partition),
             seqid=seqid,
             multi=multi,
             uuid=message.uuid,
             kbid=message.kbid,
             action=writer_pb2.Notification.Action.COMMIT,
             write_type=write_type,
             source=MESSAGE_TO_NOTIFICATION_SOURCE[message.source],
-            # including the message here again might feel a bit unusual but allows
-            # us to react to these notifications with the original payload
-            message=message,
             processing_errors=len(message.errors) > 0,
+            message_audit=message_audit,
         )
 
         await self.notify(
             const.PubSubChannels.RESOURCE_NOTIFY.format(kbid=message.kbid),
             notification.SerializeToString(),
         )
```

## nucliadb/ingest/tests/integration/consumer/test_auditing.py

```diff
@@ -27,15 +27,14 @@
 from nucliadb_utils import const
 from nucliadb_utils.audit.stream import StreamAuditStorage
 
 pytestmark = pytest.mark.asyncio
 
 
 async def test_audit_counters(
-    maindb_driver,
     stream_audit: StreamAuditStorage,
     pubsub,
     nats_manager,
     fake_node,
     knowledgebox_ingest,
 ):
     from nucliadb_utils.settings import audit_settings
@@ -46,15 +45,14 @@
     )
     await nats_manager.js.add_stream(
         name=audit_settings.audit_stream, subjects=[subject]
     )
     psub = await nats_manager.js.pull_subscribe(subject, "psub")
 
     iah = auditing.IndexAuditHandler(
-        driver=maindb_driver,
         audit=stream_audit,
         pubsub=pubsub,
         check_delay=0.05,
     )
     await iah.initialize()
 
     await pubsub.publish(
```

## nucliadb/ingest/tests/integration/ingest/test_ingest.py

```diff
@@ -65,24 +65,20 @@
 
 EXAMPLE_VECTOR = base64.b64decode(
     "k05VTVBZAQB2AHsnZGVzY3InOiAnPGY0JywgJ2ZvcnRyYW5fb3JkZXInOiBGYWxzZSwgJ3NoYXBlJzogKDc2OCwpLCB9ICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIAogKIq+lgYUvvf7bTx39oo+fFaXPbx2a71RfiK/FBroPVTawr4UEm2+AgtuvWzTTT5ipjg9JflLvMdfub6fBIE+d7gmvnJPl75alUQ+n68Hv2BYJL20+74+bHDsPV/wTT63h4E9hes9PqxHXT6h/J079HfVPF/7BD3BSMO+PuA9PjJhtD4W6pq+rmwjPp+Fzz6xUfa+FMZtOutIBT4mPik+EbsAPyRePb41IVW+i+0RPT7GtL51USY+GRjRvjWD1z4+wq+9j9kqvmq/074hHBM+kh+ZPoRfmb6R0yi/kuirvlcqLj+Ss64+0cMBP2UKsD2LtpI9927BvtCfHb5KY7U+8s64vkcGX778+NY+2pMxPNowJD7R39u+dbmfPqbrL73bIby+Nbu8voH3kr4gps6+f3L6PuJFAb3PFWA+99BPPjkLzD0vc8m79JmtvWYnbL6W+6A+WUWEveVVED0V0h8+3zPWvv19Dr2igdC9JcGRPV568z41ZVu8mRxRvdkBQr73JHO+PFxkvtHatLzVgN49NEgav0l7ab276hK+ABMDvrRrJj4akbO++zFnPRzXoDyecdi+pGq4viUgiL4XXwK+tvcOPivvgD7PV0w+D7CwPmfoiL0REec+tsx1Pe2xkD6S9Jm+ZW09P1Obiz2Ov/Q+OtsBP8Xicj7WJpi9szGJvqvWvz4hFqG++ZuGvIAmMb0r+T2+wj9RPgZN0z7KwGI+ezogPgI78D6aUrW8etzkPHpSqb7c4Sg+b6BZvXlSrr6un6a8uUCrvhbBgb7PtwA+CsSwvQzyz73G1eq+plYZP/6I7r6BRsu992/gPuIBJj9aT8u94saNvdIDG76Zar4+GeRxvncSZz3citO+ILq6vmS3D78JHk6/NdeIPWYQwb0WZJW9OnwJPhdIQL7Gta6+MZWevpRNvr0ZH/c9B//hPtNUlL1pWhu/VliNvshFjT6laVS9EpjovQBHdb4HWMe+e/rfvrcSDz620/I+krapPlnIDz5uR1Y+znjqPTFM+T1+kK8+VMcevDegSjvM7fw+e0yKPbDoVz56wk4+EeoGvnq3rT76dbW+ghE6vvos0b6CqQu+p6JDPvzn2bogOui+oZU5v6/Pvr4siDI9Kv6Dvt6TQj51LqW+qYLsPmyjZT45DkG9MQivPgIHBT/qeRW/ghXOPkcJtL6MwhA/9F5PvbR7Jr4ftKA+mdkePwm2A77WpNU+Ho/NvsWEfL75zPS9v8ycvtXFVD5ONFI7mVkOPlFd7bzacZK7aSyRPkRrhz6e8+k+glJ5Pq9mmD0X95y+APOjPveVBb9yOgM+DLlMPkqCRb7CKwW8N+TevpZtmD5lbpq+n+tdPr4+m7661Wg+gd66ve5dzr2ZH7k+x/aNPo+0Kz4PMMa+voMGv+ud8r4Nape892YZPWlDL76twQi/RC2QPk8juz1uTwC9yf3rvn8RmD5LO0e+7t5CvvYTbb5O8UA/yrZqO7aZib6FBEe+n/xAv08BGr15Vxs/FNIevkbN1r3f2Hw+oj18PJwOnb3SDpo+wf67vvy3sj6qvRM/BrljPtrlBr4w2Ck9Jh6fPv6Vn75qa7w+eWShvj6bYj56q46+x41KPvQtqb2qXVm+DTmTPpvXWz5hUnC9f7ptPAu1tsDAcUa+ckyGvTeaIz3FcaC9Zu/cvYvjzD7WUdQ+P2DFvrbdHz4CfVe+HxwAP3HZy775Q7w+eg+svcccuTwLBFW+QkVhPuSSjLymH6g+DFBKviDgWz0wxyK+1C+3PSKk975Hkxi8FKzVvRnykD5lFCa/bqnBPRACHL5uUS+/Zb3FvoK66j5CHUu+vq4TvkxWfT5wv7o+wW79PJHsrD42Aau+SuQFvdzUnz50dEe+qZNjvmZ1LLxvt529oeHDPsv3dT5O+z69vOoevm/1Cz5O7NU9i6uHPibkEr6g5d2+LobFPn+KAT/gLsY+2jm4vlpyhD48l4g+yqx3Pql7yr5sIYK+7awLPlnODb+3e7i+t9RVPQC99z6SQJk+lbXoPbyAI7mKcCu/4kX9vFuhtL61fhq+UjGgvYxSvDzCzfw+24xfvs+Sjr782jy+kTzaPmEqtD6sN2c9otXavSqTiT5hM/q+MjAFP4kflT5JOe280NUmvrQtkT4f55m9CyFwPr8GF7wNzBm+x05SvsFJtz0MG9w+HCf/vn4mkr7iMiw+DmhCPUDI/j3PrVe+glX3vlpDPz8ucKG+MexCPgoBDD+FMn68BMDnvCf+UT3bgq4+srqvvYF8H7+1VKq9qbQTvY1tBL8epwC85PUdviSEhD7hg7e9jMUzvVuFz71qCf29IudEPsAwH767q809fL0uvrk+Mr7OTVy9TNcWvhnV3T4hOwq/F/E3P4UOXz4Vade+fK8TP5v4sr4Amf8+HCqPvmYV7Lo3UMK+0urYPrSH3zw/8oq9tAHCvvs5GD91e6w9GsqJPNRo7j5ffH6+X++MvKFQxj17Es6+TA5OvW8tAz8C4nU8tiHDvm5FZL5Kv3O+fuZ0Php/9j0Gyua+mSKVvs+pDT8+TwC/qS8Gvl/z0r5iVLq+a8e/vIXlIT4r7Ty+dqrXPmn9Db4p4PS+Kv0nPfnVUz7avj0+KVOTPkG3Kz68dQa+LSKGvXnRvjxnzyM92moTvy9SnD4F9Dw+mWoyvXpXRD8nm7I9O245P6KlZT4zCxc+baKLPsyE0rw8YHO+coGePfcAYT300Jw+UoeUvlvHFD7CjpC+p9KpvlteKrvgzwG8Sbg2vn8NDz5MDtW99URGvoaaxb0svk+9+cajvUvAab1qXpS91FSbvszYlj6f9oI+Ge5yPDdVxr45qV2+WmuxPcx+qj5l88W9ApSIvsFrwT4GT8c+Vg/0PjkNT745ezC/9ogqPm7bE7/Wh1O9b7NrvlVU/j4u3ga9mv+xvaHTtD76O40+LIyTvssUDT73Q5y+QO5TvX7bgj3gY5S+YTSfvpYeIL6a+Y29CLmZvda6xz6cC9Q+9sQSPwnG+j3RS927zvaAvq7iLz0CqPw9Fir+vNr7VT5qEgM+yhqtupy5q76uVtE7eZ+Nvi/7h75rkLq9vOW0O7QhFj7JCbc+3tp7vlpEOT9+aPc+hwnnvkqLPr0Ry/4+8zOaPfE0O70OJ6I9eQlJvbAU/T0KcaK8gS2Kvulxdj0u2JY+u4mxPN4vXj7B6xQ+LjBLvuTgJ77vq7M7KbcIvnbIdD0UQd++ZyuHvlaAPr4SeMw++sRuvZ7sXz3yJ5O9cSmPvZ8mRL7X2JM9trN4PpzLt70C3Og94uwLv4pACb8LWoY9Uz+ZPvE1Ij4R8HG9JVyJvvFOZz6XkIU+had5PvoQKT7h3CK+IzATv1U3qrxUum68B1bDviBzhz7u5XI9KXwkPoszXr6en5I9VNxMPAKusT5XGTg8Ne9GvC6yBz/EidM+V8T8u3LO1D7qSJa+AlsUPeb9pb0vNFK+lFCevTGrR70aeSu+zihyvOLan77CaxE/5ZnaPUv8Nr/hBhs+oCZBPttGqr5ZrwO+O0DGPU7JOD7FxdK+pw6CPWumgz6VB7++Gjb1vq6Ns7uZ1FI9VmTLPsl2iz7h5YI8CJYXvh6MSz6ucvc9qx1bPovgpT7ZWyO+Z+d1vrXkrz3VC8s+dmievuxuHb7MOXE+ewUCvJcPuT6n2Rc8mQyYvl45Gr1ER3c9LCZYvmqQhb1lVJu+V1acPZp63z5Cfmu+4NFZPvmBJb6cmAI+J0U7PsLkSb16KrO9wj4JPo4Fq7563+09jAw8vkYbbD7/Z5q7TH1kvnJrLb1mqkS+R+a9vX0ODD4p9ak+un8VO6mSp71C66w+FlLVPr/0Wb0eLR2+AneHvVTFHD/P0X0+TsQ4vlWQQzzP8no6VtEOPHLiG78Foyg+Un5OP/fFeL3uVxc+C1VzP9IInL2Zbbo8bw2Lvt5f0b4LY9w9LyaMvIcBc70K3bs+9lz5vTSTC7770MG+B4dHvvRFSz3lO6w9ENACv5NLBz20vSk+MuMQPLQYZr/2+6o+gzANvXGTjL259Qy9ZUMKPnyCC7498ww8oGGSvouNujyvJVW+TjmIvvI8KT667mq9MC6fvVUcvz0="  # noqa
 )
 
 
 @pytest.fixture(autouse=True)
-async def audit_consumers(
-    maindb_driver: Driver, storage, pubsub, stream_audit: StreamAuditStorage
-):
+async def audit_consumers(storage, pubsub, stream_audit: StreamAuditStorage):
     index_auditor = IndexAuditHandler(
-        driver=maindb_driver,
         audit=stream_audit,
         pubsub=pubsub,
     )
     resource_writes_auditor = ResourceWritesAuditHandler(
-        driver=maindb_driver,
         storage=storage,
         audit=stream_audit,
         pubsub=pubsub,
     )
 
     await index_auditor.initialize()
     await resource_writes_auditor.initialize()
```

## nucliadb/ingest/tests/unit/consumer/test_auditing.py

```diff
@@ -19,15 +19,15 @@
 #
 
 import asyncio
 from unittest.mock import AsyncMock, MagicMock, patch
 
 import pytest
 from nucliadb_protos.audit_pb2 import AuditKBCounter, AuditRequest
-from nucliadb_protos.writer_pb2 import BrokerMessage, Notification, ShardObject
+from nucliadb_protos.writer_pb2 import Audit, BrokerMessage, Notification, ShardObject
 
 from nucliadb.ingest.consumer import auditing
 from nucliadb_protos import nodereader_pb2
 
 pytestmark = pytest.mark.asyncio
 
 
@@ -62,28 +62,26 @@
 def audit():
     yield AsyncMock()
 
 
 @pytest.fixture()
 async def index_audit_handler(pubsub, audit, shard_manager):
     iah = auditing.IndexAuditHandler(
-        driver=AsyncMock(transaction=MagicMock(return_value=AsyncMock())),
         audit=audit,
         pubsub=pubsub,
         check_delay=0.05,
     )
     await iah.initialize()
     yield iah
     await iah.finalize()
 
 
 @pytest.fixture()
 async def writes_audit_handler(pubsub, audit, shard_manager):
     rwah = auditing.ResourceWritesAuditHandler(
-        driver=AsyncMock(transaction=MagicMock(return_value=AsyncMock())),
         storage=AsyncMock(),
         audit=audit,
         pubsub=pubsub,
     )
     await rwah.initialize()
     yield rwah
     await rwah.finalize()
@@ -122,20 +120,20 @@
 
     audit.report.assert_not_called()
 
 
 async def test_resource_handle_message_processor_messages_are_not_audited(
     writes_audit_handler: auditing.ResourceWritesAuditHandler, audit
 ):
-    message = BrokerMessage()
-    message.source = BrokerMessage.MessageSource.PROCESSOR
+    message_audit = Audit()
+    message_audit.message_source = BrokerMessage.MessageSource.PROCESSOR
     notif = Notification(
         kbid="kbid",
         action=Notification.Action.COMMIT,
-        message=message,
         write_type=Notification.WriteType.MODIFIED,
+        message_audit=message_audit,
     )
     await writes_audit_handler.handle_message(notif.SerializeToString())
 
     await writes_audit_handler.finalize()
 
     audit.report.assert_not_called()
```

## nucliadb/reader/reader/notifications.py

```diff
@@ -97,17 +97,14 @@
 
     subscription_key = const.PubSubChannels.RESOURCE_NOTIFY.format(kbid=kbid)
 
     def subscription_handler(raw_data: bytes):
         data = pubsub.parse(raw_data)
         notification = writer_pb2.Notification()
         notification.ParseFromString(data)
-        # We don't need the whole broker message, so we clear it to
-        # save space, as it can potentially be very big
-        notification.ClearField("message")
         try:
             queue.put_nowait(notification)
         except asyncio.QueueFull:  # pragma: no cover
             logger.warning("Queue is full, dropping notification", extra={"kbid": kbid})
 
     async with managed_subscription(
         pubsub, key=subscription_key, handler=subscription_handler
```

## Comparing `nucliadb-4.0.0.post520.dist-info/METADATA` & `nucliadb-4.0.0.post522.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nucliadb
-Version: 4.0.0.post520
+Version: 4.0.0.post522
 Home-page: https://docs.nuclia.dev/docs/guides/nucliadb/intro
 Author: NucliaDB Community
 Author-email: nucliadb@nuclia.com
 License: BSD
 Project-URL: Nuclia, https://nuclia.com
 Project-URL: Github, https://github.com/nuclia/nucliadb
 Project-URL: Discord, https://discord.gg/8EvQwmsbzf
@@ -17,18 +17,18 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
-Requires-Dist: nucliadb-telemetry[all] >=4.0.0.post520
-Requires-Dist: nucliadb-utils[cache,fastapi,storages] >=4.0.0.post520
-Requires-Dist: nucliadb-protos >=4.0.0.post520
-Requires-Dist: nucliadb-models >=4.0.0.post520
+Requires-Dist: nucliadb-telemetry[all] >=4.0.0.post522
+Requires-Dist: nucliadb-utils[cache,fastapi,storages] >=4.0.0.post522
+Requires-Dist: nucliadb-protos >=4.0.0.post522
+Requires-Dist: nucliadb-models >=4.0.0.post522
 Requires-Dist: nucliadb-admin-assets >=1.0.0.post1224
 Requires-Dist: nucliadb-node-binding >=2.26.0
 Requires-Dist: uvicorn <0.19.0
 Requires-Dist: argdantic
 Requires-Dist: aiohttp >=3.9.4
 Requires-Dist: lru-dict >=1.1.7
 Requires-Dist: backoff
```

## Comparing `nucliadb-4.0.0.post520.dist-info/entry_points.txt` & `nucliadb-4.0.0.post522.dist-info/entry_points.txt`

 * *Files identical despite different names*

## Comparing `nucliadb-4.0.0.post520.dist-info/RECORD` & `nucliadb-4.0.0.post522.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -87,20 +87,20 @@
 nucliadb/ingest/cache.py,sha256=w7jMMzamOmQ7gwXna6Dqm6isRNBVv6l5BTBlTxaYWjE,1005
 nucliadb/ingest/partitions.py,sha256=xhonCO-gqNO-8TlitjcmchVrxCLi-99SyOWvX4va1lE,2484
 nucliadb/ingest/processing.py,sha256=om3h33CS5jDZuFdErTzLHWaUlgy8Ul-1ULKs0o7cOoQ,19555
 nucliadb/ingest/serialize.py,sha256=DM18fONnptJbUqSFQZl4kg33Q8S4GpJUqK432rzSHYU,20277
 nucliadb/ingest/settings.py,sha256=VrOfSSwadDb2LRl0rwlJl5DSiDILj03KSD-n0Jh4yaE,3207
 nucliadb/ingest/utils.py,sha256=dyFEv9V38OlkrQdM8_Xgii3YmbsRqNUoZeYApe39kx0,2314
 nucliadb/ingest/consumer/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
-nucliadb/ingest/consumer/auditing.py,sha256=rFaYeytyAbX_DfB4u8_s8m8pIXbRjmA5JMkKkD59SnI,11563
+nucliadb/ingest/consumer/auditing.py,sha256=P6a7HgEJVE5WBJuyL7Q2avuqLqQ5QE3VaxoifS3YT3k,6918
 nucliadb/ingest/consumer/consumer.py,sha256=bJgVt1G7RchZrHX-5ykG2uHfGNY_HEjsLE2ZsgAv8HA,12174
 nucliadb/ingest/consumer/materializer.py,sha256=LGd_E3-9_DlXhjmg6iQX5SGHlR1soq5AtkWWfQwfdcQ,3788
 nucliadb/ingest/consumer/metrics.py,sha256=ji1l_4cKiHJthQd8YNem1ft4iMbw9KThmVvJmLcv3Xg,1075
 nucliadb/ingest/consumer/pull.py,sha256=DQ0_EOjMk4AdYqC1sSX4zVtF4IyrsWT-kaQbAjIs3H4,9543
-nucliadb/ingest/consumer/service.py,sha256=KGk6BVA6qjlXRKFD5UIiQVtYl9ca0h0qgZXypjzwQdE,6935
+nucliadb/ingest/consumer/service.py,sha256=873H7IGwpJM7Nhmfzr0RMDSXF3uTSQ2ctkBpWo-IgwU,6871
 nucliadb/ingest/consumer/shard_creator.py,sha256=FmKQSOOC19fsr72qoJ5cbZhnU5t8XnD3nr2TBFXW_js,4331
 nucliadb/ingest/consumer/utils.py,sha256=6zWurmmhOmu80uk-fjUhJB1rrulxArlhaUWFLIY-2Jg,2656
 nucliadb/ingest/fields/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/ingest/fields/base.py,sha256=fhAygZkwhi2rywDFmD6wpkYlMN953sVrNHL749HVroc,18433
 nucliadb/ingest/fields/conversation.py,sha256=ZUPad5gS_hBlrVyWx8OSK_tsn_fkJh2EcubkgV9eyio,6516
 nucliadb/ingest/fields/date.py,sha256=jXMWfdCv87oVySDQORXhMZ1Zvpw_aOpcrYAfUSnL3uA,1223
 nucliadb/ingest/fields/exceptions.py,sha256=J0nqFK89OhckJ0GMPrT2vVAdIHpYwDK3UoYQXOHuA_M,1205
@@ -115,41 +115,42 @@
 nucliadb/ingest/orm/entities.py,sha256=q027LfocE-KIqRNC1ZOSrrvt6x9NGrB25TZsOe0SyVk,15758
 nucliadb/ingest/orm/exceptions.py,sha256=GKr20V5xLv-WHBBHhr8lBChpW5oa9k18Xuiw-dIF9DM,1279
 nucliadb/ingest/orm/knowledgebox.py,sha256=urKMAL8Rj0Unen5AZ4Au-Z-176Vk1mOiXTUF4PnqMMs,17167
 nucliadb/ingest/orm/metrics.py,sha256=OkwMSPKLZcKba0ZTwtTiIxwBgaLMX5ydhGieKvi2y7E,1096
 nucliadb/ingest/orm/resource.py,sha256=gmmVw8tkAcH8oYQdfuxSrRhD8KZ4mh0oPs3SML2RGtY,60444
 nucliadb/ingest/orm/synonyms.py,sha256=tyOEGPfuJwhM5iYm4uNPjc2E8oWPk70DzZeuxVZ5alQ,1739
 nucliadb/ingest/orm/utils.py,sha256=0GwmyP0CqskAUqKbp0LAInYE64kt8locVqZ0HB04zlw,3683
-nucliadb/ingest/orm/processor/__init__.py,sha256=5B2o6MFFX3vRpLOxk2X6xWMpKZYKzudJc04Xf5D4DVI,26420
+nucliadb/ingest/orm/processor/__init__.py,sha256=sVQkEd-TGjTUMHGXJS3IIEtydLD-jSOoAYQK05pO_rA,27042
+nucliadb/ingest/orm/processor/auditing.py,sha256=M8YLnqEJMCvjYATqIRQS2KpJyhyxxoZvBfpxxppKGOI,5090
 nucliadb/ingest/orm/processor/sequence_manager.py,sha256=Mc9SA_NfzxTwovD5yGiAcdmen4pa-QNdsYcONIWeZPc,1690
 nucliadb/ingest/service/__init__.py,sha256=C_lkkjoHm0hDT2fZjEN4mpwXtU4bWthB-vM5-28-MBM,2057
 nucliadb/ingest/service/exceptions.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/ingest/service/writer.py,sha256=WCdV-EK4WBEbNS7RPGkj0Kp0txW7MEVRc2lSyKUg7Ls,33193
 nucliadb/ingest/tests/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/ingest/tests/conftest.py,sha256=yTepuxodMXl5vEMTzFfgos9wdRnYfxPffZQDYm3Ej-E,1157
 nucliadb/ingest/tests/fixtures.py,sha256=L4HeWexZwgpzPl872er2sAisfrW0OdmgOvx7SzCDrWM,24060
 nucliadb/ingest/tests/vectors.py,sha256=CcNKx-E8LPpyvRyljbmb-Tn_wST9Juw2CBoogWrKiTk,62843
 nucliadb/ingest/tests/integration/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/ingest/tests/integration/consumer/__init__.py,sha256=itSI7dtTwFP55YMX4iK7JzdMHS5CQVUiB1XzQu4UBh8,833
-nucliadb/ingest/tests/integration/consumer/test_auditing.py,sha256=5VYFGUeaxd18mLtUfHCUPu9c1iAShNHNM5X_CSkIFSs,2549
+nucliadb/ingest/tests/integration/consumer/test_auditing.py,sha256=kUUrdaR-iDFjmkip025rpYP5v6x3MIXLWd_n_c8-DXY,2500
 nucliadb/ingest/tests/integration/consumer/test_materializer.py,sha256=6GbV8Dsy3w9XNfNCVPBkgv6HphtuIx_2dyswla-9s5o,2591
 nucliadb/ingest/tests/integration/consumer/test_pull.py,sha256=9teutVGwcirjXEFfIw0zKD8dbTR-Zwqr-ZH01OpnmwY,4470
 nucliadb/ingest/tests/integration/consumer/test_service.py,sha256=4xl19y1ad9TddI0cIJgFKGkfgz7Vht9nFZn1t22eUNc,2763
 nucliadb/ingest/tests/integration/consumer/test_shard_creator.py,sha256=t7mJNsPadYmkTYrdHrEEBAXpnYTaX0c88zKhTMG4vrQ,2019
 nucliadb/ingest/tests/integration/ingest/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
-nucliadb/ingest/tests/integration/ingest/test_ingest.py,sha256=gc9tNtp2Ewse8LIvHcSohbULCvtEph1LcjdahIFsDTk,27336
+nucliadb/ingest/tests/integration/ingest/test_ingest.py,sha256=r7edCQtLneU1a1k90mJ_43RIRONTwCUwv_zrMB5Kgm8,27247
 nucliadb/ingest/tests/integration/ingest/test_processing_engine.py,sha256=mOfmX-3pIRWeQ17PGCSb_p_yESu-I3iBA_odvMyZIPM,3040
 nucliadb/ingest/tests/integration/ingest/test_relations.py,sha256=iSaoGe1oZu9RUx07IpuOwbrl4UrqkUM-bNp1uWP8GY0,8586
 nucliadb/ingest/tests/unit/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/ingest/tests/unit/test_cache.py,sha256=jAn5C9_wu8TGlEu-HXvvXoBnURHx_oAhYEzURPN1AvA,1189
 nucliadb/ingest/tests/unit/test_partitions.py,sha256=hN8ch_aHVas58-6q6B-__D-abNHJ4I--3vDpDVz4TS8,1432
 nucliadb/ingest/tests/unit/test_processing.py,sha256=Uh2PLeFIYMKc7jnwfzHHtyLzRIJ7xR-uOJu8C7d-FAM,5807
 nucliadb/ingest/tests/unit/test_settings.py,sha256=DdCeFACJd6oMq1QP2Vfsdz604gLAielkXSSh6YruCrU,978
 nucliadb/ingest/tests/unit/consumer/__init__.py,sha256=itSI7dtTwFP55YMX4iK7JzdMHS5CQVUiB1XzQu4UBh8,833
-nucliadb/ingest/tests/unit/consumer/test_auditing.py,sha256=4LnX-LU1TlbtxNMhJA4n3lCwn5_PbSVuj1YEZ8ANiNE,4004
+nucliadb/ingest/tests/unit/consumer/test_auditing.py,sha256=bugWAL4addULELWD7fdUb4x_6bz2ptCwrJYQklufzjo,3885
 nucliadb/ingest/tests/unit/consumer/test_consumer.py,sha256=UWdQXCDoUpayaVg8IJISGYyU4xG1Di8vhS7V2agFlms,2472
 nucliadb/ingest/tests/unit/consumer/test_pull.py,sha256=j0VQLhdmJsJxqvzU25zYwKvfIJbi7vuafzeYQGQxOAY,2063
 nucliadb/ingest/tests/unit/consumer/test_shard_creator.py,sha256=PKkGJYf9k04NTWxQh3YTYvlYFmZljOik06Jx-o0nQm4,4140
 nucliadb/ingest/tests/unit/consumer/test_utils.py,sha256=sanGAv21LfsnmqqjbprnAY22n-MSvm-n34bzj0Hj4h0,1934
 nucliadb/ingest/tests/unit/orm/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/ingest/tests/unit/orm/test_brain.py,sha256=MSSG0OdWaYeYhBpvKlqGHGdTiV5xLaXwniFdqC9OWDc,9876
 nucliadb/ingest/tests/unit/orm/test_brain_vectors.py,sha256=HNi332BgnFQ_wx5Mw3AYv9mhSsRmj9F04VNZb6Nu3lE,2435
@@ -184,15 +185,15 @@
 nucliadb/reader/api/v1/knowledgebox.py,sha256=Pd71iqTVRgx5u_Gb2LegDTQ3gGTKbVLsAvgcZne5_lM,3641
 nucliadb/reader/api/v1/learning_collector.py,sha256=6XDrfEZffqPrFYGj9TDfWOS1wcy3n9DRu35aH6-2WRA,2099
 nucliadb/reader/api/v1/learning_config.py,sha256=T1bxwsNDnVaeW9lkO4WTO9RHjz6GhYCJwvS1_MNYTes,4472
 nucliadb/reader/api/v1/resource.py,sha256=GkCjExN6wUyIKKgZ9FliDFcPj_VGMhw9KJobYWZf5N8,13951
 nucliadb/reader/api/v1/router.py,sha256=eyNmEGSP9zHkCIG5XlAXl6sukq950B7gFT3X2peMtIE,1011
 nucliadb/reader/api/v1/services.py,sha256=PssrduMSIbZuSxPBYMIvjpQpzCWZ-lzFkdjlAGQHYwE,12399
 nucliadb/reader/reader/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
-nucliadb/reader/reader/notifications.py,sha256=cPpcnyHr9prcsGvkq4JwZqHjbTEkpXVcPWoYA4Up5fU,8155
+nucliadb/reader/reader/notifications.py,sha256=2In2E-2FUawjqNWKaxqrw_rB2hTzgAXVV5yFhF4gHOA,7988
 nucliadb/reader/tests/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/reader/tests/conftest.py,sha256=RH5huJVfSZ9cQgzEWC_xViGbXUelZFuHmrOnWb-FpEU,1224
 nucliadb/reader/tests/fixtures.py,sha256=pVrolKyIQaUA01Coe8WHG6OuliqREnzq8DJnnfPF8_k,4345
 nucliadb/reader/tests/test_list_resources.py,sha256=yKsG6MLh4_cB7Yhov0OoBAVCJCXnpuQmT453R1oVQ6Q,2748
 nucliadb/reader/tests/test_reader_file_download.py,sha256=V_wLTRmSlYemSPLOBo3A_jhMBluro2sJiQwSsGGBx6I,10199
 nucliadb/reader/tests/test_reader_resource.py,sha256=A7XzHngspJxPqxzyMZ2Zg2Kp8SuDTi78Fo2rG1roLyo,10586
 nucliadb/reader/tests/test_reader_resource_field.py,sha256=YQ-U2mEGhs_rPGxcWPZmWLSEoCxBo3AVDtLZCtZrGb8,6535
@@ -448,13 +449,13 @@
 nucliadb/writer/tus/exceptions.py,sha256=CmxYKnHXpXug25DYV4SpVAU47SGD-NVBd7pNTRbWHyk,2186
 nucliadb/writer/tus/gcs.py,sha256=WykJZicWKRYkVB5_Fkb_1cVLovAk86IVkEn1VgEDufc,14527
 nucliadb/writer/tus/local.py,sha256=lIOoGaylnsxPBYGskcmKSHv7MsvwIYFS4soDLey_KSs,5849
 nucliadb/writer/tus/pg.py,sha256=JUK_xKsyNcKAvWOch8gUMTc_e1evI_3aC6-Y5gMk2jw,4367
 nucliadb/writer/tus/s3.py,sha256=a9mfPtjBW3QaTYY2r6P7u_Y13V6mBefZjWgV4juZzgE,9069
 nucliadb/writer/tus/storage.py,sha256=8iBOjWIcY6PawQq_rmSiBKi0Gl6J6Q5ad6L-9nLCcJ4,4734
 nucliadb/writer/tus/utils.py,sha256=MSdVbRsRSZVdkaum69_0wku7X3p5wlZf4nr6E0GMKbw,2556
-nucliadb-4.0.0.post520.dist-info/METADATA,sha256=-7Z930e73q_JBCMVlRuO4Jm7Xai32Y_jvTHvJ-yf5R0,4423
-nucliadb-4.0.0.post520.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-nucliadb-4.0.0.post520.dist-info/entry_points.txt,sha256=XqGfgFDuY3zXQc8ewXM2TRVjTModIq851zOsgrmaXx4,1268
-nucliadb-4.0.0.post520.dist-info/top_level.txt,sha256=hwYhTVnX7jkQ9gJCkVrbqEG1M4lT2F_iPQND1fCzF80,20
-nucliadb-4.0.0.post520.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-nucliadb-4.0.0.post520.dist-info/RECORD,,
+nucliadb-4.0.0.post522.dist-info/METADATA,sha256=Xk7PMUpHMHdRsJhxvWDQMHRbfkJleSAFE4thVqID1YU,4423
+nucliadb-4.0.0.post522.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+nucliadb-4.0.0.post522.dist-info/entry_points.txt,sha256=XqGfgFDuY3zXQc8ewXM2TRVjTModIq851zOsgrmaXx4,1268
+nucliadb-4.0.0.post522.dist-info/top_level.txt,sha256=hwYhTVnX7jkQ9gJCkVrbqEG1M4lT2F_iPQND1fCzF80,20
+nucliadb-4.0.0.post522.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+nucliadb-4.0.0.post522.dist-info/RECORD,,
```

