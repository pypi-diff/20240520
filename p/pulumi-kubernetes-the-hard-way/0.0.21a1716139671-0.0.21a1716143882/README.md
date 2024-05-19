# Comparing `tmp/pulumi_kubernetes_the_hard_way-0.0.21a1716139671.tar.gz` & `tmp/pulumi_kubernetes_the_hard_way-0.0.21a1716143882.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_kubernetes_the_hard_way-0.0.21a1716139671.tar", last modified: Sun May 19 17:30:02 2024, max compression
+gzip compressed data, was "pulumi_kubernetes_the_hard_way-0.0.21a1716143882.tar", last modified: Sun May 19 18:40:26 2024, max compression
```

## Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671.tar` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882.tar`

### file list

```diff
@@ -1,83 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:30:02.659216 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-19 17:30:02.659216 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:30:02.643216 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/
--rw-------   0 runner    (1001) docker     (127)     4536 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/__init__.py
--rw-------   0 runner    (1001) docker     (127)     9268 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:30:02.647216 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/config/
--rw-------   0 runner    (1001) docker     (127)      496 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/config/__init__.py
--rw-------   0 runner    (1001) docker     (127)      427 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/config/_enums.py
--rw-------   0 runner    (1001) docker     (127)    21648 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/config/_inputs.py
--rw-------   0 runner    (1001) docker     (127)     8728 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py
--rw-------   0 runner    (1001) docker     (127)     3426 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py
--rw-------   0 runner    (1001) docker     (127)     4775 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/config/get_kubelet_configuration.py
--rw-------   0 runner    (1001) docker     (127)    23922 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py
--rw-------   0 runner    (1001) docker     (127)    12667 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/config/kubelet_configuration.py
--rw-------   0 runner    (1001) docker     (127)    38474 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/config/outputs.py
--rw-------   0 runner    (1001) docker     (127)     2783 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/provider.py
--rw-------   0 runner    (1001) docker     (127)      116 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (127)        0 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:30:02.651216 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/
--rw-------   0 runner    (1001) docker     (127)     1116 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/__init__.py
--rw-------   0 runner    (1001) docker     (127)     1095 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/_enums.py
--rw-------   0 runner    (1001) docker     (127)    24968 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    13340 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/cni_bridge_plugin_configuration.py
--rw-------   0 runner    (1001) docker     (127)     8612 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/cni_loopback_plugin_configuration.py
--rw-------   0 runner    (1001) docker     (127)     7575 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/cni_plugin_configuration.py
--rw-------   0 runner    (1001) docker     (127)    19229 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py
--rw-------   0 runner    (1001) docker     (127)     6879 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/containerd_configuration.py
--rw-------   0 runner    (1001) docker     (127)    10255 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/containerd_install.py
--rw-------   0 runner    (1001) docker     (127)    10159 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/crictl_install.py
--rw-------   0 runner    (1001) docker     (127)     8328 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/download.py
--rw-------   0 runner    (1001) docker     (127)    12377 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py
--rw-------   0 runner    (1001) docker     (127)    14905 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py
--rw-------   0 runner    (1001) docker     (127)    10651 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/etcd_install.py
--rw-------   0 runner    (1001) docker     (127)    14696 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/etcd_service.py
--rw-------   0 runner    (1001) docker     (127)     7339 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/file.py
--rw-------   0 runner    (1001) docker     (127)     9708 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py
--rw-------   0 runner    (1001) docker     (127)     9822 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py
--rw-------   0 runner    (1001) docker     (127)     9652 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py
--rw-------   0 runner    (1001) docker     (127)     9708 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py
--rw-------   0 runner    (1001) docker     (127)     9622 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py
--rw-------   0 runner    (1001) docker     (127)     9622 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py
--rw-------   0 runner    (1001) docker     (127)    25169 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/outputs.py
--rw-------   0 runner    (1001) docker     (127)    13390 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py
--rw-------   0 runner    (1001) docker     (127)     9580 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/runc_install.py
--rw-------   0 runner    (1001) docker     (127)     5113 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/start_etcd.py
--rw-------   0 runner    (1001) docker     (127)     7429 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/static_pod.py
--rw-------   0 runner    (1001) docker     (127)    10944 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/systemd_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:30:02.655216 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tls/
--rw-------   0 runner    (1001) docker     (127)      425 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tls/__init__.py
--rw-------   0 runner    (1001) docker     (127)     1000 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tls/_enums.py
--rw-------   0 runner    (1001) docker     (127)     3019 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tls/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    30597 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tls/certificate.py
--rw-------   0 runner    (1001) docker     (127)    15919 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py
--rw-------   0 runner    (1001) docker     (127)     4450 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tls/encryption_key.py
--rw-------   0 runner    (1001) docker     (127)     2983 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tls/outputs.py
--rw-------   0 runner    (1001) docker     (127)    27130 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tls/root_ca.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:30:02.659216 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/
--rw-------   0 runner    (1001) docker     (127)      590 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/__init__.py
--rw-------   0 runner    (1001) docker     (127)     3166 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/_enums.py
--rw-------   0 runner    (1001) docker     (127)   108491 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    14957 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/chmod.py
--rw-------   0 runner    (1001) docker     (127)    14976 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/curl.py
--rw-------   0 runner    (1001) docker     (127)    15049 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/etcdctl.py
--rw-------   0 runner    (1001) docker     (127)    15189 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py
--rw-------   0 runner    (1001) docker     (127)    14957 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/mkdir.py
--rw-------   0 runner    (1001) docker     (127)    14992 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/mktemp.py
--rw-------   0 runner    (1001) docker     (127)    14852 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/mv.py
--rw-------   0 runner    (1001) docker     (127)    91820 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/outputs.py
--rw-------   0 runner    (1001) docker     (127)    14852 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/rm.py
--rw-------   0 runner    (1001) docker     (127)    14887 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/sed.py
--rw-------   0 runner    (1001) docker     (127)    15119 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/systemctl.py
--rw-------   0 runner    (1001) docker     (127)    14887 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/tar.py
--rw-------   0 runner    (1001) docker     (127)    14907 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/tee.py
--rw-------   0 runner    (1001) docker     (127)    14922 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/wget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:30:02.659216 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-19 17:30:02.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-05-19 17:30:02.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 17:30:02.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-19 17:30:02.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-19 17:30:02.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way.egg-info/top_level.txt
--rw-------   0 runner    (1001) docker     (127)      899 2024-05-19 17:29:56.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 17:30:02.659216 pulumi_kubernetes_the_hard_way-0.0.21a1716139671/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:40:26.552522 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-19 18:40:26.552522 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:40:26.536522 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/
+-rw-------   0 runner    (1001) docker     (127)     4606 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     9268 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:40:26.540522 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/config/
+-rw-------   0 runner    (1001) docker     (127)      496 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/config/__init__.py
+-rw-------   0 runner    (1001) docker     (127)      427 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/config/_enums.py
+-rw-------   0 runner    (1001) docker     (127)    21648 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/config/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)     8728 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py
+-rw-------   0 runner    (1001) docker     (127)     3426 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py
+-rw-------   0 runner    (1001) docker     (127)     4775 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/config/get_kubelet_configuration.py
+-rw-------   0 runner    (1001) docker     (127)    23922 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py
+-rw-------   0 runner    (1001) docker     (127)    12667 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/config/kubelet_configuration.py
+-rw-------   0 runner    (1001) docker     (127)    38474 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/config/outputs.py
+-rw-------   0 runner    (1001) docker     (127)     2783 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/provider.py
+-rw-------   0 runner    (1001) docker     (127)      116 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/pulumi-plugin.json
+-rw-------   0 runner    (1001) docker     (127)        0 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:40:26.548522 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/
+-rw-------   0 runner    (1001) docker     (127)     1147 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     1095 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/_enums.py
+-rw-------   0 runner    (1001) docker     (127)    29297 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    13340 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/cni_bridge_plugin_configuration.py
+-rw-------   0 runner    (1001) docker     (127)     8612 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/cni_loopback_plugin_configuration.py
+-rw-------   0 runner    (1001) docker     (127)     7575 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/cni_plugin_configuration.py
+-rw-------   0 runner    (1001) docker     (127)    19229 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py
+-rw-------   0 runner    (1001) docker     (127)     6879 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/containerd_configuration.py
+-rw-------   0 runner    (1001) docker     (127)    10255 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/containerd_install.py
+-rw-------   0 runner    (1001) docker     (127)    10159 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/crictl_install.py
+-rw-------   0 runner    (1001) docker     (127)     8328 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/download.py
+-rw-------   0 runner    (1001) docker     (127)    12377 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py
+-rw-------   0 runner    (1001) docker     (127)    14905 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py
+-rw-------   0 runner    (1001) docker     (127)    10651 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/etcd_install.py
+-rw-------   0 runner    (1001) docker     (127)    14696 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/etcd_service.py
+-rw-------   0 runner    (1001) docker     (127)     7339 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/file.py
+-rw-------   0 runner    (1001) docker     (127)     9708 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py
+-rw-------   0 runner    (1001) docker     (127)     9822 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py
+-rw-------   0 runner    (1001) docker     (127)     9652 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py
+-rw-------   0 runner    (1001) docker     (127)     9708 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py
+-rw-------   0 runner    (1001) docker     (127)     9622 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py
+-rw-------   0 runner    (1001) docker     (127)     9622 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py
+-rw-------   0 runner    (1001) docker     (127)    15819 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/kubelet_service.py
+-rw-------   0 runner    (1001) docker     (127)    29099 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/outputs.py
+-rw-------   0 runner    (1001) docker     (127)    13390 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py
+-rw-------   0 runner    (1001) docker     (127)     9580 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/runc_install.py
+-rw-------   0 runner    (1001) docker     (127)     5113 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/start_etcd.py
+-rw-------   0 runner    (1001) docker     (127)     7429 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/static_pod.py
+-rw-------   0 runner    (1001) docker     (127)    10944 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/systemd_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:40:26.548522 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tls/
+-rw-------   0 runner    (1001) docker     (127)      425 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tls/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     1000 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tls/_enums.py
+-rw-------   0 runner    (1001) docker     (127)     3019 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tls/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    30597 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tls/certificate.py
+-rw-------   0 runner    (1001) docker     (127)    15919 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py
+-rw-------   0 runner    (1001) docker     (127)     4450 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tls/encryption_key.py
+-rw-------   0 runner    (1001) docker     (127)     2983 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tls/outputs.py
+-rw-------   0 runner    (1001) docker     (127)    27130 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tls/root_ca.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:40:26.552522 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/
+-rw-------   0 runner    (1001) docker     (127)      590 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     3166 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/_enums.py
+-rw-------   0 runner    (1001) docker     (127)   108491 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    14957 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/chmod.py
+-rw-------   0 runner    (1001) docker     (127)    14976 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/curl.py
+-rw-------   0 runner    (1001) docker     (127)    15049 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/etcdctl.py
+-rw-------   0 runner    (1001) docker     (127)    15189 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py
+-rw-------   0 runner    (1001) docker     (127)    14957 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/mkdir.py
+-rw-------   0 runner    (1001) docker     (127)    14992 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/mktemp.py
+-rw-------   0 runner    (1001) docker     (127)    14852 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/mv.py
+-rw-------   0 runner    (1001) docker     (127)    91820 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/outputs.py
+-rw-------   0 runner    (1001) docker     (127)    14852 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/rm.py
+-rw-------   0 runner    (1001) docker     (127)    14887 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/sed.py
+-rw-------   0 runner    (1001) docker     (127)    15119 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/systemctl.py
+-rw-------   0 runner    (1001) docker     (127)    14887 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/tar.py
+-rw-------   0 runner    (1001) docker     (127)    14907 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/tee.py
+-rw-------   0 runner    (1001) docker     (127)    14922 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/wget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:40:26.552522 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-19 18:40:26.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-05-19 18:40:26.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 18:40:26.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-19 18:40:26.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-19 18:40:26.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way.egg-info/top_level.txt
+-rw-------   0 runner    (1001) docker     (127)      899 2024-05-19 18:40:17.000000 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 18:40:26.552522 pulumi_kubernetes_the_hard_way-0.0.21a1716143882/setup.cfg
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/PKG-INFO` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kubernetes_the_hard_way
-Version: 0.0.21a1716139671
+Version: 0.0.21a1716143882
 Summary: A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way
 License: Apache-2.0
 Project-URL: Repository, https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way
 Keywords: pulumi,command,tls,kubernetes,category/utility,kind/component
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/README.md` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,15 @@
    "kubernetes-the-hard-way:remote:File": "File",
    "kubernetes-the-hard-way:remote:KubeApiServerInstall": "KubeApiServerInstall",
    "kubernetes-the-hard-way:remote:KubeControllerManagerInstall": "KubeControllerManagerInstall",
    "kubernetes-the-hard-way:remote:KubeProxyInstall": "KubeProxyInstall",
    "kubernetes-the-hard-way:remote:KubeSchedulerInstall": "KubeSchedulerInstall",
    "kubernetes-the-hard-way:remote:KubectlInstall": "KubectlInstall",
    "kubernetes-the-hard-way:remote:KubeletInstall": "KubeletInstall",
