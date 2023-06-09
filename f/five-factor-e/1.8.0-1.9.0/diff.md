# Comparing `tmp/five-factor-e-1.8.0.tar.gz` & `tmp/five-factor-e-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "five-factor-e-1.8.0.tar", last modified: Sun Jan  8 23:23:36 2023, max compression
+gzip compressed data, was "five-factor-e-1.9.0.tar", last modified: Sat Apr  1 20:11:32 2023, max compression
```

## Comparing `five-factor-e-1.8.0.tar` & `five-factor-e-1.9.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 edmc      (1000) edmc      (1000)        0 2023-01-08 23:23:36.921620 five-factor-e-1.8.0/
--rw-r--r--   0 edmc      (1000) edmc      (1000)     1064 2022-11-05 15:16:21.000000 five-factor-e-1.8.0/LICENSE
--rw-r--r--   0 edmc      (1000) edmc      (1000)    11413 2023-01-08 23:23:36.921620 five-factor-e-1.8.0/PKG-INFO
--rw-r--r--   0 edmc      (1000) edmc      (1000)    10653 2023-01-08 20:07:23.000000 five-factor-e-1.8.0/README.md
-drwxr-xr-x   0 edmc      (1000) edmc      (1000)        0 2023-01-08 23:23:36.918620 five-factor-e-1.8.0/five_factor_e.egg-info/
--rw-r--r--   0 edmc      (1000) edmc      (1000)    11413 2023-01-08 23:23:36.000000 five-factor-e-1.8.0/five_factor_e.egg-info/PKG-INFO
--rw-r--r--   0 edmc      (1000) edmc      (1000)      512 2023-01-08 23:23:36.000000 five-factor-e-1.8.0/five_factor_e.egg-info/SOURCES.txt
--rw-r--r--   0 edmc      (1000) edmc      (1000)        1 2023-01-08 23:23:36.000000 five-factor-e-1.8.0/five_factor_e.egg-info/dependency_links.txt
--rw-r--r--   0 edmc      (1000) edmc      (1000)       51 2023-01-08 23:23:36.000000 five-factor-e-1.8.0/five_factor_e.egg-info/entry_points.txt
--rw-r--r--   0 edmc      (1000) edmc      (1000)       16 2023-01-08 23:23:36.000000 five-factor-e-1.8.0/five_factor_e.egg-info/requires.txt
--rw-r--r--   0 edmc      (1000) edmc      (1000)        8 2023-01-08 23:23:36.000000 five-factor-e-1.8.0/five_factor_e.egg-info/top_level.txt
-drwxr-xr-x   0 edmc      (1000) edmc      (1000)        0 2023-01-08 23:23:36.919620 five-factor-e-1.8.0/ipipneo/
--rw-r--r--   0 edmc      (1000) edmc      (1000)      127 2023-01-08 14:30:48.000000 five-factor-e-1.8.0/ipipneo/__init__.py
--rw-r--r--   0 edmc      (1000) edmc      (1000)     6670 2023-01-08 21:31:20.000000 five-factor-e-1.8.0/ipipneo/facet.py
--rw-r--r--   0 edmc      (1000) edmc      (1000)     5503 2023-01-08 23:10:21.000000 five-factor-e-1.8.0/ipipneo/ipipneo.py
--rw-r--r--   0 edmc      (1000) edmc      (1000)     2262 2023-01-08 15:03:24.000000 five-factor-e-1.8.0/ipipneo/model.py
--rw-r--r--   0 edmc      (1000) edmc      (1000)    32965 2023-01-08 15:04:22.000000 five-factor-e-1.8.0/ipipneo/norm.py
--rw-r--r--   0 edmc      (1000) edmc      (1000)    12279 2023-01-08 19:58:05.000000 five-factor-e-1.8.0/ipipneo/quiz.py
--rw-r--r--   0 edmc      (1000) edmc      (1000)     7190 2023-01-08 15:04:52.000000 five-factor-e-1.8.0/ipipneo/reverse.py
--rw-r--r--   0 edmc      (1000) edmc      (1000)     5669 2023-01-08 15:05:04.000000 five-factor-e-1.8.0/ipipneo/utility.py
--rw-r--r--   0 edmc      (1000) edmc      (1000)       38 2023-01-08 23:23:36.921620 five-factor-e-1.8.0/setup.cfg
--rw-r--r--   0 edmc      (1000) edmc      (1000)     1659 2023-01-08 15:05:35.000000 five-factor-e-1.8.0/setup.py
-drwxr-xr-x   0 edmc      (1000) edmc      (1000)        0 2023-01-08 23:23:36.920620 five-factor-e-1.8.0/test/
--rw-r--r--   0 edmc      (1000) edmc      (1000)    42034 2023-01-08 15:12:31.000000 five-factor-e-1.8.0/test/test_facet.py
--rw-r--r--   0 edmc      (1000) edmc      (1000)    15758 2023-01-08 15:25:08.000000 five-factor-e-1.8.0/test/test_ipipneo.py
--rw-r--r--   0 edmc      (1000) edmc      (1000)     6629 2023-01-08 15:19:49.000000 five-factor-e-1.8.0/test/test_model.py
--rw-r--r--   0 edmc      (1000) edmc      (1000)    15635 2022-11-18 15:15:42.000000 five-factor-e-1.8.0/test/test_norm.py
--rw-r--r--   0 edmc      (1000) edmc      (1000)     6278 2022-11-18 15:15:53.000000 five-factor-e-1.8.0/test/test_reverse.py
--rw-r--r--   0 edmc      (1000) edmc      (1000)    16279 2022-11-27 18:53:40.000000 five-factor-e-1.8.0/test/test_utility.py
+drwxr-xr-x   0 edmc      (1000) edmc      (1000)        0 2023-04-01 20:11:32.957848 five-factor-e-1.9.0/
+-rw-r--r--   0 edmc      (1000) edmc      (1000)     1069 2023-04-01 20:09:46.000000 five-factor-e-1.9.0/LICENSE
+-rw-r--r--   0 edmc      (1000) edmc      (1000)    11460 2023-04-01 20:11:32.956848 five-factor-e-1.9.0/PKG-INFO
+-rw-r--r--   0 edmc      (1000) edmc      (1000)    10695 2023-04-01 20:09:46.000000 five-factor-e-1.9.0/README.md
+drwxr-xr-x   0 edmc      (1000) edmc      (1000)        0 2023-04-01 20:11:32.947848 five-factor-e-1.9.0/five_factor_e.egg-info/
+-rw-r--r--   0 edmc      (1000) edmc      (1000)    11460 2023-04-01 20:11:32.000000 five-factor-e-1.9.0/five_factor_e.egg-info/PKG-INFO
+-rw-r--r--   0 edmc      (1000) edmc      (1000)      512 2023-04-01 20:11:32.000000 five-factor-e-1.9.0/five_factor_e.egg-info/SOURCES.txt
+-rw-r--r--   0 edmc      (1000) edmc      (1000)        1 2023-04-01 20:11:32.000000 five-factor-e-1.9.0/five_factor_e.egg-info/dependency_links.txt
+-rw-r--r--   0 edmc      (1000) edmc      (1000)       51 2023-04-01 20:11:32.000000 five-factor-e-1.9.0/five_factor_e.egg-info/entry_points.txt
+-rw-r--r--   0 edmc      (1000) edmc      (1000)       16 2023-04-01 20:11:32.000000 five-factor-e-1.9.0/five_factor_e.egg-info/requires.txt
+-rw-r--r--   0 edmc      (1000) edmc      (1000)        8 2023-04-01 20:11:32.000000 five-factor-e-1.9.0/five_factor_e.egg-info/top_level.txt
+drwxr-xr-x   0 edmc      (1000) edmc      (1000)        0 2023-04-01 20:11:32.954848 five-factor-e-1.9.0/ipipneo/
+-rw-r--r--   0 edmc      (1000) edmc      (1000)      127 2023-04-01 20:09:46.000000 five-factor-e-1.9.0/ipipneo/__init__.py
+-rw-r--r--   0 edmc      (1000) edmc      (1000)     7154 2023-04-01 20:11:12.000000 five-factor-e-1.9.0/ipipneo/facet.py
+-rw-r--r--   0 edmc      (1000) edmc      (1000)     5659 2023-04-01 20:11:12.000000 five-factor-e-1.9.0/ipipneo/ipipneo.py
+-rw-r--r--   0 edmc      (1000) edmc      (1000)     2267 2023-04-01 20:09:46.000000 five-factor-e-1.9.0/ipipneo/model.py
+-rw-r--r--   0 edmc      (1000) edmc      (1000)    32970 2023-04-01 20:09:46.000000 five-factor-e-1.9.0/ipipneo/norm.py
+-rw-r--r--   0 edmc      (1000) edmc      (1000)    13135 2023-04-01 20:09:46.000000 five-factor-e-1.9.0/ipipneo/quiz.py
+-rw-r--r--   0 edmc      (1000) edmc      (1000)     7557 2023-04-01 20:09:46.000000 five-factor-e-1.9.0/ipipneo/reverse.py
+-rw-r--r--   0 edmc      (1000) edmc      (1000)     6044 2023-04-01 20:11:12.000000 five-factor-e-1.9.0/ipipneo/utility.py
+-rw-r--r--   0 edmc      (1000) edmc      (1000)       38 2023-04-01 20:11:32.957848 five-factor-e-1.9.0/setup.cfg
+-rw-r--r--   0 edmc      (1000) edmc      (1000)     1675 2023-04-01 20:09:46.000000 five-factor-e-1.9.0/setup.py
+drwxr-xr-x   0 edmc      (1000) edmc      (1000)        0 2023-04-01 20:11:32.956848 five-factor-e-1.9.0/test/
+-rw-r--r--   0 edmc      (1000) edmc      (1000)    42496 2023-04-01 20:09:46.000000 five-factor-e-1.9.0/test/test_facet.py
+-rw-r--r--   0 edmc      (1000) edmc      (1000)    16273 2023-04-01 20:09:46.000000 five-factor-e-1.9.0/test/test_ipipneo.py
+-rw-r--r--   0 edmc      (1000) edmc      (1000)     6667 2023-04-01 20:11:13.000000 five-factor-e-1.9.0/test/test_model.py
+-rw-r--r--   0 edmc      (1000) edmc      (1000)    15635 2023-04-01 18:02:30.000000 five-factor-e-1.9.0/test/test_norm.py
+-rw-r--r--   0 edmc      (1000) edmc      (1000)     6278 2023-04-01 20:11:13.000000 five-factor-e-1.9.0/test/test_reverse.py
+-rw-r--r--   0 edmc      (1000) edmc      (1000)    16635 2023-04-01 20:11:13.000000 five-factor-e-1.9.0/test/test_utility.py
```

### Comparing `five-factor-e-1.8.0/PKG-INFO` & `five-factor-e-1.9.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 Metadata-Version: 2.1
 Name: five-factor-e
-Version: 1.8.0
+Version: 1.9.0
 Summary: Big 5 IPIP-NEO Personality Traits
-Author: Ederson Corbari, Neural7
-Author-email: <e@neural7.com>
-Keywords: IPIP-NEO,Big-5,Big-Five,Five-Factor,Personality,Assessment,Psychometrics,Personality-Insights,People-Analytics,Python
+Author: Ederson Corbari, ReWire5
+Author-email: <e@rewire5.com>
+Keywords: IPIP,IPIP-NEO,Big-5,Big-Five,Five-Factor,Personality,Assessment,Psychometrics,Personality-Insights,People-Analytics,Python
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 Provides-Extra: quiz
 License-File: LICENSE
 
 
