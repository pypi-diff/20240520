# Comparing `tmp/vmware_reporter-0.2.0-py3-none-any.whl.zip` & `tmp/vmware_reporter-0.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,20 @@
-Zip file size: 30713 bytes, number of entries: 19
--rw-rw-rw-  2.0 fat      336 b- defN 24-Mar-22 23:04 vmware_reporter/__init__.py
--rw-rw-rw-  2.0 fat     3154 b- defN 24-Mar-22 23:04 vmware_reporter/__main__.py
--rw-rw-rw-  2.0 fat      427 b- defN 24-Mar-22 23:26 vmware_reporter/_version.py
--rw-rw-rw-  2.0 fat    16965 b- defN 24-Mar-22 23:04 vmware_reporter/client.py
--rw-rw-rw-  2.0 fat    15901 b- defN 24-Mar-22 23:04 vmware_reporter/datastore.py
--rw-rw-rw-  2.0 fat     2392 b- defN 24-Mar-22 23:04 vmware_reporter/dump.py
--rw-rw-rw-  2.0 fat     5272 b- defN 24-Mar-22 23:04 vmware_reporter/extract.py
--rw-rw-rw-  2.0 fat     8916 b- defN 24-Mar-22 23:04 vmware_reporter/inspect.py
--rw-rw-rw-  2.0 fat     7981 b- defN 24-Mar-22 23:04 vmware_reporter/inventory.py
--rw-rw-rw-  2.0 fat     5116 b- defN 24-Mar-22 23:04 vmware_reporter/network.py
--rw-rw-rw-  2.0 fat    31730 b- defN 24-Mar-22 23:04 vmware_reporter/vm.py
--rw-rw-rw-  2.0 fat      705 b- defN 24-Mar-22 23:04 vmware_reporter/config/extractions/host.yml
--rw-rw-rw-  2.0 fat     1467 b- defN 24-Mar-22 23:04 vmware_reporter/config/extractions/vm.yml
--rw-rw-rw-  2.0 fat     1098 b- defN 24-Mar-22 23:26 vmware_reporter-0.2.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     2617 b- defN 24-Mar-22 23:26 vmware_reporter-0.2.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Mar-22 23:26 vmware_reporter-0.2.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       66 b- defN 24-Mar-22 23:26 vmware_reporter-0.2.0.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       16 b- defN 24-Mar-22 23:26 vmware_reporter-0.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1642 b- defN 24-Mar-22 23:26 vmware_reporter-0.2.0.dist-info/RECORD
-19 files, 105893 bytes uncompressed, 28009 bytes compressed:  73.5%
+Zip file size: 30911 bytes, number of entries: 18
+-rw-rw-rw-  2.0 fat    17494 b- defN 24-May-20 09:08 vmware_reporter/__init__.py
+-rw-rw-rw-  2.0 fat     3302 b- defN 24-May-20 09:08 vmware_reporter/__main__.py
+-rw-rw-rw-  2.0 fat      427 b- defN 24-May-20 15:39 vmware_reporter/_version.py
+-rw-rw-rw-  2.0 fat    17592 b- defN 24-May-20 09:08 vmware_reporter/datastore.py
+-rw-rw-rw-  2.0 fat     2482 b- defN 24-May-20 09:08 vmware_reporter/dump.py
+-rw-rw-rw-  2.0 fat     5265 b- defN 24-May-20 09:08 vmware_reporter/extract.py
+-rw-rw-rw-  2.0 fat     8916 b- defN 24-May-20 09:08 vmware_reporter/inspect.py
+-rw-rw-rw-  2.0 fat     7900 b- defN 24-May-20 09:08 vmware_reporter/inventory.py
+-rw-rw-rw-  2.0 fat     5129 b- defN 24-May-20 09:08 vmware_reporter/networking.py
+-rw-rw-rw-  2.0 fat    31721 b- defN 24-May-20 09:08 vmware_reporter/vm.py
+-rw-rw-rw-  2.0 fat      705 b- defN 24-Mar-22 23:30 vmware_reporter/config/extractions/host.yml
+-rw-rw-rw-  2.0 fat     1467 b- defN 24-Mar-22 23:30 vmware_reporter/config/extractions/vm.yml
+-rw-rw-rw-  2.0 fat     1098 b- defN 24-May-20 15:39 vmware_reporter-0.2.1.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     2602 b- defN 24-May-20 15:39 vmware_reporter-0.2.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-20 15:39 vmware_reporter-0.2.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       66 b- defN 24-May-20 15:39 vmware_reporter-0.2.1.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       16 b- defN 24-May-20 15:39 vmware_reporter-0.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1564 b- defN 24-May-20 15:39 vmware_reporter-0.2.1.dist-info/RECORD
+18 files, 107838 bytes uncompressed, 28327 bytes compressed:  73.7%
```

## zipnote {}

```diff
@@ -3,17 +3,14 @@
 
 Filename: vmware_reporter/__main__.py
 Comment: 
 
 Filename: vmware_reporter/_version.py
 Comment: 
 
-Filename: vmware_reporter/client.py
-Comment: 
-
 Filename: vmware_reporter/datastore.py
 Comment: 
 
 Filename: vmware_reporter/dump.py
 Comment: 
 
 Filename: vmware_reporter/extract.py
@@ -21,38 +18,38 @@
 
 Filename: vmware_reporter/inspect.py
 Comment: 
 
 Filename: vmware_reporter/inventory.py
 Comment: 
 
-Filename: vmware_reporter/network.py
+Filename: vmware_reporter/networking.py
 Comment: 
 
 Filename: vmware_reporter/vm.py
 Comment: 
 
 Filename: vmware_reporter/config/extractions/host.yml
 Comment: 
 
 Filename: vmware_reporter/config/extractions/vm.yml
 Comment: 
 
-Filename: vmware_reporter-0.2.0.dist-info/LICENSE.txt
+Filename: vmware_reporter-0.2.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: vmware_reporter-0.2.0.dist-info/METADATA
+Filename: vmware_reporter-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: vmware_reporter-0.2.0.dist-info/WHEEL
+Filename: vmware_reporter-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: vmware_reporter-0.2.0.dist-info/entry_points.txt
+Filename: vmware_reporter-0.2.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: vmware_reporter-0.2.0.dist-info/top_level.txt
+Filename: vmware_reporter-0.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: vmware_reporter-0.2.0.dist-info/RECORD
+Filename: vmware_reporter-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vmware_reporter/__init__.py

