# Comparing `tmp/telegram_botup-0.9.2-py3-none-any.whl.zip` & `tmp/telegram_botup-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,25 +1,20 @@
-Zip file size: 34208 bytes, number of entries: 23
--rw-rw-r--  2.0 unx      134 b- defN 22-May-04 18:45 botup/__init__.py
--rw-rw-r--  2.0 unx     4991 b- defN 22-May-04 09:59 botup/cli.py
--rw-rw-r--  2.0 unx    27565 b- defN 21-Nov-08 11:46 botup/dispatcher.py
--rw-rw-r--  2.0 unx      193 b- defN 21-Nov-08 11:46 botup/exceptions.py
--rw-rw-r--  2.0 unx     4595 b- defN 21-Nov-08 11:46 botup/handlers.py
--rw-rw-r--  2.0 unx    60692 b- defN 21-Nov-11 21:08 botup/sender.py
--rw-rw-r--  2.0 unx    44573 b- defN 22-May-04 18:44 botup/types.py
--rw-rw-r--  2.0 unx     1183 b- defN 21-Nov-11 21:08 botup/utils.py
--rw-rw-r--  2.0 unx     5034 b- defN 21-Nov-08 11:46 botup/wsgi.py
--rw-rw-r--  2.0 unx        0 b- defN 21-Nov-08 11:46 tests/__init__.py
--rw-rw-r--  2.0 unx      103 b- defN 21-Nov-08 11:46 tests/conftest.py
--rw-rw-r--  2.0 unx    30297 b- defN 21-Nov-08 11:46 tests/test_dispatcher.py
--rw-rw-r--  2.0 unx    10018 b- defN 21-Nov-08 11:46 tests/test_dispatcher_decorator.py
--rw-rw-r--  2.0 unx     6703 b- defN 21-Nov-08 11:46 tests/test_dispatcher_registration.py
--rw-rw-r--  2.0 unx      276 b- defN 21-Nov-08 11:46 tests/test_serializing.py
--rw-rw-r--  2.0 unx     3242 b- defN 21-Nov-08 11:46 tests/test_state_dispatcher.py
--rw-rw-r--  2.0 unx      227 b- defN 21-Nov-08 14:12 tests/test_utils.py
--rw-rw-r--  2.0 unx    31211 b- defN 21-Nov-08 14:12 tests/utils.py
--rw-rw-r--  2.0 unx     3734 b- defN 22-May-04 18:46 telegram_botup-0.9.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-May-04 18:46 telegram_botup-0.9.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx       41 b- defN 22-May-04 18:46 telegram_botup-0.9.2.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       12 b- defN 22-May-04 18:46 telegram_botup-0.9.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1809 b- defN 22-May-04 18:46 telegram_botup-0.9.2.dist-info/RECORD
-23 files, 236725 bytes uncompressed, 31318 bytes compressed:  86.8%
+Zip file size: 14042 bytes, number of entries: 18
+-rw-rw-r--  2.0 unx       22 b- defN 23-Jun-13 09:30 botup/__init__.py
+-rw-rw-r--  2.0 unx      905 b- defN 23-Jun-13 09:12 botup/bot.py
+-rw-rw-r--  2.0 unx     1266 b- defN 23-Jun-13 09:13 botup/navigation.py
+-rw-rw-r--  2.0 unx      331 b- defN 23-Jun-13 09:13 botup/utils.py
+-rw-rw-r--  2.0 unx     1948 b- defN 23-Jun-13 09:13 botup/widget.py
+-rw-rw-r--  2.0 unx        0 b- defN 22-May-15 21:45 tests/__init__.py
+-rw-rw-r--  2.0 unx      119 b- defN 23-Jun-13 09:17 tests/conftest.py
+-rw-rw-r--  2.0 unx    32361 b- defN 22-Aug-26 20:36 tests/test_dispatcher.py
+-rw-rw-r--  2.0 unx    10599 b- defN 22-Aug-26 20:36 tests/test_dispatcher_decorator.py
+-rw-rw-r--  2.0 unx     6708 b- defN 23-Jun-13 08:57 tests/test_dispatcher_registration.py
+-rw-rw-r--  2.0 unx      441 b- defN 23-Jun-13 08:57 tests/test_serializing.py
+-rw-rw-r--  2.0 unx     3403 b- defN 23-Jun-13 08:57 tests/test_state_dispatcher.py
+-rw-rw-r--  2.0 unx      227 b- defN 22-May-15 21:45 tests/test_utils.py
+-rw-rw-r--  2.0 unx    35379 b- defN 23-Jun-13 08:57 tests/utils.py
+-rw-rw-r--  2.0 unx     4496 b- defN 23-Jun-13 09:30 telegram_botup-1.0.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-13 09:30 telegram_botup-1.0.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       12 b- defN 23-Jun-13 09:30 telegram_botup-1.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1411 b- defN 23-Jun-13 09:30 telegram_botup-1.0.1.dist-info/RECORD
+18 files, 99720 bytes uncompressed, 11752 bytes compressed:  88.2%
```

## zipnote {}

```diff
@@ -1,32 +1,20 @@
 Filename: botup/__init__.py
 Comment: 
 
-Filename: botup/cli.py
+Filename: botup/bot.py
 Comment: 
 
-Filename: botup/dispatcher.py
-Comment: 
-
-Filename: botup/exceptions.py
-Comment: 
-
-Filename: botup/handlers.py
-Comment: 
-
-Filename: botup/sender.py
-Comment: 
-
-Filename: botup/types.py
+Filename: botup/navigation.py
 Comment: 
 
 Filename: botup/utils.py
 Comment: 
 
-Filename: botup/wsgi.py
+Filename: botup/widget.py
 Comment: 
 
 Filename: tests/__init__.py
 Comment: 
 
 Filename: tests/conftest.py
 Comment: 
@@ -48,23 +36,20 @@
 
 Filename: tests/test_utils.py
 Comment: 
 
 Filename: tests/utils.py
 Comment: 
 
-Filename: telegram_botup-0.9.2.dist-info/METADATA
-Comment: 
-
-Filename: telegram_botup-0.9.2.dist-info/WHEEL
+Filename: telegram_botup-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: telegram_botup-0.9.2.dist-info/entry_points.txt
+Filename: telegram_botup-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: telegram_botup-0.9.2.dist-info/top_level.txt
+Filename: telegram_botup-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: telegram_botup-0.9.2.dist-info/RECORD
+Filename: telegram_botup-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## botup/__init__.py

```diff
@@ -1,4 +1 @@
-from .dispatcher import Dispatcher, StateDispatcher, StateManager, DictStateManager
-from .sender import Sender
-
-__version__ = "0.9.2"
+__version__ = "1.0.1"
```

## botup/utils.py

```diff
@@ -1,42 +1,16 @@
-import logging
+from botup.core.utils import get_logger, setup_logging
 
+__all__ = [
+    'get_logger',
+    'setup_logging',
+    'start_group_link',
+    'start_link'
+]
 
-def get_logger():
-    return logging.getLogger('botup')
 
-
-def setup_logging(level=logging.INFO):
-    logger = logging.getLogger('botup')
-    logger.addHandler(logging.StreamHandler())
-    logger.setLevel(level)
-
-
-def start_group_link(bot_name):
+def start_group_link(bot_name: str):
     return f'https://telegram.me/{bot_name}?startgroup='
 
 
-def start_link(bot_name):
+def start_link(bot_name: str):
     return f'https://telegram.me/{bot_name}?start='
-
-
-def get_chat_id(update):
-    if update.message:
-        return update.message.chat.id
-    if update.callback_query:
-        return update.callback_query.from_.id
-    if update.inline_query:
-        return update.inline_query.from_.id
-    if update.chosen_inline_result:
-        return update.chosen_inline_result.from_.id
-    if update.poll_answer:
-        return update.poll_answer.user.id
-    if update.edited_message:
-        return update.edited_message.chat.id
-    if update.channel_post:
-        return update.channel_post.chat.id
-    if update.edited_channel_post:
-        return update.edited_channel_post.chat.id
-    if update.shipping_query:
-        return update.shipping_query.from_.id
-    if update.pre_checkout_query:
-        return update.pre_checkout_query.from_.id
```

## tests/conftest.py

```diff
@@ -1,7 +1,7 @@
 import pytest
-from botup import Dispatcher
+from botup.core.dispatcher import Dispatcher
 
 
 @pytest.fixture
 def dispatcher():
     return Dispatcher()
```

## tests/test_dispatcher.py

