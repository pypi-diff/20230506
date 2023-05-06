# Comparing `tmp/prettycopy-0.1.3.tar.gz` & `tmp/prettycopy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prettycopy-0.1.3.tar", last modified: Sun Apr 23 15:10:27 2023, max compression
+gzip compressed data, was "prettycopy-0.2.0.tar", last modified: Sat May  6 02:30:39 2023, max compression
```

## Comparing `prettycopy-0.1.3.tar` & `prettycopy-0.2.0.tar`

### file list

```diff
@@ -1,34 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 15:10:27.118782 prettycopy-0.1.3/
--rw-rw-rw-   0        0        0      533 2023-04-23 00:51:02.000000 prettycopy-0.1.3/.bumpversion.cfg
--rw-rw-rw-   0        0        0      772 2023-04-17 05:17:35.000000 prettycopy-0.1.3/.readthedocs.yaml
--rw-rw-rw-   0        0        0     2197 2023-04-17 05:17:35.000000 prettycopy-0.1.3/CONTRIBUTING.md
--rw-rw-rw-   0        0        0    11558 2023-02-08 23:02:52.000000 prettycopy-0.1.3/LICENSE
--rw-rw-rw-   0        0        0      584 2023-04-17 05:17:35.000000 prettycopy-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2254 2023-04-22 23:54:45.000000 prettycopy-0.1.3/Makefile
--rw-rw-rw-   0        0        0    17353 2023-04-23 15:10:27.115781 prettycopy-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     3303 2023-04-22 23:35:54.000000 prettycopy-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 15:10:27.052800 prettycopy-0.1.3/docs/
--rw-rw-rw-   0        0        0      634 2023-03-31 21:48:57.000000 prettycopy-0.1.3/docs/Makefile
--rw-rw-rw-   0        0        0     1302 2023-04-23 00:51:02.000000 prettycopy-0.1.3/docs/conf.py
--rw-rw-rw-   0        0        0     2198 2023-04-22 23:18:03.000000 prettycopy-0.1.3/docs/dev_intro.md
-drwxrwxrwx   0        0        0        0 2023-04-23 15:10:27.056795 prettycopy-0.1.3/docs/images/
--rw-rw-rw-   0        0        0   185808 2023-04-17 05:17:35.000000 prettycopy-0.1.3/docs/images/bullettopar.gif
--rw-rw-rw-   0        0        0     4749 2023-04-22 23:35:54.000000 prettycopy-0.1.3/docs/index.md
--rwxrwxrwx   0        0        0      765 2023-03-31 21:48:57.000000 prettycopy-0.1.3/docs/make.bat
--rw-rw-rw-   0        0        0       64 2023-04-23 00:24:41.000000 prettycopy-0.1.3/docs/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-04-23 15:10:27.073796 prettycopy-0.1.3/prettycopy/
--rw-rw-rw-   0        0        0      103 2023-04-23 00:51:02.000000 prettycopy-0.1.3/prettycopy/__init__.py
--rw-rw-rw-   0        0        0       82 2023-03-04 17:13:11.000000 prettycopy-0.1.3/prettycopy/__main__.py
--rw-rw-rw-   0        0        0       22 2023-04-23 00:51:02.000000 prettycopy-0.1.3/prettycopy/_version.py
--rw-rw-rw-   0        0        0    11294 2023-04-22 23:35:54.000000 prettycopy-0.1.3/prettycopy/prettycopy.py
-drwxrwxrwx   0        0        0        0 2023-04-23 15:10:27.103947 prettycopy-0.1.3/prettycopy/tests/
--rw-rw-rw-   0        0        0    16889 2023-04-22 23:35:54.000000 prettycopy-0.1.3/prettycopy/tests/test_all.py
-drwxrwxrwx   0        0        0        0 2023-04-23 15:10:27.100039 prettycopy-0.1.3/prettycopy.egg-info/
--rw-rw-rw-   0        0        0    17353 2023-04-23 15:10:26.000000 prettycopy-0.1.3/prettycopy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      528 2023-04-23 15:10:26.000000 prettycopy-0.1.3/prettycopy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 15:10:26.000000 prettycopy-0.1.3/prettycopy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      253 2023-04-23 15:10:26.000000 prettycopy-0.1.3/prettycopy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-23 15:10:26.000000 prettycopy-0.1.3/prettycopy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2297 2023-04-23 00:51:02.000000 prettycopy-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-23 15:10:27.122780 prettycopy-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0       39 2023-03-02 04:28:18.000000 prettycopy-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 02:30:39.972949 prettycopy-0.2.0/
+-rw-rw-rw-   0        0        0      533 2023-05-04 21:01:54.000000 prettycopy-0.2.0/.bumpversion.cfg
+-rw-rw-rw-   0        0        0      772 2023-04-17 05:17:35.000000 prettycopy-0.2.0/.readthedocs.yaml
+-rw-rw-rw-   0        0        0     2197 2023-04-17 05:17:35.000000 prettycopy-0.2.0/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0    11558 2023-02-08 23:02:52.000000 prettycopy-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      584 2023-04-17 05:17:35.000000 prettycopy-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2254 2023-04-22 23:54:45.000000 prettycopy-0.2.0/Makefile
+-rw-rw-rw-   0        0        0    18270 2023-05-06 02:30:39.970973 prettycopy-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4210 2023-05-06 02:29:22.000000 prettycopy-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 02:30:39.863949 prettycopy-0.2.0/docs/
+-rw-rw-rw-   0        0        0      634 2023-03-31 21:48:57.000000 prettycopy-0.2.0/docs/Makefile
+-rw-rw-rw-   0        0        0     1302 2023-05-04 21:01:54.000000 prettycopy-0.2.0/docs/conf.py
+-rw-rw-rw-   0        0        0     2343 2023-05-03 21:49:41.000000 prettycopy-0.2.0/docs/dev_intro.md
+drwxrwxrwx   0        0        0        0 2023-05-06 02:30:39.923951 prettycopy-0.2.0/docs/images/
+-rw-rw-rw-   0        0        0   563910 2023-05-04 20:53:34.000000 prettycopy-0.2.0/docs/images/bullets_nopc.gif
+-rw-rw-rw-   0        0        0   464377 2023-05-04 20:53:34.000000 prettycopy-0.2.0/docs/images/bullettopar_pc.gif
+-rw-rw-rw-   0        0        0   471068 2023-05-06 02:29:22.000000 prettycopy-0.2.0/docs/images/nobullets_pc.gif
+-rw-rw-rw-   0        0        0    72027 2023-05-03 21:49:41.000000 prettycopy-0.2.0/docs/images/pchelp.gif
+-rw-rw-rw-   0        0        0   161236 2023-05-03 21:49:41.000000 prettycopy-0.2.0/docs/images/pcnonewlines.gif
+-rw-rw-rw-   0        0        0   324242 2023-05-04 20:53:34.000000 prettycopy-0.2.0/docs/images/quote_pc.gif
+-rw-rw-rw-   0        0        0   292299 2023-05-04 20:53:34.000000 prettycopy-0.2.0/docs/images/quotes_nopc.gif
+-rw-rw-rw-   0        0        0   297103 2023-05-04 20:53:34.000000 prettycopy-0.2.0/docs/images/simplequote_pc.gif
+-rw-rw-rw-   0        0        0   312971 2023-05-04 20:53:34.000000 prettycopy-0.2.0/docs/images/smartcopy_pc.gif
+-rw-rw-rw-   0        0        0   151015 2023-05-04 20:53:34.000000 prettycopy-0.2.0/docs/images/trimspace_nopc.gif
+-rw-rw-rw-   0        0        0   164560 2023-05-04 20:53:34.000000 prettycopy-0.2.0/docs/images/trimspacing_pc.gif
+-rw-rw-rw-   0        0        0     7654 2023-05-06 02:29:22.000000 prettycopy-0.2.0/docs/index.md
+-rwxrwxrwx   0        0        0      765 2023-03-31 21:48:57.000000 prettycopy-0.2.0/docs/make.bat
+-rw-rw-rw-   0        0        0       64 2023-04-23 00:24:41.000000 prettycopy-0.2.0/docs/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-05-06 02:30:39.941949 prettycopy-0.2.0/prettycopy/
+-rw-rw-rw-   0        0        0      103 2023-05-04 21:01:54.000000 prettycopy-0.2.0/prettycopy/__init__.py
+-rw-rw-rw-   0        0        0       69 2023-05-03 21:49:41.000000 prettycopy-0.2.0/prettycopy/__main__.py
+-rw-rw-rw-   0        0        0       22 2023-05-04 21:01:54.000000 prettycopy-0.2.0/prettycopy/_version.py
+-rw-rw-rw-   0        0        0     3256 2023-05-06 02:29:22.000000 prettycopy-0.2.0/prettycopy/command_line.py
+-rw-rw-rw-   0        0        0    11579 2023-05-06 02:29:22.000000 prettycopy-0.2.0/prettycopy/prettycopy.py
+drwxrwxrwx   0        0        0        0 2023-05-06 02:30:39.966951 prettycopy-0.2.0/prettycopy/tests/
+-rw-rw-rw-   0        0        0    26120 2023-05-06 02:29:22.000000 prettycopy-0.2.0/prettycopy/tests/test_all.py
+drwxrwxrwx   0        0        0        0 2023-05-06 02:30:39.962955 prettycopy-0.2.0/prettycopy.egg-info/
+-rw-rw-rw-   0        0        0    18270 2023-05-06 02:30:39.000000 prettycopy-0.2.0/prettycopy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      880 2023-05-06 02:30:39.000000 prettycopy-0.2.0/prettycopy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 02:30:39.000000 prettycopy-0.2.0/prettycopy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-06 02:30:39.000000 prettycopy-0.2.0/prettycopy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      259 2023-05-06 02:30:39.000000 prettycopy-0.2.0/prettycopy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-06 02:30:39.000000 prettycopy-0.2.0/prettycopy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2371 2023-05-06 02:29:22.000000 prettycopy-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-06 02:30:39.973959 prettycopy-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0       39 2023-04-27 19:31:32.000000 prettycopy-0.2.0/setup.py
```

### Comparing `prettycopy-0.1.3/.bumpversion.cfg` & `prettycopy-0.2.0/.bumpversion.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.3
+current_version = 0.2.0
 commit = True
 tag = True
 
 [bumpversion:file:prettycopy/_version.py]
 search = __version__ = "{current_version}"
 replace = __version__ = "{new_version}"
