# Comparing `tmp/agixt-1.2.0b0.tar.gz` & `tmp/agixt-1.2.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agixt-1.2.0b0.tar", max compression
+gzip compressed data, was "agixt-1.2.1b0.tar", max compression
```

## Comparing `agixt-1.2.0b0.tar` & `agixt-1.2.1b0.tar`

### file list

```diff
@@ -1,93 +1,97 @@
--rw-r--r--   0        0        0     1087 2023-06-08 01:05:47.963231 agixt-1.2.0b0/LICENSE
--rw-r--r--   0        0        0    19409 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/AGiXT.py
--rw-r--r--   0        0        0    23585 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/Agent.py
--rw-r--r--   0        0        0    10083 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/Chain.py
--rw-r--r--   0        0        0     1099 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/Config.py
--rw-r--r--   0        0        0     5900 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/Embedding.py
--rw-r--r--   0        0        0     6784 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/Extensions.py
--rw-r--r--   0        0        0     9489 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/Memories.py
--rw-r--r--   0        0        0     1986 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/Prompts.py
--rw-r--r--   0        0        0     7093 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/Tasks.py
--rw-r--r--   0        0        0       38 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/WORKSPACE/example.txt
--rw-r--r--   0        0        0      230 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/__init__.py
--rw-r--r--   0        0        0      244 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/agents/gpt4free/config.json
--rw-r--r--   0        0        0    17684 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/app.py
--rw-r--r--   0        0        0     2012 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/chains/Smart Chat.json
--rw-r--r--   0        0        0     7108 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/chains/Test_Commands.json
--rw-r--r--   0        0        0     1030 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/chains/Write a Poem.json
--rw-r--r--   0        0        0    11935 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/example.ipynb
--rw-r--r--   0        0        0     7807 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/extensions/agixt_agent.py
--rw-r--r--   0        0        0      860 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/extensions/briantts.py
--rw-r--r--   0        0        0     1174 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/extensions/dalle.py
--rw-r--r--   0        0        0     2818 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/extensions/discord.py
--rw-r--r--   0        0        0     1170 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/extensions/elevenlabs.py
--rw-r--r--   0        0        0     6647 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/extensions/file_system.py
--rw-r--r--   0        0        0     1841 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/extensions/github.py
--rw-r--r--   0        0        0     2042 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/extensions/google.py
--rw-r--r--   0        0        0      539 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/extensions/gtts.py
--rw-r--r--   0        0        0     2475 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/extensions/huggingface.py
--rw-r--r--   0        0        0      622 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/extensions/macostts.py
--rw-r--r--   0        0        0     4236 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/extensions/microsoft_365.py
--rw-r--r--   0        0        0     1899 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/extensions/searxng.py
--rw-r--r--   0        0        0     1001 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/extensions/sendgrid_email.py
--rw-r--r--   0        0        0      315 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/extensions/times.py
--rw-r--r--   0        0        0     1169 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/extensions/twitter.py
--rw-r--r--   0        0        0     2287 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/extensions/web_playwright.py
--rw-r--r--   0        0        0      151 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/Chat.txt
--rw-r--r--   0        0        0      181 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/Check-Instruction.txt
--rw-r--r--   0        0        0      991 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/Create New Command.txt
--rw-r--r--   0        0        0     1017 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/Execution.txt
--rw-r--r--   0        0        0     1178 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/Instruction.txt
--rw-r--r--   0        0        0      378 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/JSONFormatter.txt
--rw-r--r--   0        0        0      170 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/Pick a Poem Subject.txt
--rw-r--r--   0        0        0      430 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/Pick-a-Link.txt
--rw-r--r--   0        0        0      326 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/Prioritize.txt
--rw-r--r--   0        0        0      236 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/Pseudo Code.txt
--rw-r--r--   0        0        0      270 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/Score Response.txt
--rw-r--r--   0        0        0      349 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/SmartChat-CleanResponse.txt
--rw-r--r--   0        0        0      274 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/SmartChat-Researcher.txt
--rw-r--r--   0        0        0      304 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/SmartChat-Resolver.txt
--rw-r--r--   0        0        0      148 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/SmartChat-StepByStep.txt
--rw-r--r--   0        0        0      474 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/SmartInstruct-CleanResponse.txt
--rw-r--r--   0        0        0      528 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/SmartInstruct-Execution.txt
--rw-r--r--   0        0        0      458 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/SmartInstruct-Researcher.txt
--rw-r--r--   0        0        0      433 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/SmartInstruct-Resolver.txt
--rw-r--r--   0        0        0      160 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/SmartInstruct-StepByStep.txt
--rw-r--r--   0        0        0      507 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/SmartTask-CleanResponse.txt
--rw-r--r--   0        0        0      560 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/SmartTask-Execution.txt
--rw-r--r--   0        0        0      192 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/SmartTask-StepByStep.txt
--rw-r--r--   0        0        0      162 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/Tell Me How.txt
--rw-r--r--   0        0        0      162 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/Title a Poem.txt
--rw-r--r--   0        0        0      308 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/Validation.txt
--rw-r--r--   0        0        0      856 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/ValidationFailed.txt
--rw-r--r--   0        0        0      314 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/WebSearch.txt
--rw-r--r--   0        0        0       43 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/Write a Haiku.txt
--rw-r--r--   0        0        0       43 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/Write a Poem.txt
--rw-r--r--   0        0        0     1178 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/gpt-3.5-turbo/instruct.txt
--rw-r--r--   0        0        0     1178 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/gpt-4/instruct.txt
--rw-r--r--   0        0        0      777 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/instruct.txt
--rw-r--r--   0        0        0      824 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/starchat/instruct.txt
--rw-r--r--   0        0        0      616 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/prompts/vicuna/instruct.txt
--rw-r--r--   0        0        0     2329 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/provider/__init__.py
--rw-r--r--   0        0        0     1729 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/provider/azure.py
--rw-r--r--   0        0        0      493 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/provider/bard.py
--rw-r--r--   0        0        0     1638 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/provider/bing.py
--rw-r--r--   0        0        0      980 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/provider/chatgpt.py
--rw-r--r--   0        0        0     1012 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/provider/claude.py
--rw-r--r--   0        0        0      763 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/provider/fastchat.py
--rw-r--r--   0        0        0      873 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/provider/gpt4all.py
--rw-r--r--   0        0        0     5430 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/provider/gpt4free.py
--rw-r--r--   0        0        0     1194 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/provider/gpugpt4all.py
--rw-r--r--   0        0        0     1007 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/provider/huggingchat.py
--rw-r--r--   0        0        0     1438 2023-06-08 01:05:47.967231 agixt-1.2.0b0/agixt/provider/huggingface.py
--rw-r--r--   0        0        0     1091 2023-06-08 01:05:47.971231 agixt-1.2.0b0/agixt/provider/kobold.py
--rw-r--r--   0        0        0     2048 2023-06-08 01:05:47.971231 agixt-1.2.0b0/agixt/provider/llamacpp.py
--rw-r--r--   0        0        0     1071 2023-06-08 01:05:47.971231 agixt-1.2.0b0/agixt/provider/llamacppapi.py
--rw-r--r--   0        0        0     1585 2023-06-08 01:05:47.971231 agixt-1.2.0b0/agixt/provider/oobabooga.py
--rw-r--r--   0        0        0     1597 2023-06-08 01:05:47.971231 agixt-1.2.0b0/agixt/provider/openai.py
--rw-r--r--   0        0        0      850 2023-06-08 01:05:47.971231 agixt-1.2.0b0/agixt/provider/palm.py
--rw-r--r--   0        0        0     3730 2023-06-08 01:05:47.971231 agixt-1.2.0b0/agixt/provider/runpod.py
--rw-r--r--   0        0        0     3106 2023-06-08 01:05:47.971231 agixt-1.2.0b0/agixt/provider/transformer.py
--rw-r--r--   0        0        0    11848 2023-06-08 01:05:47.971231 agixt-1.2.0b0/docs/README.md
--rw-r--r--   0        0        0     2786 2023-06-08 01:05:47.983232 agixt-1.2.0b0/pyproject.toml
--rw-r--r--   0        0        0    14784 1970-01-01 00:00:00.000000 agixt-1.2.0b0/PKG-INFO
+-rw-r--r--   0        0        0     1087 2023-06-09 02:39:17.188328 agixt-1.2.1b0/LICENSE
+-rw-r--r--   0        0        0    19409 2023-06-09 02:39:17.188328 agixt-1.2.1b0/agixt/AGiXT.py
+-rw-r--r--   0        0        0    23585 2023-06-09 02:39:17.188328 agixt-1.2.1b0/agixt/Agent.py
+-rw-r--r--   0        0        0    10816 2023-06-09 02:39:17.188328 agixt-1.2.1b0/agixt/Chain.py
+-rw-r--r--   0        0        0     1099 2023-06-09 02:39:17.188328 agixt-1.2.1b0/agixt/Config.py
+-rw-r--r--   0        0        0     5900 2023-06-09 02:39:17.188328 agixt-1.2.1b0/agixt/Embedding.py
+-rw-r--r--   0        0        0     6784 2023-06-09 02:39:17.188328 agixt-1.2.1b0/agixt/Extensions.py
+-rw-r--r--   0        0        0     9489 2023-06-09 02:39:17.188328 agixt-1.2.1b0/agixt/Memories.py
+-rw-r--r--   0        0        0     1986 2023-06-09 02:39:17.188328 agixt-1.2.1b0/agixt/Prompts.py
+-rw-r--r--   0        0        0       38 2023-06-09 02:39:17.188328 agixt-1.2.1b0/agixt/WORKSPACE/example.txt
+-rw-r--r--   0        0        0      230 2023-06-09 02:39:17.188328 agixt-1.2.1b0/agixt/__init__.py
+-rw-r--r--   0        0        0      209 2023-06-09 02:39:17.188328 agixt-1.2.1b0/agixt/agents/gpt4free/config.json
+-rw-r--r--   0        0        0    16006 2023-06-09 02:39:17.188328 agixt-1.2.1b0/agixt/app.py
+-rw-r--r--   0        0        0     1839 2023-06-09 02:39:17.188328 agixt-1.2.1b0/agixt/chains/Poem Writing Chain/responses.json
+-rw-r--r--   0        0        0     1126 2023-06-09 02:39:17.188328 agixt-1.2.1b0/agixt/chains/Smart Chat.json
+-rw-r--r--   0        0        0     1142 2023-06-09 02:39:17.188328 agixt-1.2.1b0/agixt/chains/Smart Instruct.json
+-rw-r--r--   0        0        0      744 2023-06-09 02:39:17.188328 agixt-1.2.1b0/agixt/chains/Task.json
+-rw-r--r--   0        0        0     7108 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/chains/Test_Commands.json
+-rw-r--r--   0        0        0     1030 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/chains/Write a Poem.json
+-rw-r--r--   0        0        0    11935 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/example.ipynb
+-rw-r--r--   0        0        0     8806 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/extensions/agixt_agent.py
+-rw-r--r--   0        0        0      860 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/extensions/briantts.py
+-rw-r--r--   0        0        0     1174 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/extensions/dalle.py
+-rw-r--r--   0        0        0     2818 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/extensions/discord.py
+-rw-r--r--   0        0        0     1170 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/extensions/elevenlabs.py
+-rw-r--r--   0        0        0     6647 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/extensions/file_system.py
+-rw-r--r--   0        0        0     1841 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/extensions/github.py
+-rw-r--r--   0        0        0     2042 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/extensions/google.py
+-rw-r--r--   0        0        0      539 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/extensions/gtts.py
+-rw-r--r--   0        0        0     2475 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/extensions/huggingface.py
+-rw-r--r--   0        0        0      622 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/extensions/macostts.py
+-rw-r--r--   0        0        0     4236 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/extensions/microsoft_365.py
+-rw-r--r--   0        0        0     1899 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/extensions/searxng.py
+-rw-r--r--   0        0        0     1001 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/extensions/sendgrid_email.py
+-rw-r--r--   0        0        0      315 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/extensions/times.py
+-rw-r--r--   0        0        0     1169 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/extensions/twitter.py
+-rw-r--r--   0        0        0     2287 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/extensions/web_playwright.py
+-rw-r--r--   0        0        0      151 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/Chat.txt
+-rw-r--r--   0        0        0      181 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/Check-Instruction.txt
+-rw-r--r--   0        0        0      991 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/Create New Command.txt
+-rw-r--r--   0        0        0     1017 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/Execution.txt
+-rw-r--r--   0        0        0      396 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/Get Task List.txt
+-rw-r--r--   0        0        0     1178 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/Instruction.txt
+-rw-r--r--   0        0        0      378 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/JSONFormatter.txt
+-rw-r--r--   0        0        0      170 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/Pick a Poem Subject.txt
+-rw-r--r--   0        0        0      430 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/Pick-a-Link.txt
+-rw-r--r--   0        0        0      326 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/Prioritize.txt
+-rw-r--r--   0        0        0      236 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/Pseudo Code.txt
+-rw-r--r--   0        0        0      270 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/Score Response.txt
+-rw-r--r--   0        0        0      349 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/SmartChat-CleanResponse.txt
+-rw-r--r--   0        0        0      268 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/SmartChat-Researcher.txt
+-rw-r--r--   0        0        0      298 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/SmartChat-Resolver.txt
+-rw-r--r--   0        0        0      148 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/SmartChat-StepByStep.txt
+-rw-r--r--   0        0        0      474 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/SmartInstruct-CleanResponse.txt
+-rw-r--r--   0        0        0      528 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/SmartInstruct-Execution.txt
+-rw-r--r--   0        0        0      452 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/SmartInstruct-Researcher.txt
+-rw-r--r--   0        0        0      427 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/SmartInstruct-Resolver.txt
+-rw-r--r--   0        0        0      160 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/SmartInstruct-StepByStep.txt
+-rw-r--r--   0        0        0      507 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/SmartTask-CleanResponse.txt
+-rw-r--r--   0        0        0      560 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/SmartTask-Execution.txt
+-rw-r--r--   0        0        0      192 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/SmartTask-StepByStep.txt
+-rw-r--r--   0        0        0      836 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/Task Execution.txt
+-rw-r--r--   0        0        0      162 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/Tell Me How.txt
+-rw-r--r--   0        0        0      162 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/Title a Poem.txt
+-rw-r--r--   0        0        0      308 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/Validation.txt
+-rw-r--r--   0        0        0      856 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/ValidationFailed.txt
+-rw-r--r--   0        0        0      314 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/WebSearch.txt
+-rw-r--r--   0        0        0       43 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/Write a Haiku.txt
+-rw-r--r--   0        0        0       43 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/Write a Poem.txt
+-rw-r--r--   0        0        0     1178 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/gpt-3.5-turbo/instruct.txt
+-rw-r--r--   0        0        0     1178 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/gpt-4/instruct.txt
+-rw-r--r--   0        0        0      777 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/instruct.txt
+-rw-r--r--   0        0        0      824 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/starchat/instruct.txt
+-rw-r--r--   0        0        0      616 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/prompts/vicuna/instruct.txt
+-rw-r--r--   0        0        0     2329 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/provider/__init__.py
+-rw-r--r--   0        0        0     1729 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/provider/azure.py
+-rw-r--r--   0        0        0      493 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/provider/bard.py
+-rw-r--r--   0        0        0     1638 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/provider/bing.py
+-rw-r--r--   0        0        0      980 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/provider/chatgpt.py
+-rw-r--r--   0        0        0     1012 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/provider/claude.py
+-rw-r--r--   0        0        0      763 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/provider/fastchat.py
+-rw-r--r--   0        0        0      873 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/provider/gpt4all.py
+-rw-r--r--   0        0        0     5430 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/provider/gpt4free.py
+-rw-r--r--   0        0        0     1194 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/provider/gpugpt4all.py
+-rw-r--r--   0        0        0     1007 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/provider/huggingchat.py
+-rw-r--r--   0        0        0     1438 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/provider/huggingface.py
+-rw-r--r--   0        0        0     1091 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/provider/kobold.py
+-rw-r--r--   0        0        0     2048 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/provider/llamacpp.py
+-rw-r--r--   0        0        0     1071 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/provider/llamacppapi.py
+-rw-r--r--   0        0        0     1585 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/provider/oobabooga.py
+-rw-r--r--   0        0        0     1597 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/provider/openai.py
+-rw-r--r--   0        0        0      850 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/provider/palm.py
+-rw-r--r--   0        0        0     3730 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/provider/runpod.py
+-rw-r--r--   0        0        0     3106 2023-06-09 02:39:17.192328 agixt-1.2.1b0/agixt/provider/transformer.py
+-rw-r--r--   0        0        0    11862 2023-06-09 02:39:17.192328 agixt-1.2.1b0/docs/README.md
+-rw-r--r--   0        0        0     2786 2023-06-09 02:39:17.204328 agixt-1.2.1b0/pyproject.toml
+-rw-r--r--   0        0        0    14798 1970-01-01 00:00:00.000000 agixt-1.2.1b0/PKG-INFO
```

### Comparing `agixt-1.2.0b0/LICENSE` & `agixt-1.2.1b0/LICENSE`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0b0/agixt/AGiXT.py` & `agixt-1.2.1b0/agixt/AGiXT.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0b0/agixt/Agent.py` & `agixt-1.2.1b0/agixt/Agent.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0b0/agixt/Chain.py` & `agixt-1.2.1b0/agixt/Chain.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 import os
 import json
 from AGiXT import AGiXT
 import argparse
 from Extensions import Extensions
 import logging
+from datetime import datetime
 
 
 class Chain:
     def get_chain(self, chain_name):
+        # if chain/{chain_name}/ exists and create the folder if it does not
+        if not os.path.exists(os.path.join("chains", chain_name)):
+            os.mkdir(os.path.join("chains", chain_name))
         with open(os.path.join("chains", f"{chain_name}.json"), "r") as f:
             chain_data = json.load(f)
         return chain_data
 
     def get_chains(self):
         chains = [
             f.replace(".json", "") for f in os.listdir("chains") if f.endswith(".json")
@@ -114,46 +118,49 @@
                 logging.info(f"Running step {step_data['step']}")
                 step_response = await self.run_chain_step(
                     step=step_data, chain_name=chain_name, user_input=user_input
                 )  # Get the response of the current step.
                 responses[step_data["step"]] = step_response  # Store the response.
                 logging.info(f"Response: {step_response}")
                 # Write the responses to the json file.
+                dt = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
                 with open(
-                    os.path.join("chains", f"{chain_name}_responses.json"), "w"
+                    os.path.join("chains", chain_name, "responses.json"), "w"
                 ) as f:
                     json.dump(responses, f)
         return responses
 
     def get_step_response(self, chain_name, step_number="all"):
         try:
-            with open(os.path.join("chains", f"{chain_name}_responses.json"), "r") as f:
+            with open(os.path.join("chains", chain_name, "responses.json"), "r") as f:
                 responses = json.load(f)
             print(responses)
             if step_number == "all":
                 return responses
             else:
                 return responses.get(str(step_number))
         except:
             return ""
 
     def get_chain_responses(self, chain_name):
         try:
-            with open(os.path.join("chains", f"{chain_name}_responses.json"), "r") as f:
+            with open(os.path.join("chains", chain_name, "responses.json"), "r") as f:
                 responses = json.load(f)
             return responses
         except:
             return {}
 
-    def get_step_content(self, chain_name, prompt_content, user_input):
+    def get_step_content(self, chain_name, prompt_content, user_input, agent_name):
         new_prompt_content = {}
         if isinstance(prompt_content, dict):
             for arg, value in prompt_content.items():
                 if "{user_input}" in value:
                     value = value.replace("{user_input}", user_input)
+                if "{agent_name}" in value:
+                    value = value.replace("{agent_name}", agent_name)
                 if "{STEP" in value:
                     # Count how many times {STEP is in the value
                     step_count = value.count("{STEP")
                     for i in range(step_count):
                         # Get the step number from value between {STEP and }
                         new_step_number = int(value.split("{STEP")[1].split("}")[0])
                         # get the response from the step number
@@ -162,16 +169,23 @@
                         )
                         # replace the {STEPx} with the response
                         value = value.replace(
                             f"{{STEP{new_step_number}}}", step_response
                         )
                 new_prompt_content[arg] = value
         elif isinstance(prompt_content, str):
+            new_prompt_content = prompt_content
             if "{user_input}" in prompt_content:
-                new_prompt_content = prompt_content.replace("{user_input}", user_input)
+                new_prompt_content = new_prompt_content.replace(
+                    "{user_input}", user_input
+                )
+            if "{agent_name}" in new_prompt_content:
+                new_prompt_content = new_prompt_content.replace(
+                    "{agent_name}", agent_name
+                )
             if "{STEP" in prompt_content:
                 step_count = value.count("{STEP")
                 for i in range(step_count):
                     # Get the step number from value between {STEP and }
                     new_step_number = int(
                         prompt_content.split("{STEP")[1].split("}")[0]
                     )
@@ -199,14 +213,15 @@
                     prompt_name = step["prompt"]["prompt_name"]
                 else:
                     prompt_name = ""
                 args = self.get_step_content(
                     chain_name=chain_name,
                     prompt_content=step["prompt"],
                     user_input=user_input,
+                    agent_name=agent_name,
                 )
                 if prompt_type == "Command":
                     return await Extensions(
                         agent_config=agent.agent.agent_config
                     ).execute_command(
                         command_name=args["command_name"], command_args=args
                     )
```

