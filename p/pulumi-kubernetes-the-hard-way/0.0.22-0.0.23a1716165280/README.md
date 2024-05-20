# Comparing `tmp/pulumi_kubernetes_the_hard_way-0.0.22.tar.gz` & `tmp/pulumi_kubernetes_the_hard_way-0.0.23a1716165280.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_kubernetes_the_hard_way-0.0.22.tar", last modified: Mon May 20 00:22:35 2024, max compression
+gzip compressed data, was "pulumi_kubernetes_the_hard_way-0.0.23a1716165280.tar", last modified: Mon May 20 00:37:19 2024, max compression
```

## Comparing `pulumi_kubernetes_the_hard_way-0.0.22.tar` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280.tar`

### file list

```diff
@@ -1,81 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:22:35.327802 pulumi_kubernetes_the_hard_way-0.0.22/
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-20 00:22:35.327802 pulumi_kubernetes_the_hard_way-0.0.22/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:22:35.315802 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/
--rw-------   0 runner    (1001) docker     (127)     4454 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/__init__.py
--rw-------   0 runner    (1001) docker     (127)     9268 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:22:35.319802 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/config/
--rw-------   0 runner    (1001) docker     (127)      418 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/config/__init__.py
--rw-------   0 runner    (1001) docker     (127)      427 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/config/_enums.py
--rw-------   0 runner    (1001) docker     (127)    21101 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/config/_inputs.py
--rw-------   0 runner    (1001) docker     (127)     8728 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py
--rw-------   0 runner    (1001) docker     (127)     3426 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py
--rw-------   0 runner    (1001) docker     (127)    23922 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py
--rw-------   0 runner    (1001) docker     (127)    29159 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/config/outputs.py
--rw-------   0 runner    (1001) docker     (127)     2783 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/provider.py
--rw-------   0 runner    (1001) docker     (127)      116 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (127)        0 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:22:35.323802 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/
--rw-------   0 runner    (1001) docker     (127)     1116 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/__init__.py
--rw-------   0 runner    (1001) docker     (127)     1095 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/_enums.py
--rw-------   0 runner    (1001) docker     (127)    24968 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    13340 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/cni_bridge_plugin_configuration.py
--rw-------   0 runner    (1001) docker     (127)     8612 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/cni_loopback_plugin_configuration.py
--rw-------   0 runner    (1001) docker     (127)     7575 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/cni_plugin_configuration.py
--rw-------   0 runner    (1001) docker     (127)    19229 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py
--rw-------   0 runner    (1001) docker     (127)     6879 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/containerd_configuration.py
--rw-------   0 runner    (1001) docker     (127)    10255 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/containerd_install.py
--rw-------   0 runner    (1001) docker     (127)    10159 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/crictl_install.py
--rw-------   0 runner    (1001) docker     (127)     8328 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/download.py
--rw-------   0 runner    (1001) docker     (127)    12377 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py
--rw-------   0 runner    (1001) docker     (127)    14905 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py
--rw-------   0 runner    (1001) docker     (127)    10651 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/etcd_install.py
--rw-------   0 runner    (1001) docker     (127)    14696 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/etcd_service.py
--rw-------   0 runner    (1001) docker     (127)     7339 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/file.py
--rw-------   0 runner    (1001) docker     (127)     9708 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py
--rw-------   0 runner    (1001) docker     (127)     9822 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py
--rw-------   0 runner    (1001) docker     (127)     9652 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py
--rw-------   0 runner    (1001) docker     (127)     9708 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py
--rw-------   0 runner    (1001) docker     (127)     9622 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py
--rw-------   0 runner    (1001) docker     (127)     9622 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py
--rw-------   0 runner    (1001) docker     (127)    25169 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/outputs.py
--rw-------   0 runner    (1001) docker     (127)    13390 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py
--rw-------   0 runner    (1001) docker     (127)     9580 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/runc_install.py
--rw-------   0 runner    (1001) docker     (127)     5113 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/start_etcd.py
--rw-------   0 runner    (1001) docker     (127)     7429 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/static_pod.py
--rw-------   0 runner    (1001) docker     (127)    10944 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/systemd_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:22:35.323802 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tls/
--rw-------   0 runner    (1001) docker     (127)      425 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tls/__init__.py
--rw-------   0 runner    (1001) docker     (127)     1000 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tls/_enums.py
--rw-------   0 runner    (1001) docker     (127)     3019 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tls/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    30597 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tls/certificate.py
--rw-------   0 runner    (1001) docker     (127)    15919 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py
--rw-------   0 runner    (1001) docker     (127)     4450 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tls/encryption_key.py
--rw-------   0 runner    (1001) docker     (127)     2983 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tls/outputs.py
--rw-------   0 runner    (1001) docker     (127)    27130 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tls/root_ca.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:22:35.327802 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/
--rw-------   0 runner    (1001) docker     (127)      590 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/__init__.py
--rw-------   0 runner    (1001) docker     (127)     3166 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/_enums.py
--rw-------   0 runner    (1001) docker     (127)   108491 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    14957 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/chmod.py
--rw-------   0 runner    (1001) docker     (127)    14976 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/curl.py
--rw-------   0 runner    (1001) docker     (127)    15049 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/etcdctl.py
--rw-------   0 runner    (1001) docker     (127)    15189 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py
--rw-------   0 runner    (1001) docker     (127)    14957 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/mkdir.py
--rw-------   0 runner    (1001) docker     (127)    14992 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/mktemp.py
--rw-------   0 runner    (1001) docker     (127)    14852 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/mv.py
--rw-------   0 runner    (1001) docker     (127)    91820 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/outputs.py
--rw-------   0 runner    (1001) docker     (127)    14852 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/rm.py
--rw-------   0 runner    (1001) docker     (127)    14887 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/sed.py
--rw-------   0 runner    (1001) docker     (127)    15119 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/systemctl.py
--rw-------   0 runner    (1001) docker     (127)    14887 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/tar.py
--rw-------   0 runner    (1001) docker     (127)    14907 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/tee.py
--rw-------   0 runner    (1001) docker     (127)    14922 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/wget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:22:35.327802 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-20 00:22:35.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-05-20 00:22:35.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 00:22:35.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-20 00:22:35.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-20 00:22:35.000000 pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way.egg-info/top_level.txt
--rw-------   0 runner    (1001) docker     (127)      888 2024-05-20 00:22:28.000000 pulumi_kubernetes_the_hard_way-0.0.22/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 00:22:35.327802 pulumi_kubernetes_the_hard_way-0.0.22/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:37:19.676649 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-20 00:37:19.676649 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:37:19.660649 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/
+-rw-------   0 runner    (1001) docker     (127)     4766 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     9268 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:37:19.664649 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/config/
+-rw-------   0 runner    (1001) docker     (127)      580 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/config/__init__.py
+-rw-------   0 runner    (1001) docker     (127)      427 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/config/_enums.py
+-rw-------   0 runner    (1001) docker     (127)    21648 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/config/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)     2860 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/config/get_kube_proxy_configuration.py
+-rw-------   0 runner    (1001) docker     (127)     8791 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py
+-rw-------   0 runner    (1001) docker     (127)     3426 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py
+-rw-------   0 runner    (1001) docker     (127)     4826 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/config/get_kubelet_configuration.py
+-rw-------   0 runner    (1001) docker     (127)     5799 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/config/kube_proxy_configuration.py
+-rw-------   0 runner    (1001) docker     (127)    23901 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py
+-rw-------   0 runner    (1001) docker     (127)    12558 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/config/kubelet_configuration.py
+-rw-------   0 runner    (1001) docker     (127)    41444 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/config/outputs.py
+-rw-------   0 runner    (1001) docker     (127)     2783 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/provider.py
+-rw-------   0 runner    (1001) docker     (127)      116 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/pulumi-plugin.json
+-rw-------   0 runner    (1001) docker     (127)        0 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:37:19.668649 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/
+-rw-------   0 runner    (1001) docker     (127)     1181 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     1095 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/_enums.py
+-rw-------   0 runner    (1001) docker     (127)    30736 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    13340 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/cni_bridge_plugin_configuration.py
+-rw-------   0 runner    (1001) docker     (127)     8612 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/cni_loopback_plugin_configuration.py
+-rw-------   0 runner    (1001) docker     (127)     7575 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/cni_plugin_configuration.py
+-rw-------   0 runner    (1001) docker     (127)    19229 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py
+-rw-------   0 runner    (1001) docker     (127)     6879 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/containerd_configuration.py
+-rw-------   0 runner    (1001) docker     (127)    10255 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/containerd_install.py
+-rw-------   0 runner    (1001) docker     (127)    10159 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/crictl_install.py
+-rw-------   0 runner    (1001) docker     (127)     8328 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/download.py
+-rw-------   0 runner    (1001) docker     (127)    12377 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py
+-rw-------   0 runner    (1001) docker     (127)    14905 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py
+-rw-------   0 runner    (1001) docker     (127)    10651 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/etcd_install.py
+-rw-------   0 runner    (1001) docker     (127)    14696 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/etcd_service.py
+-rw-------   0 runner    (1001) docker     (127)     7339 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/file.py
+-rw-------   0 runner    (1001) docker     (127)     9708 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py
+-rw-------   0 runner    (1001) docker     (127)     9822 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py
+-rw-------   0 runner    (1001) docker     (127)     9652 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py
+-rw-------   0 runner    (1001) docker     (127)    13465 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/kube_proxy_service.py
+-rw-------   0 runner    (1001) docker     (127)     9708 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py
+-rw-------   0 runner    (1001) docker     (127)     9622 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py
+-rw-------   0 runner    (1001) docker     (127)     9622 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py
+-rw-------   0 runner    (1001) docker     (127)    15819 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/kubelet_service.py
+-rw-------   0 runner    (1001) docker     (127)    30935 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/outputs.py
+-rw-------   0 runner    (1001) docker     (127)    13390 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py
+-rw-------   0 runner    (1001) docker     (127)     9580 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/runc_install.py
+-rw-------   0 runner    (1001) docker     (127)     5113 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/start_etcd.py
+-rw-------   0 runner    (1001) docker     (127)     7429 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/static_pod.py
+-rw-------   0 runner    (1001) docker     (127)    10944 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/systemd_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:37:19.672649 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tls/
+-rw-------   0 runner    (1001) docker     (127)      425 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tls/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     1000 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tls/_enums.py
+-rw-------   0 runner    (1001) docker     (127)     3019 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tls/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    30597 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tls/certificate.py
+-rw-------   0 runner    (1001) docker     (127)    15919 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py
+-rw-------   0 runner    (1001) docker     (127)     4450 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tls/encryption_key.py
+-rw-------   0 runner    (1001) docker     (127)     2983 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tls/outputs.py
+-rw-------   0 runner    (1001) docker     (127)    27130 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tls/root_ca.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:37:19.676649 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tools/
+-rw-------   0 runner    (1001) docker     (127)      590 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tools/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     3166 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tools/_enums.py
+-rw-------   0 runner    (1001) docker     (127)   108491 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tools/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    14957 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tools/chmod.py
+-rw-------   0 runner    (1001) docker     (127)    14976 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tools/curl.py
+-rw-------   0 runner    (1001) docker     (127)    15049 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tools/etcdctl.py
+-rw-------   0 runner    (1001) docker     (127)    15189 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py
+-rw-------   0 runner    (1001) docker     (127)    14957 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tools/mkdir.py
+-rw-------   0 runner    (1001) docker     (127)    14992 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tools/mktemp.py
+-rw-------   0 runner    (1001) docker     (127)    14852 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tools/mv.py
+-rw-------   0 runner    (1001) docker     (127)    91820 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tools/outputs.py
+-rw-------   0 runner    (1001) docker     (127)    14852 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tools/rm.py
+-rw-------   0 runner    (1001) docker     (127)    14887 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tools/sed.py
+-rw-------   0 runner    (1001) docker     (127)    15119 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tools/systemctl.py
+-rw-------   0 runner    (1001) docker     (127)    14887 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tools/tar.py
+-rw-------   0 runner    (1001) docker     (127)    14907 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tools/tee.py
+-rw-------   0 runner    (1001) docker     (127)    14922 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tools/wget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:37:19.676649 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-20 00:37:19.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-05-20 00:37:19.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 00:37:19.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-20 00:37:19.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-20 00:37:19.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way.egg-info/top_level.txt
+-rw-------   0 runner    (1001) docker     (127)      899 2024-05-20 00:37:08.000000 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 00:37:19.676649 pulumi_kubernetes_the_hard_way-0.0.23a1716165280/setup.cfg
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/PKG-INFO` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kubernetes_the_hard_way
-Version: 0.0.22
+Version: 0.0.23a1716165280
 Summary: A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way
 License: Apache-2.0
 Project-URL: Repository, https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way
 Keywords: pulumi,command,tls,kubernetes,category/utility,kind/component
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/README.md` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,17 @@
     resource_modules="""
 [
  {
   "pkg": "kubernetes-the-hard-way",
   "mod": "config",
   "fqn": "pulumi_kubernetes_the_hard_way.config",
   "classes": {
-   "kubernetes-the-hard-way:config:KubeVipManifest": "KubeVipManifest"
+   "kubernetes-the-hard-way:config:KubeProxyConfiguration": "KubeProxyConfiguration",
+   "kubernetes-the-hard-way:config:KubeVipManifest": "KubeVipManifest",
+   "kubernetes-the-hard-way:config:KubeletConfiguration": "KubeletConfiguration"
   }
  },
  {
   "pkg": "kubernetes-the-hard-way",
   "mod": "remote",
   "fqn": "pulumi_kubernetes_the_hard_way.remote",
   "classes": {
@@ -51,17 +53,19 @@
    "kubernetes-the-hard-way:remote:EtcdConfiguration": "EtcdConfiguration",
    "kubernetes-the-hard-way:remote:EtcdInstall": "EtcdInstall",
    "kubernetes-the-hard-way:remote:EtcdService": "EtcdService",
    "kubernetes-the-hard-way:remote:File": "File",
    "kubernetes-the-hard-way:remote:KubeApiServerInstall": "KubeApiServerInstall",
    "kubernetes-the-hard-way:remote:KubeControllerManagerInstall": "KubeControllerManagerInstall",
    "kubernetes-the-hard-way:remote:KubeProxyInstall": "KubeProxyInstall",
+   "kubernetes-the-hard-way:remote:KubeProxyService": "KubeProxyService",
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

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/_utilities.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/config/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/config/_inputs.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,14 +21,17 @@
 ]
 
 @pulumi.input_type
 class KubeconfigAdminOptions:
     def __init__(__self__, *,
                  type: str,
                  public_ip: Optional[str] = None):
+        """
+        :param str public_ip: TODO
+        """
         pulumi.set(__self__, "type", 'admin')
         if public_ip is not None:
             pulumi.set(__self__, "public_ip", public_ip)
 
     @property
     @pulumi.getter
     def type(self) -> str:
@@ -37,26 +40,32 @@
     @type.setter
     def type(self, value: str):
         pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter(name="publicIp")
     def public_ip(self) -> Optional[str]:
+        """
+        TODO
+        """
         return pulumi.get(self, "public_ip")
 
     @public_ip.setter
     def public_ip(self, value: Optional[str]):
         pulumi.set(self, "public_ip", value)
 
 
 @pulumi.input_type
 class KubeconfigKubeControllerManagerOptions:
     def __init__(__self__, *,
                  type: str,
                  public_ip: Optional[str] = None):
+        """
+        :param str public_ip: TODO
+        """
         pulumi.set(__self__, "type", 'kube-controller-manager')
         if public_ip is not None:
             pulumi.set(__self__, "public_ip", public_ip)
 
     @property
     @pulumi.getter
     def type(self) -> str:
@@ -65,26 +74,32 @@
     @type.setter
     def type(self, value: str):
         pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter(name="publicIp")
     def public_ip(self) -> Optional[str]:
+        """
+        TODO
+        """
         return pulumi.get(self, "public_ip")
 
     @public_ip.setter
     def public_ip(self, value: Optional[str]):
         pulumi.set(self, "public_ip", value)
 
 
 @pulumi.input_type
 class KubeconfigKubeProxyOptions:
     def __init__(__self__, *,
                  type: str,
                  public_ip: Optional[str] = None):
+        """
+        :param str public_ip: TODO
+        """
         pulumi.set(__self__, "type", 'kube-proxy')
         if public_ip is not None:
             pulumi.set(__self__, "public_ip", public_ip)
 
     @property
     @pulumi.getter
     def type(self) -> str:
@@ -93,26 +108,32 @@
     @type.setter
     def type(self, value: str):
         pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter(name="publicIp")
     def public_ip(self) -> Optional[str]:
+        """
+        TODO
+        """
         return pulumi.get(self, "public_ip")
 
     @public_ip.setter
     def public_ip(self, value: Optional[str]):
         pulumi.set(self, "public_ip", value)
 
 
 @pulumi.input_type
 class KubeconfigKubeSchedulerOptions:
     def __init__(__self__, *,
                  type: str,
                  public_ip: Optional[str] = None):
+        """
+        :param str public_ip: TODO
+        """
         pulumi.set(__self__, "type", 'kube-scheduler')
         if public_ip is not None:
             pulumi.set(__self__, "public_ip", public_ip)
 
     @property
     @pulumi.getter
     def type(self) -> str:
@@ -121,44 +142,57 @@
     @type.setter
     def type(self, value: str):
         pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter(name="publicIp")
     def public_ip(self) -> Optional[str]:
+        """
+        TODO
+        """
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
+        """
+        :param str name: TODO
+        :param str public_ip: TODO
+        """
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "public_ip", public_ip)
         if type is not None:
             pulumi.set(__self__, "type", 'worker')
 
     @property
     @pulumi.getter
     def name(self) -> str:
+        """
+        TODO
+        """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: str):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter(name="publicIp")
     def public_ip(self) -> str:
+        """
+        TODO
+        """
         return pulumi.get(self, "public_ip")
 
     @public_ip.setter
     def public_ip(self, value: str):
         pulumi.set(self, "public_ip", value)
 
     @property
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py`

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

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py`

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

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/config/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/config/outputs.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,58 +11,179 @@
 from . import outputs
 from ._enums import *
 import pulumi_kubernetes
 
 __all__ = [
     'Cluster',
     'Context',
+    'KubeProxyConfiguration',
+    'KubeProxyConfigurationClientConnection',
     'Kubeconfig',
+    'KubeletConfiguration',
+    'KubeletConfigurationAuthentication',
+    'KubeletConfigurationAuthenticationAnonymous',
+    'KubeletConfigurationAuthenticationWebhook',
+    'KubeletConfigurationAuthenticationx509',
+    'KubeletConfigurationAuthorization',
     'PodManifest',
     'User',
 ]
 
 @pulumi.output_type
 class Cluster(dict):
     def __init__(__self__, *,
                  certificate_authority_data: str,
                  server: str):
+        """
+        :param str certificate_authority_data: TODO
+        :param str server: TODO
+        """
         pulumi.set(__self__, "certificate_authority_data", certificate_authority_data)
         pulumi.set(__self__, "server", server)
 
     @property
     @pulumi.getter(name="certificateAuthorityData")
     def certificate_authority_data(self) -> str:
+        """
+        TODO
+        """
         return pulumi.get(self, "certificate_authority_data")
 
     @property
     @pulumi.getter
     def server(self) -> str:
+        """
+        TODO
+        """
         return pulumi.get(self, "server")
 
 
 @pulumi.output_type
 class Context(dict):
     def __init__(__self__, *,
                  cluster: str,
                  user: str):
+        """
+        :param str cluster: TODO
+        :param str user: TODO
+        """
         pulumi.set(__self__, "cluster", cluster)
         pulumi.set(__self__, "user", user)
 
     @property
     @pulumi.getter
     def cluster(self) -> str:
+        """
+        TODO
+        """
         return pulumi.get(self, "cluster")
 
     @property
     @pulumi.getter
     def user(self) -> str:
+        """
+        TODO
+        """
         return pulumi.get(self, "user")
 
 
 @pulumi.output_type
+class KubeProxyConfiguration(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "clusterCIDR":
+            suggest = "cluster_cidr"
+        elif key == "apiVersion":
+            suggest = "api_version"
+        elif key == "clientConnection":
+            suggest = "client_connection"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in KubeProxyConfiguration. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        KubeProxyConfiguration.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        KubeProxyConfiguration.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 cluster_cidr: str,
+                 api_version: Optional[str] = None,
+                 client_connection: Optional['outputs.KubeProxyConfigurationClientConnection'] = None,
+                 kind: Optional[str] = None,
+                 mode: Optional[str] = None):
+        """
+        :param str cluster_cidr: TODO
+        :param str mode: TODO
+        """
+        pulumi.set(__self__, "cluster_cidr", cluster_cidr)
+        if api_version is not None:
+            pulumi.set(__self__, "api_version", 'kubeproxy.config.k8s.io/v1alpha1')
+        if client_connection is not None:
+            pulumi.set(__self__, "client_connection", client_connection)
+        if kind is not None:
+            pulumi.set(__self__, "kind", 'KubeProxyConfiguration')
+        if mode is not None:
+            pulumi.set(__self__, "mode", mode)
+
+    @property
+    @pulumi.getter(name="clusterCIDR")
+    def cluster_cidr(self) -> str:
+        """
+        TODO
+        """
+        return pulumi.get(self, "cluster_cidr")
+
+    @property
+    @pulumi.getter(name="apiVersion")
+    def api_version(self) -> Optional[str]:
+        return pulumi.get(self, "api_version")
+
+    @property
+    @pulumi.getter(name="clientConnection")
+    def client_connection(self) -> Optional['outputs.KubeProxyConfigurationClientConnection']:
+        return pulumi.get(self, "client_connection")
+
+    @property
+    @pulumi.getter
+    def kind(self) -> Optional[str]:
+        return pulumi.get(self, "kind")
+
+    @property
+    @pulumi.getter
+    def mode(self) -> Optional[str]:
+        """
+        TODO
+        """
+        return pulumi.get(self, "mode")
+
+
+@pulumi.output_type
+class KubeProxyConfigurationClientConnection(dict):
+    def __init__(__self__, *,
+                 kubeconfig: str):
+        """
+        :param str kubeconfig: Path to the kubeconfig.
+        """
+        pulumi.set(__self__, "kubeconfig", kubeconfig)
+
+    @property
+    @pulumi.getter
+    def kubeconfig(self) -> str:
+        """
+        Path to the kubeconfig.
+        """
+        return pulumi.get(self, "kubeconfig")
+
+
+@pulumi.output_type
 class Kubeconfig(dict):
     def __init__(__self__, *,
                  clusters: Sequence['outputs.Cluster'],
                  contexts: Sequence['outputs.Context'],
                  users: Sequence['outputs.User']):
         pulumi.set(__self__, "clusters", clusters)
         pulumi.set(__self__, "contexts", contexts)
@@ -81,14 +202,292 @@
     @property
     @pulumi.getter
     def users(self) -> Sequence['outputs.User']:
         return pulumi.get(self, "users")
 
 
 @pulumi.output_type
+class KubeletConfiguration(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "apiVersion":
+            suggest = "api_version"
+        elif key == "cgroupDriver":
+            suggest = "cgroup_driver"
+        elif key == "clusterDNS":
+            suggest = "cluster_dns"
+        elif key == "clusterDomain":
+            suggest = "cluster_domain"
+        elif key == "containerRuntimeEndpoint":
+            suggest = "container_runtime_endpoint"
+        elif key == "podCIDR":
+            suggest = "pod_cidr"
+        elif key == "resolvConf":
+            suggest = "resolv_conf"
+        elif key == "runtimeRequestTimeout":
+            suggest = "runtime_request_timeout"
+        elif key == "tlsCertFile":
+            suggest = "tls_cert_file"
+        elif key == "tlsPrivateKeyFile":
+            suggest = "tls_private_key_file"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in KubeletConfiguration. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        KubeletConfiguration.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        KubeletConfiguration.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 api_version: str,
+                 authentication: 'outputs.KubeletConfigurationAuthentication',
+                 authorization: 'outputs.KubeletConfigurationAuthorization',
+                 cgroup_driver: str,
+                 cluster_dns: Sequence[str],
+                 cluster_domain: str,
+                 container_runtime_endpoint: str,
+                 kind: str,
+                 pod_cidr: str,
+                 resolv_conf: str,
+                 runtime_request_timeout: str,
+                 tls_cert_file: str,
+                 tls_private_key_file: str):
+        """
+        :param str cgroup_driver: TODO
+        :param Sequence[str] cluster_dns: TODO
+        :param str cluster_domain: TODO
+        :param str container_runtime_endpoint: TODO
+        :param str pod_cidr: TODO
+        :param str resolv_conf: TODO
+        :param str runtime_request_timeout: TODO
+        :param str tls_cert_file: TODO
+        :param str tls_private_key_file: TODO
+        """
+        pulumi.set(__self__, "api_version", 'kubelet.config.k8s.io/v1beta1')
+        pulumi.set(__self__, "authentication", authentication)
+        pulumi.set(__self__, "authorization", authorization)
+        pulumi.set(__self__, "cgroup_driver", cgroup_driver)
+        pulumi.set(__self__, "cluster_dns", cluster_dns)
+        pulumi.set(__self__, "cluster_domain", cluster_domain)
+        pulumi.set(__self__, "container_runtime_endpoint", container_runtime_endpoint)
+        pulumi.set(__self__, "kind", 'KubeletConfiguration')
+        pulumi.set(__self__, "pod_cidr", pod_cidr)
+        pulumi.set(__self__, "resolv_conf", resolv_conf)
+        pulumi.set(__self__, "runtime_request_timeout", runtime_request_timeout)
+        pulumi.set(__self__, "tls_cert_file", tls_cert_file)
+        pulumi.set(__self__, "tls_private_key_file", tls_private_key_file)
+
+    @property
+    @pulumi.getter(name="apiVersion")
+    def api_version(self) -> str:
+        return pulumi.get(self, "api_version")
+
+    @property
+    @pulumi.getter
+    def authentication(self) -> 'outputs.KubeletConfigurationAuthentication':
+        return pulumi.get(self, "authentication")
+
+    @property
+    @pulumi.getter
+    def authorization(self) -> 'outputs.KubeletConfigurationAuthorization':
+        return pulumi.get(self, "authorization")
+
+    @property
+    @pulumi.getter(name="cgroupDriver")
+    def cgroup_driver(self) -> str:
+        """
+        TODO
+        """
+        return pulumi.get(self, "cgroup_driver")
+
+    @property
+    @pulumi.getter(name="clusterDNS")
+    def cluster_dns(self) -> Sequence[str]:
+        """
+        TODO
+        """
+        return pulumi.get(self, "cluster_dns")
+
+    @property
+    @pulumi.getter(name="clusterDomain")
+    def cluster_domain(self) -> str:
+        """
+        TODO
+        """
+        return pulumi.get(self, "cluster_domain")
+
+    @property
+    @pulumi.getter(name="containerRuntimeEndpoint")
+    def container_runtime_endpoint(self) -> str:
+        """
+        TODO
+        """
+        return pulumi.get(self, "container_runtime_endpoint")
+
+    @property
+    @pulumi.getter
+    def kind(self) -> str:
+        return pulumi.get(self, "kind")
+
+    @property
+    @pulumi.getter(name="podCIDR")
+    def pod_cidr(self) -> str:
+        """
+        TODO
+        """
+        return pulumi.get(self, "pod_cidr")
+
+    @property
+    @pulumi.getter(name="resolvConf")
+    def resolv_conf(self) -> str:
+        """
+        TODO
+        """
+        return pulumi.get(self, "resolv_conf")
+
+    @property
+    @pulumi.getter(name="runtimeRequestTimeout")
+    def runtime_request_timeout(self) -> str:
+        """
+        TODO
+        """
+        return pulumi.get(self, "runtime_request_timeout")
+
+    @property
+    @pulumi.getter(name="tlsCertFile")
+    def tls_cert_file(self) -> str:
+        """
+        TODO
+        """
+        return pulumi.get(self, "tls_cert_file")
+
+    @property
+    @pulumi.getter(name="tlsPrivateKeyFile")
+    def tls_private_key_file(self) -> str:
+        """
+        TODO
+        """
+        return pulumi.get(self, "tls_private_key_file")
+
+
+@pulumi.output_type
+class KubeletConfigurationAuthentication(dict):
+    def __init__(__self__, *,
+                 anonymous: 'outputs.KubeletConfigurationAuthenticationAnonymous',
+                 webhook: 'outputs.KubeletConfigurationAuthenticationWebhook',
+                 x509: 'outputs.KubeletConfigurationAuthenticationx509'):
+        pulumi.set(__self__, "anonymous", anonymous)
+        pulumi.set(__self__, "webhook", webhook)
+        pulumi.set(__self__, "x509", x509)
+
+    @property
+    @pulumi.getter
+    def anonymous(self) -> 'outputs.KubeletConfigurationAuthenticationAnonymous':
+        return pulumi.get(self, "anonymous")
+
+    @property
+    @pulumi.getter
+    def webhook(self) -> 'outputs.KubeletConfigurationAuthenticationWebhook':
+        return pulumi.get(self, "webhook")
+
+    @property
+    @pulumi.getter
+    def x509(self) -> 'outputs.KubeletConfigurationAuthenticationx509':
+        return pulumi.get(self, "x509")
+
+
+@pulumi.output_type
+class KubeletConfigurationAuthenticationAnonymous(dict):
+    def __init__(__self__, *,
+                 enabled: bool):
+        """
+        :param bool enabled: TODO
+        """
+        pulumi.set(__self__, "enabled", enabled)
+
+    @property
+    @pulumi.getter
+    def enabled(self) -> bool:
+        """
+        TODO
+        """
+        return pulumi.get(self, "enabled")
+
+
+@pulumi.output_type
+class KubeletConfigurationAuthenticationWebhook(dict):
+    def __init__(__self__, *,
+                 enabled: bool):
+        """
+        :param bool enabled: TODO
+        """
+        pulumi.set(__self__, "enabled", enabled)
+
+    @property
+    @pulumi.getter
+    def enabled(self) -> bool:
+        """
+        TODO
+        """
+        return pulumi.get(self, "enabled")
+
+
+@pulumi.output_type
+class KubeletConfigurationAuthenticationx509(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "clientCAFile":
+            suggest = "client_ca_file"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in KubeletConfigurationAuthenticationx509. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        KubeletConfigurationAuthenticationx509.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        KubeletConfigurationAuthenticationx509.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 client_ca_file: str):
+        """
+        :param str client_ca_file: TODO
+        """
+        pulumi.set(__self__, "client_ca_file", client_ca_file)
+
+    @property
+    @pulumi.getter(name="clientCAFile")
+    def client_ca_file(self) -> str:
+        """
+        TODO
+        """
+        return pulumi.get(self, "client_ca_file")
+
+
+@pulumi.output_type
+class KubeletConfigurationAuthorization(dict):
+    def __init__(__self__, *,
+                 mode: str):
+        pulumi.set(__self__, "mode", mode)
+
+    @property
+    @pulumi.getter
+    def mode(self) -> str:
+        return pulumi.get(self, "mode")
+
+
+@pulumi.output_type
 class PodManifest(dict):
     """
     Pod is a collection of containers that can run on a host. This resource is created by clients and scheduled onto hosts.
 
     This resource waits until its status is ready before registering success
     for create/update, and populating output properties from the current state of the resource.
     The following conditions are used to determine whether the resource creation has
@@ -854,21 +1253,31 @@
 
 
 @pulumi.output_type
 class User(dict):
     def __init__(__self__, *,
                  client_certificate_data: str,
                  client_key_data: str):
+        """
+        :param str client_certificate_data: TODO
+        :param str client_key_data: TODO
+        """
         pulumi.set(__self__, "client_certificate_data", client_certificate_data)
         pulumi.set(__self__, "client_key_data", client_key_data)
 
     @property
     @pulumi.getter(name="clientCertificateData")
     def client_certificate_data(self) -> str:
+        """
+        TODO
+        """
         return pulumi.get(self, "client_certificate_data")
 
     @property
     @pulumi.getter(name="clientKeyData")
     def client_key_data(self) -> str:
+        """
+        TODO
+        """
         return pulumi.get(self, "client_key_data")
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/provider.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,17 +18,19 @@
 from .etcd_configuration import *
 from .etcd_install import *
 from .etcd_service import *
 from .file import *
 from .kube_api_server_install import *
 from .kube_controller_manager_install import *
 from .kube_proxy_install import *
+from .kube_proxy_service import *
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

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/_inputs.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,14 +16,16 @@
     'ContainerdCriPluginConfigurationCniArgs',
     'ContainerdCriPluginConfigurationContainerdRuncOptionsArgs',
     'ContainerdCriPluginConfigurationContainerdRuncArgs',
     'ContainerdCriPluginConfigurationContainerdArgs',
     'ContainerdCriPluginConfigurationArgs',
     'EtcdConfigurationPropsArgs',
     'EtcdNodeArgs',
+    'KubeProxyConfigurationPropsArgs',
+    'KubeletConfigurationPropsArgs',
     'SystemdInstallSectionArgs',
     'SystemdServiceSectionArgs',
     'SystemdUnitSectionArgs',
 ]
 
 @pulumi.input_type
 class CniBridgeIpamArgs:
@@ -442,14 +444,135 @@
 
     @architecture.setter
     def architecture(self, value: Optional[pulumi.Input['Architecture']]):
         pulumi.set(self, "architecture", value)
 
 
 @pulumi.input_type
+class KubeProxyConfigurationPropsArgs:
+    def __init__(__self__, *,
+                 configuration_file_path: pulumi.Input[str],
+                 kube_proxy_path: pulumi.Input[str]):
+        """
+        Props for resources that consume kube-proxy configuration.
+        :param pulumi.Input[str] configuration_file_path: Path to the kube proxy configuration file
+        :param pulumi.Input[str] kube_proxy_path: Path to the kube-proxy binary.
+        """
+        pulumi.set(__self__, "configuration_file_path", configuration_file_path)
+        pulumi.set(__self__, "kube_proxy_path", kube_proxy_path)
+
+    @property
+    @pulumi.getter(name="configurationFilePath")
+    def configuration_file_path(self) -> pulumi.Input[str]:
+        """
+        Path to the kube proxy configuration file
+        """
+        return pulumi.get(self, "configuration_file_path")
+
+    @configuration_file_path.setter
+    def configuration_file_path(self, value: pulumi.Input[str]):
+        pulumi.set(self, "configuration_file_path", value)
+
+    @property
+    @pulumi.getter(name="kubeProxyPath")
+    def kube_proxy_path(self) -> pulumi.Input[str]:
+        """
+        Path to the kube-proxy binary.
+        """
+        return pulumi.get(self, "kube_proxy_path")
+
+    @kube_proxy_path.setter
+    def kube_proxy_path(self, value: pulumi.Input[str]):
+        pulumi.set(self, "kube_proxy_path", value)
+
+
+@pulumi.input_type
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
@@ -556,43 +679,75 @@
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

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/cni_bridge_plugin_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/cni_bridge_plugin_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/cni_loopback_plugin_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/cni_loopback_plugin_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/cni_plugin_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/cni_plugin_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/containerd_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/containerd_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/containerd_install.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/containerd_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/crictl_install.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/crictl_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/download.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/download.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/etcd_install.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/etcd_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/etcd_service.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/etcd_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/file.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/file.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/outputs.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,14 +17,16 @@
     'ContainerdCriPluginConfiguration',
     'ContainerdCriPluginConfigurationCni',
     'ContainerdCriPluginConfigurationContainerd',
     'ContainerdCriPluginConfigurationContainerdRunc',
     'ContainerdCriPluginConfigurationContainerdRuncOptions',
     'EtcdConfigurationProps',
     'EtcdNode',
+    'KubeProxyConfigurationProps',
+    'KubeletConfigurationProps',
     'SystemdInstallSection',
     'SystemdServiceSection',
     'SystemdUnitSection',
 ]
 
 @pulumi.output_type
 class CniBridgeIpam(dict):
@@ -489,14 +491,155 @@
         """
         The CPU architecture of the node.
         """
         return pulumi.get(self, "architecture")
 
 
 @pulumi.output_type
+class KubeProxyConfigurationProps(dict):
+    """
+    Props for resources that consume kube-proxy configuration.
+    """
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "configurationFilePath":
+            suggest = "configuration_file_path"
+        elif key == "kubeProxyPath":
+            suggest = "kube_proxy_path"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in KubeProxyConfigurationProps. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        KubeProxyConfigurationProps.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        KubeProxyConfigurationProps.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 configuration_file_path: str,
+                 kube_proxy_path: str):
+        """
+        Props for resources that consume kube-proxy configuration.
+        :param str configuration_file_path: Path to the kube proxy configuration file
+        :param str kube_proxy_path: Path to the kube-proxy binary.
+        """
+        pulumi.set(__self__, "configuration_file_path", configuration_file_path)
+        pulumi.set(__self__, "kube_proxy_path", kube_proxy_path)
+
+    @property
+    @pulumi.getter(name="configurationFilePath")
+    def configuration_file_path(self) -> str:
+        """
+        Path to the kube proxy configuration file
+        """
+        return pulumi.get(self, "configuration_file_path")
+
+    @property
+    @pulumi.getter(name="kubeProxyPath")
+    def kube_proxy_path(self) -> str:
+        """
+        Path to the kube-proxy binary.
+        """
+        return pulumi.get(self, "kube_proxy_path")
+
+
+@pulumi.output_type
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
@@ -643,43 +786,67 @@
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

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/runc_install.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/runc_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/start_etcd.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/start_etcd.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/static_pod.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/static_pod.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/remote/systemd_service.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/systemd_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tls/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tls/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tls/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tls/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tls/certificate.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tls/certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tls/encryption_key.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tls/encryption_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tls/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tls/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tls/root_ca.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tls/root_ca.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tools/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tools/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/chmod.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tools/chmod.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/curl.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tools/curl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/etcdctl.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tools/etcdctl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/mkdir.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tools/mkdir.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/mktemp.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tools/mktemp.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/mv.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tools/mv.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tools/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/rm.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tools/rm.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/sed.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tools/sed.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/systemctl.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tools/systemctl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/tar.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tools/tar.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/tee.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tools/tee.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way/tools/wget.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tools/wget.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kubernetes_the_hard_way
-Version: 0.0.22
+Version: 0.0.23a1716165280
 Summary: A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way
 License: Apache-2.0
 Project-URL: Repository, https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way
 Keywords: pulumi,command,tls,kubernetes,category/utility,kind/component
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -9,17 +9,21 @@
 pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt
 pulumi_kubernetes_the_hard_way.egg-info/dependency_links.txt
 pulumi_kubernetes_the_hard_way.egg-info/requires.txt
 pulumi_kubernetes_the_hard_way.egg-info/top_level.txt
 pulumi_kubernetes_the_hard_way/config/__init__.py
 pulumi_kubernetes_the_hard_way/config/_enums.py
 pulumi_kubernetes_the_hard_way/config/_inputs.py
+pulumi_kubernetes_the_hard_way/config/get_kube_proxy_configuration.py
 pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py
 pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py
+pulumi_kubernetes_the_hard_way/config/get_kubelet_configuration.py
+pulumi_kubernetes_the_hard_way/config/kube_proxy_configuration.py
 pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py
+pulumi_kubernetes_the_hard_way/config/kubelet_configuration.py
 pulumi_kubernetes_the_hard_way/config/outputs.py
 pulumi_kubernetes_the_hard_way/remote/__init__.py
 pulumi_kubernetes_the_hard_way/remote/_enums.py
 pulumi_kubernetes_the_hard_way/remote/_inputs.py
 pulumi_kubernetes_the_hard_way/remote/cni_bridge_plugin_configuration.py
 pulumi_kubernetes_the_hard_way/remote/cni_loopback_plugin_configuration.py
 pulumi_kubernetes_the_hard_way/remote/cni_plugin_configuration.py
@@ -32,17 +36,19 @@
 pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py
 pulumi_kubernetes_the_hard_way/remote/etcd_install.py
 pulumi_kubernetes_the_hard_way/remote/etcd_service.py
 pulumi_kubernetes_the_hard_way/remote/file.py
 pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py
 pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py
 pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py
+pulumi_kubernetes_the_hard_way/remote/kube_proxy_service.py
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

### Comparing `pulumi_kubernetes_the_hard_way-0.0.22/pyproject.toml` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pyproject.toml`

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
-  version = "0.0.22"
+  version = "0.0.23a1716165280"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Repository = "https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way"
 
 [build-system]
   requires = ["setuptools>=61.0"]
```

