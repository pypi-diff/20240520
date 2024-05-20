# Comparing `tmp/truefoundry-0.2.2rc1.tar.gz` & `tmp/truefoundry-0.2.2rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "truefoundry-0.2.2rc1.tar", max compression
+gzip compressed data, was "truefoundry-0.2.2rc2.tar", max compression
```

## Comparing `truefoundry-0.2.2rc1.tar` & `truefoundry-0.2.2rc2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0      871 2024-05-09 16:53:57.991343 truefoundry-0.2.2rc1/README.md
--rw-r--r--   0        0        0     1148 2024-05-09 16:54:07.603477 truefoundry-0.2.2rc1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-09 16:53:57.991343 truefoundry-0.2.2rc1/truefoundry/__init__.py
--rw-r--r--   0        0        0        0 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/autodeploy/__init__.py
--rw-r--r--   0        0        0        0 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/autodeploy/agents/__init__.py
--rw-r--r--   0        0        0     6405 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/autodeploy/agents/base.py
--rw-r--r--   0        0        0     4126 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/autodeploy/agents/developer.py
--rw-r--r--   0        0        0     4438 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/autodeploy/agents/project_identifier.py
--rw-r--r--   0        0        0     2352 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/autodeploy/agents/tester.py
--rw-r--r--   0        0        0    13651 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/autodeploy/cli.py
--rw-r--r--   0        0        0     1553 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/autodeploy/constants.py
--rw-r--r--   0        0        0      158 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/autodeploy/exception.py
--rw-r--r--   0        0        0      325 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/autodeploy/logger.py
--rw-r--r--   0        0        0      875 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/autodeploy/tools/__init__.py
--rw-r--r--   0        0        0      856 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/autodeploy/tools/ask.py
--rw-r--r--   0        0        0      665 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/autodeploy/tools/base.py
--rw-r--r--   0        0        0     5990 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/autodeploy/tools/commit.py
--rw-r--r--   0        0        0     3931 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/autodeploy/tools/docker_build.py
--rw-r--r--   0        0        0     4993 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/autodeploy/tools/docker_run.py
--rw-r--r--   0        0        0     2288 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/autodeploy/tools/file_type_counts.py
--rw-r--r--   0        0        0     2577 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/autodeploy/tools/list_files.py
--rw-r--r--   0        0        0     2187 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/autodeploy/tools/read_file.py
--rw-r--r--   0        0        0     1614 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/autodeploy/tools/send_request.py
--rw-r--r--   0        0        0     3130 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/autodeploy/tools/write_file.py
--rw-r--r--   0        0        0      453 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/autodeploy/utils/client.py
--rw-r--r--   0        0        0     5358 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/autodeploy/utils/diff.py
--rw-r--r--   0        0        0      412 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/autodeploy/utils/pydantic_compat.py
--rw-r--r--   0        0        0        0 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/cli/__init__.py
--rw-r--r--   0        0        0      916 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/cli/__main__.py
--rw-r--r--   0        0        0       43 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/deploy/__init__.py
--rw-r--r--   0        0        0        0 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/deploy/cli/__init__.py
--rw-r--r--   0        0        0     3135 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/deploy/cli/cli.py
--rw-r--r--   0        0        0     5105 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/deploy/cli/deploy.py
--rw-r--r--   0        0        0       53 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/langchain/__init__.py
--rw-r--r--   0        0        0      179 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/ml/__init__.py
--rw-r--r--   0        0        0     1839 1970-01-01 00:00:00.000000 truefoundry-0.2.2rc1/PKG-INFO
+-rw-r--r--   0        0        0      871 2024-05-20 05:25:09.300554 truefoundry-0.2.2rc2/README.md
+-rw-r--r--   0        0        0     1148 2024-05-20 05:25:18.904506 truefoundry-0.2.2rc2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-20 05:25:09.300554 truefoundry-0.2.2rc2/truefoundry/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-20 05:25:09.300554 truefoundry-0.2.2rc2/truefoundry/autodeploy/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-20 05:25:09.300554 truefoundry-0.2.2rc2/truefoundry/autodeploy/agents/__init__.py
+-rw-r--r--   0        0        0     6405 2024-05-20 05:25:09.300554 truefoundry-0.2.2rc2/truefoundry/autodeploy/agents/base.py
+-rw-r--r--   0        0        0     4126 2024-05-20 05:25:09.300554 truefoundry-0.2.2rc2/truefoundry/autodeploy/agents/developer.py
+-rw-r--r--   0        0        0     4504 2024-05-20 05:25:09.300554 truefoundry-0.2.2rc2/truefoundry/autodeploy/agents/project_identifier.py
+-rw-r--r--   0        0        0     2402 2024-05-20 05:25:09.300554 truefoundry-0.2.2rc2/truefoundry/autodeploy/agents/tester.py
+-rw-r--r--   0        0        0    13806 2024-05-20 05:25:09.300554 truefoundry-0.2.2rc2/truefoundry/autodeploy/cli.py
+-rw-r--r--   0        0        0     1553 2024-05-20 05:25:09.300554 truefoundry-0.2.2rc2/truefoundry/autodeploy/constants.py
+-rw-r--r--   0        0        0      158 2024-05-20 05:25:09.300554 truefoundry-0.2.2rc2/truefoundry/autodeploy/exception.py
+-rw-r--r--   0        0        0      325 2024-05-20 05:25:09.300554 truefoundry-0.2.2rc2/truefoundry/autodeploy/logger.py
+-rw-r--r--   0        0        0      875 2024-05-20 05:25:09.300554 truefoundry-0.2.2rc2/truefoundry/autodeploy/tools/__init__.py
+-rw-r--r--   0        0        0      856 2024-05-20 05:25:09.300554 truefoundry-0.2.2rc2/truefoundry/autodeploy/tools/ask.py
+-rw-r--r--   0        0        0      779 2024-05-20 05:25:09.300554 truefoundry-0.2.2rc2/truefoundry/autodeploy/tools/base.py
+-rw-r--r--   0        0        0     6036 2024-05-20 05:25:09.300554 truefoundry-0.2.2rc2/truefoundry/autodeploy/tools/commit.py
+-rw-r--r--   0        0        0     4000 2024-05-20 05:25:09.300554 truefoundry-0.2.2rc2/truefoundry/autodeploy/tools/docker_build.py
+-rw-r--r--   0        0        0     5061 2024-05-20 05:25:09.300554 truefoundry-0.2.2rc2/truefoundry/autodeploy/tools/docker_run.py
+-rw-r--r--   0        0        0     2338 2024-05-20 05:25:09.300554 truefoundry-0.2.2rc2/truefoundry/autodeploy/tools/file_type_counts.py
+-rw-r--r--   0        0        0     2644 2024-05-20 05:25:09.304554 truefoundry-0.2.2rc2/truefoundry/autodeploy/tools/list_files.py
+-rw-r--r--   0        0        0     2254 2024-05-20 05:25:09.304554 truefoundry-0.2.2rc2/truefoundry/autodeploy/tools/read_file.py
+-rw-r--r--   0        0        0     1680 2024-05-20 05:25:09.304554 truefoundry-0.2.2rc2/truefoundry/autodeploy/tools/send_request.py
+-rw-r--r--   0        0        0     3130 2024-05-20 05:25:09.304554 truefoundry-0.2.2rc2/truefoundry/autodeploy/tools/write_file.py
+-rw-r--r--   0        0        0      453 2024-05-20 05:25:09.304554 truefoundry-0.2.2rc2/truefoundry/autodeploy/utils/client.py
+-rw-r--r--   0        0        0     5358 2024-05-20 05:25:09.304554 truefoundry-0.2.2rc2/truefoundry/autodeploy/utils/diff.py
+-rw-r--r--   0        0        0      412 2024-05-20 05:25:09.304554 truefoundry-0.2.2rc2/truefoundry/autodeploy/utils/pydantic_compat.py
+-rw-r--r--   0        0        0        0 2024-05-20 05:25:09.304554 truefoundry-0.2.2rc2/truefoundry/cli/__init__.py
+-rw-r--r--   0        0        0      916 2024-05-20 05:25:09.304554 truefoundry-0.2.2rc2/truefoundry/cli/__main__.py
+-rw-r--r--   0        0        0       43 2024-05-20 05:25:09.304554 truefoundry-0.2.2rc2/truefoundry/deploy/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-20 05:25:09.304554 truefoundry-0.2.2rc2/truefoundry/deploy/cli/__init__.py
+-rw-r--r--   0        0        0     3135 2024-05-20 05:25:09.304554 truefoundry-0.2.2rc2/truefoundry/deploy/cli/cli.py
+-rw-r--r--   0        0        0     5105 2024-05-20 05:25:09.304554 truefoundry-0.2.2rc2/truefoundry/deploy/cli/deploy.py
+-rw-r--r--   0        0        0       53 2024-05-20 05:25:09.304554 truefoundry-0.2.2rc2/truefoundry/langchain/__init__.py
+-rw-r--r--   0        0        0      179 2024-05-20 05:25:09.304554 truefoundry-0.2.2rc2/truefoundry/ml/__init__.py
+-rw-r--r--   0        0        0     1839 1970-01-01 00:00:00.000000 truefoundry-0.2.2rc2/PKG-INFO
```

### Comparing `truefoundry-0.2.2rc1/README.md` & `truefoundry-0.2.2rc2/README.md`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.2rc1/pyproject.toml` & `truefoundry-0.2.2rc2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "truefoundry"
-version = "0.2.2rc1"
+version = "0.2.2rc2"
 description = "Truefoundry CLI"
 authors = ["Abhishek Choudhary <abhichoudhary06@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8,<3.13"
 servicefoundry = "0.10.11"
```

