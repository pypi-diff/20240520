# Comparing `tmp/pulumi_kubernetes_the_hard_way-0.0.21a1716143882.tar.gz` & `tmp/pulumi_kubernetes_the_hard_way-0.0.21a1716157484.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_kubernetes_the_hard_way-0.0.21a1716143882.tar", last modified: Sun May 19 18:40:26 2024, max compression
+gzip compressed data, was "pulumi_kubernetes_the_hard_way-0.0.21a1716157484.tar", last modified: Sun May 19 22:27:23 2024, max compression
```

## Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882.tar` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:40:26.552522 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-19 18:40:26.552522 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:40:26.536522 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/
--rw-------   0 runner    (1001) docker     (127)     4606 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/__init__.py
--rw-------   0 runner    (1001) docker     (127)     9268 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:40:26.540522 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/config/
--rw-------   0 runner    (1001) docker     (127)      496 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/config/__init__.py
--rw-------   0 runner    (1001) docker     (127)      427 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/config/_enums.py
--rw-------   0 runner    (1001) docker     (127)    21648 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/config/_inputs.py
--rw-------   0 runner    (1001) docker     (127)     8728 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py
--rw-------   0 runner    (1001) docker     (127)     3426 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py
--rw-------   0 runner    (1001) docker     (127)     4775 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/config/get_kubelet_configuration.py
--rw-------   0 runner    (1001) docker     (127)    23922 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py
--rw-------   0 runner    (1001) docker     (127)    12667 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/config/kubelet_configuration.py
--rw-------   0 runner    (1001) docker     (127)    38474 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/config/outputs.py
--rw-------   0 runner    (1001) docker     (127)     2783 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/provider.py
--rw-------   0 runner    (1001) docker     (127)      116 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (127)        0 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:40:26.548522 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/
--rw-------   0 runner    (1001) docker     (127)     1147 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/__init__.py
--rw-------   0 runner    (1001) docker     (127)     1095 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/_enums.py
--rw-------   0 runner    (1001) docker     (127)    29297 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    13340 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/cni_bridge_plugin_configuration.py
--rw-------   0 runner    (1001) docker     (127)     8612 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/cni_loopback_plugin_configuration.py
--rw-------   0 runner    (1001) docker     (127)     7575 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/cni_plugin_configuration.py
--rw-------   0 runner    (1001) docker     (127)    19229 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py
--rw-------   0 runner    (1001) docker     (127)     6879 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/containerd_configuration.py
--rw-------   0 runner    (1001) docker     (127)    10255 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/containerd_install.py
--rw-------   0 runner    (1001) docker     (127)    10159 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/crictl_install.py
--rw-------   0 runner    (1001) docker     (127)     8328 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/download.py
--rw-------   0 runner    (1001) docker     (127)    12377 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py
--rw-------   0 runner    (1001) docker     (127)    14905 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py
--rw-------   0 runner    (1001) docker     (127)    10651 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/etcd_install.py
--rw-------   0 runner    (1001) docker     (127)    14696 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/etcd_service.py
--rw-------   0 runner    (1001) docker     (127)     7339 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/file.py
--rw-------   0 runner    (1001) docker     (127)     9708 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py
--rw-------   0 runner    (1001) docker     (127)     9822 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py
--rw-------   0 runner    (1001) docker     (127)     9652 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py
--rw-------   0 runner    (1001) docker     (127)     9708 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py
--rw-------   0 runner    (1001) docker     (127)     9622 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py
--rw-------   0 runner    (1001) docker     (127)     9622 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py
--rw-------   0 runner    (1001) docker     (127)    15819 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/kubelet_service.py
--rw-------   0 runner    (1001) docker     (127)    29099 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/outputs.py
--rw-------   0 runner    (1001) docker     (127)    13390 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py
--rw-------   0 runner    (1001) docker     (127)     9580 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/runc_install.py
--rw-------   0 runner    (1001) docker     (127)     5113 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/start_etcd.py
--rw-------   0 runner    (1001) docker     (127)     7429 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/static_pod.py
--rw-------   0 runner    (1001) docker     (127)    10944 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/systemd_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:40:26.548522 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tls/
--rw-------   0 runner    (1001) docker     (127)      425 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tls/__init__.py
--rw-------   0 runner    (1001) docker     (127)     1000 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tls/_enums.py
--rw-------   0 runner    (1001) docker     (127)     3019 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tls/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    30597 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tls/certificate.py
--rw-------   0 runner    (1001) docker     (127)    15919 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py
--rw-------   0 runner    (1001) docker     (127)     4450 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tls/encryption_key.py
--rw-------   0 runner    (1001) docker     (127)     2983 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tls/outputs.py
--rw-------   0 runner    (1001) docker     (127)    27130 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tls/root_ca.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:40:26.552522 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/
--rw-------   0 runner    (1001) docker     (127)      590 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/__init__.py
--rw-------   0 runner    (1001) docker     (127)     3166 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/_enums.py
--rw-------   0 runner    (1001) docker     (127)   108491 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    14957 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/chmod.py
--rw-------   0 runner    (1001) docker     (127)    14976 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/curl.py
--rw-------   0 runner    (1001) docker     (127)    15049 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/etcdctl.py
--rw-------   0 runner    (1001) docker     (127)    15189 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py
--rw-------   0 runner    (1001) docker     (127)    14957 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/mkdir.py
--rw-------   0 runner    (1001) docker     (127)    14992 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/mktemp.py
--rw-------   0 runner    (1001) docker     (127)    14852 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/mv.py
--rw-------   0 runner    (1001) docker     (127)    91820 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/outputs.py
--rw-------   0 runner    (1001) docker     (127)    14852 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/rm.py
--rw-------   0 runner    (1001) docker     (127)    14887 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/sed.py
--rw-------   0 runner    (1001) docker     (127)    15119 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/systemctl.py
--rw-------   0 runner    (1001) docker     (127)    14887 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/tar.py
--rw-------   0 runner    (1001) docker     (127)    14907 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/tee.py
--rw-------   0 runner    (1001) docker     (127)    14922 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/wget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:40:26.552522 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-19 18:40:26.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-05-19 18:40:26.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 18:40:26.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-19 18:40:26.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-19 18:40:26.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way.egg-info/top_level.txt
--rw-------   0 runner    (1001) docker     (127)      899 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 18:40:26.552522 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:27:23.971222 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-19 22:27:23.971222 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:27:23.955223 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/
+-rw-------   0 runner    (1001) docker     (127)     4606 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     9268 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:27:23.959223 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/config/
+-rw-------   0 runner    (1001) docker     (127)      496 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/config/__init__.py
+-rw-------   0 runner    (1001) docker     (127)      427 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/config/_enums.py
+-rw-------   0 runner    (1001) docker     (127)    21648 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/config/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)     8791 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py
+-rw-------   0 runner    (1001) docker     (127)     3426 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py
+-rw-------   0 runner    (1001) docker     (127)     4826 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/config/get_kubelet_configuration.py
+-rw-------   0 runner    (1001) docker     (127)    23901 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py
+-rw-------   0 runner    (1001) docker     (127)    12558 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/config/kubelet_configuration.py
+-rw-------   0 runner    (1001) docker     (127)    38474 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/config/outputs.py
+-rw-------   0 runner    (1001) docker     (127)     2783 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/provider.py
+-rw-------   0 runner    (1001) docker     (127)      116 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/pulumi-plugin.json
+-rw-------   0 runner    (1001) docker     (127)        0 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:27:23.963223 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/
+-rw-------   0 runner    (1001) docker     (127)     1147 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     1095 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/_enums.py
+-rw-------   0 runner    (1001) docker     (127)    29297 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    13340 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/cni_bridge_plugin_configuration.py
+-rw-------   0 runner    (1001) docker     (127)     8612 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/cni_loopback_plugin_configuration.py
+-rw-------   0 runner    (1001) docker     (127)     7575 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/cni_plugin_configuration.py
+-rw-------   0 runner    (1001) docker     (127)    19229 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py
+-rw-------   0 runner    (1001) docker     (127)     6879 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/containerd_configuration.py
+-rw-------   0 runner    (1001) docker     (127)    10255 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/containerd_install.py
+-rw-------   0 runner    (1001) docker     (127)    10159 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/crictl_install.py
+-rw-------   0 runner    (1001) docker     (127)     8328 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/download.py
+-rw-------   0 runner    (1001) docker     (127)    12377 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py
+-rw-------   0 runner    (1001) docker     (127)    14905 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py
+-rw-------   0 runner    (1001) docker     (127)    10651 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/etcd_install.py
+-rw-------   0 runner    (1001) docker     (127)    14696 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/etcd_service.py
+-rw-------   0 runner    (1001) docker     (127)     7339 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/file.py
+-rw-------   0 runner    (1001) docker     (127)     9708 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py
+-rw-------   0 runner    (1001) docker     (127)     9822 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py
+-rw-------   0 runner    (1001) docker     (127)     9652 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py
+-rw-------   0 runner    (1001) docker     (127)     9708 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py
+-rw-------   0 runner    (1001) docker     (127)     9622 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py
+-rw-------   0 runner    (1001) docker     (127)     9622 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py
+-rw-------   0 runner    (1001) docker     (127)    15819 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/kubelet_service.py
+-rw-------   0 runner    (1001) docker     (127)    29099 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/outputs.py
+-rw-------   0 runner    (1001) docker     (127)    13390 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py
+-rw-------   0 runner    (1001) docker     (127)     9580 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/runc_install.py
+-rw-------   0 runner    (1001) docker     (127)     5113 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/start_etcd.py
+-rw-------   0 runner    (1001) docker     (127)     7429 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/static_pod.py
+-rw-------   0 runner    (1001) docker     (127)    10944 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/systemd_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:27:23.967223 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tls/
+-rw-------   0 runner    (1001) docker     (127)      425 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tls/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     1000 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tls/_enums.py
+-rw-------   0 runner    (1001) docker     (127)     3019 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tls/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    30597 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tls/certificate.py
+-rw-------   0 runner    (1001) docker     (127)    15919 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py
+-rw-------   0 runner    (1001) docker     (127)     4450 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tls/encryption_key.py
+-rw-------   0 runner    (1001) docker     (127)     2983 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tls/outputs.py
+-rw-------   0 runner    (1001) docker     (127)    27130 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tls/root_ca.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:27:23.971222 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/
+-rw-------   0 runner    (1001) docker     (127)      590 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     3166 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/_enums.py
+-rw-------   0 runner    (1001) docker     (127)   108491 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    14957 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/chmod.py
+-rw-------   0 runner    (1001) docker     (127)    14976 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/curl.py
+-rw-------   0 runner    (1001) docker     (127)    15049 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/etcdctl.py
+-rw-------   0 runner    (1001) docker     (127)    15189 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py
+-rw-------   0 runner    (1001) docker     (127)    14957 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/mkdir.py
+-rw-------   0 runner    (1001) docker     (127)    14992 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/mktemp.py
+-rw-------   0 runner    (1001) docker     (127)    14852 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/mv.py
+-rw-------   0 runner    (1001) docker     (127)    91820 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/outputs.py
+-rw-------   0 runner    (1001) docker     (127)    14852 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/rm.py
+-rw-------   0 runner    (1001) docker     (127)    14887 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/sed.py
+-rw-------   0 runner    (1001) docker     (127)    15119 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/systemctl.py
+-rw-------   0 runner    (1001) docker     (127)    14887 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/tar.py
+-rw-------   0 runner    (1001) docker     (127)    14907 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/tee.py
+-rw-------   0 runner    (1001) docker     (127)    14922 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/wget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:27:23.971222 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-19 22:27:23.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-05-19 22:27:23.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 22:27:23.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-19 22:27:23.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-19 22:27:23.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way.egg-info/top_level.txt
+-rw-------   0 runner    (1001) docker     (127)      899 2024-05-19 22:27:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 22:27:23.971222 pulumi_kubernetes_the_hard_way-0.0.21a1716157484/setup.cfg
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/PKG-INFO` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kubernetes_the_hard_way
-Version: 0.0.21a1716143882
+Version: 0.0.21a1716157484
 Summary: A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way
 License: Apache-2.0
 Project-URL: Repository, https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way
 Keywords: pulumi,command,tls,kubernetes,category/utility,kind/component
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/README.md` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/_utilities.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/config/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/config/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,17 @@
     'AwaitableGetKubeVipManifestResult',
     'get_kube_vip_manifest',
     'get_kube_vip_manifest_output',
 ]
 
 @pulumi.output_type
 class GetKubeVipManifestResult:
