# Comparing `tmp/pulumi_kubernetes_the_hard_way-0.0.23.tar.gz` & `tmp/pulumi_kubernetes_the_hard_way-0.0.23a1716165280.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_kubernetes_the_hard_way-0.0.23.tar", last modified: Mon May 20 00:53:13 2024, max compression
+gzip compressed data, was "pulumi_kubernetes_the_hard_way-0.0.23a1716165280.tar", last modified: Mon May 20 00:37:19 2024, max compression
```

## Comparing `pulumi_kubernetes_the_hard_way-0.0.23.tar` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280.tar`

### file list

```diff
@@ -1,84 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:53:13.095842 pulumi_kubernetes_the_hard_way-0.0.23/
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-20 00:53:13.095842 pulumi_kubernetes_the_hard_way-0.0.23/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:53:13.083841 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/
--rw-------   0 runner    (1001) docker     (127)     4606 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/__init__.py
--rw-------   0 runner    (1001) docker     (127)     9268 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:53:13.083841 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/config/
--rw-------   0 runner    (1001) docker     (127)      496 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/config/__init__.py
--rw-------   0 runner    (1001) docker     (127)      427 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/config/_enums.py
--rw-------   0 runner    (1001) docker     (127)    21648 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/config/_inputs.py
--rw-------   0 runner    (1001) docker     (127)     8728 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py
--rw-------   0 runner    (1001) docker     (127)     3426 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py
--rw-------   0 runner    (1001) docker     (127)     4775 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/config/get_kubelet_configuration.py
--rw-------   0 runner    (1001) docker     (127)    23922 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py
--rw-------   0 runner    (1001) docker     (127)    12667 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/config/kubelet_configuration.py
--rw-------   0 runner    (1001) docker     (127)    38474 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/config/outputs.py
--rw-------   0 runner    (1001) docker     (127)     2783 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/provider.py
--rw-------   0 runner    (1001) docker     (127)      116 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (127)        0 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:53:13.091842 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/
--rw-------   0 runner    (1001) docker     (127)     1147 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/__init__.py
--rw-------   0 runner    (1001) docker     (127)     1095 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/_enums.py
--rw-------   0 runner    (1001) docker     (127)    29297 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    13340 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/cni_bridge_plugin_configuration.py
--rw-------   0 runner    (1001) docker     (127)     8612 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/cni_loopback_plugin_configuration.py
--rw-------   0 runner    (1001) docker     (127)     7575 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/cni_plugin_configuration.py
--rw-------   0 runner    (1001) docker     (127)    19229 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py
--rw-------   0 runner    (1001) docker     (127)     6879 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/containerd_configuration.py
--rw-------   0 runner    (1001) docker     (127)    10255 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/containerd_install.py
--rw-------   0 runner    (1001) docker     (127)    10159 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/crictl_install.py
--rw-------   0 runner    (1001) docker     (127)     8328 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/download.py
--rw-------   0 runner    (1001) docker     (127)    12377 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py
--rw-------   0 runner    (1001) docker     (127)    14905 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py
--rw-------   0 runner    (1001) docker     (127)    10651 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/etcd_install.py
--rw-------   0 runner    (1001) docker     (127)    14696 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/etcd_service.py
--rw-------   0 runner    (1001) docker     (127)     7339 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/file.py
--rw-------   0 runner    (1001) docker     (127)     9708 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py
--rw-------   0 runner    (1001) docker     (127)     9822 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py
--rw-------   0 runner    (1001) docker     (127)     9652 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py
--rw-------   0 runner    (1001) docker     (127)     9708 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py
--rw-------   0 runner    (1001) docker     (127)     9622 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py
--rw-------   0 runner    (1001) docker     (127)     9622 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py
--rw-------   0 runner    (1001) docker     (127)    15819 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/kubelet_service.py
--rw-------   0 runner    (1001) docker     (127)    29099 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/outputs.py
--rw-------   0 runner    (1001) docker     (127)    13390 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py
--rw-------   0 runner    (1001) docker     (127)     9580 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/runc_install.py
--rw-------   0 runner    (1001) docker     (127)     5113 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/start_etcd.py
--rw-------   0 runner    (1001) docker     (127)     7429 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/static_pod.py
--rw-------   0 runner    (1001) docker     (127)    10944 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/systemd_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:53:13.091842 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/tls/
--rw-------   0 runner    (1001) docker     (127)      425 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/tls/__init__.py
--rw-------   0 runner    (1001) docker     (127)     1000 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/tls/_enums.py
--rw-------   0 runner    (1001) docker     (127)     3019 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/tls/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    30597 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/tls/certificate.py
--rw-------   0 runner    (1001) docker     (127)    15919 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py
--rw-------   0 runner    (1001) docker     (127)     4450 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/tls/encryption_key.py
--rw-------   0 runner    (1001) docker     (127)     2983 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/tls/outputs.py
--rw-------   0 runner    (1001) docker     (127)    27130 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/tls/root_ca.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:53:13.095842 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/tools/
--rw-------   0 runner    (1001) docker     (127)      590 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/tools/__init__.py
--rw-------   0 runner    (1001) docker     (127)     3166 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/tools/_enums.py
--rw-------   0 runner    (1001) docker     (127)   108491 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/tools/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    14957 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/tools/chmod.py
--rw-------   0 runner    (1001) docker     (127)    14976 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/tools/curl.py
--rw-------   0 runner    (1001) docker     (127)    15049 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/tools/etcdctl.py
--rw-------   0 runner    (1001) docker     (127)    15189 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py
--rw-------   0 runner    (1001) docker     (127)    14957 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/tools/mkdir.py
--rw-------   0 runner    (1001) docker     (127)    14992 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/tools/mktemp.py
--rw-------   0 runner    (1001) docker     (127)    14852 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/tools/mv.py
--rw-------   0 runner    (1001) docker     (127)    91820 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/tools/outputs.py
--rw-------   0 runner    (1001) docker     (127)    14852 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/tools/rm.py
--rw-------   0 runner    (1001) docker     (127)    14887 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/tools/sed.py
--rw-------   0 runner    (1001) docker     (127)    15119 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/tools/systemctl.py
--rw-------   0 runner    (1001) docker     (127)    14887 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/tools/tar.py
--rw-------   0 runner    (1001) docker     (127)    14907 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/tools/tee.py
--rw-------   0 runner    (1001) docker     (127)    14922 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/tools/wget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:53:13.095842 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-20 00:53:13.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-05-20 00:53:13.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 00:53:13.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-20 00:53:13.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-20 00:53:13.000000 pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way.egg-info/top_level.txt
--rw-------   0 runner    (1001) docker     (127)      888 2024-05-20 00:52:59.000000 pulumi_kubernetes_the_hard_way-0.0.23/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 00:53:13.095842 pulumi_kubernetes_the_hard_way-0.0.23/setup.cfg
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

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/PKG-INFO` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kubernetes_the_hard_way
-Version: 0.0.23
+Version: 0.0.23a1716165280
 Summary: A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way
 License: Apache-2.0
 Project-URL: Repository, https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way
 Keywords: pulumi,command,tls,kubernetes,category/utility,kind/component
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/README.md` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     resource_modules="""
 [
  {
   "pkg": "kubernetes-the-hard-way",
   "mod": "config",
   "fqn": "pulumi_kubernetes_the_hard_way.config",
   "classes": {
+   "kubernetes-the-hard-way:config:KubeProxyConfiguration": "KubeProxyConfiguration",
    "kubernetes-the-hard-way:config:KubeVipManifest": "KubeVipManifest",
    "kubernetes-the-hard-way:config:KubeletConfiguration": "KubeletConfiguration"
   }
  },
  {
   "pkg": "kubernetes-the-hard-way",
   "mod": "remote",
@@ -52,14 +53,15 @@
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
    "kubernetes-the-hard-way:remote:KubeletService": "KubeletService",
    "kubernetes-the-hard-way:remote:ProvisionEtcd": "ProvisionEtcd",
    "kubernetes-the-hard-way:remote:RuncInstall": "RuncInstall",
    "kubernetes-the-hard-way:remote:StartEtcd": "StartEtcd",
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/_utilities.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/config/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/config/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py`

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

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/config/get_kubelet_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/config/get_kubelet_configuration.py`

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

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py`

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

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/config/kubelet_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/config/kubelet_configuration.py`

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

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/config/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/config/outputs.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 from . import outputs
 from ._enums import *
 import pulumi_kubernetes
 
 __all__ = [
     'Cluster',
     'Context',
+    'KubeProxyConfiguration',
+    'KubeProxyConfigurationClientConnection',
     'Kubeconfig',
     'KubeletConfiguration',
     'KubeletConfigurationAuthentication',
     'KubeletConfigurationAuthenticationAnonymous',
     'KubeletConfigurationAuthenticationWebhook',
     'KubeletConfigurationAuthenticationx509',
     'KubeletConfigurationAuthorization',
@@ -81,14 +83,107 @@
         """
         TODO
         """
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
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/provider.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,15 @@
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
 from .kubelet_service import *
 from .provision_etcd import *
 from .runc_install import *
 from .start_etcd import *
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/_inputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     'ContainerdCriPluginConfigurationCniArgs',
     'ContainerdCriPluginConfigurationContainerdRuncOptionsArgs',
     'ContainerdCriPluginConfigurationContainerdRuncArgs',
     'ContainerdCriPluginConfigurationContainerdArgs',
     'ContainerdCriPluginConfigurationArgs',
     'EtcdConfigurationPropsArgs',
     'EtcdNodeArgs',
+    'KubeProxyConfigurationPropsArgs',
     'KubeletConfigurationPropsArgs',
     'SystemdInstallSectionArgs',
     'SystemdServiceSectionArgs',
     'SystemdUnitSectionArgs',
 ]
 
 @pulumi.input_type
@@ -443,14 +444,52 @@
 
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
 class KubeletConfigurationPropsArgs:
     def __init__(__self__, *,
                  configuration_file_path: pulumi.Input[str],
                  kubeconfig_path: pulumi.Input[str],
                  kubelet_path: pulumi.Input[str],
                  register_node: pulumi.Input[bool],
                  v: pulumi.Input[int]):
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/cni_bridge_plugin_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/cni_bridge_plugin_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/cni_loopback_plugin_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/cni_loopback_plugin_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/cni_plugin_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/cni_plugin_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/containerd_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/containerd_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/containerd_install.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/containerd_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/crictl_install.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/crictl_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/download.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/download.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/etcd_install.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/etcd_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/etcd_service.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/etcd_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/file.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/file.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/kubelet_service.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/kubelet_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/outputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     'ContainerdCriPluginConfiguration',
     'ContainerdCriPluginConfigurationCni',
     'ContainerdCriPluginConfigurationContainerd',
     'ContainerdCriPluginConfigurationContainerdRunc',
     'ContainerdCriPluginConfigurationContainerdRuncOptions',
     'EtcdConfigurationProps',
     'EtcdNode',
+    'KubeProxyConfigurationProps',
     'KubeletConfigurationProps',
     'SystemdInstallSection',
     'SystemdServiceSection',
     'SystemdUnitSection',
 ]
 
 @pulumi.output_type
@@ -490,14 +491,66 @@
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
 class KubeletConfigurationProps(dict):
     """
     Props for resources that consume kubelet configuration.
     """
     @staticmethod
     def __key_warning(key: str):
         suggest = None
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/runc_install.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/runc_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/start_etcd.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/start_etcd.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/static_pod.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/static_pod.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/remote/systemd_service.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/remote/systemd_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/tls/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tls/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/tls/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tls/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/tls/certificate.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tls/certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/tls/encryption_key.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tls/encryption_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/tls/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tls/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/tls/root_ca.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tls/root_ca.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/tools/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/tools/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tools/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/tools/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tools/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/tools/chmod.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tools/chmod.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/tools/curl.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tools/curl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/tools/etcdctl.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tools/etcdctl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/tools/mkdir.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tools/mkdir.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/tools/mktemp.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tools/mktemp.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/tools/mv.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tools/mv.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/tools/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tools/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/tools/rm.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tools/rm.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/tools/sed.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tools/sed.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/tools/systemctl.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tools/systemctl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/tools/tar.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tools/tar.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/tools/tee.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tools/tee.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way/tools/wget.py` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way/tools/wget.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kubernetes_the_hard_way
-Version: 0.0.23
+Version: 0.0.23a1716165280
 Summary: A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way
 License: Apache-2.0
 Project-URL: Repository, https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way
 Keywords: pulumi,command,tls,kubernetes,category/utility,kind/component
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -9,17 +9,19 @@
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
 pulumi_kubernetes_the_hard_way/config/get_kubelet_configuration.py
+pulumi_kubernetes_the_hard_way/config/kube_proxy_configuration.py
 pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py
 pulumi_kubernetes_the_hard_way/config/kubelet_configuration.py
 pulumi_kubernetes_the_hard_way/config/outputs.py
 pulumi_kubernetes_the_hard_way/remote/__init__.py
 pulumi_kubernetes_the_hard_way/remote/_enums.py
 pulumi_kubernetes_the_hard_way/remote/_inputs.py
 pulumi_kubernetes_the_hard_way/remote/cni_bridge_plugin_configuration.py
@@ -34,14 +36,15 @@
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
 pulumi_kubernetes_the_hard_way/remote/kubelet_service.py
 pulumi_kubernetes_the_hard_way/remote/outputs.py
 pulumi_kubernetes_the_hard_way/remote/provision_etcd.py
 pulumi_kubernetes_the_hard_way/remote/runc_install.py
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.23/pyproject.toml` & `pulumi_kubernetes_the_hard_way-0.0.23a1716165280/pyproject.toml`

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
-  version = "0.0.23"
+  version = "0.0.23a1716165280"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Repository = "https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way"
 
 [build-system]
   requires = ["setuptools>=61.0"]
```

