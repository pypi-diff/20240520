# Comparing `tmp/taskara-0.1.8.tar.gz` & `tmp/taskara-0.1.80.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskara-0.1.8.tar", max compression
+gzip compressed data, was "taskara-0.1.80.tar", max compression
```

## Comparing `taskara-0.1.8.tar` & `taskara-0.1.80.tar`

### file list

```diff
@@ -1,10 +1,26 @@
--rw-r--r--   0        0        0    11357 2024-03-22 17:15:53.679144 taskara-0.1.8/LICENSE
--rw-r--r--   0        0        0      753 2024-04-03 02:46:31.154602 taskara-0.1.8/README.md
--rw-r--r--   0        0        0      392 2024-04-04 17:57:52.140664 taskara-0.1.8/pyproject.toml
--rw-r--r--   0        0        0       23 2024-04-02 20:42:34.072763 taskara-0.1.8/taskara/__init__.py
--rw-r--r--   0        0        0     2001 2024-04-02 20:34:43.380692 taskara-0.1.8/taskara/db/conn.py
--rw-r--r--   0        0        0     1352 2024-04-03 02:34:26.057465 taskara-0.1.8/taskara/db/models.py
--rw-r--r--   0        0        0      195 2024-04-02 20:31:31.417190 taskara-0.1.8/taskara/env.py
--rw-r--r--   0        0        0     1513 2024-04-04 16:36:43.488474 taskara-0.1.8/taskara/models.py
--rw-r--r--   0        0        0    18411 2024-04-04 17:57:44.458394 taskara-0.1.8/taskara/task.py
--rw-r--r--   0        0        0     1324 1970-01-01 00:00:00.000000 taskara-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-17 17:09:32.374116 taskara-0.1.80/LICENSE
+-rw-r--r--   0        0        0     2060 2024-05-18 03:15:36.175112 taskara-0.1.80/README.md
+-rw-r--r--   0        0        0     1149 2024-05-20 19:13:56.118335 taskara-0.1.80/pyproject.toml
+-rw-r--r--   0        0        0       81 2024-04-30 21:36:12.359132 taskara-0.1.80/taskara/__init__.py
+-rw-r--r--   0        0        0     1725 2024-04-30 21:35:45.162984 taskara-0.1.80/taskara/agent.py
+-rw-r--r--   0        0        0       23 2024-04-25 16:52:45.140876 taskara-0.1.80/taskara/auth/default.py
+-rw-r--r--   0        0        0     2548 2024-05-18 03:15:36.178446 taskara-0.1.80/taskara/auth/key.py
+-rw-r--r--   0        0        0     3106 2024-05-18 03:15:36.178774 taskara-0.1.80/taskara/auth/provider.py
+-rw-r--r--   0        0        0     1446 2024-05-18 03:15:36.179051 taskara-0.1.80/taskara/auth/transport.py
+-rw-r--r--   0        0        0     3250 2024-05-18 03:15:36.179410 taskara-0.1.80/taskara/cli/main.py
+-rw-r--r--   0        0        0      672 2024-05-18 03:15:36.179529 taskara-0.1.80/taskara/config.py
+-rw-r--r--   0        0        0     2517 2024-05-18 03:15:36.179872 taskara-0.1.80/taskara/db/conn.py
+-rw-r--r--   0        0        0     1639 2024-05-18 03:15:36.180173 taskara-0.1.80/taskara/db/models.py
+-rw-r--r--   0        0        0      195 2024-04-30 21:35:42.361364 taskara-0.1.80/taskara/env.py
+-rw-r--r--   0        0        0     1520 2024-04-30 21:35:40.978077 taskara-0.1.80/taskara/metrics.py
+-rw-r--r--   0        0        0    11573 2024-05-18 03:15:36.180417 taskara-0.1.80/taskara/runtime/base.py
+-rw-r--r--   0        0        0    11091 2024-05-18 03:15:36.180578 taskara-0.1.80/taskara/runtime/docker.py
+-rw-r--r--   0        0        0    28338 2024-05-18 03:15:36.180876 taskara-0.1.80/taskara/runtime/kube.py
+-rw-r--r--   0        0        0     1983 2024-05-18 03:15:36.181027 taskara-0.1.80/taskara/runtime/load.py
+-rw-r--r--   0        0        0    13524 2024-05-18 03:15:36.181232 taskara-0.1.80/taskara/runtime/process.py
+-rw-r--r--   0        0        0     2243 2024-05-18 03:15:36.181763 taskara-0.1.80/taskara/server/app.py
+-rw-r--r--   0        0        0     2747 2024-05-18 03:15:36.182016 taskara-0.1.80/taskara/server/models.py
+-rw-r--r--   0        0        0     8468 2024-05-18 03:15:36.182433 taskara-0.1.80/taskara/server/router/tasks.py
+-rw-r--r--   0        0        0    35236 2024-05-20 19:13:56.118769 taskara-0.1.80/taskara/task.py
+-rw-r--r--   0        0        0     1810 2024-05-18 03:15:36.183189 taskara-0.1.80/taskara/util.py
+-rw-r--r--   0        0        0     3314 1970-01-01 00:00:00.000000 taskara-0.1.80/PKG-INFO
```

### Comparing `taskara-0.1.8/taskara/db/conn.py` & `taskara-0.1.80/taskara/db/conn.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,49 +1,64 @@
 import os