-<img src="https://raw.githubusercontent.com/neural7/five-factor-e/main/doc/neural7.png" align="right" width="80" height="70"/>
+<img src="https://raw.githubusercontent.com/rewire5-io/five-factor-e/main/doc/rewire5.png" align="right" width="80" height="70"/>
 
 # Five Factor E 🌊
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/five-factor-e.svg)](https://pypi.org/project/five-factor-e/)
 ![python 3.7 | 3.8 | 3.9 | 3.10 | 3.11][python_version]
 [![PyPi Downloads](https://pepy.tech/badge/five-factor-e)](https://pepy.tech/project/five-factor-e)
 [![Code style: Black](https://img.shields.io/badge/code%20style-Black-000000.svg)](https://github.com/psf/black)
 
 [python_version]: https://img.shields.io/static/v1.svg?label=python&message=3.7%20|%203.8%20|%203.9%20|%203.10%20|%203.11%20&color=blue
 
 <p align="center">
-  <img src="https://raw.githubusercontent.com/neural7/five-factor-e/main/doc/big-five-neural7.png" alt="Representation of the Big Five"/>
+  <img src="https://raw.githubusercontent.com/rewire5-io/five-factor-e/main/doc/big-five-rewire5.png" alt="Representation of the Big Five"/>
 </p>
 
 This project assesses a person's 🗣 personality based on an inventory of questions. The project uses the **Big Five** theory using the [IPIP-NEO-300](http://www.personal.psu.edu/~j5j/IPIP/ipipneo300.htm) model created by **Lewis R. Goldberg** and [IPIP-NEO-120](http://www.personal.psu.edu/~j5j/IPIP/ipipneo120.htm) the shorter version developed by Professor **Dr. John A. Johnson**, this is a free representation of the [NEO PI-R™](https://en.wikipedia.org/wiki/Revised_NEO_Personality_Inventory).
 
 👉 *"The IPIP-NEO is not identical to the original NEO PI-R, but in my opinion it is close enough to serve as a good substitute. More and more people are beginning to use it in published research, so its acceptance is growing."* - Dr. Johnson
 
 The main idea of the project is to facilitate the use of **Python** developers who want to use **IPIP-NEO** in their projects. *The project is also done in pure Python, it doesn't have any dependencies on other libraries*.
 
 👉 *"That is wonderful, ...! Thank you for developing the Python version of the IPIP-NEO and making it publicly available. It looks like a great resource."* - Dr. Johnson
 
-Note 🚩: *The project is based on the work of **Dhiru Kholia**, and is an adaptation of [Neural7](https://github.com/neural7) for a version that can be reused in other projects of the company.*
+Note 🚩: *The project is based on the work of **Dhiru Kholia**, and is an adaptation of [ReWire5](https://github.com/rewire5-io) for a version that can be reused in other projects of the company.*
 
 ### Synopsis 🌐
 
 A little theory, The Big Five or Five Factor is made up of **5** great human personalities also known as the 🌊 **O.C.E.A.N**. Are they:
 
  * **O**penness
  * **C**onscientiousness
@@ -76,35 +76,35 @@
 
 Note 🚩: Some answers have the order of the [score reversed](https://ipip.ori.org/newScoringInstructions.htm), the algorithm treats the questions with the score inverted by (*question_id*).
 
 ### Releases 🎈
 
 News about each version please look here:
 
-  * [Releases](https://github.com/neural7/five-factor-e/blob/main/RELEASES.md)
+  * [Releases](https://github.com/rewire5-io/five-factor-e/blob/main/RELEASES.md)
 
 ### Installation 🚀
 
 From **PyPI**:
 
 ```shell
 $ python3 -m pip install --upgrade five-factor-e
 ```
 
 From source:
 
 ```shell
-$ git clone https://github.com/neural7/five-factor-e.git
+$ git clone https://github.com/rewire5-io/five-factor-e.git
 $ cd five-factor-e
 $ python3 -m pip install .
 ```
 
 ### How to use 🔥
 
-The construtor requires the questions model, whether it is the **300** model or short model with **120** questions. It also has the version to do simulations with the questions that are [reversed](https://ipip.ori.org/newScoringInstructions.htm). For this, you must turn the **test** variable from false to true, for more details on reverse scoring tests see section [Experiments with reverse scoring questions](https://github.com/neural7/five-factor-e/blob/main/data/README.md).
+The construtor requires the questions model, whether it is the **300** model or short model with **120** questions. It also has the version to do simulations with the questions that are [reversed](https://ipip.ori.org/newScoringInstructions.htm). For this, you must turn the **test** variable from false to true, for more details on reverse scoring tests see section [Experiments with reverse scoring questions](https://github.com/rewire5-io/five-factor-e/blob/main/data/README.md).
 
 | Parameters    | Type      | Description                                                       |
 | ------------- | --------- | ----------------------------------------------------------------- |
 | question      | int       | Question type, 120 or 300.                                        |
 | test          | boolean   | Used to simulate reverse scoring questions, only used for studies.|
 
 Example:
@@ -119,31 +119,31 @@
 
 ```python
 from ipipneo import IpipNeo
 
 ipip = IpipNeo(question=300)
 ```
 
-The answers must be in a *standardized json*, you can insert this template in the [data](https://github.com/neural7/five-factor-e/blob/main/data/IPIP-NEO/120/answers.json) folder of the project. This dictionary contains random answers, used for testing purposes only. As an example, you can load the file with the **120** test responses:
+The answers must be in a *standardized json*, you can insert this template in the [data](https://github.com/rewire5-io/five-factor-e/blob/main/data/IPIP-NEO/120/answers.json) folder of the project. This dictionary contains random answers, used for testing purposes only. As an example, you can load the file with the **120** test responses:
 
 ```python
 import json, urllib.request
 
-data = urllib.request.urlopen("https://raw.githubusercontent.com/neural7"\
+data = urllib.request.urlopen("https://raw.githubusercontent.com/rewire5-io"\
    "/five-factor-e/main/data/IPIP-NEO/120/answers.json").read()
 
 answers120 = json.loads(data)
 ```
 
 For the long inventory version with **300** items.
 
 ```python
 import json, urllib.request
 
-data = urllib.request.urlopen("https://raw.githubusercontent.com/neural7"\
+data = urllib.request.urlopen("https://raw.githubusercontent.com/rewire5-io"\
    "/five-factor-e/main/data/IPIP-NEO/300/answers.json").read()
 
 answers300 = json.loads(data)
 ```
 
 #### Compute the data 🏁
 
@@ -217,15 +217,15 @@
             ]
          }
       }
    ]
 }
 ```
 
-Example of the complete output check here: [Big 5️⃣ Output](https://github.com/neural7/five-factor-e/blob/main/data/IPIP-NEO/120/result.json)
+Example of the complete output check here: [Big 5️⃣ Output](https://github.com/rewire5-io/five-factor-e/blob/main/data/IPIP-NEO/120/result.json)
 
 ### Tests 🏗
 
 For the tests it is necessary to download the repository. To run the unit tests use the command below:
 
 ```shell
 $ ./run-test
@@ -244,22 +244,22 @@
 ```shell
 $ pip install five-factor-e[quiz]
 ```
 
 Example output with graphics:
 
 <p align="center">
-  <img src="https://raw.githubusercontent.com/neural7/five-factor-e/feature/v1.5.0/doc/sample-light-1.png" alt="Big Five Results" border="1"/>
+  <img src="https://raw.githubusercontent.com/rewire5-io/five-factor-e/feature/v1.5.0/doc/sample-light-1.png" alt="Big Five Results" border="1"/>
 </p>
 
 *The complete result is saved in the run folder in json format*.
 
 ### About data 📊
 
-Inside the data [data](https://github.com/neural7/five-factor-e/blob/main/data/) directory, there are examples of questions and answers. The most important is the response data entry which must follow the pattern of this [file](https://github.com/neural7/five-factor-e/blob/main/data/IPIP-NEO/120/answers.json). Example:
+Inside the data [data](https://github.com/rewire5-io/five-factor-e/blob/main/data/) directory, there are examples of questions and answers. The most important is the response data entry which must follow the pattern of this [file](https://github.com/rewire5-io/five-factor-e/blob/main/data/IPIP-NEO/120/answers.json). Example:
 
 ```json
 {
    "answers":[
       {
          "id_question":50,
          "id_select":5
@@ -268,15 +268,15 @@
          "id_question":51,
          "id_select":2
       }
    ]
 }
 ```
 
-The id question field refers to the question in this [file](https://github.com/neural7/five-factor-e/blob/main/data/IPIP-NEO/120/questions.json).
+The id question field refers to the question in this [file](https://github.com/rewire5-io/five-factor-e/blob/main/data/IPIP-NEO/120/questions.json).
 Obviously if you want you can change the translation of the question, *but don't change the ID of the question*.
 
 Note 🚩:
   * *The order of answers does not affect the result;*
   * *You can rephrase the questions to your need, but don't change the question IDs, they are used by the algorithm.*
 
 ### Credits 🏆
@@ -296,8 +296,8 @@
   * http://www.personal.psu.edu/faculty/j/5/j5j/
   * https://ipip.ori.org/
   * https://osf.io/tbmh5/
   * https://github.com/kholia/IPIP-NEO-PI
 
 ### Authors 👨‍💻
 
-  * [Ederson Corbari](mailto:e@neural7.io) 👽
+  * [Ederson Corbari](mailto:e@rewire5.io) 👽
```

### Comparing `five-factor-e-1.8.0/README.md` & `five-factor-e-1.9.0/five_factor_e.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,52 @@
-<img src="https://raw.githubusercontent.com/neural7/five-factor-e/main/doc/neural7.png" align="right" width="80" height="70"/>
+Metadata-Version: 2.1
+Name: five-factor-e
+Version: 1.9.0
+Summary: Big 5 IPIP-NEO Personality Traits
+Author: Ederson Corbari, ReWire5
+Author-email: <e@rewire5.com>
+Keywords: IPIP,IPIP-NEO,Big-5,Big-Five,Five-Factor,Personality,Assessment,Psychometrics,Personality-Insights,People-Analytics,Python
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Education
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.5
+Description-Content-Type: text/markdown
+Provides-Extra: quiz
+License-File: LICENSE
+
+
+<img src="https://raw.githubusercontent.com/rewire5-io/five-factor-e/main/doc/rewire5.png" align="right" width="80" height="70"/>
 
 # Five Factor E 🌊
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/five-factor-e.svg)](https://pypi.org/project/five-factor-e/)
 ![python 3.7 | 3.8 | 3.9 | 3.10 | 3.11][python_version]
 [![PyPi Downloads](https://pepy.tech/badge/five-factor-e)](https://pepy.tech/project/five-factor-e)
 [![Code style: Black](https://img.shields.io/badge/code%20style-Black-000000.svg)](https://github.com/psf/black)
 
 [python_version]: https://img.shields.io/static/v1.svg?label=python&message=3.7%20|%203.8%20|%203.9%20|%203.10%20|%203.11%20&color=blue
 
 <p align="center">
-  <img src="https://raw.githubusercontent.com/neural7/five-factor-e/main/doc/big-five-neural7.png" alt="Representation of the Big Five"/>
+  <img src="https://raw.githubusercontent.com/rewire5-io/five-factor-e/main/doc/big-five-rewire5.png" alt="Representation of the Big Five"/>
 </p>
 
 This project assesses a person's 🗣 personality based on an inventory of questions. The project uses the **Big Five** theory using the [IPIP-NEO-300](http://www.personal.psu.edu/~j5j/IPIP/ipipneo300.htm) model created by **Lewis R. Goldberg** and [IPIP-NEO-120](http://www.personal.psu.edu/~j5j/IPIP/ipipneo120.htm) the shorter version developed by Professor **Dr. John A. Johnson**, this is a free representation of the [NEO PI-R™](https://en.wikipedia.org/wiki/Revised_NEO_Personality_Inventory).
 
 👉 *"The IPIP-NEO is not identical to the original NEO PI-R, but in my opinion it is close enough to serve as a good substitute. More and more people are beginning to use it in published research, so its acceptance is growing."* - Dr. Johnson
 
 The main idea of the project is to facilitate the use of **Python** developers who want to use **IPIP-NEO** in their projects. *The project is also done in pure Python, it doesn't have any dependencies on other libraries*.
 
 👉 *"That is wonderful, ...! Thank you for developing the Python version of the IPIP-NEO and making it publicly available. It looks like a great resource."* - Dr. Johnson
 
-Note 🚩: *The project is based on the work of **Dhiru Kholia**, and is an adaptation of [Neural7](https://github.com/neural7) for a version that can be reused in other projects of the company.*
+Note 🚩: *The project is based on the work of **Dhiru Kholia**, and is an adaptation of [ReWire5](https://github.com/rewire5-io) for a version that can be reused in other projects of the company.*
 
 ### Synopsis 🌐
 
 A little theory, The Big Five or Five Factor is made up of **5** great human personalities also known as the 🌊 **O.C.E.A.N**. Are they:
 
  * **O**penness
  * **C**onscientiousness
@@ -55,35 +76,35 @@
 
 Note 🚩: Some answers have the order of the [score reversed](https://ipip.ori.org/newScoringInstructions.htm), the algorithm treats the questions with the score inverted by (*question_id*).
 
 ### Releases 🎈
 
 News about each version please look here:
 
-  * [Releases](https://github.com/neural7/five-factor-e/blob/main/RELEASES.md)
+  * [Releases](https://github.com/rewire5-io/five-factor-e/blob/main/RELEASES.md)
 
 ### Installation 🚀
 
 From **PyPI**:
 
 ```shell
 $ python3 -m pip install --upgrade five-factor-e
 ```
 
 From source:
 
 ```shell
-$ git clone https://github.com/neural7/five-factor-e.git
+$ git clone https://github.com/rewire5-io/five-factor-e.git
 $ cd five-factor-e
 $ python3 -m pip install .
 ```
 
 ### How to use 🔥
 
-The construtor requires the questions model, whether it is the **300** model or short model with **120** questions. It also has the version to do simulations with the questions that are [reversed](https://ipip.ori.org/newScoringInstructions.htm). For this, you must turn the **test** variable from false to true, for more details on reverse scoring tests see section [Experiments with reverse scoring questions](https://github.com/neural7/five-factor-e/blob/main/data/README.md).
+The construtor requires the questions model, whether it is the **300** model or short model with **120** questions. It also has the version to do simulations with the questions that are [reversed](https://ipip.ori.org/newScoringInstructions.htm). For this, you must turn the **test** variable from false to true, for more details on reverse scoring tests see section [Experiments with reverse scoring questions](https://github.com/rewire5-io/five-factor-e/blob/main/data/README.md).
 
 | Parameters    | Type      | Description                                                       |
 | ------------- | --------- | ----------------------------------------------------------------- |
 | question      | int       | Question type, 120 or 300.                                        |
 | test          | boolean   | Used to simulate reverse scoring questions, only used for studies.|
 
 Example:
@@ -98,31 +119,31 @@
 
 ```python
 from ipipneo import IpipNeo
 
 ipip = IpipNeo(question=300)
 ```
 
-The answers must be in a *standardized json*, you can insert this template in the [data](https://github.com/neural7/five-factor-e/blob/main/data/IPIP-NEO/120/answers.json) folder of the project. This dictionary contains random answers, used for testing purposes only. As an example, you can load the file with the **120** test responses:
+The answers must be in a *standardized json*, you can insert this template in the [data](https://github.com/rewire5-io/five-factor-e/blob/main/data/IPIP-NEO/120/answers.json) folder of the project. This dictionary contains random answers, used for testing purposes only. As an example, you can load the file with the **120** test responses:
 
 ```python
 import json, urllib.request
 
-data = urllib.request.urlopen("https://raw.githubusercontent.com/neural7"\
+data = urllib.request.urlopen("https://raw.githubusercontent.com/rewire5-io"\
    "/five-factor-e/main/data/IPIP-NEO/120/answers.json").read()
 
 answers120 = json.loads(data)
 ```
 
 For the long inventory version with **300** items.
 
 ```python
 import json, urllib.request
 
-data = urllib.request.urlopen("https://raw.githubusercontent.com/neural7"\
+data = urllib.request.urlopen("https://raw.githubusercontent.com/rewire5-io"\
    "/five-factor-e/main/data/IPIP-NEO/300/answers.json").read()
 
 answers300 = json.loads(data)
 ```
 
 #### Compute the data 🏁
 
@@ -196,15 +217,15 @@
             ]
          }
       }
    ]
 }
 ```
 
-Example of the complete output check here: [Big 5️⃣ Output](https://github.com/neural7/five-factor-e/blob/main/data/IPIP-NEO/120/result.json)
+Example of the complete output check here: [Big 5️⃣ Output](https://github.com/rewire5-io/five-factor-e/blob/main/data/IPIP-NEO/120/result.json)
 
 ### Tests 🏗
 
 For the tests it is necessary to download the repository. To run the unit tests use the command below:
 
 ```shell
 $ ./run-test
@@ -223,22 +244,22 @@
 ```shell
 $ pip install five-factor-e[quiz]
 ```
 
 Example output with graphics:
 
 <p align="center">
-  <img src="https://raw.githubusercontent.com/neural7/five-factor-e/feature/v1.5.0/doc/sample-light-1.png" alt="Big Five Results" border="1"/>
+  <img src="https://raw.githubusercontent.com/rewire5-io/five-factor-e/feature/v1.5.0/doc/sample-light-1.png" alt="Big Five Results" border="1"/>
 </p>
 
 *The complete result is saved in the run folder in json format*.
 
 ### About data 📊
 
-Inside the data [data](https://github.com/neural7/five-factor-e/blob/main/data/) directory, there are examples of questions and answers. The most important is the response data entry which must follow the pattern of this [file](https://github.com/neural7/five-factor-e/blob/main/data/IPIP-NEO/120/answers.json). Example:
+Inside the data [data](https://github.com/rewire5-io/five-factor-e/blob/main/data/) directory, there are examples of questions and answers. The most important is the response data entry which must follow the pattern of this [file](https://github.com/rewire5-io/five-factor-e/blob/main/data/IPIP-NEO/120/answers.json). Example:
 
 ```json
 {
    "answers":[
       {
          "id_question":50,
          "id_select":5
@@ -247,15 +268,15 @@
          "id_question":51,
          "id_select":2
       }
    ]
 }
 ```
 
-The id question field refers to the question in this [file](https://github.com/neural7/five-factor-e/blob/main/data/IPIP-NEO/120/questions.json).
+The id question field refers to the question in this [file](https://github.com/rewire5-io/five-factor-e/blob/main/data/IPIP-NEO/120/questions.json).
 Obviously if you want you can change the translation of the question, *but don't change the ID of the question*.
 
 Note 🚩:
   * *The order of answers does not affect the result;*
   * *You can rephrase the questions to your need, but don't change the question IDs, they are used by the algorithm.*
 
 ### Credits 🏆
@@ -275,8 +296,8 @@
   * http://www.personal.psu.edu/faculty/j/5/j5j/
   * https://ipip.ori.org/
   * https://osf.io/tbmh5/
   * https://github.com/kholia/IPIP-NEO-PI
 
 ### Authors 👨‍💻
 
-  * [Ederson Corbari](mailto:e@neural7.io) 👽
+  * [Ederson Corbari](mailto:e@rewire5.io) 👽
```

### Comparing `five-factor-e-1.8.0/five_factor_e.egg-info/PKG-INFO` & `five-factor-e-1.9.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,31 @@
-Metadata-Version: 2.1
-Name: five-factor-e
-Version: 1.8.0
-Summary: Big 5 IPIP-NEO Personality Traits
-Author: Ederson Corbari, Neural7
-Author-email: <e@neural7.com>
-Keywords: IPIP-NEO,Big-5,Big-Five,Five-Factor,Personality,Assessment,Psychometrics,Personality-Insights,People-Analytics,Python
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Education
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-Provides-Extra: quiz
-License-File: LICENSE
-
-
-<img src="https://raw.githubusercontent.com/neural7/five-factor-e/main/doc/neural7.png" align="right" width="80" height="70"/>
+<img src="https://raw.githubusercontent.com/rewire5-io/five-factor-e/main/doc/rewire5.png" align="right" width="80" height="70"/>
 
 # Five Factor E 🌊
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/five-factor-e.svg)](https://pypi.org/project/five-factor-e/)
 ![python 3.7 | 3.8 | 3.9 | 3.10 | 3.11][python_version]
 [![PyPi Downloads](https://pepy.tech/badge/five-factor-e)](https://pepy.tech/project/five-factor-e)
 [![Code style: Black](https://img.shields.io/badge/code%20style-Black-000000.svg)](https://github.com/psf/black)
 
 [python_version]: https://img.shields.io/static/v1.svg?label=python&message=3.7%20|%203.8%20|%203.9%20|%203.10%20|%203.11%20&color=blue
 
 <p align="center">
-  <img src="https://raw.githubusercontent.com/neural7/five-factor-e/main/doc/big-five-neural7.png" alt="Representation of the Big Five"/>
+  <img src="https://raw.githubusercontent.com/rewire5-io/five-factor-e/main/doc/big-five-rewire5.png" alt="Representation of the Big Five"/>
 </p>
 
 This project assesses a person's 🗣 personality based on an inventory of questions. The project uses the **Big Five** theory using the [IPIP-NEO-300](http://www.personal.psu.edu/~j5j/IPIP/ipipneo300.htm) model created by **Lewis R. Goldberg** and [IPIP-NEO-120](http://www.personal.psu.edu/~j5j/IPIP/ipipneo120.htm) the shorter version developed by Professor **Dr. John A. Johnson**, this is a free representation of the [NEO PI-R™](https://en.wikipedia.org/wiki/Revised_NEO_Personality_Inventory).
 
 👉 *"The IPIP-NEO is not identical to the original NEO PI-R, but in my opinion it is close enough to serve as a good substitute. More and more people are beginning to use it in published research, so its acceptance is growing."* - Dr. Johnson
 
 The main idea of the project is to facilitate the use of **Python** developers who want to use **IPIP-NEO** in their projects. *The project is also done in pure Python, it doesn't have any dependencies on other libraries*.
 
 👉 *"That is wonderful, ...! Thank you for developing the Python version of the IPIP-NEO and making it publicly available. It looks like a great resource."* - Dr. Johnson
 
-Note 🚩: *The project is based on the work of **Dhiru Kholia**, and is an adaptation of [Neural7](https://github.com/neural7) for a version that can be reused in other projects of the company.*
+Note 🚩: *The project is based on the work of **Dhiru Kholia**, and is an adaptation of [ReWire5](https://github.com/rewire5-io) for a version that can be reused in other projects of the company.*
 
 ### Synopsis 🌐
 
 A little theory, The Big Five or Five Factor is made up of **5** great human personalities also known as the 🌊 **O.C.E.A.N**. Are they:
 
  * **O**penness
  * **C**onscientiousness
@@ -76,35 +55,35 @@
 
 Note 🚩: Some answers have the order of the [score reversed](https://ipip.ori.org/newScoringInstructions.htm), the algorithm treats the questions with the score inverted by (*question_id*).
 
 ### Releases 🎈
 
 News about each version please look here:
 
-  * [Releases](https://github.com/neural7/five-factor-e/blob/main/RELEASES.md)
+  * [Releases](https://github.com/rewire5-io/five-factor-e/blob/main/RELEASES.md)
 
 ### Installation 🚀
 
 From **PyPI**:
 
 ```shell
 $ python3 -m pip install --upgrade five-factor-e
 ```
 
 From source:
 
 ```shell
-$ git clone https://github.com/neural7/five-factor-e.git
+$ git clone https://github.com/rewire5-io/five-factor-e.git
 $ cd five-factor-e
 $ python3 -m pip install .
 ```
 
 ### How to use 🔥
 
-The construtor requires the questions model, whether it is the **300** model or short model with **120** questions. It also has the version to do simulations with the questions that are [reversed](https://ipip.ori.org/newScoringInstructions.htm). For this, you must turn the **test** variable from false to true, for more details on reverse scoring tests see section [Experiments with reverse scoring questions](https://github.com/neural7/five-factor-e/blob/main/data/README.md).
+The construtor requires the questions model, whether it is the **300** model or short model with **120** questions. It also has the version to do simulations with the questions that are [reversed](https://ipip.ori.org/newScoringInstructions.htm). For this, you must turn the **test** variable from false to true, for more details on reverse scoring tests see section [Experiments with reverse scoring questions](https://github.com/rewire5-io/five-factor-e/blob/main/data/README.md).
 
 | Parameters    | Type      | Description                                                       |
 | ------------- | --------- | ----------------------------------------------------------------- |
 | question      | int       | Question type, 120 or 300.                                        |
 | test          | boolean   | Used to simulate reverse scoring questions, only used for studies.|
 
 Example:
@@ -119,31 +98,31 @@
 
 ```python
 from ipipneo import IpipNeo
 
 ipip = IpipNeo(question=300)
 ```
 
-The answers must be in a *standardized json*, you can insert this template in the [data](https://github.com/neural7/five-factor-e/blob/main/data/IPIP-NEO/120/answers.json) folder of the project. This dictionary contains random answers, used for testing purposes only. As an example, you can load the file with the **120** test responses:
+The answers must be in a *standardized json*, you can insert this template in the [data](https://github.com/rewire5-io/five-factor-e/blob/main/data/IPIP-NEO/120/answers.json) folder of the project. This dictionary contains random answers, used for testing purposes only. As an example, you can load the file with the **120** test responses:
 
 ```python
 import json, urllib.request
 
-data = urllib.request.urlopen("https://raw.githubusercontent.com/neural7"\
+data = urllib.request.urlopen("https://raw.githubusercontent.com/rewire5-io"\
    "/five-factor-e/main/data/IPIP-NEO/120/answers.json").read()
 
 answers120 = json.loads(data)
 ```
 
 For the long inventory version with **300** items.
 
 ```python
 import json, urllib.request
 
-data = urllib.request.urlopen("https://raw.githubusercontent.com/neural7"\
+data = urllib.request.urlopen("https://raw.githubusercontent.com/rewire5-io"\
    "/five-factor-e/main/data/IPIP-NEO/300/answers.json").read()
 
 answers300 = json.loads(data)
 ```
 
 #### Compute the data 🏁
 
@@ -217,15 +196,15 @@
             ]
          }
       }
    ]
 }
 ```
 
-Example of the complete output check here: [Big 5️⃣ Output](https://github.com/neural7/five-factor-e/blob/main/data/IPIP-NEO/120/result.json)
+Example of the complete output check here: [Big 5️⃣ Output](https://github.com/rewire5-io/five-factor-e/blob/main/data/IPIP-NEO/120/result.json)
 
 ### Tests 🏗
 
 For the tests it is necessary to download the repository. To run the unit tests use the command below:
 
 ```shell
 $ ./run-test
@@ -244,22 +223,22 @@
 ```shell
 $ pip install five-factor-e[quiz]
 ```
 
 Example output with graphics:
 
 <p align="center">
-  <img src="https://raw.githubusercontent.com/neural7/five-factor-e/feature/v1.5.0/doc/sample-light-1.png" alt="Big Five Results" border="1"/>
+  <img src="https://raw.githubusercontent.com/rewire5-io/five-factor-e/feature/v1.5.0/doc/sample-light-1.png" alt="Big Five Results" border="1"/>
 </p>
 
 *The complete result is saved in the run folder in json format*.
 
 ### About data 📊
 
-Inside the data [data](https://github.com/neural7/five-factor-e/blob/main/data/) directory, there are examples of questions and answers. The most important is the response data entry which must follow the pattern of this [file](https://github.com/neural7/five-factor-e/blob/main/data/IPIP-NEO/120/answers.json). Example:
+Inside the data [data](https://github.com/rewire5-io/five-factor-e/blob/main/data/) directory, there are examples of questions and answers. The most important is the response data entry which must follow the pattern of this [file](https://github.com/rewire5-io/five-factor-e/blob/main/data/IPIP-NEO/120/answers.json). Example:
 
 ```json
 {
    "answers":[
       {
          "id_question":50,
          "id_select":5
@@ -268,15 +247,15 @@
          "id_question":51,
          "id_select":2
       }
    ]
 }
 ```
 
-The id question field refers to the question in this [file](https://github.com/neural7/five-factor-e/blob/main/data/IPIP-NEO/120/questions.json).
+The id question field refers to the question in this [file](https://github.com/rewire5-io/five-factor-e/blob/main/data/IPIP-NEO/120/questions.json).
 Obviously if you want you can change the translation of the question, *but don't change the ID of the question*.
 
 Note 🚩:
   * *The order of answers does not affect the result;*
   * *You can rephrase the questions to your need, but don't change the question IDs, they are used by the algorithm.*
 
 ### Credits 🏆
@@ -296,8 +275,8 @@
   * http://www.personal.psu.edu/faculty/j/5/j5j/
   * https://ipip.ori.org/
   * https://osf.io/tbmh5/
   * https://github.com/kholia/IPIP-NEO-PI
 
 ### Authors 👨‍💻
 
-  * [Ederson Corbari](mailto:e@neural7.io) 👽
+  * [Ederson Corbari](mailto:e@rewire5.io) 👽
```

### Comparing `five-factor-e-1.8.0/five_factor_e.egg-info/SOURCES.txt` & `five-factor-e-1.9.0/five_factor_e.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `five-factor-e-1.8.0/ipipneo/facet.py` & `five-factor-e-1.9.0/ipipneo/facet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Creation and scoring of the facets that make up the Big-Five."""
 
 __author__ = "Ederson Corbari"
-__email__ = "e@neural7.io"
-__copyright__ = "Copyright Neural7 2022, Big 5 Personality Traits"
+__email__ = "e@rewire5.io"
+__copyright__ = "Copyright ReWire5 2022-2023, Big 5 Personality Traits"
 __credits__ = ["John A. Johnson", "Dhiru Kholia"]
 __license__ = "MIT"
-__version__ = "1.8.0"
+__version__ = "1.9.0"
 __status__ = "production"
 
 from enum import IntEnum
 
-from ipipneo.model import FacetLevel, FacetScale, NormCubic, NormScale, QuestionNumber
+from ipipneo.model import (FacetLevel, FacetScale, NormCubic, NormScale,
+                           QuestionNumber)
 from ipipneo.utility import big5_ocean_is_valid, create_big5_dict
 
 
 class Facet:
     """Creating and scoring facets and Big-Five."""
 
     def __init__(self, nquestion: IntEnum) -> None or BaseException:
@@ -109,19 +110,39 @@
         E = [0] * size
         O = [0] * size
         A = [0] * size
         C = [0] * size
 
         try:
             for i in range(1, 7):
-                N[i] = 50 + (10 * (b5.get("N")[i] - norm.get("ns")[i + 10]) / norm.get("ns")[i + 16])
-                E[i] = 50 + (10 * (b5.get("E")[i] - norm.get("ns")[i + 22]) / norm.get("ns")[i + 28])
-                O[i] = 50 + (10 * (b5.get("O")[i] - norm.get("ns")[i + 34]) / norm.get("ns")[i + 40])
-                A[i] = 50 + (10 * (b5.get("A")[i] - norm.get("ns")[i + 46]) / norm.get("ns")[i + 52])
-                C[i] = 50 + (10 * (b5.get("C")[i] - norm.get("ns")[i + 58]) / norm.get("ns")[i + 64])
+                N[i] = 50 + (
+                    10
+                    * (b5.get("N")[i] - norm.get("ns")[i + 10])
+                    / norm.get("ns")[i + 16]
+                )
+                E[i] = 50 + (
+                    10
+                    * (b5.get("E")[i] - norm.get("ns")[i + 22])
+                    / norm.get("ns")[i + 28]
+                )
+                O[i] = 50 + (
+                    10
+                    * (b5.get("O")[i] - norm.get("ns")[i + 34])
+                    / norm.get("ns")[i + 40]
+                )
+                A[i] = 50 + (
+                    10
+                    * (b5.get("A")[i] - norm.get("ns")[i + 46])
+                    / norm.get("ns")[i + 52]
+                )
+                C[i] = 50 + (
+                    10
+                    * (b5.get("C")[i] - norm.get("ns")[i + 58])
+                    / norm.get("ns")[i + 64]
+                )
         except IndexError as e:
             raise BaseException(f"The number of questions setting is wrong: {str(e)}")
 
         return {"O": O, "C": C, "E": E, "A": A, "N": N}
 
     def personality(self, size: int, big5: dict, traits: dict, label: str) -> dict:
         """
@@ -142,15 +163,18 @@
 
         try:
             for i in range(1, 7):
                 Y[i] = traits[i]
 
                 if traits[i] < FacetLevel.LOW.value:
                     Y[i] = "low"
-                if traits[i] >= FacetLevel.LOW.value and traits[i] <= FacetLevel.HIGH.value:
+                if (
+                    traits[i] >= FacetLevel.LOW.value
+                    and traits[i] <= FacetLevel.HIGH.value
+                ):
                     Y[i] = "average"
                 if traits[i] > FacetLevel.HIGH.value:
                     Y[i] = "high"
 
                 X[i] = (
                     NormCubic.CONST1.value
                     - (NormCubic.CONST2.value * traits[i])
```

### Comparing `five-factor-e-1.8.0/ipipneo/ipipneo.py` & `five-factor-e-1.9.0/ipipneo/ipipneo.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 """It does the calculations to generate the IPIP-NEO results based on the questions and answers."""
 
 __author__ = "Ederson Corbari"
-__email__ = "e@neural7.io"
-__copyright__ = "Copyright Neural7 2022, Big 5 Personality Traits"
+__email__ = "e@rewire5.io"
+__copyright__ = "Copyright ReWire5 2022-2023, Big 5 Personality Traits"
 __credits__ = ["John A. Johnson", "Dhiru Kholia"]
 __license__ = "MIT"
-__version__ = "1.8.0"
+__version__ = "1.9.0"
 __status__ = "production"
 
 import copy
 import uuid
 
 from ipipneo.facet import Facet
 from ipipneo.model import QuestionNumber
 from ipipneo.norm import Norm
-from ipipneo.reverse import ReverseScored120, ReverseScored300, ReverseScoredCustom
-from ipipneo.utility import (
-    organize_list_json,
-    raise_if_age_is_invalid,
-    raise_if_sex_is_invalid,
-)
+from ipipneo.reverse import (ReverseScored120, ReverseScored300,
+                             ReverseScoredCustom)
+from ipipneo.utility import (add_dict_footer, organize_list_json,
+                             raise_if_age_is_invalid, raise_if_sex_is_invalid)
 
 
 class IpipNeo(Facet):
     """Class that calculates IPIP-NEO answers."""
 
     def __init__(self, question: int, test: bool = False) -> None or BaseException:
         """
@@ -54,15 +52,17 @@
         """
         norm = Norm(sex=sex, age=age, nquestion=self._nquestion)
         assert isinstance(norm, dict), "norm must be a dict"
 
         normc = Norm.calc(domain=self.domain(score=score), norm=norm)
         assert isinstance(normc, dict), "normc must be a dict"
 
-        distrib = self.distrib(size=len(score), b5=self.b5create(score=score), norm=norm)
+        distrib = self.distrib(
+            size=len(score), b5=self.b5create(score=score), norm=norm
+        )
         assert isinstance(distrib, dict), "distrib must be a dict"
 
         normalize = Norm.normalize(normc=normc, percent=Norm.percent(normc=normc))
         assert isinstance(normalize, dict), "normalize must be a dict"
 
         N = self.personality(size=len(score), big5=normalize, traits=distrib, label="N")
         E = self.personality(size=len(score), big5=normalize, traits=distrib, label="E")
@@ -75,31 +75,31 @@
         assert isinstance(E, dict), "E must be a dict"
         assert isinstance(A, dict), "A must be a dict"
         assert isinstance(N, dict), "N must be a dict"
 
         return {
             "id": str(uuid.uuid4()),
             "theory": "Big 5 Personality Traits",
-            "model": "IPIP-NEO",
+            "model": "IPIP-NEO" if self._nquestion == 120 else "IPIP",
             "question": self._nquestion,
             "test": self._test,
-            "version": __version__,
             "person": {
                 "sex": sex,
                 "age": age,
                 "result": {
                     "personalities": [
                         {"openness": self.big_five_level(big5=O, label="O")},
                         {"conscientiousness": self.big_five_level(big5=C, label="C")},
                         {"extraversion": self.big_five_level(big5=E, label="E")},
                         {"agreeableness": self.big_five_level(big5=A, label="A")},
                         {"neuroticism": self.big_five_level(big5=N, label="N")},
                     ]
                 },
             },
+            **add_dict_footer(),
         }
 
     def compute(self, sex: str, age: int, answers: dict, compare: bool = False) -> dict:
         """
         Compute the answers and generate the data with the results.
 
         Args:
@@ -116,15 +116,17 @@
         assert isinstance(original, dict), "original must be a dict"
 
         reversed = {}
         if self._test:
             reversed = ReverseScoredCustom(answers=answers)
         else:
             reversed = (
-                ReverseScored120(answers=answers) if self._nquestion == 120 else ReverseScored300(answers=answers)
+                ReverseScored120(answers=answers)
+                if self._nquestion == 120
+                else ReverseScored300(answers=answers)
             )
         assert isinstance(reversed, dict), "reversed must be a dict"
 
         score = self.score(answers=organize_list_json(answers=reversed))
         assert isinstance(score, list), "score must be a list"
 
         result = self.evaluator(sex=sex, age=age, score=score)
```

### Comparing `five-factor-e-1.8.0/ipipneo/model.py` & `five-factor-e-1.9.0/ipipneo/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Auxiliary constants that are used in the library."""
 
 __author__ = "Ederson Corbari"
-__email__ = "e@neural7.io"
-__copyright__ = "Copyright Neural7 2022, Big 5 Personality Traits"
+__email__ = "e@rewire5.io"
+__copyright__ = "Copyright ReWire5 2022-2023, Big 5 Personality Traits"
 __credits__ = ["John A. Johnson", "Dhiru Kholia"]
 __license__ = "MIT"
-__version__ = "1.8.0"
+__version__ = "1.9.0"
 __status__ = "production"
 
 from enum import Enum, IntEnum
 
 
 class QuestionNumber(IntEnum):
     """Questionnaire types."""
```

### Comparing `five-factor-e-1.8.0/ipipneo/norm.py` & `five-factor-e-1.9.0/ipipneo/norm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """The standard with the rules of IPIP-NEO norms."""
 
 __author__ = "Ederson Corbari"
-__email__ = "e@neural7.io"
-__copyright__ = "Copyright Neural7 2022, Big 5 Personality Traits"
+__email__ = "e@rewire5.io"
+__copyright__ = "Copyright ReWire5 2022-2023, Big 5 Personality Traits"
 __credits__ = ["John A. Johnson", "Dhiru Kholia"]
 __license__ = "MIT"
-__version__ = "1.8.0"
+__version__ = "1.9.0"
 __status__ = "production"
 
 from enum import IntEnum
 
 from ipipneo.model import NormCubic, NormScale
 from ipipneo.utility import raise_if_age_is_invalid, raise_if_sex_is_invalid
```

### Comparing `five-factor-e-1.8.0/ipipneo/quiz.py` & `five-factor-e-1.9.0/ipipneo/quiz.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 """We use this for testing."""
 
 __author__ = "Ederson Corbari"
-__email__ = "e@neural7.io"
-__copyright__ = "Copyright Neural7 2022, Big 5 Personality Traits"
+__email__ = "e@rewire5.io"
+__copyright__ = "Copyright ReWire5 2022-2023, Big 5 Personality Traits"
 __credits__ = ["John A. Johnson", "Dhiru Kholia"]
 __license__ = "MIT"
-__version__ = "1.8.0"
+__version__ = "1.9.0"
 __status__ = "production"
 
 import json
 import random
 import sys
 import urllib.request
 from itertools import chain, repeat
 
 try:
     from ipipneo import IpipNeo
 except ModuleNotFoundError:
     sys.path.insert(0, "../")
     from ipipneo.ipipneo import IpipNeo
 
-URL_IPIP_QUESTIONS = "https://raw.githubusercontent.com/neural7/five-factor-e/main/data/IPIP-NEO"
+URL_IPIP_QUESTIONS = (
+    "https://raw.githubusercontent.com/rewire5-io/five-factor-e/main/data/IPIP-NEO"
+)
 
 
 def load_ipip_questions(lang: int, question: int) -> dict:
     """
     Load the IPIP-NEO questions.
 
     Args:
@@ -51,15 +53,18 @@
     """
     Filter only the question list.
 
     Args:
         - lang: The language ID.
         - question: Inventory model 120 or 300.
     """
-    return [x for x in load_ipip_questions(lang=lang, question=question).get("questions", [])]
+    return [
+        x
+        for x in load_ipip_questions(lang=lang, question=question).get("questions", [])
+    ]
 
 
 def get_select(lang: int, question: int) -> list:
     """
     Filter only the select list.
 
     Args:
@@ -109,15 +114,17 @@
                 ["\nOption: "],
                 repeat("Only numbers from 1 to 5 are accepted! Try again: "),
             ),
         )
         option = int(next(filter({"1", "2", "3", "4", "5"}.__contains__, replies)))
         answers.append({"id_question": q.get("id"), "id_select": option})
 
-    result = IpipNeo(question=inventory).compute(sex=sex, age=age, answers={"answers": answers}, compare=True)
+    result = IpipNeo(question=inventory).compute(
+        sex=sex, age=age, answers={"answers": answers}, compare=True
+    )
 
     object = json.dumps(result, indent=4)
     fname = f"result-{str(inventory)}-{result.get('id', 'id')}.json"
 
     with open(fname, "w") as f:
         f.write(object)
 
@@ -136,15 +143,19 @@
     try:
         import plotext as plt
 
         big5 = result.get("person").get("result").get("personalities")
 
         print(
             "\nInventory:",
-            str(result.get("model")) + "-" + str(result.get("question")) + " v" + str(result.get("version")),
+            str(result.get("model"))
+            + "-"
+            + str(result.get("question"))
+            + " v"
+            + str(result.get("version")),
         )
         print("Case:", result.get("id"))
         print("Gender:", result.get("person").get("sex"))
         print("Age:", result.get("person").get("age"), "\n")
 
         E = [
             "EXTRAVERSION",
@@ -160,15 +171,20 @@
             E,
             [
                 int(big5[2].get("extraversion").get("E")),
                 int(big5[2].get("extraversion").get("traits")[0].get("friendliness")),
                 int(big5[2].get("extraversion").get("traits")[1].get("gregariousness")),
                 int(big5[2].get("extraversion").get("traits")[2].get("assertiveness")),
                 int(big5[2].get("extraversion").get("traits")[3].get("activity_level")),
-                int(big5[2].get("extraversion").get("traits")[4].get("excitement_seeking")),
+                int(
+                    big5[2]
+                    .get("extraversion")
+                    .get("traits")[4]
+                    .get("excitement_seeking")
+                ),
                 int(big5[2].get("extraversion").get("traits")[5].get("cheerfulness")),
             ],
             width=100,
             title="Big-Five | Extraversion",
             color="orange",
         )
         plt.show()
@@ -214,20 +230,44 @@
             "Cautiousness",
         ]
 
         plt.simple_bar(
             C,
             [
                 int(big5[1].get("conscientiousness").get("C")),
-                int(big5[1].get("conscientiousness").get("traits")[0].get("self_efficacy")),
-                int(big5[1].get("conscientiousness").get("traits")[1].get("orderliness")),
-                int(big5[1].get("conscientiousness").get("traits")[2].get("dutifulness")),
-                int(big5[1].get("conscientiousness").get("traits")[3].get("achievement_striving")),
-                int(big5[1].get("conscientiousness").get("traits")[4].get("self_discipline")),
-                int(big5[1].get("conscientiousness").get("traits")[5].get("cautiousness")),
+                int(
+                    big5[1]
+                    .get("conscientiousness")
+                    .get("traits")[0]
+                    .get("self_efficacy")
+                ),
+                int(
+                    big5[1].get("conscientiousness").get("traits")[1].get("orderliness")
+                ),
+                int(
+                    big5[1].get("conscientiousness").get("traits")[2].get("dutifulness")
+                ),
+                int(
+                    big5[1]
+                    .get("conscientiousness")
+                    .get("traits")[3]
+                    .get("achievement_striving")
+                ),
+                int(
+                    big5[1]
+                    .get("conscientiousness")
+                    .get("traits")[4]
+                    .get("self_discipline")
+                ),
+                int(
+                    big5[1]
+                    .get("conscientiousness")
+                    .get("traits")[5]
+                    .get("cautiousness")
+                ),
             ],
             width=100,
             title="Big-Five | Consciousness",
             color="magenta",
         )
         plt.show()
 
@@ -246,15 +286,20 @@
         plt.simple_bar(
             N,
             [
                 int(big5[4].get("neuroticism").get("N")),
                 int(big5[4].get("neuroticism").get("traits")[0].get("anxiety")),
                 int(big5[4].get("neuroticism").get("traits")[1].get("anger")),
                 int(big5[4].get("neuroticism").get("traits")[2].get("depression")),
-                int(big5[4].get("neuroticism").get("traits")[3].get("self_consciousness")),
+                int(
+                    big5[4]
+                    .get("neuroticism")
+                    .get("traits")[3]
+                    .get("self_consciousness")
+                ),
                 int(big5[4].get("neuroticism").get("traits")[4].get("immoderation")),
                 int(big5[4].get("neuroticism").get("traits")[5].get("vulnerability")),
             ],
             width=100,
             title="Big-Five | Neuroticism",
             color="red",
         )
@@ -319,17 +364,21 @@
             repeat("Please, only 120 or 300 are valid! Try again: "),
         ),
     )
     inventory = int(next(filter({"120", "300"}.__contains__, replies)))
 
     print("\n====================================================================")
     if inventory == 120:
-        print("The following test contains 120 questions which is estimated to take you about 15 minutes to complete!")
+        print(
+            "The following test contains 120 questions which is estimated to take you about 15 minutes to complete!"
+        )
     elif inventory == 300:
-        print("The following test contains 300 questions which is estimated to take you about 35 minutes to complete!")
+        print(
+            "The following test contains 300 questions which is estimated to take you about 35 minutes to complete!"
+        )
 
     replies = map(
         input,
         chain(
             ["\n> What is your sex Male or Female? M / F: "],
             repeat("Please, only M or F are valid! Try again: "),
         ),
@@ -360,15 +409,17 @@
     elif inventory == 300:
         print(*question_translate_300(), sep="\n")
 
     replies = map(
         input,
         chain(
             ["\n> Choose the language of the questions above: "],
-            repeat("Please, only the numbers that are on the list are valid! Try again: "),
+            repeat(
+                "Please, only the numbers that are on the list are valid! Try again: "
+            ),
         ),
     )
     lang = int(next(filter(set(map(str, range(0, 3))).__contains__, replies)))
 
     quiz(
         inventory=int(inventory),
         sex=str(sex).upper(),
```

### Comparing `five-factor-e-1.8.0/ipipneo/reverse.py` & `five-factor-e-1.9.0/ipipneo/reverse.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Reverses scores for certain questions from the IPIP-120, IPIP-300 and Custom Items."""
 
 __author__ = "Ederson Corbari"
-__email__ = "e@neural7.io"
-__copyright__ = "Copyright Neural7 2022, Big 5 Personality Traits"
+__email__ = "e@rewire5.io"
+__copyright__ = "Copyright ReWire5 2022-2023, Big 5 Personality Traits"
 __credits__ = ["John A. Johnson", "Dhiru Kholia"]
 __license__ = "MIT"
-__version__ = "1.8.0"
+__version__ = "1.9.0"
 __status__ = "production"
 
 from ipipneo.utility import reverse_scored
 
 IPIP_NEO_ITEMS_REVERSED_120 = [
     9,
     19,
@@ -248,18 +248,24 @@
         if not any("id_select" in x for x in answers.get("answers", [])):
             raise BaseException("The key named (id_select) was not found!")
 
         if not any("reverse_scored" in x for x in answers.get("answers", [])):
             raise BaseException("The key named (reverse_scored) was not found!")
 
         def is_reversed_custom(x: dict) -> dict:
-            x["id_select"] = reverse_scored(select=x["id_select"]) if x.get("reverse_scored") == 1 else x["id_select"]
+            x["id_select"] = (
+                reverse_scored(select=x["id_select"])
+                if x.get("reverse_scored") == 1
+                else x["id_select"]
+            )
             return x
 
-        return {"answers": [is_reversed_custom(x=x) for x in answers.get("answers", [])]}
+        return {
+            "answers": [is_reversed_custom(x=x) for x in answers.get("answers", [])]
+        }
 
 
 class ReverseScored120:
     """Reverse scored for IPIP-120."""
 
     def __new__(self, answers: dict) -> dict or BaseException or AssertionError:
         """
@@ -281,24 +287,32 @@
 
         if not any("id_question" in x for x in answers.get("answers", [])):
             raise BaseException("The key named (id_question) was not found!")
 
         if not any("id_select" in x for x in answers.get("answers", [])):
             raise BaseException("The key named (id_select) was not found!")
 
-        assert len(list(IPIP_NEO_ITEMS_REVERSED_120)) == 55, "The number of reverse items should be 55!"
+        assert (
+            len(list(IPIP_NEO_ITEMS_REVERSED_120)) == 55
+        ), "The number of reverse items should be 55!"
 
         def is_reversed_120(x: int, y: int) -> int:
             for i in IPIP_NEO_ITEMS_REVERSED_120:
                 if x == i:
                     return reverse_scored(select=y)
             return y
 
         update = map(
-            (lambda x: (x.__setitem__("id_select", is_reversed_120(x["id_question"], x["id_select"])))),
+            (
+                lambda x: (
+                    x.__setitem__(
+                        "id_select", is_reversed_120(x["id_question"], x["id_select"])
+                    )
+                )
+            ),
             answers.get("answers"),
         )
         assert len(list(update)) == 120, "The update number should be 120!"
 
         return answers or {}
 
 
@@ -325,22 +339,30 @@
 
         if not any("id_question" in x for x in answers.get("answers", [])):
             raise BaseException("The key named (id_question) was not found!")
 
         if not any("id_select" in x for x in answers.get("answers", [])):
             raise BaseException("The key named (id_select) was not found!")
 
-        assert len(list(IPIP_NEO_ITEMS_REVERSED_300)) == 148, "The number of reverse items should be 148!"
+        assert (
+            len(list(IPIP_NEO_ITEMS_REVERSED_300)) == 148
+        ), "The number of reverse items should be 148!"
 
         def is_reversed_300(x: int, y: int) -> int:
             for i in IPIP_NEO_ITEMS_REVERSED_300:
                 if x == i:
                     return reverse_scored(select=y)
             return y
 
         update = map(
-            (lambda x: (x.__setitem__("id_select", is_reversed_300(x["id_question"], x["id_select"])))),
+            (
+                lambda x: (
+                    x.__setitem__(
+                        "id_select", is_reversed_300(x["id_question"], x["id_select"])
+                    )
+                )
+            ),
             answers.get("answers"),
         )
         assert len(list(update)) == 300, "The update number should be 300!"
 
         return answers or {}
```

### Comparing `five-factor-e-1.8.0/ipipneo/utility.py` & `five-factor-e-1.9.0/ipipneo/utility.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 """Contains utility functions used in the library."""
 
 __author__ = "Ederson Corbari"
-__email__ = "e@neural7.io"
-__copyright__ = "Copyright Neural7 2022, Big 5 Personality Traits"
+__email__ = "e@rewire5.io"
+__copyright__ = "Copyright ReWire5 2022-2023, Big 5 Personality Traits"
 __credits__ = ["John A. Johnson", "Dhiru Kholia"]
 __license__ = "MIT"
-__version__ = "1.8.0"
+__version__ = "1.9.0"
 __status__ = "production"
 
+from datetime import datetime
 from enum import Enum
 
-from ipipneo.model import (
-    Big5Agreeableness,
-    Big5Conscientiousness,
-    Big5Extraversion,
-    Big5Neuroticism,
-    Big5Openness,
-)
+from ipipneo.model import (Big5Agreeableness, Big5Conscientiousness,
+                           Big5Extraversion, Big5Neuroticism, Big5Openness)
 
 
 def raise_if_sex_is_invalid(sex: str) -> bool or AssertionError or BaseException:
     """
     Validate the sex field.
 
     Args:
@@ -44,15 +40,17 @@
     if not age:
         raise BaseException("The (age) field is required!")
 
     assert isinstance(age, int), "The (age) field must be an integer!"
 
     min, max = (10, 110)
     if not (min <= age <= max):
-        raise AssertionError("The age (%r) must be between %r and %r!" % (age, min, max))
+        raise AssertionError(
+            "The age (%r) must be between %r and %r!" % (age, min, max)
+        )
 
     return True
 
 
 def answers_is_valid(answers: list) -> bool or AssertionError or BaseException:
     """
     Validate the answers field.
@@ -67,15 +65,17 @@
 
     if 0 in answers:
         raise BaseException("It cannot contain zeros in the answer list!")
 
     if 1 in [1 if x > 5 else 0 for x in answers]:
         raise BaseException("You cannot have answers with a number greater than 5!")
 
-    assert len(answers) == 120 or len(answers) == 300, "The (answers) field should be of size 120 or 300!"
+    assert (
+        len(answers) == 120 or len(answers) == 300
+    ), "The (answers) field should be of size 120 or 300!"
 
     return True
 
 
 def organize_list_json(answers: dict) -> list or AssertionError or BaseException:
     """
     Organize input list in json format.
@@ -92,15 +92,17 @@
         raise BaseException("The key named (id_question) was not found!")
 
     if not any("id_select" in x for x in answers.get("answers", [])):
         raise BaseException("The key named (id_select) was not found!")
 
     return [
         x["id_select"]
-        for x in sorted([x for x in answers.get("answers", [])], key=lambda x: x["id_question"])
+        for x in sorted(
+            [x for x in answers.get("answers", [])], key=lambda x: x["id_question"]
+        )
         if x["id_select"] >= 1
     ]
 
 
 def reverse_scored(select: int) -> int or BaseException:
     """
     Apply reverse scoring (1=5, 2=4, 4=2, 5=1).
@@ -144,25 +146,29 @@
 def big5_target(label: str) -> Enum or BaseException:
     """
     Return the facets of a Big-Five.
 
     Args:
         - label: The acronym for the Big-Five standard O.C.E.A.N.
     """
-    if big5_ocean_is_valid(label=label):
+    big5_ocean_is_valid(label=label)
+
+    try:
         if label == "O":
             return Big5Openness
         if label == "C":
             return Big5Conscientiousness
         if label == "E":
             return Big5Extraversion
         if label == "A":
             return Big5Agreeableness
         if label == "N":
             return Big5Neuroticism
+    except BaseException:
+        raise BaseException("The Big-Five label is invalid!")
 
 
 def create_big5_dict(label: str, big5: float, x: list, y: list) -> dict:
     """
     Create a dictionary for Big-Five final result.
 
     Args:
@@ -202,7 +208,15 @@
             {
                 "trait": 6,
                 big5_target(label=label).TRAIT6.value: x[6],
                 "score": y[6],
             },
         ],
     }
+
+
+def add_dict_footer() -> dict:
+    return {
+        "library": "five-factor-e",
+        "version": __version__,
+        "date": datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
+    }
```

### Comparing `five-factor-e-1.8.0/setup.py` & `five-factor-e-1.9.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,37 +6,38 @@
 from setuptools import find_packages, setup
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "1.8.0"
+VERSION = "1.9.0"
 DESCRIPTION = "Big 5 IPIP-NEO Personality Traits"
 LONG_DESCRIPTION = "Library with a self-administered questionnaire that assesses a person's personality according to the Big Five model, using the IPIP-NEO."
 
 setup(
     name="five-factor-e",
     version=VERSION,
-    author="Ederson Corbari, Neural7",
-    author_email="<e@neural7.com>",
+    author="Ederson Corbari, ReWire5",
+    author_email="<e@rewire5.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(exclude=("test",)),
     python_requires=">=3.5",
     include_package_data=True,
     install_requires=[],
     extras_require={"quiz": ["plotext"]},
     entry_points={
         "console_scripts": [
             "ipipneo-quiz = ipipneo.quiz:main",
         ],
     },
     keywords=[
+        "IPIP",
         "IPIP-NEO",
         "Big-5",
         "Big-Five",
         "Five-Factor",
         "Personality",
         "Assessment",
         "Psychometrics",
```

### Comparing `five-factor-e-1.8.0/test/test_facet.py` & `five-factor-e-1.9.0/test/test_facet.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,17 @@
         with self.assertRaises(BaseException) as e:
             facet.b5create(score=[0, 0, 0])
         self.assertEqual(
             str(e.exception),
             "The number of questions setting is wrong: list index out of range",
         )
 
-        b5 = facet.b5create(score=facet.score(answers=organize_list_json(load_mock_answers_120())))
+        b5 = facet.b5create(
+            score=facet.score(answers=organize_list_json(load_mock_answers_120()))
+        )
         assert isinstance(b5, dict), "b5 must be a dict"
 
         self.assertEqual(len(b5.get("O")), 121)
         self.assertEqual(len(b5.get("C")), 121)
         self.assertEqual(len(b5.get("E")), 121)
         self.assertEqual(len(b5.get("A")), 121)
         self.assertEqual(len(b5.get("N")), 121)
@@ -112,15 +114,17 @@
         with self.assertRaises(BaseException) as e:
             facet.b5create(score=[0, 0, 0])
         self.assertEqual(
             str(e.exception),
             "The number of questions setting is wrong: list index out of range",
         )
 
-        b5 = facet.b5create(score=facet.score(answers=organize_list_json(load_mock_answers_300())))
+        b5 = facet.b5create(
+            score=facet.score(answers=organize_list_json(load_mock_answers_300()))
+        )
         assert isinstance(b5, dict), "b5 must be a dict"
 
         self.assertEqual(len(b5.get("O")), 301)
         self.assertEqual(len(b5.get("C")), 301)
         self.assertEqual(len(b5.get("E")), 301)
         self.assertEqual(len(b5.get("A")), 301)
         self.assertEqual(len(b5.get("N")), 301)
@@ -137,15 +141,17 @@
         with self.assertRaises(BaseException) as e:
             facet.domain(score=[-1, -1, -1])
         self.assertEqual(
             str(e.exception),
             "Invalid position in the score array: list index out of range",
         )
 
-        domain = facet.domain(score=facet.score(answers=organize_list_json(load_mock_answers_120())))
+        domain = facet.domain(
+            score=facet.score(answers=organize_list_json(load_mock_answers_120()))
+        )
         assert isinstance(domain, dict), "domain must be a dict"
 
         self.assertEqual(domain.get("O"), 78)
         self.assertEqual(domain.get("C"), 102)
         self.assertEqual(domain.get("E"), 66)
         self.assertEqual(domain.get("A"), 87)
         self.assertEqual(domain.get("N"), 61)
@@ -156,43 +162,51 @@
         with self.assertRaises(BaseException) as e:
             facet.domain(score=[-1, -1, -1])
         self.assertEqual(
             str(e.exception),
             "Invalid position in the score array: list index out of range",
         )
 
-        domain = facet.domain(score=facet.score(answers=organize_list_json(load_mock_answers_300())))
+        domain = facet.domain(
+            score=facet.score(answers=organize_list_json(load_mock_answers_300()))
+        )
         assert isinstance(domain, dict), "domain must be a dict"
 
         self.assertEqual(domain.get("O"), 180)
         self.assertEqual(domain.get("C"), 183)
         self.assertEqual(domain.get("E"), 188)
         self.assertEqual(domain.get("A"), 188)
         self.assertEqual(domain.get("N"), 187)
 
     def test_distrib_120(self) -> None:
         facet = Facet(nquestion=120)
 
         with self.assertRaises(TypeError):
             facet.distrib(size=0, b5={}, norm={})
 
-        b5 = facet.b5create(score=facet.score(answers=organize_list_json(load_mock_answers_120())))
+        b5 = facet.b5create(
+            score=facet.score(answers=organize_list_json(load_mock_answers_120()))
+        )
         assert isinstance(b5, dict), "b5 must be a dict"
 
-        domain = facet.domain(score=facet.score(answers=organize_list_json(load_mock_answers_120())))
+        domain = facet.domain(
+            score=facet.score(answers=organize_list_json(load_mock_answers_120()))
+        )
         assert isinstance(domain, dict), "domain must be a dict"
 
         with self.assertRaises(BaseException) as e:
             facet.distrib(size=0, b5=b5, norm=Norm(sex="M", age=40, nquestion=120))
         self.assertEqual(
             str(e.exception),
             "The number of questions setting is wrong: list assignment index out of range",
         )
 
-        distrib = facet.distrib(size=7, b5=b5, norm=Norm(sex="M", age=40, nquestion=120))
+        distrib = facet.distrib(
+            size=7, b5=b5, norm=Norm(sex="M", age=40, nquestion=120)
+        )
         assert isinstance(distrib, dict), "distrib must be a dict"
 
         self.assertEqual(distrib.get("O")[0], 0)
         self.assertEqual(distrib.get("C")[0], 0)
         self.assertEqual(distrib.get("E")[0], 0)
         self.assertEqual(distrib.get("A")[0], 0)
         self.assertEqual(distrib.get("N")[0], 0)
@@ -228,15 +242,17 @@
         self.assertEqual(distrib.get("N")[1], 51.48936170212766)
         self.assertEqual(distrib.get("N")[2], 50.58139534883721)
         self.assertEqual(distrib.get("N")[3], 44.247572815533985)
         self.assertEqual(distrib.get("N")[4], 47.08661417322835)
         self.assertEqual(distrib.get("N")[5], 43.80681818181818)
         self.assertEqual(distrib.get("N")[6], 46.75287356321839)
 
-        distrib = facet.distrib(size=7, b5=b5, norm=Norm(sex="F", age=30, nquestion=120))
+        distrib = facet.distrib(
+            size=7, b5=b5, norm=Norm(sex="F", age=30, nquestion=120)
+        )
         assert isinstance(distrib, dict), "distrib must be a dict"
 
         self.assertEqual(distrib.get("O")[1], 33.113772455089816)
         self.assertEqual(distrib.get("O")[2], 34.93939393939394)
         self.assertEqual(distrib.get("O")[3], 33.605947955390334)
         self.assertEqual(distrib.get("O")[4], 59.18604651162791)
         self.assertEqual(distrib.get("O")[5], 46.31123919308357)
@@ -272,28 +288,34 @@
 
     def test_distrib_300(self) -> None:
         facet = Facet(nquestion=300)
 
         with self.assertRaises(TypeError):
             facet.distrib(size=0, b5={}, norm={})
 
-        b5 = facet.b5create(score=facet.score(answers=organize_list_json(load_mock_answers_300())))
+        b5 = facet.b5create(
+            score=facet.score(answers=organize_list_json(load_mock_answers_300()))
+        )
         assert isinstance(b5, dict), "b5 must be a dict"
 
-        domain = facet.domain(score=facet.score(answers=organize_list_json(load_mock_answers_300())))
+        domain = facet.domain(
+            score=facet.score(answers=organize_list_json(load_mock_answers_300()))
+        )
         assert isinstance(domain, dict), "domain must be a dict"
 
         with self.assertRaises(BaseException) as e:
             facet.distrib(size=0, b5=b5, norm=Norm(sex="M", age=40, nquestion=300))
         self.assertEqual(
             str(e.exception),
             "The number of questions setting is wrong: list assignment index out of range",
         )
 
-        distrib = facet.distrib(size=7, b5=b5, norm=Norm(sex="M", age=40, nquestion=300))
+        distrib = facet.distrib(
+            size=7, b5=b5, norm=Norm(sex="M", age=40, nquestion=300)
+        )
         assert isinstance(distrib, dict), "distrib must be a dict"
 
         self.assertEqual(distrib.get("O")[0], 0)
         self.assertEqual(distrib.get("C")[0], 0)
         self.assertEqual(distrib.get("E")[0], 0)
         self.assertEqual(distrib.get("A")[0], 0)
         self.assertEqual(distrib.get("N")[0], 0)
@@ -381,15 +403,17 @@
 
         normalize = Norm.normalize(normc=normc, percent=percent)
         assert isinstance(normalize, dict), "normalize must be a dict"
 
         #############################################
         # 1. Neuroticism with its facets.
         #############################################
-        N = facet.personality(size=len(score), big5=normalize, traits=distrib, label="N")
+        N = facet.personality(
+            size=len(score), big5=normalize, traits=distrib, label="N"
+        )
         assert isinstance(N, dict), "N must be a dict"
         assert isinstance(N.get("traits"), list), "traits must be a list"
 
         self.assertEqual(N.get("N"), 37.23631660596993)
 
         self.assertEqual(N.get("traits")[0]["trait"], 1)
         self.assertEqual(N.get("traits")[0]["anxiety"], 55.29153291804727)
@@ -414,15 +438,17 @@
         self.assertEqual(N.get("traits")[5]["trait"], 6)
         self.assertEqual(N.get("traits")[5]["vulnerability"], 38.536490293892996)
         self.assertEqual(N.get("traits")[5]["score"], "average")
 
         #############################################
         # 2. Extraversion with its facets.
         #############################################
-        E = facet.personality(size=len(score), big5=normalize, traits=distrib, label="E")
+        E = facet.personality(
+            size=len(score), big5=normalize, traits=distrib, label="E"
+        )
         assert isinstance(N, dict), "E must be a dict"
         assert isinstance(N.get("traits"), list), "traits must be a list"
 
         self.assertEqual(E.get("E"), 21.46713047820697)
 
         self.assertEqual(E.get("traits")[0]["trait"], 1)
         self.assertEqual(E.get("traits")[0]["friendliness"], 20.788746198012063)
@@ -447,15 +473,17 @@
         self.assertEqual(E.get("traits")[5]["trait"], 6)
         self.assertEqual(E.get("traits")[5]["cheerfulness"], 27.560328329400278)
         self.assertEqual(E.get("traits")[5]["score"], "low")
 
         #############################################
         # 3. Openness with its facets.
         #############################################
-        O = facet.personality(size=len(score), big5=normalize, traits=distrib, label="O")
+        O = facet.personality(
+            size=len(score), big5=normalize, traits=distrib, label="O"
+        )
         assert isinstance(O, dict), "O must be a dict"
         assert isinstance(O.get("traits"), list), "traits must be a list"
 
         self.assertEqual(O.get("O"), 26.882298529738506)
 
         self.assertEqual(O.get("traits")[0]["trait"], 1)
         self.assertEqual(O.get("traits")[0]["imagination"], 1)
@@ -480,15 +508,17 @@
         self.assertEqual(O.get("traits")[5]["trait"], 6)
         self.assertEqual(O.get("traits")[5]["liberalism"], 79.99472618213304)
         self.assertEqual(O.get("traits")[5]["score"], "high")
 
         #############################################
         # 4. Agreeableness with its facets.
         #############################################
-        A = facet.personality(size=len(score), big5=normalize, traits=distrib, label="A")
+        A = facet.personality(
+            size=len(score), big5=normalize, traits=distrib, label="A"
+        )
         assert isinstance(A, dict), "A must be a dict"
         assert isinstance(A.get("traits"), list), "traits must be a list"
 
         self.assertEqual(A.get("A"), 57.52658875205816)
 
         self.assertEqual(A.get("traits")[0]["trait"], 1)
         self.assertEqual(A.get("traits")[0]["trust"], 70.5561195632738)
@@ -513,15 +543,17 @@
         self.assertEqual(A.get("traits")[5]["trait"], 6)
         self.assertEqual(A.get("traits")[5]["sympathy"], 21.651269458084244)
         self.assertEqual(A.get("traits")[5]["score"], "low")
 
         #############################################
         # 5. Conscientiousness with its facets.
         #############################################
-        C = facet.personality(size=len(score), big5=normalize, traits=distrib, label="C")
+        C = facet.personality(
+            size=len(score), big5=normalize, traits=distrib, label="C"
+        )
         assert isinstance(C, dict), "C must be a dict"
         assert isinstance(C.get("traits"), list), "traits must be a list"
 
         self.assertEqual(C.get("C"), 86.96687032595662)
 
         self.assertEqual(C.get("traits")[0]["trait"], 1)
         self.assertEqual(C.get("traits")[0]["self_efficacy"], 67.18081968991703)
@@ -833,15 +865,17 @@
 
         normalize = Norm.normalize(normc=normc, percent=percent)
         assert isinstance(normalize, dict), "normalize must be a dict"
 
         #############################################
         # 1. Neuroticism with its facets.
         #############################################
-        N = facet.personality(size=len(score), big5=normalize, traits=distrib, label="N")
+        N = facet.personality(
+            size=len(score), big5=normalize, traits=distrib, label="N"
+        )
         assert isinstance(N, dict), "N must be a dict"
         assert isinstance(N.get("traits"), list), "traits must be a list"
 
         self.assertEqual(N.get("N"), 72.42696555428512)
 
         self.assertEqual(N.get("traits")[0]["trait"], 1)
         self.assertEqual(N.get("traits")[0]["anxiety"], 56.21355262825239)
@@ -866,15 +900,17 @@
         self.assertEqual(N.get("traits")[5]["trait"], 6)
         self.assertEqual(N.get("traits")[5]["vulnerability"], 98.37585552257963)
         self.assertEqual(N.get("traits")[5]["score"], "high")
 
         #############################################
         # 2. Extraversion with its facets.
         #############################################
-        E = facet.personality(size=len(score), big5=normalize, traits=distrib, label="E")
+        E = facet.personality(
+            size=len(score), big5=normalize, traits=distrib, label="E"
+        )
         assert isinstance(N, dict), "E must be a dict"
         assert isinstance(N.get("traits"), list), "traits must be a list"
 
         self.assertEqual(E.get("E"), 44.65415108872236)
 
         self.assertEqual(E.get("traits")[0]["trait"], 1)
         self.assertEqual(E.get("traits")[0]["friendliness"], 49.56063603396092)
@@ -899,15 +935,17 @@
         self.assertEqual(E.get("traits")[5]["trait"], 6)
         self.assertEqual(E.get("traits")[5]["cheerfulness"], 37.907163869258454)
         self.assertEqual(E.get("traits")[5]["score"], "average")
 
         #############################################
         # 3. Openness with its facets.
         #############################################
-        O = facet.personality(size=len(score), big5=normalize, traits=distrib, label="O")
+        O = facet.personality(
+            size=len(score), big5=normalize, traits=distrib, label="O"
+        )
         assert isinstance(O, dict), "O must be a dict"
         assert isinstance(O.get("traits"), list), "traits must be a list"
 
         self.assertEqual(O.get("O"), 6.765261759154043)
 
         self.assertEqual(O.get("traits")[0]["trait"], 1)
         self.assertEqual(O.get("traits")[0]["imagination"], 3.019669333842657)
@@ -932,15 +970,17 @@
         self.assertEqual(O.get("traits")[5]["trait"], 6)
         self.assertEqual(O.get("traits")[5]["liberalism"], 29.473450015379456)
         self.assertEqual(O.get("traits")[5]["score"], "low")
 
         #############################################
         # 4. Agreeableness with its facets.
         #############################################
-        A = facet.personality(size=len(score), big5=normalize, traits=distrib, label="A")
+        A = facet.personality(
+            size=len(score), big5=normalize, traits=distrib, label="A"
+        )
         assert isinstance(A, dict), "A must be a dict"
         assert isinstance(A.get("traits"), list), "traits must be a list"
 
         self.assertEqual(A.get("A"), 31.13757270081055)
 
         self.assertEqual(A.get("traits")[0]["trait"], 1)
         self.assertEqual(A.get("traits")[0]["trust"], 56.53893235643574)
@@ -965,15 +1005,17 @@
         self.assertEqual(A.get("traits")[5]["trait"], 6)
         self.assertEqual(A.get("traits")[5]["sympathy"], 1.7779210136593235)
         self.assertEqual(A.get("traits")[5]["score"], "low")
 
         #############################################
         # 5. Conscientiousness with its facets.
         #############################################
-        C = facet.personality(size=len(score), big5=normalize, traits=distrib, label="C")
+        C = facet.personality(
+            size=len(score), big5=normalize, traits=distrib, label="C"
+        )
         assert isinstance(C, dict), "C must be a dict"
         assert isinstance(C.get("traits"), list), "traits must be a list"
 
         self.assertEqual(C.get("C"), 15.799085796472156)
 
         self.assertEqual(C.get("traits")[0]["trait"], 1)
         self.assertEqual(C.get("traits")[0]["self_efficacy"], 17.11734969494421)
```

### Comparing `five-factor-e-1.8.0/test/test_ipipneo.py` & `five-factor-e-1.9.0/test/test_ipipneo.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 def load_mock_answers_custom() -> dict:
     with open(f"test/mock/answers-test-6.json") as f:
         data = json.load(f)
     return data
 
 
 class TestIpipNeo(unittest.TestCase):
-
     maxDiff = None
 
     def test_invalid_params(self) -> None:
         with self.assertRaises(BaseException):
             IpipNeo(question="")
 
         with self.assertRaises(BaseException):
@@ -53,15 +52,17 @@
             big5.compute("")
 
         big5 = None
 
         #############################################
         # 1. Test with 40 year old man.
         #############################################
-        result = IpipNeo(question=120).compute(sex="M", age=40, answers=load_mock_answers_120())
+        result = IpipNeo(question=120).compute(
+            sex="M", age=40, answers=load_mock_answers_120()
+        )
 
         self.assertTrue(len(result.get("id")))
         self.assertTrue(len(result.get("theory")))
         self.assertTrue(len(result.get("model")))
 
         self.assertEqual(result.get("question"), 120)
         self.assertEqual(result.get("person").get("sex"), "M")
@@ -70,23 +71,27 @@
         self.assertTrue(len(result.get("person").get("result")))
         self.assertTrue(len(result.get("person").get("result").get("personalities")))
 
         personalities = result.get("person").get("result").get("personalities")
         self.assertEqual(len(personalities), 5)
 
         self.assertEqual(personalities[0]["openness"].get("O"), 13.262383714475419)
-        self.assertEqual(personalities[1]["conscientiousness"].get("C"), 18.62283542366208)
+        self.assertEqual(
+            personalities[1]["conscientiousness"].get("C"), 18.62283542366208
+        )
         self.assertEqual(personalities[2]["extraversion"].get("E"), 34.10779114957646)
         self.assertEqual(personalities[3]["agreeableness"].get("A"), 1.9889215690788262)
         self.assertEqual(personalities[4]["neuroticism"].get("N"), 58.6632925696303)
 
         #############################################
         # 2. Test with 30 year old woman.
         #############################################
-        result = IpipNeo(question=120).compute(sex="F", age=30, answers=load_mock_answers_120())
+        result = IpipNeo(question=120).compute(
+            sex="F", age=30, answers=load_mock_answers_120()
+        )
 
         self.assertTrue(len(result.get("id")))
         self.assertTrue(len(result.get("theory")))
         self.assertTrue(len(result.get("model")))
 
         self.assertEqual(result.get("question"), 120)
         self.assertEqual(result.get("person").get("sex"), "F")
@@ -95,23 +100,27 @@
         self.assertTrue(len(result.get("person").get("result")))
         self.assertTrue(len(result.get("person").get("result").get("personalities")))
 
         personalities = result.get("person").get("result").get("personalities")
         self.assertEqual(len(personalities), 5)
 
         self.assertEqual(personalities[0]["openness"].get("O"), 8.876064362586419)
-        self.assertEqual(personalities[1]["conscientiousness"].get("C"), 13.877369975064141)
+        self.assertEqual(
+            personalities[1]["conscientiousness"].get("C"), 13.877369975064141
+        )
         self.assertEqual(personalities[2]["extraversion"].get("E"), 29.240137885780882)
         self.assertEqual(personalities[3]["agreeableness"].get("A"), 1)
         self.assertEqual(personalities[4]["neuroticism"].get("N"), 47.49034742252866)
 
         #############################################
         # 3. Test with 65 year old woman.
         #############################################
-        result = IpipNeo(question=120).compute(sex="F", age=65, answers=load_mock_answers_120(), compare=True)
+        result = IpipNeo(question=120).compute(
+            sex="F", age=65, answers=load_mock_answers_120(), compare=True
+        )
 
         self.assertIn("id", result)
         self.assertIn("theory", result)
         self.assertIn("model", result)
         self.assertIn("question", result)
         self.assertIn("person", result)
 
@@ -139,19 +148,29 @@
 
         self.assertEqual(personalities[0]["openness"].get("O"), 24.29091080263288)
         self.assertEqual(personalities[1]["conscientiousness"].get("C"), 1)
         self.assertEqual(personalities[2]["extraversion"].get("E"), 32.92660962191414)
         self.assertEqual(personalities[3]["agreeableness"].get("A"), 1)
         self.assertEqual(personalities[4]["neuroticism"].get("N"), 67.59105722337824)
 
-        original = result.get("person").get("result").get("compare").get("user_answers_original")
+        original = (
+            result.get("person")
+            .get("result")
+            .get("compare")
+            .get("user_answers_original")
+        )
         assert isinstance(original, list), "original must be a list"
         self.assertEqual(len(original), 120)
 
-        reversed = result.get("person").get("result").get("compare").get("user_answers_reversed")
+        reversed = (
+            result.get("person")
+            .get("result")
+            .get("compare")
+            .get("user_answers_reversed")
+        )
         assert isinstance(reversed, list), "reversed must be a list"
         self.assertEqual(len(reversed), 120)
 
         a = [x.get("id_select") for x in original]
         assert isinstance(original, list), "reversed must be a list"
 
         b = [x.get("id_select") for x in reversed]
@@ -208,15 +227,17 @@
         self.assertEqual(a[66], 2)
         self.assertEqual(b[66], 4)
 
     def test_compute_300(self) -> None:
         #############################################
         # 1. Test with 40 year old man.
         #############################################
-        result = IpipNeo(question=300).compute(sex="M", age=40, answers=load_mock_answers_300())
+        result = IpipNeo(question=300).compute(
+            sex="M", age=40, answers=load_mock_answers_300()
+        )
 
         self.assertTrue(len(result.get("id")))
         self.assertTrue(len(result.get("theory")))
         self.assertTrue(len(result.get("model")))
 
         self.assertEqual(result.get("question"), 300)
         self.assertEqual(result.get("person").get("sex"), "M")
@@ -225,23 +246,27 @@
         self.assertTrue(len(result.get("person").get("result")))
         self.assertTrue(len(result.get("person").get("result").get("personalities")))
 
         personalities = result.get("person").get("result").get("personalities")
         self.assertEqual(len(personalities), 5)
 
         self.assertEqual(personalities[0]["openness"].get("O"), 38.846625568407774)
-        self.assertEqual(personalities[1]["conscientiousness"].get("C"), 4.6266733183044835)
+        self.assertEqual(
+            personalities[1]["conscientiousness"].get("C"), 4.6266733183044835
+        )
         self.assertEqual(personalities[2]["extraversion"].get("E"), 58.00148636052478)
         self.assertEqual(personalities[3]["agreeableness"].get("A"), 11.934721812005705)
         self.assertEqual(personalities[4]["neuroticism"].get("N"), 78.82240987792443)
 
         #############################################
         # 2. Test with 30 year old woman.
         #############################################
-        result = IpipNeo(question=300).compute(sex="F", age=30, answers=load_mock_answers_300())
+        result = IpipNeo(question=300).compute(
+            sex="F", age=30, answers=load_mock_answers_300()
+        )
 
         self.assertTrue(len(result.get("id")))
         self.assertTrue(len(result.get("theory")))
         self.assertTrue(len(result.get("model")))
 
         self.assertEqual(result.get("question"), 300)
         self.assertEqual(result.get("person").get("sex"), "F")
@@ -258,15 +283,17 @@
         self.assertEqual(personalities[2]["extraversion"].get("E"), 54.26151488253112)
         self.assertEqual(personalities[3]["agreeableness"].get("A"), 1)
         self.assertEqual(personalities[4]["neuroticism"].get("N"), 71.14096931653722)
 
         #############################################
         # 3. Test with 65 year old woman.
         #############################################
-        result = IpipNeo(question=300).compute(sex="F", age=65, answers=load_mock_answers_300(), compare=True)
+        result = IpipNeo(question=300).compute(
+            sex="F", age=65, answers=load_mock_answers_300(), compare=True
+        )
 
         self.assertIn("id", result)
         self.assertIn("theory", result)
         self.assertIn("model", result)
         self.assertIn("question", result)
         self.assertIn("person", result)
 
@@ -294,19 +321,29 @@
 
         self.assertEqual(personalities[0]["openness"].get("O"), 28.963387129747275)
         self.assertEqual(personalities[1]["conscientiousness"].get("C"), 1)
         self.assertEqual(personalities[2]["extraversion"].get("E"), 54.26151488253112)
         self.assertEqual(personalities[3]["agreeableness"].get("A"), 1)
         self.assertEqual(personalities[4]["neuroticism"].get("N"), 71.14096931653722)
 
-        original = result.get("person").get("result").get("compare").get("user_answers_original")
+        original = (
+            result.get("person")
+            .get("result")
+            .get("compare")
+            .get("user_answers_original")
+        )
         assert isinstance(original, list), "original must be a list"
         self.assertEqual(len(original), 300)
 
-        reversed = result.get("person").get("result").get("compare").get("user_answers_reversed")
+        reversed = (
+            result.get("person")
+            .get("result")
+            .get("compare")
+            .get("user_answers_reversed")
+        )
         assert isinstance(reversed, list), "reversed must be a list"
         self.assertEqual(len(reversed), 300)
 
         a = [x.get("id_select") for x in original]
         assert isinstance(original, list), "reversed must be a list"
 
         b = [x.get("id_select") for x in reversed]
@@ -349,24 +386,30 @@
         personalities = result.get("person").get("result").get("personalities")
         self.assertEqual(len(personalities), 5)
 
         compare = result.get("person").get("result").get("compare")
         self.assertIn("user_answers_original", compare)
         self.assertIn("user_answers_reversed", compare)
 
-        select1 = [x.get("reverse_scored") for x in compare.get("user_answers_original", [])]
+        select1 = [
+            x.get("reverse_scored") for x in compare.get("user_answers_original", [])
+        ]
         assert isinstance(select1, list), "select1 must be a list"
 
         self.assertEqual(select1.count(0), 67)
         self.assertEqual(select1.count(1), 53)
 
-        select2 = [x.get("reverse_scored") for x in compare.get("user_answers_reversed", [])]
+        select2 = [
+            x.get("reverse_scored") for x in compare.get("user_answers_reversed", [])
+        ]
         assert isinstance(select2, list), "select2 must be a list"
 
         self.assertEqual(select2.count(0), select1.count(0))
         self.assertEqual(select2.count(1), select1.count(1))
 
         self.assertEqual(personalities[0]["openness"].get("O"), 17.42235805055492)
-        self.assertEqual(personalities[1]["conscientiousness"].get("C"), 18.62283542366208)
+        self.assertEqual(
+            personalities[1]["conscientiousness"].get("C"), 18.62283542366208
+        )
         self.assertEqual(personalities[2]["extraversion"].get("E"), 34.10779114957646)
         self.assertEqual(personalities[3]["agreeableness"].get("A"), 6.331832993524202)
         self.assertEqual(personalities[4]["neuroticism"].get("N"), 58.6632925696303)
```

### Comparing `five-factor-e-1.8.0/test/test_model.py` & `five-factor-e-1.9.0/test/test_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,15 @@
 """Unit tests for Model."""
 
 import unittest
 
-from ipipneo.model import (
-    Big5Agreeableness,
-    Big5Conscientiousness,
-    Big5Extraversion,
-    Big5Neuroticism,
-    Big5Openness,
-    FacetLevel,
-    FacetScale,
-    NormCubic,
-    NormScale,
-    QuestionNumber,
-)
+from ipipneo.model import (Big5Agreeableness, Big5Conscientiousness,
+                           Big5Extraversion, Big5Neuroticism, Big5Openness,
+                           FacetLevel, FacetScale, NormCubic, NormScale,
+                           QuestionNumber)
 
 
 class TestModel(unittest.TestCase):
     def test_question_number(self) -> None:
         model = QuestionNumber
 
         self.assertEqual(model.IPIP_120, 120)
```

### Comparing `five-factor-e-1.8.0/test/test_norm.py` & `five-factor-e-1.9.0/test/test_norm.py`

 * *Files identical despite different names*

### Comparing `five-factor-e-1.8.0/test/test_reverse.py` & `five-factor-e-1.9.0/test/test_reverse.py`

 * *Files identical despite different names*

### Comparing `five-factor-e-1.8.0/test/test_utility.py` & `five-factor-e-1.9.0/test/test_utility.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 """Unit tests for Utility."""
 
 import json
 import unittest
 
-from ipipneo.utility import (answers_is_valid, big5_ocean_is_valid,
-                             big5_target, create_big5_dict, organize_list_json,
+from ipipneo.utility import (add_dict_footer, answers_is_valid,
+                             big5_ocean_is_valid, big5_target,
+                             create_big5_dict, organize_list_json,
                              raise_if_age_is_invalid, raise_if_sex_is_invalid,
                              reverse_scored)
 
+LIB_CURRENT_VERSION = "1.9.0"
+
 
 def load_mock_answers(idx: int) -> dict:
     if idx == 1:
         name = "answers-test-1.json"
     elif idx == 2:
         name = "answers-test-2.json"
     with open(f"test/mock/{name}") as f:
         data = json.load(f)
     return data
 
 
 class TestUtility(unittest.TestCase):
-
     maxDiff = None
 
     def test_raise_if_sex_is_invalid(self) -> None:
         with self.assertRaises(BaseException):
             raise_if_sex_is_invalid(sex="")
 
         with self.assertRaises(AssertionError):
@@ -587,7 +589,14 @@
         )
 
         self.assertEqual(reverse_scored(select=1), 5)
         self.assertEqual(reverse_scored(select=2), 4)
         self.assertEqual(reverse_scored(select=3), 3)
         self.assertEqual(reverse_scored(select=4), 2)
         self.assertEqual(reverse_scored(select=5), 1)
+
+    def test_add_dict_footer(self) -> None:
+        footer = add_dict_footer()
+        assert isinstance(footer, dict), "footer must be a dict"
+
+        self.assertEqual(footer.get("library"), "five-factor-e")
+        self.assertEqual(footer.get("version"), LIB_CURRENT_VERSION)
```

