# Comparing `tmp/patchwork_cli-0.0.87.tar.gz` & `tmp/patchwork_cli-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "patchwork_cli-0.0.87.tar", max compression
+gzip compressed data, was "patchwork_cli-0.0.9.tar", max compression
```

## Comparing `patchwork_cli-0.0.87.tar` & `patchwork_cli-0.0.9.tar`

### file list

```diff
@@ -1,132 +1,132 @@
--rw-r--r--   0        0        0    34523 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/LICENSE
--rw-r--r--   0        0        0     5037 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/README.md
--rw-r--r--   0        0        0        0 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/__init__.py
--rw-r--r--   0        0        0        0 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/__main__.py
--rw-r--r--   0        0        0     5253 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/app.py
--rw-r--r--   0        0        0        0 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/common/client/__init__.py
--rw-r--r--   0        0        0    15540 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/common/client/scm.py
--rw-r--r--   0        0        0     3945 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/common/utils.py
--rw-r--r--   0        0        0     1546 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/logger.py
--rw-r--r--   0        0        0      168 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/managed_files.py
--rw-r--r--   0        0        0     3718 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/patchflows/AutoFix/AutoFix.py
--rw-r--r--   0        0        0     6059 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/patchflows/AutoFix/README.md
--rw-r--r--   0        0        0     2182 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/patchflows/AutoFix/default_prompt.json
--rw-r--r--   0        0        0      919 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/patchflows/AutoFix/defaults.yml
--rw-r--r--   0        0        0     5422 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/patchflows/DependencyUpgrade/DependencyUpgrade.py
--rw-r--r--   0        0        0     5441 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/patchflows/DependencyUpgrade/README.md
--rw-r--r--   0        0        0      754 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/patchflows/DependencyUpgrade/defaults.yml
--rw-r--r--   0        0        0     2495 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/patchflows/DependencyUpgrade/dependency_upgrade_prompt.json
--rw-r--r--   0        0        0     2204 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/patchflows/GenerateREADME/GenerateREADME.py
--rw-r--r--   0        0        0     3855 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/patchflows/GenerateREADME/README.md
--rw-r--r--   0        0        0      662 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/patchflows/GenerateREADME/defaults.yml
--rw-r--r--   0        0        0      484 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/patchflows/GenerateREADME/generate_readme_prompt.json
--rw-r--r--   0        0        0     3542 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/patchflows/PRReview/PRReview.py
--rw-r--r--   0        0        0     3653 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/patchflows/PRReview/README.md
--rw-r--r--   0        0        0        0 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/patchflows/PRReview/__init__.py
--rw-r--r--   0        0        0      659 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/patchflows/PRReview/defaults.yml
--rw-r--r--   0        0        0      557 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/patchflows/PRReview/pr_review_prompt.json
--rw-r--r--   0        0        0     2163 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/patchflows/README.md
--rw-r--r--   0        0        0     3773 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/patchflows/ResolveIssue/README.md
--rw-r--r--   0        0        0     3819 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/patchflows/ResolveIssue/ResolveIssue.py
--rw-r--r--   0        0        0        0 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/patchflows/ResolveIssue/__init__.py
--rw-r--r--   0        0        0      714 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/patchflows/ResolveIssue/defaults.yml
--rw-r--r--   0        0        0      728 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/patchflows/ResolveIssue/prompt.json
--rw-r--r--   0        0        0      344 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/patchflows/__init__.py
--rw-r--r--   0        0        0      499 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/step.py
--rw-r--r--   0        0        0     5984 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/steps/AnalyzeImpact/AnalyzeImpact.py
--rw-r--r--   0        0        0     1205 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/steps/AnalyzeImpact/README.md
--rw-r--r--   0        0        0        0 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/steps/AnalyzeImpact/__init__.py
--rw-r--r--   0        0        0      501 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/steps/AnalyzeImpact/typed.py
--rw-r--r--   0        0        0     2461 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/steps/CallCode2Prompt/CallCode2Prompt.py
--rw-r--r--   0        0        0      967 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/steps/CallCode2Prompt/README.md
--rw-r--r--   0        0        0      575 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/steps/CallCode2Prompt/TestCallCode2Prompt.py
--rw-r--r--   0        0        0        0 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/steps/CallCode2Prompt/__init__.py
--rw-r--r--   0        0        0      303 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/steps/CallCode2Prompt/typed.py
--rw-r--r--   0        0        0     7462 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/steps/CallLLM/CallLLM.py
--rw-r--r--   0        0        0      503 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/steps/CallLLM/README.md
--rw-r--r--   0        0        0        0 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/steps/CallLLM/__init__.py
--rw-r--r--   0        0        0      453 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/steps/CallLLM/typed.py
--rw-r--r--   0        0        0     5255 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/steps/CommitChanges/CommitChanges.py
--rw-r--r--   0        0        0     1106 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/steps/CommitChanges/README.md
--rw-r--r--   0        0        0        0 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/steps/CommitChanges/__init__.py
--rw-r--r--   0        0        0      368 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/steps/CommitChanges/typed.py
--rw-r--r--   0        0        0     1346 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/steps/CreateIssueComment/CreateIssueComment.py
--rw-r--r--   0        0        0      541 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/steps/CreateIssueComment/README.md
--rw-r--r--   0        0        0        0 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/steps/CreateIssueComment/__init__.py
--rw-r--r--   0        0        0      320 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/steps/CreateIssueComment/typed.py
--rw-r--r--   0        0        0     3907 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/CreatePR/CreatePR.py
--rw-r--r--   0        0        0     1279 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/CreatePR/README.md
--rw-r--r--   0        0        0        0 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/CreatePR/__init__.py
--rw-r--r--   0        0        0      437 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/CreatePR/typed.py
--rw-r--r--   0        0        0     1358 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/CreatePRComment/CreatePRComment.py
--rw-r--r--   0        0        0      621 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/CreatePRComment/README.md
--rw-r--r--   0        0        0        0 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/CreatePRComment/__init__.py
--rw-r--r--   0        0        0      326 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/CreatePRComment/typed.py
--rw-r--r--   0        0        0    11511 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ExtractCode/ExtractCode.py
--rw-r--r--   0        0        0      755 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ExtractCode/README.md
--rw-r--r--   0        0        0        0 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ExtractCode/__init__.py
--rw-r--r--   0        0        0        0 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ExtractCode/context_strategy/__init__.py
--rw-r--r--   0        0        0     2585 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ExtractCode/context_strategy/context_strategies.py
--rw-r--r--   0        0        0      593 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ExtractCode/context_strategy/generic.py
--rw-r--r--   0        0        0     1491 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ExtractCode/context_strategy/java.py
--rw-r--r--   0        0        0     2442 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ExtractCode/context_strategy/javascript.py
--rw-r--r--   0        0        0      281 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ExtractCode/context_strategy/protocol.py
--rw-r--r--   0        0        0     2885 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ExtractCode/context_strategy/python.py
--rw-r--r--   0        0        0      463 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ExtractCode/typed.py
--rw-r--r--   0        0        0     8722 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ExtractDiff/ExtractDiff.py
--rw-r--r--   0        0        0      833 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ExtractDiff/README.md
--rw-r--r--   0        0        0        0 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ExtractDiff/__init__.py
--rw-r--r--   0        0        0      404 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ExtractDiff/typed.py
--rw-r--r--   0        0        0     1648 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ExtractModelResponse/ExtractModelResponse.py
--rw-r--r--   0        0        0     1318 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ExtractModelResponse/README.md
--rw-r--r--   0        0        0        0 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ExtractModelResponse/__init__.py
--rw-r--r--   0        0        0      301 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ExtractModelResponse/typed.py
--rw-r--r--   0        0        0    12415 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ExtractPackageManagerFile/ExtractPackageManagerFile.py
--rw-r--r--   0        0        0     1765 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ExtractPackageManagerFile/README.md
--rw-r--r--   0        0        0     6173 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ExtractPackageManagerFile/TestExtractPackageManagerFile.py
--rw-r--r--   0        0        0        0 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ExtractPackageManagerFile/__init__.py
--rw-r--r--   0        0        0      338 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ExtractPackageManagerFile/typed.py
--rw-r--r--   0        0        0     5337 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/GenerateCodeRepositoryEmbeddings/GenerateCodeRepositoryEmbeddings.py
--rw-r--r--   0        0        0     1572 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/GenerateCodeRepositoryEmbeddings/README.md
--rw-r--r--   0        0        0        0 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/GenerateCodeRepositoryEmbeddings/__init__.py
--rw-r--r--   0        0        0      211 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/GenerateCodeRepositoryEmbeddings/typed.py
--rw-r--r--   0        0        0     2941 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/GenerateEmbeddings/GenerateEmbeddings.py
--rw-r--r--   0        0        0     1011 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/GenerateEmbeddings/README.md
--rw-r--r--   0        0        0        0 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/GenerateEmbeddings/__init__.py
--rw-r--r--   0        0        0      238 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/GenerateEmbeddings/typed.py
--rw-r--r--   0        0        0     3366 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ModifyCode/ModifyCode.py
--rw-r--r--   0        0        0     1045 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ModifyCode/README.md
--rw-r--r--   0        0        0        0 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ModifyCode/__init__.py
--rw-r--r--   0        0        0      346 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ModifyCode/typed.py
--rw-r--r--   0        0        0     3125 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/PreparePR/PreparePR.py
--rw-r--r--   0        0        0      743 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/PreparePR/README.md
--rw-r--r--   0        0        0        0 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/PreparePR/__init__.py
--rw-r--r--   0        0        0      327 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/PreparePR/typed.py
--rw-r--r--   0        0        0     3289 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/PreparePrompt/PreparePrompt.py
--rw-r--r--   0        0        0     1274 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/PreparePrompt/README.md
--rw-r--r--   0        0        0        0 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/PreparePrompt/__init__.py
--rw-r--r--   0        0        0      335 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/PreparePrompt/typed.py
--rw-r--r--   0        0        0     2617 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/QueryEmbeddings/QueryEmbeddings.py
--rw-r--r--   0        0        0     1117 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/QueryEmbeddings/README.md
--rw-r--r--   0        0        0        0 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/QueryEmbeddings/__init__.py
--rw-r--r--   0        0        0      313 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/QueryEmbeddings/typed.py
--rw-r--r--   0        0        0     1652 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/README.md
--rw-r--r--   0        0        0     1078 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ReadIssues/README.md
--rw-r--r--   0        0        0     1149 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ReadIssues/ReadIssues.py
--rw-r--r--   0        0        0        0 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ReadIssues/__init__.py
--rw-r--r--   0        0        0      277 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ReadIssues/typed.py
--rw-r--r--   0        0        0      903 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ReadPRDiffs/README.md
--rw-r--r--   0        0        0     1830 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ReadPRDiffs/ReadPRDiffs.py
--rw-r--r--   0        0        0        0 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ReadPRDiffs/__init__.py
--rw-r--r--   0        0        0      362 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ReadPRDiffs/typed.py
--rw-r--r--   0        0        0     1588 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ScanDepscan/README.md
--rw-r--r--   0        0        0     4884 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ScanDepscan/ScanDepscan.py
--rw-r--r--   0        0        0        0 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ScanDepscan/__init__.py
--rw-r--r--   0        0        0      189 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ScanDepscan/typed.py
--rw-r--r--   0        0        0      677 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ScanSemgrep/README.md
--rw-r--r--   0        0        0     1096 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ScanSemgrep/ScanSemgrep.py
--rw-r--r--   0        0        0        0 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ScanSemgrep/__init__.py
--rw-r--r--   0        0        0      193 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ScanSemgrep/typed.py
--rw-r--r--   0        0        0     2045 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/__init__.py
--rw-r--r--   0        0        0     2286 2024-05-09 09:16:47.293329 patchwork_cli-0.0.87/pyproject.toml
--rw-r--r--   0        0        0     6852 1970-01-01 00:00:00.000000 patchwork_cli-0.0.87/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-05-20 07:15:51.385954 patchwork_cli-0.0.9/LICENSE
+-rw-r--r--   0        0        0     6460 2024-05-20 07:15:51.385954 patchwork_cli-0.0.9/README.md
+-rw-r--r--   0        0        0        0 2024-05-20 07:15:51.385954 patchwork_cli-0.0.9/patchwork/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-20 07:15:51.385954 patchwork_cli-0.0.9/patchwork/__main__.py
+-rw-r--r--   0        0        0     6551 2024-05-20 07:15:51.385954 patchwork_cli-0.0.9/patchwork/app.py
+-rw-r--r--   0        0        0        0 2024-05-20 07:15:51.385954 patchwork_cli-0.0.9/patchwork/common/client/__init__.py
+-rw-r--r--   0        0        0    15551 2024-05-20 07:15:51.385954 patchwork_cli-0.0.9/patchwork/common/client/scm.py
+-rw-r--r--   0        0        0     3956 2024-05-20 07:15:51.385954 patchwork_cli-0.0.9/patchwork/common/utils.py
+-rw-r--r--   0        0        0     1703 2024-05-20 07:15:51.385954 patchwork_cli-0.0.9/patchwork/logger.py
+-rw-r--r--   0        0        0      168 2024-05-20 07:15:51.385954 patchwork_cli-0.0.9/patchwork/managed_files.py
+-rw-r--r--   0        0        0     3718 2024-05-20 07:15:51.385954 patchwork_cli-0.0.9/patchwork/patchflows/AutoFix/AutoFix.py
+-rw-r--r--   0        0        0     6059 2024-05-20 07:15:51.385954 patchwork_cli-0.0.9/patchwork/patchflows/AutoFix/README.md
+-rw-r--r--   0        0        0     2182 2024-05-20 07:15:51.385954 patchwork_cli-0.0.9/patchwork/patchflows/AutoFix/default_prompt.json
+-rw-r--r--   0        0        0      919 2024-05-20 07:15:51.385954 patchwork_cli-0.0.9/patchwork/patchflows/AutoFix/defaults.yml
+-rw-r--r--   0        0        0     5422 2024-05-20 07:15:51.385954 patchwork_cli-0.0.9/patchwork/patchflows/DependencyUpgrade/DependencyUpgrade.py
+-rw-r--r--   0        0        0     5441 2024-05-20 07:15:51.385954 patchwork_cli-0.0.9/patchwork/patchflows/DependencyUpgrade/README.md
+-rw-r--r--   0        0        0      754 2024-05-20 07:15:51.385954 patchwork_cli-0.0.9/patchwork/patchflows/DependencyUpgrade/defaults.yml
+-rw-r--r--   0        0        0     2495 2024-05-20 07:15:51.385954 patchwork_cli-0.0.9/patchwork/patchflows/DependencyUpgrade/dependency_upgrade_prompt.json
+-rw-r--r--   0        0        0     2204 2024-05-20 07:15:51.385954 patchwork_cli-0.0.9/patchwork/patchflows/GenerateREADME/GenerateREADME.py
+-rw-r--r--   0        0        0     3855 2024-05-20 07:15:51.385954 patchwork_cli-0.0.9/patchwork/patchflows/GenerateREADME/README.md
+-rw-r--r--   0        0        0      662 2024-05-20 07:15:51.385954 patchwork_cli-0.0.9/patchwork/patchflows/GenerateREADME/defaults.yml
+-rw-r--r--   0        0        0      484 2024-05-20 07:15:51.385954 patchwork_cli-0.0.9/patchwork/patchflows/GenerateREADME/generate_readme_prompt.json
+-rw-r--r--   0        0        0     3542 2024-05-20 07:15:51.385954 patchwork_cli-0.0.9/patchwork/patchflows/PRReview/PRReview.py
+-rw-r--r--   0        0        0     3653 2024-05-20 07:15:51.385954 patchwork_cli-0.0.9/patchwork/patchflows/PRReview/README.md
+-rw-r--r--   0        0        0        0 2024-05-20 07:15:51.385954 patchwork_cli-0.0.9/patchwork/patchflows/PRReview/__init__.py
+-rw-r--r--   0        0        0      659 2024-05-20 07:15:51.385954 patchwork_cli-0.0.9/patchwork/patchflows/PRReview/defaults.yml
+-rw-r--r--   0        0        0      557 2024-05-20 07:15:51.385954 patchwork_cli-0.0.9/patchwork/patchflows/PRReview/pr_review_prompt.json
+-rw-r--r--   0        0        0     2163 2024-05-20 07:15:51.385954 patchwork_cli-0.0.9/patchwork/patchflows/README.md
+-rw-r--r--   0        0        0     3773 2024-05-20 07:15:51.385954 patchwork_cli-0.0.9/patchwork/patchflows/ResolveIssue/README.md
+-rw-r--r--   0        0        0     3875 2024-05-20 07:15:51.385954 patchwork_cli-0.0.9/patchwork/patchflows/ResolveIssue/ResolveIssue.py
+-rw-r--r--   0        0        0        0 2024-05-20 07:15:51.385954 patchwork_cli-0.0.9/patchwork/patchflows/ResolveIssue/__init__.py
+-rw-r--r--   0        0        0      714 2024-05-20 07:15:51.385954 patchwork_cli-0.0.9/patchwork/patchflows/ResolveIssue/defaults.yml
+-rw-r--r--   0        0        0      964 2024-05-20 07:15:51.385954 patchwork_cli-0.0.9/patchwork/patchflows/ResolveIssue/prompt.json
+-rw-r--r--   0        0        0      344 2024-05-20 07:15:51.385954 patchwork_cli-0.0.9/patchwork/patchflows/__init__.py
+-rw-r--r--   0        0        0      510 2024-05-20 07:15:51.385954 patchwork_cli-0.0.9/patchwork/step.py
+-rw-r--r--   0        0        0     5745 2024-05-20 07:15:51.385954 patchwork_cli-0.0.9/patchwork/steps/AnalyzeImpact/AnalyzeImpact.py
+-rw-r--r--   0        0        0     1205 2024-05-20 07:15:51.385954 patchwork_cli-0.0.9/patchwork/steps/AnalyzeImpact/README.md
+-rw-r--r--   0        0        0        0 2024-05-20 07:15:51.385954 patchwork_cli-0.0.9/patchwork/steps/AnalyzeImpact/__init__.py
+-rw-r--r--   0        0        0      559 2024-05-20 07:15:51.385954 patchwork_cli-0.0.9/patchwork/steps/AnalyzeImpact/typed.py
+-rw-r--r--   0        0        0     2229 2024-05-20 07:15:51.385954 patchwork_cli-0.0.9/patchwork/steps/CallCode2Prompt/CallCode2Prompt.py
+-rw-r--r--   0        0        0      967 2024-05-20 07:15:51.385954 patchwork_cli-0.0.9/patchwork/steps/CallCode2Prompt/README.md
+-rw-r--r--   0        0        0      575 2024-05-20 07:15:51.385954 patchwork_cli-0.0.9/patchwork/steps/CallCode2Prompt/TestCallCode2Prompt.py
+-rw-r--r--   0        0        0        0 2024-05-20 07:15:51.385954 patchwork_cli-0.0.9/patchwork/steps/CallCode2Prompt/__init__.py
+-rw-r--r--   0        0        0      308 2024-05-20 07:15:51.385954 patchwork_cli-0.0.9/patchwork/steps/CallCode2Prompt/typed.py
+-rw-r--r--   0        0        0     7276 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/CallLLM/CallLLM.py
+-rw-r--r--   0        0        0      503 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/CallLLM/README.md
+-rw-r--r--   0        0        0        0 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/CallLLM/__init__.py
+-rw-r--r--   0        0        0      513 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/CallLLM/typed.py
+-rw-r--r--   0        0        0     5266 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/CommitChanges/CommitChanges.py
+-rw-r--r--   0        0        0     1106 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/CommitChanges/README.md
+-rw-r--r--   0        0        0        0 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/CommitChanges/__init__.py
+-rw-r--r--   0        0        0      368 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/CommitChanges/typed.py
+-rw-r--r--   0        0        0     1346 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/CreateIssueComment/CreateIssueComment.py
+-rw-r--r--   0        0        0      541 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/CreateIssueComment/README.md
+-rw-r--r--   0        0        0        0 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/CreateIssueComment/__init__.py
+-rw-r--r--   0        0        0      320 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/CreateIssueComment/typed.py
+-rw-r--r--   0        0        0     3907 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/CreatePR/CreatePR.py
+-rw-r--r--   0        0        0     1279 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/CreatePR/README.md
+-rw-r--r--   0        0        0        0 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/CreatePR/__init__.py
+-rw-r--r--   0        0        0      437 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/CreatePR/typed.py
+-rw-r--r--   0        0        0     1358 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/CreatePRComment/CreatePRComment.py
+-rw-r--r--   0        0        0      621 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/CreatePRComment/README.md
+-rw-r--r--   0        0        0        0 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/CreatePRComment/__init__.py
+-rw-r--r--   0        0        0      326 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/CreatePRComment/typed.py
+-rw-r--r--   0        0        0    10907 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/ExtractCode/ExtractCode.py
+-rw-r--r--   0        0        0      755 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/ExtractCode/README.md
+-rw-r--r--   0        0        0        0 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/ExtractCode/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/ExtractCode/context_strategy/__init__.py
+-rw-r--r--   0        0        0     2585 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/ExtractCode/context_strategy/context_strategies.py
+-rw-r--r--   0        0        0      604 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/ExtractCode/context_strategy/generic.py
+-rw-r--r--   0        0        0     1501 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/ExtractCode/context_strategy/java.py
+-rw-r--r--   0        0        0     2452 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/ExtractCode/context_strategy/javascript.py
+-rw-r--r--   0        0        0      292 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/ExtractCode/context_strategy/protocol.py
+-rw-r--r--   0        0        0     2895 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/ExtractCode/context_strategy/python.py
+-rw-r--r--   0        0        0      486 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/ExtractCode/typed.py
+-rw-r--r--   0        0        0     8530 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/ExtractDiff/ExtractDiff.py
+-rw-r--r--   0        0        0      833 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/ExtractDiff/README.md
+-rw-r--r--   0        0        0        0 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/ExtractDiff/__init__.py
+-rw-r--r--   0        0        0      421 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/ExtractDiff/typed.py
+-rw-r--r--   0        0        0     1648 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/ExtractModelResponse/ExtractModelResponse.py
+-rw-r--r--   0        0        0     1318 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/ExtractModelResponse/README.md
+-rw-r--r--   0        0        0        0 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/ExtractModelResponse/__init__.py
+-rw-r--r--   0        0        0      301 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/ExtractModelResponse/typed.py
+-rw-r--r--   0        0        0    12412 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/ExtractPackageManagerFile/ExtractPackageManagerFile.py
+-rw-r--r--   0        0        0     1765 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/ExtractPackageManagerFile/README.md
+-rw-r--r--   0        0        0     6173 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/ExtractPackageManagerFile/TestExtractPackageManagerFile.py
+-rw-r--r--   0        0        0        0 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/ExtractPackageManagerFile/__init__.py
+-rw-r--r--   0        0        0      423 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/ExtractPackageManagerFile/typed.py
+-rw-r--r--   0        0        0     6168 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/GenerateCodeRepositoryEmbeddings/GenerateCodeRepositoryEmbeddings.py
+-rw-r--r--   0        0        0     1572 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/GenerateCodeRepositoryEmbeddings/README.md
+-rw-r--r--   0        0        0        0 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/GenerateCodeRepositoryEmbeddings/__init__.py
+-rw-r--r--   0        0        0      252 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/GenerateCodeRepositoryEmbeddings/typed.py
+-rw-r--r--   0        0        0     3425 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/GenerateEmbeddings/GenerateEmbeddings.py
+-rw-r--r--   0        0        0     1011 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/GenerateEmbeddings/README.md
+-rw-r--r--   0        0        0        0 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/GenerateEmbeddings/__init__.py
+-rw-r--r--   0        0        0      269 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/GenerateEmbeddings/typed.py
+-rw-r--r--   0        0        0     3316 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/ModifyCode/ModifyCode.py
+-rw-r--r--   0        0        0     1045 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/ModifyCode/README.md
+-rw-r--r--   0        0        0        0 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/ModifyCode/__init__.py
+-rw-r--r--   0        0        0      362 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/ModifyCode/typed.py
+-rw-r--r--   0        0        0     3125 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/PreparePR/PreparePR.py
+-rw-r--r--   0        0        0      743 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/PreparePR/README.md
+-rw-r--r--   0        0        0        0 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/PreparePR/__init__.py
+-rw-r--r--   0        0        0      327 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/PreparePR/typed.py
+-rw-r--r--   0        0        0     3084 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/PreparePrompt/PreparePrompt.py
+-rw-r--r--   0        0        0     1274 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/PreparePrompt/README.md
+-rw-r--r--   0        0        0        0 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/PreparePrompt/__init__.py
+-rw-r--r--   0        0        0      323 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/PreparePrompt/typed.py
+-rw-r--r--   0        0        0     2617 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/QueryEmbeddings/QueryEmbeddings.py
+-rw-r--r--   0        0        0     1117 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/QueryEmbeddings/README.md
+-rw-r--r--   0        0        0        0 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/QueryEmbeddings/__init__.py
+-rw-r--r--   0        0        0      294 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/QueryEmbeddings/typed.py
+-rw-r--r--   0        0        0     1652 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/README.md
+-rw-r--r--   0        0        0     1078 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/ReadIssues/README.md
+-rw-r--r--   0        0        0     1149 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/ReadIssues/ReadIssues.py
+-rw-r--r--   0        0        0        0 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/ReadIssues/__init__.py
+-rw-r--r--   0        0        0      277 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/ReadIssues/typed.py
+-rw-r--r--   0        0        0      903 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/ReadPRDiffs/README.md
+-rw-r--r--   0        0        0     1555 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/ReadPRDiffs/ReadPRDiffs.py
+-rw-r--r--   0        0        0        0 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/ReadPRDiffs/__init__.py
+-rw-r--r--   0        0        0      362 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/ReadPRDiffs/typed.py
+-rw-r--r--   0        0        0     1588 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/ScanDepscan/README.md
+-rw-r--r--   0        0        0     5253 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/ScanDepscan/ScanDepscan.py
+-rw-r--r--   0        0        0        0 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/ScanDepscan/__init__.py
+-rw-r--r--   0        0        0      186 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/ScanDepscan/typed.py
+-rw-r--r--   0        0        0      677 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/ScanSemgrep/README.md
+-rw-r--r--   0        0        0     1555 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/ScanSemgrep/ScanSemgrep.py
+-rw-r--r--   0        0        0        0 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/ScanSemgrep/__init__.py
+-rw-r--r--   0        0        0      288 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/ScanSemgrep/typed.py
+-rw-r--r--   0        0        0     2045 2024-05-20 07:15:51.389954 patchwork_cli-0.0.9/patchwork/steps/__init__.py
+-rw-r--r--   0        0        0     2313 2024-05-20 07:15:51.393954 patchwork_cli-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     8424 1970-01-01 00:00:00.000000 patchwork_cli-0.0.9/PKG-INFO
```

### Comparing `patchwork_cli-0.0.87/LICENSE` & `patchwork_cli-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.87/patchwork/app.py` & `patchwork_cli-0.0.9/patchwork/app.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import importlib
 import importlib.util
 import json
 import traceback
 from collections import deque
 from pathlib import Path
 from types import ModuleType