### Comparing `truefoundry-0.2.2rc1/truefoundry/autodeploy/agents/base.py` & `truefoundry-0.2.2rc2/truefoundry/autodeploy/agents/base.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.2rc1/truefoundry/autodeploy/agents/developer.py` & `truefoundry-0.2.2rc2/truefoundry/autodeploy/agents/developer.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.2rc1/truefoundry/autodeploy/agents/project_identifier.py` & `truefoundry-0.2.2rc2/truefoundry/autodeploy/agents/project_identifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,14 +88,15 @@
         )
         justification: str = Field(
             ...,
             description="Justification behind each response field.",
         )
 
         def render(self, console: Console):
+            console.rule("[bold green]Project Identification[/]")
             if self.primary_programming_language is not None:
                 console.print(
                     f"[bold magenta]TrueFoundry:[/] Identified a project using [bold cyan]{self.primary_programming_language}[/]."
                 )
                 console.print(
                     f"[bold magenta]TrueFoundry:[/] Framework Identified: [bold cyan]{'Not applicable' if self.framework is None else self.framework}[/]"
                 )
```

### Comparing `truefoundry-0.2.2rc1/truefoundry/autodeploy/agents/tester.py` & `truefoundry-0.2.2rc2/truefoundry/autodeploy/agents/tester.py`

 * *Files 9% similar despite different names*

```diff
@@ -48,14 +48,15 @@
             description="""
 Why was the testing a failure or successful?
         """,
         )
         logs: str
 
         def render(self, console: Console):
