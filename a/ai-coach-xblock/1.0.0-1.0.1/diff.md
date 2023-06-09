# Comparing `tmp/ai-coach-xblock-1.0.0.tar.gz` & `tmp/ai-coach-xblock-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai-coach-xblock-1.0.0.tar", last modified: Fri Jun  9 09:32:27 2023, max compression
+gzip compressed data, was "ai-coach-xblock-1.0.1.tar", last modified: Fri Jun  9 14:39:01 2023, max compression
```

## Comparing `ai-coach-xblock-1.0.0.tar` & `ai-coach-xblock-1.0.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 09:32:27.865096 ai-coach-xblock-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-06-09 09:32:24.000000 ai-coach-xblock-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     3287 2023-06-09 09:32:27.865096 ai-coach-xblock-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2465 2023-06-09 09:32:24.000000 ai-coach-xblock-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 09:32:27.861096 ai-coach-xblock-1.0.0/ai_coach/
--rw-r--r--   0 runner    (1001) docker     (122)       36 2023-06-09 09:32:24.000000 ai-coach-xblock-1.0.0/ai_coach/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5778 2023-06-09 09:32:24.000000 ai-coach-xblock-1.0.0/ai_coach/ai_coach.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 09:32:27.861096 ai-coach-xblock-1.0.0/ai_coach/static/
--rw-r--r--   0 runner    (1001) docker     (122)      767 2023-06-09 09:32:24.000000 ai-coach-xblock-1.0.0/ai_coach/static/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 09:32:27.861096 ai-coach-xblock-1.0.0/ai_coach/static/css/
--rw-r--r--   0 runner    (1001) docker     (122)      984 2023-06-09 09:32:24.000000 ai-coach-xblock-1.0.0/ai_coach/static/css/ai_coach.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 09:32:27.861096 ai-coach-xblock-1.0.0/ai_coach/static/html/
--rw-r--r--   0 runner    (1001) docker     (122)      679 2023-06-09 09:32:24.000000 ai-coach-xblock-1.0.0/ai_coach/static/html/ai_coach.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 09:32:27.857096 ai-coach-xblock-1.0.0/ai_coach/static/js/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 09:32:27.861096 ai-coach-xblock-1.0.0/ai_coach/static/js/src/
--rw-r--r--   0 runner    (1001) docker     (122)     1944 2023-06-09 09:32:24.000000 ai-coach-xblock-1.0.0/ai_coach/static/js/src/ai_coach.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 09:32:27.865096 ai-coach-xblock-1.0.0/ai_coach_xblock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3287 2023-06-09 09:32:27.000000 ai-coach-xblock-1.0.0/ai_coach_xblock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      434 2023-06-09 09:32:27.000000 ai-coach-xblock-1.0.0/ai_coach_xblock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-09 09:32:27.000000 ai-coach-xblock-1.0.0/ai_coach_xblock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       47 2023-06-09 09:32:27.000000 ai-coach-xblock-1.0.0/ai_coach_xblock.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-06-09 09:32:27.000000 ai-coach-xblock-1.0.0/ai_coach_xblock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-09 09:32:27.000000 ai-coach-xblock-1.0.0/ai_coach_xblock.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-09 09:32:27.865096 ai-coach-xblock-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1281 2023-06-09 09:32:24.000000 ai-coach-xblock-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:39:01.011066 ai-coach-xblock-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-06-09 14:38:58.000000 ai-coach-xblock-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     3647 2023-06-09 14:39:01.011066 ai-coach-xblock-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2825 2023-06-09 14:38:58.000000 ai-coach-xblock-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:39:01.011066 ai-coach-xblock-1.0.1/ai_coach/
+-rw-r--r--   0 runner    (1001) docker     (122)       36 2023-06-09 14:38:58.000000 ai-coach-xblock-1.0.1/ai_coach/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5778 2023-06-09 14:38:58.000000 ai-coach-xblock-1.0.1/ai_coach/ai_coach.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:39:01.011066 ai-coach-xblock-1.0.1/ai_coach/static/
+-rw-r--r--   0 runner    (1001) docker     (122)      767 2023-06-09 14:38:58.000000 ai-coach-xblock-1.0.1/ai_coach/static/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:39:01.011066 ai-coach-xblock-1.0.1/ai_coach/static/css/
+-rw-r--r--   0 runner    (1001) docker     (122)      984 2023-06-09 14:38:58.000000 ai-coach-xblock-1.0.1/ai_coach/static/css/ai_coach.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:39:01.011066 ai-coach-xblock-1.0.1/ai_coach/static/html/
+-rw-r--r--   0 runner    (1001) docker     (122)      679 2023-06-09 14:38:58.000000 ai-coach-xblock-1.0.1/ai_coach/static/html/ai_coach.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:39:01.007066 ai-coach-xblock-1.0.1/ai_coach/static/js/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:39:01.011066 ai-coach-xblock-1.0.1/ai_coach/static/js/src/
+-rw-r--r--   0 runner    (1001) docker     (122)     2002 2023-06-09 14:38:58.000000 ai-coach-xblock-1.0.1/ai_coach/static/js/src/ai_coach.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:39:01.011066 ai-coach-xblock-1.0.1/ai_coach_xblock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3647 2023-06-09 14:39:00.000000 ai-coach-xblock-1.0.1/ai_coach_xblock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      434 2023-06-09 14:39:00.000000 ai-coach-xblock-1.0.1/ai_coach_xblock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-09 14:39:00.000000 ai-coach-xblock-1.0.1/ai_coach_xblock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       47 2023-06-09 14:39:00.000000 ai-coach-xblock-1.0.1/ai_coach_xblock.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-06-09 14:39:00.000000 ai-coach-xblock-1.0.1/ai_coach_xblock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-09 14:39:00.000000 ai-coach-xblock-1.0.1/ai_coach_xblock.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-09 14:39:01.011066 ai-coach-xblock-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1281 2023-06-09 14:38:59.000000 ai-coach-xblock-1.0.1/setup.py
```

### Comparing `ai-coach-xblock-1.0.0/LICENSE` & `ai-coach-xblock-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ai-coach-xblock-1.0.0/PKG-INFO` & `ai-coach-xblock-1.0.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-coach-xblock
-Version: 1.0.0
+Version: 1.0.1
 Summary: AI Coach Xblock evaluates open response answer of a question using Open AI
 Home-page: https://github.com/edly-io/ai-feedback-xblock
 Author: edly
 License: AGPL v3
 Description: # **AI Coach XBlock**
         
         AI Coach Xblock helps learner in improving their answers by levering power of AI. It evaluates open response answer of a question using Open AI and provides feedback to learner.