### Comparing `agixt-1.2.0b0/agixt/Config.py` & `agixt-1.2.1b0/agixt/Config.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0b0/agixt/Embedding.py` & `agixt-1.2.1b0/agixt/Embedding.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0b0/agixt/Extensions.py` & `agixt-1.2.1b0/agixt/Extensions.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0b0/agixt/Memories.py` & `agixt-1.2.1b0/agixt/Memories.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0b0/agixt/Prompts.py` & `agixt-1.2.1b0/agixt/Prompts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0b0/agixt/app.py` & `agixt-1.2.1b0/agixt/app.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from fastapi import FastAPI, HTTPException
 from fastapi.middleware.cors import CORSMiddleware
 from pydantic import BaseModel
 from Config import Config
 from AGiXT import AGiXT
 from Agent import Agent
 from Chain import Chain
-from Tasks import Tasks
 from Prompts import Prompts
 from typing import Optional, Dict, List, Any
 from provider import get_provider_options
 from Embedding import get_embedding_providers
 from Extensions import Extensions
 import os
 import logging
@@ -337,63 +336,14 @@
         logging.info(e)
         raise HTTPException(
             status_code=500,
             detail=f"Error enabling all commands for agent '{agent_name}': {str(e)}",
         )
 
 
-@app.post("/api/agent/{agent_name}/task", tags=["Agent"])
-async def start_task_agent(agent_name: str, objective: Objective) -> ResponseMessage:
-    task = Tasks(agent_name=agent_name)
-    # If it's running stop it.
-    task_status = task.get_status()
-    if task_status != False:
-        task.stop_tasks()
-        return ResponseMessage(message="Task agent stopped")
-    # If it's not running start it.
-    try:
-        asyncio.create_task(task.run_task(objective=objective.objective))
-        return ResponseMessage(message="Task agent started")
-    except Exception as e:
-        raise HTTPException(
-            status_code=500, detail="Error occurred while starting the task"
-        )
-
-
-# Get tasks Tasks(agent_name=agent_name).get_tasks()
-@app.get("/api/agent/{agent_name}/tasks", tags=["Agent"])
-async def get_tasks(agent_name: str) -> Dict[str, List[str]]:
-    tasks = Tasks(agent_name=agent_name).get_tasks()
-    return {"tasks": tasks}
-
-
-@app.get("/api/agent/{agent_name}/task", tags=["Agent"])
-async def get_task_output(agent_name: str) -> TaskOutput:
-    try:
-        task_output = Tasks(agent_name=agent_name).get_task_output()
-    except:
-        task_output = False
-    if task_output != False:
-        return TaskOutput(
-            output=task_output,
-            message="Task agent is not running",
-        )
-    else:
-        return TaskOutput(
-            output="",
-            message="Task agent is not running",
-        )
-
-
-@app.get("/api/agent/{agent_name}/task/status", tags=["Agent"])
-async def get_task_status(agent_name: str):
-    task_status = Tasks(agent_name=agent_name).get_status()
-    return {"status": task_status}
-
-
 @app.get("/api/chain", tags=["Chain"])
 async def get_chains():
     chains = Chain().get_chains()
     return chains
 
 
 @app.get("/api/chain/{chain_name}", tags=["Chain"])