```diff
@@ -1,8 +1,9 @@
 import re
+import asyncio
 
 from tests import utils
 
 
 def test_patterns_regexp(dispatcher):
     foobar_message_update = utils.message_update_by_text('foobar')
     hi_dude_message_update = utils.message_update_by_text('hi dude')
@@ -16,932 +17,932 @@
     foobar_inline_query_update = utils.inline_query_update_by_query('foobar')
     send_a_inline_query_update = utils.inline_query_update_by_query('send a')
     send_b_inline_query_update = utils.inline_query_update_by_query('send b')
 
     calls = list()
     updates = list()
 
-    def hi_message_handler(c, u):
+    async def hi_message_handler(c, u):
         updates.append(u)
         calls.append(hi_message_handler)
 
-    def drop_callback_handler(c, u):
+    async def drop_callback_handler(c, u):
         updates.append(u)
         calls.append(drop_callback_handler)
 
-    def give_command_handler(c, u):
+    async def give_command_handler(c, u):
         updates.append(u)
         calls.append(give_command_handler)
 
-    def send_inline_query_handler(c, u):
+    async def send_inline_query_handler(c, u):
         updates.append(u)
         calls.append(send_inline_query_handler)
 
-    def common_handler(c, u):
+    async def common_handler(c, u):
         updates.append(u)
         calls.append(common_handler)
 
     before_calls_counter = len(calls)
-    dispatcher.handle(hi_dude_message_update)
-    dispatcher.handle(hi_mate_message_update)
-    dispatcher.handle(foobar_message_update)
+    asyncio.run(dispatcher.handle(hi_dude_message_update))
+    asyncio.run(dispatcher.handle(hi_mate_message_update))
+    asyncio.run(dispatcher.handle(foobar_message_update))
     assert before_calls_counter == len(calls)
     dispatcher.register_message_handler(re.compile('^hi'), hi_message_handler)
-    dispatcher.handle(hi_dude_message_update)
+    asyncio.run(dispatcher.handle(hi_dude_message_update))
     assert calls[-1] is hi_message_handler
     assert updates[-1] is hi_dude_message_update
-    dispatcher.handle(hi_mate_message_update)
+    asyncio.run(dispatcher.handle(hi_mate_message_update))
     assert calls[-1] is hi_message_handler
     assert updates[-1] is hi_mate_message_update
     before_calls_counter = len(calls)
-    dispatcher.handle(foobar_message_update)
+    asyncio.run(dispatcher.handle(foobar_message_update))
     assert before_calls_counter == len(calls)
     dispatcher.register_message_handler(re.compile('.*'), common_handler)
-    dispatcher.handle(foobar_message_update)
+    asyncio.run(dispatcher.handle(foobar_message_update))
     assert calls[-1] is common_handler
     assert updates[-1] is foobar_message_update
 
     before_calls_counter = len(calls)
-    dispatcher.handle(drop_a_callback_update)
-    dispatcher.handle(drop_b_callback_update)
-    dispatcher.handle(foobar_callback_update)
+    asyncio.run(dispatcher.handle(drop_a_callback_update))
+    asyncio.run(dispatcher.handle(drop_b_callback_update))
+    asyncio.run(dispatcher.handle(foobar_callback_update))
     assert before_calls_counter == len(calls)
     dispatcher.register_callback_handler(re.compile('^drop'), drop_callback_handler)
-    dispatcher.handle(drop_a_callback_update)
+    asyncio.run(dispatcher.handle(drop_a_callback_update))
     assert calls[-1] is drop_callback_handler
     assert updates[-1] is drop_a_callback_update
-    dispatcher.handle(drop_b_callback_update)
+    asyncio.run(dispatcher.handle(drop_b_callback_update))
     assert calls[-1] is drop_callback_handler
     assert updates[-1] is drop_b_callback_update
     before_calls_counter = len(calls)
-    dispatcher.handle(foobar_callback_update)
+    asyncio.run(dispatcher.handle(foobar_callback_update))
     assert before_calls_counter == len(calls)
     dispatcher.register_callback_handler(re.compile('.*'), common_handler)
-    dispatcher.handle(foobar_callback_update)
+    asyncio.run(dispatcher.handle(foobar_callback_update))
     assert calls[-1] is common_handler
     assert updates[-1] is foobar_callback_update
 
     before_calls_counter = len(calls)
-    dispatcher.handle(give_1_command_update)
-    dispatcher.handle(give_2_command_update)
-    dispatcher.handle(foobar_command_update)
+    asyncio.run(dispatcher.handle(give_1_command_update))
+    asyncio.run(dispatcher.handle(give_2_command_update))
+    asyncio.run(dispatcher.handle(foobar_command_update))
     assert before_calls_counter == len(calls)
     dispatcher.register_command_handler(re.compile('^/give'), give_command_handler)
-    dispatcher.handle(give_1_command_update)
+    asyncio.run(dispatcher.handle(give_1_command_update))
     assert calls[-1] is give_command_handler
     assert updates[-1] is give_1_command_update
-    dispatcher.handle(give_2_command_update)
+    asyncio.run(dispatcher.handle(give_2_command_update))
     assert calls[-1] is give_command_handler
     assert updates[-1] is give_2_command_update
     before_calls_counter = len(calls)
-    dispatcher.handle(foobar_command_update)
+    asyncio.run(dispatcher.handle(foobar_command_update))
     assert before_calls_counter == len(calls)
     dispatcher.register_command_handler(re.compile('^/.*'), common_handler)
-    dispatcher.handle(foobar_command_update)
+    asyncio.run(dispatcher.handle(foobar_command_update))
     assert calls[-1] is common_handler
     assert updates[-1] is foobar_command_update
     
     before_calls_counter = len(calls)
-    dispatcher.handle(send_a_inline_query_update)
-    dispatcher.handle(send_b_inline_query_update)
-    dispatcher.handle(foobar_inline_query_update)
+    asyncio.run(dispatcher.handle(send_a_inline_query_update))
+    asyncio.run(dispatcher.handle(send_b_inline_query_update))
+    asyncio.run(dispatcher.handle(foobar_inline_query_update))
     assert before_calls_counter == len(calls)
     dispatcher.register_inline_handler(re.compile('^send'), send_inline_query_handler)
-    dispatcher.handle(send_a_inline_query_update)
+    asyncio.run(dispatcher.handle(send_a_inline_query_update))
     assert calls[-1] is send_inline_query_handler
     assert updates[-1] is send_a_inline_query_update
-    dispatcher.handle(send_b_inline_query_update)
+    asyncio.run(dispatcher.handle(send_b_inline_query_update))
     assert calls[-1] is send_inline_query_handler
     assert updates[-1] is send_b_inline_query_update
     before_calls_counter = len(calls)
-    dispatcher.handle(foobar_inline_query_update)
+    asyncio.run(dispatcher.handle(foobar_inline_query_update))
     assert before_calls_counter == len(calls)
     dispatcher.register_inline_handler(re.compile('.*'), common_handler)
-    dispatcher.handle(foobar_inline_query_update)
+    asyncio.run(dispatcher.handle(foobar_inline_query_update))
     assert calls[-1] is common_handler
     assert updates[-1] is foobar_inline_query_update
 
 
 def test_middleware(dispatcher):
     update = utils.message_update_by_text('test')
     calls = list()
 
-    def mw_true(u):
+    async def mw_true(u):
         calls.append(mw_true)
         return True
 
-    def mw_false(u):
+    async def mw_false(u):
         calls.append(mw_false)
         return False
 
-    def message_handler(c, u):
+    async def message_handler(c, u):
         calls.append(message_handler)
 
-    dispatcher.handle(update)
+    asyncio.run(dispatcher.handle(update))
     assert not calls
     dispatcher.register_message_handler('test', message_handler)
-    dispatcher.handle(update)
+    asyncio.run(dispatcher.handle(update))
     assert len(calls) == 1
     assert calls[-1] is message_handler
     dispatcher.register_middleware(mw_false)
-    dispatcher.handle(update)
+    asyncio.run(dispatcher.handle(update))
     assert len(calls) == 3
     assert calls[-2] is mw_false
     assert calls[-1] is message_handler
     dispatcher.register_middleware(mw_true)
-    dispatcher.handle(update)
+    asyncio.run(dispatcher.handle(update))
     assert len(calls) == 5
     assert calls[-2] is mw_false
     assert calls[-1] is mw_true
 
 
 def test_messages(dispatcher):
     a_messsage_update = utils.message_update_by_text('a')
     b_message_update = utils.message_update_by_text('b')
     c_message_update = utils.message_update_by_text('c')
     command_update = utils.command_update_by_text('/command')
 
     calls = list()
     updates = list()
 
-    def a_handler(c, u):
+    async def a_handler(c, u):
         updates.append(u)
         calls.append(a_handler)
 
-    def b_handler(c, u):
+    async def b_handler(c, u):
         updates.append(u)
         calls.append(b_handler)
 
-    def c_handler(c, u):
+    async def c_handler(c, u):
         updates.append(u)
         calls.append(c_handler)
 
     before_calls_counter = len(calls)
-    dispatcher.handle(a_messsage_update)
-    dispatcher.handle(b_message_update)
-    dispatcher.handle(c_message_update)
+    asyncio.run(dispatcher.handle(a_messsage_update))
+    asyncio.run(dispatcher.handle(b_message_update))
+    asyncio.run(dispatcher.handle(c_message_update))
     assert before_calls_counter == len(calls)
 
     dispatcher.register_message_handler('a', a_handler)
     dispatcher.register_message_handler('b', b_handler)
 
-    dispatcher.handle(a_messsage_update)
+    asyncio.run(dispatcher.handle(a_messsage_update))
     assert calls[-1] is a_handler
     assert updates[-1] is a_messsage_update
 
-    dispatcher.handle(b_message_update)
+    asyncio.run(dispatcher.handle(b_message_update))
     assert calls[-1] is b_handler
     assert updates[-1] is b_message_update
 
     before_calls_counter = len(calls)
-    dispatcher.handle(command_update)
+    asyncio.run(dispatcher.handle(command_update))
     assert before_calls_counter == len(calls)
 
     before_calls_counter = len(calls)
-    dispatcher.handle(c_message_update)
+    asyncio.run(dispatcher.handle(c_message_update))
     assert before_calls_counter == len(calls)
 
     dispatcher.register_message_handler('c', c_handler)
-    dispatcher.handle(c_message_update)
+    asyncio.run(dispatcher.handle(c_message_update))
     assert calls[-1] is c_handler
     assert updates[-1] is c_message_update
 
 
 def test_commands(dispatcher):
     a_command_update = utils.command_update_by_text('/a')
     b_command_update = utils.command_update_by_text('/b')
     c_command_update = utils.command_update_by_text('/c')
     message_update = utils.message_update_by_text('message')
 
     calls = list()
     updates = list()
 
-    def a_handler(c, u):
+    async def a_handler(c, u):
         updates.append(u)
         calls.append(a_handler)
 
-    def b_handler(c, u):
+    async def b_handler(c, u):
         updates.append(u)
         calls.append(b_handler)
 
-    def c_handler(c, u):
+    async def c_handler(c, u):
         updates.append(u)
         calls.append(c_handler)
 
     before_calls_counter = len(calls)
-    dispatcher.handle(a_command_update)
-    dispatcher.handle(b_command_update)
-    dispatcher.handle(c_command_update)
+    asyncio.run(dispatcher.handle(a_command_update))
+    asyncio.run(dispatcher.handle(b_command_update))
+    asyncio.run(dispatcher.handle(c_command_update))
     assert before_calls_counter == len(calls)
 
     dispatcher.register_command_handler('/a', a_handler)
     dispatcher.register_command_handler('/b', b_handler)
 
-    dispatcher.handle(a_command_update)
+    asyncio.run(dispatcher.handle(a_command_update))
     assert calls[-1] is a_handler
     assert updates[-1] is a_command_update
 
-    dispatcher.handle(b_command_update)
+    asyncio.run(dispatcher.handle(b_command_update))
     assert calls[-1] is b_handler
     assert updates[-1] is b_command_update
 
     before_calls_counter = len(calls)
-    dispatcher.handle(message_update)
+    asyncio.run(dispatcher.handle(message_update))
     assert before_calls_counter == len(calls)
 
     before_calls_counter = len(calls)
-    dispatcher.handle(c_command_update)
+    asyncio.run(dispatcher.handle(c_command_update))
     assert before_calls_counter == len(calls)
 
     dispatcher.register_command_handler('/c', c_handler)
-    dispatcher.handle(c_command_update)
+    asyncio.run(dispatcher.handle(c_command_update))
     assert calls[-1] is c_handler
     assert updates[-1] is c_command_update
 
 
 def test_callbacks(dispatcher):
     a_callback_update = utils.callback_update_by_data('a')
     b_callback_update = utils.callback_update_by_data('b')
     c_callback_update = utils.callback_update_by_data('c')
     message_update = utils.message_update_by_text('message')
 
     calls = list()
     updates = list()
 
-    def a_handler(c, u):
+    async def a_handler(c, u):
         updates.append(u)
         calls.append(a_handler)
 
-    def b_handler(c, u):
+    async def b_handler(c, u):
         updates.append(u)
         calls.append(b_handler)
 
-    def c_handler(c, u):
+    async def c_handler(c, u):
         updates.append(u)
         calls.append(c_handler)
 
     before_calls_counter = len(calls)
-    dispatcher.handle(a_callback_update)
-    dispatcher.handle(b_callback_update)
-    dispatcher.handle(c_callback_update)
+    asyncio.run(dispatcher.handle(a_callback_update))
+    asyncio.run(dispatcher.handle(b_callback_update))
+    asyncio.run(dispatcher.handle(c_callback_update))
     assert before_calls_counter == len(calls)
 
     dispatcher.register_callback_handler('a', a_handler)
     dispatcher.register_callback_handler('b', b_handler)
 
-    dispatcher.handle(a_callback_update)
+    asyncio.run(dispatcher.handle(a_callback_update))
     assert calls[-1] is a_handler
     assert updates[-1] is a_callback_update
 
-    dispatcher.handle(b_callback_update)
+    asyncio.run(dispatcher.handle(b_callback_update))
     assert calls[-1] is b_handler
     assert updates[-1] is b_callback_update
 
     before_calls_counter = len(calls)
-    dispatcher.handle(message_update)
+    asyncio.run(dispatcher.handle(message_update))
     assert before_calls_counter == len(calls)
 
     before_calls_counter = len(calls)
-    dispatcher.handle(c_callback_update)
+    asyncio.run(dispatcher.handle(c_callback_update))
     assert before_calls_counter == len(calls)
 
     dispatcher.register_callback_handler('c', c_handler)
-    dispatcher.handle(c_callback_update)
+    asyncio.run(dispatcher.handle(c_callback_update))
     assert calls[-1] is c_handler
     assert updates[-1] is c_callback_update
 
 
 def test_inline_query(dispatcher):
     a_inline_query_update = utils.inline_query_update_by_query('a')
     b_inline_query_update = utils.inline_query_update_by_query('b')
     c_inline_query_update = utils.inline_query_update_by_query('c')
     message_update = utils.message_update_by_text('message')
 
     calls = list()
     updates = list()
 
-    def a_handler(c, u):
+    async def a_handler(c, u):
         updates.append(u)
         calls.append(a_handler)
 
-    def b_handler(c, u):
+    async def b_handler(c, u):
         updates.append(u)
         calls.append(b_handler)
 
-    def c_handler(c, u):
+    async def c_handler(c, u):
         updates.append(u)
         calls.append(c_handler)
 
     before_calls_counter = len(calls)
-    dispatcher.handle(a_inline_query_update)
-    dispatcher.handle(b_inline_query_update)
-    dispatcher.handle(c_inline_query_update)
+    asyncio.run(dispatcher.handle(a_inline_query_update))
+    asyncio.run(dispatcher.handle(b_inline_query_update))
+    asyncio.run(dispatcher.handle(c_inline_query_update))
     assert before_calls_counter == len(calls)
 
     dispatcher.register_inline_handler('a', a_handler)
     dispatcher.register_inline_handler('b', b_handler)
 
-    dispatcher.handle(a_inline_query_update)
+    asyncio.run(dispatcher.handle(a_inline_query_update))
     assert calls[-1] is a_handler
     assert updates[-1] is a_inline_query_update
 
-    dispatcher.handle(b_inline_query_update)
+    asyncio.run(dispatcher.handle(b_inline_query_update))
     assert calls[-1] is b_handler
     assert updates[-1] is b_inline_query_update
 
     before_calls_counter = len(calls)
-    dispatcher.handle(message_update)
+    asyncio.run(dispatcher.handle(message_update))
     assert before_calls_counter == len(calls)
 
     before_calls_counter = len(calls)
-    dispatcher.handle(c_inline_query_update)
+    asyncio.run(dispatcher.handle(c_inline_query_update))
     assert before_calls_counter == len(calls)
 
     dispatcher.register_inline_handler('c', c_handler)
-    dispatcher.handle(c_inline_query_update)
+    asyncio.run(dispatcher.handle(c_inline_query_update))
     assert calls[-1] is c_handler
     assert updates[-1] is c_inline_query_update
 
 
 def test_chosen_inline_result(dispatcher):
     chosen_inline_result_update = utils.chosen_inline_result_update()
 
     calls = list()
     updates = list()
 
-    def chosen_inline_result_handler(c, u):
+    async def chosen_inline_result_handler(c, u):
         updates.append(u)
         calls.append(chosen_inline_result_handler)
 
     before_calls_counter = len(calls)
-    dispatcher.handle(chosen_inline_result_update)
+    asyncio.run(dispatcher.handle(chosen_inline_result_update))
     assert before_calls_counter == len(calls)
     dispatcher.register_chosen_inline_result_handler(chosen_inline_result_handler)
-    dispatcher.handle(chosen_inline_result_update)
+    asyncio.run(dispatcher.handle(chosen_inline_result_update))
     assert calls[-1] is chosen_inline_result_handler
     assert updates[-1] is chosen_inline_result_update
 
 
 def test_edited_message(dispatcher):
     edited_message_update = utils.edited_message_update_by_text('abc')
 
     calls = list()
     updates = list()
 
-    def edited_message_handler(c, u):
+    async def edited_message_handler(c, u):
         updates.append(u)
         calls.append(edited_message_handler)
 
     before_calls_counter = len(calls)
-    dispatcher.handle(edited_message_update)
+    asyncio.run(dispatcher.handle(edited_message_update))
     assert before_calls_counter == len(calls)
     dispatcher.register_edited_message_handler(edited_message_handler)
-    dispatcher.handle(edited_message_update)
+    asyncio.run(dispatcher.handle(edited_message_update))
     assert calls[-1] is edited_message_handler
     assert updates[-1] is edited_message_update
 
 
 def test_channel_post(dispatcher):
     channel_post_update = utils.channel_post_update()
 
     calls = list()
     updates = list()
 
-    def channel_post_handler(c, u):
+    async def channel_post_handler(c, u):
         updates.append(u)
         calls.append(channel_post_handler)
 
     before_calls_counter = len(calls)
-    dispatcher.handle(channel_post_update)
+    asyncio.run(dispatcher.handle(channel_post_update))
     assert before_calls_counter == len(calls)
     dispatcher.register_channel_post_handler(channel_post_handler)
-    dispatcher.handle(channel_post_update)
+    asyncio.run(dispatcher.handle(channel_post_update))
     assert calls[-1] is channel_post_handler
     assert updates[-1] is channel_post_update
 
 
 def test_edited_channel_post(dispatcher):
     edited_channel_post_update = utils.edited_channel_post_update()
 
     calls = list()
     updates = list()
 
-    def edited_channel_post_handler(c, u):
+    async def edited_channel_post_handler(c, u):
         updates.append(u)
         calls.append(edited_channel_post_handler)
 
     before_calls_counter = len(calls)
-    dispatcher.handle(edited_channel_post_update)
+    asyncio.run(dispatcher.handle(edited_channel_post_update))
     assert before_calls_counter == len(calls)
     dispatcher.register_edited_channel_post_handler(edited_channel_post_handler)
-    dispatcher.handle(edited_channel_post_update)
+    asyncio.run(dispatcher.handle(edited_channel_post_update))
     assert calls[-1] is edited_channel_post_handler
     assert updates[-1] is edited_channel_post_update
 
 
 def test_dice(dispatcher):
     dice_update = utils.dice_update()
     message_update = utils.message_update_by_text('message')
 
     calls = list()
     updates = list()
 
-    def dice_handler(c, u):
+    async def dice_handler(c, u):
         updates.append(u)
         calls.append(dice_handler)
 
-    def message_handler(c, u):
+    async def message_handler(c, u):
         updates.append(u)
         calls.append(message_handler)
 
     dispatcher.register_message_handler(re.compile('.*'), message_handler)
-    dispatcher.handle(message_update)
-    dispatcher.handle(dice_update)
+    asyncio.run(dispatcher.handle(message_update))
+    asyncio.run(dispatcher.handle(dice_update))
     assert calls[-1] is message_handler
     assert updates[-1] is message_update
     dispatcher.register_dice_handler(dice_handler)
-    dispatcher.handle(dice_update)
+    asyncio.run(dispatcher.handle(dice_update))
     assert calls[-1] is dice_handler
     assert updates[-1] is dice_update
 
 
 def test_document(dispatcher):
     document_update = utils.document_update()
     message_update = utils.message_update_by_text('message')
 
     calls = list()
     updates = list()
 
-    def document_handler(c, u):
+    async def document_handler(c, u):
         updates.append(u)
         calls.append(document_handler)
 
-    def message_handler(c, u):
+    async def message_handler(c, u):
         updates.append(u)
         calls.append(message_handler)
 
     dispatcher.register_message_handler(re.compile('.*'), message_handler)
-    dispatcher.handle(message_update)
-    dispatcher.handle(document_update)
+    asyncio.run(dispatcher.handle(message_update))
+    asyncio.run(dispatcher.handle(document_update))
     assert calls[-1] is message_handler
     assert updates[-1] is message_update
     dispatcher.register_document_handler(document_handler)
-    dispatcher.handle(document_update)
+    asyncio.run(dispatcher.handle(document_update))
     assert calls[-1] is document_handler
     assert updates[-1] is document_update
 
 
 def test_animation(dispatcher):
     animation_update = utils.animation_update()
     message_update = utils.message_update_by_text('message')
 
     calls = list()
     updates = list()
 
-    def animation_handler(c, u):
+    async def animation_handler(c, u):
         updates.append(u)
         calls.append(animation_handler)
 
-    def message_handler(c, u):
+    async def message_handler(c, u):
         updates.append(u)
         calls.append(message_handler)
 
     dispatcher.register_message_handler(re.compile('.*'), message_handler)
-    dispatcher.handle(message_update)
-    dispatcher.handle(animation_update)
+    asyncio.run(dispatcher.handle(message_update))
+    asyncio.run(dispatcher.handle(animation_update))
     assert calls[-1] is message_handler
     assert updates[-1] is message_update
     dispatcher.register_animation_handler(animation_handler)
-    dispatcher.handle(animation_update)
+    asyncio.run(dispatcher.handle(animation_update))
     assert calls[-1] is animation_handler
     assert updates[-1] is animation_update
 
 
 def test_animation_document_conflict(dispatcher):
     animation_update = utils.animation_update()
     document_update = utils.document_update()
 
     calls = list()
     updates = list()
 
-    def animation_handler(c, u):
+    async def animation_handler(c, u):
         updates.append(u)
         calls.append(animation_handler)
 
-    def document_handler(c, u):
+    async def document_handler(c, u):
         updates.append(u)
         calls.append(document_handler)
 
     dispatcher.register_document_handler(document_handler)
-    dispatcher.handle(document_update)
-    dispatcher.handle(animation_update)
+    asyncio.run(dispatcher.handle(document_update))
+    asyncio.run(dispatcher.handle(animation_update))
     assert calls[-1] is document_handler
     assert updates[-1] is document_update
     dispatcher.register_animation_handler(animation_handler)
-    dispatcher.handle(animation_update)
+    asyncio.run(dispatcher.handle(animation_update))
     assert calls[-1] is animation_handler
     assert updates[-1] is animation_update
-    dispatcher.handle(document_update)
+    asyncio.run(dispatcher.handle(document_update))
     assert calls[-1] is document_handler
     assert updates[-1] is document_update
 
 
 def test_audio(dispatcher):
     audio_update = utils.audio_update()
     message_update = utils.message_update_by_text('message')
 
     calls = list()
     updates = list()
 
-    def audio_handler(c, u):
+    async def audio_handler(c, u):
         updates.append(u)
         calls.append(audio_handler)
 
-    def message_handler(c, u):
+    async def message_handler(c, u):
         updates.append(u)
         calls.append(message_handler)
 
     dispatcher.register_message_handler(re.compile('.*'), message_handler)
-    dispatcher.handle(message_update)
-    dispatcher.handle(audio_update)
+    asyncio.run(dispatcher.handle(message_update))
+    asyncio.run(dispatcher.handle(audio_update))
     assert calls[-1] is message_handler
     assert updates[-1] is message_update
     dispatcher.register_audio_handler(audio_handler)
-    dispatcher.handle(audio_update)
+    asyncio.run(dispatcher.handle(audio_update))
     assert calls[-1] is audio_handler
     assert updates[-1] is audio_update
 
 
 def test_contact(dispatcher):
     contact_update = utils.contact_update()
     message_update = utils.message_update_by_text('message')
 
     calls = list()
     updates = list()
 
-    def contact_handler(c, u):
+    async def contact_handler(c, u):
         updates.append(u)
         calls.append(contact_handler)
 
-    def message_handler(c, u):
+    async def message_handler(c, u):
         updates.append(u)
         calls.append(message_handler)
 
     dispatcher.register_message_handler(re.compile('.*'), message_handler)
-    dispatcher.handle(message_update)
-    dispatcher.handle(contact_update)
+    asyncio.run(dispatcher.handle(message_update))
+    asyncio.run(dispatcher.handle(contact_update))
     assert calls[-1] is message_handler
     assert updates[-1] is message_update
     dispatcher.register_contact_handler(contact_handler)
-    dispatcher.handle(contact_update)
+    asyncio.run(dispatcher.handle(contact_update))
     assert calls[-1] is contact_handler
     assert updates[-1] is contact_update
 
 
 def test_new_chat_members(dispatcher):
     new_chat_members_update = utils.new_chat_members_update()
     message_update = utils.message_update_by_text('message')
 
     calls = list()
     updates = list()
 
-    def new_chat_members_handler(c, u):
+    async def new_chat_members_handler(c, u):
         updates.append(u)
         calls.append(new_chat_members_handler)
 
-    def message_handler(c, u):
+    async def message_handler(c, u):
         updates.append(u)
         calls.append(message_handler)
 
     dispatcher.register_message_handler(re.compile('.*'), message_handler)
-    dispatcher.handle(message_update)
-    dispatcher.handle(new_chat_members_update)
+    asyncio.run(dispatcher.handle(message_update))
+    asyncio.run(dispatcher.handle(new_chat_members_update))
     assert calls[-1] is message_handler
     assert updates[-1] is message_update
     dispatcher.register_new_chat_members_handler(new_chat_members_handler)
-    dispatcher.handle(new_chat_members_update)
+    asyncio.run(dispatcher.handle(new_chat_members_update))
     assert calls[-1] is new_chat_members_handler
     assert updates[-1] is new_chat_members_update
 
 
 def test_new_chat_title(dispatcher):
     new_chat_title_update = utils.new_chat_title_update()
     message_update = utils.message_update_by_text('message')
 
     calls = list()
     updates = list()
 
-    def new_chat_title_handler(c, u):
+    async def new_chat_title_handler(c, u):
         updates.append(u)
         calls.append(new_chat_title_handler)
 
-    def message_handler(c, u):
+    async def message_handler(c, u):
         updates.append(u)
         calls.append(message_handler)
 
     dispatcher.register_message_handler(re.compile('.*'), message_handler)
-    dispatcher.handle(message_update)
-    dispatcher.handle(new_chat_title_update)
+    asyncio.run(dispatcher.handle(message_update))
+    asyncio.run(dispatcher.handle(new_chat_title_update))
     assert calls[-1] is message_handler
     assert updates[-1] is message_update
     dispatcher.register_new_chat_title_handler(new_chat_title_handler)
-    dispatcher.handle(new_chat_title_update)
+    asyncio.run(dispatcher.handle(new_chat_title_update))
     assert calls[-1] is new_chat_title_handler
     assert updates[-1] is new_chat_title_update
 
 
 def test_new_chat_photo(dispatcher):
     new_chat_photo_update = utils.new_chat_photo_update()
     message_update = utils.message_update_by_text('message')
 
     calls = list()
     updates = list()
 
-    def new_chat_photo_handler(c, u):
+    async def new_chat_photo_handler(c, u):
         updates.append(u)
         calls.append(new_chat_photo_handler)
 
-    def message_handler(c, u):
+    async def message_handler(c, u):
         updates.append(u)
         calls.append(message_handler)
 
     dispatcher.register_message_handler(re.compile('.*'), message_handler)
-    dispatcher.handle(message_update)
-    dispatcher.handle(new_chat_photo_update)
+    asyncio.run(dispatcher.handle(message_update))
+    asyncio.run(dispatcher.handle(new_chat_photo_update))
     assert calls[-1] is message_handler
     assert updates[-1] is message_update
     dispatcher.register_new_chat_photo_handler(new_chat_photo_handler)
-    dispatcher.handle(new_chat_photo_update)
+    asyncio.run(dispatcher.handle(new_chat_photo_update))
     assert calls[-1] is new_chat_photo_handler
     assert updates[-1] is new_chat_photo_update
 
 
 def test_left_chat_member(dispatcher):
     left_chat_member_update = utils.left_chat_member_update()
     message_update = utils.message_update_by_text('message')
 
     calls = list()
     updates = list()
 
-    def left_chat_member_handler(c, u):
+    async def left_chat_member_handler(c, u):
         updates.append(u)
         calls.append(left_chat_member_handler)
 
-    def message_handler(c, u):
+    async def message_handler(c, u):
         updates.append(u)
         calls.append(message_handler)
 
     dispatcher.register_message_handler(re.compile('.*'), message_handler)
-    dispatcher.handle(message_update)
-    dispatcher.handle(left_chat_member_update)
+    asyncio.run(dispatcher.handle(message_update))
+    asyncio.run(dispatcher.handle(left_chat_member_update))
     assert calls[-1] is message_handler
     assert updates[-1] is message_update
     dispatcher.register_left_chat_member_handler(left_chat_member_handler)
-    dispatcher.handle(left_chat_member_update)
+    asyncio.run(dispatcher.handle(left_chat_member_update))
     assert calls[-1] is left_chat_member_handler
     assert updates[-1] is left_chat_member_update
 
 
 def test_location(dispatcher):
     location_update = utils.location_update()
     message_update = utils.message_update_by_text('message')
 
     calls = list()
     updates = list()
 
-    def location_handler(c, u):
+    async def location_handler(c, u):
         updates.append(u)
         calls.append(location_handler)
 
-    def message_handler(c, u):
+    async def message_handler(c, u):
         updates.append(u)
         calls.append(message_handler)
 
     dispatcher.register_message_handler(re.compile('.*'), message_handler)
-    dispatcher.handle(message_update)
-    dispatcher.handle(location_update)
+    asyncio.run(dispatcher.handle(message_update))
+    asyncio.run(dispatcher.handle(location_update))
     assert calls[-1] is message_handler
     assert updates[-1] is message_update
     dispatcher.register_location_handler(location_handler)
-    dispatcher.handle(location_update)
+    asyncio.run(dispatcher.handle(location_update))
     assert calls[-1] is location_handler
     assert updates[-1] is location_update
 
 
 def test_poll(dispatcher):
     poll_update = utils.poll_update()
 
     calls = list()
     updates = list()
 
-    def poll_handler(c, u):
+    async def poll_handler(c, u):
         updates.append(u)
         calls.append(poll_handler)
 
     before_calls_counter = len(calls)
-    dispatcher.handle(poll_update)
+    asyncio.run(dispatcher.handle(poll_update))
     assert before_calls_counter == len(calls)
     dispatcher.register_poll_handler(poll_handler)
-    dispatcher.handle(poll_update)
+    asyncio.run(dispatcher.handle(poll_update))
     assert calls[-1] is poll_handler
     assert updates[-1] is poll_update
 
 
 def test_poll_answer(dispatcher):
     poll_answer_update = utils.poll_answer_update()
 
     calls = list()
     updates = list()
 
-    def poll_answer_handler(c, u):
+    async def poll_answer_handler(c, u):
         updates.append(u)
         calls.append(poll_answer_handler)
 
     before_calls_counter = len(calls)
-    dispatcher.handle(poll_answer_update)
+    asyncio.run(dispatcher.handle(poll_answer_update))
     assert before_calls_counter == len(calls)
     dispatcher.register_poll_answer_handler(poll_answer_handler)
-    dispatcher.handle(poll_answer_update)
+    asyncio.run(dispatcher.handle(poll_answer_update))
     assert calls[-1] is poll_answer_handler
     assert updates[-1] is poll_answer_update
 
 
 def test_photo(dispatcher):
     photo_update = utils.photo_update()
     message_update = utils.message_update_by_text('message')
 
     calls = list()
     updates = list()
 
-    def photo_handler(c, u):
+    async def photo_handler(c, u):
         updates.append(u)
         calls.append(photo_handler)
 
-    def message_handler(c, u):
+    async def message_handler(c, u):
         updates.append(u)
         calls.append(message_handler)
 
     dispatcher.register_message_handler(re.compile('.*'), message_handler)
-    dispatcher.handle(message_update)
-    dispatcher.handle(photo_update)
+    asyncio.run(dispatcher.handle(message_update))
+    asyncio.run(dispatcher.handle(photo_update))
     assert calls[-1] is message_handler
     assert updates[-1] is message_update
     dispatcher.register_photo_handler(photo_handler)
-    dispatcher.handle(photo_update)
+    asyncio.run(dispatcher.handle(photo_update))
     assert calls[-1] is photo_handler
     assert updates[-1] is photo_update
 
 
 def test_sticker(dispatcher):
     sticker_update = utils.sticker_update()
     message_update = utils.message_update_by_text('message')
 
     calls = list()
     updates = list()
 
-    def sticker_handler(c, u):
+    async def sticker_handler(c, u):
         updates.append(u)
         calls.append(sticker_handler)
 
-    def message_handler(c, u):
+    async def message_handler(c, u):
         updates.append(u)
         calls.append(message_handler)
 
     dispatcher.register_message_handler(re.compile('.*'), message_handler)
-    dispatcher.handle(message_update)
-    dispatcher.handle(sticker_update)
+    asyncio.run(dispatcher.handle(message_update))
+    asyncio.run(dispatcher.handle(sticker_update))
     assert calls[-1] is message_handler
     assert updates[-1] is message_update
     dispatcher.register_sticker_handler(sticker_handler)
-    dispatcher.handle(sticker_update)
+    asyncio.run(dispatcher.handle(sticker_update))
     assert calls[-1] is sticker_handler
     assert updates[-1] is sticker_update
 
 
 def test_video(dispatcher):
     video_update = utils.video_update()
     message_update = utils.message_update_by_text('message')
 
     calls = list()
     updates = list()
 
-    def video_handler(c, u):
+    async def video_handler(c, u):
         updates.append(u)
         calls.append(video_handler)
 
-    def message_handler(c, u):
+    async def message_handler(c, u):
         updates.append(u)
         calls.append(message_handler)
 
     dispatcher.register_message_handler(re.compile('.*'), message_handler)
-    dispatcher.handle(message_update)
-    dispatcher.handle(video_update)
+    asyncio.run(dispatcher.handle(message_update))
+    asyncio.run(dispatcher.handle(video_update))
     assert calls[-1] is message_handler
     assert updates[-1] is message_update
     dispatcher.register_video_handler(video_handler)
-    dispatcher.handle(video_update)
+    asyncio.run(dispatcher.handle(video_update))
     assert calls[-1] is video_handler
     assert updates[-1] is video_update
 
 
 def test_video_note(dispatcher):
     video_note_update = utils.video_note_update()
     message_update = utils.message_update_by_text('message')
 
     calls = list()
     updates = list()
 
-    def video_note_handler(c, u):
+    async def video_note_handler(c, u):
         updates.append(u)
         calls.append(video_note_handler)
 
-    def message_handler(c, u):
+    async def message_handler(c, u):
         updates.append(u)
         calls.append(message_handler)
 
     dispatcher.register_message_handler(re.compile('.*'), message_handler)
-    dispatcher.handle(message_update)
-    dispatcher.handle(video_note_update)
+    asyncio.run(dispatcher.handle(message_update))
+    asyncio.run(dispatcher.handle(video_note_update))
     assert calls[-1] is message_handler
     assert updates[-1] is message_update
     dispatcher.register_video_note_handler(video_note_handler)
-    dispatcher.handle(video_note_update)
+    asyncio.run(dispatcher.handle(video_note_update))
     assert calls[-1] is video_note_handler
     assert updates[-1] is video_note_update
 
 
 def test_voice(dispatcher):
     voice_update = utils.voice_update()
     message_update = utils.message_update_by_text('message')
 
     calls = list()
     updates = list()
 
-    def voice_handler(c, u):
+    async def voice_handler(c, u):
         updates.append(u)
         calls.append(voice_handler)
 
-    def message_handler(c, u):
+    async def message_handler(c, u):
         updates.append(u)
         calls.append(message_handler)
 
     dispatcher.register_message_handler(re.compile('.*'), message_handler)
-    dispatcher.handle(message_update)
-    dispatcher.handle(voice_update)
+    asyncio.run(dispatcher.handle(message_update))
+    asyncio.run(dispatcher.handle(voice_update))
     assert calls[-1] is message_handler
     assert updates[-1] is message_update
     dispatcher.register_voice_handler(voice_handler)
-    dispatcher.handle(voice_update)
+    asyncio.run(dispatcher.handle(voice_update))
     assert calls[-1] is voice_handler
     assert updates[-1] is voice_update
 
 
 def test_venue(dispatcher):
     venue_update = utils.venue_update()
     message_update = utils.message_update_by_text('message')
 
     calls = list()
     updates = list()
 
-    def venue_handler(c, u):
+    async def venue_handler(c, u):
         updates.append(u)
         calls.append(venue_handler)
 
-    def message_handler(c, u):
+    async def message_handler(c, u):
         updates.append(u)
         calls.append(message_handler)
 
     dispatcher.register_message_handler(re.compile('.*'), message_handler)
-    dispatcher.handle(message_update)
-    dispatcher.handle(venue_update)
+    asyncio.run(dispatcher.handle(message_update))
+    asyncio.run(dispatcher.handle(venue_update))
     assert calls[-1] is message_handler
     assert updates[-1] is message_update
     dispatcher.register_venue_handler(venue_handler)
-    dispatcher.handle(venue_update)
+    asyncio.run(dispatcher.handle(venue_update))
     assert calls[-1] is venue_handler
     assert updates[-1] is venue_update
 
 
 def test_match_sequence(dispatcher):
     abc_message_update = utils.message_update_by_text('abc')
 
     updates = list()
     calls = list()
 
-    def universal_handler(c, u):
+    async def universal_handler(c, u):
         updates.append(u)
         calls.append(universal_handler)
 
-    def abc_handler(c, u):
+    async def abc_handler(c, u):
         updates.append(u)
         calls.append(abc_handler)
 
     dispatcher.register_message_handler(re.compile('.*'), universal_handler)
     dispatcher.register_message_handler('abc', abc_handler)
-    dispatcher.handle(abc_message_update)
+    asyncio.run(dispatcher.handle(abc_message_update))
     assert calls[-1] is abc_handler
     assert updates[-1] is abc_message_update
 
 # TODO test_pre_checkout_query
 # TODO test_shipping_query
 # TODO test_connected_website
 # TODO test_game
```