```diff
@@ -1,14 +1,489 @@
 from __future__ import annotations
 
+import logging
+import re
+from collections.abc import Callable, Iterator
+from configparser import ConfigParser
+from inspect import signature
+from pathlib import Path
+from typing import Literal, TypeVar, overload
+from uuid import UUID
+
+from pyVim.connect import Disconnect, SmartConnect
+from pyVmomi import vim, vmodl
+from pyVmomi.VmomiSupport import _managedDefMap
+from zut import Filters, MessageError, get_config, resolve_host
+
+import vmware_reporter
+
+from .inspect import get_obj_ref
+
 __prog__ = 'vmware-reporter'
 
 try:
     # Version generated by setuptools_scm during build
     from ._version import __version__, __version_tuple__
 except ImportError:
     __version__ = None
     __version_tuple__ = None
 
+
+T_Obj = TypeVar('T_Obj', bound=vim.ManagedEntity)
+
+
+class VCenterClient:
+    """
+    Main entry point of the library to retrieve VMWare managed objects and interact with them. 
+    """
+    def __init__(self, env: str = None, *, host: str = None, user: str = None, password: str = None, no_ssl_verify: bool = None, config: ConfigParser = None, section: str = None):
+        """
+        Create a new vCenter client.
+
+        If `host`, `user`, `password` or `no_ssl_verify` options are not provided, they are read from configuration file
+        in section `[vmware-reporter]` (or `[vmware-reporter:{name}]` if `name` is given).
+
+        :param env: An optional name to distinguish between several vCenters.
+        :param host: Host name of the vCenter.
+        :param user: Name of the vCenter user having access to the API.
+        :param password: Password of the vCenter user having access to the API.
+        """        
+        if not config:
+            config = get_config(vmware_reporter)
+        if not section:
+            section = __prog__
+        
+        if not env:
+            envs = VCenterClient.get_configured_envs(config=config, section=section)
+            if len(envs) > 1:
+                raise MessageError(f"Name of the environment / VCenter to use must be provided. Available: {', '.join(envs) if envs else 'none'}.")
+            elif len(envs) == 1:
+                env = envs[0]
+            else:
+                raise MessageError(f"No VCenter client configured.")
+        self.env = env or 'default'
+
+        full_section = section + ('' if env == 'default' else f':{env}')
+        self.host = host if host is not None else config.get(full_section, 'host')
+        self.user = user if user is not None else config.get(full_section, 'user')
+        self.password = password if password is not None else config.get(full_section, 'password')
+        self.no_ssl_verify = no_ssl_verify if no_ssl_verify is not None else config.getboolean(full_section, 'no_ssl_verify', fallback=False)
+        
+        self.logger = logging.getLogger(f'{self.__class__.__module__}.{self.__class__.__qualname__}' + ('' if env == 'default' else f'.{self.env}'))
+
+
+    #region Enter/connect and exit/close
+
+    def __enter__(self):
+        self.connect()
+        return self
+
+
+    def __exit__(self, exc_type = None, exc_value = None, exc_traceback = None):
+        self.close()
+
+
+    def connect(self):
+        addrs = resolve_host(self.host, timeout=2.0)
+        if not addrs:
+            raise ValueError(f"Cannot resolve host name \"{self.host}\"")
+        
+        addr = addrs[0]
+        self.logger.debug(f"Connect to {addr} ({self.host}) with user {self.user}")
+
+        options = {}
+        if 'httpConnectionTimeout' in signature(SmartConnect).parameters:
+            # Introduced in pyVmomi 8.0.0.1 (see https://github.com/vmware/pyvmomi/issues/627)
+            options['httpConnectionTimeout'] = 5.0
+
+        self._service_instance = SmartConnect(host=self.host, user=self.user, pwd=self.password, disableSslCertValidation=self.no_ssl_verify, **options)
+
+
+    def close(self):
+        try:
+            Disconnect(self._service_instance)
+        except AttributeError:
+            pass
+    
+
+    @property
+    def service_instance(self) -> vim.ServiceInstance:
+        try:
+            return self._service_instance
+        except AttributeError:
+            pass
+
+        self.connect()
+        return self._service_instance
+
+
+    @property
+    def service_content(self) -> vim.ServiceInstanceContent:
+        try:
+            return self._service_content
+        except AttributeError:
+            pass
+
+        self._service_content = self.service_instance.RetrieveContent()
+        return self._service_content
+
+    #endregion
+
+
+    #region Retrieve managed objects
+
+    @property
+    def datacenter(self):
+        try:
+            return self._datacenter
+        except AttributeError:
+            pass
+
+        datacenters = self.get_objs(vim.Datacenter)
+        if not datacenters:
+            raise ValueError(f"Datacenter not found")
+        if len(datacenters) > 1:
+            raise ValueError(f"Several datacenter found")
+        self._datacenter = datacenters[0]
+        return self._datacenter
+
+
+    def get_obj(self, type: type[T_Obj], search: list[str|re.Pattern]|str|re.Pattern|UUID, *, normalize: bool = False, key: Literal['name', 'ref', 'uuid', 'bios_uuid'] = 'name') -> T_Obj:
+        """
+        Find a single VMWare managed object.
+
+        Raise KeyError if not found or several found.
+        """
+        if key in ['uuid', 'bios_uuid']:
+            if not isinstance(search, (UUID,str)):
+                raise TypeError(f"specs must be UUID or str for key {key}, got {type(search).__name__}")
+            
+            if isinstance(search, UUID):
+                uuid = search
+            else:
+                uuid = UUID(search)
+
+            obj = None
+            
+            if key == 'bios_uuid':
+                # NOTE: uuid is "BIOS UUID". Seems to match the end of `sudo cat /sys/class/dmi/id/product_uuid`.
+                if type == vim.VirtualMachine:
+                    obj = self._find_by_uuid(uuid, for_vm=True, instance_uuid=False)
+                else:
+                    raise ValueError(f"key '{key}' can be used only for virtual machines")
+                
+            else:
+                if type == vim.VirtualMachine:
+                    obj = self._find_by_uuid(uuid, for_vm=True, instance_uuid=True)
+                elif type == vim.HostSystem:
+                    obj = self._find_by_uuid(uuid, for_vm=False, instance_uuid=False)
+                else:
+                    raise ValueError(f"key '{key}' can be used only for virtual machines or host systems")
+
+            if obj:
+                return obj
+            else:
+                raise KeyError(f"Not found: {search} (type: {type.__name__})")
+
+        else:
+            iterator = self.iter_objs(types=type, search=search, normalize=normalize, key=key)
+            try:
+                found = next(iterator)
+            except StopIteration:
+                raise KeyError(f"Not found: {search} (type: {type.__name__})")
+            
+            try:
+                next(iterator)
+                raise KeyError(f"Several found: {search} (type: {type.__name__})")
+            except StopIteration:
+                pass
+            return found
+            
+
+    def _find_by_uuid(self, uuid: UUID|str, for_vm: bool, instance_uuid: bool):
+        if isinstance(uuid, UUID):
+            uuid = str(uuid)
+        
+        for datacenter in self.iter_objs(vim.Datacenter):
+            obj = self.service_content.searchIndex.FindByUuid(datacenter, uuid, vmSearch=for_vm, instanceUuid=instance_uuid)
+            if obj:
+                return obj
+
+
+    @overload
+    def get_objs(self, types: type[T_Obj], search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = None, key: Literal['name', 'ref'] = 'name', sort_key: str|list[str]|Callable = None) -> list[T_Obj]:
+        ...
+
+    def get_objs(self, types: list[type|str]|type|str = None, search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = None, key: Literal['name', 'ref'] = 'name', sort_key: str|list[str]|Callable = None):        
+        """
+        List VMWare managed objects matching the given search.
+        """
+        objs = [obj for obj in self.iter_objs(types, search, normalize=normalize, key=key)]
+
+        if sort_key:
+            if isinstance(sort_key, str):
+                sort_key = [sort_key]
+
+            if isinstance(sort_key, list):
+                sort_func = lambda obj: [getattr(obj, attr) for attr in sort_key]
+            else:
+                sort_func = sort_key
+
+            objs.sort(key=sort_func)
+
+        return objs
+
+
+    @overload
+    def iter_objs(self, types: type[T_Obj], search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = None, key: Literal['name', 'ref'] = 'name') -> Iterator[T_Obj]:
+        ...
+
+    def iter_objs(self, types: list[type|str]|type|str = None, search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = None, key: Literal['name', 'ref'] = 'name'):
+        """
+        Iterate over VMWare managed objects matching the given search.
+        """
+
+        # Prepare value filter
+        filters = Filters(search, normalize=normalize)
+
+        # Prepare types
+        if not types:
+            types = []
+        elif isinstance(types, (str,type)):
+            types = [types]
+        
+        types = [self.parse_obj_type(_type) for _type in types]
+
+        # Search using a container view
+        view = None
+        try:
+            view = self.service_content.viewManager.CreateContainerView(self.service_content.rootFolder, types, recursive=True)
+
+            for obj in view.view:
+                if self._obj_matches(obj, key, filters):
+                    yield obj
+        finally:
+            if view:
+                view.Destroy()
+
+
+    def _obj_matches(self, obj: vim.ManagedEntity, key: Literal['name', 'ref'], filters: Filters):
+        if not filters:
+            return True
+        
+        if key == 'name':
+            try:
+                value = obj.name
+            except vim.fault.NoPermission:
+                return False
+            
+        elif key == 'ref':
+            value = get_obj_ref(obj)
+            
+        else:
+            raise ValueError(f"key not supported: {key}")
+        
+        return filters.matches(value)
+
+    #endregion
+
+
+    #region Instance helpers
+
+    @property
+    def cookie(self) -> dict:
+        try:
+            return self._cookie
+        except AttributeError:
+            pass
+    
+        # Get the cookie built from the current session
+        client_cookie = self.service_instance._stub.cookie
+
+        # Break apart the cookie into it's component parts
+        cookie_name = client_cookie.split("=", 1)[0]
+        cookie_value = client_cookie.split("=", 1)[1].split(";", 1)[0]
+        cookie_path = client_cookie.split("=", 1)[1].split(";", 1)[1].split(
+            ";", 1)[0].lstrip()
+        cookie_text = " " + cookie_value + "; $" + cookie_path
+
+        # Make a cookie
+        self._cookie = dict()
+        self._cookie[cookie_name] = cookie_text
+        return self._cookie
+
+
+    def wait_for_task(self, *tasks: vim.Task):
+        """
+        Given a service instance and tasks, return after all the tasks are complete.
+        """
+        property_collector = self.service_instance.content.propertyCollector
+        task_list = [str(task) for task in tasks]
+        # Create filter
+        obj_specs = [vmodl.query.PropertyCollector.ObjectSpec(obj=task) for task in tasks]
+        property_spec = vmodl.query.PropertyCollector.PropertySpec(type=vim.Task, pathSet=[], all=True)
+        filter_spec = vmodl.query.PropertyCollector.FilterSpec()
+        filter_spec.objectSet = obj_specs
+        filter_spec.propSet = [property_spec]
+        pc_filter = property_collector.CreateFilter(filter_spec, True)
+        try:
+            version, state = None, None
+            # Loop looking for updates till the state moves to a completed state.
+            while task_list:
+                update = property_collector.WaitForUpdates(version)
+                for filter_set in update.filterSet:
+                    for obj_set in filter_set.objectSet:
+                        task = obj_set.obj
+                        for change in obj_set.changeSet:
+                            if change.name == 'info':
+                                state = change.val.state
+                            elif change.name == 'info.state':
+                                state = change.val
+                            else:
+                                continue
+
+                            if not str(task) in task_list:
+                                continue
+
+                            if state == vim.TaskInfo.State.success:
+                                # Remove task from taskList
+                                task_list.remove(str(task))
+                            elif state == vim.TaskInfo.State.error:
+                                raise task.info.error
+                # Move to next version
+                version = update.version
+        finally:
+            if pc_filter:
+                pc_filter.Destroy()
+
+
+    def get_out_dir(self):
+        return Path('data' if self.env == 'default' else f'data/{self.env}')
+
+    #endregion
+
+
+    #region Class helpers
+    
+    @classmethod
+    def get_configured_envs(cls, *, config: ConfigParser = None, section: str = None):
+        if not config:
+            config = get_config(vmware_reporter)
+        if not section:
+            section = __prog__
+        
+        envs: list[str] = []
+        for _section in config.sections():
+            if m := re.match(r'^' + re.escape(section) + r'(?:\:(.+))?', _section):
+                env = m[1]
+                if env == 'default':
+                    raise ValueError(f"Invalid configuration section \"{_section}\": name \"default\" is reserved")
+                if not env:
+                    env = 'default'
+                envs.append(env)
+        return envs
+        
+    @classmethod
+    def parse_obj_type(cls, value: str|type|vim.ManagedEntity) -> type[vim.ManagedEntity]:
+        if not value:
+            raise ValueError(f"name cannot be blank")
+        
+        elif isinstance(value, type):
+            if not issubclass(value, vim.ManagedEntity):
+                raise TypeError(f"type {value} is not a subclass of vim.ManagedEntity")
+            
+            return value
+        
+        elif isinstance(value, vim.ManagedEntity):
+            return type(value)
+        
+        elif not isinstance(value, str):
+            raise TypeError(f"invalid type for name: {value}")
+        
+        else:
+            lower = value.lower()
+
+            # Search in types
+            if lower in cls.OBJ_TYPES:
+                return cls.OBJ_TYPES[lower]
+
+            # Handle aliases            
+            if lower == 'vm':
+                return vim.VirtualMachine
+            if lower == 'host':
+                return vim.HostSystem
+            if lower == 'net':
+                return vim.Network
+            if lower == 'dvs':
+                return vim.DistributedVirtualSwitch
+            if lower == 'dvp':
+                return vim.dvs.DistributedVirtualPortgroup
+            if lower == 'ds':
+                return vim.Datastore
+            if lower == 'dc':
+                return vim.Datacenter
+            if lower == 'cluster':
+                return vim.ClusterComputeResource
+
+            raise KeyError(f"vim managed object type not found for name {value}")
+
+    def _build_obj_types() -> dict[str,type[vim.ManagedEntity]]:
+        types = {}
+
+        for key in _managedDefMap.keys():
+            if not key.startswith('vim.'):
+                continue
+
+            attr = key[len('vim.'):]
+            _type = getattr(vim, attr)
+            if not issubclass(_type, vim.ManagedEntity):
+                continue
+
+            lower = attr.lower()
+            if lower in types:
+                continue
+
+            types[lower] = _type
+
+        return types
+            
+    OBJ_TYPES = _build_obj_types()
+    
+    #endregion
+
+
+    #region Retrieve network objects by key
+    
+    def get_portgroup_by_key(self, key: str) -> vim.dvs.DistributedVirtualPortgroup:
+        if key is None:
+            return None
+        
+        try:
+            by_key = self._portgroups_by_key
+        except AttributeError:
+            by_key = {}
+            for obj in self.iter_objs(vim.dvs.DistributedVirtualPortgroup):
+                by_key[obj.key] = obj
+            self._portgroups_by_key = by_key
+
+        return by_key.get(key)
+    
+    def get_switch_by_uuid(self, uuid: str) -> vim.DistributedVirtualSwitch:
+        if uuid is None:
+            return None
+        
+        try:
+            by_uuid = self._switchs_by_uuid
+        except AttributeError:
+            by_uuid = {}
+            for obj in self.iter_objs(vim.DistributedVirtualSwitch):
+                by_uuid[obj.uuid] = obj
+            self._switchs_by_uuid = by_uuid
+
+        return by_uuid.get(uuid)
+
+    #endregion
+
+
 __all__ = (
     '__prog__', '__version__', '__version_tuple__',
 )
```

