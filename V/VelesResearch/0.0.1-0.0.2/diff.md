# Comparing `tmp/VelesResearch-0.0.1.tar.gz` & `tmp/VelesResearch-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VelesResearch-0.0.1.tar", last modified: Fri Jun  9 00:27:22 2023, max compression
+gzip compressed data, was "VelesResearch-0.0.2.tar", last modified: Fri Jun  9 19:22:17 2023, max compression
```

## Comparing `VelesResearch-0.0.1.tar` & `VelesResearch-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jakub     (1000) jakub     (1000)        0 2023-06-09 00:27:22.802350 VelesResearch-0.0.1/
--rw-r--r--   0 jakub     (1000) jakub     (1000)      298 2023-06-09 00:27:22.802350 VelesResearch-0.0.1/PKG-INFO
--rw-r--r--   0 jakub     (1000) jakub     (1000)     1150 2023-06-06 20:34:45.000000 VelesResearch-0.0.1/README.md
-drwxr-xr-x   0 jakub     (1000) jakub     (1000)        0 2023-06-09 00:27:22.802350 VelesResearch-0.0.1/VelesResearch.egg-info/
--rw-r--r--   0 jakub     (1000) jakub     (1000)      298 2023-06-09 00:27:22.000000 VelesResearch-0.0.1/VelesResearch.egg-info/PKG-INFO
--rw-r--r--   0 jakub     (1000) jakub     (1000)      334 2023-06-09 00:27:22.000000 VelesResearch-0.0.1/VelesResearch.egg-info/SOURCES.txt
--rw-r--r--   0 jakub     (1000) jakub     (1000)        1 2023-06-09 00:27:22.000000 VelesResearch-0.0.1/VelesResearch.egg-info/dependency_links.txt
--rw-r--r--   0 jakub     (1000) jakub     (1000)       15 2023-06-09 00:27:22.000000 VelesResearch-0.0.1/VelesResearch.egg-info/top_level.txt
--rw-r--r--   0 jakub     (1000) jakub     (1000)       38 2023-06-09 00:27:22.802350 VelesResearch-0.0.1/setup.cfg
--rw-r--r--   0 jakub     (1000) jakub     (1000)      536 2023-06-08 19:16:48.000000 VelesResearch-0.0.1/setup.py
-drwxr-xr-x   0 jakub     (1000) jakub     (1000)        0 2023-06-09 00:27:22.802350 VelesResearch-0.0.1/veles_research/
--rw-r--r--   0 jakub     (1000) jakub     (1000)      114 2023-06-08 20:34:09.000000 VelesResearch-0.0.1/veles_research/__init__.py
--rw-r--r--   0 jakub     (1000) jakub     (1000)     1004 2023-06-09 00:06:20.000000 VelesResearch-0.0.1/veles_research/options.py
--rw-r--r--   0 jakub     (1000) jakub     (1000)     1343 2023-06-08 21:24:52.000000 VelesResearch-0.0.1/veles_research/question_types.py
--rw-r--r--   0 jakub     (1000) jakub     (1000)     3684 2023-06-09 00:06:54.000000 VelesResearch-0.0.1/veles_research/structure.py
--rw-r--r--   0 jakub     (1000) jakub     (1000)      736 2023-06-08 23:43:17.000000 VelesResearch-0.0.1/veles_research/survey_tools.py
--rw-r--r--   0 jakub     (1000) jakub     (1000)     1077 2023-06-08 23:10:02.000000 VelesResearch-0.0.1/veles_research/test.py
+drwxr-xr-x   0 jakub     (1000) jakub     (1000)        0 2023-06-09 19:22:17.037184 VelesResearch-0.0.2/
+-rw-r--r--   0 jakub     (1000) jakub     (1000)      298 2023-06-09 19:22:17.033851 VelesResearch-0.0.2/PKG-INFO
+-rw-r--r--   0 jakub     (1000) jakub     (1000)     1261 2023-06-09 15:14:07.000000 VelesResearch-0.0.2/README.md
+drwxr-xr-x   0 jakub     (1000) jakub     (1000)        0 2023-06-09 19:22:17.033851 VelesResearch-0.0.2/VelesResearch/
+-rw-r--r--   0 jakub     (1000) jakub     (1000)      114 2023-06-08 20:34:09.000000 VelesResearch-0.0.2/VelesResearch/__init__.py
+-rw-r--r--   0 jakub     (1000) jakub     (1000)     1355 2023-06-09 17:35:19.000000 VelesResearch-0.0.2/VelesResearch/options.py
+-rw-r--r--   0 jakub     (1000) jakub     (1000)     1656 2023-06-09 18:41:19.000000 VelesResearch-0.0.2/VelesResearch/question_types.py
+-rw-r--r--   0 jakub     (1000) jakub     (1000)     4456 2023-06-09 18:41:06.000000 VelesResearch-0.0.2/VelesResearch/structure.py
+-rw-r--r--   0 jakub     (1000) jakub     (1000)     1377 2023-06-09 18:43:57.000000 VelesResearch-0.0.2/VelesResearch/survey_tools.py
+-rw-r--r--   0 jakub     (1000) jakub     (1000)     1391 2023-06-09 18:04:17.000000 VelesResearch-0.0.2/VelesResearch/test.py
+drwxr-xr-x   0 jakub     (1000) jakub     (1000)        0 2023-06-09 19:22:17.033851 VelesResearch-0.0.2/VelesResearch.egg-info/
+-rw-r--r--   0 jakub     (1000) jakub     (1000)      298 2023-06-09 19:22:17.000000 VelesResearch-0.0.2/VelesResearch.egg-info/PKG-INFO
+-rw-r--r--   0 jakub     (1000) jakub     (1000)      328 2023-06-09 19:22:17.000000 VelesResearch-0.0.2/VelesResearch.egg-info/SOURCES.txt
+-rw-r--r--   0 jakub     (1000) jakub     (1000)        1 2023-06-09 19:22:17.000000 VelesResearch-0.0.2/VelesResearch.egg-info/dependency_links.txt
+-rw-r--r--   0 jakub     (1000) jakub     (1000)       14 2023-06-09 19:22:17.000000 VelesResearch-0.0.2/VelesResearch.egg-info/top_level.txt
+-rw-r--r--   0 jakub     (1000) jakub     (1000)       38 2023-06-09 19:22:17.037184 VelesResearch-0.0.2/setup.cfg
+-rw-r--r--   0 jakub     (1000) jakub     (1000)      536 2023-06-09 19:21:23.000000 VelesResearch-0.0.2/setup.py
```

### Comparing `VelesResearch-0.0.1/README.md` & `VelesResearch-0.0.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -3,36 +3,34 @@
     <source media="(prefers-color-scheme: dark)" srcset="./figs/Veles-logo-white.svg">
     <source media="(prefers-color-scheme: light)" srcset="./figs/Veles-logo.svg">
     <img alt="Veles logo, text Veles with Veles' rune instead of V." src="Veles-logo.svg" width=60%>
   </picture>
 </p>
 <br>
 
