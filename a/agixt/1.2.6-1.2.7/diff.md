# Comparing `tmp/agixt-1.2.6.tar.gz` & `tmp/agixt-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agixt-1.2.6.tar", last modified: Mon Jun 12 04:26:37 2023, max compression
+gzip compressed data, was "agixt-1.2.7.tar", last modified: Tue Jun 13 02:04:55 2023, max compression
```

## Comparing `agixt-1.2.6.tar` & `agixt-1.2.7.tar`

### file list

```diff
@@ -1,200 +1,207 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:26:37.787020 agixt-1.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-12 04:26:23.000000 agixt-1.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-12 04:26:23.000000 agixt-1.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-06-12 04:26:37.787020 agixt-1.2.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:26:37.759019 agixt-1.2.6/agixt/
--rw-r--r--   0 runner    (1001) docker     (123)    15552 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/Agent.py
--rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/Chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/Embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/Extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)    19672 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/Interactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/Memories.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/Prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:26:37.763019 agixt-1.2.6/agixt/WORKSPACE/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/WORKSPACE/example.txt
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:26:37.755019 agixt-1.2.6/agixt/agents/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:26:37.763019 agixt-1.2.6/agixt/agents/gpt4free/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/agents/gpt4free/config.json
--rw-r--r--   0 runner    (1001) docker     (123)    16613 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:26:37.763019 agixt-1.2.6/agixt/chains/
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/chains/Smart Chat.json
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/chains/Smart Instruct.json
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/chains/Task.json
--rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/chains/Test_Commands.json
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/chains/Write a Poem.json
--rw-r--r--   0 runner    (1001) docker     (123)    11977 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/example.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:26:37.763019 agixt-1.2.6/agixt/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)    10082 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/extensions/agixt_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/extensions/briantts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/extensions/dalle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/extensions/discord.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/extensions/elevenlabs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/extensions/file_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/extensions/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/extensions/google.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/extensions/gtts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/extensions/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/extensions/macostts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/extensions/microsoft_365.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/extensions/searxng.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/extensions/sendgrid_email.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/extensions/times.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/extensions/twitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/extensions/web_playwright.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:26:37.771019 agixt-1.2.6/agixt/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/Chat.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/Check-Instruction.txt
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/Create New Command.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/Custom Input.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/Execution.txt
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/Get Task List.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/Instruction.txt
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/JSONFormatter.txt
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/Pick a Poem Subject.txt
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/Pick-a-Link.txt
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/Prioritize.txt
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/Pseudo Code.txt
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/Score Response.txt
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/SmartChat-CleanResponse.txt
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/SmartChat-Researcher.txt
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/SmartChat-Resolver.txt
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/SmartChat-StepByStep.txt
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/SmartInstruct-CleanResponse.txt
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/SmartInstruct-Execution.txt
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/SmartInstruct-Researcher.txt
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/SmartInstruct-Resolver.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/SmartInstruct-StepByStep.txt
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/SmartTask-CleanResponse.txt
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/SmartTask-Execution.txt
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/SmartTask-StepByStep.txt
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/Task Execution.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/Tell Me How.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/Title a Poem.txt
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/Validation.txt
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/ValidationFailed.txt
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/WebSearch.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/Write a Haiku.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/Write a Poem.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:26:37.771019 agixt-1.2.6/agixt/prompts/gpt-3.5-turbo/
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/gpt-3.5-turbo/instruct.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:26:37.771019 agixt-1.2.6/agixt/prompts/gpt-4/
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/gpt-4/instruct.txt
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/instruct.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:26:37.771019 agixt-1.2.6/agixt/prompts/starchat/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/starchat/instruct.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:26:37.771019 agixt-1.2.6/agixt/prompts/vicuna/
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/prompts/vicuna/instruct.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:26:37.775020 agixt-1.2.6/agixt/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/provider/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/provider/bard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/provider/bing.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/provider/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/provider/claude.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/provider/fastchat.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/provider/gpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/provider/gpt4free.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/provider/gpugpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/provider/huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/provider/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/provider/kobold.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/provider/llamacpp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/provider/llamacppapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/provider/oobabooga.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/provider/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/provider/palm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/provider/runpod.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/provider/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-12 04:26:23.000000 agixt-1.2.6/agixt/version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:26:37.759019 agixt-1.2.6/agixt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-06-12 04:26:37.000000 agixt-1.2.6/agixt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-12 04:26:37.000000 agixt-1.2.6/agixt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 04:26:37.000000 agixt-1.2.6/agixt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-12 04:26:37.000000 agixt-1.2.6/agixt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-12 04:26:37.000000 agixt-1.2.6/agixt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:26:37.775020 agixt-1.2.6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:26:37.775020 agixt-1.2.6/docs/1-Getting started/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/1-Getting started/Quick Start.md
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/1-Getting started/Screenshots.md
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/1-Getting started/Support.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:26:37.775020 agixt-1.2.6/docs/2-Concepts/
--rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/2-Concepts/0-Core Concepts.md
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/2-Concepts/Agents.md
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/2-Concepts/Chains.md
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/2-Concepts/Chat.md
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/2-Concepts/Commands.md
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/2-Concepts/Instructions.md
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/2-Concepts/Prompts.md
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/2-Concepts/Providers.md
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/2-Concepts/Smart Chat.md
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/2-Concepts/Smart Instruct.md
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/2-Concepts/Smart Task.md
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/2-Concepts/Tasks.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:26:37.779019 agixt-1.2.6/docs/3-Providers/
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/3-Providers/Anthropic Claude.md
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/3-Providers/Azure OpenAI.md
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/3-Providers/ChatGPT.md
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/3-Providers/FastChat.md
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/3-Providers/GPT4ALL-GPU.md
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/3-Providers/GPT4ALL.md
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/3-Providers/GPT4Free.md
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/3-Providers/Google Bard.md
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/3-Providers/Google Palm.md
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/3-Providers/Hugging Face Transformers.md
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/3-Providers/HuggingChat.md
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/3-Providers/Kobold.md
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/3-Providers/Microsoft Bing.md
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/3-Providers/Oobabooga Text Generation Web UI.md
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/3-Providers/OpenAI.md
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/3-Providers/llamacpp API.md
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/3-Providers/llamacpp.md
--rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:26:37.783020 agixt-1.2.6/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/images/AGiXT-gradient-flat.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/images/AGiXT-gradient-light.svg
--rw-r--r--   0 runner    (1001) docker     (123)    35125 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/images/AGiXT.png
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/images/AGiXT.svg
--rw-r--r--   0 runner    (1001) docker     (123)  1707562 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/images/AGiXT_Original_PSD.psd
--rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/images/AGiXTwhiteborder.svg
--rw-r--r--   0 runner    (1001) docker     (123)    22316 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/images/Docker-desktop-win-setting-streamlit.png
--rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/images/Smart Instruct.drawio
--rw-r--r--   0 runner    (1001) docker     (123)    20691 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/images/Smart Instruct.drawio.svg
--rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/images/Smart Tasks.drawio
--rw-r--r--   0 runner    (1001) docker     (123)    22011 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/images/Smart Tasks.drawio.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-06-12 04:26:23.000000 agixt-1.2.6/docs/images/Untitled Diagram.drawio
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-12 04:26:23.000000 agixt-1.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-12 04:26:23.000000 agixt-1.2.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 04:26:37.787020 agixt-1.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-12 04:26:23.000000 agixt-1.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:26:37.783020 agixt-1.2.6/streamlit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:26:37.783020 agixt-1.2.6/streamlit/.streamlit/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-12 04:26:23.000000 agixt-1.2.6/streamlit/.streamlit/config.toml
--rw-r--r--   0 runner    (1001) docker     (123)    11948 2023-06-12 04:26:23.000000 agixt-1.2.6/streamlit/ApiClient.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-12 04:26:23.000000 agixt-1.2.6/streamlit/Main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:26:37.783020 agixt-1.2.6/streamlit/auth_libs/
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-12 04:26:23.000000 agixt-1.2.6/streamlit/auth_libs/Cfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-12 04:26:23.000000 agixt-1.2.6/streamlit/auth_libs/Redirect.py
--rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-06-12 04:26:23.000000 agixt-1.2.6/streamlit/auth_libs/Users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:26:37.783020 agixt-1.2.6/streamlit/auth_libs/pages/
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-12 04:26:23.000000 agixt-1.2.6/streamlit/auth_libs/pages/Login.py
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-06-12 04:26:23.000000 agixt-1.2.6/streamlit/auth_libs/pages/Profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-12 04:26:23.000000 agixt-1.2.6/streamlit/auth_libs/pages/Register.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:26:37.783020 agixt-1.2.6/streamlit/components/
--rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-06-12 04:26:23.000000 agixt-1.2.6/streamlit/components/chain.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-12 04:26:23.000000 agixt-1.2.6/streamlit/components/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-06-12 04:26:23.000000 agixt-1.2.6/streamlit/components/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-12 04:26:23.000000 agixt-1.2.6/streamlit/components/learning.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-06-12 04:26:23.000000 agixt-1.2.6/streamlit/components/selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-12 04:26:23.000000 agixt-1.2.6/streamlit/components/verify_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-12 04:26:23.000000 agixt-1.2.6/streamlit/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:26:37.787020 agixt-1.2.6/streamlit/pages/
--rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-06-12 04:26:23.000000 agixt-1.2.6/streamlit/pages/0-Agent_Settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-12 04:26:23.000000 agixt-1.2.6/streamlit/pages/1-Prompt_Templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-06-12 04:26:23.000000 agixt-1.2.6/streamlit/pages/2-Chain_Management.py
--rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-06-12 04:26:23.000000 agixt-1.2.6/streamlit/pages/3-Interact.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:26:37.787020 agixt-1.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    11948 2023-06-12 04:26:23.000000 agixt-1.2.6/tests/ApiClient.py
--rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-06-12 04:26:23.000000 agixt-1.2.6/tests/test-commands.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    54844 2023-06-12 04:26:23.000000 agixt-1.2.6/tests/tests.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:04:55.137424 agixt-1.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-13 02:04:45.000000 agixt-1.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-13 02:04:45.000000 agixt-1.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-06-13 02:04:55.137424 agixt-1.2.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:04:55.117424 agixt-1.2.7/agixt/
+-rw-r--r--   0 runner    (1001) docker     (123)    15882 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/Agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/Chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/Embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/Extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24534 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/Interactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/Memories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/Prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:04:55.117424 agixt-1.2.7/agixt/WORKSPACE/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/WORKSPACE/example.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:04:55.113424 agixt-1.2.7/agixt/agents/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:04:55.117424 agixt-1.2.7/agixt/agents/gpt4free/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/agents/gpt4free/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16614 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:04:55.117424 agixt-1.2.7/agixt/chains/
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/chains/Generate Smart Task Chain.json
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/chains/Generate Task Chain.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/chains/Generate and Run Smart Task Chain.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/chains/Generate and Run Task Chain.json
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/chains/Smart Chat.json
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/chains/Smart Instruct.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/chains/Test_Commands.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/chains/Write a Poem.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12075 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/example.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:04:55.121424 agixt-1.2.7/agixt/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/extensions/agixt_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/extensions/agixt_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/extensions/briantts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/extensions/dalle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/extensions/discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/extensions/elevenlabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/extensions/file_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/extensions/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/extensions/google.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/extensions/gtts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/extensions/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/extensions/macostts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/extensions/microsoft_365.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/extensions/searxng.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/extensions/sendgrid_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/extensions/times.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/extensions/twitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/extensions/web_playwright.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:04:55.121424 agixt-1.2.7/agixt/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/Chat.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/Check-Instruction.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/Create New Command.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/Custom Input.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/Execution.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/Get Task Description.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/Get Task List.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/Instruction.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/JSONFormatter.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/Pick a Poem Subject.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/Pick-a-Link.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/Prioritize.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/Pseudo Code.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/Score Response.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/SmartChat-CleanResponse.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/SmartChat-Researcher.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/SmartChat-Resolver.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/SmartChat-StepByStep.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/SmartInstruct-CleanResponse.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/SmartInstruct-Execution.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/SmartInstruct-Researcher.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/SmartInstruct-Resolver.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/SmartInstruct-StepByStep.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/SmartTask-CleanResponse.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/SmartTask-Execution.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/SmartTask-StepByStep.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/Task Execution.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/Tell Me How.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/Title a Poem.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/Validation.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/ValidationFailed.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/WebSearch.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/Write a Haiku.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/Write a Poem.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:04:55.121424 agixt-1.2.7/agixt/prompts/gpt-3.5-turbo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/gpt-3.5-turbo/instruct.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:04:55.125424 agixt-1.2.7/agixt/prompts/gpt-4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/gpt-4/instruct.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/instruct.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:04:55.125424 agixt-1.2.7/agixt/prompts/starchat/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/starchat/instruct.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:04:55.125424 agixt-1.2.7/agixt/prompts/vicuna/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/prompts/vicuna/instruct.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:04:55.125424 agixt-1.2.7/agixt/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/provider/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/provider/bard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/provider/bing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/provider/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/provider/claude.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/provider/fastchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/provider/gpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/provider/gpt4free.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/provider/gpugpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/provider/huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/provider/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/provider/kobold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/provider/llamacpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/provider/llamacppapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/provider/oobabooga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/provider/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/provider/palm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/provider/poe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/provider/runpod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/provider/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-13 02:04:45.000000 agixt-1.2.7/agixt/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:04:55.117424 agixt-1.2.7/agixt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-06-13 02:04:55.000000 agixt-1.2.7/agixt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-06-13 02:04:55.000000 agixt-1.2.7/agixt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 02:04:55.000000 agixt-1.2.7/agixt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-13 02:04:55.000000 agixt-1.2.7/agixt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-13 02:04:55.000000 agixt-1.2.7/agixt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:04:55.125424 agixt-1.2.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:04:55.125424 agixt-1.2.7/docs/1-Getting started/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/1-Getting started/Quick Start.md
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/1-Getting started/Screenshots.md
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/1-Getting started/Support.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:04:55.129424 agixt-1.2.7/docs/2-Concepts/
+-rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/2-Concepts/0-Core Concepts.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/2-Concepts/Agents.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/2-Concepts/Chains.md
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/2-Concepts/Chat.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/2-Concepts/Commands.md
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/2-Concepts/Instructions.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/2-Concepts/Prompts.md
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/2-Concepts/Providers.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/2-Concepts/Smart Chat.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/2-Concepts/Smart Instruct.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/2-Concepts/Smart Task.md
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/2-Concepts/Tasks.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:04:55.129424 agixt-1.2.7/docs/3-Providers/
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/3-Providers/Anthropic Claude.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/3-Providers/Azure OpenAI.md
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/3-Providers/ChatGPT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/3-Providers/FastChat.md
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/3-Providers/GPT4ALL-GPU.md
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/3-Providers/GPT4ALL.md
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/3-Providers/GPT4Free.md
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/3-Providers/Google Bard.md
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/3-Providers/Google Palm.md
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/3-Providers/Hugging Face Transformers.md
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/3-Providers/HuggingChat.md
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/3-Providers/Kobold.md
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/3-Providers/Microsoft Bing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/3-Providers/Oobabooga Text Generation Web UI.md
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/3-Providers/OpenAI.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/3-Providers/Poe.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/3-Providers/llamacpp API.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/3-Providers/llamacpp.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:04:55.133424 agixt-1.2.7/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/images/AGiXT-gradient-flat.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/images/AGiXT-gradient-light.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    35125 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/images/AGiXT.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/images/AGiXT.svg
+-rw-r--r--   0 runner    (1001) docker     (123)  1707562 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/images/AGiXT_Original_PSD.psd
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/images/AGiXTwhiteborder.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    22316 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/images/Docker-desktop-win-setting-streamlit.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/images/Smart Instruct.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)    20691 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/images/Smart Instruct.drawio.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/images/Smart Tasks.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)    22011 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/images/Smart Tasks.drawio.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-06-13 02:04:45.000000 agixt-1.2.7/docs/images/Untitled Diagram.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-13 02:04:45.000000 agixt-1.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-13 02:04:45.000000 agixt-1.2.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 02:04:55.137424 agixt-1.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-13 02:04:45.000000 agixt-1.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:04:55.133424 agixt-1.2.7/streamlit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:04:55.133424 agixt-1.2.7/streamlit/.streamlit/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-13 02:04:45.000000 agixt-1.2.7/streamlit/.streamlit/config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    11948 2023-06-13 02:04:45.000000 agixt-1.2.7/streamlit/ApiClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-13 02:04:45.000000 agixt-1.2.7/streamlit/Main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:04:55.133424 agixt-1.2.7/streamlit/auth_libs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-13 02:04:45.000000 agixt-1.2.7/streamlit/auth_libs/Cfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-13 02:04:45.000000 agixt-1.2.7/streamlit/auth_libs/Redirect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-06-13 02:04:45.000000 agixt-1.2.7/streamlit/auth_libs/Users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:04:55.133424 agixt-1.2.7/streamlit/auth_libs/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-13 02:04:45.000000 agixt-1.2.7/streamlit/auth_libs/pages/Login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-06-13 02:04:45.000000 agixt-1.2.7/streamlit/auth_libs/pages/Profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-13 02:04:45.000000 agixt-1.2.7/streamlit/auth_libs/pages/Register.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:04:55.133424 agixt-1.2.7/streamlit/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-06-13 02:04:45.000000 agixt-1.2.7/streamlit/components/chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-13 02:04:45.000000 agixt-1.2.7/streamlit/components/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-13 02:04:45.000000 agixt-1.2.7/streamlit/components/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-13 02:04:45.000000 agixt-1.2.7/streamlit/components/learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-06-13 02:04:45.000000 agixt-1.2.7/streamlit/components/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-13 02:04:45.000000 agixt-1.2.7/streamlit/components/verify_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-13 02:04:45.000000 agixt-1.2.7/streamlit/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:04:55.133424 agixt-1.2.7/streamlit/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-06-13 02:04:45.000000 agixt-1.2.7/streamlit/pages/0-Agent_Settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-13 02:04:45.000000 agixt-1.2.7/streamlit/pages/1-Prompt_Templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-06-13 02:04:45.000000 agixt-1.2.7/streamlit/pages/2-Chain_Management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-06-13 02:04:45.000000 agixt-1.2.7/streamlit/pages/3-Interact.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:04:55.133424 agixt-1.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    11948 2023-06-13 02:04:45.000000 agixt-1.2.7/tests/ApiClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-06-13 02:04:45.000000 agixt-1.2.7/tests/test-commands.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    56800 2023-06-13 02:04:45.000000 agixt-1.2.7/tests/tests.ipynb
```

### Comparing `agixt-1.2.6/LICENSE` & `agixt-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/PKG-INFO` & `agixt-1.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.2.6
+Version: 1.2.7
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `agixt-1.2.6/agixt/Agent.py` & `agixt-1.2.7/agixt/Agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,19 @@
 from provider import Provider
 from Memories import Memories
 from Extensions import Extensions
 from datetime import datetime
 
 DEFAULT_SETTINGS = {
     "provider": "gpt4free",
-    "AI_MODEL": "gpt-4",
+    "AI_MODEL": "gpt-3.5-turbo",
     "AI_TEMPERATURE": "0.7",
-    "MAX_TOKENS": "4000",
+    "MAX_TOKENS": "4096",
     "embedder": "default",
+    "autonomous_execution": "false",
 }
 
 
 def get_agent_file_paths(agent_name):
     base_path = os.path.join(os.getcwd(), "agents")
     folder_path = os.path.normpath(os.path.join(base_path, agent_name))
     config_path = os.path.normpath(os.path.join(folder_path, "config.json"))
@@ -115,15 +116,15 @@
         self.AGENT_CONFIG = self.get_agent_config()
         if "settings" in self.AGENT_CONFIG:
             self.PROVIDER_SETTINGS = self.AGENT_CONFIG["settings"]
             if "provider" in self.PROVIDER_SETTINGS:
                 self.AI_PROVIDER = self.PROVIDER_SETTINGS["provider"]
                 self.PROVIDER = Provider(self.AI_PROVIDER, **self.PROVIDER_SETTINGS)
                 self._load_agent_config_keys(
-                    ["AI_MODEL", "AI_TEMPERATURE", "MAX_TOKENS"]
+                    ["AI_MODEL", "AI_TEMPERATURE", "MAX_TOKENS", "autonomous_execution"]
                 )
             if "AI_MODEL" in self.PROVIDER_SETTINGS:
                 self.AI_MODEL = self.PROVIDER_SETTINGS["AI_MODEL"]
                 if self.AI_MODEL == "":
                     self.AI_MODEL = "default"
             else:
                 self.AI_MODEL = "openassistant"
@@ -138,14 +139,20 @@
                 self.MAX_TOKENS = self.PROVIDER_SETTINGS["MAX_TOKENS"]
             else:
                 self.MAX_TOKENS = 4000
             if "LOG_REQUESTS" in self.PROVIDER_SETTINGS:
                 self.LOG_REQUESTS = self.PROVIDER_SETTINGS["LOG_REQUESTS"]
             else:
                 self.LOG_REQUESTS = True
+            if "autonomous_execution" in self.PROVIDER_SETTINGS:
+                self.AUTONOMOUS_EXECUTION = self.PROVIDER_SETTINGS[
+                    "autonomous_execution"
+                ]
+            else:
+                self.AUTONOMOUS_EXECUTION = True
             self.commands = self.load_commands()
             self.available_commands = Extensions(
                 agent_config=self.AGENT_CONFIG
             ).get_available_commands()
             self.clean_agent_config_commands()
             self.history = self.load_history()
             self.agent_instances = {}
```

