# Comparing `tmp/interactions.py-5.4.0.tar.gz` & `tmp/interactions.py-5.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interactions.py-5.4.0.tar", last modified: Wed May 17 19:05:05 2023, max compression
+gzip compressed data, was "interactions.py-5.5.0.tar", last modified: Sun May 21 18:25:05 2023, max compression
```

## Comparing `interactions.py-5.4.0.tar` & `interactions.py-5.5.0.tar`

### file list

```diff
@@ -1,192 +1,192 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:05:05.838810 interactions.py-5.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-17 19:04:21.000000 interactions.py-5.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-17 19:04:21.000000 interactions.py-5.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-05-17 19:05:05.838810 interactions.py-5.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-17 19:04:21.000000 interactions.py-5.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:05:05.786810 interactions.py-5.4.0/interactions/
--rw-r--r--   0 runner    (1001) docker     (123)    15113 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:05:05.790810 interactions.py-5.4.0/interactions/api/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:05:05.790810 interactions.py-5.4.0/interactions/api/events/
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/api/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/api/events/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    23833 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/api/events/discord.py
--rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/api/events/internal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:05:05.790810 interactions.py-5.4.0/interactions/api/events/processors/
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/api/events/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/api/events/processors/_template.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/api/events/processors/_template.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/api/events/processors/auto_mod.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/api/events/processors/channel_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/api/events/processors/guild_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/api/events/processors/integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/api/events/processors/member_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/api/events/processors/message_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/api/events/processors/reaction_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/api/events/processors/role_events.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/api/events/processors/stage_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/api/events/processors/thread_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/api/events/processors/user_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/api/events/processors/voice_events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:05:05.794810 interactions.py-5.4.0/interactions/api/gateway/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/api/gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13569 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/api/gateway/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/api/gateway/state.py
--rw-r--r--   0 runner    (1001) docker     (123)    11590 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/api/gateway/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:05:05.794810 interactions.py-5.4.0/interactions/api/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/api/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22204 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/api/http/http_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:05:05.798810 interactions.py-5.4.0/interactions/api/http/http_requests/
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/api/http/http_requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/api/http/http_requests/bot.py
--rw-r--r--   0 runner    (1001) docker     (123)    22816 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/api/http/http_requests/channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/api/http/http_requests/emojis.py
--rw-r--r--   0 runner    (1001) docker     (123)    35368 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/api/http/http_requests/guild.py
--rw-r--r--   0 runner    (1001) docker     (123)    12056 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/api/http/http_requests/interactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/api/http/http_requests/members.py
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/api/http/http_requests/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/api/http/http_requests/reactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/api/http/http_requests/scheduled_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/api/http/http_requests/stickers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9054 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/api/http/http_requests/threads.py
--rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/api/http/http_requests/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/api/http/http_requests/webhooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/api/http/route.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:05:05.798810 interactions.py-5.4.0/interactions/api/voice/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/api/voice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11922 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/api/voice/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     9016 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/api/voice/audio_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/api/voice/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)    11470 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/api/voice/opus.py
--rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/api/voice/player.py
--rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/api/voice/recorder.py
--rw-r--r--   0 runner    (1001) docker     (123)    15215 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/api/voice/voice_gateway.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:05:05.802810 interactions.py-5.4.0/interactions/bin/
--rw-r--r--   0 runner    (1001) docker     (123)   441856 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/bin/opus-x64.dll
--rw-r--r--   0 runner    (1001) docker     (123)   366080 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/bin/opus-x86.dll
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:05:05.802810 interactions.py-5.4.0/interactions/client/
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9537 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/client/auto_shard_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    91574 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8051 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/client/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    13209 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/client/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:05:05.806810 interactions.py-5.4.0/interactions/client/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/client/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/client/mixins/modal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/client/mixins/send.py
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/client/mixins/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)    31386 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/client/smart_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:05:05.810810 interactions.py-5.4.0/interactions/client/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/client/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/client/utils/attr_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/client/utils/attr_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/client/utils/attr_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/client/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/client/utils/deserialise_app_cmds.py
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/client/utils/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/client/utils/input_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/client/utils/misc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/client/utils/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/client/utils/text_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:05:05.810810 interactions.py-5.4.0/interactions/ext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/ext/console.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:05:05.810810 interactions.py-5.4.0/interactions/ext/debug_extension/
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/ext/debug_extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7919 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/ext/debug_extension/debug_application_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/ext/debug_extension/debug_exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/ext/debug_extension/debug_exts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6065 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/ext/debug_extension/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8179 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/ext/jurigged.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:05:05.810810 interactions.py-5.4.0/interactions/ext/mypy/
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/ext/mypy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15840 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/ext/paginators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:05:05.814810 interactions.py-5.4.0/interactions/ext/prefixed_commands/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/ext/prefixed_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27889 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/ext/prefixed_commands/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/ext/prefixed_commands/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/ext/prefixed_commands/help.py
--rw-r--r--   0 runner    (1001) docker     (123)    14126 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/ext/prefixed_commands/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/ext/prefixed_commands/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/ext/sentry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:05:05.814810 interactions.py-5.4.0/interactions/models/
--rw-r--r--   0 runner    (1001) docker     (123)    12369 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:05:05.826810 interactions.py-5.4.0/interactions/models/discord/
--rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/models/discord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/models/discord/activity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/models/discord/app_perms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/models/discord/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/models/discord/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)    13612 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/models/discord/auto_mod.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/models/discord/base.py
--rw-r--r--   0 runner    (1001) docker     (123)   103108 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/models/discord/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/models/discord/color.py
--rw-r--r--   0 runner    (1001) docker     (123)    24769 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/models/discord/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    16286 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/models/discord/embed.py
--rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/models/discord/emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)    30758 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/models/discord/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/models/discord/file.py
--rw-r--r--   0 runner    (1001) docker     (123)    95600 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/models/discord/guild.py
--rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/models/discord/invite.py
--rw-r--r--   0 runner    (1001) docker     (123)    38395 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/models/discord/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/models/discord/modal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/models/discord/reaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     8191 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/models/discord/role.py
--rw-r--r--   0 runner    (1001) docker     (123)     9485 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/models/discord/scheduled_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/models/discord/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/models/discord/stage_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/models/discord/sticker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/models/discord/team.py
--rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/models/discord/thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/models/discord/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)    25942 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/models/discord/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/models/discord/user.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/models/discord/voice_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    12406 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/models/discord/webhooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:05:05.834810 interactions.py-5.4.0/interactions/models/internal/
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/models/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11266 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/models/internal/active_voice_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:05:05.834810 interactions.py-5.4.0/interactions/models/internal/annotations/
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/models/internal/annotations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7405 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/models/internal/annotations/slash.py
--rw-r--r--   0 runner    (1001) docker     (123)    55763 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/models/internal/application_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/models/internal/auto_defer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/models/internal/callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/models/internal/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)    12390 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/models/internal/command.py
--rw-r--r--   0 runner    (1001) docker     (123)    35118 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/models/internal/context.py
--rw-r--r--   0 runner    (1001) docker     (123)    19351 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/models/internal/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)    17655 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/models/internal/cooldowns.py
--rw-r--r--   0 runner    (1001) docker     (123)    10168 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/models/internal/extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/models/internal/listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/models/internal/localisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/models/internal/protocols.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:05:05.834810 interactions.py-5.4.0/interactions/models/internal/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/models/internal/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/models/internal/tasks/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/models/internal/tasks/triggers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/models/internal/wait.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:05:05.834810 interactions.py-5.4.0/interactions/models/misc/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/models/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/models/misc/context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/models/misc/iterator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 19:04:21.000000 interactions.py-5.4.0/interactions/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:05:05.786810 interactions.py-5.4.0/interactions.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-05-17 19:05:05.000000 interactions.py-5.4.0/interactions.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-05-17 19:05:05.000000 interactions.py-5.4.0/interactions.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 19:05:05.000000 interactions.py-5.4.0/interactions.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-17 19:05:05.000000 interactions.py-5.4.0/interactions.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-17 19:05:05.000000 interactions.py-5.4.0/interactions.py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-05-17 19:04:21.000000 interactions.py-5.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-17 19:04:21.000000 interactions.py-5.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-17 19:05:05.838810 interactions.py-5.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-17 19:04:57.000000 interactions.py-5.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:05:05.838810 interactions.py-5.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 19:04:21.000000 interactions.py-5.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-05-17 19:04:21.000000 interactions.py-5.4.0/tests/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    16999 2023-05-17 19:04:21.000000 interactions.py-5.4.0/tests/test_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-17 19:04:21.000000 interactions.py-5.4.0/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-17 19:04:21.000000 interactions.py-5.4.0/tests/test_contexts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-17 19:04:21.000000 interactions.py-5.4.0/tests/test_cooldowns.py
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-05-17 19:04:21.000000 interactions.py-5.4.0/tests/test_emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-17 19:04:21.000000 interactions.py-5.4.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:25:05.190549 interactions.py-5.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-21 18:24:28.000000 interactions.py-5.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-21 18:24:28.000000 interactions.py-5.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-05-21 18:25:05.190549 interactions.py-5.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-21 18:24:28.000000 interactions.py-5.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:25:05.158549 interactions.py-5.5.0/interactions/
+-rw-r--r--   0 runner    (1001) docker     (123)    15113 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:25:05.158549 interactions.py-5.5.0/interactions/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:25:05.162549 interactions.py-5.5.0/interactions/api/events/
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/api/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/api/events/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23833 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/api/events/discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/api/events/internal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:25:05.166549 interactions.py-5.5.0/interactions/api/events/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/api/events/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/api/events/processors/_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/api/events/processors/_template.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/api/events/processors/auto_mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/api/events/processors/channel_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/api/events/processors/guild_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/api/events/processors/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/api/events/processors/member_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/api/events/processors/message_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/api/events/processors/reaction_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/api/events/processors/role_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/api/events/processors/stage_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/api/events/processors/thread_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/api/events/processors/user_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/api/events/processors/voice_events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:25:05.166549 interactions.py-5.5.0/interactions/api/gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/api/gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13569 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/api/gateway/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/api/gateway/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11590 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/api/gateway/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:25:05.170549 interactions.py-5.5.0/interactions/api/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/api/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22204 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/api/http/http_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:25:05.174549 interactions.py-5.5.0/interactions/api/http/http_requests/
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/api/http/http_requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/api/http/http_requests/bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22816 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/api/http/http_requests/channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/api/http/http_requests/emojis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35368 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/api/http/http_requests/guild.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12056 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/api/http/http_requests/interactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/api/http/http_requests/members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/api/http/http_requests/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/api/http/http_requests/reactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/api/http/http_requests/scheduled_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/api/http/http_requests/stickers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9054 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/api/http/http_requests/threads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/api/http/http_requests/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/api/http/http_requests/webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/api/http/route.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:25:05.178549 interactions.py-5.5.0/interactions/api/voice/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/api/voice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11922 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/api/voice/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9016 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/api/voice/audio_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/api/voice/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11470 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/api/voice/opus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/api/voice/player.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/api/voice/recorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15215 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/api/voice/voice_gateway.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:25:05.178549 interactions.py-5.5.0/interactions/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)   441856 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/bin/opus-x64.dll
+-rw-r--r--   0 runner    (1001) docker     (123)   366080 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/bin/opus-x86.dll
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:25:05.178549 interactions.py-5.5.0/interactions/client/
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9537 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/client/auto_shard_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92216 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/client/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13209 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/client/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:25:05.178549 interactions.py-5.5.0/interactions/client/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/client/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/client/mixins/modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/client/mixins/send.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/client/mixins/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31386 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/client/smart_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:25:05.182549 interactions.py-5.5.0/interactions/client/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/client/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/client/utils/attr_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/client/utils/attr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/client/utils/attr_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/client/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/client/utils/deserialise_app_cmds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/client/utils/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/client/utils/input_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/client/utils/misc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/client/utils/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/client/utils/text_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:25:05.182549 interactions.py-5.5.0/interactions/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/ext/console.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:25:05.182549 interactions.py-5.5.0/interactions/ext/debug_extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/ext/debug_extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7919 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/ext/debug_extension/debug_application_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/ext/debug_extension/debug_exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/ext/debug_extension/debug_exts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6065 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/ext/debug_extension/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8179 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/ext/jurigged.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:25:05.182549 interactions.py-5.5.0/interactions/ext/mypy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/ext/mypy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15840 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/ext/paginators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:25:05.182549 interactions.py-5.5.0/interactions/ext/prefixed_commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/ext/prefixed_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27889 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/ext/prefixed_commands/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/ext/prefixed_commands/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/ext/prefixed_commands/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14126 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/ext/prefixed_commands/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/ext/prefixed_commands/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/ext/sentry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:25:05.182549 interactions.py-5.5.0/interactions/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    12369 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:25:05.186549 interactions.py-5.5.0/interactions/models/discord/
+-rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/models/discord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/models/discord/activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/models/discord/app_perms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/models/discord/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/models/discord/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13612 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/models/discord/auto_mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/models/discord/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)   103108 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/models/discord/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/models/discord/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24769 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/models/discord/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16286 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/models/discord/embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/models/discord/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30758 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/models/discord/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/models/discord/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95600 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/models/discord/guild.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/models/discord/invite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38395 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/models/discord/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/models/discord/modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/models/discord/reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8191 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/models/discord/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9485 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/models/discord/scheduled_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/models/discord/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/models/discord/stage_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/models/discord/sticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/models/discord/team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/models/discord/thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/models/discord/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25942 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/models/discord/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/models/discord/user.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/models/discord/voice_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12406 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/models/discord/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:25:05.190549 interactions.py-5.5.0/interactions/models/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/models/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11266 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/models/internal/active_voice_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:25:05.190549 interactions.py-5.5.0/interactions/models/internal/annotations/
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/models/internal/annotations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7405 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/models/internal/annotations/slash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55763 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/models/internal/application_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/models/internal/auto_defer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/models/internal/callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/models/internal/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12390 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/models/internal/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35980 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/models/internal/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19351 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/models/internal/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17655 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/models/internal/cooldowns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10168 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/models/internal/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/models/internal/listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/models/internal/localisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/models/internal/protocols.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:25:05.190549 interactions.py-5.5.0/interactions/models/internal/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/models/internal/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/models/internal/tasks/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/models/internal/tasks/triggers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/models/internal/wait.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:25:05.190549 interactions.py-5.5.0/interactions/models/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/models/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/models/misc/context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/models/misc/iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 18:24:28.000000 interactions.py-5.5.0/interactions/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:25:05.158549 interactions.py-5.5.0/interactions.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-05-21 18:25:05.000000 interactions.py-5.5.0/interactions.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-05-21 18:25:05.000000 interactions.py-5.5.0/interactions.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 18:25:05.000000 interactions.py-5.5.0/interactions.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-21 18:25:05.000000 interactions.py-5.5.0/interactions.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-21 18:25:05.000000 interactions.py-5.5.0/interactions.py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-05-21 18:24:28.000000 interactions.py-5.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-21 18:24:28.000000 interactions.py-5.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-21 18:25:05.190549 interactions.py-5.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-21 18:24:58.000000 interactions.py-5.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:25:05.190549 interactions.py-5.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 18:24:28.000000 interactions.py-5.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-05-21 18:24:28.000000 interactions.py-5.5.0/tests/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16999 2023-05-21 18:24:28.000000 interactions.py-5.5.0/tests/test_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-21 18:24:28.000000 interactions.py-5.5.0/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-21 18:24:28.000000 interactions.py-5.5.0/tests/test_contexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-21 18:24:28.000000 interactions.py-5.5.0/tests/test_cooldowns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-05-21 18:24:28.000000 interactions.py-5.5.0/tests/test_emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-21 18:24:28.000000 interactions.py-5.5.0/tests/utils.py
```

### Comparing `interactions.py-5.4.0/LICENSE` & `interactions.py-5.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/PKG-INFO` & `interactions.py-5.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interactions.py
-Version: 5.4.0
+Version: 5.5.0
 Summary: Easy, simple, scalable and modular: a Python API wrapper for interactions.
 Home-page: https://github.com/interactions-py/interactions.py
 Author: LordOfPolls
 Author-email: dev@lordofpolls.com
 Project-URL: Discord, https://discord.gg/KkgMBVuEkx
 Project-URL: Documentation, https://naff-docs.readthedocs.io/en/latest/
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `interactions.py-5.4.0/README.md` & `interactions.py-5.5.0/README.md`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/__init__.py` & `interactions.py-5.5.0/interactions/__init__.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/api/events/__init__.py` & `interactions.py-5.5.0/interactions/api/events/__init__.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/api/events/base.py` & `interactions.py-5.5.0/interactions/api/events/base.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/api/events/discord.py` & `interactions.py-5.5.0/interactions/api/events/discord.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/api/events/internal.py` & `interactions.py-5.5.0/interactions/api/events/internal.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/api/events/processors/__init__.py` & `interactions.py-5.5.0/interactions/api/events/processors/__init__.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/api/events/processors/_template.py` & `interactions.py-5.5.0/interactions/api/events/processors/_template.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/api/events/processors/auto_mod.py` & `interactions.py-5.5.0/interactions/api/events/processors/auto_mod.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/api/events/processors/channel_events.py` & `interactions.py-5.5.0/interactions/api/events/processors/channel_events.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/api/events/processors/guild_events.py` & `interactions.py-5.5.0/interactions/api/events/processors/guild_events.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/api/events/processors/integrations.py` & `interactions.py-5.5.0/interactions/api/events/processors/integrations.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/api/events/processors/member_events.py` & `interactions.py-5.5.0/interactions/api/events/processors/member_events.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/api/events/processors/message_events.py` & `interactions.py-5.5.0/interactions/api/events/processors/message_events.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/api/events/processors/reaction_events.py` & `interactions.py-5.5.0/interactions/api/events/processors/reaction_events.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/api/events/processors/role_events.py` & `interactions.py-5.5.0/interactions/api/events/processors/role_events.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/api/events/processors/stage_events.py` & `interactions.py-5.5.0/interactions/api/events/processors/stage_events.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/api/events/processors/thread_events.py` & `interactions.py-5.5.0/interactions/api/events/processors/thread_events.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/api/events/processors/user_events.py` & `interactions.py-5.5.0/interactions/api/events/processors/user_events.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/api/events/processors/voice_events.py` & `interactions.py-5.5.0/interactions/api/events/processors/voice_events.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/api/gateway/gateway.py` & `interactions.py-5.5.0/interactions/api/gateway/gateway.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/api/gateway/state.py` & `interactions.py-5.5.0/interactions/api/gateway/state.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/api/gateway/websocket.py` & `interactions.py-5.5.0/interactions/api/gateway/websocket.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/api/http/http_client.py` & `interactions.py-5.5.0/interactions/api/http/http_client.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/api/http/http_requests/__init__.py` & `interactions.py-5.5.0/interactions/api/http/http_requests/__init__.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/api/http/http_requests/bot.py` & `interactions.py-5.5.0/interactions/api/http/http_requests/bot.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/api/http/http_requests/channels.py` & `interactions.py-5.5.0/interactions/api/http/http_requests/channels.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/api/http/http_requests/emojis.py` & `interactions.py-5.5.0/interactions/api/http/http_requests/emojis.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/api/http/http_requests/guild.py` & `interactions.py-5.5.0/interactions/api/http/http_requests/guild.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/api/http/http_requests/interactions.py` & `interactions.py-5.5.0/interactions/api/http/http_requests/interactions.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/api/http/http_requests/members.py` & `interactions.py-5.5.0/interactions/api/http/http_requests/members.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/api/http/http_requests/messages.py` & `interactions.py-5.5.0/interactions/api/http/http_requests/messages.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/api/http/http_requests/reactions.py` & `interactions.py-5.5.0/interactions/api/http/http_requests/reactions.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/api/http/http_requests/scheduled_events.py` & `interactions.py-5.5.0/interactions/api/http/http_requests/scheduled_events.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/api/http/http_requests/stickers.py` & `interactions.py-5.5.0/interactions/api/http/http_requests/stickers.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/api/http/http_requests/threads.py` & `interactions.py-5.5.0/interactions/api/http/http_requests/threads.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/api/http/http_requests/users.py` & `interactions.py-5.5.0/interactions/api/http/http_requests/users.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/api/http/http_requests/webhooks.py` & `interactions.py-5.5.0/interactions/api/http/http_requests/webhooks.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/api/http/route.py` & `interactions.py-5.5.0/interactions/api/http/route.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/api/voice/audio.py` & `interactions.py-5.5.0/interactions/api/voice/audio.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/api/voice/audio_writer.py` & `interactions.py-5.5.0/interactions/api/voice/audio_writer.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/api/voice/encryption.py` & `interactions.py-5.5.0/interactions/api/voice/encryption.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/api/voice/opus.py` & `interactions.py-5.5.0/interactions/api/voice/opus.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/api/voice/player.py` & `interactions.py-5.5.0/interactions/api/voice/player.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/api/voice/recorder.py` & `interactions.py-5.5.0/interactions/api/voice/recorder.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/api/voice/voice_gateway.py` & `interactions.py-5.5.0/interactions/api/voice/voice_gateway.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/bin/opus-x64.dll` & `interactions.py-5.5.0/interactions/bin/opus-x64.dll`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/bin/opus-x86.dll` & `interactions.py-5.5.0/interactions/bin/opus-x86.dll`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/client/__init__.py` & `interactions.py-5.5.0/interactions/client/__init__.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/client/auto_shard_client.py` & `interactions.py-5.5.0/interactions/client/auto_shard_client.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/client/client.py` & `interactions.py-5.5.0/interactions/client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -540,14 +540,15 @@
 
     def get_guild_websocket(self, id: "Snowflake_Type") -> GatewayClient:
         return self.ws
 
     def _sanity_check(self) -> None:
         """Checks for possible and common errors in the bot's configuration."""
         self.logger.debug("Running client sanity checks...")