## vmware_reporter/__main__.py

```diff
@@ -1,82 +1,82 @@
 """
-Extract data easily from your VMWare clusters.
+Interact easily with your VMWare clusters.
 """
+from __future__ import annotations
+from configparser import ConfigParser
 import inspect
 import logging
 import os
-import sys
-from argparse import ArgumentParser, RawTextHelpFormatter
+from argparse import ArgumentParser, RawTextHelpFormatter, _SubParsersAction
 from contextlib import nullcontext
 from types import FunctionType
 
-from zut import add_func_command, configure_logging, get_help_text, OutTable
+from zut import (OutTable, add_func_command, configure_logging, exec_command,
+                 get_help_text, register_locale)
 
-from . import __prog__, __version__
-from .client import VCenterClient
+from . import VCenterClient, __prog__, __version__
 from .datastore import add_datastore_commands
 from .dump import dump
+from .extract import handle as extract_handle
 from .inventory import export_inventory
-from .network import add_network_commands
+from .networking import add_networking_commands
 from .vm import add_vm_commands
-from .extract import handle as extract_handle
 
 logger = logging.getLogger(__name__)
 
 def main():
     configure_logging()
-    OutTable.DEFAULT_EXCEL_ATEXIT = True
+    register_locale(use_excel_csv=(os.environ.get('USE_EXCEL_CSV') or '1').lower() in ['1', 'yes', 'true', 'on'])
+    OutTable.DEFAULT_EXCEL_ATEXIT = (os.environ.get('DEFAULT_EXCEL_ATEXIT') or '1').lower() in ['1', 'yes', 'true', 'on']
+
+    parser = init_parser(__prog__, __version__, __doc__)
+
+    subparsers = parser.add_subparsers(title='Commands')
+    add_commands(subparsers)
+    
+    parse_and_exec_command(parser)
     
-    vcenter_names = VCenterClient.get_configured_names()
 
-    parser = ArgumentParser(prog=__prog__, description=get_help_text(__doc__), formatter_class=RawTextHelpFormatter, add_help=False, epilog='\n'.join(__doc__.splitlines()[2:]))
+def init_parser(prog: str = None, version: str = None, doc: str = None, *, config: ConfigParser = None, section: str = None):
+    parser = ArgumentParser(prog=prog, description=get_help_text(doc), formatter_class=RawTextHelpFormatter, add_help=False, epilog='\n'.join(doc.splitlines()[2:]))
     
+    envs = VCenterClient.get_configured_envs(config=config, section=section)
+
     group = parser.add_argument_group(title='General options')
-    group.add_argument('-e', '--vcenter', '--env', default=os.environ.get('VMWARE_DEFAULT_CLIENT'), help=f"Name of the vCenter client to use. Available: {', '.join(vcenter_names) if vcenter_names else 'none'}.")
+    group.add_argument('-e', '--env', default=os.environ.get('VMWARE_DEFAULT_ENV'), help=f"Name of the vCenter to use. Available: {', '.join(envs) if envs else 'none'}.")
     group.add_argument('-h', '--help', action='help', help=f"Show this program help message and exit.")
-    group.add_argument('--version', action='version', version=f"{__prog__} {__version__ or '?'}", help="Show version information and exit.")
+    group.add_argument('--version', action='version', version=f"{prog} {version or '?'}", help="Show version information and exit.")
 
-    subparsers = parser.add_subparsers(title='Commands')
+    return parser
+
+
+def add_commands(subparsers: _SubParsersAction[ArgumentParser]):
     add_func_command(subparsers, export_inventory, name='inventory')
     add_func_command(subparsers, dump, name='dump')
     add_func_command(subparsers, extract_handle, name='extract')
     
     add_datastore_commands(subparsers, name='datastore')
-    add_network_commands(subparsers, name='network')
+    add_networking_commands(subparsers, name='networking')
     add_vm_commands(subparsers, name='vm')
+        
 
-    args = vars(parser.parse_args())
-    handle = args.pop('handle', None)
-    if not handle:
-        logger.error(f"No command provided.")
-        sys.exit(1)
+def get_vcenter(handle: FunctionType, args: dict, *, config: ConfigParser = None, section: str = None):
+    if 'vcenter' in inspect.signature(handle).parameters:
+        env = args.pop('env', None)
+        vcenter = VCenterClient(env, config=config, section=section)
+        args['vcenter'] = vcenter    
+    else:
+        vcenter = nullcontext()
 
-    with get_vcenter_context(handle, args):
-        handle(**args)
+    return vcenter
         
 
-def get_vcenter_context(handle: FunctionType, args: dict):
-    vcenter_name = args.pop('vcenter')
-    need_vcenter = 'vcenter' in inspect.signature(handle).parameters
-
-    if need_vcenter:        
-        if not vcenter_name:
-            vcenter_names = VCenterClient.get_configured_names()
-            if len(vcenter_names) > 1:
-                logger.error(f"Name of the vCenter client to use must be provided (option --vcenter). Available: {', '.join(vcenter_names) if vcenter_names else 'none'}.")
-                sys.exit(1)
-            elif len(vcenter_names) == 1:
-                vcenter_name = vcenter_names[0]
-            elif 'vcenter' in args:
-                logger.error(f"No vCenter client configured.")
-                sys.exit(1)
-        
-        context = VCenterClient(vcenter_name)
-        args['vcenter'] = context
-    
-    else:
-        context = nullcontext()
+def parse_and_exec_command(parser: ArgumentParser, *, config: ConfigParser = None, section: str = None):    
+    args = vars(parser.parse_args())
+    handle = args.pop('handle', None)
+
+    with get_vcenter(handle, args, config=config, section=section):
+        exec_command(handle, args)
 
-    return context
 
 if __name__ == '__main__':
     main()
```

