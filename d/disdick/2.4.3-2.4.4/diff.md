# Comparing `tmp/disdick-2.4.3.tar.gz` & `tmp/disdick-2.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "disdick-2.4.3.tar", last modified: Tue Jun 13 14:52:46 2023, max compression
+gzip compressed data, was "disdick-2.4.4.tar", last modified: Tue Jun 13 14:54:38 2023, max compression
```

## Comparing `disdick-2.4.3.tar` & `disdick-2.4.4.tar`

### file list

```diff
@@ -1,140 +1,140 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:52:46.531048 disdick-2.4.3/
--rw-r--r--   0 root         (0) root         (0)       44 2023-06-13 14:52:37.000000 disdick-2.4.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4396 2023-06-13 14:52:46.531048 disdick-2.4.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3231 2023-06-03 18:12:35.000000 disdick-2.4.3/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:52:46.507049 disdick-2.4.3/discord/
--rw-r--r--   0 root         (0) root         (0)     1951 2023-06-13 14:31:19.000000 disdick-2.4.3/discord/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11051 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/__main__.py
--rw-r--r--   0 root         (0) root         (0)     1410 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/_types.py
--rw-r--r--   0 root         (0) root         (0)    65794 2023-06-12 18:55:21.000000 disdick-2.4.3/discord/abc.py
--rw-r--r--   0 root         (0) root         (0)    26864 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/activity.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:52:46.511049 disdick-2.4.3/discord/app_commands/
--rw-r--r--   0 root         (0) root         (0)      424 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/app_commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18077 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/app_commands/checks.py
--rw-r--r--   0 root         (0) root         (0)    95614 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/app_commands/commands.py
--rw-r--r--   0 root         (0) root         (0)    19006 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/app_commands/errors.py
--rw-r--r--   0 root         (0) root         (0)    38500 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/app_commands/models.py
--rw-r--r--   0 root         (0) root         (0)    13123 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/app_commands/namespace.py
--rw-r--r--   0 root         (0) root         (0)    32499 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/app_commands/transformers.py
--rw-r--r--   0 root         (0) root         (0)    10686 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/app_commands/translator.py
--rw-r--r--   0 root         (0) root         (0)    47965 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/app_commands/tree.py
--rw-r--r--   0 root         (0) root         (0)    12713 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/appinfo.py
--rw-r--r--   0 root         (0) root         (0)    15839 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/asset.py
--rw-r--r--   0 root         (0) root         (0)    34652 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/audit_logs.py
--rw-r--r--   0 root         (0) root         (0)    23833 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/automod.py
--rw-r--r--   0 root         (0) root         (0)     3751 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/backoff.py
--rw-r--r--   0 root         (0) root         (0)   116580 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/channel.py
--rw-r--r--   0 root         (0) root         (0)    87180 2023-06-13 13:56:41.000000 disdick-2.4.3/discord/client.py
--rw-r--r--   0 root         (0) root         (0)    14242 2023-06-08 16:21:24.000000 disdick-2.4.3/discord/colour.py
--rw-r--r--   0 root         (0) root         (0)    16836 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/components.py
--rw-r--r--   0 root         (0) root         (0)     3032 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/context_managers.py
--rw-r--r--   0 root         (0) root         (0)    22722 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/embeds.py
--rw-r--r--   0 root         (0) root         (0)     8574 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/emoji.py
--rw-r--r--   0 root         (0) root         (0)    22242 2023-06-08 16:19:51.000000 disdick-2.4.3/discord/enums.py
--rw-r--r--   0 root         (0) root         (0)     9387 2023-06-03 11:19:26.000000 disdick-2.4.3/discord/errors.py
--rw-r--r--   0 root         (0) root         (0)     2730 2023-06-01 11:41:53.000000 disdick-2.4.3/discord/expiringdictionary.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:52:46.475050 disdick-2.4.3/discord/ext/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:52:46.519049 disdick-2.4.3/discord/ext/commands/
--rw-r--r--   0 root         (0) root         (0)      437 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/ext/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2638 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/ext/commands/_types.py
--rw-r--r--   0 root         (0) root         (0)    51719 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/ext/commands/bot.py
--rw-r--r--   0 root         (0) root         (0)    30163 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/ext/commands/cog.py
--rw-r--r--   0 root         (0) root         (0)    40048 2023-06-12 18:52:17.000000 disdick-2.4.3/discord/ext/commands/context.py
--rw-r--r--   0 root         (0) root         (0)    45780 2023-06-12 19:18:43.000000 disdick-2.4.3/discord/ext/commands/converter.py
--rw-r--r--   0 root         (0) root         (0)     9716 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/ext/commands/cooldowns.py
--rw-r--r--   0 root         (0) root         (0)    89681 2023-06-10 13:41:32.000000 disdick-2.4.3/discord/ext/commands/core.py
--rw-r--r--   0 root         (0) root         (0)    36354 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/ext/commands/errors.py
--rw-r--r--   0 root         (0) root         (0)    22966 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/ext/commands/flags.py
--rw-r--r--   0 root         (0) root         (0)    57705 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/ext/commands/help.py
--rw-r--r--   0 root         (0) root         (0)    36595 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/ext/commands/hybrid.py
--rw-r--r--   0 root         (0) root         (0)     8361 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/ext/commands/parameters.py
--rw-r--r--   0 root         (0) root         (0)     6247 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/ext/commands/view.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:52:46.519049 disdick-2.4.3/discord/ext/tasks/
--rw-r--r--   0 root         (0) root         (0)    29180 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/ext/tasks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5378 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/file.py
--rw-r--r--   0 root         (0) root         (0)    52266 2023-06-12 20:22:45.000000 disdick-2.4.3/discord/flags.py
--rw-r--r--   0 root         (0) root         (0)    35191 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/gateway.py
--rw-r--r--   0 root         (0) root         (0)   151023 2023-06-12 19:08:47.000000 disdick-2.4.3/discord/guild.py
--rw-r--r--   0 root         (0) root         (0)    93406 2023-06-10 14:01:26.000000 disdick-2.4.3/discord/http.py
--rw-r--r--   0 root         (0) root         (0)    13334 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/integrations.py
--rw-r--r--   0 root         (0) root         (0)    44610 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/interactions.py
--rw-r--r--   0 root         (0) root         (0)    20595 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/invite.py
--rw-r--r--   0 root         (0) root         (0)    42376 2023-06-12 19:12:46.000000 disdick-2.4.3/discord/member.py
--rw-r--r--   0 root         (0) root         (0)     5592 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/mentions.py
--rw-r--r--   0 root         (0) root         (0)    85805 2023-06-13 14:08:03.000000 disdick-2.4.3/discord/message.py
--rw-r--r--   0 root         (0) root         (0)     1485 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/mixins.py
--rw-r--r--   0 root         (0) root         (0)     3702 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/object.py
--rw-r--r--   0 root         (0) root         (0)     3646 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/oggparse.py
--rw-r--r--   0 root         (0) root         (0)    15065 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/opus.py
--rw-r--r--   0 root         (0) root         (0)     7950 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/partial_emoji.py
--rw-r--r--   0 root         (0) root         (0)    30255 2023-06-12 19:32:01.000000 disdick-2.4.3/discord/permissions.py
--rw-r--r--   0 root         (0) root         (0)    26460 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/player.py
--rw-r--r--   0 root         (0) root         (0)     1818 2023-06-08 16:53:31.000000 disdick-2.4.3/discord/pool.py
--rw-r--r--   0 root         (0) root         (0)     3493 2023-06-06 13:44:27.000000 disdick-2.4.3/discord/punishments.py
--rw-r--r--   0 root         (0) root         (0)    16826 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/raw_models.py
--rw-r--r--   0 root         (0) root         (0)     8229 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/reaction.py
--rw-r--r--   0 root         (0) root         (0)    18449 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/role.py
--rw-r--r--   0 root         (0) root         (0)    23629 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/scheduled_event.py
--rw-r--r--   0 root         (0) root         (0)    20414 2023-06-06 13:59:42.000000 disdick-2.4.3/discord/shard.py
--rw-r--r--   0 root         (0) root         (0)     6498 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/stage_instance.py
--rw-r--r--   0 root         (0) root         (0)    74000 2023-06-13 14:02:39.000000 disdick-2.4.3/discord/state.py
--rw-r--r--   0 root         (0) root         (0)    16039 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/sticker.py
--rw-r--r--   0 root         (0) root         (0)     4607 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/team.py
--rw-r--r--   0 root         (0) root         (0)     9574 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/template.py
--rw-r--r--   0 root         (0) root         (0)    32449 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/threads.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:52:46.527048 disdick-2.4.3/discord/types/
--rw-r--r--   0 root         (0) root         (0)      149 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/types/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2707 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/types/activity.py
--rw-r--r--   0 root         (0) root         (0)     2487 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/types/appinfo.py
--rw-r--r--   0 root         (0) root         (0)     8192 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/types/audit_log.py
--rw-r--r--   0 root         (0) root         (0)     4009 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/types/automod.py
--rw-r--r--   0 root         (0) root         (0)     4637 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/types/channel.py
--rw-r--r--   0 root         (0) root         (0)     6266 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/types/command.py
--rw-r--r--   0 root         (0) root         (0)     3057 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/types/components.py
--rw-r--r--   0 root         (0) root         (0)     2329 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/types/embed.py
--rw-r--r--   0 root         (0) root         (0)     1528 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/types/emoji.py
--rw-r--r--   0 root         (0) root         (0)     8453 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/types/gateway.py
--rw-r--r--   0 root         (0) root         (0)     5251 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/types/guild.py
--rw-r--r--   0 root         (0) root         (0)     2288 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/types/integration.py
--rw-r--r--   0 root         (0) root         (0)     6923 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/types/interactions.py
--rw-r--r--   0 root         (0) root         (0)     2704 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/types/invite.py
--rw-r--r--   0 root         (0) root         (0)     1898 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/types/member.py
--rw-r--r--   0 root         (0) root         (0)     4246 2023-06-12 20:27:32.000000 disdick-2.4.3/discord/types/message.py
--rw-r--r--   0 root         (0) root         (0)     1746 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/types/role.py
--rw-r--r--   0 root         (0) root         (0)     3294 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/types/scheduled_event.py
--rw-r--r--   0 root         (0) root         (0)     1182 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/types/snowflake.py
--rw-r--r--   0 root         (0) root         (0)     2257 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/types/sticker.py
--rw-r--r--   0 root         (0) root         (0)     1499 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/types/team.py
--rw-r--r--   0 root         (0) root         (0)     1609 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/types/template.py
--rw-r--r--   0 root         (0) root         (0)     2454 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/types/threads.py
--rw-r--r--   0 root         (0) root         (0)     3173 2023-06-12 19:01:26.000000 disdick-2.4.3/discord/types/user.py
--rw-r--r--   0 root         (0) root         (0)     2268 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/types/voice.py
--rw-r--r--   0 root         (0) root         (0)     1978 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/types/webhook.py
--rw-r--r--   0 root         (0) root         (0)     1460 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/types/welcome_screen.py
--rw-r--r--   0 root         (0) root         (0)     1883 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/types/widget.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:52:46.531048 disdick-2.4.3/discord/ui/
--rw-r--r--   0 root         (0) root         (0)      285 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/ui/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10620 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/ui/button.py
--rw-r--r--   0 root         (0) root         (0)     4372 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/ui/item.py
--rw-r--r--   0 root         (0) root         (0)     7012 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/ui/modal.py
--rw-r--r--   0 root         (0) root         (0)    34049 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/ui/select.py
--rw-r--r--   0 root         (0) root         (0)     8058 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/ui/text_input.py
--rw-r--r--   0 root         (0) root         (0)    22878 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/ui/view.py
--rw-r--r--   0 root         (0) root         (0)    15863 2023-06-12 19:05:18.000000 disdick-2.4.3/discord/user.py
--rw-r--r--   0 root         (0) root         (0)    41931 2023-06-12 20:29:02.000000 disdick-2.4.3/discord/utils.py
--rw-r--r--   0 root         (0) root         (0)    24974 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/voice_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:52:46.531048 disdick-2.4.3/discord/webhook/
--rw-r--r--   0 root         (0) root         (0)      182 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/webhook/__init__.py
--rw-r--r--   0 root         (0) root         (0)    69598 2023-06-12 19:20:29.000000 disdick-2.4.3/discord/webhook/async_.py
--rw-r--r--   0 root         (0) root         (0)    42591 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/webhook/sync.py
--rw-r--r--   0 root         (0) root         (0)     7539 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/welcome_screen.py
--rw-r--r--   0 root         (0) root         (0)    10168 2023-05-31 20:28:39.000000 disdick-2.4.3/discord/widget.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:52:46.531048 disdick-2.4.3/disdick.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4396 2023-06-13 14:52:46.000000 disdick-2.4.3/disdick.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3034 2023-06-13 14:52:46.000000 disdick-2.4.3/disdick.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 14:52:46.000000 disdick-2.4.3/disdick.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      373 2023-06-13 14:52:46.000000 disdick-2.4.3/disdick.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-13 14:52:46.000000 disdick-2.4.3/disdick.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       71 2023-06-11 16:32:56.000000 disdick-2.4.3/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       66 2023-06-13 14:52:46.531048 disdick-2.4.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2969 2023-06-13 14:52:26.000000 disdick-2.4.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:54:38.479806 disdick-2.4.4/
+-rw-r--r--   0 root         (0) root         (0)       44 2023-06-13 14:52:37.000000 disdick-2.4.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4396 2023-06-13 14:54:38.479806 disdick-2.4.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3231 2023-06-03 18:12:35.000000 disdick-2.4.4/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:54:38.455807 disdick-2.4.4/discord/
+-rw-r--r--   0 root         (0) root         (0)     1951 2023-06-13 14:31:19.000000 disdick-2.4.4/discord/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11051 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     1410 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/_types.py
+-rw-r--r--   0 root         (0) root         (0)    65794 2023-06-12 18:55:21.000000 disdick-2.4.4/discord/abc.py
+-rw-r--r--   0 root         (0) root         (0)    26864 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/activity.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:54:38.459807 disdick-2.4.4/discord/app_commands/
+-rw-r--r--   0 root         (0) root         (0)      424 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/app_commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18077 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/app_commands/checks.py
+-rw-r--r--   0 root         (0) root         (0)    95614 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/app_commands/commands.py
+-rw-r--r--   0 root         (0) root         (0)    19006 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/app_commands/errors.py
+-rw-r--r--   0 root         (0) root         (0)    38500 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/app_commands/models.py
+-rw-r--r--   0 root         (0) root         (0)    13123 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/app_commands/namespace.py
+-rw-r--r--   0 root         (0) root         (0)    32499 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/app_commands/transformers.py
+-rw-r--r--   0 root         (0) root         (0)    10686 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/app_commands/translator.py
+-rw-r--r--   0 root         (0) root         (0)    47965 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/app_commands/tree.py
+-rw-r--r--   0 root         (0) root         (0)    12713 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/appinfo.py
+-rw-r--r--   0 root         (0) root         (0)    15839 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/asset.py
+-rw-r--r--   0 root         (0) root         (0)    34652 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/audit_logs.py
+-rw-r--r--   0 root         (0) root         (0)    23833 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/automod.py
+-rw-r--r--   0 root         (0) root         (0)     3751 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/backoff.py
+-rw-r--r--   0 root         (0) root         (0)   116580 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/channel.py
+-rw-r--r--   0 root         (0) root         (0)    87180 2023-06-13 13:56:41.000000 disdick-2.4.4/discord/client.py
+-rw-r--r--   0 root         (0) root         (0)    14242 2023-06-08 16:21:24.000000 disdick-2.4.4/discord/colour.py
+-rw-r--r--   0 root         (0) root         (0)    16836 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/components.py
+-rw-r--r--   0 root         (0) root         (0)     3032 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/context_managers.py
+-rw-r--r--   0 root         (0) root         (0)    22722 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/embeds.py
+-rw-r--r--   0 root         (0) root         (0)     8574 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/emoji.py
+-rw-r--r--   0 root         (0) root         (0)    22242 2023-06-08 16:19:51.000000 disdick-2.4.4/discord/enums.py
+-rw-r--r--   0 root         (0) root         (0)     9387 2023-06-03 11:19:26.000000 disdick-2.4.4/discord/errors.py
+-rw-r--r--   0 root         (0) root         (0)     2730 2023-06-01 11:41:53.000000 disdick-2.4.4/discord/expiringdictionary.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:54:38.431807 disdick-2.4.4/discord/ext/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:54:38.463806 disdick-2.4.4/discord/ext/commands/
+-rw-r--r--   0 root         (0) root         (0)      437 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/ext/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2638 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/ext/commands/_types.py
+-rw-r--r--   0 root         (0) root         (0)    51719 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/ext/commands/bot.py
+-rw-r--r--   0 root         (0) root         (0)    30163 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/ext/commands/cog.py
+-rw-r--r--   0 root         (0) root         (0)    40048 2023-06-12 18:52:17.000000 disdick-2.4.4/discord/ext/commands/context.py
+-rw-r--r--   0 root         (0) root         (0)    45780 2023-06-12 19:18:43.000000 disdick-2.4.4/discord/ext/commands/converter.py
+-rw-r--r--   0 root         (0) root         (0)     9716 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/ext/commands/cooldowns.py
+-rw-r--r--   0 root         (0) root         (0)    89681 2023-06-10 13:41:32.000000 disdick-2.4.4/discord/ext/commands/core.py
+-rw-r--r--   0 root         (0) root         (0)    36354 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/ext/commands/errors.py
+-rw-r--r--   0 root         (0) root         (0)    22966 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/ext/commands/flags.py
+-rw-r--r--   0 root         (0) root         (0)    57705 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/ext/commands/help.py
+-rw-r--r--   0 root         (0) root         (0)    36595 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/ext/commands/hybrid.py
+-rw-r--r--   0 root         (0) root         (0)     8361 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/ext/commands/parameters.py
+-rw-r--r--   0 root         (0) root         (0)     6247 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/ext/commands/view.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:54:38.463806 disdick-2.4.4/discord/ext/tasks/
+-rw-r--r--   0 root         (0) root         (0)    29180 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/ext/tasks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5378 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/file.py
+-rw-r--r--   0 root         (0) root         (0)    52266 2023-06-12 20:22:45.000000 disdick-2.4.4/discord/flags.py
+-rw-r--r--   0 root         (0) root         (0)    35191 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/gateway.py
+-rw-r--r--   0 root         (0) root         (0)   151023 2023-06-12 19:08:47.000000 disdick-2.4.4/discord/guild.py
+-rw-r--r--   0 root         (0) root         (0)    93406 2023-06-10 14:01:26.000000 disdick-2.4.4/discord/http.py
+-rw-r--r--   0 root         (0) root         (0)    13334 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/integrations.py
+-rw-r--r--   0 root         (0) root         (0)    44610 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/interactions.py
+-rw-r--r--   0 root         (0) root         (0)    20595 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/invite.py
+-rw-r--r--   0 root         (0) root         (0)    42376 2023-06-12 19:12:46.000000 disdick-2.4.4/discord/member.py
+-rw-r--r--   0 root         (0) root         (0)     5592 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/mentions.py
+-rw-r--r--   0 root         (0) root         (0)    85805 2023-06-13 14:08:03.000000 disdick-2.4.4/discord/message.py
+-rw-r--r--   0 root         (0) root         (0)     1485 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/mixins.py
+-rw-r--r--   0 root         (0) root         (0)     3702 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/object.py
+-rw-r--r--   0 root         (0) root         (0)     3646 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/oggparse.py
+-rw-r--r--   0 root         (0) root         (0)    15065 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/opus.py
+-rw-r--r--   0 root         (0) root         (0)     7950 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/partial_emoji.py
+-rw-r--r--   0 root         (0) root         (0)    30255 2023-06-12 19:32:01.000000 disdick-2.4.4/discord/permissions.py
+-rw-r--r--   0 root         (0) root         (0)    26460 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/player.py
+-rw-r--r--   0 root         (0) root         (0)     1818 2023-06-08 16:53:31.000000 disdick-2.4.4/discord/pool.py
+-rw-r--r--   0 root         (0) root         (0)     3493 2023-06-06 13:44:27.000000 disdick-2.4.4/discord/punishments.py
+-rw-r--r--   0 root         (0) root         (0)    16826 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/raw_models.py
+-rw-r--r--   0 root         (0) root         (0)     8229 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/reaction.py
+-rw-r--r--   0 root         (0) root         (0)    18449 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/role.py
+-rw-r--r--   0 root         (0) root         (0)    23629 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/scheduled_event.py
+-rw-r--r--   0 root         (0) root         (0)    20414 2023-06-06 13:59:42.000000 disdick-2.4.4/discord/shard.py
+-rw-r--r--   0 root         (0) root         (0)     6498 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/stage_instance.py
+-rw-r--r--   0 root         (0) root         (0)    74000 2023-06-13 14:02:39.000000 disdick-2.4.4/discord/state.py
+-rw-r--r--   0 root         (0) root         (0)    16039 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/sticker.py
+-rw-r--r--   0 root         (0) root         (0)     4607 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/team.py
+-rw-r--r--   0 root         (0) root         (0)     9574 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/template.py
+-rw-r--r--   0 root         (0) root         (0)    32449 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/threads.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:54:38.471806 disdick-2.4.4/discord/types/
+-rw-r--r--   0 root         (0) root         (0)      149 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/types/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2707 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/types/activity.py
+-rw-r--r--   0 root         (0) root         (0)     2487 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/types/appinfo.py
+-rw-r--r--   0 root         (0) root         (0)     8192 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/types/audit_log.py
+-rw-r--r--   0 root         (0) root         (0)     4009 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/types/automod.py
+-rw-r--r--   0 root         (0) root         (0)     4637 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/types/channel.py
+-rw-r--r--   0 root         (0) root         (0)     6266 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/types/command.py
+-rw-r--r--   0 root         (0) root         (0)     3057 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/types/components.py
+-rw-r--r--   0 root         (0) root         (0)     2329 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/types/embed.py
+-rw-r--r--   0 root         (0) root         (0)     1528 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/types/emoji.py
+-rw-r--r--   0 root         (0) root         (0)     8453 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/types/gateway.py
+-rw-r--r--   0 root         (0) root         (0)     5251 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/types/guild.py
+-rw-r--r--   0 root         (0) root         (0)     2288 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/types/integration.py
+-rw-r--r--   0 root         (0) root         (0)     6923 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/types/interactions.py
+-rw-r--r--   0 root         (0) root         (0)     2704 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/types/invite.py
+-rw-r--r--   0 root         (0) root         (0)     1898 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/types/member.py
+-rw-r--r--   0 root         (0) root         (0)     4246 2023-06-12 20:27:32.000000 disdick-2.4.4/discord/types/message.py
+-rw-r--r--   0 root         (0) root         (0)     1746 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/types/role.py
+-rw-r--r--   0 root         (0) root         (0)     3294 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/types/scheduled_event.py
+-rw-r--r--   0 root         (0) root         (0)     1182 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/types/snowflake.py
+-rw-r--r--   0 root         (0) root         (0)     2257 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/types/sticker.py
+-rw-r--r--   0 root         (0) root         (0)     1499 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/types/team.py
+-rw-r--r--   0 root         (0) root         (0)     1609 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/types/template.py
+-rw-r--r--   0 root         (0) root         (0)     2454 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/types/threads.py
+-rw-r--r--   0 root         (0) root         (0)     3173 2023-06-12 19:01:26.000000 disdick-2.4.4/discord/types/user.py
+-rw-r--r--   0 root         (0) root         (0)     2268 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/types/voice.py
+-rw-r--r--   0 root         (0) root         (0)     1978 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/types/webhook.py
+-rw-r--r--   0 root         (0) root         (0)     1460 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/types/welcome_screen.py
+-rw-r--r--   0 root         (0) root         (0)     1883 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/types/widget.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:54:38.475806 disdick-2.4.4/discord/ui/
+-rw-r--r--   0 root         (0) root         (0)      285 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/ui/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10620 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/ui/button.py
+-rw-r--r--   0 root         (0) root         (0)     4372 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/ui/item.py
+-rw-r--r--   0 root         (0) root         (0)     7012 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/ui/modal.py
+-rw-r--r--   0 root         (0) root         (0)    34049 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/ui/select.py
+-rw-r--r--   0 root         (0) root         (0)     8058 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/ui/text_input.py
+-rw-r--r--   0 root         (0) root         (0)    22878 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/ui/view.py
+-rw-r--r--   0 root         (0) root         (0)    15863 2023-06-12 19:05:18.000000 disdick-2.4.4/discord/user.py
+-rw-r--r--   0 root         (0) root         (0)    41931 2023-06-12 20:29:02.000000 disdick-2.4.4/discord/utils.py
+-rw-r--r--   0 root         (0) root         (0)    24974 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/voice_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:54:38.475806 disdick-2.4.4/discord/webhook/
+-rw-r--r--   0 root         (0) root         (0)      182 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/webhook/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    69598 2023-06-12 19:20:29.000000 disdick-2.4.4/discord/webhook/async_.py
+-rw-r--r--   0 root         (0) root         (0)    42591 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/webhook/sync.py
+-rw-r--r--   0 root         (0) root         (0)     7539 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/welcome_screen.py
+-rw-r--r--   0 root         (0) root         (0)    10168 2023-05-31 20:28:39.000000 disdick-2.4.4/discord/widget.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:54:38.475806 disdick-2.4.4/disdick.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4396 2023-06-13 14:54:38.000000 disdick-2.4.4/disdick.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3034 2023-06-13 14:54:38.000000 disdick-2.4.4/disdick.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 14:54:38.000000 disdick-2.4.4/disdick.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      373 2023-06-13 14:54:38.000000 disdick-2.4.4/disdick.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-13 14:54:38.000000 disdick-2.4.4/disdick.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       71 2023-06-11 16:32:56.000000 disdick-2.4.4/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2023-06-13 14:54:38.503805 disdick-2.4.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2998 2023-06-13 14:54:33.000000 disdick-2.4.4/setup.py
```

### Comparing `disdick-2.4.3/PKG-INFO` & `disdick-2.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: disdick
-Version: 2.4.3
+Version: 2.4.4
 Summary: A Python wrapper for the Discord API
 Home-page: https://github.com/cop-discord/disdick
 Download-URL: https://github.com/cop-discord/disdick/archive/refs/tags/2.4.1.tar.gz
 Author: cop-discord
 License: MIT
 Project-URL: Documentation, https://discordpy.readthedocs.io/en/latest/
 Project-URL: Issue tracker, https://github.com/cop-discord/disdick/issues
