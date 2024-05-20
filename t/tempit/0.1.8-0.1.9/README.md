# Comparing `tmp/tempit-0.1.8.tar.gz` & `tmp/tempit-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tempit-0.1.8.tar", last modified: Fri May 17 15:01:48 2024, max compression
+gzip compressed data, was "tempit-0.1.9.tar", last modified: Mon May 20 07:12:46 2024, max compression
```

## Comparing `tempit-0.1.8.tar` & `tempit-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 15:01:48.619592 tempit-0.1.8/
--rw-rw-rw-   0        0        0     1068 2024-05-10 08:37:29.000000 tempit-0.1.8/LICENSE
--rw-rw-rw-   0        0        0     7657 2024-05-17 15:01:48.617586 tempit-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     7002 2024-05-14 09:53:27.000000 tempit-0.1.8/README.md
--rw-rw-rw-   0        0        0       42 2024-05-17 15:01:48.619592 tempit-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      878 2024-05-17 15:00:30.000000 tempit-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-17 15:01:48.593976 tempit-0.1.8/tempit/
--rw-rw-rw-   0        0        0       50 2024-05-09 20:06:13.000000 tempit-0.1.8/tempit/__init__.py
--rw-rw-rw-   0        0        0    11326 2024-05-17 14:59:23.000000 tempit-0.1.8/tempit/core.py
--rw-rw-rw-   0        0        0     5498 2024-05-17 14:59:23.000000 tempit-0.1.8/tempit/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-17 15:01:48.616588 tempit-0.1.8/tempit.egg-info/
--rw-rw-rw-   0        0        0     7657 2024-05-17 15:01:48.000000 tempit-0.1.8/tempit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-05-17 15:01:48.000000 tempit-0.1.8/tempit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 15:01:48.000000 tempit-0.1.8/tempit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-17 15:01:48.000000 tempit-0.1.8/tempit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-17 15:01:48.000000 tempit-0.1.8/tempit.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-17 15:01:48.615587 tempit-0.1.8/tests/
--rw-rw-rw-   0        0        0    12853 2024-05-17 14:59:23.000000 tempit-0.1.8/tests/test_tempit.py
+drwxrwxrwx   0        0        0        0 2024-05-20 07:12:46.045259 tempit-0.1.9/
+-rw-rw-rw-   0        0        0     1068 2024-05-10 08:37:29.000000 tempit-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0    11301 2024-05-20 07:12:46.044261 tempit-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0    10646 2024-05-19 19:08:39.000000 tempit-0.1.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-20 07:12:46.046259 tempit-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      878 2024-05-20 07:07:12.000000 tempit-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 07:12:46.008465 tempit-0.1.9/tempit/
+-rw-rw-rw-   0        0        0       50 2024-05-09 20:06:13.000000 tempit-0.1.9/tempit/__init__.py
+-rw-rw-rw-   0        0        0    16241 2024-05-19 19:40:08.000000 tempit-0.1.9/tempit/core.py
+-rw-rw-rw-   0        0        0     6498 2024-05-19 17:19:40.000000 tempit-0.1.9/tempit/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-20 07:12:46.040262 tempit-0.1.9/tempit.egg-info/
+-rw-rw-rw-   0        0        0    11301 2024-05-20 07:12:45.000000 tempit-0.1.9/tempit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-05-20 07:12:45.000000 tempit-0.1.9/tempit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 07:12:45.000000 tempit-0.1.9/tempit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-20 07:12:45.000000 tempit-0.1.9/tempit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-20 07:12:45.000000 tempit-0.1.9/tempit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-20 07:12:46.038263 tempit-0.1.9/tests/
+-rw-rw-rw-   0        0        0    13028 2024-05-20 07:06:35.000000 tempit-0.1.9/tests/test_tempit.py
```

### Comparing `tempit-0.1.8/LICENSE` & `tempit-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tempit-0.1.8/PKG-INFO` & `tempit-0.1.9/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,30 @@
-Metadata-Version: 2.1
-Name: tempit
-Version: 0.1.8
-Summary: A dead simple time decorator
-Home-page: https://github.com/mcrespoae/tempit
-Author: mcrespoae
-Author-email: info@mariocrespo.es
-Keywords: tempit,time,decorator,performance,concurrency,parallel,benchmark
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Developers
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: joblib==1.4.2
-
 
 # Tempit
 
 ![PyPI](https://img.shields.io/pypi/v/tempit?label=pypi%20package)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/tempit)
 
 ## Overview
 
-Tempit is a Python package designed to simplify the process of measuring the execution time of your functions through a straightforward decorator.
+`tempit` is a Python package designed to simplify the process of measuring the execution time of your functions through a straightforward decorator.
 
 ## Installation
 
-You can install Tempit using pip:
+You can install `tempit` using pip:
 
 ```bash
 pip install tempit
 ```
 
 ## Usage
 
 Tempit decorator should only be used for benchmarking; it is not intended for production code.
 
-Below are some examples demonstrating Tempit's usage:
+Below are some examples demonstrating `tempit`'s usage:
 
 ### Basic Usage
 
 ```python
 from tempit import tempit
 
 @tempit
@@ -75,56 +57,66 @@
 ```text
 ***** tempit data for function my_function_with_args: *****
 Function name: my_function_with_args
         Funcion object: <function my_function_with_args at 0x0000000000000000>
         Args: (1,)
         Kwargs: {'b': 2}
         Run times: 20
-        Mean: 0.7000Âµs
-        Median: 0.8000Âµs
-        Min: 0.4000Âµs
-        Max: 1.0000Âµs
-        Standard deviation: 0.2828Âµs
-        Sum time: 3.5000Âµs
-        Real time: 965.1000Âµs
+        Mean: 0.7000µs
+        Median: 0.8000µs
+        Min: 0.4000µs
+        Max: 1.0000µs
+        Standard deviation: 0.2828µs
+        Sum time: 3.5000µs
+        Real time: 965.1000µs
 ***** End of tempit data. *****
 ```
 
 More examples can be found in the [examples.py](https://github.com/mcrespoae/tempit/blob/main/examples/examples.py) script.
 
 ## Features
 
 - Simplified usage.
 - Accurate measurement of function execution time.
 - Support for functions, methods, `classmethod`, `staticmethods` and classes.
 - Parallel execution mode for performance measurement.
 - Human-readable time formatting.
 - Optional verbose mode for detailed information.
-- Optional recursion checker.
+- Automatic recursion checker.
 
 ## Parameters
 
-Using the decorator @tempit without any parameters executes the function once and displays the execution time. However, you can enhance the experience using the following arguments:
+Using the decorator `@tempit` without any parameters executes the function once and displays the execution time. However, you can enhance the experience using the following arguments:
 
 - `run_times` (int, optional): Specifies the number of function executions. Defaults to 1.
-- `concurrency_mode` (bool, optional): Determines the concurrency mode for the function execution. It uses [joblib](https://pypi.org/project/joblib/) for parallel computing. The  default execution backend is "loky" but if the function is being triggered other than the main thread or main process, the backend will be changed to multithreading to aovid pickle errors. If, for any other reason, fails, the program will try to execute the func run_times non concurrently in the main process. Defaults to True.
+- `concurrency_mode` (bool, optional): Determines the concurrency mode for the function execution. It uses [joblib](https://pypi.org/project/joblib/) for parallel computing. Defaults to True. **Will be changed to False as default in v.0.2.0**
 - `verbose` (bool, optional): Controls whether detailed information is printed after execution. Defaults to False.
-- `check_for_recursion` (bool, optional): Checks for recursion in the decorated function. Please, read the [Recursive functions](#recursive-functions) for detailed information. Defaults to False.
+- `check_for_recursion` ~~(bool, optional):~~ Will be **DEPRECRATED in v0.2.0**. ~~Checks for recursion in the decorated function~~. Please, read the [Recursive functions](#recursive-functions) for detailed information. Defaults to False.
 
-## Recursive functions
+## Best practices
+
+The ideal way to use this package is by applying the decorator to the functions you want to measure and running them side by side to compare the results more easily.
+
+- If you want to measure several times to get an average, you can use the `run_times` parameter.
 
-Measuring the time of recursive functions using decorators can be tricky due to potential verbosity in output. Using recursive functions with this package may result in very verbose output (one per each recursive call plus the original one), making it difficult to read.
+- For more precise time execution, it is recommended to set `concurrency_mode` to `False`. Please see the [Concurrency](#concurrency) section to understand the limitations of concurrency.
+
+- Recursive functions should be encapsulated for better benchmarking. Please refer to the [Recursive functions](#recursive-functions) section to to learn more about recursion and `tempit`.
+
+- Avoid decorating classes directly, as a `PicklingError` may occur if the class is then instantiated in another process. For more information, please see the [Decorating classes that could be instantiated in another processes](#decorating-classes-that-could-be-instantiated-in-another-processes) in the [Other Limitations](#other-limitations) section.
+
+## Recursive functions
 
-There are two potential solutions for this issue, [use the recursion detector](#using-the-check_for_recursion-parameter) or [encapsulating the recursive function](#encapsulating-the-recursive-function).
+Measuring the execution time of recursive functions using decorators can be challenging due to potential verbosity in the output. This package offers an automatic recursion detection feature, but it is strongly recommended to use the [encapsulating the recursive function](#encapsulating-the-recursive-function) solution for cleaner, more precise and safer results.
 
-### Using the `check_for_recursion` parameter
+### Using the autio recursion feature
 
-If you're aware that your function utilizes recursion, you can use the `check_for_recursion` parameter.
+The auto recursion feature detects recursion in the decorated function by checking the parent call function. If recursion is found, it will only output the time taken to run the appropriate function, plus an overhead. It is not recommended to rely on this feature intentionally since the collected time data will not be accurate and the process will take longer.
 
-Activating this option has some overhead in performance but it enables users to decorate recursive functions with a clean output.
+This feature is intended for passive use in case the user forgets to encapsulate the recursive function or for non-accurate comparisons.
 
 ```python
 @tempit(run_times=3, concurrent_execution=True, verbose=False, check_for_recursion=True)
 def recursive_func(n):
     if n == 0:
         return 0
     else:
@@ -133,15 +125,15 @@
 
 # Using the check_for_recursion parameter for the tempit decorator recursive function
 result = recursive_func(3)
 ```
 
 ### Encapsulating the recursive function
 
-Another option is to encapsulate the recursive function within another function then, decorate and call the parent function. Here's an example:
+The recommended option is to encapsulate the recursive function within another function then, decorate and call the parent function. Here's an example:
 
 ```python
 @tempit
 def encapsulated_recursive_function(n):
     """A non-verbose wrapper for the recursive function."""
     def recursive_func(n):
         if n == 0:
@@ -153,35 +145,77 @@
 
 # Encapsulating the recursive function
 result = encapsulated_recursive_function(3)
 ```
 
 This approach enhances readability without incurring any performance penalties. However, its main drawback is that users must modify their code to measure this type of function.
 
-## Limitations
+## Concurrency
+
+### How concurrency works in timeit
+
+`tempit` uses [joblib](https://pypi.org/project/joblib/) for parallel computing. By default, the execution backend is "loky". If a `PicklingError` occurs while trying to execute the decorated function, `tempit` switches the backend to "threading" and retries the execution. If any other error occurs with "loky" or "threading", `tempit` falls back to sequential execution, discarding the joblib option.
+
+The "threading" backend is chosen if `tempit` is detected to be running outside the MainProcess or MainThread.
+
+The number of workers for any parallel execution is `num_processors - 1`. While this may not always be the optimal approach (especially for multithreading with large I/O operations), simplicity of use has been prioritized over complexity for this decorator.
+
+Additionally, if the `run_times` parameter exceeds `num_processors - 1`, it will be downsized to match the number of available processors minus one to maximize parallelization. Finally, if `tempit` detects that it is running in concurrency mode and finds that the downsized `run_times` is equal to 1, `tempit` falls back to sequential execution, discarding the joblib option.
+
+### Concurrency caveats
+
+There are some caveats when using parallel computing. Creating a process or thread incurs overhead, so it's normal to find that for very low CPU-intensive functions, the concurrent mode may be slower than the sequential one. However, as the functions become more CPU-intensive, concurrency usually results in faster execution times.
+
+That being said, timings measured when using concurrent executions may not be as accurate as those in sequential mode.
+
+## Other limitations
+
+### Decorating classes that could be instantiated in another processes
 
 While this package generally delivers excellent performance and reliability, it's essential to be aware of certain scenarios where using the `tempit` decorator could lead to unexpected behavior or crashes:
 
-- If a class is decorated with tempit, and subsequently, a new process is spawned after creating an instance of the class, calling a method within the newly created process may result in a `PicklingError`.
+- If a class is decorated with `tempit`, and subsequently, a new process is spawned after creating an instance of the class, calling a method within the newly created process may result in a `PicklingError`.
 
 This limitation arises due to how Python's pickling mechanism handles decorated classes and processes. When a decorated class instance is pickled for use in a separate process, inconsistencies in object references can occur, leading to pickling failures.
 
-To mitigate this issue, consider redesigning your application logic to avoid decorating classes that are used within processes spawned later in the program's execution. Alternatively, explore alternative serialization approaches or use dill or other serialization libraries that offer more robust handling of complex object hierarchies.
+To mitigate this issue, avoid decorating classes that will be used in processes spawned later in the program's execution.
+
+### Zero values
+
+In some rare cases where multiple recursively decorated functions are called nested within each other, `tempit` may return two values, with one being zero.
+
+## Error managment and warnings
+
+### Errors
+
+If an error occurs while executing the decorated function in sequential mode or within a recursively decorated function, the error will be propagated to the user's function.
+
+### Warnings
+
+- Deprecation warnings will be added before removing a feature.
+
+- Decorated classes will rise a warning to inform the user about the potential issues described in [Decorating classes that could be instantiated in another processes](#decorating-classes-that-could-be-instantiated-in-another-processes) section.
+
+- If the `run_times` parameter exceeds `num_processors - 1`, it will be downsized to match the number of available processors minus one to maximize parallelization.
+
+- If recursion has been detected, a warning will be promted. If so, please, go to [Recursive functions](#recursive-functions).
 
 ## Contributing
 
 Contributions are welcome! Please follow these guidelines when contributing:
 
 1. Fork the repository.
 2. Use `make install` to install all depedencies.
 3. Create a new branch for your changes.
 4. Implement your changes and commit them.
 5. Push your changes to your forked repository.
 6. Submit a pull request.
 
+You can also open an issue if you find a bug or have a suggestion.
+
 You can test your code using `make test` and `make example` to trigger the examples. Please, check the [Makefile](https://github.com/mcrespoae/tempit/blob/main/Makefile) to know more about commands.
 
 ## Testing
 
 The package has been thoroughly tested using unittesting. Test cases can be found in the [tests folder](https://github.com/mcrespoae/tempit/tree/main/tests).
 
 ## License
```

### Comparing `tempit-0.1.8/setup.py` & `tempit-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-VERSION = "0.1.8"
+VERSION = "0.1.9"
 setup(
     name="tempit",
     version=VERSION,
     author="mcrespoae",
     author_email="info@mariocrespo.es",
     packages=["tempit"],
     description="A dead simple time decorator",
```

### Comparing `tempit-0.1.8/tempit/core.py` & `tempit-0.1.9/tempit/core.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,44 @@
+import inspect
 import time
+import warnings
+from collections import deque
 from functools import partial, wraps
+from threading import Lock
 from typing import Any, Callable, Dict, List, Tuple
 
-from .utils import print_tempit_values
+from .utils import print_tempit_values, show_error
 
 
 def tempit(
     *args: Any,
     run_times: int = 1,
     concurrent_execution: bool = True,
     verbose: bool = False,
-    check_for_recursion: bool = False,
+    check_for_recursion: bool | None = None,
 ) -> Callable:
     """
     Decorator function that measures the execution time of a given function. It can be called like @tempit or using arguments @tempit(...)
 
     Args:
         args: contains the function to be decorated if no arguments are provided when calling the decorator
         run_times (int, optional): The number of times the function should be executed. Defaults to 1.
         concurrent_execution (bool, optional): This parameter will allow for the concurrent execution of the function using joblib.
                                                The default execution backend is "loky" but if the function is being triggered other than the main thread or main process, the backend will be changed to multithreading.
                                                If the execution of the concurrency fails, it will try to execute the func run_times non concurrently in the main process.
                                                Defaults to True.
         verbose (bool, optional): Whether to print detailed information after execution. Defaults to False.
+        check_for_recursion (bool | None, optional): DEPRECATED. Whether to check if the function is being called recursively. Defaults to None.
 
     Returns:
         Callable: The decorated function if arguments are provided, otherwise a partial function.
 
     Raises:
         RuntimeError: If the concurrency mode fails, the function is executed in the main process.
+        Exception: If the function crashes, it will raise the exception given by the user's function.
 
     Notes:
         - If `run_times` is less than 1, it will be set to 1.
         - If the function is a method, the first argument will be removed from `args_to_print`.
         - If the function is a class method, the first argument will be replaced with the class itself.
         - If the function is a static method, the first argument will be removed.
 
@@ -44,109 +50,147 @@
         @tempit
         def my_function(arg1, arg2):
             # function body
 
         # The decorated function can be used as usual
         result = my_function(arg1_value, arg2_value)
     """
+    if check_for_recursion is not None:
+        warning_msg = "check_for_recursion is deprecated and will be removed in future versions."
+        warnings.warn(warning_msg, DeprecationWarning, stacklevel=2)
 
     def decorator(
-        func: Callable,
-        run_times: int = 1,
-        concurrent_execution: bool = True,
-        verbose: bool = False,
-        check_for_recursion: bool = False,
+        func: Callable, run_times: int = 1, concurrent_execution: bool = True, verbose: bool = False
     ) -> Callable:
+
+        potential_recursion_func_stack: deque[Callable] = deque()
+        is_recursive: bool = False
+        time_wasted_lock: Lock = Lock()
+        time_wasted: float = 0
+
         @wraps(func)
         def tempit_wrapper(*args: Tuple, **kwargs: Dict) -> Any:
-            is_recursive, run_times_final, concurrent_execution_final = check_is_recursive_func(
-                check_for_recursion, func, run_times, concurrent_execution
+            nonlocal potential_recursion_func_stack, is_recursive, time_wasted
+
+            start_time: float = time.perf_counter()
+            run_times_final, concurrent_execution_final, is_recursive = check_is_recursive_func(
+                func, run_times, concurrent_execution, potential_recursion_func_stack
             )
-            callable_func, args, args_to_print = extract_callable_and_args_if_method(func, *args)
+            callable_func, args, args_to_print = extract_callable_and_args_if_method(func, *args, **kwargs)
+
+            if is_recursive:  # If the function is recursive, it will be executed directly
+                with time_wasted_lock:  # Update the time non-ocurring in the function execution
+                    end_time: float = time.perf_counter()
+                    time_wasted += end_time - start_time
+                result: Any = run_func_recursive(func, *args, **kwargs)
+                potential_recursion_func_stack.pop()
+                return result
+
             result, total_times, real_time = function_execution(
                 callable_func,
                 run_times_final,
                 concurrent_execution_final,
                 *args,
                 **kwargs,
             )
-            if not is_recursive:
+
+            total_times: List[float] = update_total_times(total_times, time_wasted)
+
+            potential_recursion_func_stack.pop()
+            if not potential_recursion_func_stack:  # The function is not recursive at the moment, so it will be printed
                 print_tempit_values(
-                    run_times_final, verbose, callable_func, total_times, real_time, *args_to_print, **kwargs
+                    run_times_final,
+                    verbose,
+                    callable_func,
+                    total_times,
+                    real_time,
+                    *args_to_print,
+                    **kwargs,
                 )
+
             return result
 
         return tempit_wrapper
 
     if args:  # If arguments are not provided, return a decorator
-        return decorator(
-            *args,
-            run_times=run_times,
-            concurrent_execution=concurrent_execution,
-            verbose=verbose,
-            check_for_recursion=check_for_recursion,
-        )
+        return decorator(*args)
 
     else:  # Otherwise, return a partial function
-        return partial(
-            decorator,
-            run_times=run_times,
-            concurrent_execution=concurrent_execution,
-            verbose=verbose,
-            check_for_recursion=check_for_recursion,
-        )
+        return partial(decorator, run_times=run_times, concurrent_execution=concurrent_execution, verbose=verbose)
+
+
+def update_total_times(total_times: List[float], time_wasted: float) -> List[float]:
+    """
+    Updates the total times by subtracting the average time wasted from each time if the function was recursive.
+    Args:
+        total_times (List[float]): A list of total times for each run.
+        time_wasted (float): The total time wasted. Only used if the function is recursive.
+    Returns:
+        List[float]: A list of updated total times.
+    """
+    if time_wasted == 0:  # Early return
+        return total_times
+    time_wasted_avg: float = time_wasted / len(total_times)
+    # The max (x, 0) is due to the fact that the time wasted can be negative if we are analyzing a decorated function inside a decorated function
+    return [max(x - time_wasted_avg, 0) for x in total_times]
 
 
 def check_is_recursive_func(
-    check_for_recursion: bool, func: Callable, run_times: int, concurrent_execution: bool
-) -> Tuple[bool, int, bool]:
+    func: Callable, run_times: int, concurrent_execution: bool, potential_recursion_func_stack: deque[Callable]
+) -> Tuple[int, bool, bool]:
     """
     Checks if the function is being called recursively.
     Returns:
-        Tuple[bool, int, bool]: A tuple containing True if the function is being called recursively, False otherwise.
-        The second element is the number of times the function has been called, and the third element is a boolean indicating if the function has crashed.
+        Tuple[List[Callable], int, bool]: A tuple containing the potential recursive function stack to check if the function is being called recursively, None otherwise.
+        The second element is the run_times parameter, and the third element is a boolean indicating if concurrent_execution is enabled.
     """
 
-    if check_for_recursion:
-        import sys
-        from inspect import getframeinfo
+    if potential_recursion_func_stack and potential_recursion_func_stack[-1] == func:
+        potential_recursion_func_stack.append(func)
+        # Check if the function is being called recursively by checking the object identity. This is way faster than using getFrameInfo
+        warning_msg = "Recursive function detected. This process may be slow. Consider wrapping the recursive function in another function and applying the @tempit decorator to the new function."
+        warnings.warn(warning_msg, stacklevel=3)
+        return 1, False, True
+    potential_recursion_func_stack.append(func)
+    return run_times, concurrent_execution, False
 
-        func_name = func.__name__
-        func_filename = ""
-        if hasattr(func, "__code__"):
-            func_filename = func.__code__.co_filename
-        frame = getframeinfo(sys._getframe(2), context=0)
-        if frame.function == func_name and func_filename == frame.filename:
-            return True, 1, False
-    return False, run_times, concurrent_execution
 
-
-def extract_callable_and_args_if_method(func, *args) -> Tuple[Callable, Tuple, Tuple]:
+def extract_callable_and_args_if_method(func: Callable, *args: Tuple, **kwargs: Dict) -> Tuple[Callable, Tuple, Tuple]:
     """
     Extracts the callable function and arguments from a given function, if it is a method.
     Args:
         func (Callable): The function to extract the callable from.
-        args: Variable length argument list.
+        *args: Variable length argument list.
+        **kwargs (Dict): The keyword arguments to be passed to the function.
     Returns:
         Tuple[Callable, Tuple, Tuple]: A tuple containing the extracted callable function, the modified arguments,
         and the arguments to be printed.
-    Raises:
-        None
     """
-    callable_func = func
-    args_to_print = args
-    is_method = hasattr(args[0], func.__name__) if args else False
+
+    callable_func: Callable = func
+    args_to_print: Tuple = args
+    is_method: bool = hasattr(args[0], func.__name__) if args else False
+    if inspect.isclass(func):
+        # TODO: Add proper support for class decorators
+        # This is calling the class constructor directly. Move it into the execution function. I think it shuold be func.__init__(*args, **kwargs)
+        # class_wrapper = func.__init__(args, kwargs)  # prettier-ignore
+
+        # func.__new__ = class_wrapper
+        # callable_func = func
+        # if isinstance(func, type):
+        warning_msg = "Class decoration detected. It is not recommended to use @tempit with classes that will be triggered from a new process, as it will raise a pickle exception."
+        warnings.warn(warning_msg, stacklevel=3)
+
     if is_method:
         args_to_print = args[1:]
         if isinstance(func, classmethod):
             args = (args[0].__class__,) + args[1:]  # type: ignore
             callable_func = func.__func__
         elif isinstance(func, staticmethod):
             args = args[1:]
-
     return callable_func, args, args_to_print
 
 
 def function_execution(
     callable_func: Callable, run_times: int, concurrent_execution: bool, *args: Tuple, **kwargs: Dict
 ) -> Tuple[Any, List[float], float]:
     """
@@ -157,108 +201,134 @@
         concurrency_mode (str): The concurrency mode for executing the function.
         *args (Tuple): The positional arguments to be passed to the function.
         **kwargs (Dict): The keyword arguments to be passed to the function.
     Returns:
         Tuple[Any, List[float], float]: A tuple containing the result of the function,
         a list of execution times for each run, and the total real time taken.
     """
+    if inspect.isclass(callable_func):
+        pass  # TODO: Add proper support for class decorators
+
     if run_times < 1:
         run_times = 1
-    start_time = time.perf_counter()
+    start_time: float = time.perf_counter()
     if run_times > 1 and concurrent_execution:
         try:
-            result, total_times = tempit_with_concurrency(callable_func, run_times, *args, **kwargs)
+            result, total_times = run_func_concurrency(callable_func, run_times, *args, **kwargs)
         except RuntimeError as e:
-            print(e)
-            result, total_times = tempit_main_process(callable_func, run_times, *args, **kwargs)
+            show_error(e, filename=__file__)
+            result, total_times = run_func_sequential(callable_func, run_times, *args, **kwargs)
     else:
-        result, total_times = tempit_main_process(callable_func, run_times, *args, **kwargs)
-    end_time = time.perf_counter()
-    real_time = end_time - start_time
-
+        result, total_times = run_func_sequential(callable_func, run_times, *args, **kwargs)
+    end_time: float = time.perf_counter()
+    real_time: float = end_time - start_time
     return result, total_times, real_time
 
 
-def tempit_main_process(func: Callable, run_times: int, *args: Tuple, **kwargs: Dict) -> Tuple[Any, List[float]]:
+def run_func_recursive(func: Callable, *args: Tuple, **kwargs: Dict) -> Any:
     """
-    Run and measure the execution time of a function in the main process. It also returns the value of the function return and the execution times.
+    Run the given function that has been determined as recursive with the provided arguments and keyword arguments.
+    Args:
+        func (Callable): The function to be executed.
+        *args (Tuple): Positional arguments to be passed to the function.
+        **kwargs (Dict): Keyword arguments to be passed to the function.
+    Returns:
+        Any: The result of the function execution.
+    Note:
+        This function does not catch any errors.
+    """
+    # Don't try to catch any errors here since the problem should be handled in the user's function or is already handled in the concurrent executor
+    return func(*args, **kwargs)
+
+
+def run_func_sequential(func: Callable, run_times: int, *args: Tuple, **kwargs: Dict) -> Tuple[Any, List[float]]:
+    """
+    Run and measure the execution time of a function sequentially. It also returns the value of the function return and the execution times.
     Args:
         func (Callable): The function to be executed.
         run_times (int): The number of times the function should be executed.
         *args (Tuple): The positional arguments to be passed to the function.
         **kwargs (Dict): The keyword arguments to be passed to the function.
     Returns:
         Tuple[Any, List[float]]: A tuple containing the result of the function and a list of execution times for each run.
     """
 
     total_times: List[float] = []
     for _ in range(run_times):
         start_time: float = time.perf_counter()
-        try:
-            result: Any = func(*args, **kwargs)
-        except Exception as e:
-            print(e)
-        finally:
-            end_time: float = time.perf_counter()
-            total_times.append(end_time - start_time)
+        # Don't try to catch any errors here since the problem should be handled in the user's function
+        result: Any = func(*args, **kwargs)
+        end_time: float = time.perf_counter()
+        total_times.append((end_time - start_time))
     return result, total_times
 
 
-def tempit_with_concurrency(func: Callable, run_times: int, *args: Tuple, **kwargs: Dict) -> Tuple[Any, List[float]]:
+def run_func_concurrency(func: Callable, run_times: int, *args: Tuple, **kwargs: Dict) -> Tuple[Any, List[float]]:
     """
     Executes a given function concurrently a specified number of times using joblib.
 
     Args:
         func (Callable): The function to be executed.
         run_times (int): The number of times the function should be executed.
         *args (Tuple): The positional arguments to be passed to the function.
         **kwargs (Dict): The keyword arguments to be passed to the function.
 
     Returns:
         Tuple[Any, List[float]]: A tuple containing the result of the function and a list of execution times for each run.
-        If an exception was raised in one of the concurrent tasks, the function will raise a RuntimeError and returns control
+
+    Raises:
+        RuntimeError: If an exception was raised in one of the concurrent tasks. If an exception was raised in one of the concurrent tasks, the function will raise a RuntimeError and returns control
         to the main process, then the function will be executed in the main process non-concurrently.
     """
 
     from multiprocessing import current_process
     from os import cpu_count
+    from pickle import PicklingError
     from threading import current_thread
 
     from joblib import Parallel, delayed
 
-    def run_func(
-        func: Callable,
-        *args: Tuple,
-        **kwargs: Dict,
-    ) -> Tuple[Any, float, bool]:
-
-        has_crashed: bool = False
-        start_time = time.perf_counter()
-        try:
-            result: Any = func(*args, **kwargs)
-        except Exception:
-            has_crashed = True
-            result = None
-        finally:
-            end_time = time.perf_counter()
-            return result, end_time - start_time, has_crashed
-
+    EXCEPTION_MSG: str = (
+        "An exception was raised in one of the concurrent jobs. Trying to execute in the main process non-concurrently."
+    )
     joblib_backend = None  # Default backend for joblib
-    # Rule of thumb, use at least 2 workers or at least the number of cores minus 1.
-    # It is not ideal for multithreading, but it will make good balance
-    workers: int = max(2, cpu_count() - 1) if cpu_count() is not None else 2  # type: ignore
+    # Rule of thumb, use all the cores but 1.
+    # It is not ideal for multithreading with large I/O operations, but it will make good balance
+    workers: int = -2  # This is how joblib says to use all the cores but 1
+    num_cores: int | None = cpu_count()
+    if num_cores:
+        available_cpu_cores = max(1, num_cores - 1)
+        if run_times > available_cpu_cores:
+
+            warning_msg = f"Available cpu cores to use: {available_cpu_cores}. The {run_times} number of runs will be reduced to {available_cpu_cores} in order to maximize parallelism."
+            warnings.warn(warning_msg)
+            run_times = available_cpu_cores
+            if run_times == 1:
+                raise RuntimeError("Run times=1 found while running in concurrency. Switching to sequential execution.")
 
     if current_process().name != "MainProcess" or current_thread().name != "MainThread":
         joblib_backend = "threading"  # If we are running in other than the main process or main thread, use threading instead of multiprocessing
 
-    results: List[Tuple[Any, float, bool]] = Parallel(n_jobs=workers, backend=joblib_backend)(
-        delayed(run_func)(func, *args, **kwargs) for _ in range(run_times)
-    )  # type: ignore
-
-    if any(has_crashed for _, _, has_crashed in results):
-        raise RuntimeError(
-            "An exception was raised in one of the concurrent jobs. Trying to execute in the main process non-concurrently."
-        )
+    try:
+        start_time: float = time.perf_counter()
+        results: List[Tuple[Any, float, bool]] = Parallel(n_jobs=workers, backend=joblib_backend)(
+            delayed(func)(*args, **kwargs) for _ in range(run_times)
+        )  # type: ignore
+        end_time: float = time.perf_counter()
 
-    total_times = [total_time for _, total_time, has_crashed in results if not has_crashed]
-    result = results[0][0]
-    return result, total_times
+    except PicklingError:  # If a pickle error is raised, use threading instead of multiprocessing
+        joblib_backend = "threading"
+        try:
+            start_time: float = time.perf_counter()
+            results: List[Tuple[Any, float, bool]] = Parallel(n_jobs=workers, backend=joblib_backend, prefer="threads")(
+                delayed(func)(*args, **kwargs) for _ in range(run_times)
+            )  # type: ignore
+            end_time: float = time.perf_counter()
+        except Exception:
+            raise RuntimeError(EXCEPTION_MSG)
+
+    except Exception:
+        raise RuntimeError(EXCEPTION_MSG)
+
+    average_runtimes: float = (end_time - start_time) / run_times
+    total_times: List[float] = [average_runtimes] * run_times
+    return results[0], total_times
```

### Comparing `tempit-0.1.8/tempit.egg-info/PKG-INFO` & `tempit-0.1.9/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tempit
-Version: 0.1.8
+Version: 0.1.9
 Summary: A dead simple time decorator
 Home-page: https://github.com/mcrespoae/tempit
 Author: mcrespoae
 Author-email: info@mariocrespo.es
 Keywords: tempit,time,decorator,performance,concurrency,parallel,benchmark
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
@@ -20,29 +20,29 @@
 # Tempit
 
 ![PyPI](https://img.shields.io/pypi/v/tempit?label=pypi%20package)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/tempit)
 
 ## Overview
 
-Tempit is a Python package designed to simplify the process of measuring the execution time of your functions through a straightforward decorator.
+`tempit` is a Python package designed to simplify the process of measuring the execution time of your functions through a straightforward decorator.
 
 ## Installation
 
-You can install Tempit using pip:
+You can install `tempit` using pip:
 
 ```bash
 pip install tempit
 ```
 
 ## Usage
 
 Tempit decorator should only be used for benchmarking; it is not intended for production code.
 
-Below are some examples demonstrating Tempit's usage:
+Below are some examples demonstrating `tempit`'s usage:
 
 ### Basic Usage
 
 ```python
 from tempit import tempit
 
 @tempit
@@ -95,36 +95,46 @@
 
 - Simplified usage.
 - Accurate measurement of function execution time.
 - Support for functions, methods, `classmethod`, `staticmethods` and classes.
 - Parallel execution mode for performance measurement.
 - Human-readable time formatting.
 - Optional verbose mode for detailed information.
-- Optional recursion checker.
+- Automatic recursion checker.
 
 ## Parameters
 
-Using the decorator @tempit without any parameters executes the function once and displays the execution time. However, you can enhance the experience using the following arguments:
+Using the decorator `@tempit` without any parameters executes the function once and displays the execution time. However, you can enhance the experience using the following arguments:
 
 - `run_times` (int, optional): Specifies the number of function executions. Defaults to 1.
-- `concurrency_mode` (bool, optional): Determines the concurrency mode for the function execution. It uses [joblib](https://pypi.org/project/joblib/) for parallel computing. The  default execution backend is "loky" but if the function is being triggered other than the main thread or main process, the backend will be changed to multithreading to aovid pickle errors. If, for any other reason, fails, the program will try to execute the func run_times non concurrently in the main process. Defaults to True.
+- `concurrency_mode` (bool, optional): Determines the concurrency mode for the function execution. It uses [joblib](https://pypi.org/project/joblib/) for parallel computing. Defaults to True. **Will be changed to False as default in v.0.2.0**
 - `verbose` (bool, optional): Controls whether detailed information is printed after execution. Defaults to False.
-- `check_for_recursion` (bool, optional): Checks for recursion in the decorated function. Please, read the [Recursive functions](#recursive-functions) for detailed information. Defaults to False.
+- `check_for_recursion` ~~(bool, optional):~~ Will be **DEPRECRATED in v0.2.0**. ~~Checks for recursion in the decorated function~~. Please, read the [Recursive functions](#recursive-functions) for detailed information. Defaults to False.
 
-## Recursive functions
+## Best practices
+
+The ideal way to use this package is by applying the decorator to the functions you want to measure and running them side by side to compare the results more easily.
+
+- If you want to measure several times to get an average, you can use the `run_times` parameter.
+
+- For more precise time execution, it is recommended to set `concurrency_mode` to `False`. Please see the [Concurrency](#concurrency) section to understand the limitations of concurrency.
 
-Measuring the time of recursive functions using decorators can be tricky due to potential verbosity in output. Using recursive functions with this package may result in very verbose output (one per each recursive call plus the original one), making it difficult to read.
+- Recursive functions should be encapsulated for better benchmarking. Please refer to the [Recursive functions](#recursive-functions) section to to learn more about recursion and `tempit`.
+
+- Avoid decorating classes directly, as a `PicklingError` may occur if the class is then instantiated in another process. For more information, please see the [Decorating classes that could be instantiated in another processes](#decorating-classes-that-could-be-instantiated-in-another-processes) in the [Other Limitations](#other-limitations) section.
+
+## Recursive functions
 
-There are two potential solutions for this issue, [use the recursion detector](#using-the-check_for_recursion-parameter) or [encapsulating the recursive function](#encapsulating-the-recursive-function).
+Measuring the execution time of recursive functions using decorators can be challenging due to potential verbosity in the output. This package offers an automatic recursion detection feature, but it is strongly recommended to use the [encapsulating the recursive function](#encapsulating-the-recursive-function) solution for cleaner, more precise and safer results.
 
-### Using the `check_for_recursion` parameter
+### Using the autio recursion feature
 
-If you're aware that your function utilizes recursion, you can use the `check_for_recursion` parameter.
+The auto recursion feature detects recursion in the decorated function by checking the parent call function. If recursion is found, it will only output the time taken to run the appropriate function, plus an overhead. It is not recommended to rely on this feature intentionally since the collected time data will not be accurate and the process will take longer.
 
-Activating this option has some overhead in performance but it enables users to decorate recursive functions with a clean output.
+This feature is intended for passive use in case the user forgets to encapsulate the recursive function or for non-accurate comparisons.
 
 ```python
 @tempit(run_times=3, concurrent_execution=True, verbose=False, check_for_recursion=True)
 def recursive_func(n):
     if n == 0:
         return 0
     else:
@@ -133,15 +143,15 @@
 
 # Using the check_for_recursion parameter for the tempit decorator recursive function
 result = recursive_func(3)
 ```
 
 ### Encapsulating the recursive function
 
-Another option is to encapsulate the recursive function within another function then, decorate and call the parent function. Here's an example:
+The recommended option is to encapsulate the recursive function within another function then, decorate and call the parent function. Here's an example:
 
 ```python
 @tempit
 def encapsulated_recursive_function(n):
     """A non-verbose wrapper for the recursive function."""
     def recursive_func(n):
         if n == 0:
@@ -153,35 +163,77 @@
 
 # Encapsulating the recursive function
 result = encapsulated_recursive_function(3)
 ```
 
 This approach enhances readability without incurring any performance penalties. However, its main drawback is that users must modify their code to measure this type of function.
 
-## Limitations
+## Concurrency
+
+### How concurrency works in timeit
+
+`tempit` uses [joblib](https://pypi.org/project/joblib/) for parallel computing. By default, the execution backend is "loky". If a `PicklingError` occurs while trying to execute the decorated function, `tempit` switches the backend to "threading" and retries the execution. If any other error occurs with "loky" or "threading", `tempit` falls back to sequential execution, discarding the joblib option.
+
+The "threading" backend is chosen if `tempit` is detected to be running outside the MainProcess or MainThread.
+
+The number of workers for any parallel execution is `num_processors - 1`. While this may not always be the optimal approach (especially for multithreading with large I/O operations), simplicity of use has been prioritized over complexity for this decorator.
+
+Additionally, if the `run_times` parameter exceeds `num_processors - 1`, it will be downsized to match the number of available processors minus one to maximize parallelization. Finally, if `tempit` detects that it is running in concurrency mode and finds that the downsized `run_times` is equal to 1, `tempit` falls back to sequential execution, discarding the joblib option.
+
+### Concurrency caveats
+
+There are some caveats when using parallel computing. Creating a process or thread incurs overhead, so it's normal to find that for very low CPU-intensive functions, the concurrent mode may be slower than the sequential one. However, as the functions become more CPU-intensive, concurrency usually results in faster execution times.
+
+That being said, timings measured when using concurrent executions may not be as accurate as those in sequential mode.
+
+## Other limitations
+
+### Decorating classes that could be instantiated in another processes
 
 While this package generally delivers excellent performance and reliability, it's essential to be aware of certain scenarios where using the `tempit` decorator could lead to unexpected behavior or crashes:
 
-- If a class is decorated with tempit, and subsequently, a new process is spawned after creating an instance of the class, calling a method within the newly created process may result in a `PicklingError`.
+- If a class is decorated with `tempit`, and subsequently, a new process is spawned after creating an instance of the class, calling a method within the newly created process may result in a `PicklingError`.
 
 This limitation arises due to how Python's pickling mechanism handles decorated classes and processes. When a decorated class instance is pickled for use in a separate process, inconsistencies in object references can occur, leading to pickling failures.
 
-To mitigate this issue, consider redesigning your application logic to avoid decorating classes that are used within processes spawned later in the program's execution. Alternatively, explore alternative serialization approaches or use dill or other serialization libraries that offer more robust handling of complex object hierarchies.
+To mitigate this issue, avoid decorating classes that will be used in processes spawned later in the program's execution.
+
+### Zero values
+
+In some rare cases where multiple recursively decorated functions are called nested within each other, `tempit` may return two values, with one being zero.
+
+## Error managment and warnings
+
+### Errors
+
+If an error occurs while executing the decorated function in sequential mode or within a recursively decorated function, the error will be propagated to the user's function.
+
+### Warnings
+
+- Deprecation warnings will be added before removing a feature.
+
+- Decorated classes will rise a warning to inform the user about the potential issues described in [Decorating classes that could be instantiated in another processes](#decorating-classes-that-could-be-instantiated-in-another-processes) section.
+
+- If the `run_times` parameter exceeds `num_processors - 1`, it will be downsized to match the number of available processors minus one to maximize parallelization.
+
+- If recursion has been detected, a warning will be promted. If so, please, go to [Recursive functions](#recursive-functions).
 
 ## Contributing
 
 Contributions are welcome! Please follow these guidelines when contributing:
 
 1. Fork the repository.
 2. Use `make install` to install all depedencies.
 3. Create a new branch for your changes.
 4. Implement your changes and commit them.
 5. Push your changes to your forked repository.
 6. Submit a pull request.
 
+You can also open an issue if you find a bug or have a suggestion.
+
 You can test your code using `make test` and `make example` to trigger the examples. Please, check the [Makefile](https://github.com/mcrespoae/tempit/blob/main/Makefile) to know more about commands.
 
 ## Testing
 
 The package has been thoroughly tested using unittesting. Test cases can be found in the [tests folder](https://github.com/mcrespoae/tempit/tree/main/tests).
 
 ## License
```

### Comparing `tempit-0.1.8/tests/test_tempit.py` & `tempit-0.1.9/tests/test_tempit.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,40 +13,40 @@
 
 class TempitTestClass:
     @tempit()
     def tempit_basic(self):
         time.sleep(0.01)
 
     @tempit
-    def tempit_basic_no_parenthesis(self):
-        time.sleep(0.01)
+    def tempit_basic_no_parenthesis(self, a: int, b: int = 2):
+        return a + b
 
-    @tempit(run_times=5)
+    @tempit(run_times=2)
     def test_tempit_with_concurrency(self):
         time.sleep(0.01)
 
-    @tempit(run_times=5, concurrent_execution=False, verbose=False)
+    @tempit(run_times=2, concurrent_execution=False, verbose=False)
     def test_tempit_no_concurrency(self):
         time.sleep(0.01)
 
-    @tempit(run_times=5, concurrent_execution=True, verbose=True)
+    @tempit(run_times=2, concurrent_execution=True, verbose=True)
     def test_tempit_concurrency_verbose(self):
         time.sleep(0.01)
 
-    @tempit(run_times=10, concurrent_execution=True, verbose=True)
+    @tempit(run_times=2, concurrent_execution=True, verbose=True)
     def test_tempit_thread_crash(self, a: int = 1, b: int = 2, thread_name: str = "ThreadPoolExecutor-"):
         current_thread_name = threading.current_thread().name
         if not current_thread_name.startswith(thread_name):
             raise RuntimeError("Crashing intentionally for testing other process inside a class")
         return a + b
 
     def sum(self, a: int = 1, b: int = 2):
         return a + b
 
-    @tempit(run_times=10)
+    @tempit(run_times=2)
     def test_tempit_args(self, a: int = 1, b: int = 2):
         return self.sum(a, b)
 
     @tempit(run_times=2)
     @staticmethod
     def static_method(a: int = 1, b: int = 2):
         return a + b
@@ -69,19 +69,20 @@
 
         execution_time = end_time - start_time
         self.assertAlmostEqual(execution_time, 0.01, delta=0.01)
 
     def test_tempit_basic_no_parenthesis(self):
 
         start_time = time.perf_counter()
-        self.test_class.tempit_basic_no_parenthesis()
+        result = self.test_class.tempit_basic_no_parenthesis(1, b=2)
         end_time = time.perf_counter()
 
         execution_time = end_time - start_time
         self.assertAlmostEqual(execution_time, 0.01, delta=0.01)
+        self.assertEqual(result, 3)
 
     def test_tempit_with_concurrency(self):
 
         start_time = time.perf_counter()
         self.test_class.test_tempit_with_concurrency()
         end_time = time.perf_counter()
 
@@ -197,66 +198,67 @@
         my_function()
         end_time = time.perf_counter()
 
         execution_time = end_time - start_time
         self.assertAlmostEqual(execution_time, 0.01, delta=0.01)
 
     def test_tempit_with_concurrency(self):
-        @tempit(run_times=5, concurrent_execution=True)
+        @tempit(run_times=2, concurrent_execution=True)
         def my_function():
             time.sleep(0.01)
 
         start_time = time.perf_counter()
         my_function()
         end_time = time.perf_counter()
 
         execution_time = end_time - start_time
         self.assertAlmostEqual(execution_time, 0.01, delta=0.1)  # Check if execution time is close to 0.1 seconds
 
     def test_tempit_no_concurrency(self):
-        @tempit(run_times=5, concurrent_execution=False)
+        @tempit(run_times=3, concurrent_execution=False)
         def my_function():
             time.sleep(0.01)
 
         start_time = time.perf_counter()
         my_function()
         end_time = time.perf_counter()
 
         execution_time = end_time - start_time
         self.assertAlmostEqual(execution_time, 0.05, delta=0.1)
 
-    def test_tempit_multithreading_verbose(self):
+    def test_tempit_concurrency_verbose(self):
         # Just check it doesn't crash
-        @tempit(run_times=5, concurrent_execution=True, verbose=True)
+        @tempit(run_times=2, concurrent_execution=True, verbose=True)
         def my_function():
             time.sleep(0.01)
 
         start_time = time.perf_counter()
         my_function()
         end_time = time.perf_counter()
 
         execution_time = end_time - start_time
-        self.assertAlmostEqual(execution_time, 0.01, delta=0.1)
+        self.assertAlmostEqual(execution_time, 0.01, delta=1)
 
-    def test_tempit_multithreading_crash(self):
-        # Just check if it the multihreading doesn't work, it should be executed in the main thread
-        @tempit(run_times=5, concurrent_execution=True)
+    def test_tempit_concurrency_crash(self):
+        # Just check if it the parallel execution doesn't work, it should be executed in the main thread
+        @tempit(run_times=2, concurrent_execution=True)
         def my_function():
             current_thread_name = threading.current_thread().name
             process_name = current_process().name
             if current_thread_name != "MainThread" or process_name != "MainProcess":
                 raise RuntimeError("Crashing intentionally for testing multithreading outside class")
             time.sleep(0.01)
 
         start_time = time.perf_counter()
         my_function()
         end_time = time.perf_counter()
 
         execution_time = end_time - start_time
-        self.assertLess(execution_time, 0.5)
+        # It could trigger a while since it will try to use parallel processing, then parallel threading and then the sequential execution
+        self.assertLess(execution_time, 3)
 
     def test_tempit_args(self):
         @tempit(run_times=0, concurrent_execution=True, verbose=True)
         def my_function(a: int = 1, b: int = 2):
             return a + b
 
         start_time = time.perf_counter()
@@ -282,32 +284,32 @@
         with ProcessPoolExecutor(max_workers=1) as executor:
             future = executor.submit(my_process_function, 1, b=2)
             result = future.result()
 
         self.assertEqual(result, 3)
 
     def test_recursive(self):
-        @tempit(run_times=2, concurrent_execution=True, verbose=True, check_for_recursion=True)
+        @tempit(run_times=2, concurrent_execution=True, verbose=True)
         def my_function(n: int = 10):
             if n < 2:
                 return n
             return my_function(n - 2) + my_function(n - 1)
 
         result = my_function(7)
         self.assertEqual(result, 13)
 
     @unittest.skipUnless(not IN_GITHUB_ACTIONS, "Skip if running in GitHub Actions: too expensive.")
     def test_tempit_long_running_function(self):
-        @tempit(run_times=4, concurrent_execution=True)
+        @tempit(run_times=2, concurrent_execution=True)
         def my_concurrent_function(a=2_000_000, n=16):
             for _ in range(a):
                 pass  #
             return fib(n=n)
 
-        @tempit(run_times=4, concurrent_execution=False)
+        @tempit(run_times=2, concurrent_execution=False)
         def my_sequential_function(a=2_000_000, n=16):
             for _ in range(a):
                 pass  #
             return fib(n=n)
 
         start_time = time.perf_counter()
         result_concurrent = my_concurrent_function(20_000_000, n=16)
@@ -316,15 +318,15 @@
 
         start_time = time.perf_counter()
         result_sequential = my_sequential_function(20_000_000, n=16)
         end_time = time.perf_counter()
         execution_time_sequential = end_time - start_time
 
         self.assertLessEqual(
-            execution_time_concurrent, (execution_time_sequential / 3) + (execution_time_sequential * 0.2)
+            execution_time_concurrent, (execution_time_sequential / 2) + (execution_time_sequential * 0.3)
         )
 
         self.assertEqual(result_concurrent, 987)
         self.assertEqual(result_sequential, 987)
 
 
 def fib(n):
```

