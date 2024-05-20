# Comparing `tmp/pulumi_kubernetes_the_hard_way-0.0.21a1716157484.tar.gz` & `tmp/pulumi_kubernetes_the_hard_way-0.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_kubernetes_the_hard_way-0.0.21a1716157484.tar", last modified: Sun May 19 22:27:23 2024, max compression
+gzip compressed data, was "pulumi_kubernetes_the_hard_way-0.0.22.tar", last modified: Mon May 20 00:22:35 2024, max compression
```

## Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484.tar` & `pulumi_kubernetes_the_hard_way-0.0.22.tar`

### file list

```diff
@@ -1,84 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:27:23.971222 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-19 22:27:23.971222 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:27:23.955223 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/
--rw-------   0 runner    (1001) docker     (127)     4606 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/__init__.py
--rw-------   0 runner    (1001) docker     (127)     9268 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:27:23.959223 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/config/
--rw-------   0 runner    (1001) docker     (127)      496 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/config/__init__.py
--rw-------   0 runner    (1001) docker     (127)      427 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/config/_enums.py
--rw-------   0 runner    (1001) docker     (127)    21648 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/config/_inputs.py
--rw-------   0 runner    (1001) docker     (127)     8791 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py
--rw-------   0 runner    (1001) docker     (127)     3426 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py
--rw-------   0 runner    (1001) docker     (127)     4826 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/config/get_kubelet_configuration.py
--rw-------   0 runner    (1001) docker     (127)    23901 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py
--rw-------   0 runner    (1001) docker     (127)    12558 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/config/kubelet_configuration.py
--rw-------   0 runner    (1001) docker     (127)    38474 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/config/outputs.py
--rw-------   0 runner    (1001) docker     (127)     2783 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/provider.py
--rw-------   0 runner    (1001) docker     (127)      116 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (127)        0 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:27:23.963223 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/
--rw-------   0 runner    (1001) docker     (127)     1147 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/__init__.py
--rw-------   0 runner    (1001) docker     (127)     1095 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/_enums.py
--rw-------   0 runner    (1001) docker     (127)    29297 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    13340 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/cni_bridge_plugin_configuration.py
--rw-------   0 runner    (1001) docker     (127)     8612 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/cni_loopback_plugin_configuration.py
--rw-------   0 runner    (1001) docker     (127)     7575 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/cni_plugin_configuration.py
--rw-------   0 runner    (1001) docker     (127)    19229 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py
--rw-------   0 runner    (1001) docker     (127)     6879 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/containerd_configuration.py
--rw-------   0 runner    (1001) docker     (127)    10255 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/containerd_install.py
--rw-------   0 runner    (1001) docker     (127)    10159 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/crictl_install.py
--rw-------   0 runner    (1001) docker     (127)     8328 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/download.py
--rw-------   0 runner    (1001) docker     (127)    12377 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py
--rw-------   0 runner    (1001) docker     (127)    14905 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py
--rw-------   0 runner    (1001) docker     (127)    10651 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/etcd_install.py
--rw-------   0 runner    (1001) docker     (127)    14696 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/etcd_service.py
--rw-------   0 runner    (1001) docker     (127)     7339 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/file.py
--rw-------   0 runner    (1001) docker     (127)     9708 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py
--rw-------   0 runner    (1001) docker     (127)     9822 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py
--rw-------   0 runner    (1001) docker     (127)     9652 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py
--rw-------   0 runner    (1001) docker     (127)     9708 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py
--rw-------   0 runner    (1001) docker     (127)     9622 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py
--rw-------   0 runner    (1001) docker     (127)     9622 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py
--rw-------   0 runner    (1001) docker     (127)    15819 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/kubelet_service.py
--rw-------   0 runner    (1001) docker     (127)    29099 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/outputs.py
--rw-------   0 runner    (1001) docker     (127)    13390 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py
--rw-------   0 runner    (1001) docker     (127)     9580 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/runc_install.py
--rw-------   0 runner    (1001) docker     (127)     5113 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/start_etcd.py
--rw-------   0 runner    (1001) docker     (127)     7429 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/static_pod.py
--rw-------   0 runner    (1001) docker     (127)    10944 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/systemd_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:27:23.967223 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tls/
--rw-------   0 runner    (1001) docker     (127)      425 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tls/__init__.py
--rw-------   0 runner    (1001) docker     (127)     1000 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tls/_enums.py
--rw-------   0 runner    (1001) docker     (127)     3019 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tls/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    30597 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tls/certificate.py
--rw-------   0 runner    (1001) docker     (127)    15919 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py
--rw-------   0 runner    (1001) docker     (127)     4450 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tls/encryption_key.py
--rw-------   0 runner    (1001) docker     (127)     2983 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tls/outputs.py
--rw-------   0 runner    (1001) docker     (127)    27130 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tls/root_ca.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:27:23.971222 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/
--rw-------   0 runner    (1001) docker     (127)      590 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/__init__.py
--rw-------   0 runner    (1001) docker     (127)     3166 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/_enums.py
--rw-------   0 runner    (1001) docker     (127)   108491 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    14957 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/chmod.py
--rw-------   0 runner    (1001) docker     (127)    14976 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/curl.py
--rw-------   0 runner    (1001) docker     (127)    15049 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/etcdctl.py
--rw-------   0 runner    (1001) docker     (127)    15189 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py
--rw-------   0 runner    (1001) docker     (127)    14957 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/mkdir.py
--rw-------   0 runner    (1001) docker     (127)    14992 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/mktemp.py
--rw-------   0 runner    (1001) docker     (127)    14852 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/mv.py
--rw-------   0 runner    (1001) docker     (127)    91820 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/outputs.py
--rw-------   0 runner    (1001) docker     (127)    14852 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/rm.py
--rw-------   0 runner    (1001) docker     (127)    14887 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/sed.py
--rw-------   0 runner    (1001) docker     (127)    15119 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/systemctl.py
--rw-------   0 runner    (1001) docker     (127)    14887 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/tar.py
--rw-------   0 runner    (1001) docker     (127)    14907 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/tee.py
--rw-------   0 runner    (1001) docker     (127)    14922 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/wget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:27:23.971222 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-19 22:27:23.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-05-19 22:27:23.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 22:27:23.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-19 22:27:23.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-19 22:27:23.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way.egg-info/top_level.txt
--rw-------   0 runner    (1001) docker     (127)      899 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 22:27:23.971222 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:22:35.327802 pulumi_kubernetes_the_hard_way-0.0.22/
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-20 00:22:35.327802 pulumi_kubernetes_the_hard_way-0.0.22/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:22:35.315802 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/
+-rw-------   0 runner    (1001) docker     (127)     4454 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     9268 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:22:35.319802 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/config/
+-rw-------   0 runner    (1001) docker     (127)      418 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/config/__init__.py
+-rw-------   0 runner    (1001) docker     (127)      427 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/config/_enums.py
+-rw-------   0 runner    (1001) docker     (127)    21101 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/config/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)     8728 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py
+-rw-------   0 runner    (1001) docker     (127)     3426 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py
+-rw-------   0 runner    (1001) docker     (127)    23922 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py
+-rw-------   0 runner    (1001) docker     (127)    29159 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/config/outputs.py
+-rw-------   0 runner    (1001) docker     (127)     2783 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/provider.py
+-rw-------   0 runner    (1001) docker     (127)      116 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/pulumi-plugin.json
+-rw-------   0 runner    (1001) docker     (127)        0 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:22:35.323802 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/
+-rw-------   0 runner    (1001) docker     (127)     1116 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     1095 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/_enums.py
+-rw-------   0 runner    (1001) docker     (127)    24968 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    13340 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/cni_bridge_plugin_configuration.py
+-rw-------   0 runner    (1001) docker     (127)     8612 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/cni_loopback_plugin_configuration.py
+-rw-------   0 runner    (1001) docker     (127)     7575 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/cni_plugin_configuration.py
+-rw-------   0 runner    (1001) docker     (127)    19229 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py
+-rw-------   0 runner    (1001) docker     (127)     6879 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/containerd_configuration.py
+-rw-------   0 runner    (1001) docker     (127)    10255 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/containerd_install.py
+-rw-------   0 runner    (1001) docker     (127)    10159 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/crictl_install.py
+-rw-------   0 runner    (1001) docker     (127)     8328 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/download.py
+-rw-------   0 runner    (1001) docker     (127)    12377 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py
+-rw-------   0 runner    (1001) docker     (127)    14905 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py
+-rw-------   0 runner    (1001) docker     (127)    10651 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/etcd_install.py
+-rw-------   0 runner    (1001) docker     (127)    14696 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/etcd_service.py
+-rw-------   0 runner    (1001) docker     (127)     7339 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/file.py
+-rw-------   0 runner    (1001) docker     (127)     9708 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py
+-rw-------   0 runner    (1001) docker     (127)     9822 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py
+-rw-------   0 runner    (1001) docker     (127)     9652 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py
+-rw-------   0 runner    (1001) docker     (127)     9708 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py
+-rw-------   0 runner    (1001) docker     (127)     9622 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py
+-rw-------   0 runner    (1001) docker     (127)     9622 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py
+-rw-------   0 runner    (1001) docker     (127)    25169 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/outputs.py
+-rw-------   0 runner    (1001) docker     (127)    13390 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py
+-rw-------   0 runner    (1001) docker     (127)     9580 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/runc_install.py
+-rw-------   0 runner    (1001) docker     (127)     5113 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/start_etcd.py
+-rw-------   0 runner    (1001) docker     (127)     7429 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/static_pod.py
+-rw-------   0 runner    (1001) docker     (127)    10944 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/systemd_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:22:35.323802 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tls/
+-rw-------   0 runner    (1001) docker     (127)      425 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tls/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     1000 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tls/_enums.py
+-rw-------   0 runner    (1001) docker     (127)     3019 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tls/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    30597 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tls/certificate.py
+-rw-------   0 runner    (1001) docker     (127)    15919 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py
+-rw-------   0 runner    (1001) docker     (127)     4450 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tls/encryption_key.py
+-rw-------   0 runner    (1001) docker     (127)     2983 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tls/outputs.py
+-rw-------   0 runner    (1001) docker     (127)    27130 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tls/root_ca.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:22:35.327802 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/
+-rw-------   0 runner    (1001) docker     (127)      590 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     3166 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/_enums.py
+-rw-------   0 runner    (1001) docker     (127)   108491 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    14957 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/chmod.py
+-rw-------   0 runner    (1001) docker     (127)    14976 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/curl.py
+-rw-------   0 runner    (1001) docker     (127)    15049 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/etcdctl.py
+-rw-------   0 runner    (1001) docker     (127)    15189 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py
+-rw-------   0 runner    (1001) docker     (127)    14957 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/mkdir.py
+-rw-------   0 runner    (1001) docker     (127)    14992 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/mktemp.py
+-rw-------   0 runner    (1001) docker     (127)    14852 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/mv.py
+-rw-------   0 runner    (1001) docker     (127)    91820 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/outputs.py
+-rw-------   0 runner    (1001) docker     (127)    14852 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/rm.py
+-rw-------   0 runner    (1001) docker     (127)    14887 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/sed.py
+-rw-------   0 runner    (1001) docker     (127)    15119 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/systemctl.py
+-rw-------   0 runner    (1001) docker     (127)    14887 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/tar.py
+-rw-------   0 runner    (1001) docker     (127)    14907 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/tee.py
+-rw-------   0 runner    (1001) docker     (127)    14922 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/wget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:22:35.327802 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-20 00:22:35.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-05-20 00:22:35.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 00:22:35.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-20 00:22:35.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-20 00:22:35.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way.egg-info/top_level.txt
+-rw-------   0 runner    (1001) docker     (127)      888 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 00:22:35.327802 pulumi_kubernetes_the_hard_way-0.0.22/setup.cfg
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/PKG-INFO` & `pulumi_kubernetes_the_hard_way-0.0.22/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kubernetes_the_hard_way
-Version: 0.0.21a1716157484
+Version: 0.0.22
 Summary: A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way
 License: Apache-2.0
 Project-URL: Repository, https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way
 Keywords: pulumi,command,tls,kubernetes,category/utility,kind/component
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/README.md` & `pulumi_kubernetes_the_hard_way-0.0.22/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,16 +27,15 @@
     resource_modules="""
 [
  {
   "pkg": "kubernetes-the-hard-way",
   "mod": "config",
   "fqn": "pulumi_kubernetes_the_hard_way.config",
   "classes": {
-   "kubernetes-the-hard-way:config:KubeVipManifest": "KubeVipManifest",
-   "kubernetes-the-hard-way:config:KubeletConfiguration": "KubeletConfiguration"
+   "kubernetes-the-hard-way:config:KubeVipManifest": "KubeVipManifest"
   }
  },
  {
   "pkg": "kubernetes-the-hard-way",
   "mod": "remote",
   "fqn": "pulumi_kubernetes_the_hard_way.remote",
   "classes": {
@@ -55,15 +54,14 @@
    "kubernetes-the-hard-way:remote:File": "File",
    "kubernetes-the-hard-way:remote:KubeApiServerInstall": "KubeApiServerInstall",
    "kubernetes-the-hard-way:remote:KubeControllerManagerInstall": "KubeControllerManagerInstall",
    "kubernetes-the-hard-way:remote:KubeProxyInstall": "KubeProxyInstall",
    "kubernetes-the-hard-way:remote:KubeSchedulerInstall": "KubeSchedulerInstall",
    "kubernetes-the-hard-way:remote:KubectlInstall": "KubectlInstall",
    "kubernetes-the-hard-way:remote:KubeletInstall": "KubeletInstall",
-   "kubernetes-the-hard-way:remote:KubeletService": "KubeletService",
    "kubernetes-the-hard-way:remote:ProvisionEtcd": "ProvisionEtcd",
    "kubernetes-the-hard-way:remote:RuncInstall": "RuncInstall",
    "kubernetes-the-hard-way:remote:StartEtcd": "StartEtcd",
    "kubernetes-the-hard-way:remote:StaticPod": "StaticPod",
    "kubernetes-the-hard-way:remote:SystemdService": "SystemdService"
   }
  },
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/_utilities.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/config/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/config/_inputs.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,17 +21,14 @@
 ]
 
 @pulumi.input_type
 class KubeconfigAdminOptions:
     def __init__(__self__, *,
                  type: str,
                  public_ip: Optional[str] = None):
-        """
-        :param str public_ip: TODO
-        """
         pulumi.set(__self__, "type", 'admin')
         if public_ip is not None:
             pulumi.set(__self__, "public_ip", public_ip)
 
     @property
     @pulumi.getter
     def type(self) -> str:
@@ -40,32 +37,26 @@
     @type.setter
     def type(self, value: str):
         pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter(name="publicIp")
     def public_ip(self) -> Optional[str]:
-        """
-        TODO
-        """
         return pulumi.get(self, "public_ip")
 
     @public_ip.setter
     def public_ip(self, value: Optional[str]):
         pulumi.set(self, "public_ip", value)
 
 
 @pulumi.input_type
 class KubeconfigKubeControllerManagerOptions:
     def __init__(__self__, *,
                  type: str,
                  public_ip: Optional[str] = None):
-        """
-        :param str public_ip: TODO
-        """
         pulumi.set(__self__, "type", 'kube-controller-manager')
         if public_ip is not None:
             pulumi.set(__self__, "public_ip", public_ip)
 
     @property
     @pulumi.getter
     def type(self) -> str:
@@ -74,32 +65,26 @@
     @type.setter
     def type(self, value: str):
         pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter(name="publicIp")
     def public_ip(self) -> Optional[str]:
-        """
-        TODO
-        """
         return pulumi.get(self, "public_ip")
 
     @public_ip.setter
     def public_ip(self, value: Optional[str]):
         pulumi.set(self, "public_ip", value)
 
 
 @pulumi.input_type
 class KubeconfigKubeProxyOptions:
     def __init__(__self__, *,
                  type: str,
                  public_ip: Optional[str] = None):
-        """
-        :param str public_ip: TODO
-        """
         pulumi.set(__self__, "type", 'kube-proxy')
         if public_ip is not None:
             pulumi.set(__self__, "public_ip", public_ip)
 
     @property
     @pulumi.getter
     def type(self) -> str:
@@ -108,32 +93,26 @@
     @type.setter
     def type(self, value: str):
         pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter(name="publicIp")
     def public_ip(self) -> Optional[str]:
-        """
-        TODO
-        """
         return pulumi.get(self, "public_ip")
 
     @public_ip.setter
     def public_ip(self, value: Optional[str]):
         pulumi.set(self, "public_ip", value)
 
 
 @pulumi.input_type
 class KubeconfigKubeSchedulerOptions:
     def __init__(__self__, *,
                  type: str,
                  public_ip: Optional[str] = None):
-        """
-        :param str public_ip: TODO
-        """
         pulumi.set(__self__, "type", 'kube-scheduler')
         if public_ip is not None:
             pulumi.set(__self__, "public_ip", public_ip)
 
     @property
     @pulumi.getter
     def type(self) -> str:
@@ -142,57 +121,44 @@
     @type.setter
     def type(self, value: str):
         pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter(name="publicIp")
     def public_ip(self) -> Optional[str]:
-        """
-        TODO
-        """
         return pulumi.get(self, "public_ip")
 
     @public_ip.setter
     def public_ip(self, value: Optional[str]):
         pulumi.set(self, "public_ip", value)
 
 
 @pulumi.input_type
 class KubeconfigWorkerOptions:
     def __init__(__self__, *,
                  name: str,
                  public_ip: str,
                  type: Optional[str] = None):
-        """
-        :param str name: TODO
-        :param str public_ip: TODO
-        """
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "public_ip", public_ip)
         if type is not None:
             pulumi.set(__self__, "type", 'worker')
 
     @property
     @pulumi.getter
     def name(self) -> str:
-        """
-        TODO
-        """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: str):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter(name="publicIp")
     def public_ip(self) -> str:
-        """
-        TODO
-        """
         return pulumi.get(self, "public_ip")
 
     @public_ip.setter
     def public_ip(self, value: str):
         pulumi.set(self, "public_ip", value)
 
     @property
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,14 @@
     'AwaitableGetKubeVipManifestResult',
     'get_kube_vip_manifest',
     'get_kube_vip_manifest_output',
 ]
 
 @pulumi.output_type
 class GetKubeVipManifestResult:
-    """
-    Gets the static pod manifests for KubeVip.
-    """
     def __init__(__self__, result=None):
         if result and not isinstance(result, dict):
             raise TypeError("Expected argument 'result' to be a dict")
         pulumi.set(__self__, "result", result)
 
     @property
     @pulumi.getter
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py`

 * *Files 1% similar despite different names*

