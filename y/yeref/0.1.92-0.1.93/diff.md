# Comparing `tmp/yeref-0.1.92.tar.gz` & `tmp/yeref-0.1.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.1.92.tar", last modified: Mon Jun 12 18:24:20 2023, max compression
+gzip compressed data, was "yeref-0.1.93.tar", last modified: Tue Jun 13 14:31:00 2023, max compression
```

## Comparing `yeref-0.1.92.tar` & `yeref-0.1.93.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-12 18:24:20.152635 yeref-0.1.92/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-12 18:24:20.152811 yeref-0.1.92/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-12 18:24:20.154101 yeref-0.1.92/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1391 2023-06-12 18:24:03.000000 yeref-0.1.92/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-12 18:24:20.146036 yeref-0.1.92/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.92/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   547540 2023-06-12 16:51:53.000000 yeref-0.1.92/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   215610 2023-06-12 18:17:26.000000 yeref-0.1.92/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-12 18:24:20.152025 yeref-0.1.92/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-12 18:24:20.000000 yeref-0.1.92/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-12 18:24:20.000000 yeref-0.1.92/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-12 18:24:20.000000 yeref-0.1.92/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-12 18:24:20.000000 yeref-0.1.92/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-13 14:31:00.090739 yeref-0.1.93/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-13 14:31:00.090892 yeref-0.1.93/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-13 14:31:00.091555 yeref-0.1.93/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1391 2023-06-13 14:30:44.000000 yeref-0.1.93/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-13 14:31:00.085403 yeref-0.1.93/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.93/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   551418 2023-06-13 11:23:32.000000 yeref-0.1.93/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   210914 2023-06-13 13:35:20.000000 yeref-0.1.93/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-13 14:31:00.090309 yeref-0.1.93/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-13 14:31:00.000000 yeref-0.1.93/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-13 14:31:00.000000 yeref-0.1.93/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-13 14:31:00.000000 yeref-0.1.93/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-13 14:31:00.000000 yeref-0.1.93/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.1.92/setup.py` & `yeref-0.1.93/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.1.92',
+      version='0.1.93',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
@@ -43,12 +43,12 @@
 
 # twine upload dist/*
 # freey.sitner.ya
 # cejwez-nosgin-vaVfe7
 
 # python3 -m pip install --upgrade yeref
 
-# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.91-py3-none-any.whl
+# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.92-py3-none-any.whl
 # pip install --force-reinstall -v "yeref==0.1.30"
 # pip install https://github.com/aiogram/aiogram/archive/refs/heads/dev-3.x.zip
 # pip show aiogram
 # ARCHFLAGS="-arch x86_64" pip install pycurl
```

### Comparing `yeref-0.1.92/yeref/l_.py` & `yeref-0.1.93/yeref/l_.py`

 * *Files 0% similar despite different names*

```diff
@@ -347,14 +347,30 @@
     'ru': "✏️ 4. <b>Выбери дату</b> на календаре\n\n(<i>или нажми «➡️️/Next», чтобы пропустить этот шаг</i>)",
     'en': "✏️ 4. <b>Select a date</b> on the calendar\n\n( <i>or press &quot;➡️️/Next&quot; to skip this step</i> )",
     'es': "✏️ 4. <b>Selecciona una fecha</b> en el calendario\n\n( <i>o presiona &quot;➡️️/Siguiente&quot; para omitir este paso</i> )",
     'fr': "✏️ 4. <b>Sélectionnez une date</b> sur le calendrier\n\n( <i>ou appuyez sur &quot;➡️️/Suivant&quot; pour ignorer cette étape</i> )",
     'zh': "✏️ 4. 在日历上<b>选择一个日期</b>\n\n（<i>或按“➡️️/Next”跳过此步骤</i>）",
     'ar': "✏️ 4. <b>حدد تاريخًا</b> في التقويم\n\n( <i>أو اضغط على &quot;➡️️ / التالي&quot; لتخطي هذه الخطوة</i> )",
 }
