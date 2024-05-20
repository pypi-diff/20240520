# Comparing `tmp/migro-0.3.0-py3-none-any.whl.zip` & `tmp/migro-0.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 9982 bytes, number of entries: 19
+Zip file size: 13020 bytes, number of entries: 19
 -rw-r--r--  2.0 unx        0 b- defN 21-Dec-07 14:30 migro/__init__.py
--rw-r--r--  2.0 unx     4732 b- defN 22-Jun-03 17:17 migro/database.py
--rw-r--r--  2.0 unx      622 b- defN 22-Jan-01 03:36 migro/dbt.py
+-rw-r--r--  2.0 unx     6511 b- defN 24-May-20 03:11 migro/database.py
+-rw-r--r--  2.0 unx     2134 b- defN 24-May-20 03:11 migro/dbt.py
 -rw-r--r--  2.0 unx      540 b- defN 21-Dec-12 05:26 migro/jinja.py
--rw-r--r--  2.0 unx     1442 b- defN 22-Jun-03 15:50 migro/main.py
--rw-r--r--  2.0 unx     3004 b- defN 22-Jun-03 15:50 migro/migrations.py
+-rw-r--r--  2.0 unx     1901 b- defN 24-May-20 03:11 migro/main.py
+-rw-r--r--  2.0 unx     3581 b- defN 24-May-20 03:11 migro/migrations.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Dec-16 05:05 tests/__init__.py
 -rw-r--r--  2.0 unx      138 b- defN 21-Dec-13 01:18 tests/conftest.py
--rw-r--r--  2.0 unx     1509 b- defN 22-Jan-19 20:01 tests/test_database.py
--rw-r--r--  2.0 unx      668 b- defN 22-Jan-01 03:36 tests/test_dbt.py
+-rw-r--r--  2.0 unx     3415 b- defN 24-May-20 03:11 tests/test_database.py
+-rw-r--r--  2.0 unx     5592 b- defN 24-May-20 03:11 tests/test_dbt.py
 -rw-r--r--  2.0 unx      303 b- defN 21-Dec-27 05:06 tests/test_jinja.py
--rw-r--r--  2.0 unx     1418 b- defN 21-Dec-27 05:26 tests/test_main.py
--rw-r--r--  2.0 unx     2994 b- defN 22-Jun-03 15:50 tests/test_migrations.py
--rw-r--r--  2.0 unx     1068 b- defN 22-Jun-03 20:20 migro-0.3.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1835 b- defN 22-Jun-03 20:20 migro-0.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Jun-03 20:20 migro-0.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       41 b- defN 22-Jun-03 20:20 migro-0.3.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       12 b- defN 22-Jun-03 20:20 migro-0.3.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1425 b- defN 22-Jun-03 20:20 migro-0.3.0.dist-info/RECORD
-19 files, 21843 bytes uncompressed, 7690 bytes compressed:  64.8%
+-rw-r--r--  2.0 unx     1406 b- defN 24-May-20 03:11 tests/test_main.py
+-rw-r--r--  2.0 unx     4006 b- defN 24-May-20 03:11 tests/test_migrations.py
+-rw-r--r--  2.0 unx     1068 b- defN 24-May-20 03:13 migro-0.4.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3383 b- defN 24-May-20 03:13 migro-0.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-20 03:13 migro-0.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       41 b- defN 24-May-20 03:13 migro-0.4.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 24-May-20 03:13 migro-0.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1427 b- defN 24-May-20 03:13 migro-0.4.0.dist-info/RECORD
+19 files, 35550 bytes uncompressed, 10728 bytes compressed:  69.8%
```

## zipnote {}

```diff
@@ -33,26 +33,26 @@
 
 Filename: tests/test_main.py
 Comment: 
 
 Filename: tests/test_migrations.py
 Comment: 
 
-Filename: migro-0.3.0.dist-info/LICENSE
+Filename: migro-0.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: migro-0.3.0.dist-info/METADATA
+Filename: migro-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: migro-0.3.0.dist-info/WHEEL
+Filename: migro-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: migro-0.3.0.dist-info/entry_points.txt
+Filename: migro-0.4.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: migro-0.3.0.dist-info/top_level.txt
+Filename: migro-0.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: migro-0.3.0.dist-info/RECORD
+Filename: migro-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## migro/database.py