```diff
@@ -452,15 +452,15 @@
                  vip_interface: Optional[pulumi.Input[str]] = None,
                  vip_leader_election: Optional[pulumi.Input[bool]] = None,
                  vip_lease_duration: Optional[pulumi.Input[int]] = None,
                  vip_renew_deadline: Optional[pulumi.Input[int]] = None,
                  vip_retry_period: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         """
-        Gets the static pod manifests for KubeVip.
+        Pseudo resource for generating the kube-vip manifest.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] address: TODO
         :param pulumi.Input[int] bgp_as: TODO
         :param pulumi.Input[bool] bgp_enable: TODO
         :param pulumi.Input[str] bgp_peer_address: TODO
@@ -489,15 +489,15 @@
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: KubeVipManifestArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Gets the static pod manifests for KubeVip.
+        Pseudo resource for generating the kube-vip manifest.
 
         :param str resource_name: The name of the resource.
         :param KubeVipManifestArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
@@ -597,11 +597,11 @@
     def result(self) -> pulumi.Output['outputs.PodManifest']:
         return pulumi.get(self, "result")
 
     @property
     @pulumi.getter
     def yaml(self) -> pulumi.Output[str]:
         """
-        The yaml representation of the manifest.
+        The yaml representation of the manifest
         """
         return pulumi.get(self, "yaml")
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/config/kubelet_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,283 +5,314 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
+from .. import tls as _tls
+from ._enums import *
+from ._inputs import *
+from .etcd_configuration import EtcdConfiguration
+from .etcd_install import EtcdInstall
+from .etcd_service import EtcdService
+from .start_etcd import StartEtcd
+import pulumi_command
 
-__all__ = ['KubeletConfigurationArgs', 'KubeletConfiguration']
+__all__ = ['EtcdClusterArgs', 'EtcdCluster']
 
 @pulumi.input_type
-class KubeletConfigurationArgs:
+class EtcdClusterArgs:
     def __init__(__self__, *,
-                 pod_cidr: pulumi.Input[str],
-                 anonymous: Optional[pulumi.Input[bool]] = None,
-                 authorization_mode: Optional[pulumi.Input[str]] = None,
-                 cgroup_driver: Optional[pulumi.Input[str]] = None,
-                 client_ca_file: Optional[pulumi.Input[str]] = None,
-                 cluster_dns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 cluster_domain: Optional[pulumi.Input[str]] = None,
-                 container_runtime_endpoint: Optional[pulumi.Input[str]] = None,
-                 resolv_conf: Optional[pulumi.Input[str]] = None,
-                 runtime_request_timeout: Optional[pulumi.Input[str]] = None,
-                 tls_cert_file: Optional[pulumi.Input[str]] = None,
-                 tls_private_key_file: Optional[pulumi.Input[str]] = None,
-                 webhook: Optional[pulumi.Input[bool]] = None):
+                 bundle: pulumi.Input['_tls.BundleArgs'],
+                 nodes: Mapping[str, pulumi.Input['EtcdNodeArgs']],
+                 architecture: Optional[pulumi.Input['Architecture']] = None,
+                 binary_directory: Optional[pulumi.Input[str]] = None,
+                 configuration_directory: Optional[pulumi.Input[str]] = None,
+                 data_directory: Optional[pulumi.Input[str]] = None,
+                 version: Optional[pulumi.Input[str]] = None):
         """
-        The set of arguments for constructing a KubeletConfiguration resource.
+        The set of arguments for constructing a EtcdCluster resource.
+        :param pulumi.Input['_tls.BundleArgs'] bundle: The TLS bundle.
+        :param Mapping[str, pulumi.Input['EtcdNodeArgs']] nodes: Etcd node configuration. The key should be a name used to identify the node.
+        :param pulumi.Input['Architecture'] architecture: TODO
+        :param pulumi.Input[str] binary_directory: TODO
+        :param pulumi.Input[str] configuration_directory: The directory to use for etcd configuration.
+        :param pulumi.Input[str] data_directory: The directory to use for etcd data.
+        :param pulumi.Input[str] version: The version to install.
         """
-        pulumi.set(__self__, "pod_cidr", pod_cidr)
-        if anonymous is not None:
-            pulumi.set(__self__, "anonymous", anonymous)
-        if authorization_mode is not None:
-            pulumi.set(__self__, "authorization_mode", authorization_mode)
-        if cgroup_driver is not None:
-            pulumi.set(__self__, "cgroup_driver", cgroup_driver)
-        if client_ca_file is not None:
-            pulumi.set(__self__, "client_ca_file", client_ca_file)
-        if cluster_dns is not None:
-            pulumi.set(__self__, "cluster_dns", cluster_dns)
-        if cluster_domain is not None:
-            pulumi.set(__self__, "cluster_domain", cluster_domain)
-        if container_runtime_endpoint is not None:
-            pulumi.set(__self__, "container_runtime_endpoint", container_runtime_endpoint)
-        if resolv_conf is not None:
-            pulumi.set(__self__, "resolv_conf", resolv_conf)
-        if runtime_request_timeout is not None:
-            pulumi.set(__self__, "runtime_request_timeout", runtime_request_timeout)
-        if tls_cert_file is not None:
-            pulumi.set(__self__, "tls_cert_file", tls_cert_file)
-        if tls_private_key_file is not None:
-            pulumi.set(__self__, "tls_private_key_file", tls_private_key_file)
-        if webhook is not None:
-            pulumi.set(__self__, "webhook", webhook)
-
-    @property
-    @pulumi.getter(name="podCIDR")
-    def pod_cidr(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "pod_cidr")
-
-    @pod_cidr.setter
-    def pod_cidr(self, value: pulumi.Input[str]):
-        pulumi.set(self, "pod_cidr", value)
+        pulumi.set(__self__, "bundle", bundle)
+        pulumi.set(__self__, "nodes", nodes)
+        if architecture is not None:
+            pulumi.set(__self__, "architecture", architecture)
+        if binary_directory is not None:
+            pulumi.set(__self__, "binary_directory", binary_directory)
+        if configuration_directory is not None:
+            pulumi.set(__self__, "configuration_directory", configuration_directory)
+        if data_directory is not None:
+            pulumi.set(__self__, "data_directory", data_directory)
+        if version is not None:
+            pulumi.set(__self__, "version", version)
 
     @property
     @pulumi.getter
-    def anonymous(self) -> Optional[pulumi.Input[bool]]:
-        return pulumi.get(self, "anonymous")
-
-    @anonymous.setter
-    def anonymous(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "anonymous", value)
-
-    @property
-    @pulumi.getter(name="authorizationMode")
-    def authorization_mode(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "authorization_mode")
-
-    @authorization_mode.setter
-    def authorization_mode(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "authorization_mode", value)
-
-    @property
-    @pulumi.getter(name="cgroupDriver")
-    def cgroup_driver(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "cgroup_driver")
-
-    @cgroup_driver.setter
-    def cgroup_driver(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "cgroup_driver", value)
-
-    @property
-    @pulumi.getter(name="clientCAFile")
-    def client_ca_file(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "client_ca_file")
-
-    @client_ca_file.setter
-    def client_ca_file(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "client_ca_file", value)
-
-    @property
-    @pulumi.getter(name="clusterDNS")
-    def cluster_dns(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        return pulumi.get(self, "cluster_dns")
-
-    @cluster_dns.setter
-    def cluster_dns(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "cluster_dns", value)
-
-    @property
-    @pulumi.getter(name="clusterDomain")
-    def cluster_domain(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "cluster_domain")
+    def bundle(self) -> pulumi.Input['_tls.BundleArgs']:
+        """
+        The TLS bundle.
+        """
+        return pulumi.get(self, "bundle")
 
-    @cluster_domain.setter
-    def cluster_domain(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "cluster_domain", value)
+    @bundle.setter
+    def bundle(self, value: pulumi.Input['_tls.BundleArgs']):
+        pulumi.set(self, "bundle", value)
 
     @property
-    @pulumi.getter(name="containerRuntimeEndpoint")
-    def container_runtime_endpoint(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "container_runtime_endpoint")
+    @pulumi.getter
+    def nodes(self) -> Mapping[str, pulumi.Input['EtcdNodeArgs']]:
+        """
+        Etcd node configuration. The key should be a name used to identify the node.
+        """
+        return pulumi.get(self, "nodes")
 
-    @container_runtime_endpoint.setter
-    def container_runtime_endpoint(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "container_runtime_endpoint", value)
+    @nodes.setter
+    def nodes(self, value: Mapping[str, pulumi.Input['EtcdNodeArgs']]):
+        pulumi.set(self, "nodes", value)
 
     @property
-    @pulumi.getter(name="resolvConf")
-    def resolv_conf(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "resolv_conf")
+    @pulumi.getter
+    def architecture(self) -> Optional[pulumi.Input['Architecture']]:
+        """
+        TODO
+        """
+        return pulumi.get(self, "architecture")
 
-    @resolv_conf.setter
-    def resolv_conf(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "resolv_conf", value)
+    @architecture.setter
+    def architecture(self, value: Optional[pulumi.Input['Architecture']]):
+        pulumi.set(self, "architecture", value)
 
     @property
-    @pulumi.getter(name="runtimeRequestTimeout")
-    def runtime_request_timeout(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "runtime_request_timeout")
+    @pulumi.getter(name="binaryDirectory")
+    def binary_directory(self) -> Optional[pulumi.Input[str]]:
+        """
+        TODO
+        """
+        return pulumi.get(self, "binary_directory")
 
-    @runtime_request_timeout.setter
-    def runtime_request_timeout(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "runtime_request_timeout", value)
+    @binary_directory.setter
+    def binary_directory(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "binary_directory", value)
 
     @property
-    @pulumi.getter(name="tlsCertFile")
-    def tls_cert_file(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "tls_cert_file")
+    @pulumi.getter(name="configurationDirectory")
+    def configuration_directory(self) -> Optional[pulumi.Input[str]]:
+        """
+        The directory to use for etcd configuration.
+        """
+        return pulumi.get(self, "configuration_directory")
 
-    @tls_cert_file.setter
-    def tls_cert_file(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "tls_cert_file", value)
+    @configuration_directory.setter
+    def configuration_directory(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "configuration_directory", value)
 
     @property
-    @pulumi.getter(name="tlsPrivateKeyFile")
-    def tls_private_key_file(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "tls_private_key_file")
+    @pulumi.getter(name="dataDirectory")
+    def data_directory(self) -> Optional[pulumi.Input[str]]:
+        """
+        The directory to use for etcd data.
+        """
+        return pulumi.get(self, "data_directory")
 
-    @tls_private_key_file.setter
-    def tls_private_key_file(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "tls_private_key_file", value)
+    @data_directory.setter
+    def data_directory(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "data_directory", value)
 
     @property
     @pulumi.getter
-    def webhook(self) -> Optional[pulumi.Input[bool]]:
-        return pulumi.get(self, "webhook")
+    def version(self) -> Optional[pulumi.Input[str]]:
+        """
+        The version to install.
+        """
+        return pulumi.get(self, "version")
 
-    @webhook.setter
-    def webhook(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "webhook", value)
+    @version.setter
+    def version(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "version", value)
 
 
-class KubeletConfiguration(pulumi.ComponentResource):
+class EtcdCluster(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 anonymous: Optional[pulumi.Input[bool]] = None,
-                 authorization_mode: Optional[pulumi.Input[str]] = None,
-                 cgroup_driver: Optional[pulumi.Input[str]] = None,
-                 client_ca_file: Optional[pulumi.Input[str]] = None,
-                 cluster_dns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 cluster_domain: Optional[pulumi.Input[str]] = None,
-                 container_runtime_endpoint: Optional[pulumi.Input[str]] = None,
-                 pod_cidr: Optional[pulumi.Input[str]] = None,
-                 resolv_conf: Optional[pulumi.Input[str]] = None,
-                 runtime_request_timeout: Optional[pulumi.Input[str]] = None,
-                 tls_cert_file: Optional[pulumi.Input[str]] = None,
-                 tls_private_key_file: Optional[pulumi.Input[str]] = None,
-                 webhook: Optional[pulumi.Input[bool]] = None,
+                 architecture: Optional[pulumi.Input['Architecture']] = None,
+                 binary_directory: Optional[pulumi.Input[str]] = None,
+                 bundle: Optional[pulumi.Input[pulumi.InputType['_tls.BundleArgs']]] = None,
+                 configuration_directory: Optional[pulumi.Input[str]] = None,
+                 data_directory: Optional[pulumi.Input[str]] = None,
+                 nodes: Optional[Mapping[str, pulumi.Input[pulumi.InputType['EtcdNodeArgs']]]] = None,
+                 version: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Get the kubelet configuration.
+        Creates an etcd cluster from one or more remote systems.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input['Architecture'] architecture: TODO
+        :param pulumi.Input[str] binary_directory: TODO
+        :param pulumi.Input[pulumi.InputType['_tls.BundleArgs']] bundle: The TLS bundle.
+        :param pulumi.Input[str] configuration_directory: The directory to use for etcd configuration.
+        :param pulumi.Input[str] data_directory: The directory to use for etcd data.
+        :param Mapping[str, pulumi.Input[pulumi.InputType['EtcdNodeArgs']]] nodes: Etcd node configuration. The key should be a name used to identify the node.
+        :param pulumi.Input[str] version: The version to install.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: KubeletConfigurationArgs,
+                 args: EtcdClusterArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Get the kubelet configuration.
+        Creates an etcd cluster from one or more remote systems.
 
         :param str resource_name: The name of the resource.
-        :param KubeletConfigurationArgs args: The arguments to use to populate this resource's properties.
+        :param EtcdClusterArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(KubeletConfigurationArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(EtcdClusterArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 anonymous: Optional[pulumi.Input[bool]] = None,
-                 authorization_mode: Optional[pulumi.Input[str]] = None,
-                 cgroup_driver: Optional[pulumi.Input[str]] = None,
-                 client_ca_file: Optional[pulumi.Input[str]] = None,
-                 cluster_dns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 cluster_domain: Optional[pulumi.Input[str]] = None,
-                 container_runtime_endpoint: Optional[pulumi.Input[str]] = None,
-                 pod_cidr: Optional[pulumi.Input[str]] = None,
-                 resolv_conf: Optional[pulumi.Input[str]] = None,
-                 runtime_request_timeout: Optional[pulumi.Input[str]] = None,
-                 tls_cert_file: Optional[pulumi.Input[str]] = None,
-                 tls_private_key_file: Optional[pulumi.Input[str]] = None,
-                 webhook: Optional[pulumi.Input[bool]] = None,
+                 architecture: Optional[pulumi.Input['Architecture']] = None,
+                 binary_directory: Optional[pulumi.Input[str]] = None,
+                 bundle: Optional[pulumi.Input[pulumi.InputType['_tls.BundleArgs']]] = None,
+                 configuration_directory: Optional[pulumi.Input[str]] = None,
+                 data_directory: Optional[pulumi.Input[str]] = None,
+                 nodes: Optional[Mapping[str, pulumi.Input[pulumi.InputType['EtcdNodeArgs']]]] = None,
+                 version: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = KubeletConfigurationArgs.__new__(KubeletConfigurationArgs)
+            __props__ = EtcdClusterArgs.__new__(EtcdClusterArgs)
 
-            __props__.__dict__["anonymous"] = anonymous
-            __props__.__dict__["authorization_mode"] = authorization_mode
-            __props__.__dict__["cgroup_driver"] = cgroup_driver
-            __props__.__dict__["client_ca_file"] = client_ca_file
-            __props__.__dict__["cluster_dns"] = cluster_dns
-            __props__.__dict__["cluster_domain"] = cluster_domain
-            __props__.__dict__["container_runtime_endpoint"] = container_runtime_endpoint
-            if pod_cidr is None and not opts.urn:
-                raise TypeError("Missing required property 'pod_cidr'")
-            __props__.__dict__["pod_cidr"] = pod_cidr
-            __props__.__dict__["resolv_conf"] = resolv_conf
-            __props__.__dict__["runtime_request_timeout"] = runtime_request_timeout
-            __props__.__dict__["tls_cert_file"] = tls_cert_file
-            __props__.__dict__["tls_private_key_file"] = tls_private_key_file
-            __props__.__dict__["webhook"] = webhook
-            __props__.__dict__["result"] = None
-            __props__.__dict__["yaml"] = None
-        super(KubeletConfiguration, __self__).__init__(
-            'kubernetes-the-hard-way:config:KubeletConfiguration',
+            __props__.__dict__["architecture"] = architecture
+            __props__.__dict__["binary_directory"] = binary_directory
+            if bundle is None and not opts.urn:
+                raise TypeError("Missing required property 'bundle'")
+            __props__.__dict__["bundle"] = bundle
+            __props__.__dict__["configuration_directory"] = configuration_directory
+            __props__.__dict__["data_directory"] = data_directory
+            if nodes is None and not opts.urn:
+                raise TypeError("Missing required property 'nodes'")
+            __props__.__dict__["nodes"] = nodes
+            __props__.__dict__["version"] = version
+            __props__.__dict__["configuration"] = None
+            __props__.__dict__["install"] = None
+            __props__.__dict__["service"] = None
+            __props__.__dict__["start"] = None
+        super(EtcdCluster, __self__).__init__(
+            'kubernetes-the-hard-way:remote:EtcdCluster',
             resource_name,
             __props__,
             opts,
             remote=True)
 
     @property
     @pulumi.getter
-    def result(self) -> pulumi.Output['outputs.KubeletConfiguration']:
-        return pulumi.get(self, "result")
+    def architecture(self) -> pulumi.Output[Optional['Architecture']]:
+        """
+        TODO
+        """
+        return pulumi.get(self, "architecture")
+
+    @property
+    @pulumi.getter(name="binaryDirectory")
+    def binary_directory(self) -> pulumi.Output[Optional[str]]:
+        """
+        TODO
+        """
+        return pulumi.get(self, "binary_directory")
+
+    @property
+    @pulumi.getter
+    def bundle(self) -> pulumi.Output['_tls.outputs.Bundle']:
+        """
+        The TLS bundle.
+        """
+        return pulumi.get(self, "bundle")
+
+    @property
+    @pulumi.getter
+    def configuration(self) -> pulumi.Output[Mapping[str, 'EtcdConfiguration']]:
+        """
+        Map of node name to etcd configuration.
+        """
+        return pulumi.get(self, "configuration")
+
+    @property
+    @pulumi.getter(name="configurationDirectory")
+    def configuration_directory(self) -> pulumi.Output[Optional[str]]:
+        """
+        The directory to use for etcd configuration.
+        """
+        return pulumi.get(self, "configuration_directory")
+
+    @property
+    @pulumi.getter(name="dataDirectory")
+    def data_directory(self) -> pulumi.Output[Optional[str]]:
+        """
+        The directory to use for etcd data.
+        """
+        return pulumi.get(self, "data_directory")
+
+    @property
+    @pulumi.getter
+    def install(self) -> pulumi.Output[Mapping[str, 'EtcdInstall']]:
+        """
+        Map of node name to etcd install.
+        """
+        return pulumi.get(self, "install")
+
+    @property
+    @pulumi.getter
+    def nodes(self) -> pulumi.Output[Mapping[str, 'outputs.EtcdNode']]:
+        """
+        Etcd node configuration. The key should be a name used to identify the node.
+        """
+        return pulumi.get(self, "nodes")
+
+    @property
+    @pulumi.getter
+    def service(self) -> pulumi.Output[Mapping[str, 'EtcdService']]:
+        """
+        Map of node name to etcd systemd service.
+        """
+        return pulumi.get(self, "service")
+
+    @property
+    @pulumi.getter
+    def start(self) -> pulumi.Output[Mapping[str, 'StartEtcd']]:
+        """
+        Map of node name to etcd start commands.
+        """
+        return pulumi.get(self, "start")
 
     @property
     @pulumi.getter
-    def yaml(self) -> pulumi.Output[str]:
+    def version(self) -> pulumi.Output[Optional[str]]:
         """
-        The yaml representation of the manifest.
+        The version to install.
         """
-        return pulumi.get(self, "yaml")
+        return pulumi.get(self, "version")
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/config/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/config/outputs.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,79 +12,53 @@
 from ._enums import *
 import pulumi_kubernetes
 
 __all__ = [
     'Cluster',
     'Context',
     'Kubeconfig',
-    'KubeletConfiguration',
-    'KubeletConfigurationAuthentication',
-    'KubeletConfigurationAuthenticationAnonymous',
-    'KubeletConfigurationAuthenticationWebhook',
-    'KubeletConfigurationAuthenticationx509',
-    'KubeletConfigurationAuthorization',
     'PodManifest',
     'User',
 ]
 
 @pulumi.output_type
 class Cluster(dict):
     def __init__(__self__, *,
                  certificate_authority_data: str,
                  server: str):
-        """
-        :param str certificate_authority_data: TODO
-        :param str server: TODO
-        """
         pulumi.set(__self__, "certificate_authority_data", certificate_authority_data)
         pulumi.set(__self__, "server", server)
 
     @property
     @pulumi.getter(name="certificateAuthorityData")
     def certificate_authority_data(self) -> str:
-        """
-        TODO
-        """
         return pulumi.get(self, "certificate_authority_data")
 
     @property
     @pulumi.getter
     def server(self) -> str:
-        """
-        TODO
-        """
         return pulumi.get(self, "server")
 
 
 @pulumi.output_type
 class Context(dict):
     def __init__(__self__, *,
                  cluster: str,
                  user: str):
-        """
-        :param str cluster: TODO
-        :param str user: TODO
-        """
         pulumi.set(__self__, "cluster", cluster)
         pulumi.set(__self__, "user", user)
 
     @property
     @pulumi.getter
     def cluster(self) -> str:
-        """
-        TODO
-        """
         return pulumi.get(self, "cluster")
 
     @property
     @pulumi.getter
     def user(self) -> str:
-        """
-        TODO
-        """
         return pulumi.get(self, "user")
 
 
 @pulumi.output_type
 class Kubeconfig(dict):
     def __init__(__self__, *,
                  clusters: Sequence['outputs.Cluster'],
@@ -107,292 +81,14 @@
     @property
     @pulumi.getter
     def users(self) -> Sequence['outputs.User']:
         return pulumi.get(self, "users")
 
 
 @pulumi.output_type
-class KubeletConfiguration(dict):
-    @staticmethod
-    def __key_warning(key: str):
-        suggest = None
-        if key == "apiVersion":
-            suggest = "api_version"
-        elif key == "cgroupDriver":
-            suggest = "cgroup_driver"
-        elif key == "clusterDNS":
-            suggest = "cluster_dns"
-        elif key == "clusterDomain":
-            suggest = "cluster_domain"
-        elif key == "containerRuntimeEndpoint":
-            suggest = "container_runtime_endpoint"
-        elif key == "podCIDR":
-            suggest = "pod_cidr"
-        elif key == "resolvConf":
-            suggest = "resolv_conf"
-        elif key == "runtimeRequestTimeout":
-            suggest = "runtime_request_timeout"
-        elif key == "tlsCertFile":
-            suggest = "tls_cert_file"
-        elif key == "tlsPrivateKeyFile":
-            suggest = "tls_private_key_file"
-
-        if suggest:
-            pulumi.log.warn(f"Key '{key}' not found in KubeletConfiguration. Access the value via the '{suggest}' property getter instead.")
-
-    def __getitem__(self, key: str) -> Any:
-        KubeletConfiguration.__key_warning(key)
-        return super().__getitem__(key)
-
-    def get(self, key: str, default = None) -> Any:
-        KubeletConfiguration.__key_warning(key)
-        return super().get(key, default)
-
-    def __init__(__self__, *,
-                 api_version: str,
-                 authentication: 'outputs.KubeletConfigurationAuthentication',
-                 authorization: 'outputs.KubeletConfigurationAuthorization',
-                 cgroup_driver: str,
-                 cluster_dns: Sequence[str],
-                 cluster_domain: str,
-                 container_runtime_endpoint: str,
-                 kind: str,
-                 pod_cidr: str,
-                 resolv_conf: str,
-                 runtime_request_timeout: str,
-                 tls_cert_file: str,
-                 tls_private_key_file: str):
-        """
-        :param str cgroup_driver: TODO
-        :param Sequence[str] cluster_dns: TODO
-        :param str cluster_domain: TODO
-        :param str container_runtime_endpoint: TODO
-        :param str pod_cidr: TODO
-        :param str resolv_conf: TODO
-        :param str runtime_request_timeout: TODO
-        :param str tls_cert_file: TODO
-        :param str tls_private_key_file: TODO
-        """
-        pulumi.set(__self__, "api_version", 'kubelet.config.k8s.io/v1beta1')
-        pulumi.set(__self__, "authentication", authentication)
-        pulumi.set(__self__, "authorization", authorization)
-        pulumi.set(__self__, "cgroup_driver", cgroup_driver)
-        pulumi.set(__self__, "cluster_dns", cluster_dns)
-        pulumi.set(__self__, "cluster_domain", cluster_domain)
-        pulumi.set(__self__, "container_runtime_endpoint", container_runtime_endpoint)
-        pulumi.set(__self__, "kind", 'KubeletConfiguration')
-        pulumi.set(__self__, "pod_cidr", pod_cidr)
-        pulumi.set(__self__, "resolv_conf", resolv_conf)
-        pulumi.set(__self__, "runtime_request_timeout", runtime_request_timeout)
-        pulumi.set(__self__, "tls_cert_file", tls_cert_file)
-        pulumi.set(__self__, "tls_private_key_file", tls_private_key_file)
-
-    @property
-    @pulumi.getter(name="apiVersion")
-    def api_version(self) -> str:
-        return pulumi.get(self, "api_version")
-
-    @property
-    @pulumi.getter
-    def authentication(self) -> 'outputs.KubeletConfigurationAuthentication':
-        return pulumi.get(self, "authentication")
-
-    @property
-    @pulumi.getter
-    def authorization(self) -> 'outputs.KubeletConfigurationAuthorization':
-        return pulumi.get(self, "authorization")
-
-    @property
-    @pulumi.getter(name="cgroupDriver")
-    def cgroup_driver(self) -> str:
-        """
-        TODO
-        """
-        return pulumi.get(self, "cgroup_driver")
-
-    @property
-    @pulumi.getter(name="clusterDNS")
-    def cluster_dns(self) -> Sequence[str]:
-        """
-        TODO
-        """
-        return pulumi.get(self, "cluster_dns")
-
-    @property
-    @pulumi.getter(name="clusterDomain")
-    def cluster_domain(self) -> str:
-        """
-        TODO
-        """
-        return pulumi.get(self, "cluster_domain")
-
-    @property
-    @pulumi.getter(name="containerRuntimeEndpoint")
-    def container_runtime_endpoint(self) -> str:
-        """
-        TODO
-        """
-        return pulumi.get(self, "container_runtime_endpoint")
-
-    @property
-    @pulumi.getter
-    def kind(self) -> str:
-        return pulumi.get(self, "kind")
-
-    @property
-    @pulumi.getter(name="podCIDR")
-    def pod_cidr(self) -> str:
-        """
-        TODO
-        """
-        return pulumi.get(self, "pod_cidr")
-
-    @property
-    @pulumi.getter(name="resolvConf")
-    def resolv_conf(self) -> str:
-        """
-        TODO
-        """
-        return pulumi.get(self, "resolv_conf")
-
-    @property
-    @pulumi.getter(name="runtimeRequestTimeout")
-    def runtime_request_timeout(self) -> str:
-        """
-        TODO
-        """
-        return pulumi.get(self, "runtime_request_timeout")
-
-    @property
-    @pulumi.getter(name="tlsCertFile")
-    def tls_cert_file(self) -> str:
-        """
-        TODO
-        """
-        return pulumi.get(self, "tls_cert_file")
-
-    @property
-    @pulumi.getter(name="tlsPrivateKeyFile")
-    def tls_private_key_file(self) -> str:
-        """
-        TODO
-        """
-        return pulumi.get(self, "tls_private_key_file")
-
-
-@pulumi.output_type
-class KubeletConfigurationAuthentication(dict):
-    def __init__(__self__, *,
-                 anonymous: 'outputs.KubeletConfigurationAuthenticationAnonymous',
-                 webhook: 'outputs.KubeletConfigurationAuthenticationWebhook',
-                 x509: 'outputs.KubeletConfigurationAuthenticationx509'):
-        pulumi.set(__self__, "anonymous", anonymous)
-        pulumi.set(__self__, "webhook", webhook)
-        pulumi.set(__self__, "x509", x509)
-
-    @property
-    @pulumi.getter
-    def anonymous(self) -> 'outputs.KubeletConfigurationAuthenticationAnonymous':
-        return pulumi.get(self, "anonymous")
-
-    @property
-    @pulumi.getter
-    def webhook(self) -> 'outputs.KubeletConfigurationAuthenticationWebhook':
-        return pulumi.get(self, "webhook")
-
-    @property
-    @pulumi.getter
-    def x509(self) -> 'outputs.KubeletConfigurationAuthenticationx509':
-        return pulumi.get(self, "x509")
-
-
-@pulumi.output_type
-class KubeletConfigurationAuthenticationAnonymous(dict):
-    def __init__(__self__, *,
-                 enabled: bool):
-        """
-        :param bool enabled: TODO
-        """
-        pulumi.set(__self__, "enabled", enabled)
-
-    @property
-    @pulumi.getter
-    def enabled(self) -> bool:
-        """
-        TODO
-        """
-        return pulumi.get(self, "enabled")
-
-
-@pulumi.output_type
-class KubeletConfigurationAuthenticationWebhook(dict):
-    def __init__(__self__, *,
-                 enabled: bool):
-        """
-        :param bool enabled: TODO
-        """
-        pulumi.set(__self__, "enabled", enabled)
-
-    @property
-    @pulumi.getter
-    def enabled(self) -> bool:
-        """
-        TODO
-        """
-        return pulumi.get(self, "enabled")
-
-
-@pulumi.output_type
-class KubeletConfigurationAuthenticationx509(dict):
-    @staticmethod
-    def __key_warning(key: str):
-        suggest = None
-        if key == "clientCAFile":
-            suggest = "client_ca_file"
-
-        if suggest:
-            pulumi.log.warn(f"Key '{key}' not found in KubeletConfigurationAuthenticationx509. Access the value via the '{suggest}' property getter instead.")
-
-    def __getitem__(self, key: str) -> Any:
-        KubeletConfigurationAuthenticationx509.__key_warning(key)
-        return super().__getitem__(key)
-
-    def get(self, key: str, default = None) -> Any:
-        KubeletConfigurationAuthenticationx509.__key_warning(key)
-        return super().get(key, default)
-
-    def __init__(__self__, *,
-                 client_ca_file: str):
-        """
-        :param str client_ca_file: TODO
-        """
-        pulumi.set(__self__, "client_ca_file", client_ca_file)
-
-    @property
-    @pulumi.getter(name="clientCAFile")
-    def client_ca_file(self) -> str:
-        """
-        TODO
-        """
-        return pulumi.get(self, "client_ca_file")
-
-
-@pulumi.output_type
-class KubeletConfigurationAuthorization(dict):
-    def __init__(__self__, *,
-                 mode: str):
-        pulumi.set(__self__, "mode", mode)
-
-    @property
-    @pulumi.getter
-    def mode(self) -> str:
-        return pulumi.get(self, "mode")
-
-
-@pulumi.output_type
 class PodManifest(dict):
     """
     Pod is a collection of containers that can run on a host. This resource is created by clients and scheduled onto hosts.
 
     This resource waits until its status is ready before registering success
     for create/update, and populating output properties from the current state of the resource.
     The following conditions are used to determine whether the resource creation has
@@ -1158,31 +854,21 @@
 
 
 @pulumi.output_type
 class User(dict):
     def __init__(__self__, *,
                  client_certificate_data: str,
                  client_key_data: str):
-        """
-        :param str client_certificate_data: TODO
-        :param str client_key_data: TODO
-        """
         pulumi.set(__self__, "client_certificate_data", client_certificate_data)
         pulumi.set(__self__, "client_key_data", client_key_data)
 
     @property
     @pulumi.getter(name="clientCertificateData")
     def client_certificate_data(self) -> str:
-        """
-        TODO
-        """
         return pulumi.get(self, "client_certificate_data")
 
     @property
     @pulumi.getter(name="clientKeyData")
     def client_key_data(self) -> str:
-        """
-        TODO
-        """
         return pulumi.get(self, "client_key_data")
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/provider.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 from .file import *
 from .kube_api_server_install import *
 from .kube_controller_manager_install import *
 from .kube_proxy_install import *
 from .kube_scheduler_install import *
 from .kubectl_install import *
 from .kubelet_install import *
-from .kubelet_service import *
 from .provision_etcd import *
 from .runc_install import *
 from .start_etcd import *
 from .static_pod import *
 from .systemd_service import *
 from ._inputs import *
 from . import outputs
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/_inputs.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,14 @@
     'ContainerdCriPluginConfigurationCniArgs',
     'ContainerdCriPluginConfigurationContainerdRuncOptionsArgs',
     'ContainerdCriPluginConfigurationContainerdRuncArgs',
     'ContainerdCriPluginConfigurationContainerdArgs',
     'ContainerdCriPluginConfigurationArgs',
     'EtcdConfigurationPropsArgs',
     'EtcdNodeArgs',
-    'KubeletConfigurationPropsArgs',
     'SystemdInstallSectionArgs',
     'SystemdServiceSectionArgs',
     'SystemdUnitSectionArgs',
 ]
 
 @pulumi.input_type
 class CniBridgeIpamArgs:
@@ -443,97 +442,14 @@
 
     @architecture.setter
     def architecture(self, value: Optional[pulumi.Input['Architecture']]):
         pulumi.set(self, "architecture", value)
 
 
 @pulumi.input_type
-class KubeletConfigurationPropsArgs:
-    def __init__(__self__, *,
-                 configuration_file_path: pulumi.Input[str],
-                 kubeconfig_path: pulumi.Input[str],
-                 kubelet_path: pulumi.Input[str],
-                 register_node: pulumi.Input[bool],
-                 v: pulumi.Input[int]):
-        """
-        Props for resources that consume kubelet configuration.
-        :param pulumi.Input[str] configuration_file_path: Path to the kubelet configuration.
-        :param pulumi.Input[str] kubeconfig_path: Path to the kubeconfig the kubelet will use
-        :param pulumi.Input[str] kubelet_path: Path to the kubelet binary.
-        :param pulumi.Input[bool] register_node: Whether to register the node. Defaults to `true`.
-        :param pulumi.Input[int] v: Verbosity. Defaults to `2`.
-        """
-        pulumi.set(__self__, "configuration_file_path", configuration_file_path)
-        pulumi.set(__self__, "kubeconfig_path", kubeconfig_path)
-        pulumi.set(__self__, "kubelet_path", kubelet_path)
-        pulumi.set(__self__, "register_node", register_node)
-        pulumi.set(__self__, "v", v)
-
-    @property
-    @pulumi.getter(name="configurationFilePath")
-    def configuration_file_path(self) -> pulumi.Input[str]:
-        """
-        Path to the kubelet configuration.
-        """
-        return pulumi.get(self, "configuration_file_path")
-
-    @configuration_file_path.setter
-    def configuration_file_path(self, value: pulumi.Input[str]):
-        pulumi.set(self, "configuration_file_path", value)
-
-    @property
-    @pulumi.getter(name="kubeconfigPath")
-    def kubeconfig_path(self) -> pulumi.Input[str]:
-        """
-        Path to the kubeconfig the kubelet will use
-        """
-        return pulumi.get(self, "kubeconfig_path")
-
-    @kubeconfig_path.setter
-    def kubeconfig_path(self, value: pulumi.Input[str]):
-        pulumi.set(self, "kubeconfig_path", value)
-
-    @property
-    @pulumi.getter(name="kubeletPath")
-    def kubelet_path(self) -> pulumi.Input[str]:
-        """
-        Path to the kubelet binary.
-        """
-        return pulumi.get(self, "kubelet_path")
-
-    @kubelet_path.setter
-    def kubelet_path(self, value: pulumi.Input[str]):
-        pulumi.set(self, "kubelet_path", value)
-
-    @property
-    @pulumi.getter(name="registerNode")
-    def register_node(self) -> pulumi.Input[bool]:
-        """
-        Whether to register the node. Defaults to `true`.
-        """
-        return pulumi.get(self, "register_node")
-
-    @register_node.setter
-    def register_node(self, value: pulumi.Input[bool]):
-        pulumi.set(self, "register_node", value)
-
-    @property
-    @pulumi.getter
-    def v(self) -> pulumi.Input[int]:
-        """
-        Verbosity. Defaults to `2`.
-        """
-        return pulumi.get(self, "v")
-
-    @v.setter
-    def v(self, value: pulumi.Input[int]):
-        pulumi.set(self, "v", value)
-
-
-@pulumi.input_type
 class SystemdInstallSectionArgs:
     def __init__(__self__, *,
                  wanted_by: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         https://www.freedesktop.org/software/systemd/man/latest/systemd.unit.html#%5BInstall%5D%20Section%20Options
         :param pulumi.Input[Sequence[pulumi.Input[str]]] wanted_by: A symbolic link is created in the .wants/, .requires/, or .upholds/ directory of each of the listed units when this unit is installed by systemctl enable.
         """
@@ -640,75 +556,43 @@
     def type(self, value: Optional[pulumi.Input['SystemdServiceType']]):
         pulumi.set(self, "type", value)
 
 
 @pulumi.input_type
 class SystemdUnitSectionArgs:
     def __init__(__self__, *,
-                 after: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 before: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  binds_to: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  documentation: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  requires: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  requisite: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  wants: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         https://www.freedesktop.org/software/systemd/man/latest/systemd.unit.html#
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] after: Those two settings configure ordering dependencies between units.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] before: Those two settings configure ordering dependencies between units.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] binds_to: Configures requirement dependencies, very similar in style to Requires=.
         :param pulumi.Input[str] description: A short human readable title of the unit.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] documentation: A space-separated list of URIs referencing documentation for this unit or its configuration.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] requires: Similar to Wants=, but declares a stronger requirement dependency.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] requisite: Similar to Requires=. However, if the units listed here are not started already, they will not be started and the starting of this unit will fail immediately.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] wants: Configures (weak) requirement dependencies on other units.
         """
-        if after is not None:
-            pulumi.set(__self__, "after", after)
-        if before is not None:
-            pulumi.set(__self__, "before", before)
         if binds_to is not None:
             pulumi.set(__self__, "binds_to", binds_to)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if documentation is not None:
             pulumi.set(__self__, "documentation", documentation)
         if requires is not None:
             pulumi.set(__self__, "requires", requires)
         if requisite is not None:
             pulumi.set(__self__, "requisite", requisite)
         if wants is not None:
             pulumi.set(__self__, "wants", wants)
 
     @property
-    @pulumi.getter
-    def after(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        """
-        Those two settings configure ordering dependencies between units.
-        """
-        return pulumi.get(self, "after")
-
-    @after.setter
-    def after(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "after", value)
-
-    @property
-    @pulumi.getter
-    def before(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        """
-        Those two settings configure ordering dependencies between units.
-        """
-        return pulumi.get(self, "before")
-
-    @before.setter
-    def before(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "before", value)
-
-    @property
     @pulumi.getter(name="bindsTo")
     def binds_to(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         Configures requirement dependencies, very similar in style to Requires=.
         """
         return pulumi.get(self, "binds_to")
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/cni_bridge_plugin_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/cni_bridge_plugin_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/cni_loopback_plugin_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/cni_loopback_plugin_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/cni_plugin_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/cni_plugin_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/containerd_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/containerd_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/containerd_install.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/containerd_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/crictl_install.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/crictl_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/download.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/download.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,48 +4,49 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
-from . import outputs
 from .. import tls as _tls
 from ._enums import *
-from ._inputs import *
 from .etcd_configuration import EtcdConfiguration
 from .etcd_install import EtcdInstall
-from .etcd_service import EtcdService
 from .start_etcd import StartEtcd
+from .systemd_service import SystemdService
 import pulumi_command
 
-__all__ = ['EtcdClusterArgs', 'EtcdCluster']
+__all__ = ['ProvisionEtcdArgs', 'ProvisionEtcd']
 
 @pulumi.input_type
-class EtcdClusterArgs:
+class ProvisionEtcdArgs:
     def __init__(__self__, *,
                  bundle: pulumi.Input['_tls.BundleArgs'],
-                 nodes: Mapping[str, pulumi.Input['EtcdNodeArgs']],
+                 connection: pulumi.Input['pulumi_command.remote.ConnectionArgs'],
+                 internal_ip: pulumi.Input[str],
                  architecture: Optional[pulumi.Input['Architecture']] = None,
                  binary_directory: Optional[pulumi.Input[str]] = None,
                  configuration_directory: Optional[pulumi.Input[str]] = None,
                  data_directory: Optional[pulumi.Input[str]] = None,
                  version: Optional[pulumi.Input[str]] = None):
         """
-        The set of arguments for constructing a EtcdCluster resource.
+        The set of arguments for constructing a ProvisionEtcd resource.
         :param pulumi.Input['_tls.BundleArgs'] bundle: The TLS bundle.
-        :param Mapping[str, pulumi.Input['EtcdNodeArgs']] nodes: Etcd node configuration. The key should be a name used to identify the node.
+        :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: The parameters with which to connect to the remote host.
+        :param pulumi.Input[str] internal_ip: The internal IP of the etcd node
         :param pulumi.Input['Architecture'] architecture: TODO
         :param pulumi.Input[str] binary_directory: TODO
         :param pulumi.Input[str] configuration_directory: The directory to use for etcd configuration.
         :param pulumi.Input[str] data_directory: The directory to use for etcd data.
         :param pulumi.Input[str] version: The version to install.
         """
         pulumi.set(__self__, "bundle", bundle)
-        pulumi.set(__self__, "nodes", nodes)
+        pulumi.set(__self__, "connection", connection)
+        pulumi.set(__self__, "internal_ip", internal_ip)
         if architecture is not None:
             pulumi.set(__self__, "architecture", architecture)
         if binary_directory is not None:
             pulumi.set(__self__, "binary_directory", binary_directory)
         if configuration_directory is not None:
             pulumi.set(__self__, "configuration_directory", configuration_directory)
         if data_directory is not None:
@@ -63,23 +64,35 @@
 
     @bundle.setter
     def bundle(self, value: pulumi.Input['_tls.BundleArgs']):
         pulumi.set(self, "bundle", value)
 
     @property
     @pulumi.getter
-    def nodes(self) -> Mapping[str, pulumi.Input['EtcdNodeArgs']]:
+    def connection(self) -> pulumi.Input['pulumi_command.remote.ConnectionArgs']:
         """
-        Etcd node configuration. The key should be a name used to identify the node.
+        The parameters with which to connect to the remote host.
         """
-        return pulumi.get(self, "nodes")
+        return pulumi.get(self, "connection")
 
-    @nodes.setter
-    def nodes(self, value: Mapping[str, pulumi.Input['EtcdNodeArgs']]):
-        pulumi.set(self, "nodes", value)
+    @connection.setter
+    def connection(self, value: pulumi.Input['pulumi_command.remote.ConnectionArgs']):
+        pulumi.set(self, "connection", value)
+
+    @property
+    @pulumi.getter(name="internalIp")
+    def internal_ip(self) -> pulumi.Input[str]:
+        """
+        The internal IP of the etcd node
+        """
+        return pulumi.get(self, "internal_ip")
+
+    @internal_ip.setter
+    def internal_ip(self, value: pulumi.Input[str]):
+        pulumi.set(self, "internal_ip", value)
 
     @property
     @pulumi.getter
     def architecture(self) -> Optional[pulumi.Input['Architecture']]:
         """
         TODO
         """
@@ -134,99 +147,105 @@
         return pulumi.get(self, "version")
 
     @version.setter
     def version(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "version", value)
 
 
-class EtcdCluster(pulumi.ComponentResource):
+class ProvisionEtcd(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  architecture: Optional[pulumi.Input['Architecture']] = None,
                  binary_directory: Optional[pulumi.Input[str]] = None,
                  bundle: Optional[pulumi.Input[pulumi.InputType['_tls.BundleArgs']]] = None,
                  configuration_directory: Optional[pulumi.Input[str]] = None,
+                 connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
                  data_directory: Optional[pulumi.Input[str]] = None,
-                 nodes: Optional[Mapping[str, pulumi.Input[pulumi.InputType['EtcdNodeArgs']]]] = None,
+                 internal_ip: Optional[pulumi.Input[str]] = None,
                  version: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Creates an etcd cluster from one or more remote systems.
+        Starts etcd on a remote system.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input['Architecture'] architecture: TODO
         :param pulumi.Input[str] binary_directory: TODO
         :param pulumi.Input[pulumi.InputType['_tls.BundleArgs']] bundle: The TLS bundle.
         :param pulumi.Input[str] configuration_directory: The directory to use for etcd configuration.
+        :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: The parameters with which to connect to the remote host.
         :param pulumi.Input[str] data_directory: The directory to use for etcd data.
-        :param Mapping[str, pulumi.Input[pulumi.InputType['EtcdNodeArgs']]] nodes: Etcd node configuration. The key should be a name used to identify the node.
+        :param pulumi.Input[str] internal_ip: The internal IP of the etcd node
         :param pulumi.Input[str] version: The version to install.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: EtcdClusterArgs,
+                 args: ProvisionEtcdArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Creates an etcd cluster from one or more remote systems.
+        Starts etcd on a remote system.
 
         :param str resource_name: The name of the resource.
-        :param EtcdClusterArgs args: The arguments to use to populate this resource's properties.
+        :param ProvisionEtcdArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(EtcdClusterArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(ProvisionEtcdArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  architecture: Optional[pulumi.Input['Architecture']] = None,
                  binary_directory: Optional[pulumi.Input[str]] = None,
                  bundle: Optional[pulumi.Input[pulumi.InputType['_tls.BundleArgs']]] = None,
                  configuration_directory: Optional[pulumi.Input[str]] = None,
+                 connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
                  data_directory: Optional[pulumi.Input[str]] = None,
-                 nodes: Optional[Mapping[str, pulumi.Input[pulumi.InputType['EtcdNodeArgs']]]] = None,
+                 internal_ip: Optional[pulumi.Input[str]] = None,
                  version: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = EtcdClusterArgs.__new__(EtcdClusterArgs)
+            __props__ = ProvisionEtcdArgs.__new__(ProvisionEtcdArgs)
 
             __props__.__dict__["architecture"] = architecture
             __props__.__dict__["binary_directory"] = binary_directory
             if bundle is None and not opts.urn:
                 raise TypeError("Missing required property 'bundle'")
             __props__.__dict__["bundle"] = bundle
             __props__.__dict__["configuration_directory"] = configuration_directory
+            if connection is None and not opts.urn:
+                raise TypeError("Missing required property 'connection'")
+            __props__.__dict__["connection"] = connection
             __props__.__dict__["data_directory"] = data_directory
-            if nodes is None and not opts.urn:
-                raise TypeError("Missing required property 'nodes'")
-            __props__.__dict__["nodes"] = nodes
+            if internal_ip is None and not opts.urn:
+                raise TypeError("Missing required property 'internal_ip'")
+            __props__.__dict__["internal_ip"] = internal_ip
             __props__.__dict__["version"] = version
             __props__.__dict__["configuration"] = None
             __props__.__dict__["install"] = None
             __props__.__dict__["service"] = None
             __props__.__dict__["start"] = None
-        super(EtcdCluster, __self__).__init__(
-            'kubernetes-the-hard-way:remote:EtcdCluster',
+        super(ProvisionEtcd, __self__).__init__(
+            'kubernetes-the-hard-way:remote:ProvisionEtcd',
             resource_name,
             __props__,
             opts,
             remote=True)
 
     @property
     @pulumi.getter
@@ -250,65 +269,73 @@
         """
         The TLS bundle.
         """
         return pulumi.get(self, "bundle")
 
     @property
     @pulumi.getter
-    def configuration(self) -> pulumi.Output[Mapping[str, 'EtcdConfiguration']]:
+    def configuration(self) -> pulumi.Output['EtcdConfiguration']:
         """
-        Map of node name to etcd configuration.
+        Etcd configuration.
         """
         return pulumi.get(self, "configuration")
 
     @property
     @pulumi.getter(name="configurationDirectory")
     def configuration_directory(self) -> pulumi.Output[Optional[str]]:
         """
         The directory to use for etcd configuration.
         """
         return pulumi.get(self, "configuration_directory")
 
     @property
+    @pulumi.getter
+    def connection(self) -> pulumi.Output['pulumi_command.remote.outputs.Connection']:
+        """
+        The parameters with which to connect to the remote host.
+        """
+        return pulumi.get(self, "connection")
+
+    @property
     @pulumi.getter(name="dataDirectory")
     def data_directory(self) -> pulumi.Output[Optional[str]]:
         """
         The directory to use for etcd data.
         """
         return pulumi.get(self, "data_directory")
 
     @property
     @pulumi.getter
-    def install(self) -> pulumi.Output[Mapping[str, 'EtcdInstall']]:
+    def install(self) -> pulumi.Output['EtcdInstall']:
         """
-        Map of node name to etcd install.
+        Install etcd.
         """
         return pulumi.get(self, "install")
 
     @property
-    @pulumi.getter
-    def nodes(self) -> pulumi.Output[Mapping[str, 'outputs.EtcdNode']]:
+    @pulumi.getter(name="internalIp")
+    def internal_ip(self) -> pulumi.Output[str]:
         """
-        Etcd node configuration. The key should be a name used to identify the node.
+        The internal IP of the etcd node
         """
-        return pulumi.get(self, "nodes")
+        return pulumi.get(self, "internal_ip")
 
     @property
     @pulumi.getter
-    def service(self) -> pulumi.Output[Mapping[str, 'EtcdService']]:
+    def service(self) -> pulumi.Output['SystemdService']:
         """
-        Map of node name to etcd systemd service.
+        Systemd service.
         """
         return pulumi.get(self, "service")
 
     @property
     @pulumi.getter
-    def start(self) -> pulumi.Output[Mapping[str, 'StartEtcd']]:
+    def start(self) -> pulumi.Output['StartEtcd']:
         """
-        Map of node name to etcd start commands.
+        Start etcd
         """
         return pulumi.get(self, "start")
 
     @property
     @pulumi.getter
     def version(self) -> pulumi.Output[Optional[str]]:
         """
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/etcd_install.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/etcd_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/etcd_service.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/etcd_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/file.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/file.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/kubelet_service.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/tee.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,367 +7,345 @@
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 from ._enums import *
 from ._inputs import *
-from .systemd_service import SystemdService
 import pulumi_command
 
-__all__ = ['KubeletServiceArgs', 'KubeletService']
+__all__ = ['TeeArgs', 'Tee']
 
 @pulumi.input_type
-class KubeletServiceArgs:
+class TeeArgs:
     def __init__(__self__, *,
-                 after: pulumi.Input[Sequence[pulumi.Input[str]]],
-                 configuration: pulumi.Input['KubeletConfigurationPropsArgs'],
                  connection: pulumi.Input['pulumi_command.remote.ConnectionArgs'],
-                 requires: pulumi.Input[Sequence[pulumi.Input[str]]],
-                 description: Optional[pulumi.Input[str]] = None,
-                 directory: Optional[pulumi.Input[str]] = None,
-                 documentation: Optional[pulumi.Input[str]] = None,
-                 restart: Optional[pulumi.Input['SystemdServiceRestart']] = None,
-                 restart_sec: Optional[pulumi.Input[str]] = None,
-                 wanted_by: Optional[pulumi.Input[str]] = None):
-        """
-        The set of arguments for constructing a KubeletService resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] after: Waits for any units defined here.
-        :param pulumi.Input['KubeletConfigurationPropsArgs'] configuration: Kubelet configuration.
-        :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: The parameters with which to connect to the remote host.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] requires: Requires any units defined here.
-        :param pulumi.Input[str] description: Optional systemd unit description.
-        :param pulumi.Input[str] directory: The location to create the service file.
-        :param pulumi.Input[str] documentation: Optional systemd unit documentation
-        :param pulumi.Input['SystemdServiceRestart'] restart: Optionally override the systemd service restart behaviour. Defaults to `on-failure`.
-        :param pulumi.Input[str] restart_sec: Optionally override the systemd service RestartSec. Defaults to `5`.
-        :param pulumi.Input[str] wanted_by: Optionally override the systemd service wanted-by. Defaults to `multi-user.target`.
+                 binary_path: Optional[pulumi.Input[str]] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']]] = None,
+                 environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
+                 stdin: Optional[pulumi.Input[str]] = None,
+                 triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']]] = None):
+        """
+        The set of arguments for constructing a Tee resource.
+        :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: Connection details for the remote system
+        :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
+        :param Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']] create: The command to run on create.
+        :param Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+               and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
+               Command resource from previous create or update steps.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
+        :param pulumi.Input[str] stdin: TODO
+        :param pulumi.Input[Sequence[Any]] triggers: TODO
+        :param Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']] update: The command to run on update, if empty, create will 
+               run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
+               are set to the stdout and stderr properties of the Command resource from previous 
+               create or update steps.
         """
-        pulumi.set(__self__, "after", after)
-        pulumi.set(__self__, "configuration", configuration)
         pulumi.set(__self__, "connection", connection)
-        pulumi.set(__self__, "requires", requires)
-        if description is not None:
-            pulumi.set(__self__, "description", description)
-        if directory is not None:
-            pulumi.set(__self__, "directory", directory)
-        if documentation is not None:
-            pulumi.set(__self__, "documentation", documentation)
-        if restart is not None:
-            pulumi.set(__self__, "restart", restart)
-        if restart_sec is not None:
-            pulumi.set(__self__, "restart_sec", restart_sec)
-        if wanted_by is not None:
-            pulumi.set(__self__, "wanted_by", wanted_by)
-
-    @property
-    @pulumi.getter
-    def after(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
-        """
-        Waits for any units defined here.
-        """
-        return pulumi.get(self, "after")
-
-    @after.setter
-    def after(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
-        pulumi.set(self, "after", value)
-
-    @property
-    @pulumi.getter
-    def configuration(self) -> pulumi.Input['KubeletConfigurationPropsArgs']:
-        """
-        Kubelet configuration.
-        """
-        return pulumi.get(self, "configuration")
-
-    @configuration.setter
-    def configuration(self, value: pulumi.Input['KubeletConfigurationPropsArgs']):
-        pulumi.set(self, "configuration", value)
+        if binary_path is not None:
+            pulumi.set(__self__, "binary_path", binary_path)
+        if create is not None:
+            pulumi.set(__self__, "create", create)
+        if delete is not None:
+            pulumi.set(__self__, "delete", delete)
+        if environment is not None:
+            pulumi.set(__self__, "environment", environment)
+        if stdin is not None:
+            pulumi.set(__self__, "stdin", stdin)
+        if triggers is not None:
+            pulumi.set(__self__, "triggers", triggers)
+        if update is not None:
+            pulumi.set(__self__, "update", update)
 
     @property
     @pulumi.getter
     def connection(self) -> pulumi.Input['pulumi_command.remote.ConnectionArgs']:
         """
-        The parameters with which to connect to the remote host.
+        Connection details for the remote system
         """
         return pulumi.get(self, "connection")
 
     @connection.setter
     def connection(self, value: pulumi.Input['pulumi_command.remote.ConnectionArgs']):
         pulumi.set(self, "connection", value)
 
     @property
-    @pulumi.getter
-    def requires(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
+    @pulumi.getter(name="binaryPath")
+    def binary_path(self) -> Optional[pulumi.Input[str]]:
         """
-        Requires any units defined here.
+        Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
         """
-        return pulumi.get(self, "requires")
+        return pulumi.get(self, "binary_path")
 
-    @requires.setter
-    def requires(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
-        pulumi.set(self, "requires", value)
+    @binary_path.setter
+    def binary_path(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "binary_path", value)
 
     @property
     @pulumi.getter
-    def description(self) -> Optional[pulumi.Input[str]]:
+    def create(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']]]:
         """
-        Optional systemd unit description.
+        The command to run on create.
         """
-        return pulumi.get(self, "description")
+        return pulumi.get(self, "create")
 
-    @description.setter
-    def description(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "description", value)
+    @create.setter
+    def create(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']]]):
+        pulumi.set(self, "create", value)
 
     @property
     @pulumi.getter
-    def directory(self) -> Optional[pulumi.Input[str]]:
+    def delete(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']]]:
         """
-        The location to create the service file.
+        The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+        and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
+        Command resource from previous create or update steps.
         """
-        return pulumi.get(self, "directory")
+        return pulumi.get(self, "delete")
 
-    @directory.setter
-    def directory(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "directory", value)
+    @delete.setter
+    def delete(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']]]):
+        pulumi.set(self, "delete", value)
 
     @property
     @pulumi.getter
-    def documentation(self) -> Optional[pulumi.Input[str]]:
+    def environment(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        Optional systemd unit documentation
+        Environment variables
         """
-        return pulumi.get(self, "documentation")
+        return pulumi.get(self, "environment")
 
-    @documentation.setter
-    def documentation(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "documentation", value)
+    @environment.setter
+    def environment(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "environment", value)
 
     @property
     @pulumi.getter
-    def restart(self) -> Optional[pulumi.Input['SystemdServiceRestart']]:
+    def stdin(self) -> Optional[pulumi.Input[str]]:
         """
-        Optionally override the systemd service restart behaviour. Defaults to `on-failure`.
+        TODO
         """
-        return pulumi.get(self, "restart")
+        return pulumi.get(self, "stdin")
 
-    @restart.setter
-    def restart(self, value: Optional[pulumi.Input['SystemdServiceRestart']]):
-        pulumi.set(self, "restart", value)
+    @stdin.setter
+    def stdin(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "stdin", value)
 
     @property
-    @pulumi.getter(name="restartSec")
-    def restart_sec(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def triggers(self) -> Optional[pulumi.Input[Sequence[Any]]]:
         """
-        Optionally override the systemd service RestartSec. Defaults to `5`.
+        TODO
         """
-        return pulumi.get(self, "restart_sec")
+        return pulumi.get(self, "triggers")
 
-    @restart_sec.setter
-    def restart_sec(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "restart_sec", value)
+    @triggers.setter
+    def triggers(self, value: Optional[pulumi.Input[Sequence[Any]]]):
+        pulumi.set(self, "triggers", value)
 
     @property
-    @pulumi.getter(name="wantedBy")
-    def wanted_by(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def update(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']]]:
         """
-        Optionally override the systemd service wanted-by. Defaults to `multi-user.target`.
+        The command to run on update, if empty, create will 
+        run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
+        are set to the stdout and stderr properties of the Command resource from previous 
+        create or update steps.
         """
-        return pulumi.get(self, "wanted_by")
+        return pulumi.get(self, "update")
 
-    @wanted_by.setter
-    def wanted_by(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "wanted_by", value)
+    @update.setter
+    def update(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']]]):
+        pulumi.set(self, "update", value)
 
 
-class KubeletService(pulumi.ComponentResource):
+class Tee(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 after: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 configuration: Optional[pulumi.Input[pulumi.InputType['KubeletConfigurationPropsArgs']]] = None,
+                 binary_path: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 description: Optional[pulumi.Input[str]] = None,
-                 directory: Optional[pulumi.Input[str]] = None,
-                 documentation: Optional[pulumi.Input[str]] = None,
-                 requires: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 restart: Optional[pulumi.Input['SystemdServiceRestart']] = None,
-                 restart_sec: Optional[pulumi.Input[str]] = None,
-                 wanted_by: Optional[pulumi.Input[str]] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['TeeOptsArgs']]]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['TeeOptsArgs']]]] = None,
+                 environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
+                 stdin: Optional[pulumi.Input[str]] = None,
+                 triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['TeeOptsArgs']]]] = None,
                  __props__=None):
         """
-        Kubelet systemd service file. Will likely get replaced with a static function when https://github.com/pulumi/pulumi/issues/7583 gets resolved.
+        Abstraction over the `rm` utility on a remote system.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] after: Waits for any units defined here.
-        :param pulumi.Input[pulumi.InputType['KubeletConfigurationPropsArgs']] configuration: Kubelet configuration.
-        :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: The parameters with which to connect to the remote host.
-        :param pulumi.Input[str] description: Optional systemd unit description.
-        :param pulumi.Input[str] directory: The location to create the service file.
-        :param pulumi.Input[str] documentation: Optional systemd unit documentation
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] requires: Requires any units defined here.
-        :param pulumi.Input['SystemdServiceRestart'] restart: Optionally override the systemd service restart behaviour. Defaults to `on-failure`.
-        :param pulumi.Input[str] restart_sec: Optionally override the systemd service RestartSec. Defaults to `5`.
-        :param pulumi.Input[str] wanted_by: Optionally override the systemd service wanted-by. Defaults to `multi-user.target`.
+        :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
+        :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: Connection details for the remote system
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['TeeOptsArgs']]] create: The command to run on create.
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['TeeOptsArgs']]] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+               and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
+               Command resource from previous create or update steps.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
+        :param pulumi.Input[str] stdin: TODO
+        :param pulumi.Input[Sequence[Any]] triggers: TODO
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['TeeOptsArgs']]] update: The command to run on update, if empty, create will 
+               run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
+               are set to the stdout and stderr properties of the Command resource from previous 
+               create or update steps.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: KubeletServiceArgs,
+                 args: TeeArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Kubelet systemd service file. Will likely get replaced with a static function when https://github.com/pulumi/pulumi/issues/7583 gets resolved.
+        Abstraction over the `rm` utility on a remote system.
 
         :param str resource_name: The name of the resource.
-        :param KubeletServiceArgs args: The arguments to use to populate this resource's properties.
+        :param TeeArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(KubeletServiceArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(TeeArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 after: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 configuration: Optional[pulumi.Input[pulumi.InputType['KubeletConfigurationPropsArgs']]] = None,
+                 binary_path: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 description: Optional[pulumi.Input[str]] = None,
-                 directory: Optional[pulumi.Input[str]] = None,
-                 documentation: Optional[pulumi.Input[str]] = None,
-                 requires: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 restart: Optional[pulumi.Input['SystemdServiceRestart']] = None,
-                 restart_sec: Optional[pulumi.Input[str]] = None,
-                 wanted_by: Optional[pulumi.Input[str]] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['TeeOptsArgs']]]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['TeeOptsArgs']]]] = None,
+                 environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
+                 stdin: Optional[pulumi.Input[str]] = None,
+                 triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['TeeOptsArgs']]]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = KubeletServiceArgs.__new__(KubeletServiceArgs)
+            __props__ = TeeArgs.__new__(TeeArgs)
 
-            if after is None and not opts.urn:
-                raise TypeError("Missing required property 'after'")
-            __props__.__dict__["after"] = after
-            if configuration is None and not opts.urn:
-                raise TypeError("Missing required property 'configuration'")
-            __props__.__dict__["configuration"] = configuration
+            __props__.__dict__["binary_path"] = binary_path
             if connection is None and not opts.urn:
                 raise TypeError("Missing required property 'connection'")
             __props__.__dict__["connection"] = connection
-            __props__.__dict__["description"] = description
-            __props__.__dict__["directory"] = directory
-            __props__.__dict__["documentation"] = documentation
-            if requires is None and not opts.urn:
-                raise TypeError("Missing required property 'requires'")
-            __props__.__dict__["requires"] = requires
-            __props__.__dict__["restart"] = restart
-            __props__.__dict__["restart_sec"] = restart_sec
-            __props__.__dict__["wanted_by"] = wanted_by
-            __props__.__dict__["service"] = None
-        super(KubeletService, __self__).__init__(
-            'kubernetes-the-hard-way:remote:KubeletService',
+            __props__.__dict__["create"] = create
+            __props__.__dict__["delete"] = delete
+            __props__.__dict__["environment"] = environment
+            __props__.__dict__["stdin"] = stdin
+            __props__.__dict__["triggers"] = triggers
+            __props__.__dict__["update"] = update
+            __props__.__dict__["command"] = None
+            __props__.__dict__["stderr"] = None
+            __props__.__dict__["stdout"] = None
+        super(Tee, __self__).__init__(
+            'kubernetes-the-hard-way:tools:Tee',
             resource_name,
             __props__,
             opts,
             remote=True)
 
     @property
-    @pulumi.getter
-    def after(self) -> pulumi.Output[Sequence[str]]:
+    @pulumi.getter(name="binaryPath")
+    def binary_path(self) -> pulumi.Output[str]:
         """
-        Waits for any units defined here.
+        Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
         """
-        return pulumi.get(self, "after")
+        return pulumi.get(self, "binary_path")
 
     @property
     @pulumi.getter
-    def configuration(self) -> pulumi.Output['outputs.KubeletConfigurationProps']:
+    def command(self) -> pulumi.Output['pulumi_command.remote.Command']:
         """
-        Kubelet configuration.
+        The underlying command
         """
-        return pulumi.get(self, "configuration")
+        return pulumi.get(self, "command")
 
     @property
     @pulumi.getter
     def connection(self) -> pulumi.Output['pulumi_command.remote.outputs.Connection']:
         """
-        The parameters with which to connect to the remote host.
+        Connection details for the remote system
         """
         return pulumi.get(self, "connection")
 
     @property
     @pulumi.getter
-    def description(self) -> pulumi.Output[Optional[str]]:
+    def create(self) -> pulumi.Output[Optional[Any]]:
         """
-        Optional systemd unit description.
+        The command to run on create.
         """
-        return pulumi.get(self, "description")
+        return pulumi.get(self, "create")
 
     @property
     @pulumi.getter
-    def directory(self) -> pulumi.Output[Optional[str]]:
+    def delete(self) -> pulumi.Output[Optional[Any]]:
         """
-        The location to create the service file.
+        The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+        and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
+        Command resource from previous create or update steps.
         """
-        return pulumi.get(self, "directory")
+        return pulumi.get(self, "delete")
 
     @property
     @pulumi.getter
-    def documentation(self) -> pulumi.Output[Optional[str]]:
+    def environment(self) -> pulumi.Output[Mapping[str, str]]:
         """
-        Optional systemd unit documentation
+        Environment variables
         """
-        return pulumi.get(self, "documentation")
+        return pulumi.get(self, "environment")
 
     @property
     @pulumi.getter
-    def requires(self) -> pulumi.Output[Sequence[str]]:
+    def stderr(self) -> pulumi.Output[str]:
         """
-        Requires any units defined here.
+        TODO
         """
-        return pulumi.get(self, "requires")
+        return pulumi.get(self, "stderr")
 
     @property
     @pulumi.getter
-    def restart(self) -> pulumi.Output[Optional['SystemdServiceRestart']]:
+    def stdin(self) -> pulumi.Output[Optional[str]]:
         """
-        Optionally override the systemd service restart behaviour. Defaults to `on-failure`.
+        TODO
         """
-        return pulumi.get(self, "restart")
+        return pulumi.get(self, "stdin")
 
     @property
-    @pulumi.getter(name="restartSec")
-    def restart_sec(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter
+    def stdout(self) -> pulumi.Output[str]:
         """
-        Optionally override the systemd service RestartSec. Defaults to `5`.
+        TODO
         """
-        return pulumi.get(self, "restart_sec")
+        return pulumi.get(self, "stdout")
 
     @property
     @pulumi.getter
-    def service(self) -> pulumi.Output['SystemdService']:
+    def triggers(self) -> pulumi.Output[Sequence[Any]]:
         """
-        The remote systemd service.
+        TODO
         """
-        return pulumi.get(self, "service")
+        return pulumi.get(self, "triggers")
 
     @property
-    @pulumi.getter(name="wantedBy")
-    def wanted_by(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter
+    def update(self) -> pulumi.Output[Optional[Any]]:
         """
-        Optionally override the systemd service wanted-by. Defaults to `multi-user.target`.
+        The command to run on update, if empty, create will 
+        run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
+        are set to the stdout and stderr properties of the Command resource from previous 
+        create or update steps.
         """
-        return pulumi.get(self, "wanted_by")
+        return pulumi.get(self, "update")
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/outputs.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     'ContainerdCriPluginConfiguration',
     'ContainerdCriPluginConfigurationCni',
     'ContainerdCriPluginConfigurationContainerd',
     'ContainerdCriPluginConfigurationContainerdRunc',
     'ContainerdCriPluginConfigurationContainerdRuncOptions',
     'EtcdConfigurationProps',
     'EtcdNode',
-    'KubeletConfigurationProps',
     'SystemdInstallSection',
     'SystemdServiceSection',
     'SystemdUnitSection',
 ]
 
 @pulumi.output_type
 class CniBridgeIpam(dict):
@@ -490,103 +489,14 @@
         """
         The CPU architecture of the node.
         """
         return pulumi.get(self, "architecture")
 
 
 @pulumi.output_type
-class KubeletConfigurationProps(dict):
-    """
-    Props for resources that consume kubelet configuration.
-    """
-    @staticmethod
-    def __key_warning(key: str):
-        suggest = None
-        if key == "configurationFilePath":
-            suggest = "configuration_file_path"
-        elif key == "kubeconfigPath":
-            suggest = "kubeconfig_path"
-        elif key == "kubeletPath":
-            suggest = "kubelet_path"
-        elif key == "registerNode":
-            suggest = "register_node"
-
-        if suggest:
-            pulumi.log.warn(f"Key '{key}' not found in KubeletConfigurationProps. Access the value via the '{suggest}' property getter instead.")
-
-    def __getitem__(self, key: str) -> Any:
-        KubeletConfigurationProps.__key_warning(key)
-        return super().__getitem__(key)
-
-    def get(self, key: str, default = None) -> Any:
-        KubeletConfigurationProps.__key_warning(key)
-        return super().get(key, default)
-
-    def __init__(__self__, *,
-                 configuration_file_path: str,
-                 kubeconfig_path: str,
-                 kubelet_path: str,
-                 register_node: bool,
-                 v: int):
-        """
-        Props for resources that consume kubelet configuration.
-        :param str configuration_file_path: Path to the kubelet configuration.
-        :param str kubeconfig_path: Path to the kubeconfig the kubelet will use
-        :param str kubelet_path: Path to the kubelet binary.
-        :param bool register_node: Whether to register the node. Defaults to `true`.
-        :param int v: Verbosity. Defaults to `2`.
-        """
-        pulumi.set(__self__, "configuration_file_path", configuration_file_path)
-        pulumi.set(__self__, "kubeconfig_path", kubeconfig_path)
-        pulumi.set(__self__, "kubelet_path", kubelet_path)
-        pulumi.set(__self__, "register_node", register_node)
-        pulumi.set(__self__, "v", v)
-
-    @property
-    @pulumi.getter(name="configurationFilePath")
-    def configuration_file_path(self) -> str:
-        """
-        Path to the kubelet configuration.
-        """
-        return pulumi.get(self, "configuration_file_path")
-
-    @property
-    @pulumi.getter(name="kubeconfigPath")
-    def kubeconfig_path(self) -> str:
-        """
-        Path to the kubeconfig the kubelet will use
-        """
-        return pulumi.get(self, "kubeconfig_path")
-
-    @property
-    @pulumi.getter(name="kubeletPath")
-    def kubelet_path(self) -> str:
-        """
-        Path to the kubelet binary.
-        """
-        return pulumi.get(self, "kubelet_path")
-
-    @property
-    @pulumi.getter(name="registerNode")
-    def register_node(self) -> bool:
-        """
-        Whether to register the node. Defaults to `true`.
-        """
-        return pulumi.get(self, "register_node")
-
-    @property
-    @pulumi.getter
-    def v(self) -> int:
-        """
-        Verbosity. Defaults to `2`.
-        """
-        return pulumi.get(self, "v")
-
-
-@pulumi.output_type
 class SystemdInstallSection(dict):
     """
     https://www.freedesktop.org/software/systemd/man/latest/systemd.unit.html#%5BInstall%5D%20Section%20Options
     """
     @staticmethod
     def __key_warning(key: str):
         suggest = None
@@ -733,67 +643,43 @@
         return super().__getitem__(key)
 
     def get(self, key: str, default = None) -> Any:
         SystemdUnitSection.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
-                 after: Optional[Sequence[str]] = None,
-                 before: Optional[Sequence[str]] = None,
                  binds_to: Optional[Sequence[str]] = None,
                  description: Optional[str] = None,
                  documentation: Optional[Sequence[str]] = None,
                  requires: Optional[Sequence[str]] = None,
                  requisite: Optional[Sequence[str]] = None,
                  wants: Optional[Sequence[str]] = None):
         """
         https://www.freedesktop.org/software/systemd/man/latest/systemd.unit.html#
-        :param Sequence[str] after: Those two settings configure ordering dependencies between units.
-        :param Sequence[str] before: Those two settings configure ordering dependencies between units.
         :param Sequence[str] binds_to: Configures requirement dependencies, very similar in style to Requires=.
         :param str description: A short human readable title of the unit.
         :param Sequence[str] documentation: A space-separated list of URIs referencing documentation for this unit or its configuration.
         :param Sequence[str] requires: Similar to Wants=, but declares a stronger requirement dependency.
         :param Sequence[str] requisite: Similar to Requires=. However, if the units listed here are not started already, they will not be started and the starting of this unit will fail immediately.
         :param Sequence[str] wants: Configures (weak) requirement dependencies on other units.
         """
-        if after is not None:
-            pulumi.set(__self__, "after", after)
-        if before is not None:
-            pulumi.set(__self__, "before", before)
         if binds_to is not None:
             pulumi.set(__self__, "binds_to", binds_to)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if documentation is not None:
             pulumi.set(__self__, "documentation", documentation)
         if requires is not None:
             pulumi.set(__self__, "requires", requires)
         if requisite is not None:
             pulumi.set(__self__, "requisite", requisite)
         if wants is not None:
             pulumi.set(__self__, "wants", wants)
 
     @property
-    @pulumi.getter
-    def after(self) -> Optional[Sequence[str]]:
-        """
-        Those two settings configure ordering dependencies between units.
-        """
-        return pulumi.get(self, "after")
-
-    @property
-    @pulumi.getter
-    def before(self) -> Optional[Sequence[str]]:
-        """
-        Those two settings configure ordering dependencies between units.
-        """
-        return pulumi.get(self, "before")
-
-    @property
     @pulumi.getter(name="bindsTo")
     def binds_to(self) -> Optional[Sequence[str]]:
         """
         Configures requirement dependencies, very similar in style to Requires=.
         """
         return pulumi.get(self, "binds_to")
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/systemd_service.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,342 +4,260 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
-from .. import tls as _tls
+from . import outputs
 from ._enums import *
-from .etcd_configuration import EtcdConfiguration
-from .etcd_install import EtcdInstall
-from .start_etcd import StartEtcd
-from .systemd_service import SystemdService
+from ._inputs import *
+from .file import File
 import pulumi_command
 
-__all__ = ['ProvisionEtcdArgs', 'ProvisionEtcd']
+__all__ = ['SystemdServiceArgs', 'SystemdService']
 
 @pulumi.input_type
-class ProvisionEtcdArgs:
+class SystemdServiceArgs:
     def __init__(__self__, *,
-                 bundle: pulumi.Input['_tls.BundleArgs'],
                  connection: pulumi.Input['pulumi_command.remote.ConnectionArgs'],
-                 internal_ip: pulumi.Input[str],
-                 architecture: Optional[pulumi.Input['Architecture']] = None,
-                 binary_directory: Optional[pulumi.Input[str]] = None,
-                 configuration_directory: Optional[pulumi.Input[str]] = None,
-                 data_directory: Optional[pulumi.Input[str]] = None,
-                 version: Optional[pulumi.Input[str]] = None):
+                 service: pulumi.Input['SystemdServiceSectionArgs'],
+                 directory: Optional[pulumi.Input[str]] = None,
+                 install: Optional[pulumi.Input['SystemdInstallSectionArgs']] = None,
+                 unit: Optional[pulumi.Input['SystemdUnitSectionArgs']] = None,
+                 unit_name: Optional[pulumi.Input[str]] = None):
         """
-        The set of arguments for constructing a ProvisionEtcd resource.
-        :param pulumi.Input['_tls.BundleArgs'] bundle: The TLS bundle.
+        The set of arguments for constructing a SystemdService resource.
         :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: The parameters with which to connect to the remote host.
-        :param pulumi.Input[str] internal_ip: The internal IP of the etcd node
-        :param pulumi.Input['Architecture'] architecture: TODO
-        :param pulumi.Input[str] binary_directory: TODO
-        :param pulumi.Input[str] configuration_directory: The directory to use for etcd configuration.
-        :param pulumi.Input[str] data_directory: The directory to use for etcd data.
-        :param pulumi.Input[str] version: The version to install.
+        :param pulumi.Input['SystemdServiceSectionArgs'] service: Describes the [Service] section of a systemd service file.
+        :param pulumi.Input[str] directory: The location to create the service file.
+        :param pulumi.Input['SystemdInstallSectionArgs'] install: Describes the [Install] section of a systemd service file.
+        :param pulumi.Input['SystemdUnitSectionArgs'] unit: Describes the [Unit] section of a systemd service file.
+        :param pulumi.Input[str] unit_name: Name of the systemd unit.
         """
-        pulumi.set(__self__, "bundle", bundle)
         pulumi.set(__self__, "connection", connection)
-        pulumi.set(__self__, "internal_ip", internal_ip)
-        if architecture is not None:
-            pulumi.set(__self__, "architecture", architecture)
-        if binary_directory is not None:
-            pulumi.set(__self__, "binary_directory", binary_directory)
-        if configuration_directory is not None:
-            pulumi.set(__self__, "configuration_directory", configuration_directory)
-        if data_directory is not None:
-            pulumi.set(__self__, "data_directory", data_directory)
-        if version is not None:
-            pulumi.set(__self__, "version", version)
-
-    @property
-    @pulumi.getter
-    def bundle(self) -> pulumi.Input['_tls.BundleArgs']:
-        """
-        The TLS bundle.
-        """
-        return pulumi.get(self, "bundle")
-
-    @bundle.setter
-    def bundle(self, value: pulumi.Input['_tls.BundleArgs']):
-        pulumi.set(self, "bundle", value)
+        pulumi.set(__self__, "service", service)
+        if directory is None:
+            directory = '/etc/systemd/system'
+        if directory is not None:
+            pulumi.set(__self__, "directory", directory)
+        if install is not None:
+            pulumi.set(__self__, "install", install)
+        if unit is not None:
+            pulumi.set(__self__, "unit", unit)
+        if unit_name is not None:
+            pulumi.set(__self__, "unit_name", unit_name)
 
     @property
     @pulumi.getter
     def connection(self) -> pulumi.Input['pulumi_command.remote.ConnectionArgs']:
         """
         The parameters with which to connect to the remote host.
         """
         return pulumi.get(self, "connection")
 
     @connection.setter
     def connection(self, value: pulumi.Input['pulumi_command.remote.ConnectionArgs']):
         pulumi.set(self, "connection", value)
 
     @property
-    @pulumi.getter(name="internalIp")
-    def internal_ip(self) -> pulumi.Input[str]:
-        """
-        The internal IP of the etcd node
-        """
-        return pulumi.get(self, "internal_ip")
-
-    @internal_ip.setter
-    def internal_ip(self, value: pulumi.Input[str]):
-        pulumi.set(self, "internal_ip", value)
-
-    @property
     @pulumi.getter
-    def architecture(self) -> Optional[pulumi.Input['Architecture']]:
+    def service(self) -> pulumi.Input['SystemdServiceSectionArgs']:
         """
-        TODO
+        Describes the [Service] section of a systemd service file.
         """
-        return pulumi.get(self, "architecture")
+        return pulumi.get(self, "service")
 
-    @architecture.setter
-    def architecture(self, value: Optional[pulumi.Input['Architecture']]):
-        pulumi.set(self, "architecture", value)
+    @service.setter
+    def service(self, value: pulumi.Input['SystemdServiceSectionArgs']):
+        pulumi.set(self, "service", value)
 
     @property
-    @pulumi.getter(name="binaryDirectory")
-    def binary_directory(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def directory(self) -> Optional[pulumi.Input[str]]:
         """
-        TODO
+        The location to create the service file.
         """
-        return pulumi.get(self, "binary_directory")
+        return pulumi.get(self, "directory")
 
-    @binary_directory.setter
-    def binary_directory(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "binary_directory", value)
+    @directory.setter
+    def directory(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "directory", value)
 
     @property
-    @pulumi.getter(name="configurationDirectory")
-    def configuration_directory(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def install(self) -> Optional[pulumi.Input['SystemdInstallSectionArgs']]:
         """
-        The directory to use for etcd configuration.
+        Describes the [Install] section of a systemd service file.
         """
-        return pulumi.get(self, "configuration_directory")
+        return pulumi.get(self, "install")
 
-    @configuration_directory.setter
-    def configuration_directory(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "configuration_directory", value)
+    @install.setter
+    def install(self, value: Optional[pulumi.Input['SystemdInstallSectionArgs']]):
+        pulumi.set(self, "install", value)
 
     @property
-    @pulumi.getter(name="dataDirectory")
-    def data_directory(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def unit(self) -> Optional[pulumi.Input['SystemdUnitSectionArgs']]:
         """
-        The directory to use for etcd data.
+        Describes the [Unit] section of a systemd service file.
         """
-        return pulumi.get(self, "data_directory")
+        return pulumi.get(self, "unit")
 
-    @data_directory.setter
-    def data_directory(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "data_directory", value)
+    @unit.setter
+    def unit(self, value: Optional[pulumi.Input['SystemdUnitSectionArgs']]):
+        pulumi.set(self, "unit", value)
 
     @property
-    @pulumi.getter
-    def version(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="unitName")
+    def unit_name(self) -> Optional[pulumi.Input[str]]:
         """
-        The version to install.
+        Name of the systemd unit.
         """
-        return pulumi.get(self, "version")
+        return pulumi.get(self, "unit_name")
 
-    @version.setter
-    def version(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "version", value)
+    @unit_name.setter
+    def unit_name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "unit_name", value)
 
 
-class ProvisionEtcd(pulumi.ComponentResource):
+class SystemdService(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 architecture: Optional[pulumi.Input['Architecture']] = None,
-                 binary_directory: Optional[pulumi.Input[str]] = None,
-                 bundle: Optional[pulumi.Input[pulumi.InputType['_tls.BundleArgs']]] = None,
-                 configuration_directory: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 data_directory: Optional[pulumi.Input[str]] = None,
-                 internal_ip: Optional[pulumi.Input[str]] = None,
-                 version: Optional[pulumi.Input[str]] = None,
+                 directory: Optional[pulumi.Input[str]] = None,
+                 install: Optional[pulumi.Input[pulumi.InputType['SystemdInstallSectionArgs']]] = None,
+                 service: Optional[pulumi.Input[pulumi.InputType['SystemdServiceSectionArgs']]] = None,
+                 unit: Optional[pulumi.Input[pulumi.InputType['SystemdUnitSectionArgs']]] = None,
+                 unit_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Starts etcd on a remote system.
+        A systemd service on a remote system.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input['Architecture'] architecture: TODO
-        :param pulumi.Input[str] binary_directory: TODO
-        :param pulumi.Input[pulumi.InputType['_tls.BundleArgs']] bundle: The TLS bundle.
-        :param pulumi.Input[str] configuration_directory: The directory to use for etcd configuration.
         :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: The parameters with which to connect to the remote host.
-        :param pulumi.Input[str] data_directory: The directory to use for etcd data.
-        :param pulumi.Input[str] internal_ip: The internal IP of the etcd node
-        :param pulumi.Input[str] version: The version to install.
+        :param pulumi.Input[str] directory: The location to create the service file.
+        :param pulumi.Input[pulumi.InputType['SystemdInstallSectionArgs']] install: Describes the [Install] section of a systemd service file.
+        :param pulumi.Input[pulumi.InputType['SystemdServiceSectionArgs']] service: Describes the [Service] section of a systemd service file.
+        :param pulumi.Input[pulumi.InputType['SystemdUnitSectionArgs']] unit: Describes the [Unit] section of a systemd service file.
+        :param pulumi.Input[str] unit_name: Name of the systemd unit.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: ProvisionEtcdArgs,
+                 args: SystemdServiceArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Starts etcd on a remote system.
+        A systemd service on a remote system.
 
         :param str resource_name: The name of the resource.
-        :param ProvisionEtcdArgs args: The arguments to use to populate this resource's properties.
+        :param SystemdServiceArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(ProvisionEtcdArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(SystemdServiceArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 architecture: Optional[pulumi.Input['Architecture']] = None,
-                 binary_directory: Optional[pulumi.Input[str]] = None,
-                 bundle: Optional[pulumi.Input[pulumi.InputType['_tls.BundleArgs']]] = None,
-                 configuration_directory: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 data_directory: Optional[pulumi.Input[str]] = None,
-                 internal_ip: Optional[pulumi.Input[str]] = None,
-                 version: Optional[pulumi.Input[str]] = None,
+                 directory: Optional[pulumi.Input[str]] = None,
+                 install: Optional[pulumi.Input[pulumi.InputType['SystemdInstallSectionArgs']]] = None,
+                 service: Optional[pulumi.Input[pulumi.InputType['SystemdServiceSectionArgs']]] = None,
+                 unit: Optional[pulumi.Input[pulumi.InputType['SystemdUnitSectionArgs']]] = None,
+                 unit_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = ProvisionEtcdArgs.__new__(ProvisionEtcdArgs)
+            __props__ = SystemdServiceArgs.__new__(SystemdServiceArgs)
 
-            __props__.__dict__["architecture"] = architecture
-            __props__.__dict__["binary_directory"] = binary_directory
-            if bundle is None and not opts.urn:
-                raise TypeError("Missing required property 'bundle'")
-            __props__.__dict__["bundle"] = bundle
-            __props__.__dict__["configuration_directory"] = configuration_directory
             if connection is None and not opts.urn:
                 raise TypeError("Missing required property 'connection'")
             __props__.__dict__["connection"] = connection
-            __props__.__dict__["data_directory"] = data_directory
-            if internal_ip is None and not opts.urn:
-                raise TypeError("Missing required property 'internal_ip'")
-            __props__.__dict__["internal_ip"] = internal_ip
-            __props__.__dict__["version"] = version
-            __props__.__dict__["configuration"] = None
-            __props__.__dict__["install"] = None
-            __props__.__dict__["service"] = None
-            __props__.__dict__["start"] = None
-        super(ProvisionEtcd, __self__).__init__(
-            'kubernetes-the-hard-way:remote:ProvisionEtcd',
+            if directory is None:
+                directory = '/etc/systemd/system'
+            __props__.__dict__["directory"] = directory
+            __props__.__dict__["install"] = install
+            if service is None and not opts.urn:
+                raise TypeError("Missing required property 'service'")
+            __props__.__dict__["service"] = service
+            __props__.__dict__["unit"] = unit
+            __props__.__dict__["unit_name"] = unit_name
+            __props__.__dict__["file"] = None
+        super(SystemdService, __self__).__init__(
+            'kubernetes-the-hard-way:remote:SystemdService',
             resource_name,
             __props__,
             opts,
             remote=True)
 
     @property
     @pulumi.getter
-    def architecture(self) -> pulumi.Output[Optional['Architecture']]:
-        """
-        TODO
-        """
-        return pulumi.get(self, "architecture")
-
-    @property
-    @pulumi.getter(name="binaryDirectory")
-    def binary_directory(self) -> pulumi.Output[Optional[str]]:
-        """
-        TODO
-        """
-        return pulumi.get(self, "binary_directory")
-
-    @property
-    @pulumi.getter
-    def bundle(self) -> pulumi.Output['_tls.outputs.Bundle']:
-        """
-        The TLS bundle.
-        """
-        return pulumi.get(self, "bundle")
-
-    @property
-    @pulumi.getter
-    def configuration(self) -> pulumi.Output['EtcdConfiguration']:
-        """
-        Etcd configuration.
-        """
-        return pulumi.get(self, "configuration")
-
-    @property
-    @pulumi.getter(name="configurationDirectory")
-    def configuration_directory(self) -> pulumi.Output[Optional[str]]:
-        """
-        The directory to use for etcd configuration.
-        """
-        return pulumi.get(self, "configuration_directory")
-
-    @property
-    @pulumi.getter
     def connection(self) -> pulumi.Output['pulumi_command.remote.outputs.Connection']:
         """
         The parameters with which to connect to the remote host.
         """
         return pulumi.get(self, "connection")
 
     @property
-    @pulumi.getter(name="dataDirectory")
-    def data_directory(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter
+    def directory(self) -> pulumi.Output[str]:
         """
-        The directory to use for etcd data.
+        The location to create the service file.
         """
-        return pulumi.get(self, "data_directory")
+        return pulumi.get(self, "directory")
 
     @property
     @pulumi.getter
-    def install(self) -> pulumi.Output['EtcdInstall']:
+    def file(self) -> pulumi.Output['File']:
         """
-        Install etcd.
+        The service file on the remote machine.
         """
-        return pulumi.get(self, "install")
+        return pulumi.get(self, "file")
 
     @property
-    @pulumi.getter(name="internalIp")
-    def internal_ip(self) -> pulumi.Output[str]:
+    @pulumi.getter
+    def install(self) -> pulumi.Output[Optional['outputs.SystemdInstallSection']]:
         """
-        The internal IP of the etcd node
+        Describes the [Install] section of a systemd service file.
         """
-        return pulumi.get(self, "internal_ip")
+        return pulumi.get(self, "install")
 
     @property
     @pulumi.getter
-    def service(self) -> pulumi.Output['SystemdService']:
+    def service(self) -> pulumi.Output['outputs.SystemdServiceSection']:
         """
-        Systemd service.
+        Describes the [Service] section of a systemd service file.
         """
         return pulumi.get(self, "service")
 
     @property
     @pulumi.getter
-    def start(self) -> pulumi.Output['StartEtcd']:
+    def unit(self) -> pulumi.Output[Optional['outputs.SystemdUnitSection']]:
         """
-        Start etcd
+        Describes the [Unit] section of a systemd service file.
         """
-        return pulumi.get(self, "start")
+        return pulumi.get(self, "unit")
 
     @property
-    @pulumi.getter
-    def version(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter(name="unitName")
+    def unit_name(self) -> pulumi.Output[Optional[str]]:
         """
-        The version to install.
+        Name of the systemd unit.
         """
-        return pulumi.get(self, "version")
+        return pulumi.get(self, "unit_name")
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/runc_install.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/runc_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/start_etcd.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/start_etcd.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/static_pod.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/static_pod.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tls/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tls/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tls/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tls/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tls/certificate.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tls/certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tls/encryption_key.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tls/encryption_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tls/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tls/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tls/root_ca.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tls/root_ca.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/chmod.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/chmod.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/curl.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/curl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/etcdctl.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/etcdctl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/mkdir.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/mkdir.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/mktemp.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/mktemp.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/mv.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/mv.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/rm.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/rm.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/sed.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/sed.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/systemctl.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/systemctl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/tar.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/tar.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/tee.py` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/wget.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,43 +5,42 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
-from ._enums import *
 from ._inputs import *
 import pulumi_command
 
