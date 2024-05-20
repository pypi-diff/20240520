# Comparing `tmp/m3-users-3.0.1.tar.gz` & `tmp/m3-users-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/m3-users-3.0.1.tar", last modified: Thu Feb 26 13:23:29 2015, max compression
+gzip compressed data, was "dist/m3-users-3.0.2.tar", last modified: Thu Mar  5 05:25:00 2015, max compression
```

## Comparing `m3-users-3.0.1.tar` & `m3-users-3.0.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 babay     (1000) babay     (1000)        0 2015-02-26 13:23:29.000000 m3-users-3.0.1/
--rw-r--r--   0 babay     (1000) babay     (1000)       23 2015-02-26 12:58:58.000000 m3-users-3.0.1/README.txt
--rw-r--r--   0 babay     (1000) babay     (1000)      925 2015-02-26 13:19:32.000000 m3-users-3.0.1/setup.py
--rw-r--r--   0 babay     (1000) babay     (1000)        9 2015-02-26 12:58:58.000000 m3-users-3.0.1/MANIFEST.in
--rw-r--r--   0 babay     (1000) babay     (1000)      617 2015-02-26 13:23:29.000000 m3-users-3.0.1/PKG-INFO
-drwxr-xr-x   0 babay     (1000) babay     (1000)        0 2015-02-26 13:23:29.000000 m3-users-3.0.1/src/
-drwxr-xr-x   0 babay     (1000) babay     (1000)        0 2015-02-26 13:23:29.000000 m3-users-3.0.1/src/m3_users/
--rw-r--r--   0 babay     (1000) babay     (1000)     2721 2015-02-26 13:02:24.000000 m3-users-3.0.1/src/m3_users/app_meta.py
--rw-r--r--   0 babay     (1000) babay     (1000)     3785 2015-02-26 13:02:24.000000 m3-users-3.0.1/src/m3_users/api.py
--rw-r--r--   0 babay     (1000) babay     (1000)     3535 2015-02-26 13:02:24.000000 m3-users-3.0.1/src/m3_users/models.py
--rw-r--r--   0 babay     (1000) babay     (1000)      281 2015-02-26 13:02:24.000000 m3-users-3.0.1/src/m3_users/__init__.py
--rw-r--r--   0 babay     (1000) babay     (1000)     3052 2015-02-26 13:02:24.000000 m3-users-3.0.1/src/m3_users/helpers.py
--rw-r--r--   0 babay     (1000) babay     (1000)      111 2015-02-26 13:02:24.000000 m3-users-3.0.1/src/m3_users/version.py
--rw-r--r--   0 babay     (1000) babay     (1000)     3153 2015-02-26 13:02:24.000000 m3-users-3.0.1/src/m3_users/permissions.py
-drwxr-xr-x   0 babay     (1000) babay     (1000)        0 2015-02-26 13:23:29.000000 m3-users-3.0.1/src/m3_users/migrations/
--rw-r--r--   0 babay     (1000) babay     (1000)        0 2015-02-26 12:58:58.000000 m3-users-3.0.1/src/m3_users/migrations/__init__.py
--rw-r--r--   0 babay     (1000) babay     (1000)     6619 2015-02-26 12:58:58.000000 m3-users-3.0.1/src/m3_users/migrations/0001_initial.py
-drwxr-xr-x   0 babay     (1000) babay     (1000)        0 2015-02-26 13:23:29.000000 m3-users-3.0.1/src/m3_users/templates/
-drwxr-xr-x   0 babay     (1000) babay     (1000)        0 2015-02-26 13:23:29.000000 m3-users-3.0.1/src/m3_users/templates/m3-users/
--rw-r--r--   0 babay     (1000) babay     (1000)     1710 2015-02-26 13:02:24.000000 m3-users-3.0.1/src/m3_users/templates/m3-users/edit-role-window.js
--rw-r--r--   0 babay     (1000) babay     (1000)     2045 2015-02-26 13:02:24.000000 m3-users-3.0.1/src/m3_users/templates/m3-users/roles-list-window.js
--rw-r--r--   0 babay     (1000) babay     (1000)     1862 2015-02-26 13:02:24.000000 m3-users-3.0.1/src/m3_users/templates/m3-users/select-users-window.js
--rw-r--r--   0 babay     (1000) babay     (1000)     7461 2015-02-26 13:02:24.000000 m3-users-3.0.1/src/m3_users/metaroles.py
--rw-r--r--   0 babay     (1000) babay     (1000)    40132 2015-02-26 13:02:24.000000 m3-users-3.0.1/src/m3_users/roles.py
--rw-r--r--   0 babay     (1000) babay     (1000)     2335 2015-02-26 13:02:24.000000 m3-users-3.0.1/src/m3_users/users.py
--rw-r--r--   0 babay     (1000) babay     (1000)        0 2015-02-26 12:58:58.000000 m3-users-3.0.1/src/requires.txt
-drwxr-xr-x   0 babay     (1000) babay     (1000)        0 2015-02-26 13:23:29.000000 m3-users-3.0.1/src/tests/
--rw-r--r--   0 babay     (1000) babay     (1000)      656 2015-02-26 12:58:58.000000 m3-users-3.0.1/src/tests/urls.py
--rwxr-xr-x   0 babay     (1000) babay     (1000)      779 2015-02-26 12:58:58.000000 m3-users-3.0.1/src/tests/manage.py
--rw-r--r--   0 babay     (1000) babay     (1000)    13515 2015-02-26 12:58:58.000000 m3-users-3.0.1/src/tests/prepare_env.py
--rw-r--r--   0 babay     (1000) babay     (1000)     4124 2015-02-26 12:58:58.000000 m3-users-3.0.1/src/tests/settings.py
--rw-r--r--   0 babay     (1000) babay     (1000)      436 2015-02-26 12:58:58.000000 m3-users-3.0.1/src/tests/__init__.py
--rwxr-xr-x   0 babay     (1000) babay     (1000)       58 2015-02-26 12:58:58.000000 m3-users-3.0.1/src/tests/test.sh
--rw-r--r--   0 babay     (1000) babay     (1000)      472 2015-02-26 12:58:58.000000 m3-users-3.0.1/src/tests/version.py
--rwxr-xr-x   0 babay     (1000) babay     (1000)       59 2015-02-26 12:58:58.000000 m3-users-3.0.1/src/tests/shell.sh
-drwxr-xr-x   0 babay     (1000) babay     (1000)        0 2015-02-26 13:23:29.000000 m3-users-3.0.1/src/tests/core/
--rw-r--r--   0 babay     (1000) babay     (1000)        0 2015-02-26 12:58:58.000000 m3-users-3.0.1/src/tests/core/__init__.py
--rw-r--r--   0 babay     (1000) babay     (1000)      247 2015-02-26 12:58:58.000000 m3-users-3.0.1/src/tests/core/tests.py
-drwxr-xr-x   0 babay     (1000) babay     (1000)        0 2015-02-26 13:23:29.000000 m3-users-3.0.1/src/m3_users.egg-info/
--rw-r--r--   0 babay     (1000) babay     (1000)       15 2015-02-26 13:23:29.000000 m3-users-3.0.1/src/m3_users.egg-info/top_level.txt
--rw-r--r--   0 babay     (1000) babay     (1000)        1 2015-02-26 13:23:29.000000 m3-users-3.0.1/src/m3_users.egg-info/dependency_links.txt
--rw-r--r--   0 babay     (1000) babay     (1000)      883 2015-02-26 13:23:29.000000 m3-users-3.0.1/src/m3_users.egg-info/SOURCES.txt
--rw-r--r--   0 babay     (1000) babay     (1000)      617 2015-02-26 13:23:29.000000 m3-users-3.0.1/src/m3_users.egg-info/PKG-INFO
--rw-r--r--   0 babay     (1000) babay     (1000)       59 2015-02-26 13:23:29.000000 m3-users-3.0.1/setup.cfg
+drwxr-xr-x   0 babay     (1000) babay     (1000)        0 2015-03-05 05:25:00.000000 m3-users-3.0.2/
+-rw-r--r--   0 babay     (1000) babay     (1000)       23 2015-02-26 12:58:58.000000 m3-users-3.0.2/README.txt
+-rw-r--r--   0 babay     (1000) babay     (1000)      925 2015-03-05 05:22:20.000000 m3-users-3.0.2/setup.py
+-rw-r--r--   0 babay     (1000) babay     (1000)        9 2015-02-26 12:58:58.000000 m3-users-3.0.2/MANIFEST.in
+-rw-r--r--   0 babay     (1000) babay     (1000)      617 2015-03-05 05:25:00.000000 m3-users-3.0.2/PKG-INFO
+drwxr-xr-x   0 babay     (1000) babay     (1000)        0 2015-03-05 05:25:00.000000 m3-users-3.0.2/src/
+drwxr-xr-x   0 babay     (1000) babay     (1000)        0 2015-03-05 05:25:00.000000 m3-users-3.0.2/src/m3_users/
+-rw-r--r--   0 babay     (1000) babay     (1000)     2849 2015-03-05 05:21:02.000000 m3-users-3.0.2/src/m3_users/app_meta.py
+-rw-r--r--   0 babay     (1000) babay     (1000)     3785 2015-02-26 13:02:24.000000 m3-users-3.0.2/src/m3_users/api.py
+-rw-r--r--   0 babay     (1000) babay     (1000)     3535 2015-02-26 13:02:24.000000 m3-users-3.0.2/src/m3_users/models.py
+-rw-r--r--   0 babay     (1000) babay     (1000)      281 2015-02-26 13:02:24.000000 m3-users-3.0.2/src/m3_users/__init__.py
+-rw-r--r--   0 babay     (1000) babay     (1000)     3052 2015-02-26 13:02:24.000000 m3-users-3.0.2/src/m3_users/helpers.py
+-rw-r--r--   0 babay     (1000) babay     (1000)      111 2015-02-26 13:02:24.000000 m3-users-3.0.2/src/m3_users/version.py
+-rw-r--r--   0 babay     (1000) babay     (1000)     3153 2015-02-26 13:02:24.000000 m3-users-3.0.2/src/m3_users/permissions.py
+drwxr-xr-x   0 babay     (1000) babay     (1000)        0 2015-03-05 05:25:00.000000 m3-users-3.0.2/src/m3_users/migrations/
+-rw-r--r--   0 babay     (1000) babay     (1000)        0 2015-02-26 12:58:58.000000 m3-users-3.0.2/src/m3_users/migrations/__init__.py
+-rw-r--r--   0 babay     (1000) babay     (1000)     6619 2015-02-26 12:58:58.000000 m3-users-3.0.2/src/m3_users/migrations/0001_initial.py
+drwxr-xr-x   0 babay     (1000) babay     (1000)        0 2015-03-05 05:25:00.000000 m3-users-3.0.2/src/m3_users/templates/
+drwxr-xr-x   0 babay     (1000) babay     (1000)        0 2015-03-05 05:25:00.000000 m3-users-3.0.2/src/m3_users/templates/m3-users/
+-rw-r--r--   0 babay     (1000) babay     (1000)     1710 2015-02-26 13:02:24.000000 m3-users-3.0.2/src/m3_users/templates/m3-users/edit-role-window.js
+-rw-r--r--   0 babay     (1000) babay     (1000)     2045 2015-02-26 13:02:24.000000 m3-users-3.0.2/src/m3_users/templates/m3-users/roles-list-window.js
+-rw-r--r--   0 babay     (1000) babay     (1000)     1862 2015-02-26 13:02:24.000000 m3-users-3.0.2/src/m3_users/templates/m3-users/select-users-window.js
+-rw-r--r--   0 babay     (1000) babay     (1000)     7461 2015-02-26 13:02:24.000000 m3-users-3.0.2/src/m3_users/metaroles.py
+-rw-r--r--   0 babay     (1000) babay     (1000)    40216 2015-03-05 05:21:02.000000 m3-users-3.0.2/src/m3_users/roles.py
+-rw-r--r--   0 babay     (1000) babay     (1000)     2335 2015-02-26 13:02:24.000000 m3-users-3.0.2/src/m3_users/users.py
+-rw-r--r--   0 babay     (1000) babay     (1000)        0 2015-02-26 12:58:58.000000 m3-users-3.0.2/src/requires.txt
+drwxr-xr-x   0 babay     (1000) babay     (1000)        0 2015-03-05 05:25:00.000000 m3-users-3.0.2/src/tests/
+-rw-r--r--   0 babay     (1000) babay     (1000)      656 2015-02-26 12:58:58.000000 m3-users-3.0.2/src/tests/urls.py
+-rwxr-xr-x   0 babay     (1000) babay     (1000)      779 2015-02-26 12:58:58.000000 m3-users-3.0.2/src/tests/manage.py
+-rw-r--r--   0 babay     (1000) babay     (1000)    13515 2015-02-26 12:58:58.000000 m3-users-3.0.2/src/tests/prepare_env.py
+-rw-r--r--   0 babay     (1000) babay     (1000)     4124 2015-02-26 12:58:58.000000 m3-users-3.0.2/src/tests/settings.py
+-rw-r--r--   0 babay     (1000) babay     (1000)      436 2015-02-26 12:58:58.000000 m3-users-3.0.2/src/tests/__init__.py
+-rwxr-xr-x   0 babay     (1000) babay     (1000)       58 2015-02-26 12:58:58.000000 m3-users-3.0.2/src/tests/test.sh
+-rw-r--r--   0 babay     (1000) babay     (1000)      472 2015-02-26 12:58:58.000000 m3-users-3.0.2/src/tests/version.py
+-rwxr-xr-x   0 babay     (1000) babay     (1000)       59 2015-02-26 12:58:58.000000 m3-users-3.0.2/src/tests/shell.sh
+drwxr-xr-x   0 babay     (1000) babay     (1000)        0 2015-03-05 05:25:00.000000 m3-users-3.0.2/src/tests/core/
+-rw-r--r--   0 babay     (1000) babay     (1000)        0 2015-02-26 12:58:58.000000 m3-users-3.0.2/src/tests/core/__init__.py
+-rw-r--r--   0 babay     (1000) babay     (1000)      247 2015-02-26 12:58:58.000000 m3-users-3.0.2/src/tests/core/tests.py
+drwxr-xr-x   0 babay     (1000) babay     (1000)        0 2015-03-05 05:25:00.000000 m3-users-3.0.2/src/m3_users.egg-info/
+-rw-r--r--   0 babay     (1000) babay     (1000)       15 2015-03-05 05:25:00.000000 m3-users-3.0.2/src/m3_users.egg-info/top_level.txt
+-rw-r--r--   0 babay     (1000) babay     (1000)        1 2015-03-05 05:25:00.000000 m3-users-3.0.2/src/m3_users.egg-info/dependency_links.txt
+-rw-r--r--   0 babay     (1000) babay     (1000)      883 2015-03-05 05:25:00.000000 m3-users-3.0.2/src/m3_users.egg-info/SOURCES.txt
+-rw-r--r--   0 babay     (1000) babay     (1000)      617 2015-03-05 05:25:00.000000 m3-users-3.0.2/src/m3_users.egg-info/PKG-INFO
+-rw-r--r--   0 babay     (1000) babay     (1000)       59 2015-03-05 05:25:00.000000 m3-users-3.0.2/setup.cfg
```

### Comparing `m3-users-3.0.1/setup.py` & `m3-users-3.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 requires = []
 with open('src/requires.txt', 'r') as f:
     requires.extend(f.readlines())
 
 setup(name='m3-users',
-      version='3.0.1',
+      version='3.0.2',
       url='https://bitbucket.org/barsgroup/m3_users',
       license='MIT',
       author='BARS Group',
       author_email='bars@bars-open.ru',
       package_dir={'': 'src'},
       packages=find_packages('src'),
       description=u'Пользователи и роли',
```

### Comparing `m3-users-3.0.1/PKG-INFO` & `m3-users-3.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: m3-users
-Version: 3.0.1
+Version: 3.0.2
 Summary: Пользователи и роли
 Home-page: https://bitbucket.org/barsgroup/m3_users
 Author: BARS Group
 Author-email: bars@bars-open.ru
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `m3-users-3.0.1/src/m3_users/app_meta.py` & `m3-users-3.0.2/src/m3_users/app_meta.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,28 +6,31 @@
 """
 
 from django.conf import urls
 
 from m3 import authenticated_user_required
 from m3.actions import ActionController
 
-from roles import RolesActions, Roles_DictPack
-from users import UsersActions
 from metaroles import UserMetarole, Metaroles_DictPack
-
+    
 # Константы:
 GENERIC_USER = 'generic-user'
 ADMIN = 'admin'
 SUPER_ADMIN = 'super-admin'
 
 # контроллер
 users_controller = ActionController(url='/m3-users', name=u'Пользователи М3')
 
 
 def register_actions():
+
+    # защита от кроссимпорта при импорте констант типов метаролей
+    from roles import RolesActions, Roles_DictPack
+    from users import UsersActions
+
     users_controller.packs.extend([
         RolesActions(),
         UsersActions(),
         Roles_DictPack(),
         
         Metaroles_DictPack(), # метароли пользователей
     ])
@@ -46,15 +49,15 @@
 def register_metaroles(manager):
     """
     Функция возвращает список метаролей, которые регистрируются
     по умолчанию на уровне Платформы М3.
     
     @param manager: объект, отвечающий за управление метаролями.
     """
-    
+
     # метароль обычного пользователя системы
     manager.GENERIC_USER_METAROLE = UserMetarole(GENERIC_USER, u'Обобщенный пользователь')
     
     # метароль администратора системы
     manager.ADMIN_METAROLE = UserMetarole(ADMIN, u'Администратор')
     manager.ADMIN_METAROLE.included_metaroles.extend([manager.GENERIC_USER_METAROLE])
```

### Comparing `m3-users-3.0.1/src/m3_users/api.py` & `m3-users-3.0.2/src/m3_users/api.py`

 * *Files identical despite different names*

### Comparing `m3-users-3.0.1/src/m3_users/models.py` & `m3-users-3.0.2/src/m3_users/models.py`

 * *Files identical despite different names*

### Comparing `m3-users-3.0.1/src/m3_users/helpers.py` & `m3-users-3.0.2/src/m3_users/helpers.py`

 * *Files identical despite different names*

### Comparing `m3-users-3.0.1/src/m3_users/permissions.py` & `m3-users-3.0.2/src/m3_users/permissions.py`

 * *Files identical despite different names*

### Comparing `m3-users-3.0.1/src/m3_users/migrations/0001_initial.py` & `m3-users-3.0.2/src/m3_users/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `m3-users-3.0.1/src/m3_users/templates/m3-users/edit-role-window.js` & `m3-users-3.0.2/src/m3_users/templates/m3-users/edit-role-window.js`

 * *Files identical despite different names*

### Comparing `m3-users-3.0.1/src/m3_users/templates/m3-users/roles-list-window.js` & `m3-users-3.0.2/src/m3_users/templates/m3-users/roles-list-window.js`

 * *Files identical despite different names*

### Comparing `m3-users-3.0.1/src/m3_users/templates/m3-users/select-users-window.js` & `m3-users-3.0.2/src/m3_users/templates/m3-users/select-users-window.js`

 * *Files identical despite different names*

### Comparing `m3-users-3.0.1/src/m3_users/metaroles.py` & `m3-users-3.0.2/src/m3_users/metaroles.py`

 * *Files identical despite different names*

### Comparing `m3-users-3.0.1/src/m3_users/roles.py` & `m3-users-3.0.2/src/m3_users/roles.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 except ImportError:
     _M3_AUDIT_INSTALLED = False
 
 from users import SelectUsersListWindow
 import helpers
 import models
 import metaroles
-import app_meta
 import api
 
 PERM_OBJECT_NOT_FOUND = u'** объект права не найден **'
 
 class ExtUIScriptResult(object): pass
 class ExtTreeNode(object): pass
 
@@ -710,14 +709,18 @@
 
 class RolesEditWindow(windows.ExtEditWindow):
     '''
     Окно редактирования роли
     '''
 
     def __init__(self, new_role=False, *args, **kwargs):
+    
+        # Защита от кроссимпорта
+        from app_meta import users_controller
+    
         super(RolesEditWindow, self).__init__(*args, **kwargs)
 
         self.width = 500
         self.height = 400
         self.modal = True
 
         self.new_role = new_role
@@ -728,15 +731,15 @@
         self.layout = 'border'
         self.form = panels.ExtForm(layout='form', region='north', height=60, style={'padding': '5px'})
         self.form.label_width = 100
         self.form.url = SaveRoleAction.absolute_url()
 
         field_name = fields.ExtStringField(name='name', label=u'Наименование', allow_blank=False, anchor='100%')
         field_metarole = fields.ExtDictSelectField(name='metarole', label=u'Метароль', anchor='100%', hide_trigger=False)
-        field_metarole.configure_by_dictpack(metaroles.Metaroles_DictPack, app_meta.users_controller)
+        field_metarole.configure_by_dictpack(metaroles.Metaroles_DictPack, users_controller)
         field_metarole.editable = False
         field_metarole.hide_dict_select_trigger = True
 
         self.form.items.extend([field_name, field_metarole])
 
         self.grid = ExtObjectGrid(title=u"Права доступа", region="center")
         self.grid.action_data = GetRolePermissionAction
```

### Comparing `m3-users-3.0.1/src/m3_users/users.py` & `m3-users-3.0.2/src/m3_users/users.py`

 * *Files identical despite different names*

### Comparing `m3-users-3.0.1/src/tests/urls.py` & `m3-users-3.0.2/src/tests/urls.py`

 * *Files identical despite different names*

### Comparing `m3-users-3.0.1/src/tests/manage.py` & `m3-users-3.0.2/src/tests/manage.py`

 * *Files identical despite different names*

### Comparing `m3-users-3.0.1/src/tests/prepare_env.py` & `m3-users-3.0.2/src/tests/prepare_env.py`

 * *Files identical despite different names*

### Comparing `m3-users-3.0.1/src/tests/settings.py` & `m3-users-3.0.2/src/tests/settings.py`

 * *Files identical despite different names*

### Comparing `m3-users-3.0.1/src/m3_users.egg-info/SOURCES.txt` & `m3-users-3.0.2/src/m3_users.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `m3-users-3.0.1/src/m3_users.egg-info/PKG-INFO` & `m3-users-3.0.2/src/m3_users.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: m3-users
-Version: 3.0.1
+Version: 3.0.2
 Summary: Пользователи и роли
 Home-page: https://bitbucket.org/barsgroup/m3_users
 Author: BARS Group
 Author-email: bars@bars-open.ru
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