```diff
@@ -1,46 +1,51 @@
+import base64
 import psycopg2
 import psycopg2.extras
 import snowflake.connector
 import sqlite3
 from dataclasses import dataclass
-from typing import ClassVar
+from typing import ClassVar, Optional
+from cryptography.hazmat.backends import default_backend
+from cryptography.hazmat.primitives import serialization
 
 from migro import dbt
 
 
-def get_database_instance(profile=None):
-    db_config = dbt.get_output(profile=profile)
+def get_database_instance(profile=None, target=None):
+    db_config = dbt.get_target_output(profile_name=profile, target=target)
 
     if db_config["type"] == "redshift":
         return RedshiftDatabase(
             host=db_config["host"],
             user=db_config["user"],
-            password=db_config["password"]
-            if "password" in db_config
-            else db_config["pass"],
+            password=(
+                db_config["password"] if "password" in db_config else db_config["pass"]
+            ),
             port=db_config["port"],
             dbname=db_config["dbname"],
         )
 
     if db_config["type"] == "sqlite":
         return SqliteDatabase()
 
     if db_config["type"] == "snowflake":
         return SnowflakeDatabase(
             account=db_config["account"],
             user=db_config["user"],
-            password=db_config["password"],
+            password=db_config.get("password"),
             database=db_config["database"],
+            warehouse=db_config["warehouse"],
+            private_key=db_config.get("private_key"),
+            private_key_passphrase=db_config.get("private_key_passphrase"),
         )
 
 
 @dataclass
 class Database:
-
     MIGRATIONS_TABLE_SQL: ClassVar[str]
 
     def _get_connection(self):
         raise NotImplementedError
 
     def create_migrations_table(self):
         raise NotImplementedError
@@ -54,18 +59,15 @@
 
     def get_migrations(self):
         raise NotImplementedError
 
 
 @dataclass
 class SqliteDatabase(Database):
-
-    MIGRATIONS_TABLE_SQL: ClassVar[
-        str
-    ] = """
+    MIGRATIONS_TABLE_SQL: ClassVar[str] = """
         create table if not exists migrations
         (
             id integer primary key,
             migration varchar(2000) not null,
             applied_at timestamp default current_timestamp not null
         )
     """
@@ -91,17 +93,15 @@
 class RedshiftDatabase(Database):
     host: str
     user: str
     password: str
     port: int
     dbname: str
 
-    MIGRATIONS_TABLE_SQL: ClassVar[
-        str
-    ] = """
+    MIGRATIONS_TABLE_SQL: ClassVar[str] = """
         create table if not exists migrations
         (
             id int identity not null,
             migration varchar(2000) not null,
             applied_at timestamp default getdate() not null
         )
     """
@@ -140,45 +140,81 @@
 
 @dataclass
 class SnowflakeDatabase(Database):
     account: str
     user: str
     password: str
     database: str
+    warehouse: str
+    private_key: Optional[str] = None
+    private_key_passphrase: Optional[str] = None
 
-    MIGRATIONS_TABLE_SQL: ClassVar[
-        str
-    ] = """
+    MIGRATIONS_TABLE_SQL: ClassVar[str] = """
         create table if not exists PUBLIC.migrations
         (
             id int identity not null,
             migration varchar(2000) not null,
             applied_at timestamp default current_timestamp() not null
         )
     """
 
     def _get_connection(self):
         return snowflake.connector.connect(
             user=self.user,
             password=self.password,
             account=self.account,
             database=self.database,
+            warehouse=self.warehouse,
+            private_key=self._get_private_key(),
+        )
+
+    def _get_private_key(self):
+        """
+        base64 decode the private key, decrypt it, and return an instance of AuthByKeyPair
+        See dbt-snowflake private key code:
+        https://github.com/dbt-labs/dbt-snowflake/blob/87a6e808dfb025df1eeef3741ad3822635249889/dbt/adapters/snowflake/connections.py#L244
+        """
+        if not self.private_key:
+            return None
+
+        if self.private_key_passphrase:
+            encoded_passphrase = self.private_key_passphrase.encode()
+        else:
+            encoded_passphrase = None
+
+        if self.private_key.startswith("-"):
+            p_key = serialization.load_pem_private_key(
+                data=bytes(self.private_key, "utf-8"),
+                password=encoded_passphrase,
+                backend=default_backend(),
+            )
+        else:
+            p_key = serialization.load_der_private_key(
+                data=base64.b64decode(self.private_key),
+                password=encoded_passphrase,
+                backend=default_backend(),
+            )
+
+        return p_key.private_bytes(
+            encoding=serialization.Encoding.DER,
+            format=serialization.PrivateFormat.PKCS8,
+            encryption_algorithm=serialization.NoEncryption(),
         )
 
     def create_migrations_table(self):
         self.execute(self.MIGRATIONS_TABLE_SQL)
 
     def get_migrations(self):
         con = self._get_connection()
         with con.cursor(snowflake.connector.DictCursor) as cur:
             cur.execute(
                 (
                     """
-                SELECT ID as "id", MIGRATION as "migration", APPLIED_AT as "applied_at"
-                FROM public.migrations ORDER BY migration ASC
-                """
+                    SELECT ID as "id", MIGRATION as "migration", APPLIED_AT as "applied_at"
+                    FROM PUBLIC.migrations ORDER BY migration ASC
+                    """
                 )
             )
             migrations = cur.fetchall()
             cur.close()
         con.close()
         return migrations
```

