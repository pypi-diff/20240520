# Comparing `tmp/airbyte_source_github-1.7.2.tar.gz` & `tmp/airbyte_source_github-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_github-1.7.2.tar", max compression
+gzip compressed data, was "airbyte_source_github-1.7.3.tar", max compression
```

## Comparing `airbyte_source_github-1.7.2.tar` & `airbyte_source_github-1.7.3.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0     4496 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/README.md
--rw-r--r--   0        0        0      801 2024-05-07 12:18:55.974254 airbyte_source_github-1.7.2/pyproject.toml
--rw-r--r--   0        0        0     1134 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/__init__.py
--rw-r--r--   0        0        0     3849 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/config_migrations.py
--rw-r--r--   0        0        0      238 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/constants.py
--rw-r--r--   0        0        0  1600314 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/github_schema.py
--rw-r--r--   0        0        0    11625 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/graphql.py
--rw-r--r--   0        0        0      407 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/run.py
--rw-r--r--   0        0        0     2335 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/schemas/assignees.json
--rw-r--r--   0        0        0     2734 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/schemas/branches.json
--rw-r--r--   0        0        0     3505 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/schemas/collaborators.json
--rw-r--r--   0        0        0     4193 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/schemas/comments.json
--rw-r--r--   0        0        0       87 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/schemas/commit_comment_reactions.json
--rw-r--r--   0        0        0     2164 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/schemas/commit_comments.json
--rw-r--r--   0        0        0     5122 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/schemas/commits.json
--rw-r--r--   0        0        0     3957 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/schemas/contributor_activity.json
--rw-r--r--   0        0        0     2893 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/schemas/deployments.json
--rw-r--r--   0        0        0     2299 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/schemas/events.json
--rw-r--r--   0        0        0       87 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/schemas/issue_comment_reactions.json
--rw-r--r--   0        0        0    13840 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/schemas/issue_events.json
--rw-r--r--   0        0        0     1200 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/schemas/issue_labels.json
--rw-r--r--   0        0        0     2309 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/schemas/issue_milestones.json
--rw-r--r--   0        0        0      998 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/schemas/issue_reactions.json
--rw-r--r--   0        0        0    30392 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/schemas/issue_timeline_events.json
--rw-r--r--   0        0        0    11962 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/schemas/issues.json
--rw-r--r--   0        0        0     9349 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/schemas/organizations.json
--rw-r--r--   0        0        0     2016 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/schemas/project_cards.json
--rw-r--r--   0        0        0     1489 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/schemas/project_columns.json
--rw-r--r--   0        0        0     1848 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/schemas/projects.json
--rw-r--r--   0        0        0     3162 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/schemas/projects_v2.json
--rw-r--r--   0        0        0     1038 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/schemas/pull_request_comment_reactions.json
--rw-r--r--   0        0        0     4800 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/schemas/pull_request_commits.json
--rw-r--r--   0        0        0     3497 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/schemas/pull_request_stats.json
--rw-r--r--   0        0        0    12196 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/schemas/pull_requests.json
--rw-r--r--   0        0        0     5140 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/schemas/releases.json
--rw-r--r--   0        0        0    13319 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/schemas/repositories.json
--rw-r--r--   0        0        0     4905 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/schemas/review_comments.json
--rw-r--r--   0        0        0     2731 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/schemas/reviews.json
--rw-r--r--   0        0        0     7387 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/schemas/shared/events/comment.json
--rw-r--r--   0        0        0     4197 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/schemas/shared/events/commented.json
--rw-r--r--   0        0        0     1443 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/schemas/shared/events/committed.json
--rw-r--r--   0        0        0    36914 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/schemas/shared/events/cross_referenced.json
--rw-r--r--   0        0        0     2764 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/schemas/shared/events/reviewed.json
--rw-r--r--   0        0        0      449 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/schemas/shared/reaction.json
--rw-r--r--   0        0        0      616 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/schemas/shared/reactions.json
--rw-r--r--   0        0        0     1135 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/schemas/shared/user.json
--rw-r--r--   0        0        0      453 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/schemas/shared/user_graphql.json
--rw-r--r--   0        0        0      630 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/schemas/stargazers.json
--rw-r--r--   0        0        0     1133 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/schemas/tags.json
--rw-r--r--   0        0        0     2518 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/schemas/team_members.json
--rw-r--r--   0        0        0      911 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/schemas/team_memberships.json
--rw-r--r--   0        0        0     1796 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/schemas/teams.json
--rw-r--r--   0        0        0     2530 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/schemas/users.json
--rw-r--r--   0        0        0     3934 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/schemas/workflow_jobs.json
--rw-r--r--   0        0        0    19453 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/schemas/workflow_runs.json
--rw-r--r--   0        0        0     1470 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/schemas/workflows.json
--rw-r--r--   0        0        0    13879 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/source.py
--rw-r--r--   0        0        0     7074 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/spec.json
--rw-r--r--   0        0        0    77006 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/streams.py
--rw-r--r--   0        0        0     5462 2024-05-07 10:14:31.000000 airbyte_source_github-1.7.2/source_github/utils.py
--rw-r--r--   0        0        0     5230 1970-01-01 00:00:00.000000 airbyte_source_github-1.7.2/PKG-INFO
+-rw-r--r--   0        0        0     4506 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/README.md
+-rw-r--r--   0        0        0      801 2024-05-20 16:41:31.758973 airbyte_source_github-1.7.3/pyproject.toml
+-rw-r--r--   0        0        0     1134 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/__init__.py
+-rw-r--r--   0        0        0     3849 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/config_migrations.py
+-rw-r--r--   0        0        0      238 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/constants.py
+-rw-r--r--   0        0        0  1600314 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/github_schema.py
+-rw-r--r--   0        0        0    11625 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/graphql.py
+-rw-r--r--   0        0        0      407 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/run.py
+-rw-r--r--   0        0        0     2335 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/schemas/assignees.json
+-rw-r--r--   0        0        0     2734 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/schemas/branches.json
+-rw-r--r--   0        0        0     3505 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/schemas/collaborators.json
+-rw-r--r--   0        0        0     4193 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/schemas/comments.json
+-rw-r--r--   0        0        0       87 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/schemas/commit_comment_reactions.json
+-rw-r--r--   0        0        0     2164 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/schemas/commit_comments.json
+-rw-r--r--   0        0        0     5122 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/schemas/commits.json
+-rw-r--r--   0        0        0     3957 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/schemas/contributor_activity.json
+-rw-r--r--   0        0        0     2893 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/schemas/deployments.json
+-rw-r--r--   0        0        0     2299 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/schemas/events.json
+-rw-r--r--   0        0        0       87 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/schemas/issue_comment_reactions.json
+-rw-r--r--   0        0        0    13840 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/schemas/issue_events.json
+-rw-r--r--   0        0        0     1200 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/schemas/issue_labels.json
+-rw-r--r--   0        0        0     2309 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/schemas/issue_milestones.json
+-rw-r--r--   0        0        0      998 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/schemas/issue_reactions.json
+-rw-r--r--   0        0        0    30392 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/schemas/issue_timeline_events.json
+-rw-r--r--   0        0        0    11962 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/schemas/issues.json
+-rw-r--r--   0        0        0     9349 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/schemas/organizations.json
+-rw-r--r--   0        0        0     2016 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/schemas/project_cards.json
+-rw-r--r--   0        0        0     1489 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/schemas/project_columns.json
+-rw-r--r--   0        0        0     1848 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/schemas/projects.json
+-rw-r--r--   0        0        0     3162 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/schemas/projects_v2.json
+-rw-r--r--   0        0        0     1038 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/schemas/pull_request_comment_reactions.json
+-rw-r--r--   0        0        0     4800 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/schemas/pull_request_commits.json
+-rw-r--r--   0        0        0     3497 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/schemas/pull_request_stats.json
+-rw-r--r--   0        0        0    12196 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/schemas/pull_requests.json
+-rw-r--r--   0        0        0     5140 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/schemas/releases.json
+-rw-r--r--   0        0        0    13319 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/schemas/repositories.json
+-rw-r--r--   0        0        0     4905 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/schemas/review_comments.json
+-rw-r--r--   0        0        0     2731 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/schemas/reviews.json
+-rw-r--r--   0        0        0     7387 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/schemas/shared/events/comment.json
+-rw-r--r--   0        0        0     4197 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/schemas/shared/events/commented.json
+-rw-r--r--   0        0        0     1443 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/schemas/shared/events/committed.json
+-rw-r--r--   0        0        0    36914 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/schemas/shared/events/cross_referenced.json
+-rw-r--r--   0        0        0     2764 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/schemas/shared/events/reviewed.json
+-rw-r--r--   0        0        0      449 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/schemas/shared/reaction.json
+-rw-r--r--   0        0        0      616 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/schemas/shared/reactions.json
+-rw-r--r--   0        0        0     1135 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/schemas/shared/user.json
+-rw-r--r--   0        0        0      453 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/schemas/shared/user_graphql.json
+-rw-r--r--   0        0        0      630 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/schemas/stargazers.json
+-rw-r--r--   0        0        0     1133 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/schemas/tags.json
+-rw-r--r--   0        0        0     2518 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/schemas/team_members.json
+-rw-r--r--   0        0        0      911 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/schemas/team_memberships.json
+-rw-r--r--   0        0        0     1796 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/schemas/teams.json
+-rw-r--r--   0        0        0     2530 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/schemas/users.json
+-rw-r--r--   0        0        0     3934 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/schemas/workflow_jobs.json
+-rw-r--r--   0        0        0    19453 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/schemas/workflow_runs.json
+-rw-r--r--   0        0        0     1470 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/schemas/workflows.json
+-rw-r--r--   0        0        0    13879 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/source.py
+-rw-r--r--   0        0        0     7073 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/spec.json
+-rw-r--r--   0        0        0    77006 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/streams.py
+-rw-r--r--   0        0        0     5462 2024-05-20 15:28:42.000000 airbyte_source_github-1.7.3/source_github/utils.py
+-rw-r--r--   0        0        0     5240 1970-01-01 00:00:00.000000 airbyte_source_github-1.7.3/PKG-INFO
```

### Comparing `airbyte_source_github-1.7.2/README.md` & `airbyte_source_github-1.7.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,91 +1,104 @@
 # Github source connector
 