```

### Comparing `prettycopy-0.1.3/.readthedocs.yaml` & `prettycopy-0.2.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `prettycopy-0.1.3/CONTRIBUTING.md` & `prettycopy-0.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `prettycopy-0.1.3/LICENSE` & `prettycopy-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prettycopy-0.1.3/MANIFEST.in` & `prettycopy-0.2.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `prettycopy-0.1.3/Makefile` & `prettycopy-0.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `prettycopy-0.1.3/PKG-INFO` & `prettycopy-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prettycopy
-Version: 0.1.3
+Version: 0.2.0
 Summary: A better copy-paster
 Author-email: Adi Gal <adigal03@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -243,21 +243,31 @@
 
 If you already have Python, just run:
 
 ```bash
 pip install prettycopy
 ```
 
-### Usage
+## Usage
 
-Copy a piece of text. Run a PrettyCopy function. Now, when you paste, the text will already by corrected. That's all!
+So... how do you use PrettyCopy? It's very simple! You can use PrettyCopy at the command line, or through your own program.
 
-For added flexibility:
+### Command Line
+Copy a piece of text.
+In the command line, type `prettycopy [function_name] [any_args]`. 
+PrettyCopy will print the corrected text, just to show you what your clipboard current contains. 
+Now, as soon as you paste, the text will already be corrected.
 