+            console.rule("[bold green]Result[/]")
             console.print(
                 f"[bold cyan]TrueFoundry:[/] The given project has been {'[bold green]successfully built[/]' if self.successful else '[bold red]failed to build[/]'}"
             )
             console.print(
                 f"[bold magenta]TrueFoundry:[/] [italic]{self.justification}[/]"
             )
             if not self.successful:
```

### Comparing `truefoundry-0.2.2rc1/truefoundry/autodeploy/cli.py` & `truefoundry-0.2.2rc2/truefoundry/autodeploy/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,15 +207,15 @@
     if isinstance(event, (Tester.Request, DockerRun.Response)):
         status.update(
             "[bold magenta]TrueFoundry[/] is currently running tests on the project..."
         )
 
     if isinstance(event, DockerRunLog):
         status.update(
-            "[bold cyan]Running:[/] [bold magenta]TrueFoundry[/] is executing the Docker container. Press [yellow]control + c[/] to stop waiting for additional logs..."
+            "[bold cyan]Running:[/] [bold magenta]TrueFoundry[/] is running your app in a Docker container. You can view logs here for potential warnings/errors. If you do not see any issues then you can press [yellow]control + c[/] to move to the next step."
         )
 
 
 def _get_default_project_name(project_root_path: str):
     path = os.path.abspath(project_root_path).rstrip(os.path.sep)
     name = path.split(os.path.sep)[-1].lower()
     name = re.sub(r"[^a-z0-9]", "-", name)
@@ -331,14 +331,15 @@
                 _update_status(event=event, status=status)
                 inp = event.render(console)
             except StopIteration as ex:
                 response = ex.value
                 break
 
     if deploy:
+        console.rule("[bold green]Deploying to Truefoundry[/]")
         deploy_component(
             workspace_fqn=workspace_fqn,
             project_root_path=project_root_path,
             dockerfile_path=response.dockerfile_path,
             name=name,
             component_type=component_type,
             env=env,
```

### Comparing `truefoundry-0.2.2rc1/truefoundry/autodeploy/constants.py` & `truefoundry-0.2.2rc2/truefoundry/autodeploy/constants.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.2rc1/truefoundry/autodeploy/tools/__init__.py` & `truefoundry-0.2.2rc2/truefoundry/autodeploy/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.2rc1/truefoundry/autodeploy/tools/ask.py` & `truefoundry-0.2.2rc2/truefoundry/autodeploy/tools/ask.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.2rc1/truefoundry/autodeploy/tools/base.py` & `truefoundry-0.2.2rc2/truefoundry/autodeploy/tools/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -25,7 +25,14 @@
 
 
 class Message(Event):
     message: Any
 
     def render(self, console: Console):
         console.print(self.message)
+
+
+class Rule(Event):
+    message: Any
+
+    def render(self, console: Console):
+        console.rule(self.message)
```

### Comparing `truefoundry-0.2.2rc1/truefoundry/autodeploy/tools/commit.py` & `truefoundry-0.2.2rc2/truefoundry/autodeploy/tools/commit.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
 
 class CommitConfirmation(Event):
     patch: str
     commit_message: str
 
     def render(self, console: Console) -> Optional["Commit.Response"]:
+        console.rule("[bold green]Commit[/]")
         console.print("[bold magenta]TrueFoundry[/] wants to make a commit,", end=" ")
         console.print(f"with Commit Message: [green]{self.commit_message}[/]")
         console.print("[yellow]Displaying changes to be made by the patch[/]")
         console.print(Padding.indent(renderable=LLMDiff(self.patch), level=2))
 
         response = Confirm.ask(
             "Apply patch?",
```

### Comparing `truefoundry-0.2.2rc1/truefoundry/autodeploy/tools/docker_build.py` & `truefoundry-0.2.2rc2/truefoundry/autodeploy/tools/docker_build.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from rich.text import Text
 
 from truefoundry.autodeploy.tools.base import (
     Event,
     Message,
     RequestEvent,
     ResponseEvent,
+    Rule,
     Tool,
 )
 
 
 class DockerBuildLog(Event):
     log: str
 
@@ -86,14 +87,15 @@
             yield Text.from_markup(f"  [yellow]error[/]={error_text}\n)")
 
     def __init__(self, project_root_path: str, docker_client: docker.DockerClient):
         self.project_root_path = project_root_path
         self.docker_client = docker_client
 
     def run(self, request: DockerBuild.Request) -> Generator[Event, Any, ResponseEvent]:
+        yield Rule(message="[bold green] Docker Build[/]")
         yield Message(message="[bold cyan]Processing:[/] Building Docker image...")
         yield Message(message="[bold yellow]Docker build logs:[/]")
         try:
             for message in _build(
                 self.docker_client,
                 path=self.project_root_path,
                 tag=request.image_tag,
```

### Comparing `truefoundry-0.2.2rc1/truefoundry/autodeploy/tools/docker_run.py` & `truefoundry-0.2.2rc2/truefoundry/autodeploy/tools/docker_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from rich.text import Text
 
 from truefoundry.autodeploy.tools.base import (
     Event,
     Message,
     RequestEvent,
     ResponseEvent,
+    Rule,
     Tool,
 )
 
 
 class DockerRunLog(Event):
     log: str
 
@@ -100,14 +101,16 @@
             try:
                 container.remove(force=True)
             except docker.errors.APIError:
                 pass
 
     def run(self, request: DockerRun.Request) -> Generator[Event, Any, ResponseEvent]:
         self._kill_running_containers()
+
+        yield Rule(message="[bold green] Docker Run[/]")
         yield Message(message="[bold cyan]Testing:[/] Running Docker container...")
         try:
             container = self.docker_client.containers.run(
                 request.image_tag,
                 detach=True,
                 remove=False,
                 stderr=True,
```

### Comparing `truefoundry-0.2.2rc1/truefoundry/autodeploy/tools/file_type_counts.py` & `truefoundry-0.2.2rc2/truefoundry/autodeploy/tools/file_type_counts.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from rich.table import Table
 
 from truefoundry.autodeploy.tools.base import (
     Event,
     Message,
     RequestEvent,
     ResponseEvent,
+    Rule,
     Tool,
 )
 
 
 class ShowFileCount(Event):
     file_types: Dict[str, int]
 
@@ -49,15 +50,15 @@
     def __init__(self, project_root_path: str):
         self.project_root_path = project_root_path
 
     def run(
         self, request: FileTypeCounts.Request
     ) -> Generator[Event, Any, ResponseEvent]:
         counter = Counter()
-
+        yield Rule(message="List Files")
         yield Message(
             message="[bold cyan]Processing:[/] Scanning for various file types..."
         )
 
         def gitignore(_):
             return False
```

### Comparing `truefoundry-0.2.2rc1/truefoundry/autodeploy/tools/list_files.py` & `truefoundry-0.2.2rc2/truefoundry/autodeploy/tools/list_files.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from pydantic import Field
 
 from truefoundry.autodeploy.tools.base import (
     Event,
     Message,
     RequestEvent,
     ResponseEvent,
+    Rule,
     Tool,
 )
 
 
 class ListFiles(Tool):
     description = """
 List all files.
@@ -37,14 +38,15 @@
         )
         error: Optional[str] = Field(None)
 
     def __init__(self, project_root_path: str):
         self.project_root_path = project_root_path
 
     def run(self, request: ListFiles.Request) -> Generator[Event, Any, ResponseEvent]:
+        yield Rule(message="[bold green] List Files[/]")
         yield Message(
             message=f"[bold cyan]Searching:[/] 🔍 Looking for files matching the pattern [magenta]{request.pattern}[/]"
         )
 
         paths: List[str] = []
 
         def gitignore(_):
```

### Comparing `truefoundry-0.2.2rc1/truefoundry/autodeploy/tools/read_file.py` & `truefoundry-0.2.2rc2/truefoundry/autodeploy/tools/read_file.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from truefoundry.autodeploy.constants import MAX_FILE_SIZE_READ
 from truefoundry.autodeploy.tools.base import (
     Event,
     Message,
     RequestEvent,
     ResponseEvent,
+    Rule,
     Tool,
 )
 
 
 class Line(BaseModel):
     line_number: int
     content: str
@@ -46,14 +47,15 @@
     def __init__(
         self,
         project_root_path: str,
     ):
         self.project_root_path = project_root_path
 
     def run(self, request: ReadFile.Request) -> Generator[Event, Any, ResponseEvent]:
+        yield Rule(message="[bold green] Read files[/]")
         yield Message(
             message=f"[bold cyan]Processing:[/] Reading file at [magenta]{request.path}[/] and extracting details..."
         )
 
         try:
             file_path = os.path.join(self.project_root_path, request.path)
             file_size = os.path.getsize(file_path)
```

### Comparing `truefoundry-0.2.2rc1/truefoundry/autodeploy/tools/send_request.py` & `truefoundry-0.2.2rc2/truefoundry/autodeploy/tools/send_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from pydantic import Field
 
 from truefoundry.autodeploy.tools.base import (
     Event,
     Message,
     RequestEvent,
     ResponseEvent,
+    Rule,
     Tool,
 )
 
 
 class SendRequest(Tool):
     description = """
 Send an HTTP request.
@@ -29,16 +30,17 @@
     class Response(ResponseEvent):
         response_code: Optional[int] = Field(None, description="Response Code")
         response_body: Optional[str] = None
         error: Optional[str] = Field(None, description="Error.")
 
     def run(self, request: SendRequest.Request) -> Generator[Event, Any, ResponseEvent]:
         self.call_count += 1
+        yield Rule(message="[bold green] Request send[/]")
         yield Message(
-            message=f"[bold cyan]Testing:[/] Sending a [magenta]{request.method.upper()}[/] request to [magenta]{request.url}[/]..."
+            message=f"[bold cyan]Testing:[/] Sending a [magenta]{request.method.upper()}[/] request to [magenta]{request.url}[/]"
         )
         try:
             response = requests.request(request.method.lower(), url=request.url)
             yield Message(
                 message=f"[bold green]Success:[/] Received response with status code [magenta]{response.status_code}[/]"
             )
             return SendRequest.Response(
```

### Comparing `truefoundry-0.2.2rc1/truefoundry/autodeploy/tools/write_file.py` & `truefoundry-0.2.2rc2/truefoundry/autodeploy/tools/write_file.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.2rc1/truefoundry/autodeploy/utils/diff.py` & `truefoundry-0.2.2rc2/truefoundry/autodeploy/utils/diff.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.2rc1/truefoundry/cli/__main__.py` & `truefoundry-0.2.2rc2/truefoundry/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.2rc1/truefoundry/deploy/cli/cli.py` & `truefoundry-0.2.2rc2/truefoundry/deploy/cli/cli.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.2rc1/truefoundry/deploy/cli/deploy.py` & `truefoundry-0.2.2rc2/truefoundry/deploy/cli/deploy.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.2rc1/PKG-INFO` & `truefoundry-0.2.2rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: truefoundry
-Version: 0.2.2rc1
+Version: 0.2.2rc2
 Summary: Truefoundry CLI
 Author: Abhishek Choudhary
 Author-email: abhichoudhary06@gmail.com
 Requires-Python: >=3.8,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