## tests/test_dispatcher_decorator.py

```diff
@@ -1,446 +1,448 @@
+import asyncio
+
 from tests import utils
 
 
 def test_middleware(dispatcher):
     update = utils.message_update_by_text('test')
     calls = list()
 
     @dispatcher.middleware
-    def mw_first(u):
+    async def mw_first(u):
         calls.append(mw_first)
 
-    dispatcher.handle(update)
+    asyncio.run(dispatcher.handle(update))
     assert calls[-1] is mw_first
 
 
 def test_command_handler(dispatcher):
     a_command_update = utils.command_update_by_text('/a')
     b_command_update = utils.command_update_by_text('/b')
 
     updates = list()
     calls = list()
 
     @dispatcher.command_handler('/a')
-    def a_handler(c, u):
+    async def a_handler(c, u):
         updates.append(u)
         calls.append(a_handler)
 
-    dispatcher.handle(b_command_update)
+    asyncio.run(dispatcher.handle(b_command_update))
     assert not calls
-    dispatcher.handle(a_command_update)
+    asyncio.run(dispatcher.handle(a_command_update))
     assert calls[-1] is a_handler
     assert updates[-1] is a_command_update
 
 
 def test_callback_handler(dispatcher):
     a_callback_update = utils.callback_update_by_data('a')
     b_callback_update = utils.callback_update_by_data('b')
 
     updates = list()
     calls = list()
 
     @dispatcher.callback_handler('a')
-    def a_callback_handler(c, u):
+    async def a_callback_handler(c, u):
         updates.append(u)
         calls.append(a_callback_handler)
 
-    dispatcher.handle(b_callback_update)
+    asyncio.run(dispatcher.handle(b_callback_update))
     assert not calls
-    dispatcher.handle(a_callback_update)
+    asyncio.run(dispatcher.handle(a_callback_update))
     assert calls[-1] is a_callback_handler
     assert updates[-1] is a_callback_update
 
 
 def test_message_handler(dispatcher):
     a_message_update = utils.message_update_by_text('a')
     b_message_update = utils.message_update_by_text('b')
 
     updates = list()
     calls = list()
 
     @dispatcher.message_handler('a')
-    def a_message_handler(c, u):
+    async def a_message_handler(c, u):
         updates.append(u)
         calls.append(a_message_handler)
 
-    dispatcher.handle(b_message_update)
+    asyncio.run(dispatcher.handle(b_message_update))
     assert not calls
-    dispatcher.handle(a_message_update)
+    asyncio.run(dispatcher.handle(a_message_update))
     assert calls[-1] is a_message_handler
     assert updates[-1] is a_message_update
 
 
 def test_inline_handler(dispatcher):
     a_inline_update = utils.inline_query_update_by_query('a')
     b_inline_update = utils.inline_query_update_by_query('b')
 
     updates = list()
     calls = list()
 
     @dispatcher.inline_handler('a')
-    def a_inline_handler(c, u):
+    async def a_inline_handler(c, u):
         updates.append(u)
         calls.append(a_inline_handler)
 
-    dispatcher.handle(b_inline_update)
+    asyncio.run(dispatcher.handle(b_inline_update))
     assert not calls
-    dispatcher.handle(a_inline_update)
+    asyncio.run(dispatcher.handle(a_inline_update))
     assert calls[-1] is a_inline_handler
     assert updates[-1] is a_inline_update
 
 
 def test_channel_post_handler(dispatcher):
     channel_post_update = utils.channel_post_update()
 
     updates = list()
     calls = list()
 
     @dispatcher.channel_post_handler
-    def channel_post_handler(c, u):
+    async def channel_post_handler(c, u):
         updates.append(u)
         calls.append(channel_post_handler)
 
-    dispatcher.handle(channel_post_update)
+    asyncio.run(dispatcher.handle(channel_post_update))
     assert calls[-1] is channel_post_handler
     assert updates[-1] is channel_post_update
 
 
 def test_chosen_inline_result_handler(dispatcher):
     update = utils.chosen_inline_result_update()
 
     updates = list()
     calls = list()
 
     @dispatcher.chosen_inline_result_handler
-    def handler(c, u):
+    async def handler(c, u):
         updates.append(u)
         calls.append(handler)
 
-    dispatcher.handle(update)
+    asyncio.run(dispatcher.handle(update))
     assert calls[-1] is handler
     assert updates[-1] is update
 
 
 def test_edited_channel_post_handler(dispatcher):
     update = utils.edited_channel_post_update()
 
     updates = list()
     calls = list()
 
     @dispatcher.edited_channel_post_handler
-    def handler(c, u):
+    async def handler(c, u):
         updates.append(u)
         calls.append(handler)
 
-    dispatcher.handle(update)
+    asyncio.run(dispatcher.handle(update))
     assert calls[-1] is handler
     assert updates[-1] is update
 
 
 def test_edited_message_handler(dispatcher):
     update = utils.edited_message_update_by_text('message')
 
     updates = list()
     calls = list()
 
     @dispatcher.edited_message_handler
-    def handler(c, u):
+    async def handler(c, u):
         updates.append(u)
         calls.append(handler)
 
-    dispatcher.handle(update)
+    asyncio.run(dispatcher.handle(update))
     assert calls[-1] is handler
     assert updates[-1] is update
 
 
 def test_poll_handler(dispatcher):
     update = utils.poll_update()
 
     updates = list()
     calls = list()
 
     @dispatcher.poll_handler
-    def handler(c, u):
+    async def handler(c, u):
         updates.append(u)
         calls.append(handler)
 
-    dispatcher.handle(update)
+    asyncio.run(dispatcher.handle(update))
     assert calls[-1] is handler
     assert updates[-1] is update
 
 
 def test_poll_answer_handler(dispatcher):
     update = utils.poll_answer_update()
 
     updates = list()
     calls = list()
 
     @dispatcher.poll_answer_handler
-    def handler(c, u):
+    async def handler(c, u):
         updates.append(u)
         calls.append(handler)
 
-    dispatcher.handle(update)
+    asyncio.run(dispatcher.handle(update))
     assert calls[-1] is handler
     assert updates[-1] is update
 
 
 def test_dice_handler(dispatcher):
     update = utils.dice_update()
 
     updates = list()
     calls = list()
 
     @dispatcher.dice_handler
-    def handler(c, u):
+    async def handler(c, u):
         updates.append(u)
         calls.append(handler)
 
-    dispatcher.handle(update)
+    asyncio.run(dispatcher.handle(update))
     assert calls[-1] is handler
     assert updates[-1] is update
 
 
 def test_document_handler(dispatcher):
     update = utils.document_update()
 
     updates = list()
     calls = list()
 
     @dispatcher.document_handler
-    def handler(c, u):
+    async def handler(c, u):
         updates.append(u)
         calls.append(handler)
 
-    dispatcher.handle(update)
+    asyncio.run(dispatcher.handle(update))
     assert calls[-1] is handler
     assert updates[-1] is update
 
 
 def test_animation_handler(dispatcher):
     update = utils.animation_update()
 
     updates = list()
     calls = list()
 
     @dispatcher.animation_handler
-    def handler(c, u):
+    async def handler(c, u):
         updates.append(u)
         calls.append(handler)
 
-    dispatcher.handle(update)
+    asyncio.run(dispatcher.handle(update))
     assert calls[-1] is handler
     assert updates[-1] is update
 
 
 def test_audio_handler(dispatcher):
     update = utils.audio_update()
 
     updates = list()
     calls = list()
 
     @dispatcher.audio_handler
-    def handler(c, u):
+    async def handler(c, u):
         updates.append(u)
         calls.append(handler)
 
-    dispatcher.handle(update)
+    asyncio.run(dispatcher.handle(update))
     assert calls[-1] is handler
     assert updates[-1] is update
 
 
 def test_contact_handler(dispatcher):
     update = utils.contact_update()
 
     updates = list()
     calls = list()
 
     @dispatcher.contact_handler
-    def handler(c, u):
+    async def handler(c, u):
         updates.append(u)
         calls.append(handler)
 
-    dispatcher.handle(update)
+    asyncio.run(dispatcher.handle(update))
     assert calls[-1] is handler
     assert updates[-1] is update
 
 
 def test_left_chat_member_handler(dispatcher):
     update = utils.left_chat_member_update()
 
     updates = list()
     calls = list()
 
     @dispatcher.left_chat_member_handler
-    def handler(c, u):
+    async def handler(c, u):
         updates.append(u)
         calls.append(handler)
 
-    dispatcher.handle(update)
+    asyncio.run(dispatcher.handle(update))
     assert calls[-1] is handler
     assert updates[-1] is update
 
 
 def test_location_handler(dispatcher):
     update = utils.location_update()
 
     updates = list()
     calls = list()
 
     @dispatcher.location_handler
-    def handler(c, u):
+    async def handler(c, u):
         updates.append(u)
         calls.append(handler)
 
-    dispatcher.handle(update)
+    asyncio.run(dispatcher.handle(update))
     assert calls[-1] is handler
     assert updates[-1] is update
 
 
 def test_new_chat_members_handler(dispatcher):
     update = utils.new_chat_members_update()
 
     updates = list()
     calls = list()
 
     @dispatcher.new_chat_members_handler
-    def handler(c, u):
+    async def handler(c, u):
         updates.append(u)
         calls.append(handler)
 
-    dispatcher.handle(update)
+    asyncio.run(dispatcher.handle(update))
     assert calls[-1] is handler
     assert updates[-1] is update
 
 
 def test_new_chat_photo_handler(dispatcher):
     update = utils.new_chat_photo_update()
 
     updates = list()
     calls = list()
 
     @dispatcher.new_chat_photo_handler
-    def handler(c, u):
+    async def handler(c, u):
         updates.append(u)
         calls.append(handler)
 
-    dispatcher.handle(update)
+    asyncio.run(dispatcher.handle(update))
     assert calls[-1] is handler
     assert updates[-1] is update
 
 
 def test_new_chat_title_handler(dispatcher):
     update = utils.new_chat_title_update()
 
     updates = list()
     calls = list()
 
     @dispatcher.new_chat_title_handler
-    def handler(c, u):
+    async def handler(c, u):
         updates.append(u)
         calls.append(handler)
 
-    dispatcher.handle(update)
+    asyncio.run(dispatcher.handle(update))
     assert calls[-1] is handler
     assert updates[-1] is update
 
 
 def test_photo_handler(dispatcher):
     update = utils.photo_update()
 
     updates = list()
     calls = list()
 
     @dispatcher.photo_handler
-    def handler(c, u):
+    async def handler(c, u):
         updates.append(u)
         calls.append(handler)
 
-    dispatcher.handle(update)
+    asyncio.run(dispatcher.handle(update))
     assert calls[-1] is handler
     assert updates[-1] is update
 
 
 def test_sticker_handler(dispatcher):
     update = utils.sticker_update()
 
     updates = list()
     calls = list()
 
     @dispatcher.sticker_handler
-    def handler(c, u):
+    async def handler(c, u):
         updates.append(u)
         calls.append(handler)
 
-    dispatcher.handle(update)
+    asyncio.run(dispatcher.handle(update))
     assert calls[-1] is handler
     assert updates[-1] is update
 
 
 def test_venue_handler(dispatcher):
     update = utils.venue_update()
 
     updates = list()
     calls = list()
 
     @dispatcher.venue_handler
-    def handler(c, u):
+    async def handler(c, u):
         updates.append(u)
         calls.append(handler)
 
-    dispatcher.handle(update)
+    asyncio.run(dispatcher.handle(update))
     assert calls[-1] is handler
     assert updates[-1] is update
 
 
 def test_video_handler(dispatcher):
     update = utils.video_update()
 
     updates = list()
     calls = list()
 
     @dispatcher.video_handler
-    def handler(c, u):
+    async def handler(c, u):
         updates.append(u)
         calls.append(handler)
 
-    dispatcher.handle(update)
+    asyncio.run(dispatcher.handle(update))
     assert calls[-1] is handler
     assert updates[-1] is update
 
 
 def test_video_note_handler(dispatcher):
     update = utils.video_note_update()
 
     updates = list()
     calls = list()
 
     @dispatcher.video_note_handler
-    def handler(c, u):
+    async def handler(c, u):
         updates.append(u)
         calls.append(handler)
 
-    dispatcher.handle(update)
+    asyncio.run(dispatcher.handle(update))
     assert calls[-1] is handler
     assert updates[-1] is update
 
 
 def test_voice_handler(dispatcher):
     update = utils.voice_update()
 
     updates = list()
     calls = list()
 
     @dispatcher.voice_handler
-    def handler(c, u):
+    async def handler(c, u):
         updates.append(u)
         calls.append(handler)
 
-    dispatcher.handle(update)
+    asyncio.run(dispatcher.handle(update))
     assert calls[-1] is handler
     assert updates[-1] is update
 
 
 # TODO test_pre_checkout_query_handler
 # TODO test_shipping_query_handler
 # TODO test_connected_website_handler
```