```

### Comparing `agixt-1.2.0b0/agixt/chains/Test_Commands.json` & `agixt-1.2.1b0/agixt/chains/Test_Commands.json`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0b0/agixt/chains/Write a Poem.json` & `agixt-1.2.1b0/agixt/chains/Write a Poem.json`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0b0/agixt/example.ipynb` & `agixt-1.2.1b0/agixt/example.ipynb`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0b0/agixt/extensions/agixt_agent.py` & `agixt-1.2.1b0/agixt/extensions/agixt_agent.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,14 +15,16 @@
             "Evaluate Code": self.evaluate_code,
             "Analyze Pull Request": self.analyze_pull_request,
             "Perform Automated Testing": self.perform_automated_testing,
             "Run CI-CD Pipeline": self.run_ci_cd_pipeline,
             "Improve Code": self.improve_code,
             "Write Tests": self.write_tests,
             "Create a new command": self.create_command,
+            "Execute Task List": self.execute_task_list,
+            "Prompt AI Agent": self.prompt_agent,
         }
         if agents != None:
             for agent in agents:
                 if "name" in agent:
                     name = f" AI Agent {agent['name']}"
                     self.commands.update(
                         {
@@ -38,132 +40,163 @@
                         {f"Run Chain: {chain['name']}": self.run_chain}
                     )
 
     def command_exists(self, file_name: str) -> bool:
         return os.path.exists(f"commands/{file_name}.py")
 
     async def create_command(
-        self, function_description: str, agent_name: str = "AGiXT"
+        self, function_description: str, agent: str = "AGiXT"
     ) -> List[str]:
         with open(f"prompts/Create New Command.txt", "r") as f:
             prompt = f.read()
         prompt = prompt.replace("{{NEW_FUNCTION_DESCRIPTION}}", function_description)
-        response = await AGiXT(agent_name=agent_name).run(user_input=prompt)
+        response = await AGiXT(agent_name=agent).run(user_input=prompt)
         file_name = response.split("class ")[1].split("(")[0]
         code = code.replace("```", "")
 
         if not self.command_exists(file_name):
             with open(f"commands/{file_name}.py", "w") as f:
                 f.write(code)
             return f"Created new command: {file_name}."
         else:
             return f"Command {file_name} already exists. No changes were made."
 