+
         contexts = {
             self.interaction_context: InteractionContext,
             self.component_context: ComponentContext,
             self.autocomplete_context: AutocompleteContext,
             self.modal_context: ModalContext,
         }
         for obj, expected in contexts.items():
@@ -907,14 +908,19 @@
         self.token = (token or self.token).strip()
 
         # i needed somewhere to put this call,
         # login will always run after initialisation
         # so im gathering commands here
         self._gather_callbacks()
 
+        if any(v for v in constants.CLIENT_FEATURE_FLAGS.values()):
+            # list all enabled flags
+            enabled_flags = [k for k, v in constants.CLIENT_FEATURE_FLAGS.items() if v]
+            self.logger.info(f"Enabled feature flags: {', '.join(enabled_flags)}")
+
         self.logger.debug("Attempting to login")
         me = await self.http.login(self.token)
         self._user = ClientUser.from_dict(me, self)
         self.cache.place_user_data(me)
         self._app = Application.from_dict(await self.http.get_current_bot_information(), self)
         self._mention_reg = re.compile(rf"^(<@!?{self.user.id}*>\s)")
 
@@ -1101,15 +1107,15 @@
             Union[
                 List[List[Union["BaseComponent", dict]]],
                 List[Union["BaseComponent", dict]],
                 "BaseComponent",
                 dict,
             ]
         ] = None,