## migro/dbt.py

```diff
@@ -1,24 +1,74 @@
-import click
 import os
 import yaml
 from migro import jinja
 
 
-def get_output(profile=None):
+def _get_profiles_path():
+    """
+    dbt best practice is to store the profiles.yml file in the ~/.dbt directory.
+    But it's common to store the profiles.yml file in the root of the dbt project.
+    migro checks the local project directory and then checks the .dbt home directory.
+    Return the path to the profiles.yml file.
+    """
 
-    if not os.path.isfile("profiles.yml"):
-        click.echo(click.style("Missing dbt profiles.yml", fg="red"))
-        exit()
+    if os.path.isfile("./profiles.yml"):
+        return "./profiles.yml"
+    elif os.path.isfile("~/.dbt/profiles.yml"):
+        return "~/.dbt/profiles.yml"
+    else:
+        raise Exception("Missing dbt profiles.yml")
 
-    profiles = jinja.render_jinja_template("profiles.yml")
-    profiles = yaml.safe_load(profiles)
 
-    for profile_name, p in profiles.items():
-        if profile and profile != profile_name:
+def _profiles_yaml_to_dict(profiles_path):
+    """
+    Render the profiles.yml file using jinja.
+    Return the rendered profiles.yml file as a dictionary.
+    """
+
+    profiles_yaml: str = jinja.render_jinja_template(profiles_path)
+    return yaml.safe_load(profiles_yaml)
+
+
+def _get_profile(profiles: dict, profile_name: str = None) -> dict:
+    """
+    Return the target dbt profile from a list of profiles.
+    """
+
+    for key, profile in profiles.items():
+        # Return the first profile when no profile_name is specified.
+        if profile_name is None:
+            return profile
+
+        if key == profile_name:
+            return profile
+
+    raise Exception(f"Profile {profile_name} not found in profiles.yml")
+
+
+def _get_output(profile: dict, target: str = None) -> dict:
+    """
+    Return the target dbt output from a profile.
+    """
+
+    if not target:
+        target = profile.get("target")
+
+    assert target is not None, "No target specified"
+
+    for output_name, output in profile["outputs"].items():
+        if target != output_name:
             continue
+        return output
+
+    raise Exception(f"Target {target} not found in profiles.yml")
+
 
-        target = p["target"]
+def get_target_output(profile_name: str = None, target=None) -> dict:
+    """
+    Get the target output database configuration from the dbt profiles.yml file.
+    """
 
-        for output_key, output in p["outputs"].items():
-            if len(p["outputs"].keys()) == 1 or target == output_key:
-                return output
+    profiles_path = _get_profiles_path()
+    profiles = _profiles_yaml_to_dict(profiles_path)
+    profile = _get_profile(profiles, profile_name)
+    return _get_output(profile, target)
```

## migro/main.py

```diff
@@ -1,35 +1,42 @@
 import click
-from migro.migrations import MigrationRepository
+from migro.migrations import MigrationRepository, DEFAULT_MIGRATION_DIRECTORY
 
 
 @click.group()
 def cli():
     """Data Warehouse migrations"""
 
 
+@click.command()
 @click.option(
     "--pretend",
     is_flag=True,
     default=False,
     help="Show the queries that migro would run",
 )
 @click.option("--limit", type=int, help="Limit the number of migrations to run")
-@click.option("--dbt-profile", help="dbt profile key in profiles.yml")
-@click.command()
-def up(pretend, limit, dbt_profile):
+@click.option("--profile", help="dbt profile key in profiles.yml")
+@click.option(
+    "--directory",
+    help="Directory to store migrations",
+    default=DEFAULT_MIGRATION_DIRECTORY,
+)
+@click.option("--target", help="dbt output target (warehouse) key in profiles.yml")
+def up(pretend, limit, profile, directory, target):
     """Run the unapplied SQL in the migrations directory"""
 
     applied = 0
-    migrations_repo = MigrationRepository(dbt_profile)
+    migrations_repo = MigrationRepository(
+        profile=profile, directory=directory, target=target
+    )
 
     migrations_repo.create_migrations_table()
 
     for migration in migrations_repo.all():
-
         if limit and applied >= limit:
             break
 
         if migration.applied_at:
             continue
 
         click.echo(click.style(f"Migrating: {migration.file_path}", fg="yellow"))
@@ -40,18 +47,23 @@
             click.echo(click.style(f"Migrated:  {migration.file_path}", fg="green"))
 
         applied += 1
 
 
 @click.command()
 @click.argument("name")
-def make(name):
+@click.option(
+    "--directory",
+    help="Directory to store migrations",
+    default=DEFAULT_MIGRATION_DIRECTORY,
+)
+def make(name, directory):
     """Create a new migration file. For example, migro make add_user_tharvey"""
 
-    migrations_repo = MigrationRepository()
+    migrations_repo = MigrationRepository(profile=None, directory=directory)
     migration_file = migrations_repo.make(name)
 
     click.echo(click.style(f"Created: {migration_file}", fg="green"))
 
 
 cli.add_command(up)
 cli.add_command(make)
```