### Comparing `agixt-1.2.6/agixt/Chain.py` & `agixt-1.2.7/agixt/Chain.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,36 @@
 import os
 import json
-from Interactions import Interactions
 import argparse
-from Extensions import Extensions
 import logging
 from datetime import datetime
 
 
+def create_command_suggestion_chain(agent_name, command_name, command_args):
+    chain = Chain()
+    chains = chain.get_chains()
+    chain_name = f"{agent_name} Command Suggestions"
+    if chain_name in chains:
+        step = int(chain.get_chain(chain_name=chain_name)["steps"][-1]["step"]) + 1
+    else:
+        chain.add_chain(chain_name=chain_name)
+        step = 1
+    chain.add_chain_step(
+        chain_name=chain_name,
+        agent_name=agent_name,
+        step_number=step,
+        prompt_type="Command",
+        prompt={
+            "command_name": command_name,
+            **command_args,
+        },
+    )
+    return f"The command has been added to a chain called '{agent_name} Command Suggestions' for you to review and execute manually."
+
+
 def get_chain_file_path(chain_name):
     base_path = os.path.join(os.getcwd(), "chains")
     folder_path = os.path.normpath(os.path.join(base_path, chain_name))
     file_path = os.path.normpath(os.path.join(base_path, f"{chain_name}.json"))
     if not file_path.startswith(base_path) or not folder_path.startswith(base_path):
         raise ValueError("Invalid path, chain name must not contain slashes.")
     if not os.path.exists(folder_path):
@@ -179,32 +199,34 @@
         except:
             return {}
 
     def get_step_content(self, chain_name, prompt_content, user_input, agent_name):
         new_prompt_content = {}
         if isinstance(prompt_content, dict):
             for arg, value in prompt_content.items():
-                if "{user_input}" in value:
-                    value = value.replace("{user_input}", user_input)
-                if "{agent_name}" in value:
-                    value = value.replace("{agent_name}", agent_name)
-                if "{STEP" in value:
-                    # Count how many times {STEP is in the value
-                    step_count = value.count("{STEP")
-                    for i in range(step_count):
-                        # Get the step number from value between {STEP and }
-                        new_step_number = int(value.split("{STEP")[1].split("}")[0])
-                        # get the response from the step number
-                        step_response = self.get_step_response(
-                            chain_name=chain_name, step_number=new_step_number
-                        )
-                        # replace the {STEPx} with the response
-                        value = value.replace(
-                            f"{{STEP{new_step_number}}}", f"{step_response['response']}"
-                        )
+                if isinstance(value, str):
+                    if "{user_input}" in value:
+                        value = value.replace("{user_input}", user_input)
+                    if "{agent_name}" in value:
+                        value = value.replace("{agent_name}", agent_name)
+                    if "{STEP" in value:
+                        # Count how many times {STEP is in the value
+                        step_count = value.count("{STEP")
+                        for i in range(step_count):
+                            # Get the step number from value between {STEP and }
+                            new_step_number = int(value.split("{STEP")[1].split("}")[0])
+                            # get the response from the step number
+                            step_response = self.get_step_response(
+                                chain_name=chain_name, step_number=new_step_number
+                            )
+                            # replace the {STEPx} with the response
+                            value = value.replace(
+                                f"{{STEP{new_step_number}}}",
+                                f"{step_response['response']}",
+                            )
                 new_prompt_content[arg] = value
         elif isinstance(prompt_content, str):
             new_prompt_content = prompt_content
             if "{user_input}" in prompt_content:
                 new_prompt_content = new_prompt_content.replace(
                     "{user_input}", user_input
                 )
@@ -227,56 +249,14 @@
                     new_prompt_content = prompt_content.replace(
                         f"{{STEP{new_step_number}}}", f"{step_response['response']}"
                     )
             if new_prompt_content == {}:
                 new_prompt_content = prompt_content
         return new_prompt_content
 
-    async def run_chain_step(self, step: dict = {}, chain_name="", user_input=""):
-        logging.info(step)
-        if step:
-            if "prompt_type" in step:
-                agent_name = step["agent_name"]
-                agent = Interactions(agent_name)
-                prompt_type = step["prompt_type"]
-                step_number = step["step"]
-                if "prompt_name" in step["prompt"]:
-                    prompt_name = step["prompt"]["prompt_name"]
-                else:
-                    prompt_name = ""
-                args = self.get_step_content(
-                    chain_name=chain_name,
-                    prompt_content=step["prompt"],
-                    user_input=user_input,
-                    agent_name=agent_name,
-                )
-                if prompt_type == "Command":
-                    return await Extensions(
-                        agent_config=agent.agent.agent_config
-                    ).execute_command(
-                        command_name=args["command_name"],
-                        command_args=args,
-                    )
-                elif prompt_type == "Prompt":
-                    result = await agent.run(
-                        user_input=user_input,
-                        prompt=prompt_name,
-                        chain_name=chain_name,
-                        step_number=step_number,
-                        **args,
-                    )
-                elif prompt_type == "Chain":
-                    result = await self.run_chain(
-                        chain_name=step["prompt"]["chain_name"], user_input=user_input
-                    )
-        if result:
-            return result
-        else:
-            return None
-
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("--chain", type=str, default="")
     parser.add_argument("--user_input", type=str, default="")
     args = parser.parse_args()
     chain_name = args.chain
```

### Comparing `agixt-1.2.6/agixt/Embedding.py` & `agixt-1.2.7/agixt/Embedding.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/agixt/Extensions.py` & `agixt-1.2.7/agixt/Extensions.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/agixt/Interactions.py` & `agixt-1.2.7/agixt/Interactions.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,24 +4,30 @@
 import json
 import time
 import spacy
 from datetime import datetime
 from Agent import Agent
 from Prompts import Prompts
 from extensions.searxng import searxng
+from Chain import Chain, get_chain_responses_file_path, create_command_suggestion_chain
 from urllib.parse import urlparse
 import logging
 from concurrent.futures import Future
 
 
 class Interactions:
-    def __init__(self, agent_name: str = "AGiXT"):
-        self.agent_name = agent_name
-        self.agent = Agent(self.agent_name)
-        self.agent_commands = self.agent.get_commands_string()
+    def __init__(self, agent_name: str = ""):
+        if agent_name != "":
+            self.agent_name = agent_name
+            self.agent = Agent(self.agent_name)
+            self.agent_commands = self.agent.get_commands_string()
+        else:
+            self.agent_name = ""
+            self.agent = None
+            self.agent_commands = ""
         self.stop_running_event = None
         self.browsed_links = []
         self.failures = 0
         self.nlp = None
 
     def load_spacy_model(self):
         if not self.nlp:
@@ -149,17 +155,17 @@
         prompt: str = "",
         context_results: int = 5,
         websearch: bool = False,
         websearch_depth: int = 3,
         learn_file: str = "",
         chain_name: str = "",
         step_number: int = 0,
+        shots: int = 1,
         **kwargs,
     ):