-
 This is the repository for the Github source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/github).
 
 ## Local development
 
 ### Prerequisites
-* Python (~=3.9)
-* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
+- Python (~=3.9)
+- Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
 ### Installing the connector
+
 From this connector directory, run:
+
 ```bash
 poetry install --with dev
 ```
 
-
 ### Create credentials
+
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/github)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_github/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-github spec
 poetry run source-github check --config secrets/config.json
 poetry run source-github discover --config secrets/config.json
 poetry run source-github read --config secrets/config.json --catalog sample_files/configured_catalog.json
 ```
 
 ### Running unit tests
+
 To run unit tests locally, from the connector directory run:
+
 ```
 poetry run pytest unit_tests
 ```
 
 ### Building the docker image
+
 1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
 2. Run the following command to build the docker image:
+
 ```bash
 airbyte-ci connectors --name=source-github build
 ```
 
 An image will be available on your host with the tag `airbyte/source-github:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-github:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-github:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-github:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-github:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-github test
 ```
 
 ### Customizing acceptance Tests
+
 Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
 ### Dependency Management
-All of your dependencies should be managed via Poetry. 
+
+All of your dependencies should be managed via Poetry.
 To add a new dependency, run:
+
 ```bash
 poetry add <package-name>
 ```
 
 Please commit the changes to `pyproject.toml` and `poetry.lock` files.
 
 ## Publishing a new version of the connector
+
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
+
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-github test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/github.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte_source_github-1.7.2/pyproject.toml` & `airbyte_source_github-1.7.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "1.7.2"
+version = "1.7.3"
 name = "airbyte-source-github"
 description = "Source implementation for GitHub."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `airbyte_source_github-1.7.2/source_github/__init__.py` & `airbyte_source_github-1.7.3/source_github/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.2/source_github/config_migrations.py` & `airbyte_source_github-1.7.3/source_github/config_migrations.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.2/source_github/github_schema.py` & `airbyte_source_github-1.7.3/source_github/github_schema.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.2/source_github/graphql.py` & `airbyte_source_github-1.7.3/source_github/graphql.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.2/source_github/schemas/assignees.json` & `airbyte_source_github-1.7.3/source_github/schemas/assignees.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.2/source_github/schemas/branches.json` & `airbyte_source_github-1.7.3/source_github/schemas/branches.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.2/source_github/schemas/collaborators.json` & `airbyte_source_github-1.7.3/source_github/schemas/collaborators.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.2/source_github/schemas/comments.json` & `airbyte_source_github-1.7.3/source_github/schemas/comments.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.2/source_github/schemas/commit_comments.json` & `airbyte_source_github-1.7.3/source_github/schemas/commit_comments.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.2/source_github/schemas/commits.json` & `airbyte_source_github-1.7.3/source_github/schemas/commits.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.2/source_github/schemas/contributor_activity.json` & `airbyte_source_github-1.7.3/source_github/schemas/contributor_activity.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.2/source_github/schemas/deployments.json` & `airbyte_source_github-1.7.3/source_github/schemas/deployments.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.2/source_github/schemas/events.json` & `airbyte_source_github-1.7.3/source_github/schemas/events.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.2/source_github/schemas/issue_events.json` & `airbyte_source_github-1.7.3/source_github/schemas/issue_events.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.2/source_github/schemas/issue_labels.json` & `airbyte_source_github-1.7.3/source_github/schemas/issue_labels.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.2/source_github/schemas/issue_milestones.json` & `airbyte_source_github-1.7.3/source_github/schemas/issue_milestones.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.2/source_github/schemas/issue_reactions.json` & `airbyte_source_github-1.7.3/source_github/schemas/issue_reactions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.2/source_github/schemas/issue_timeline_events.json` & `airbyte_source_github-1.7.3/source_github/schemas/issue_timeline_events.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.2/source_github/schemas/issues.json` & `airbyte_source_github-1.7.3/source_github/schemas/issues.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.2/source_github/schemas/organizations.json` & `airbyte_source_github-1.7.3/source_github/schemas/organizations.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.2/source_github/schemas/project_cards.json` & `airbyte_source_github-1.7.3/source_github/schemas/project_cards.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.2/source_github/schemas/project_columns.json` & `airbyte_source_github-1.7.3/source_github/schemas/project_columns.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.2/source_github/schemas/projects.json` & `airbyte_source_github-1.7.3/source_github/schemas/projects.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.2/source_github/schemas/projects_v2.json` & `airbyte_source_github-1.7.3/source_github/schemas/projects_v2.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.2/source_github/schemas/pull_request_comment_reactions.json` & `airbyte_source_github-1.7.3/source_github/schemas/pull_request_comment_reactions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.2/source_github/schemas/pull_request_commits.json` & `airbyte_source_github-1.7.3/source_github/schemas/pull_request_commits.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.2/source_github/schemas/pull_request_stats.json` & `airbyte_source_github-1.7.3/source_github/schemas/pull_request_stats.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.2/source_github/schemas/pull_requests.json` & `airbyte_source_github-1.7.3/source_github/schemas/pull_requests.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.2/source_github/schemas/releases.json` & `airbyte_source_github-1.7.3/source_github/schemas/releases.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.2/source_github/schemas/repositories.json` & `airbyte_source_github-1.7.3/source_github/schemas/repositories.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.2/source_github/schemas/review_comments.json` & `airbyte_source_github-1.7.3/source_github/schemas/review_comments.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.2/source_github/schemas/reviews.json` & `airbyte_source_github-1.7.3/source_github/schemas/reviews.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.2/source_github/schemas/shared/events/comment.json` & `airbyte_source_github-1.7.3/source_github/schemas/shared/events/comment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.2/source_github/schemas/shared/events/commented.json` & `airbyte_source_github-1.7.3/source_github/schemas/shared/events/commented.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.2/source_github/schemas/shared/events/committed.json` & `airbyte_source_github-1.7.3/source_github/schemas/shared/events/committed.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.2/source_github/schemas/shared/events/cross_referenced.json` & `airbyte_source_github-1.7.3/source_github/schemas/shared/events/cross_referenced.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.2/source_github/schemas/shared/events/reviewed.json` & `airbyte_source_github-1.7.3/source_github/schemas/shared/events/reviewed.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.2/source_github/schemas/shared/reactions.json` & `airbyte_source_github-1.7.3/source_github/schemas/shared/reactions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.2/source_github/schemas/shared/user.json` & `airbyte_source_github-1.7.3/source_github/schemas/shared/user.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.2/source_github/schemas/stargazers.json` & `airbyte_source_github-1.7.3/source_github/schemas/stargazers.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.2/source_github/schemas/tags.json` & `airbyte_source_github-1.7.3/source_github/schemas/tags.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.2/source_github/schemas/team_members.json` & `airbyte_source_github-1.7.3/source_github/schemas/team_members.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.2/source_github/schemas/team_memberships.json` & `airbyte_source_github-1.7.3/source_github/schemas/team_memberships.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.2/source_github/schemas/teams.json` & `airbyte_source_github-1.7.3/source_github/schemas/teams.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.2/source_github/schemas/users.json` & `airbyte_source_github-1.7.3/source_github/schemas/users.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.2/source_github/schemas/workflow_jobs.json` & `airbyte_source_github-1.7.3/source_github/schemas/workflow_jobs.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.2/source_github/schemas/workflow_runs.json` & `airbyte_source_github-1.7.3/source_github/schemas/workflow_runs.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.2/source_github/schemas/workflows.json` & `airbyte_source_github-1.7.3/source_github/schemas/workflows.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.2/source_github/source.py` & `airbyte_source_github-1.7.3/source_github/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.2/source_github/spec.json` & `airbyte_source_github-1.7.3/source_github/spec.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999999192656664%*

 * *Differences: {"'connectionSpecification'": "{'properties': {'credentials': {'oneOf': {0: {'properties': "*

 * *                              "{'client_secret': {'title': 'Client secret'}}}}}}}"}*

