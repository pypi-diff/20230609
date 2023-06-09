# Comparing `tmp/recon_lw-2.0.0.dev5152737981.tar.gz` & `tmp/recon_lw-2.0.0.dev5222319522.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev5152737981.tar", last modified: Fri Jun  2 06:56:35 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev5222319522.tar", last modified: Fri Jun  9 13:17:45 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev5152737981.tar` & `recon_lw-2.0.0.dev5222319522.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 06:56:35.000000 recon_lw-2.0.0.dev5152737981/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-02 06:55:51.000000 recon_lw-2.0.0.dev5152737981/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-02 06:56:35.000000 recon_lw-2.0.0.dev5152737981/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-02 06:55:51.000000 recon_lw-2.0.0.dev5152737981/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-02 06:56:16.000000 recon_lw-2.0.0.dev5152737981/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 06:56:35.000000 recon_lw-2.0.0.dev5152737981/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-06-02 06:55:51.000000 recon_lw-2.0.0.dev5152737981/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)     1096 2023-06-02 06:55:51.000000 recon_lw-2.0.0.dev5152737981/recon_lw/LastStateMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-06-02 06:55:51.000000 recon_lw-2.0.0.dev5152737981/recon_lw/LiveObjectsCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-06-02 06:55:51.000000 recon_lw-2.0.0.dev5152737981/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-02 06:55:51.000000 recon_lw-2.0.0.dev5152737981/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13270 2023-06-02 06:55:51.000000 recon_lw-2.0.0.dev5152737981/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    32667 2023-06-02 06:55:51.000000 recon_lw-2.0.0.dev5152737981/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    22335 2023-06-02 06:55:51.000000 recon_lw-2.0.0.dev5152737981/recon_lw/recon_ob_cross_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 06:56:35.000000 recon_lw-2.0.0.dev5152737981/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-02 06:56:35.000000 recon_lw-2.0.0.dev5152737981/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      454 2023-06-02 06:56:35.000000 recon_lw-2.0.0.dev5152737981/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-02 06:56:35.000000 recon_lw-2.0.0.dev5152737981/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-06-02 06:56:35.000000 recon_lw-2.0.0.dev5152737981/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-02 06:56:35.000000 recon_lw-2.0.0.dev5152737981/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-06-02 06:55:51.000000 recon_lw-2.0.0.dev5152737981/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-02 06:56:35.000000 recon_lw-2.0.0.dev5152737981/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-06-02 06:55:51.000000 recon_lw-2.0.0.dev5152737981/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 06:56:35.000000 recon_lw-2.0.0.dev5152737981/test/
--rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-06-02 06:55:51.000000 recon_lw-2.0.0.dev5152737981/test/test_recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 13:17:45.000000 recon_lw-2.0.0.dev5222319522/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-09 13:17:03.000000 recon_lw-2.0.0.dev5222319522/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-09 13:17:45.000000 recon_lw-2.0.0.dev5222319522/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-09 13:17:03.000000 recon_lw-2.0.0.dev5222319522/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-09 13:17:27.000000 recon_lw-2.0.0.dev5222319522/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 13:17:45.000000 recon_lw-2.0.0.dev5222319522/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-06-09 13:17:03.000000 recon_lw-2.0.0.dev5222319522/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1096 2023-06-09 13:17:03.000000 recon_lw-2.0.0.dev5222319522/recon_lw/LastStateMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-06-09 13:17:03.000000 recon_lw-2.0.0.dev5222319522/recon_lw/LiveObjectsCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-06-09 13:17:03.000000 recon_lw-2.0.0.dev5222319522/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-09 13:17:03.000000 recon_lw-2.0.0.dev5222319522/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13270 2023-06-09 13:17:03.000000 recon_lw-2.0.0.dev5222319522/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32791 2023-06-09 13:17:03.000000 recon_lw-2.0.0.dev5222319522/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22335 2023-06-09 13:17:03.000000 recon_lw-2.0.0.dev5222319522/recon_lw/recon_ob_cross_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 13:17:45.000000 recon_lw-2.0.0.dev5222319522/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-09 13:17:45.000000 recon_lw-2.0.0.dev5222319522/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      454 2023-06-09 13:17:45.000000 recon_lw-2.0.0.dev5222319522/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-09 13:17:45.000000 recon_lw-2.0.0.dev5222319522/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-06-09 13:17:45.000000 recon_lw-2.0.0.dev5222319522/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-09 13:17:45.000000 recon_lw-2.0.0.dev5222319522/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-06-09 13:17:03.000000 recon_lw-2.0.0.dev5222319522/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-09 13:17:45.000000 recon_lw-2.0.0.dev5222319522/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-06-09 13:17:03.000000 recon_lw-2.0.0.dev5222319522/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 13:17:45.000000 recon_lw-2.0.0.dev5222319522/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-06-09 13:17:03.000000 recon_lw-2.0.0.dev5222319522/test/test_recon_ob.py
```

### Comparing `recon_lw-2.0.0.dev5152737981/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev5222319522/recon_lw/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5152737981/recon_lw/LastStateMatcher.py` & `recon_lw-2.0.0.dev5222319522/recon_lw/LastStateMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5152737981/recon_lw/LiveObjectsCache.py` & `recon_lw-2.0.0.dev5222319522/recon_lw/LiveObjectsCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5152737981/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev5222319522/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5152737981/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev5222319522/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5152737981/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev5222319522/recon_lw/recon_ob.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,14 +102,15 @@
             book["v"] += 1
 
         if len(result) > 0:
             result["operation"] = operation.__name__
             result["operation_params"] = initial_parameters
             result["initial_book"] = initial_book
             result["book_id"] = book_id
