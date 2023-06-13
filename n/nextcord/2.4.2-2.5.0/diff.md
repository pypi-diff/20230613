# Comparing `tmp/nextcord-2.4.2.tar.gz` & `tmp/nextcord-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nextcord-2.4.2.tar", last modified: Wed Apr  5 17:30:03 2023, max compression
+gzip compressed data, was "nextcord-2.5.0.tar", last modified: Tue Jun 13 16:15:31 2023, max compression
```

## Comparing `nextcord-2.4.2.tar` & `nextcord-2.5.0.tar`

### file list

```diff
@@ -1,256 +1,256 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:30:03.188474 nextcord-2.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-05 17:29:54.000000 nextcord-2.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-05 17:29:54.000000 nextcord-2.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-04-05 17:30:03.188474 nextcord-2.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-04-05 17:29:54.000000 nextcord-2.4.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:30:03.168474 nextcord-2.4.2/discord/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/abc.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/activity.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/appinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/application_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/audit_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/backoff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/colour.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/components.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/context_managers.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/cooldowns.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/embeds.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:30:03.160473 nextcord-2.4.2/discord/ext/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:30:03.168474 nextcord-2.4.2/discord/ext/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/ext/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/ext/commands/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/ext/commands/bot.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/ext/commands/cog.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/ext/commands/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/ext/commands/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/ext/commands/cooldowns.py
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/ext/commands/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/ext/commands/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/ext/commands/flags.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/ext/commands/help.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/ext/commands/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:30:03.168474 nextcord-2.4.2/discord/ext/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/ext/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/flags.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/guild.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/health_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/http.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/interactions.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/invite.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/iterators.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/member.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/mentions.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/message.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/object.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/oggparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/opus.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/partial_emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/player.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/raw_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/reaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/role.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/shard.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/stage_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/state.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/sticker.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/team.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/template.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/threads.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:30:03.172474 nextcord-2.4.2/discord/types/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/types/activity.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/types/appinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/types/audit_log.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/types/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/types/components.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/types/embed.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/types/emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/types/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/types/guild.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/types/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/types/interactions.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/types/invite.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/types/member.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/types/message.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/types/raw_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/types/role.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/types/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/types/sticker.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/types/team.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/types/template.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/types/threads.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/types/user.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/types/voice.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/types/webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/types/welcome_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/types/widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:30:03.172474 nextcord-2.4.2/discord/ui/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/ui/button.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/ui/item.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/ui/select.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/ui/view.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/voice_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:30:03.172474 nextcord-2.4.2/discord/webhook/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/webhook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/webhook/async_.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/webhook/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/welcome_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-05 17:29:54.000000 nextcord-2.4.2/discord/widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:30:03.180474 nextcord-2.4.2/nextcord/
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9306 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    61714 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/abc.py
--rw-r--r--   0 runner    (1001) docker     (123)    26362 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/activity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/appinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)   154389 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/application_command.py
--rw-r--r--   0 runner    (1001) docker     (123)    14093 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)    22950 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/audit_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)    20228 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/auto_moderation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/backoff.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/bans.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:30:03.180474 nextcord-2.4.2/nextcord/bin/
--rw-r--r--   0 runner    (1001) docker     (123)   441856 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/bin/libopus-0.x64.dll
--rw-r--r--   0 runner    (1001) docker     (123)   366080 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/bin/libopus-0.x86.dll
--rw-r--r--   0 runner    (1001) docker     (123)   102231 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)   104588 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/colour.py
--rw-r--r--   0 runner    (1001) docker     (123)    20689 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/context_managers.py
--rw-r--r--   0 runner    (1001) docker     (123)    20403 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/embeds.py
--rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)    21491 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     9331 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:30:03.160473 nextcord-2.4.2/nextcord/ext/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:30:03.180474 nextcord-2.4.2/nextcord/ext/application_checks/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/ext/application_checks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24410 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/ext/application_checks/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     8495 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/ext/application_checks/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:30:03.184474 nextcord-2.4.2/nextcord/ext/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/ext/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/ext/commands/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    63942 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/ext/commands/bot.py
--rw-r--r--   0 runner    (1001) docker     (123)    15956 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/ext/commands/cog.py
--rw-r--r--   0 runner    (1001) docker     (123)    13546 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/ext/commands/context.py
--rw-r--r--   0 runner    (1001) docker     (123)    41015 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/ext/commands/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11920 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/ext/commands/cooldowns.py
--rw-r--r--   0 runner    (1001) docker     (123)    81076 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/ext/commands/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    32454 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/ext/commands/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    20676 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/ext/commands/flags.py
--rw-r--r--   0 runner    (1001) docker     (123)    47649 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/ext/commands/help.py
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/ext/commands/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:30:03.184474 nextcord-2.4.2/nextcord/ext/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)    25499 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/ext/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/file.py
--rw-r--r--   0 runner    (1001) docker     (123)    39264 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/flags.py
--rw-r--r--   0 runner    (1001) docker     (123)    34263 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)   135571 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/guild.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/health_check.py
--rw-r--r--   0 runner    (1001) docker     (123)    88731 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/http.py
--rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)    48659 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/interactions.py
--rw-r--r--   0 runner    (1001) docker     (123)    17250 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/invite.py
--rw-r--r--   0 runner    (1001) docker     (123)    35411 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/iterators.py
--rw-r--r--   0 runner    (1001) docker     (123)    35466 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/member.py
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/mentions.py
--rw-r--r--   0 runner    (1001) docker     (123)    74484 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/oggparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    14456 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/opus.py
--rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/partial_emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)    25206 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    26236 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/player.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10499 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/raw_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/reaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    16175 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/role.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/role_connections.py
--rw-r--r--   0 runner    (1001) docker     (123)    14767 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/scheduled_events.py
--rw-r--r--   0 runner    (1001) docker     (123)    21853 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/shard.py
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/stage_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    99773 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/state.py
--rw-r--r--   0 runner    (1001) docker     (123)    14987 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/sticker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/team.py
--rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/template.py
--rw-r--r--   0 runner    (1001) docker     (123)    28558 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/threads.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:30:03.184474 nextcord-2.4.2/nextcord/types/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/types/activity.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/types/appinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/types/audit_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/types/auto_moderation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/types/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/types/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/types/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/types/embed.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/types/emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/types/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/types/guild.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/types/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/types/interactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/types/invite.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/types/member.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/types/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/types/raw_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/types/role.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/types/role_connections.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/types/scheduled_events.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/types/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/types/sticker.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/types/team.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/types/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/types/threads.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/types/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/types/voice.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/types/webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/types/welcome_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/types/widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:30:03.188474 nextcord-2.4.2/nextcord/ui/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9488 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/ui/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/ui/item.py
--rw-r--r--   0 runner    (1001) docker     (123)    13861 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/ui/modal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:30:03.188474 nextcord-2.4.2/nextcord/ui/select/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/ui/select/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7419 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/ui/select/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/ui/select/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/ui/select/mentionable.py
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/ui/select/role.py
--rw-r--r--   0 runner    (1001) docker     (123)     9350 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/ui/select/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/ui/select/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     7798 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/ui/text_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    18559 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/ui/view.py
--rw-r--r--   0 runner    (1001) docker     (123)    14658 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    36255 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    23782 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/voice_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:30:03.188474 nextcord-2.4.2/nextcord/webhook/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/webhook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57902 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/webhook/async_.py
--rw-r--r--   0 runner    (1001) docker     (123)    37369 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/webhook/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     8686 2023-04-05 17:29:54.000000 nextcord-2.4.2/nextcord/widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:30:03.180474 nextcord-2.4.2/nextcord.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-04-05 17:30:03.000000 nextcord-2.4.2/nextcord.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-04-05 17:30:03.000000 nextcord-2.4.2/nextcord.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 17:30:03.000000 nextcord-2.4.2/nextcord.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-05 17:30:03.000000 nextcord-2.4.2/nextcord.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-05 17:30:03.000000 nextcord-2.4.2/nextcord.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-05 17:29:54.000000 nextcord-2.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-05 17:29:54.000000 nextcord-2.4.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 17:30:03.188474 nextcord-2.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-04-05 17:29:54.000000 nextcord-2.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:15:31.642610 nextcord-2.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-13 16:15:19.000000 nextcord-2.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-13 16:15:19.000000 nextcord-2.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-06-13 16:15:31.642610 nextcord-2.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-06-13 16:15:19.000000 nextcord-2.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:15:31.610609 nextcord-2.5.0/discord/
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/appinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/application_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/audit_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/backoff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/colour.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/context_managers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/cooldowns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/embeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:15:31.598609 nextcord-2.5.0/discord/ext/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:15:31.614610 nextcord-2.5.0/discord/ext/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/ext/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/ext/commands/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/ext/commands/bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/ext/commands/cog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/ext/commands/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/ext/commands/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/ext/commands/cooldowns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/ext/commands/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/ext/commands/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/ext/commands/flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/ext/commands/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/ext/commands/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:15:31.614610 nextcord-2.5.0/discord/ext/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/ext/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/guild.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/health_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/interactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/invite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/iterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/member.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/mentions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/oggparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/opus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/partial_emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/player.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/raw_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/shard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/stage_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/sticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/team.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/threads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:15:31.618610 nextcord-2.5.0/discord/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/types/activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/types/appinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/types/audit_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/types/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/types/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/types/embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/types/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/types/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/types/guild.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/types/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/types/interactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/types/invite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/types/member.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/types/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/types/raw_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/types/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/types/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/types/sticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/types/team.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/types/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/types/threads.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/types/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/types/voice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/types/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/types/welcome_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/types/widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:15:31.618610 nextcord-2.5.0/discord/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/ui/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/ui/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/ui/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/ui/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/voice_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:15:31.618610 nextcord-2.5.0/discord/webhook/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/webhook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/webhook/async_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/webhook/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/welcome_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-13 16:15:19.000000 nextcord-2.5.0/discord/widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:15:31.630610 nextcord-2.5.0/nextcord/
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9306 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61714 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26362 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/appinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)   154833 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/application_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14093 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22538 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/audit_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20228 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/auto_moderation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/backoff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/bans.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:15:31.630610 nextcord-2.5.0/nextcord/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)   441856 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/bin/libopus-0.x64.dll
+-rw-r--r--   0 runner    (1001) docker     (123)   366080 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/bin/libopus-0.x86.dll
+-rw-r--r--   0 runner    (1001) docker     (123)   102469 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)   104588 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9044 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/colour.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20689 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/context_managers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20403 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/embeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21491 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9331 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:15:31.598609 nextcord-2.5.0/nextcord/ext/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:15:31.630610 nextcord-2.5.0/nextcord/ext/application_checks/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/ext/application_checks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24410 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/ext/application_checks/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8495 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/ext/application_checks/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:15:31.634610 nextcord-2.5.0/nextcord/ext/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/ext/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/ext/commands/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63942 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/ext/commands/bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15956 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/ext/commands/cog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13546 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/ext/commands/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41015 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/ext/commands/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11920 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/ext/commands/cooldowns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81054 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/ext/commands/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32454 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/ext/commands/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20676 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/ext/commands/flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47649 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/ext/commands/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/ext/commands/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:15:31.634610 nextcord-2.5.0/nextcord/ext/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)    25499 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/ext/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39264 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34263 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)   135572 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/guild.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/health_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88793 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48659 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/interactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17250 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/invite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35411 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/iterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35466 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/mentions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74484 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/oggparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14456 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/opus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/partial_emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25206 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26236 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/player.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10499 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/raw_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16175 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/role_connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14767 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/scheduled_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21853 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/shard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/stage_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99773 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14987 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/sticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28529 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/threads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:15:31.638610 nextcord-2.5.0/nextcord/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/types/activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/types/appinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/types/audit_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/types/auto_moderation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/types/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/types/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/types/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/types/embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/types/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/types/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/types/guild.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/types/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/types/interactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/types/invite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/types/member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/types/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/types/raw_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/types/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/types/role_connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/types/scheduled_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/types/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/types/sticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/types/team.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/types/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/types/threads.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/types/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/types/voice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/types/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/types/welcome_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/types/widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:15:31.638610 nextcord-2.5.0/nextcord/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9488 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/ui/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/ui/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13861 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/ui/modal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:15:31.642610 nextcord-2.5.0/nextcord/ui/select/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/ui/select/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7419 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/ui/select/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/ui/select/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/ui/select/mentionable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/ui/select/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9350 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/ui/select/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/ui/select/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7798 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/ui/text_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18559 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/ui/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14658 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36255 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23782 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/voice_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:15:31.642610 nextcord-2.5.0/nextcord/webhook/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/webhook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58116 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/webhook/async_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37583 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/webhook/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8686 2023-06-13 16:15:19.000000 nextcord-2.5.0/nextcord/widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:15:31.630610 nextcord-2.5.0/nextcord.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-06-13 16:15:31.000000 nextcord-2.5.0/nextcord.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-06-13 16:15:31.000000 nextcord-2.5.0/nextcord.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 16:15:31.000000 nextcord-2.5.0/nextcord.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-13 16:15:31.000000 nextcord-2.5.0/nextcord.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-13 16:15:31.000000 nextcord-2.5.0/nextcord.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-13 16:15:19.000000 nextcord-2.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-13 16:15:19.000000 nextcord-2.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 16:15:31.642610 nextcord-2.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-06-13 16:15:19.000000 nextcord-2.5.0/setup.py
```

### Comparing `nextcord-2.4.2/LICENSE` & `nextcord-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/PKG-INFO` & `nextcord-2.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextcord
-Version: 2.4.2
+Version: 2.5.0
 Summary: A Python wrapper for the Discord API forked from discord.py
 Home-page: https://github.com/nextcord/nextcord
 Author: Nextcord Developers & Rapptz
 License: MIT
 Project-URL: Documentation, https://docs.nextcord.dev/
 Project-URL: Issue tracker, https://github.com/nextcord/nextcord/issues
 Platform: UNKNOWN