-Veles is a free and open source research tool, primarly for social scientists. It's goal is to provide an interface for surveys and chronometric experiments. It combines the power of Survey.js and PsychoPy (PsychJS) to create self contained units that can be self-hosted. Veles' own web service for creating and hosting experiments is planned.
+Veles is a free and open source python research package, primarly for social scientists. It's goal is to provide an interface for surveys and chronometric experiments. It combines the power of Survey.js and PsychoJS (PsychoPy) with python interface to create self contained research units that can be self-hosted. Veles' own web service for creating and hosting experiments are planned.
 
 Veles is in pre-alpha development, but the goal features are:
 
-- Free and open source.
+-   Free and open source.
 
-- Text-based with optional GUI.
+-   Text-based, so automatable and easily modifiable.
 
-- Integration with GitHub.
+-   Integration with GitHub.
 
-- Ability to use JavaScript and CSS drectly.
+-   Ability to use JavaScript and CSS directly.
 
-- Syntax highlighting.
+-   [Open source documentation](https://jakub-jedrusiak.github.io/veles-docs/).
 
-- Open source documentation.
+-   Python-based, so every python tools work.
 
-- Collaboration features.
+-   Esay to collaborate through git.
 
-- VS code extension pack.
+-   VS code extension pack.
 
-- Custom redirection in the end (for panels).
+-   Custom redirection in the end (for panels).
 
-- PsychoPy integration?
+-   PsychoPy integration.
 
-- Real logs and debug window with variables.
+-   JavaScript code preview.
 
-- Real time JavaScript code preview.
-
-- Modifiable themes.
+-   Modifiable themes.
```

### Comparing `VelesResearch-0.0.1/setup.py` & `VelesResearch-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 DESCRIPTION = "Surveys and experiments tool"
 LONG_DESCRIPTION = "Free and open source surveys and experiments tool for social sciences"
 
 setup(
     name="VelesResearch",
     version = VERSION,
     author = "Jakub Jędrusiak",
```

### Comparing `VelesResearch-0.0.1/veles_research/options.py` & `VelesResearch-0.0.2/VelesResearch/options.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 from typeguard import typechecked
 
 from typing import Optional
 
 @typechecked
-class Question_options:
-    def __init__(self, required: bool=False, answers_order: str="none", inherit_answers: Optional[str]=None, comment: bool=False, comment_text: str="Other", comment_placeholder: str="", visible: bool=True):
+class QuestionOptions:
+    def __init__(self, required: bool=False, answers_order: str="none", inherit_answers: Optional[str]=None, comment: bool=False, comment_text: str="Other", comment_placeholder: str="", visible: bool=True, other: bool=False, other_text: str="Other", other_placeholder: str="", none: bool=False, none_text: str="None", clear_button: bool=False):
         self.required = required
         self.answers_order = answers_order
         self.inherit_answers = inherit_answers
         self.comment = comment
         self.comment_text = comment_text
         self.comment_placeholder = comment_placeholder
         self.visible = visible
+        self.other = other
+        self.other_text = other_text
+        self.other_placeholder = other_placeholder
+        self.none = none
+        self.none_text = none_text
+        self.clear_button = clear_button
 
-class Page_options:
+class PageOptions:
     def __init__(self, read_only: bool=False, time_limit: Optional[int]=None, visible: bool=True):
         self.read_only = read_only
         self.time_limit = time_limit
         self.visible = visible
         
-class Survey_options:
+class SurveyOptions:
     def __init__(self, language: str="en", url_on_complete: Optional[str]=None):
         self.language = language
         self.url_on_complete = url_on_complete
```

### Comparing `VelesResearch-0.0.1/veles_research/question_types.py` & `VelesResearch-0.0.2/VelesResearch/question_types.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 "Classes for different types of questions"
 
 from typeguard import typechecked
 
-from typing import Optional, List
+from typing import Optional, List, Union, Sequence
 from json import dumps
-from options import Question_options
+from options import QuestionOptions
 
 @typechecked
 class Question:
     "General question class"
 
-    def __init__(self, label: str, question_type: str, question_text: str, answers: List[str], options: Optional[Question_options]=None, description: Optional[str]=None):
+    def __init__(self, label: str, question_type: str, question_text: str, *answers: Union[str, Sequence[str]], options: Optional[QuestionOptions]=None, description: Optional[str]=None):
         self.label = label
         self.question_type = question_type
         self.question_text = question_text
         self.answers = answers
         self.options = options
         self.description = description
 
@@ -26,16 +26,14 @@
         return f"Question({self.label})"
 
     def json(self):
         "Converts question to SurveyJS-compliant json"
         from structure import SurveyEncoder
         return dumps(self, cls=SurveyEncoder, indent=4)
 
-
-def radio(label, options, question_text, answers):
+def radio(self, label: str, question_text: str, *answers: Union[str, List[str]], options: Optional[QuestionOptions]=None, description: Optional[str]=None):
     "Single choice question"
-    return Question(label, "radio", options, question_text, answers)
-
+    return Question(label, "radio", options, question_text, answers, options=options, description=description)
 
-def checkbox(label, options, question_text, answers):
-    "Multiple choice question class"
-    return Question(label, "checkbox", options, question_text, answers)
+def radio(self, label: str, question_text: str, *answers: Union[str, List[str]], options: Optional[QuestionOptions]=None, description: Optional[str]=None):
+    "Single choice question"
+    return Question(label, "checkbox", options, question_text, answers, options=options, description=description)
```

### Comparing `VelesResearch-0.0.1/veles_research/structure.py` & `VelesResearch-0.0.2/VelesResearch/structure.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 from typeguard import typechecked
 
 from typing import Union, List, Optional
 from json import JSONEncoder
 from numpy import concatenate, array
 from question_types import Question
+from options import *
 
 @typechecked
 class Page:
-    def __init__(self, label: str, *questions: Union[Question, List[Question]], title: Optional[str]=None, description: Optional[str]=None, options: Optional[Page_options]=None):
+    def __init__(self, label: str, *questions: Union[Question, List[Question]], title: Optional[str]=None, description: Optional[str]=None, options: Optional[PageOptions]=None):
         self.label = label
         self.questions = list(concatenate([questions]).flat)
         self.title = title
         self.description = description
+        self.options = options
 
 @typechecked
 class Survey:
-    def __init__(self, *pages: Union[Page, List[Page]], title: Optional[str]=None, description: Optional[str]=None, options: Optional[Survey_options]=None):
+    def __init__(self, *pages: Union[Page, List[Page]], title: Optional[str]=None, description: Optional[str]=None, options: Optional[SurveyOptions]=None):
         self.pages = list(concatenate([pages]).flat)
         self.title = title
         self.description = description
-        self.language = language
+        self.options = options
     
     def json(self):
         from json import dumps
         return dumps(obj=self, cls=SurveyEncoder, indent=2)
     
     def create(self):
         from json import dumps
@@ -73,15 +75,15 @@
             # SurveyJS types dictionary
             surveyjs_types = {"radio": "radiogroup", "checkbox": "checkbox"}
             
             json = {
                 "name": o.label,
                 "type": surveyjs_types[o.question_type],
                 "title": o.question_text,
-                "choices": o.answers
+                "choices": list(concatenate([o.answers]).flat)
             }
             
             if o.description:
                 json["description"] = o.description
                 
             if o.options:
                 opts = o.options.__dict__
@@ -91,11 +93,25 @@
                     json["isRequired"] = True
                 if opts["answers_order"] != "none":
                     json["choicesOrder"] = opts["answers_order"]
                 if opts["inherit_answers"]:
                     json["choicesFromQuestion"] = opts["inherit_answers"]
                 if opts["comment"]:
                     json["showCommentArea"] = True
-                    json["commentText"] = opts["comment_text"]
-                    json["commentPlaceholder"] = opts["comment_placeholder"]
+                    if opts["comment_text"]:
+                        json["commentText"] = opts["comment_text"]
+                    if opts["comment_placeholder"]:
+                        json["commentPlaceholder"] = opts["comment_placeholder"]
+                if opts["other"]:
+                    json["showOtherItem"] = True
+                    if opts["other_text"]:
+                        json["otherText"] = opts["other_text"]
+                    if opts["other_placeholder"]:
+                        json["otherPlaceHolder"] = opts["other_placeholder"]
+                if opts["none"]:
+                    json["showNoneItem"] = True
+                    if opts["none_text"]:
+                        json["noneText"] = opts["none_text"]
+                if opts["clear_button"]:
+                    json["showClearButton"] = True
             
         return json
```

### Comparing `VelesResearch-0.0.1/veles_research/test.py` & `VelesResearch-0.0.2/VelesResearch/test.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,48 @@
-from json import dumps
-from question_types import Question
-from survey_tools import *
+from question_types import *
 from structure import *
-from options import Question_options
+from options import *
+from survey_tools import *
+
 
 RSSI = """I feel that I am a person of worth, at least on an equal plane with others.
 I feel that I have a number of good qualities.
 All in all, I am inclined to feel that I am a failure.
 I am able to do things as well as most other people.
 I feel I do not have much to be proud of.
 I take a positive attitude toward myself.
 On the whole, I am satisfied with myself.
 I wish I could have more respect for myself.
 I certainly feel useless at times.
 At times I think I am no good at all.""".split("\n")
 
 scale = ["Strongly Agree", "Agree", "Disagree", "Strongly Disagree"]
 
-opts = Question_options(required=True)
+opts = QuestionOptions(required=True)
 
 q = questionnaire("RSSI", RSSI, scale, options=opts)
 
 q1 = Question("RSSI_1", "radio", RSSI[0], scale, options=opts)
 
 p = Page("RSSI", q)
 
 s = Survey(p, title="Rosenberg Self-Esteem Scale", description="This scale is a measure of self-esteem, that is, how positively or negatively people view themselves.")
 
-s.create()
+s.create()
+
+gender = question(
+  "gender",
+  "radio",
+  "What is your gender?",
+  "Woman",
+  "Man",
+  options=QuestionOptions(
+    answers_order="random",
+    none=True,
+    none_text="I don't want to answer",
+    other=True,
+    other_placeholder="Write your gender."
+  ),
+  description="Choose an answer from options below."
+)
+
+Survey(Page("metric", gender)).create()
```