```diff
@@ -110,15 +110,15 @@
                                 "description": "OAuth Client Id",
                                 "title": "Client Id",
                                 "type": "string"
                             },
                             "client_secret": {
                                 "airbyte_secret": true,
                                 "description": "OAuth Client secret",
-                                "title": "Client ssecret",
+                                "title": "Client secret",
                                 "type": "string"
                             },
                             "option_title": {
                                 "const": "OAuth Credentials",
                                 "order": 0,
                                 "type": "string"
                             }
```

### Comparing `airbyte_source_github-1.7.2/source_github/streams.py` & `airbyte_source_github-1.7.3/source_github/streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.2/source_github/utils.py` & `airbyte_source_github-1.7.3/source_github/utils.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.2/PKG-INFO` & `airbyte_source_github-1.7.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-github
-Version: 1.7.2
+Version: 1.7.3
 Summary: Source implementation for GitHub.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -16,96 +16,110 @@
 Requires-Dist: sgqlc (==16.3)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/github
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Github source connector
 
-
 This is the repository for the Github source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/github).
 
 ## Local development
 
 ### Prerequisites
-* Python (~=3.9)
-* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
+- Python (~=3.9)
+- Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
 ### Installing the connector
+
 From this connector directory, run:
+
 ```bash
 poetry install --with dev
 ```
 
-
 ### Create credentials
+
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/github)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_github/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-github spec
 poetry run source-github check --config secrets/config.json
 poetry run source-github discover --config secrets/config.json
 poetry run source-github read --config secrets/config.json --catalog sample_files/configured_catalog.json
 ```
 
 ### Running unit tests
+
 To run unit tests locally, from the connector directory run:
+
 ```
 poetry run pytest unit_tests
 ```
 
 ### Building the docker image
+
 1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
 2. Run the following command to build the docker image:
+
 ```bash
 airbyte-ci connectors --name=source-github build
 ```
 
 An image will be available on your host with the tag `airbyte/source-github:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-github:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-github:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-github:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-github:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-github test
 ```
 
 ### Customizing acceptance Tests
+
 Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
 ### Dependency Management
-All of your dependencies should be managed via Poetry. 
+
+All of your dependencies should be managed via Poetry.
 To add a new dependency, run:
+
 ```bash
 poetry add <package-name>
 ```
 
 Please commit the changes to `pyproject.toml` and `poetry.lock` files.
 
 ## Publishing a new version of the connector
+
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
+
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-github test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/github.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
 8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+
```