-__all__ = ['TeeArgs', 'Tee']
+__all__ = ['WgetArgs', 'Wget']
 
 @pulumi.input_type
-class TeeArgs:
+class WgetArgs:
     def __init__(__self__, *,
                  connection: pulumi.Input['pulumi_command.remote.ConnectionArgs'],
                  binary_path: Optional[pulumi.Input[str]] = None,
-                 create: Optional[Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']]] = None,
-                 delete: Optional[Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']]] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input['WgetOptsArgs']]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input['WgetOptsArgs']]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 update: Optional[Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']]] = None):
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input['WgetOptsArgs']]] = None):
         """
-        The set of arguments for constructing a Tee resource.
+        The set of arguments for constructing a Wget resource.
         :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: Connection details for the remote system
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
-        :param Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']] create: The command to run on create.
-        :param Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+        :param Union[pulumi.Input[str], pulumi.Input['WgetOptsArgs']] create: The command to run on create.
+        :param Union[pulumi.Input[str], pulumi.Input['WgetOptsArgs']] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
                and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
                Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
         :param pulumi.Input[str] stdin: TODO
         :param pulumi.Input[Sequence[Any]] triggers: TODO
-        :param Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']] update: The command to run on update, if empty, create will 
+        :param Union[pulumi.Input[str], pulumi.Input['WgetOptsArgs']] update: The command to run on update, if empty, create will 
                run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
                are set to the stdout and stderr properties of the Command resource from previous 
                create or update steps.
         """
         pulumi.set(__self__, "connection", connection)
         if binary_path is not None:
             pulumi.set(__self__, "binary_path", binary_path)