## migro/migrations.py

```diff
@@ -4,98 +4,115 @@
 import string
 
 from datetime import datetime
 from dataclasses import dataclass
 
 from migro import jinja, database
 
-MIGRATION_FILE_PATH = "./migrations"
+DEFAULT_MIGRATION_DIRECTORY = "migrations"
 
 
 @dataclass
 class Migration:
     id: int = None
     name: str = None
     applied_at: datetime = None
+    directory: str = DEFAULT_MIGRATION_DIRECTORY
     file_path: str = None
 
     def _password(self):
         """
         Generate a random password with lowercase, uppercase, numbers,
         and special characters
         """
         return "".join(
             random.choice(string.ascii_letters + string.digits + "$%@")
             for _ in range(32)
         )
 
+    def _full_path(self):
+        return f"./{self.directory}/{self.file_path}"
+
     def sql(self):
-        sql = jinja.render_jinja_template(
-            f"{MIGRATION_FILE_PATH}/{self.file_path}", password=self._password()
-        )
+        sql = jinja.render_jinja_template(self._full_path(), password=self._password())
         return sqlparse.format(sql, strip_comments=True).strip()
 
 
 class MigrationRepository:
-    def __init__(self, profile=None):
+    def __init__(
+        self, profile=None, directory=DEFAULT_MIGRATION_DIRECTORY, target=None
+    ):
+        self.directory = directory
         self.profile = profile
-        self.db = database.get_database_instance(profile)
+        self.target = target
+        self.db = None
+
+    def _get_db(self):
+        """
+        A singletown database instance for the repository.
+        """
+        if not self.db:
+            self.db = database.get_database_instance(
+                profile=self.profile, target=self.target
+            )
+        return self.db
 
     def _get_migration_files(self):
         migration_files = []
-        for file in sorted(os.listdir(MIGRATION_FILE_PATH)):
+        for file in sorted(os.listdir(f"./{self.directory}")):
             if file.endswith(".sql"):
                 migration_files.append(file)
         return migration_files
 
     def _log_migration(self, migration: Migration):
-        self.db.execute(
+        self._get_db().execute(
             f"insert into migrations (migration) values ('{migration.file_path}')"
         )
 
     def all(self):
         migrations = []
         migration_files = self._get_migration_files()
-        migration_records = self.db.get_migrations()
+        migration_records = self._get_db().get_migrations()
 
         while migration_files:
-            migration = Migration(file_path=migration_files.pop(0))
+            migration_file = migration_files.pop(0)
+            migration = Migration(file_path=migration_file, directory=self.directory)
 
             if migration_records:
                 migration_record = migration_records.pop(0)
 
-                if migration.file_path != migration_record["migration"]:
+                if migration_record["migration"] not in migration.file_path:
                     raise Exception(
                         (
                             f"""
-                        Migrations table out of sync with migrations on the filesystem.
-                        {migration.file_path} != {migration_record['migration']}
-                        """
+                            Migrations table out of sync with migrations on the filesystem.
+                            {migration.file_path} != {migration_record['migration']}
+                            """
                         )
                     )
 
                 migration.id = migration_record["id"]
                 migration.name = migration_record["migration"]
                 migration.applied_at = migration_record["applied_at"]
 
             migrations.append(migration)
         return migrations
 
     def apply(self, migration: Migration) -> str:
         sql = migration.sql()
         if sql:
-            self.db.execute(sql)
+            self._get_db().execute(sql)
         self._log_migration(migration)
         return sql
 
     def create_migrations_table(self):
-        self.db.create_migrations_table()
+        self._get_db().create_migrations_table()
 
     def make(self, name) -> str:
         migration_date = datetime.now().strftime("%Y%m%d%H%M%S")
-        migration_file = f"{MIGRATION_FILE_PATH}/{migration_date}_{name}.sql"
+        migration_file = f"./{self.directory}/{migration_date}_{name}.sql"
 
         if not os.path.exists(migration_file):
             with open(migration_file, "w"):
                 pass
 
         return migration_file
```

## tests/test_database.py