+            result["sessionId"] = mess["sessionId"]
             update_event = recon_lw.create_event("UpdateBookError:" + parent_event["eventName"], "UpdateBookError",
                                                  event_sequence,
                                                  ok=False,
                                                  body=result,
                                                  parentId=parent_event["eventId"])
             update_event["attachedMessageIds"] = [mess["messageId"]]
             events.append(update_event)
@@ -198,15 +199,15 @@
 def process_market_data_update(mess_batch, events,  books_cache, get_book_id_func ,update_book_rule,
                                check_book_rule, event_sequence, parent_event, initial_book_params, log_books_filter,
                                log_books_collection, aggregate_batch_updates):
     books_updates = {}
     for m in mess_batch:
         book_ids_list, result = get_book_id_func(m)
         if result is not None:
-            book_id_event = recon_lw.create_event("GetBookEroor:" + parent_event["eventName"], "GetBookEroor",
+            book_id_event = recon_lw.create_event("GetBookError:" + parent_event["eventName"], "GetBookError",
                                                   event_sequence,
                                                   ok=False,
                                                   body=result,
                                                   parentId=parent_event["eventId"])
             book_id_event["attachedMessageIds"] = [m["messageId"]]
             events.append(book_id_event)
         if book_ids_list is not None:
@@ -245,15 +246,15 @@
     log_books_collection = []
     for m in sequenced_batch:
         seq = m[0]
         mess = m[1]
         # process gaps
         if "gap" in mess:
             gap_event = recon_lw.create_event("SeqGap:" + parent_event["eventName"], "SeqGap", event_sequence, ok=False,
-                                              body={"seq_num": seq}, parentId=parent_event["eventId"])
+                                              body={"seq_num": seq, "sessionId":mess['sessionId']}, parentId=parent_event["eventId"])
             events.append(gap_event)
             n_processed += 1
             continue
         messages_chunk.extend(message_utils.expand_message(mess))
         n_processed += 1
 
     process_market_data_update(messages_chunk, events, books_cache, get_book_id_func, update_book_rule,
@@ -313,15 +314,15 @@
     n_dupl = len(duplicates)
     dupl_events = []
     for i in range(0, n_dupl):
         item = duplicates.pop(0)
         d_ev = recon_lw.create_event("Duplicate:" + rule_settings["rule_root_event"]["eventName"], "Duplicate",
                                      event_sequence,
                                      ok=False,
-                                     body={"seq_num": item[0]},
+                                     body={"seq_num": item[0], "sessionId": rule_settings["sessionId"]},
                                      parentId=rule_settings["rule_root_event"]["eventId"])
         d_ev["attachedMessageIds"] = [item[1], item[2]]
         dupl_events.append(d_ev)
     save_events_func(dupl_events)
     duplicates.clear()
     flush_sequence_clear_cache(n_processed, rule_settings["sequence_cache"])
```

### Comparing `recon_lw-2.0.0.dev5152737981/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev5222319522/recon_lw/recon_ob_cross_stream.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5152737981/setup.py` & `recon_lw-2.0.0.dev5222319522/setup.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5152737981/test/test_recon_ob.py` & `recon_lw-2.0.0.dev5222319522/test/test_recon_ob.py`

 * *Files identical despite different names*