@@ -134,17 +134,17 @@
 
     @bot.slash_command(description="Replies with pong!")
     async def ping(interaction: nextcord.Interaction):
         await interaction.send("Pong!", ephemeral=True)
 
     bot.run("token")
 
-You can find more examples in the `examples directory <https://github.com/nextcord/nextcord/blob/stable/examples/>`_.
+You can find more examples in the `examples directory <https://github.com/nextcord/nextcord/blob/master/examples/>`_.
 
-**NOTE:** It is not advised to leave your token directly in your code, as it allows anyone with it to access your bot. If you intend to make your code public you should `store it securely <https://github.com/nextcord/nextcord/blob/stable/examples/secure_token_storage.py/>`_.
+**NOTE:** It is not advised to leave your token directly in your code, as it allows anyone with it to access your bot. If you intend to make your code public you should `store it securely <https://github.com/nextcord/nextcord/blob/master/examples/secure_token_storage.py/>`_.
 
 Links
 ------
 
 - `Documentation <https://docs.nextcord.dev/>`_
 - `Official Discord Server <https://discord.gg/nextcord>`_
 - `Discord API <https://discord.gg/discord-api>`_
```

### Comparing `nextcord-2.4.2/README.rst` & `nextcord-2.5.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -101,17 +101,17 @@
 
     @bot.slash_command(description="Replies with pong!")
     async def ping(interaction: nextcord.Interaction):
         await interaction.send("Pong!", ephemeral=True)
 
     bot.run("token")
 
