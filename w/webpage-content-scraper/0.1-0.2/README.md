# Comparing `tmp/webpage_content_scraper-0.1.tar.gz` & `tmp/webpage_content_scraper-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webpage_content_scraper-0.1.tar", last modified: Wed May 15 05:45:08 2024, max compression
+gzip compressed data, was "webpage_content_scraper-0.2.tar", last modified: Mon May 20 05:05:46 2024, max compression
```

## Comparing `webpage_content_scraper-0.1.tar` & `webpage_content_scraper-0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:45:08.723105 webpage_content_scraper-0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-15 05:45:02.000000 webpage_content_scraper-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-05-15 05:45:08.723105 webpage_content_scraper-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-15 05:45:02.000000 webpage_content_scraper-0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-15 05:45:02.000000 webpage_content_scraper-0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 05:45:08.723105 webpage_content_scraper-0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:45:08.719105 webpage_content_scraper-0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8864 2024-05-15 05:45:02.000000 webpage_content_scraper-0.1/tests/test_webpage_content_scraper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:45:08.719105 webpage_content_scraper-0.1/webpage_content_scraper/
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-15 05:45:02.000000 webpage_content_scraper-0.1/webpage_content_scraper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:45:08.719105 webpage_content_scraper-0.1/webpage_content_scraper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-05-15 05:45:08.000000 webpage_content_scraper-0.1/webpage_content_scraper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-15 05:45:08.000000 webpage_content_scraper-0.1/webpage_content_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 05:45:08.000000 webpage_content_scraper-0.1/webpage_content_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-15 05:45:08.000000 webpage_content_scraper-0.1/webpage_content_scraper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-15 05:45:08.000000 webpage_content_scraper-0.1/webpage_content_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:05:46.845031 webpage_content_scraper-0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-20 05:05:32.000000 webpage_content_scraper-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-20 05:05:46.845031 webpage_content_scraper-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-20 05:05:32.000000 webpage_content_scraper-0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-20 05:05:32.000000 webpage_content_scraper-0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 05:05:46.845031 webpage_content_scraper-0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:05:46.841031 webpage_content_scraper-0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8390 2024-05-20 05:05:32.000000 webpage_content_scraper-0.2/tests/test_webpage_content_scraper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:05:46.845031 webpage_content_scraper-0.2/webpage_content_scraper/
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-20 05:05:32.000000 webpage_content_scraper-0.2/webpage_content_scraper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:05:46.845031 webpage_content_scraper-0.2/webpage_content_scraper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-20 05:05:46.000000 webpage_content_scraper-0.2/webpage_content_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-20 05:05:46.000000 webpage_content_scraper-0.2/webpage_content_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 05:05:46.000000 webpage_content_scraper-0.2/webpage_content_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-20 05:05:46.000000 webpage_content_scraper-0.2/webpage_content_scraper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-20 05:05:46.000000 webpage_content_scraper-0.2/webpage_content_scraper.egg-info/top_level.txt
```

### Comparing `webpage_content_scraper-0.1/LICENSE` & `webpage_content_scraper-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `webpage_content_scraper-0.1/PKG-INFO` & `webpage_content_scraper-0.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 Metadata-Version: 2.1
 Name: webpage-content-scraper
-Version: 0.1
+Version: 0.2
 Summary: Scrape only the content from a webpage using Firefox's reader view.
 Author: Ryan Blunden
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/ryan-blunden/python-webpage-content-scraper
 Project-URL: Changelog, https://github.com/ryan-blunden/python-webpage-content-scraper/releases
 Project-URL: Issues, https://github.com/ryan-blunden/python-webpage-content-scraper/issues
 Project-URL: CI, https://github.com/ryan-blunden/python-webpage-content-scraper/actions
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: playwright
 Requires-Dist: markdownify
 Requires-Dist: beautifulsoup4
+Provides-Extra: dev
+Requires-Dist: symbex; extra == "dev"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-mock; extra == "test"
 Requires-Dist: ruff; extra == "test"
+Requires-Dist: mypy; extra == "test"
 
 # Webpage Content Scraper
 
-[![PyPI](https://img.shields.io/pypi/v/python-webpage-content-scraper.svg)](https://pypi.org/project/python-webpage-content-scraper/)
+[![PyPI](https://img.shields.io/pypi/v/webpage-content-scraper.svg)](https://pypi.org/project/python-webpage-content-scraper/)
 [![Tests](https://github.com/ryan-blunden/python-webpage-content-scraper/actions/workflows/test.yml/badge.svg)](https://github.com/ryan-blunden/python-webpage-content-scraper/actions/workflows/test.yml)
 [![Changelog](https://img.shields.io/github/v/release/ryan-blunden/python-webpage-content-scraper?include_prereleases&label=changelog)](https://github.com/ryan-blunden/python-webpage-content-scraper/releases)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/ryan-blunden/python-webpage-content-scraper/blob/main/LICENSE)
 
 Scrape only the content from a webpage using Firefox's reader view.
 
 ## Installation
@@ -40,20 +43,20 @@
 
 ```bash
 playwright install firefox
 ```
 
 ## Usage
 
-Simply supply a URL and optionally, a format and timeout.
+Simply supply a list of pages and optionally, a format and timeout.
 
 ```python
 from webpage_content_scraper import fetch_page_content, Formats
 