```

### Comparing `disdick-2.4.3/README.rst` & `disdick-2.4.4/README.rst`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/__init__.py` & `disdick-2.4.4/discord/__init__.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/__main__.py` & `disdick-2.4.4/discord/__main__.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/_types.py` & `disdick-2.4.4/discord/_types.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/abc.py` & `disdick-2.4.4/discord/abc.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/activity.py` & `disdick-2.4.4/discord/activity.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/app_commands/checks.py` & `disdick-2.4.4/discord/app_commands/checks.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/app_commands/commands.py` & `disdick-2.4.4/discord/app_commands/commands.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/app_commands/errors.py` & `disdick-2.4.4/discord/app_commands/errors.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/app_commands/models.py` & `disdick-2.4.4/discord/app_commands/models.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/app_commands/namespace.py` & `disdick-2.4.4/discord/app_commands/namespace.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/app_commands/transformers.py` & `disdick-2.4.4/discord/app_commands/transformers.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/app_commands/translator.py` & `disdick-2.4.4/discord/app_commands/translator.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/app_commands/tree.py` & `disdick-2.4.4/discord/app_commands/tree.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/appinfo.py` & `disdick-2.4.4/discord/appinfo.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/asset.py` & `disdick-2.4.4/discord/asset.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/audit_logs.py` & `disdick-2.4.4/discord/audit_logs.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/automod.py` & `disdick-2.4.4/discord/automod.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/backoff.py` & `disdick-2.4.4/discord/backoff.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/channel.py` & `disdick-2.4.4/discord/channel.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/client.py` & `disdick-2.4.4/discord/client.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/colour.py` & `disdick-2.4.4/discord/colour.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/components.py` & `disdick-2.4.4/discord/components.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/context_managers.py` & `disdick-2.4.4/discord/context_managers.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/embeds.py` & `disdick-2.4.4/discord/embeds.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/emoji.py` & `disdick-2.4.4/discord/emoji.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/enums.py` & `disdick-2.4.4/discord/enums.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/errors.py` & `disdick-2.4.4/discord/errors.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/expiringdictionary.py` & `disdick-2.4.4/discord/expiringdictionary.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/ext/commands/_types.py` & `disdick-2.4.4/discord/ext/commands/_types.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/ext/commands/bot.py` & `disdick-2.4.4/discord/ext/commands/bot.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/ext/commands/cog.py` & `disdick-2.4.4/discord/ext/commands/cog.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/ext/commands/context.py` & `disdick-2.4.4/discord/ext/commands/context.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/ext/commands/converter.py` & `disdick-2.4.4/discord/ext/commands/converter.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/ext/commands/cooldowns.py` & `disdick-2.4.4/discord/ext/commands/cooldowns.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/ext/commands/core.py` & `disdick-2.4.4/discord/ext/commands/core.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/ext/commands/errors.py` & `disdick-2.4.4/discord/ext/commands/errors.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/ext/commands/flags.py` & `disdick-2.4.4/discord/ext/commands/flags.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/ext/commands/help.py` & `disdick-2.4.4/discord/ext/commands/help.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/ext/commands/hybrid.py` & `disdick-2.4.4/discord/ext/commands/hybrid.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/ext/commands/parameters.py` & `disdick-2.4.4/discord/ext/commands/parameters.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/ext/commands/view.py` & `disdick-2.4.4/discord/ext/commands/view.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/ext/tasks/__init__.py` & `disdick-2.4.4/discord/ext/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/file.py` & `disdick-2.4.4/discord/file.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/flags.py` & `disdick-2.4.4/discord/flags.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/gateway.py` & `disdick-2.4.4/discord/gateway.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/guild.py` & `disdick-2.4.4/discord/guild.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/http.py` & `disdick-2.4.4/discord/http.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/integrations.py` & `disdick-2.4.4/discord/integrations.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/interactions.py` & `disdick-2.4.4/discord/interactions.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/invite.py` & `disdick-2.4.4/discord/invite.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/member.py` & `disdick-2.4.4/discord/member.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/mentions.py` & `disdick-2.4.4/discord/mentions.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/message.py` & `disdick-2.4.4/discord/message.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/mixins.py` & `disdick-2.4.4/discord/mixins.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/object.py` & `disdick-2.4.4/discord/object.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/oggparse.py` & `disdick-2.4.4/discord/oggparse.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/opus.py` & `disdick-2.4.4/discord/opus.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/partial_emoji.py` & `disdick-2.4.4/discord/partial_emoji.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/permissions.py` & `disdick-2.4.4/discord/permissions.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/player.py` & `disdick-2.4.4/discord/player.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/pool.py` & `disdick-2.4.4/discord/pool.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/punishments.py` & `disdick-2.4.4/discord/punishments.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/raw_models.py` & `disdick-2.4.4/discord/raw_models.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/reaction.py` & `disdick-2.4.4/discord/reaction.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/role.py` & `disdick-2.4.4/discord/role.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/scheduled_event.py` & `disdick-2.4.4/discord/scheduled_event.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/shard.py` & `disdick-2.4.4/discord/shard.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/stage_instance.py` & `disdick-2.4.4/discord/stage_instance.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/state.py` & `disdick-2.4.4/discord/state.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/sticker.py` & `disdick-2.4.4/discord/sticker.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/team.py` & `disdick-2.4.4/discord/team.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/template.py` & `disdick-2.4.4/discord/template.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/threads.py` & `disdick-2.4.4/discord/threads.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/types/activity.py` & `disdick-2.4.4/discord/types/activity.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/types/appinfo.py` & `disdick-2.4.4/discord/types/appinfo.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/types/audit_log.py` & `disdick-2.4.4/discord/types/audit_log.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/types/automod.py` & `disdick-2.4.4/discord/types/automod.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/types/channel.py` & `disdick-2.4.4/discord/types/channel.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/types/command.py` & `disdick-2.4.4/discord/types/command.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/types/components.py` & `disdick-2.4.4/discord/types/components.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/types/embed.py` & `disdick-2.4.4/discord/types/embed.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/types/emoji.py` & `disdick-2.4.4/discord/types/emoji.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/types/gateway.py` & `disdick-2.4.4/discord/types/gateway.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/types/guild.py` & `disdick-2.4.4/discord/types/guild.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/types/integration.py` & `disdick-2.4.4/discord/types/integration.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/types/interactions.py` & `disdick-2.4.4/discord/types/interactions.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/types/invite.py` & `disdick-2.4.4/discord/types/invite.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/types/member.py` & `disdick-2.4.4/discord/types/member.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/types/message.py` & `disdick-2.4.4/discord/types/message.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/types/role.py` & `disdick-2.4.4/discord/types/role.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/types/scheduled_event.py` & `disdick-2.4.4/discord/types/scheduled_event.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/types/snowflake.py` & `disdick-2.4.4/discord/types/snowflake.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/types/sticker.py` & `disdick-2.4.4/discord/types/sticker.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/types/team.py` & `disdick-2.4.4/discord/types/team.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/types/template.py` & `disdick-2.4.4/discord/types/template.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/types/threads.py` & `disdick-2.4.4/discord/types/threads.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/types/user.py` & `disdick-2.4.4/discord/types/user.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/types/voice.py` & `disdick-2.4.4/discord/types/voice.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/types/webhook.py` & `disdick-2.4.4/discord/types/webhook.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/types/welcome_screen.py` & `disdick-2.4.4/discord/types/welcome_screen.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/types/widget.py` & `disdick-2.4.4/discord/types/widget.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/ui/button.py` & `disdick-2.4.4/discord/ui/button.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/ui/item.py` & `disdick-2.4.4/discord/ui/item.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/ui/modal.py` & `disdick-2.4.4/discord/ui/modal.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/ui/select.py` & `disdick-2.4.4/discord/ui/select.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/ui/text_input.py` & `disdick-2.4.4/discord/ui/text_input.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/ui/view.py` & `disdick-2.4.4/discord/ui/view.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/user.py` & `disdick-2.4.4/discord/user.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/utils.py` & `disdick-2.4.4/discord/utils.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/voice_client.py` & `disdick-2.4.4/discord/voice_client.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/webhook/async_.py` & `disdick-2.4.4/discord/webhook/async_.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/webhook/sync.py` & `disdick-2.4.4/discord/webhook/sync.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/welcome_screen.py` & `disdick-2.4.4/discord/welcome_screen.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/discord/widget.py` & `disdick-2.4.4/discord/widget.py`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/disdick.egg-info/PKG-INFO` & `disdick-2.4.4/disdick.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: disdick
-Version: 2.4.3
+Version: 2.4.4
 Summary: A Python wrapper for the Discord API
 Home-page: https://github.com/cop-discord/disdick
 Download-URL: https://github.com/cop-discord/disdick/archive/refs/tags/2.4.1.tar.gz
 Author: cop-discord
 License: MIT
 Project-URL: Documentation, https://discordpy.readthedocs.io/en/latest/
 Project-URL: Issue tracker, https://github.com/cop-discord/disdick/issues
```

### Comparing `disdick-2.4.3/disdick.egg-info/SOURCES.txt` & `disdick-2.4.4/disdick.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `disdick-2.4.3/setup.py` & `disdick-2.4.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 import re
 
-requirements = []
-with open('requirements.txt') as f:
-    requirements = f.read().splitlines()
+#requirements = []
+#with open('requirements.txt') as f:
+#    requirements = f.read().splitlines()
 
-version = '2.4.3'
+version = '2.4.4'
 if not version:
     raise RuntimeError('version is not set')
 
 if version.endswith(('a', 'b', 'rc')):
     # append version identifier based on commit count
     try:
         import subprocess
@@ -22,16 +22,18 @@
         out, err = p.communicate()
         if out:
             version += '+g' + out.decode('utf-8').strip()
     except Exception:
         pass
 
 readme = ''
-with open('README.rst') as f:
-    readme = f.read()
+try:
+    with open('README.rst') as f:
+        readme = f.read()
+except: pass
 
 extras_require = {
     'voice': ['PyNaCl>=1.3.0,<1.6'],
     'docs': [
         'sphinx==4.4.0',
         'sphinxcontrib_trio==1.1.2',
         'sphinxcontrib-websupport',
```