+import time
+import logging
 
 from sqlalchemy import create_engine, Engine
 from sqlalchemy.orm import sessionmaker
 
 from .models import Base
 
 
+from taskara import config
+
+logger = logging.getLogger(__name__)
+
 DB_TYPE = os.environ.get("DB_TYPE", "sqlite")
 
 
 def get_pg_conn() -> Engine:
-    # Env Vars
-    db_user = os.environ.get("DB_USER")
-    if not db_user:
-        raise ValueError("$DB_USER must be set to a valid postgres db user")
-
-    db_password = os.environ.get("DB_PASS")
-    if not db_password:
-        raise ValueError("$DB_PASS must be set to a valid postgres db user password")
-
-    db_host = os.environ.get("DB_HOST")
-    if not db_user:
-        raise ValueError("$DB_HOST must be set to a running postgres server")
-
-    db_name = os.environ.get("DB_NAME")
-    if not db_name:
-        raise ValueError("$DB_NAME must be set to a postgres db name")
+    # Helper function to get environment variable with fallback
+    def get_env_var(key: str) -> str:
+        task_key = f"TASKS_{key}"
+        value = os.environ.get(task_key)
+        if value is None:
+            value = os.environ.get(key)
+            if value is None:
+                raise ValueError(f"${key} must be set")
+        return value
+
+    # Retrieve environment variables with fallbacks
+    db_user = get_env_var("DB_USER")
+    db_password = get_env_var("DB_PASS")
+    db_host = get_env_var("DB_HOST")
+    db_name = get_env_var("DB_NAME")
 
-    print(f"\nconnecting to db on postgres host '{db_host}' with db '{db_name}'")
+    logger.debug(f"connecting to db on postgres host '{db_host}' with db '{db_name}'")
     engine = create_engine(
         f"postgresql+psycopg2://{db_user}:{db_password}@{db_host}/{db_name}",
         client_encoding="utf8",
     )
 
     return engine
 
 
 def get_sqlite_conn() -> Engine:
-    print("\nconnecting to local sqlite db ./data/tasks.db")
-    os.makedirs(os.path.dirname("./data/tasks.db"), exist_ok=True)
-    engine = create_engine("sqlite:///./data/tasks.db")
+    db_name = os.environ.get("TASKS_DB_NAME", "tasks.db")
+    agentsea_home_path = os.path.expanduser(
+        os.environ.get("AGENTSEA_HOME", "~/.agentsea")
+    )
+    db_path = os.path.expanduser(
+        os.environ.get("AGENTSEA_DB_DIR", os.path.join(agentsea_home_path, "data"))
+    )
+    db_test = os.environ.get("TASKS_DB_TEST", "false") == "true"
+    if db_test:
+        db_name = f"tasks_test_{int(time.time())}.db"
+    logger.debug(f"connecting to local sqlite db ./.data/{db_name}")
+    os.makedirs(os.path.dirname(f"{db_path}/{db_name}"), exist_ok=True)
+    engine = create_engine(f"sqlite:///{db_path}/{db_name}")
     return engine
 
 
 if DB_TYPE == "postgres":
     engine = get_pg_conn()
 else:
     engine = get_sqlite_conn()
```

### Comparing `taskara-0.1.8/taskara/db/models.py` & `taskara-0.1.80/taskara/db/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,47 @@
+import time
+
 from sqlalchemy import Column, String, Float, Integer
 from sqlalchemy.orm import declarative_base
 
-from ..models import V1UserProfile
-
 Base = declarative_base()
 
 
 class TaskRecord(Base):
     __tablename__ = "tasks"
 
     id = Column(String, primary_key=True)
-    owner_id = Column(String, nullable=False)
+    owner_id = Column(String, nullable=True)
     description = Column(String, nullable=False)
-    url = Column(String, nullable=True)
+    max_steps = Column(Integer, nullable=False, default=30)
+    device = Column(String, nullable=True)
+    device_type = Column(String, nullable=True)
     assigned_to = Column(String, nullable=True)
+    assigned_type = Column(String, nullable=True)
     status = Column(String, nullable=False)
     created = Column(Float, nullable=False)
     started = Column(Float, nullable=False, default=0.0)
     completed = Column(Float, nullable=False, default=0.0)
-    error = Column(String, default="")
-    output = Column(String, default="")
+    error = Column(String, nullable=True)
+    output = Column(String, nullable=True)
     threads = Column(String, nullable=False)
-    version = Column(String, nullable=False)
+    prompts = Column(String, nullable=True)
+    parameters = Column(String, nullable=True)
+    version = Column(String, nullable=True)
+    tags = Column(String, nullable=True)
+    labels = Column(String, nullable=True)
+    episode_id = Column(String, nullable=True)
 
 
-class UserRecord(Base):
-    __tablename__ = "users"
+class TrackerRecord(Base):
+    __tablename__ = "trackers"
 
