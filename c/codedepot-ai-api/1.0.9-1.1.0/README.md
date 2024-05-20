# Comparing `tmp/codedepot_ai_api-1.0.9.tar.gz` & `tmp/codedepot_ai_api-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codedepot_ai_api-1.0.9.tar", last modified: Tue May 14 10:11:26 2024, max compression
+gzip compressed data, was "codedepot_ai_api-1.1.0.tar", last modified: Mon May 20 10:09:49 2024, max compression
```

## Comparing `codedepot_ai_api-1.0.9.tar` & `codedepot_ai_api-1.1.0.tar`

### file list

```diff
@@ -1,57 +1,59 @@
--rw-r--r--   0        0        0     8533 2024-05-13 13:15:22.292626 codedepot_ai_api-1.0.9/README.md
--rw-r--r--   0        0        0     1963 2024-05-13 13:15:22.307433 codedepot_ai_api-1.0.9/ai_api/__init__.py
--rw-r--r--   0        0        0       94 2024-05-13 13:15:22.308947 codedepot_ai_api-1.0.9/ai_api/api/__init__.py
--rw-r--r--   0        0        0   288511 2024-05-13 13:15:22.275189 codedepot_ai_api-1.0.9/ai_api/api/default_api.py
--rw-r--r--   0        0        0    25743 2024-05-13 13:15:22.311594 codedepot_ai_api-1.0.9/ai_api/api_client.py
--rw-r--r--   0        0        0      652 2024-05-13 13:15:22.312585 codedepot_ai_api-1.0.9/ai_api/api_response.py
--rw-r--r--   0        0        0    14732 2024-05-13 13:15:22.305802 codedepot_ai_api-1.0.9/ai_api/configuration.py
--rw-r--r--   0        0        0     5972 2024-05-13 13:15:22.309855 codedepot_ai_api-1.0.9/ai_api/exceptions.py
--rw-r--r--   0        0        0     1445 2024-05-13 13:15:22.308339 codedepot_ai_api-1.0.9/ai_api/models/__init__.py
--rw-r--r--   0        0        0     4826 2024-05-13 13:15:21.992927 codedepot_ai_api-1.0.9/ai_api/models/client_id.py
--rw-r--r--   0        0        0     4850 2024-05-13 13:15:22.001126 codedepot_ai_api-1.0.9/ai_api/models/client_secret.py
--rw-r--r--   0        0        0     2716 2024-05-13 13:15:22.007520 codedepot_ai_api-1.0.9/ai_api/models/cluster_in.py
--rw-r--r--   0        0        0     2908 2024-05-13 13:15:22.015739 codedepot_ai_api-1.0.9/ai_api/models/cluster_out.py
--rw-r--r--   0        0        0     4838 2024-05-13 13:15:22.021001 codedepot_ai_api-1.0.9/ai_api/models/finished_at.py
--rw-r--r--   0        0        0     4897 2024-05-13 13:15:22.038002 codedepot_ai_api-1.0.9/ai_api/models/grant_type.py
--rw-r--r--   0        0        0     2975 2024-05-13 13:15:22.047618 codedepot_ai_api-1.0.9/ai_api/models/http_validation_error.py
--rw-r--r--   0        0        0     4801 2024-05-13 13:15:22.061931 codedepot_ai_api-1.0.9/ai_api/models/id.py
--rw-r--r--   0        0        0     2428 2024-05-13 13:15:22.068266 codedepot_ai_api-1.0.9/ai_api/models/id_out.py
--rw-r--r--   0        0        0     2925 2024-05-13 13:15:22.072251 codedepot_ai_api-1.0.9/ai_api/models/job_instance_in.py
--rw-r--r--   0        0        0     3950 2024-05-13 13:15:22.079265 codedepot_ai_api-1.0.9/ai_api/models/job_instance_out.py
--rw-r--r--   0        0        0     2436 2024-05-13 13:15:22.082664 codedepot_ai_api-1.0.9/ai_api/models/log_out.py
--rw-r--r--   0        0        0     3053 2024-05-13 13:15:22.085576 codedepot_ai_api-1.0.9/ai_api/models/provider.py
--rw-r--r--   0        0        0     2957 2024-05-13 13:15:22.088663 codedepot_ai_api-1.0.9/ai_api/models/provider_out.py
--rw-r--r--   0        0        0     2617 2024-05-13 13:15:22.091543 codedepot_ai_api-1.0.9/ai_api/models/provider_type_out.py
--rw-r--r--   0        0        0     2650 2024-05-13 13:15:22.095035 codedepot_ai_api-1.0.9/ai_api/models/repository_in.py
--rw-r--r--   0        0        0     2796 2024-05-13 13:15:22.108508 codedepot_ai_api-1.0.9/ai_api/models/repository_out.py
--rw-r--r--   0        0        0     2715 2024-05-13 13:15:22.116892 codedepot_ai_api-1.0.9/ai_api/models/ssh_key_in.py
--rw-r--r--   0        0        0     2542 2024-05-13 13:15:22.128261 codedepot_ai_api-1.0.9/ai_api/models/ssh_key_out.py
--rw-r--r--   0        0        0     3076 2024-05-13 13:15:22.132453 codedepot_ai_api-1.0.9/ai_api/models/validation_error.py
--rw-r--r--   0        0        0     4901 2024-05-13 13:15:22.136397 codedepot_ai_api-1.0.9/ai_api/models/validation_error_loc_inner.py
--rw-r--r--   0        0        0        0 2024-05-13 13:15:22.303739 codedepot_ai_api-1.0.9/ai_api/py.typed
--rw-r--r--   0        0        0     9224 2024-05-13 13:15:22.313410 codedepot_ai_api-1.0.9/ai_api/rest.py
--rw-r--r--   0        0        0     1835 2024-05-14 10:11:26.745293 codedepot_ai_api-1.0.9/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-13 13:15:22.310466 codedepot_ai_api-1.0.9/test/__init__.py
--rw-r--r--   0        0        0     1273 2024-05-13 13:15:21.995760 codedepot_ai_api-1.0.9/test/test_client_id.py
--rw-r--r--   0        0        0     1321 2024-05-13 13:15:22.002246 codedepot_ai_api-1.0.9/test/test_client_secret.py
--rw-r--r--   0        0        0     1614 2024-05-13 13:15:22.009050 codedepot_ai_api-1.0.9/test/test_cluster_in.py
--rw-r--r--   0        0        0     2068 2024-05-13 13:15:22.016938 codedepot_ai_api-1.0.9/test/test_cluster_out.py
--rw-r--r--   0        0        0     5920 2024-05-13 13:15:22.277431 codedepot_ai_api-1.0.9/test/test_default_api.py
--rw-r--r--   0        0        0     1297 2024-05-13 13:15:22.022203 codedepot_ai_api-1.0.9/test/test_finished_at.py
--rw-r--r--   0        0        0     1285 2024-05-13 13:15:22.039775 codedepot_ai_api-1.0.9/test/test_grant_type.py
--rw-r--r--   0        0        0     1692 2024-05-13 13:15:22.050867 codedepot_ai_api-1.0.9/test/test_http_validation_error.py
--rw-r--r--   0        0        0     1200 2024-05-13 13:15:22.064542 codedepot_ai_api-1.0.9/test/test_id.py
--rw-r--r--   0        0        0     1286 2024-05-13 13:15:22.069042 codedepot_ai_api-1.0.9/test/test_id_out.py
--rw-r--r--   0        0        0     1723 2024-05-13 13:15:22.074921 codedepot_ai_api-1.0.9/test/test_job_instance_in.py
--rw-r--r--   0        0        0     2937 2024-05-13 13:15:22.080109 codedepot_ai_api-1.0.9/test/test_job_instance_out.py
--rw-r--r--   0        0        0     1300 2024-05-13 13:15:22.083287 codedepot_ai_api-1.0.9/test/test_log_out.py
--rw-r--r--   0        0        0     1562 2024-05-13 13:15:22.086190 codedepot_ai_api-1.0.9/test/test_provider.py
--rw-r--r--   0        0        0     1770 2024-05-13 13:15:22.089295 codedepot_ai_api-1.0.9/test/test_provider_out.py
--rw-r--r--   0        0        0     1519 2024-05-13 13:15:22.092147 codedepot_ai_api-1.0.9/test/test_provider_type_out.py
--rw-r--r--   0        0        0     1510 2024-05-13 13:15:22.095935 codedepot_ai_api-1.0.9/test/test_repository_in.py
--rw-r--r--   0        0        0     1628 2024-05-13 13:15:22.110380 codedepot_ai_api-1.0.9/test/test_repository_out.py
--rw-r--r--   0        0        0     1525 2024-05-13 13:15:22.119204 codedepot_ai_api-1.0.9/test/test_ssh_key_in.py
--rw-r--r--   0        0        0     1403 2024-05-13 13:15:22.129420 codedepot_ai_api-1.0.9/test/test_ssh_key_out.py
--rw-r--r--   0        0        0     1606 2024-05-13 13:15:22.133303 codedepot_ai_api-1.0.9/test/test_validation_error.py
--rw-r--r--   0        0        0     1455 2024-05-13 13:15:22.137269 codedepot_ai_api-1.0.9/test/test_validation_error_loc_inner.py
--rw-r--r--   0        0        0     9225 1970-01-01 00:00:00.000000 codedepot_ai_api-1.0.9/PKG-INFO
+-rw-r--r--   0        0        0     8517 2024-05-19 18:39:54.421229 codedepot_ai_api-1.1.0/README.md
+-rw-r--r--   0        0        0     1936 2024-05-19 18:39:54.442733 codedepot_ai_api-1.1.0/ai_api/__init__.py
+-rw-r--r--   0        0        0       94 2024-05-19 18:39:54.446050 codedepot_ai_api-1.1.0/ai_api/api/__init__.py
+-rw-r--r--   0        0        0   288582 2024-05-19 18:39:54.404483 codedepot_ai_api-1.1.0/ai_api/api/default_api.py
+-rw-r--r--   0        0        0    25743 2024-05-19 18:39:54.453757 codedepot_ai_api-1.1.0/ai_api/api_client.py
+-rw-r--r--   0        0        0      652 2024-05-19 18:39:54.454496 codedepot_ai_api-1.1.0/ai_api/api_response.py
+-rw-r--r--   0        0        0    14732 2024-05-19 18:39:54.441257 codedepot_ai_api-1.1.0/ai_api/configuration.py
+-rw-r--r--   0        0        0     5972 2024-05-19 18:39:54.448211 codedepot_ai_api-1.1.0/ai_api/exceptions.py
+-rw-r--r--   0        0        0     1418 2024-05-19 18:39:54.444787 codedepot_ai_api-1.1.0/ai_api/models/__init__.py
+-rw-r--r--   0        0        0     4826 2024-05-19 18:39:54.135680 codedepot_ai_api-1.1.0/ai_api/models/client_id.py
+-rw-r--r--   0        0        0     4850 2024-05-19 18:39:54.145871 codedepot_ai_api-1.1.0/ai_api/models/client_secret.py
+-rw-r--r--   0        0        0     2809 2024-05-19 18:39:54.156207 codedepot_ai_api-1.1.0/ai_api/models/cluster_in.py
+-rw-r--r--   0        0        0     2823 2024-05-19 18:39:54.163963 codedepot_ai_api-1.1.0/ai_api/models/cluster_out.py
+-rw-r--r--   0        0        0     4838 2024-05-19 18:39:54.171198 codedepot_ai_api-1.1.0/ai_api/models/finished_at.py
+-rw-r--r--   0        0        0     4897 2024-05-19 18:39:54.178740 codedepot_ai_api-1.1.0/ai_api/models/grant_type.py
+-rw-r--r--   0        0        0     2975 2024-05-19 18:39:54.184573 codedepot_ai_api-1.1.0/ai_api/models/http_validation_error.py
+-rw-r--r--   0        0        0     4801 2024-05-19 13:16:34.127325 codedepot_ai_api-1.1.0/ai_api/models/id.py
+-rw-r--r--   0        0        0     2428 2024-05-19 18:39:54.190674 codedepot_ai_api-1.1.0/ai_api/models/id_out.py
+-rw-r--r--   0        0        0     2925 2024-05-19 18:39:54.195110 codedepot_ai_api-1.1.0/ai_api/models/job_instance_in.py
+-rw-r--r--   0        0        0     3865 2024-05-19 18:39:54.199357 codedepot_ai_api-1.1.0/ai_api/models/job_instance_out.py
+-rw-r--r--   0        0        0     2436 2024-05-19 18:39:54.205347 codedepot_ai_api-1.1.0/ai_api/models/log_out.py
+-rw-r--r--   0        0        0     3053 2024-05-19 13:16:34.130306 codedepot_ai_api-1.1.0/ai_api/models/provider.py
+-rw-r--r--   0        0        0     2735 2024-05-19 18:39:54.211724 codedepot_ai_api-1.1.0/ai_api/models/provider_in.py
+-rw-r--r--   0        0        0     2957 2024-05-19 18:39:54.216491 codedepot_ai_api-1.1.0/ai_api/models/provider_out.py
+-rw-r--r--   0        0        0     2617 2024-05-19 18:39:54.221990 codedepot_ai_api-1.1.0/ai_api/models/provider_type_out.py
+-rw-r--r--   0        0        0     2650 2024-05-19 18:39:54.227193 codedepot_ai_api-1.1.0/ai_api/models/repository_in.py
+-rw-r--r--   0        0        0     2796 2024-05-19 18:39:54.234862 codedepot_ai_api-1.1.0/ai_api/models/repository_out.py
+-rw-r--r--   0        0        0     2715 2024-05-19 18:39:54.239276 codedepot_ai_api-1.1.0/ai_api/models/ssh_key_in.py
+-rw-r--r--   0        0        0     2542 2024-05-19 18:39:54.243548 codedepot_ai_api-1.1.0/ai_api/models/ssh_key_out.py
+-rw-r--r--   0        0        0     3076 2024-05-19 18:39:54.247984 codedepot_ai_api-1.1.0/ai_api/models/validation_error.py
+-rw-r--r--   0        0        0     4901 2024-05-19 18:39:54.252451 codedepot_ai_api-1.1.0/ai_api/models/validation_error_loc_inner.py
+-rw-r--r--   0        0        0        0 2024-05-19 18:39:54.436868 codedepot_ai_api-1.1.0/ai_api/py.typed
+-rw-r--r--   0        0        0     9224 2024-05-19 18:39:54.456858 codedepot_ai_api-1.1.0/ai_api/rest.py
+-rw-r--r--   0        0        0     1835 2024-05-20 10:09:49.145282 codedepot_ai_api-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-19 18:39:54.448918 codedepot_ai_api-1.1.0/test/__init__.py
+-rw-r--r--   0        0        0     1273 2024-05-19 13:16:34.152650 codedepot_ai_api-1.1.0/test/test_client_id.py
+-rw-r--r--   0        0        0     1321 2024-05-19 13:16:34.152879 codedepot_ai_api-1.1.0/test/test_client_secret.py
+-rw-r--r--   0        0        0     1614 2024-05-19 13:16:34.153049 codedepot_ai_api-1.1.0/test/test_cluster_in.py
+-rw-r--r--   0        0        0     2068 2024-05-19 13:16:34.153880 codedepot_ai_api-1.1.0/test/test_cluster_out.py
+-rw-r--r--   0        0        0     5920 2024-05-19 13:16:34.154057 codedepot_ai_api-1.1.0/test/test_default_api.py
+-rw-r--r--   0        0        0     1297 2024-05-19 13:16:34.154185 codedepot_ai_api-1.1.0/test/test_finished_at.py
+-rw-r--r--   0        0        0     1285 2024-05-19 13:16:34.154304 codedepot_ai_api-1.1.0/test/test_grant_type.py
+-rw-r--r--   0        0        0     1692 2024-05-19 13:16:34.154429 codedepot_ai_api-1.1.0/test/test_http_validation_error.py
+-rw-r--r--   0        0        0     1200 2024-05-19 13:16:34.154540 codedepot_ai_api-1.1.0/test/test_id.py
+-rw-r--r--   0        0        0     1286 2024-05-19 13:16:34.154815 codedepot_ai_api-1.1.0/test/test_id_out.py
+-rw-r--r--   0        0        0     1723 2024-05-19 13:16:34.155028 codedepot_ai_api-1.1.0/test/test_job_instance_in.py
+-rw-r--r--   0        0        0     2937 2024-05-19 13:16:34.155330 codedepot_ai_api-1.1.0/test/test_job_instance_out.py
+-rw-r--r--   0        0        0     1300 2024-05-19 13:16:34.155501 codedepot_ai_api-1.1.0/test/test_log_out.py
+-rw-r--r--   0        0        0     1562 2024-05-19 13:16:34.155641 codedepot_ai_api-1.1.0/test/test_provider.py
+-rw-r--r--   0        0        0     1554 2024-05-19 13:19:47.158788 codedepot_ai_api-1.1.0/test/test_provider_in.py
+-rw-r--r--   0        0        0     1770 2024-05-19 13:16:34.155836 codedepot_ai_api-1.1.0/test/test_provider_out.py
+-rw-r--r--   0        0        0     1519 2024-05-19 13:16:34.156049 codedepot_ai_api-1.1.0/test/test_provider_type_out.py
+-rw-r--r--   0        0        0     1510 2024-05-19 13:16:34.156238 codedepot_ai_api-1.1.0/test/test_repository_in.py
+-rw-r--r--   0        0        0     1628 2024-05-19 13:16:34.159478 codedepot_ai_api-1.1.0/test/test_repository_out.py
+-rw-r--r--   0        0        0     1525 2024-05-19 13:16:34.159597 codedepot_ai_api-1.1.0/test/test_ssh_key_in.py
+-rw-r--r--   0        0        0     1403 2024-05-19 13:16:34.159886 codedepot_ai_api-1.1.0/test/test_ssh_key_out.py
+-rw-r--r--   0        0        0     1606 2024-05-19 13:16:34.160174 codedepot_ai_api-1.1.0/test/test_validation_error.py
+-rw-r--r--   0        0        0     1455 2024-05-19 13:16:34.160346 codedepot_ai_api-1.1.0/test/test_validation_error_loc_inner.py
+-rw-r--r--   0        0        0     9209 1970-01-01 00:00:00.000000 codedepot_ai_api-1.1.0/PKG-INFO
```

### Comparing `codedepot_ai_api-1.0.9/README.md` & `codedepot_ai_api-1.1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -127,20 +127,19 @@
  - [ClientId](docs/ClientId.md)
  - [ClientSecret](docs/ClientSecret.md)
  - [ClusterIn](docs/ClusterIn.md)
  - [ClusterOut](docs/ClusterOut.md)
  - [FinishedAt](docs/FinishedAt.md)
  - [GrantType](docs/GrantType.md)
  - [HTTPValidationError](docs/HTTPValidationError.md)