+l_post_window = {
+    'ru': "✏️ *<b>Введи</b> текст (без форматирования) для <i>диалогового окна</i> при нажатии на <u>кнопки</u> <b>поста</b> (по умолчанию: ❤️)\n\n(<i>или нажми «➡️️/Next», чтобы пропустить этот шаг</i>)",
+    'en': "✅ <b>Post is ready</b>\n\n<i>Press &quot;➡️️/Next&quot; to confirm, and then press the button 🔗 Publish</i>",
+    'es': "✅ <b>La publicación está lista</b>\n\n<i>Presiona &quot;➡️️/Siguiente&quot; para confirmar y luego presiona el botón 🔗 Publicar</i>",
+    'fr': "✅ <b>La publication est prête</b>\n\n<i>Appuyez sur &quot;➡️️/Suivant&quot; pour confirmer, puis appuyez sur le bouton 🔗 Publier</i>",
+    'zh': "✅<b>发布准备就绪</b>\n\n<i>按“➡️️/Next”确认，然后按按钮🔗发布</i>",
+    'ar': "✅ <b>النشر جاهز</b>\n\n<i>اضغط على &quot;➡️️ / التالي&quot; للتأكيد ، ثم اضغط على الزر 🔗 نشر</i>",
+}
+l_post_window_limit = {
+    'ru': "❗️ <b>Количество символов</b> диалогового окна: <u>{0}</u> больше допустимых 200",
+    'en': "❗️ <b>Number of characters</b> of text ( <i>including formatting</i> ): <u>{0}</u> more than allowed 1024",
+    'es': "❗️ <b>Número de caracteres</b> de texto ( <i>incluido el formato</i> ): <u>{0}</u> más de los permitidos 1024",
+    'fr': "❗️ <b>Nombre de caractères</b> de texte ( <i>y compris le formatage</i> ) : <u>{0}</u> plus que autorisé 1024",
+    'zh': "❗️ 文本<b>字符数</b>（<i>包括格式</i>）： <u>{0}</u>超过允许的 1024",
+    'ar': "❗️ <b>عدد أحرف</b> النص ( <i>بما في ذلك التنسيق</i> ): <u>{0}</u> أكثر من العدد المسموح به وهو 1024",
+}
 l_post_finish = {
     'ru': "✅ <b>Пост готов</b>\n\n<i>Нажми «➡️️/Next», чтобы подтвердить, а затем на кнопку 🔗 Опубликовать</i>",
     'en': "✅ <b>Post is ready</b>\n\n<i>Press &quot;➡️️/Next&quot; to confirm, and then press the button 🔗 Publish</i>",
     'es': "✅ <b>La publicación está lista</b>\n\n<i>Presiona &quot;➡️️/Siguiente&quot; para confirmar y luego presiona el botón 🔗 Publicar</i>",
     'fr': "✅ <b>La publication est prête</b>\n\n<i>Appuyez sur &quot;➡️️/Suivant&quot; pour confirmer, puis appuyez sur le bouton 🔗 Publier</i>",
     'zh': "✅<b>发布准备就绪</b>\n\n<i>按“➡️️/Next”确认，然后按按钮🔗发布</i>",
     'ar': "✅ <b>النشر جاهز</b>\n\n<i>اضغط على &quot;➡️️ / التالي&quot; للتأكيد ، ثم اضغط على الزر 🔗 نشر</i>",
@@ -501,14 +517,31 @@
     'ru': "спойлер",
     'en': "spoiler",
     'es': "revelación",
     'fr': "divulgacher",
     'zh': "剧透",
     'ar': "المفسد",
 }