-        check: Optional[Callable] = None,
+        check: Absent[Optional[Union[Callable[..., bool], Callable[..., Awaitable[bool]]]]] = None,
         timeout: Optional[float] = None,
     ) -> "events.Component":
         """
         Waits for a component to be sent to the bot.
 
         Args:
             messages: The message object to check for.
@@ -1132,30 +1138,34 @@
         )
         custom_ids = list(get_components_ids(components)) if components else None
 
         # automatically convert improper custom_ids
         if custom_ids and not all(isinstance(x, str) for x in custom_ids):
             custom_ids = [str(i) for i in custom_ids]
 
-        def _check(event: events.Component) -> bool:
+        async def _check(event: events.Component) -> bool:
             ctx: ComponentContext = event.ctx
             # if custom_ids is empty or there is a match
             wanted_message = not message_ids or ctx.message.id in (
                 [message_ids] if isinstance(message_ids, int) else message_ids
             )
             wanted_component = not custom_ids or ctx.custom_id in custom_ids
             if wanted_message and wanted_component:
+                if asyncio.iscoroutinefunction(check):
+                    return bool(check is None or await check(event))
                 return bool(check is None or check(event))
             return False
 
         return await self.wait_for("component", checks=_check, timeout=timeout)
 
     def command(self, *args, **kwargs) -> Callable:
         """A decorator that registers a command. Aliases `interactions.slash_command`"""
-        raise NotImplementedError  # TODO: implement
+        raise NotImplementedError(
+            "Use interactions.slash_command instead. Please consult the v4 -> v5 migration guide https://interactions-py.github.io/interactions.py/Guides/98%20Migration%20from%204.X/"
+        )
 
     def listen(self, event_name: Absent[str] = MISSING) -> Callable[[AsyncCallable], Listener]:
         """
         A decorator to be used in situations that the library can't automatically hook your listeners. Ideally, the standard listen decorator should be used, not this.
 
         Args:
             event_name: The event name to use, if not the coroutine name