-    async def evaluate_code(self, code: str, agent_name: str = "AGiXT") -> List[str]:
+    async def evaluate_code(self, code: str, agent: str = "AGiXT") -> List[str]:
         args = [code]
         function_string = "def analyze_code(code: str) -> List[str]:"
         description_string = "Analyzes the given code and returns a list of suggestions for improvements."
         prompt = f"You are now the following python function: ```# {description_string}\n{function_string}```\n\nOnly respond with your `return` value. Args: {args}"
-        return await AGiXT(agent_name=agent_name).run(user_input=prompt)
+        return await AGiXT(agent_name=agent).run(user_input=prompt)
 
     async def analyze_pull_request(
-        self, pr_url: str, agent_name: str = "AGiXT"
+        self, pr_url: str, agent: str = "AGiXT"
     ) -> List[str]:
         args = [pr_url]
         function_string = "def analyze_pr(pr_url: str) -> List[str]:"
         description_string = "Analyzes the given pull request and returns a list of suggestions for improvements."
         prompt = f"You are now the following python function: ```# {description_string}\n{function_string}```\n\nOnly respond with your `return` value. Args: {args}"
-        return await AGiXT(agent_name=agent_name).run(user_input=prompt)
+        return await AGiXT(agent_name=agent).run(user_input=prompt)
 
     async def perform_automated_testing(
-        self, test_url: str, agent_name: str = "AGiXT"
+        self, test_url: str, agent: str = "AGiXT"
     ) -> List[str]:
         args = [test_url]
         function_string = "def perform_testing(test_url: str) -> List[str]:"
         description_string = "Performs automated testing using AI-driven tools and returns a list of test results."
         prompt = f"You are now the following python function: ```# {description_string}\n{function_string}```\n\nOnly respond with your `return` value. Args: {args}"