@@ -28,48 +28,48 @@
         ```python
         OPENAI_SECRET_KEY='set-secret-key'
         ```
         
         ### **Update Advanced Settings of course**
         Update course advanced settings by adding `ai_coach` as shown in below image
         
-        ![Update settings image](./docs/images/update-settings.png)
+        ![Update settings image](https://github.com/edly-io/ai-coach-xblock/blob/main/docs/images/update-settings.png?raw=True)
         
         ### **Update settings of AI Coach Component**
         
         AI Coach Xblock will be available in Advanced component of course unit now. Add "AI Coach" xblock in unit and click "Edit" button to
         add `question` & `question context` and configure it.
         
         > `Context` is the context of question with answer which is provided to OpenAI for feedback generation. Question and Learner Answer is integrated into context using `{{question}}` and `{{answer}}` keywords which automatically picks question & learner aswer value. 
         > Example: 
         ```I am grade 8 student studying leadership. My teacher asked me question: {{question}} . I answered {{answer}} . Provide two tips to improve my answer as a grade 8 student. ```   
         
         
-        ![Configure AI Coach XBlock Image](./docs/images/configure-ai-coach.png)
+        ![Configure AI Coach XBlock Image](https://github.com/edly-io/ai-coach-xblock/blob/main/docs/images/configure-ai-coach.png?raw=True)
         
         
         ### **Publish Content**
         
         Use "Preview" button to preview it or publish your content and use "View Live Version" button to see how it appears on LMS
         
-        ![Preview Live XBlock](./docs/images/ai-coach-preview.png)
+        ![Preview Live XBlock](https://github.com/edly-io/ai-coach-xblock/blob/main/docs/images/ai-coach-preview.png?raw=True)
         
         
         ### **Ask For Feedback**
         
         After adding answer, learner click on `Ask from Coach` button for feedback. Feedback is provided by OPEN AI on the basis of question context and answer. 
         
         > "**Ask from Coach**" button disappears when the feedback threshold (Maximum no. of times one can request for feedback) is reached. By default, feedback threshold is 1.
         
-        ![Ask from Coach](./docs/images/ask-from-coach.png)
+        ![Ask from Coach](https://github.com/edly-io/ai-coach-xblock/blob/main/docs/images/ask-from-coach.png?raw=True)
         
         
         
         ### **Submitting Answer**
         
         Submit button saves the learner answer and mark the completion of Xblock.
         
-        ![Submit Answer](./docs/images/submit-answer.png)
-        ![Xblock Completion](./docs/images/xblock-completion.png)
+        ![Submit Answer](https://github.com/edly-io/ai-coach-xblock/blob/main/docs/images/submit-answer.png?raw=True)
+        ![Xblock Completion](https://github.com/edly-io/ai-coach-xblock/blob/main/docs/images/xblock-completion.png?raw=True)
         
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `ai-coach-xblock-1.0.0/README.md` & `ai-coach-xblock-1.0.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -21,45 +21,45 @@
 ```python
 OPENAI_SECRET_KEY='set-secret-key'
 ```
 
 ### **Update Advanced Settings of course**
 Update course advanced settings by adding `ai_coach` as shown in below image
 
-![Update settings image](./docs/images/update-settings.png)
+![Update settings image](https://github.com/edly-io/ai-coach-xblock/blob/main/docs/images/update-settings.png?raw=True)
 
 ### **Update settings of AI Coach Component**
 
 AI Coach Xblock will be available in Advanced component of course unit now. Add "AI Coach" xblock in unit and click "Edit" button to
 add `question` & `question context` and configure it.
 
 > `Context` is the context of question with answer which is provided to OpenAI for feedback generation. Question and Learner Answer is integrated into context using `{{question}}` and `{{answer}}` keywords which automatically picks question & learner aswer value. 
 > Example: 
 ```I am grade 8 student studying leadership. My teacher asked me question: {{question}} . I answered {{answer}} . Provide two tips to improve my answer as a grade 8 student. ```   
 
 
-![Configure AI Coach XBlock Image](./docs/images/configure-ai-coach.png)
+![Configure AI Coach XBlock Image](https://github.com/edly-io/ai-coach-xblock/blob/main/docs/images/configure-ai-coach.png?raw=True)
 
 
 ### **Publish Content**
 
 Use "Preview" button to preview it or publish your content and use "View Live Version" button to see how it appears on LMS
 
-![Preview Live XBlock](./docs/images/ai-coach-preview.png)
+![Preview Live XBlock](https://github.com/edly-io/ai-coach-xblock/blob/main/docs/images/ai-coach-preview.png?raw=True)
 
 
 ### **Ask For Feedback**
 
 After adding answer, learner click on `Ask from Coach` button for feedback. Feedback is provided by OPEN AI on the basis of question context and answer. 
 
 > "**Ask from Coach**" button disappears when the feedback threshold (Maximum no. of times one can request for feedback) is reached. By default, feedback threshold is 1.
 
-![Ask from Coach](./docs/images/ask-from-coach.png)
+![Ask from Coach](https://github.com/edly-io/ai-coach-xblock/blob/main/docs/images/ask-from-coach.png?raw=True)
 
 
 
 ### **Submitting Answer**
 
 Submit button saves the learner answer and mark the completion of Xblock.
 
-![Submit Answer](./docs/images/submit-answer.png)
-![Xblock Completion](./docs/images/xblock-completion.png)
+![Submit Answer](https://github.com/edly-io/ai-coach-xblock/blob/main/docs/images/submit-answer.png?raw=True)
+![Xblock Completion](https://github.com/edly-io/ai-coach-xblock/blob/main/docs/images/xblock-completion.png?raw=True)
```

### Comparing `ai-coach-xblock-1.0.0/ai_coach/ai_coach.py` & `ai-coach-xblock-1.0.1/ai_coach/ai_coach.py`

 * *Files identical despite different names*

### Comparing `ai-coach-xblock-1.0.0/ai_coach/static/README.txt` & `ai-coach-xblock-1.0.1/ai_coach/static/README.txt`

 * *Files identical despite different names*

### Comparing `ai-coach-xblock-1.0.0/ai_coach/static/css/ai_coach.css` & `ai-coach-xblock-1.0.1/ai_coach/static/css/ai_coach.css`

 * *Files identical despite different names*

### Comparing `ai-coach-xblock-1.0.0/ai_coach/static/html/ai_coach.html` & `ai-coach-xblock-1.0.1/ai_coach/static/html/ai_coach.html`

 * *Files identical despite different names*

### Comparing `ai-coach-xblock-1.0.0/ai_coach/static/js/src/ai_coach.js` & `ai-coach-xblock-1.0.1/ai_coach/static/js/src/ai_coach.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -13,15 +13,17 @@
             messageElement.text(result.error);
             return;
         }
 
         messageElement.text('');
         coachAnswer.text(result.coach_answer);
 
-        $('.ask-from-coach', element).hide();
+        if (!result.can_request_feedback) {
+            $('.ask-from-coach', element).hide();
+        }
         $('.coach-answer ', element).show();
     }
 
     function submitAnswer(result) {
         removeClassesFromMsgElement();
 
         if (result.hasOwnProperty('error')) {
```

### Comparing `ai-coach-xblock-1.0.0/ai_coach_xblock.egg-info/PKG-INFO` & `ai-coach-xblock-1.0.1/ai_coach_xblock.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-coach-xblock
-Version: 1.0.0
+Version: 1.0.1
 Summary: AI Coach Xblock evaluates open response answer of a question using Open AI
 Home-page: https://github.com/edly-io/ai-feedback-xblock
 Author: edly
 License: AGPL v3
 Description: # **AI Coach XBlock**
         
         AI Coach Xblock helps learner in improving their answers by levering power of AI. It evaluates open response answer of a question using Open AI and provides feedback to learner.
@@ -28,48 +28,48 @@
         ```python
         OPENAI_SECRET_KEY='set-secret-key'
         ```
         
         ### **Update Advanced Settings of course**
         Update course advanced settings by adding `ai_coach` as shown in below image
         
-        ![Update settings image](./docs/images/update-settings.png)
+        ![Update settings image](https://github.com/edly-io/ai-coach-xblock/blob/main/docs/images/update-settings.png?raw=True)
         
         ### **Update settings of AI Coach Component**
         
         AI Coach Xblock will be available in Advanced component of course unit now. Add "AI Coach" xblock in unit and click "Edit" button to
         add `question` & `question context` and configure it.
         
         > `Context` is the context of question with answer which is provided to OpenAI for feedback generation. Question and Learner Answer is integrated into context using `{{question}}` and `{{answer}}` keywords which automatically picks question & learner aswer value. 
         > Example: 
         ```I am grade 8 student studying leadership. My teacher asked me question: {{question}} . I answered {{answer}} . Provide two tips to improve my answer as a grade 8 student. ```   
         
         
-        ![Configure AI Coach XBlock Image](./docs/images/configure-ai-coach.png)
+        ![Configure AI Coach XBlock Image](https://github.com/edly-io/ai-coach-xblock/blob/main/docs/images/configure-ai-coach.png?raw=True)
         
         
         ### **Publish Content**
         
         Use "Preview" button to preview it or publish your content and use "View Live Version" button to see how it appears on LMS
         
-        ![Preview Live XBlock](./docs/images/ai-coach-preview.png)
+        ![Preview Live XBlock](https://github.com/edly-io/ai-coach-xblock/blob/main/docs/images/ai-coach-preview.png?raw=True)
         
         
         ### **Ask For Feedback**
         
         After adding answer, learner click on `Ask from Coach` button for feedback. Feedback is provided by OPEN AI on the basis of question context and answer. 
         
         > "**Ask from Coach**" button disappears when the feedback threshold (Maximum no. of times one can request for feedback) is reached. By default, feedback threshold is 1.
         
-        ![Ask from Coach](./docs/images/ask-from-coach.png)
+        ![Ask from Coach](https://github.com/edly-io/ai-coach-xblock/blob/main/docs/images/ask-from-coach.png?raw=True)
         
         
         
         ### **Submitting Answer**
         
         Submit button saves the learner answer and mark the completion of Xblock.
         
-        ![Submit Answer](./docs/images/submit-answer.png)
-        ![Xblock Completion](./docs/images/xblock-completion.png)
+        ![Submit Answer](https://github.com/edly-io/ai-coach-xblock/blob/main/docs/images/submit-answer.png?raw=True)
+        ![Xblock Completion](https://github.com/edly-io/ai-coach-xblock/blob/main/docs/images/xblock-completion.png?raw=True)
         
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `ai-coach-xblock-1.0.0/setup.py` & `ai-coach-xblock-1.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
                 data.append(os.path.relpath(os.path.join(dirname, fname), pkg))
 
     return {pkg: data}
 
 
 setup(
     name='ai-coach-xblock',
-    version='1.0.0',
+    version='1.0.1',
     description="AI Coach Xblock evaluates open response answer of a question using Open AI",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/edly-io/ai-feedback-xblock',
     license='AGPL v3',
     author='edly',
     packages=[
```