+l_notice = {
+    'ru': "нотис",
+    'en': "notice",
+    'es': "revelación",
+    'fr': "divulgacher",
+    'zh': "剧透",
+    'ar': "المفسد",
+}
+l_window = {
+    'ru': "окно",
+    'en': "window",
+    'es': "revelación",
+    'fr': "divulgacher",
+    'zh': "剧透",
+    'ar': "المفسد",
+}
+
 l_buttons_text = {
     'ru': "👩🏽‍💻 Режим [кнопки] доступен, если создана хотя бы 1 кнопка при создании поста",
     'en': "👩🏽‍💻 [Buttons] mode is available if at least 1 button is created when creating a post",
     'es': "👩🏽‍💻 El modo [Botones] está disponible si se crea al menos 1 botón al crear una publicación",
     'fr': "👩🏽‍💻 Le mode [Boutons] est disponible si au moins 1 bouton est créé lors de la création d'une publication",
     'zh': "👩🏽‍💻 如果在创建帖子时至少创建了 1 个按钮，则可以使用 [按钮] 模式",
     'ar': "يكون وضع [الأزرار] متاحًا إذا تم إنشاء زر واحد على الأقل عند إنشاء منشور",
@@ -533,14 +566,22 @@
     'ru': "👩🏽‍💻 Режим [спойлер] доступен для photo/gif/video",
     'en': "👩🏽‍💻 [spoiler] mode available for photo/gif/video",
     'es': "👩🏽‍💻 Modo [spoiler] disponible para foto/gif/video",
     'fr': "👩🏽‍💻 Mode [spoiler] disponible pour photo/gif/vidéo",
     'zh': "👩🏽‍💻 [剧透] 模式可用于照片/gif/视频",
     'ar': "👩🏽‍💻 وضع [المفسد] متاح للصور / gif / الفيديو",
 }
+l_window_text = {
+    'ru': "👩🏽‍💻 Режим [окно] доступен для постов с кнопками без ссылок",
+    'en': "👩🏽‍💻 [spoiler] mode available for photo/gif/video",
+    'es': "👩🏽‍💻 Modo [spoiler] disponible para foto/gif/video",
+    'fr': "👩🏽‍💻 Mode [spoiler] disponible pour photo/gif/vidéo",
+    'zh': "👩🏽‍💻 [剧透] 模式可用于照片/gif/视频",
+    'ar': "👩🏽‍💻 وضع [المفسد] متاح للصور / gif / الفيديو",
+}
 l_post_has_restricted = {
     'ru': "👩🏽‍💻 У вас premium-аккаунт! В настройках <b>[Конфиденциальность]</b> добавь @{0} в <i>исключения</i> для <b>[Голосовые сообщения]</b>, чтобы отобразить видео-заметку/голосовое",
     'en': "👩🏽‍💻 You have a premium account! In the <b>[Privacy]</b> settings, add @{0} to <i>the exclusions</i> for <b>[Voice Messages]</b> to display видео-заметку / голосовое",
     'es': "👩🏽‍💻 ¡Tienes una cuenta premium! En la configuración <b>de [Privacidad]</b> , agregue @{0} a <i>las exclusiones</i> de <b>[Mensajes de voz]</b> para mostrar видео-заметку / голосовое",
     'fr': "👩🏽‍💻 Vous avez un compte premium ! Dans les paramètres <b>[Confidentialité]</b> , ajoutez @{0} aux <i>exclusions</i> pour <b>[Messages vocaux]</b> pour afficher видео-заметку / голосовое",
     'zh': "👩🏽‍💻 您拥有高级帐户！在<b>[隐私]</b>设置中，将@{0}添加到<b>[语音消息]</b>的<i>排除项</i>中以显示видео-заметку / голосовое",
     'ar': "👩🏽‍💻 لديك حساب مميز! في إعدادات <b>[الخصوصية]</b> ، أضف @ {0} إلى <i>استثناءات</i> <b>[الرسائل الصوتية]</b> لعرض видео-заметку / голосовое",
@@ -1361,14 +1402,22 @@
     'en': "👩🏽‍💻 <b>Sign up for</b> a monthly\n\n¹ <i>subscription</i> to @{0}-bot [{1} ₽]\n▪️ no ads\n▪️ creative tasks\n² Subscribe to <u>all</u> bots [{2} ₽]",
     'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
     'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
     'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
     'ar': "👩🏽‍💻 <b>اشترك للحصول على</b> <i>اشتراك</i> شهري\n\n¹ في @ {0} -bot [{1} ₽]\n▪️ بلا إعلانات\n▪️ مهام إبداعية\n² اشترك في <u>جميع</u> برامج التتبُّع [{2} ₽]",
 }
 
