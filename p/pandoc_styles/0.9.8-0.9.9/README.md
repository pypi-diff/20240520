# Comparing `tmp/pandoc_styles-0.9.8.tar.gz` & `tmp/pandoc_styles-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandoc_styles-0.9.8.tar", last modified: Sat Aug 28 22:00:51 2021, max compression
+gzip compressed data, was "pandoc_styles-0.9.9.tar", last modified: Tue Oct 12 10:18:26 2021, max compression
```

## Comparing `pandoc_styles-0.9.8.tar` & `pandoc_styles-0.9.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1089 2019-11-07 16:16:10.000000 pandoc_styles-0.9.8/LICENSE.md
--rw-r--r--   0        0        0      360 2019-11-07 16:16:10.000000 pandoc_styles-0.9.8/pandoc_styles/__init__.py
--rw-r--r--   0        0        0     2036 2019-11-07 16:16:10.000000 pandoc_styles-0.9.8/pandoc_styles/cl_stylepacks.py
--rw-r--r--   0        0        0     2230 2021-02-20 11:26:57.361670 pandoc_styles-0.9.8/pandoc_styles/cl_tools.py
--rw-r--r--   0        0        0      242 2019-11-07 16:16:10.000000 pandoc_styles-0.9.8/pandoc_styles/config_dir/config.yaml
--rw-r--r--   0        0        0     4054 2019-11-07 16:16:10.000000 pandoc_styles-0.9.8/pandoc_styles/config_dir/css/default.css
--rw-r--r--   0        0        0      462 2019-11-07 16:16:10.000000 pandoc_styles-0.9.8/pandoc_styles/config_dir/filter/alignment.py
--rw-r--r--   0        0        0      482 2019-11-07 16:16:10.000000 pandoc_styles-0.9.8/pandoc_styles/config_dir/filter/include.py
--rw-r--r--   0        0        0      406 2019-11-07 16:16:10.000000 pandoc_styles-0.9.8/pandoc_styles/config_dir/filter/new_page.py
--rw-r--r--   0        0        0      255 2019-11-07 16:16:10.000000 pandoc_styles-0.9.8/pandoc_styles/config_dir/filter/noindent.py
--rw-r--r--   0        0        0      293 2019-11-07 16:16:10.000000 pandoc_styles-0.9.8/pandoc_styles/config_dir/postflight/delete_output.py
--rw-r--r--   0        0        0      391 2019-11-07 16:16:10.000000 pandoc_styles-0.9.8/pandoc_styles/config_dir/preflight/append_to_file.py
--rw-r--r--   0        0        0     3810 2019-11-07 16:16:10.000000 pandoc_styles-0.9.8/pandoc_styles/config_dir/sass/default.scss
--rw-r--r--   0        0        0     2648 2019-11-07 16:16:10.000000 pandoc_styles-0.9.8/pandoc_styles/config_dir/sass/default_epub.scss
--rw-r--r--   0        0        0     2962 2019-11-07 16:16:10.000000 pandoc_styles-0.9.8/pandoc_styles/config_dir/sass/extra_styles.scss
--rw-r--r--   0        0        0     3671 2019-11-07 16:16:10.000000 pandoc_styles-0.9.8/pandoc_styles/config_dir/sass/navigation.scss
--rw-r--r--   0        0        0     7575 2021-02-20 11:30:11.075302 pandoc_styles-0.9.8/pandoc_styles/config_dir/styles.yaml
--rw-r--r--   0        0        0     1899 2021-08-28 14:32:47.120136 pandoc_styles-0.9.8/pandoc_styles/constants.py
--rw-r--r--   0        0        0    12297 2020-05-11 18:05:57.264931 pandoc_styles-0.9.8/pandoc_styles/filter.py
--rw-r--r--   0        0        0     1368 2020-02-17 16:23:31.924798 pandoc_styles-0.9.8/pandoc_styles/flight_scripts.py
--rw-r--r--   0        0        0     1230 2019-11-07 16:16:10.000000 pandoc_styles-0.9.8/pandoc_styles/format_mappings.py
--rw-r--r--   0        0        0    25043 2021-08-28 15:01:22.963534 pandoc_styles-0.9.8/pandoc_styles/main.py
--rw-r--r--   0        0        0     1877 2021-02-14 00:01:50.889183 pandoc_styles-0.9.8/pandoc_styles/pandoc_cmd_line_options.py
--rw-r--r--   0        0        0     5623 2021-02-28 11:14:28.087595 pandoc_styles-0.9.8/pandoc_styles/utils.py
--rw-r--r--   0        0        0     1169 2021-08-28 22:00:29.107746 pandoc_styles-0.9.8/pyproject.toml
--rw-r--r--   0        0        0    14340 2021-03-20 14:11:02.285483 pandoc_styles-0.9.8/README.md
--rw-r--r--   0        0        0    15650 2021-08-28 22:00:51.888621 pandoc_styles-0.9.8/setup.py
--rw-r--r--   0        0        0    14987 2021-08-28 22:00:51.890628 pandoc_styles-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0     1089 2019-11-07 16:16:10.000000 pandoc_styles-0.9.9/LICENSE.md
+-rw-r--r--   0        0        0      360 2019-11-07 16:16:10.000000 pandoc_styles-0.9.9/pandoc_styles/__init__.py
+-rw-r--r--   0        0        0     2036 2019-11-07 16:16:10.000000 pandoc_styles-0.9.9/pandoc_styles/cl_stylepacks.py
+-rw-r--r--   0        0        0     2230 2021-02-20 11:26:57.361670 pandoc_styles-0.9.9/pandoc_styles/cl_tools.py
+-rw-r--r--   0        0        0      242 2019-11-07 16:16:10.000000 pandoc_styles-0.9.9/pandoc_styles/config_dir/config.yaml
+-rw-r--r--   0        0        0     4054 2019-11-07 16:16:10.000000 pandoc_styles-0.9.9/pandoc_styles/config_dir/css/default.css
+-rw-r--r--   0        0        0      462 2019-11-07 16:16:10.000000 pandoc_styles-0.9.9/pandoc_styles/config_dir/filter/alignment.py
+-rw-r--r--   0        0        0      482 2019-11-07 16:16:10.000000 pandoc_styles-0.9.9/pandoc_styles/config_dir/filter/include.py
+-rw-r--r--   0        0        0      406 2019-11-07 16:16:10.000000 pandoc_styles-0.9.9/pandoc_styles/config_dir/filter/new_page.py
+-rw-r--r--   0        0        0      255 2019-11-07 16:16:10.000000 pandoc_styles-0.9.9/pandoc_styles/config_dir/filter/noindent.py
+-rw-r--r--   0        0        0      293 2019-11-07 16:16:10.000000 pandoc_styles-0.9.9/pandoc_styles/config_dir/postflight/delete_output.py
+-rw-r--r--   0        0        0      391 2019-11-07 16:16:10.000000 pandoc_styles-0.9.9/pandoc_styles/config_dir/preflight/append_to_file.py
+-rw-r--r--   0        0        0     3810 2019-11-07 16:16:10.000000 pandoc_styles-0.9.9/pandoc_styles/config_dir/sass/default.scss
+-rw-r--r--   0        0        0     2648 2019-11-07 16:16:10.000000 pandoc_styles-0.9.9/pandoc_styles/config_dir/sass/default_epub.scss
+-rw-r--r--   0        0        0     2962 2019-11-07 16:16:10.000000 pandoc_styles-0.9.9/pandoc_styles/config_dir/sass/extra_styles.scss
+-rw-r--r--   0        0        0     3671 2019-11-07 16:16:10.000000 pandoc_styles-0.9.9/pandoc_styles/config_dir/sass/navigation.scss
+-rw-r--r--   0        0        0     7575 2021-02-20 11:30:11.075302 pandoc_styles-0.9.9/pandoc_styles/config_dir/styles.yaml
+-rw-r--r--   0        0        0     1899 2021-08-28 14:32:47.120136 pandoc_styles-0.9.9/pandoc_styles/constants.py
+-rw-r--r--   0        0        0    12381 2021-10-07 14:47:35.090387 pandoc_styles-0.9.9/pandoc_styles/filter.py
+-rw-r--r--   0        0        0     1368 2020-02-17 16:23:31.924798 pandoc_styles-0.9.9/pandoc_styles/flight_scripts.py
+-rw-r--r--   0        0        0     1230 2019-11-07 16:16:10.000000 pandoc_styles-0.9.9/pandoc_styles/format_mappings.py
+-rw-r--r--   0        0        0    25047 2021-10-11 13:08:48.886150 pandoc_styles-0.9.9/pandoc_styles/main.py
+-rw-r--r--   0        0        0     1877 2021-02-14 00:01:50.889183 pandoc_styles-0.9.9/pandoc_styles/pandoc_cmd_line_options.py
+-rw-r--r--   0        0        0     5623 2021-02-28 11:14:28.087595 pandoc_styles-0.9.9/pandoc_styles/utils.py
+-rw-r--r--   0        0        0     1169 2021-10-12 10:18:04.827337 pandoc_styles-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0    14340 2021-03-20 14:11:02.285483 pandoc_styles-0.9.9/README.md
+-rw-r--r--   0        0        0    15650 2021-10-12 10:18:26.768241 pandoc_styles-0.9.9/setup.py
+-rw-r--r--   0        0        0    14987 2021-10-12 10:18:26.770246 pandoc_styles-0.9.9/PKG-INFO
```

### Comparing `pandoc_styles-0.9.8/LICENSE.md` & `pandoc_styles-0.9.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pandoc_styles-0.9.8/pandoc_styles/cl_stylepacks.py` & `pandoc_styles-0.9.9/pandoc_styles/cl_stylepacks.py`

 * *Files identical despite different names*

### Comparing `pandoc_styles-0.9.8/pandoc_styles/cl_tools.py` & `pandoc_styles-0.9.9/pandoc_styles/cl_tools.py`

 * *Files identical despite different names*

### Comparing `pandoc_styles-0.9.8/pandoc_styles/config_dir/css/default.css` & `pandoc_styles-0.9.9/pandoc_styles/config_dir/css/default.css`

 * *Files identical despite different names*

### Comparing `pandoc_styles-0.9.8/pandoc_styles/config_dir/sass/default.scss` & `pandoc_styles-0.9.9/pandoc_styles/config_dir/sass/default.scss`

 * *Files identical despite different names*

### Comparing `pandoc_styles-0.9.8/pandoc_styles/config_dir/sass/default_epub.scss` & `pandoc_styles-0.9.9/pandoc_styles/config_dir/sass/default_epub.scss`

 * *Files identical despite different names*

### Comparing `pandoc_styles-0.9.8/pandoc_styles/config_dir/sass/extra_styles.scss` & `pandoc_styles-0.9.9/pandoc_styles/config_dir/sass/extra_styles.scss`

 * *Files identical despite different names*

### Comparing `pandoc_styles-0.9.8/pandoc_styles/config_dir/sass/navigation.scss` & `pandoc_styles-0.9.9/pandoc_styles/config_dir/sass/navigation.scss`

 * *Files identical despite different names*

### Comparing `pandoc_styles-0.9.8/pandoc_styles/config_dir/styles.yaml` & `pandoc_styles-0.9.9/pandoc_styles/config_dir/styles.yaml`

 * *Files identical despite different names*

### Comparing `pandoc_styles-0.9.8/pandoc_styles/constants.py` & `pandoc_styles-0.9.9/pandoc_styles/constants.py`

 * *Files identical despite different names*

### Comparing `pandoc_styles-0.9.8/pandoc_styles/filter.py` & `pandoc_styles-0.9.9/pandoc_styles/filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     def _init_filter(self, elem, doc):
         self.elem = elem
         self.doc = doc
         self.cfg = dict()
         self._get_format()
         self.classes = elem.classes if hasattr(elem, "classes") else None
         self.attributes = elem.attributes if hasattr(elem, "attributes") else None