@@ -80,36 +79,36 @@
 
     @binary_path.setter
     def binary_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "binary_path", value)
 
     @property
     @pulumi.getter
-    def create(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']]]:
+    def create(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['WgetOptsArgs']]]:
         """
         The command to run on create.
         """
         return pulumi.get(self, "create")
 
     @create.setter
-    def create(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']]]):
+    def create(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['WgetOptsArgs']]]):
         pulumi.set(self, "create", value)
 
     @property
     @pulumi.getter
-    def delete(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']]]:
+    def delete(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['WgetOptsArgs']]]:
         """
         The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
         and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
         Command resource from previous create or update steps.
         """
         return pulumi.get(self, "delete")
 
     @delete.setter
-    def delete(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']]]):
+    def delete(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['WgetOptsArgs']]]):
         pulumi.set(self, "delete", value)
 
     @property
     @pulumi.getter
     def environment(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Environment variables
@@ -142,119 +141,119 @@
 
     @triggers.setter
     def triggers(self, value: Optional[pulumi.Input[Sequence[Any]]]):
         pulumi.set(self, "triggers", value)
 
     @property
     @pulumi.getter
-    def update(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']]]:
+    def update(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['WgetOptsArgs']]]:
         """
         The command to run on update, if empty, create will 
         run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
         are set to the stdout and stderr properties of the Command resource from previous 
         create or update steps.
         """
         return pulumi.get(self, "update")
 
     @update.setter
-    def update(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']]]):
+    def update(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['WgetOptsArgs']]]):
         pulumi.set(self, "update", value)
 
 