-        return await AGiXT(agent_name=agent_name).run(user_input=prompt)
+        return await AGiXT(agent_name=agent).run(user_input=prompt)
 
     async def improve_code(
-        self, suggestions: List[str], code: str, agent_name: str = "AGiXT"
+        self, suggestions: List[str], code: str, agent: str = "AGiXT"
     ) -> str:
         args = [json.dumps(suggestions), code]
         function_string = (
             "def generate_improved_code(suggestions: List[str], code: str) -> str:"
         )
         description_string = "Improves the provided code based on the suggestions provided, making no other changes."
         prompt = f"You are now the following python function: ```# {description_string}\n{function_string}```\n\nOnly respond with your `return` value. Args: {args}"
-        return await AGiXT(agent_name=agent_name).run(user_input=prompt)
+        return await AGiXT(agent_name=agent).run(user_input=prompt)
 
     async def write_tests(
         self,
         code: str,
         focus: Optional[List[str]] = None,
-        agent_name: str = "AGiXT",
+        agent: str = "AGiXT",
     ) -> str:
         args = [code, json.dumps(focus) if focus else "None"]
         function_string = "def create_test_cases(code: str, focus: Optional[List[str]] = None) -> str:"
         description_string = "Generates test cases for the existing code, focusing on specific areas if required."
         prompt = f"You are now the following python function: ```# {description_string}\n{function_string}```\n\nOnly respond with your `return` value. Args: {args}"