-You can enter the text as an argument to the function, and PrettyCopy will automatically copy the corrected text to your clipboard. Plus, if you're using PrettyCopy functions through code, the functions return the corrected text as a string.
+If you want, you can add the option `--text "your_text_here"` to the instruction. In this case, PrettyCopy will take your inputted string, correct it, and place it in the clipboard. Remember to add quotation marks around your input string if it contains whitespace. This option can go anywhere as long as the input string is to the right of the --text flag.
+
+Confused? Type `prettycopy --help` to get a list of possible functions, and `prettycopy [function_name] --help` to get help for any particular function.
+
+### In a Program
+PrettyCopy will take in some text, correct it, and copy the corrected text to your clipboard. It will also return the corrected text as a return value, in case you want to keep using it (for example, in a nested function).
+By default, PrettyCopy will run on the text in your clipboard. If you want to correct a different text, enter your preferred text as an argument.
 
 ### Functions
 
 `prettycopy.nonewlines(optional_text)`: Removes all line breaks from the text.
 
 `prettycopy.nobullets(optional_text)`: Removes all bullet symbols (•) and replaces them with line breaks.
```

### Comparing `prettycopy-0.1.3/docs/Makefile` & `prettycopy-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `prettycopy-0.1.3/docs/conf.py` & `prettycopy-0.2.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'prettycopy'
 copyright = '2023, Adi Gal'
 author = 'Adi Gal'
-release = "0.1.3"
+release = "0.2.0"
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = ['myst_parser', 'sphinx.ext.autodoc', 'sphinx.ext.githubpages'] #prev, recommonmark
 source_suffix = ['.rst', '.md']
```