-class Tee(pulumi.ComponentResource):
+class Wget(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  binary_path: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 create: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['TeeOptsArgs']]]] = None,
-                 delete: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['TeeOptsArgs']]]] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['WgetOptsArgs']]]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['WgetOptsArgs']]]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 update: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['TeeOptsArgs']]]] = None,
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['WgetOptsArgs']]]] = None,
                  __props__=None):
         """
-        Abstraction over the `rm` utility on a remote system.
+        Abstraction over the `wget` utility on a remote system.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
         :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: Connection details for the remote system
-        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['TeeOptsArgs']]] create: The command to run on create.
-        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['TeeOptsArgs']]] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['WgetOptsArgs']]] create: The command to run on create.
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['WgetOptsArgs']]] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
                and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
                Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
         :param pulumi.Input[str] stdin: TODO
         :param pulumi.Input[Sequence[Any]] triggers: TODO
-        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['TeeOptsArgs']]] update: The command to run on update, if empty, create will 
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['WgetOptsArgs']]] update: The command to run on update, if empty, create will 
                run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
                are set to the stdout and stderr properties of the Command resource from previous 
                create or update steps.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: TeeArgs,
+                 args: WgetArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Abstraction over the `rm` utility on a remote system.
+        Abstraction over the `wget` utility on a remote system.
 
         :param str resource_name: The name of the resource.
-        :param TeeArgs args: The arguments to use to populate this resource's properties.
+        :param WgetArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(TeeArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(WgetArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  binary_path: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 create: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['TeeOptsArgs']]]] = None,
-                 delete: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['TeeOptsArgs']]]] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['WgetOptsArgs']]]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['WgetOptsArgs']]]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 update: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['TeeOptsArgs']]]] = None,
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['WgetOptsArgs']]]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = TeeArgs.__new__(TeeArgs)
+            __props__ = WgetArgs.__new__(WgetArgs)
 
             __props__.__dict__["binary_path"] = binary_path
             if connection is None and not opts.urn:
                 raise TypeError("Missing required property 'connection'")
             __props__.__dict__["connection"] = connection
             __props__.__dict__["create"] = create
             __props__.__dict__["delete"] = delete
             __props__.__dict__["environment"] = environment
             __props__.__dict__["stdin"] = stdin
             __props__.__dict__["triggers"] = triggers
             __props__.__dict__["update"] = update
             __props__.__dict__["command"] = None
             __props__.__dict__["stderr"] = None
             __props__.__dict__["stdout"] = None
-        super(Tee, __self__).__init__(
-            'kubernetes-the-hard-way:tools:Tee',
+        super(Wget, __self__).__init__(
+            'kubernetes-the-hard-way:tools:Wget',
             resource_name,
             __props__,
             opts,
             remote=True)
 
     @property
     @pulumi.getter(name="binaryPath")
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kubernetes_the_hard_way
-Version: 0.0.21a1716157484
+Version: 0.0.22
 Summary: A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way
 License: Apache-2.0
 Project-URL: Repository, https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way
 Keywords: pulumi,command,tls,kubernetes,category/utility,kind/component
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt` & `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -11,17 +11,15 @@
 pulumi_kubernetes_the_hard_way.egg-info/requires.txt
 pulumi_kubernetes_the_hard_way.egg-info/top_level.txt
 pulumi_kubernetes_the_hard_way/config/__init__.py
 pulumi_kubernetes_the_hard_way/config/_enums.py
 pulumi_kubernetes_the_hard_way/config/_inputs.py
 pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py
 pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py
-pulumi_kubernetes_the_hard_way/config/get_kubelet_configuration.py
 pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py
-pulumi_kubernetes_the_hard_way/config/kubelet_configuration.py
 pulumi_kubernetes_the_hard_way/config/outputs.py
 pulumi_kubernetes_the_hard_way/remote/__init__.py
 pulumi_kubernetes_the_hard_way/remote/_enums.py
 pulumi_kubernetes_the_hard_way/remote/_inputs.py
 pulumi_kubernetes_the_hard_way/remote/cni_bridge_plugin_configuration.py
 pulumi_kubernetes_the_hard_way/remote/cni_loopback_plugin_configuration.py
 pulumi_kubernetes_the_hard_way/remote/cni_plugin_configuration.py
@@ -37,15 +35,14 @@
 pulumi_kubernetes_the_hard_way/remote/file.py
 pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py
 pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py
 pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py
 pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py
 pulumi_kubernetes_the_hard_way/remote/kubectl_install.py
 pulumi_kubernetes_the_hard_way/remote/kubelet_install.py
-pulumi_kubernetes_the_hard_way/remote/kubelet_service.py
 pulumi_kubernetes_the_hard_way/remote/outputs.py
 pulumi_kubernetes_the_hard_way/remote/provision_etcd.py
 pulumi_kubernetes_the_hard_way/remote/runc_install.py
 pulumi_kubernetes_the_hard_way/remote/start_etcd.py
 pulumi_kubernetes_the_hard_way/remote/static_pod.py
 pulumi_kubernetes_the_hard_way/remote/systemd_service.py
 pulumi_kubernetes_the_hard_way/tls/__init__.py
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pyproject.toml` & `pulumi_kubernetes_the_hard_way-0.0.22/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_kubernetes_the_hard_way"
   description = "A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way"
   dependencies = ["parver>=0.2.1", "pulumi>=3.91.1,<4.0.0", "pulumi-command>=0.11.1,<1.0.0", "pulumi-kubernetes>=4.11.0,<5.0.0", "pulumi-random>=4.16.1,<5.0.0", "pulumi-tls>=5.0.2,<6.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "command", "tls", "kubernetes", "category/utility", "kind/component"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "0.0.21a1716157484"
+  version = "0.0.22"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Repository = "https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way"
 
 [build-system]
   requires = ["setuptools>=61.0"]
```