-        logging.info(f"KWARGS: {kwargs}")
         memories = self.agent.get_memories()
         if learn_file != "":
             learning_file = await memories.mem_read_file(file_path=learn_file)
             if learning_file == False:
                 return "Failed to read file."
         formatted_prompt, unformatted_prompt, tokens = await self.format_prompt(
             user_input=user_input,
@@ -206,40 +212,134 @@
             execution_response = await self.execution_agent(
                 execution_response=self.response,
                 user_input=user_input,
                 context_results=context_results,
                 **kwargs,
             )
             return_response = ""
-            try:
-                self.response = json.loads(self.response)
-                if "response" in self.response:
-                    return_response = self.response["response"]
-                if "commands" in self.response:
-                    if self.response["commands"] != {}:
+            if bool(self.agent.AUTONOMOUS_EXECUTION) == True:
+                try:
+                    self.response = json.loads(self.response)
+                    if "response" in self.response:
+                        return_response = self.response["response"]
+                    if "commands" in self.response:
+                        if self.response["commands"] != {}:
+                            return_response += (
+                                f"\n\nCommands Executed:\n{self.response['commands']}"
+                            )
+                    if execution_response:
                         return_response += (
-                            f"\n\nCommands Executed:\n{self.response['commands']}"
+                            f"\n\nCommand Execution Response:\n{execution_response}"
                         )
-                if execution_response:
-                    return_response += (
-                        f"\n\nCommand Execution Response:\n{execution_response}"
-                    )
-            except:
-                return_response = self.response
+                except:
+                    return_response = self.response
+            else:
+                return_response = f"{self.response}\n\n{execution_response}"
             self.response = return_response
         logging.info(f"Response: {self.response}")
         if self.response != "" and self.response != None:
             try:
                 await memories.store_result(input=user_input, result=self.response)
             except:
                 pass
-            self.agent.log_interaction(role="USER", message=user_input)
+            if prompt == "Chat":
+                self.agent.log_interaction(role="USER", message=user_input)
+            else:
+                self.agent.log_interaction(role="USER", message=formatted_prompt)
             self.agent.log_interaction(role=self.agent_name, message=self.response)
+
+        if shots > 1:
+            responses = [self.response]
+            for shot in range(shots - 1):
+                shot_response = self.run(
+                    user_input=user_input,
+                    prompt=prompt,
+                    context_results=context_results,
+                    shots=shots - 1,
+                    chain_name=chain_name,
+                    step_number=step_number,
+                    **kwargs,
+                )
+                time.sleep(1)
+                responses.append(shot_response)
+            return "\n".join(
+                [
+                    f"Response {shot + 1}:\n{response}"
+                    for shot, response in enumerate(responses)
+                ]
+            )
         return self.response
 
+    async def run_chain_step(self, step: dict = {}, chain_name="", user_input=""):
+        logging.info(step)
+        chain = Chain()
+        if step:
+            if "prompt_type" in step:
+                self.agent_name = step["agent_name"]
+                self.agent = Agent(self.agent_name)
+                self.agent_commands = self.agent.get_commands_string()
+                prompt_type = step["prompt_type"]
+                step_number = step["step"]
+                if "prompt_name" in step["prompt"]:
+                    prompt_name = step["prompt"]["prompt_name"]
+                else:
+                    prompt_name = ""
+                args = chain.get_step_content(
+                    chain_name=chain_name,
+                    prompt_content=step["prompt"],
+                    user_input=user_input,
+                    agent_name=self.agent_name,
+                )
+                if prompt_type == "Command":
+                    return await self.agent.execute(
+                        command_name=args["command_name"],
+                        command_args=args,
+                    )
+                elif prompt_type == "Prompt":
+                    result = await self.run(
+                        user_input=user_input,
+                        prompt=prompt_name,
+                        chain_name=chain_name,
+                        step_number=step_number,
+                        **args,
+                    )
+                elif prompt_type == "Chain":
+                    result = await self.run_chain(
+                        chain_name=step["prompt"]["chain_name"], user_input=user_input
+                    )
+        if result:
+            return result
+        else:
+            return None
+
+    async def run_chain(self, chain_name, user_input=None):
+        chain = Chain()
+        file_path = get_chain_responses_file_path(chain_name=chain_name)
+        chain_data = chain.get_chain(chain_name=chain_name)
+        logging.info(f"Running chain '{chain_name}'")
+        responses = {}  # Create a dictionary to hold responses.
+        for step_data in chain_data["steps"]:
+            if "prompt" in step_data and "step" in step_data:
+                logging.info(f"Running step {step_data['step']}")
+                step = {}
+                step_response = await self.run_chain_step(
+                    step=step_data, chain_name=chain_name, user_input=user_input
+                )  # Get the response of the current step.
+                step["response"] = step_response
+                step["agent_name"] = step_data["agent_name"]
+                step["prompt"] = step_data["prompt"]
+                step["prompt_type"] = step_data["prompt_type"]
+                responses[step_data["step"]] = step  # Store the response.
+                logging.info(f"Response: {step_response}")
+                # Write the responses to the json file.
+                dt = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
+                with open(file_path, "w") as f:
+                    json.dump(responses, f)
+        return responses
+
     async def smart_instruct(
         self,
         user_input: str = "Write a tweet about AI.",
         shots: int = 3,
         learn_file: str = "",
         objective: str = None,
         **kwargs,
@@ -393,17 +493,25 @@
             for command_name, command_args in validated_response["commands"].items():
                 # Search for the command in the available_commands list, and if found, use the command's name attribute for execution
                 if command_name is not None:
                     for available_command in self.agent.available_commands:
                         if command_name == available_command["friendly_name"]:
                             # Check if the command is a valid command in the self.avent.available_commands list
                             try:
-                                command_output = await self.agent.execute(
-                                    command_name=command_name, command_args=command_args
-                                )
+                                if bool(self.agent.AUTONOMOUS_EXECUTION) == True:
+                                    command_output = await self.agent.execute(
+                                        command_name=command_name,
+                                        command_args=command_args,
+                                    )
+                                else:
+                                    command_output = create_command_suggestion_chain(
+                                        agent_name=self.agent_name,
+                                        command_name=command_name,
+                                        command_args=command_args,
+                                    )
                             except Exception as e:
                                 logging.info("Command validation failed, retrying...")
                                 validate_command = await self.run(
                                     user_input=user_input,
                                     prompt="ValidationFailed",
                                     command_name=command_name,
                                     command_args=command_args,
```

### Comparing `agixt-1.2.6/agixt/Memories.py` & `agixt-1.2.7/agixt/Memories.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/agixt/Prompts.py` & `agixt-1.2.7/agixt/Prompts.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,17 +11,14 @@
         os.path.join(base_path, f"{prompt_name}.txt")
     )
     if (
         not base_model_path.startswith(base_path)
         or not model_prompt_file.startswith(base_model_path)
         or not default_prompt_file.startswith(base_path)
     ):
-        print(base_model_path)
-        print(model_prompt_file)
-        print(default_prompt_file)
         raise ValueError(
             "Invalid file path. Prompt name cannot contain '/', '\\' or '..' in"
         )
     if not os.path.exists(base_path):
         os.mkdir(base_path)
     if not os.path.exists(base_model_path):
         os.mkdir(base_model_path)
```

### Comparing `agixt-1.2.6/agixt/app.py` & `agixt-1.2.7/agixt/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -323,15 +323,14 @@
 
 
 @app.patch("/api/agent/{agent_name}/command", tags=["Agent"])
 async def toggle_command(
     agent_name: str, payload: ToggleCommandPayload
 ) -> ResponseMessage:
     agent = Agent(agent_name=agent_name)
-    print(payload)
     try:
         if payload.command_name == "*":
             for each_command_name in agent.agent_config["commands"]:
                 agent.agent_config["commands"][each_command_name] = payload.enable
 
             agent.update_agent_config(
                 new_config=agent.agent_config["commands"], config_key="commands"
@@ -377,15 +376,15 @@
         return {"chain": chain_data}
     except:
         raise HTTPException(status_code=404, detail="Chain not found")
 
 
 @app.post("/api/chain/{chain_name}/run", tags=["Chain"])
 async def run_chain(chain_name: str, user_input: Prompt):
-    chain_response = await Chain().run_chain(
+    chain_response = await Interactions(agent_name="").run_chain(
         chain_name=chain_name, user_input=user_input.prompt
     )
     return chain_response
 
 
 @app.post("/api/chain", tags=["Chain"])
 async def add_chain(chain_name: ChainName) -> ResponseMessage:
```

### Comparing `agixt-1.2.6/agixt/chains/Smart Chat.json` & `agixt-1.2.7/agixt/chains/Smart Chat.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9849537037037037%*

 * *Differences: {"'steps'": "{0: {'prompt_type': 'Prompt', 'prompt': {delete: ['command_name', 'user_input', "*

 * *            "'prompt_args', 'agent']}}}"}*

```diff
@@ -1,24 +1,20 @@
 {
     "chain_name": "Smart Chat",
     "steps": [
         {
             "agent_name": "gpt4free",
             "prompt": {
-                "agent": "{agent_name}",
-                "command_name": "Prompt AI Agent",
                 "context_results": 5,
-                "prompt_args": {},
                 "prompt_name": "SmartChat-StepByStep",
                 "shots": 3,
-                "user_input": "{user_input}",
                 "websearch": true,
                 "websearch_depth": 3
             },
-            "prompt_type": "Command",
+            "prompt_type": "Prompt",
             "step": 1
         },
         {
             "agent_name": "gpt4free",
             "prompt": {
                 "prompt_name": "SmartChat-Researcher",
                 "shots": "3",
```

### Comparing `agixt-1.2.6/agixt/chains/Smart Instruct.json` & `agixt-1.2.7/agixt/chains/Smart Instruct.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9849537037037037%*

 * *Differences: {"'steps'": "{0: {'prompt_type': 'Prompt', 'prompt': {delete: ['command_name', 'user_input', "*

 * *            "'prompt_args', 'agent']}}}"}*

```diff
@@ -1,24 +1,20 @@
 {
     "chain_name": "Smart Instruct",
     "steps": [
         {
             "agent_name": "gpt4free",
             "prompt": {
-                "agent": "{agent_name}",
-                "command_name": "Prompt AI Agent",
                 "context_results": 5,
-                "prompt_args": {},
                 "prompt_name": "SmartInstruct-StepByStep",
                 "shots": 3,
-                "user_input": "{user_input}",
                 "websearch": true,
                 "websearch_depth": 3
             },
-            "prompt_type": "Command",
+            "prompt_type": "Prompt",
             "step": 1
         },
         {
             "agent_name": "gpt4free",
             "prompt": {
                 "prompt_name": "SmartInstruct-Researcher",
                 "shots": "3",
```

### Comparing `agixt-1.2.6/agixt/chains/Task.json` & `agixt-1.2.7/agixt/chains/Generate Task Chain.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6385416666666667%*

 * *Differences: {"'chain_name'": "'Generate Task Chain'",*

 * * "'steps'": "{0: {'prompt': {'websearch': True, 'websearch_depth': 3, 'context_results': 5, "*

 * *            "delete: ['user_input']}}, 2: {'step': 3, 'prompt': {'command_name': 'Create Task "*

 * *            "Chain', 'agent': 'gpt4free', 'primary_objective': '{user_input}', "*

 * *            "'numbered_list_of_tasks': '{STEP1}', 'short_task_description': '{STEP2}', delete: "*

 * *            "['user_input', 'tasks', 'websearch', 'websearch_depth', 'context_results']}}, insert: "*

 * *  […]*

```diff
@@ -1,28 +1,36 @@
 {
-    "chain_name": "Task",
+    "chain_name": "Generate Task Chain",
     "steps": [
         {
             "agent_name": "gpt4free",
             "prompt": {
+                "context_results": 5,
                 "prompt_name": "Get Task List",
-                "user_input": "{user_input}"
+                "websearch": true,
+                "websearch_depth": 3
             },
             "prompt_type": "Prompt",
             "step": 1
         },
         {
             "agent_name": "gpt4free",
             "prompt": {
-                "agent": "{agent_name}",
-                "command_name": "Execute Task List",
-                "context_results": 5,
-                "tasks": "{STEP1}",
-                "user_input": "{user_input}",
-                "websearch": false,
-                "websearch_depth": 0
+                "prompt_name": "Get Task Description"
             },
-            "prompt_type": "Command",
+            "prompt_type": "Prompt",
             "step": 2
+        },
+        {
+            "agent_name": "gpt4free",
+            "prompt": {
+                "agent": "gpt4free",
+                "command_name": "Create Task Chain",
+                "numbered_list_of_tasks": "{STEP1}",
+                "primary_objective": "{user_input}",
+                "short_task_description": "{STEP2}"
+            },
+            "prompt_type": "Command",
+            "step": 3
         }
     ]
 }
```

### Comparing `agixt-1.2.6/agixt/chains/Test_Commands.json` & `agixt-1.2.7/agixt/chains/Test_Commands.json`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/agixt/chains/Write a Poem.json` & `agixt-1.2.7/agixt/chains/Write a Poem.json`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/agixt/example.ipynb` & `agixt-1.2.7/agixt/example.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9984751793345543%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(19, ')\\n')], delete: [19]}}, 3: {'source': {insert: [(24, "*

 * *            "'chain.add_chain(chain_name)')], delete: [24]}}, 5: {'source': {insert: [(14, "*

 * *            "')\\n')], delete: [14]}}, 7: {'source': {insert: [(22, ')\\n')], delete: [22]}}, 9: "*

 * *            "{'source': {insert: [(22, ')\\n')], delete: [22]}}, 11: {'source': ['from "*

 * *            "Interactions import Interactions\\n', '\\n', "*

 * *            '\'Interactions(agent_name="").run_chain(chain_name=chain_n […]*

```diff
@@ -59,15 +59,15 @@
                 "    industry=\"software\",\n",
                 "    business_description=\"I am a software company that makes software for software companies.\",\n",
                 "    # Other available options:\n",
                 "    # context_results = 5,  # Number of memories to inject into context\n",
                 "    # websearch = False,   # Use websearch to find context\n",
                 "    # websearch_depth = 3,  # Number of websearch results to use\n",
                 "    # learn_file: str = \"/path/to/file/to/learn/from.txt\",  # File to learn from\n",
-                ")"
+                ")\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -111,15 +111,15 @@
                 "business_description = \"We're a artificial intelligence software development company.\"\n",
                 "website = \"https://devxt.com\"\n",
                 "\n",
                 "# Set up your ai agent\n",
                 "ai = Interactions(agent_name)\n",
                 "\n",
                 "# Create the new chain to start adding steps to.\n",
-                "chain.add_chain(chain_name)\n"
+                "chain.add_chain(chain_name)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -144,15 +144,15 @@
                 ")\n",
                 "\n",
                 "cp.add_prompt(\n",
                 "    prompt_name=\"Good email subject for blog post\",\n",
                 "    prompt=\"\"\"\n",
                 "    I need a good email subject for this blog post, I'm going to send it out to customers, so I need something that is attractive. Please respond only with the subject line.\n",
                 "    Blog post: {blog_post}\"\"\",\n",
-                ")"
+                ")\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -185,15 +185,15 @@
                 "    agent_name=agent_name,\n",
                 "    step_number=2,\n",
                 "    prompt_type=\"Prompt\",\n",
                 "    prompt={\n",
                 "        \"prompt_name\": \"Good email subject for blog post\",\n",
                 "        \"blog_post\": \"{STEP1}\",  # <- Intentionally not an f-string, we want to use the response from the previous step in the chain.\n",
                 "    },\n",
-                ")"
+                ")\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -226,15 +226,15 @@
                 "    prompt_type=\"Command\",\n",
                 "    prompt={\n",
                 "        \"command_name\": \"send_email\",\n",
                 "        \"email\": f\"your@customers-email.com\",\n",
                 "        \"subject\": \"{STEP2}\",\n",
                 "        \"body\": \"{STEP1}\",\n",
                 "    },\n",
-                ")"
+                ")\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -243,15 +243,17 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "chain.run_chain(chain_name)"
+                "from Interactions import Interactions\n",
+                "\n",
+                "Interactions(agent_name=\"\").run_chain(chain_name=chain_name)"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3",
             "language": "python",
```

### Comparing `agixt-1.2.6/agixt/extensions/agixt_agent.py` & `agixt-1.2.7/agixt/extensions/agixt_agent.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,53 +1,42 @@
 from Extensions import Extensions
 from Agent import get_agents
-from Chain import Chain
 from Interactions import Interactions
 import json
 import os
 from typing import List, Optional
 from transformers import BlipProcessor, BlipForConditionalGeneration
 import torch
 from PIL import Image
 import requests
 
 
 class agixt_agent(Extensions):
     def __init__(self, **kwargs):
         agents = get_agents()
-        self.chains = Chain().get_chains()
         self.commands = {
             "Evaluate Code": self.evaluate_code,
             "Analyze Pull Request": self.analyze_pull_request,
             "Perform Automated Testing": self.perform_automated_testing,
             "Run CI-CD Pipeline": self.run_ci_cd_pipeline,
             "Improve Code": self.improve_code,
             "Write Tests": self.write_tests,
             "Create a new command": self.create_command,
-            "Execute Task List": self.execute_task_list,
-            "Prompt AI Agent": self.prompt_agent,
             "Describe Image": self.describe_image,
         }
         if agents != None:
             for agent in agents:
                 if "name" in agent:
                     name = f" AI Agent {agent['name']}"
                     self.commands.update(
                         {
                             f"Ask{name}": self.ask,
                             f"Instruct{name}": self.instruct,
-                            f"Prompt{name}": self.prompt_agent,
                         }
                     )
-        if self.chains != None:
-            for chain in self.chains:
-                if "name" in chain:
-                    self.commands.update(
-                        {f"Run Chain: {chain['name']}": self.run_chain}
-                    )
 
     def command_exists(self, file_name: str) -> bool:
         return os.path.exists(f"commands/{file_name}.py")
 
     async def create_command(
         self, function_description: str, agent: str = "AGiXT"
     ) -> List[str]:
@@ -118,99 +107,26 @@
         function_string = "def run_pipeline(repo_url: str) -> str:"
         description_string = (
             "Runs the entire CI/CD pipeline for the given repository URL."
         )
         prompt = f"You are now the following python function: ```# {description_string}\n{function_string}```\n\nOnly respond with your `return` value. Args: {args}"
         return await Interactions(agent_name=agent).run(user_input=prompt)
 
-    async def run_chain(self, chain_name: str = "", user_input: str = ""):
-        await Chain().run_chain(chain_name=chain_name, user_input=user_input)
-        return "Chain started successfully."
-
     async def ask(self, user_input: str, agent: str = "AGiXT") -> str:
         response = await Interactions(agent_name=agent).run(
             user_input=user_input, prompt="chat", websearch=True, websearch_depth=4
         )
         return response
 
     async def instruct(self, user_input: str, agent: str = "AGiXT") -> str:
         response = await Interactions(agent_name=agent).run(
             user_input=user_input, prompt="instruct", websearch=True, websearch_depth=8
         )
         return response
 
-    async def prompt_agent(
-        self,
-        agent: str = "gpt4free",
-        user_input: str = "",
-        prompt_name: str = "",
-        prompt_args: dict = {},
-        websearch: bool = False,
-        websearch_depth: int = 3,
-        context_results: int = 5,
-        shots: int = 1,
-    ) -> str:
-        response = await Interactions(agent_name=agent).run(
-            user_input=user_input,
-            prompt=prompt_name,
-            websearch=websearch,
-            websearch_depth=websearch_depth,
-            context_results=context_results,
-            **prompt_args,
-        )
-        if shots > 1:
-            responses = [response]
-            for shot in range(shots - 1):
-                response = await Interactions(agent_name=agent).run(
-                    user_input=user_input,
-                    prompt=prompt_name,
-                    context_results=context_results,
-                    **prompt_args,
-                )
-                responses.append(response)
-            # Join responses by "Response # <shot number>:" and return
-            return "\n".join(
-                [
-                    f"Response {shot + 1}:\n{response}"
-                    for shot, response in enumerate(responses)
-                ]
-            )
-        return response
-
-    async def execute_task_list(
-        self,
-        agent: str,
-        tasks: str,
-        user_input: str,
-        websearch: bool = False,
-        websearch_depth: int = 3,
-        context_results: int = 5,
-    ):
-        task_list = tasks.split("\n")
-        task_list = [
-            task
-            for task in task_list
-            if task and task[0] in [str(i) for i in range(10)]
-        ]
-        responses = []
-        for task in task_list:
-            if "task_name" in task:
-                response = await Interactions(agent_name=agent).run(
-                    user_input=user_input,
-                    prompt="Task Execution",
-                    prompt_args={
-                        "task": task["task_name"],
-                    },
-                    websearch=websearch,
-                    websearch_depth=websearch_depth,
-                    context_results=context_results,
-                )
-                responses.append(response)
-        return "\n".join(responses)
-
     async def describe_image(self, image_url):
         """
         Describe an image using FuseCap.
         """
         if image_url:
             processor = BlipProcessor.from_pretrained("noamrot/FuseCap")
             model = BlipForConditionalGeneration.from_pretrained("noamrot/FuseCap")
```

### Comparing `agixt-1.2.6/agixt/extensions/briantts.py` & `agixt-1.2.7/agixt/extensions/briantts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/agixt/extensions/dalle.py` & `agixt-1.2.7/agixt/extensions/dalle.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/agixt/extensions/discord.py` & `agixt-1.2.7/agixt/extensions/discord.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/agixt/extensions/elevenlabs.py` & `agixt-1.2.7/agixt/extensions/elevenlabs.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/agixt/extensions/file_system.py` & `agixt-1.2.7/agixt/extensions/file_system.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/agixt/extensions/github.py` & `agixt-1.2.7/agixt/extensions/github.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/agixt/extensions/google.py` & `agixt-1.2.7/agixt/extensions/google.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/agixt/extensions/gtts.py` & `agixt-1.2.7/agixt/extensions/gtts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/agixt/extensions/huggingface.py` & `agixt-1.2.7/agixt/extensions/huggingface.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/agixt/extensions/macostts.py` & `agixt-1.2.7/agixt/extensions/macostts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/agixt/extensions/microsoft_365.py` & `agixt-1.2.7/agixt/extensions/microsoft_365.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/agixt/extensions/searxng.py` & `agixt-1.2.7/agixt/extensions/searxng.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/agixt/extensions/sendgrid_email.py` & `agixt-1.2.7/agixt/extensions/sendgrid_email.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/agixt/extensions/twitter.py` & `agixt-1.2.7/agixt/extensions/twitter.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/agixt/extensions/web_playwright.py` & `agixt-1.2.7/agixt/extensions/web_playwright.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/agixt/prompts/Create New Command.txt` & `agixt-1.2.7/agixt/prompts/Create New Command.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/agixt/prompts/Execution.txt` & `agixt-1.2.7/agixt/prompts/Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/agixt/prompts/Instruction.txt` & `agixt-1.2.7/agixt/prompts/Instruction.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/agixt/prompts/SmartInstruct-Execution.txt` & `agixt-1.2.7/agixt/prompts/SmartInstruct-Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/agixt/prompts/SmartTask-Execution.txt` & `agixt-1.2.7/agixt/prompts/SmartTask-Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/agixt/prompts/Task Execution.txt` & `agixt-1.2.7/agixt/prompts/Task Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/agixt/prompts/ValidationFailed.txt` & `agixt-1.2.7/agixt/prompts/ValidationFailed.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/agixt/prompts/gpt-3.5-turbo/instruct.txt` & `agixt-1.2.7/agixt/prompts/gpt-3.5-turbo/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/agixt/prompts/gpt-4/instruct.txt` & `agixt-1.2.7/agixt/prompts/gpt-4/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/agixt/prompts/instruct.txt` & `agixt-1.2.7/agixt/prompts/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/agixt/prompts/starchat/instruct.txt` & `agixt-1.2.7/agixt/prompts/starchat/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/agixt/prompts/vicuna/instruct.txt` & `agixt-1.2.7/agixt/prompts/vicuna/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/agixt/provider/__init__.py` & `agixt-1.2.7/agixt/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/agixt/provider/azure.py` & `agixt-1.2.7/agixt/provider/azure.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/agixt/provider/bing.py` & `agixt-1.2.7/agixt/provider/bing.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/agixt/provider/chatgpt.py` & `agixt-1.2.7/agixt/provider/chatgpt.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/agixt/provider/claude.py` & `agixt-1.2.7/agixt/provider/claude.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/agixt/provider/fastchat.py` & `agixt-1.2.7/agixt/provider/fastchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/agixt/provider/gpt4all.py` & `agixt-1.2.7/agixt/provider/gpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/agixt/provider/gpt4free.py` & `agixt-1.2.7/agixt/provider/gpt4free.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/agixt/provider/gpugpt4all.py` & `agixt-1.2.7/agixt/provider/gpugpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/agixt/provider/huggingchat.py` & `agixt-1.2.7/agixt/provider/huggingchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/agixt/provider/huggingface.py` & `agixt-1.2.7/agixt/provider/huggingface.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/agixt/provider/kobold.py` & `agixt-1.2.7/agixt/provider/kobold.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/agixt/provider/llamacpp.py` & `agixt-1.2.7/agixt/provider/llamacpp.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/agixt/provider/llamacppapi.py` & `agixt-1.2.7/agixt/provider/llamacppapi.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/agixt/provider/oobabooga.py` & `agixt-1.2.7/agixt/provider/oobabooga.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/agixt/provider/openai.py` & `agixt-1.2.7/agixt/provider/openai.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/agixt/provider/palm.py` & `agixt-1.2.7/agixt/provider/palm.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/agixt/provider/runpod.py` & `agixt-1.2.7/agixt/provider/runpod.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/agixt/provider/transformer.py` & `agixt-1.2.7/agixt/provider/transformer.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/agixt.egg-info/PKG-INFO` & `agixt-1.2.7/agixt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.2.6
+Version: 1.2.7
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `agixt-1.2.6/agixt.egg-info/SOURCES.txt` & `agixt-1.2.7/agixt.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -17,20 +17,24 @@
 agixt.egg-info/PKG-INFO
 agixt.egg-info/SOURCES.txt
 agixt.egg-info/dependency_links.txt
 agixt.egg-info/requires.txt
 agixt.egg-info/top_level.txt
 agixt/WORKSPACE/example.txt
 agixt/agents/gpt4free/config.json
+agixt/chains/Generate Smart Task Chain.json
+agixt/chains/Generate Task Chain.json
+agixt/chains/Generate and Run Smart Task Chain.json
+agixt/chains/Generate and Run Task Chain.json
 agixt/chains/Smart Chat.json
 agixt/chains/Smart Instruct.json
-agixt/chains/Task.json
 agixt/chains/Test_Commands.json
 agixt/chains/Write a Poem.json
 agixt/extensions/agixt_agent.py
+agixt/extensions/agixt_chain.py
 agixt/extensions/briantts.py
 agixt/extensions/dalle.py
 agixt/extensions/discord.py
 agixt/extensions/elevenlabs.py
 agixt/extensions/file_system.py
 agixt/extensions/github.py
 agixt/extensions/google.py
@@ -44,14 +48,15 @@
 agixt/extensions/twitter.py
 agixt/extensions/web_playwright.py
 agixt/prompts/Chat.txt
 agixt/prompts/Check-Instruction.txt
 agixt/prompts/Create New Command.txt
 agixt/prompts/Custom Input.txt
 agixt/prompts/Execution.txt
+agixt/prompts/Get Task Description.txt
 agixt/prompts/Get Task List.txt
 agixt/prompts/Instruction.txt
 agixt/prompts/JSONFormatter.txt
 agixt/prompts/Pick a Poem Subject.txt
 agixt/prompts/Pick-a-Link.txt
 agixt/prompts/Prioritize.txt
 agixt/prompts/Pseudo Code.txt
@@ -95,14 +100,15 @@
 agixt/provider/huggingface.py
 agixt/provider/kobold.py
 agixt/provider/llamacpp.py
 agixt/provider/llamacppapi.py
 agixt/provider/oobabooga.py
 agixt/provider/openai.py
 agixt/provider/palm.py
+agixt/provider/poe.py
 agixt/provider/runpod.py
 agixt/provider/transformer.py
 docs/.gitignore
 docs/README.md
 docs/1-Getting started/Quick Start.md
 docs/1-Getting started/Screenshots.md
 docs/1-Getting started/Support.md
@@ -129,14 +135,15 @@
 docs/3-Providers/Google Palm.md
 docs/3-Providers/Hugging Face Transformers.md
 docs/3-Providers/HuggingChat.md
 docs/3-Providers/Kobold.md
 docs/3-Providers/Microsoft Bing.md
 docs/3-Providers/Oobabooga Text Generation Web UI.md
 docs/3-Providers/OpenAI.md
+docs/3-Providers/Poe.md
 docs/3-Providers/llamacpp API.md
 docs/3-Providers/llamacpp.md
 docs/images/AGiXT-gradient-flat.svg
 docs/images/AGiXT-gradient-light.svg
 docs/images/AGiXT.png
 docs/images/AGiXT.svg
 docs/images/AGiXT_Original_PSD.psd
```

### Comparing `agixt-1.2.6/docs/1-Getting started/Quick Start.md` & `agixt-1.2.7/docs/1-Getting started/Quick Start.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/docs/1-Getting started/Screenshots.md` & `agixt-1.2.7/docs/1-Getting started/Screenshots.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/docs/1-Getting started/Support.md` & `agixt-1.2.7/docs/1-Getting started/Support.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/docs/2-Concepts/0-Core Concepts.md` & `agixt-1.2.7/docs/2-Concepts/0-Core Concepts.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/docs/2-Concepts/Agents.md` & `agixt-1.2.7/docs/2-Concepts/Agents.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/docs/2-Concepts/Chains.md` & `agixt-1.2.7/docs/2-Concepts/Chains.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/docs/2-Concepts/Chat.md` & `agixt-1.2.7/docs/2-Concepts/Chat.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/docs/2-Concepts/Commands.md` & `agixt-1.2.7/docs/2-Concepts/Commands.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/docs/2-Concepts/Instructions.md` & `agixt-1.2.7/docs/2-Concepts/Instructions.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/docs/2-Concepts/Prompts.md` & `agixt-1.2.7/docs/2-Concepts/Prompts.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/docs/2-Concepts/Smart Chat.md` & `agixt-1.2.7/docs/2-Concepts/Smart Chat.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/docs/2-Concepts/Smart Instruct.md` & `agixt-1.2.7/docs/2-Concepts/Smart Instruct.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/docs/2-Concepts/Smart Task.md` & `agixt-1.2.7/docs/2-Concepts/Smart Task.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/docs/3-Providers/Anthropic Claude.md` & `agixt-1.2.7/docs/3-Providers/Anthropic Claude.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/docs/3-Providers/Azure OpenAI.md` & `agixt-1.2.7/docs/3-Providers/Azure OpenAI.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/docs/3-Providers/ChatGPT.md` & `agixt-1.2.7/docs/3-Providers/ChatGPT.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/docs/3-Providers/FastChat.md` & `agixt-1.2.7/docs/3-Providers/FastChat.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/docs/3-Providers/GPT4ALL-GPU.md` & `agixt-1.2.7/docs/3-Providers/GPT4ALL-GPU.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/docs/3-Providers/GPT4ALL.md` & `agixt-1.2.7/docs/3-Providers/GPT4ALL.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/docs/3-Providers/GPT4Free.md` & `agixt-1.2.7/docs/3-Providers/GPT4Free.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/docs/3-Providers/Google Bard.md` & `agixt-1.2.7/docs/3-Providers/Google Bard.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/docs/3-Providers/Hugging Face Transformers.md` & `agixt-1.2.7/docs/3-Providers/Hugging Face Transformers.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/docs/3-Providers/HuggingChat.md` & `agixt-1.2.7/docs/3-Providers/HuggingChat.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/docs/3-Providers/Microsoft Bing.md` & `agixt-1.2.7/docs/3-Providers/Microsoft Bing.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/docs/3-Providers/Oobabooga Text Generation Web UI.md` & `agixt-1.2.7/docs/3-Providers/Oobabooga Text Generation Web UI.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/docs/3-Providers/OpenAI.md` & `agixt-1.2.7/docs/3-Providers/OpenAI.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/docs/3-Providers/llamacpp API.md` & `agixt-1.2.7/docs/3-Providers/llamacpp API.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/docs/3-Providers/llamacpp.md` & `agixt-1.2.7/docs/3-Providers/llamacpp.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/docs/README.md` & `agixt-1.2.7/docs/README.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/docs/images/AGiXT-gradient-flat.svg` & `agixt-1.2.7/docs/images/AGiXT-gradient-flat.svg`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/docs/images/AGiXT-gradient-light.svg` & `agixt-1.2.7/docs/images/AGiXT-gradient-light.svg`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/docs/images/AGiXT.png` & `agixt-1.2.7/docs/images/AGiXT.png`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/docs/images/AGiXT.svg` & `agixt-1.2.7/docs/images/AGiXT.svg`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/docs/images/AGiXT_Original_PSD.psd` & `agixt-1.2.7/docs/images/AGiXT_Original_PSD.psd`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/docs/images/AGiXTwhiteborder.svg` & `agixt-1.2.7/docs/images/AGiXTwhiteborder.svg`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/docs/images/Docker-desktop-win-setting-streamlit.png` & `agixt-1.2.7/docs/images/Docker-desktop-win-setting-streamlit.png`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/docs/images/Smart Instruct.drawio` & `agixt-1.2.7/docs/images/Smart Instruct.drawio`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/docs/images/Smart Instruct.drawio.svg` & `agixt-1.2.7/docs/images/Smart Instruct.drawio.svg`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/docs/images/Smart Tasks.drawio` & `agixt-1.2.7/docs/images/Smart Tasks.drawio`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/docs/images/Smart Tasks.drawio.svg` & `agixt-1.2.7/docs/images/Smart Tasks.drawio.svg`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/docs/images/Untitled Diagram.drawio` & `agixt-1.2.7/docs/images/Untitled Diagram.drawio`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/setup.py` & `agixt-1.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/streamlit/ApiClient.py` & `agixt-1.2.7/streamlit/ApiClient.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/streamlit/Main.py` & `agixt-1.2.7/streamlit/Main.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/streamlit/auth_libs/Cfig.py` & `agixt-1.2.7/streamlit/auth_libs/Cfig.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/streamlit/auth_libs/Redirect.py` & `agixt-1.2.7/streamlit/auth_libs/Redirect.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/streamlit/auth_libs/Users.py` & `agixt-1.2.7/streamlit/auth_libs/Users.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/streamlit/auth_libs/pages/Login.py` & `agixt-1.2.7/streamlit/auth_libs/pages/Login.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/streamlit/auth_libs/pages/Profile.py` & `agixt-1.2.7/streamlit/auth_libs/pages/Profile.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/streamlit/auth_libs/pages/Register.py` & `agixt-1.2.7/streamlit/auth_libs/pages/Register.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/streamlit/components/chain.py` & `agixt-1.2.7/streamlit/components/chain.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/streamlit/components/docs.py` & `agixt-1.2.7/streamlit/components/docs.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/streamlit/components/learning.py` & `agixt-1.2.7/streamlit/components/learning.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/streamlit/components/selectors.py` & `agixt-1.2.7/streamlit/components/selectors.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/streamlit/components/verify_backend.py` & `agixt-1.2.7/streamlit/components/verify_backend.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/streamlit/pages/0-Agent_Settings.py` & `agixt-1.2.7/streamlit/pages/0-Agent_Settings.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/streamlit/pages/1-Prompt_Templates.py` & `agixt-1.2.7/streamlit/pages/1-Prompt_Templates.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/streamlit/pages/2-Chain_Management.py` & `agixt-1.2.7/streamlit/pages/2-Chain_Management.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,18 +14,20 @@
 
 agixt_docs()
 st.session_state = {}
 chain_names = ApiClient.get_chains()
 agents = ApiClient.get_agents()
 st.header("Chain Management")
 chain_action = st.selectbox("Action", ["Create Chain", "Modify Chain", "Delete Chain"])
-if chain_action == "Create Chain":
-    chain_name = st.text_input("Chain Name")
-else:
-    chain_name = st.selectbox("Chains", options=chain_names)
+
+# Replace this line
+# chain_name = st.text_input("Chain Name")
+
+# With this line
+chain_name = st.text_area("Chain Name")
 
 if chain_action == "Create Chain":
     action_button = st.button("Create New Chain")
     if action_button:
         if chain_name:
             ApiClient.add_chain(chain_name=chain_name)
             st.success(f"Chain '{chain_name}' created.")
```

### Comparing `agixt-1.2.6/streamlit/pages/3-Interact.py` & `agixt-1.2.7/streamlit/pages/3-Interact.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,16 +29,18 @@
 mode = st.selectbox("Select Mode", ["Prompt", "Chat", "Instruct", "Learning", "Chains"])
 
 if "chat_history" not in st.session_state:
     st.session_state["chat_history"] = ""
 
 agent_name = agent_selection() if mode != "Chains" else None
 
-if agent_name:
-    st.session_state["chat_history"] = get_history(agent_name=agent_name)
+
+with st.container():
+    if agent_name:
+        st.session_state["chat_history"] = get_history(agent_name=agent_name)
 
 
 # If the user selects Prompt, then show the prompt functionality
 if mode == "Prompt":
     st.markdown("### Choose an Agent and Prompt")
     # Add a dropdown to select a prompt
     prompt_name = st.selectbox("Choose a prompt", prompts)
@@ -47,15 +49,15 @@
 
     # Add input fields for prompt arguments
     st.markdown("### Prompt Variables")
     prompt_args_values = {}
     skip_args = ["command_list", "context", "COMMANDS", "date"]
     for arg in prompt_args:
         if arg not in skip_args:
-            prompt_args_values[arg] = st.text_input(arg)
+            prompt_args_values[arg] = st.text_area(arg)
 
     # Add a checkbox for websearch option
     websearch = st.checkbox("Enable websearch")
     websearch_depth = (
         3 if websearch else 0
     )  # Default depth is 3 if websearch is enabled
 
@@ -83,15 +85,15 @@
 
         # Print the response
         st.write(f"{agent_name}: {agent_prompt_resp}")
 
 if mode == "Chat":
     st.markdown("### Choose an Agent to Chat With")
     smart_chat_toggle = st.checkbox("Enable Smart Chat")
-    chat_prompt = st.text_input("Enter your message", key="chat_prompt")
+    chat_prompt = st.text_area("Enter your message", key="chat_prompt")
     send_button = st.button("Send Message")
 
     if send_button:
         if agent_name and chat_prompt:
             with st.spinner("Thinking, please wait..."):
                 if smart_chat_toggle:
                     response = ApiClient.smartchat(
@@ -104,15 +106,15 @@
                 if response:
                     st.experimental_rerun()
 
 
 if mode == "Instruct":
     st.markdown("### Choose an Agent to Instruct")
     smart_instruct_toggle = st.checkbox("Enable Smart Instruct")
-    instruct_prompt = st.text_input("Enter your instruction", key="instruct_prompt")
+    instruct_prompt = st.text_area("Enter your instruction", key="instruct_prompt")
     send_button = st.button("Send Message")
 
     if send_button:
         if agent_name and instruct_prompt:
             with st.spinner("Thinking, please wait..."):
                 if smart_instruct_toggle:
                     response = ApiClient.smartinstruct(
@@ -132,15 +134,15 @@
         learning_page(agent_name)
 
 if mode == "Chains":
     st.markdown("### Chain to Run")
     chain_names = ApiClient.get_chains()
     chain_action = "Run Chain"
     chain_name = st.selectbox("Chains", chain_names)
-    user_input = st.text_input("User Input")
+    user_input = st.text_area("User Input")
 
     if st.button("Perform Action"):
         if chain_name:
             if chain_action == "Run Chain":
                 responses = ApiClient.run_chain(
                     chain_name=chain_name, user_input=user_input
                 )
```

### Comparing `agixt-1.2.6/tests/ApiClient.py` & `agixt-1.2.7/tests/ApiClient.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/tests/test-commands.ipynb` & `agixt-1.2.7/tests/test-commands.ipynb`

 * *Files identical despite different names*

### Comparing `agixt-1.2.6/tests/tests.ipynb` & `agixt-1.2.7/tests/tests.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.993646023487891%*

 * *Differences: {"'cells'": '{3: {\'execution_count\': 111, \'outputs\': {0: {\'text\': ["Providers: '*

 * *            "['gpt4free', 'azure', 'chatgpt', 'runpod', 'poe', 'oobabooga', 'openai', "*

 * *            "'huggingface', 'fastchat', 'transformer', 'bing', 'palm', 'claude', 'gpt4all', "*

 * *            "'huggingchat', 'llamacppapi', 'kobold', 'llamacpp', 'gpugpt4all', "*

 * *            '\'bard\']\\n"]}}}, 5: {\'execution_count\': 112}, 7: {\'execution_count\': 113}, 9: '*

 * *            "{'execution_count': 114}, 11: {'execution_count':  […]*

```diff
@@ -24,22 +24,22 @@
                 "## Get Providers\n",
                 "\n",
                 "This will get a list of AI providers available to use with AGiXT.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 1,
+            "execution_count": 111,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Providers: ['gpt4free', 'azure', 'chatgpt', 'runpod', 'oobabooga', 'openai', 'huggingface', 'fastchat', 'transformer', 'bing', 'palm', 'claude', 'gpt4all', 'huggingchat', 'llamacppapi', 'kobold', 'llamacpp', 'gpugpt4all', 'bard']\n"
+                        "Providers: ['gpt4free', 'azure', 'chatgpt', 'runpod', 'poe', 'oobabooga', 'openai', 'huggingface', 'fastchat', 'transformer', 'bing', 'palm', 'claude', 'gpt4all', 'huggingchat', 'llamacppapi', 'kobold', 'llamacpp', 'gpugpt4all', 'bard']\n"
                     ]
                 }
             ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test get_providers()\n",
@@ -55,15 +55,15 @@
                 "## Get Default Provider Settings\n",
                 "\n",
                 "Choose a provider from the list of AI providers and get the default settings for that provider.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 112,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Settings for gpt4free: {'AI_MODEL': 'gpt-3.5-turbo', 'AI_TEMPERATURE': 0.7, 'MAX_TOKENS': 4000, 'provider': 'gpt4free'}\n"
@@ -87,15 +87,15 @@
                 "## Get Embedding Providers\n",
                 "\n",
                 "Embedding providers are used to embed information to vectors to store in the vector database to be searched for context injection.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 113,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Embed Providers: ['azure', 'cohere', 'default', 'embed_text', 'get_embedder', 'google_palm', 'google_vertex', 'large_local', 'llamacpp', 'openai']\n"
@@ -118,15 +118,15 @@
                 "## Get Extension Settings\n",
                 "\n",
                 "This is where we get all third party extension settings for the agent with defaults to fill in when there is nothing entered on the front end.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 114,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Extension Settings response: {'macostts': {'USE_MAC_OS_TTS': False}, 'file_system': {'WORKING_DIRECTORY': './WORKSPACE', 'WORKING_DIRECTORY_RESTRICTED': True}, 'huggingface': {'HUGGINGFACE_API_KEY': '', 'HUGGINGFACE_AUDIO_TO_TEXT_MODEL': 'facebook/wav2vec2-large-960h-lv60-self', 'WORKING_DIRECTORY': './WORKSPACE'}, 'discord': {'DISCORD_API_KEY': '', 'DISCORD_COMMAND_PREFIX': '/AGiXT'}, 'dalle': {'HUGGINGFACE_API_KEY': '', 'OPENAI_API_KEY': '', 'WORKING_DIRECTORY': './WORKSPACE'}, 'briantts': {'USE_BRIAN_TTS': True}, 'google': {'GOOGLE_API_KEY': ''}, 'microsoft_365': {'MICROSOFT_365_CLIENT_ID': '', 'MICROSOFT_365_CLIENT_SECRET': '', 'MICROSOFT_365_REDIRECT_URI': ''}, 'github': {'GITHUB_USERNAME': '', 'GITHUB_API_KEY': '', 'WORKING_DIRECTORY': './WORKSPACE'}, 'gtts': {'USE_GTTS': False}, 'elevenlabs': {'ELEVENLABS_API_KEY': '', 'ELEVENLABS_VOICE': 'Josh'}, 'sendgrid_email': {'SENDGRID_API_KEY': '', 'SENDGRID_EMAIL': ''}, 'searxng': {'SEARXNG_INSTANCE_URL': ''}, 'twitter': {'TW_CONSUMER_KEY': '', 'TW_CONSUMER_SECRET': '', 'TW_ACCESS_TOKEN': '', 'TW_ACCESS_TOKEN_SECRET': ''}}\n"
@@ -147,22 +147,22 @@
             "metadata": {},
             "source": [
                 "## Get Extension Commands\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 115,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Extensions response: [['Scrape Text with Playwright', 'scrape_text_with_playwright', {'url': None}], ['Scrape Links with Playwright', 'scrape_links_with_playwright', {'url': None}], ['Speak with MacOS TTS', 'speak_with_macos_speech', {'text': None, 'voice_index': 0}], ['Evaluate Code', 'evaluate_code', {'code': None, 'agent': 'AGiXT'}], ['Analyze Pull Request', 'analyze_pull_request', {'pr_url': None, 'agent': 'AGiXT'}], ['Perform Automated Testing', 'perform_automated_testing', {'test_url': None, 'agent': 'AGiXT'}], ['Run CI-CD Pipeline', 'run_ci_cd_pipeline', {'repo_url': None, 'agent': 'AGiXT'}], ['Improve Code', 'improve_code', {'suggestions': None, 'code': None, 'agent': 'AGiXT'}], ['Write Tests', 'write_tests', {'code': None, 'focus': None, 'agent': 'AGiXT'}], ['Create a new command', 'create_command', {'function_description': None, 'agent': 'AGiXT'}], ['Execute Task List', 'execute_task_list', {'agent': None, 'tasks': None, 'user_input': None, 'websearch': False, 'websearch_depth': 3, 'context_results': 5}], ['Prompt AI Agent', 'prompt_agent', {'user_input': None, 'prompt_name': None, 'prompt_args': None, 'websearch': False, 'websearch_depth': 3, 'context_results': 5, 'shots': 1}], ['Ask AI Agent Bing', 'ask', {'user_input': None, 'agent': 'AGiXT'}], ['Instruct AI Agent Bing', 'instruct', {'user_input': None, 'agent': 'AGiXT'}], ['Prompt AI Agent Bing', 'prompt_agent', {'user_input': None, 'prompt_name': None, 'prompt_args': None, 'websearch': False, 'websearch_depth': 3, 'context_results': 5, 'shots': 1}], ['Ask AI Agent gpt4free', 'ask', {'user_input': None, 'agent': 'AGiXT'}], ['Instruct AI Agent gpt4free', 'instruct', {'user_input': None, 'agent': 'AGiXT'}], ['Prompt AI Agent gpt4free', 'prompt_agent', {'user_input': None, 'prompt_name': None, 'prompt_args': None, 'websearch': False, 'websearch_depth': 3, 'context_results': 5, 'shots': 1}], ['Ask AI Agent Bard', 'ask', {'user_input': None, 'agent': 'AGiXT'}], ['Instruct AI Agent Bard', 'instruct', {'user_input': None, 'agent': 'AGiXT'}], ['Prompt AI Agent Bard', 'prompt_agent', {'user_input': None, 'prompt_name': None, 'prompt_args': None, 'websearch': False, 'websearch_depth': 3, 'context_results': 5, 'shots': 1}], ['Ask AI Agent Vicuna', 'ask', {'user_input': None, 'agent': 'AGiXT'}], ['Instruct AI Agent Vicuna', 'instruct', {'user_input': None, 'agent': 'AGiXT'}], ['Prompt AI Agent Vicuna', 'prompt_agent', {'user_input': None, 'prompt_name': None, 'prompt_args': None, 'websearch': False, 'websearch_depth': 3, 'context_results': 5, 'shots': 1}], ['Ask AI Agent OpenAI', 'ask', {'user_input': None, 'agent': 'AGiXT'}], ['Instruct AI Agent OpenAI', 'instruct', {'user_input': None, 'agent': 'AGiXT'}], ['Prompt AI Agent OpenAI', 'prompt_agent', {'user_input': None, 'prompt_name': None, 'prompt_args': None, 'websearch': False, 'websearch_depth': 3, 'context_results': 5, 'shots': 1}], ['Ask AI Agent azure', 'ask', {'user_input': None, 'agent': 'AGiXT'}], ['Instruct AI Agent azure', 'instruct', {'user_input': None, 'agent': 'AGiXT'}], ['Prompt AI Agent azure', 'prompt_agent', {'user_input': None, 'prompt_name': None, 'prompt_args': None, 'websearch': False, 'websearch_depth': 3, 'context_results': 5, 'shots': 1}], ['Ask AI Agent ChatGPT', 'ask', {'user_input': None, 'agent': 'AGiXT'}], ['Instruct AI Agent ChatGPT', 'instruct', {'user_input': None, 'agent': 'AGiXT'}], ['Prompt AI Agent ChatGPT', 'prompt_agent', {'user_input': None, 'prompt_name': None, 'prompt_args': None, 'websearch': False, 'websearch_depth': 3, 'context_results': 5, 'shots': 1}], ['Ask AI Agent Guanaco', 'ask', {'user_input': None, 'agent': 'AGiXT'}], ['Instruct AI Agent Guanaco', 'instruct', {'user_input': None, 'agent': 'AGiXT'}], ['Prompt AI Agent Guanaco', 'prompt_agent', {'user_input': None, 'prompt_name': None, 'prompt_args': None, 'websearch': False, 'websearch_depth': 3, 'context_results': 5, 'shots': 1}], ['Write to File', 'write_to_file', {'filename': None, 'text': None}], ['Read File', 'read_file', {'filename': None}], ['Search Files', 'search_files', {'directory': None}], ['Append to File', 'append_to_file', {'filename': None, 'text': None}], ['Execute Python File', 'execute_python_file', {'file': None}], ['Delete File', 'delete_file', {'filename': None}], ['Execute Shell', 'execute_shell', {'command_line': None}], ['Read Audio from File', 'read_audio_from_file', {'audio_path': None}], ['Read Audio', 'read_audio', {'audio': None}], ['Generate Image with Stable Diffusion', 'generate_image_with_hf', {'prompt': None, 'filename': None}], ['Speak with TTS with BrianTTS', 'speak_with_briantts', {'text': None}], ['Clone Github Repository', 'clone_repo', {'repo_url': None, 'clone_path': None}], ['Get Datetime', 'get_datetime', {}], ['Speak with TTS Using Elevenlabs', 'speak_with_elevenlabs', {'text': None, 'voice_index': 0}], ['Use The Search Engine', 'search', {'query': None}]]\n"
+                        "Extensions response: [['Scrape Text with Playwright', 'scrape_text_with_playwright', {'url': None}], ['Scrape Links with Playwright', 'scrape_links_with_playwright', {'url': None}], ['Speak with MacOS TTS', 'speak_with_macos_speech', {'text': None, 'voice_index': 0}], ['Evaluate Code', 'evaluate_code', {'code': None, 'agent': 'AGiXT'}], ['Analyze Pull Request', 'analyze_pull_request', {'pr_url': None, 'agent': 'AGiXT'}], ['Perform Automated Testing', 'perform_automated_testing', {'test_url': None, 'agent': 'AGiXT'}], ['Run CI-CD Pipeline', 'run_ci_cd_pipeline', {'repo_url': None, 'agent': 'AGiXT'}], ['Improve Code', 'improve_code', {'suggestions': None, 'code': None, 'agent': 'AGiXT'}], ['Write Tests', 'write_tests', {'code': None, 'focus': None, 'agent': 'AGiXT'}], ['Create a new command', 'create_command', {'function_description': None, 'agent': 'AGiXT'}], ['Describe Image', 'describe_image', {'image_url': None}], ['Ask AI Agent Bing', 'ask', {'user_input': None, 'agent': 'AGiXT'}], ['Instruct AI Agent Bing', 'instruct', {'user_input': None, 'agent': 'AGiXT'}], ['Ask AI Agent tester', 'ask', {'user_input': None, 'agent': 'AGiXT'}], ['Instruct AI Agent tester', 'instruct', {'user_input': None, 'agent': 'AGiXT'}], ['Ask AI Agent gpt4free', 'ask', {'user_input': None, 'agent': 'AGiXT'}], ['Instruct AI Agent gpt4free', 'instruct', {'user_input': None, 'agent': 'AGiXT'}], ['Ask AI Agent Bard', 'ask', {'user_input': None, 'agent': 'AGiXT'}], ['Instruct AI Agent Bard', 'instruct', {'user_input': None, 'agent': 'AGiXT'}], ['Ask AI Agent Vicuna', 'ask', {'user_input': None, 'agent': 'AGiXT'}], ['Instruct AI Agent Vicuna', 'instruct', {'user_input': None, 'agent': 'AGiXT'}], ['Ask AI Agent OpenAI', 'ask', {'user_input': None, 'agent': 'AGiXT'}], ['Instruct AI Agent OpenAI', 'instruct', {'user_input': None, 'agent': 'AGiXT'}], ['Ask AI Agent azure', 'ask', {'user_input': None, 'agent': 'AGiXT'}], ['Instruct AI Agent azure', 'instruct', {'user_input': None, 'agent': 'AGiXT'}], ['Ask AI Agent ChatGPT', 'ask', {'user_input': None, 'agent': 'AGiXT'}], ['Instruct AI Agent ChatGPT', 'instruct', {'user_input': None, 'agent': 'AGiXT'}], ['Ask AI Agent Guanaco', 'ask', {'user_input': None, 'agent': 'AGiXT'}], ['Instruct AI Agent Guanaco', 'instruct', {'user_input': None, 'agent': 'AGiXT'}], ['Write to File', 'write_to_file', {'filename': None, 'text': None}], ['Read File', 'read_file', {'filename': None}], ['Search Files', 'search_files', {'directory': None}], ['Append to File', 'append_to_file', {'filename': None, 'text': None}], ['Execute Python File', 'execute_python_file', {'file': None}], ['Delete File', 'delete_file', {'filename': None}], ['Execute Shell', 'execute_shell', {'command_line': None}], ['Read Audio from File', 'read_audio_from_file', {'audio_path': None}], ['Read Audio', 'read_audio', {'audio': None}], ['Generate Image with Stable Diffusion', 'generate_image_with_hf', {'prompt': None, 'filename': None}], ['Speak with TTS with BrianTTS', 'speak_with_briantts', {'text': None}], ['Clone Github Repository', 'clone_repo', {'repo_url': None, 'clone_path': None}], ['Get Datetime', 'get_datetime', {}], ['Speak with TTS Using Elevenlabs', 'speak_with_elevenlabs', {'text': None, 'voice_index': 0}], ['Use The Search Engine', 'search', {'query': None}], ['Create Task Chain', 'create_task_chain', {'agent': None, 'primary_objective': None, 'numbered_list_of_tasks': None, 'short_task_description': None}], ['Create Smart Task Chain', 'create_smart_task_chain', {'agent': None, 'primary_objective': None, 'numbered_list_of_tasks': None, 'short_task_description': None}]]\n"
                     ]
                 }
             ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test get_extensions()\n",
@@ -178,22 +178,22 @@
                 "## Get a list of all current Agents\n",
                 "\n",
                 "Any agents that you have created will be listed here. The `status` field is to say if the agent is currently running a task or not.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 116,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Agents: [{'name': 'Bing', 'status': False}, {'name': 'gpt4free', 'status': False}, {'name': 'Bard', 'status': False}, {'name': 'Vicuna', 'status': False}, {'name': 'OpenAI', 'status': False}, {'name': 'azure', 'status': False}, {'name': 'ChatGPT', 'status': False}, {'name': 'Guanaco', 'status': False}]\n"
+                        "Agents: [{'name': 'Bing', 'status': False}, {'name': 'tester', 'status': False}, {'name': 'gpt4free', 'status': False}, {'name': 'Bard', 'status': False}, {'name': 'Vicuna', 'status': False}, {'name': 'OpenAI', 'status': False}, {'name': 'azure', 'status': False}, {'name': 'ChatGPT', 'status': False}, {'name': 'Guanaco', 'status': False}]\n"
                     ]
                 }
             ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test get_agents()\n",
@@ -209,15 +209,15 @@
                 "## Create a new Agent\n",
                 "\n",
                 "Creates a new agent with the `gpt4free` provider. We'll use `gpt4free` because it is the one that requires the least configuration.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 117,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Add agent response: {'message': 'Agent test_agent created.'}\n"
@@ -245,15 +245,15 @@
                 "## Rename the test agent\n",
                 "\n",
                 "We will just rename it to `new_agent`.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 118,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Rename agent response: {'message': 'Agent renamed.'}\n"
@@ -280,22 +280,22 @@
                 "## Get the agent's settings\n",
                 "\n",
                 "This will get the settings for the agent we just created, this will tell you all commands available to the agent as well as all of the provider settings for the agent.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 119,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Config for new_agent: {'commands': {'Scrape Text with Playwright': False, 'Scrape Links with Playwright': False, 'Speak with MacOS TTS': False, 'Evaluate Code': False, 'Analyze Pull Request': False, 'Perform Automated Testing': False, 'Run CI-CD Pipeline': False, 'Improve Code': False, 'Write Tests': False, 'Create a new command': False, 'Execute Task List': False, 'Prompt AI Agent': False, 'Ask AI Agent Bing': False, 'Instruct AI Agent Bing': False, 'Prompt AI Agent Bing': False, 'Ask AI Agent gpt4free': False, 'Instruct AI Agent gpt4free': False, 'Prompt AI Agent gpt4free': False, 'Ask AI Agent Bard': False, 'Instruct AI Agent Bard': False, 'Prompt AI Agent Bard': False, 'Ask AI Agent Vicuna': False, 'Instruct AI Agent Vicuna': False, 'Prompt AI Agent Vicuna': False, 'Ask AI Agent OpenAI': False, 'Instruct AI Agent OpenAI': False, 'Prompt AI Agent OpenAI': False, 'Ask AI Agent azure': False, 'Instruct AI Agent azure': False, 'Prompt AI Agent azure': False, 'Ask AI Agent ChatGPT': False, 'Instruct AI Agent ChatGPT': False, 'Prompt AI Agent ChatGPT': False, 'Ask AI Agent new_agent': False, 'Instruct AI Agent new_agent': False, 'Prompt AI Agent new_agent': False, 'Ask AI Agent Guanaco': False, 'Instruct AI Agent Guanaco': False, 'Prompt AI Agent Guanaco': False, 'Write to File': False, 'Read File': False, 'Search Files': False, 'Append to File': False, 'Execute Python File': False, 'Delete File': False, 'Execute Shell': False, 'Read Audio from File': False, 'Read Audio': False, 'Generate Image with Stable Diffusion': False, 'Speak with TTS with BrianTTS': False, 'Clone Github Repository': False, 'Get Datetime': False, 'Speak with TTS Using Elevenlabs': False, 'Use The Search Engine': False}, 'settings': {'AI_MODEL': 'gpt-3.5-turbo', 'AI_TEMPERATURE': 0.7, 'MAX_TOKENS': 4000, 'provider': 'gpt4free'}}\n"
+                        "Config for new_agent: {'commands': {'Scrape Text with Playwright': False, 'Scrape Links with Playwright': False, 'Speak with MacOS TTS': False, 'Evaluate Code': False, 'Analyze Pull Request': False, 'Perform Automated Testing': False, 'Run CI-CD Pipeline': False, 'Improve Code': False, 'Write Tests': False, 'Create a new command': False, 'Describe Image': False, 'Ask AI Agent Bing': False, 'Instruct AI Agent Bing': False, 'Ask AI Agent tester': False, 'Instruct AI Agent tester': False, 'Ask AI Agent gpt4free': False, 'Instruct AI Agent gpt4free': False, 'Ask AI Agent Bard': False, 'Instruct AI Agent Bard': False, 'Ask AI Agent Vicuna': False, 'Instruct AI Agent Vicuna': False, 'Ask AI Agent OpenAI': False, 'Instruct AI Agent OpenAI': False, 'Ask AI Agent azure': False, 'Instruct AI Agent azure': False, 'Ask AI Agent ChatGPT': False, 'Instruct AI Agent ChatGPT': False, 'Ask AI Agent new_agent': False, 'Instruct AI Agent new_agent': False, 'Ask AI Agent Guanaco': False, 'Instruct AI Agent Guanaco': False, 'Write to File': False, 'Read File': False, 'Search Files': False, 'Append to File': False, 'Execute Python File': False, 'Delete File': False, 'Execute Shell': False, 'Read Audio from File': False, 'Read Audio': False, 'Generate Image with Stable Diffusion': False, 'Speak with TTS with BrianTTS': False, 'Clone Github Repository': False, 'Get Datetime': False, 'Speak with TTS Using Elevenlabs': False, 'Use The Search Engine': False, 'Create Task Chain': False, 'Create Smart Task Chain': False}, 'settings': {'AI_MODEL': 'gpt-3.5-turbo', 'AI_TEMPERATURE': 0.7, 'MAX_TOKENS': 4000, 'provider': 'gpt4free'}}\n"
                     ]
                 }
             ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test get_agentconfig()\n",
@@ -312,23 +312,23 @@
                 "## Update the agent's settings\n",
                 "\n",
                 "We'll just update the temperature from the default `0.7` to `0.5` to confirm that we can modify a setting.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 120,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Update agent settings response: Agent new_agent configuration updated.\n",
-                        "New config for new_agent: {'commands': {'Scrape Text with Playwright': False, 'Scrape Links with Playwright': False, 'Speak with MacOS TTS': False, 'Evaluate Code': False, 'Analyze Pull Request': False, 'Perform Automated Testing': False, 'Run CI-CD Pipeline': False, 'Improve Code': False, 'Write Tests': False, 'Create a new command': False, 'Execute Task List': False, 'Prompt AI Agent': False, 'Ask AI Agent Bing': False, 'Instruct AI Agent Bing': False, 'Prompt AI Agent Bing': False, 'Ask AI Agent gpt4free': False, 'Instruct AI Agent gpt4free': False, 'Prompt AI Agent gpt4free': False, 'Ask AI Agent Bard': False, 'Instruct AI Agent Bard': False, 'Prompt AI Agent Bard': False, 'Ask AI Agent Vicuna': False, 'Instruct AI Agent Vicuna': False, 'Prompt AI Agent Vicuna': False, 'Ask AI Agent OpenAI': False, 'Instruct AI Agent OpenAI': False, 'Prompt AI Agent OpenAI': False, 'Ask AI Agent azure': False, 'Instruct AI Agent azure': False, 'Prompt AI Agent azure': False, 'Ask AI Agent ChatGPT': False, 'Instruct AI Agent ChatGPT': False, 'Prompt AI Agent ChatGPT': False, 'Ask AI Agent new_agent': False, 'Instruct AI Agent new_agent': False, 'Prompt AI Agent new_agent': False, 'Ask AI Agent Guanaco': False, 'Instruct AI Agent Guanaco': False, 'Prompt AI Agent Guanaco': False, 'Write to File': False, 'Read File': False, 'Search Files': False, 'Append to File': False, 'Execute Python File': False, 'Delete File': False, 'Execute Shell': False, 'Read Audio from File': False, 'Read Audio': False, 'Generate Image with Stable Diffusion': False, 'Speak with TTS with BrianTTS': False, 'Clone Github Repository': False, 'Get Datetime': False, 'Speak with TTS Using Elevenlabs': False, 'Use The Search Engine': False}, 'settings': {'AI_MODEL': 'gpt-3.5-turbo', 'AI_TEMPERATURE': 0.5, 'MAX_TOKENS': 4000, 'provider': 'gpt4free'}}\n"
+                        "New config for new_agent: {'commands': {'Scrape Text with Playwright': False, 'Scrape Links with Playwright': False, 'Speak with MacOS TTS': False, 'Evaluate Code': False, 'Analyze Pull Request': False, 'Perform Automated Testing': False, 'Run CI-CD Pipeline': False, 'Improve Code': False, 'Write Tests': False, 'Create a new command': False, 'Describe Image': False, 'Ask AI Agent Bing': False, 'Instruct AI Agent Bing': False, 'Ask AI Agent tester': False, 'Instruct AI Agent tester': False, 'Ask AI Agent gpt4free': False, 'Instruct AI Agent gpt4free': False, 'Ask AI Agent Bard': False, 'Instruct AI Agent Bard': False, 'Ask AI Agent Vicuna': False, 'Instruct AI Agent Vicuna': False, 'Ask AI Agent OpenAI': False, 'Instruct AI Agent OpenAI': False, 'Ask AI Agent azure': False, 'Instruct AI Agent azure': False, 'Ask AI Agent ChatGPT': False, 'Instruct AI Agent ChatGPT': False, 'Ask AI Agent new_agent': False, 'Instruct AI Agent new_agent': False, 'Ask AI Agent Guanaco': False, 'Instruct AI Agent Guanaco': False, 'Write to File': False, 'Read File': False, 'Search Files': False, 'Append to File': False, 'Execute Python File': False, 'Delete File': False, 'Execute Shell': False, 'Read Audio from File': False, 'Read Audio': False, 'Generate Image with Stable Diffusion': False, 'Speak with TTS with BrianTTS': False, 'Clone Github Repository': False, 'Get Datetime': False, 'Speak with TTS Using Elevenlabs': False, 'Use The Search Engine': False, 'Create Task Chain': False, 'Create Smart Task Chain': False}, 'settings': {'AI_MODEL': 'gpt-3.5-turbo', 'AI_TEMPERATURE': 0.5, 'MAX_TOKENS': 4000, 'provider': 'gpt4free'}}\n"
                     ]
                 }
             ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test update_agent_settings()\n",
@@ -353,22 +353,22 @@
                 "## Get a list of the agent's commands\n",
                 "\n",
                 "This will get a list of all commands available to the agent.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 121,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Commands: {'Scrape Text with Playwright': False, 'Scrape Links with Playwright': False, 'Speak with MacOS TTS': False, 'Evaluate Code': False, 'Analyze Pull Request': False, 'Perform Automated Testing': False, 'Run CI-CD Pipeline': False, 'Improve Code': False, 'Write Tests': False, 'Create a new command': False, 'Execute Task List': False, 'Prompt AI Agent': False, 'Ask AI Agent Bing': False, 'Instruct AI Agent Bing': False, 'Prompt AI Agent Bing': False, 'Ask AI Agent gpt4free': False, 'Instruct AI Agent gpt4free': False, 'Prompt AI Agent gpt4free': False, 'Ask AI Agent Bard': False, 'Instruct AI Agent Bard': False, 'Prompt AI Agent Bard': False, 'Ask AI Agent Vicuna': False, 'Instruct AI Agent Vicuna': False, 'Prompt AI Agent Vicuna': False, 'Ask AI Agent OpenAI': False, 'Instruct AI Agent OpenAI': False, 'Prompt AI Agent OpenAI': False, 'Ask AI Agent azure': False, 'Instruct AI Agent azure': False, 'Prompt AI Agent azure': False, 'Ask AI Agent ChatGPT': False, 'Instruct AI Agent ChatGPT': False, 'Prompt AI Agent ChatGPT': False, 'Ask AI Agent new_agent': False, 'Instruct AI Agent new_agent': False, 'Prompt AI Agent new_agent': False, 'Ask AI Agent Guanaco': False, 'Instruct AI Agent Guanaco': False, 'Prompt AI Agent Guanaco': False, 'Write to File': False, 'Read File': False, 'Search Files': False, 'Append to File': False, 'Execute Python File': False, 'Delete File': False, 'Execute Shell': False, 'Read Audio from File': False, 'Read Audio': False, 'Generate Image with Stable Diffusion': False, 'Speak with TTS with BrianTTS': False, 'Clone Github Repository': False, 'Get Datetime': False, 'Speak with TTS Using Elevenlabs': False, 'Use The Search Engine': False}\n"
+                        "Commands: {'Scrape Text with Playwright': False, 'Scrape Links with Playwright': False, 'Speak with MacOS TTS': False, 'Evaluate Code': False, 'Analyze Pull Request': False, 'Perform Automated Testing': False, 'Run CI-CD Pipeline': False, 'Improve Code': False, 'Write Tests': False, 'Create a new command': False, 'Describe Image': False, 'Ask AI Agent Bing': False, 'Instruct AI Agent Bing': False, 'Ask AI Agent tester': False, 'Instruct AI Agent tester': False, 'Ask AI Agent gpt4free': False, 'Instruct AI Agent gpt4free': False, 'Ask AI Agent Bard': False, 'Instruct AI Agent Bard': False, 'Ask AI Agent Vicuna': False, 'Instruct AI Agent Vicuna': False, 'Ask AI Agent OpenAI': False, 'Instruct AI Agent OpenAI': False, 'Ask AI Agent azure': False, 'Instruct AI Agent azure': False, 'Ask AI Agent ChatGPT': False, 'Instruct AI Agent ChatGPT': False, 'Ask AI Agent new_agent': False, 'Instruct AI Agent new_agent': False, 'Ask AI Agent Guanaco': False, 'Instruct AI Agent Guanaco': False, 'Write to File': False, 'Read File': False, 'Search Files': False, 'Append to File': False, 'Execute Python File': False, 'Delete File': False, 'Execute Shell': False, 'Read Audio from File': False, 'Read Audio': False, 'Generate Image with Stable Diffusion': False, 'Speak with TTS with BrianTTS': False, 'Clone Github Repository': False, 'Get Datetime': False, 'Speak with TTS Using Elevenlabs': False, 'Use The Search Engine': False, 'Create Task Chain': False, 'Create Smart Task Chain': False}\n"
                     ]
                 }
             ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test get_commands()\n",
@@ -385,15 +385,15 @@
                 "## Toggle a Command for the Agent\n",
                 "\n",
                 "We'll toggle the `Write to File` command to `true` to confirm that we can toggle a command.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": 122,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Toggle command response: Command 'Write to File' toggled for agent 'new_agent'.\n"
@@ -418,15 +418,15 @@
                 "## Chat with the Agent\n",
                 "\n",
                 "We'll chat with the agent to confirm that it is working. We'll ask a simple question like `What is the capital of France?`\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": 123,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Chat response: The capital of France is Paris.\n"
@@ -452,45 +452,45 @@
                 "## Prompt the Agent\n",
                 "\n",
                 "Use a custom Prompt Template to prompt the agent. For our example, we'll use our \"Write a Poem\" prompt template to have the agent write a poem for us about dragons.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": 124,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Agent prompt response: In the sky they soar\n",
-                        "With flames of fire they roar\n",
-                        "Majestic creatures of lore\n",
-                        "The dragons we adore\n",
+                        "Agent prompt response: In a land of fire and stone,\n",
+                        "Where dragons reign and wander alone,\n",
+                        "Their scales as hard as any stone,\n",
+                        "Their eyes as bright as the sun's own throne.\n",
                         "\n",
-                        "Their scales shimmer in the sun\n",
-                        "A sight that can't be outdone\n",
-                        "Powerful beings second to none\n",
-                        "They make our hearts run\n",
+                        "They fly through skies of blue and red,\n",
+                        "And breathe out flames that can leave you dead,\n",
+                        "Horned beasts with sharp-toothed grins,\n",
+                        "That strike fear in the hearts of mortal men.\n",
                         "\n",
-                        "Through mountains they fly\n",
-                        "With wings that reach the sky\n",
-                        "A sight that makes us sigh\n",
-                        "Our spirits begin to rise high\n",
+                        "Their wings move swift in the air,\n",
+                        "And their roars make kingdoms shake with care,\n",
+                        "Gold and jewels they hold in their keep,\n",
+                        "And woe to those who dare to steal or creep.\n",
                         "\n",
-                        "Legends of them surround\n",
-                        "As their presence astounds\n",
-                        "Bringers of both fear and renown\n",
-                        "The dragons are all around\n",
+                        "Yet for all their strength and might,\n",
+                        "These creatures have a heart that's bright,\n",
+                        "They guard the sky with all their might,\n",
+                        "And in their lair they sleep at night.\n",
                         "\n",
-                        "Their beauty and might\n",
-                        "Enchants us through the night\n",
-                        "A sight that's truly a delight\n",
-                        "The dragons, our hearts take flight\n"
+                        "So let us honor these mighty beasts,\n",
+                        "For they are creatures we should please,\n",
+                        "With respect and homage we should treat,\n",
+                        "These dragons fierce and full of heat.\n"
                     ]
                 }
             ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test prompt_agent()\n",
@@ -521,22 +521,31 @@
                 "## Instruct the Agent to do something\n",
                 "\n",
                 "We'll do something simple with it for the sake of the basic example, we'll just tell it to `Tell me the capital of France`.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
+            "execution_count": 125,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Instruct response: The capital of France is Paris.\n"
+                        "Instruct response: The capital of France is Paris.\n",
+                        "\n",
+                        "Commands Executed:\n",
+                        "{'Write to File': {'filename': 'france_capital.txt', 'text': 'Paris'}}\n",
+                        "\n",
+                        "Command Execution Response:\n",
+                        "\n",
+                        "Executed Command:Write to File with args {'filename': 'france_capital.txt', 'text': 'Paris'}.\n",
+                        "Command Output: File written to successfully.\n",
+                        "\n"
                     ]
                 }
             ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test instruct()\n",
@@ -555,22 +564,22 @@
                 "## Chat History of the Agent\n",
                 "\n",
                 "Get the chat history from the Agent.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
+            "execution_count": 126,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Chat history: [{'USER': 'June 11, 2023 02:15 PM\\nWhat is the capital of France?'}, {'new_agent': 'June 11, 2023 02:15 PM\\nThe capital of France is Paris.'}, {'USER': 'June 11, 2023 02:15 PM\\n'}, {'new_agent': \"June 11, 2023 02:15 PM\\nIn the sky they soar\\nWith flames of fire they roar\\nMajestic creatures of lore\\nThe dragons we adore\\n\\nTheir scales shimmer in the sun\\nA sight that can't be outdone\\nPowerful beings second to none\\nThey make our hearts run\\n\\nThrough mountains they fly\\nWith wings that reach the sky\\nA sight that makes us sigh\\nOur spirits begin to rise high\\n\\nLegends of them surround\\nAs their presence astounds\\nBringers of both fear and renown\\nThe dragons are all around\\n\\nTheir beauty and might\\nEnchants us through the night\\nA sight that's truly a delight\\nThe dragons, our hearts take flight\"}, {'USER': 'June 11, 2023 02:15 PM\\nTell me the capital of France.'}, {'new_agent': 'June 11, 2023 02:15 PM\\nThe capital of France is Paris.'}]\n"
+                        "Chat history: [{'USER': 'June 12, 2023 09:54 PM\\nWhat is the capital of France?'}, {'new_agent': 'June 12, 2023 09:54 PM\\nThe capital of France is Paris.'}, {'USER': 'June 12, 2023 09:54 PM\\nWrite a poem about dragons .\\n'}, {'new_agent': \"June 12, 2023 09:54 PM\\nIn a land of fire and stone,\\nWhere dragons reign and wander alone,\\nTheir scales as hard as any stone,\\nTheir eyes as bright as the sun's own throne.\\n\\nThey fly through skies of blue and red,\\nAnd breathe out flames that can leave you dead,\\nHorned beasts with sharp-toothed grins,\\nThat strike fear in the hearts of mortal men.\\n\\nTheir wings move swift in the air,\\nAnd their roars make kingdoms shake with care,\\nGold and jewels they hold in their keep,\\nAnd woe to those who dare to steal or creep.\\n\\nYet for all their strength and might,\\nThese creatures have a heart that's bright,\\nThey guard the sky with all their might,\\nAnd in their lair they sleep at night.\\n\\nSo let us honor these mighty beasts,\\nFor they are creatures we should please,\\nWith respect and homage we should treat,\\nThese dragons fierce and full of heat.\"}, {'USER': 'June 12, 2023 09:54 PM\\nCommands Available To Complete Task:\\n`Write to File` - Arguments: {\\'filename\\': None, \\'text\\': None}\\n\\n\\nYou are an AI language model. Your name is {AGENT_NAME}. Your role is to do anything asked of you with precision. You have the following constraints:\\n1. ~4000 word limit for short term memory. Your short term memory is short, so immediately save important information to files.\\n2. If you are unsure how you previously did something or want to recall past events, thinking about similar events will help you remember.\\n3. No user assistance.\\n4. Exclusively use the commands listed in double quotes e.g. \"command name\".\\n\\nYou have the following resources:\\n1. Internet access for searches and information gathering.\\n2. Long Term memory management.\\n3. GPT-3.5 powered Agents for delegation of simple tasks.\\n4. File output.\\n\\nRESPOND IN THE FOLLOWING JSON FORMAT ONLY! If there are no commands, simply make the commands section an empty object like {}.\\n```JSON\\n{\\n    \"response\": \"Your response to the task.\",\\n    \"commands\": {\\n        \"command_name\": {\\n            \"arg1\": \"val1\",\\n            \"arg2\": \"val2\"\\n        },\\n        \"command_name2\": {\\n            \"arg1\": \"val1\",\\n            \"arg2\": \"val2\",\\n            \"argN\": \"valN\"\\n        }\\n    }\\n}\\n```\\n\\nYour task: Tell me the capital of France.'}, {'new_agent': \"June 12, 2023 09:54 PM\\nThe capital of France is Paris.\\n\\nCommands Executed:\\n{'Write to File': {'filename': 'france_capital.txt', 'text': 'Paris'}}\\n\\nCommand Execution Response:\\n\\nExecuted Command:Write to File with args {'filename': 'france_capital.txt', 'text': 'Paris'}.\\nCommand Output: File written to successfully.\\n\"}]\n"
                     ]
                 }
             ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test get_chat_history()\n",
@@ -587,23 +596,23 @@
                 "## Update Agent Commands\n",
                 "\n",
                 "In this example, we'll only change the `Write to File` command to `False`, but we could change any (or all) of the commands with this API call.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 17,
+            "execution_count": 127,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Update agent commands response: Agent new_agent configuration updated.\n",
-                        "New config for new_agent: {'commands': {'Scrape Text with Playwright': False, 'Scrape Links with Playwright': False, 'Speak with MacOS TTS': False, 'Evaluate Code': False, 'Analyze Pull Request': False, 'Perform Automated Testing': False, 'Run CI-CD Pipeline': False, 'Improve Code': False, 'Write Tests': False, 'Create a new command': False, 'Execute Task List': False, 'Prompt AI Agent': False, 'Ask AI Agent Bing': False, 'Instruct AI Agent Bing': False, 'Prompt AI Agent Bing': False, 'Ask AI Agent gpt4free': False, 'Instruct AI Agent gpt4free': False, 'Prompt AI Agent gpt4free': False, 'Ask AI Agent Bard': False, 'Instruct AI Agent Bard': False, 'Prompt AI Agent Bard': False, 'Ask AI Agent Vicuna': False, 'Instruct AI Agent Vicuna': False, 'Prompt AI Agent Vicuna': False, 'Ask AI Agent OpenAI': False, 'Instruct AI Agent OpenAI': False, 'Prompt AI Agent OpenAI': False, 'Ask AI Agent azure': False, 'Instruct AI Agent azure': False, 'Prompt AI Agent azure': False, 'Ask AI Agent ChatGPT': False, 'Instruct AI Agent ChatGPT': False, 'Prompt AI Agent ChatGPT': False, 'Ask AI Agent new_agent': False, 'Instruct AI Agent new_agent': False, 'Prompt AI Agent new_agent': False, 'Ask AI Agent Guanaco': False, 'Instruct AI Agent Guanaco': False, 'Prompt AI Agent Guanaco': False, 'Write to File': False, 'Read File': False, 'Search Files': False, 'Append to File': False, 'Execute Python File': False, 'Delete File': False, 'Execute Shell': False, 'Read Audio from File': False, 'Read Audio': False, 'Generate Image with Stable Diffusion': False, 'Speak with TTS with BrianTTS': False, 'Clone Github Repository': False, 'Get Datetime': False, 'Speak with TTS Using Elevenlabs': False, 'Use The Search Engine': False}, 'settings': {'AI_MODEL': 'gpt-3.5-turbo', 'AI_TEMPERATURE': 0.5, 'MAX_TOKENS': 4000, 'provider': 'gpt4free'}}\n"
+                        "New config for new_agent: {'commands': {'Scrape Text with Playwright': False, 'Scrape Links with Playwright': False, 'Speak with MacOS TTS': False, 'Evaluate Code': False, 'Analyze Pull Request': False, 'Perform Automated Testing': False, 'Run CI-CD Pipeline': False, 'Improve Code': False, 'Write Tests': False, 'Create a new command': False, 'Describe Image': False, 'Ask AI Agent Bing': False, 'Instruct AI Agent Bing': False, 'Ask AI Agent tester': False, 'Instruct AI Agent tester': False, 'Ask AI Agent gpt4free': False, 'Instruct AI Agent gpt4free': False, 'Ask AI Agent Bard': False, 'Instruct AI Agent Bard': False, 'Ask AI Agent Vicuna': False, 'Instruct AI Agent Vicuna': False, 'Ask AI Agent OpenAI': False, 'Instruct AI Agent OpenAI': False, 'Ask AI Agent azure': False, 'Instruct AI Agent azure': False, 'Ask AI Agent ChatGPT': False, 'Instruct AI Agent ChatGPT': False, 'Ask AI Agent new_agent': False, 'Instruct AI Agent new_agent': False, 'Ask AI Agent Guanaco': False, 'Instruct AI Agent Guanaco': False, 'Write to File': False, 'Read File': False, 'Search Files': False, 'Append to File': False, 'Execute Python File': False, 'Delete File': False, 'Execute Shell': False, 'Read Audio from File': False, 'Read Audio': False, 'Generate Image with Stable Diffusion': False, 'Speak with TTS with BrianTTS': False, 'Clone Github Repository': False, 'Get Datetime': False, 'Speak with TTS Using Elevenlabs': False, 'Use The Search Engine': False, 'Create Task Chain': False, 'Create Smart Task Chain': False}, 'settings': {'AI_MODEL': 'gpt-3.5-turbo', 'AI_TEMPERATURE': 0.5, 'MAX_TOKENS': 4000, 'provider': 'gpt4free'}}\n"
                     ]
                 }
             ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test update_agent_commands()\n",
@@ -625,15 +634,15 @@
             "metadata": {},
             "source": [
                 "## Have the Agent Learn from a File\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 18,
+            "execution_count": 128,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "File Learning response: Agent learned the content from the file.\n"
@@ -657,15 +666,15 @@
             "metadata": {},
             "source": [
                 "## Have the Agent Learn from a URL\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 19,
+            "execution_count": 129,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "URL Learning response: Agent learned the content from the url.\n"
@@ -689,15 +698,15 @@
                 "## Wipe the agents memories\n",
                 "\n",
                 "This is necessary if you want the agent to serve a different purpose than its original intent after it has learned things. It may inject unnecessary context into the conversation if you don't wipe its memory and try to give it a different purpose, even temporarily.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 20,
+            "execution_count": 130,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Wipe agent memories response: Memories for agent new_agent deleted.\n"
@@ -728,22 +737,22 @@
             "metadata": {},
             "source": [
                 "## Get a list of Chains available to use\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 21,
+            "execution_count": 131,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Chains: ['Smart Instruct', 'Test_Commands', 'Write a Poem', 'Smart Chat', 'Task']\n"
+                        "Chains: ['Smart Instruct', 'Test_Commands', 'Generate and Run Smart Task Chain', 'Write a Poem', 'Generate and Run Task Chain', 'Generate Task Chain', 'Generate Smart Task Chain', 'Smart Chat']\n"
                     ]
                 }
             ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test get_chains()\n",
@@ -757,15 +766,15 @@
             "metadata": {},
             "source": [
                 "## Create a new chain\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 22,
+            "execution_count": 132,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Add chain response: Chain 'Write another Poem' created.\n"
@@ -787,15 +796,15 @@
             "metadata": {},
             "source": [
                 "## Rename the chain\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 23,
+            "execution_count": 133,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Rename chain response: Chain 'Write another Poem' renamed to 'Poem Writing Chain'.\n"
@@ -820,15 +829,15 @@
             "metadata": {},
             "source": [
                 "## Add Chain Steps\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 24,
+            "execution_count": 134,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Add step response: Step 1 added to chain 'Poem Writing Chain'.\n",
@@ -872,15 +881,15 @@
             "metadata": {},
             "source": [
                 "## Get the content of the chain\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 25,
+            "execution_count": 135,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Chain: {'chain_name': 'Poem Writing Chain', 'steps': [{'step': 1, 'agent_name': 'new_agent', 'prompt_type': 'Prompt', 'prompt': {'prompt_name': 'Write a Poem', 'subject': 'Artificial Intelligence'}}, {'step': 2, 'agent_name': 'new_agent', 'prompt_type': 'Prompt', 'prompt': {'prompt_name': 'Write a Poem', 'subject': 'Quantum Computers'}}]}\n"
@@ -904,15 +913,15 @@
                 "## Modify a chain step\n",
                 "\n",
                 "Instead of the subject of the poem just being Artificial Intelligence, we'll change it to be Artificial General Intelligence.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 26,
+            "execution_count": 136,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Update step response: Step 1 updated for chain 'Poem Writing Chain'.\n"
@@ -946,15 +955,15 @@
                 "## Move the chain step\n",
                 "\n",
                 "When you move a step, it will automatically reassign the order of the steps to match the new order. If there are only 2 steps like in our case, it will just swap them.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 27,
+            "execution_count": 137,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Move step response: Step 1 moved to 2 in chain 'Poem Writing Chain'.\n"
@@ -982,15 +991,15 @@
                 "## Add a Command to the Chain\n",
                 "\n",
                 "We'll write the result to a file for an example.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 28,
+            "execution_count": 138,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Add step response: Step 3 added to chain 'Poem Writing Chain'.\n"
@@ -1023,22 +1032,22 @@
             "metadata": {},
             "source": [
                 "## Run the chain\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 29,
+            "execution_count": 139,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Run chain response: {'1': {'response': \"Quantum computers, they say, are the future of computing\\nWith qubits and entanglement, they solve problems baffling\\n\\nThey work not with zeroes and ones, but with quantum bits\\nWith probability and superposition, they can compute with wits\\n\\nThey're faster and smarter than any computer we know\\nAble to break encryptions, that would have taken ages, just so\\n\\nThey can simulate particles, that classical computers dread\\nRevolutionizing science, with simulations ahead\\n\\nTheir power is immense, and their potential is vast\\nQuantum computers, a technology that's here to last\\n\\nThey usher in a new era of computing, unprecedented\\nA marvel of science and technology, and dreams, unrestricted.\", 'agent_name': 'new_agent', 'prompt': {'prompt_name': 'Write a Poem', 'subject': 'Quantum Computers'}, 'prompt_type': 'Prompt'}, '2': {'response': 'Artificial General Intelligence,\\nA future we all hope to see\\nA machine with true intelligence,\\nWith abilities beyond what we conceive\\n\\nNo longer limited to programmed commands,\\nThis AGI can think on its own\\nMaking decisions, solving problems,\\nAnd perhaps even creating unknowns\\n\\nA new era of progress and breakthroughs,\\nWith technology as our guide\\nAGI leading the way,\\nInnovation at its side\\n\\nBut with great power comes great responsibility,\\nAs we entrust this intelligence to lead\\nWe must ensure it is programmed ethically,\\nGuided by values, empathy, and the need\\n\\nFor progress, for peace, for a better future,\\nAGI can be our partner and friend\\nWith its brilliance and our humanity,\\nTogether we can change the world and transcend.', 'agent_name': 'new_agent', 'prompt': {'prompt_name': 'Write a Poem', 'subject': 'Artificial General Intelligence'}, 'prompt_type': 'Prompt'}, '3': {'response': 'File written to successfully.', 'agent_name': 'new_agent', 'prompt': {'command_name': 'Write to File', 'filename': '{user_input}.txt', 'text': 'First Poem:\\n{STEP1}\\n\\nSecond Poem:\\n{STEP2}'}, 'prompt_type': 'Command'}}\n"
+                        "Run chain response: {'1': {'response': \"Quantum computers, machines of wonder\\nWith qubits and gates to ponder\\nTheir power and speed beyond compare\\nA technological marvel, so rare.\\n\\nThey harness quantum physics' strange ways\\nTo solve problems in an astonishing craze\\nSimulating complex systems and more\\nTheir potential, endless, to explore.\\n\\nWith parallel universes to explore\\nQuantum computers will open new doors\\nTo knowledge and science, they'll lead the way\\nTo the discoveries of a brighter day.\\n\\nFrom cryptography to medicine and more\\nQuantum computers will help us explore\\nThe mysteries of our universe, vast and deep\\nWith great power, they'll help us reach.\\n\\nSo let us praise these machines of wonder\\nFor their potential, too great to ponder\\nQuantum computers, with their power and might\\nWill bring us closer to the light.\", 'agent_name': 'new_agent', 'prompt': {'prompt_name': 'Write a Poem', 'subject': 'Quantum Computers'}, 'prompt_type': 'Prompt'}, '2': {'response': 'Artificial General Intelligence, a phrase so vast and deep\\nIt speaks of a world beyond our reach, where machines think and speak\\nWith their own kind of intelligence, separate from our own\\nA way of seeing, thinking, feeling, that\u2019s different, and yet somehow known\\n\\nAGI is a quest for man, to understand the mind\\nTo create intelligent machines that are of a similar kind\\nIt\u2019s a world beyond our reach, a place we\u2019ve never known\\nA world of pure intelligence, of metal, wires and chrome\\n\\nWe\u2019ve built machines to think before, but they\u2019re limited in their scope\\nAGI is different, it\u2019s a new kind of hope\\nA hope for a world where we can speak to our machines\\nAnd they will answer us with thoughts and hopes and dreams\\n\\nThe AI revolution is upon us, and AGI is the crown\\nIt will change the world forever, and turn it upside down\\nOur machines will be as smart as men, and much more efficient too\\nWe\u2019ll create a world of wonder, where anything we want to do, we\u2019ll do.\\n\\nSo let us claim this superpower, and build a new world with it\\nA world without limits, without boundaries or any limit\\nA world where our machines can think and speak, and where we\u2019ll all get along\\nA world where our machines can truly sing, and we\u2019ll all join in the song.', 'agent_name': 'new_agent', 'prompt': {'prompt_name': 'Write a Poem', 'subject': 'Artificial General Intelligence'}, 'prompt_type': 'Prompt'}, '3': {'response': 'File written to successfully.', 'agent_name': 'new_agent', 'prompt': {'command_name': 'Write to File', 'filename': '{user_input}.txt', 'text': 'First Poem:\\n{STEP1}\\n\\nSecond Poem:\\n{STEP2}'}, 'prompt_type': 'Command'}}\n"
                     ]
                 }
             ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test run_chain()\n",
@@ -1055,22 +1064,22 @@
             "metadata": {},
             "source": [
                 "## Get the responses from the chain running\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 30,
+            "execution_count": 140,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Chain: {'1': {'response': \"Quantum computers, they say, are the future of computing\\nWith qubits and entanglement, they solve problems baffling\\n\\nThey work not with zeroes and ones, but with quantum bits\\nWith probability and superposition, they can compute with wits\\n\\nThey're faster and smarter than any computer we know\\nAble to break encryptions, that would have taken ages, just so\\n\\nThey can simulate particles, that classical computers dread\\nRevolutionizing science, with simulations ahead\\n\\nTheir power is immense, and their potential is vast\\nQuantum computers, a technology that's here to last\\n\\nThey usher in a new era of computing, unprecedented\\nA marvel of science and technology, and dreams, unrestricted.\", 'agent_name': 'new_agent', 'prompt': {'prompt_name': 'Write a Poem', 'subject': 'Quantum Computers'}, 'prompt_type': 'Prompt'}, '2': {'response': 'Artificial General Intelligence,\\nA future we all hope to see\\nA machine with true intelligence,\\nWith abilities beyond what we conceive\\n\\nNo longer limited to programmed commands,\\nThis AGI can think on its own\\nMaking decisions, solving problems,\\nAnd perhaps even creating unknowns\\n\\nA new era of progress and breakthroughs,\\nWith technology as our guide\\nAGI leading the way,\\nInnovation at its side\\n\\nBut with great power comes great responsibility,\\nAs we entrust this intelligence to lead\\nWe must ensure it is programmed ethically,\\nGuided by values, empathy, and the need\\n\\nFor progress, for peace, for a better future,\\nAGI can be our partner and friend\\nWith its brilliance and our humanity,\\nTogether we can change the world and transcend.', 'agent_name': 'new_agent', 'prompt': {'prompt_name': 'Write a Poem', 'subject': 'Artificial General Intelligence'}, 'prompt_type': 'Prompt'}, '3': {'response': 'File written to successfully.', 'agent_name': 'new_agent', 'prompt': {'command_name': 'Write to File', 'filename': '{user_input}.txt', 'text': 'First Poem:\\n{STEP1}\\n\\nSecond Poem:\\n{STEP2}'}, 'prompt_type': 'Command'}}\n"
+                        "Chain: {'1': {'response': \"Quantum computers, machines of wonder\\nWith qubits and gates to ponder\\nTheir power and speed beyond compare\\nA technological marvel, so rare.\\n\\nThey harness quantum physics' strange ways\\nTo solve problems in an astonishing craze\\nSimulating complex systems and more\\nTheir potential, endless, to explore.\\n\\nWith parallel universes to explore\\nQuantum computers will open new doors\\nTo knowledge and science, they'll lead the way\\nTo the discoveries of a brighter day.\\n\\nFrom cryptography to medicine and more\\nQuantum computers will help us explore\\nThe mysteries of our universe, vast and deep\\nWith great power, they'll help us reach.\\n\\nSo let us praise these machines of wonder\\nFor their potential, too great to ponder\\nQuantum computers, with their power and might\\nWill bring us closer to the light.\", 'agent_name': 'new_agent', 'prompt': {'prompt_name': 'Write a Poem', 'subject': 'Quantum Computers'}, 'prompt_type': 'Prompt'}, '2': {'response': 'Artificial General Intelligence, a phrase so vast and deep\\nIt speaks of a world beyond our reach, where machines think and speak\\nWith their own kind of intelligence, separate from our own\\nA way of seeing, thinking, feeling, that\u2019s different, and yet somehow known\\n\\nAGI is a quest for man, to understand the mind\\nTo create intelligent machines that are of a similar kind\\nIt\u2019s a world beyond our reach, a place we\u2019ve never known\\nA world of pure intelligence, of metal, wires and chrome\\n\\nWe\u2019ve built machines to think before, but they\u2019re limited in their scope\\nAGI is different, it\u2019s a new kind of hope\\nA hope for a world where we can speak to our machines\\nAnd they will answer us with thoughts and hopes and dreams\\n\\nThe AI revolution is upon us, and AGI is the crown\\nIt will change the world forever, and turn it upside down\\nOur machines will be as smart as men, and much more efficient too\\nWe\u2019ll create a world of wonder, where anything we want to do, we\u2019ll do.\\n\\nSo let us claim this superpower, and build a new world with it\\nA world without limits, without boundaries or any limit\\nA world where our machines can think and speak, and where we\u2019ll all get along\\nA world where our machines can truly sing, and we\u2019ll all join in the song.', 'agent_name': 'new_agent', 'prompt': {'prompt_name': 'Write a Poem', 'subject': 'Artificial General Intelligence'}, 'prompt_type': 'Prompt'}, '3': {'response': 'File written to successfully.', 'agent_name': 'new_agent', 'prompt': {'command_name': 'Write to File', 'filename': '{user_input}.txt', 'text': 'First Poem:\\n{STEP1}\\n\\nSecond Poem:\\n{STEP2}'}, 'prompt_type': 'Command'}}\n"
                     ]
                 }
             ],
             "source": [
                 "# Need to make a function to get_chain_responses() as it's not in the API yet.\n",
                 "from ApiClient import ApiClient\n",
                 "\n",
@@ -1086,15 +1095,15 @@
             "metadata": {},
             "source": [
                 "## Delete a step from the chain\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 31,
+            "execution_count": 141,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Delete step response: Step 2 deleted from chain 'Poem Writing Chain'.\n"
@@ -1116,15 +1125,15 @@
             "metadata": {},
             "source": [
                 "## Delete the chain\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 32,
+            "execution_count": 142,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Delete chain response: Chain 'Poem Writing Chain' deleted.\n"
@@ -1148,22 +1157,22 @@
                 "# Prompts\n",
                 "\n",
                 "## Get a list of prompts available to use\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 33,
+            "execution_count": 143,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Prompts: ['Pseudo Code', 'SmartInstruct-Researcher', 'Custom Input', 'Title a Poem', 'ValidationFailed', 'SmartTask-CleanResponse', 'SmartChat-Researcher', 'Tell Me How', 'Execution', 'Score Response', 'Validation', 'Write a Haiku', 'SmartInstruct-Resolver', 'SmartInstruct-CleanResponse', 'SmartInstruct-StepByStep', 'instruct', 'Pick a Poem Subject', 'Task Execution', 'Check-Instruction', 'SmartTask-Execution', 'SmartChat-Resolver', 'Chat', 'Create New Command', 'SmartChat-CleanResponse', 'Prioritize', 'Pick-a-Link', 'SmartInstruct-Execution', 'Write a Poem', 'JSONFormatter', 'SmartTask-StepByStep', 'Instruction', 'WebSearch', 'SmartChat-StepByStep', 'Get Task List']\n"
+                        "Prompts: ['Pseudo Code', 'SmartInstruct-Researcher', 'Custom Input', 'Title a Poem', 'ValidationFailed', 'SmartTask-CleanResponse', 'SmartChat-Researcher', 'Tell Me How', 'Execution', 'Score Response', 'Get Task Description', 'Validation', 'Write a Haiku', 'SmartInstruct-Resolver', 'SmartInstruct-CleanResponse', 'SmartInstruct-StepByStep', 'instruct', 'Pick a Poem Subject', 'Task Execution', 'Check-Instruction', 'SmartTask-Execution', 'SmartChat-Resolver', 'Chat', 'Create New Command', 'SmartChat-CleanResponse', 'Prioritize', 'Pick-a-Link', 'SmartInstruct-Execution', 'Write a Poem', 'JSONFormatter', 'SmartTask-StepByStep', 'Instruction', 'WebSearch', 'SmartChat-StepByStep', 'Get Task List']\n"
                     ]
                 }
             ],
             "source": [
                 "from ApiClient import ApiClient\n",
                 "\n",
                 "# Test get_prompts()\n",
@@ -1179,15 +1188,15 @@
                 "## Create a new prompt\n",
                 "\n",
                 "We'll make a basic prompt that asks the AI to tell us a short story about a subject. The subject is not yet defined, it would be defined in a chain. Using `{variable_name}` in a prompt will allow you to define the variable in a chain and have it be used in the prompt.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 34,
+            "execution_count": 144,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Add prompt response: Prompt 'Short Story' added.\n"
@@ -1210,15 +1219,15 @@
             "metadata": {},
             "source": [
                 "## Get the prompt content\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 35,
+            "execution_count": 145,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Get prompt response: Write a poem about {subject} .\n",
@@ -1240,15 +1249,15 @@
             "metadata": {},
             "source": [
                 "## Get the prompt variables\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 36,
+            "execution_count": 146,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Get prompt args response: ['subject']\n"
@@ -1272,15 +1281,15 @@
                 "## Update the prompt content\n",
                 "\n",
                 "We'll ask it to `Add a dragon to the story somehow` in the prompt to make the short story more interesting.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 37,
+            "execution_count": 147,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Update prompt response: Prompt 'Short Story' updated.\n"
@@ -1306,15 +1315,15 @@
                 "## Delete the prompt\n",
                 "\n",
                 "If you don't want the prompt anymore, delete it.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 38,
+            "execution_count": 148,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Delete prompt response: Prompt 'Short Story' deleted.\n"
@@ -1337,15 +1346,15 @@
                 "## Delete Agent History\n",
                 "\n",
                 "Delete the history for the agent.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 39,
+            "execution_count": 149,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Delete agent response: History for agent new_agent deleted.\n"
@@ -1369,15 +1378,15 @@
                 "## Delete the Agent\n",
                 "\n",
                 "If you are done with the agent and don't want or need it anymore, you can delete it along with everything associated with it, such as its memories, settings, and history. The Agent isn't just fired, it is dead.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 40,
+            "execution_count": 150,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Delete agent response: Agent new_agent deleted.\n"
```