## tests/test_dispatcher_registration.py

```diff
@@ -1,10 +1,10 @@
 import re
 
-from botup import handlers
+from botup.core import handlers
 
 
 def middleware(u):
     pass
 
 
 def function(c, u):
```

## tests/test_serializing.py

```diff
@@ -1,8 +1,14 @@
-from botup.types import InlineKeyboardMarkup
+from botup.core.types import InlineKeyboardMarkup, InlineKeyboardButton
 
 
 def test_inline_keyboard_markup():
-    k = InlineKeyboardMarkup()
-    k.line(k.callback_data('text1', 'callback1'), k.callback_data('text2', 'callback2'))
-    k.line(k.url('text3', 'url'))
-    InlineKeyboardMarkup(**k.as_dict())
+    k = InlineKeyboardMarkup(
+        [
+            [InlineKeyboardButton('text1', callback_data='callback1'),
+             InlineKeyboardButton('text2', callback_data='callback2')],
+            [
+                InlineKeyboardButton('text3', url='url')
+            ]
+        ]
+    )
+    InlineKeyboardMarkup.from_dict(k.as_dict())
```

## tests/test_state_dispatcher.py

```diff
@@ -1,8 +1,10 @@
-from botup.dispatcher import DictStateManager, StateDispatcher, Dispatcher
+import asyncio
+
+from botup.core.dispatcher import DictStateManager, StateDispatcher, Dispatcher
 
 from tests import utils
 
 
 def test_reverse_dispatching():
     update = utils.command_update_by_text('/test')
     start_update = utils.command_update_by_text('/start')
@@ -16,58 +18,58 @@
     dispatcher.register_state('2', child_two)
 
     dispatcher_calls, dispatcher_updates = list(), list()
     child_one_calls, child_one_updates = list(), list()
     child_two_calls, child_two_updates = list(), list()
 
     @dispatcher.command_handler('test')
-    def dispatcher_test(c, u):
+    async def dispatcher_test(c, u):
         dispatcher_calls.append(dispatcher_test)
         dispatcher_updates.append(u)
 
     @dispatcher.command_handler('start')
-    def dispatcher_start(c, u):
+    async def dispatcher_start(c, u):
         dispatcher_calls.append(dispatcher_start)
         dispatcher_updates.append(u)
 
     @child_one.command_handler('test')
-    def child_one_test(c, u):
+    async def child_one_test(c, u):
         child_one_calls.append(child_one_test)
         child_one_updates.append(u)
 
     @child_two.command_handler('test')
-    def child_two_test(c, u):
+    async def child_two_test(c, u):
         child_two_calls.append(child_two_test)
         child_two_updates.append(u)
 
-    dispatcher.handle(update)
+    asyncio.run(dispatcher.handle(update))
     assert dispatcher_calls[-1] == dispatcher_test
     assert len(dispatcher_updates) == 1
     assert len(child_one_updates) == 0
     assert len(child_two_updates) == 0
 
     sm.update = update
     sm.set('main', '1')
 
-    dispatcher.handle(update)
+    asyncio.run(dispatcher.handle(update))
     assert child_one_calls[-1] == child_one_test
     assert len(dispatcher_updates) == 1
     assert len(child_one_updates) == 1
     assert len(child_two_updates) == 0
 
     sm.update = update
     sm.set('main', '2')
 
-    dispatcher.handle(update)
+    asyncio.run(dispatcher.handle(update))
     assert child_two_calls[-1] == child_two_test
     assert len(dispatcher_updates) == 1
     assert len(child_one_updates) == 1
     assert len(child_two_updates) == 1
 
-    dispatcher.handle(start_update)
+    asyncio.run(dispatcher.handle(start_update))
     assert dispatcher_calls[-1] == dispatcher_start
     assert dispatcher_updates[-1] == start_update
     assert len(dispatcher_updates) == 2
     assert len(child_one_updates) == 1
     assert len(child_two_updates) == 1
 
 
@@ -77,37 +79,37 @@
     sm = DictStateManager()
     dispatcher = StateDispatcher(sm, 'main')
     child_one = Dispatcher()
     dispatcher.register_state('1', child_one)
     dispatcher_updates = list()
 
     @dispatcher.command_handler('test')
-    def dispatcher_test(c, u):
+    async def dispatcher_test(c, u):
         dispatcher_updates.append(u)
 
-    dispatcher.handle(update)
+    asyncio.run(dispatcher.handle(update))
     assert len(dispatcher_updates) == 1
 
     sm.update = update
     sm.set('main', '1')
 
-    dispatcher.handle(update)
+    asyncio.run(dispatcher.handle(update))
     assert len(dispatcher_updates) == 2
 
     # with direct handling
 
     @dispatcher.command_handler('test')
     @dispatcher.direct_handling
-    def dispatcher_test_direct_handling(c, u):
+    async def dispatcher_test_direct_handling(c, u):
         dispatcher_updates.append(u)
 
     sm.update = update
     assert sm.get('main') == '1'
 
-    dispatcher.handle(update)
+    asyncio.run(dispatcher.handle(update))
     assert len(dispatcher_updates) == 2
 
     sm.update = update
     sm.reset('main')
     assert not sm.get('main')
-    dispatcher.handle(update)
+    asyncio.run(dispatcher.handle(update))
     assert len(dispatcher_updates) == 3
```