+   "kubernetes-the-hard-way:remote:KubeletService": "KubeletService",
    "kubernetes-the-hard-way:remote:ProvisionEtcd": "ProvisionEtcd",
    "kubernetes-the-hard-way:remote:RuncInstall": "RuncInstall",
    "kubernetes-the-hard-way:remote:StartEtcd": "StartEtcd",
    "kubernetes-the-hard-way:remote:StaticPod": "StaticPod",
    "kubernetes-the-hard-way:remote:SystemdService": "SystemdService"
   }
  },
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/_utilities.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/config/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/config/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/config/get_kubelet_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/config/get_kubelet_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/config/kubelet_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/config/kubelet_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/config/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/provider.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from .file import *
 from .kube_api_server_install import *
 from .kube_controller_manager_install import *
 from .kube_proxy_install import *
 from .kube_scheduler_install import *
 from .kubectl_install import *
 from .kubelet_install import *
+from .kubelet_service import *
 from .provision_etcd import *
 from .runc_install import *
 from .start_etcd import *
 from .static_pod import *
 from .systemd_service import *
 from ._inputs import *
 from . import outputs
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/_inputs.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     'ContainerdCriPluginConfigurationCniArgs',
     'ContainerdCriPluginConfigurationContainerdRuncOptionsArgs',
     'ContainerdCriPluginConfigurationContainerdRuncArgs',
     'ContainerdCriPluginConfigurationContainerdArgs',
     'ContainerdCriPluginConfigurationArgs',
     'EtcdConfigurationPropsArgs',
     'EtcdNodeArgs',