-You can find more examples in the `examples directory <https://github.com/nextcord/nextcord/blob/stable/examples/>`_.
+You can find more examples in the `examples directory <https://github.com/nextcord/nextcord/blob/master/examples/>`_.
 
-**NOTE:** It is not advised to leave your token directly in your code, as it allows anyone with it to access your bot. If you intend to make your code public you should `store it securely <https://github.com/nextcord/nextcord/blob/stable/examples/secure_token_storage.py/>`_.
+**NOTE:** It is not advised to leave your token directly in your code, as it allows anyone with it to access your bot. If you intend to make your code public you should `store it securely <https://github.com/nextcord/nextcord/blob/master/examples/secure_token_storage.py/>`_.
 
 Links
 ------
 
 - `Documentation <https://docs.nextcord.dev/>`_
 - `Official Discord Server <https://discord.gg/nextcord>`_
 - `Discord API <https://discord.gg/discord-api>`_
```

### Comparing `nextcord-2.4.2/discord/abc.py` & `nextcord-2.5.0/discord/abc.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/discord/activity.py` & `nextcord-2.5.0/discord/activity.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/discord/application_command.py` & `nextcord-2.5.0/discord/application_command.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/discord/audit_logs.py` & `nextcord-2.5.0/discord/audit_logs.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/discord/channel.py` & `nextcord-2.5.0/discord/channel.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/discord/client.py` & `nextcord-2.5.0/discord/client.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/discord/components.py` & `nextcord-2.5.0/discord/components.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/discord/enums.py` & `nextcord-2.5.0/discord/enums.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/discord/errors.py` & `nextcord-2.5.0/discord/errors.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/discord/ext/commands/__init__.py` & `nextcord-2.5.0/discord/ext/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/discord/ext/commands/bot.py` & `nextcord-2.5.0/discord/ext/commands/bot.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/discord/ext/commands/converter.py` & `nextcord-2.5.0/discord/ext/commands/converter.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/discord/ext/commands/cooldowns.py` & `nextcord-2.5.0/discord/ext/commands/cooldowns.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/discord/ext/commands/core.py` & `nextcord-2.5.0/discord/ext/commands/core.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/discord/ext/commands/errors.py` & `nextcord-2.5.0/discord/ext/commands/errors.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/discord/ext/commands/flags.py` & `nextcord-2.5.0/discord/ext/commands/flags.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/discord/ext/commands/help.py` & `nextcord-2.5.0/discord/ext/commands/help.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/discord/ext/tasks/__init__.py` & `nextcord-2.5.0/discord/ext/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/discord/flags.py` & `nextcord-2.5.0/discord/flags.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/discord/gateway.py` & `nextcord-2.5.0/discord/gateway.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/discord/guild.py` & `nextcord-2.5.0/discord/guild.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/discord/http.py` & `nextcord-2.5.0/discord/http.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/discord/integrations.py` & `nextcord-2.5.0/discord/integrations.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/discord/interactions.py` & `nextcord-2.5.0/discord/interactions.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/discord/invite.py` & `nextcord-2.5.0/discord/invite.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/discord/iterators.py` & `nextcord-2.5.0/discord/iterators.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/discord/member.py` & `nextcord-2.5.0/discord/member.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/discord/message.py` & `nextcord-2.5.0/discord/message.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/discord/opus.py` & `nextcord-2.5.0/discord/opus.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/discord/permissions.py` & `nextcord-2.5.0/discord/permissions.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/discord/player.py` & `nextcord-2.5.0/discord/player.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/discord/raw_models.py` & `nextcord-2.5.0/discord/raw_models.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/discord/shard.py` & `nextcord-2.5.0/discord/shard.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/discord/state.py` & `nextcord-2.5.0/discord/state.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/discord/sticker.py` & `nextcord-2.5.0/discord/sticker.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/discord/threads.py` & `nextcord-2.5.0/discord/threads.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/discord/types/activity.py` & `nextcord-2.5.0/discord/types/activity.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/discord/types/audit_log.py` & `nextcord-2.5.0/discord/types/audit_log.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/discord/types/channel.py` & `nextcord-2.5.0/discord/types/channel.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/discord/types/guild.py` & `nextcord-2.5.0/discord/types/guild.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/discord/types/integration.py` & `nextcord-2.5.0/discord/types/integration.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/discord/types/interactions.py` & `nextcord-2.5.0/discord/types/interactions.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/discord/types/invite.py` & `nextcord-2.5.0/discord/types/invite.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/discord/types/message.py` & `nextcord-2.5.0/discord/types/message.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/discord/types/raw_models.py` & `nextcord-2.5.0/discord/types/raw_models.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/discord/types/sticker.py` & `nextcord-2.5.0/discord/types/sticker.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/discord/ui/select.py` & `nextcord-2.5.0/discord/ui/select.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/discord/ui/view.py` & `nextcord-2.5.0/discord/ui/view.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/discord/utils.py` & `nextcord-2.5.0/discord/utils.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/discord/voice_client.py` & `nextcord-2.5.0/discord/voice_client.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/discord/webhook/async_.py` & `nextcord-2.5.0/discord/webhook/async_.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/discord/webhook/sync.py` & `nextcord-2.5.0/discord/webhook/sync.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/discord/widget.py` & `nextcord-2.5.0/discord/widget.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/__init__.py` & `nextcord-2.5.0/nextcord/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 :license: MIT, see LICENSE for more details.
 """
 
 __title__ = "nextcord"
 __author__ = "Nextcord Developers & Rapptz"
 __license__ = "MIT"
 __copyright__ = "Copyright 2015-2021 Rapptz & 2021-present Nextcord Developers"
-__version__ = "2.4.2"
+__version__ = "2.5.0"
 
 __path__ = __import__("pkgutil").extend_path(__path__, __name__)
 
 import logging
 from typing import Literal, NamedTuple
 
 from . import abc, opus, ui, utils
@@ -71,10 +71,10 @@
     major: int
     minor: int
     micro: int
     releaselevel: Literal["alpha", "beta", "candidate", "final"]
     serial: int
 
 
-version_info: VersionInfo = VersionInfo(major=2, minor=4, micro=0, releaselevel="final", serial=0)
+version_info: VersionInfo = VersionInfo(major=2, minor=5, micro=0, releaselevel="final", serial=0)
 
 logging.getLogger(__name__).addHandler(logging.NullHandler())
```

### Comparing `nextcord-2.4.2/nextcord/__main__.py` & `nextcord-2.5.0/nextcord/__main__.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/abc.py` & `nextcord-2.5.0/nextcord/abc.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/activity.py` & `nextcord-2.5.0/nextcord/activity.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/appinfo.py` & `nextcord-2.5.0/nextcord/appinfo.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/application_command.py` & `nextcord-2.5.0/nextcord/application_command.py`

 * *Files 0% similar despite different names*

```diff
@@ -752,14 +752,19 @@
                     # could be a self or interaction parameter
                     param.annotation is param.empty
                     # will always be an interaction parameter
                     or (
                         isinstance(param.annotation, type)
                         and issubclass(param.annotation, Interaction)
                     )
+                    # will always be an interaction parameter (generic with the outermost type being Interaction)
+                    or (
+                        (origin := typing_extensions.get_origin(param.annotation))
+                        and issubclass(origin, Interaction)
+                    )
                     # will always be a self parameter
                     # TODO: use typing.Self when 3.11 is standard
                     or param.annotation is typing_extensions.Self
                     # will always be a self parameter
                     or isinstance(param.annotation, TypeVar)
                     for param in list(callback_params.values())[:skip_counter]
                 )
@@ -3398,15 +3403,15 @@
                 role = Role(guild=interaction.guild, state=state, data=role_payload)
 
             ret.append(role)
 
     return ret
 
 
-def unpack_annotated(given_annotation: Any, resolve_list: list[type] = []) -> type:
+def unpack_annotated(given_annotation: Any, resolve_list: Optional[list[type]] = None) -> type:
     """Takes an annotation. If the origin is Annotated, it will attempt to resolve it using the given list of accepted
     types, going from the last type and working up to the first. If no matches to the given list is found, the last
     type specified in the Annotated typehint will be returned.
 
     If the origin is not Annotated, the typehint will be returned as-is.
 
     Parameters