## tests/utils.py

```diff
@@ -1,8 +1,8 @@
-from botup.types import Update
+from botup.core.types import Update
 
 USER_FIRST_NAME = 'FirstName'
 USER_LAST_NAME = 'LastName'
 USER_USERNAME = 'username'
 USER_ID = 123456789
 BOT_NAME = 'BotName'
 BOT_USERNAME = 'botusername'
@@ -10,551 +10,557 @@
 GROUP_TITLE = 'GroupTitle'
 GROUP_ID = -456123789
 CHANNEL_TITLE = 'ChannelTitle'
 CHANNEL_ID = -654321987
 
 
 def message_update_by_text(text):
-    return Update(**{'message': {'chat': {'first_name': USER_FIRST_NAME,
-                                          'id': USER_ID,
-                                          'last_name': USER_LAST_NAME,
-                                          'type': 'private',
-                                          'username': USER_USERNAME},
-                                 'date': 1579384330,
-                                 'from': {'first_name': USER_FIRST_NAME,
-                                          'id': USER_ID,
-                                          'is_bot': False,
-                                          'language_code': 'en',
-                                          'last_name': USER_LAST_NAME,
-                                          'username': USER_USERNAME},
-                                 'message_id': 10590,
-                                 'text': text},
-                     'update_id': 751167721})
+    return Update.from_dict({'message': {'chat': {'first_name': USER_FIRST_NAME,
+                                                  'id': USER_ID,
+                                                  'last_name': USER_LAST_NAME,
+                                                  'type': 'private',
+                                                  'username': USER_USERNAME},
+                                         'date': 1579384330,
+                                         'from': {'first_name': USER_FIRST_NAME,
+                                                  'id': USER_ID,
+                                                  'is_bot': False,
+                                                  'language_code': 'en',
+                                                  'last_name': USER_LAST_NAME,
+                                                  'username': USER_USERNAME},
+                                         'message_id': 10590,
+                                         'text': text},
+                             'update_id': 751167721})
 
 
 def command_update_by_text(text):
-    return Update(**{'message': {'chat': {'first_name': USER_FIRST_NAME,
-                                          'id': USER_ID,
-                                          'last_name': USER_LAST_NAME,
-                                          'type': 'private',
-                                          'username': USER_USERNAME},
-                                 'date': 1579426411,
-                                 'entities': [{'length': 6, 'offset': 0, 'type': 'bot_command'}],
-                                 'from': {'first_name': USER_FIRST_NAME,
-                                          'id': USER_ID,
-                                          'is_bot': False,
-                                          'language_code': 'en',
-                                          'last_name': USER_LAST_NAME,
-                                          'username': USER_USERNAME},
-                                 'message_id': 10594,
-                                 'text': text},
-                     'update_id': 751167722})
+    return Update.from_dict({'message': {'chat': {'first_name': USER_FIRST_NAME,
+                                                  'id': USER_ID,
+                                                  'last_name': USER_LAST_NAME,
+                                                  'type': 'private',
+                                                  'username': USER_USERNAME},
+                                         'date': 1579426411,
+                                         'entities': [{'length': 6, 'offset': 0, 'type': 'bot_command'}],
+                                         'from': {'first_name': USER_FIRST_NAME,
+                                                  'id': USER_ID,
+                                                  'is_bot': False,
+                                                  'language_code': 'en',
+                                                  'last_name': USER_LAST_NAME,
+                                                  'username': USER_USERNAME},
+                                         'message_id': 10594,
+                                         'text': text},
+                             'update_id': 751167722})
 
 
 def callback_update_by_data(data):
-    return Update(**{'callback_query': {'chat_instance': '123',
-                                        'data': data,
-                                        'from': {'first_name': USER_FIRST_NAME,
-                                                 'id': USER_ID,
-                                                 'is_bot': False,
-                                                 'language_code': 'en',
-                                                 'last_name': USER_LAST_NAME,
-                                                 'username': USER_USERNAME},
-                                        'id': '123',
-                                        'message': {'chat': {'first_name': USER_FIRST_NAME,
-                                                             'id': USER_ID,
-                                                             'last_name': USER_LAST_NAME,
-                                                             'type': 'private',
-                                                             'username': USER_USERNAME},
-                                                    'date': 123,
-                                                    'from_': {'first_name': BOT_NAME,
-                                                              'id': BOT_ID,
-                                                              'is_bot': True,
-                                                              'username': BOT_USERNAME},
-                                                    'message_id': 123,
-                                                    'text': 'test'}},
-                     'update_id': 123})
+    return Update.from_dict({'callback_query': {'chat_instance': '123',
+                                                'data': data,
+                                                'from': {'first_name': USER_FIRST_NAME,
+                                                         'id': USER_ID,
+                                                         'is_bot': False,
+                                                         'language_code': 'en',
+                                                         'last_name': USER_LAST_NAME,
+                                                         'username': USER_USERNAME},
+                                                'id': '123',
+                                                'message': {'chat': {'first_name': USER_FIRST_NAME,
+                                                                     'id': USER_ID,
+                                                                     'last_name': USER_LAST_NAME,
+                                                                     'type': 'private',
+                                                                     'username': USER_USERNAME},
+                                                            'date': 123,
+                                                            'from_': {'first_name': BOT_NAME,
+                                                                      'id': BOT_ID,
+                                                                      'is_bot': True,
+                                                                      'username': BOT_USERNAME},
+                                                            'message_id': 123,
+                                                            'text': 'test'}},
+                             'update_id': 123})
 
 
 def inline_query_update_by_query(query):
-    return Update(**{'inline_query': {'from': {'first_name': USER_FIRST_NAME,
-                                               'id': USER_ID,
-                                               'is_bot': False,
-                                               'language_code': 'en',
-                                               'last_name': USER_LAST_NAME,
-                                               'username': USER_USERNAME},
-                                      'id': '123',
-                                      'offset': '',
-                                      'query': query},
-                     'update_id': 123})
-
-
-def chosen_inline_result_update():
-    return Update(**{'chosen_inline_result': {'from': {'first_name': USER_FIRST_NAME,
+    return Update.from_dict({'inline_query': {'from': {'first_name': USER_FIRST_NAME,
                                                        'id': USER_ID,
                                                        'is_bot': False,
                                                        'language_code': 'en',
                                                        'last_name': USER_LAST_NAME,
                                                        'username': USER_USERNAME},
-                                              'query': 'share',
-                                              'result_id': '1'},
-                     'update_id': 123})
+                                              'id': '123',
+                                              'offset': '',
+                                              'query': query},
+                             'update_id': 123})
+
+
+def chosen_inline_result_update():
+    return Update.from_dict({'chosen_inline_result': {'from': {'first_name': USER_FIRST_NAME,
+                                                               'id': USER_ID,
+                                                               'is_bot': False,
+                                                               'language_code': 'en',
+                                                               'last_name': USER_LAST_NAME,
+                                                               'username': USER_USERNAME},
+                                                      'query': 'share',
+                                                      'result_id': '1'},
+                             'update_id': 123})
 
 
 def edited_message_update_by_text(text):
-    return Update(**{'edited_message': {'chat': {'first_name': USER_FIRST_NAME,
-                                                 'id': USER_ID,
-                                                 'last_name': USER_LAST_NAME,
-                                                 'type': 'private',
-                                                 'username': USER_USERNAME},
-                                        'date': 123,
-                                        'edit_date': 123,
-                                        'from': {'first_name': USER_FIRST_NAME,
-                                                 'id': USER_ID,
-                                                 'is_bot': False,
-                                                 'language_code': 'en',
-                                                 'last_name': USER_LAST_NAME,
-                                                 'username': USER_USERNAME},
-                                        'message_id': 123,
-                                        'text': text},
-                     'update_id': 123})
+    return Update.from_dict({'edited_message': {'chat': {'first_name': USER_FIRST_NAME,
+                                                         'id': USER_ID,
+                                                         'last_name': USER_LAST_NAME,
+                                                         'type': 'private',
+                                                         'username': USER_USERNAME},
+                                                'date': 123,
+                                                'edit_date': 123,
+                                                'from': {'first_name': USER_FIRST_NAME,
+                                                         'id': USER_ID,
+                                                         'is_bot': False,
+                                                         'language_code': 'en',
+                                                         'last_name': USER_LAST_NAME,
+                                                         'username': USER_USERNAME},
+                                                'message_id': 123,
+                                                'text': text},
+                             'update_id': 123})
 
 
 def channel_post_update():
-    return Update(**{'channel_post': {'chat': {'id': CHANNEL_ID,
-                                               'title': CHANNEL_TITLE,
-                                               'type': 'channel'},
-                                      'date': 123,
-                                      'message_id': 2,
-                                      'text': 'Channel post'},
-                     'update_id': 123})
+    return Update.from_dict({'channel_post': {'chat': {'id': CHANNEL_ID,
+                                                       'title': CHANNEL_TITLE,
+                                                       'type': 'channel'},
+                                              'date': 123,
+                                              'message_id': 2,
+                                              'text': 'Channel post'},
+                             'update_id': 123})
 
 
 def edited_channel_post_update():
-    return Update(**{'edited_channel_post': {'chat': {'id': CHANNEL_ID,
-                                                      'title': CHANNEL_TITLE,
-                                                      'type': 'channel'},
-                                             'date': 123,
-                                             'edit_date': 124,
-                                             'message_id': 2,
-                                             'text': 'Channel post 1234'},
-                     'update_id': 123})
+    return Update.from_dict({'edited_channel_post': {'chat': {'id': CHANNEL_ID,
+                                                              'title': CHANNEL_TITLE,
+                                                              'type': 'channel'},
+                                                     'date': 123,
+                                                     'edit_date': 124,
+                                                     'message_id': 2,
+                                                     'text': 'Channel post 1234'},
+                             'update_id': 123})
 
 
 def dice_update():
-    return Update(**{'message': {'chat': {'first_name': USER_FIRST_NAME,
-                                          'id': USER_ID,
-                                          'last_name': USER_LAST_NAME,
-                                          'type': 'private',
-                                          'username': USER_USERNAME},
-                                 'date': 123,
-                                 'dice': {'value': 6},
-                                 'from': {'first_name': USER_FIRST_NAME,
-                                          'id': USER_ID,
-                                          'is_bot': False,
-                                          'language_code': 'en',
-                                          'last_name': USER_LAST_NAME,
-                                          'username': USER_USERNAME},
-                                 'message_id': 2},
-                     'update_id': 123})
+    return Update.from_dict({'message': {'chat': {'first_name': USER_FIRST_NAME,
+                                                  'id': USER_ID,
+                                                  'last_name': USER_LAST_NAME,
+                                                  'type': 'private',
+                                                  'username': USER_USERNAME},
+                                         'date': 123,
+                                         'dice': {'value': 6, 'emoji': '😊'},
+                                         'from': {'first_name': USER_FIRST_NAME,
+                                                  'id': USER_ID,
+                                                  'is_bot': False,
+                                                  'language_code': 'en',
+                                                  'last_name': USER_LAST_NAME,
+                                                  'username': USER_USERNAME},
+                                         'message_id': 2},
+                             'update_id': 123})
 
 
 def document_update():
-    return Update(**{'message': {'chat': {'first_name': USER_FIRST_NAME,
-                                          'id': USER_ID,
-                                          'last_name': USER_LAST_NAME,
-                                          'type': 'private',
-                                          'username': USER_USERNAME},
-                                 'date': 123,
-                                 'document': {'file_id': '123',
-                                              'file_name': 'Title.txt',
-                                              'file_size': 105,
-                                              'file_unique_id': 'asfa',
-                                              'mime_type': 'text/plain'},
-                                 'from': {'first_name': USER_FIRST_NAME,
-                                          'id': USER_ID,
-                                          'is_bot': False,
-                                          'language_code': 'en',
-                                          'last_name': USER_LAST_NAME,
-                                          'username': USER_USERNAME},
-                                 'message_id': 123},
-                     'update_id': 123})
+    return Update.from_dict({'message': {'chat': {'first_name': USER_FIRST_NAME,
+                                                  'id': USER_ID,
+                                                  'last_name': USER_LAST_NAME,
+                                                  'type': 'private',
+                                                  'username': USER_USERNAME},
+                                         'date': 123,
+                                         'document': {'file_id': '123',
+                                                      'file_name': 'Title.txt',
+                                                      'file_size': 105,
+                                                      'file_unique_id': 'asfa',
+                                                      'mime_type': 'text/plain'},
+                                         'from': {'first_name': USER_FIRST_NAME,
+                                                  'id': USER_ID,
+                                                  'is_bot': False,
+                                                  'language_code': 'en',
+                                                  'last_name': USER_LAST_NAME,
+                                                  'username': USER_USERNAME},
+                                         'message_id': 123},
+                             'update_id': 123})
 
 
 def animation_update():
-    return Update(**{'message': {'animation': {'duration': 3,
-                                               'file_id': 'qwe',
-                                               'file_name': 'giphy.mp4',
-                                               'file_size': 253953,
-                                               'file_unique_id': 'asd',
-                                               'height': 270,
-                                               'mime_type': 'video/mp4',
-                                               'thumb': {
-                                                   'file_id': 'qwe',
-                                                   'file_size': 16022,
-                                                   'file_unique_id': 'asd',
-                                                   'height': 180,
-                                                   'width': 320},
-                                               'width': 480},
-                                 'chat': {'first_name': USER_FIRST_NAME,
-                                          'id': USER_ID,
-                                          'last_name': USER_LAST_NAME,
-                                          'type': 'private',
-                                          'username': USER_USERNAME},
-                                 'date': 123,
-                                 'document': {'file_id': 'qwe',
-                                              'file_name': 'giphy.mp4',
-                                              'file_size': 253953,
-                                              'file_unique_id': 'asd',
-                                              'mime_type': 'video/mp4',
-                                              'thumb': {
-                                                  'file_id': 'qwe',
-                                                  'file_size': 16022,
-                                                  'file_unique_id': 'asd',
-                                                  'height': 180,
-                                                  'width': 320}},
-                                 'from': {'first_name': USER_FIRST_NAME,
-                                          'id': USER_ID,
-                                          'is_bot': False,
-                                          'language_code': 'en',
-                                          'last_name': USER_LAST_NAME,
-                                          'username': USER_USERNAME},
-                                 'message_id': 123},
-                     'update_id': 123})
+    return Update.from_dict({'message': {'animation': {'duration': 3,
+                                                       'file_id': 'qwe',
+                                                       'file_name': 'giphy.mp4',
+                                                       'file_size': 253953,
+                                                       'file_unique_id': 'asd',
+                                                       'height': 270,
+                                                       'mime_type': 'video/mp4',
+                                                       'thumb': {
+                                                           'file_id': 'qwe',
+                                                           'file_size': 16022,
+                                                           'file_unique_id': 'asd',
+                                                           'height': 180,
+                                                           'width': 320},
+                                                       'width': 480},
+                                         'chat': {'first_name': USER_FIRST_NAME,
+                                                  'id': USER_ID,
+                                                  'last_name': USER_LAST_NAME,
+                                                  'type': 'private',
+                                                  'username': USER_USERNAME},
+                                         'date': 123,
+                                         'document': {'file_id': 'qwe',
+                                                      'file_name': 'giphy.mp4',
+                                                      'file_size': 253953,
+                                                      'file_unique_id': 'asd',
+                                                      'mime_type': 'video/mp4',
+                                                      'thumb': {
+                                                          'file_id': 'qwe',
+                                                          'file_size': 16022,
+                                                          'file_unique_id': 'asd',
+                                                          'height': 180,
+                                                          'width': 320}},
+                                         'from': {'first_name': USER_FIRST_NAME,
+                                                  'id': USER_ID,
+                                                  'is_bot': False,
+                                                  'language_code': 'en',
+                                                  'last_name': USER_LAST_NAME,
+                                                  'username': USER_USERNAME},
+                                         'message_id': 123},
+                             'update_id': 123})
 
 
 def audio_update():
-    return Update(**{'message': {'audio': {'duration': 187,
-                                           'file_id': 'qwe-_ustVZpRYE',
-                                           'file_size': 3005143,
-                                           'file_unique_id': 'asd',
-                                           'mime_type': 'audio/mpeg',
-                                           'performer': 'Performer',
-                                           'title': 'Title'},
-                                 'chat': {'first_name': USER_FIRST_NAME,
-                                          'id': USER_ID,
-                                          'last_name': USER_LAST_NAME,
-                                          'type': 'private',
-                                          'username': USER_USERNAME},
-                                 'date': 123,
-                                 'from_': {'first_name': USER_FIRST_NAME,
-                                           'id': USER_ID,
-                                           'is_bot': False,
-                                           'language_code': 'en',
-                                           'last_name': USER_LAST_NAME,
-                                           'username': USER_USERNAME},
-                                 'message_id': 123},
-                     'update_id': 123})
+    return Update.from_dict({'message': {'audio': {'duration': 187,
+                                                   'file_id': 'qwe-_ustVZpRYE',
+                                                   'file_size': 3005143,
+                                                   'file_unique_id': 'asd',
+                                                   'mime_type': 'audio/mpeg',
+                                                   'performer': 'Performer',
+                                                   'title': 'Title'},
+                                         'chat': {'first_name': USER_FIRST_NAME,
+                                                  'id': USER_ID,
+                                                  'last_name': USER_LAST_NAME,
+                                                  'type': 'private',
+                                                  'username': USER_USERNAME},
+                                         'date': 123,
+                                         'from_': {'first_name': USER_FIRST_NAME,
+                                                   'id': USER_ID,
+                                                   'is_bot': False,
+                                                   'language_code': 'en',
+                                                   'last_name': USER_LAST_NAME,
+                                                   'username': USER_USERNAME},
+                                         'message_id': 123},
+                             'update_id': 123})
 
 
 def contact_update():
-    return Update(**{'message': {'chat': {'first_name': USER_FIRST_NAME,
-                                          'id': USER_ID,
-                                          'last_name': USER_LAST_NAME,
-                                          'type': 'private',
-                                          'username': USER_USERNAME},
-                                 'contact': {'first_name': USER_FIRST_NAME,
-                                             'phone_number': '+123456789',
-                                             'user_id': USER_ID,
-                                             'vcard': 'BEGIN:VCARD \n'
-                                                      'VERSION:3.0 \n'
-                                                      'PRODID:-//Apple Inc.//iPhone OS '
-                                                      '13.1.2//EN \n'
-                                                      'N:;ContactName;;; \n'
-                                                      'FN:ContactName \n'
-                                                      'TEL;type=CELL;type=VOICE;type=pref:+123456789 \n'
-                                                      'END:VCARD \n'},
-                                 'date': 123,
-                                 'from_': {'first_name': USER_FIRST_NAME,
-                                           'id': USER_ID,
-                                           'is_bot': False,
-                                           'language_code': 'en',
-                                           'last_name': USER_LAST_NAME,
-                                           'username': USER_USERNAME},
-                                 'message_id': 123},
-                     'update_id': 123})
+    return Update.from_dict({'message': {'chat': {'first_name': USER_FIRST_NAME,
+                                                  'id': USER_ID,
+                                                  'last_name': USER_LAST_NAME,
+                                                  'type': 'private',
+                                                  'username': USER_USERNAME},
+                                         'contact': {'first_name': USER_FIRST_NAME,
+                                                     'phone_number': '+123456789',
+                                                     'user_id': USER_ID,
+                                                     'vcard': 'BEGIN:VCARD \n'
+                                                              'VERSION:3.0 \n'
+                                                              'PRODID:-//Apple Inc.//iPhone OS '
+                                                              '13.1.2//EN \n'
+                                                              'N:;ContactName;;; \n'
+                                                              'FN:ContactName \n'
+                                                              'TEL;type=CELL;type=VOICE;type=pref:+123456789 \n'
+                                                              'END:VCARD \n'},
+                                         'date': 123,
+                                         'from_': {'first_name': USER_FIRST_NAME,
+                                                   'id': USER_ID,
+                                                   'is_bot': False,
+                                                   'language_code': 'en',
+                                                   'last_name': USER_LAST_NAME,
+                                                   'username': USER_USERNAME},
+                                         'message_id': 123},
+                             'update_id': 123})
 
 
 def new_chat_members_update():
-    return Update(**{'message': {'chat': {'id': GROUP_ID,
-                                          'title': GROUP_TITLE,
-                                          'type': 'group'},
-                                 'date': 123,
-                                 'from': {'first_name': USER_FIRST_NAME,
-                                          'id': USER_ID,
-                                          'is_bot': False,
-                                          'language_code': 'en',
-                                          'last_name': USER_LAST_NAME,
-                                          'username': USER_USERNAME},
-                                 'message_id': 123,
-                                 'new_chat_members': [{'first_name': BOT_NAME,
-                                                       'id': BOT_ID,
-                                                       'is_bot': True,
-                                                       'username': BOT_USERNAME}]},
-                     'update_id': 123})
+    return Update.from_dict({'message': {'chat': {'id': GROUP_ID,
+                                                  'title': GROUP_TITLE,
+                                                  'type': 'group'},
+                                         'date': 123,
+                                         'from': {'first_name': USER_FIRST_NAME,
+                                                  'id': USER_ID,
+                                                  'is_bot': False,
+                                                  'language_code': 'en',
+                                                  'last_name': USER_LAST_NAME,
+                                                  'username': USER_USERNAME},
+                                         'message_id': 123,
+                                         'new_chat_members': [{'first_name': BOT_NAME,
+                                                               'id': BOT_ID,
+                                                               'is_bot': True,
+                                                               'username': BOT_USERNAME}]},
+                             'update_id': 123})
 
 
 def new_chat_title_update():
-    return Update(**{'message': {'chat': {'id': GROUP_ID,
-                                          'title': GROUP_TITLE,
-                                          'type': 'group'},
-                                 'date': 123,
-                                 'from': {'first_name': USER_FIRST_NAME,
-                                          'id': USER_ID,
-                                          'is_bot': False,
-                                          'language_code': 'en',
-                                          'last_name': USER_LAST_NAME,
-                                          'username': USER_USERNAME},
-                                 'message_id': 123,
-                                 'new_chat_title': GROUP_TITLE},
-                     'update_id': 123})
+    return Update.from_dict({'message': {'chat': {'id': GROUP_ID,
+                                                  'title': GROUP_TITLE,
+                                                  'type': 'group'},
+                                         'date': 123,
+                                         'from': {'first_name': USER_FIRST_NAME,
+                                                  'id': USER_ID,
+                                                  'is_bot': False,
+                                                  'language_code': 'en',
+                                                  'last_name': USER_LAST_NAME,
+                                                  'username': USER_USERNAME},
+                                         'message_id': 123,
+                                         'new_chat_title': GROUP_TITLE},
+                             'update_id': 123})
 
 
 def new_chat_photo_update():
-    return Update(**{'message': {'chat': {'id': GROUP_ID,
-                                          'title': GROUP_TITLE,
-                                          'type': 'group'},
-                                 'date': 123,
-                                 'from': {'first_name': USER_FIRST_NAME,
-                                          'id': USER_ID,
-                                          'is_bot': False,
-                                          'language_code': 'en',
-                                          'last_name': USER_LAST_NAME,
-                                          'username': USER_USERNAME},
-                                 'message_id': 123,
-                                 'new_chat_photo': [
-                                     {'file_id': 'qwe',
-                                      'file_size': 5790,
-                                      'file_unique_id': 'asd',
-                                      'height': 160,
-                                      'width': 160},
-                                     {'file_id': 'qwe',
-                                      'file_size': 17376,
-                                      'file_unique_id': 'asd',
-                                      'height': 320,
-                                      'width': 320},
-                                     {'file_id': 'qwe',
-                                      'file_size': 58606,
-                                      'file_unique_id': 'asd',
-                                      'height': 640,
-                                      'width': 640}]},
-                     'update_id': 123})
+    return Update.from_dict({'message': {'chat': {'id': GROUP_ID,
+                                                  'title': GROUP_TITLE,
+                                                  'type': 'group'},
+                                         'date': 123,
+                                         'from': {'first_name': USER_FIRST_NAME,
+                                                  'id': USER_ID,
+                                                  'is_bot': False,
+                                                  'language_code': 'en',
+                                                  'last_name': USER_LAST_NAME,
+                                                  'username': USER_USERNAME},
+                                         'message_id': 123,
+                                         'new_chat_photo': [
+                                             {'file_id': 'qwe',
+                                              'file_size': 5790,
+                                              'file_unique_id': 'asd',
+                                              'height': 160,
+                                              'width': 160},
+                                             {'file_id': 'qwe',
+                                              'file_size': 17376,
+                                              'file_unique_id': 'asd',
+                                              'height': 320,
+                                              'width': 320},
+                                             {'file_id': 'qwe',
+                                              'file_size': 58606,
+                                              'file_unique_id': 'asd',
+                                              'height': 640,
+                                              'width': 640}]},
+                             'update_id': 123})
 
 
 def left_chat_member_update():
-    return Update(**{'message': {'chat': {'id': GROUP_ID,
-                                          'title': GROUP_TITLE,
-                                          'type': 'group'},
-                                 'date': 123,
-                                 'from': {'first_name': USER_FIRST_NAME,
-                                          'id': USER_ID,
-                                          'is_bot': False,
-                                          'language_code': 'en',
-                                          'last_name': USER_LAST_NAME,
-                                          'username': USER_USERNAME},
-                                 'left_chat_member': {'first_name': BOT_NAME,
-                                                      'id': BOT_ID,
-                                                      'is_bot': True,
-                                                      'username': BOT_USERNAME},
-                                 'message_id': 123},
-                     'update_id': 123})
+    return Update.from_dict({'message': {'chat': {'id': GROUP_ID,
+                                                  'title': GROUP_TITLE,
+                                                  'type': 'group'},
+                                         'date': 123,
+                                         'from': {'first_name': USER_FIRST_NAME,
+                                                  'id': USER_ID,
+                                                  'is_bot': False,
+                                                  'language_code': 'en',
+                                                  'last_name': USER_LAST_NAME,
+                                                  'username': USER_USERNAME},
+                                         'left_chat_member': {'first_name': BOT_NAME,
+                                                              'id': BOT_ID,
+                                                              'is_bot': True,
+                                                              'username': BOT_USERNAME},
+                                         'message_id': 123},
+                             'update_id': 123})
 
 
 def location_update():
-    return Update(**{'message': {'chat': {'first_name': USER_FIRST_NAME,
-                                          'id': USER_ID,
-                                          'last_name': USER_LAST_NAME,
-                                          'type': 'private',
-                                          'username': USER_USERNAME},
-                                 'date': 123,
-                                 'from': {'first_name': USER_FIRST_NAME,
-                                          'id': USER_ID,
-                                          'is_bot': False,
-                                          'language_code': 'en',
-                                          'last_name': USER_LAST_NAME,
-                                          'username': USER_USERNAME},
-                                 'location': {'latitude': 11.111111, 'longitude': 11.111111},
-                                 'message_id': 123},
-                     'update_id': 123})
+    return Update.from_dict({'message': {'chat': {'first_name': USER_FIRST_NAME,
+                                                  'id': USER_ID,
+                                                  'last_name': USER_LAST_NAME,
+                                                  'type': 'private',
+                                                  'username': USER_USERNAME},
+                                         'date': 123,
+                                         'from': {'first_name': USER_FIRST_NAME,
+                                                  'id': USER_ID,
+                                                  'is_bot': False,
+                                                  'language_code': 'en',
+                                                  'last_name': USER_LAST_NAME,
+                                                  'username': USER_USERNAME},
+                                         'location': {'latitude': 11.111111, 'longitude': 11.111111},
+                                         'message_id': 123},
+                             'update_id': 123})
 
 
 def poll_update():
-    return Update(**{'poll': {'id': '123',
-                              'is_closed': False,
-                              'options': [{'text': 'option1', 'voter_count': 1},
-                                          {'text': 'option2', 'voter_count': 0},
-                                          {'text': 'option3', 'voter_count': 0}],
-                              'question': 'question?'},
-                     'update_id': 123})
+    return Update.from_dict({'poll': {'id': '123',
+                                      'total_voter_count': 3,
+                                      'is_anonymous': True,
+                                      'type': 'regular',
+                                      'allows_multiple_answers': True,
+                                      'is_closed': False,
+                                      'options': [{'text': 'option1', 'voter_count': 1},
+                                                  {'text': 'option2', 'voter_count': 0},
+                                                  {'text': 'option3', 'voter_count': 0}],
+                                      'question': 'question?'},
+                             'update_id': 123})
 
 
 def poll_answer_update():
-    return Update(**{'poll_answer': {'option_ids': [0],
-                                     'poll_id': '123',
-                                     'user': {'first_name': USER_FIRST_NAME,
-                                              'id': USER_ID,
-                                              'is_bot': False,
-                                              'language_code': 'en',
-                                              'last_name': USER_LAST_NAME,
-                                              'username': USER_USERNAME}},
-                     'update_id': 123})
+    return Update.from_dict({'poll_answer': {'option_ids': [0],
+                                             'poll_id': '123',
+                                             'user': {'first_name': USER_FIRST_NAME,
+                                                      'id': USER_ID,
+                                                      'is_bot': False,
+                                                      'language_code': 'en',
+                                                      'last_name': USER_LAST_NAME,
+                                                      'username': USER_USERNAME}},
+                             'update_id': 123})
 
 
 def photo_update():
-    return Update(**{'message': {'chat': {'first_name': USER_FIRST_NAME,
-                                          'id': USER_ID,
-                                          'last_name': USER_LAST_NAME,
-                                          'type': 'private',
-                                          'username': USER_USERNAME},
-                                 'date': 123,
-                                 'from': {'first_name': USER_FIRST_NAME,
-                                          'id': USER_ID,
-                                          'is_bot': False,
-                                          'language_code': 'en',
-                                          'last_name': USER_LAST_NAME,
-                                          'username': USER_USERNAME},
-                                 'message_id': 123,
-                                 'photo': [{'file_id': 'qwe',
-                                            'file_size': 12292,
-                                            'file_unique_id': 'asd',
-                                            'height': 320,
-                                            'width': 320},
-                                           {'file_id': 'qwe',
-                                            'file_size': 46695,
-                                            'file_unique_id': 'asd',
-                                            'height': 640,
-                                            'width': 640}]},
-                     'update_id': 123})
+    return Update.from_dict({'message': {'chat': {'first_name': USER_FIRST_NAME,
+                                                  'id': USER_ID,
+                                                  'last_name': USER_LAST_NAME,
+                                                  'type': 'private',
+                                                  'username': USER_USERNAME},
+                                         'date': 123,
+                                         'from': {'first_name': USER_FIRST_NAME,
+                                                  'id': USER_ID,
+                                                  'is_bot': False,
+                                                  'language_code': 'en',
+                                                  'last_name': USER_LAST_NAME,
+                                                  'username': USER_USERNAME},
+                                         'message_id': 123,
+                                         'photo': [{'file_id': 'qwe',
+                                                    'file_size': 12292,
+                                                    'file_unique_id': 'asd',
+                                                    'height': 320,
+                                                    'width': 320},
+                                                   {'file_id': 'qwe',
+                                                    'file_size': 46695,
+                                                    'file_unique_id': 'asd',
+                                                    'height': 640,
+                                                    'width': 640}]},
+                             'update_id': 123})
 
 
 def sticker_update():
-    return Update(**{'message': {'chat': {'first_name': USER_FIRST_NAME,
-                                          'id': USER_ID,
-                                          'last_name': USER_LAST_NAME,
-                                          'type': 'private',
-                                          'username': USER_USERNAME},
-                                 'date': 123,
-                                 'from': {'first_name': USER_FIRST_NAME,
-                                          'id': USER_ID,
-                                          'is_bot': False,
-                                          'language_code': 'en',
-                                          'last_name': USER_LAST_NAME,
-                                          'username': USER_USERNAME},
-                                 'message_id': 123,
-                                 'sticker': {'emoji': '😊',
-                                             'file_id': 'qwe',
-                                             'file_size': 56464,
-                                             'file_unique_id': 'asd',
-                                             'height': 512,
-                                             'is_animated': False,
-                                             'set_name': 'pussycat',
-                                             'thumb': {
-                                                 'file_id': 'qwe-ifbCEKgAEAQAHbQADeAoAAhYE',
-                                                 'file_size': 5648,
-                                                 'file_unique_id': 'asd',
-                                                 'height': 128,
-                                                 'width': 128},
-                                             'width': 512}},
-                     'update_id': 123})
+    return Update.from_dict({'message': {'chat': {'first_name': USER_FIRST_NAME,
+                                                  'id': USER_ID,
+                                                  'last_name': USER_LAST_NAME,
+                                                  'type': 'private',
+                                                  'username': USER_USERNAME},
+                                         'date': 123,
+                                         'from': {'first_name': USER_FIRST_NAME,
+                                                  'id': USER_ID,
+                                                  'is_bot': False,
+                                                  'language_code': 'en',
+                                                  'last_name': USER_LAST_NAME,
+                                                  'username': USER_USERNAME},
+                                         'message_id': 123,
+                                         'sticker': {'emoji': '😊',
+                                                     'type': 'regular',
+                                                     'is_video': False,
+                                                     'file_id': 'qwe',
+                                                     'file_size': 56464,
+                                                     'file_unique_id': 'asd',
+                                                     'height': 512,
+                                                     'is_animated': False,
+                                                     'set_name': 'pussycat',
+                                                     'thumb': {
+                                                         'file_id': 'qwe-ifbCEKgAEAQAHbQADeAoAAhYE',
+                                                         'file_size': 5648,
+                                                         'file_unique_id': 'asd',
+                                                         'height': 128,
+                                                         'width': 128},
+                                                     'width': 512}},
+                             'update_id': 123})
 
 
 def video_update():
-    return Update(**{'message': {'chat': {'first_name': USER_FIRST_NAME,
-                                          'id': USER_ID,
-                                          'last_name': USER_LAST_NAME,
-                                          'type': 'private',
-                                          'username': USER_USERNAME},
-                                 'date': 123,
-                                 'from': {'first_name': USER_FIRST_NAME,
-                                          'id': USER_ID,
-                                          'is_bot': False,
-                                          'language_code': 'en',
-                                          'last_name': USER_LAST_NAME,
-                                          'username': USER_USERNAME},
-                                 'message_id': 123,
-                                 'video': {'duration': 5,
-                                           'file_id': 'qwe',
-                                           'file_size': 537084,
-                                           'file_unique_id': 'asd',
-                                           'height': 560,
-                                           'mime_type': 'video/mp4',
-                                           'thumb': {'file_id': 'qwe',
-                                                     'file_size': 14353,
-                                                     'file_unique_id': 'asd',
-                                                     'height': 320,
-                                                     'width': 182},
-                                           'width': 320}},
-                     'update_id': 123})
+    return Update.from_dict({'message': {'chat': {'first_name': USER_FIRST_NAME,
+                                                  'id': USER_ID,
+                                                  'last_name': USER_LAST_NAME,
+                                                  'type': 'private',
+                                                  'username': USER_USERNAME},
+                                         'date': 123,
+                                         'from': {'first_name': USER_FIRST_NAME,
+                                                  'id': USER_ID,
+                                                  'is_bot': False,
+                                                  'language_code': 'en',
+                                                  'last_name': USER_LAST_NAME,
+                                                  'username': USER_USERNAME},
+                                         'message_id': 123,
+                                         'video': {'duration': 5,
+                                                   'file_id': 'qwe',
+                                                   'file_size': 537084,
+                                                   'file_unique_id': 'asd',
+                                                   'height': 560,
+                                                   'mime_type': 'video/mp4',
+                                                   'thumb': {'file_id': 'qwe',
+                                                             'file_size': 14353,
+                                                             'file_unique_id': 'asd',
+                                                             'height': 320,
+                                                             'width': 182},
+                                                   'width': 320}},
+                             'update_id': 123})
 
 
 def video_note_update():
-    return Update(**{'message': {'chat': {'first_name': USER_FIRST_NAME,
-                                          'id': USER_ID,
-                                          'last_name': USER_LAST_NAME,
-                                          'type': 'private',
-                                          'username': USER_USERNAME},
-                                 'date': 123,
-                                 'from': {'first_name': USER_FIRST_NAME,
-                                          'id': USER_ID,
-                                          'is_bot': False,
-                                          'language_code': 'en',
-                                          'last_name': USER_LAST_NAME,
-                                          'username': USER_USERNAME},
-                                 'message_id': 123,
-                                 'video_note': {'duration': 3,
-                                                'file_id': 'qwe-vHFBYE',
-                                                'file_size': 156977,
-                                                'file_unique_id': 'asd',
-                                                'length': 240,
-                                                'thumb': {
-                                                    'file_id': 'qwe',
-                                                    'file_size': 8225,
-                                                    'file_unique_id': 'asd',
-                                                    'height': 240,
-                                                    'width': 240}}},
-                     'update_id': 123})
+    return Update.from_dict({'message': {'chat': {'first_name': USER_FIRST_NAME,
+                                                  'id': USER_ID,
+                                                  'last_name': USER_LAST_NAME,
+                                                  'type': 'private',
+                                                  'username': USER_USERNAME},
+                                         'date': 123,
+                                         'from': {'first_name': USER_FIRST_NAME,
+                                                  'id': USER_ID,
+                                                  'is_bot': False,
+                                                  'language_code': 'en',
+                                                  'last_name': USER_LAST_NAME,
+                                                  'username': USER_USERNAME},
+                                         'message_id': 123,
+                                         'video_note': {'duration': 3,
+                                                        'file_id': 'qwe-vHFBYE',
+                                                        'file_size': 156977,
+                                                        'file_unique_id': 'asd',
+                                                        'length': 240,
+                                                        'thumb': {
+                                                            'file_id': 'qwe',
+                                                            'file_size': 8225,
+                                                            'file_unique_id': 'asd',
+                                                            'height': 240,
+                                                            'width': 240}}},
+                             'update_id': 123})
 
 
 def voice_update():
-    return Update(**{'message': {'chat': {'first_name': USER_FIRST_NAME,
-                                          'id': USER_ID,
-                                          'last_name': USER_LAST_NAME,
-                                          'type': 'private',
-                                          'username': USER_USERNAME},
-                                 'date': 123,
-                                 'from': {'first_name': USER_FIRST_NAME,
-                                          'id': USER_ID,
-                                          'is_bot': False,
-                                          'language_code': 'en',
-                                          'last_name': USER_LAST_NAME,
-                                          'username': USER_USERNAME},
-                                 'message_id': 123,
-                                 'voice': {'duration': 2,
-                                           'file_id': 'qwe',
-                                           'file_size': 10927,
-                                           'file_unique_id': 'asas',
-                                           'mime_type': 'audio/ogg'}},
-                     'update_id': 123})
+    return Update.from_dict({'message': {'chat': {'first_name': USER_FIRST_NAME,
+                                                  'id': USER_ID,
+                                                  'last_name': USER_LAST_NAME,
+                                                  'type': 'private',
+                                                  'username': USER_USERNAME},
+                                         'date': 123,
+                                         'from': {'first_name': USER_FIRST_NAME,
+                                                  'id': USER_ID,
+                                                  'is_bot': False,
+                                                  'language_code': 'en',
+                                                  'last_name': USER_LAST_NAME,
+                                                  'username': USER_USERNAME},
+                                         'message_id': 123,
+                                         'voice': {'duration': 2,
+                                                   'file_id': 'qwe',
+                                                   'file_size': 10927,
+                                                   'file_unique_id': 'asas',
+                                                   'mime_type': 'audio/ogg'}},
+                             'update_id': 123})
 
 
 def venue_update():
-    return Update(**{'message': {'chat': {'first_name': USER_FIRST_NAME,
-                                          'id': USER_ID,
-                                          'last_name': USER_LAST_NAME,
-                                          'type': 'private',
-                                          'username': USER_USERNAME},
-                                 'date': 123,
-                                 'from': {'first_name': USER_FIRST_NAME,
-                                          'id': USER_ID,
-                                          'is_bot': False,
-                                          'language_code': 'en',
-                                          'last_name': USER_LAST_NAME,
-                                          'username': USER_USERNAME},
-                                 'location': {'latitude': 11.111111, 'longitude': 11.111111},
-                                 'message_id': 123,
-                                 'venue': {'address': 'street, number',
-                                           'foursquare_id': 'abcdef123456789',
-                                           'foursquare_type': 'food/coffeeshop',
-                                           'location': {'latitude': 11.111111,
-                                                        'longitude': 11.111111},
-                                           'title': 'VenueTitle'}},
-                     'update_id': 123})
+    return Update.from_dict({'message': {'chat': {'first_name': USER_FIRST_NAME,
+                                                  'id': USER_ID,
+                                                  'last_name': USER_LAST_NAME,
+                                                  'type': 'private',
+                                                  'username': USER_USERNAME},
+                                         'date': 123,
+                                         'from': {'first_name': USER_FIRST_NAME,
+                                                  'id': USER_ID,
+                                                  'is_bot': False,
+                                                  'language_code': 'en',
+                                                  'last_name': USER_LAST_NAME,
+                                                  'username': USER_USERNAME},
+                                         'location': {'latitude': 11.111111, 'longitude': 11.111111},
+                                         'message_id': 123,
+                                         'venue': {'address': 'street, number',
+                                                   'foursquare_id': 'abcdef123456789',
+                                                   'foursquare_type': 'food/coffeeshop',
+                                                   'location': {'latitude': 11.111111,
+                                                                'longitude': 11.111111},
+                                                   'title': 'VenueTitle'}},
+                             'update_id': 123})
```