```diff
@@ -1,7 +1,8 @@
+import base64
 import pytest
 from migro import database
 from unittest import mock
 
 
 def test_get_sqlite_database_instance():
     db = database.get_database_instance("sqlite_profile")
@@ -50,13 +51,81 @@
 @mock.patch("snowflake.connector.connect")
 def test_snowflake_database(snowflake_mock):
     db = database.SnowflakeDatabase(
         account="account",
         user="user",
         password="password",
         database="database",
+        warehouse="warehouse",
     )
 
     db.create_migrations_table()
     db.get_migrations()
 
     snowflake_mock.assert_called()
+
+
+def test_get_private_key_pem():
+    """
+    openssl command used to create the pem fixture:
+    openssl genrsa 2048 | openssl pkcs8 -topk8 -inform PEM -out tests/fixtures/private_key.pem
+    """
+    with open("tests/fixtures/private_key.pem", "r") as f:
+        pem_key = f.read()
+
+    db = database.SnowflakeDatabase(
+        account="test",
+        user="test",
+        password="test",
+        database="test",
+        warehouse="test",
+        private_key=pem_key,
+        private_key_passphrase="fripper",
+    )
+    result = db._get_private_key()
+
+    assert isinstance(result, bytes)
+
+
+def test_get_private_key_pem_no_passphrase():
+    """
+    openssl command used to create the pem fixture:
+    openssl genrsa 2048 | openssl pkcs8 -topk8 -inform PEM -out tests/fixtures/private_key_no_passphrase.pem -nocrypt
+    """
+
+    with open("tests/fixtures/private_key_no_passphrase.pem", "r") as f:
+        pem_key = f.read()
+
+    db = database.SnowflakeDatabase(
+        account="test",
+        user="test",
+        password="test",
+        database="test",
+        warehouse="test",
+        private_key=pem_key,
+    )
+    result = db._get_private_key()
+
+    assert isinstance(result, bytes)
+
+
+def test_get_private_key_der():
+    """
+    openssl command used to create the der fixture:
+    openssl pkcs8 -topk8 -in tests/fixtures/private_key.pem -outform DER -out tests/fixtures/private_key.der
+    """
+    with open("tests/fixtures/private_key.der", "rb") as f:
+        der_key = f.read()
+        der_key = base64.b64encode(der_key).decode("utf-8")
+
+    db = database.SnowflakeDatabase(
+        account="test",
+        user="test",
+        password="test",
+        database="test",
+        warehouse="test",
+        private_key=der_key,
+        private_key_passphrase="fripper",
+    )
+    result = db._get_private_key()
+
+    assert isinstance(result, bytes)
```

## tests/test_dbt.py