- - [Id](docs/Id.md)
  - [IdOut](docs/IdOut.md)
  - [JobInstanceIn](docs/JobInstanceIn.md)
  - [JobInstanceOut](docs/JobInstanceOut.md)
  - [LogOut](docs/LogOut.md)
- - [Provider](docs/Provider.md)
+ - [ProviderIn](docs/ProviderIn.md)
  - [ProviderOut](docs/ProviderOut.md)
  - [ProviderTypeOut](docs/ProviderTypeOut.md)
  - [RepositoryIn](docs/RepositoryIn.md)
  - [RepositoryOut](docs/RepositoryOut.md)
  - [SshKeyIn](docs/SshKeyIn.md)
  - [SshKeyOut](docs/SshKeyOut.md)
  - [ValidationError](docs/ValidationError.md)
```

### Comparing `codedepot_ai_api-1.0.9/ai_api/__init__.py` & `codedepot_ai_api-1.1.0/ai_api/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,20 +34,19 @@
 from ai_api.models.client_id import ClientId
 from ai_api.models.client_secret import ClientSecret
 from ai_api.models.cluster_in import ClusterIn
 from ai_api.models.cluster_out import ClusterOut
 from ai_api.models.finished_at import FinishedAt
 from ai_api.models.grant_type import GrantType
 from ai_api.models.http_validation_error import HTTPValidationError