## Comparing `telegram_botup-0.9.2.dist-info/RECORD` & `telegram_botup-1.0.1.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,18 @@
-botup/__init__.py,sha256=9Kgv0TXNq0lmwC0aV5DKeJmW8nPcYSUWIEx4HTmGa_4,134
-botup/cli.py,sha256=GBvf_ixi1UD2eUwRq2_T4iYVspuCwnTmg-4QOcaWXts,4991
-botup/dispatcher.py,sha256=t-SS-Rof9BfWKWpvTll-ePH3xLA9j_v2nV4xAanR50E,27565
-botup/exceptions.py,sha256=Gjkhf-hQvJoUNVMuNvPaePAHrVDMbpWdJOMCgyhbNVM,193
-botup/handlers.py,sha256=oXu6xmkekeI7RmwsMEYQKk_rkjxXChrkO7DzNnGeQaM,4595
-botup/sender.py,sha256=LrUgRHudpxpPzgh1AegJGubO4sV_CEaABIsKUFd2xgw,60692
-botup/types.py,sha256=Io4MBouOYfOMz7L-f5vAt7CIXZ5uoe8NwPyXZlZixr8,44573
-botup/utils.py,sha256=UWPxS2jbS-FyNooJGSknPtao__K8ffrkDQ2iTps8FAk,1183
-botup/wsgi.py,sha256=diGPif4xq8rwhCXvULiZg2hORZDKmotTut5HxQo8Y3Q,5034
+botup/__init__.py,sha256=d4QHYmS_30j0hPN8NmNPnQ_Z0TphDRbu4MtQj9cT9e8,22
+botup/bot.py,sha256=WydZRSYhH9i7Xo3XRrR-6YwaKBe6OWS_tAR9MFaW37o,905
+botup/navigation.py,sha256=pEE4Jo0olM9ZvHsvag2HNrSyLjSW9mvtw0VFBLNkACE,1266
+botup/utils.py,sha256=79UXKDZmEjjKjrleFBEKyiT6wWDwbOFGDpeHn2-ehqw,331
+botup/widget.py,sha256=pGKgwWMvbdVnWS0pR7NjG7GCiAXxlyDFtkQC3c4yT4s,1948
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-tests/conftest.py,sha256=BcSh3IPdquV05eVZJF_JOtboAKibvQnuJDgj0CKqnes,103
-tests/test_dispatcher.py,sha256=QDhOgTcaGzHJnMcdubit76i0sorFn3ZdtLHyTK1QkNU,30297
-tests/test_dispatcher_decorator.py,sha256=PfbT87lkzlR1GYvFXMiT7l07M5_wxLbA9AzNSfJcVbE,10018
-tests/test_dispatcher_registration.py,sha256=CebiiYZ3jFTlm5jtvxr3Iv-JdSZCLvm0yNKipDrv_Xo,6703
-tests/test_serializing.py,sha256=6mJMAZa2cHXpxDrPduI8YjlvN_9SYquaLhZO_O1Kt7A,276
-tests/test_state_dispatcher.py,sha256=yYCNVQdczuW2LB2O9NpS0rnLs6zY4FTc-9rq6nuQYrk,3242
+tests/conftest.py,sha256=kvSuN6G_9iR8TyLWIHr437h6H91DOaX80d926VHJ-9Y,119
+tests/test_dispatcher.py,sha256=g8sHIub-5t46fqGNnrgkvlD-_mZdQboPxvByIaeNQwY,32361
+tests/test_dispatcher_decorator.py,sha256=Dm8M56aE5FI48Xxcm-1DmhlrEKPUr5nwiamHB0YLe7Q,10599
+tests/test_dispatcher_registration.py,sha256=iHYq-NEig8aHbjCh5u-vQuxC0AK-f_71BTLozQOY3YA,6708
+tests/test_serializing.py,sha256=otX8e4hKzrrbq8V5JSyKh5DewhrSRTwit9Q4rhb4XoY,441
+tests/test_state_dispatcher.py,sha256=OhzDHblYOoKR-EnbspBBWH5zUfvkv-NslZYvYrfgSDk,3403
 tests/test_utils.py,sha256=EGUK4AWS05NUR5Rq9EixEi-aGglZRhY5uQkHSDpFG6w,227