```

### Comparing `interactions.py-5.4.0/interactions/client/const.py` & `interactions.py-5.5.0/interactions/client/const.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,14 +28,17 @@
     GLOBAL_SCOPE _sentinel: A sentinel that represents a global scope for application commands.
     MENTION_PREFIX _sentinel: A sentinel representing the bot will be mentioned for a prefix
     MISSING _sentinel: A sentinel value that indicates something has not been set
 
     T TypeVar: A type variable used for generic typing.
     Absent Union[T, Missing]: A type hint for a value that may be MISSING.
 
+    CLIENT_FEATURE_FLAGS dict: A dict of feature flags that can be enabled or disabled for the client.
+    has_feature_flag Callable[[str], bool]: A function that returns whether a feature flag is enabled.
+
 """
 import inspect
 import logging
 import os
 import sys
 from collections import defaultdict
 from importlib.metadata import version as _v, PackageNotFoundError
@@ -74,14 +77,16 @@
     "PREMIUM_GUILD_LIMITS",
     "Absent",
     "T",
     "T_co",
     "LIB_PATH",
     "RECOVERABLE_WEBSOCKET_CLOSE_CODES",
     "NON_RESUMABLE_WEBSOCKET_CLOSE_CODES",
+    "CLIENT_FEATURE_FLAGS",
+    "has_client_feature",
 )
 
 _ver_info = sys.version_info
 
 repo_names = ("interactions.py", "discord-py-interactions")
 for repo_name in repo_names:
     try:
@@ -191,14 +196,26 @@
     {
         1: {"emoji": 100, "stickers": 15, "bitrate": 128000, "filesize": 26214400},
         2: {"emoji": 150, "stickers": 30, "bitrate": 256000, "filesize": 52428800},
         3: {"emoji": 250, "stickers": 60, "bitrate": 384000, "filesize": 104857600},
     },
 )
 
+CLIENT_FEATURE_FLAGS = {
+    "FOLLOWUP_INTERACTIONS_FOR_IMAGES": False,  # Experimental fix to bypass Discord's broken image proxy
+}
+
+
+def has_client_feature(feature: str) -> bool:
+    """Checks if a feature is enabled for the client."""
+    if feature.upper() not in CLIENT_FEATURE_FLAGS:
+        get_logger().warning(f"Unknown feature {feature!r} - Known features: {list(CLIENT_FEATURE_FLAGS)}")
+        return False
+    return CLIENT_FEATURE_FLAGS[feature.upper()]
+
 
 GUILD_WELCOME_MESSAGES = (
     "{0} joined the party.",
     "{0} is here.",
     "Welcome, {0}. We hope you brought pizza.",
     "A wild {0} appeared.",
     "{0} just landed.",
```

### Comparing `interactions.py-5.4.0/interactions/client/errors.py` & `interactions.py-5.5.0/interactions/client/errors.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/client/mixins/modal.py` & `interactions.py-5.5.0/interactions/client/mixins/modal.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/client/mixins/send.py` & `interactions.py-5.5.0/interactions/client/mixins/send.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/client/mixins/serialization.py` & `interactions.py-5.5.0/interactions/client/mixins/serialization.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/client/smart_cache.py` & `interactions.py-5.5.0/interactions/client/smart_cache.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/client/utils/__init__.py` & `interactions.py-5.5.0/interactions/client/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/client/utils/attr_converters.py` & `interactions.py-5.5.0/interactions/client/utils/attr_converters.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/client/utils/attr_utils.py` & `interactions.py-5.5.0/interactions/client/utils/attr_utils.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/client/utils/attr_utils.pyi` & `interactions.py-5.5.0/interactions/client/utils/attr_utils.pyi`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/client/utils/cache.py` & `interactions.py-5.5.0/interactions/client/utils/cache.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/client/utils/deserialise_app_cmds.py` & `interactions.py-5.5.0/interactions/client/utils/deserialise_app_cmds.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/client/utils/formatting.py` & `interactions.py-5.5.0/interactions/client/utils/formatting.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/client/utils/input_utils.py` & `interactions.py-5.5.0/interactions/client/utils/input_utils.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/client/utils/misc_utils.py` & `interactions.py-5.5.0/interactions/client/utils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/client/utils/serializer.py` & `interactions.py-5.5.0/interactions/client/utils/serializer.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/client/utils/text_utils.py` & `interactions.py-5.5.0/interactions/client/utils/text_utils.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/ext/console.py` & `interactions.py-5.5.0/interactions/ext/console.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/ext/debug_extension/__init__.py` & `interactions.py-5.5.0/interactions/ext/debug_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/ext/debug_extension/debug_application_cmd.py` & `interactions.py-5.5.0/interactions/ext/debug_extension/debug_application_cmd.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/ext/debug_extension/debug_exec.py` & `interactions.py-5.5.0/interactions/ext/debug_extension/debug_exec.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/ext/debug_extension/debug_exts.py` & `interactions.py-5.5.0/interactions/ext/debug_extension/debug_exts.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/ext/debug_extension/utils.py` & `interactions.py-5.5.0/interactions/ext/debug_extension/utils.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/ext/jurigged.py` & `interactions.py-5.5.0/interactions/ext/jurigged.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/ext/mypy/__init__.py` & `interactions.py-5.5.0/interactions/ext/mypy/__init__.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/ext/paginators.py` & `interactions.py-5.5.0/interactions/ext/paginators.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/ext/prefixed_commands/__init__.py` & `interactions.py-5.5.0/interactions/ext/prefixed_commands/__init__.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/ext/prefixed_commands/command.py` & `interactions.py-5.5.0/interactions/ext/prefixed_commands/command.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/ext/prefixed_commands/context.py` & `interactions.py-5.5.0/interactions/ext/prefixed_commands/context.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/ext/prefixed_commands/help.py` & `interactions.py-5.5.0/interactions/ext/prefixed_commands/help.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/ext/prefixed_commands/manager.py` & `interactions.py-5.5.0/interactions/ext/prefixed_commands/manager.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/ext/prefixed_commands/utils.py` & `interactions.py-5.5.0/interactions/ext/prefixed_commands/utils.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/ext/sentry.py` & `interactions.py-5.5.0/interactions/ext/sentry.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/models/__init__.py` & `interactions.py-5.5.0/interactions/models/__init__.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/models/discord/__init__.py` & `interactions.py-5.5.0/interactions/models/discord/__init__.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/models/discord/activity.py` & `interactions.py-5.5.0/interactions/models/discord/activity.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/models/discord/app_perms.py` & `interactions.py-5.5.0/interactions/models/discord/app_perms.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/models/discord/application.py` & `interactions.py-5.5.0/interactions/models/discord/application.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/models/discord/asset.py` & `interactions.py-5.5.0/interactions/models/discord/asset.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/models/discord/auto_mod.py` & `interactions.py-5.5.0/interactions/models/discord/auto_mod.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/models/discord/base.py` & `interactions.py-5.5.0/interactions/models/discord/base.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/models/discord/channel.py` & `interactions.py-5.5.0/interactions/models/discord/channel.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/models/discord/color.py` & `interactions.py-5.5.0/interactions/models/discord/color.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/models/discord/components.py` & `interactions.py-5.5.0/interactions/models/discord/components.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/models/discord/embed.py` & `interactions.py-5.5.0/interactions/models/discord/embed.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/models/discord/emoji.py` & `interactions.py-5.5.0/interactions/models/discord/emoji.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/models/discord/enums.py` & `interactions.py-5.5.0/interactions/models/discord/enums.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/models/discord/file.py` & `interactions.py-5.5.0/interactions/models/discord/file.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/models/discord/guild.py` & `interactions.py-5.5.0/interactions/models/discord/guild.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/models/discord/invite.py` & `interactions.py-5.5.0/interactions/models/discord/invite.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/models/discord/message.py` & `interactions.py-5.5.0/interactions/models/discord/message.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/models/discord/modal.py` & `interactions.py-5.5.0/interactions/models/discord/modal.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/models/discord/reaction.py` & `interactions.py-5.5.0/interactions/models/discord/reaction.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/models/discord/role.py` & `interactions.py-5.5.0/interactions/models/discord/role.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/models/discord/scheduled_event.py` & `interactions.py-5.5.0/interactions/models/discord/scheduled_event.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/models/discord/snowflake.py` & `interactions.py-5.5.0/interactions/models/discord/snowflake.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/models/discord/stage_instance.py` & `interactions.py-5.5.0/interactions/models/discord/stage_instance.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/models/discord/sticker.py` & `interactions.py-5.5.0/interactions/models/discord/sticker.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/models/discord/team.py` & `interactions.py-5.5.0/interactions/models/discord/team.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/models/discord/thread.py` & `interactions.py-5.5.0/interactions/models/discord/thread.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/models/discord/timestamp.py` & `interactions.py-5.5.0/interactions/models/discord/timestamp.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/models/discord/user.py` & `interactions.py-5.5.0/interactions/models/discord/user.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/models/discord/user.pyi` & `interactions.py-5.5.0/interactions/models/discord/user.pyi`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/models/discord/voice_state.py` & `interactions.py-5.5.0/interactions/models/discord/voice_state.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/models/discord/webhooks.py` & `interactions.py-5.5.0/interactions/models/discord/webhooks.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/models/internal/__init__.py` & `interactions.py-5.5.0/interactions/models/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/models/internal/active_voice_state.py` & `interactions.py-5.5.0/interactions/models/internal/active_voice_state.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/models/internal/annotations/slash.py` & `interactions.py-5.5.0/interactions/models/internal/annotations/slash.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/models/internal/application_commands.py` & `interactions.py-5.5.0/interactions/models/internal/application_commands.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/models/internal/auto_defer.py` & `interactions.py-5.5.0/interactions/models/internal/auto_defer.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/models/internal/callback.py` & `interactions.py-5.5.0/interactions/models/internal/callback.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/models/internal/checks.py` & `interactions.py-5.5.0/interactions/models/internal/checks.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/models/internal/command.py` & `interactions.py-5.5.0/interactions/models/internal/command.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/models/internal/context.py` & `interactions.py-5.5.0/interactions/models/internal/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import datetime
 import re
 import typing
 from typing_extensions import Self
 
 import discord_typings
 from aiohttp import FormData
+
+from interactions.client import const
 from interactions.client.const import get_logger, MISSING
 from interactions.models.discord.components import BaseComponent
 from interactions.models.discord.file import UPLOADABLE_TYPE
 from interactions.models.discord.sticker import Sticker
 from interactions.models.discord.user import Member, User
 
 from interactions.models.internal.command import BaseCommand
@@ -397,25 +399,38 @@
         await self.client.http.post_initial_response(payload, self.id, self.token)
         self.deferred = True
         self.ephemeral = ephemeral
 
     async def _send_http_request(
         self, message_payload: dict, files: typing.Iterable["UPLOADABLE_TYPE"] | None = None
     ) -> dict:
+        if const.has_client_feature("FOLLOWUP_INTERACTIONS_FOR_IMAGES") and not self.deferred:
+            # experimental bypass for discords broken image proxy
+            if embeds := message_payload.get("embeds", {}):
+                if any(e.get("image") for e in embeds) or any(e.get("thumbnail") for e in embeds):
+                    if MessageFlags.EPHEMERAL in message_payload.get("flags", MessageFlags.NONE):
+                        self.ephemeral = True
+                    await self.defer(ephemeral=self.ephemeral)
+
         if self.responded:
             message_data = await self.client.http.post_followup(
                 message_payload, self.client.app.id, self.token, files=files
             )
         else:
             if isinstance(message_payload, FormData) and not self.deferred:
                 await self.defer(ephemeral=self.ephemeral)
             if self.deferred:
-                message_data = await self.client.http.edit_interaction_message(
-                    message_payload, self.client.app.id, self.token, files=files
-                )
+                if const.has_client_feature("FOLLOWUP_INTERACTIONS_FOR_IMAGES"):
+                    message_data = await self.client.http.post_followup(
+                        message_payload, self.client.app.id, self.token, files=files
+                    )
+                else:
+                    message_data = await self.client.http.edit_interaction_message(
+                        message_payload, self.client.app.id, self.token, files=files
+                    )
             else:
                 payload = {
                     "type": CallbackType.CHANNEL_MESSAGE_WITH_SOURCE,
                     "data": message_payload,
                 }
                 message_data = await self.client.http.post_initial_response(payload, self.id, self.token, files=files)
```

### Comparing `interactions.py-5.4.0/interactions/models/internal/converters.py` & `interactions.py-5.5.0/interactions/models/internal/converters.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/models/internal/cooldowns.py` & `interactions.py-5.5.0/interactions/models/internal/cooldowns.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/models/internal/extension.py` & `interactions.py-5.5.0/interactions/models/internal/extension.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/models/internal/listener.py` & `interactions.py-5.5.0/interactions/models/internal/listener.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/models/internal/localisation.py` & `interactions.py-5.5.0/interactions/models/internal/localisation.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/models/internal/protocols.py` & `interactions.py-5.5.0/interactions/models/internal/protocols.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/models/internal/tasks/task.py` & `interactions.py-5.5.0/interactions/models/internal/tasks/task.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/models/internal/tasks/triggers.py` & `interactions.py-5.5.0/interactions/models/internal/tasks/triggers.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/models/internal/wait.py` & `interactions.py-5.5.0/interactions/models/internal/wait.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/models/misc/context_manager.py` & `interactions.py-5.5.0/interactions/models/misc/context_manager.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions/models/misc/iterator.py` & `interactions.py-5.5.0/interactions/models/misc/iterator.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions.py.egg-info/PKG-INFO` & `interactions.py-5.5.0/interactions.py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interactions.py
-Version: 5.4.0
+Version: 5.5.0
 Summary: Easy, simple, scalable and modular: a Python API wrapper for interactions.
 Home-page: https://github.com/interactions-py/interactions.py
 Author: LordOfPolls
 Author-email: dev@lordofpolls.com
 Project-URL: Discord, https://discord.gg/KkgMBVuEkx
 Project-URL: Documentation, https://naff-docs.readthedocs.io/en/latest/
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `interactions.py-5.4.0/interactions.py.egg-info/SOURCES.txt` & `interactions.py-5.5.0/interactions.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/interactions.py.egg-info/requires.txt` & `interactions.py-5.5.0/interactions.py.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/pyproject.toml` & `interactions.py-5.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "interactions.py"
-version = "5.4.0"
+version = "5.5.0"
 description = "Easy, simple, scalable and modular: a Python API wrapper for interactions."
 authors = [
     "LordOfPolls <dev@lordofpolls.com>",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
```

### Comparing `interactions.py-5.4.0/setup.py` & `interactions.py-5.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/tests/consts.py` & `interactions.py-5.5.0/tests/consts.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/tests/test_bot.py` & `interactions.py-5.5.0/tests/test_bot.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/tests/test_cache.py` & `interactions.py-5.5.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/tests/test_contexts.py` & `interactions.py-5.5.0/tests/test_contexts.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/tests/test_cooldowns.py` & `interactions.py-5.5.0/tests/test_cooldowns.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/tests/test_emoji.py` & `interactions.py-5.5.0/tests/test_emoji.py`

 * *Files identical despite different names*

### Comparing `interactions.py-5.4.0/tests/utils.py` & `interactions.py-5.5.0/tests/utils.py`

 * *Files identical despite different names*