-from typing import Iterable
 
 import click
 import yaml
+from click import echo
+from typing_extensions import Iterable
 
 from patchwork.logger import init_cli_logger, logger
 from patchwork.steps.PreparePrompt import PreparePrompt
 
 _DATA_FORMAT_MAPPING = {
     "yaml": yaml.dump,
     "json": json.dumps,
@@ -20,30 +21,73 @@
 
 _CONFIG_NAME = "config.yml"
 _PROMPT_NAME = "prompt.json"
 _PATCHFLOW_MODULE_NAME = "patchwork.patchflows"
 
 
 def _get_config_path(config: str | None, patchflow: str) -> Path | None:
-    prompt_path = None
     config_path = Path(config)
     if config_path.is_dir():
         patchwork_path = config_path / patchflow
         if patchwork_path.is_dir():
             return patchwork_path
 
 
+def _get_patchflow_names(base_path: Path | str | None) -> Iterable[str]:
+    names = []
+    if base_path is None:
+        return names
+
+    base_path = Path(base_path)
+    if not base_path.is_dir():
+        return names
+
+    for path in base_path.iterdir():
+        if path.is_dir() and (path / f"{path.name}.py").is_file():
+            names.append(path.name)
+    return names
+
+
+def list_option_callback(ctx: click.Context, param: click.Parameter, value: str | None) -> None:
+    if not value or ctx.resilient_parsing:
+        return
+
+    patchflows = []
+    default_path = Path(__file__).parent / "patchflows"
+    patchflows.extend(_get_patchflow_names(default_path))
+
+    config_path = ctx.params.get("config")
+    patchflows.extend(_get_patchflow_names(config_path))
+
+    echo("\n".join(patchflows), color=ctx.color)
+    ctx.exit()
+
+
 @click.command(
     context_settings=dict(
         ignore_unknown_options=True,
     )
 )
 @click.version_option(message="%(version)s", package_name="patchwork-cli")
 @click.help_option("-h", "--help")
 @click.option(
+    "--config",
+    is_eager=True,
+    type=click.Path(exists=True, dir_okay=True, resolve_path=True, file_okay=True),
+    help="Path to the configurations folder, see https://github.com/patched-codes/patchwork-configs for examples.",
+)
+@click.option(
+    "-l",
+    "--list",
+    is_flag=True,
+    expose_value=False,
+    callback=list_option_callback,
+    help="Show a list of available patchflows, see https://docs.patched.codes/patchflows/patchflows for details.",
+)
+@click.option(
     "--log",
     hidden=True,
     default="INFO",
     type=click.Choice(
         [
             "CRITICAL",
             "FATAL",
@@ -56,17 +100,16 @@
         case_sensitive=False,
     ),
     is_eager=True,
     callback=lambda x, y, z: init_cli_logger(z),
 )
 @click.argument("patchflow", nargs=1, required=True)
 @click.argument("opts", nargs=-1, type=click.UNPROCESSED, required=False)
-@click.option("--config", type=click.Path(exists=True, dir_okay=True, resolve_path=True, file_okay=True))
-@click.option("--output", type=click.Path(exists=False, resolve_path=True, writable=True), help="Output data file")
-@click.option("data_format", "--format", type=click.Choice(["yaml", "json"]), default="json", help="Output data format")
+@click.option("--output", type=click.Path(exists=False, resolve_path=True, writable=True), help="Path to the output file which contains the state after the patchflow finishes.")
+@click.option("data_format", "--format", type=click.Choice(["yaml", "json"]), default="json", help="Format of the output file.")
 def cli(log: str, patchflow: str, opts: list[str], config: str | None, output: str | None, data_format: str):
     if "::" in patchflow:
         module_path, _, patchflow_name = patchflow.partition("::")
     else:
         patchflow_name = patchflow
         module_path = _PATCHFLOW_MODULE_NAME
```

### Comparing `patchwork_cli-0.0.87/patchwork/common/client/scm.py` & `patchwork_cli-0.0.9/patchwork/common/client/scm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import functools
 import hashlib
 from dataclasses import dataclass
 from itertools import chain
-from typing import Protocol
 
 import gitlab.const
 from github import Auth, Consts, Github, GithubException, PullRequest
 from gitlab import Gitlab, GitlabAuthenticationError, GitlabError
 from gitlab.v4.objects import ProjectMergeRequest
+from typing_extensions import Protocol
 
 from patchwork.logger import logger
 
 
 @dataclass(slots=True)
 class Comment:
     path: str
```

### Comparing `patchwork_cli-0.0.87/patchwork/common/utils.py` & `patchwork_cli-0.0.9/patchwork/common/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import atexit
 import signal
 import tempfile
 from pathlib import Path
-from typing import Callable
 
 import tiktoken
 from chardet.universaldetector import UniversalDetector
 from chromadb.api.types import Documents, EmbeddingFunction
 from chromadb.utils import embedding_functions
+from typing_extensions import Callable
 
 from patchwork.managed_files import HOME_FOLDER
 
 _CLEANUP_FILES: set[Path] = set()
 
 
 def _cleanup_files():
```

### Comparing `patchwork_cli-0.0.87/patchwork/logger.py` & `patchwork_cli-0.0.9/patchwork/logger.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
-from typing import Callable
-
+import os
 import click
+from typing_extensions import Callable
 
-from patchwork.managed_files import LOG_FILE
+from patchwork.managed_files import LOG_FILE, HOME_FOLDER
 
 # default noop logger
 logger = logging.getLogger("patched")
 _noop = logging.NullHandler()
 logger.addHandler(_noop)
 
 
@@ -38,14 +38,16 @@
 
 def init_cli_logger(log_level: str) -> logging.Logger:
     global logger, _noop
 
     logger.removeHandler(_noop)
     logger.addHandler(ClickHandler(log_level.upper()))
     logger.setLevel(logging.DEBUG)
+    if not os.path.exists(HOME_FOLDER):        # Check if HOME_FOLDER exists at this point
+        os.makedirs(HOME_FOLDER)
 
     try:
         fh = logging.FileHandler(LOG_FILE, mode="w")
     except FileNotFoundError:
         logger.error(f"Unable to create log file: {LOG_FILE}")
         return logger
```

### Comparing `patchwork_cli-0.0.87/patchwork/patchflows/AutoFix/AutoFix.py` & `patchwork_cli-0.0.9/patchwork/patchflows/AutoFix/AutoFix.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.87/patchwork/patchflows/AutoFix/README.md` & `patchwork_cli-0.0.9/patchwork/patchflows/AutoFix/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.87/patchwork/patchflows/AutoFix/default_prompt.json` & `patchwork_cli-0.0.9/patchwork/patchflows/AutoFix/default_prompt.json`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.87/patchwork/patchflows/AutoFix/defaults.yml` & `patchwork_cli-0.0.9/patchwork/patchflows/AutoFix/defaults.yml`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.87/patchwork/patchflows/DependencyUpgrade/DependencyUpgrade.py` & `patchwork_cli-0.0.9/patchwork/patchflows/DependencyUpgrade/DependencyUpgrade.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.87/patchwork/patchflows/DependencyUpgrade/README.md` & `patchwork_cli-0.0.9/patchwork/patchflows/DependencyUpgrade/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.87/patchwork/patchflows/DependencyUpgrade/defaults.yml` & `patchwork_cli-0.0.9/patchwork/patchflows/DependencyUpgrade/defaults.yml`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.87/patchwork/patchflows/DependencyUpgrade/dependency_upgrade_prompt.json` & `patchwork_cli-0.0.9/patchwork/patchflows/DependencyUpgrade/dependency_upgrade_prompt.json`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.87/patchwork/patchflows/GenerateREADME/GenerateREADME.py` & `patchwork_cli-0.0.9/patchwork/patchflows/GenerateREADME/GenerateREADME.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.87/patchwork/patchflows/GenerateREADME/README.md` & `patchwork_cli-0.0.9/patchwork/patchflows/GenerateREADME/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.87/patchwork/patchflows/GenerateREADME/defaults.yml` & `patchwork_cli-0.0.9/patchwork/patchflows/GenerateREADME/defaults.yml`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.87/patchwork/patchflows/PRReview/PRReview.py` & `patchwork_cli-0.0.9/patchwork/patchflows/PRReview/PRReview.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.87/patchwork/patchflows/PRReview/README.md` & `patchwork_cli-0.0.9/patchwork/patchflows/PRReview/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.87/patchwork/patchflows/PRReview/defaults.yml` & `patchwork_cli-0.0.9/patchwork/patchflows/PRReview/defaults.yml`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.87/patchwork/patchflows/PRReview/pr_review_prompt.json` & `patchwork_cli-0.0.9/patchwork/patchflows/PRReview/pr_review_prompt.json`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.87/patchwork/patchflows/README.md` & `patchwork_cli-0.0.9/patchwork/patchflows/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.87/patchwork/patchflows/ResolveIssue/README.md` & `patchwork_cli-0.0.9/patchwork/patchflows/ResolveIssue/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.87/patchwork/patchflows/ResolveIssue/ResolveIssue.py` & `patchwork_cli-0.0.9/patchwork/patchflows/ResolveIssue/ResolveIssue.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,17 @@
         # Save extracted data to JSON
         output_file = Path(tempfile.mktemp(".json"))
         with open(output_file, "w", encoding="utf-8") as f:
             json.dump(extracted_code_contexts, f, indent=2)
 
         self.inputs["code_file"] = output_file
         self.inputs["prompt_id"] = "resolve_issue"
-        self.inputs["response_partitions"] = {"patch": []}
+        self.inputs["response_partitions"] = {
+            "patch": ["Fixed Code:", "```", "\n", "```"],
+        }
         outputs = PreparePrompt(self.inputs).run()
         self.inputs.update(outputs)
         outputs = CallLLM(self.inputs).run()
         self.inputs.update(outputs)
         outputs = ExtractModelResponse(self.inputs).run()
         self.inputs.update(outputs)
```

### Comparing `patchwork_cli-0.0.87/patchwork/patchflows/ResolveIssue/defaults.yml` & `patchwork_cli-0.0.9/patchwork/patchflows/ResolveIssue/defaults.yml`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.87/patchwork/steps/AnalyzeImpact/AnalyzeImpact.py` & `patchwork_cli-0.0.9/patchwork/steps/AnalyzeImpact/AnalyzeImpact.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-import json
 import os
 from pathlib import Path
 
-from patchwork.common.utils import defered_temp_file
 from patchwork.logger import logger
 from patchwork.step import Step
 
 _PURL_TO_LANGUAGE_ = {
     "pypi": "python",
     "npm": "javascript",
     "maven": "java",
@@ -140,15 +138,9 @@
                 endLine=len(lines),
                 uri=impacted_file,
                 previousCode=file_content,
                 methodInfoList="\n".join(method_infos),
             )
             extracted_data.append(data)
 
-        # Save extracted data to JSON
-
-        with defered_temp_file("w", suffix=".json") as fp:
-            json.dump(extracted_data, fp)
-            output_file = Path(fp.name)
-
         logger.info(f"Run completed {self.__class__.__name__}")
-        return dict(prompt_value_file=output_file, code_file=output_file)
+        return dict(prompt_values=extracted_data, files_to_patch=extracted_data)
```

### Comparing `patchwork_cli-0.0.87/patchwork/steps/AnalyzeImpact/README.md` & `patchwork_cli-0.0.9/patchwork/steps/AnalyzeImpact/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.87/patchwork/steps/CallCode2Prompt/CallCode2Prompt.py` & `patchwork_cli-0.0.9/patchwork/steps/CallCode2Prompt/CallCode2Prompt.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,10 @@
-import json
 import os
 import subprocess
-from pathlib import Path
 
-from patchwork.common.utils import defered_temp_file
 from patchwork.logger import logger
 from patchwork.step import Step
 
 FOLDER_PATH = "folder_path"
 
 
 class CallCode2Prompt(Step):
@@ -65,13 +62,9 @@
 
         data["uri"] = self.code_file_path
         data["startLine"] = 0
         data["endLine"] = len(lines)
 
         self.extracted_data.append(data)
 
-        with defered_temp_file("w", suffix=".json") as fp:
-            json.dump(self.extracted_data, fp, indent=2)
-            output_file = Path(fp.name)
-
         logger.info(f"Run completed {self.__class__.__name__}")
-        return {"prompt_value_file": output_file, "code_file": output_file}
+        return dict(prompt_values=self.extracted_data, files_to_patch=self.extracted_data)
```

### Comparing `patchwork_cli-0.0.87/patchwork/steps/CallCode2Prompt/README.md` & `patchwork_cli-0.0.9/patchwork/steps/CallCode2Prompt/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.87/patchwork/steps/CallCode2Prompt/TestCallCode2Prompt.py` & `patchwork_cli-0.0.9/patchwork/steps/CallCode2Prompt/TestCallCode2Prompt.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.87/patchwork/steps/CallLLM/CallLLM.py` & `patchwork_cli-0.0.9/patchwork/steps/CallLLM/CallLLM.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import json
 import os
 from pathlib import Path
 from pprint import pformat
 from textwrap import indent
-from typing import Any, Protocol
 
 import requests
 from openai import OpenAI
+from typing_extensions import Any, Protocol
 
-from patchwork.common.utils import defered_temp_file
 from patchwork.logger import logger
 from patchwork.step import Step
 
 _TOKEN_URL = "https://app.patched.codes/signin"
 _DEFAULT_PATCH_URL = "https://patchwork.patched.codes/v1"
 
 
@@ -117,33 +116,34 @@
 
             contents.append(content)
 
         return contents
 
 
 class CallLLM(Step):
-    required_keys = {"prompt_file"}
-
     def __init__(self, inputs: dict):
         logger.info(f"Run started {self.__class__.__name__}")
 
         # Set 'openai_key' from inputs or environment if not already set
         inputs.setdefault("openai_api_key", os.environ.get("OPENAI_API_KEY"))
 
-        if not all(key in inputs.keys() for key in self.required_keys):
-            raise ValueError(f'Missing required data: "{self.required_keys}"')
-
-        self.prompt_file = Path(inputs["prompt_file"])
-        if not self.prompt_file.is_file():
-            raise ValueError(f'Unable to find Prompt file: "{self.prompt_file}"')
-        try:
-            with open(self.prompt_file, "r") as fp:
-                json.load(fp)
-        except json.JSONDecodeError as e:
-            raise ValueError(f'Invalid Json Prompt file "{self.prompt_file}": {e}')
+        prompt_file = inputs.get("prompt_file")
+        if prompt_file is not None:
+            prompt_file_path = Path(prompt_file)
+            if not prompt_file_path.is_file():
+                raise ValueError(f'Unable to find Prompt file: "{prompt_file}"')
+            try:
+                with open(prompt_file_path, "r") as fp:
+                    self.prompts = json.load(fp)
+            except json.JSONDecodeError as e:
+                raise ValueError(f'Invalid Json Prompt file "{prompt_file}": {e}')
+        elif "prompts" in inputs.keys():
+            self.prompts = inputs["prompts"]
+        else:
+            raise ValueError('Missing required data: "prompt_file" or "prompts"')
 
         self.model_args = {key[len("model_") :]: value for key, value in inputs.items() if key.startswith("model_")}
         self.client_args = {key[len("client_") :]: value for key, value in inputs.items() if key.startswith("client_")}
 
         llm_key = inputs.get("openai_api_key") or os.environ.get("OPENAI_API_KEY")
 
         patched_key = inputs.get("patched_api_key")
@@ -179,18 +179,11 @@
             "Please copy the access token that is generated, "
             "and add `--patched_api_key=<token>` to the command line.\n"
             "\n"
             "If you are using a OpenAI API Key, please set `--openai_api_key=<token>`.\n"
         )
 
     def run(self) -> dict:
-        with open(self.prompt_file, "r") as fp:
-            prompts = json.load(fp)
-
-        contents = self.llm.call(prompts)
-
-        with defered_temp_file("w", suffix=".json") as outfile:
-            json.dump(contents, outfile, indent=2)
-            response_file = Path(outfile.name)
+        contents = self.llm.call(self.prompts)
 
         logger.info(f"Run completed {self.__class__.__name__}")
-        return dict(new_code=response_file, openai_responses=contents)
+        return dict(new_code=contents, openai_responses=contents)
```

### Comparing `patchwork_cli-0.0.87/patchwork/steps/CommitChanges/CommitChanges.py` & `patchwork_cli-0.0.9/patchwork/steps/CommitChanges/CommitChanges.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import contextlib
 from pathlib import Path
-from typing import Generator
 
 import git
 from git import Head, Repo
+from typing_extensions import Generator
 
 from patchwork.logger import logger
 from patchwork.step import Step
 
 
 def get_slug_from_remote_url(remote_url: str) -> str:
     # TODO: consider using https://github.com/nephila/giturlparse instead
```

### Comparing `patchwork_cli-0.0.87/patchwork/steps/CommitChanges/README.md` & `patchwork_cli-0.0.9/patchwork/steps/CommitChanges/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.87/patchwork/steps/CreateIssueComment/CreateIssueComment.py` & `patchwork_cli-0.0.9/patchwork/steps/CreateIssueComment/CreateIssueComment.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.87/patchwork/steps/CreateIssueComment/README.md` & `patchwork_cli-0.0.9/patchwork/steps/CreateIssueComment/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.87/patchwork/steps/CreatePR/CreatePR.py` & `patchwork_cli-0.0.9/patchwork/steps/CreatePR/CreatePR.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.87/patchwork/steps/CreatePR/README.md` & `patchwork_cli-0.0.9/patchwork/steps/CreatePR/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.87/patchwork/steps/CreatePRComment/CreatePRComment.py` & `patchwork_cli-0.0.9/patchwork/steps/CreatePRComment/CreatePRComment.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.87/patchwork/steps/CreatePRComment/README.md` & `patchwork_cli-0.0.9/patchwork/steps/CreatePRComment/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.87/patchwork/steps/ExtractCode/ExtractCode.py` & `patchwork_cli-0.0.9/patchwork/steps/ExtractCode/ExtractCode.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,17 @@
-import json
 import os
 import sys
 from collections import defaultdict
 from enum import IntEnum
 from pathlib import Path
-from typing import Any
 from urllib.parse import urlparse
 
-from patchwork.common.utils import (
-    count_openai_tokens,
-    defered_temp_file,
-    open_with_chardet,
-)
+from typing_extensions import Any
+
+from patchwork.common.utils import count_openai_tokens, open_with_chardet
 from patchwork.logger import logger
 from patchwork.step import Step
 from patchwork.steps.ExtractCode.context_strategy.context_strategies import (
     ContextStrategies,
 )
 
 
@@ -250,61 +246,48 @@
                 if 0 < vulnerability_limit <= vulnerability_count:
                     return grouped_messages
 
     return grouped_messages
 
 
 class ExtractCode(Step):
-    required_keys = {"sarif_file_path"}
+    required_keys = {"sarif_values"}
 
     def __init__(self, inputs: dict):
         logger.info(f"Run started {self.__class__.__name__}")
 
         if not all(key in inputs.keys() for key in self.required_keys):
             raise ValueError(f'Missing required data: "{self.required_keys}"')
 
-        # Validate and set the SARIF file path
-        self.sarif_file_path = Path(inputs["sarif_file_path"])
-        if not self.sarif_file_path.exists() or not self.sarif_file_path.is_file():
-            raise ValueError(f'SARIF file path does not exist or is not a file: "{self.sarif_file_path}"')
-
+        self.sarif_data = inputs["sarif_values"]
         # Check and set number of lines to extract
         self.context_length = inputs.get("context_size", 1000)
         self.vulnerability_limit = inputs.get("vulnerability_limit", 10)
         self.severity_threshold = Severity.from_str(inputs.get("severity", "UNKNOWN"))
 
         # Prepare for data extraction
         self.extracted_code_contexts = []
 
     def run(self) -> dict:
-        # Load SARIF data
-        with open_with_chardet(self.sarif_file_path, "r") as file:
-            sarif_data = json.load(file)
-
         base_path = Path.cwd()
 
         grouped_messages = transform_sarif_results(
-            sarif_data, base_path, self.context_length, self.vulnerability_limit, self.severity_threshold
+            self.sarif_data, base_path, self.context_length, self.vulnerability_limit, self.severity_threshold
         )
 
         self.extracted_code_contexts = [
             {
                 "uri": str(file_path),
                 "startLine": start,
                 "endLine": end,
                 "affectedCode": context,
                 "messageText": "\n".join(msgs),
             }
             for (file_path, start, end, context), msgs in grouped_messages.items()
         ]
 
-        # Save extracted data to JSON
-        with defered_temp_file("w", suffix=".json") as fp:
-            json.dump(self.extracted_code_contexts, fp, indent=2)
-            output_file = Path(fp.name)
-
         logger.info(f"Run completed {self.__class__.__name__}")
 
         return dict(
-            code_file=output_file,
+            files_to_patch=self.extracted_code_contexts,
             prompt_values=self.extracted_code_contexts,
         )
```

### Comparing `patchwork_cli-0.0.87/patchwork/steps/ExtractCode/README.md` & `patchwork_cli-0.0.9/patchwork/steps/ExtractCode/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.87/patchwork/steps/ExtractCode/context_strategy/context_strategies.py` & `patchwork_cli-0.0.9/patchwork/steps/ExtractCode/context_strategy/context_strategies.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.87/patchwork/steps/ExtractCode/context_strategy/generic.py` & `patchwork_cli-0.0.9/patchwork/steps/ExtractCode/context_strategy/generic.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Tuple
+from typing_extensions import Tuple
 
 from .protocol import ContextStrategyProtocol
 
 
 class FullFileStrategy(ContextStrategyProtocol):
     def get_context_indexes(self, src: list[str], start: int, end: int) -> Tuple[int, int]:
         return 0, len(src)
```

### Comparing `patchwork_cli-0.0.87/patchwork/steps/ExtractCode/context_strategy/java.py` & `patchwork_cli-0.0.9/patchwork/steps/ExtractCode/context_strategy/java.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-from typing import Tuple
-
 from tree_sitter_languages import get_language, get_parser
+from typing_extensions import Tuple
 
 from .protocol import ContextStrategyProtocol
 
 
 class JavaStrategy(ContextStrategyProtocol):
     def __init__(self, query: str):
         self.query = query
```

### Comparing `patchwork_cli-0.0.87/patchwork/steps/ExtractCode/context_strategy/javascript.py` & `patchwork_cli-0.0.9/patchwork/steps/ExtractCode/context_strategy/javascript.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-from typing import Tuple
-
 from tree_sitter_languages import get_language, get_parser
+from typing_extensions import Tuple
 
 from .protocol import ContextStrategyProtocol
 
 
 class JavascriptContextStrategy(ContextStrategyProtocol):
     def __init__(self, language: str, query: str, exts: list[str]):
         self.language = language
```

### Comparing `patchwork_cli-0.0.87/patchwork/steps/ExtractCode/context_strategy/python.py` & `patchwork_cli-0.0.9/patchwork/steps/ExtractCode/context_strategy/python.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from typing import Callable, Optional, Tuple
-
 import libcst
 from libcst import FunctionDef, IndentedBlock
+from typing_extensions import Callable, Optional, Tuple
 
 from .protocol import ContextStrategyProtocol
 
 
 class _PythonCollector(libcst.CSTVisitor):
     METADATA_DEPENDENCIES = (libcst.metadata.WhitespaceInclusivePositionProvider,)
```

### Comparing `patchwork_cli-0.0.87/patchwork/steps/ExtractDiff/ExtractDiff.py` & `patchwork_cli-0.0.9/patchwork/steps/ExtractDiff/ExtractDiff.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-import json
 import re
 import string
 from pathlib import Path
-from typing import Dict, List
 
 import requests
 from packageurl import PackageURL
+from typing_extensions import Dict, List
 
 from patchwork.common.utils import defered_temp_file
 from patchwork.logger import logger
 from patchwork.step import Step
 
 _PURL_TO_LANGUAGE_ = {
     "pypi": "python",
@@ -220,14 +219,9 @@
 
         diff_sections = get_diff_sections(temp_file_path, _PURL_TO_LANGUAGE_.get(platform_type))
         extracted_data = []
 
         for diff_section in diff_sections:
             extracted_data.append({"diffSection": diff_section})
 
-        # Save extracted data to JSON
-        with defered_temp_file("w", suffix=".json") as fp:
-            json.dump(extracted_data, fp, indent=2)
-            output_file = Path(fp.name)
-
         logger.info(f"Run completed {self.__class__.__name__}")
-        return dict(prompt_value_file=output_file, library_name=name, platform_type=platform_type)
+        return dict(prompt_values=extracted_data, library_name=name, platform_type=platform_type)
```

### Comparing `patchwork_cli-0.0.87/patchwork/steps/ExtractDiff/README.md` & `patchwork_cli-0.0.9/patchwork/steps/ExtractDiff/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.87/patchwork/steps/ExtractModelResponse/ExtractModelResponse.py` & `patchwork_cli-0.0.9/patchwork/steps/ExtractModelResponse/ExtractModelResponse.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.87/patchwork/steps/ExtractModelResponse/README.md` & `patchwork_cli-0.0.9/patchwork/steps/ExtractModelResponse/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.87/patchwork/steps/ExtractPackageManagerFile/ExtractPackageManagerFile.py` & `patchwork_cli-0.0.9/patchwork/steps/ExtractPackageManagerFile/ExtractPackageManagerFile.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import re
 from collections import defaultdict
 from pathlib import Path
 
 import semver
 from packageurl import PackageURL
 
-from patchwork.common.utils import defered_temp_file
 from patchwork.logger import logger
 from patchwork.step import Step
 
 # Define a mapping from CVSS severity level strings to numbers
 SEVERITY_LEVELS = {"none": 0, "low": 1, "medium": 2, "high": 3, "critical": 4}
 
 
@@ -78,15 +77,15 @@
     except FileNotFoundError:
         print(f"The directory {directory} was not found.")
 
     return found_files
 
 
 class ExtractPackageManagerFile(Step):
-    required_keys = {"sbom_vdr_file_path"}
+    required_keys = {}
 
     def __init__(self, inputs: dict):
         """
         Initializes an instance of the class, setting up necessary validations and preparations
         for data extraction based on the provided input parameters.
 
         This method performs the following actions:
@@ -109,17 +108,25 @@
         """
         logger.info(f"Run started {self.__class__.__name__}")
 
         if not all(key in inputs.keys() for key in self.required_keys):
             raise ValueError(f'Missing required data: "{self.required_keys}"')
 
         # Validate and set the SBOM VDR file path
-        self.sbom_vdr_file_path = Path(inputs["sbom_vdr_file_path"])
-        if not self.sbom_vdr_file_path.exists() or not self.sbom_vdr_file_path.is_file():
-            raise ValueError(f'SBOM VDR file path does not exist or is not a file: "{self.sbom_vdr_file_path}"')
+        sbom_vdr_file_path = inputs.get("sbom_vdr_file_path")
+        if sbom_vdr_file_path is not None:
+            sbom_vdr_file_path = Path(sbom_vdr_file_path)
+            if not sbom_vdr_file_path.is_file():
+                raise ValueError(f'SBOM VDR file path does not exist or is not a file: "{sbom_vdr_file_path}"')
+            with open(sbom_vdr_file_path, "r") as file:
+                self.sbom_vdr_values = json.load(file)
+        if "sbom_vdr_values" in inputs.keys():
+            self.sbom_vdr_values = inputs["sbom_vdr_values"]
+        else:
+            raise ValueError('"sbom_vdr_file_path" or "sbom_vdr_values" not found in inputs')
 
         self.package_manager_file = inputs.get("package_manager_file", None)
 
         self.upgrade_threshold = inputs.get("upgrade_threshold", "major")
 
         self.severity_threshold_level = SEVERITY_LEVELS.get(inputs.get("severity", "none").lower())
 
@@ -151,19 +158,15 @@
             FileNotFoundError: If any specified source file in the SBOM VDR data cannot be found.
 
         Note:
             This method assumes that the SBOM VDR file is correctly formatted and accessible. It also
             assumes that the source files referenced within the SBOM VDR data are accessible for reading.
             The method logs detailed information about its execution status, including any file access issues.
         """
-        # Load SARIF data
-        with self.sbom_vdr_file_path.open("r", encoding="utf-8") as file:
-            sbom_vdr_data = json.load(file)
-
-        components = sbom_vdr_data.get("components", [])
+        components = self.sbom_vdr_values.get("components", [])
         # Initialize a dictionary to hold the mapping of purls to SrcFiles
         purl_to_srcfile = {}
 
         # Iterate over each component in the components list from SBOM VDR data
         for component in components:
             purl = component.get("purl", "")
             if self.package_manager_file is not None:
@@ -188,15 +191,15 @@
                 purl_to_srcfile[purl] = src_file
 
         # Initialize a dictionary to hold the final structure
         result = {}
 
         # Process each vulnerabiility in SBOM VDR data
         purl_list = []
-        for vul in sbom_vdr_data.get("vulnerabilities", []):
+        for vul in self.sbom_vdr_values.get("vulnerabilities", []):
             for rating in vul.get("ratings", []):
                 severity = rating.get("severity", "")
 
             if SEVERITY_LEVELS.get(severity.lower()) < self.severity_threshold_level:
                 continue
 
             for affect in vul.get("affects", []):
@@ -268,14 +271,9 @@
             data["PackageManagerFile"] = file_content
             data["UpdateMsg"] = update_msg
             data["uri"] = src_file
             data["startLine"] = 0
             data["endLine"] = len(lines)
             self.extracted_data.append(data)
 
-        # Save extracted data to JSON
-        with defered_temp_file("w", suffix=".json") as fp:
-            json.dump(self.extracted_data, fp, indent=2)
-            output_file = Path(fp.name)
-
         logger.info(f"Run completed {self.__class__.__name__}")
-        return dict(prompt_value_file=output_file, code_file=output_file)
+        return dict(prompt_values=self.extracted_data, files_to_patch=self.extracted_data)
```

### Comparing `patchwork_cli-0.0.87/patchwork/steps/ExtractPackageManagerFile/README.md` & `patchwork_cli-0.0.9/patchwork/steps/ExtractPackageManagerFile/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.87/patchwork/steps/ExtractPackageManagerFile/TestExtractPackageManagerFile.py` & `patchwork_cli-0.0.9/patchwork/steps/ExtractPackageManagerFile/TestExtractPackageManagerFile.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.87/patchwork/steps/GenerateCodeRepositoryEmbeddings/GenerateCodeRepositoryEmbeddings.py` & `patchwork_cli-0.0.9/patchwork/steps/GenerateCodeRepositoryEmbeddings/GenerateCodeRepositoryEmbeddings.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import hashlib
 import time
 from itertools import islice
 from pathlib import Path
-from typing import Iterable
 
 import chromadb
 import git
+from typing_extensions import Iterable
 
 from patchwork.common.utils import get_vector_db_path, open_with_chardet
 from patchwork.logger import logger
 from patchwork.step import Step
 from patchwork.steps.GenerateEmbeddings.GenerateEmbeddings import GenerateEmbeddings
 
 _EXTENSION_WHITELIST = [
@@ -38,14 +38,74 @@
     ".php3",
     ".php4",
     ".php5",
     # Go
     ".go",
     # HTML
     ".html",
+    # OCaml
+    ".ml",
+    ".mli",
+    # F#
+    ".fs",
+    ".fsi",
+    # Haskell
+    ".hs",
+    ".lhs",
+    # Kotlin
+    ".kt",
+    ".kts",
+    # Ruby
+    ".rb",
+    # Swift
+    ".swift",
+    # Rust
+    ".rs",
+    # Scala
+    ".scala",
+    # TypeScript
+    ".ts",
+    # Visual Basic.NET
+    ".vb",
+    ".vbs",
+    # Perl
+    ".pl",
+    ".pm",
+    # R
+    ".r",
+    # SQL
+    ".sql",
+    # TypeScript React
+    ".tsx",
+    # Julia
+    ".jl",
+    # Lua
+    ".lua",
+    # MATLAB
+    ".m",
+    # Pascal
+    ".pas",
+    # PowerShell
+    ".ps1",
+    # Racket
+    ".rkt",
+    # Shell
+    ".sh",
+    # SQL
+    ".sql",
+    # Tcl
+    ".tcl",
+    # Visual Basic
+    ".vb",
+    # XML
+    ".xml",
+    # YAML
+    ".yaml",
+    # Zig
+    ".zig",
 ]
 
 _DIRECTORY_BLACKLIST = [
     "test",
     "tests",
     "___init__.py",
     "___main__.py",
@@ -81,15 +141,15 @@
     def __init__(self, inputs: dict):
         logger.info(f"Run started {self.__class__.__name__}")
 
         if not all(key in inputs.keys() for key in self.required_keys):
             raise ValueError(f'Missing required data: "{self.required_keys}"')
 
         self.client = chromadb.PersistentClient(path=get_vector_db_path())
-
+        self.disable_cache = inputs.get("disable_cache", False)
         self.inputs = inputs
 
     def run(self) -> dict:
         cwd = Path.cwd()
         base_embedding_name = cwd.name
         embedding_name = base_embedding_name
 
@@ -143,15 +203,15 @@
                     id=file,
                     document=text,
                     hash=text_hash,
                     created_at=int(time.time()),
                     path=file,
                 )
             ]
-            if reference_collection is not None:
+            if reference_collection is not None and not self.disable_cache:
                 result = reference_collection.get(
                     where={"$and": [{"hash": text_hash}, {"path": file}]}, include=["metadatas", "embeddings"]
                 )
                 if len(result["ids"]) > 0:
                     documents_to_add = []
                     for embedding_id, embedding, metadata in zip(
                         result["ids"], result["embeddings"], result["metadatas"]
```

### Comparing `patchwork_cli-0.0.87/patchwork/steps/GenerateCodeRepositoryEmbeddings/README.md` & `patchwork_cli-0.0.9/patchwork/steps/GenerateCodeRepositoryEmbeddings/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.87/patchwork/steps/GenerateEmbeddings/GenerateEmbeddings.py` & `patchwork_cli-0.0.9/patchwork/steps/GenerateEmbeddings/GenerateEmbeddings.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import uuid
-from typing import Any
 
 import chromadb
+from typing_extensions import Any
 
 from patchwork.common.utils import get_embedding_function, get_vector_db_path
 from patchwork.logger import logger
 from patchwork.step import Step
 
 
 def filter_by_extension(file, extensions):
@@ -21,46 +21,59 @@
             continue
 
         chunks.append(chunk)
 
     return chunks
 
 
+def delete_collection(client, collection_name):
+    for collection in client.list_collections():
+        if collection.name == collection_name:
+            client.delete_collection(collection_name)
+            break
+
+
 class GenerateEmbeddings(Step):
     required_keys = {"embedding_name", "documents"}
 
     def __init__(self, inputs: dict):
         logger.info(f"Run started {self.__class__.__name__}")
 
         if not all(key in inputs.keys() for key in self.required_keys):
             raise ValueError(f'Missing required data: "{self.required_keys}"')
 
         client = chromadb.PersistentClient(path=get_vector_db_path())
 
+        if inputs.get("disable_cache", False):
+            delete_collection(client, inputs["embedding_name"])
+
         embedding_function = get_embedding_function(inputs)
         self.collection = client.get_or_create_collection(
             inputs["embedding_name"], embedding_function=embedding_function, metadata={"hnsw:space": "cosine"}
         )
         self.documents: list[dict[str, Any]] = inputs["documents"]
 
+        self.chunk_size = inputs.get("chunk_size", 4000)
+        self.overlap_size = inputs.get("overlap_size", 2000)
+
     def run(self) -> dict:
         document_ids = []
         documents = []
         document_metadatas = []
 
         embedding_ids = []
         embeddings = []
         embedding_metadatas = []
         for document in self.documents:
             document_text = document.get("document")
             embedding = document.get("embedding")
 
             if document_text is not None:
                 doc_id = str(document.get("id"))
-                document_texts = split_text(document_text, 4000, 2000)
+                document_texts = split_text(document_text, self.chunk_size, self.overlap_size)
                 for i, document_text in enumerate(document_texts):
                     document_ids.append(str(uuid.uuid4()))
                     documents.append(document_text)
 
                     metadata = {key: value for key, value in document.items() if key not in ["id", "document"]}
                     metadata["original_document"] = document_text
                     metadata["original_id"] = doc_id
```

### Comparing `patchwork_cli-0.0.87/patchwork/steps/GenerateEmbeddings/README.md` & `patchwork_cli-0.0.9/patchwork/steps/GenerateEmbeddings/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.87/patchwork/steps/ModifyCode/ModifyCode.py` & `patchwork_cli-0.0.9/patchwork/steps/ModifyCode/ModifyCode.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 import json
 from pathlib import Path
 
 from patchwork.logger import logger
 from patchwork.step import Step
 
-CODE_SNIPPETS_KEY = "code_file"
-UPDATED_SNIPPETS_KEY = "extracted_responses"
-
 
 def load_json_file(file_path):
     """Utility function to load a json file."""
     file_path = Path(file_path)
 
     if not file_path.is_file():
         raise ValueError(f'Unable to find input file: "{file_path}"')
@@ -55,31 +52,31 @@
     lines[start_line:end_line] = handle_indent(lines[start_line:end_line], new_code.splitlines(keepends=True))
 
     # Save the modified contents back to the file
     save_file_contents(file_path, "".join(lines))
 
 
 class ModifyCode(Step):
-    required_keys = {CODE_SNIPPETS_KEY, UPDATED_SNIPPETS_KEY}
+    UPDATED_SNIPPETS_KEY = "extracted_responses"
+    FILES_TO_PATCH = "files_to_patch"
+    required_keys = {FILES_TO_PATCH, UPDATED_SNIPPETS_KEY}
 
     def __init__(self, inputs: dict):
         logger.info(f"Run started {self.__class__.__name__}")
 
         if not all(key in inputs.keys() for key in self.required_keys):
             raise ValueError(f'Missing required data: "{self.required_keys}"')
 
-        self.code_snippets_path = inputs[CODE_SNIPPETS_KEY]
-        self.extracted_responses = inputs[UPDATED_SNIPPETS_KEY]
+        self.files_to_patch = inputs[self.FILES_TO_PATCH]
+        self.extracted_responses = inputs[self.UPDATED_SNIPPETS_KEY]
 
     def run(self) -> dict:
-        code_snippets = load_json_file(self.code_snippets_path)
-
         modified_code_files = []
         sorted_list = sorted(
-            zip(code_snippets, self.extracted_responses), key=lambda x: x[0]["startLine"], reverse=True
+            zip(self.files_to_patch, self.extracted_responses), key=lambda x: x[0]["startLine"], reverse=True
         )
         for code_snippet, extracted_response in sorted_list:
             uri = code_snippet["uri"]
             start_line = code_snippet["startLine"]
             end_line = code_snippet["endLine"]
             new_code = extracted_response.get("patch")
             if new_code is None:
```

### Comparing `patchwork_cli-0.0.87/patchwork/steps/ModifyCode/README.md` & `patchwork_cli-0.0.9/patchwork/steps/ModifyCode/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.87/patchwork/steps/PreparePR/PreparePR.py` & `patchwork_cli-0.0.9/patchwork/steps/PreparePR/PreparePR.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.87/patchwork/steps/PreparePR/README.md` & `patchwork_cli-0.0.9/patchwork/steps/PreparePR/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.87/patchwork/steps/PreparePrompt/PreparePrompt.py` & `patchwork_cli-0.0.9/patchwork/steps/PreparePrompt/PreparePrompt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import json
 from pathlib import Path
 
-from patchwork.common.utils import defered_temp_file
 from patchwork.logger import logger
 from patchwork.step import Step
 
 PROMPT_TEMPLATE_FILE_KEY = "prompt_template_file"
 
 
 class PreparePrompt(Step):
@@ -63,13 +62,9 @@
                     new_value = value
                     for replacement_key, replacement_value in prompt_value.items():
                         new_value = new_value.replace("{{" + replacement_key + "}}", str(replacement_value))
                     prompt_instance[key] = new_value
                 prompt.append(prompt_instance)
             prompts.append(prompt)
 
-        with defered_temp_file("w", suffix=".json") as fp:
-            json.dump(prompts, fp, indent=2)
-            prompt_file = Path(fp.name)
-
         logger.info(f"Run completed {self.__class__.__name__}")
-        return {"prompt_file": prompt_file}
+        return dict(prompts=prompts)
```

### Comparing `patchwork_cli-0.0.87/patchwork/steps/PreparePrompt/README.md` & `patchwork_cli-0.0.9/patchwork/steps/PreparePrompt/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.87/patchwork/steps/QueryEmbeddings/QueryEmbeddings.py` & `patchwork_cli-0.0.9/patchwork/steps/QueryEmbeddings/QueryEmbeddings.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.87/patchwork/steps/QueryEmbeddings/README.md` & `patchwork_cli-0.0.9/patchwork/steps/QueryEmbeddings/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.87/patchwork/steps/README.md` & `patchwork_cli-0.0.9/patchwork/steps/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.87/patchwork/steps/ReadIssues/README.md` & `patchwork_cli-0.0.9/patchwork/steps/ReadIssues/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.87/patchwork/steps/ReadIssues/ReadIssues.py` & `patchwork_cli-0.0.9/patchwork/steps/ReadIssues/ReadIssues.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.87/patchwork/steps/ReadPRDiffs/README.md` & `patchwork_cli-0.0.9/patchwork/steps/ReadPRDiffs/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.87/patchwork/steps/ReadPRDiffs/ReadPRDiffs.py` & `patchwork_cli-0.0.9/patchwork/steps/ReadPRDiffs/ReadPRDiffs.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,8 @@
-import json
-from pathlib import Path
-
 from patchwork.common.client.scm import GithubClient, GitlabClient
-from patchwork.common.utils import defered_temp_file
 from patchwork.logger import logger
 from patchwork.step import Step
 
 _IGNORED_EXTENSIONS = [
     ".png",
     ".jpg",
     ".jpeg",
@@ -51,12 +47,8 @@
     def run(self) -> dict:
         prompt_values = []
         for path, diffs in self.pr.file_diffs().items():
             if filter_by_extension(path, _IGNORED_EXTENSIONS):
                 continue
             prompt_values.append(dict(path=path, diff=diffs))
 
-        with defered_temp_file("w", suffix=".json") as fp:
-            json.dump(prompt_values, fp)
-            prompt_value_file = Path(fp.name)
-
-        return dict(prompt_value_file=prompt_value_file, prompt_values=prompt_values)
+        return dict(prompt_values=prompt_values)
```

### Comparing `patchwork_cli-0.0.87/patchwork/steps/ScanDepscan/README.md` & `patchwork_cli-0.0.9/patchwork/steps/ScanDepscan/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.87/patchwork/steps/ScanDepscan/ScanDepscan.py` & `patchwork_cli-0.0.9/patchwork/steps/ScanDepscan/ScanDepscan.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import atexit
-import os
+import json
 import shutil
 import subprocess
 import tempfile
 from pathlib import Path
 
 from patchwork.logger import logger
 from patchwork.step import Step
@@ -102,11 +102,20 @@
             cmd.append(self.language)
             sbom_vdr_file_name = "sbom-" + self.language
         else:
             sbom_vdr_file_name = "sbom-universal"
 
         p = subprocess.run(cmd, capture_output=True, text=True)
 
-        sbom_vdr_file_path = os.path.join(temp_file_path, sbom_vdr_file_name + ".vdr.json")
+        sbom_vdr_file_path = temp_file_path / f"{sbom_vdr_file_name}.vdr.json"
+        try:
+            with open(sbom_vdr_file_path, "r") as f:
+                sbom_values = json.load(f)
+        except json.JSONDecodeError as e:
+            logger.debug(e)
+            raise ValueError(f"Error reading SBOM VDR file from Depscan")
+        except FileNotFoundError as e:
+            logger.debug(e)
+            raise ValueError(f"SBOM VDR file not found from Depscan")
 
         logger.info(f"Run completed {self.__class__.__name__}")
-        return {"sbom_vdr_file_path": sbom_vdr_file_path}
+        return {"sbom_vdr_values": sbom_values}
```

### Comparing `patchwork_cli-0.0.87/patchwork/steps/ScanSemgrep/README.md` & `patchwork_cli-0.0.9/patchwork/steps/ScanSemgrep/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.87/patchwork/steps/__init__.py` & `patchwork_cli-0.0.9/patchwork/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.87/pyproject.toml` & `patchwork_cli-0.0.9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 [tool.poetry]
 name = "patchwork-cli"
-version = "0.0.87"
+version = "0.0.9"
 description = ""
 authors = ["patched.codes"]
 license = "AGPL"
 readme = "README.md"
 packages = [
     { include = "patchwork", from = "." }
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.8",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Software Development :: Quality Assurance",
     "Topic :: Software Development :: Testing",
     "Topic :: Utilities"
 ]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.8"
+typing-extensions = "^4.11.0"
 click = "~8.1.0"
 semgrep = "^1.51.0"
 openai = "^1.13.3"
 tree-sitter-languages = "^1.10.2"
 python-gitlab = "^4.4.0"
 owasp-depscan = "~5.2.12"
 pygithub = "~2.1.1"
 gitpython = "~3.1.40"
 pydantic = "~2.6.4"
 tiktoken = "~0.6.0"
-libcst = "~1.2.0"
+libcst = "~1.1.0"
 patched-code2prompt = "0.2.0"
 pyyaml = "^6.0.1"
 packageurl-python = "~0.15.0"
 semver = "~3.0.2"
 requests = "~2.31.0"
 chardet = "^5.2.0"
 chromadb = "~0.4.24"
```

### Comparing `patchwork_cli-0.0.87/PKG-INFO` & `patchwork_cli-0.0.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 Metadata-Version: 2.1
 Name: patchwork-cli
-Version: 0.0.87
+Version: 0.0.9
 Summary: 
 License: AGPL
 Author: patched.codes
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Utilities
 Requires-Dist: chardet (>=5.2.0,<6.0.0)
 Requires-Dist: chromadb (>=0.4.24,<0.5.0)
 Requires-Dist: click (>=8.1.0,<8.2.0)
 Requires-Dist: gitpython (>=3.1.40,<3.2.0)
-Requires-Dist: libcst (>=1.2.0,<1.3.0)
+Requires-Dist: libcst (>=1.1.0,<1.2.0)
 Requires-Dist: openai (>=1.13.3,<2.0.0)
 Requires-Dist: orjson (>=3.9.15,<3.10.0)
 Requires-Dist: owasp-depscan (>=5.2.12,<5.3.0)
 Requires-Dist: packageurl-python (>=0.15.0,<0.16.0)
 Requires-Dist: patched-code2prompt (==0.2.0)
 Requires-Dist: pydantic (>=2.6.4,<2.7.0)
 Requires-Dist: pygithub (>=2.1.1,<2.2.0)
@@ -36,115 +38,114 @@
 Requires-Dist: requests (>=2.31.0,<2.32.0)
 Requires-Dist: semgrep (>=1.51.0,<2.0.0)
 Requires-Dist: semver (>=3.0.2,<3.1.0)
 Requires-Dist: sentence-transformers (>=2.7.0,<2.8.0)
 Requires-Dist: tiktoken (>=0.6.0,<0.7.0)
 Requires-Dist: torch (>=2.2.2,<2.3.0)
 Requires-Dist: tree-sitter-languages (>=1.10.2,<2.0.0)
+Requires-Dist: typing-extensions (>=4.11.0,<5.0.0)
 Description-Content-Type: text/markdown
 
-<p align="center">
-  <img src="https://github.com/patched-codes/patchwork/assets/126385808/a7adcf24-b615-43a0-a244-45789d184f0a" width="160" alt="PatchWork Logo">
-</p>
+<div align="center">
+  <picture>
+    <img alt="Patchwork logo" src="https://repository-images.githubusercontent.com/782544882/a9743f35-5e1c-43ed-a0e0-536322056d38" width="36%">
+  </picture>
+</div>
+
+<br>
+
+<div align="center">
+
+![Build](https://github.com/patched-codes/patchwork/actions/workflows/release.yml/badge.svg)
+![Tests](https://github.com/patched-codes/patchwork/actions/workflows/test.yml/badge.svg)
+[![Downloads](https://static.pepy.tech/badge/patchwork-cli)](https://pepy.tech/project/patchwork-cli)
+[![Discord](https://img.shields.io/discord/1236886480471855104?style=flat&logo=discord&logoColor=white&label=discord)](https://discord.gg/XDxA3mJyhE)
+
+[Demo](https://youtu.be/3gRpqQoIino) |
+[Docs](https://docs.patched.codes/)
+
+</div>
+
 
 # PatchWork
 
 An open-source framework for automating development chores using large language models. PatchWork allows you to automate workflows like PR reviews, bug fixing, security patching, and more using a self-hosted CLI agent and your preferred LLMs.
 
 ## Key Components
 
-- **Steps**: A set of reusable atomic actions that define various operations.
-- **Patchflows**: LLM-assisted automations such as PR reviews, code fixing, debugging.
+- **Steps**: Reusable atomic actions like Create PR, commit changes, call an LLM etc
+- **Prompt Templates**: Customizable LLM prompts optimized for a chore like library updates, code generation, issue analysis etc.
+- **Patchflows**: LLM-assisted automations such as PR reviews, code fixing, documentation etc. built by combining steps and prompts.
+
+Patchflows can be run locally in your CLI and IDE, or as part of your CI/CD pipeline. There are [5 patchflows available](#patchflows) out of the box, and you can always [create your own](#contributing).
+
+## Quickstart
 
-Patchflows can be run locally in your CLI and IDE, or as part of your CI/CD pipeline.
+[![Patchwork CLI Quickstart](https://img.youtube.com/vi/3gRpqQoIino/0.jpg)](https://youtu.be/3gRpqQoIino)
 
 ## Installation
 
 ### Using Pip
 
 PatchWork is available on PyPI and can be installed using pip:
 
 ```bash
 pip install patchwork-cli --upgrade
 ```
 
 ### Using Poetry
 
-PatchWork is built using Poetry, a dependency management and packaging tool for Python. To install PatchWork using Poetry, follow these steps:
-
-1. Make sure you have Poetry installed. If you don't have it installed, you can install it by running:
-   ```
-   curl -sSL https://install.python-poetry.org | python3 -
-   ```
-
-2. Clone the PatchWork repository:
-   ```
-   git clone https://github.com/patched-codes/patchwork.git
-   ```
-
-3. Navigate to the project directory:
-   ```
-   cd patchwork
-   ```
-
-4. Activate a shell using virtual environment:
-   ```
-   poetry shell
-   ```
-
-5. Install the dependencies using Poetry:
-   ```
-   poetry install
-   ```
+If you'd like to build from source using poetry, please see detailed documentation [here](INSTALL.md) .
 
 ## PatchWork CLI
 
 The CLI runs Patchflows, as follows:
 
 ```
-patchwork <Patchflow> <?Arguments>
+patchwork <PatchFlow> <?Arguments>
 ```
 
 Where
 - **Arguments**: Allow for overriding default/optional attributes of the Patchflow in the format of `key=value`. If `key` does not have any value, it is considered a boolean `True` flag.
 
 ### Example
 
 For an AutoFix patchflow which patches vulnerabilities based on a scan using Semgrep:
 
 ```bash
 patchwork AutoFix openai_api_key=<YOUR_OPENAI_API_KEY> github_api_key=<YOUR_GITHUB_TOKEN>
 ```
 
-The above command will default to patching code in the current directory, by running Semgrep to identify the vulnerabilities.
+The above command will default to patching code in the current directory, by running Semgrep to identify the vulnerabilities. You can take a look at the `default.yml` [file](patchwork/patchflows/AutoFix/defaults.yml) for the list of configurations you can set to manage the AutoFix patchflow. 
 
-You can take a look at the `default.yml` [file](patchwork/patchflows/AutoFix/defaults.yml) for the list of configurations you can set to manage the AutoFix patchflow. You will need to pass your own `openai_api_key` to call the LLM. Otherwise, to get started, you can get a `patched_api_key` for free by
+You can replace the OpenAI key with a key from our managed service
 by signing in at [https://app.patched.codes/signin](https://app.patched.codes/signin) and generating an API key from the integrations tab. You can then call the patchflow with the key as follows:
 
 ```bash
 patchwork AutoFix patched_api_key=<YOUR_PATCHED_API_KEY> github_api_key=<YOUR_GITHUB_TOKEN>
 ```
 
-Similarly, to use Google's models you can set the `google_api_key` and `model`, this is useful if you want to work with large contexts as the `gemini-pro-1.5` model supports a input context length of 1 million tokens.
 
-The [patchwork-configs](https://github.com/patched-codes/patchwork-configs) repository contains the default configuration and prompts for all the patchflows. You can clone that repo and pass it as a flag to the CLI:
+Similarly, to use Google's models you can set the `google_api_key` and `model`, this is useful if you want to work with large contexts as the `gemini-pro-1.5` model supports an input context length of 1 million tokens.
+
+The [patchwork-template](https://github.com/patched-codes/patchwork-configs) repository contains the default configuration and prompts for all the patchflows. You can clone that repo and pass it as a flag to the CLI:
 
 ```bash
 patchwork AutoFix --config /path/to/patchwork-configs/patchflows
 ```
 
 ## Patchflows
 
 Patchwork comes with a set of predefined patchflows, and more will be added over time. Below is a sample list of patchflows:
 
 - **AutoFix**: Generate and apply fixes to code vulnerabilities in a repository.
-- **DependencyUpgrade**: Update your dependencies from vulnerable to fixed versions.
 - **PRReview**: On PR creation, extract code diff, summarize changes, and comment on PR.
-- **GenerateREADME**: Create a README.md file for a given folder, to add documentation to your repository.
-- **ResolveIssue**: Identify the files in your repository that need to be updated to resolve an issue (or bug) and create a PR to fix it.
+- **GenerateREADME**: Create a README markdown file for a given folder, to add documentation to your repository.
+- **[Experimental] DependencyUpgrade**: Update your dependencies from vulnerable to fixed versions.
+- **[Experimental] ResolveIssue**: Identify the files in your repository that need to be updated to resolve an issue (or bug) and create a PR to fix it.
 
 ## Prompt Templates
 
 Prompt templates are used by patchflows and passed as queries to LLMs. Templates contain prompts with placeholder variables enclosed by {{}} which are replaced by the data from the steps or inputs on every run. 
 
 Below is a sample prompt template:
 
@@ -160,16 +161,36 @@
 }
 ```
 
 Each patchflow comes with an optimized default prompt template. But you can specify your own using the `prompt_template_file=/path/to/prompt/template/file` option. 
 
 ## Contributing
 
-To create a new patchflow, follow [these instructions](patchwork/patchflows/README.md).
+Contributions for new patchflows and steps, or even to the core framework are welcome. Please look at open issues for details.
 
-To create a new step, follow [these instructions](patchwork/steps/README.md).
+- To create a new patchflow, follow [these instructions](patchwork/patchflows/README.md).
+- To create a new step, follow [these instructions](patchwork/steps/README.md).
 
-We also provide chat assitants to help you create new steps and patchflows easily.
+We also provide chat assistants to help you create new steps and patchflows easily. Fair warning: they suffer from the same limitations as their underlying model.
 
 - [Patchwork Assistant GPT](https://chatgpt.com/g/g-0G4sCAd2y-patchwork-assistant) (requires ChatGPT pro subscription)
 - [Patchwork Assistant on HuggingChat ](https://hf.co/chat/assistant/66322701fd4787e0c1f7696b) (free)
 
+## Roadmap
+
+### Short Term Q2 '24
+- Expand patchflow library and integration options
+- Patchflow debugger and validation module
+- Bug fixing and performance improvements
+- Refactor code and documentation
+
+### Long Term Q3/Q4 '24
+- Support large-scale code embeddings in patchflows
+- Support parallelization and branching
+- Fine-tuned models that can be self-hosted
+- Open-source GUI
+
+## License
+
+Patchwork is licensed under [AGPL-3.0 terms](https://github.com/patched-codes/patchwork?tab=AGPL-3.0-1-ov-file#readme). However, custom patchflows and steps can be created and shared using the [patchwork template](https://github.com/patched-codes/patchwork-configs) repository which is licensed under [Apache-2.0 terms](https://github.com/patched-codes/patchwork-configs/blob/main/LICENSE).
+
+
```