-from ai_api.models.id import Id
 from ai_api.models.id_out import IdOut
 from ai_api.models.job_instance_in import JobInstanceIn
 from ai_api.models.job_instance_out import JobInstanceOut
 from ai_api.models.log_out import LogOut
-from ai_api.models.provider import Provider
+from ai_api.models.provider_in import ProviderIn
 from ai_api.models.provider_out import ProviderOut
 from ai_api.models.provider_type_out import ProviderTypeOut
 from ai_api.models.repository_in import RepositoryIn
 from ai_api.models.repository_out import RepositoryOut
 from ai_api.models.ssh_key_in import SshKeyIn
 from ai_api.models.ssh_key_out import SshKeyOut
 from ai_api.models.validation_error import ValidationError
```

### Comparing `codedepot_ai_api-1.0.9/ai_api/api/default_api.py` & `codedepot_ai_api-1.1.0/ai_api/api/default_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from ai_api.models.cluster_in import ClusterIn
 from ai_api.models.cluster_out import ClusterOut
 from ai_api.models.grant_type import GrantType
 from ai_api.models.id_out import IdOut
 from ai_api.models.job_instance_in import JobInstanceIn
 from ai_api.models.job_instance_out import JobInstanceOut
 from ai_api.models.log_out import LogOut
-from ai_api.models.provider import Provider
+from ai_api.models.provider_in import ProviderIn
 from ai_api.models.provider_out import ProviderOut
 from ai_api.models.provider_type_out import ProviderTypeOut
 from ai_api.models.repository_in import RepositoryIn
 from ai_api.models.repository_out import RepositoryOut
 from ai_api.models.ssh_key_in import SshKeyIn
 from ai_api.models.ssh_key_out import SshKeyOut
 