@@ -3417,14 +3422,17 @@
         List of types the annotation can resolve to.
 
     Returns
     -------
     :class:`type`
         Resolved annotation.
     """
+    if resolve_list is None:
+        resolve_list = []
+
     # origin = typing.get_origin(given_annotation)  # TODO: Once Python 3.10 is standard, use this.
     origin = typing_extensions.get_origin(given_annotation)
     if origin is Annotated:
         located_annotation = MISSING
         # arg_list = typing.get_args(given_annotation)  # TODO: Once Python 3.10 is standard, use this
         arg_list = typing_extensions.get_args(given_annotation)
         for arg in reversed(arg_list[1:]):
@@ -3437,15 +3445,15 @@
 
         return located_annotation
     else:
         return given_annotation
 
 
 def unpack_annotation(
-    given_annotation: Any, annotated_list: List[type] = []
+    given_annotation: Any, annotated_list: Optional[List[type]] = None
 ) -> Tuple[List[type], list]:
     """Unpacks the given parameter annotation into its components.
 
     Parameters
     ----------
     given_annotation: Any
         Given annotation to unpack. Should be from ``parameter.annotation``
@@ -3455,14 +3463,17 @@
     Returns
     -------
     Tuple[List[:class:`type`], :class:`list`]
         A list of unpacked type annotations,
         and a list of unpacked literal arguments.
 
     """
+    if annotated_list is None:
+        annotated_list = []
+
     type_ret = []
     literal_ret = []
     # origin = typing.get_origin(given_annotation)  # TODO: Once Python 3.10 is standard, use this.
     origin = typing_extensions.get_origin(given_annotation)
     if origin is None:
         # It doesn't have a fancy origin, just a normal type/object.
         if isinstance(given_annotation, type):
```

### Comparing `nextcord-2.4.2/nextcord/asset.py` & `nextcord-2.5.0/nextcord/asset.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/audit_logs.py` & `nextcord-2.5.0/nextcord/audit_logs.py`

 * *Files 2% similar despite different names*

```diff
@@ -458,47 +458,43 @@
 
     def _from_data(self, data: AuditLogEntryPayload) -> None:
         self.action = enums.try_enum(enums.AuditLogAction, data["action_type"])
         self.id = int(data["id"])
 
         # this key is technically not usually present
         self.reason = data.get("reason")
-        self.extra = data.get("options")  # type: ignore
+        self.extra = data.get("options", {})  # type: ignore
         # I gave up trying to fix this
 
+        elems: Dict[str, Any] = {}
+        channel_id = int(self.extra["channel_id"]) if self.extra.get("channel_id", None) else None
+
         if isinstance(self.action, enums.AuditLogAction) and self.extra:
             if self.action is enums.AuditLogAction.member_prune:
                 # member prune has two keys with useful information
                 self.extra = type(  # type: ignore
                     "_AuditLogProxy", (), {k: int(v) for k, v in self.extra.items()}  # type: ignore
                 )()
             elif (
                 self.action is enums.AuditLogAction.member_move
                 or self.action is enums.AuditLogAction.message_delete
             ):
-                channel_id = int(self.extra["channel_id"])
                 elems = {
                     "count": int(self.extra["count"]),
-                    "channel": self.guild.get_channel(channel_id) or Object(id=channel_id),
                 }
-                self.extra = type("_AuditLogProxy", (), elems)()  # type: ignore
             elif self.action is enums.AuditLogAction.member_disconnect:
                 # The member disconnect action has a dict with some information
                 elems = {
                     "count": int(self.extra["count"]),
                 }
-                self.extra = type("_AuditLogProxy", (), elems)()  # type: ignore
             elif self.action.name.endswith("pin"):
                 # the pin actions have a dict with some information
-                channel_id = int(self.extra["channel_id"])
                 elems = {
-                    "channel": self.guild.get_channel(channel_id) or Object(id=channel_id),
                     "message_id": int(self.extra["message_id"]),
                 }
-                self.extra = type("_AuditLogProxy", (), elems)()  # type: ignore
             elif self.action.name.startswith("overwrite_"):
                 # the overwrite_ actions have a dict with some information
                 instance_id = int(self.extra["id"])
                 the_type = self.extra.get("type")
                 if the_type == "1":
                     self.extra = self._get_member(instance_id)
                 elif the_type == "0":
@@ -506,32 +502,33 @@
                     if role is None:
                         role = Object(id=instance_id)
                         role.name = self.extra.get("role_name")  # type: ignore
                     self.extra = role  # type: ignore
             elif self.action.name.startswith("stage_instance"):
                 channel_id = int(self.extra["channel_id"])
                 elems = {"channel": self.guild.get_channel(channel_id) or Object(id=channel_id)}
-                self.extra = type("_AuditLogProxy", (), elems)()  # type: ignore
             elif (
                 self.action is enums.AuditLogAction.auto_moderation_block_message
                 or self.action is enums.AuditLogAction.auto_moderation_flag_to_channel
                 or self.action is enums.AuditLogAction.auto_moderation_user_communication_disabled
             ):
-                channel_id = int(self.extra["channel_id"])
                 elems = {
-                    "channel": (
-                        self.guild.get_channel_or_thread(channel_id) or Object(id=channel_id)
-                    ),
                     "rule_name": self.extra["auto_moderation_rule_name"],
                     "rule_trigger_type": enums.try_enum(
                         enums.AutoModerationTriggerType,
                         int(self.extra["auto_moderation_rule_trigger_type"]),
                     ),
                 }
-                self.extra = type("_AuditLogProxy", (), elems)()  # type: ignore
+
+        # this just gets automatically filled in if present, this way prevents crashes if channel_id is None
+        if channel_id and self.action:
+            elems["channel"] = self.guild.get_channel_or_thread(channel_id) or Object(id=channel_id)
+
+        if type(self.extra) is dict:
+            self.extra = type("_AuditLogProxy", (), elems)()  # type: ignore
 
         # this key is not present when the above is present, typically.
         # It's a list of { new_value: a, old_value: b, key: c }
         # where new_value and old_value are not guaranteed to be there depending
         # on the action type, so let's just fetch it for now and only turn it
         # into meaningful data when requested
         self._changes = data.get("changes", [])
```

### Comparing `nextcord-2.4.2/nextcord/auto_moderation.py` & `nextcord-2.5.0/nextcord/auto_moderation.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/backoff.py` & `nextcord-2.5.0/nextcord/backoff.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/bin/libopus-0.x64.dll` & `nextcord-2.5.0/nextcord/bin/libopus-0.x64.dll`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/bin/libopus-0.x86.dll` & `nextcord-2.5.0/nextcord/bin/libopus-0.x86.dll`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/channel.py` & `nextcord-2.5.0/nextcord/channel.py`

 * *Files 1% similar despite different names*

```diff
@@ -712,14 +712,15 @@
     async def create_thread(
         self,
         *,
         name: str,
         message: Optional[Snowflake] = None,
         auto_archive_duration: ThreadArchiveDuration = MISSING,
         type: Optional[ChannelType] = None,
+        invitable: bool = True,
         reason: Optional[str] = None,
     ) -> Thread:
         """|coro|
 
         Creates a thread in this text channel.
 
         To create a public thread, you must have :attr:`~nextcord.Permissions.create_public_threads`.
