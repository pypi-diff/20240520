# Comparing `tmp/pydpu-0.2.0.tar.gz` & `tmp/pydpu-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydpu-0.2.0.tar", max compression
+gzip compressed data, was "pydpu-0.2.1.tar", max compression
```

## Comparing `pydpu-0.2.0.tar` & `pydpu-0.2.1.tar`

### file list

```diff
@@ -1,94 +1,94 @@
--rw-r--r--   0        0        0    11357 2024-05-17 13:56:00.625090 pydpu-0.2.0/LICENSE
--rw-r--r--   0        0        0     4428 2024-05-17 13:56:00.625090 pydpu-0.2.0/README.md
--rw-r--r--   0        0        0      113 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/__init__.py
--rw-r--r--   0        0        0       70 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/__main__.py
--rw-r--r--   0        0        0     6018 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/cli.py
--rw-r--r--   0        0        0        0 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/dpuredfish/__init__.py
--rw-r--r--   0        0        0     1236 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/dpuredfish/accounts.py
--rw-r--r--   0        0        0     1261 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/dpuredfish/certificates.py
--rw-r--r--   0        0        0     4733 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/dpuredfish/managers.py
--rw-r--r--   0        0        0     3246 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/dpuredfish/systems.py
--rw-r--r--   0        0        0     1771 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/dpuredfish/update.py
--rw-r--r--   0        0        0     1615 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/evpn.py
--rw-r--r--   0        0        0      475 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/inventory.py
--rw-r--r--   0        0        0     1060 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/ipsec.py
--rw-r--r--   0        0        0        0 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/proto/__init__.py
--rw-r--r--   0        0        0      237 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/proto/v1/__init__.py
--rw-r--r--   0        0        0    10979 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/proto/v1/backend_aio_pb2.py
--rw-r--r--   0        0        0    10677 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/proto/v1/backend_aio_pb2_grpc.py
--rw-r--r--   0        0        0     1203 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/proto/v1/backend_iscsi_pb2.py
--rw-r--r--   0        0        0      159 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/proto/v1/backend_iscsi_pb2_grpc.py
--rw-r--r--   0        0        0    11443 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/proto/v1/backend_malloc_pb2.py
--rw-r--r--   0        0        0    11053 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/proto/v1/backend_malloc_pb2_grpc.py
--rw-r--r--   0        0        0    10920 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/proto/v1/backend_null_pb2.py
--rw-r--r--   0        0        0    10795 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/proto/v1/backend_null_pb2_grpc.py
--rw-r--r--   0        0        0    31330 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/proto/v1/backend_nvme_pb2.py
--rw-r--r--   0        0        0    26793 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/proto/v1/backend_nvme_pb2_grpc.py
--rw-r--r--   0        0        0    21683 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/proto/v1/bgp_pb2.py
--rw-r--r--   0        0        0      159 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/proto/v1/bgp_pb2_grpc.py
--rw-r--r--   0        0        0   115486 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/proto/v1/cloudrpc_pb2.py
--rw-r--r--   0        0        0   160377 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/proto/v1/cloudrpc_pb2_grpc.py
--rw-r--r--   0        0        0     2476 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/proto/v1/component_pb2.py
--rw-r--r--   0        0        0      159 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/proto/v1/component_pb2_grpc.py
--rw-r--r--   0        0        0     6088 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/proto/v1/device_pb2.py
--rw-r--r--   0        0        0      159 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/proto/v1/device_pb2_grpc.py
--rw-r--r--   0        0        0    39939 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/proto/v1/frontend_nvme_pb2.py
--rw-r--r--   0        0        0    31407 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/proto/v1/frontend_nvme_pb2_grpc.py
--rw-r--r--   0        0        0    11460 2024-05-17 13:56:00.625090 pydpu-0.2.0/pydpu/proto/v1/frontend_virtio_blk_pb2.py
--rw-r--r--   0        0        0    11241 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/frontend_virtio_blk_pb2_grpc.py
--rw-r--r--   0        0        0     1214 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/frontend_virtio_fs_pb2.py
--rw-r--r--   0        0        0      159 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/frontend_virtio_fs_pb2_grpc.py
--rw-r--r--   0        0        0    32429 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/frontend_virtio_scsi_pb2.py
--rw-r--r--   0        0        0    33020 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/frontend_virtio_scsi_pb2_grpc.py
--rw-r--r--   0        0        0     7161 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/interface_pb2.py
--rw-r--r--   0        0        0      159 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/interface_pb2_grpc.py
--rw-r--r--   0        0        0     5931 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/inventory_pb2.py
--rw-r--r--   0        0        0     2513 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/inventory_pb2_grpc.py
--rw-r--r--   0        0        0    25046 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/ipsec_pb2.py
--rw-r--r--   0        0        0    16579 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/ipsec_pb2_grpc.py
--rw-r--r--   0        0        0     1173 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/k8s_pb2.py
--rw-r--r--   0        0        0      159 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/k8s_pb2_grpc.py
--rw-r--r--   0        0        0    22564 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/l2_xpu_infra_mgr_pb2.py
--rw-r--r--   0        0        0    18666 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/l2_xpu_infra_mgr_pb2_grpc.py
--rw-r--r--   0        0        0    20461 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/l3_xpu_infra_mgr_pb2.py
--rw-r--r--   0        0        0    17364 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/l3_xpu_infra_mgr_pb2_grpc.py
--rw-r--r--   0        0        0     5526 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/mapping_pb2.py
--rw-r--r--   0        0        0      159 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/mapping_pb2_grpc.py
--rw-r--r--   0        0        0    12210 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/middleend_encryption_pb2.py
--rw-r--r--   0        0        0    11693 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/middleend_encryption_pb2_grpc.py
--rw-r--r--   0        0        0    11668 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/middleend_qos_volume_pb2.py
--rw-r--r--   0        0        0    11224 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/middleend_qos_volume_pb2_grpc.py
--rw-r--r--   0        0        0     9053 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/networkethernet_pb2.py
--rw-r--r--   0        0        0      159 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/networkethernet_pb2_grpc.py
--rw-r--r--   0        0        0    25191 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/networkinterfaces_pb2.py
--rw-r--r--   0        0        0     6223 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/networkinterfaces_pb2_grpc.py
--rw-r--r--   0        0        0    12778 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/networkpolicy_pb2.py
--rw-r--r--   0        0        0      159 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/networkpolicy_pb2_grpc.py
--rw-r--r--   0        0        0    10272 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/networktypes_pb2.py
--rw-r--r--   0        0        0      159 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/networktypes_pb2_grpc.py
--rw-r--r--   0        0        0     6922 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/networkvlan_pb2.py
--rw-r--r--   0        0        0      159 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/networkvlan_pb2_grpc.py
--rw-r--r--   0        0        0     6830 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/nexthop_pb2.py
--rw-r--r--   0        0        0      159 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/nexthop_pb2_grpc.py
--rw-r--r--   0        0        0     8855 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/opicommon_pb2.py
--rw-r--r--   0        0        0      159 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/opicommon_pb2_grpc.py
--rw-r--r--   0        0        0    11334 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/port_pb2.py
--rw-r--r--   0        0        0      159 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/port_pb2_grpc.py
--rw-r--r--   0        0        0     6551 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/route_pb2.py
--rw-r--r--   0        0        0      159 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/route_pb2_grpc.py
--rw-r--r--   0        0        0     3971 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/subnet_pb2.py
--rw-r--r--   0        0        0      159 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/subnet_pb2_grpc.py
--rw-r--r--   0        0        0     1191 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/telco_pb2.py
--rw-r--r--   0        0        0      159 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/telco_pb2_grpc.py
--rw-r--r--   0        0        0     3745 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/tunnel_pb2.py
--rw-r--r--   0        0        0      159 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/tunnel_pb2_grpc.py
--rw-r--r--   0        0        0     4397 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/underlayroute_pb2.py
--rw-r--r--   0        0        0      159 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/underlayroute_pb2_grpc.py
--rw-r--r--   0        0        0     4668 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/vnic_pb2.py
--rw-r--r--   0        0        0      159 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/vnic_pb2_grpc.py
--rw-r--r--   0        0        0     4440 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/vpc_pb2.py
--rw-r--r--   0        0        0      159 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/proto/v1/vpc_pb2_grpc.py
--rw-r--r--   0        0        0    21661 2024-05-17 13:56:00.629090 pydpu-0.2.0/pydpu/storage.py
--rw-r--r--   0        0        0      868 2024-05-17 13:56:00.629090 pydpu-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     5483 1970-01-01 00:00:00.000000 pydpu-0.2.0/setup.py
--rw-r--r--   0        0        0     5159 1970-01-01 00:00:00.000000 pydpu-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-20 15:37:33.887033 pydpu-0.2.1/LICENSE
+-rw-r--r--   0        0        0     4428 2024-05-20 15:37:33.887033 pydpu-0.2.1/README.md
+-rw-r--r--   0        0        0      112 2024-05-20 15:37:33.887033 pydpu-0.2.1/pydpu/__init__.py
+-rw-r--r--   0        0        0       70 2024-05-20 15:37:33.887033 pydpu-0.2.1/pydpu/__main__.py
+-rw-r--r--   0        0        0     6018 2024-05-20 15:37:33.887033 pydpu-0.2.1/pydpu/cli.py
+-rw-r--r--   0        0        0        0 2024-05-20 15:37:33.887033 pydpu-0.2.1/pydpu/dpuredfish/__init__.py
+-rw-r--r--   0        0        0     1236 2024-05-20 15:37:33.887033 pydpu-0.2.1/pydpu/dpuredfish/accounts.py
+-rw-r--r--   0        0        0     1261 2024-05-20 15:37:33.887033 pydpu-0.2.1/pydpu/dpuredfish/certificates.py
+-rw-r--r--   0        0        0     4733 2024-05-20 15:37:33.887033 pydpu-0.2.1/pydpu/dpuredfish/managers.py
+-rw-r--r--   0        0        0     3246 2024-05-20 15:37:33.887033 pydpu-0.2.1/pydpu/dpuredfish/systems.py
+-rw-r--r--   0        0        0     1771 2024-05-20 15:37:33.887033 pydpu-0.2.1/pydpu/dpuredfish/update.py
+-rw-r--r--   0        0        0     1615 2024-05-20 15:37:33.887033 pydpu-0.2.1/pydpu/evpn.py
+-rw-r--r--   0        0        0      475 2024-05-20 15:37:33.887033 pydpu-0.2.1/pydpu/inventory.py
+-rw-r--r--   0        0        0     1060 2024-05-20 15:37:33.887033 pydpu-0.2.1/pydpu/ipsec.py
+-rw-r--r--   0        0        0        0 2024-05-20 15:37:33.887033 pydpu-0.2.1/pydpu/proto/__init__.py
+-rw-r--r--   0        0        0      237 2024-05-20 15:37:33.887033 pydpu-0.2.1/pydpu/proto/v1/__init__.py
+-rw-r--r--   0        0        0    10979 2024-05-20 15:37:33.887033 pydpu-0.2.1/pydpu/proto/v1/backend_aio_pb2.py
+-rw-r--r--   0        0        0    10677 2024-05-20 15:37:33.887033 pydpu-0.2.1/pydpu/proto/v1/backend_aio_pb2_grpc.py
+-rw-r--r--   0        0        0     1203 2024-05-20 15:37:33.887033 pydpu-0.2.1/pydpu/proto/v1/backend_iscsi_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-20 15:37:33.887033 pydpu-0.2.1/pydpu/proto/v1/backend_iscsi_pb2_grpc.py
+-rw-r--r--   0        0        0    11443 2024-05-20 15:37:33.887033 pydpu-0.2.1/pydpu/proto/v1/backend_malloc_pb2.py
+-rw-r--r--   0        0        0    11053 2024-05-20 15:37:33.887033 pydpu-0.2.1/pydpu/proto/v1/backend_malloc_pb2_grpc.py
+-rw-r--r--   0        0        0    10920 2024-05-20 15:37:33.887033 pydpu-0.2.1/pydpu/proto/v1/backend_null_pb2.py
+-rw-r--r--   0        0        0    10795 2024-05-20 15:37:33.887033 pydpu-0.2.1/pydpu/proto/v1/backend_null_pb2_grpc.py
+-rw-r--r--   0        0        0    31330 2024-05-20 15:37:33.887033 pydpu-0.2.1/pydpu/proto/v1/backend_nvme_pb2.py
+-rw-r--r--   0        0        0    26793 2024-05-20 15:37:33.887033 pydpu-0.2.1/pydpu/proto/v1/backend_nvme_pb2_grpc.py
+-rw-r--r--   0        0        0    21683 2024-05-20 15:37:33.887033 pydpu-0.2.1/pydpu/proto/v1/bgp_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-20 15:37:33.887033 pydpu-0.2.1/pydpu/proto/v1/bgp_pb2_grpc.py
+-rw-r--r--   0        0        0   115486 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/cloudrpc_pb2.py
+-rw-r--r--   0        0        0   160377 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/cloudrpc_pb2_grpc.py
+-rw-r--r--   0        0        0     2476 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/component_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/component_pb2_grpc.py
+-rw-r--r--   0        0        0     6088 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/device_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/device_pb2_grpc.py
+-rw-r--r--   0        0        0    39939 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/frontend_nvme_pb2.py
+-rw-r--r--   0        0        0    31407 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/frontend_nvme_pb2_grpc.py
+-rw-r--r--   0        0        0    11460 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/frontend_virtio_blk_pb2.py
+-rw-r--r--   0        0        0    11241 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/frontend_virtio_blk_pb2_grpc.py
+-rw-r--r--   0        0        0     1214 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/frontend_virtio_fs_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/frontend_virtio_fs_pb2_grpc.py
+-rw-r--r--   0        0        0    32429 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/frontend_virtio_scsi_pb2.py
+-rw-r--r--   0        0        0    33020 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/frontend_virtio_scsi_pb2_grpc.py
+-rw-r--r--   0        0        0     7161 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/interface_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/interface_pb2_grpc.py
+-rw-r--r--   0        0        0     5931 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/inventory_pb2.py
+-rw-r--r--   0        0        0     2513 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/inventory_pb2_grpc.py
+-rw-r--r--   0        0        0    25046 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/ipsec_pb2.py
+-rw-r--r--   0        0        0    16579 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/ipsec_pb2_grpc.py
+-rw-r--r--   0        0        0     1173 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/k8s_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/k8s_pb2_grpc.py
+-rw-r--r--   0        0        0    22564 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/l2_xpu_infra_mgr_pb2.py
+-rw-r--r--   0        0        0    18666 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/l2_xpu_infra_mgr_pb2_grpc.py
+-rw-r--r--   0        0        0    20461 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/l3_xpu_infra_mgr_pb2.py
+-rw-r--r--   0        0        0    17364 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/l3_xpu_infra_mgr_pb2_grpc.py
+-rw-r--r--   0        0        0     5526 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/mapping_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/mapping_pb2_grpc.py
+-rw-r--r--   0        0        0    12210 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/middleend_encryption_pb2.py
+-rw-r--r--   0        0        0    11693 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/middleend_encryption_pb2_grpc.py
+-rw-r--r--   0        0        0    11668 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/middleend_qos_volume_pb2.py
+-rw-r--r--   0        0        0    11224 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/middleend_qos_volume_pb2_grpc.py
+-rw-r--r--   0        0        0     9053 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/networkethernet_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/networkethernet_pb2_grpc.py
+-rw-r--r--   0        0        0    25191 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/networkinterfaces_pb2.py
+-rw-r--r--   0        0        0     6223 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/networkinterfaces_pb2_grpc.py
+-rw-r--r--   0        0        0    12778 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/networkpolicy_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/networkpolicy_pb2_grpc.py
+-rw-r--r--   0        0        0    10272 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/networktypes_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/networktypes_pb2_grpc.py
+-rw-r--r--   0        0        0     6922 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/networkvlan_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/networkvlan_pb2_grpc.py
+-rw-r--r--   0        0        0     6830 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/nexthop_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/nexthop_pb2_grpc.py
+-rw-r--r--   0        0        0     8855 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/opicommon_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/opicommon_pb2_grpc.py
+-rw-r--r--   0        0        0    11334 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/port_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/port_pb2_grpc.py
+-rw-r--r--   0        0        0     6551 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/route_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/route_pb2_grpc.py
+-rw-r--r--   0        0        0     3971 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/subnet_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/subnet_pb2_grpc.py
+-rw-r--r--   0        0        0     1191 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/telco_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/telco_pb2_grpc.py
+-rw-r--r--   0        0        0     3745 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/tunnel_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/tunnel_pb2_grpc.py
+-rw-r--r--   0        0        0     4397 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/underlayroute_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/underlayroute_pb2_grpc.py
+-rw-r--r--   0        0        0     4668 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/vnic_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/vnic_pb2_grpc.py
+-rw-r--r--   0        0        0     4440 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/vpc_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-20 15:37:33.891033 pydpu-0.2.1/pydpu/proto/v1/vpc_pb2_grpc.py
+-rw-r--r--   0        0        0    21661 2024-05-20 15:37:33.895033 pydpu-0.2.1/pydpu/storage.py
+-rw-r--r--   0        0        0      868 2024-05-20 15:37:33.895033 pydpu-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5483 1970-01-01 00:00:00.000000 pydpu-0.2.1/setup.py
+-rw-r--r--   0        0        0     5159 1970-01-01 00:00:00.000000 pydpu-0.2.1/PKG-INFO
```

### Comparing `pydpu-0.2.0/LICENSE` & `pydpu-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/README.md` & `pydpu-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/cli.py` & `pydpu-0.2.1/pydpu/cli.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/dpuredfish/accounts.py` & `pydpu-0.2.1/pydpu/dpuredfish/accounts.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/dpuredfish/certificates.py` & `pydpu-0.2.1/pydpu/dpuredfish/certificates.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/dpuredfish/managers.py` & `pydpu-0.2.1/pydpu/dpuredfish/managers.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/dpuredfish/systems.py` & `pydpu-0.2.1/pydpu/dpuredfish/systems.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/dpuredfish/update.py` & `pydpu-0.2.1/pydpu/dpuredfish/update.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/evpn.py` & `pydpu-0.2.1/pydpu/evpn.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/ipsec.py` & `pydpu-0.2.1/pydpu/ipsec.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/proto/v1/backend_aio_pb2.py` & `pydpu-0.2.1/pydpu/proto/v1/backend_aio_pb2.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/proto/v1/backend_aio_pb2_grpc.py` & `pydpu-0.2.1/pydpu/proto/v1/backend_aio_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/proto/v1/backend_iscsi_pb2.py` & `pydpu-0.2.1/pydpu/proto/v1/backend_iscsi_pb2.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/proto/v1/backend_malloc_pb2.py` & `pydpu-0.2.1/pydpu/proto/v1/backend_malloc_pb2.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/proto/v1/backend_malloc_pb2_grpc.py` & `pydpu-0.2.1/pydpu/proto/v1/backend_malloc_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/proto/v1/backend_null_pb2.py` & `pydpu-0.2.1/pydpu/proto/v1/backend_null_pb2.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/proto/v1/backend_null_pb2_grpc.py` & `pydpu-0.2.1/pydpu/proto/v1/backend_null_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/proto/v1/backend_nvme_pb2.py` & `pydpu-0.2.1/pydpu/proto/v1/backend_nvme_pb2.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/proto/v1/backend_nvme_pb2_grpc.py` & `pydpu-0.2.1/pydpu/proto/v1/backend_nvme_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/proto/v1/bgp_pb2.py` & `pydpu-0.2.1/pydpu/proto/v1/bgp_pb2.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/proto/v1/cloudrpc_pb2.py` & `pydpu-0.2.1/pydpu/proto/v1/cloudrpc_pb2.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/proto/v1/cloudrpc_pb2_grpc.py` & `pydpu-0.2.1/pydpu/proto/v1/cloudrpc_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/proto/v1/component_pb2.py` & `pydpu-0.2.1/pydpu/proto/v1/component_pb2.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/proto/v1/device_pb2.py` & `pydpu-0.2.1/pydpu/proto/v1/device_pb2.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/proto/v1/frontend_nvme_pb2.py` & `pydpu-0.2.1/pydpu/proto/v1/frontend_nvme_pb2.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/proto/v1/frontend_nvme_pb2_grpc.py` & `pydpu-0.2.1/pydpu/proto/v1/frontend_nvme_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/proto/v1/frontend_virtio_blk_pb2.py` & `pydpu-0.2.1/pydpu/proto/v1/frontend_virtio_blk_pb2.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/proto/v1/frontend_virtio_blk_pb2_grpc.py` & `pydpu-0.2.1/pydpu/proto/v1/frontend_virtio_blk_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/proto/v1/frontend_virtio_fs_pb2.py` & `pydpu-0.2.1/pydpu/proto/v1/frontend_virtio_fs_pb2.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/proto/v1/frontend_virtio_scsi_pb2.py` & `pydpu-0.2.1/pydpu/proto/v1/frontend_virtio_scsi_pb2.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/proto/v1/frontend_virtio_scsi_pb2_grpc.py` & `pydpu-0.2.1/pydpu/proto/v1/frontend_virtio_scsi_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/proto/v1/interface_pb2.py` & `pydpu-0.2.1/pydpu/proto/v1/interface_pb2.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/proto/v1/inventory_pb2.py` & `pydpu-0.2.1/pydpu/proto/v1/inventory_pb2.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/proto/v1/inventory_pb2_grpc.py` & `pydpu-0.2.1/pydpu/proto/v1/inventory_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/proto/v1/ipsec_pb2.py` & `pydpu-0.2.1/pydpu/proto/v1/ipsec_pb2.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/proto/v1/ipsec_pb2_grpc.py` & `pydpu-0.2.1/pydpu/proto/v1/ipsec_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/proto/v1/k8s_pb2.py` & `pydpu-0.2.1/pydpu/proto/v1/k8s_pb2.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/proto/v1/l2_xpu_infra_mgr_pb2.py` & `pydpu-0.2.1/pydpu/proto/v1/l2_xpu_infra_mgr_pb2.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/proto/v1/l2_xpu_infra_mgr_pb2_grpc.py` & `pydpu-0.2.1/pydpu/proto/v1/l2_xpu_infra_mgr_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/proto/v1/l3_xpu_infra_mgr_pb2.py` & `pydpu-0.2.1/pydpu/proto/v1/l3_xpu_infra_mgr_pb2.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/proto/v1/l3_xpu_infra_mgr_pb2_grpc.py` & `pydpu-0.2.1/pydpu/proto/v1/l3_xpu_infra_mgr_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/proto/v1/mapping_pb2.py` & `pydpu-0.2.1/pydpu/proto/v1/mapping_pb2.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/proto/v1/middleend_encryption_pb2.py` & `pydpu-0.2.1/pydpu/proto/v1/middleend_encryption_pb2.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/proto/v1/middleend_encryption_pb2_grpc.py` & `pydpu-0.2.1/pydpu/proto/v1/middleend_encryption_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/proto/v1/middleend_qos_volume_pb2.py` & `pydpu-0.2.1/pydpu/proto/v1/middleend_qos_volume_pb2.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/proto/v1/middleend_qos_volume_pb2_grpc.py` & `pydpu-0.2.1/pydpu/proto/v1/middleend_qos_volume_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/proto/v1/networkethernet_pb2.py` & `pydpu-0.2.1/pydpu/proto/v1/networkethernet_pb2.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/proto/v1/networkinterfaces_pb2.py` & `pydpu-0.2.1/pydpu/proto/v1/networkinterfaces_pb2.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/proto/v1/networkinterfaces_pb2_grpc.py` & `pydpu-0.2.1/pydpu/proto/v1/networkinterfaces_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/proto/v1/networkpolicy_pb2.py` & `pydpu-0.2.1/pydpu/proto/v1/networkpolicy_pb2.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/proto/v1/networktypes_pb2.py` & `pydpu-0.2.1/pydpu/proto/v1/networktypes_pb2.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/proto/v1/networkvlan_pb2.py` & `pydpu-0.2.1/pydpu/proto/v1/networkvlan_pb2.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/proto/v1/nexthop_pb2.py` & `pydpu-0.2.1/pydpu/proto/v1/nexthop_pb2.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/proto/v1/opicommon_pb2.py` & `pydpu-0.2.1/pydpu/proto/v1/opicommon_pb2.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/proto/v1/port_pb2.py` & `pydpu-0.2.1/pydpu/proto/v1/port_pb2.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/proto/v1/route_pb2.py` & `pydpu-0.2.1/pydpu/proto/v1/route_pb2.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/proto/v1/subnet_pb2.py` & `pydpu-0.2.1/pydpu/proto/v1/subnet_pb2.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/proto/v1/telco_pb2.py` & `pydpu-0.2.1/pydpu/proto/v1/telco_pb2.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/proto/v1/tunnel_pb2.py` & `pydpu-0.2.1/pydpu/proto/v1/tunnel_pb2.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/proto/v1/underlayroute_pb2.py` & `pydpu-0.2.1/pydpu/proto/v1/underlayroute_pb2.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/proto/v1/vnic_pb2.py` & `pydpu-0.2.1/pydpu/proto/v1/vnic_pb2.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/proto/v1/vpc_pb2.py` & `pydpu-0.2.1/pydpu/proto/v1/vpc_pb2.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pydpu/storage.py` & `pydpu-0.2.1/pydpu/storage.py`

 * *Files identical despite different names*

### Comparing `pydpu-0.2.0/pyproject.toml` & `pydpu-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydpu"
-version = "0.2.0"
+version = "0.2.1"
 description = "Python library and cli to communicate with DPUs and IPUs"
 authors = ["OPI Dev <opi-dev@lists.opiproject.org>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.scripts]
 dpu = "pydpu.cli:main"
```

### Comparing `pydpu-0.2.0/setup.py` & `pydpu-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'redfish>=3.2.1,<4.0.0']
 
 entry_points = \
 {'console_scripts': ['dpu = pydpu.cli:main']}
 
 setup_kwargs = {
     'name': 'pydpu',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': 'Python library and cli to communicate with DPUs and IPUs',
     'long_description': '# pydpu\n\n[![License](https://img.shields.io/github/license/opiproject/pydpu?style=flat&color=blue&label=License)](https://github.com/opiproject/pydpu/blob/main/LICENSE)\n[![Pulls](https://img.shields.io/docker/pulls/opiproject/pydpu.svg?logo=docker&style=flat&label=Pulls)](https://hub.docker.com/r/opiproject/pydpu)\n[![PyPI](https://img.shields.io/pypi/v/pydpu)](https://pypi.org/project/pydpu/)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat)](https://github.com/psf/black)\n[![codecov](https://codecov.io/gh/opiproject/pydpu/branch/main/graph/badge.svg)](https://codecov.io/gh/opiproject/pydpu)\n[![Linters](https://github.com/opiproject/pydpu/actions/workflows/linters.yml/badge.svg)](https://github.com/opiproject/pydpu/actions/workflows/linters.yml)\n[![CodeQL](https://github.com/opiproject/pydpu/actions/workflows/codeql.yml/badge.svg)](https://github.com/opiproject/pydpu/actions/workflows/codeql.yml)\n[![OpenSSF Scorecard](https://api.securityscorecards.dev/projects/github.com/opiproject/pydpu/badge)](https://securityscorecards.dev/viewer/?platform=github.com&org=opiproject&repo=pydpu)\n[![Docker](https://github.com/opiproject/pydpu/actions/workflows/docker.yaml/badge.svg)](https://github.com/opiproject/pydpu/actions/workflows/docker.yaml)\n[![Tests](https://github.com/opiproject/pydpu/actions/workflows/python.yaml/badge.svg)](https://github.com/opiproject/pydpu/actions/workflows/python.yaml)\n[![GitHub stars](https://img.shields.io/github/stars/opiproject/pydpu.svg?style=flat-square&label=github%20stars)](https://github.com/opiproject/pydpu)\n[![GitHub Contributors](https://img.shields.io/github/contributors/opiproject/pydpu.svg?style=flat-square)](https://github.com/opiproject/pydpu/graphs/contributors)\n\nPython library and cli to communicate with DPUs and IPUs\n\n## I Want To Contribute\n\nThis project welcomes contributions and suggestions.  We are happy to have the Community involved via submission of **Issues and Pull Requests** (with substantive content or even just fixes). We are hoping for the documents, test framework, etc. to become a community process with active engagement.  PRs can be reviewed by by any number of people, and a maintainer may accept.\n\nSee [CONTRIBUTING](https://github.com/opiproject/opi/blob/main/CONTRIBUTING.md) and [GitHub Basic Process](https://github.com/opiproject/opi/blob/main/doc-github-rules.md) for more details.\n\n## Installation\n\nThere are several ways of running this CLI.\n\n### Docker\n\n```sh\ndocker pull opiproject/pydpu:<version>\n```\n\nYou can specify a version like `0.1.1` or use `latest` to get the most up-to-date version.\n\nRun latest version of the CLI in a container:\n\n```sh\ndocker run -it --rm --network=host opiproject/pydpu:latest --help\n```\n\nReplace `--help` with any `pydpu` command, without `pydpu` itself.\n\n### PyPI\n\n```sh\npip install pydpu\n```\n\n## Usage\n\n### Version\n\nTo get version, run:\n\n```sh\n$ pydpu --version\ndpu, version 0.1.1\n```\n\n### Redfish\n\nTo communicate over redfish, run:\n\n```sh\npydpu --address=10.10.10.10 redfish --username root --password 0penBmc test\n```\n\n### Inventory\n\nTo get inventory, run:\n\n```sh\npydpu --address=localhost:50151 inventory get\n```\n\n### Ipsec\n\nTo create a tunnel, run:\n\n```sh\npydpu --address=localhost:50151 ipsec create-tunnel\n```\n\nTo get statistics, run:\n\n```sh\npydpu --address=localhost:50151 ipsec stats\n```\n\n### Storage\n\nTo create a subsystem, run:\n\n```sh\npydpu --address=localhost:50151 storage subsystem\n```\n\nTo create a controller, run:\n\n```sh\npydpu --address=localhost:50151 storage controller\n```\n\nTo create a namespace, run:\n\n```sh\npydpu --address=localhost:50151 storage namespace\n```\n\n### Evpn\n\nTo create a logical bridge, run:\n\n```sh\npydpu --address=localhost:50151 evpn bridge\n```\n\nTo create a bridge port, run:\n\n```sh\npydpu --address=localhost:50151 evpn port\n```\n\nTo create a vrf, run:\n\n```sh\npydpu --address=localhost:50151 evpn vrf\n```\n\nTo create a svi, run:\n\n```sh\npydpu --address=localhost:50151 evpn svi\n```\n\n## Packaging\n\nThis project uses [poetry](https://python-poetry.org/) to manage dependencies, build, etc.\n\n## Releasing new versions\n\n```sh\n# Make sure you have dev dependencies installed\n$ poetry install --group dev\n# Use bump2version to update version strings and create a new tag\n$ bump2version <patch|minor|major>\n# Push new tag\n$ git push --tags\n# Create GitHub release\n$ gh release create v$(poetry version -s) --generate-notes\n```\n',
     'author': 'OPI Dev',
     'author_email': 'opi-dev@lists.opiproject.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pydpu-0.2.0/PKG-INFO` & `pydpu-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydpu
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python library and cli to communicate with DPUs and IPUs
 License: Apache-2.0
 Author: OPI Dev
 Author-email: opi-dev@lists.opiproject.org
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