+    'KubeletConfigurationPropsArgs',
     'SystemdInstallSectionArgs',
     'SystemdServiceSectionArgs',
     'SystemdUnitSectionArgs',
 ]
 
 @pulumi.input_type
 class CniBridgeIpamArgs:
@@ -442,14 +443,97 @@
 
     @architecture.setter
     def architecture(self, value: Optional[pulumi.Input['Architecture']]):
         pulumi.set(self, "architecture", value)
 
 
 @pulumi.input_type
+class KubeletConfigurationPropsArgs:
+    def __init__(__self__, *,
+                 configuration_file_path: pulumi.Input[str],
+                 kubeconfig_path: pulumi.Input[str],
+                 kubelet_path: pulumi.Input[str],
+                 register_node: pulumi.Input[bool],
+                 v: pulumi.Input[int]):
+        """
+        Props for resources that consume kubelet configuration.
+        :param pulumi.Input[str] configuration_file_path: Path to the kubelet configuration.
+        :param pulumi.Input[str] kubeconfig_path: Path to the kubeconfig the kubelet will use
+        :param pulumi.Input[str] kubelet_path: Path to the kubelet binary.
+        :param pulumi.Input[bool] register_node: Whether to register the node. Defaults to `true`.
+        :param pulumi.Input[int] v: Verbosity. Defaults to `2`.
+        """
+        pulumi.set(__self__, "configuration_file_path", configuration_file_path)
+        pulumi.set(__self__, "kubeconfig_path", kubeconfig_path)
+        pulumi.set(__self__, "kubelet_path", kubelet_path)
+        pulumi.set(__self__, "register_node", register_node)
+        pulumi.set(__self__, "v", v)
+
+    @property
+    @pulumi.getter(name="configurationFilePath")
+    def configuration_file_path(self) -> pulumi.Input[str]:
+        """
+        Path to the kubelet configuration.
+        """
+        return pulumi.get(self, "configuration_file_path")
+
+    @configuration_file_path.setter
+    def configuration_file_path(self, value: pulumi.Input[str]):
+        pulumi.set(self, "configuration_file_path", value)
+
+    @property
+    @pulumi.getter(name="kubeconfigPath")
+    def kubeconfig_path(self) -> pulumi.Input[str]:
+        """
+        Path to the kubeconfig the kubelet will use
+        """
+        return pulumi.get(self, "kubeconfig_path")
+
+    @kubeconfig_path.setter
+    def kubeconfig_path(self, value: pulumi.Input[str]):
+        pulumi.set(self, "kubeconfig_path", value)
+
+    @property
+    @pulumi.getter(name="kubeletPath")
+    def kubelet_path(self) -> pulumi.Input[str]:
+        """
+        Path to the kubelet binary.
+        """
+        return pulumi.get(self, "kubelet_path")
+
+    @kubelet_path.setter
+    def kubelet_path(self, value: pulumi.Input[str]):
+        pulumi.set(self, "kubelet_path", value)
+
+    @property
+    @pulumi.getter(name="registerNode")
+    def register_node(self) -> pulumi.Input[bool]:
+        """
+        Whether to register the node. Defaults to `true`.
+        """
+        return pulumi.get(self, "register_node")
+
+    @register_node.setter
+    def register_node(self, value: pulumi.Input[bool]):
+        pulumi.set(self, "register_node", value)
+
+    @property
+    @pulumi.getter
+    def v(self) -> pulumi.Input[int]:
+        """
+        Verbosity. Defaults to `2`.
+        """
+        return pulumi.get(self, "v")
+
+    @v.setter
+    def v(self, value: pulumi.Input[int]):
+        pulumi.set(self, "v", value)
+
+
+@pulumi.input_type
 class SystemdInstallSectionArgs:
     def __init__(__self__, *,
                  wanted_by: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         https://www.freedesktop.org/software/systemd/man/latest/systemd.unit.html#%5BInstall%5D%20Section%20Options
         :param pulumi.Input[Sequence[pulumi.Input[str]]] wanted_by: A symbolic link is created in the .wants/, .requires/, or .upholds/ directory of each of the listed units when this unit is installed by systemctl enable.
         """
@@ -556,43 +640,75 @@
     def type(self, value: Optional[pulumi.Input['SystemdServiceType']]):
         pulumi.set(self, "type", value)
 
 
 @pulumi.input_type
 class SystemdUnitSectionArgs:
     def __init__(__self__, *,
+                 after: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 before: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  binds_to: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  documentation: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  requires: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  requisite: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  wants: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         https://www.freedesktop.org/software/systemd/man/latest/systemd.unit.html#
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] after: Those two settings configure ordering dependencies between units.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] before: Those two settings configure ordering dependencies between units.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] binds_to: Configures requirement dependencies, very similar in style to Requires=.
         :param pulumi.Input[str] description: A short human readable title of the unit.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] documentation: A space-separated list of URIs referencing documentation for this unit or its configuration.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] requires: Similar to Wants=, but declares a stronger requirement dependency.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] requisite: Similar to Requires=. However, if the units listed here are not started already, they will not be started and the starting of this unit will fail immediately.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] wants: Configures (weak) requirement dependencies on other units.
         """
+        if after is not None:
+            pulumi.set(__self__, "after", after)
+        if before is not None:
+            pulumi.set(__self__, "before", before)
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
+    @pulumi.getter
+    def after(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        Those two settings configure ordering dependencies between units.
+        """
+        return pulumi.get(self, "after")
+
+    @after.setter
+    def after(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "after", value)
+
+    @property
+    @pulumi.getter
+    def before(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        Those two settings configure ordering dependencies between units.
+        """
+        return pulumi.get(self, "before")
+
+    @before.setter
+    def before(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "before", value)
+
+    @property
     @pulumi.getter(name="bindsTo")
     def binds_to(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         Configures requirement dependencies, very similar in style to Requires=.
         """
         return pulumi.get(self, "binds_to")
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/cni_bridge_plugin_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/cni_bridge_plugin_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/cni_loopback_plugin_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/cni_loopback_plugin_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/cni_plugin_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/cni_plugin_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/containerd_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/containerd_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/containerd_install.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/containerd_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/crictl_install.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/crictl_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/download.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/download.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/etcd_install.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/etcd_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/etcd_service.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/etcd_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/file.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/file.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/outputs.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     'ContainerdCriPluginConfiguration',
     'ContainerdCriPluginConfigurationCni',
     'ContainerdCriPluginConfigurationContainerd',
     'ContainerdCriPluginConfigurationContainerdRunc',
     'ContainerdCriPluginConfigurationContainerdRuncOptions',
     'EtcdConfigurationProps',
     'EtcdNode',
+    'KubeletConfigurationProps',
     'SystemdInstallSection',
     'SystemdServiceSection',
     'SystemdUnitSection',
 ]
 
 @pulumi.output_type
 class CniBridgeIpam(dict):
@@ -489,14 +490,103 @@
         """
         The CPU architecture of the node.
         """
         return pulumi.get(self, "architecture")
 
 
 @pulumi.output_type
+class KubeletConfigurationProps(dict):
+    """
+    Props for resources that consume kubelet configuration.
+    """
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "configurationFilePath":
+            suggest = "configuration_file_path"
+        elif key == "kubeconfigPath":
+            suggest = "kubeconfig_path"
+        elif key == "kubeletPath":
+            suggest = "kubelet_path"
+        elif key == "registerNode":
+            suggest = "register_node"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in KubeletConfigurationProps. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        KubeletConfigurationProps.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        KubeletConfigurationProps.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 configuration_file_path: str,
+                 kubeconfig_path: str,
+                 kubelet_path: str,
+                 register_node: bool,
+                 v: int):
+        """
+        Props for resources that consume kubelet configuration.
+        :param str configuration_file_path: Path to the kubelet configuration.
+        :param str kubeconfig_path: Path to the kubeconfig the kubelet will use
+        :param str kubelet_path: Path to the kubelet binary.
+        :param bool register_node: Whether to register the node. Defaults to `true`.
+        :param int v: Verbosity. Defaults to `2`.
+        """
+        pulumi.set(__self__, "configuration_file_path", configuration_file_path)
+        pulumi.set(__self__, "kubeconfig_path", kubeconfig_path)
+        pulumi.set(__self__, "kubelet_path", kubelet_path)
+        pulumi.set(__self__, "register_node", register_node)
+        pulumi.set(__self__, "v", v)
+
+    @property
+    @pulumi.getter(name="configurationFilePath")
+    def configuration_file_path(self) -> str:
+        """
+        Path to the kubelet configuration.
+        """
+        return pulumi.get(self, "configuration_file_path")
+
+    @property
+    @pulumi.getter(name="kubeconfigPath")
+    def kubeconfig_path(self) -> str:
+        """
+        Path to the kubeconfig the kubelet will use
+        """
+        return pulumi.get(self, "kubeconfig_path")
+
+    @property
+    @pulumi.getter(name="kubeletPath")
+    def kubelet_path(self) -> str:
+        """
+        Path to the kubelet binary.
+        """
+        return pulumi.get(self, "kubelet_path")
+
+    @property
+    @pulumi.getter(name="registerNode")
+    def register_node(self) -> bool:
+        """
+        Whether to register the node. Defaults to `true`.
+        """
+        return pulumi.get(self, "register_node")
+
+    @property
+    @pulumi.getter
+    def v(self) -> int:
+        """
+        Verbosity. Defaults to `2`.
+        """
+        return pulumi.get(self, "v")
+
+
+@pulumi.output_type
 class SystemdInstallSection(dict):
     """
     https://www.freedesktop.org/software/systemd/man/latest/systemd.unit.html#%5BInstall%5D%20Section%20Options
     """
     @staticmethod
     def __key_warning(key: str):
         suggest = None
@@ -643,43 +733,67 @@
         return super().__getitem__(key)
 
     def get(self, key: str, default = None) -> Any:
         SystemdUnitSection.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
+                 after: Optional[Sequence[str]] = None,
+                 before: Optional[Sequence[str]] = None,
                  binds_to: Optional[Sequence[str]] = None,
                  description: Optional[str] = None,
                  documentation: Optional[Sequence[str]] = None,
                  requires: Optional[Sequence[str]] = None,
                  requisite: Optional[Sequence[str]] = None,
                  wants: Optional[Sequence[str]] = None):
         """
         https://www.freedesktop.org/software/systemd/man/latest/systemd.unit.html#
+        :param Sequence[str] after: Those two settings configure ordering dependencies between units.
+        :param Sequence[str] before: Those two settings configure ordering dependencies between units.
         :param Sequence[str] binds_to: Configures requirement dependencies, very similar in style to Requires=.
         :param str description: A short human readable title of the unit.
         :param Sequence[str] documentation: A space-separated list of URIs referencing documentation for this unit or its configuration.
         :param Sequence[str] requires: Similar to Wants=, but declares a stronger requirement dependency.
         :param Sequence[str] requisite: Similar to Requires=. However, if the units listed here are not started already, they will not be started and the starting of this unit will fail immediately.
         :param Sequence[str] wants: Configures (weak) requirement dependencies on other units.
         """
+        if after is not None:
+            pulumi.set(__self__, "after", after)
+        if before is not None:
+            pulumi.set(__self__, "before", before)
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
+    @pulumi.getter
+    def after(self) -> Optional[Sequence[str]]:
+        """
+        Those two settings configure ordering dependencies between units.
+        """
+        return pulumi.get(self, "after")
+
+    @property
+    @pulumi.getter
+    def before(self) -> Optional[Sequence[str]]:
+        """
+        Those two settings configure ordering dependencies between units.
+        """
+        return pulumi.get(self, "before")
+
+    @property
     @pulumi.getter(name="bindsTo")
     def binds_to(self) -> Optional[Sequence[str]]:
         """
         Configures requirement dependencies, very similar in style to Requires=.
         """
         return pulumi.get(self, "binds_to")
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/runc_install.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/runc_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/start_etcd.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/start_etcd.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/static_pod.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/static_pod.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/remote/systemd_service.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/remote/systemd_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tls/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tls/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tls/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tls/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tls/certificate.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tls/certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tls/encryption_key.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tls/encryption_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tls/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tls/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tls/root_ca.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tls/root_ca.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/chmod.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/chmod.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/curl.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/curl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/etcdctl.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/etcdctl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/mkdir.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/mkdir.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/mktemp.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/mktemp.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/mv.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/mv.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/rm.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/rm.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/sed.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/sed.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/systemctl.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/systemctl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/tar.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/tar.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/tee.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/tee.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way/tools/wget.py` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way/tools/wget.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kubernetes_the_hard_way
-Version: 0.0.21a1716139671
+Version: 0.0.21a1716143882
 Summary: A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way
 License: Apache-2.0
 Project-URL: Repository, https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way
 Keywords: pulumi,command,tls,kubernetes,category/utility,kind/component
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 pulumi_kubernetes_the_hard_way/remote/file.py
 pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py
 pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py
 pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py
 pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py
 pulumi_kubernetes_the_hard_way/remote/kubectl_install.py
 pulumi_kubernetes_the_hard_way/remote/kubelet_install.py
+pulumi_kubernetes_the_hard_way/remote/kubelet_service.py
 pulumi_kubernetes_the_hard_way/remote/outputs.py
 pulumi_kubernetes_the_hard_way/remote/provision_etcd.py
 pulumi_kubernetes_the_hard_way/remote/runc_install.py
 pulumi_kubernetes_the_hard_way/remote/start_etcd.py
 pulumi_kubernetes_the_hard_way/remote/static_pod.py
 pulumi_kubernetes_the_hard_way/remote/systemd_service.py
 pulumi_kubernetes_the_hard_way/tls/__init__.py
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.21a1716139671/pyproject.toml` & `pulumi_kubernetes_the_hard_way-0.0.21a1716143882/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_kubernetes_the_hard_way"
   description = "A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way"
   dependencies = ["parver>=0.2.1", "pulumi>=3.91.1,<4.0.0", "pulumi-command>=0.11.1,<1.0.0", "pulumi-kubernetes>=4.11.0,<5.0.0", "pulumi-random>=4.16.1,<5.0.0", "pulumi-tls>=5.0.2,<6.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "command", "tls", "kubernetes", "category/utility", "kind/component"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "0.0.21a1716139671"
+  version = "0.0.21a1716143882"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Repository = "https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way"
 
 [build-system]
   requires = ["setuptools>=61.0"]
```