@@ -738,14 +739,17 @@
         auto_archive_duration: :class:`int`
             The duration in minutes before a thread is automatically archived for inactivity.
             If not provided, the channel's default auto archive duration is used.
         type: Optional[:class:`ChannelType`]
             The type of thread to create. If a ``message`` is passed then this parameter
             is ignored, as a thread created with a message is always a public thread.
             By default this creates a private thread if this is ``None``.
+        invitable: :class:`bool`
+            Whether non-moderators can add other non-moderators to this thread.
+            Only available for private threads and threads created without a ``message``.
         reason: :class:`str`
             The reason for creating a new thread. Shows up on the audit log.
 
         Raises
         ------
         Forbidden
             You do not have permissions to create a thread.
@@ -763,14 +767,15 @@
 
         if message is None:
             data = await self._state.http.start_thread_without_message(
                 self.id,
                 name=name,
                 auto_archive_duration=auto_archive_duration or self.default_auto_archive_duration,
                 type=type.value,
+                invitable=invitable,
                 reason=reason,
             )
         else:
             data = await self._state.http.start_thread_with_message(
                 self.id,
                 message.id,
                 name=name,
@@ -952,15 +957,15 @@
         else:
             self.default_sort_order: Optional[SortOrderType] = None
 
         self.default_thread_slowmode_delay: Optional[int] = data.get(
             "default_thread_slowmode_delay"
         )
         self._available_tags: Dict[int, ForumTag] = {
-            int(data["id"]): ForumTag.from_data(tag) for tag in data.get("available_tags", [])
+            int(tag["id"]): ForumTag.from_data(tag) for tag in data.get("available_tags", [])
         }
 
         self.default_reaction: Optional[PartialEmoji]
 
         reaction = data.get("default_reaction_emoji")
         if reaction is None:
             self.default_reaction = None
@@ -3033,15 +3038,15 @@
 
         inner = " ".join("%s=%r" % t for t in attrs)
         return f"{type(self).__name__} {inner}"
 
     @property
     def payload(self) -> ForumTagPayload:
         data: ForumTagPayload = {
-            "id": str(self.id) if self.id is not None else None,
+            "id": str(self.id),
             "name": self.name,
             "moderated": self.moderated,
         }
 
         if self.emoji is not None:
             if self.emoji.id is not None:
                 data["emoji_id"] = str(self.emoji.id)
```

### Comparing `nextcord-2.4.2/nextcord/client.py` & `nextcord-2.5.0/nextcord/client.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/colour.py` & `nextcord-2.5.0/nextcord/colour.py`

 * *Files 2% similar despite different names*

```diff
@@ -273,20 +273,23 @@
     @classmethod
     def greyple(cls) -> Self:
         """A factory method that returns a :class:`Colour` with a value of ``0x99aab5``."""
         return cls(0x99AAB5)
 
     @classmethod
     def dark_theme(cls) -> Self:
-        """A factory method that returns a :class:`Colour` with a value of ``0x36393F``.
+        """A factory method that returns a :class:`Colour` with a value of ``0x313338``.
         This will appear transparent on Discord's dark theme.
 
         .. versionadded:: 1.5
+
+        .. versionchanged:: 2.5
+            Colour was replaced by the new dark theme colour on the UI.
         """
-        return cls(0x36393F)
+        return cls(0x313338)
 
     @classmethod
     def fuchsia(cls) -> Self:
         """A factory method that returns a :class:`Colour` with a value of ``0xEB459E``.
 
         .. versionadded:: 2.0
         """
```

### Comparing `nextcord-2.4.2/nextcord/components.py` & `nextcord-2.5.0/nextcord/components.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/context_managers.py` & `nextcord-2.5.0/nextcord/context_managers.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/embeds.py` & `nextcord-2.5.0/nextcord/embeds.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/emoji.py` & `nextcord-2.5.0/nextcord/emoji.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/enums.py` & `nextcord-2.5.0/nextcord/enums.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/errors.py` & `nextcord-2.5.0/nextcord/errors.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/ext/application_checks/core.py` & `nextcord-2.5.0/nextcord/ext/application_checks/core.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/ext/application_checks/errors.py` & `nextcord-2.5.0/nextcord/ext/application_checks/errors.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/ext/commands/_types.py` & `nextcord-2.5.0/nextcord/ext/commands/_types.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/ext/commands/bot.py` & `nextcord-2.5.0/nextcord/ext/commands/bot.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/ext/commands/cog.py` & `nextcord-2.5.0/nextcord/ext/commands/cog.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/ext/commands/context.py` & `nextcord-2.5.0/nextcord/ext/commands/context.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/ext/commands/converter.py` & `nextcord-2.5.0/nextcord/ext/commands/converter.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/ext/commands/cooldowns.py` & `nextcord-2.5.0/nextcord/ext/commands/cooldowns.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/ext/commands/core.py` & `nextcord-2.5.0/nextcord/ext/commands/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1338,15 +1338,15 @@
 
         return obj
 
     @overload
     def command(
         self,
         name: str = ...,
-        cls: Type[Command[CogT, P, T]] = Command[CogT, P, T],
+        cls: Type[Command[CogT, P, T]] = Command,
         *args: Any,
         **kwargs: Any,
     ) -> Callable[
         [
             Union[
                 Callable[Concatenate[CogT, ContextT, P], Coro[T]],
                 Callable[Concatenate[ContextT, P], Coro[T]],
@@ -1559,15 +1559,15 @@
 
 # Decorators
 
 
 @overload
 def command(
     name: str = ...,
-    cls: Type[Command[CogT, P, T]] = Command[CogT, P, T],
+    cls: Type[Command[CogT, P, T]] = Command,
     **attrs: Any,
 ) -> Callable[
     [
         Union[
             Callable[Concatenate[CogT, ContextT, P], Coro[T]],
             Callable[Concatenate[ContextT, P], Coro[T]],
         ]
@@ -1652,19 +1652,19 @@
 @overload
 def group(
     name: str = ...,
     **attrs: Any,
 ) -> Callable[
     [
         Union[
-            Callable[Concatenate[Cog, ContextT, P], Coro[T]],
+            Callable[Concatenate[CogT, ContextT, P], Coro[T]],
             Callable[Concatenate[ContextT, P], Coro[T]],
         ]
     ],
-    Group[Cog, P, T],
+    Group[CogT, P, T],
 ]:
     ...
 
 
 @overload
 def group(
     name: str = ...,
```

### Comparing `nextcord-2.4.2/nextcord/ext/commands/errors.py` & `nextcord-2.5.0/nextcord/ext/commands/errors.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/ext/commands/flags.py` & `nextcord-2.5.0/nextcord/ext/commands/flags.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/ext/commands/help.py` & `nextcord-2.5.0/nextcord/ext/commands/help.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/ext/commands/view.py` & `nextcord-2.5.0/nextcord/ext/commands/view.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/ext/tasks/__init__.py` & `nextcord-2.5.0/nextcord/ext/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/file.py` & `nextcord-2.5.0/nextcord/file.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,20 @@
 __all__ = ("File",)
 
 
 class File:
     r"""A parameter object used for :meth:`abc.Messageable.send`
     for sending file objects.
 
+    .. versionchanged:: 2.5
+
+        You can now use nextcord.File as a context manager. This will
+        automatically call :meth:`close` when the context manager exits scope.
+        When using the context manager, force_close will default to True.
+
     .. note::
 
         File objects are single use and are not meant to be reused in
         multiple :meth:`abc.Messageable.send`\s.
 
     Parameters
     ----------
@@ -43,14 +49,15 @@
         Whether the attachment is a spoiler.
     force_close: :class:`bool`
         Whether to forcibly close the bytes used to create the file
         when ``.close()`` is called.
         This will also make the file bytes unusable by flushing it from
         memory after it is sent once.
         Enable this if you don't wish to reuse the same bytes.
+        Defaults to ``True`` when using context manager.
 
         .. versionadded:: 2.2
 
     Attributes
     ----------
     fp: Union[:class:`io.BufferedReader`, :class:`io.BufferedIOBase`]
         A file-like object opened in binary mode and read mode.
@@ -86,24 +93,24 @@
     )
 
     if TYPE_CHECKING:
         fp: Union[io.BufferedReader, io.BufferedIOBase]
         filename: Optional[str]
         description: Optional[str]
         spoiler: bool