```diff
@@ -1,25 +1,205 @@
+import os
 import pytest
 
 from migro import dbt
-from pathlib import Path
 
 
 def test_get_output():
-    output = dbt.get_output()
+    profile = {
+        "outputs": {
+            "redshift": {
+                "type": "redshift",
+                "threads": 8,
+                "host": "localhost",
+                "port": "5555",
+                "user": "tharvey",
+                "pass": "password",
+                "dbname": "derp",
+                "schema": "public",
+                "ra3_node": True,
+                "retries": 3,
+            },
+            "snowflake": {
+                "type": "snowflake",
+                "account": "xt83740.us-east-1",
+                "user": "troyharvey",
+                "password": "password",
+                "database": "US_TESTING",
+                "warehouse": "US_TESTING_WH",
+                "schema": "PUBLIC",
+                "threads": 4,
+            },
+        },
+        "target": "redshift",
+    }
+
+    output = dbt._get_output(profile=profile, target="snowflake")
+    assert output["type"] == "snowflake"
+    assert output["account"] == "xt83740.us-east-1"
+    assert output["user"] == "troyharvey"
+    assert output["database"] == "US_TESTING"
+    assert output["warehouse"] == "US_TESTING_WH"
+    assert output["schema"] == "PUBLIC"
+    assert output["threads"] == 4
+
+    output = dbt._get_output(profile=profile)
     assert output["type"] == "redshift"
     assert output["host"] == "localhost"
+    assert output["port"] == "5555"
     assert output["user"] == "tharvey"
-    assert output["port"] == 55091
-    assert output["dbname"] == "sandbox_tharvey"
+    assert output["dbname"] == "derp"
+    assert output["schema"] == "public"
+
 
+def test_get_output_no_target_specified():
+    profile = {
+        "outputs": {
+            "redshift": {
+                "type": "redshift",
+                "host": "localhost",
+            }
+        }
+    }
+
+    with pytest.raises(Exception) as e:
+        dbt._get_output(profile=profile)
+    assert str(e.value) == "No target specified"
+
+
+def test_get_output_target_not_found():
+    profile = {
+        "outputs": {
+            "redshift": {
+                "type": "redshift",
+                "host": "localhost",
+            }
+        }
+    }
+
+    with pytest.raises(Exception) as e:
+        dbt._get_output(profile=profile, target="donkeykong")
+    assert str(e.value) == "Target donkeykong not found in profiles.yml"
+
+
+def test_get_profile():
+    profiles = {
+        "default": {
+            "outputs": {
+                "redshift": {
+                    "type": "redshift",
+                    "threads": 8,
+                    "host": "localhost",
+                }
+            },
+            "target": "redshift",
+        },
+        "dev": {
+            "outputs": {
+                "snowflake": {
+                    "type": "snowflake",
+                }
+            },
+            "target": "snowflake",
+        },
+        "config": {"send_anonymous_usage_stats": False},
+    }
+
+    profile = dbt._get_profile(profiles, "default")
+    assert profile.get("target") == "redshift"
+
+    profile = dbt._get_profile(profiles, "dev")
+    assert profile.get("target") == "snowflake"
+
+
+def test_get_profile_no_profile_name_provided():
+    profiles = {
+        "default": {
+            "outputs": {
+                "redshift": {
+                    "type": "redshift",
+                    "threads": 8,
+                    "host": "localhost",
+                }
+            },
+            "target": "redshift",
+        },
+        "config": {"send_anonymous_usage_stats": False},
+    }
+
+    profile = dbt._get_profile(profiles)
+    assert profile.get("target") == "redshift"
+
+
+def test_get_profile_not_found():
+    profiles = {
+        "default": {
+            "outputs": {
+                "redshift": {
+                    "type": "redshift",
+                    "threads": 8,
+                    "host": "localhost",
+                }
+            },
+            "target": "redshift",
+        },
+        "dev": {
+            "outputs": {
+                "snowflake": {
+                    "type": "snowflake",
+                }
+            },
+            "target": "snowflake",
+        },
+        "config": {"send_anonymous_usage_stats": False},
+    }
+
+    profile = dbt._get_profile(profiles, "default")
+    assert profile.get("target") == "redshift"
+
+    profile = dbt._get_profile(profiles, "dev")
+    assert profile.get("target") == "snowflake"
+
+    with pytest.raises(Exception) as e:
+        dbt._get_profile(profiles, "skibiti")
+    assert str(e.value) == "Profile skibiti not found in profiles.yml"
+
+
+def test_profiles_yaml_to_dict():
+    profiles_path = "./profiles.yml"
+    profiles = dbt._profiles_yaml_to_dict(profiles_path)
+    assert profiles["redshift_profile"]["target"] == "dev"
+    assert profiles["sqlite_profile"]["outputs"]["dev"]["type"] == "sqlite"
+
+
+def test_get_profiles_path(monkeypatch):
+    def mock_isfile(path):
+        if path == "./profiles.yml":
+            return True
+
+    monkeypatch.setattr(os.path, "isfile", mock_isfile)
+
+    assert dbt._get_profiles_path() == "./profiles.yml"
+
+
+def test_get_profiles_path_dbt(monkeypatch):
+    def mock_isfile(path):
+        if path == "./profiles.yml":
+            return False
+        elif path == "~/.dbt/profiles.yml":
+            return True
+
+    monkeypatch.setattr(os.path, "isfile", mock_isfile)
+
+    assert dbt._get_profiles_path() == "~/.dbt/profiles.yml"
+
+
+def test_get_profiles_path_exception(monkeypatch):
+    def mock_isfile(path):
+        return False
 
-def test_get_output_sqlite():
-    output = dbt.get_output(profile="sqlite_profile")
-    assert output["type"] == "sqlite"
+    monkeypatch.setattr(os.path, "isfile", mock_isfile)
 
+    with pytest.raises(Exception) as e_info:
+        dbt._get_profiles_path()
 
-def test_get_output_without_dbt_profile_yaml():
-    Path("./profiles.yml").rename("./profiles.yml.bak")
-    with pytest.raises(SystemExit):
-        dbt.get_output()
-    Path("./profiles.yml.bak").rename("./profiles.yml")
+    assert str(e_info.value) == "Missing dbt profiles.yml"
```

## tests/test_main.py

```diff
@@ -20,27 +20,27 @@
     assert "Created:" in result.output
     assert "_add_user_zharvey.sql" in result.output
 
 
 def test_up_pretend():
     runner = CliRunner()
     result = runner.invoke(
-        main.up, ["--pretend", "--limit=1", "--dbt-profile=sqlite_profile"]
+        main.up, ["--pretend", "--limit=1", "--profile=sqlite_profile"]
     )
     assert result.exit_code == 0
     assert "Migrating:" in result.output
     assert "_add_user_tharvey.sql" in result.output
 
 
 def test_up():
     runner = CliRunner()
-    result = runner.invoke(main.up, ["--limit=1", "--dbt-profile=sqlite_profile"])
+    result = runner.invoke(main.up, ["--limit=1", "--profile=sqlite_profile"])
     assert result.exit_code == 0
     assert "Migrating:" in result.output
     assert "_add_user_tharvey.sql" in result.output
     assert "Migrated:" in result.output
 
-    result = runner.invoke(main.up, ["--dbt-profile=sqlite_profile"])
+    result = runner.invoke(main.up, ["--profile=sqlite_profile"])
     assert result.exit_code == 0
     assert "Migrating:" in result.output
     assert "_add_user_zharvey.sql" in result.output
     assert "Migrated:" in result.output
```