## vmware_reporter/_version.py

```diff
@@ -8,9 +8,9 @@
     VERSION_TUPLE = object
 
 version: str
 __version__: str
 __version_tuple__: VERSION_TUPLE
 version_tuple: VERSION_TUPLE
 
-__version__ = version = '0.2.0'
-__version_tuple__ = version_tuple = (0, 2, 0)
+__version__ = version = '0.2.1'
+__version_tuple__ = version_tuple = (0, 2, 1)
```

## vmware_reporter/datastore.py

```diff
@@ -2,47 +2,94 @@
 Analyze datastore files or perform operations on datastores.
 """
 from __future__ import annotations
 
 import logging
 import os
 import re
-from argparse import _SubParsersAction, ArgumentParser, RawTextHelpFormatter
+from argparse import ArgumentParser, RawTextHelpFormatter, _SubParsersAction
 from contextlib import nullcontext
 from datetime import datetime
 from http import HTTPStatus
 from io import IOBase
 from pathlib import Path
 from typing import BinaryIO
 from urllib.parse import urlencode
 
 import requests
 from pyVmomi import vim
+from zut import (Header, add_func_command, get_description_text, get_help_text,
+                 out_table)
+from zut.excel import openpyxl
 
-from .client import VCenterClient
-from .inspect import get_obj_path
-from zut import Header, add_func_command, get_help_text, get_description_text, out_table
+from . import VCenterClient
+from .inspect import get_obj_path, get_obj_ref
 
 logger = logging.getLogger(__name__)
 
 
 def add_datastore_commands(commands_subparsers: _SubParsersAction[ArgumentParser], *, name: str):
     parser = commands_subparsers.add_parser(name, help=get_help_text(__doc__), description=get_description_text(__doc__), formatter_class=RawTextHelpFormatter, add_help=False)
 
     group = parser.add_argument_group(title='Command options')
     group.add_argument('-h', '--help', action='help', help=f"Show this command help message and exit.")
 
     subparsers = parser.add_subparsers(title='Sub commands')
-    add_func_command(subparsers, export_datastore_elements, name='elements')
-    add_func_command(subparsers, export_datastore_stats, name='stats')
+    add_func_command(subparsers, list_datastores, name='list')
+    add_func_command(subparsers, analyze_datastore_elements, name='elements')
+    add_func_command(subparsers, analyze_datastore_stats, name='stats')
     add_func_command(subparsers, download_from_datastore, name='download')
     add_func_command(subparsers, upload_to_datastore, name='upload')
     add_func_command(subparsers, delete_from_datastore, name='delete')
 
 
+DEFAULT_OUT = 'datastores.xlsx#{title}' if openpyxl else 'datastores-{title}.csv'
+
+
+def list_datastores(vcenter: VCenterClient, search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = False, key: str = 'name', out: os.PathLike|IOBase = DEFAULT_OUT):
+    headers = [
+        'name',
+        'ref',
+        Header('capacity', fmt='gib'),
+        Header('freespace', fmt='gib'),
+        'url',
+        'extent',
+    ]
+
+    with out_table(out, title='datastores', dir=vcenter.get_out_dir(), headers=headers) as t:
+        for obj in vcenter.iter_objs(vim.Datastore, search, normalize=normalize, key=key):            
+            try:
+                logger.info(f"Analyze {obj.name}")
+
+                t.append([
+                    obj.name,
+                    get_obj_ref(obj),
+                    obj.info.vmfs.capacity,
+                    obj.info.freeSpace,
+                    obj.info.url,
+                    parse_extent(obj.info.vmfs.extent),
+                ])
+            
+            except Exception as err:
+                logger.exception(f"Error while analyzing {str(obj)}")
+
+def _add_arguments(parser: ArgumentParser):
+    parser.add_argument('search', nargs='*', help="Search term(s).")
+    parser.add_argument('-n', '--normalize', action='store_true', help="Normalise search term(s).")
+    parser.add_argument('-k', '--key', choices=['name', 'ref'], default='name', help="Search key (default: %(default)s).")
+    parser.add_argument('-o', '--out', default=DEFAULT_OUT, help="Output table (default: %(default)s).")
+
+list_datastores.add_arguments = _add_arguments
+
+def parse_extent(extent: list[vim.host.ScsiDisk.Partition]):
+    if extent is None:
+        return None
+    return [part.diskName + ('' if part.partition == 1 else f' (partition {part.partition})') for part in extent]
+
+
 
 def iterate_datastore_elements(vcenter: VCenterClient, obj: vim.Datastore, path: str = None, *, pattern: str = None, max_depth: int = None, with_size: bool = True, with_mtime: bool = True, with_owner: bool = True, case_sensitive: bool = False):
     """
     Iterate over datastore elements (files and directories).
     """
     if path:
         path = path.strip("/\\")
@@ -125,20 +172,20 @@
             stat.file_count += 1
         else:
             stat.other_count += 1
 
     return sorted(stats.values(), key=lambda stat: stat.path)
 
 
-def export_datastore_elements(vcenter: VCenterClient, search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = False, key: str = 'name', path: str = None, max_depth: int = None, out: os.PathLike|IOBase = None, csv: bool = None, bytes: bool = False):
+def analyze_datastore_elements(vcenter: VCenterClient, search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = False, key: str = 'name', path: str = None, max_depth: int = None, out: os.PathLike|IOBase = None, bytes: bool = False):
     """
-    Export list of datastore elements (files and directories).
+    Analyze datastore elements (files and directories).
     """
-    with out_table(out, headers=DatastoreElement.get_headers(bytes=bytes), title="datastore elements", csv=csv) as t:
-        for obj in vcenter.list_objs(vim.Datastore, search, normalize=normalize, key=key, sort_key='name'):
+    with out_table(out, headers=DatastoreElement.get_headers(bytes=bytes), title="datastore elements", dir=vcenter.get_out_dir()) as t:
+        for obj in vcenter.get_objs(vim.Datastore, search, normalize=normalize, key=key, sort_key='name'):
             logger.info(f'analyze datastore {obj.name}')
 
             try:
                 for info in sorted(iterate_datastore_elements(vcenter, obj, path=path, max_depth=max_depth), key=lambda info: info.path):
                     t.append(info.as_row())
             except:
                 logger.exception(f'cannot analyze datastore {obj.name}')
@@ -147,26 +194,25 @@
 def _add_arguments(parser: ArgumentParser):
     parser.add_argument('search', nargs='*', help="Search term(s).")
     parser.add_argument('-n', '--normalize', action='store_true', help="Normalise search term(s).")
     parser.add_argument('-k', '--key', choices=['name', 'ref'], default='name', help="Search key (default: %(default)s).")
     parser.add_argument("--path", help="Detail elements only for the given path.")
     parser.add_argument("--max-depth", type=int, help="Detail elements until the given depth (default: %(default)s).")
     parser.add_argument('-o', '--out', help="Output file (default: stdout).")
-    parser.add_argument('--csv', action="store_true", default=None, help="Force CSV output (even if out is set to stdout or stderr).")
     parser.add_argument('--bytes', action="store_true", help="Display size as bytes.")
 
-export_datastore_elements.add_arguments = _add_arguments
+analyze_datastore_elements.add_arguments = _add_arguments
 
 
-def export_datastore_stats(vcenter: VCenterClient, search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = False, key: str = 'name', path: str = None, max_depth: int = None, out: os.PathLike|IOBase = None, csv: bool = None, bytes: bool = False):
+def analyze_datastore_stats(vcenter: VCenterClient, search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = False, key: str = 'name', path: str = None, max_depth: int = None, out: os.PathLike|IOBase = None, bytes: bool = False):
     """
-    Export stats about datastore elements (files and directories).
+    Analyze stats about datastore elements (files and directories).
     """
-    with out_table(out, headers=DatastoreStat.get_headers(bytes=bytes), title="datastore elements", csv=csv) as t:
-        for obj in vcenter.list_objs(vim.Datastore, search, normalize=normalize, key=key, sort_key='name'):
+    with out_table(out, headers=DatastoreStat.get_headers(bytes=bytes), title="datastore elements", dir=vcenter.get_out_dir()) as t:
+        for obj in vcenter.get_objs(vim.Datastore, search, normalize=normalize, key=key, sort_key='name'):
             logger.info(f'analyze datastore {obj.name}')
 
             try:
                 for info in get_datastore_stats(vcenter, obj, path=path, max_depth=max_depth):
                     t.append(info.as_row())
             except:
                 logger.exception(f'cannot analyze datastore {obj.name}')
@@ -175,18 +221,17 @@
 def _add_arguments(parser: ArgumentParser):
     parser.add_argument('search', nargs='*', help="Search term(s).")
     parser.add_argument('-n', '--normalize', action='store_true', help="Normalise search term(s).")
     parser.add_argument('-k', '--key', choices=['name', 'ref'], default='name', help="Search key (default: %(default)s).")
     parser.add_argument("--path", help="Detail elements only for the given path.")
     parser.add_argument("--max-depth", type=int, default=1, help="Detail elements until the given depth (default: %(default)s).")
     parser.add_argument('-o', '--out', help="Output file (default: stdout).")
-    parser.add_argument('--csv', action="store_true", default=None, help="Force CSV output (even if out is set to stdout or stderr).")
     parser.add_argument('--bytes', action="store_true", help="Display size as bytes.")
 
-export_datastore_stats.add_arguments = _add_arguments
+analyze_datastore_stats.add_arguments = _add_arguments
 
 
 def request_datastore_resource(method: str, vcenter: VCenterClient, datastore: vim.Datastore|str, path: os.PathLike, data: BinaryIO = None):
     datastore_name = datastore.name if isinstance(datastore, vim.Datastore) else datastore
 
     if not isinstance(path, Path):
         path = Path(path)
@@ -304,15 +349,15 @@
 
     @classmethod
     def get_headers(cls, *, bytes = False):
         return [
             'datastore',
             'path',
             'nature',
-            'size' if bytes else Header('size', format='giga_bytes'),
+            'size' if bytes else Header('size', fmt='gib'),
             'mtime',
             'owner',
         ]
 
     def as_row(self):
         return [
             self.obj.name,
@@ -345,15 +390,15 @@
 
     @classmethod
     def get_headers(cls, *, bytes = False):
         return [
             'datastore',
             'path',
             'nature',
-            'size' if bytes else Header('size', format='giga_bytes'),
+            'size' if bytes else Header('size', fmt='gib'),
             'mtime',
             'owner',
             'depth',
             'dir_count',
             'file_count',
             'other_count',
         ]
```