-        force_close: bool
+        force_close: Optional[bool]
 
     def __init__(
         self,
         fp: Union[str, bytes, os.PathLike, io.BufferedIOBase],
         filename: Optional[str] = None,
         *,
         description: Optional[str] = None,
         spoiler: bool = False,
-        force_close: bool = False,
+        force_close: Optional[bool] = None,
     ) -> None:
         if isinstance(fp, io.IOBase):
             if not (fp.seekable() and fp.readable()):
                 raise ValueError(f"File buffer {fp!r} must be seekable and readable")
             self.fp = fp
             self._original_pos = fp.tell()
             self._owner = False
@@ -134,14 +141,24 @@
         if spoiler and self.filename is not None and not self.filename.startswith("SPOILER_"):
             self.filename = "SPOILER_" + self.filename
 
         self.spoiler = spoiler or (
             self.filename is not None and self.filename.startswith("SPOILER_")
         )
 
+    def __enter__(self) -> File:
+        # Set force_close to true when using context manager
+        # and force_close was not provided to __init__
+        if self.force_close is None:
+            self.force_close = True
+        return self
+
+    def __exit__(self, *_) -> None:
+        self.close()
+
     def reset(self, *, seek: Union[int, bool] = True) -> None:
         # The `seek` parameter is needed because
         # the retry-loop is iterated over multiple times
         # starting from 0, as an implementation quirk
         # the resetting must be done at the beginning
         # before a request is done, since the first index
         # is 0, and thus false, then this prevents an