## tests/test_migrations.py

```diff
@@ -10,28 +10,32 @@
 class TestMigrationRepository:
     def setup_class(self):
         try:
             os.remove("./tests/demo.db")
         except Exception:
             pass
 
-        for f in glob.glob(os.path.join(migrations.MIGRATION_FILE_PATH, "*.sql")):
+        for f in glob.glob(
+            os.path.join("./", migrations.DEFAULT_MIGRATION_DIRECTORY, "*.sql")
+        ):
             os.remove(f)
 
     def teardown_class(self):
         try:
             os.remove("./tests/demo.db")
         except Exception:
             pass
 
-        for f in glob.glob(os.path.join(migrations.MIGRATION_FILE_PATH, "*.sql")):
+        for f in glob.glob(
+            os.path.join("./", migrations.DEFAULT_MIGRATION_DIRECTORY, "*.sql")
+        ):
             os.remove(f)
 
     def test_migrations_flow(self):
-        migrations_repo = migrations.MigrationRepository("sqlite_profile")
+        migrations_repo = migrations.MigrationRepository(profile="sqlite_profile")
 
         # Test setting up migrations log table
         migrations_repo.create_migrations_table()
         assert [] == migrations_repo.all()
 
         # Test making a migration file
         migration_file = migrations_repo.make("create_attribution_table")
@@ -51,45 +55,74 @@
             assert sql == "CREATE TABLE attribution(foo TEXT);"
 
         # There should be no migration left to apply
         for m in migrations_repo.all():
             assert m.applied_at is not None
 
         # Force migrations file system out of sync with migrations table
-        os.rename(migration_file, f"{migrations.MIGRATION_FILE_PATH}/foo.sql")
+        os.rename(migration_file, f"{migrations.DEFAULT_MIGRATION_DIRECTORY}/foo.sql")
         with pytest.raises(
             Exception,
             match="Migrations table out of sync with migrations on the filesystem.",
         ):
             migrations_repo.all()
 
 
 class TestMigration:
+    DIRECTORY = f"./{migrations.DEFAULT_MIGRATION_DIRECTORY}"
+
     def setup_method(self):
-        with open(f"{migrations.MIGRATION_FILE_PATH}/test.sql", "w") as f:
+        if not os.path.exists(self.DIRECTORY):
+            os.makedirs(self.DIRECTORY)
+
+        with open(f"{self.DIRECTORY}/test.sql", "w") as f:
             f.write(
                 """
                 -- This comment should be removed when sql is rendered
                 select '{{password}}' as pw;
                 """
             )
 
     def teardown_method(self):
-        try:
-            os.remove(f"{migrations.MIGRATION_FILE_PATH}/test.sql")
-        except Exception:
-            pass
+        for f in glob.glob(
+            os.path.join("./", migrations.DEFAULT_MIGRATION_DIRECTORY, "*.sql")
+        ):
+            os.remove(f)
 
     def test_migrations_path_constant(self):
-        assert migrations.MIGRATION_FILE_PATH == "./migrations"
+        assert migrations.DEFAULT_MIGRATION_DIRECTORY == "migrations"
 
     def test_password(self):
         m = migrations.Migration()
         password = m._password()
         assert len(password) == 32
         assert re.match(PASSWORD_REGEX, password)
 
     def test_sql(self):
-        m = migrations.Migration()
-        m.file_path = "test.sql"
+        m = migrations.Migration(file_path="test.sql")
+        sql = m.sql()
+        assert re.match(f"^select '{PASSWORD_REGEX}' as pw;$", sql)
+
+
+class TestMigrationWithCustomDirectory:
+    DIRECTORY = "./migrations_snowflake"
+
+    def setup_method(self):
+        if not os.path.exists(self.DIRECTORY):
+            os.makedirs(self.DIRECTORY)
+
+        with open(f"{self.DIRECTORY}/test.sql", "w") as f:
+            f.write(
+                """
+                -- This comment should be removed when sql is rendered
+                select '{{password}}' as pw;
+                """
+            )
+
+    def teardown_method(self):
+        for f in glob.glob(os.path.join("./", self.DIRECTORY, "*.sql")):
+            os.remove(f)
+
+    def test_sql(self):
+        m = migrations.Migration(file_path="test.sql", directory=self.DIRECTORY)
         sql = m.sql()
         assert re.match(f"^select '{PASSWORD_REGEX}' as pw;$", sql)
```