## vmware_reporter/dump.py

```diff
@@ -3,23 +3,23 @@
 import logging
 import os
 import re
 import sys
 from argparse import ArgumentParser
 from io import IOBase
 
-from .client import VCenterClient
+from . import VCenterClient
 from .inspect import get_obj_ref, dump_obj
 
 logger = logging.getLogger(__name__)
 
-DEFAULT_OUT_MASK = VCenterClient.DEFAULT_OUT_DIR_MASK.joinpath("dumps", "{type}", "{name} ({ref}).json")
+DEFAULT_OUT = os.path.join("dumps", "{type}", "{name} ({ref}).json")
 
 
-def dump(vcenter: VCenterClient, search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = False, key: str = 'name', first: bool = False, types: list[type|str]|type|str = None, out: os.PathLike|IOBase = DEFAULT_OUT_MASK):
+def dump(vcenter: VCenterClient, search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = False, key: str = 'name', first: bool = False, types: list[type|str]|type|str = None, out: os.PathLike|IOBase = DEFAULT_OUT):
     """
     Export all available data about VMWare managed objects to JSON files.
     """
     if not out or out == 'stdout':
         out = sys.stdout
     elif out == 'stderr':
         out = sys.stderr
@@ -27,34 +27,37 @@
         if not isinstance(out, str):
             out = str(out)
         if not '{name}' in out and not '{ref}' in out:
             raise ValueError("out must contain {name} or {ref} placeholder")
 
     first_types = []
 
-    for obj in vcenter.get_objs(types, search, normalize=normalize, key=key):
+    for obj in vcenter.iter_objs(types, search, normalize=normalize, key=key):
         if first:
             if type(obj) in first_types:
                 continue
 
         name = obj.name
         ref = get_obj_ref(obj)
         
         if isinstance(out, IOBase):
             obj_out = out
         else:
-            obj_out = vcenter.compile_path_mask(out, type=type(obj).__name__, name=name, ref=ref, parent_mkdir=True)
+            obj_out = os.path.join(vcenter.get_out_dir(), str(out).format(type=type(obj).__name__, name=name, ref=ref))
+            obj_out_dir = os.path.dirname(obj_out)
+            if obj_out_dir:
+                os.makedirs(obj_out_dir, exist_ok=True)
         
         dump_obj(obj, obj_out, title=f'{name} ({ref})')
 
         if first:
             first_types.append(type(obj))
 
 def _add_arguments(parser: ArgumentParser):
     parser.add_argument('search', nargs='*', help="Search term(s).")
     parser.add_argument('-n', '--normalize', action='store_true', help="Normalise search term(s).")
     parser.add_argument('-k', '--key', choices=['name', 'ref'], default='name', help="Search key (default: %(default)s).")
     parser.add_argument('-t', '--type', dest='types', metavar='type', help="Managed object type name (example: datastore).")
     parser.add_argument('--first', action='store_true', help="Only handle the first object found for each type.")
-    parser.add_argument('-o', '--out', default=DEFAULT_OUT_MASK, help="Output JSON file (default: %(default)s).")
+    parser.add_argument('-o', '--out', default=DEFAULT_OUT, help="Output JSON file (default: %(default)s).")
 
 dump.add_arguments = _add_arguments
```

## vmware_reporter/extract.py

```diff
@@ -7,27 +7,27 @@
 
 from pyVmomi import vim
 
 from zut import out_table, Literal, get_config_paths
 from reporter_utils.extractions import Extraction, get_extractions
 
 import vmware_reporter
-from .client import VCenterClient
+from . import VCenterClient
 from .inspect import dictify_value, dictify_obj, get_obj_path, get_obj_ref
 from .vm import extract_disks, extract_nics
 
 logger = logging.getLogger(__name__)
 
 class VMWareExtraction(Extraction):
     def __init__(self, *args, vcenter: VCenterClient, **kwargs):
         super().__init__(*args, **kwargs)
         self.vcenter = vcenter
 
     def get_objs(self, search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = False, key: str = 'name'):
-        return self.vcenter.list_objs(self.type, search, normalize=normalize, key=key)
+        return self.vcenter.get_objs(self.type, search, normalize=normalize, key=key)
         
     def get_obj_name_or_ignore_reason(self, obj: vim.ManagedEntity):
         try:
             return obj.name, None
         except vim.fault.NoPermission:
             return get_obj_ref(obj), "no permission"
```

## vmware_reporter/inspect.py

```diff
@@ -265,10 +265,10 @@
     if isinstance(obj_out, IOBase):
         out_name = getattr(obj_out, 'name', '<io>')
     else:
         out_name = str(obj_out)
 
     data = dictify_obj(obj)
 
-    logger.info(f"export {title} to {out_name}")
+    logger.info(f"Export {title} to {out_name}")
     with nullcontext(obj_out) if isinstance(obj_out, IOBase) else open(obj_out, 'w', encoding='utf-8') as fp:
         json.dump(data, fp=fp, indent=4, cls=ExtendedJSONEncoder, ensure_ascii=False)
```

## vmware_reporter/inventory.py