-        return await AGiXT(agent_name=agent_name).run(user_input=prompt)
+        return await AGiXT(agent_name=agent).run(user_input=prompt)
 
-    async def run_ci_cd_pipeline(self, repo_url: str, agent_name: str = "AGiXT") -> str:
+    async def run_ci_cd_pipeline(self, repo_url: str, agent: str = "AGiXT") -> str:
         args = [repo_url]
         function_string = "def run_pipeline(repo_url: str) -> str:"
         description_string = (
             "Runs the entire CI/CD pipeline for the given repository URL."
         )
         prompt = f"You are now the following python function: ```# {description_string}\n{function_string}```\n\nOnly respond with your `return` value. Args: {args}"
-        return await AGiXT(agent_name=agent_name).run(user_input=prompt)
+        return await AGiXT(agent_name=agent).run(user_input=prompt)
 
     async def run_chain(self, chain_name: str = "", user_input: str = ""):
         await Chain().run_chain(chain_name=chain_name, user_input=user_input)
         return "Chain started successfully."
 
-    async def ask(self, user_input: str, agent_name: str = "AGiXT") -> str:
-        response = await AGiXT(agent_name=agent_name).run(
+    async def ask(self, user_input: str, agent: str = "AGiXT") -> str:
+        response = await AGiXT(agent_name=agent).run(
             user_input=user_input, prompt="chat", websearch=True, websearch_depth=4
         )
         return response
 
-    async def instruct(self, user_input: str, agent_name: str = "AGiXT") -> str:
-        response = await AGiXT(agent_name=agent_name).run(
+    async def instruct(self, user_input: str, agent: str = "AGiXT") -> str:
+        response = await AGiXT(agent_name=agent).run(
             user_input=user_input, prompt="instruct", websearch=True, websearch_depth=8
         )
         return response
 
     async def prompt_agent(
-        agent_name: str,
+        agent: str,
         user_input: str,
         prompt_name: int,
         prompt_args: dict,
         websearch: bool = False,
         websearch_depth: int = 3,
         context_results: int = 5,
         shots: int = 1,
     ) -> str:
-        response = await AGiXT(agent_name=agent_name).run(
+        response = await AGiXT(agent_name=agent).run(
             user_input=user_input,
             prompt=prompt_name,
             prompt_args=prompt_args,
             websearch=websearch,
             websearch_depth=websearch_depth,
             context_results=context_results,
         )
         if shots > 1:
             responses = [response]
             for shot in range(shots - 1):
-                response = await AGiXT(agent_name=agent_name).run(
+                response = await AGiXT(agent_name=agent).run(
                     user_input=user_input,
                     prompt=prompt_name,
                     prompt_args=prompt_args,
                     context_results=context_results,
                 )
                 responses.append(response)
             # Join responses by "Response # <shot number>:" and return
             return "\n".join(
                 [
                     f"Response {shot + 1}:\n{response}"
                     for shot, response in enumerate(responses)
                 ]
             )
         return response
+
+    async def execute_task_list(
+        self,
+        agent: str,
+        tasks: str,
+        user_input: str,
+        websearch: bool = False,
+        websearch_depth: int = 3,
+        context_results: int = 5,
+    ):
+        task_list = tasks.split("\n")
+        task_list = [
+            task
+            for task in task_list
+            if task and task[0] in [str(i) for i in range(10)]
+        ]
+        responses = []
+        for task in task_list:
+            if "task_name" in task:
+                response = await AGiXT(agent_name=agent).run(
+                    user_input=user_input,
+                    prompt="Task Execution",
+                    prompt_args={
+                        "task": task["task_name"],
+                    },
+                    websearch=websearch,
+                    websearch_depth=websearch_depth,
+                    context_results=context_results,
+                )
+                responses.append(response)
+        return "\n".join(responses)
```

### Comparing `agixt-1.2.0b0/agixt/extensions/briantts.py` & `agixt-1.2.1b0/agixt/extensions/briantts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0b0/agixt/extensions/dalle.py` & `agixt-1.2.1b0/agixt/extensions/dalle.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0b0/agixt/extensions/discord.py` & `agixt-1.2.1b0/agixt/extensions/discord.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0b0/agixt/extensions/elevenlabs.py` & `agixt-1.2.1b0/agixt/extensions/elevenlabs.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0b0/agixt/extensions/file_system.py` & `agixt-1.2.1b0/agixt/extensions/file_system.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0b0/agixt/extensions/github.py` & `agixt-1.2.1b0/agixt/extensions/github.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0b0/agixt/extensions/google.py` & `agixt-1.2.1b0/agixt/extensions/google.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0b0/agixt/extensions/gtts.py` & `agixt-1.2.1b0/agixt/extensions/gtts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0b0/agixt/extensions/huggingface.py` & `agixt-1.2.1b0/agixt/extensions/huggingface.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0b0/agixt/extensions/macostts.py` & `agixt-1.2.1b0/agixt/extensions/macostts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0b0/agixt/extensions/microsoft_365.py` & `agixt-1.2.1b0/agixt/extensions/microsoft_365.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0b0/agixt/extensions/searxng.py` & `agixt-1.2.1b0/agixt/extensions/searxng.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0b0/agixt/extensions/sendgrid_email.py` & `agixt-1.2.1b0/agixt/extensions/sendgrid_email.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0b0/agixt/extensions/twitter.py` & `agixt-1.2.1b0/agixt/extensions/twitter.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0b0/agixt/extensions/web_playwright.py` & `agixt-1.2.1b0/agixt/extensions/web_playwright.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0b0/agixt/prompts/Create New Command.txt` & `agixt-1.2.1b0/agixt/prompts/Create New Command.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0b0/agixt/prompts/Execution.txt` & `agixt-1.2.1b0/agixt/prompts/Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0b0/agixt/prompts/Instruction.txt` & `agixt-1.2.1b0/agixt/prompts/Instruction.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0b0/agixt/prompts/SmartInstruct-Execution.txt` & `agixt-1.2.1b0/agixt/prompts/SmartInstruct-Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0b0/agixt/prompts/SmartTask-Execution.txt` & `agixt-1.2.1b0/agixt/prompts/SmartTask-Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0b0/agixt/prompts/ValidationFailed.txt` & `agixt-1.2.1b0/agixt/prompts/ValidationFailed.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0b0/agixt/prompts/gpt-3.5-turbo/instruct.txt` & `agixt-1.2.1b0/agixt/prompts/gpt-3.5-turbo/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0b0/agixt/prompts/gpt-4/instruct.txt` & `agixt-1.2.1b0/agixt/prompts/gpt-4/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0b0/agixt/prompts/instruct.txt` & `agixt-1.2.1b0/agixt/prompts/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0b0/agixt/prompts/starchat/instruct.txt` & `agixt-1.2.1b0/agixt/prompts/starchat/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0b0/agixt/prompts/vicuna/instruct.txt` & `agixt-1.2.1b0/agixt/prompts/vicuna/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0b0/agixt/provider/__init__.py` & `agixt-1.2.1b0/agixt/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0b0/agixt/provider/azure.py` & `agixt-1.2.1b0/agixt/provider/azure.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0b0/agixt/provider/bing.py` & `agixt-1.2.1b0/agixt/provider/bing.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0b0/agixt/provider/chatgpt.py` & `agixt-1.2.1b0/agixt/provider/chatgpt.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0b0/agixt/provider/claude.py` & `agixt-1.2.1b0/agixt/provider/claude.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0b0/agixt/provider/fastchat.py` & `agixt-1.2.1b0/agixt/provider/fastchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0b0/agixt/provider/gpt4all.py` & `agixt-1.2.1b0/agixt/provider/gpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0b0/agixt/provider/gpt4free.py` & `agixt-1.2.1b0/agixt/provider/gpt4free.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0b0/agixt/provider/gpugpt4all.py` & `agixt-1.2.1b0/agixt/provider/gpugpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0b0/agixt/provider/huggingchat.py` & `agixt-1.2.1b0/agixt/provider/huggingchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0b0/agixt/provider/huggingface.py` & `agixt-1.2.1b0/agixt/provider/huggingface.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0b0/agixt/provider/kobold.py` & `agixt-1.2.1b0/agixt/provider/kobold.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0b0/agixt/provider/llamacpp.py` & `agixt-1.2.1b0/agixt/provider/llamacpp.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0b0/agixt/provider/llamacppapi.py` & `agixt-1.2.1b0/agixt/provider/llamacppapi.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0b0/agixt/provider/oobabooga.py` & `agixt-1.2.1b0/agixt/provider/oobabooga.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0b0/agixt/provider/openai.py` & `agixt-1.2.1b0/agixt/provider/openai.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0b0/agixt/provider/palm.py` & `agixt-1.2.1b0/agixt/provider/palm.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0b0/agixt/provider/runpod.py` & `agixt-1.2.1b0/agixt/provider/runpod.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0b0/agixt/provider/transformer.py` & `agixt-1.2.1b0/agixt/provider/transformer.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.0b0/docs/README.md` & `agixt-1.2.1b0/docs/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![Contribute](https://img.shields.io/github/issues/Josh-XT/AGiXT/help%20wanted?color=purple&label=Quick%20Contribute%20Backend&logo=github&style=plastic)](https://github.com/Josh-XT/AGiXT/labels/help%20wanted) 
 [![GitHub](https://img.shields.io/badge/GitHub-NextJS_Front_End-grey?logo=github&style=plastic)](https://github.com/JamesonRGrieve/Agent-LLM-Frontend)
 
 
 [![Discord](https://img.shields.io/discord/1097720481970397356?label=Discord&logo=discord&logoColor=white&style=plastic&color=5865f2)](https://discord.gg/d3TkHRZcjD) 
 [![Twitter](https://img.shields.io/badge/Twitter-Follow_@Josh_XT-blue?logo=twitter&style=plastic)](https://twitter.com/Josh_XT) 
 
-[![Logo](images/AGiXT.svg)](https://josh-xt.github.io/AGiXT/)
+[![Logo](images/AGiXT-gradient-flat.svg)](https://josh-xt.github.io/AGiXT/)
 
 AGiXT is a dynamic Artificial Intelligence Automation Platform engineered to orchestrate efficient AI instruction management and task execution across a multitude of providers. Our solution infuses adaptive memory handling with a broad spectrum of commands to enhance AI's understanding and responsiveness, leading to improved task completion. The platform's smart features, like Smart Instruct and Smart Chat, seamlessly integrate web search, planning strategies, and conversation continuity, transforming the interaction between users and AI. By leveraging a powerful plugin system that includes web browsing and command execution, AGiXT stands as a versatile bridge between AI models and users. With an expanding roster of AI providers, code evaluation capabilities, comprehensive chain management, and platform interoperability, AGiXT is consistently evolving to drive a multitude of applications, affirming its place at the forefront of AI technology.
 
 Embracing the spirit of extremity in every facet of life, we introduce AGiXT. This advanced AI Automation Platform is our bold step towards the realization of Artificial General Intelligence (AGI). Seamlessly orchestrating instruction management and executing complex tasks across diverse AI providers, AGiXT combines adaptive memory, smart features, and a versatile plugin system to maximize AI potential. With our unwavering commitment to innovation, we're dedicated to pushing the boundaries of AI and bringing AGI closer to reality.
 
 ## Table of Contents 📖
```

### Comparing `agixt-1.2.0b0/pyproject.toml` & `agixt-1.2.1b0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AGiXT"
-version = "v1.2.0-beta"
+version = "v1.2.1-beta"
 description = "An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day."
 homepage = "https://AGiXT.com"
 documentation = "https://AGiXT.com"
 keywords = ["AI", "AGI", "Agent", "skynet"]
 license = "MIT"
 authors = ["Josh XT <josh@devxt.com>"]
 maintainers = [
```

### Comparing `agixt-1.2.0b0/PKG-INFO` & `agixt-1.2.1b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.2.0b0
+Version: 1.2.1b0
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Home-page: https://AGiXT.com
 License: MIT
 Keywords: AI,AGI,Agent,skynet
 Author: Josh XT
 Author-email: josh@devxt.com
 Maintainer: Josh XT
@@ -71,15 +71,15 @@
 [![Contribute](https://img.shields.io/github/issues/Josh-XT/AGiXT/help%20wanted?color=purple&label=Quick%20Contribute%20Backend&logo=github&style=plastic)](https://github.com/Josh-XT/AGiXT/labels/help%20wanted) 
 [![GitHub](https://img.shields.io/badge/GitHub-NextJS_Front_End-grey?logo=github&style=plastic)](https://github.com/JamesonRGrieve/Agent-LLM-Frontend)
 
 
 [![Discord](https://img.shields.io/discord/1097720481970397356?label=Discord&logo=discord&logoColor=white&style=plastic&color=5865f2)](https://discord.gg/d3TkHRZcjD) 
 [![Twitter](https://img.shields.io/badge/Twitter-Follow_@Josh_XT-blue?logo=twitter&style=plastic)](https://twitter.com/Josh_XT) 
 
-[![Logo](images/AGiXT.svg)](https://josh-xt.github.io/AGiXT/)
+[![Logo](images/AGiXT-gradient-flat.svg)](https://josh-xt.github.io/AGiXT/)
 
 AGiXT is a dynamic Artificial Intelligence Automation Platform engineered to orchestrate efficient AI instruction management and task execution across a multitude of providers. Our solution infuses adaptive memory handling with a broad spectrum of commands to enhance AI's understanding and responsiveness, leading to improved task completion. The platform's smart features, like Smart Instruct and Smart Chat, seamlessly integrate web search, planning strategies, and conversation continuity, transforming the interaction between users and AI. By leveraging a powerful plugin system that includes web browsing and command execution, AGiXT stands as a versatile bridge between AI models and users. With an expanding roster of AI providers, code evaluation capabilities, comprehensive chain management, and platform interoperability, AGiXT is consistently evolving to drive a multitude of applications, affirming its place at the forefront of AI technology.
 
 Embracing the spirit of extremity in every facet of life, we introduce AGiXT. This advanced AI Automation Platform is our bold step towards the realization of Artificial General Intelligence (AGI). Seamlessly orchestrating instruction management and executing complex tasks across diverse AI providers, AGiXT combines adaptive memory, smart features, and a versatile plugin system to maximize AI potential. With our unwavering commitment to innovation, we're dedicated to pushing the boundaries of AI and bringing AGI closer to reality.
 
 ## Table of Contents 📖
```