+        self.identifier = elem.identifier if hasattr(elem, "identifier") else None
         self._text = elem.text if hasattr(elem, "text") else None
         self.content = elem.content if hasattr(elem, "content") else None
 
     def _return_filter(self):
         if self.new_text is None:
             return
         elif self.new_text == []:
```

### Comparing `pandoc_styles-0.9.8/pandoc_styles/flight_scripts.py` & `pandoc_styles-0.9.9/pandoc_styles/flight_scripts.py`

 * *Files identical despite different names*

### Comparing `pandoc_styles-0.9.8/pandoc_styles/format_mappings.py` & `pandoc_styles-0.9.9/pandoc_styles/format_mappings.py`

 * *Files identical despite different names*

### Comparing `pandoc_styles-0.9.8/pandoc_styles/main.py` & `pandoc_styles-0.9.9/pandoc_styles/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,16 +122,16 @@
             style = self._get_stylepack_style(style, stylepacks)
         new_style = dict()
         if inherited:
             del style[MD_INHERITS]
             for extra_style in inherited:
                 extra_style = self._get_style(all_styles[extra_style], all_styles)
                 self.update_dict(new_style, extra_style)
-        self.update_dict(style, new_style)
-        return style
+        self.update_dict(new_style, style)
+        return new_style
 
     def make_format(self, fmt):
         """
         Converts to the given format.
         All attributes defined here change with each format
         """
         self.cfg = self._get_cfg(fmt)