```diff
@@ -5,52 +5,52 @@
 import sys
 from argparse import ArgumentParser
 from contextlib import nullcontext
 from io import IOBase
 
 from pyVmomi import vim
 
-from .client import VCenterClient
+from . import VCenterClient
 from .inspect import get_obj_ref
 
 logger = logging.getLogger(__name__)
 
-DEFAULT_OUT_MASK = VCenterClient.DEFAULT_OUT_DIR_MASK.joinpath("inventory.yml")
+DEFAULT_OUT = "inventory.yml"
 
 
-def export_inventory(vcenter: VCenterClient, assets: list[str] = None, out: os.PathLike|IOBase = DEFAULT_OUT_MASK):
+def export_inventory(vcenter: VCenterClient, assets: list[str] = None, out: os.PathLike|IOBase = DEFAULT_OUT):
     """
     Export inventory of VMWare managed objects to a YAML file.
     """
     inventory = build_inventory(vcenter, assets=assets)
     
     if not out or out == 'stdout':
         out = sys.stdout
     elif out == 'stderr':
         out = sys.stderr
 
     if isinstance(out, IOBase):
         out_name = getattr(out, 'name', '<io>')
     else:
-        out = vcenter.compile_path_mask(out, parent_mkdir=True)
+        out = os.path.join(vcenter.get_out_dir(), out)
         out_name = str(out)
         
     logger.info(f"export inventory to {out_name}")
     inventory.to_yaml(out)
 
 
 def _add_arguments(parser: ArgumentParser):
-    parser.add_argument('-o', '--out', default=DEFAULT_OUT_MASK, help="Output YAML file (default: %(default)s).")
+    parser.add_argument('-o', '--out', default=DEFAULT_OUT, help="Output YAML file (default: %(default)s).")
     parser.add_argument('--asset', nargs='*', dest='assets')
 
 export_inventory.add_arguments = _add_arguments
 
 
 def build_inventory(vcenter: VCenterClient, assets: list[str] = None) -> InventoryNode:
-    node = InventoryNode(vcenter.name, nature=VCenterClient)
+    node = InventoryNode(vcenter.env, nature=VCenterClient)
 
     if not assets:
         assets = ['folder', 'license', 'authorization']
 
     for asset in assets:
         if asset == 'folder':
             logger.info(f"build folder inventory")
@@ -205,11 +205,11 @@
         for name, value in self.attrs.items():
             result += (', ' if need_comma else ' ') + f'{name}={value}'
             need_comma = True
 
         return result
 
     def to_yaml(self, file, depth = 0):
-        with open(file, 'w', encoding='utf-8') if isinstance(file, os.PathLike) else nullcontext(file) as fp:
+        with nullcontext(file) if isinstance(file, IOBase) else open(file, 'w', encoding='utf-8') as fp:
             print(f"{' ' * self.indent_size * depth + '- ' if depth > 0 else ''}{self}:", file=fp)
             for child in self.children:
                 child.to_yaml(fp, depth+1)
```

## vmware_reporter/vm.py