-tests/utils.py,sha256=WhGfOigkyTCTYr5DWHJ7XCvNtgDjQZmueDm7PK_z60U,31211
-telegram_botup-0.9.2.dist-info/METADATA,sha256=8OMPFNFoHrTKBwzw3vxWrU95pWeJsQqjqQ7nM8-jBbs,3734
-telegram_botup-0.9.2.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-telegram_botup-0.9.2.dist-info/entry_points.txt,sha256=es0AcHSLk9AbjmRUSCSWUAUQgQtMMhmlmvpwht3G1Ck,41
-telegram_botup-0.9.2.dist-info/top_level.txt,sha256=5xSddxEvjN25GjUZSsBTJZ1OyYrsPAApb5FXZUYYoLU,12
-telegram_botup-0.9.2.dist-info/RECORD,,
+tests/utils.py,sha256=ZJesYuEPqLPP2PWVIJyD8vatfQLybVreJsg3Qd0R9-k,35379
+telegram_botup-1.0.1.dist-info/METADATA,sha256=GIh1Mjhw5iOe9wqftn6hpiHwDHYMOGNIM_vpfNTEPoU,4496
+telegram_botup-1.0.1.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+telegram_botup-1.0.1.dist-info/top_level.txt,sha256=5xSddxEvjN25GjUZSsBTJZ1OyYrsPAApb5FXZUYYoLU,12
+telegram_botup-1.0.1.dist-info/RECORD,,
```