-url = 'https://microsoft.github.io/autogen/blog/2023/10/18/RetrieveChat/'
+pages = ['https://microsoft.github.io/autogen/blog/2023/10/18/RetrieveChat/']
 
 html_content = fetch_page_content(url)
 markdown_content = fetch_page_content(url, Formats.MARKDOWN)
 ```
 
 ## Development
```

### Comparing `webpage_content_scraper-0.1/README.md` & `webpage_content_scraper-0.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Webpage Content Scraper
 
-[![PyPI](https://img.shields.io/pypi/v/python-webpage-content-scraper.svg)](https://pypi.org/project/python-webpage-content-scraper/)
+[![PyPI](https://img.shields.io/pypi/v/webpage-content-scraper.svg)](https://pypi.org/project/python-webpage-content-scraper/)
 [![Tests](https://github.com/ryan-blunden/python-webpage-content-scraper/actions/workflows/test.yml/badge.svg)](https://github.com/ryan-blunden/python-webpage-content-scraper/actions/workflows/test.yml)
 [![Changelog](https://img.shields.io/github/v/release/ryan-blunden/python-webpage-content-scraper?include_prereleases&label=changelog)](https://github.com/ryan-blunden/python-webpage-content-scraper/releases)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/ryan-blunden/python-webpage-content-scraper/blob/main/LICENSE)
 
 Scrape only the content from a webpage using Firefox's reader view.
 
 ## Installation
@@ -18,20 +18,20 @@
 
 ```bash
 playwright install firefox
 ```
 
 ## Usage
 
-Simply supply a URL and optionally, a format and timeout.
+Simply supply a list of pages and optionally, a format and timeout.
 
 ```python
 from webpage_content_scraper import fetch_page_content, Formats
 
-url = 'https://microsoft.github.io/autogen/blog/2023/10/18/RetrieveChat/'
+pages = ['https://microsoft.github.io/autogen/blog/2023/10/18/RetrieveChat/']
 
 html_content = fetch_page_content(url)
 markdown_content = fetch_page_content(url, Formats.MARKDOWN)
 ```
 
 ## Development
```

### Comparing `webpage_content_scraper-0.1/tests/test_webpage_content_scraper.py` & `webpage_content_scraper-0.2/tests/test_webpage_content_scraper.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import pytest
 from bs4 import BeautifulSoup
 from unittest.mock import MagicMock, patch
 from webpage_content_scraper import _get_reader_content, fetch_page_content, Formats
 
 
 def _generate_reader_content_html(content):
     return f"""<!DOCTYPE html><html platform="macosx" lang="en-US" dir="ltr"><head>
@@ -81,74 +80,61 @@
       <div aria-owns="toolbar"></div>
     </div>
   
 
 </body></html>
 """
 
+
 # Test _get_reader_content function
 def test_get_reader_content_with_reader_content():
-    html = _generate_reader_content_html("<h1>Test content</h1>")
+    html = _generate_reader_content_html('<h1>Test content</h1>')
     reader_content = _get_reader_content(html)
     assert reader_content is not None
-    assert reader_content.find().text == "Test content"
+    assert reader_content.find().text == 'Test content'
 
 
 def test_get_reader_content_without_reader_content():
     html = _generate_reader_content_html('')
     reader_content = _get_reader_content(html)
     assert reader_content is None
 
 
-# Test fetch_page_content function
-@patch("webpage_content_scraper.sync_playwright")
-@patch("webpage_content_scraper._get_reader_content")
-def test_fetch_page_content_html(mock_get_reader_content, mock_sync_playwright):
-    # Mock the Playwright context
+# Helper function to mock the Playwright context
+def mock_playwright_context(mock_sync_playwright):
     mock_browser = MagicMock()
     mock_page = MagicMock()
     mock_context = MagicMock()
     mock_context.__enter__.return_value = mock_context
     mock_sync_playwright.return_value.__enter__.return_value = mock_context
     mock_context.firefox.launch.return_value = mock_browser
     mock_browser.new_page.return_value = mock_page
+    return mock_page
+
+
+# Test fetch_page_content function
+@patch('webpage_content_scraper.sync_playwright')
+@patch('webpage_content_scraper._get_reader_content')
+def test_fetch_page_content_html(mock_get_reader_content, mock_sync_playwright):
+    mock_page = mock_playwright_context(mock_sync_playwright)
 
-    mock_page.content.return_value = (
-        _generate_reader_content_html('<article><h1>Test content</h1></article>')
+    mock_page.content.return_value = _generate_reader_content_html(
+        '<article><h1>Test content</h1></article>'
     )
     mock_get_reader_content.return_value = BeautifulSoup(
-        mock_page.content.return_value, "html.parser"
+        mock_page.content.return_value, 'html.parser'
     )
 
-    url = "http://example.com"
-    result = fetch_page_content(url, format=Formats.HTML)
+    urls = ['http://example.com']
+    result = fetch_page_content(urls, format=Formats.HTML)
 
-    assert '<article><h1>Test content</h1></article>' in result
+    assert '<article><h1>Test content</h1></article>' in result[0]
 
 
-@patch("webpage_content_scraper.sync_playwright")
-@patch("webpage_content_scraper._get_reader_content")
+@patch('webpage_content_scraper.sync_playwright')
+@patch('webpage_content_scraper._get_reader_content')
 def test_fetch_page_content_markdown(mock_get_reader_content, mock_sync_playwright):
-    # Mock the Playwright context
-    mock_browser = MagicMock()
-    mock_page = MagicMock()
-    mock_context = MagicMock()
-    mock_context.__enter__.return_value = mock_context
-    mock_sync_playwright.return_value.__enter__.return_value = mock_context
-    mock_context.firefox.launch.return_value = mock_browser
-    mock_browser.new_page.return_value = mock_page
+    mock_page = mock_playwright_context(mock_sync_playwright)
 
-    mock_page.content.return_value = (
-       _generate_reader_content_html('<article><h1>Test Title</h1><p>Test content.</p></article>')
-    )
-    mock_get_reader_content.return_value = BeautifulSoup(
-        mock_page.content.return_value, "html.parser"
+    mock_page.content.return_value = _generate_reader_content_html(
+        '<article><h1>Test Title</h1><p>Test content.</p></article>'
     )
-
-    url = "http://example.com"
-    result = fetch_page_content(url, format=Formats.MARKDOWN)
-
-    assert "# Test Title\n\nTest content" in result
-
-
-if __name__ == "__main__":
-    pytest.main()
```

### Comparing `webpage_content_scraper-0.1/webpage_content_scraper/__init__.py` & `webpage_content_scraper-0.2/webpage_content_scraper/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,48 +1,59 @@
-import time
+from typing import List, Union
 
-from bs4 import BeautifulSoup
-from playwright.sync_api import sync_playwright
+from bs4 import BeautifulSoup, NavigableString, Tag
+from playwright.sync_api import sync_playwright, TimeoutError
 from markdownify import MarkdownConverter
 
 
 class Formats:
-    MARKDOWN = "markdown"
-    HTML = "html"
+    MARKDOWN = 'markdown'
+    HTML = 'html'
 
 
-def _get_reader_content(html):
-    soup = BeautifulSoup(html, "html.parser")
-    reader_content = soup.find(class_="moz-reader-content")
+def _get_reader_content(html: str) -> Union[Tag, NavigableString]:
+    soup = BeautifulSoup(html, 'html.parser')
+    reader_content = soup.find(class_='moz-reader-content')
 
-    if reader_content and reader_content.find():
-        return reader_content
+    return reader_content if reader_content and reader_content.contents else None
 
-    return None
 
+def fetch_page_content(
+    urls: List[str], format: str = Formats.HTML, timeout: int = 10
+) -> List[Union[str, None]]:
+    if not isinstance(urls, list) or not all(isinstance(url, str) for url in urls):
+        raise ValueError('urls must be a list of strings')
+
+    pages_content: List[Union[str, None]] = []
 
-def fetch_page_content(url, format=Formats.HTML, timeout=30):
     with sync_playwright() as p:
         browser = p.firefox.launch()
         page = browser.new_page()
-        page.goto(f"about:reader?url={url}")
-
-        start_time = time.time()
-        reader_content = None
-
-        while time.time() - start_time < timeout:
-            html = page.content()
-            reader_content = _get_reader_content(html)
 
-            if reader_content:
-                break
-
-            time.sleep(1)
+        for url in urls:
+            try:
+                page.goto(f'about:reader?url={url}', timeout=timeout * 1000)
+                page.wait_for_selector('.moz-reader-content *', timeout=timeout * 1000)
+
+                html = page.content()
+                reader_content = _get_reader_content(html)
+
+                if not reader_content:
+                    pages_content.append('')
+                    continue
+
+                if format == Formats.MARKDOWN:
+                    pages_content.append(
+                        MarkdownConverter(
+                            heading_style='ATX', heading_level=2
+                        ).convert_soup(reader_content)
+                    )
+                else:
+                    pages_content.append(str(reader_content))
+            except TimeoutError:
+                pages_content.append('')
+            except Exception as e:
+                pages_content.append(f'Error: {e}')
 
         browser.close()
 
-        if format == Formats.MARKDOWN:
-            return MarkdownConverter(heading_style="ATX", heading_level=2).convert_soup(
-                reader_content
-            )
-
-        return str(reader_content)
+    return pages_content
```

### Comparing `webpage_content_scraper-0.1/webpage_content_scraper.egg-info/PKG-INFO` & `webpage_content_scraper-0.2/webpage_content_scraper.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 Metadata-Version: 2.1
 Name: webpage-content-scraper
-Version: 0.1
+Version: 0.2
 Summary: Scrape only the content from a webpage using Firefox's reader view.
 Author: Ryan Blunden
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/ryan-blunden/python-webpage-content-scraper
 Project-URL: Changelog, https://github.com/ryan-blunden/python-webpage-content-scraper/releases
 Project-URL: Issues, https://github.com/ryan-blunden/python-webpage-content-scraper/issues
 Project-URL: CI, https://github.com/ryan-blunden/python-webpage-content-scraper/actions
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: playwright
 Requires-Dist: markdownify
 Requires-Dist: beautifulsoup4
+Provides-Extra: dev
+Requires-Dist: symbex; extra == "dev"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-mock; extra == "test"
 Requires-Dist: ruff; extra == "test"
+Requires-Dist: mypy; extra == "test"
 
 # Webpage Content Scraper
 
-[![PyPI](https://img.shields.io/pypi/v/python-webpage-content-scraper.svg)](https://pypi.org/project/python-webpage-content-scraper/)
+[![PyPI](https://img.shields.io/pypi/v/webpage-content-scraper.svg)](https://pypi.org/project/python-webpage-content-scraper/)
 [![Tests](https://github.com/ryan-blunden/python-webpage-content-scraper/actions/workflows/test.yml/badge.svg)](https://github.com/ryan-blunden/python-webpage-content-scraper/actions/workflows/test.yml)
 [![Changelog](https://img.shields.io/github/v/release/ryan-blunden/python-webpage-content-scraper?include_prereleases&label=changelog)](https://github.com/ryan-blunden/python-webpage-content-scraper/releases)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/ryan-blunden/python-webpage-content-scraper/blob/main/LICENSE)
 
 Scrape only the content from a webpage using Firefox's reader view.
 
 ## Installation
@@ -40,20 +43,20 @@
 
 ```bash
 playwright install firefox
 ```
 
 ## Usage
 
-Simply supply a URL and optionally, a format and timeout.
+Simply supply a list of pages and optionally, a format and timeout.
 
 ```python
 from webpage_content_scraper import fetch_page_content, Formats
 
-url = 'https://microsoft.github.io/autogen/blog/2023/10/18/RetrieveChat/'
+pages = ['https://microsoft.github.io/autogen/blog/2023/10/18/RetrieveChat/']
 
 html_content = fetch_page_content(url)
 markdown_content = fetch_page_content(url, Formats.MARKDOWN)
 ```
 
 ## Development
```