```diff
@@ -1,48 +1,50 @@
 """
 Analyze VM disks or NICs.
 """
 from __future__ import annotations
 
 import logging
-from argparse import _SubParsersAction, ArgumentParser, RawTextHelpFormatter
-from pathlib import Path
 import re
+from argparse import ArgumentParser, RawTextHelpFormatter, _SubParsersAction
+from pathlib import Path
 from typing import Literal
 
 from pyVmomi import vim
-from zut import Header, out_table, gigi_bytes, get_help_text, get_description_text, add_func_command
+from zut import (Header, add_func_command, get_description_text, get_help_text,
+                 gigi_bytes, out_table)
 from zut.excel import openpyxl
 
-from .client import VCenterClient
+from . import VCenterClient
 from .inspect import dictify_obj, dictify_value, get_obj_ref
 
 logger = logging.getLogger(__name__)
 
 def add_vm_commands(commands_subparsers: _SubParsersAction[ArgumentParser], *, name: str):
     parser = commands_subparsers.add_parser(name, help=get_help_text(__doc__), description=get_description_text(__doc__), formatter_class=RawTextHelpFormatter, add_help=False)
 
     group = parser.add_argument_group(title='Command options')
     group.add_argument('-h', '--help', action='help', help=f"Show this command help message and exit.")
 
     subparsers = parser.add_subparsers(title='Sub commands')
+    #TODO add_func_command(subparsers, list_vms, name='list')
     add_func_command(subparsers, analyze_disks, name='disks')
     add_func_command(subparsers, analyze_nics, name='nics')
 
 
-#region Disks
+DEFAULT_OUT = 'vms.xlsx#{title}' if openpyxl else 'vms-{title}.csv'
 
-DEFAULT_DISKS_OUT = VCenterClient.DEFAULT_OUT_DIR_MASK.joinpath('disks.xlsx#{title}' if openpyxl else 'disks-{title}.csv')
 
+#region Disks
 
-def analyze_disks(vcenter: VCenterClient, search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = False, key: str = 'name', out: str = DEFAULT_DISKS_OUT, top: int = None):
+def analyze_disks(vcenter: VCenterClient, search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = False, key: str = 'name', out: str = DEFAULT_OUT, top: int = None):
     """
     Analyze VM disks.
     """
-    vms_headers = [
+    disks_per_vm_headers = [
         'vm',
         'power_state',
         'os_info',
         'os_family',
         'os_name',
         'device_disks',
         'guest_disks',
@@ -57,15 +59,15 @@
         Header('mapped_guests_freespace', fmt='gib'),
         Header('unmapped_disks_capacity', fmt='gib'),
         Header('unmapped_guests_capacity', fmt='gib'),
         Header('unmapped_guests_freespace', fmt='gib'),
         'issues',
     ]
 
-    details_headers = [
+    disks_headers = [
         'vm',
         'power_state',
         'os_info',
         'os_family',
         'os_name',
         'key',
         'backing',
@@ -79,18 +81,18 @@
         'mapping',
         'guests',
         Header('guests_capacity', fmt='gib'),
         Header('guests_freespace', fmt='gib'),
         'capacity_loss_pct',
     ]
     
-    with (out_table(out, title='details', vcenter=vcenter.name, headers=details_headers) as t_details,
-          out_table(out, title='vms', vcenter=vcenter.name, headers=vms_headers) as t_vms):
+    with (out_table(out, title='disks', headers=disks_headers, dir=vcenter.get_out_dir()) as t_disks,
+          out_table(out, title='disks_per_vm', headers=disks_per_vm_headers, dir=vcenter.get_out_dir()) as t_disks_per_vm):
         
-        for i, vm in enumerate(vcenter.get_objs(vim.VirtualMachine, search, normalize=normalize, key=key)):
+        for i, vm in enumerate(vcenter.iter_objs(vim.VirtualMachine, search, normalize=normalize, key=key)):
             if top is not None and i == top:
                 break
             
             try:
                 logger.info(f"Analyze {vm.name} disks")
 
                 info = extract_disks(vm)
@@ -102,15 +104,15 @@
                 os_name = os.get('prettyName')
 
                 mapped_guests: list[vim.vm.GuestInfo.DiskInfo] = []
                 for disk in info.disks:
                     for guest in disk.guests:
                         mapped_guests.append(guest)
 
-                t_vms.append([
+                t_disks_per_vm.append([
                     vm.name, # vm
                     vm.runtime.powerState, # power_state
                     vm.config.guestFullName, # os_info
                     os_family, # os_family
                     os_name, # os_name
                     len(info.disks), # 'device_disks',
                     len(mapped_guests) + len(info.unmapped_guests), # 'guest_disks',
@@ -138,15 +140,15 @@
                     fileName = device_backing.pop('fileName', None)
                     diskMode = device_backing.pop('diskMode', None)
                     sharing = device_backing.pop('sharing', None)
 
                     capacity_loss = disk.capacity - disk.guests_capacity if disk.guests else None
                     capacity_loss_pct = 100 * capacity_loss / disk.capacity if disk.guests else None
                     
-                    t_details.append([
+                    t_disks.append([
                         vm.name, # vm
                         vm.runtime.powerState, # power_state
                         vm.config.guestFullName, # os_info
                         os_family, # os_family
                         os_name, # os_name
                         disk.device.key, # key
                         backing_typename, # backing
@@ -161,15 +163,15 @@
                         sorted(f'{guest.diskPath} ({guest.filesystemType})' if guest.filesystemType else guest.diskPath for guest in disk.guests), # guests
                         disk.guests_capacity if disk.guests else None,
                         disk.guests_freespace if disk.guests else None,
                         capacity_loss_pct,
                     ])
 
                 for guest in [*info.unmapped_guests, *info.ignored_guests]:
-                    t_details.append([
+                    t_disks.append([
                         vm.name, # vm
                         vm.runtime.powerState, # power_state
                         vm.config.guestFullName, # os_info
                         os_family, # os_family
                         os_name, # os_name
                         None, # key
                         guest.mappings, # backing
@@ -192,15 +194,15 @@
 
 
 def _add_arguments(parser: ArgumentParser):
     parser.add_argument('search', nargs='*', help="Search term(s).")
     parser.add_argument('-n', '--normalize', action='store_true', help="Normalise search term(s).")
     parser.add_argument('-k', '--key', choices=['name', 'ref'], default='name', help="Search key (default: %(default)s).")
     parser.add_argument('--top', type=int)
-    parser.add_argument('-o', '--out', default=DEFAULT_DISKS_OUT, help="Output Excel or CSV file (default: %(default)s).")
+    parser.add_argument('-o', '--out', default=DEFAULT_OUT, help="Output Excel or CSV file (default: %(default)s).")
 
 analyze_disks.add_arguments = _add_arguments
 
 
 def extract_disks(vm: vim.VirtualMachine):
     info = VmDisks(vm)
 
@@ -462,55 +464,52 @@
         return data
 
 #endregion
 
 
 #region NICs
 
-DEFAULT_NICS_OUT = VCenterClient.DEFAULT_OUT_DIR_MASK.joinpath('nics.xlsx#{title}' if openpyxl else 'nics-{title}.csv')
-
-
-def analyze_nics(vcenter: VCenterClient, search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = False, key: str = 'name', out: str = DEFAULT_NICS_OUT, top: int = None):
+def analyze_nics(vcenter: VCenterClient, search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = False, key: str = 'name', out: str = DEFAULT_OUT, top: int = None):
     """
     Analyze VM network interfaces.
     """
-    vms_headers = [
+    nics_per_vm_headers = [
         'vm',
         'power_state',
         'os_info',
         'os_family',
         'os_name',
         'device_networks',
         'guest_networks',
         'with_mappings',
         'without_mappings',
         'mapped_guest',
         'unmapped_guest',
         'issues',
     ]
 
-    details_headers = [
+    nics_headers = [
         'vm',
         'power_state',
         'os_info',
         'os_family',
         'os_name',
         'backing',
         'network',
         'address_type',
         'key',
         'mac',
         'guests_ips',
         'guests_network_name',
     ]
     
-    with (out_table(out, title='details', vcenter=vcenter.name, headers=details_headers) as t_details,
-          out_table(out, title='vms', vcenter=vcenter.name, headers=vms_headers) as t_vms):
+    with (out_table(out, title='nics', headers=nics_headers, dir=vcenter.get_out_dir()) as t_nics,
+          out_table(out, title='nics_per_vm', headers=nics_per_vm_headers, dir=vcenter.get_out_dir()) as t_nics_per_vm):
         
-        for i, vm in enumerate(vcenter.get_objs(vim.VirtualMachine, search, normalize=normalize, key=key)):
+        for i, vm in enumerate(vcenter.iter_objs(vim.VirtualMachine, search, normalize=normalize, key=key)):
             if top is not None and i == top:
                 break
             
             try:
                 logger.info(f"Analyze {vm.name} nics")
 
                 info = extract_nics(vm, vcenter=vcenter)
@@ -522,15 +521,15 @@
                 os_name = os.get('prettyName')
 
                 mapped_guests: list[vim.vm.GuestInfo.NicInfo] = []
                 for nic in info.nics:
                     for guest in nic.guests:
                         mapped_guests.append(guest)
 
-                t_vms.append([
+                t_nics_per_vm.append([
                     vm.name, # vm
                     vm.runtime.powerState, # power_state
                     vm.config.guestFullName, # os_info
                     os_family, # os_family
                     os_name, # os_name
                     len(info.nics), # 'device_networks',
                     len(mapped_guests) + len(info.unmapped_guests), # 'guest_networks',
@@ -566,15 +565,15 @@
                     ip_addresses = []
                     networks = []
                     for guest in nic.guests:
                         for ip in guest.ipAddress:
                             ip_addresses.append(ip)
                         networks.append(guest.network)
                     
-                    t_details.append([
+                    t_nics.append([
                         vm.name, # vm
                         vm.runtime.powerState, # power_state
                         vm.config.guestFullName, # os_info
                         os_family, # os_family
                         os_name, # os_name
                         backing_typename, # backing
                         network,
@@ -582,15 +581,15 @@
                         nic.device.key, # key
                         nic.device.macAddress.lower(), # mac
                         ip_addresses,
                         networks,
                     ])
 
                 for guest in info.unmapped_guests:
-                    t_details.append([
+                    t_nics.append([
                         vm.name, # vm
                         vm.runtime.powerState, # power_state
                         vm.config.guestFullName, # os_info
                         os_family, # os_family
                         os_name, # os_name
                         None, # backing
                         None, # network
@@ -606,15 +605,15 @@
 
 
 def _add_arguments(parser: ArgumentParser):
     parser.add_argument('search', nargs='*', help="Search term(s).")
     parser.add_argument('-n', '--normalize', action='store_true', help="Normalise search term(s).")
     parser.add_argument('-k', '--key', choices=['name', 'ref'], default='name', help="Search key (default: %(default)s).")
     parser.add_argument('--top', type=int)
-    parser.add_argument('-o', '--out', default=DEFAULT_NICS_OUT, help="Output Excel or CSV file (default: %(default)s).")
+    parser.add_argument('-o', '--out', default=DEFAULT_OUT, help="Output Excel or CSV file (default: %(default)s).")
 
 analyze_nics.add_arguments = _add_arguments
 
 
 def extract_nics(vm: vim.VirtualMachine, *, vcenter: VCenterClient):
     info = VmNics(vm)
 
@@ -735,15 +734,15 @@
         if isinstance(self.device.backing, vim.vm.device.VirtualEthernetCard.DistributedVirtualPortBackingInfo):
             connection_obj = self.device.backing.port
             network_obj = self.vcenter.get_portgroup_by_key(connection_obj.portgroupKey)
             if network_obj:
                 return network_obj
             else:
                 switch_obj = self.vcenter.get_switch_by_uuid(connection_obj.switchUuid)
-                port_key = int(connection_obj.portKey) if re.match(r'^\d+$', connection_obj.portKey) else connection_obj.portKey
+                port_key = int(connection_obj.portKey) if connection_obj.portKey is not None and re.match(r'^\d+$', connection_obj.portKey) else connection_obj.portKey
                 if switch_obj:
                     return {'switch': switch_obj, 'port': port_key}
                 else:
                     return {'switch_uuid': connection_obj.switchUuid, 'port': port_key}
         elif isinstance(self.device.backing, vim.vm.device.VirtualEthernetCard.NetworkBackingInfo):
             return self.device.backing.network
         else:
```

## Comparing `vmware_reporter/network.py` & `vmware_reporter/networking.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,42 +8,42 @@
 import re
 from argparse import ArgumentParser, _SubParsersAction
 
 from pyVmomi import vim
 from zut import add_func_command, out_table
 from zut.excel import openpyxl
 
-from .client import VCenterClient
+from . import VCenterClient
 from .inspect import get_obj_ref
 
 
-def add_network_commands(commands_subparsers: _SubParsersAction[ArgumentParser], *, name: str):
+def add_networking_commands(commands_subparsers: _SubParsersAction[ArgumentParser], *, name: str):
     add_func_command(commands_subparsers, analyze_networks, name=name, doc=__doc__)
 
 
-DEFAULT_NETWORKS_OUT = VCenterClient.DEFAULT_OUT_DIR_MASK.joinpath('networks.xlsx#{title}' if openpyxl else 'networks-{title}.csv')
+DEFAULT_OUT = 'networking.xlsx#{title}' if openpyxl else 'networking-{title}.csv'
 
-def analyze_networks(vcenter: VCenterClient, *, out: str = DEFAULT_NETWORKS_OUT):
-    with out_table(out, title='switchs', vcenter=vcenter.name) as t:
-        for obj in vcenter.get_objs(vim.DistributedVirtualSwitch):
+def analyze_networks(vcenter: VCenterClient, *, out: str = DEFAULT_OUT):
+    with out_table(out, title='switchs', dir=vcenter.get_out_dir()) as t:
+        for obj in vcenter.iter_objs(vim.DistributedVirtualSwitch):
             uplinks = []
             for portgroup in obj.config.uplinkPortgroup:
                 uplink = portgroup.name
                 uplinks.append(uplink)
 
             t.append({
                 'ref': get_obj_ref(obj),
                 'name': obj.name,
                 'uuid': obj.uuid,
                 'uplinks': uplinks,
                 'default_vlan': _vlan_repr(obj.config.defaultPortConfig.vlan),
             })
 
-    with out_table(out, title='networks', vcenter=vcenter.name) as t:
-        for obj in sorted(vcenter.get_objs(vim.Network), key=_network_sortkey):
+    with out_table(out, title='networks', dir=vcenter.get_out_dir()) as t:
+        for obj in sorted(vcenter.iter_objs(vim.Network), key=_network_sortkey):
             if isinstance(obj, vim.dvs.DistributedVirtualPortgroup):
                 typename = 'DVP'
                 switch = obj.config.distributedVirtualSwitch.name
                 vlan = obj.config.defaultPortConfig.vlan
                 ports = f'{obj.config.numPorts}: ' + ','.join(_get_portkey_ranges(obj.portKeys))
             elif isinstance(obj, vim.Network):
                 typename = 'Network'