+l_post_bot_button_push = {
+    'ru': "👩🏽‍💻 <b>Пользователь</b>: {0} нажал на: [{1}] (пост #<u>{2}</u>)",
+    'en': "👩🏽‍💻 <b>Пользователь</b>: {name} нажал на: [{button}] (пост #<u>{post_id}</u>)",
+    'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
+    'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
+    'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
+    'ar': "👩🏽‍💻 <b>اشترك للحصول على</b> <i>اشتراك</i> شهري\n\n¹ في @ {0} -bot [{1} ₽]\n▪️ بلا إعلانات\n▪️ مهام إبداعية\n² اشترك في <u>جميع</u> برامج التتبُّع [{2} ₽]",
+}
 # endregion
 
 
 # region FereyVPNBot
 l_vpn_btn1 = {
     'ru': "⛰️ VPN",
     'en': "⛰️ VPN",
```

### Comparing `yeref-0.1.92/yeref/yeref.py` & `yeref-0.1.93/yeref/yeref.py`

 * *Files 1% similar despite different names*

```diff
@@ -1158,22 +1158,22 @@
 
             OFFER_FILEID = OFFER_FILEID[current - 1] if message_id else OFFER_FILEID[0]
             OFFER_MEDIATYPE = OFFER_MEDIATYPE[current - 1] if message_id else OFFER_MEDIATYPE[0]
             OFFER_TGPHLINK = OFFER_TGPHLINK[current - 1] if message_id else OFFER_TGPHLINK[0]
 
         if OFFER_ISTGPH and OFFER_TGPHLINK and '[' not in OFFER_TGPHLINK:
             OFFER_MEDIATYPE = 'text'
-            OFFER_TEXT = OFFER_TEXT if OFFER_TEXT and OFFER_TEXT != '' else "."
+            OFFER_TEXT = OFFER_TEXT if OFFER_TEXT and OFFER_TEXT != '' else str_empty
             OFFER_TEXT = f"<a href='{OFFER_TGPHLINK}'>​</a>{OFFER_TEXT}"
 
             if OFFER_ISGALLERY:
+                OFFER_TEXT = '' if OFFER_TEXT == str_empty and OFFER_MEDIATYPE != 'text' else OFFER_TEXT
                 buttons = [
                     types.InlineKeyboardButton(text="←", callback_data=f'gallery_prev_{offer_id}_{current}_{len_}'),
-                    types.InlineKeyboardButton(text=f"{current}/{len_}",
-                                               callback_data=f'gallery_current_{offer_id}_{current}_{len_}'),
+                    types.InlineKeyboardButton(text=f"{current}/{len_}", switch_inline_query_current_chat=f"{offer_id} ~"),
                     types.InlineKeyboardButton(text="→", callback_data=f'gallery_next_{offer_id}_{current}_{len_}'),
                 ]
                 reply_markup.row(*buttons)
 
         if '[' in OFFER_MEDIATYPE and not message_id:
             media = []
             for i in range(0, len(OFFER_FILEID)):
@@ -1564,19 +1564,18 @@
         file_name_part = None
 
         if message.text == '⬅️ Prev':
             await bot.send_message(chat_id, yeref.l_post_text[lz])
             await state.set_state(FsmOffer.text)
         elif message.text in ['➡️️ Next', '/Next']:
             if not offer_text:
-                await bot.send_message(chat_id, yeref.l_post_text_empty[lz].format(yeref.l_post_text[lz]))
-                await state.set_state(FsmOffer.text)
-            else:
-                await generate_calendar_admin(bot, state, lz, chat_id)
-                await state.set_state(FsmOffer.date_)
+                await state.update_data(offer_text=str_empty)
+
+            await generate_calendar_admin(bot, state, lz, chat_id)
+            await state.set_state(FsmOffer.date_)
         else:
             await bot.send_message(chat_id, yeref.l_post_media_wait[lz].format('album', 1))
 
             for obj in album:
                 if obj.photo:
                     media_id = obj.photo[-1].file_id
                     media_type = 'photo'
@@ -1641,21 +1640,20 @@
         offer_text = data.get('offer_text', None)
 
         if message.text == '⬅️ Prev':
             await bot.send_message(chat_id, yeref.l_post_text[lz])
             await state.set_state(FsmOffer.text)
         elif message.text in ['➡️️ Next', '/Next']:
             if not offer_text:
-                await bot.send_message(chat_id, yeref.l_post_text_empty[lz].format(yeref.l_post_text[lz]))
-                await state.set_state(FsmOffer.text)
-            else:
-                text = yeref.l_post_button[lz].replace('XXXXX', message.chat.username) if message.chat.username else \
-                    yeref.l_post_button[lz].replace('XXXXX', '')
-                await bot.send_message(chat_id, text)
-                await state.set_state(FsmOffer.button)
+                await state.update_data(offer_text=str_empty)
+
+            text = yeref.l_post_button[lz].replace('XXXXX', message.chat.username) if message.chat.username else \
+                yeref.l_post_button[lz].replace('XXXXX', '')
+            await bot.send_message(chat_id, text)
+            await state.set_state(FsmOffer.button)
         else:
             file_name = file_name_part = file_id = file_id_note = file_type = None
             if message.text:
                 await bot.send_message(chat_id=chat_id, text=yeref.l_post_media[lz])
                 return
             elif message.photo:
                 file_id = message.photo[-1].file_id
@@ -2090,132 +2088,50 @@
         logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
         await asyncio.sleep(e.retry_after + 1)
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
 
 
-async def edit_inline(bot, post_id, inline_message_id, current, BASE_D):
-    result = None
-    try:
-        sql = "SELECT POST_TEXT, POST_MEDIATYPE, POST_FILEID, POST_FILEIDNOTE, POST_BUTTON, POST_ISBUTTON, " \
-              "POST_TGPHLINK, POST_ISTGPH, POST_ISGALLERY, POST_ISSPOILER FROM POST WHERE POST_ID=?"
-        data_posts = await db_select(sql, (post_id,), BASE_D)
-        if not len(data_posts): return
-        item = data_posts[0]
-        POST_TEXT, POST_MEDIATYPE, POST_FILEID, POST_FILEIDNOTE, POST_BUTTON, POST_ISBUTTON, POST_TGPHLINK, \
-            POST_ISTGPH, POST_ISGALLERY, POST_ISSPOILER = item
-
-        len_ = 0
-        POST_TEXT = POST_TEXT if POST_TEXT else ''
-        reply_markup = await create_replymarkup2(bot, post_id,
-                                                 POST_BUTTON) if POST_ISBUTTON else InlineKeyboardBuilder()
-
-        if '[' in POST_MEDIATYPE:
-            POST_FILEID = ast.literal_eval(POST_FILEID)
-            POST_MEDIATYPE = ast.literal_eval(POST_MEDIATYPE)
-            POST_TGPHLINK = ast.literal_eval(POST_TGPHLINK)
-
-            len_ = len(POST_FILEID)
-            POST_FILEID = POST_FILEID[0]
-            POST_MEDIATYPE = POST_MEDIATYPE[0]
-            POST_TGPHLINK = POST_TGPHLINK[0]
-
-        if POST_ISTGPH and POST_TGPHLINK:
-            POST_MEDIATYPE = 'text'
-            POST_TEXT = POST_TEXT if POST_TEXT and POST_TEXT != '' else "."
-            POST_TEXT = f"<a href='{POST_TGPHLINK}'>​</a>{POST_TEXT}"
-
-        if POST_ISGALLERY:
-            buttons = [
-                types.InlineKeyboardButton(text="←", callback_data=f'gal_prev_{post_id}_{current}_{len_}'),
-                types.InlineKeyboardButton(text=f"{current}/{len_}",
-                                           callback_data=f'gal_current_{post_id}_{current}_{len_}'),
-                types.InlineKeyboardButton(text="→", callback_data=f'gal_next_{post_id}_{current}_{len_}'),
-            ]
-            reply_markup.row(*buttons)
-
-        if POST_MEDIATYPE == 'text':
-            await bot.edit_message_text(inline_message_id=inline_message_id, text=POST_TEXT,
-                                        reply_markup=reply_markup.as_markup())
-        elif POST_MEDIATYPE == 'photo':
-            media = types.InputMediaPhoto(media=POST_FILEID, caption=POST_TEXT)
-            await bot.edit_message_media(media=media, inline_message_id=inline_message_id,
-                                         reply_markup=reply_markup.as_markup())
-        elif POST_MEDIATYPE == 'animation':
-            media = types.InputMediaAnimation(media=POST_FILEID, caption=POST_TEXT)
-            await bot.edit_message_media(media=media, inline_message_id=inline_message_id,
-                                         reply_markup=reply_markup.as_markup())
-        elif POST_MEDIATYPE == 'video':
-            media = types.InputMediaVideo(media=POST_FILEID, caption=POST_TEXT)
-            await bot.edit_message_media(media=media, inline_message_id=inline_message_id,
-                                         reply_markup=reply_markup.as_markup())
-        elif POST_MEDIATYPE == 'video_note':
-            media = types.InputMediaVideo(media=POST_FILEIDNOTE, caption=POST_TEXT)
-            await bot.edit_message_media(media=media, inline_message_id=inline_message_id,
-                                         reply_markup=reply_markup.as_markup())
-        elif POST_MEDIATYPE == 'audio':
-            media = types.InputMediaAudio(media=POST_FILEID, caption=POST_TEXT)
-            await bot.edit_message_media(media=media, inline_message_id=inline_message_id,
-                                         reply_markup=reply_markup.as_markup())
-        elif POST_MEDIATYPE == 'voice':
-            media = types.InputMediaAudio(media=POST_FILEIDNOTE, caption=POST_TEXT)
-            await bot.edit_message_media(media=media, inline_message_id=inline_message_id,
-                                         reply_markup=reply_markup.as_markup())
-        elif POST_MEDIATYPE == 'document':
-            media = types.InputMediaDocument(media=POST_FILEID, caption=POST_TEXT)
-            await bot.edit_message_media(media=media, inline_message_id=inline_message_id,
-                                         reply_markup=reply_markup.as_markup())
-        else:
-            media = types.InputMedia(media=POST_FILEID, caption=POST_TEXT)
-            await bot.edit_message_media(media=media, inline_message_id=inline_message_id,
-                                         reply_markup=reply_markup.as_markup())
-    except Exception as e:
-        logger.info(log_ % str(e))
-        await asyncio.sleep(round(random.uniform(1, 2), 2))
-    finally:
-        return result
-
-
 async def edit_simple(bot, chat_id, post_id, message_id, current, BASE_D):
     result = None
     try:
         sql = "SELECT POST_TEXT, POST_MEDIATYPE, POST_FILEID, POST_FILEIDNOTE, POST_BUTTON, POST_ISBUTTON, " \
               "POST_TGPHLINK, POST_ISTGPH, POST_ISGALLERY, POST_ISSPOILER FROM POST WHERE POST_ID=?"
         data_posts = await db_select(sql, (post_id,), BASE_D)
         if not len(data_posts): return
         item = data_posts[0]
         POST_TEXT, POST_MEDIATYPE, POST_FILEID, POST_FILEIDNOTE, POST_BUTTON, POST_ISBUTTON, POST_TGPHLINK, \
             POST_ISTGPH, POST_ISGALLERY, POST_ISSPOILER = item
 
         len_ = 0
-        POST_TEXT = POST_TEXT if POST_TEXT else ''
+        POST_TEXT = POST_TEXT if POST_TEXT else str_empty
         reply_markup = await create_replymarkup2(bot, post_id,
                                                  POST_BUTTON) if POST_ISBUTTON else InlineKeyboardBuilder()
 
         if '[' in POST_MEDIATYPE and POST_ISGALLERY:
             POST_FILEID = ast.literal_eval(POST_FILEID)
             POST_MEDIATYPE = ast.literal_eval(POST_MEDIATYPE)
             POST_TGPHLINK = ast.literal_eval(POST_TGPHLINK)
 
             len_ = len(POST_FILEID)
-            POST_FILEID = POST_FILEID[0]
-            POST_MEDIATYPE = POST_MEDIATYPE[0]
-            POST_TGPHLINK = POST_TGPHLINK[0]
+            POST_FILEID = POST_FILEID[current - 1]
+            POST_MEDIATYPE = POST_MEDIATYPE[current - 1]
+            POST_TGPHLINK = POST_TGPHLINK[current - 1]
 
         if POST_ISTGPH and POST_TGPHLINK:
             POST_MEDIATYPE = 'text'
-            POST_TEXT = POST_TEXT if POST_TEXT and POST_TEXT != '' else "."
+            POST_TEXT = POST_TEXT if POST_TEXT and POST_TEXT != '' else str_empty
             POST_TEXT = f"<a href='{POST_TGPHLINK}'>​</a>{POST_TEXT}"
 
         if POST_ISGALLERY:
+            POST_TEXT = '' if POST_TEXT == str_empty and POST_MEDIATYPE != 'text' else POST_TEXT
             buttons = [
                 types.InlineKeyboardButton(text="←", callback_data=f'gal_prev_{post_id}_{current}_{len_}'),
-                types.InlineKeyboardButton(text=f"{current}/{len_}",
-                                           callback_data=f'gal_current_{post_id}_{current}_{len_}'),
+                types.InlineKeyboardButton(text=f"{current}/{len_}", switch_inline_query_current_chat=f"{post_id} ~"),
                 types.InlineKeyboardButton(text="→", callback_data=f'gal_next_{post_id}_{current}_{len_}'),
             ]
             reply_markup.row(*buttons)
 
         if POST_MEDIATYPE == 'text':
             await bot.edit_message_text(chat_id=chat_id, message_id=message_id, text=POST_TEXT,
                                         reply_markup=reply_markup.as_markup())
@@ -2250,14 +2166,15 @@
                                          reply_markup=reply_markup.as_markup())
         else:
             OFFER_FILEID = ast.literal_eval(POST_FILEID) if POST_FILEID and '[' in POST_FILEID else POST_FILEID
             OFFER_MEDIATYPE = ast.literal_eval(
                 POST_MEDIATYPE) if POST_MEDIATYPE and '[' in POST_MEDIATYPE else POST_MEDIATYPE
 
             media = []
+            POST_TEXT = None if POST_TEXT == str_empty else POST_TEXT
             for i in range(0, len(OFFER_FILEID)):
                 caption = POST_TEXT if i == 0 else None
 
                 if OFFER_MEDIATYPE[i] == 'photo':
                     media.append(
                         types.InputMediaPhoto(media=OFFER_FILEID[i], caption=caption, has_spoiler=POST_ISSPOILER))
                 elif OFFER_MEDIATYPE[i] == 'video':
```