-    email = Column(String, unique=True, index=True, primary_key=True)
-    display_name = Column(String)
-    handle = Column(String)
-    picture = Column(String)
-    created = Column(Integer)
-    updated = Column(Integer)
-
-    def to_v1_schema(self) -> V1UserProfile:
-        return V1UserProfile(
-            email=self.email,
-            display_name=self.display_name,
-            picture=self.picture,
-            created=self.created,
-            updated=self.updated,
-        )
+    id = Column(String, primary_key=True)
+    name = Column(String, unique=True, index=True)
+    runtime_name = Column(String)
+    runtime_config = Column(String)
+    status = Column(String)
+    port = Column(Integer)
+    owner_id = Column(String, nullable=True)
+    labels = Column(String, nullable=True)
+    created = Column(Float, default=time.time)
+    updated = Column(Float, default=time.time)
```

### Comparing `taskara-0.1.8/taskara/models.py` & `taskara-0.1.80/taskara/server/models.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,59 +1,115 @@
-from typing import Optional, List
+from typing import Optional, List, Dict, Any
 import uuid
 import time
 
-from threadmem.server.models import RoleThreadModel
+from threadmem.server.models import V1RoleThread
 from pydantic import BaseModel, Field
+from devicebay.models import V1Device
+from devicebay import V1Device, V1DeviceType
+from mllm import V1Prompt
 
 
-class TaskCreateModel(BaseModel):
-    description: str
-    url: Optional[str] = None
-    assigned_to: Optional[str] = None
-
-
-class TaskUpdateModel(BaseModel):
+class V1TaskUpdate(BaseModel):
     status: Optional[str] = None
     description: Optional[str] = None
-    url: Optional[str] = None
+    max_steps: Optional[int] = None
     error: Optional[str] = None
     output: Optional[str] = None
     assigned_to: Optional[str] = None
     completed: Optional[float] = None
     version: Optional[str] = None
 
 
-class TaskModel(BaseModel):
+class V1Task(BaseModel):
     id: str = Field(default_factory=lambda: str(uuid.uuid4()))
     description: str
+    max_steps: int = 30
+    device: Optional[V1Device] = None
+    device_type: Optional[V1DeviceType] = None
     status: Optional[str] = None
-    threads: Optional[List[RoleThreadModel]] = None
+    threads: Optional[List[V1RoleThread]] = None
+    prompts: Optional[List[str]] = None
     assigned_to: Optional[str] = None
-    url: Optional[str] = None
+    assigned_type: Optional[str] = None
     created: float = Field(default_factory=time.time)
     started: float = 0.0
     completed: float = 0.0
-    error: str = ""
-    output: str = ""
+    error: Optional[str] = None
+    output: Optional[str] = None
+    parameters: Optional[Dict[str, Any]] = {}
     version: Optional[str] = None
+    remote: Optional[str] = None
+    owner_id: Optional[str] = None
+    tags: List[str] = []
+    labels: Dict[str, str] = {}
+    episode_id: Optional[str] = None
 
 
-class TasksModel(BaseModel):
-    tasks: List[TaskModel]
+class V1Tasks(BaseModel):
+    tasks: List[V1Task]
 
 
 class V1UserProfile(BaseModel):
     email: Optional[str] = None
     display_name: Optional[str] = None
     handle: Optional[str] = None
     picture: Optional[str] = None
     created: Optional[int] = None
     updated: Optional[int] = None
     token: Optional[str] = None
 
 
-class SolveTaskModel(BaseModel):
-    task: TaskModel
-    desktop_name: Optional[str] = None
-    max_steps: int = 20
-    site: Optional[str] = None
+class V1AddThread(BaseModel):
+    public: bool
+    name: Optional[str] = None
+    metadata: Optional[dict] = None
+    id: Optional[str] = None
+
+
+class V1RemoveThread(BaseModel):
+    id: str
+
+
+class V1PostMessage(BaseModel):
+    role: str
+    msg: str
+    images: List[str] = []
+    thread: Optional[str] = None
+
+
+class V1TrackerRuntimeConnect(BaseModel):
+    name: str
+    connect_config: BaseModel
+
+
+class V1Tracker(BaseModel):
+    name: str
+    runtime: V1TrackerRuntimeConnect
+    version: Optional[str] = None
+    port: int = 9090
+    labels: Dict[str, str] = {}
+    tags: List[str] = []
+    status: str
+    owner_id: Optional[str] = None
+    created: float
+    updated: float
+
+
+class V1Runtime(BaseModel):
+    type: str
+    preference: List[str] = []
+
+
+class V1ResourceLimits(BaseModel):
+    cpu: str = "2"
+    memory: str = "2Gi"
+
+
+class V1ResourceRequests(BaseModel):
+    cpu: str = "1"
+    memory: str = "500m"
+    gpu: Optional[str] = None
+
+
+class V1Prompts(BaseModel):
+    prompts: List[V1Prompt]
```