@@ -63,28 +63,30 @@
                 'switch': switch,
                 'ports': ports,
                 'default_vlan': _vlan_repr(vlan),
             })
 
 
 def _add_arguments(parser: ArgumentParser):
-    parser.add_argument('-o', '--out', default=DEFAULT_NETWORKS_OUT, help="Output Excel or CSV file (default: %(default)s).")
+    parser.add_argument('-o', '--out', default=DEFAULT_OUT, help="Output Excel or CSV file (default: %(default)s).")
 
 analyze_networks.add_arguments = _add_arguments
 
 
 def _network_sortkey(obj: vim.Network):
     if isinstance(obj, vim.dvs.DistributedVirtualPortgroup):
         minkey = None
         for key in obj.portKeys:
-            if re.match(r'^\d+$', key):
+            if key is not None and re.match(r'^\d+$', key):
                 key = int(key)
                 if minkey is None or key < minkey:
                     minkey = key
 
+        if minkey is None:
+            minkey = 0
         return (1, obj.config.distributedVirtualSwitch.name, minkey ,obj.name)
 
     else:
         return (2, obj.name)
 
 
 def _vlan_repr(vlan: vim.dvs.VmwareDistributedVirtualSwitch.VlanIdSpec|vim.dvs.VmwareDistributedVirtualSwitch.TrunkVlanSpec) -> int|str:
```

## Comparing `vmware_reporter-0.2.0.dist-info/LICENSE.txt` & `vmware_reporter-0.2.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `vmware_reporter-0.2.0.dist-info/METADATA` & `vmware_reporter-0.2.1.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: vmware-reporter
-Version: 0.2.0
-Summary: Extract data easily from your VMWare clusters.
+Version: 0.2.1
+Summary: Interact easily with your VMWare clusters.
 Author-email: Sébastien Hocquet <dev@ipamo.net>
 Project-URL: Homepage, https://github.com/ipamo/vmware-reporter
 Project-URL: Bug Tracker, https://github.com/ipamo/vmware-reporter/issues
 Keywords: vmware,vsphere,vm,reporter
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,15 +18,15 @@
 Requires-Dist: reporter-utils
 Requires-Dist: pyvmomi
 Requires-Dist: requests
 
 VMWare-reporter
 ===============
 
-Extract data easily from your VMWare clusters.
+Interact easily with your VMWare clusters.
 
 
 ## Installation
 
 VMWare-reporter package is published [on PyPI](https://pypi.org/project/vmware-reporter/):
 
 ```sh
@@ -50,15 +50,15 @@
 ## Usage examples
 
 See also [full documentation](https://ipamo.net/vmware-reporter) (including [API reference](https://ipamo.net/vmware-reporter/latest/api-reference.html)).
 
 VMWare-reporter may be used as a library in your Python code:
 
 ```py
-from vmware_reporter.client import VCenterClient
+from vmware_reporter import VCenterClient
 with VCenterClient() as vcenter:
     for vm in vcenter.iterate_objs('vm'):
         print(vm.name)
 ```
 
 VMWare-reporter may also be invoked as a command-line application (the `vmware-reporter` executable is installed with the package). Examples:
```

## Comparing `vmware_reporter-0.2.0.dist-info/RECORD` & `vmware_reporter-0.2.1.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-vmware_reporter/__init__.py,sha256=b8MIpvOjW-k9HksMbjgYmMVqFsij4zmxv4hrSXt7ZOs,336
-vmware_reporter/__main__.py,sha256=jZxx0pgzjqci40dVhtYVBb3hgC5VakygOc08f8XSQZs,3154
-vmware_reporter/_version.py,sha256=dwm-k_Z-jVJh3XvUUihA4YH_iqS5EfkubVd6suUFZB0,427
-vmware_reporter/client.py,sha256=ZbYU7LAVg6q82XSGubiTnW11c992T3prWejGy3NV9rc,16965
-vmware_reporter/datastore.py,sha256=4xM_s_363panCabPE2-mvdWeoCZ6UMRZHUScPB1Z-8Q,15901
-vmware_reporter/dump.py,sha256=HmLP1sSS44IuiIBTAHyCTAKE-mCMDD8PhiV0aIDHtS8,2392
-vmware_reporter/extract.py,sha256=jmk7FKg967wzWoOcvyELXiCO4J5l2-vLh33T_Z0-17g,5272
-vmware_reporter/inspect.py,sha256=H-P3dW8WFI-0DqIBXZ1KBk0vT3PVtYNS9DXdK0hgSaU,8916
-vmware_reporter/inventory.py,sha256=qgrMTjbQBtvnKxXqFkYI178sjxO8dAsINsTyUnnElrQ,7981
-vmware_reporter/network.py,sha256=kGpImZctSEWRgi5K24MSv0G2ORebytn5mKVSj2edqHg,5116
-vmware_reporter/vm.py,sha256=_W8QCF-lHLjw0T_eUgeltps1LJLV3kXG9lkxulotXZI,31730
+vmware_reporter/__init__.py,sha256=CRiHWqdhR6L0AVO9oiHHq1eK-J7J6KfCajHDEu4Hnkg,17494
+vmware_reporter/__main__.py,sha256=sa0IIK20o46T8AtiH6Hk3BIP6BQ0mn45DVjxAMox1c8,3302
+vmware_reporter/_version.py,sha256=ZX5om7Ovkz6dOhGLYm2Tr_wCABow6rirLhSHdYiHgpk,427
+vmware_reporter/datastore.py,sha256=gfNgh56wsPIP3YRU0wujN44pgYJwGpvjNMGrOYiSjIs,17592
+vmware_reporter/dump.py,sha256=jxLKRSNiYwt2Y4KDYLZ-E0Msdrxo5P49xmSI1UhtOe8,2482
+vmware_reporter/extract.py,sha256=8vQiYmdIOgAS0mosmQ3lv2kvdX_MJVjcBQsEH4gCpUY,5265
+vmware_reporter/inspect.py,sha256=zui_U7u9w0t3Jmf6SJSuqrNXOZDEEKNDhOvGiFaaZOI,8916
+vmware_reporter/inventory.py,sha256=6cF4StyNkqYPPJGeZAQ-x_8oSgo1SabXb2b8T9DP3qU,7900
+vmware_reporter/networking.py,sha256=uReP1HvWBKbKoEn5mX-Smtt-U9uVlxw6Nycvcubbz0M,5129
+vmware_reporter/vm.py,sha256=57R-gchEh5Axy0gm9oA2dlfwY_v1z_CBg4PMVPHwjdg,31721
 vmware_reporter/config/extractions/host.yml,sha256=yMXT4cJru1a84rqLYOTT6EpcreNmY_ukTKbtIv5xneo,705
 vmware_reporter/config/extractions/vm.yml,sha256=dUU89TGM3eEumVYtbYITMcQq-t_ZgojgOPnrrRLm3vM,1467
-vmware_reporter-0.2.0.dist-info/LICENSE.txt,sha256=GIOy7i81R9zaxGmerWRrvgsSukOj10VspxRwsEWtlCY,1098
-vmware_reporter-0.2.0.dist-info/METADATA,sha256=IRxhrdjq8l83MWoZrXrAdGpraiyU7e5IQWn6WV4tQu4,2617
-vmware_reporter-0.2.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-vmware_reporter-0.2.0.dist-info/entry_points.txt,sha256=Sd7R6PmUzLkJr4eez7nM8-z6yISX2pb3Dc8mnXDuguM,66
-vmware_reporter-0.2.0.dist-info/top_level.txt,sha256=uBrhSJjB5QxsyeQKqRdCv8l6JOmXKhnfPKnetEEAqso,16
-vmware_reporter-0.2.0.dist-info/RECORD,,
+vmware_reporter-0.2.1.dist-info/LICENSE.txt,sha256=GIOy7i81R9zaxGmerWRrvgsSukOj10VspxRwsEWtlCY,1098
+vmware_reporter-0.2.1.dist-info/METADATA,sha256=kaVLbZRTN5RB-p4HM4TtHC7CZX4wHStpsVkoebY0GX8,2602
+vmware_reporter-0.2.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+vmware_reporter-0.2.1.dist-info/entry_points.txt,sha256=Sd7R6PmUzLkJr4eez7nM8-z6yISX2pb3Dc8mnXDuguM,66
+vmware_reporter-0.2.1.dist-info/top_level.txt,sha256=uBrhSJjB5QxsyeQKqRdCv8l6JOmXKhnfPKnetEEAqso,16
+vmware_reporter-0.2.1.dist-info/RECORD,,
```