```

### Comparing `nextcord-2.4.2/nextcord/flags.py` & `nextcord-2.5.0/nextcord/flags.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/gateway.py` & `nextcord-2.5.0/nextcord/gateway.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/guild.py` & `nextcord-2.5.0/nextcord/guild.py`

 * *Files 0% similar despite different names*

```diff
@@ -3733,15 +3733,15 @@
             The name to use for this rule.
         event_type: :class:`AutoModerationEventType`
             The type of event conteto listen to for this rule.
         actions: List[:class:`AutoModerationAction`]
             The actions to execute when this rule is triggered.
         trigger_type: :class:`AutoModerationTriggerType`
             The type of content that triggers this rule.
-        trigger_metadata: Optinal[:class:`AutoModerationTriggerMetadata`]
+        trigger_metadata: Optional[:class:`AutoModerationTriggerMetadata`]
             The additional data to use to determine if this rule has been triggered.
         enabled: Optional[:class:`bool`]
             If this rule should be enabled.
         exempt_roles: Optional[List[:class:`abc.Snowflake`]]
             Roles that should be exempt from this rule.
         exempt_channels: Optional[List[:class:`abc.Snowflake`]]
             Channels that should be exempt from this rule.
```

### Comparing `nextcord-2.4.2/nextcord/health_check.py` & `nextcord-2.5.0/nextcord/health_check.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/http.py` & `nextcord-2.5.0/nextcord/http.py`

 * *Files 0% similar despite different names*

```diff
@@ -2280,20 +2280,23 @@
         )
         return self.request(r)
 
     def create_followup_message(
         self,
         application_id: Snowflake,
         token: str,
-        files: List[File] = [],
+        files: Optional[List[File]] = None,
         content: Optional[str] = None,
         tts: bool = False,
         embeds: Optional[List[embed.Embed]] = None,
         allowed_mentions: Optional[message.AllowedMentions] = None,
     ) -> Response[message.Message]:
+        if files is None:
+            files = []
+
         r = Route(
             "POST",
             "/webhooks/{application_id}/{interaction_token}",
             application_id=application_id,
             interaction_token=token,
         )
         return self.send_multipart_helper(
```

### Comparing `nextcord-2.4.2/nextcord/integrations.py` & `nextcord-2.5.0/nextcord/integrations.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/interactions.py` & `nextcord-2.5.0/nextcord/interactions.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/invite.py` & `nextcord-2.5.0/nextcord/invite.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/iterators.py` & `nextcord-2.5.0/nextcord/iterators.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/member.py` & `nextcord-2.5.0/nextcord/member.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/mentions.py` & `nextcord-2.5.0/nextcord/mentions.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/message.py` & `nextcord-2.5.0/nextcord/message.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/mixins.py` & `nextcord-2.5.0/nextcord/mixins.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/object.py` & `nextcord-2.5.0/nextcord/object.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/oggparse.py` & `nextcord-2.5.0/nextcord/oggparse.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/opus.py` & `nextcord-2.5.0/nextcord/opus.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/partial_emoji.py` & `nextcord-2.5.0/nextcord/partial_emoji.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/permissions.py` & `nextcord-2.5.0/nextcord/permissions.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/player.py` & `nextcord-2.5.0/nextcord/player.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/raw_models.py` & `nextcord-2.5.0/nextcord/raw_models.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/reaction.py` & `nextcord-2.5.0/nextcord/reaction.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/role.py` & `nextcord-2.5.0/nextcord/role.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/role_connections.py` & `nextcord-2.5.0/nextcord/role_connections.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/scheduled_events.py` & `nextcord-2.5.0/nextcord/scheduled_events.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/shard.py` & `nextcord-2.5.0/nextcord/shard.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/stage_instance.py` & `nextcord-2.5.0/nextcord/stage_instance.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/state.py` & `nextcord-2.5.0/nextcord/state.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/sticker.py` & `nextcord-2.5.0/nextcord/sticker.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/team.py` & `nextcord-2.5.0/nextcord/team.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/template.py` & `nextcord-2.5.0/nextcord/template.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/threads.py` & `nextcord-2.5.0/nextcord/threads.py`

 * *Files 0% similar despite different names*

```diff
@@ -173,17 +173,15 @@
         try:
             member = data["member"]
         except KeyError:
             self.me = None
         else:
             self.me = ThreadMember(self, member)
 
-        self.applied_tag_ids: List[int] = [
-            int(tag_id) for tag_id in data.get("applied_thread_tags", [])
-        ]
+        self.applied_tag_ids: List[int] = [int(tag_id) for tag_id in data.get("applied_tags", [])]
 
     def _unroll_metadata(self, data: ThreadMetadata) -> None:
         self.archived = data["archived"]
         self.archiver_id = get_as_snowflake(data, "archiver_id")
         self.auto_archive_duration = data["auto_archive_duration"]
         self.archive_timestamp = parse_time(data["archive_timestamp"])
         self.locked = data.get("locked", False)
```

### Comparing `nextcord-2.4.2/nextcord/types/activity.py` & `nextcord-2.5.0/nextcord/types/activity.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/types/appinfo.py` & `nextcord-2.5.0/nextcord/types/appinfo.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/types/audit_log.py` & `nextcord-2.5.0/nextcord/types/audit_log.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/types/auto_moderation.py` & `nextcord-2.5.0/nextcord/types/auto_moderation.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/types/channel.py` & `nextcord-2.5.0/nextcord/types/channel.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,12 +147,12 @@
     channel_id: Snowflake
     topic: str
     privacy_level: PrivacyLevel
     discoverable_disabled: bool
 
 
 class ForumTag(TypedDict):
-    id: Optional[Snowflake]
+    id: Snowflake
     name: str
     moderated: bool
     emoji_id: NotRequired[Optional[Snowflake]]
     emoji_name: NotRequired[Optional[str]]
```

### Comparing `nextcord-2.4.2/nextcord/types/checks.py` & `nextcord-2.5.0/nextcord/types/checks.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/types/components.py` & `nextcord-2.5.0/nextcord/types/components.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/types/embed.py` & `nextcord-2.5.0/nextcord/types/embed.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/types/emoji.py` & `nextcord-2.5.0/nextcord/types/emoji.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/types/guild.py` & `nextcord-2.5.0/nextcord/types/guild.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/types/integration.py` & `nextcord-2.5.0/nextcord/types/integration.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/types/interactions.py` & `nextcord-2.5.0/nextcord/types/interactions.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/types/invite.py` & `nextcord-2.5.0/nextcord/types/invite.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/types/member.py` & `nextcord-2.5.0/nextcord/types/member.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/types/message.py` & `nextcord-2.5.0/nextcord/types/message.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/types/raw_models.py` & `nextcord-2.5.0/nextcord/types/raw_models.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/types/role.py` & `nextcord-2.5.0/nextcord/types/role.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/types/scheduled_events.py` & `nextcord-2.5.0/nextcord/types/scheduled_events.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/types/sticker.py` & `nextcord-2.5.0/nextcord/types/sticker.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/types/template.py` & `nextcord-2.5.0/nextcord/types/template.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/types/threads.py` & `nextcord-2.5.0/nextcord/types/threads.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/types/voice.py` & `nextcord-2.5.0/nextcord/types/voice.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/types/webhook.py` & `nextcord-2.5.0/nextcord/types/webhook.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/types/widget.py` & `nextcord-2.5.0/nextcord/types/widget.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/ui/button.py` & `nextcord-2.5.0/nextcord/ui/button.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/ui/item.py` & `nextcord-2.5.0/nextcord/ui/item.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/ui/modal.py` & `nextcord-2.5.0/nextcord/ui/modal.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/ui/select/base.py` & `nextcord-2.5.0/nextcord/ui/select/base.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/ui/select/channel.py` & `nextcord-2.5.0/nextcord/ui/select/channel.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/ui/select/mentionable.py` & `nextcord-2.5.0/nextcord/ui/select/mentionable.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/ui/select/role.py` & `nextcord-2.5.0/nextcord/ui/select/role.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/ui/select/string.py` & `nextcord-2.5.0/nextcord/ui/select/string.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/ui/select/user.py` & `nextcord-2.5.0/nextcord/ui/select/user.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/ui/text_input.py` & `nextcord-2.5.0/nextcord/ui/text_input.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/ui/view.py` & `nextcord-2.5.0/nextcord/ui/view.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/user.py` & `nextcord-2.5.0/nextcord/user.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/utils.py` & `nextcord-2.5.0/nextcord/utils.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/voice_client.py` & `nextcord-2.5.0/nextcord/voice_client.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord/webhook/async_.py` & `nextcord-2.5.0/nextcord/webhook/async_.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     Optional,
     Tuple,
     Type,
     Union,
     overload,
 )
 from urllib.parse import quote as urlquote