## Comparing `migro-0.3.0.dist-info/LICENSE` & `migro-0.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `migro-0.3.0.dist-info/RECORD` & `migro-0.4.0.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 migro/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-migro/database.py,sha256=DF-2AnjWomYYZT31gDCuDN9YbSxzBFEjofTGqHTZkak,4732
-migro/dbt.py,sha256=FRYznaJlfAzGsLaukXmlzpwMEzcizsxU9WYN2aU2ZAo,622
+migro/database.py,sha256=WrAXndLlUYwVBDH85i7uudxjxLMdnzECPe4tWgTawoU,6511
+migro/dbt.py,sha256=t6igE6WyNeVMEt_nOvz9R8OAHcy2JpObGpiSXJnALV4,2134
 migro/jinja.py,sha256=KcdcxLwDMyUhYNie1tUIG3Yis21ZwLwk4Drq2WQR-I8,540
-migro/main.py,sha256=IQYCuFVb9FZciOFKs5om7HAKO_wOhVM_km8vBJUrIA0,1442
-migro/migrations.py,sha256=gEfQoFG0msB47gEHvBCiM6eCtGLoXN-GNB_rdyhBPNs,3004
+migro/main.py,sha256=fWvGOT4A5EFYG6m7fsoD-Il3W-GEzoDfNJA4cfPpD7o,1901
+migro/migrations.py,sha256=j98TTvtBsGF_p4hLIa73yhm73lGAprh6AKg_Z2GT04g,3581
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/conftest.py,sha256=39PwUhVSrVDvHTuhTUYZE91894gPyjLFwHsSvvdBUw4,138
-tests/test_database.py,sha256=q5YlqWsz0bR6Q01JDHSAHGszdCMF6KW1HbumnoLkSyc,1509
-tests/test_dbt.py,sha256=rmsM1SZvuBWp5sVM4qUWrh8v1rWNejRXKKC5uzzpZhw,668
+tests/test_database.py,sha256=gmHy1obzwR5SpL_WXXE9Twv-JqQNzt9t0R4TEtOrFsY,3415
+tests/test_dbt.py,sha256=IKiWVCHvDBUgmZuoZ5MQ-Ch1ccTN9lptdtVQYHKGPPc,5592
 tests/test_jinja.py,sha256=7d4jAjUgpa5vLv1ttfSw4-uefu7_FHQqeXaTW2AnXrk,303
-tests/test_main.py,sha256=pNF9-u9l00ZyIVzFzZrKXeaikaowKykjUgdxmMnmJAI,1418
-tests/test_migrations.py,sha256=f1AfCwprS7xBTlUEsXR5WA6VIa-hfTKqm8fXlNIrZOY,2994
-migro-0.3.0.dist-info/LICENSE,sha256=iU8Cdw6sv5YFmOpHdlznB-7LLqeue5lNaxCG4DE_fYk,1068
-migro-0.3.0.dist-info/METADATA,sha256=AS1uxXxqwo5OePVhufaKm_BswVRsmnggbfJDJa2JZVs,1835
-migro-0.3.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-migro-0.3.0.dist-info/entry_points.txt,sha256=iRvWtn5NfTe8nT65yQy1EgF4BaqQwlJu7Xu_ycVlSW8,41
-migro-0.3.0.dist-info/top_level.txt,sha256=dmA0PXpRlfZYmyQ7TQnSJNtHZfP5R6E9613gDT8Vhps,12
-migro-0.3.0.dist-info/RECORD,,
+tests/test_main.py,sha256=rbd5hjXpgHdDzm3Lftd8knCnjhaBI9E0Hxy7i3nxPwY,1406
+tests/test_migrations.py,sha256=fcqWQRef07zEmKIWLBCgmVM0qHJgyF15eU3-A22iJOI,4006
+migro-0.4.0.dist-info/LICENSE,sha256=iU8Cdw6sv5YFmOpHdlznB-7LLqeue5lNaxCG4DE_fYk,1068
+migro-0.4.0.dist-info/METADATA,sha256=pdHNeUgwxvCiPDoNK5EbxLWy7-dh6P-00_PeygfTspg,3383
+migro-0.4.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+migro-0.4.0.dist-info/entry_points.txt,sha256=iRvWtn5NfTe8nT65yQy1EgF4BaqQwlJu7Xu_ycVlSW8,41
+migro-0.4.0.dist-info/top_level.txt,sha256=dmA0PXpRlfZYmyQ7TQnSJNtHZfP5R6E9613gDT8Vhps,12
+migro-0.4.0.dist-info/RECORD,,
```