```

### Comparing `pandoc_styles-0.9.8/pandoc_styles/pandoc_cmd_line_options.py` & `pandoc_styles-0.9.9/pandoc_styles/pandoc_cmd_line_options.py`

 * *Files identical despite different names*

### Comparing `pandoc_styles-0.9.8/pandoc_styles/utils.py` & `pandoc_styles-0.9.9/pandoc_styles/utils.py`

 * *Files identical despite different names*

### Comparing `pandoc_styles-0.9.8/pyproject.toml` & `pandoc_styles-0.9.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pandoc_styles"
-version = "0.9.8"
+version = "0.9.9"
 description = "A script to convert files with pandoc using styles."
 authors = ["dickloraine <dickloraine@gmx.net>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/dickloraine/pandoc_styles"
 keywords = ["pandoc", "writing", "text", "conversion"]
 classifiers=[
```

### Comparing `pandoc_styles-0.9.8/README.md` & `pandoc_styles-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `pandoc_styles-0.9.8/setup.py` & `pandoc_styles-0.9.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 {'console_scripts': ['pandoc-styles = pandoc_styles.main:main',
                      'pandoc-styles-tools = pandoc_styles.cl_tools:main',
                      'pandoc_styles = pandoc_styles.main:main',
                      'pandoc_styles_tools = pandoc_styles.cl_tools:main']}
 
 setup_kwargs = {
     'name': 'pandoc-styles',
-    'version': '0.9.8',
+    'version': '0.9.9',
     'description': 'A script to convert files with pandoc using styles.',
     'long_description': '# pandoc-styles\n\nThis script allows you to define styles for pandoc. In styles you can define, with which arguments pandoc should be invoked for different formats. In addition it allows to run scripts before and after a conversion and gives much power to these scripts and to filters.\n\n- [pandoc-styles](#pandoc-styles)\n  - [Installation](#installation)\n    - [Requirements](#requirements)\n    - [Install](#install)\n    - [Setup](#setup)\n  - [Usage](#usage)\n  - [Defining Styles](#defining-styles)\n    - [Basic Usage](#basic-usage)\n    - [Inheritance](#inheritance)\n  - [Stylepacks](#stylepacks)\n  - [Advanced Feature](#advanced-feature)\n    - [Adressing files in the configuration folder](#adressing-files-in-the-configuration-folder)\n    - [Verbatim Variables](#verbatim-variables)\n    - [Preflight](#preflight)\n    - [Process Sass](#process-sass)\n    - [Add to template](#add-to-template)\n    - [Replace in template](#replace-in-template)\n    - [Replace in output](#replace-in-output)\n    - [Postflight](#postflight)\n    - [Filter](#filter)\n    - [Advanced Example](#advanced-example)\n  - [Commandline tools](#commandline-tools)\n  - [Creating stylepacks](#creating-stylepacks)\n\n## Installation\n\n### Requirements\n\nTo use this script, you need the following:\n\n1. Python 3.6 or higher:\n    You can get [python here](https://www.python.org/).\n\n2. Pandoc 2.11 or higher:\n    You can download [pandoc here](http://pandoc.org/index.html).\n\n### Install\n\nNow you need to install this script itself. Open the console and enter:\n\n    pip3 install pandoc_styles\n    pandoc-styles --init\n\n### Setup\n\nDepending on your system, you may have to configure some settings for everything to work.\nUpon initialization this script created the directory "pandoc_styles" in your user folder. Inside you can find the config.yaml file. Set the option in there that are needed for your system.\n\n## Usage\n\nThe "pandoc_styles" folder can be used as a central point to store styles, scripts, filter etc. Some subfolders are pre-created for you to use.\n\nThe "styles.yaml" file contains all the styles. Here you define your styles and the script looks here for styles specified in the metadata block of your files.\n\nTo use your styles, your source files need to have a metadata block. These commands in the block are recognized by this script:\n\n- styles: A list of styles to be used for the file\n- style-defintion: In addition of defining styles in the "styles.yaml" file, you can define a style here too. Style settings given here have precedence over those given in "styles.yaml"\n- formats: A list of formats the source file should be converted to. If none is given, html- and pdf-files are build.\n- destination: A directory to create the output in.\n- output-name: The desired name of the outputfile without extension. In none is given, the filename is used.\n- fields that exist in the style. They override the default given in the style.\n\nIf you convert all files in a folder as one document, these additional commands are available:\n\n- file-list: Specify exactly which files in the folder should be converted.\n- excluded-files: Exclude the listed files from beeing converted.\n\nThen to convert your file, open the console and enter:\n\n    pandoc-styles "your_file"\n\nOr if you want to convert all files in a folder as one document:\n    pandoc-styles -f\n\nThe commandline script has many optional parameters to be useful in macros, batch files etc. Enter\n\n    pandoc-styles -h\n\nto see all the options.\n\n## Defining Styles\n\n### Basic Usage\n\nStyles are written in yaml, just like pandoc metadata-blocks. A style is defined like this:\n\n~~~yaml\nName:\n  format:\n      pandoc-option: value\n      pandoc-variable: value\n~~~\n\n"Name" is how the style is adressed. A style directly defined in the metadata-block has no name. "Format" specifies for which format the following commands should be invoked. There is a special value: "all". Everything under "all" is used in any format. Examples for formats are html, pdf, latex, epub etc.\n\nUnder the format you just enter pandoc options and variables. If a parameter is a flag, use "true". Parameters given the value "false" are ignored.\n\n**A Basic example**\n\nThis is an example metadata-block in a source file:\n\n~~~yaml\n\n---\ntitle:  Example\nauthor: John Doe\nformats:\n    - html\n    - pdf\nstyle-definition:\n    all:\n        toc: true\n        toc-depth: 3\n        highlight-style: tango\n        language: en\n    html:\n        standalone: true\n    pdf:\n        pdf-engine: xelatex\n---\n~~~\n\n### Inheritance\n\nA style can have a field named "inherit". This is a list of other styles it inherits from. Styles lower on the list update styles that are higher. The following rules are in place:\n\n- Single values are replaced\n- If a value is another dictionary, new values are appended to it, if a value exists, these rules are used again on it\n- If a value is a list, new values are appended to it.\n\n## Stylepacks\n\nIt is possible, to bundle all files necessary for a particular style and share this as a stylepack. You can install a stylepack either through extracting its contents into the styles folder inside the config folder or through the pandoc_styles_tools command line interface with the option `import` command.\n\nTo use a stylepack, include a field "stylepacks" in the matadata. It looks like this:\n\n~~~\nstylepacks:\n  - stylepack_1_name:\n    - style_1\n    - style2\n  - stylepack_2_name\n~~~\n\nIf you do not specify styles from the stylepack, it uses its default style.\n\n**Example**\n\n[pandoc_styles: novel](https://github.com/dickloraine/pandoc_styles_novel) is a stylepack to create novels out of your source files. A documentation for using this stylepack is found on the github page and inside the style folder of the pack once installed. You can install it with this command:\n\n~~~\npandoc-styles-tools import novel -u https://github.com/dickloraine/pandoc_styles_novel/releases/latest/download/novel.zip\n~~~\n\n## Advanced Feature\n\n### Adressing files in the configuration folder\n\nYou can point to a file in the configuration directory, if you prepend the path with "~/". The script searches first for the given path and then looks in appropiatly named subfolders and finally in the "misc" subfolder. For example:\n\n~~~yaml\nfilter:\n  - ~/test-filter.py\n~~~\n\nWould find the file "test-filter.py" in the subfolder "filter" in the configuration directory.\n\n### Verbatim Variables\n\nIf you need template variables that should not be rendered in the output format (for example file paths), you can add these under the "verbatim-variables" field:\n\n~~~yaml\nverbatim-variables:\n  my-path: "my/path"\n~~~\n\nSome variables are predefiened and always usable in templates:\n\n- config-dir: The path to the config dir\n- stylepackName-dir: The path to the directory of the given stylepack\n- temp-dir: The path to the currently used temporary directory\n\n### Preflight\n\nYou can run other command-line apps and scripts before the conversion happens. Just enter the command-line command in the preflight field in the style definition. You can pass the files list to it with `<files>`. Explicitly mark the value as a string, to avoid any hassle with special characters. For example:\n\n~~~yaml\nTest-style:\n  html:\n    preflight:\n      - \'some_app -d -f <files>\'\n~~~\n\nIf you give it just a single python file, it assumes that it is a special preflight script. These are written in python and have access to the style infos and files that should be converted.\n\nHere a basic example of a preflight script, that appends text given in the field "append-to-file" in the style definition to the end of the files:\n\n~~~python\nfrom pandoc_styles import run_preflight_script, file_read, file_write\n\n\ndef preflight(self):\n    text_to_append = self.cfg["append-to-file"]\n    if isinstance(text_to_append, list):\n        text_to_append = "\\n".join(text_to_append)\n    file_write(self.files[-1], f"{file_read(self.files[-1])}\\n{text_to_append}")\n\n\nif __name__ == \'__main__\':\n    run_preflight_script(preflight)\n~~~\n\nModify only the preflight function to include your code.\n\nAnd to run it in your style definition:\n\n~~~yaml\nTest-style:\n  html:\n    preflight:\n      - append-to-file.py\n    append-to-file: "Test"\n~~~\n\n### Process Sass\n\nYou can point to sass-files that should be used for html output and this script converts them for you to css and uses that in the output. In addition you can define variables used in the sass file and specify, where the compiled css file shoud be copied.\n\n~~~yaml\nTest-style:\n  html:\n    sass:\n      files: ~/default.scss\n      output-path: temp\n      variables:\n        body-font-size: 10pt\n~~~\n\n"files" is a list of sass files to be included.\n\n"output-path" can be "~/" to output to the css folder in the configuration folder, a relative path or "temp" to be used with the "self-contained" parameter. If ommited, the css output is in the same folder as the source files output.\n\n"variables" can be any variables in your sass files.\n\n### Add to template\n\nSometimes you want to include some code directly into the template, instead of just including it in the header. Mostly, if you want to define and use your own template variables.\n\nThis option just injects the given code directly into the head of the template.\n\nIt accepts a path to a file and will add the contents of the file to the template.\n\n~~~yaml\nTest-style:\n  pdf:\n    add-to-template:\n      - |\n        \\titlehead{{$titletop-left$\n        \\hfill $titletop-right$\\\\}\n        $titlehead$}\n        \\publishers{\\small $titlebottom$}\n~~~\n\n### Replace in template\n\nAs above, but instead of just adding the code to the head, it replaces arbitrary text in the template. You need to give it a pattern and a replacement text. Optionally you can use the flag "add" to not replace the text, but prepend to it and the field "count" if only some matches should be replaced.\n\n~~~yaml\nTest-style:\n  html:\n    replace-in-template:\n      - pattern: \\$body\\$\n        replacement-text: |\n          <div class="content">\n          $body$\n          </div>\n~~~\n\n### Replace in output\n\nExactly the same as replace-in-template but for text in the output-file\n\n### Postflight\n\nThese scripts are called after the source is converted. Pretty similar to preflight, but instead of `<files>` it only accepts a single `<file>`\n\n**Some app:**\n\n~~~yaml\nTest-style:\n  html:\n    preflight:\n      - \'some_app -d -f <file>\'\n~~~\n\n**Custome script:**\n\n~~~python\nfrom pandoc_styles import run_postflight_script, file_read, file_write\n\n\ndef postflight(self):\n    text_to_append = self.cfg["append-to-output"]\n    if isinstance(text_to_append, list):\n        text_to_append = "\\n".join(text_to_append)\n    file_write(ffile, f"{file_read(ffile)}\\n{text_to_append}")\n\n\nif __name__ == \'__main__\':\n    run_postflight_script(postflight)\n~~~\n\n~~~yaml\nTest-style:\n  html:\n    preflight:\n      - append-to-output.py\n    append-to-output: "Test"\n~~~\n\n### Filter\n\nThis script includes some functionality to make writing filters a little bit more easy.\n\n### Advanced Example\n\nPandocs self-contained flag doesn\'t work for html if math is used, because mathjax can\'t be included. This style is not really self-contained, but it allows for single files with all css included. This example useses the default.sass file included in this script. Fonts are also just referenced instead of included, to make for small file-sizes.\n\nFor code in pdfs, it introduces line-wrap in code blocks and ligatures in the font.\n\nIn addition, inheritance is shown.\n\n~~~yaml\nAll:\n  all:\n    lang: en\n  pdf:\n    pdf-engine: "xelatex"\n\nMath-document:\n  inherits:\n    - Code\n  html:\n    self-contained: true\n    mathjax: true\n    sass:\n      files: ~/default.scss\n      output-path: temp\n    replace-in-template:\n      - pattern: \\$body\\$\n        replacement-text: |\n          <div class="content">\n          $body$\n          </div>\n      - pattern: \\$table-of-contents\\$\n        replacement-text: |\n          <div id="sidebar">\n          <input class="trigger" type="checkbox" id="mainNavButton">\n          <label for="mainNavButton" onclick></label>\n          $table-of-contents$\n          </div>\n    replace-in-output:\n      - pattern: (<\\/head>)\n        count: 1\n        add: true\n        replacement-text: |\n          <link href="https://fonts.googleapis.com/css?family=Noto+Sans|Noto+Serif|Oswald" rel="stylesheet">\n          <link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/tonsky/FiraCode@1.206/distr/fira_code.css">\n      - pattern: <script type="text\\/javascript">\\/\\*\\n\\s+\\*\\s+\\/MathJax\\.js.*?<\\/script>\n        replacement-text: |\n          <script src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.2/MathJax.js?config=TeX-AMS_CHTML-full" type="text/javascript"></script>\n\nCode:\n  all:\n    highlight-style: tango\n  pdf:\n    monofont: Fira Code\n    # allow code line break\n    add-to-template:\n      - |\n        \\usepackage{fvextra}\n        \\DefineVerbatimEnvironment{Highlighting}{Verbatim}{breaklines,breakautoindent=true,commandchars=\\\\\\{\\}}\n      - |\n        \\setmonofont[\n          Contextuals={Alternate}\n        ]{$monofont$}\n        \\makeatletter\n        \\def\\verbatim@nolig@list{}\n        \\makeatother\n~~~\n\n## Commandline tools\n\nSome additional tools are available on the commandline with the command:\n\n```bash\npandoc-styles-tools\n```\n\nThe import option is used to import stylepacks.\n\nOne tool merges styles and outputs the new style in a file.\n\nThe localize tool copies all used assets into the local directory, to have a self-contingent project folder.\n\n## Creating stylepacks\n\nTo create a stylepack, just create a folder with the name of the stylepack. Inside the folder put a yaml file containing the style definitions with the name of the stylepack. Then mimick the config folder for organizing the files provided.\n\nIn the yaml file reference links to files inside the stylepack with "stylepack_name@path".\n\nCreate a zip of your folder (with the folder inside the zip) and name it after your stylepack.\n',
     'author': 'dickloraine',
     'author_email': 'dickloraine@gmx.net',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/dickloraine/pandoc_styles',
```

### Comparing `pandoc_styles-0.9.8/PKG-INFO` & `pandoc_styles-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandoc-styles
-Version: 0.9.8
+Version: 0.9.9
 Summary: A script to convert files with pandoc using styles.
 Home-page: https://github.com/dickloraine/pandoc_styles
 License: MIT
 Keywords: pandoc,writing,text,conversion
 Author: dickloraine
 Author-email: dickloraine@gmx.net
 Requires-Python: >=3.6,<4.0
```