### Comparing `prettycopy-0.1.3/docs/dev_intro.md` & `prettycopy-0.2.0/docs/dev_intro.md`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 - Anything else you think is relevant.
 
 The more information you give us, the more likely it is that we can find a solution!
 
 ## Developing
 Want to help with development? Even better! Here's how to begin.
 
+(Note: PrettyCopy comes equipped with a Makefile, so you'll be able to simply type 'make [X]' into the command line for a lot of the commands.)
+
 ### Setup
 Prerequisites: Install Python. At the moment, PrettyCopy runs on Python version 3.7 and higher.
 
 1. Fork the repository on GitHub.
 2. Clone your forked repository to your local computer using `git clone https://github.com/[YOUR_USERNAME]/prettycopy.git`
 3. Navigate to the folder, and type `make develop` to install the development dependencies. (You can check the file *pyproject.toml* to see what they are.)
 4. Congrats, you're ready to get started coding!
```

### Comparing `prettycopy-0.1.3/docs/make.bat` & `prettycopy-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `prettycopy-0.1.3/prettycopy/prettycopy.py` & `prettycopy-0.2.0/prettycopy/prettycopy.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,26 +6,30 @@
 
 from google.auth.transport.requests import Request
 from google.oauth2.credentials import Credentials
 from google_auth_oauthlib.flow import InstalledAppFlow
 
 import googleapiclient.discovery
 
-# TODO add to list of reqs
 import nltk
 from nltk import tokenize
 from nltk.corpus import words
 from textblob import TextBlob
 from spellchecker import SpellChecker
 
 try:
     nltk.data.find('tokenizers/words')
 except LookupError:
     nltk.download("words", quiet=True)
 
+try:
+    nltk.data.find('tokenizers/punkt')
+except LookupError:
+    nltk.download("punkt", quiet=True)
+
 
 # PUBLIC FUNCTIONS
 
 
 def nonewlines(text=None):
     """Remove all newlines.
 
@@ -69,15 +73,15 @@
 
     """
     if text is None:
         text = pyperclip.paste()
     if not isinstance(text, str):
         raise ValueError("PrettyCopy can only take in strings!")
 
-    text = nonewlines().strip("• ")
+    text = nonewlines(text).strip("• ")
     text = re.sub(r"\s*•\s*", "\n", text)
     pyperclip.copy(text)
     return text
 
 
 def bullettopar(text=None):
     """Remove newlines, replace bullets with spaces
@@ -122,21 +126,25 @@
 
     """
     if text is None:
         text = pyperclip.paste()
     if not isinstance(text, str):
         raise ValueError("PrettyCopy can only take in strings!")
 
-    text = '"' + text + '"'
+    text = text.strip()
+    if text[0] == '"' and text[-1] == '"':
+        return smartcopy(text)
+
+    text = '"' + smartcopy(text) + '"'
     pyperclip.copy(text)
     return text
 
 
 def quote(end_punctuation=None, text=None):
-    """Add quotes (and optional comma) around clipboard contents.
+    """Add quotes (and optional punctuation) around clipboard contents.
 
     Adds quotation marks and end punctuation to a text input from the argument or (by default) the clipboard.
 
     Args:
         end_punctuation (str): A single-character string containing one of: [.,!?]
         text (str): Any text; optional, default None.
 
@@ -148,22 +156,26 @@
 
     """
     if text is None:
         text = pyperclip.paste()
     if not isinstance(text, str):
         raise ValueError("PrettyCopy can only take in strings!")
 
+    text = text.strip()
+    if text[0] == '"' and text[-1] == '"':
+        return smartcopy(text)
+
     if end_punctuation is not None:
         if len(end_punctuation) != 1:
             raise ValueError("End punctuation should be a single character.")
         elif end_punctuation not in [',', '.', '!', '?']:
             raise ValueError("End punctuation should be one of: [.,!?]")
-        text = '"' + text + end_punctuation + '"'
+        text = '"' + smartcopy(text) + end_punctuation + '"'
     else:
-        text = '"' + text + ',"'
+        text = '"' + smartcopy(text) + '"'
     pyperclip.copy(text)
     return text
 
 
 def trimspacing(text=None):
     """Removes empty lines clipboard contents.
 
@@ -350,20 +362,19 @@
     except HttpError as err:
         print(err)
         return
 
     return service
 
 
-# Removes newlines from a sentence,
-# adding a space if it's surrounded by recognizable English words
-# and no space if it isn't.
-# RETURNS NOTHING.
-# TODO that's an anti-pattern imo
 def _cleanlines(line):
+    """
+    Removes newlines from a given line, adding a space if it's surrounded by
+    recognizable English words, and no space if it isn't.
+    """
     spell = SpellChecker()
     # remove newlines "within words"
     for match in re.finditer(r"([A-Za-z0-9]+)(\r?\n)+([A-Za-z0-9]+)", line):
         b1 = TextBlob(match.group(1))
         b2 = TextBlob(match.group(3))
 
         loc = line.find(str(match.group(1) + match.group(2) + match.group(3))) + len(match.group(1))
```

### Comparing `prettycopy-0.1.3/prettycopy.egg-info/PKG-INFO` & `prettycopy-0.2.0/prettycopy.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prettycopy
-Version: 0.1.3
+Version: 0.2.0
 Summary: A better copy-paster
 Author-email: Adi Gal <adigal03@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -243,21 +243,31 @@
 
 If you already have Python, just run:
 
 ```bash
 pip install prettycopy
 ```
 
-### Usage
+## Usage
 
-Copy a piece of text. Run a PrettyCopy function. Now, when you paste, the text will already by corrected. That's all!
+So... how do you use PrettyCopy? It's very simple! You can use PrettyCopy at the command line, or through your own program.
 
-For added flexibility:
+### Command Line
+Copy a piece of text.
+In the command line, type `prettycopy [function_name] [any_args]`. 
+PrettyCopy will print the corrected text, just to show you what your clipboard current contains. 
+Now, as soon as you paste, the text will already be corrected.
 
-You can enter the text as an argument to the function, and PrettyCopy will automatically copy the corrected text to your clipboard. Plus, if you're using PrettyCopy functions through code, the functions return the corrected text as a string.
+If you want, you can add the option `--text "your_text_here"` to the instruction. In this case, PrettyCopy will take your inputted string, correct it, and place it in the clipboard. Remember to add quotation marks around your input string if it contains whitespace. This option can go anywhere as long as the input string is to the right of the --text flag.
+
+Confused? Type `prettycopy --help` to get a list of possible functions, and `prettycopy [function_name] --help` to get help for any particular function.
+
+### In a Program
+PrettyCopy will take in some text, correct it, and copy the corrected text to your clipboard. It will also return the corrected text as a return value, in case you want to keep using it (for example, in a nested function).
+By default, PrettyCopy will run on the text in your clipboard. If you want to correct a different text, enter your preferred text as an argument.
 
 ### Functions
 
 `prettycopy.nonewlines(optional_text)`: Removes all line breaks from the text.
 
 `prettycopy.nobullets(optional_text)`: Removes all bullet symbols (•) and replaces them with line breaks.
```

### Comparing `prettycopy-0.1.3/prettycopy.egg-info/SOURCES.txt` & `prettycopy-0.2.0/prettycopy.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -9,18 +9,30 @@
 setup.py
 docs/Makefile
 docs/conf.py
 docs/dev_intro.md
 docs/index.md
 docs/make.bat
 docs/requirements.txt
-docs/images/bullettopar.gif
+docs/images/bullets_nopc.gif
+docs/images/bullettopar_pc.gif
+docs/images/nobullets_pc.gif
+docs/images/pchelp.gif
+docs/images/pcnonewlines.gif
+docs/images/quote_pc.gif
+docs/images/quotes_nopc.gif
+docs/images/simplequote_pc.gif
+docs/images/smartcopy_pc.gif
+docs/images/trimspace_nopc.gif
+docs/images/trimspacing_pc.gif
 prettycopy/__init__.py
 prettycopy/__main__.py
 prettycopy/_version.py
+prettycopy/command_line.py
 prettycopy/prettycopy.py
 prettycopy.egg-info/PKG-INFO
 prettycopy.egg-info/SOURCES.txt
 prettycopy.egg-info/dependency_links.txt
+prettycopy.egg-info/entry_points.txt
 prettycopy.egg-info/requires.txt
 prettycopy.egg-info/top_level.txt
 prettycopy/tests/test_all.py
```

### Comparing `prettycopy-0.1.3/pyproject.toml` & `prettycopy-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -7,24 +7,25 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "prettycopy"
 authors = [{name = "Adi Gal", email = "adigal03@gmail.com"}]
 description="A better copy-paster"
 readme = "README.md"
-version = "0.1.3"
+version = "0.2.0"
 requires-python = ">=3.7"
 
 dependencies = [
     "pyperclip",
     "google-auth-oauthlib",
     "google-auth",
     "google-api-python-client",
     "nltk",
     "textblob",
+    "typer",
     "pyspellchecker",
 ]
 
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
@@ -32,14 +33,16 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
+[project.scripts]
+prettycopy = "prettycopy.command_line:app"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 repository = "https://github.com/hippothebrave/prettycopy"
```

