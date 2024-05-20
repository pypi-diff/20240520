# Comparing `tmp/dbt_platform_helper-8.2.1.tar.gz` & `tmp/dbt_platform_helper-8.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_platform_helper-8.2.1.tar", max compression
+gzip compressed data, was "dbt_platform_helper-8.3.0.tar", max compression
```

## Comparing `dbt_platform_helper-8.2.1.tar` & `dbt_platform_helper-8.3.0.tar`

### file list

```diff
@@ -1,92 +1,92 @@
--rw-r--r--   0        0        0     1090 2024-05-07 16:06:28.912030 dbt_platform_helper-8.2.1/LICENSE
--rw-r--r--   0        0        0    17552 2024-05-07 16:06:28.912030 dbt_platform_helper-8.2.1/dbt_platform_helper/COMMANDS.md
--rw-r--r--   0        0        0     1762 2024-05-07 16:06:28.912030 dbt_platform_helper-8.2.1/dbt_platform_helper/README.md
--rw-r--r--   0        0        0        0 2024-05-07 16:06:28.912030 dbt_platform_helper-8.2.1/dbt_platform_helper/__init__.py
--rw-r--r--   0        0        0     4522 2024-05-07 16:06:28.912030 dbt_platform_helper-8.2.1/dbt_platform_helper/addon-plans.yml
--rw-r--r--   0        0        0     1315 2024-05-07 16:06:28.912030 dbt_platform_helper-8.2.1/dbt_platform_helper/addons-template-map.yml
--rw-r--r--   0        0        0        0 2024-05-07 16:06:28.912030 dbt_platform_helper-8.2.1/dbt_platform_helper/commands/__init__.py
--rw-r--r--   0        0        0     9957 2024-05-07 16:06:28.912030 dbt_platform_helper-8.2.1/dbt_platform_helper/commands/application.py
--rwxr-xr-x   0        0        0     3226 2024-05-07 16:06:28.912030 dbt_platform_helper-8.2.1/dbt_platform_helper/commands/check_cloudformation.py
--rw-r--r--   0        0        0    11192 2024-05-07 16:06:28.912030 dbt_platform_helper-8.2.1/dbt_platform_helper/commands/codebase.py
--rw-r--r--   0        0        0    14847 2024-05-07 16:06:28.912030 dbt_platform_helper-8.2.1/dbt_platform_helper/commands/conduit.py
--rw-r--r--   0        0        0     7953 2024-05-07 16:06:28.912030 dbt_platform_helper-8.2.1/dbt_platform_helper/commands/config.py
--rwxr-xr-x   0        0        0    15859 2024-05-07 16:06:28.912030 dbt_platform_helper-8.2.1/dbt_platform_helper/commands/copilot.py
--rwxr-xr-x   0        0        0    35037 2024-05-07 16:06:28.912030 dbt_platform_helper-8.2.1/dbt_platform_helper/commands/dns.py
--rw-r--r--   0        0        0    11417 2024-05-07 16:06:28.912030 dbt_platform_helper-8.2.1/dbt_platform_helper/commands/environment.py
--rw-r--r--   0        0        0      853 2024-05-07 16:06:28.912030 dbt_platform_helper-8.2.1/dbt_platform_helper/commands/generate.py
--rw-r--r--   0        0        0     6218 2024-05-07 16:06:28.912030 dbt_platform_helper-8.2.1/dbt_platform_helper/commands/pipeline.py
--rwxr-xr-x   0        0        0     3860 2024-05-07 16:06:28.912030 dbt_platform_helper-8.2.1/dbt_platform_helper/commands/secrets.py
--rw-r--r--   0        0        0        0 2024-05-07 16:06:28.912030 dbt_platform_helper-8.2.1/dbt_platform_helper/custom_resources/__init__.py
--rw-r--r--   0        0        0     2396 2024-05-07 16:06:28.912030 dbt_platform_helper-8.2.1/dbt_platform_helper/custom_resources/s3_object.py
--rw-r--r--   0        0        0      342 2024-05-07 16:06:28.912030 dbt_platform_helper-8.2.1/dbt_platform_helper/default-extensions.yml
--rw-r--r--   0        0        0      499 2024-05-07 16:06:28.912030 dbt_platform_helper-8.2.1/dbt_platform_helper/exceptions.py
--rw-r--r--   0        0        0      369 2024-05-07 16:06:28.912030 dbt_platform_helper-8.2.1/dbt_platform_helper/jinja2_tags.py
--rw-r--r--   0        0        0      158 2024-05-07 16:06:28.912030 dbt_platform_helper-8.2.1/dbt_platform_helper/templates/.copilot/config.yml
--rwxr-xr-x   0        0        0      164 2024-05-07 16:06:28.912030 dbt_platform_helper-8.2.1/dbt_platform_helper/templates/.copilot/image_build_run.sh
--rwxr-xr-x   0        0        0      121 2024-05-07 16:06:28.912030 dbt_platform_helper-8.2.1/dbt_platform_helper/templates/.copilot/phases/build.sh
--rwxr-xr-x   0        0        0      123 2024-05-07 16:06:28.912030 dbt_platform_helper-8.2.1/dbt_platform_helper/templates/.copilot/phases/install.sh
--rwxr-xr-x   0        0        0      126 2024-05-07 16:06:28.912030 dbt_platform_helper-8.2.1/dbt_platform_helper/templates/.copilot/phases/post_build.sh
--rwxr-xr-x   0        0        0      125 2024-05-07 16:06:28.912030 dbt_platform_helper-8.2.1/dbt_platform_helper/templates/.copilot/phases/pre_build.sh
--rw-r--r--   0        0        0     1081 2024-05-07 16:06:28.912030 dbt_platform_helper-8.2.1/dbt_platform_helper/templates/COMMANDS.md.jinja
--rw-r--r--   0        0        0      618 2024-05-07 16:06:28.912030 dbt_platform_helper-8.2.1/dbt_platform_helper/templates/addon-instructions.txt
--rw-r--r--   0        0        0      412 2024-05-07 16:06:28.912030 dbt_platform_helper-8.2.1/dbt_platform_helper/templates/addons/README.md
--rw-r--r--   0        0        0      734 2024-05-07 16:06:28.912030 dbt_platform_helper-8.2.1/dbt_platform_helper/templates/addons/env/addons.parameters.yml
--rw-r--r--   0        0        0    26381 2024-05-07 16:06:28.912030 dbt_platform_helper-8.2.1/dbt_platform_helper/templates/addons/env/aurora-postgres.yml
--rw-r--r--   0        0        0     6064 2024-05-07 16:06:28.912030 dbt_platform_helper-8.2.1/dbt_platform_helper/templates/addons/env/monitoring.yml
--rw-r--r--   0        0        0    10853 2024-05-07 16:06:28.912030 dbt_platform_helper-8.2.1/dbt_platform_helper/templates/addons/env/opensearch.yml
--rw-r--r--   0        0        0    25624 2024-05-07 16:06:28.912030 dbt_platform_helper-8.2.1/dbt_platform_helper/templates/addons/env/rds-postgres.yml
--rw-r--r--   0        0        0     7613 2024-05-07 16:06:28.912030 dbt_platform_helper-8.2.1/dbt_platform_helper/templates/addons/env/redis-cluster.yml
--rw-r--r--   0        0        0     7626 2024-05-07 16:06:28.912030 dbt_platform_helper-8.2.1/dbt_platform_helper/templates/addons/env/s3.yml
--rw-r--r--   0        0        0     3658 2024-05-07 16:06:28.912030 dbt_platform_helper-8.2.1/dbt_platform_helper/templates/addons/env/vpc.yml
--rw-r--r--   0        0        0      956 2024-05-07 16:06:28.912030 dbt_platform_helper-8.2.1/dbt_platform_helper/templates/addons/svc/appconfig-ipfilter.yml
--rw-r--r--   0        0        0     2403 2024-05-07 16:06:28.912030 dbt_platform_helper-8.2.1/dbt_platform_helper/templates/addons/svc/s3-policy.yml
--rw-r--r--   0        0        0      893 2024-05-07 16:06:28.912030 dbt_platform_helper-8.2.1/dbt_platform_helper/templates/addons/svc/subscription-filter.yml
--rw-r--r--   0        0        0     1836 2024-05-07 16:06:28.912030 dbt_platform_helper-8.2.1/dbt_platform_helper/templates/ci-codebuild-role-policy.json
--rw-r--r--   0        0        0      197 2024-05-07 16:06:28.912030 dbt_platform_helper-8.2.1/dbt_platform_helper/templates/create-codebuild-role.json
--rw-r--r--   0        0        0     1180 2024-05-07 16:06:28.912030 dbt_platform_helper-8.2.1/dbt_platform_helper/templates/custom-codebuild-role-policy.json
--rw-r--r--   0        0        0      781 2024-05-07 16:06:28.912030 dbt_platform_helper-8.2.1/dbt_platform_helper/templates/env/manifest.yml
--rw-r--r--   0        0        0      169 2024-05-07 16:06:28.912030 dbt_platform_helper-8.2.1/dbt_platform_helper/templates/env/overrides/.gitignore
--rw-r--r--   0        0        0      443 2024-05-07 16:06:28.912030 dbt_platform_helper-8.2.1/dbt_platform_helper/templates/env/overrides/README.md
--rw-r--r--   0        0        0      284 2024-05-07 16:06:28.912030 dbt_platform_helper-8.2.1/dbt_platform_helper/templates/env/overrides/bin/override.ts
--rw-r--r--   0        0        0      339 2024-05-07 16:06:28.912030 dbt_platform_helper-8.2.1/dbt_platform_helper/templates/env/overrides/cdk.json
--rw-r--r--   0        0        0     1760 2024-05-07 16:06:28.912030 dbt_platform_helper-8.2.1/dbt_platform_helper/templates/env/overrides/log_resource_policy.json
--rw-r--r--   0        0        0   155387 2024-05-07 16:06:28.912030 dbt_platform_helper-8.2.1/dbt_platform_helper/templates/env/overrides/package-lock.json
--rw-r--r--   0        0        0      536 2024-05-07 16:06:28.912030 dbt_platform_helper-8.2.1/dbt_platform_helper/templates/env/overrides/package.json
--rw-r--r--   0        0        0     1910 2024-05-07 16:06:28.912030 dbt_platform_helper-8.2.1/dbt_platform_helper/templates/env/overrides/stack.ts
--rw-r--r--   0        0        0      710 2024-05-07 16:06:28.912030 dbt_platform_helper-8.2.1/dbt_platform_helper/templates/env/overrides/tsconfig.json
--rw-r--r--   0        0        0      208 2024-05-07 16:06:28.912030 dbt_platform_helper-8.2.1/dbt_platform_helper/templates/env/terraform-overrides/cfn.patches.yml
--rw-r--r--   0        0        0     1959 2024-05-07 16:06:28.922030 dbt_platform_helper-8.2.1/dbt_platform_helper/templates/pipelines/codebase/manifest.yml
--rw-r--r--   0        0        0      169 2024-05-07 16:06:28.922030 dbt_platform_helper-8.2.1/dbt_platform_helper/templates/pipelines/codebase/overrides/.gitignore
--rw-r--r--   0        0        0      227 2024-05-07 16:06:28.922030 dbt_platform_helper-8.2.1/dbt_platform_helper/templates/pipelines/codebase/overrides/bin/override.ts
--rw-r--r--   0        0        0      287 2024-05-07 16:06:28.922030 dbt_platform_helper-8.2.1/dbt_platform_helper/templates/pipelines/codebase/overrides/buildspec.deploy.yml
--rw-r--r--   0        0        0      781 2024-05-07 16:06:28.922030 dbt_platform_helper-8.2.1/dbt_platform_helper/templates/pipelines/codebase/overrides/buildspec.image.yml
--rw-r--r--   0        0        0      339 2024-05-07 16:06:28.922030 dbt_platform_helper-8.2.1/dbt_platform_helper/templates/pipelines/codebase/overrides/cdk.json
--rw-r--r--   0        0        0   152518 2024-05-07 16:06:28.922030 dbt_platform_helper-8.2.1/dbt_platform_helper/templates/pipelines/codebase/overrides/package-lock.json
--rw-r--r--   0        0        0      536 2024-05-07 16:06:28.922030 dbt_platform_helper-8.2.1/dbt_platform_helper/templates/pipelines/codebase/overrides/package.json
--rw-r--r--   0        0        0    20142 2024-05-07 16:06:28.922030 dbt_platform_helper-8.2.1/dbt_platform_helper/templates/pipelines/codebase/overrides/stack.ts
--rw-r--r--   0        0        0      651 2024-05-07 16:06:28.922030 dbt_platform_helper-8.2.1/dbt_platform_helper/templates/pipelines/codebase/overrides/tsconfig.json
--rw-r--r--   0        0        0     1205 2024-05-07 16:06:28.922030 dbt_platform_helper-8.2.1/dbt_platform_helper/templates/pipelines/codebase/overrides/types.ts
--rw-r--r--   0        0        0     3178 2024-05-07 16:06:28.922030 dbt_platform_helper-8.2.1/dbt_platform_helper/templates/pipelines/environments/buildspec.yml
--rw-r--r--   0        0        0     1778 2024-05-07 16:06:28.922030 dbt_platform_helper-8.2.1/dbt_platform_helper/templates/pipelines/environments/manifest.yml
--rw-r--r--   0        0        0      617 2024-05-07 16:06:28.922030 dbt_platform_helper-8.2.1/dbt_platform_helper/templates/pipelines/environments/overrides/cfn.patches.yml
--rw-r--r--   0        0        0      741 2024-05-07 16:06:28.922030 dbt_platform_helper-8.2.1/dbt_platform_helper/templates/svc/maintenance_pages/default.html
--rw-r--r--   0        0        0      783 2024-05-07 16:06:28.922030 dbt_platform_helper-8.2.1/dbt_platform_helper/templates/svc/maintenance_pages/migration.html
--rw-r--r--   0        0        0     2881 2024-05-07 16:06:28.922030 dbt_platform_helper-8.2.1/dbt_platform_helper/templates/svc/manifest-backend.yml
--rw-r--r--   0        0        0     3921 2024-05-07 16:06:28.922030 dbt_platform_helper-8.2.1/dbt_platform_helper/templates/svc/manifest-public.yml
--rw-r--r--   0        0        0      386 2024-05-07 16:06:28.922030 dbt_platform_helper-8.2.1/dbt_platform_helper/templates/svc/overrides/cfn.patches.yml
--rw-r--r--   0        0        0        0 2024-05-07 16:06:28.922030 dbt_platform_helper-8.2.1/dbt_platform_helper/utils/__init__.py
--rw-r--r--   0        0        0     3555 2024-05-07 16:06:28.922030 dbt_platform_helper-8.2.1/dbt_platform_helper/utils/application.py
--rw-r--r--   0        0        0    10297 2024-05-07 16:06:28.922030 dbt_platform_helper-8.2.1/dbt_platform_helper/utils/aws.py
--rw-r--r--   0        0        0     2943 2024-05-07 16:06:28.922030 dbt_platform_helper-8.2.1/dbt_platform_helper/utils/click.py
--rw-r--r--   0        0        0     1053 2024-05-07 16:06:28.922030 dbt_platform_helper-8.2.1/dbt_platform_helper/utils/cloudformation.py
--rw-r--r--   0        0        0      484 2024-05-07 16:06:28.922030 dbt_platform_helper-8.2.1/dbt_platform_helper/utils/cloudfoundry.py
--rw-r--r--   0        0        0     1720 2024-05-07 16:06:28.922030 dbt_platform_helper-8.2.1/dbt_platform_helper/utils/files.py
--rw-r--r--   0        0        0      304 2024-05-07 16:06:28.922030 dbt_platform_helper-8.2.1/dbt_platform_helper/utils/git.py
--rw-r--r--   0        0        0      507 2024-05-07 16:06:28.922030 dbt_platform_helper-8.2.1/dbt_platform_helper/utils/manifests.py
--rw-r--r--   0        0        0      115 2024-05-07 16:06:28.922030 dbt_platform_helper-8.2.1/dbt_platform_helper/utils/messages.py
--rw-r--r--   0        0        0      469 2024-05-07 16:06:28.922030 dbt_platform_helper-8.2.1/dbt_platform_helper/utils/template.py
--rw-r--r--   0        0        0    17799 2024-05-07 16:06:28.922030 dbt_platform_helper-8.2.1/dbt_platform_helper/utils/validation.py
--rw-r--r--   0        0        0     6695 2024-05-07 16:06:28.922030 dbt_platform_helper-8.2.1/dbt_platform_helper/utils/versioning.py
--rwxr-xr-x   0        0        0     1930 2024-05-07 16:06:28.922030 dbt_platform_helper-8.2.1/platform_helper.py
--rw-r--r--   0        0        0     1392 2024-05-07 16:06:28.922030 dbt_platform_helper-8.2.1/pyproject.toml
--rw-r--r--   0        0        0     3315 1970-01-01 00:00:00.000000 dbt_platform_helper-8.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1090 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/LICENSE
+-rw-r--r--   0        0        0    17907 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/COMMANDS.md
+-rw-r--r--   0        0        0     1762 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/README.md
+-rw-r--r--   0        0        0        0 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/__init__.py
+-rw-r--r--   0        0        0     4522 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/addon-plans.yml
+-rw-r--r--   0        0        0     1315 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/addons-template-map.yml
+-rw-r--r--   0        0        0        0 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/commands/__init__.py
+-rw-r--r--   0        0        0     9957 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/commands/application.py
+-rwxr-xr-x   0        0        0     3226 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/commands/check_cloudformation.py
+-rw-r--r--   0        0        0    11192 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/commands/codebase.py
+-rw-r--r--   0        0        0    14847 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/commands/conduit.py
+-rw-r--r--   0        0        0    11480 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/commands/config.py
+-rwxr-xr-x   0        0        0    16114 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/commands/copilot.py
+-rwxr-xr-x   0        0        0    35037 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/commands/dns.py
+-rw-r--r--   0        0        0    11417 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/commands/environment.py
+-rw-r--r--   0        0        0      853 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/commands/generate.py
+-rw-r--r--   0        0        0     6198 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/commands/pipeline.py
+-rwxr-xr-x   0        0        0     3860 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/commands/secrets.py
+-rw-r--r--   0        0        0        0 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/custom_resources/__init__.py
+-rw-r--r--   0        0        0     2396 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/custom_resources/s3_object.py
+-rw-r--r--   0        0        0      342 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/default-extensions.yml
+-rw-r--r--   0        0        0      499 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/exceptions.py
+-rw-r--r--   0        0        0      369 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/jinja2_tags.py
+-rw-r--r--   0        0        0      158 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/.copilot/config.yml
+-rwxr-xr-x   0        0        0      164 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/.copilot/image_build_run.sh
+-rwxr-xr-x   0        0        0      121 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/.copilot/phases/build.sh
+-rwxr-xr-x   0        0        0      123 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/.copilot/phases/install.sh
+-rwxr-xr-x   0        0        0      126 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/.copilot/phases/post_build.sh
+-rwxr-xr-x   0        0        0      125 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/.copilot/phases/pre_build.sh
+-rw-r--r--   0        0        0     1081 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/COMMANDS.md.jinja
+-rw-r--r--   0        0        0      618 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/addon-instructions.txt
+-rw-r--r--   0        0        0      412 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/addons/README.md
+-rw-r--r--   0        0        0      734 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/addons/env/addons.parameters.yml
+-rw-r--r--   0        0        0    26381 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/addons/env/aurora-postgres.yml
+-rw-r--r--   0        0        0     6064 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/addons/env/monitoring.yml
+-rw-r--r--   0        0        0    10853 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/addons/env/opensearch.yml
+-rw-r--r--   0        0        0    25624 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/addons/env/rds-postgres.yml
+-rw-r--r--   0        0        0     7613 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/addons/env/redis-cluster.yml
+-rw-r--r--   0        0        0     7626 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/addons/env/s3.yml
+-rw-r--r--   0        0        0     3658 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/addons/env/vpc.yml
+-rw-r--r--   0        0        0      956 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/addons/svc/appconfig-ipfilter.yml
+-rw-r--r--   0        0        0     2403 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/addons/svc/s3-policy.yml
+-rw-r--r--   0        0        0      893 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/addons/svc/subscription-filter.yml
+-rw-r--r--   0        0        0     1836 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/ci-codebuild-role-policy.json
+-rw-r--r--   0        0        0      197 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/create-codebuild-role.json
+-rw-r--r--   0        0        0     1180 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/custom-codebuild-role-policy.json
+-rw-r--r--   0        0        0      781 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/env/manifest.yml
+-rw-r--r--   0        0        0      169 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/env/overrides/.gitignore
+-rw-r--r--   0        0        0      443 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/env/overrides/README.md
+-rw-r--r--   0        0        0      284 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/env/overrides/bin/override.ts
+-rw-r--r--   0        0        0      339 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/env/overrides/cdk.json
+-rw-r--r--   0        0        0     1760 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/env/overrides/log_resource_policy.json
+-rw-r--r--   0        0        0   155387 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/env/overrides/package-lock.json
+-rw-r--r--   0        0        0      536 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/env/overrides/package.json
+-rw-r--r--   0        0        0     1910 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/env/overrides/stack.ts
+-rw-r--r--   0        0        0      710 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/env/overrides/tsconfig.json
+-rw-r--r--   0        0        0      208 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/env/terraform-overrides/cfn.patches.yml
+-rw-r--r--   0        0        0     1959 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/pipelines/codebase/manifest.yml
+-rw-r--r--   0        0        0      169 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/pipelines/codebase/overrides/.gitignore
+-rw-r--r--   0        0        0      227 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/pipelines/codebase/overrides/bin/override.ts
+-rw-r--r--   0        0        0      287 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/pipelines/codebase/overrides/buildspec.deploy.yml
+-rw-r--r--   0        0        0      781 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/pipelines/codebase/overrides/buildspec.image.yml
+-rw-r--r--   0        0        0      339 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/pipelines/codebase/overrides/cdk.json
+-rw-r--r--   0        0        0   152518 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/pipelines/codebase/overrides/package-lock.json
+-rw-r--r--   0        0        0      536 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/pipelines/codebase/overrides/package.json
+-rw-r--r--   0        0        0    20142 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/pipelines/codebase/overrides/stack.ts
+-rw-r--r--   0        0        0      651 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/pipelines/codebase/overrides/tsconfig.json
+-rw-r--r--   0        0        0     1205 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/pipelines/codebase/overrides/types.ts
+-rw-r--r--   0        0        0     3178 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/pipelines/environments/buildspec.yml
+-rw-r--r--   0        0        0     1778 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/pipelines/environments/manifest.yml
+-rw-r--r--   0        0        0      617 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/pipelines/environments/overrides/cfn.patches.yml
+-rw-r--r--   0        0        0      741 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/svc/maintenance_pages/default.html
+-rw-r--r--   0        0        0      783 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/svc/maintenance_pages/migration.html
+-rw-r--r--   0        0        0     2881 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/svc/manifest-backend.yml
+-rw-r--r--   0        0        0     3921 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/svc/manifest-public.yml
+-rw-r--r--   0        0        0      386 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/templates/svc/overrides/cfn.patches.yml
+-rw-r--r--   0        0        0        0 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/utils/__init__.py
+-rw-r--r--   0        0        0     3555 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/utils/application.py
+-rw-r--r--   0        0        0    10297 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/utils/aws.py
+-rw-r--r--   0        0        0     2943 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/utils/click.py
+-rw-r--r--   0        0        0     1053 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/utils/cloudformation.py
+-rw-r--r--   0        0        0      484 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/utils/cloudfoundry.py
+-rw-r--r--   0        0        0     1720 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/utils/files.py
+-rw-r--r--   0        0        0      384 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/utils/git.py
+-rw-r--r--   0        0        0      507 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/utils/manifests.py
+-rw-r--r--   0        0        0      115 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/utils/messages.py
+-rw-r--r--   0        0        0      469 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/utils/template.py
+-rw-r--r--   0        0        0    14979 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/utils/validation.py
+-rw-r--r--   0        0        0     6695 2024-05-20 14:11:39.484018 dbt_platform_helper-8.3.0/dbt_platform_helper/utils/versioning.py
+-rwxr-xr-x   0        0        0     1930 2024-05-20 14:11:39.494018 dbt_platform_helper-8.3.0/platform_helper.py
+-rw-r--r--   0        0        0     1392 2024-05-20 14:11:39.494018 dbt_platform_helper-8.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3315 1970-01-01 00:00:00.000000 dbt_platform_helper-8.3.0/PKG-INFO
```

### Comparing `dbt_platform_helper-8.2.1/LICENSE` & `dbt_platform_helper-8.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/COMMANDS.md` & `dbt_platform_helper-8.3.0/dbt_platform_helper/COMMANDS.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 - [platform-helper codebase prepare](#platform-helper-codebase-prepare)
 - [platform-helper codebase list](#platform-helper-codebase-list)
 - [platform-helper codebase build](#platform-helper-codebase-build)
 - [platform-helper codebase deploy](#platform-helper-codebase-deploy)
 - [platform-helper conduit](#platform-helper-conduit)
 - [platform-helper config](#platform-helper-config)
 - [platform-helper config validate](#platform-helper-config-validate)
+- [platform-helper config aws](#platform-helper-config-aws)
 - [platform-helper copilot](#platform-helper-copilot)
 - [platform-helper copilot make-addons](#platform-helper-copilot-make-addons)
 - [platform-helper domain](#platform-helper-domain)
 - [platform-helper domain configure](#platform-helper-domain-configure)
 - [platform-helper domain assign](#platform-helper-domain-assign)
 - [platform-helper environment](#platform-helper-environment)
 - [platform-helper environment offline](#platform-helper-environment-offline)
@@ -451,24 +452,25 @@
 [↩ Parent](#platform-helper)
 
     Perform actions on configuration files.
 
 ## Usage
 
 ```
-platform-helper config validate 
+platform-helper config (validate|aws) 
 ```
 
 ## Options
 
 - `--help <boolean>` _Defaults to False._
   - Show this message and exit.
 
 ## Commands
 
+- [`aws` ↪](#platform-helper-config-aws)
 - [`validate` ↪](#platform-helper-config-validate)
 
 # platform-helper config validate
 
 [↩ Parent](#platform-helper-config)
 
     Validate deployment or application configuration.
@@ -480,14 +482,37 @@
 ```
 
 ## Options
 
 - `--help <boolean>` _Defaults to False._
   - Show this message and exit.
 
+# platform-helper config aws
+
+[↩ Parent](#platform-helper-config)
+
+    Writes a local config file containing all the AWS profiles to which the
+    logged in user has access.
+
+    If no `--file-path` is specified, defaults to `~/.aws/config`.
+
+## Usage
+
+```
+platform-helper config aws [--file-path <file_path>] 
+```
+
+## Options
+
+- `--file-path
+-fp <text>` _Defaults to ~/.aws/config._
+
+- `--help <boolean>` _Defaults to False._
+  - Show this message and exit.
+
 # platform-helper copilot
 
 [↩ Parent](#platform-helper)
 
 ## Usage
 
 ```
@@ -503,17 +528,14 @@
 
 - [`make-addons` ↪](#platform-helper-copilot-make-addons)
 
 # platform-helper copilot make-addons
 
 [↩ Parent](#platform-helper-copilot)
 
-    WARNING: this command should not be used as a stand-alone.
-    Use `platform-helper generate` instead.
-
     Generate addons CloudFormation for each environment.
 
 ## Usage
 
 ```
 platform-helper copilot make-addons 
 ```
@@ -722,17 +744,14 @@
 
 - [`generate` ↪](#platform-helper-pipeline-generate)
 
 # platform-helper pipeline generate
 
 [↩ Parent](#platform-helper-pipeline)
 
-    WARNING: this command should not be used as a stand-alone.
-    Use `platform-helper generate` instead.
-
     Given a pipelines.yml file, generate environment and service deployment
     pipelines.
 
 ## Usage
 
 ```
 platform-helper pipeline generate
```

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/README.md` & `dbt_platform_helper-8.3.0/dbt_platform_helper/README.md`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/addon-plans.yml` & `dbt_platform_helper-8.3.0/dbt_platform_helper/addon-plans.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/addons-template-map.yml` & `dbt_platform_helper-8.3.0/dbt_platform_helper/addons-template-map.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/commands/application.py` & `dbt_platform_helper-8.3.0/dbt_platform_helper/commands/application.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/commands/check_cloudformation.py` & `dbt_platform_helper-8.3.0/dbt_platform_helper/commands/check_cloudformation.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/commands/codebase.py` & `dbt_platform_helper-8.3.0/dbt_platform_helper/commands/codebase.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/commands/conduit.py` & `dbt_platform_helper-8.3.0/dbt_platform_helper/commands/conduit.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/commands/config.py` & `dbt_platform_helper-8.3.0/dbt_platform_helper/commands/config.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,14 @@
+import os
+import webbrowser
 from pathlib import Path
 from typing import Dict
 
+import boto3
+import botocore
 import click
 from prettytable import PrettyTable
 
 from dbt_platform_helper.exceptions import IncompatibleMajorVersion
 from dbt_platform_helper.exceptions import ValidationException
 from dbt_platform_helper.utils import versioning
 from dbt_platform_helper.utils.click import ClickDocOptGroup
@@ -20,14 +24,27 @@
     ),
     "dbt-platform-helper-upgrade-note": (
         "Post upgrade, run `platform-helper copilot make-addons` to " "update your addon templates."
     ),
     "generic-tool-upgrade": "Upgrade {tool} to version {version}.",
 }
 
+SSO_START_URL = "https://uktrade.awsapps.com/start"
+
+AWS_CONFIG = """
+#
+# uktrade
+#
+
+[sso-session uktrade]
+sso_start_url = https://uktrade.awsapps.com/start#/
+sso_region = eu-west-2
+sso_registration_scopes = sso:account:access
+"""
+
 
 @click.group(cls=ClickDocOptGroup)
 def config():
     """Perform actions on configuration files."""
 
 
 @config.command()
@@ -221,7 +238,97 @@
             if name.endswith("-note"):
                 continue
             click.secho(f"  - {recommendation}")
             if recommendations.get(f"{name}-note", False):
                 click.secho(f"    {recommendations.get(f'{name}-note')}")
 
         click.secho()
+
+
+@config.command()
+@click.option("--file-path", "-fp", default="~/.aws/config")
+def aws(file_path):
+    """
+    Writes a local config file containing all the AWS profiles to which the
+    logged in user has access.
+
+    If no `--file-path` is specified, defaults to `~/.aws/config`.
+    """
+    sso_oidc_client = boto3.client("sso-oidc", region_name="eu-west-2")
+    sso_client = boto3.client("sso", region_name="eu-west-2")
+    oidc_app = create_oidc_application(sso_oidc_client)
+    verification_url, device_code = get_device_code(sso_oidc_client, oidc_app, SSO_START_URL)
+
+    if click.confirm(
+        "You are about to be redirected to a verification page. You will need to complete sign-in before returning to the command line. Do you want to continue?",
+        abort=True,
+    ):
+        webbrowser.open(verification_url)
+
+    if click.confirm("Have you completed the sign-in process in your browser?", abort=True):
+        access_token = get_access_token(device_code, sso_oidc_client, oidc_app)
+
+    aws_config_path = os.path.expanduser(file_path)
+
+    with open(aws_config_path, "w") as config_file:
+        config_file.write(AWS_CONFIG)
+
+        for account in retrieve_aws_accounts(sso_client, access_token):
+            config_file.write(f"[profile {account['accountName']}]\n")
+            config_file.write("sso_session = uktrade\n")
+            config_file.write(f"sso_account_id = {account['accountId']}\n")
+            config_file.write("sso_role_name = AdministratorAccess\n")
+            config_file.write("region = eu-west-2\n")
+            config_file.write("output = json\n")
+
+
+def create_oidc_application(sso_oidc_client):
+    print("Creating temporary AWS SSO OIDC application")
+    client = sso_oidc_client.register_client(
+        clientName="platform-helper",
+        clientType="public",
+    )
+    client_id = client.get("clientId")
+    client_secret = client.get("clientSecret")
+
+    return client_id, client_secret
+
+
+def get_device_code(sso_oidc_client, oidc_application, start_url):
+    print("Initiating device code flow")
+    authz = sso_oidc_client.start_device_authorization(
+        clientId=oidc_application[0],
+        clientSecret=oidc_application[1],
+        startUrl=start_url,
+    )
+    url = authz.get("verificationUriComplete")
+    deviceCode = authz.get("deviceCode")
+
+    return url, deviceCode
+
+
+def retrieve_aws_accounts(sso_client, aws_sso_token):
+    aws_accounts_response = sso_client.list_accounts(
+        accessToken=aws_sso_token,
+        maxResults=100,
+    )
+    if len(aws_accounts_response.get("accountList", [])) == 0:
+        raise RuntimeError("Unable to retrieve AWS SSO account list\n")
+    return aws_accounts_response.get("accountList")
+
+
+def get_access_token(device_code, sso_oidc_client, oidc_app):
+
+    try:
+        token_response = sso_oidc_client.create_token(
+            clientId=oidc_app[0],
+            clientSecret=oidc_app[1],
+            grantType="urn:ietf:params:oauth:grant-type:device_code",
+            deviceCode=device_code,
+        )
+
+        return token_response.get("accessToken")
+
+    except botocore.exceptions.ClientError as e:
+        breakpoint()
+        if e.response["Error"]["Code"] != "AuthorizationPendingException":
+            raise e
```

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/commands/copilot.py` & `dbt_platform_helper-8.3.0/dbt_platform_helper/commands/copilot.py`

 * *Files 3% similar despite different names*

```diff
@@ -116,14 +116,15 @@
         exit(1)
 
     if not svc_names:
         click.echo(click.style(f"No services found in ./copilot/; exiting", fg="red"))
         exit(1)
 
     normalised_config = {}
+    config_has_errors = False
     for addon_name, addon_config in config.items():
         addon_type = addon_config["type"]
         normalised_config[addon_name] = copy.deepcopy(addon_config)
 
         if "services" in normalised_config[addon_name]:
             if normalised_config[addon_name]["services"] == "__all__":
                 normalised_config[addon_name]["services"] = svc_names
@@ -131,42 +132,55 @@
             if not set(normalised_config[addon_name]["services"]).issubset(set(svc_names)):
                 click.echo(
                     click.style(
                         f"Services listed in {addon_name}.services do not exist in ./copilot/",
                         fg="red",
                     ),
                 )
-                exit(1)
+                config_has_errors = True
 
         environments = normalised_config[addon_name].pop("environments", {})
         default = environments.pop("*", environments.pop("default", {}))
 
         initial = _lookup_plan(addon_type, default)
 
-        if not set(environments.keys()).issubset(set(env_names)):
+        missing_envs = set(environments.keys()) - set(env_names)
+        if missing_envs:
             click.echo(
                 click.style(
-                    f"Environment keys listed in {addon_name} do not match ./copilot/environments",
+                    f"Environment keys listed in {addon_name} do not match those defined in ./copilot/environments.",
                     fg="red",
+                )
+            ),
+            click.echo(
+                click.style(
+                    f"  Missing environments: {', '.join(sorted(missing_envs))}",
+                    fg="white",
                 ),
             )
-            exit(1)
+            config_has_errors = True
+
+        if config_has_errors:
+            continue
 
         normalised_environments = {}
 
         for env in env_names:
             normalised_environments[env] = _normalise_keys(initial)
 
         for env_name, env_config in environments.items():
             normalised_environments[env_name].update(
                 _lookup_plan(addon_type, _normalise_keys(env_config))
             )
 
         normalised_config[addon_name]["environments"] = normalised_environments
 
+    if config_has_errors:
+        exit(1)
+
     return normalised_config
 
 
 def get_log_destination_arn():
     """Get destination arns stored in param store in projects aws account."""
     session = get_aws_session_or_abort()
     client = session.client("ssm", region_name="eu-west-2")
@@ -212,22 +226,17 @@
             pass
         else:
             arns[environment_name] = response["KeyMetadata"]["Arn"]
 
     return arns
 
 
-@copilot.command(deprecated=True, hidden=True)
+@copilot.command()
 def make_addons():
-    """
-    WARNING: this command should not be used as a stand-alone.
-    Use `platform-helper generate` instead.
-
-    Generate addons CloudFormation for each environment.
-    """
+    """Generate addons CloudFormation for each environment."""
     output_dir = Path(".").absolute()
     ensure_cwd_is_repo_root()
     is_terraform = is_terraform_project()
 
     templates = setup_templates()
     config = _get_config()
     session = get_aws_session_or_abort()
```

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/commands/dns.py` & `dbt_platform_helper-8.3.0/dbt_platform_helper/commands/dns.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/commands/environment.py` & `dbt_platform_helper-8.3.0/dbt_platform_helper/commands/environment.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/commands/generate.py` & `dbt_platform_helper-8.3.0/dbt_platform_helper/commands/generate.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/commands/pipeline.py` & `dbt_platform_helper-8.3.0/dbt_platform_helper/commands/pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python
 from os import makedirs
 from pathlib import Path
 
 import click
 from yaml.parser import ParserError
 
+from dbt_platform_helper.commands.copilot import is_terraform_project
 from dbt_platform_helper.utils.application import get_application_name
 from dbt_platform_helper.utils.aws import get_account_details
 from dbt_platform_helper.utils.aws import get_codestar_connection_arn
 from dbt_platform_helper.utils.aws import get_public_repository_arn
 from dbt_platform_helper.utils.click import ClickDocOptGroup
 from dbt_platform_helper.utils.files import generate_override_files
 from dbt_platform_helper.utils.files import load_and_validate_config
@@ -24,21 +25,17 @@
 
 @click.group(chain=True, cls=ClickDocOptGroup)
 def pipeline():
     """Pipeline commands."""
     check_platform_helper_version_needs_update()
 
 
-@pipeline.command(deprecated=True, hidden=True)
+@pipeline.command()
 def generate():
-    """
-    WARNING: this command should not be used as a stand-alone.
-    Use `platform-helper generate` instead.
-
-    Given a pipelines.yml file, generate environment and service deployment
+    """Given a pipelines.yml file, generate environment and service deployment
     pipelines."""
     templates = setup_templates()
 
     app_name = get_application_name()
 
     pipeline_config = _safe_load_config("pipelines.yml", PIPELINES_SCHEMA)
 
@@ -46,17 +43,17 @@
 
     git_repo = git_remote()
     if not git_repo:
         abort_with_error("The current directory is not a git repository")
 
     codestar_connection_arn = get_codestar_connection_arn(app_name)
     if codestar_connection_arn is None:
-        abort_with_error("There is no CodeStar Connection to use")
+        abort_with_error(f'There is no CodeStar Connection named "{app_name}" to use')
 
-    if "environments" in pipeline_config:
+    if not is_terraform_project() and "environments" in pipeline_config:
         _generate_environments_pipeline(
             app_name, codestar_connection_arn, git_repo, pipeline_config["environments"], templates
         )
 
     if "codebases" in pipeline_config:
         account_id, _ = get_account_details()
```

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/commands/secrets.py` & `dbt_platform_helper-8.3.0/dbt_platform_helper/commands/secrets.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/custom_resources/s3_object.py` & `dbt_platform_helper-8.3.0/dbt_platform_helper/custom_resources/s3_object.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/templates/COMMANDS.md.jinja` & `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/COMMANDS.md.jinja`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/templates/addon-instructions.txt` & `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/addon-instructions.txt`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/templates/addons/env/addons.parameters.yml` & `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/addons/env/addons.parameters.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/templates/addons/env/aurora-postgres.yml` & `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/addons/env/aurora-postgres.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/templates/addons/env/monitoring.yml` & `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/addons/env/monitoring.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/templates/addons/env/opensearch.yml` & `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/addons/env/opensearch.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/templates/addons/env/rds-postgres.yml` & `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/addons/env/rds-postgres.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/templates/addons/env/redis-cluster.yml` & `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/addons/env/redis-cluster.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/templates/addons/env/s3.yml` & `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/addons/env/s3.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/templates/addons/env/vpc.yml` & `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/addons/env/vpc.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/templates/addons/svc/appconfig-ipfilter.yml` & `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/addons/svc/appconfig-ipfilter.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/templates/addons/svc/s3-policy.yml` & `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/addons/svc/s3-policy.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/templates/addons/svc/subscription-filter.yml` & `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/addons/svc/subscription-filter.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/templates/ci-codebuild-role-policy.json` & `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/ci-codebuild-role-policy.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/templates/custom-codebuild-role-policy.json` & `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/custom-codebuild-role-policy.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/templates/env/manifest.yml` & `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/env/manifest.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/templates/env/overrides/log_resource_policy.json` & `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/env/overrides/log_resource_policy.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/templates/env/overrides/package-lock.json` & `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/env/overrides/package-lock.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/templates/env/overrides/package.json` & `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/env/overrides/package.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/templates/env/overrides/stack.ts` & `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/env/overrides/stack.ts`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/templates/env/overrides/tsconfig.json` & `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/env/overrides/tsconfig.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/templates/pipelines/codebase/manifest.yml` & `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/pipelines/codebase/manifest.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/templates/pipelines/codebase/overrides/buildspec.image.yml` & `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/pipelines/codebase/overrides/buildspec.image.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/templates/pipelines/codebase/overrides/package-lock.json` & `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/pipelines/codebase/overrides/package-lock.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/templates/pipelines/codebase/overrides/package.json` & `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/pipelines/codebase/overrides/package.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/templates/pipelines/codebase/overrides/stack.ts` & `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/pipelines/codebase/overrides/stack.ts`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/templates/pipelines/codebase/overrides/tsconfig.json` & `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/pipelines/codebase/overrides/tsconfig.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/templates/pipelines/codebase/overrides/types.ts` & `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/pipelines/codebase/overrides/types.ts`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/templates/pipelines/environments/buildspec.yml` & `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/pipelines/environments/buildspec.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/templates/pipelines/environments/manifest.yml` & `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/pipelines/environments/manifest.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/templates/pipelines/environments/overrides/cfn.patches.yml` & `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/pipelines/environments/overrides/cfn.patches.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/templates/svc/maintenance_pages/default.html` & `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/svc/maintenance_pages/default.html`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/templates/svc/maintenance_pages/migration.html` & `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/svc/maintenance_pages/migration.html`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/templates/svc/manifest-backend.yml` & `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/svc/manifest-backend.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/templates/svc/manifest-public.yml` & `dbt_platform_helper-8.3.0/dbt_platform_helper/templates/svc/manifest-public.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/utils/application.py` & `dbt_platform_helper-8.3.0/dbt_platform_helper/utils/application.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/utils/aws.py` & `dbt_platform_helper-8.3.0/dbt_platform_helper/utils/aws.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/utils/click.py` & `dbt_platform_helper-8.3.0/dbt_platform_helper/utils/click.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/utils/cloudformation.py` & `dbt_platform_helper-8.3.0/dbt_platform_helper/utils/cloudformation.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/utils/files.py` & `dbt_platform_helper-8.3.0/dbt_platform_helper/utils/files.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/utils/validation.py` & `dbt_platform_helper-8.3.0/dbt_platform_helper/utils/validation.py`

 * *Files 16% similar despite different names*

```diff
@@ -148,100 +148,31 @@
     error="Environment name {} is invalid: names must only contain lowercase alphanumeric characters, or be the '*' default environment",
     # For values the "error" parameter works and outputs the custom text. For keys the custom text doesn't get reported in the exception for some reason.
 )
 
 range_validator = validate_string(r"^\d+-\d+$")
 seconds_validator = validate_string(r"^\d+s$")
 
-BOOTSTRAP_SCHEMA = Schema(
+PIPELINES_SCHEMA = Schema(
     {
-        "app": str,
-        "environments": {str: {Optional("certificate_arns"): [str]}},
-        "services": [
+        # The following line is for the AWS Copilot version, will be removed under DBTP-1002
+        Optional("accounts"): list[str],
+        Optional("environments"): [
             {
                 "name": str,
-                "type": lambda s: s
-                in (
-                    "public",
-                    "backend",
-                ),
-                "repo": str,
-                "image_location": str,
-                Optional("notes"): str,
-                Optional("secrets_from"): str,
-                "environments": {
-                    str: {
-                        "paas": str,
-                        Optional("url"): str,
-                        Optional("ipfilter"): bool,
-                        Optional("memory"): int,
-                        Optional("count"): Or(
-                            int,
-                            {
-                                # https://aws.github.io/copilot-cli/docs/manifest/lb-web-service/#count
-                                "range": range_validator,  # e.g. 1-10
-                                Optional("cooldown"): {
-                                    "in": seconds_validator,  # e.g 30s
-                                    "out": seconds_validator,  # e.g 30s
-                                },
-                                Optional("cpu_percentage"): int,
-                                Optional("memory_percentage"): Or(
-                                    int,
-                                    {
-                                        "value": int,
-                                        "cooldown": {
-                                            "in": seconds_validator,  # e.g. 80s
-                                            "out": seconds_validator,  # e.g 160s
-                                        },
-                                    },
-                                ),
-                                Optional("requests"): int,
-                                Optional("response_time"): seconds_validator,  # e.g. 2s
-                            },
-                        ),
+                Optional("accounts"): {
+                    "deploy": {
+                        "name": str,
+                        "id": str,
                     },
-                },
-                Optional("backing_services"): [
-                    {
+                    "dns": {
                         "name": str,
-                        "type": lambda s: s
-                        in (
-                            "s3",
-                            "s3-policy",
-                            "aurora-postgres",
-                            "rds-postgres",
-                            "redis",
-                            "opensearch",
-                        ),
-                        Optional("paas_description"): str,
-                        Optional("paas_instance"): str,
-                        Optional("notes"): str,
-                        Optional("bucket_name"): str,  # for external-s3 type
-                        Optional("readonly"): bool,  # for external-s3 type
-                        Optional("shared"): bool,
+                        "id": str,
                     },
-                ],
-                Optional("overlapping_secrets"): [str],
-                "secrets": {
-                    Optional(str): str,
-                },
-                "env_vars": {
-                    Optional(str): str,
                 },
-            },
-        ],
-    },
-)
-
-PIPELINES_SCHEMA = Schema(
-    {
-        Optional("accounts"): list[str],
-        Optional("environments"): [
-            {
-                "name": str,
                 Optional("requires_approval"): bool,
             },
         ],
         Optional("codebases"): [
             {
                 "name": str,
                 "repository": str,
```

### Comparing `dbt_platform_helper-8.2.1/dbt_platform_helper/utils/versioning.py` & `dbt_platform_helper-8.3.0/dbt_platform_helper/utils/versioning.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.2.1/platform_helper.py` & `dbt_platform_helper-8.3.0/platform_helper.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.2.1/pyproject.toml` & `dbt_platform_helper-8.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.black]
 line-length = 100
 
 [tool.poetry]
 name = "dbt-platform-helper"
-version = "8.2.1"
+version = "8.3.0"
 description = "Set of tools to help transfer applications/services from GOV.UK PaaS to DBT PaaS augmenting AWS Copilot."
 authors = ["Department for Business and Trade Platform Team <sre-team@digital.trade.gov.uk>"]
 license = "MIT"
 readme = "dbt_platform_helper/README.md"
 packages = [
     { include = "dbt_platform_helper" },
     { include = "platform_helper.py" }
```

### Comparing `dbt_platform_helper-8.2.1/PKG-INFO` & `dbt_platform_helper-8.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-platform-helper
-Version: 8.2.1
+Version: 8.3.0
 Summary: Set of tools to help transfer applications/services from GOV.UK PaaS to DBT PaaS augmenting AWS Copilot.
 License: MIT
 Author: Department for Business and Trade Platform Team
 Author-email: sre-team@digital.trade.gov.uk
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

