# Comparing `tmp/django_ninja_crud-0.4.1.tar.gz` & `tmp/django_ninja_crud-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_ninja_crud-0.4.1.tar", max compression
+gzip compressed data, was "django_ninja_crud-0.5.0.tar", max compression
```

## Comparing `django_ninja_crud-0.4.1.tar` & `django_ninja_crud-0.5.0.tar`

### file list

```diff
@@ -1,44 +1,17 @@
--rw-r--r--   0        0        0     1069 2023-11-29 17:39:43.148638 django_ninja_crud-0.4.1/LICENSE.md
--rw-r--r--   0        0        0     8444 2023-11-29 17:39:43.148638 django_ninja_crud-0.4.1/README.md
--rw-r--r--   0        0        0        0 2023-11-29 17:39:43.152638 django_ninja_crud-0.4.1/ninja_crud/__init__.py
--rw-r--r--   0        0        0      246 2023-11-29 17:39:43.152638 django_ninja_crud-0.4.1/ninja_crud/schemas.py
--rw-r--r--   0        0        0      106 2023-11-29 17:39:43.152638 django_ninja_crud-0.4.1/ninja_crud/testing/__init__.py
--rw-r--r--   0        0        0      198 2023-11-29 17:39:43.152638 django_ninja_crud-0.4.1/ninja_crud/testing/core/__init__.py
--rw-r--r--   0        0        0      241 2023-11-29 17:39:43.152638 django_ninja_crud-0.4.1/ninja_crud/testing/core/components/__init__.py
--rw-r--r--   0        0        0     2522 2023-11-29 17:39:43.152638 django_ninja_crud-0.4.1/ninja_crud/testing/core/components/headers.py
--rw-r--r--   0        0        0     2015 2023-11-29 17:39:43.152638 django_ninja_crud-0.4.1/ninja_crud/testing/core/components/path_parameters.py
--rw-r--r--   0        0        0     2449 2023-11-29 17:39:43.152638 django_ninja_crud-0.4.1/ninja_crud/testing/core/components/payloads.py
--rw-r--r--   0        0        0     2127 2023-11-29 17:39:43.152638 django_ninja_crud-0.4.1/ninja_crud/testing/core/components/query_parameters.py
--rw-r--r--   0        0        0      892 2023-11-29 17:39:43.152638 django_ninja_crud-0.4.1/ninja_crud/testing/core/components/utils.py
--rw-r--r--   0        0        0    11507 2023-11-29 17:39:43.152638 django_ninja_crud-0.4.1/ninja_crud/testing/core/view_test_manager.py
--rw-r--r--   0        0        0      519 2023-11-29 17:39:43.152638 django_ninja_crud-0.4.1/ninja_crud/testing/views/__init__.py
--rw-r--r--   0        0        0     4843 2023-11-29 17:39:43.152638 django_ninja_crud-0.4.1/ninja_crud/testing/views/abstract_model_view_test.py
--rw-r--r--   0        0        0    10463 2023-11-29 17:39:43.152638 django_ninja_crud-0.4.1/ninja_crud/testing/views/create_model_view_test.py
--rw-r--r--   0        0        0     8440 2023-11-29 17:39:43.152638 django_ninja_crud-0.4.1/ninja_crud/testing/views/delete_model_view_test.py
--rw-r--r--   0        0        0    12374 2023-11-29 17:39:43.152638 django_ninja_crud-0.4.1/ninja_crud/testing/views/list_model_view_test.py
--rw-r--r--   0        0        0     9556 2023-11-29 17:39:43.152638 django_ninja_crud-0.4.1/ninja_crud/testing/views/retrieve_model_view_test.py
--rw-r--r--   0        0        0    10751 2023-11-29 17:39:43.152638 django_ninja_crud-0.4.1/ninja_crud/testing/views/update_model_view_test.py
--rw-r--r--   0        0        0      101 2023-11-29 17:39:43.152638 django_ninja_crud-0.4.1/ninja_crud/testing/viewsets/__init__.py
--rw-r--r--   0        0        0    10592 2023-11-29 17:39:43.152638 django_ninja_crud-0.4.1/ninja_crud/testing/viewsets/model_viewset_test_case.py
--rw-r--r--   0        0        0     2411 2023-11-29 17:39:43.152638 django_ninja_crud-0.4.1/ninja_crud/utils.py
--rw-r--r--   0        0        0      441 2023-11-29 17:39:43.152638 django_ninja_crud-0.4.1/ninja_crud/views/__init__.py
--rw-r--r--   0        0        0     8428 2023-11-29 17:39:43.156638 django_ninja_crud-0.4.1/ninja_crud/views/abstract_model_view.py
--rw-r--r--   0        0        0    12960 2023-11-29 17:39:43.156638 django_ninja_crud-0.4.1/ninja_crud/views/create_model_view.py
--rw-r--r--   0        0        0     5625 2023-11-29 17:39:43.156638 django_ninja_crud-0.4.1/ninja_crud/views/delete_model_view.py
--rw-r--r--   0        0        0       62 2023-11-29 17:39:43.156638 django_ninja_crud-0.4.1/ninja_crud/views/enums/__init__.py
--rw-r--r--   0        0        0      675 2023-11-29 17:39:43.156638 django_ninja_crud-0.4.1/ninja_crud/views/enums/http_method.py
--rw-r--r--   0        0        0        0 2023-11-29 17:39:43.156638 django_ninja_crud-0.4.1/ninja_crud/views/helpers/__init__.py
--rw-r--r--   0        0        0     3152 2023-11-29 17:39:43.156638 django_ninja_crud-0.4.1/ninja_crud/views/helpers/types.py
--rw-r--r--   0        0        0     1133 2023-11-29 17:39:43.156638 django_ninja_crud-0.4.1/ninja_crud/views/helpers/utils.py
--rw-r--r--   0        0        0    11580 2023-11-29 17:39:43.156638 django_ninja_crud-0.4.1/ninja_crud/views/list_model_view.py
--rw-r--r--   0        0        0     6392 2023-11-29 17:39:43.156638 django_ninja_crud-0.4.1/ninja_crud/views/retrieve_model_view.py
--rw-r--r--   0        0        0     8149 2023-11-29 17:39:43.156638 django_ninja_crud-0.4.1/ninja_crud/views/update_model_view.py
--rw-r--r--   0        0        0        0 2023-11-29 17:39:43.156638 django_ninja_crud-0.4.1/ninja_crud/views/validators/__init__.py
--rw-r--r--   0        0        0     2099 2023-11-29 17:39:43.156638 django_ninja_crud-0.4.1/ninja_crud/views/validators/model_factory_validator.py
--rw-r--r--   0        0        0     1176 2023-11-29 17:39:43.156638 django_ninja_crud-0.4.1/ninja_crud/views/validators/path_validator.py
--rw-r--r--   0        0        0     2251 2023-11-29 17:39:43.156638 django_ninja_crud-0.4.1/ninja_crud/views/validators/queryset_getter_validator.py
--rw-r--r--   0        0        0      137 2023-11-29 17:39:43.156638 django_ninja_crud-0.4.1/ninja_crud/viewsets/__init__.py
--rw-r--r--   0        0        0     3565 2023-11-29 17:39:43.156638 django_ninja_crud-0.4.1/ninja_crud/viewsets/base_model_viewset.py
--rw-r--r--   0        0        0     6237 2023-11-29 17:39:43.156638 django_ninja_crud-0.4.1/ninja_crud/viewsets/model_viewset.py
--rw-r--r--   0        0        0     1955 2023-11-29 17:39:43.156638 django_ninja_crud-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     9860 1970-01-01 00:00:00.000000 django_ninja_crud-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-20 00:02:50.465019 django_ninja_crud-0.5.0/LICENSE.md
+-rw-r--r--   0        0        0    11984 2024-05-20 00:02:50.465019 django_ninja_crud-0.5.0/README.md
+-rw-r--r--   0        0        0      161 2024-05-20 00:02:50.469020 django_ninja_crud-0.5.0/ninja_crud/__init__.py
+-rw-r--r--   0        0        0      475 2024-05-20 00:02:50.469020 django_ninja_crud-0.5.0/ninja_crud/testing.py
+-rw-r--r--   0        0        0      318 2024-05-20 00:02:50.469020 django_ninja_crud-0.5.0/ninja_crud/views/__init__.py
+-rw-r--r--   0        0        0    12861 2024-05-20 00:02:50.469020 django_ninja_crud-0.5.0/ninja_crud/views/api_view.py
+-rw-r--r--   0        0        0     9911 2024-05-20 00:02:50.473019 django_ninja_crud-0.5.0/ninja_crud/views/create_view.py
+-rw-r--r--   0        0        0     7783 2024-05-20 00:02:50.473019 django_ninja_crud-0.5.0/ninja_crud/views/delete_view.py
+-rw-r--r--   0        0        0      112 2024-05-20 00:02:50.473019 django_ninja_crud-0.5.0/ninja_crud/views/helpers/__init__.py
+-rw-r--r--   0        0        0     4983 2024-05-20 00:02:50.473019 django_ninja_crud-0.5.0/ninja_crud/views/helpers/path_parameters_type_resolver.py
+-rw-r--r--   0        0        0     9386 2024-05-20 00:02:50.473019 django_ninja_crud-0.5.0/ninja_crud/views/list_view.py
+-rw-r--r--   0        0        0     7079 2024-05-20 00:02:50.473019 django_ninja_crud-0.5.0/ninja_crud/views/read_view.py
+-rw-r--r--   0        0        0     9933 2024-05-20 00:02:50.473019 django_ninja_crud-0.5.0/ninja_crud/views/update_view.py
+-rw-r--r--   0        0        0       62 2024-05-20 00:02:50.473019 django_ninja_crud-0.5.0/ninja_crud/viewsets/__init__.py
+-rw-r--r--   0        0        0     4841 2024-05-20 00:02:50.473019 django_ninja_crud-0.5.0/ninja_crud/viewsets/api_viewset.py
+-rw-r--r--   0        0        0     1987 2024-05-20 00:02:50.473019 django_ninja_crud-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0    13388 1970-01-01 00:00:00.000000 django_ninja_crud-0.5.0/PKG-INFO
```

### Comparing `django_ninja_crud-0.4.1/LICENSE.md` & `django_ninja_crud-0.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django_ninja_crud-0.4.1/README.md` & `django_ninja_crud-0.5.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,70 @@
 # Django Ninja CRUD
 [![Tests](https://github.com/hbakri/django-ninja-crud/actions/workflows/tests.yml/badge.svg)](https://github.com/hbakri/django-ninja-crud/actions)
 [![Coverage](https://img.shields.io/codecov/c/github/hbakri/django-ninja-crud/main.svg?label=coverage&logo=codecov&logoColor=white)](https://codecov.io/gh/hbakri/django-ninja-crud)
 [![PyPI version](https://img.shields.io/pypi/v/django-ninja-crud?color=blue&logo=pypi&logoColor=white)](https://pypi.org/project/django-ninja-crud/)
 [![Downloads](https://static.pepy.tech/badge/django-ninja-crud/month)](https://pepy.tech/project/django-ninja-crud)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
+[![MyPy](https://img.shields.io/badge/mypy-checked-blue.svg)](https://github.com/python/mypy)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 ![Django Ninja CRUD](https://raw.githubusercontent.com/hbakri/django-ninja-crud/main/docs/assets/images/django-ninja-crud-cover.png)
 
-Django Ninja CRUD is a [declarative](https://en.wikipedia.org/wiki/Declarative_programming), powerful, and yet opinionated framework that simplifies the development of **CRUD** ([**C**reate, **R**ead, **U**pdate, **D**elete](https://en.wikipedia.org/wiki/Create,_read,_update_and_delete)) views and tests with [Django Ninja](https://github.com/vitalik/django-ninja).
-It promotes best practices for efficient, robust endpoint creation, allowing you to focus on what matters most: solving real problems.
-Initially inspired by DRF's [ModelViewSet](https://www.django-rest-framework.org/api-guide/viewsets/#modelviewset), Django Ninja CRUD evolved to address its limitations, adopting a [composition-over-inheritance](https://en.wikipedia.org/wiki/Composition_over_inheritance) approach to achieve true modularity – a foundational step towards a broader declarative interface for endpoint creation.
+> [!IMPORTANT]
+> With the release of version `0.5`, Django Ninja CRUD introduces significant
+> and breaking changes. Users are strongly advised to pin their requirements to the
+> appropriate version to ensure compatibility with their projects.
+
+Django Ninja CRUD is a powerful, [declarative](https://en.wikipedia.org/wiki/Declarative_programming), and yet a little bit opinionated framework that
+simplifies the development of **CRUD** ([**C**reate, **R**ead, **U**pdate, **D**elete](https://en.wikipedia.org/wiki/Create,_read,_update_and_delete))
+endpoints with [Django Ninja](https://github.com/vitalik/django-ninja), and also
+provides a declarative scenario-based way for testing these endpoints with
+[Django REST Testing](https://github.com/hbakri/django-rest-testing) _(the little brother of this package)_ 🐣.
+
+It allows you to define common endpoints as class-based views and customize them to
+conform to your project's conventions with ease, and also create easily your own
+custom views and declare them alongside the provided CRUD views, fostering modularity
+and extensibility. This package promotes focusing on what matters most:
+**solving real problems**, not reinventing the wheel all over your project.
+
+Initially inspired by DRF's [ModelViewSet](https://www.django-rest-framework.org/api-guide/viewsets/#modelviewset),
+Django Ninja CRUD evolved to address its limitations, adopting a
+[composition-over-inheritance](https://en.wikipedia.org/wiki/Composition_over_inheritance)
+approach to achieve true modularity – a foundational step towards a broader declarative
+interface for endpoint creation.
+
+Key challenges with inheritance-based viewsets:
+- **Unicity of CRUD endpoints per model**: Django Ninja CRUD allows you to define multiple endpoints for the same model, enabling versioning or alternative representations.
+- **Customization inflexibility**: Instead of overriding methods on a monolithic class, you can customize individual views through composition and configuration.
+- **Implicit relations within inheritance hierarchies**: Composition decouples views, reducing dependencies and promoting reusability.
+- **Lack of modularity for new endpoints**: Adding custom endpoints no longer requires subclassing the entire viewset, making it easier to introduce new functionality incrementally.
 
 ## ✨ Key Features
-- **Purely Declarative**: Embrace an approach where defining views and tests is a matter of declaring what you want, not how to achieve it.
-- **Unmatched Modularity**: Tailor your viewsets with the desired CRUD views and customize each view's behavior with ease. Extend the flexibility by creating your own subclasses of the provided views and tests.
-- **Powerful Testing Framework**: Leverage a matrix-based testing framework for defining diverse test scenarios declaratively.
-- **Focus on What Matters**: Spend more time solving real-world problems and less on CRUD boilerplate.
-
-Its blend of declarative syntax, modularity, and powerful testing capabilities sets a new standard for developers seeking efficiency and precision.
+- **Purely Declarative**: Define views and tests by declaring what you want, not how to do it.
+- **Unmatched Modularity**: Tailor your viewsets with desired CRUD views, customize each view's behavior.
+- **Easy to Extend**: Create your own custom views and use them alongside the provided CRUD views as reusable components.
+- **Scenario-based Testing Framework**: Leverage a scenario-based testing framework for defining diverse test cases declaratively and concisely.
+- **Focus on What Matters**: Spend more time solving real-world problems and less on common and repetitive tasks.
 
 > **Django Ninja CRUD is not just a tool; it's a paradigm shift in Django web application development and testing.**
 
 ## 📝 Requirements
 
-![Python versions](https://img.shields.io/pypi/pyversions/django-ninja-crud.svg?color=306998&label=python&logo=python&logoColor=white)
-![Django versions](https://img.shields.io/badge/3.2%20|%204.1%20|%204.2%20|%205.0b1-blue?color=0C4B33&label=django&logo=django&logoColor=white)
-![Django Ninja versions](https://img.shields.io/badge/0.21%20|%200.22%20|%201.0-blue?color=black&label=django-ninja&logo=fastapi&logoColor=white)
+[![Python versions](https://img.shields.io/pypi/pyversions/django-ninja-crud.svg?color=306998&label=python&logo=python&logoColor=white)](https://github.com/python/cpython)
+[![Django versions](https://img.shields.io/badge/3.2_|_4.1_|_4.2_|_5.0-blue?color=0C4B33&label=django&logo=django&logoColor=white)](https://github.com/django/django)
+[![Django Ninja versions](https://img.shields.io/badge/1.0_|_1.1-blue?color=black&label=django-ninja&logo=fastapi&logoColor=white)](https://github.com/vitalik/django-ninja)
 
 ## ⚒️ Installation
 ```bash
-pip install django-ninja-crud
+pip install django-ninja-crud[testing]
 ```
 For more information, see the [installation guide](https://django-ninja-crud.readme.io/docs/02-installation).
 
-## 👨‍🎨 Example
-### Usage
+## 🌞 How It Works
+
 Let's imagine you're building a system for a university and you have a model called `Department`. Each department in your university has a unique title.
 
 ```python
 # examples/models.py
 from django.db import models
 
 class Department(models.Model):
@@ -58,106 +83,170 @@
 class DepartmentOut(Schema):
     id: int
     title: str
 ```
 
 The `DepartmentIn` schema defines what data we need when creating or updating a department. The `DepartmentOut` schema defines what data we'll provide when retrieving a department.
 
-Now, here comes the power of Django Ninja CRUD. With it, you can set up the **CRUD** operations for the `Department` model with just a few lines of code:
+Now, here comes the power of the package. With it, you can set up the **CRUD**
+operations for the `Department` model with just a few lines of code:
 
 ```python
 # examples/views/department_views.py
+from typing import List
 from django.http import HttpRequest
-from ninja import Router
+from ninja import NinjaAPI
 from ninja_crud import views, viewsets
 
 from examples.models import Department
 from examples.schemas import DepartmentIn, DepartmentOut
 
-router = Router()
+api = NinjaAPI()
 
 
-class DepartmentViewSet(viewsets.ModelViewSet):
+class DepartmentViewSet(viewsets.APIViewSet):
+    api = api
     model = Department
-    default_input_schema = DepartmentIn
-    default_output_schema = DepartmentOut
-
-    list_view = views.ListModelView()
-    create_view = views.CreateModelView()
-    retrieve_view = views.RetrieveModelView()
-    update_view = views.UpdateModelView()
-    delete_view = views.DeleteModelView()
-
 
-# The register_routes method must be called to register the routes
-DepartmentViewSet.register_routes(router)
+    list_departments = views.ListView(
+        response_body=List[DepartmentOut]
+    )
+    create_department = views.CreateView(
+        request_body=DepartmentIn,
+        response_body=DepartmentOut,
+    )
+    read_department = views.ReadView(
+        response_body=DepartmentOut
+    )
+    update_department = views.UpdateView(
+        request_body=DepartmentIn,
+        response_body=DepartmentOut,
+    )
+    delete_department = views.DeleteView()
 
 
 # Beyond the CRUD operations managed by the viewset,
-# the router can be used in the standard Django Ninja way
-@router.get("/statistics/", response=dict)
-def retrieve_department_statistics(request: HttpRequest):
+# the api or router can be used in the standard Django Ninja way
+@api.get("/statistics/", response=dict)
+def get_department_statistics(request: HttpRequest):
     return {"total": Department.objects.count()}
 ```
 
-### Testing
-A key advantage of this package is that it makes your views easy to test. Once you've set up your **CRUD** operations, you can write tests to ensure they're working as expected. Here's an example of how you might test the `Department` operations:
+And if your viewset is as simple as the one above, you can leverage the `APIViewSet`
+class to define it in a more concise way, with default request and response bodies:
+```python
+# examples/views/department_views.py
+from ninja import NinjaAPI
+from ninja_crud import views, viewsets
+
+from examples.models import Department
+from examples.schemas import DepartmentIn, DepartmentOut
+
+api = NinjaAPI()
+
+
+class DepartmentViewSet(viewsets.APIViewSet):
+    api = api
+    model = Department
+    default_request_body = DepartmentIn
+    default_response_body = DepartmentOut
+
+    list_departments = views.ListView()
+    create_department = views.CreateView()
+    read_department = views.ReadView()
+    update_department = views.UpdateView()
+    delete_department = views.DeleteView()
+```
+
+## ☔️ Scenario-based Testing
+
+Django Ninja CRUD integrates seamlessly with [Django REST Testing](https://github.com/hbakri/django-rest-testing),
+and ensures comprehensive coverage and robust validation of your CRUD endpoints. At
+first, the testing framework was part of this package, but it was later extracted
+to its own package to allow for more flexibility and to be used with other Django
+REST frameworks than Django Ninja.
+
+With this package, you can:
+- **Declaratively Define Test Scenarios**: Specify expected request and response details for each scenario, making your tests self-documenting and easy to understand.
+- **Test Diverse Conditions**: Validate endpoint behaviors under various conditions, including valid and invalid inputs, nonexistent resources, and custom business rules.
+- **Enhance Clarity and Maintainability**: Break tests into modular, manageable units, improving code organization and reducing technical debt.
+- **Ensure Comprehensive Coverage**: Rigorously test your endpoints, leaving no stone unturned, thanks to the scenario-based approach.
+
+To handle exceptions like `ObjectDoesNotExist` and return appropriate responses in your
+tests, you can define an exception handler like this:
 
 ```python
-# examples/tests/test_department_views.py
-from ninja_crud import testing
+# examples/exception_handlers.py
+from ninja import NinjaAPI
+from django.core.exceptions import ObjectDoesNotExist
+
+api = NinjaAPI()
+
+
+@api.exception_handler(ObjectDoesNotExist)
+def handle_object_does_not_exist(request, exc):
+    return api.create_response(
+        request,
+        {"message": "ObjectDoesNotExist", "detail": str(exc)},
+        status=404,
+    )
+
+# ... other exception handlers
+```
+
+Now, you can write tests for your CRUD views using the scenario-based testing framework:
 
+```python
+# examples/tests/test_department_views.py
 from examples.models import Department
-from examples.views.department_views import DepartmentViewSet
+from examples.schemas import DepartmentOut
 
+from ninja_crud.testing import APITestCase, APIViewTestScenario
 
-class TestDepartmentViewSet(testing.viewsets.ModelViewSetTestCase):
-    model_viewset_class = DepartmentViewSet
-    base_path = "api/departments"
+
+class TestDepartmentViewSet(APITestCase):
+    department: Department
 
     @classmethod
     def setUpTestData(cls):
-        cls.department_1 = Department.objects.create(title="department-1")
-        cls.department_2 = Department.objects.create(title="department-2")
+        cls.department = Department.objects.create(title="department")
 
-    @property
-    def path_parameters(self):
-        return testing.components.PathParameters(
-            ok={"id": self.department_1.id},
-            not_found={"id": 9999}
+    def test_read_department(self):
+        self.assertScenariosSucceed(
+            method="GET",
+            path="/api/departments/{id}",
+            scenarios=[
+                APIViewTestScenario(
+                    path_parameters={"id": self.department.id},
+                    expected_response_status=200,
+                    expected_response_body_type=DepartmentOut,
+                    expected_response_body={
+                        "id": self.department.id,
+                        "title": self.department.title,
+                    },
+                ),
+                APIViewTestScenario(
+                    path_parameters={"id": 9999},
+                    expected_response_status=404,
+                ),
+            ],
         )
-
-    @property
-    def payloads(self):
-        return testing.components.Payloads(
-            ok={"title": "department-3"},
-            bad_request={},
-            conflict={"title": self.department_2.title},
-        )
-
-    test_list_view = testing.views.ListModelViewTest()
-    test_create_view = testing.views.CreateModelViewTest(payloads)
-    test_retrieve_view = testing.views.RetrieveModelViewTest(path_parameters)
-    test_update_view = testing.views.UpdateModelViewTest(path_parameters, payloads)
-    test_delete_view = testing.views.DeleteModelViewTest(path_parameters)
-
-    # You can then add additional tests as needed
-    def test_retrieve_department_statistics(self):
-        response = self.client.get(f"{self.base_path}/statistics/")
-        self.assertEqual(response.status_code, 200)
-        ... # Additional assertions
 ```
 
+By combining Django Ninja CRUD's declarative views with Django REST Testing's
+scenario-based testing capabilities, you can confidently build and maintain robust,
+well-tested RESTful APIs with ease.
+
 ## 📚 Documentation
 For more information, see the [documentation](https://django-ninja-crud.readme.io/).
 
 ## 🫶 Support
-First and foremost, a heartfelt thank you for taking an interest in this project. If it has been helpful to you or you believe in its potential, kindly consider giving it a star on GitHub. Such recognition not only fuels my drive to maintain and improve this work but also makes it more visible to new potential users and contributors.
+First and foremost, a heartfelt thank you to the 400+ stargazers who have shown their support for this project. Your recognition and belief in its potential fuel my drive to maintain and improve this work, making it more visible to new potential users and contributors.
 
-![GitHub Repo stars](https://img.shields.io/github/stars/hbakri/django-ninja-crud?style=social)
+[![Star History Chart](https://api.star-history.com/svg?repos=hbakri/django-ninja-crud&type=Date)](https://star-history.com/#hbakri/django-ninja-crud&Date)
 
 If you've benefited from this project or appreciate the dedication behind it, consider showing further support. Whether it's the price of a coffee, a word of encouragement, or a sponsorship, every gesture adds fuel to the open-source fire, making it shine even brighter. ✨
 
 [![Sponsor](https://img.shields.io/badge/sponsor-donate-pink?logo=github-sponsors&logoColor=white)](https://github.com/sponsors/hbakri)
-[![Buy me a coffee](https://img.shields.io/badge/buy%20me%20a%20coffee-donate-pink?logo=buy-me-a-coffee&logoColor=white)](https://www.buymeacoffee.com/hbakri)
+[![Buy me a coffee](https://img.shields.io/badge/buy_me_a_coffee-donate-pink?logo=buy-me-a-coffee&logoColor=white)](https://www.buymeacoffee.com/hbakri)
 
 Your kindness and support make a world of difference. Thank you! 🙏
```

### Comparing `django_ninja_crud-0.4.1/ninja_crud/testing/views/delete_model_view_test.py` & `django_ninja_crud-0.5.0/ninja_crud/views/create_view.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,204 +1,228 @@
-import http
-from typing import Optional
+from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Type
 
-import django.http
-import django.test
-from django.core.exceptions import ObjectDoesNotExist
+from django.db.models import ManyToManyField, Model
+from django.http import HttpRequest
+from pydantic import BaseModel
 
-from ninja_crud.testing.core import ArgOrCallable, TestCaseType, ViewTestManager
-from ninja_crud.testing.core.components import Headers, PathParameters
-from ninja_crud.testing.views import AbstractModelViewTest
-from ninja_crud.views import DeleteModelView
+from ninja_crud.views.api_view import APIView, ViewDecorator, ViewFunction
 
+if TYPE_CHECKING:  # pragma: no cover
+    from ninja_crud.viewsets import APIViewSet
 
-class DeleteModelViewTest(AbstractModelViewTest):
-    """
-    Provides a declarative and powerful way to test the delete model view.
 
-    This class executes a matrix of test cases to validate the functionality of the `DeleteModelView`,
-    assessing its behavior under various conditions using combinations of path parameters and headers.
+class CreateView(APIView):
+    """
+    Declarative class-based view for creating a model instance in Django Ninja.
 
-    Each test method within this class is automatically attached to the test case when instantiated
-    as a class attribute on a `ModelViewSetTestCase` subclass. The test method names are dynamically
-    generated based on the class attribute name. For example, if the `DeleteModelViewTest` is used
-    to test a `DeleteModelView` named `delete_department_view`, the test methods will be named
-    `test_delete_department_view__test_delete_model_ok`,
-    `test_delete_department_view__test_delete_model_headers_unauthorized`, etc.
-
-    This naming convention ensures clear and consistent identification of test cases.
-
-    Attributes:
-        model_view (DeleteModelView): The delete model view to be tested.
-        model_viewset_test_case (ModelViewSetTestCase): The test case to which this test belongs.
+    This class provides a standard implementation for a create view, which creates a
+    new model instance based on the request body and saves it to the database. It is
+    intended to be used in viewsets or as standalone views to simplify the creation of
+    create endpoints.
+
+    Args:
+        method (str, optional): The HTTP method for the view. Defaults to "POST".
+        path (str, optional): The URL path for the view. Defaults to "/{id}".
+        response_status (int, optional): The HTTP status code for the response.
+            Defaults to 201 (Created).
+        response_body (Optional[Type[Any]], optional): The response body type.
+            Defaults to None. If not provided, the default response body of the viewset
+            will be used.
+        view_function (Optional[ViewFunction], optional): The function that handles the
+            view logic. Default implementation is `default_view_function`, which calls
+            `init_model` to create a new model instance, sets the instance attributes
+            based on the request body, calls the pre-save hook, saves the instance, and
+            calls the post-save hook.
+        view_function_name (Optional[str], optional): The name of the view function.
+            Defaults to None, which will use the default function name. If bound to a
+            viewset, the function name will be the class attribute name. Useful for
+            standalone views outside viewsets.
+        path_parameters (Optional[Type[BaseModel]], optional): The path parameters type.
+            Defaults to None. If not provided, the default path parameters will be
+            resolved based on the model, specified in the viewset or standalone view.
+        request_body (Optional[Type[BaseModel]], optional): The request body type.
+            Defaults to None. If not provided, the default request body of the viewset
+            will be used.
+        model (Optional[Type[Model]], optional): The Django model associated with the
+            view. Defaults to None. Mandatory if not bound to a viewset, otherwise
+            inherited from the viewset.
+        decorators (Optional[List[ViewDecorator]], optional): List of decorators to
+            apply to the view function. Decorators are applied in reverse order.
+        operation_kwargs (Optional[Dict[str, Any]], optional): Additional keyword
+            arguments for the operation.
+        init_model (Optional[Callable], optional): A callable to initialize the model
+            instance. By default, it creates a new instance of the model using the model
+            class defined in the view: `Model()`.
+            Should have the signature:
+            - `init_model(request: HttpRequest, path_parameters: Optional[BaseModel])
+            -> Model`.
+        pre_save (Optional[Callable], optional): A callable to perform pre-create
+            operations on the model instance. By default, it calls `full_clean` on the
+            instance to validate the data before creating.
+            Should have the signature:
+            - `pre_save(request: HttpRequest, instance: Model) -> None`.
+        post_save (Optional[Callable], optional): A callable to perform post-create
+            operations on the model instance. By default, it does nothing. Useful for
+            additional processing or side effects after saving.
+            Should have the signature:
+            - `post_save(request: HttpRequest, instance: Model) -> None`.
 
     Example:
-    1. Let's say you defined a `DeleteModelView` like this:
     ```python
-    # examples/views/department_views.py
+    from ninja import NinjaAPI
     from ninja_crud import views, viewsets
 
     from examples.models import Department
+    from examples.schemas import DepartmentIn, DepartmentOut
 
-    class DepartmentViewSet(viewsets.ModelViewSet):
-        model = Department
+    api = NinjaAPI()
 
-        delete_department_view = views.DeleteModelView()
-    ```
-    2. You can test the `delete_department_view` like this:
-    ```python
-    # examples/tests/test_department_views.py
-    from ninja_crud import testing
+    # Usage as a class attribute in a viewset:
+    class DepartmentViewSet(viewsets.APIViewSet):
+        api = api
+        model = Department
+        default_response_body = DepartmentOut
+        default_request_body = DepartmentOut
 
-    from examples.views.department_views import DepartmentViewSet
+        # Usage with default request and response bodies:
+        create_department = views.CreateView()
 
-    class TestDepartmentViewSet(testing.viewsets.ModelViewSetTestCase):
-        model_viewset_class = DepartmentViewSet
-        base_path = "api/departments"
-
-        def setUpTestData(cls):
-            super().setUpTestData()
-            cls.department_1 = Department.objects.create(title="department-1")
-
-        test_delete_department_view = testing.views.DeleteModelViewTest(
-            path_parameters=lambda test_case: testing.components.PathParameters(
-                ok={"id": test_case.department_1.id},
-                not_found={"id": 999}
-            )
-        )
+        # Usage with explicit request and response bodies:
+        create_department = views.CreateView(
+            request_body=DepartmentIn,
+            response_body=DepartmentOut,
+        )
+
+    # Usage as a standalone view:
+    views.CreateView(
+        model=Department,
+        request_body=DepartmentIn,
+        response_body=DepartmentOut,
+        view_function_name="create_department",
+    ).add_view_to(api)
     ```
-
-    Note:
-        The class attribute `DeleteModelViewTest` should be named after the view being tested.
-        For example, if you are testing the `delete_department_view` attribute of the
-        `DepartmentViewSet` class, the class attribute should be named
-        `test_delete_department_view`.
     """
 
-    model_view: DeleteModelView
-
     def __init__(
         self,
-        path_parameters: ArgOrCallable[PathParameters, TestCaseType],
-        headers: Optional[ArgOrCallable[Headers, TestCaseType]] = None,
+        method: str = "POST",
+        path: str = "/",
+        response_status: int = 201,
+        response_body: Optional[Type[Any]] = None,
+        view_function: Optional[ViewFunction] = None,
+        view_function_name: Optional[str] = None,
+        path_parameters: Optional[Type[BaseModel]] = None,
+        request_body: Optional[Type[BaseModel]] = None,
+        model: Optional[Type[Model]] = None,
+        decorators: Optional[List[ViewDecorator]] = None,
+        operation_kwargs: Optional[Dict[str, Any]] = None,
+        init_model: Optional[
+            Callable[[HttpRequest, Optional[BaseModel]], Model]
+        ] = None,
+        pre_save: Optional[Callable[[HttpRequest, Model], None]] = None,
+        post_save: Optional[Callable[[HttpRequest, Model], None]] = None,
     ) -> None:
-        """
-        Initializes the DeleteModelViewTest with path parameters and optional headers.
-
-        Args:
-            path_parameters (ArgOrCallable[PathParameters, TestCaseType]): Path parameters for
-                the request. Can be a static object, a callable, or a property on the test case.
-            headers (Optional[ArgOrCallable[Headers, TestCaseType]], optional): Headers for the
-                request. Can be a static object, a callable, or a property on the test case.
-                Defaults to None.
-        """
-        super().__init__(model_view_class=DeleteModelView)
-        self.view_test_manager = ViewTestManager(
-            handle_request=self.handle_request,
+        super().__init__(
+            method=method,
+            path=path,
+            response_status=response_status,
+            response_body=response_body,
+            view_function=view_function or self.default_view_function,
+            view_function_name=view_function_name,
             path_parameters=path_parameters,
-            headers=headers,
+            query_parameters=None,
+            request_body=request_body,
+            model=model,
+            decorators=decorators,
+            operation_kwargs=operation_kwargs,
         )
+        self.init_model = init_model or self.default_init_model
+        self.pre_save = pre_save or self.default_pre_save
+        self.post_save = post_save or self.default_post_save
 
-    def on_successful_request(
-        self,
-        response: django.http.HttpResponse,
-        path_parameters: dict,
-        query_parameters: dict,
-        headers: dict,
-        payload: dict,
-    ):
-        """
-        Callback method to handle the response for a successful request.
-
-        This method is called when the view returns a successful HTTP response. It verifies that
-        the response content matches the expected output, ensuring the correctness of the view's output.
-        The expected output is derived from the model instance specified in the path parameters.
-
-        Args:
-            response (django.http.HttpResponse): The HttpResponse object from the view.
-            path_parameters (dict): The path parameters used in the request.
-            query_parameters (dict): The query parameters used in the request.
-            headers (dict): The headers used in the request.
-            payload (dict): The payload sent with the request.
-        """
-        self.model_viewset_test_case.assertEqual(response.content, b"")
-
-        model_class = self.model_viewset_test_case.model_viewset_class.model
-        with self.model_viewset_test_case.assertRaises(ObjectDoesNotExist):
-            model_class.objects.get(id=path_parameters["id"])
-
-    def on_failed_request(
-        self,
-        response: django.http.HttpResponse,
-        path_parameters: dict,
-        query_parameters: dict,
-        headers: dict,
-        payload: dict,
-    ):
-        """
-        Callback method to handle the response for a failed request.
-
-        This method is called when the view returns a failed HTTP response. It only verifies that
-        the response status code matches the expected status code, ensuring the correctness of the
-        view's error handling.
-
-        Args:
-            response (django.http.HttpResponse): The HttpResponse object from the view.
-            path_parameters (dict): The path parameters used in the request.
-            query_parameters (dict): The query parameters used in the request.
-            headers (dict): The headers used in the request.
-            payload (dict): The payload sent with the request.
+    def default_init_model(
+        self, request: HttpRequest, path_parameters: Optional[BaseModel]
+    ) -> Model:
         """
-        pass
-
-    @django.test.tag("delete")
-    def test_delete_model_ok(self):
+        Default implementation of the model initialization hook for the view. This
+        method creates a new instance of the model using the model class defined in the
+        view: `Model()`.
         """
-        Tests the successful scenarios.
+        if self.model is None:
+            raise ValueError("No model set for the view.")
 
-        Executes subtests combining various `ok` path parameters and `ok` headers to verify the correct
-        handling and response output under valid conditions. Each combination is tested as a subtest.
-        """
-        self.view_test_manager.test_view_ok(
-            test_case=self.model_viewset_test_case,
-            on_completion=self.on_successful_request,
-            status=http.HTTPStatus.NO_CONTENT,
-        )
+        return self.model()
 
-    @django.test.tag("delete")
-    def test_delete_model_headers_unauthorized(self):
+    @staticmethod
+    def default_pre_save(request: HttpRequest, instance: Model) -> None:
         """
-        Tests the unauthorized headers scenarios.
+        Default implementation of the pre-save hook for the view. This method calls
+        `full_clean` on the model instance to validate the data before creating.
+        """
+        instance.full_clean()
 
-        Executes subtests combining various `ok` path parameters and `unauthorized` headers to verify the correct
-        handling and response output under unauthorized conditions. Each combination of parameters is tested.
+    @staticmethod
+    def default_post_save(request: HttpRequest, instance: Model) -> None:
         """
-        self.view_test_manager.test_view_headers_unauthorized(
-            test_case=self.model_viewset_test_case,
-            on_completion=self.on_failed_request,
-        )
+        Default implementation of the post-save hook for the view. This method does
+        nothing by default and can be overridden in init or subclasses to perform
+        additional operations after creating the instance.
+        """
+        pass
 
-    @django.test.tag("delete")
-    def test_delete_model_headers_forbidden(self):
+    def default_view_function(
+        self,
+        request: HttpRequest,
+        path_parameters: Optional[BaseModel],
+        query_parameters: Optional[BaseModel],
+        request_body: Optional[BaseModel],
+    ) -> Model:
         """
-        Tests the forbidden headers scenarios.
+        Default implementation of the view function for the view. This method creates
+        a new instance of the model by calling the `init_model` method, sets the
+        instance attributes based on the request body, calls the pre-save hook, saves
+        the instance, and calls the post-save hook.
 
-        Executes subtests combining various `ok` path parameters and `forbidden` headers to verify the correct
-        handling and response output under forbidden conditions. Each combination of parameters is tested.
+        Note:
+            If the request body contains many-to-many fields, they are set after saving
+            the instance to ensure that the instance exists in the database before setting
+            the many-to-many relationships.
         """
-        self.view_test_manager.test_view_headers_forbidden(
-            test_case=self.model_viewset_test_case,
-            on_completion=self.on_failed_request,
-        )
+        instance = self.init_model(request, path_parameters)
 
-    @django.test.tag("delete")
-    def test_delete_model_path_parameters_not_found(self):
+        m2m_fields_to_set = []
+        if request_body:
+            for field, value in request_body.dict().items():
+                if isinstance(instance._meta.get_field(field), ManyToManyField):
+                    m2m_fields_to_set.append((field, value))
+                else:
+                    setattr(instance, field, value)
+
+        self.pre_save(request, instance)
+        instance.save()
+        self.post_save(request, instance)
+
+        for field, value in m2m_fields_to_set:
+            getattr(instance, field).set(value)
+
+        return instance
+
+    def set_api_viewset_class(self, api_viewset_class: Type["APIViewSet"]) -> None:
         """
-        Tests the not found path parameter scenarios.
+        Bind the view to a viewset class.
 
-        Executes subtests combining various `not_found` path parameters and `ok` headers to verify the correct
-        handling and response output under not found conditions. Each combination of parameters is tested.
+        This method sets the model and path parameters type based on the viewset class,
+        and assigns the request body and response body from the viewset class's
+        `default_request_body` and `default_response_body`, respectively, if they are
+        not already set.
+
+        Note:
+            This method is called internally and automatically by the viewset when
+            defining views as class attributes. It should not be called manually.
         """
-        self.view_test_manager.test_view_path_parameters_not_found(
-            test_case=self.model_viewset_test_case,
-            on_completion=self.on_failed_request,
-        )
+        super().set_api_viewset_class(api_viewset_class)
+
+        if self.request_body is None:
+            self.request_body = api_viewset_class.default_request_body
+
+        if self.response_body is None:
+            self.response_body = api_viewset_class.default_response_body
```

### Comparing `django_ninja_crud-0.4.1/pyproject.toml` & `django_ninja_crud-0.5.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,65 +1,68 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "django-ninja-crud"
-version = "0.4.1"
-description = "Declarative CRUD Views & Tests with Django Ninja."
+version = "0.5.0"
+description = "Declarative Endpoints & Tests for RESTful APIs with Django Ninja."
 authors = ["Hicham Bakri <hicham.bakri76@gmail.com>"]
 maintainers = ["Hicham Bakri <hicham.bakri76@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/hbakri/django-ninja-crud"
 license = "MIT"
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Development Status :: 4 - Beta",
-    "Topic :: Software Development :: Libraries :: Application Frameworks",
-    "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Testing",
     "Topic :: Software Development",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python",
     "Framework :: Django :: 3.2",
     "Framework :: Django :: 4.1",
     "Framework :: Django :: 4.2",
+    "Framework :: Django :: 5.0",
     "Framework :: Django",
     "Typing :: Typed",
 ]
 packages = [{ include = "ninja_crud" },]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
-Django = ">=3.2"
-django-ninja = ">=0.21"
+django = ">=3.2"
+django-ninja = ">=1.0"
+django-rest-testing = { version = ">=0.1", optional = true }
+
+[tool.poetry.extras]
+testing = ["django-rest-testing"]
 
 [tool.poetry.group.dev.dependencies]
 coverage = "^6.5.0"
 pre-commit = "^2.20.0"
 pydoc-markdown = "^4.8.2"
 pyyaml = "^6.0.1"
 python-frontmatter = "^1.0.1"
 
-[tool.ruff]
+[tool.ruff.lint]
 select = [
     "E",  # pycodestyle errors
     "W",  # pycodestyle warnings
     "F",  # pyflakes
     "I",  # isort
     "C",  # flake8-comprehensions
     "B",  # flake8-bugbear
     "UP", # pyupgrade
 ]
 ignore = [
     "E501",  # line too long, handled by black
     "B008",  # do not perform function calls in argument defaults
 ]
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 known-local-folder = ["ninja_crud", "tests", "examples"]
```

### Comparing `django_ninja_crud-0.4.1/PKG-INFO` & `django_ninja_crud-0.5.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,80 +1,106 @@
 Metadata-Version: 2.1
 Name: django-ninja-crud
-Version: 0.4.1
-Summary: Declarative CRUD Views & Tests with Django Ninja.
+Version: 0.5.0
+Summary: Declarative Endpoints & Tests for RESTful APIs with Django Ninja.
 Home-page: https://github.com/hbakri/django-ninja-crud
 License: MIT
 Author: Hicham Bakri
 Author-email: hicham.bakri76@gmail.com
 Maintainer: Hicham Bakri
 Maintainer-email: hicham.bakri76@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Testing
 Classifier: Typing :: Typed
-Requires-Dist: Django (>=3.2)
-Requires-Dist: django-ninja (>=0.21)
+Provides-Extra: testing
+Requires-Dist: django (>=3.2)
+Requires-Dist: django-ninja (>=1.0)
+Requires-Dist: django-rest-testing (>=0.1) ; extra == "testing"
 Description-Content-Type: text/markdown
 
 # Django Ninja CRUD
 [![Tests](https://github.com/hbakri/django-ninja-crud/actions/workflows/tests.yml/badge.svg)](https://github.com/hbakri/django-ninja-crud/actions)
 [![Coverage](https://img.shields.io/codecov/c/github/hbakri/django-ninja-crud/main.svg?label=coverage&logo=codecov&logoColor=white)](https://codecov.io/gh/hbakri/django-ninja-crud)
 [![PyPI version](https://img.shields.io/pypi/v/django-ninja-crud?color=blue&logo=pypi&logoColor=white)](https://pypi.org/project/django-ninja-crud/)
 [![Downloads](https://static.pepy.tech/badge/django-ninja-crud/month)](https://pepy.tech/project/django-ninja-crud)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
+[![MyPy](https://img.shields.io/badge/mypy-checked-blue.svg)](https://github.com/python/mypy)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 ![Django Ninja CRUD](https://raw.githubusercontent.com/hbakri/django-ninja-crud/main/docs/assets/images/django-ninja-crud-cover.png)
 
-Django Ninja CRUD is a [declarative](https://en.wikipedia.org/wiki/Declarative_programming), powerful, and yet opinionated framework that simplifies the development of **CRUD** ([**C**reate, **R**ead, **U**pdate, **D**elete](https://en.wikipedia.org/wiki/Create,_read,_update_and_delete)) views and tests with [Django Ninja](https://github.com/vitalik/django-ninja).
-It promotes best practices for efficient, robust endpoint creation, allowing you to focus on what matters most: solving real problems.
-Initially inspired by DRF's [ModelViewSet](https://www.django-rest-framework.org/api-guide/viewsets/#modelviewset), Django Ninja CRUD evolved to address its limitations, adopting a [composition-over-inheritance](https://en.wikipedia.org/wiki/Composition_over_inheritance) approach to achieve true modularity – a foundational step towards a broader declarative interface for endpoint creation.
+> [!IMPORTANT]
+> With the release of version `0.5`, Django Ninja CRUD introduces significant
+> and breaking changes. Users are strongly advised to pin their requirements to the
+> appropriate version to ensure compatibility with their projects.
+
+Django Ninja CRUD is a powerful, [declarative](https://en.wikipedia.org/wiki/Declarative_programming), and yet a little bit opinionated framework that
+simplifies the development of **CRUD** ([**C**reate, **R**ead, **U**pdate, **D**elete](https://en.wikipedia.org/wiki/Create,_read,_update_and_delete))
+endpoints with [Django Ninja](https://github.com/vitalik/django-ninja), and also
+provides a declarative scenario-based way for testing these endpoints with
+[Django REST Testing](https://github.com/hbakri/django-rest-testing) _(the little brother of this package)_ 🐣.
+
+It allows you to define common endpoints as class-based views and customize them to
+conform to your project's conventions with ease, and also create easily your own
+custom views and declare them alongside the provided CRUD views, fostering modularity
+and extensibility. This package promotes focusing on what matters most:
+**solving real problems**, not reinventing the wheel all over your project.
+
+Initially inspired by DRF's [ModelViewSet](https://www.django-rest-framework.org/api-guide/viewsets/#modelviewset),
+Django Ninja CRUD evolved to address its limitations, adopting a
+[composition-over-inheritance](https://en.wikipedia.org/wiki/Composition_over_inheritance)
+approach to achieve true modularity – a foundational step towards a broader declarative
+interface for endpoint creation.
+
+Key challenges with inheritance-based viewsets:
+- **Unicity of CRUD endpoints per model**: Django Ninja CRUD allows you to define multiple endpoints for the same model, enabling versioning or alternative representations.
+- **Customization inflexibility**: Instead of overriding methods on a monolithic class, you can customize individual views through composition and configuration.
+- **Implicit relations within inheritance hierarchies**: Composition decouples views, reducing dependencies and promoting reusability.
+- **Lack of modularity for new endpoints**: Adding custom endpoints no longer requires subclassing the entire viewset, making it easier to introduce new functionality incrementally.
 
 ## ✨ Key Features
-- **Purely Declarative**: Embrace an approach where defining views and tests is a matter of declaring what you want, not how to achieve it.
-- **Unmatched Modularity**: Tailor your viewsets with the desired CRUD views and customize each view's behavior with ease. Extend the flexibility by creating your own subclasses of the provided views and tests.
-- **Powerful Testing Framework**: Leverage a matrix-based testing framework for defining diverse test scenarios declaratively.
-- **Focus on What Matters**: Spend more time solving real-world problems and less on CRUD boilerplate.
-
-Its blend of declarative syntax, modularity, and powerful testing capabilities sets a new standard for developers seeking efficiency and precision.
+- **Purely Declarative**: Define views and tests by declaring what you want, not how to do it.
+- **Unmatched Modularity**: Tailor your viewsets with desired CRUD views, customize each view's behavior.
+- **Easy to Extend**: Create your own custom views and use them alongside the provided CRUD views as reusable components.
+- **Scenario-based Testing Framework**: Leverage a scenario-based testing framework for defining diverse test cases declaratively and concisely.
+- **Focus on What Matters**: Spend more time solving real-world problems and less on common and repetitive tasks.
 
 > **Django Ninja CRUD is not just a tool; it's a paradigm shift in Django web application development and testing.**
 
 ## 📝 Requirements
 
-![Python versions](https://img.shields.io/pypi/pyversions/django-ninja-crud.svg?color=306998&label=python&logo=python&logoColor=white)
-![Django versions](https://img.shields.io/badge/3.2%20|%204.1%20|%204.2%20|%205.0b1-blue?color=0C4B33&label=django&logo=django&logoColor=white)
-![Django Ninja versions](https://img.shields.io/badge/0.21%20|%200.22%20|%201.0-blue?color=black&label=django-ninja&logo=fastapi&logoColor=white)
+[![Python versions](https://img.shields.io/pypi/pyversions/django-ninja-crud.svg?color=306998&label=python&logo=python&logoColor=white)](https://github.com/python/cpython)
+[![Django versions](https://img.shields.io/badge/3.2_|_4.1_|_4.2_|_5.0-blue?color=0C4B33&label=django&logo=django&logoColor=white)](https://github.com/django/django)
+[![Django Ninja versions](https://img.shields.io/badge/1.0_|_1.1-blue?color=black&label=django-ninja&logo=fastapi&logoColor=white)](https://github.com/vitalik/django-ninja)
 
 ## ⚒️ Installation
 ```bash
-pip install django-ninja-crud
+pip install django-ninja-crud[testing]
 ```
 For more information, see the [installation guide](https://django-ninja-crud.readme.io/docs/02-installation).
 
-## 👨‍🎨 Example
-### Usage
+## 🌞 How It Works
+
 Let's imagine you're building a system for a university and you have a model called `Department`. Each department in your university has a unique title.
 
 ```python
 # examples/models.py
 from django.db import models
 
 class Department(models.Model):
@@ -93,107 +119,171 @@
 class DepartmentOut(Schema):
     id: int
     title: str
 ```
 
 The `DepartmentIn` schema defines what data we need when creating or updating a department. The `DepartmentOut` schema defines what data we'll provide when retrieving a department.
 
-Now, here comes the power of Django Ninja CRUD. With it, you can set up the **CRUD** operations for the `Department` model with just a few lines of code:
+Now, here comes the power of the package. With it, you can set up the **CRUD**
+operations for the `Department` model with just a few lines of code:
 
 ```python
 # examples/views/department_views.py
+from typing import List
 from django.http import HttpRequest
-from ninja import Router
+from ninja import NinjaAPI
 from ninja_crud import views, viewsets
 
 from examples.models import Department
 from examples.schemas import DepartmentIn, DepartmentOut
 
-router = Router()
+api = NinjaAPI()
 
 
-class DepartmentViewSet(viewsets.ModelViewSet):
+class DepartmentViewSet(viewsets.APIViewSet):
+    api = api
     model = Department
-    default_input_schema = DepartmentIn
-    default_output_schema = DepartmentOut
-
-    list_view = views.ListModelView()
-    create_view = views.CreateModelView()
-    retrieve_view = views.RetrieveModelView()
-    update_view = views.UpdateModelView()
-    delete_view = views.DeleteModelView()
-
 
-# The register_routes method must be called to register the routes
-DepartmentViewSet.register_routes(router)
+    list_departments = views.ListView(
+        response_body=List[DepartmentOut]
+    )
+    create_department = views.CreateView(
+        request_body=DepartmentIn,
+        response_body=DepartmentOut,
+    )
+    read_department = views.ReadView(
+        response_body=DepartmentOut
+    )
+    update_department = views.UpdateView(
+        request_body=DepartmentIn,
+        response_body=DepartmentOut,
+    )
+    delete_department = views.DeleteView()
 
 
 # Beyond the CRUD operations managed by the viewset,
-# the router can be used in the standard Django Ninja way
-@router.get("/statistics/", response=dict)
-def retrieve_department_statistics(request: HttpRequest):
+# the api or router can be used in the standard Django Ninja way
+@api.get("/statistics/", response=dict)
+def get_department_statistics(request: HttpRequest):
     return {"total": Department.objects.count()}
 ```
 
-### Testing
-A key advantage of this package is that it makes your views easy to test. Once you've set up your **CRUD** operations, you can write tests to ensure they're working as expected. Here's an example of how you might test the `Department` operations:
+And if your viewset is as simple as the one above, you can leverage the `APIViewSet`
+class to define it in a more concise way, with default request and response bodies:
+```python
+# examples/views/department_views.py
+from ninja import NinjaAPI
+from ninja_crud import views, viewsets
+
+from examples.models import Department
+from examples.schemas import DepartmentIn, DepartmentOut
+
+api = NinjaAPI()
+
+
+class DepartmentViewSet(viewsets.APIViewSet):
+    api = api
+    model = Department
+    default_request_body = DepartmentIn
+    default_response_body = DepartmentOut
+
+    list_departments = views.ListView()
+    create_department = views.CreateView()
+    read_department = views.ReadView()
+    update_department = views.UpdateView()
+    delete_department = views.DeleteView()
+```
+
+## ☔️ Scenario-based Testing
+
+Django Ninja CRUD integrates seamlessly with [Django REST Testing](https://github.com/hbakri/django-rest-testing),
+and ensures comprehensive coverage and robust validation of your CRUD endpoints. At
+first, the testing framework was part of this package, but it was later extracted
+to its own package to allow for more flexibility and to be used with other Django
+REST frameworks than Django Ninja.
+
+With this package, you can:
+- **Declaratively Define Test Scenarios**: Specify expected request and response details for each scenario, making your tests self-documenting and easy to understand.
+- **Test Diverse Conditions**: Validate endpoint behaviors under various conditions, including valid and invalid inputs, nonexistent resources, and custom business rules.
+- **Enhance Clarity and Maintainability**: Break tests into modular, manageable units, improving code organization and reducing technical debt.
+- **Ensure Comprehensive Coverage**: Rigorously test your endpoints, leaving no stone unturned, thanks to the scenario-based approach.
+
+To handle exceptions like `ObjectDoesNotExist` and return appropriate responses in your
+tests, you can define an exception handler like this:
 
 ```python
-# examples/tests/test_department_views.py
-from ninja_crud import testing
+# examples/exception_handlers.py
+from ninja import NinjaAPI
+from django.core.exceptions import ObjectDoesNotExist
+
+api = NinjaAPI()
+
+
+@api.exception_handler(ObjectDoesNotExist)
+def handle_object_does_not_exist(request, exc):
+    return api.create_response(
+        request,
+        {"message": "ObjectDoesNotExist", "detail": str(exc)},
+        status=404,
+    )
+
+# ... other exception handlers
+```
+
+Now, you can write tests for your CRUD views using the scenario-based testing framework:
 
+```python
+# examples/tests/test_department_views.py
 from examples.models import Department
-from examples.views.department_views import DepartmentViewSet
+from examples.schemas import DepartmentOut
 
+from ninja_crud.testing import APITestCase, APIViewTestScenario
 
-class TestDepartmentViewSet(testing.viewsets.ModelViewSetTestCase):
-    model_viewset_class = DepartmentViewSet
-    base_path = "api/departments"
+
+class TestDepartmentViewSet(APITestCase):
+    department: Department
 
     @classmethod
     def setUpTestData(cls):
-        cls.department_1 = Department.objects.create(title="department-1")
-        cls.department_2 = Department.objects.create(title="department-2")
+        cls.department = Department.objects.create(title="department")
 
-    @property
-    def path_parameters(self):
-        return testing.components.PathParameters(
-            ok={"id": self.department_1.id},
-            not_found={"id": 9999}
+    def test_read_department(self):
+        self.assertScenariosSucceed(
+            method="GET",
+            path="/api/departments/{id}",
+            scenarios=[
+                APIViewTestScenario(
+                    path_parameters={"id": self.department.id},
+                    expected_response_status=200,
+                    expected_response_body_type=DepartmentOut,
+                    expected_response_body={
+                        "id": self.department.id,
+                        "title": self.department.title,
+                    },
+                ),
+                APIViewTestScenario(
+                    path_parameters={"id": 9999},
+                    expected_response_status=404,
+                ),
+            ],
         )
-
-    @property
-    def payloads(self):
-        return testing.components.Payloads(
-            ok={"title": "department-3"},
-            bad_request={},
-            conflict={"title": self.department_2.title},
-        )
-
-    test_list_view = testing.views.ListModelViewTest()
-    test_create_view = testing.views.CreateModelViewTest(payloads)
-    test_retrieve_view = testing.views.RetrieveModelViewTest(path_parameters)
-    test_update_view = testing.views.UpdateModelViewTest(path_parameters, payloads)
-    test_delete_view = testing.views.DeleteModelViewTest(path_parameters)
-
-    # You can then add additional tests as needed
-    def test_retrieve_department_statistics(self):
-        response = self.client.get(f"{self.base_path}/statistics/")
-        self.assertEqual(response.status_code, 200)
-        ... # Additional assertions
 ```
 
+By combining Django Ninja CRUD's declarative views with Django REST Testing's
+scenario-based testing capabilities, you can confidently build and maintain robust,
+well-tested RESTful APIs with ease.
+
 ## 📚 Documentation
 For more information, see the [documentation](https://django-ninja-crud.readme.io/).
 
 ## 🫶 Support
-First and foremost, a heartfelt thank you for taking an interest in this project. If it has been helpful to you or you believe in its potential, kindly consider giving it a star on GitHub. Such recognition not only fuels my drive to maintain and improve this work but also makes it more visible to new potential users and contributors.
+First and foremost, a heartfelt thank you to the 400+ stargazers who have shown their support for this project. Your recognition and belief in its potential fuel my drive to maintain and improve this work, making it more visible to new potential users and contributors.
 
-![GitHub Repo stars](https://img.shields.io/github/stars/hbakri/django-ninja-crud?style=social)
+[![Star History Chart](https://api.star-history.com/svg?repos=hbakri/django-ninja-crud&type=Date)](https://star-history.com/#hbakri/django-ninja-crud&Date)
 
 If you've benefited from this project or appreciate the dedication behind it, consider showing further support. Whether it's the price of a coffee, a word of encouragement, or a sponsorship, every gesture adds fuel to the open-source fire, making it shine even brighter. ✨
 
 [![Sponsor](https://img.shields.io/badge/sponsor-donate-pink?logo=github-sponsors&logoColor=white)](https://github.com/sponsors/hbakri)
-[![Buy me a coffee](https://img.shields.io/badge/buy%20me%20a%20coffee-donate-pink?logo=buy-me-a-coffee&logoColor=white)](https://www.buymeacoffee.com/hbakri)
+[![Buy me a coffee](https://img.shields.io/badge/buy_me_a_coffee-donate-pink?logo=buy-me-a-coffee&logoColor=white)](https://www.buymeacoffee.com/hbakri)
 
 Your kindness and support make a world of difference. Thank you! 🙏
```