@@ -854,15 +854,15 @@
 
 
 
 
     @validate_call
     def create_provider_providers_post(
         self,
-        provider: Provider,
+        provider_in: ProviderIn,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -871,16 +871,16 @@
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ProviderOut:
         """Create Provider
 
 
-        :param provider: (required)
-        :type provider: Provider
+        :param provider_in: (required)
+        :type provider_in: ProviderIn
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -896,15 +896,15 @@
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._create_provider_providers_post_serialize(
-            provider=provider,
+            provider_in=provider_in,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -921,15 +921,15 @@
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
     def create_provider_providers_post_with_http_info(
         self,
-        provider: Provider,
+        provider_in: ProviderIn,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -938,16 +938,16 @@
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[ProviderOut]:
         """Create Provider
 
 
-        :param provider: (required)
-        :type provider: Provider
+        :param provider_in: (required)
+        :type provider_in: ProviderIn
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -963,15 +963,15 @@
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._create_provider_providers_post_serialize(
-            provider=provider,
+            provider_in=provider_in,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -988,15 +988,15 @@
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
     def create_provider_providers_post_without_preload_content(
         self,
-        provider: Provider,
+        provider_in: ProviderIn,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -1005,16 +1005,16 @@
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """Create Provider
 
 
-        :param provider: (required)
-        :type provider: Provider
+        :param provider_in: (required)
+        :type provider_in: ProviderIn
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1030,15 +1030,15 @@
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._create_provider_providers_post_serialize(
-            provider=provider,
+            provider_in=provider_in,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -1050,15 +1050,15 @@
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
     def _create_provider_providers_post_serialize(
         self,
-        provider,
+        provider_in,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -1074,16 +1074,16 @@
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
-        if provider is not None:
-            _body_params = provider
+        if provider_in is not None:
+            _body_params = provider_in
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 'application/json'
             ]
```

### Comparing `codedepot_ai_api-1.0.9/ai_api/api_client.py` & `codedepot_ai_api-1.1.0/ai_api/api_client.py`

 * *Files identical despite different names*

### Comparing `codedepot_ai_api-1.0.9/ai_api/api_response.py` & `codedepot_ai_api-1.1.0/ai_api/api_response.py`

 * *Files identical despite different names*

### Comparing `codedepot_ai_api-1.0.9/ai_api/configuration.py` & `codedepot_ai_api-1.1.0/ai_api/configuration.py`

 * *Files identical despite different names*

### Comparing `codedepot_ai_api-1.0.9/ai_api/exceptions.py` & `codedepot_ai_api-1.1.0/ai_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `codedepot_ai_api-1.0.9/ai_api/models/__init__.py` & `codedepot_ai_api-1.1.0/ai_api/models/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,20 +17,19 @@
 from ai_api.models.client_id import ClientId
 from ai_api.models.client_secret import ClientSecret
 from ai_api.models.cluster_in import ClusterIn
 from ai_api.models.cluster_out import ClusterOut
 from ai_api.models.finished_at import FinishedAt
 from ai_api.models.grant_type import GrantType
 from ai_api.models.http_validation_error import HTTPValidationError
-from ai_api.models.id import Id
 from ai_api.models.id_out import IdOut
 from ai_api.models.job_instance_in import JobInstanceIn
 from ai_api.models.job_instance_out import JobInstanceOut
 from ai_api.models.log_out import LogOut
-from ai_api.models.provider import Provider
+from ai_api.models.provider_in import ProviderIn
 from ai_api.models.provider_out import ProviderOut
 from ai_api.models.provider_type_out import ProviderTypeOut
 from ai_api.models.repository_in import RepositoryIn
 from ai_api.models.repository_out import RepositoryOut
 from ai_api.models.ssh_key_in import SshKeyIn
 from ai_api.models.ssh_key_out import SshKeyOut
 from ai_api.models.validation_error import ValidationError
```

### Comparing `codedepot_ai_api-1.0.9/ai_api/models/client_id.py` & `codedepot_ai_api-1.1.0/ai_api/models/client_id.py`

 * *Files identical despite different names*

### Comparing `codedepot_ai_api-1.0.9/ai_api/models/client_secret.py` & `codedepot_ai_api-1.1.0/ai_api/models/client_secret.py`

 * *Files identical despite different names*

### Comparing `codedepot_ai_api-1.0.9/ai_api/models/cluster_in.py` & `codedepot_ai_api-1.1.0/ai_api/models/ssh_key_in.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,28 +13,28 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictInt, StrictStr
+from pydantic import BaseModel, ConfigDict, StrictStr
 from typing import Any, ClassVar, Dict, List
 from typing import Optional, Set
 from typing_extensions import Self
 
-class ClusterIn(BaseModel):
+class SshKeyIn(BaseModel):
     """
-    ClusterIn
+    SshKeyIn
     """ # noqa: E501
     name: StrictStr
     userlogin: StrictStr
-    provider_id: StrictInt
-    nodes: List[StrictStr]
-    __properties: ClassVar[List[str]] = ["name", "userlogin", "provider_id", "nodes"]
+    public_key: StrictStr
+    private_key: StrictStr
+    __properties: ClassVar[List[str]] = ["name", "userlogin", "public_key", "private_key"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -46,15 +46,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of ClusterIn from a JSON string"""
+        """Create an instance of SshKeyIn from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -71,23 +71,23 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of ClusterIn from a dict"""
+        """Create an instance of SshKeyIn from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "name": obj.get("name"),
             "userlogin": obj.get("userlogin"),
-            "provider_id": obj.get("provider_id"),
-            "nodes": obj.get("nodes")
+            "public_key": obj.get("public_key"),
+            "private_key": obj.get("private_key")
         })
         return _obj
```

### Comparing `codedepot_ai_api-1.0.9/ai_api/models/cluster_out.py` & `codedepot_ai_api-1.1.0/ai_api/models/provider_out.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,28 +13,28 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictStr
+from pydantic import BaseModel, ConfigDict, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List
-from ai_api.models.provider_out import ProviderOut
+from ai_api.models.provider_type_out import ProviderTypeOut
 from typing import Optional, Set
 from typing_extensions import Self
 
-class ClusterOut(BaseModel):
+class ProviderOut(BaseModel):
     """
-    ClusterOut
+    ProviderOut
     """ # noqa: E501
+    id: StrictInt
     name: StrictStr
-    userlogin: StrictStr
-    provider: ProviderOut
-    __properties: ClassVar[List[str]] = ["name", "userlogin", "provider"]
+    provider_type: ProviderTypeOut
+    __properties: ClassVar[List[str]] = ["id", "name", "provider_type"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -46,15 +46,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of ClusterOut from a JSON string"""
+        """Create an instance of ProviderOut from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -67,29 +67,29 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of provider
-        if self.provider:
-            _dict['provider'] = self.provider.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of provider_type
+        if self.provider_type:
+            _dict['provider_type'] = self.provider_type.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of ClusterOut from a dict"""
+        """Create an instance of ProviderOut from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
+            "id": obj.get("id"),
             "name": obj.get("name"),
-            "userlogin": obj.get("userlogin"),
-            "provider": ProviderOut.from_dict(obj["provider"]) if obj.get("provider") is not None else None
+            "provider_type": ProviderTypeOut.from_dict(obj["provider_type"]) if obj.get("provider_type") is not None else None
         })
         return _obj
```

### Comparing `codedepot_ai_api-1.0.9/ai_api/models/finished_at.py` & `codedepot_ai_api-1.1.0/ai_api/models/finished_at.py`

 * *Files identical despite different names*

### Comparing `codedepot_ai_api-1.0.9/ai_api/models/grant_type.py` & `codedepot_ai_api-1.1.0/ai_api/models/grant_type.py`

 * *Files identical despite different names*

### Comparing `codedepot_ai_api-1.0.9/ai_api/models/http_validation_error.py` & `codedepot_ai_api-1.1.0/ai_api/models/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `codedepot_ai_api-1.0.9/ai_api/models/id.py` & `codedepot_ai_api-1.1.0/ai_api/models/id.py`

 * *Files identical despite different names*

### Comparing `codedepot_ai_api-1.0.9/ai_api/models/id_out.py` & `codedepot_ai_api-1.1.0/ai_api/models/id_out.py`

 * *Files identical despite different names*

### Comparing `codedepot_ai_api-1.0.9/ai_api/models/job_instance_in.py` & `codedepot_ai_api-1.1.0/ai_api/models/job_instance_in.py`

 * *Files identical despite different names*

### Comparing `codedepot_ai_api-1.0.9/ai_api/models/job_instance_out.py` & `codedepot_ai_api-1.1.0/ai_api/models/job_instance_out.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,20 +30,19 @@
     """ # noqa: E501
     id: StrictInt
     name: StrictStr
     job_name: StrictStr
     repository_url: StrictStr
     starting_commit: StrictStr
     cluster_name: StrictStr
-    userlogin: StrictStr
     status: StrictStr
     started_at: StrictStr
     finished_at: Optional[FinishedAt] = None
     cluster: ClusterOut
-    __properties: ClassVar[List[str]] = ["id", "name", "job_name", "repository_url", "starting_commit", "cluster_name", "userlogin", "status", "started_at", "finished_at", "cluster"]
+    __properties: ClassVar[List[str]] = ["id", "name", "job_name", "repository_url", "starting_commit", "cluster_name", "status", "started_at", "finished_at", "cluster"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -100,15 +99,14 @@
         _obj = cls.model_validate({
             "id": obj.get("id"),
             "name": obj.get("name"),
             "job_name": obj.get("job_name"),
             "repository_url": obj.get("repository_url"),
             "starting_commit": obj.get("starting_commit"),
             "cluster_name": obj.get("cluster_name"),
-            "userlogin": obj.get("userlogin"),
             "status": obj.get("status"),
             "started_at": obj.get("started_at"),
             "finished_at": FinishedAt.from_dict(obj["finished_at"]) if obj.get("finished_at") is not None else None,
             "cluster": ClusterOut.from_dict(obj["cluster"]) if obj.get("cluster") is not None else None
         })
         return _obj
```

### Comparing `codedepot_ai_api-1.0.9/ai_api/models/log_out.py` & `codedepot_ai_api-1.1.0/ai_api/models/log_out.py`

 * *Files identical despite different names*

### Comparing `codedepot_ai_api-1.0.9/ai_api/models/provider.py` & `codedepot_ai_api-1.1.0/ai_api/models/provider.py`

 * *Files identical despite different names*

### Comparing `codedepot_ai_api-1.0.9/ai_api/models/provider_out.py` & `codedepot_ai_api-1.1.0/ai_api/models/cluster_out.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,28 +13,27 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictInt, StrictStr
+from pydantic import BaseModel, ConfigDict, StrictStr
 from typing import Any, ClassVar, Dict, List
-from ai_api.models.provider_type_out import ProviderTypeOut
+from ai_api.models.provider_out import ProviderOut
 from typing import Optional, Set
 from typing_extensions import Self
 
-class ProviderOut(BaseModel):
+class ClusterOut(BaseModel):
     """
-    ProviderOut
+    ClusterOut
     """ # noqa: E501
-    id: StrictInt
     name: StrictStr
-    provider_type: ProviderTypeOut
-    __properties: ClassVar[List[str]] = ["id", "name", "provider_type"]
+    provider: ProviderOut
+    __properties: ClassVar[List[str]] = ["name", "provider"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -46,15 +45,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of ProviderOut from a JSON string"""
+        """Create an instance of ClusterOut from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -67,29 +66,28 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of provider_type
-        if self.provider_type:
-            _dict['provider_type'] = self.provider_type.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of provider
+        if self.provider:
+            _dict['provider'] = self.provider.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of ProviderOut from a dict"""
+        """Create an instance of ClusterOut from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "id": obj.get("id"),
             "name": obj.get("name"),
-            "provider_type": ProviderTypeOut.from_dict(obj["provider_type"]) if obj.get("provider_type") is not None else None
+            "provider": ProviderOut.from_dict(obj["provider"]) if obj.get("provider") is not None else None
         })
         return _obj
```

### Comparing `codedepot_ai_api-1.0.9/ai_api/models/provider_type_out.py` & `codedepot_ai_api-1.1.0/ai_api/models/provider_type_out.py`

 * *Files identical despite different names*

### Comparing `codedepot_ai_api-1.0.9/ai_api/models/repository_in.py` & `codedepot_ai_api-1.1.0/ai_api/models/repository_in.py`

 * *Files identical despite different names*

### Comparing `codedepot_ai_api-1.0.9/ai_api/models/repository_out.py` & `codedepot_ai_api-1.1.0/ai_api/models/repository_out.py`

 * *Files identical despite different names*

### Comparing `codedepot_ai_api-1.0.9/ai_api/models/ssh_key_in.py` & `codedepot_ai_api-1.1.0/ai_api/models/validation_error.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,26 +15,26 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictStr
 from typing import Any, ClassVar, Dict, List
+from ai_api.models.validation_error_loc_inner import ValidationErrorLocInner
 from typing import Optional, Set
 from typing_extensions import Self
 
-class SshKeyIn(BaseModel):
+class ValidationError(BaseModel):
     """
-    SshKeyIn
+    ValidationError
     """ # noqa: E501
-    name: StrictStr
-    userlogin: StrictStr
-    public_key: StrictStr
-    private_key: StrictStr
-    __properties: ClassVar[List[str]] = ["name", "userlogin", "public_key", "private_key"]
+    loc: List[ValidationErrorLocInner]
+    msg: StrictStr
+    type: StrictStr
+    __properties: ClassVar[List[str]] = ["loc", "msg", "type"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -46,15 +46,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of SshKeyIn from a JSON string"""
+        """Create an instance of ValidationError from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -67,27 +67,33 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
+        # override the default output from pydantic by calling `to_dict()` of each item in loc (list)
+        _items = []
+        if self.loc:
+            for _item in self.loc:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['loc'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of SshKeyIn from a dict"""
+        """Create an instance of ValidationError from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "name": obj.get("name"),
-            "userlogin": obj.get("userlogin"),
-            "public_key": obj.get("public_key"),
-            "private_key": obj.get("private_key")
+            "loc": [ValidationErrorLocInner.from_dict(_item) for _item in obj["loc"]] if obj.get("loc") is not None else None,
+            "msg": obj.get("msg"),
+            "type": obj.get("type")
         })
         return _obj
```

### Comparing `codedepot_ai_api-1.0.9/ai_api/models/ssh_key_out.py` & `codedepot_ai_api-1.1.0/ai_api/models/ssh_key_out.py`

 * *Files identical despite different names*

### Comparing `codedepot_ai_api-1.0.9/ai_api/models/validation_error.py` & `codedepot_ai_api-1.1.0/ai_api/models/provider_in.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,26 +15,26 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictStr
 from typing import Any, ClassVar, Dict, List
-from ai_api.models.validation_error_loc_inner import ValidationErrorLocInner
 from typing import Optional, Set
 from typing_extensions import Self
 
-class ValidationError(BaseModel):
+class ProviderIn(BaseModel):
     """
-    ValidationError
+    ProviderIn
     """ # noqa: E501
-    loc: List[ValidationErrorLocInner]
-    msg: StrictStr
-    type: StrictStr
-    __properties: ClassVar[List[str]] = ["loc", "msg", "type"]
+    name: StrictStr
+    provider_type: StrictStr
+    credentials: StrictStr
+    userlogin: StrictStr
+    __properties: ClassVar[List[str]] = ["name", "provider_type", "credentials", "userlogin"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -46,15 +46,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of ValidationError from a JSON string"""
+        """Create an instance of ProviderIn from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -67,33 +67,27 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in loc (list)
-        _items = []
-        if self.loc:
-            for _item in self.loc:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['loc'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of ValidationError from a dict"""
+        """Create an instance of ProviderIn from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "loc": [ValidationErrorLocInner.from_dict(_item) for _item in obj["loc"]] if obj.get("loc") is not None else None,
-            "msg": obj.get("msg"),
-            "type": obj.get("type")
+            "name": obj.get("name"),
+            "provider_type": obj.get("provider_type"),
+            "credentials": obj.get("credentials"),
+            "userlogin": obj.get("userlogin")
         })
         return _obj
```

### Comparing `codedepot_ai_api-1.0.9/ai_api/models/validation_error_loc_inner.py` & `codedepot_ai_api-1.1.0/ai_api/models/validation_error_loc_inner.py`

 * *Files identical despite different names*

### Comparing `codedepot_ai_api-1.0.9/ai_api/rest.py` & `codedepot_ai_api-1.1.0/ai_api/rest.py`

 * *Files identical despite different names*

### Comparing `codedepot_ai_api-1.0.9/pyproject.toml` & `codedepot_ai_api-1.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     "typing-extensions>=4.7.1",
     "pydantic >= 2",
     "python-dateutil",
     "typing-extensions >= 4.7.1",
     "urllib3 >= 1.25.3, < 2.1.0",
 ]
 name = "codedepot-ai-api"
-version = "1.0.9"
+version = "1.1.0"
 description = "AI API"
 readme = "README.md"
 keywords = [
     "OpenAPI",
     "OpenAPI-Generator",
     "FastAPI",
 ]
```

### Comparing `codedepot_ai_api-1.0.9/test/test_client_id.py` & `codedepot_ai_api-1.1.0/test/test_client_id.py`

 * *Files identical despite different names*

### Comparing `codedepot_ai_api-1.0.9/test/test_client_secret.py` & `codedepot_ai_api-1.1.0/test/test_client_secret.py`

 * *Files identical despite different names*

### Comparing `codedepot_ai_api-1.0.9/test/test_cluster_in.py` & `codedepot_ai_api-1.1.0/test/test_cluster_in.py`

 * *Files identical despite different names*

### Comparing `codedepot_ai_api-1.0.9/test/test_cluster_out.py` & `codedepot_ai_api-1.1.0/test/test_cluster_out.py`

 * *Files identical despite different names*

### Comparing `codedepot_ai_api-1.0.9/test/test_default_api.py` & `codedepot_ai_api-1.1.0/test/test_default_api.py`

 * *Files identical despite different names*

### Comparing `codedepot_ai_api-1.0.9/test/test_finished_at.py` & `codedepot_ai_api-1.1.0/test/test_finished_at.py`

 * *Files identical despite different names*

### Comparing `codedepot_ai_api-1.0.9/test/test_grant_type.py` & `codedepot_ai_api-1.1.0/test/test_grant_type.py`

 * *Files identical despite different names*

### Comparing `codedepot_ai_api-1.0.9/test/test_http_validation_error.py` & `codedepot_ai_api-1.1.0/test/test_http_validation_error.py`

 * *Files identical despite different names*

### Comparing `codedepot_ai_api-1.0.9/test/test_id.py` & `codedepot_ai_api-1.1.0/test/test_id.py`

 * *Files identical despite different names*

### Comparing `codedepot_ai_api-1.0.9/test/test_id_out.py` & `codedepot_ai_api-1.1.0/test/test_id_out.py`

 * *Files identical despite different names*

### Comparing `codedepot_ai_api-1.0.9/test/test_job_instance_in.py` & `codedepot_ai_api-1.1.0/test/test_job_instance_in.py`

 * *Files identical despite different names*

### Comparing `codedepot_ai_api-1.0.9/test/test_job_instance_out.py` & `codedepot_ai_api-1.1.0/test/test_job_instance_out.py`

 * *Files identical despite different names*

### Comparing `codedepot_ai_api-1.0.9/test/test_log_out.py` & `codedepot_ai_api-1.1.0/test/test_log_out.py`

 * *Files identical despite different names*

### Comparing `codedepot_ai_api-1.0.9/test/test_provider.py` & `codedepot_ai_api-1.1.0/test/test_provider.py`

 * *Files identical despite different names*

### Comparing `codedepot_ai_api-1.0.9/test/test_provider_out.py` & `codedepot_ai_api-1.1.0/test/test_provider_out.py`

 * *Files identical despite different names*

### Comparing `codedepot_ai_api-1.0.9/test/test_provider_type_out.py` & `codedepot_ai_api-1.1.0/test/test_provider_type_out.py`

 * *Files identical despite different names*

### Comparing `codedepot_ai_api-1.0.9/test/test_repository_in.py` & `codedepot_ai_api-1.1.0/test/test_repository_in.py`

 * *Files identical despite different names*

### Comparing `codedepot_ai_api-1.0.9/test/test_repository_out.py` & `codedepot_ai_api-1.1.0/test/test_repository_out.py`

 * *Files identical despite different names*

### Comparing `codedepot_ai_api-1.0.9/test/test_ssh_key_in.py` & `codedepot_ai_api-1.1.0/test/test_ssh_key_in.py`

 * *Files identical despite different names*

### Comparing `codedepot_ai_api-1.0.9/test/test_ssh_key_out.py` & `codedepot_ai_api-1.1.0/test/test_ssh_key_out.py`

 * *Files identical despite different names*

### Comparing `codedepot_ai_api-1.0.9/test/test_validation_error.py` & `codedepot_ai_api-1.1.0/test/test_validation_error.py`

 * *Files identical despite different names*

### Comparing `codedepot_ai_api-1.0.9/test/test_validation_error_loc_inner.py` & `codedepot_ai_api-1.1.0/test/test_validation_error_loc_inner.py`

 * *Files identical despite different names*

### Comparing `codedepot_ai_api-1.0.9/PKG-INFO` & `codedepot_ai_api-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codedepot-ai-api
-Version: 1.0.9
+Version: 1.1.0
 Summary: AI API
 Keywords: OpenAPI,OpenAPI-Generator,FastAPI
 Author-Email: OpenAPI Generator Community <team@openapitools.org>, CodeDepot <contact@codedepot.ai>
 License: NoLicense
 Project-URL: Repository, https://github.com/GIT_USER_ID/GIT_REPO_ID
 Project-URL: Homepage, https://codedepot.ai
 Requires-Python: <4.0,>=3.7
@@ -147,20 +147,19 @@
  - [ClientId](docs/ClientId.md)
  - [ClientSecret](docs/ClientSecret.md)
  - [ClusterIn](docs/ClusterIn.md)
  - [ClusterOut](docs/ClusterOut.md)
  - [FinishedAt](docs/FinishedAt.md)
  - [GrantType](docs/GrantType.md)
  - [HTTPValidationError](docs/HTTPValidationError.md)
- - [Id](docs/Id.md)
  - [IdOut](docs/IdOut.md)
  - [JobInstanceIn](docs/JobInstanceIn.md)
  - [JobInstanceOut](docs/JobInstanceOut.md)
  - [LogOut](docs/LogOut.md)
- - [Provider](docs/Provider.md)
+ - [ProviderIn](docs/ProviderIn.md)
  - [ProviderOut](docs/ProviderOut.md)
  - [ProviderTypeOut](docs/ProviderTypeOut.md)
  - [RepositoryIn](docs/RepositoryIn.md)
  - [RepositoryOut](docs/RepositoryOut.md)
  - [SshKeyIn](docs/SshKeyIn.md)
  - [SshKeyOut](docs/SshKeyOut.md)
  - [ValidationError](docs/ValidationError.md)
```