+    """
+    Gets the static pod manifests for KubeVip.
+    """
     def __init__(__self__, result=None):
         if result and not isinstance(result, dict):
             raise TypeError("Expected argument 'result' to be a dict")
         pulumi.set(__self__, "result", result)
 
     @property
     @pulumi.getter
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/config/get_kubelet_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/config/get_kubelet_configuration.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,17 @@
     'AwaitableGetKubeletConfigurationResult',
     'get_kubelet_configuration',
     'get_kubelet_configuration_output',
 ]
 
 @pulumi.output_type
 class GetKubeletConfigurationResult:
+    """
+    Get the kubelet configuration.
+    """
     def __init__(__self__, result=None):
         if result and not isinstance(result, dict):
             raise TypeError("Expected argument 'result' to be a dict")
         pulumi.set(__self__, "result", result)
 
     @property
     @pulumi.getter
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py`

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
-        Pseudo resource for generating the kube-vip manifest.
+        Gets the static pod manifests for KubeVip.
 
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
-        Pseudo resource for generating the kube-vip manifest.
+        Gets the static pod manifests for KubeVip.
 
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
-        The yaml representation of the manifest
+        The yaml representation of the manifest.
         """
         return pulumi.get(self, "yaml")
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/config/kubelet_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/config/kubelet_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,26 +191,28 @@
                  resolv_conf: Optional[pulumi.Input[str]] = None,
                  runtime_request_timeout: Optional[pulumi.Input[str]] = None,
                  tls_cert_file: Optional[pulumi.Input[str]] = None,
                  tls_private_key_file: Optional[pulumi.Input[str]] = None,
                  webhook: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         """
-        Create a KubeletConfiguration resource with the given unique name, props, and options.
+        Get the kubelet configuration.
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: KubeletConfigurationArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Create a KubeletConfiguration resource with the given unique name, props, and options.
+        Get the kubelet configuration.
+
         :param str resource_name: The name of the resource.
         :param KubeletConfigurationArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(KubeletConfigurationArgs, pulumi.ResourceOptions, *args, **kwargs)
@@ -275,11 +277,11 @@
     def result(self) -> pulumi.Output['outputs.KubeletConfiguration']:
         return pulumi.get(self, "result")
 
     @property
     @pulumi.getter
     def yaml(self) -> pulumi.Output[str]:
         """
-        The yaml representation of the manifest
+        The yaml representation of the manifest.
         """
         return pulumi.get(self, "yaml")
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/config/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/provider.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/cni_bridge_plugin_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/cni_bridge_plugin_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/cni_loopback_plugin_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/cni_loopback_plugin_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/cni_plugin_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/cni_plugin_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/containerd_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/containerd_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/containerd_install.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/containerd_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/crictl_install.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/crictl_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/download.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/download.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/etcd_install.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/etcd_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/etcd_service.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/etcd_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/file.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/file.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/kubelet_service.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/kubelet_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/runc_install.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/runc_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/start_etcd.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/start_etcd.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/static_pod.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/static_pod.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/systemd_service.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/remote/systemd_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tls/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tls/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tls/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tls/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tls/certificate.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tls/certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tls/encryption_key.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tls/encryption_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tls/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tls/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tls/root_ca.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tls/root_ca.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/chmod.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/chmod.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/curl.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/curl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/etcdctl.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/etcdctl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/mkdir.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/mkdir.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/mktemp.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/mktemp.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/mv.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/mv.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/rm.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/rm.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/sed.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/sed.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/systemctl.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/systemctl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/tar.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/tar.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/tee.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/tee.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/wget.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way/tools/wget.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kubernetes_the_hard_way
-Version: 0.0.21a1716143882
+Version: 0.0.21a1716157484
 Summary: A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way
 License: Apache-2.0
 Project-URL: Repository, https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way
 Keywords: pulumi,command,tls,kubernetes,category/utility,kind/component
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pyproject.toml` & `pulumi_kubernetes_the_hard_way-0.0.21a1716157484/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_kubernetes_the_hard_way"
   description = "A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way"
   dependencies = ["parver>=0.2.1", "pulumi>=3.91.1,<4.0.0", "pulumi-command>=0.11.1,<1.0.0", "pulumi-kubernetes>=4.11.0,<5.0.0", "pulumi-random>=4.16.1,<5.0.0", "pulumi-tls>=5.0.2,<6.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "command", "tls", "kubernetes", "category/utility", "kind/component"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "0.0.21a1716143882"
+  version = "0.0.21a1716157484"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Repository = "https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way"
 
 [build-system]
   requires = ["setuptools>=61.0"]
```