+from weakref import WeakValueDictionary
 
 import aiohttp
 
 from .. import utils
 from ..asset import Asset
 from ..channel import PartialMessageable
 from ..enums import WebhookType, try_enum
@@ -53,14 +54,15 @@
     from ..embeds import Embed
     from ..file import File
     from ..guild import Guild
     from ..http import Response
     from ..mentions import AllowedMentions
     from ..state import ConnectionState
     from ..types.message import Message as MessagePayload
+    from ..types.snowflake import Snowflake as SnowflakeAlias
     from ..types.webhook import Webhook as WebhookPayload
     from ..ui.view import View
 
 MISSING = utils.MISSING
 
 
 class AsyncDeferredLock:
@@ -84,15 +86,18 @@
         if self.delta:
             await asyncio.sleep(self.delta)
         self.lock.release()
 
 
 class AsyncWebhookAdapter:
     def __init__(self) -> None:
-        self._locks: Dict[Any, asyncio.Lock] = {}
+        self._locks: WeakValueDictionary[
+            Tuple[Optional[SnowflakeAlias], Optional[str]],
+            asyncio.Lock,
+        ] = WeakValueDictionary()
 
     async def request(
         self,
         route: Route,
         session: aiohttp.ClientSession,
         *,
         payload: Optional[Dict[str, Any]] = None,
```

### Comparing `nextcord-2.4.2/nextcord/webhook/sync.py` & `nextcord-2.5.0/nextcord/webhook/sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import logging
 import re
 import threading
 import time
 from types import TracebackType
 from typing import TYPE_CHECKING, Any, Dict, List, Literal, Optional, Tuple, Type, Union, overload
 from urllib.parse import quote as urlquote
+from weakref import WeakValueDictionary
 
 from .. import utils
 from ..channel import PartialMessageable
 from ..errors import DiscordServerError, Forbidden, HTTPException, InvalidArgument, NotFound
 from ..http import Route
 from ..message import Attachment, Message
 from .async_ import BaseWebhook, _WebhookState, handle_message_parameters
@@ -32,14 +33,15 @@
 _log = logging.getLogger(__name__)
 
 if TYPE_CHECKING:
     from ..abc import Snowflake
     from ..embeds import Embed
     from ..file import File
     from ..mentions import AllowedMentions
+    from ..types.snowflake import Snowflake as SnowflakeAlias
     from ..types.webhook import Webhook as WebhookPayload
 
     try:
         from requests import Response, Session
     except ModuleNotFoundError:
         pass
 
@@ -67,15 +69,18 @@
         if self.delta:
             time.sleep(self.delta)
         self.lock.release()
 
 
 class WebhookAdapter:
     def __init__(self) -> None:
-        self._locks: Dict[Any, threading.Lock] = {}
+        self._locks: WeakValueDictionary[
+            Tuple[Optional[SnowflakeAlias], Optional[str]],
+            threading.Lock,
+        ] = WeakValueDictionary()
 
     def request(
         self,
         route: Route,
         session: Session,
         *,
         payload: Optional[Dict[str, Any]] = None,
```

### Comparing `nextcord-2.4.2/nextcord/widget.py` & `nextcord-2.5.0/nextcord/widget.py`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/nextcord.egg-info/PKG-INFO` & `nextcord-2.5.0/nextcord.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextcord
-Version: 2.4.2
+Version: 2.5.0
 Summary: A Python wrapper for the Discord API forked from discord.py
 Home-page: https://github.com/nextcord/nextcord
 Author: Nextcord Developers & Rapptz
 License: MIT
 Project-URL: Documentation, https://docs.nextcord.dev/
 Project-URL: Issue tracker, https://github.com/nextcord/nextcord/issues
 Platform: UNKNOWN
@@ -134,17 +134,17 @@
 
     @bot.slash_command(description="Replies with pong!")
     async def ping(interaction: nextcord.Interaction):
         await interaction.send("Pong!", ephemeral=True)
 
     bot.run("token")
 
-You can find more examples in the `examples directory <https://github.com/nextcord/nextcord/blob/stable/examples/>`_.
+You can find more examples in the `examples directory <https://github.com/nextcord/nextcord/blob/master/examples/>`_.
 
-**NOTE:** It is not advised to leave your token directly in your code, as it allows anyone with it to access your bot. If you intend to make your code public you should `store it securely <https://github.com/nextcord/nextcord/blob/stable/examples/secure_token_storage.py/>`_.
+**NOTE:** It is not advised to leave your token directly in your code, as it allows anyone with it to access your bot. If you intend to make your code public you should `store it securely <https://github.com/nextcord/nextcord/blob/master/examples/secure_token_storage.py/>`_.
 
 Links
 ------
 
 - `Documentation <https://docs.nextcord.dev/>`_
 - `Official Discord Server <https://discord.gg/nextcord>`_
 - `Discord API <https://discord.gg/discord-api>`_
```

### Comparing `nextcord-2.4.2/nextcord.egg-info/SOURCES.txt` & `nextcord-2.5.0/nextcord.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/pyproject.toml` & `nextcord-2.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nextcord-2.4.2/setup.py` & `nextcord-2.5.0/setup.py`

 * *Files identical despite different names*

